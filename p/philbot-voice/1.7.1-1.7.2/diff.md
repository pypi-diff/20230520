# Comparing `tmp/philbot_voice-1.7.1.tar.gz` & `tmp/philbot_voice-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "philbot_voice-1.7.1.tar", max compression
+gzip compressed data, was "philbot_voice-1.7.2.tar", max compression
```

## Comparing `philbot_voice-1.7.1.tar` & `philbot_voice-1.7.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       19 2023-05-12 13:27:54.459877 philbot_voice-1.7.1/philbot-voice/__init__.py
--rw-r--r--   0        0        0       26 2023-05-12 13:27:54.459877 philbot_voice-1.7.1/philbot-voice/__main__.py
--rw-r--r--   0        0        0    33783 2023-05-12 13:27:54.459877 philbot_voice-1.7.1/philbot-voice/voice.py
--rw-r--r--   0        0        0      625 2023-05-12 13:27:54.459877 philbot_voice-1.7.1/pyproject.toml
--rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 philbot_voice-1.7.1/PKG-INFO
+-rw-r--r--   0        0        0       19 2023-05-19 22:15:23.470142 philbot_voice-1.7.2/philbot-voice/__init__.py
+-rw-r--r--   0        0        0       26 2023-05-19 22:15:23.470142 philbot_voice-1.7.2/philbot-voice/__main__.py
+-rw-r--r--   0        0        0    33127 2023-05-19 22:15:23.470142 philbot_voice-1.7.2/philbot-voice/voice.py
+-rw-r--r--   0        0        0      625 2023-05-19 22:15:23.470142 philbot_voice-1.7.2/pyproject.toml
+-rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 philbot_voice-1.7.2/PKG-INFO
```

### Comparing `philbot_voice-1.7.1/philbot-voice/voice.py` & `philbot_voice-1.7.2/philbot-voice/voice.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,17 @@
 import requests
 import subprocess
 import websocket
 from flask import Flask, request, Response
 import yt_dlp
 import opentelemetry
 from opentelemetry.sdk.resources import Resource
+from opentelemetry import metrics
 from opentelemetry.sdk.metrics import MeterProvider
-from opentelemetry.sdk.metrics.export import PeriodicExportingMetricReader, AggregationTemporality
+from opentelemetry.sdk.metrics.export import PeriodicExportingMetricReader
 from opentelemetry.exporter.otlp.proto.http.metric_exporter import OTLPMetricExporter
 from opentelemetry.sdk.trace import TracerProvider, sampling
 from opentelemetry.sdk.trace.export import BatchSpanProcessor
 from opentelemetry.exporter.otlp.proto.http.trace_exporter import OTLPSpanExporter
 
 merged = dict()
 for name in ["dt_metadata_e617c525669e072eebe3d0f08212e8f2.json", "/var/lib/dynatrace/enrichment/dt_metadata.json"]:
@@ -151,16 +152,14 @@
         file.close()
         os.remove(filename)
         raise RuntimeError('unexpected sample width: ' + str(file.getsampwidth()))
     file.close()
     os.utime(filename)
     return 'file://' + filename
 
-counter_concurrent_connections = meter.create_up_down_counter(name = 'discord.gateway.voice.connections.concurrent', description = 'Number concurrent open connections', unit="count")
-counter_concurrent_streams = meter.create_up_down_counter(name = 'discord.gateway.voice.streams.concurrent', description = 'Number of concurrent streams', unit="count")
 counter_streams = meter.create_counter(name = 'discord.gateway.voice.streams', description = 'Number of streams', unit="count")
 counter_streaming = meter.create_counter(name = 'discord.gateway.voice.streaming', description = 'Amount of time streamed', unit="milliseconds")
 
 class Context:
     lock = threading.Lock()
     callback_url = None
     guild_id = None
@@ -298,15 +297,14 @@
                     file.close()
                     try:
                         os.remove(filename)
                     except:
                         pass
                     file = None
                     filename = None
-                    counter_concurrent_streams.add(-1, { "guild_id": self.guild_id })
                     print('VOICE CONNECTION ' + self.guild_id + ' stream completed')
                     threading.Thread(target=self.__callback_playback_finished).start()
                 elif not filename and self.url:
                     filename = self.url[len('file://'):]
                     if not os.path.exists(filename):
                         print('VOICE CONNECTION ' + self.guild_id + ' skipping source because local file is not available')
                         filename = None
@@ -323,15 +321,14 @@
                             except:
                                 pass
                             filename = None
                             self.url = None
                             threading.Thread(target=self.__callback_playback_finished).start()
                         else:
                             print('VOICE CONNECTION ' + self.guild_id + ' streaming ' + filename + ' (' + str(file.getnframes() / file.getframerate() / 60) + 'mins)')
-                            counter_concurrent_streams.add(1, { "guild_id": self.guild_id })
                             counter_streams.add(1, { "guild_id": self.guild_id })
                 elif filename and self.url and filename != self.url[len('file://'):]:
                     file.close()
                     try:
                         os.remove(filename)
                     except:
                         pass
@@ -390,22 +387,20 @@
 
         if filename:
             file.close()
             try:
                 os.remove(filename)
             except:
                 pass
-            counter_concurrent_streams.add(-1, { "guild_id": self.guild_id })
         pyogg.opus.opus_encoder_destroy(encoder)
         
         print('VOICE CONNECTION ' + self.guild_id + ' stream closed')
 
     def __ws_on_open(self, ws):
         print('VOICE GATEWAY ' + self.guild_id + ' connection established')
-        counter_concurrent_connections.add(1, { "guild_id": self.guild_id, "server": self.endpoint if self.endpoint else "" })
 
     def __ws_on_message(self, ws, message):
         with self.lock:
             payload = json.loads(message)
             if payload['op'] != 6: 
                 print('VOICE GATEWAY ' + self.guild_id + ' received message: ' + str(payload['op'])) # heartbeat acks are very spammy
             match payload['op']:
@@ -551,15 +546,14 @@
                 pass
             case 4016: # unknown encryption mode
                 # fault must be in the code somewhere
                 # lets wait a bit to avoid busy loops and try again
                 time.sleep(5)
             case _: # something else
                 pass
-        counter_concurrent_connections.add(-1, { "guild_id": self.guild_id, "server": self.endpoint if self.endpoint else "", "close_code": close_code if close_code else 0 })
         self.__stop()
     
     def __try_start(self):
         with self.lock:
             if self.ws or not self.channel_id or not self.session_id or not self.endpoint or not self.token or not self.url:
                 return
             print('VOICE GATEWAY ' + self.guild_id + ' connection starting')
@@ -643,14 +637,24 @@
 def get_context(guild_id):
     with contexts_lock:
         context = contexts.get(guild_id)
         if not context:
             context = contexts[guild_id] = Context(guild_id)
         return context
 
+def get_connection_count(options):
+    count = 0
+    with contexts_lock:
+        for context in contexts.values():
+            if context.is_connected():
+                count = count + 1
+    yield metrics.Observation(count)
+
+meter.create_observable_gauge('discord.gateway.voice.connections.concurrent', [get_connection_count])
+
 @app.route('/ping', methods=['GET'])
 def ping():
     return 'pong'
 
 @app.route('/voice_state_update', methods=['POST'])
 def voice_state_update():
     if not request.headers.get('x-authorization'): return Response('Unauthorized', status=401)
@@ -742,8 +746,7 @@
             get_context(file[len('.state.'):len(file) - len('.json')])
         elif (file.endswith('.wav') or file.endswith('.aac') or file.endswith('.part')) and os.path.getmtime(file) + 60 * 60 * 24 < time_seconds():
             os.remove(file)
     print('VOICE ready')
     # app.run(port=HTTP_PORT, ssl_context='adhoc', threaded=True)
     app.run(port=HTTP_PORT, threaded=True)
 
-# https://github.com/ytdl-org/youtube-dl/blob/master/README.md#embedding-youtube-dl
```

### Comparing `philbot_voice-1.7.1/pyproject.toml` & `philbot_voice-1.7.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "philbot-voice"
-version = "1.7.1"
+version = "1.7.2"
 description = ""
 authors = ["philipp.lengauer <p.lengauer@gmail.com>"]
 packages = [{include = "philbot-voice"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 Flask = "^2.2.2"
```

### Comparing `philbot_voice-1.7.1/PKG-INFO` & `philbot_voice-1.7.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: philbot-voice
-Version: 1.7.1
+Version: 1.7.2
 Summary: 
 Author: philipp.lengauer
 Author-email: p.lengauer@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

