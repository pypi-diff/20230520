# Comparing `tmp/mqttasgi-1.2.1.tar.gz` & `tmp/mqttasgi-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mqttasgi-1.2.1.tar", last modified: Sat Oct 15 10:30:54 2022, max compression
+gzip compressed data, was "mqttasgi-1.2.2.tar", last modified: Sat May 20 11:07:36 2023, max compression
```

## Comparing `mqttasgi-1.2.1.tar` & `mqttasgi-1.2.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 sivulich   (501) staff       (20)        0 2022-10-15 10:30:54.535473 mqttasgi-1.2.1/
--rw-r--r--   0 sivulich   (501) staff       (20)     1073 2021-12-26 14:23:26.000000 mqttasgi-1.2.1/LICENSE
--rw-r--r--   0 sivulich   (501) staff       (20)     6944 2022-10-15 10:30:54.535304 mqttasgi-1.2.1/PKG-INFO
--rw-r--r--   0 sivulich   (501) staff       (20)     5892 2022-08-29 22:02:19.000000 mqttasgi-1.2.1/README.md
-drwxr-xr-x   0 sivulich   (501) staff       (20)        0 2022-10-15 10:30:54.533892 mqttasgi-1.2.1/mqttasgi/
--rw-r--r--   0 sivulich   (501) staff       (20)       22 2022-10-15 10:28:39.000000 mqttasgi-1.2.1/mqttasgi/__init__.py
--rw-r--r--   0 sivulich   (501) staff       (20)     2670 2022-08-29 21:55:44.000000 mqttasgi-1.2.1/mqttasgi/cli.py
--rw-r--r--   0 sivulich   (501) staff       (20)     3622 2022-07-29 22:42:10.000000 mqttasgi-1.2.1/mqttasgi/consumers.py
--rw-r--r--   0 sivulich   (501) staff       (20)    18081 2022-10-15 10:27:37.000000 mqttasgi-1.2.1/mqttasgi/server.py
--rw-r--r--   0 sivulich   (501) staff       (20)     1695 2021-06-04 18:10:17.000000 mqttasgi-1.2.1/mqttasgi/testing.py
--rw-r--r--   0 sivulich   (501) staff       (20)      402 2022-08-29 21:55:32.000000 mqttasgi-1.2.1/mqttasgi/utils.py
-drwxr-xr-x   0 sivulich   (501) staff       (20)        0 2022-10-15 10:30:54.535082 mqttasgi-1.2.1/mqttasgi.egg-info/
--rw-r--r--   0 sivulich   (501) staff       (20)     6944 2022-10-15 10:30:54.000000 mqttasgi-1.2.1/mqttasgi.egg-info/PKG-INFO
--rw-r--r--   0 sivulich   (501) staff       (20)      336 2022-10-15 10:30:54.000000 mqttasgi-1.2.1/mqttasgi.egg-info/SOURCES.txt
--rw-r--r--   0 sivulich   (501) staff       (20)        1 2022-10-15 10:30:54.000000 mqttasgi-1.2.1/mqttasgi.egg-info/dependency_links.txt
--rw-r--r--   0 sivulich   (501) staff       (20)       48 2022-10-15 10:30:54.000000 mqttasgi-1.2.1/mqttasgi.egg-info/entry_points.txt
--rw-r--r--   0 sivulich   (501) staff       (20)       40 2022-10-15 10:30:54.000000 mqttasgi-1.2.1/mqttasgi.egg-info/requires.txt
--rw-r--r--   0 sivulich   (501) staff       (20)        9 2022-10-15 10:30:54.000000 mqttasgi-1.2.1/mqttasgi.egg-info/top_level.txt
--rw-r--r--   0 sivulich   (501) staff       (20)       38 2022-10-15 10:30:54.535544 mqttasgi-1.2.1/setup.cfg
--rw-r--r--   0 sivulich   (501) staff       (20)     1664 2022-08-29 21:56:42.000000 mqttasgi-1.2.1/setup.py
+drwxr-xr-x   0 sivulich   (501) staff       (20)        0 2023-05-20 11:07:36.853866 mqttasgi-1.2.2/
+-rw-r--r--   0 sivulich   (501) staff       (20)     1073 2021-12-26 14:23:26.000000 mqttasgi-1.2.2/LICENSE
+-rw-r--r--   0 sivulich   (501) staff       (20)     7094 2023-05-20 11:07:36.853757 mqttasgi-1.2.2/PKG-INFO
+-rw-r--r--   0 sivulich   (501) staff       (20)     6042 2023-05-20 11:05:45.000000 mqttasgi-1.2.2/README.md
+drwxr-xr-x   0 sivulich   (501) staff       (20)        0 2023-05-20 11:07:36.852645 mqttasgi-1.2.2/mqttasgi/
+-rw-r--r--   0 sivulich   (501) staff       (20)       22 2023-05-20 09:42:43.000000 mqttasgi-1.2.2/mqttasgi/__init__.py
+-rw-r--r--   0 sivulich   (501) staff       (20)     2935 2023-05-20 09:42:11.000000 mqttasgi-1.2.2/mqttasgi/cli.py
+-rw-r--r--   0 sivulich   (501) staff       (20)     3622 2022-07-29 22:42:10.000000 mqttasgi-1.2.2/mqttasgi/consumers.py
+-rw-r--r--   0 sivulich   (501) staff       (20)    18315 2023-05-20 11:01:15.000000 mqttasgi-1.2.2/mqttasgi/server.py
+-rw-r--r--   0 sivulich   (501) staff       (20)     1695 2021-06-04 18:10:17.000000 mqttasgi-1.2.2/mqttasgi/testing.py
+-rw-r--r--   0 sivulich   (501) staff       (20)      402 2022-08-29 21:55:32.000000 mqttasgi-1.2.2/mqttasgi/utils.py
+drwxr-xr-x   0 sivulich   (501) staff       (20)        0 2023-05-20 11:07:36.853595 mqttasgi-1.2.2/mqttasgi.egg-info/
+-rw-r--r--   0 sivulich   (501) staff       (20)     7094 2023-05-20 11:07:36.000000 mqttasgi-1.2.2/mqttasgi.egg-info/PKG-INFO
+-rw-r--r--   0 sivulich   (501) staff       (20)      336 2023-05-20 11:07:36.000000 mqttasgi-1.2.2/mqttasgi.egg-info/SOURCES.txt
+-rw-r--r--   0 sivulich   (501) staff       (20)        1 2023-05-20 11:07:36.000000 mqttasgi-1.2.2/mqttasgi.egg-info/dependency_links.txt
+-rw-r--r--   0 sivulich   (501) staff       (20)       48 2023-05-20 11:07:36.000000 mqttasgi-1.2.2/mqttasgi.egg-info/entry_points.txt
+-rw-r--r--   0 sivulich   (501) staff       (20)       40 2023-05-20 11:07:36.000000 mqttasgi-1.2.2/mqttasgi.egg-info/requires.txt
+-rw-r--r--   0 sivulich   (501) staff       (20)        9 2023-05-20 11:07:36.000000 mqttasgi-1.2.2/mqttasgi.egg-info/top_level.txt
+-rw-r--r--   0 sivulich   (501) staff       (20)       38 2023-05-20 11:07:36.853907 mqttasgi-1.2.2/setup.cfg
+-rw-r--r--   0 sivulich   (501) staff       (20)     1664 2022-08-29 21:56:42.000000 mqttasgi-1.2.2/setup.py
```

### Comparing `mqttasgi-1.2.1/LICENSE` & `mqttasgi-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mqttasgi-1.2.1/PKG-INFO` & `mqttasgi-1.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mqttasgi
-Version: 1.2.1
+Version: 1.2.2
 Summary: MQTT ASGI Protocol Server
 Home-page: https://github.com/sivulich/mqttasgi
 Author: Santiago Ivulich
 Author-email: sivulich@itba.edu.ar
 License: MIT
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
@@ -48,27 +48,28 @@
 # Usage
 ## Unit
 Mqttasgi provides a cli interface to run the protocol server. 
 ```bash
 mqttasgi -H localhost -p 1883 my_application.asgi:application
 ```
 Parameters:
-| Parameter   | Explanation      | Environment variable |
-|-------------|------------------|:--------------------:|
-| -H / --host | MQTT broker host | MQTT_HOSTNAME |
-| -p / --port | MQTT broker port | MQTT_PORT |
-| -c / --cleansession | MQTT Clean Session | MQTT_CLEAN |
-| -v / --verbosity | Logging verbosity | VERBOSITY |
-| -U / --username | MQTT Username | MQTT_USERNAME |
-| -P / --password | MQTT Password | MQTT_PASSWORD |
-| -i / --id | MQTT Client ID | MQTT_CLIENT_ID |
-| -C / --cert | TLS Certificate | TLS_CERT |
-| -K / --key | TLS Key | TLS_KEY |
-| -S / --cacert | TLS CA Certificate | TLS_CA |
-| Last argument | ASGI Apllication |  |
+| Parameter   | Explanation      | Environment variable | Default |
+|-------------|------------------|:--------------------:|:--------------------:|
+| -H / --host | MQTT broker host | MQTT_HOSTNAME | localhost |
+| -p / --port | MQTT broker port | MQTT_PORT | 1883 |
+| -c / --cleansession | MQTT Clean Session | MQTT_CLEAN | True |
+| -v / --verbosity | Logging verbosity | VERBOSITY | 0 |
+| -U / --username | MQTT Username | MQTT_USERNAME |  |
+| -P / --password | MQTT Password | MQTT_PASSWORD |  |
+| -i / --id | MQTT Client ID | MQTT_CLIENT_ID |  |
+| -C / --cert | TLS Certificate | TLS_CERT |  |
+| -K / --key | TLS Key | TLS_KEY |  |
+| -S / --cacert | TLS CA Certificate | TLS_CA |  |
+| -r / --retries | Num. retries on disconnect | MQTT_RETRIES | 3 |
+| Last argument | ASGI Apllication |  | |
 
 Environment variables are supported and can be set using a `.env` file on the root of the project, but passing a parameter overrides this value.
 
 ## Consumer
 
 To add your consumer to the `asgi.py` file in your django application:
 ```python
```

### Comparing `mqttasgi-1.2.1/README.md` & `mqttasgi-1.2.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -21,27 +21,28 @@
 # Usage
 ## Unit
 Mqttasgi provides a cli interface to run the protocol server. 
 ```bash
 mqttasgi -H localhost -p 1883 my_application.asgi:application
 ```
 Parameters:
-| Parameter   | Explanation      | Environment variable |
-|-------------|------------------|:--------------------:|
-| -H / --host | MQTT broker host | MQTT_HOSTNAME |
-| -p / --port | MQTT broker port | MQTT_PORT |
-| -c / --cleansession | MQTT Clean Session | MQTT_CLEAN |
-| -v / --verbosity | Logging verbosity | VERBOSITY |
-| -U / --username | MQTT Username | MQTT_USERNAME |
-| -P / --password | MQTT Password | MQTT_PASSWORD |
-| -i / --id | MQTT Client ID | MQTT_CLIENT_ID |
-| -C / --cert | TLS Certificate | TLS_CERT |
-| -K / --key | TLS Key | TLS_KEY |
-| -S / --cacert | TLS CA Certificate | TLS_CA |
-| Last argument | ASGI Apllication |  |
+| Parameter   | Explanation      | Environment variable | Default |
+|-------------|------------------|:--------------------:|:--------------------:|
+| -H / --host | MQTT broker host | MQTT_HOSTNAME | localhost |
+| -p / --port | MQTT broker port | MQTT_PORT | 1883 |
+| -c / --cleansession | MQTT Clean Session | MQTT_CLEAN | True |
+| -v / --verbosity | Logging verbosity | VERBOSITY | 0 |
+| -U / --username | MQTT Username | MQTT_USERNAME |  |
+| -P / --password | MQTT Password | MQTT_PASSWORD |  |
+| -i / --id | MQTT Client ID | MQTT_CLIENT_ID |  |
+| -C / --cert | TLS Certificate | TLS_CERT |  |
+| -K / --key | TLS Key | TLS_KEY |  |
+| -S / --cacert | TLS CA Certificate | TLS_CA |  |
+| -r / --retries | Num. retries on disconnect | MQTT_RETRIES | 3 |
+| Last argument | ASGI Apllication |  | |
 
 Environment variables are supported and can be set using a `.env` file on the root of the project, but passing a parameter overrides this value.
 
 ## Consumer
 
 To add your consumer to the `asgi.py` file in your django application:
 ```python
```

### Comparing `mqttasgi-1.2.1/mqttasgi/cli.py` & `mqttasgi-1.2.2/mqttasgi/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,14 +28,16 @@
     # add support for certificate authentication (TLS)
     parser.add_argument("-C", "--cert", help="MQTT TLS certificate",
                         default=os.environ.get("TLS_CERT", None))
     parser.add_argument("-K", "--key", help="MQTT TLS key",
                         default=os.environ.get("TLS_KEY", None))
     parser.add_argument("-S", "--cacert", help="MQTT TLS CA certificate",
                         default=os.environ.get("TLS_CA", None))
+    parser.add_argument("-r", "--retries", help="Maximum number of connection retries after unexpected disconnect (0 to always try to reconnect)",
+                        default=os.environ.get("MQTT_RETRIES", 3), type=int)
 
     parser.add_argument("application",
                         help=("The ASGI application instance to use as "
                               "path.to.module:application"))
 
     args = parser.parse_args()
 
@@ -57,13 +59,14 @@
         args.password,
         args.client_id,
         logger=logger,
         clean_session=args.cleansession,
         cert=args.cert,
         key=args.key,
         ca_cert=args.cacert,
+        connect_max_retries=args.retries
     )
 
     server.run()
 
 if __name__ == '__main__':
     main()
```

### Comparing `mqttasgi-1.2.1/mqttasgi/consumers.py` & `mqttasgi-1.2.2/mqttasgi/consumers.py`

 * *Files identical despite different names*

### Comparing `mqttasgi-1.2.1/mqttasgi/server.py` & `mqttasgi-1.2.2/mqttasgi/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,16 @@
         self.port = port
         self.client_id = client_id
         self.client = mqtt.Client(client_id=self.client_id, userdata={
             "server": self,
             "host": self.host,
             "port": self.port,
         }, clean_session=clean_session)
-        # self.client.enable_logger(self.log)
+
+        self.client.enable_logger(self.log)
         self.username = username
         self.password = password
         # certificates
         self.cert = cert
         self.key = key
         self.ca_cert = ca_cert
         self.client.on_connect = self._on_connect
@@ -70,50 +71,46 @@
                 })
             except Exception as e:
                 self.log.error("[mqttasgi][mqtt][connect] - Cant add to queue"
                                "of {}".format(app_id))
                 self.log.exception(e)
 
     def _on_disconnect(self, client, userdata, rc):
-        self.log.warning("[mqttasgi][connection][disconnected] - Disconnected from {}:{}".format(self.host,self.port))
+        self.log.warning("[mqttasgi][connection][disconnected] - Disconnected from {}:{}".format(self.host, self.port))
         if not self.stop:
-            if self.connect_max_retries != 0:
-                for i in range(self.connect_max_retries):
-                    self.log.info("[mqttasgi][connection][reconnect] - Attempting {} reconnect".format(i+1))
-                    try:
-                        client.reconnect()
-                        self.log.warning("[mqttasgi][connection][reconnect] - Reconnected after {} attempts".format(i+1))
-                        break
-                    except Exception as e:
-                        if i < self.connect_max_retries:
-                            self.log.info("[mqttasgi][connection][reconnect] - Failed {} sleeping for {} seconds".format(i+1, i+1))
-                            time.sleep(i+1)
-                            continue
-                        else:
-                            for app_id in self.application_data:
-
-                                self.application_data[app_id]['receive'].put_nowait({
-                                    'type': 'mqtt.disconnect',
-                                    'mqtt': {
-
-                                    }
-                                })
-                            raise
-            else:
-                exit = False
-                tries = 0
-                while not exit:
-                    try:
-                        client.reconnect()
-                        self.log.warning("[mqttasgi][connection][reconnect] - Reconnected after {} attempts".format(tries+1))
-                        exit = True
-                        break
-                    except Exception as e:
-                        tries += 1
-                        time.sleep(tries + 1 if tries<10 else 10)
+            self._handle_reconnect()
+
+    def _handle_reconnect(self, on_connect=False):
+        tries = 0
+        while tries < self.connect_max_retries or self.connect_max_retries == 0:
+            self.log.info("[mqttasgi][connection][reconnect] - Attempting {} reconnect".format(tries))
+            try:
+                if on_connect is False:
+                    self.client.reconnect()
+                else:
+                    self.client.connect(self.host, self.port)
+                self.log.warning("[mqttasgi][connection][reconnect] - Reconnected after {} attempts".format(tries))
+                break
+            except KeyboardInterrupt as e:
+                self.log.warning("[mqttasgi][connection][reconnect] - Keyboard Interrupt. Stopped trying to reconnect.")
+                raise e
+            except Exception as e:
+                self.log.debug("[mqttasgi][connection][reconnect] - Exception occurred during reconnect", exc_info=True)
+                time.sleep(min(tries,30))
+            tries += 1
+        else:  # executed only if the for-loop completes without a break
+            self._handle_reconnect_failure()
+
+    def _handle_reconnect_failure(self):
+        for app_id in self.application_data:
+            self.application_data[app_id]['receive'].put_nowait({
+                'type': 'mqtt.disconnect',
+                'mqtt': {}
+            })
+        raise Exception("[mqttasgi][connection][reconnect] - Failed to reconnect after {} attempts".format(self.connect_max_retries))
 
     def _mqtt_receive(self, subscription, topic, payload, qos):
         if subscription == -1:
             self.log.warning("[mqttasgi][mqtt][receive] - Received message that no app is subscribed"
                            " to topic:{} adding to queue".format(topic))
             if topic not in self.topic_queues:
                 self.topic_queues[topic] = []
@@ -137,35 +134,42 @@
                 })
             except Exception as e:
                 self.log.error("[mqttasgi][mqtt][receive] - Cant add to queue"
                                "of {}".format(app_id))
                 self.log.exception(e)
         self.log.debug("[mqttasgi][mqtt][receive] - Added message to queue app_ids:{} topic:{}".format(self.topics_subscription[subscription]['apps'], topic))
 
-
     async def mqtt_receive_loop(self):
 
         if self.username:
             self.client.username_pw_set(username=self.username, password=self.password)
 
         if all([self.cert, self.key, self.ca_cert]):
             self.client.tls_set(
                 ca_certs=self.ca_cert,
                 certfile=self.cert,
                 keyfile=self.key,
             )
 
-
-        self.client.connect(self.host, self.port)
+        try:
+            self.client.connect(self.host, self.port)
+        except Exception as e:
+            try:
+                self._handle_reconnect(on_connect=True)
+            except Exception as e:
+                await self.shutdown('CONNECTION_ERROR')
 
         self.log.info(f"MQTT loop start")
 
-        while True:
-            self.client.loop(0.01)
-            await asyncio.sleep(0.01)
+        try:
+            while not self.stop:
+                self.client.loop(timeout=0.01)
+                await asyncio.sleep(0.01)
+        except Exception as e:
+            await self.shutdown('Exception in receive loop')
 
     async def mqtt_publish(self, app_id, msg):
         mqqt_publication = msg['mqtt']
         self.log.debug("[mqttasgi][app][publish] - Application {} publishing at {}:{}"
                      .format(app_id, mqqt_publication['topic'], mqqt_publication.get('qos', 1)))
         self.client.publish(
             mqqt_publication['topic'],
@@ -228,15 +232,14 @@
                                        "of {}".format(app_id))
                         self.log.exception(e)
                 flushed_topics += [msg_topic]
 
         for msg_topic in flushed_topics:
             del self.topic_queues[msg_topic]
 
-
     async def mqtt_unsubscribe(self, app_id, msg, soft=False):
         mqqt_unsubscritpion = msg['mqtt']
         topic = mqqt_unsubscritpion['topic']
         if topic not in self.topics_subscription:
             self.log.error("[mqttasgi][app][unsubscribe] - Tried to unsubscribe from non existing topic {}".format(topic))
             return
         status = self.topics_subscription[topic]
@@ -322,17 +325,18 @@
             )
         self.log.warning("MQTTASGI Waiting for all applications to close")
         await asyncio.gather(*[self.application_data[app_id]["task"] for app_id in self.application_data])
         all_tasks = asyncio.Task.all_tasks if sys.version_info[1] < 7 else asyncio.all_tasks
         tasks = [t for t in all_tasks() if t is not asyncio.current_task()]
         self.log.info(f"Cancelling {len(tasks)} outstanding tasks")
         [task.cancel() for task in tasks]
-        self.loop.stop()
+        self.client.loop_stop()
         await asyncio.gather(*tasks, return_exceptions=True)
         self.log.info("Shutdown complete")
+        self.loop.stop()
 
     def create_application(self, app_id, instance_type='worker', consumer_path=None, consumer_parameters=None):
         scope = {}
         if consumer_parameters is not None:
             scope = {**consumer_parameters}
         scope = {**scope, **self.base_scope, 'app_id': app_id, 'instance_type': instance_type}
         if app_id in self.application_data:
```

### Comparing `mqttasgi-1.2.1/mqttasgi/testing.py` & `mqttasgi-1.2.2/mqttasgi/testing.py`

 * *Files identical despite different names*

### Comparing `mqttasgi-1.2.1/mqttasgi.egg-info/PKG-INFO` & `mqttasgi-1.2.2/mqttasgi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mqttasgi
-Version: 1.2.1
+Version: 1.2.2
 Summary: MQTT ASGI Protocol Server
 Home-page: https://github.com/sivulich/mqttasgi
 Author: Santiago Ivulich
 Author-email: sivulich@itba.edu.ar
 License: MIT
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
@@ -48,27 +48,28 @@
 # Usage
 ## Unit
 Mqttasgi provides a cli interface to run the protocol server. 
 ```bash
 mqttasgi -H localhost -p 1883 my_application.asgi:application
 ```
 Parameters:
-| Parameter   | Explanation      | Environment variable |
-|-------------|------------------|:--------------------:|
-| -H / --host | MQTT broker host | MQTT_HOSTNAME |
-| -p / --port | MQTT broker port | MQTT_PORT |
-| -c / --cleansession | MQTT Clean Session | MQTT_CLEAN |
-| -v / --verbosity | Logging verbosity | VERBOSITY |
-| -U / --username | MQTT Username | MQTT_USERNAME |
-| -P / --password | MQTT Password | MQTT_PASSWORD |
-| -i / --id | MQTT Client ID | MQTT_CLIENT_ID |
-| -C / --cert | TLS Certificate | TLS_CERT |
-| -K / --key | TLS Key | TLS_KEY |
-| -S / --cacert | TLS CA Certificate | TLS_CA |
-| Last argument | ASGI Apllication |  |
+| Parameter   | Explanation      | Environment variable | Default |
+|-------------|------------------|:--------------------:|:--------------------:|
+| -H / --host | MQTT broker host | MQTT_HOSTNAME | localhost |
+| -p / --port | MQTT broker port | MQTT_PORT | 1883 |
+| -c / --cleansession | MQTT Clean Session | MQTT_CLEAN | True |
+| -v / --verbosity | Logging verbosity | VERBOSITY | 0 |
+| -U / --username | MQTT Username | MQTT_USERNAME |  |
+| -P / --password | MQTT Password | MQTT_PASSWORD |  |
+| -i / --id | MQTT Client ID | MQTT_CLIENT_ID |  |
+| -C / --cert | TLS Certificate | TLS_CERT |  |
+| -K / --key | TLS Key | TLS_KEY |  |
+| -S / --cacert | TLS CA Certificate | TLS_CA |  |
+| -r / --retries | Num. retries on disconnect | MQTT_RETRIES | 3 |
+| Last argument | ASGI Apllication |  | |
 
 Environment variables are supported and can be set using a `.env` file on the root of the project, but passing a parameter overrides this value.
 
 ## Consumer
 
 To add your consumer to the `asgi.py` file in your django application:
 ```python
```

### Comparing `mqttasgi-1.2.1/setup.py` & `mqttasgi-1.2.2/setup.py`

 * *Files identical despite different names*

