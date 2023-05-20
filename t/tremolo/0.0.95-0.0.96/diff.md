# Comparing `tmp/tremolo-0.0.95.tar.gz` & `tmp/tremolo-0.0.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tremolo-0.0.95.tar", last modified: Mon May 15 04:17:18 2023, max compression
+gzip compressed data, was "dist/tremolo-0.0.96.tar", last modified: Sat May 20 02:14:41 2023, max compression
```

## Comparing `tremolo-0.0.95.tar` & `tremolo-0.0.96.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-15 04:17:18.000000 tremolo-0.0.95/
--rw-r--r--   0 tux       (1000) users      (100)     1063 2023-05-08 03:43:30.000000 tremolo-0.0.95/LICENSE.txt
--rw-r--r--   0 tux       (1000) users      (100)     4619 2023-05-15 04:17:18.000000 tremolo-0.0.95/PKG-INFO
--rw-r--r--   0 tux       (1000) users      (100)     4019 2023-05-15 04:15:11.000000 tremolo-0.0.95/README.md
--rw-r--r--   0 tux       (1000) users      (100)       38 2023-05-15 04:17:18.000000 tremolo-0.0.95/setup.cfg
--rwxr-xr-x   0 tux       (1000) users      (100)      975 2023-05-15 04:14:43.000000 tremolo-0.0.95/setup.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-15 04:17:18.000000 tremolo-0.0.95/tremolo/
--rwxr-xr-x   0 tux       (1000) users      (100)       54 2023-05-08 03:43:30.000000 tremolo-0.0.95/tremolo/__init__.py
--rw-r--r--   0 tux       (1000) users      (100)     4465 2023-05-08 03:43:30.000000 tremolo-0.0.95/tremolo/__main__.py
--rw-r--r--   0 tux       (1000) users      (100)     2278 2023-05-08 03:43:30.000000 tremolo-0.0.95/tremolo/asgi_lifespan.py
--rw-r--r--   0 tux       (1000) users      (100)     5850 2023-05-14 00:12:56.000000 tremolo-0.0.95/tremolo/asgi_server.py
--rw-r--r--   0 tux       (1000) users      (100)      542 2023-05-08 03:43:30.000000 tremolo-0.0.95/tremolo/contexts.py
--rw-r--r--   0 tux       (1000) users      (100)      586 2023-05-08 03:43:30.000000 tremolo-0.0.95/tremolo/exceptions.py
--rw-r--r--   0 tux       (1000) users      (100)    11243 2023-05-08 03:43:30.000000 tremolo-0.0.95/tremolo/http_server.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-15 04:17:18.000000 tremolo-0.0.95/tremolo/lib/
--rwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-08 03:43:30.000000 tremolo-0.0.95/tremolo/lib/__init__.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-15 04:17:18.000000 tremolo-0.0.95/tremolo/lib/h1parser/
--rw-r--r--   0 tux       (1000) users      (100)       38 2023-05-08 03:43:30.000000 tremolo-0.0.95/tremolo/lib/h1parser/__init__.py
--rwxr-xr-x   0 tux       (1000) users      (100)     4954 2023-05-08 03:43:30.000000 tremolo-0.0.95/tremolo/lib/h1parser/parse_header.py
--rw-r--r--   0 tux       (1000) users      (100)     1798 2023-05-08 03:43:30.000000 tremolo-0.0.95/tremolo/lib/http_exception.py
--rwxr-xr-x   0 tux       (1000) users      (100)    13737 2023-05-08 03:43:30.000000 tremolo-0.0.95/tremolo/lib/http_protocol.py
--rwxr-xr-x   0 tux       (1000) users      (100)     9307 2023-05-08 03:43:30.000000 tremolo-0.0.95/tremolo/lib/http_request.py
--rwxr-xr-x   0 tux       (1000) users      (100)    11322 2023-05-12 01:18:27.000000 tremolo-0.0.95/tremolo/lib/http_response.py
--rw-r--r--   0 tux       (1000) users      (100)      844 2023-05-08 03:43:30.000000 tremolo-0.0.95/tremolo/lib/object_pool.py
--rwxr-xr-x   0 tux       (1000) users      (100)     1259 2023-05-08 03:43:30.000000 tremolo-0.0.95/tremolo/lib/request.py
--rwxr-xr-x   0 tux       (1000) users      (100)      810 2023-05-08 03:43:30.000000 tremolo-0.0.95/tremolo/lib/response.py
--rwxr-xr-x   0 tux       (1000) users      (100)    15287 2023-05-08 03:43:30.000000 tremolo-0.0.95/tremolo/tremolo.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-15 04:17:18.000000 tremolo-0.0.95/tremolo.egg-info/
--rw-r--r--   0 tux       (1000) users      (100)     4619 2023-05-15 04:17:18.000000 tremolo-0.0.95/tremolo.egg-info/PKG-INFO
--rw-r--r--   0 tux       (1000) users      (100)      610 2023-05-15 04:17:18.000000 tremolo-0.0.95/tremolo.egg-info/SOURCES.txt
--rw-r--r--   0 tux       (1000) users      (100)        1 2023-05-15 04:17:18.000000 tremolo-0.0.95/tremolo.egg-info/dependency_links.txt
--rw-r--r--   0 tux       (1000) users      (100)        8 2023-05-15 04:17:18.000000 tremolo-0.0.95/tremolo.egg-info/top_level.txt
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-20 02:14:41.000000 tremolo-0.0.96/
+-rw-r--r--   0 tux       (1000) users      (100)     1063 2023-05-08 03:43:30.000000 tremolo-0.0.96/LICENSE.txt
+-rw-r--r--   0 tux       (1000) users      (100)     4619 2023-05-20 02:14:41.000000 tremolo-0.0.96/PKG-INFO
+-rw-r--r--   0 tux       (1000) users      (100)     4019 2023-05-15 04:15:11.000000 tremolo-0.0.96/README.md
+-rw-r--r--   0 tux       (1000) users      (100)       38 2023-05-20 02:14:41.000000 tremolo-0.0.96/setup.cfg
+-rwxr-xr-x   0 tux       (1000) users      (100)      975 2023-05-20 01:27:53.000000 tremolo-0.0.96/setup.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-20 02:14:41.000000 tremolo-0.0.96/tremolo/
+-rwxr-xr-x   0 tux       (1000) users      (100)       54 2023-05-08 03:43:30.000000 tremolo-0.0.96/tremolo/__init__.py
+-rw-r--r--   0 tux       (1000) users      (100)     4465 2023-05-08 03:43:30.000000 tremolo-0.0.96/tremolo/__main__.py
+-rw-r--r--   0 tux       (1000) users      (100)     2278 2023-05-08 03:43:30.000000 tremolo-0.0.96/tremolo/asgi_lifespan.py
+-rw-r--r--   0 tux       (1000) users      (100)     5666 2023-05-19 13:26:48.000000 tremolo-0.0.96/tremolo/asgi_server.py
+-rw-r--r--   0 tux       (1000) users      (100)      542 2023-05-08 03:43:30.000000 tremolo-0.0.96/tremolo/contexts.py
+-rw-r--r--   0 tux       (1000) users      (100)      586 2023-05-08 03:43:30.000000 tremolo-0.0.96/tremolo/exceptions.py
+-rw-r--r--   0 tux       (1000) users      (100)    10617 2023-05-19 14:03:18.000000 tremolo-0.0.96/tremolo/http_server.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-20 02:14:41.000000 tremolo-0.0.96/tremolo/lib/
+-rwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-08 03:43:30.000000 tremolo-0.0.96/tremolo/lib/__init__.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-20 02:14:41.000000 tremolo-0.0.96/tremolo/lib/h1parser/
+-rw-r--r--   0 tux       (1000) users      (100)       38 2023-05-08 03:43:30.000000 tremolo-0.0.96/tremolo/lib/h1parser/__init__.py
+-rwxr-xr-x   0 tux       (1000) users      (100)     4954 2023-05-08 03:43:30.000000 tremolo-0.0.96/tremolo/lib/h1parser/parse_header.py
+-rw-r--r--   0 tux       (1000) users      (100)     1798 2023-05-08 03:43:30.000000 tremolo-0.0.96/tremolo/lib/http_exception.py
+-rwxr-xr-x   0 tux       (1000) users      (100)    13730 2023-05-19 23:48:54.000000 tremolo-0.0.96/tremolo/lib/http_protocol.py
+-rwxr-xr-x   0 tux       (1000) users      (100)     9281 2023-05-19 23:50:26.000000 tremolo-0.0.96/tremolo/lib/http_request.py
+-rwxr-xr-x   0 tux       (1000) users      (100)    11322 2023-05-20 00:56:10.000000 tremolo-0.0.96/tremolo/lib/http_response.py
+-rw-r--r--   0 tux       (1000) users      (100)      772 2023-05-19 07:52:08.000000 tremolo-0.0.96/tremolo/lib/object_pool.py
+-rwxr-xr-x   0 tux       (1000) users      (100)     1259 2023-05-19 02:59:43.000000 tremolo-0.0.96/tremolo/lib/request.py
+-rwxr-xr-x   0 tux       (1000) users      (100)      810 2023-05-08 03:43:30.000000 tremolo-0.0.96/tremolo/lib/response.py
+-rwxr-xr-x   0 tux       (1000) users      (100)    15287 2023-05-08 03:43:30.000000 tremolo-0.0.96/tremolo/tremolo.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-20 02:14:41.000000 tremolo-0.0.96/tremolo.egg-info/
+-rw-r--r--   0 tux       (1000) users      (100)     4619 2023-05-20 02:14:40.000000 tremolo-0.0.96/tremolo.egg-info/PKG-INFO
+-rw-r--r--   0 tux       (1000) users      (100)      610 2023-05-20 02:14:41.000000 tremolo-0.0.96/tremolo.egg-info/SOURCES.txt
+-rw-r--r--   0 tux       (1000) users      (100)        1 2023-05-20 02:14:40.000000 tremolo-0.0.96/tremolo.egg-info/dependency_links.txt
+-rw-r--r--   0 tux       (1000) users      (100)        8 2023-05-20 02:14:40.000000 tremolo-0.0.96/tremolo.egg-info/top_level.txt
```

### Comparing `tremolo-0.0.95/LICENSE.txt` & `tremolo-0.0.96/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.95/PKG-INFO` & `tremolo-0.0.96/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tremolo
-Version: 0.0.95
+Version: 0.0.96
 Summary: Tremolo is a stream-oriented, asynchronous web server/framework written in pure Python
 Home-page: https://github.com/nggit/tremolo
 Author: nggit
 Author-email: contact@anggit.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tremolo-0.0.95/README.md` & `tremolo-0.0.96/README.md`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.95/setup.py` & `tremolo-0.0.96/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='tremolo',
     packages=['tremolo'],
     package_data={'': ['lib/*', 'lib/h1parser/*']},
-    version='0.0.95',
+    version='0.0.96',
     license='MIT',
     author='nggit',
     author_email='contact@anggit.com',
     description='Tremolo is a stream-oriented, asynchronous web server/framework written in pure Python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/nggit/tremolo',
```

### Comparing `tremolo-0.0.95/tremolo/__main__.py` & `tremolo-0.0.96/tremolo/__main__.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.95/tremolo/asgi_lifespan.py` & `tremolo-0.0.96/tremolo/asgi_lifespan.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.95/tremolo/asgi_server.py` & `tremolo-0.0.96/tremolo/asgi_server.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,50 +11,46 @@
 from .contexts import ServerContext
 from .exceptions import ExpectationFailed, InternalServerError
 from .lib.http_protocol import HTTPProtocol
 
 class ASGIServer(HTTPProtocol):
     def __init__(self, **kwargs):
         self._app = kwargs['_app']
-        self._request = None
-        self._response = None
         self._read = None
         self._task = None
         self._timer = None
         self._timeout = 30
 
         super().__init__(ServerContext(), **kwargs)
 
-    async def header_received(self, request, response):
-        if request.http_continue:
-            if request.content_length > self.options['client_max_body_size']:
+    async def header_received(self):
+        if self.request.http_continue:
+            if self.request.content_length > self.options['client_max_body_size']:
                 raise ExpectationFailed
 
-            await response.send(b'HTTP/%s 100 Continue\r\n\r\n' % request.version)
+            await self.response.send(b'HTTP/%s 100 Continue\r\n\r\n' % self.request.version)
 
         scope = {
             'type': 'http',
             'asgi': {'version': '3.0'},
-            'http_version': request.version.decode(encoding='utf-8'),
-            'method': request.method.decode(encoding='utf-8'),
+            'http_version': self.request.version.decode(encoding='utf-8'),
+            'method': self.request.method.decode(encoding='utf-8'),
             'scheme': {True: 'http',
-                       False: 'https'}[request.transport.get_extra_info('sslcontext') is None],
-            'path': unquote(request.path.decode(encoding='utf-8'), encoding='utf-8'),
-            'raw_path': request.path,
-            'query_string': request.query_string,
-            'headers': request.protocol.header.getheaders(),
-            'client': request.transport.get_extra_info('peername'),
-            'server': request.transport.get_extra_info('sockname')
+                       False: 'https'}[self.request.transport.get_extra_info('sslcontext') is None],
+            'path': unquote(self.request.path.decode(encoding='utf-8'), encoding='utf-8'),
+            'raw_path': self.request.path,
+            'query_string': self.request.query_string,
+            'headers': self.request.header.getheaders(),
+            'client': self.request.transport.get_extra_info('peername'),
+            'server': self.request.transport.get_extra_info('sockname')
         }
 
-        self._request = request
-        self._response = response
-        self._read = request.read(cache=False)
+        self._read = self.request.read(cache=False)
 
-        if not (b'transfer-encoding' in request.headers or b'content-length' in request.headers
+        if not (b'transfer-encoding' in self.request.headers or b'content-length' in self.request.headers
                 ) and self.queue[0] is not None:
             # avoid blocking on initial receive() due to empty Queue
             # in the case of bodyless requests, e.g. GET
             self.queue[0].put_nowait(b'')
 
         self._task = self.loop.create_task(self.app(scope))
 
@@ -69,74 +65,73 @@
             await self._app(scope, self.receive, self.send)
 
             if self._timer is not None:
                 self._timer.cancel()
         except asyncio.CancelledError:
             self.options['logger'].warning('task: ASGI application is cancelled due to timeout')
         except Exception as exc:
-            await self.handle_exception(InternalServerError(cause=exc), self._request, self._response)
+            await self.handle_exception(InternalServerError(cause=exc))
 
     async def receive(self):
         try:
             data = await self._read.__anext__()
 
             return {
                 'type': 'http.request',
                 'body': data,
-                'more_body': ((data != b'' and self._request.content_length == -1)
-                    or self._request.body_size < self._request.content_length)
+                'more_body': ((data != b'' and self.request.content_length == -1)
+                    or self.request.body_size < self.request.content_length)
             }
         except Exception as exc:
-            if not (self._request is None or isinstance(exc, StopAsyncIteration)):
+            if not (self.request is None or isinstance(exc, StopAsyncIteration)):
                 self.print_exception(exc)
 
             if self._timer is None:
                 self._timer = self.loop.call_at(self.loop.time() + self._timeout, self._task.cancel)
 
             return {'type': 'http.disconnect'}
 
     async def send(self, data):
         try:
             if data['type'] == 'http.response.start':
-                self._response.set_status(data['status'], HTTPStatus(data['status']).phrase)
-                self._response.append_header(b'Date: %s\r\nServer: %s\r\n' % (
-                                             datetime.utcnow().strftime('%a, %d %b %Y %H:%M:%S GMT').encode(encoding='latin-1'),
-                                             self.options['server_name']))
+                self.response.set_status(data['status'], HTTPStatus(data['status']).phrase)
+                self.response.append_header(b'Date: %s\r\nServer: %s\r\n' % (
+                                            datetime.utcnow().strftime('%a, %d %b %Y %H:%M:%S GMT').encode(encoding='latin-1'),
+                                            self.options['server_name']))
 
                 if 'headers' in data:
                     for header in data['headers']:
                         if not (header[0].find(b'\n') == -1 and header[1].find(b'\n') == -1):
                             await self.handle_exception(
-                                InternalServerError('name or value cannot contain illegal characters'),
-                                self._request, self._response)
+                                InternalServerError('name or value cannot contain illegal characters'))
                             return
 
                         name = header[0].lower()
 
                         if name == b'content-type':
-                            self._response.set_content_type(header[1])
+                            self.response.set_content_type(header[1])
                             continue
 
                         if name in (b'connection', b'date', b'server', b'transfer-encoding'):
                             # disallow apps from changing them, as they are managed by Tremolo
                             continue
 
                         if name == b'content-length':
-                            # will disable http chunked in the self._response.write()
-                            self._request.http_keepalive = False
+                            # will disable http chunked in the self.response.write()
+                            self.request.http_keepalive = False
 
                         if isinstance(header, list):
                             header = tuple(header)
 
-                        self._response.append_header(b'%s: %s\r\n' % header)
+                        self.response.append_header(b'%s: %s\r\n' % header)
             elif data['type'] == 'http.response.body':
                 if 'body' in data:
-                    await self._response.write(data['body'])
+                    await self.response.write(data['body'])
 
                 if 'more_body' not in data or data['more_body'] is False:
-                    await self._response.write(b'', throttle=False)
-                    await self._response.send(None)
+                    await self.response.write(b'', throttle=False)
+                    await self.response.send(None)
         except asyncio.CancelledError:
             pass
         except Exception as exc:
-            if not (self._request is None or self._response is None):
+            if not (self.request is None or self.response is None):
                 self.print_exception(exc)
```

### Comparing `tremolo-0.0.95/tremolo/contexts.py` & `tremolo-0.0.96/tremolo/contexts.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.95/tremolo/exceptions.py` & `tremolo-0.0.96/tremolo/exceptions.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.95/tremolo/http_server.py` & `tremolo-0.0.96/tremolo/lib/http_protocol.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,298 +1,370 @@
 # Copyright (c) 2023 nggit
 
-__all__ = ('HTTPServer',)
+import asyncio
+import traceback
 
 from datetime import datetime
-from urllib.parse import parse_qs
 
-from .contexts import ServerContext
-from .exceptions import ExpectationFailed
-from .lib.http_protocol import HTTPProtocol
-
-class HTTPServer(HTTPProtocol):
-    def __init__(self, **kwargs):
-        self._route_handlers = kwargs['_handlers']
-        self._middlewares = kwargs['_middlewares']
-        self._server = {
-            'loop': kwargs['loop'],
-            'logger': kwargs['logger'],
-            'socket': kwargs['sock'],
-            'context': ServerContext(),
-            'request': None,
-            'response': None
-        }
-
-        super().__init__(self._server['context'], **kwargs)
+from .h1parser import ParseHeader
+from .http_exception import HTTPException, BadRequest, InternalServerError
+from .http_request import HTTPRequest
+from .http_response import HTTPResponse
+
+class HTTPProtocol(asyncio.Protocol):
+    def __init__(self, context, **kwargs):
+        self._context = context
+        self._options = kwargs
 
-    async def _connection_made(self, func):
-        await func(**self._server)
-
-        if self._server['context']._on_connect is not None:
-            self._server['context']._on_connect.set_result(None)
-
-    async def _connection_lost(self, func, exc):
         try:
-            await func(**self._server)
-        finally:
-            super().connection_lost(exc)
+            self._loop = kwargs['loop']
+        except KeyError:
+            self._loop = asyncio.get_event_loop()
+
+        self._transport = None
+        self._queue = (None, None)
+        self._request = None
+        self._response = None
+        self._watermarks = {'high': 65536, 'low': 8192}
+
+    @property
+    def context(self):
+        return self._context
+
+    @property
+    def tasks(self):
+        return self._context.tasks
+
+    @property
+    def options(self):
+        return self._options
+
+    @property
+    def loop(self):
+        return self._loop
+
+    @property
+    def transport(self):
+        return self._transport
+
+    @property
+    def queue(self):
+        return self._queue
+
+    @property
+    def request(self):
+        return self._request
+
+    @property
+    def response(self):
+        return self._response
 
     def connection_made(self, transport):
-        super().connection_made(transport)
+        self._transport = transport
+        self._pool = self._options['_pool'].get()
+        self._queue = self._pool['queue']
 
-        func = self._middlewares['connect'][-1][0]
-        self._server['context'].set('options', self._middlewares['connect'][-1][1])
+        self._data = bytearray()
+        self._timeout_waiters = {'request': self._loop.create_future()}
 
-        if func is None:
-            self._server['context']._on_connect = None
-        else:
-            self._server['context']._on_connect = self._server['loop'].create_future()
+        for task in (self._send_data(), self.set_timeout(self._timeout_waiters['request'],
+                                                         timeout=self._options['request_timeout'],
+                                                         timeout_cb=self.request_timeout)):
+            self.tasks.append(self._loop.create_task(task))
 
-            self._server['context'].tasks.append(
-                self._server['loop'].create_task(self._connection_made(func))
-            )
+    async def request_timeout(self, timeout):
+        self._options['logger'].info('request timeout after {:g}s'.format(timeout))
 
-    def connection_lost(self, exc):
-        func = self._middlewares['close'][-1][0]
+    async def keepalive_timeout(self, timeout):
+        self._options['logger'].info('keepalive timeout after {:g}s'.format(timeout))
 
-        if func is None:
-            super().connection_lost(exc)
-            return
+    async def send_timeout(self, timeout):
+        self._options['logger'].info('send timeout after {:g}s'.format(timeout))
 
-        self._server['loop'].create_task(self._connection_lost(func, exc))
+    async def set_timeout(self, waiter, timeout=30, timeout_cb=None):
+        timer = self._loop.call_at(self._loop.time() + timeout, waiter.cancel)
 
-    def _set_base_header(self, options={}):
-        if self._server['response'].header is None or self._server['response'].header[1] != b'':
-            return
+        try:
+            return await waiter
+        except asyncio.CancelledError:
+            if self._transport is not None:
+                if callable(timeout_cb):
+                    await timeout_cb(timeout)
 
-        options['server_name'] = options.get('server_name', self.options['server_name'])
+                if self._transport is not None and not self._transport.is_closing():
+                    self._transport.abort()
+        finally:
+            timer.cancel()
 
-        if isinstance(options['server_name'], str):
-            options['server_name'] = options['server_name'].encode(encoding='latin-1')
+    async def put_to_queue(self, data, queue=None, transport=None, rate=1048576, buffer_size=16 * 1024):
+        data_size = len(data)
 
-        self._server['response'].append_header(b'Date: %s\r\nServer: %s\r\n' % (
-                                               datetime.utcnow().strftime('%a, %d %b %Y %H:%M:%S GMT').encode(encoding='latin-1'),
-                                               options['server_name']))
+        if data_size >= 2 * buffer_size:
+            mv = memoryview(data)
 
-    async def _handle_middleware(self, func, options={}):
-        if self._server['response'].header is not None:
-            self._set_base_header(options)
-            self._server['context'].set('options', options)
+            while mv and queue is not None:
+                queue.put_nowait(mv[:buffer_size].tobytes())
+                await asyncio.sleep(1 / (rate / max(queue.qsize(), 1) / mv[:buffer_size].nbytes))
+                mv = mv[buffer_size:]
+
+        elif data != b'' and queue is not None:
+            queue.put_nowait(data)
+            await asyncio.sleep(1 / (rate / max(queue.qsize(), 1) / data_size))
+
+        if transport is not None and self._request is not None:
+            if self._request.http_upgrade:
+                transport.resume_reading()
+                return
 
-        data = await func(**self._server)
+            self._request.body_size += data_size
 
-        if data is None:
-            return options
+            if (b'content-length' in self._request.headers and self._request.body_size >= self._request.content_length
+                    and queue is not None):
+                queue.put_nowait(None)
+            elif self._request.body_size < self._options['client_max_body_size']:
+                transport.resume_reading()
+            else:
+                if self._queue[1] is not None:
+                    self._request.http_keepalive = False
+                    self._queue[1].put_nowait(None)
+
+                self._options['logger'].info('payload too large')
+
+    async def header_received(self):
+        return
+
+    def print_exception(self, exc, *args):
+        self._options['logger'].error(': '.join(
+            (*args, exc.__class__.__name__, str(exc))
+        ), exc_info={True: exc, False: False}[self._options['debug']])
 
-        if not isinstance(data, (bytes, bytearray, str, tuple)):
+    async def handle_exception(self, exc):
+        if self._request is None or self._response is None or self._response.header is None:
             return
 
-        if 'status' in options:
-            self._server['response'].set_status(*options['status'])
-
-        if 'content_type' in options:
-            self._server['response'].set_content_type(options['content_type'])
+        self.print_exception(exc, self._request.path.decode(encoding='latin-1'))
 
-        encoding = ('utf-8',)
+        encoding = 'utf-8'
 
-        if isinstance(data, tuple):
-            data, *encoding = (*data, 'utf-8')
+        for v in exc.content_type.split(';'):
+            v = v.lstrip()
 
-        if isinstance(data, str):
-            data = data.encode(encoding=encoding[0])
+            if v.startswith('charset='):
+                charset = v[len('charset='):].strip()
 
-        await self._server['response'].end(data)
+                if charset != '':
+                    encoding = charset
 
-    async def _handle_continue(self):
-        if self._server['request'].http_continue:
-            if self._server['request'].content_length > self.options['client_max_body_size']:
-                raise ExpectationFailed
+                break
 
-            await self._server['response'].send(b'HTTP/%s 100 Continue\r\n\r\n' % self._server['request'].version)
-
-    async def _handle_response(self, func, options={}):
-        options['rate'] = options.get('rate', self.options['download_rate'])
-        options['buffer_size'] = options.get('buffer_size', self.options['buffer_size'])
-
-        if 'status' in options:
-            self._server['response'].set_status(*options['status'])
+        if self.options['debug']:
+            data = b'<ul><li>%s</li></ul>' % '</li><li>'.join(
+                traceback.TracebackException.from_exception(exc).format()
+            ).encode(encoding=encoding)
+        else:
+            data = str(exc).encode(encoding=encoding)
 
-        if 'content_type' in options:
-            self._server['response'].set_content_type(options['content_type'])
+        await self._response.send((
+            b'HTTP/%s %d %s\r\nContent-Type: %s\r\nContent-Length: %d\r\nConnection: close\r\n' +
+            b'Date: %s\r\nServer: %s\r\n\r\n%s') % (self._request.version,
+                                                    exc.code,
+                                                    exc.message.encode(encoding='latin-1'),
+                                                    exc.content_type.encode(encoding='latin-1'),
+                                                    len(data),
+                                                    datetime.utcnow().strftime(
+                                                        '%a, %d %b %Y %H:%M:%S GMT').encode(encoding='latin-1'),
+                                                    self._options['server_name'],
+                                                    data))
+
+        self._response.close()
+
+    async def _handle_request_header(self, data, header_size):
+        self._data = None
+        header = ParseHeader(data, header_size=header_size, excludes=[b'proxy'])
+
+        if not header.is_request:
+            if self._queue[1] is not None:
+                self._queue[1].put_nowait(None)
 
-        self._set_base_header(options)
+            self._options['logger'].info('bad request: not a request')
+            return
 
-        self._server['context'].set('options', options)
-        agen = func(**self._server)
+        self._request = HTTPRequest(self, header)
+        self._response = HTTPResponse(self._request)
 
         try:
-            data = await agen.__anext__()
-            is_agen = True
-        except AttributeError:
-            data = await agen
-
-            if data is None:
-                self._server['response'].close()
-                return
-
-            if not isinstance(data, (bytes, bytearray, str, tuple)):
-                return
-
-            is_agen = False
-
-        status = self._server['response'].get_status()
-        no_content = status[0] in (204, 304) or 100 <= status[0] < 200
-        self._server['response'].http_chunked = options.get(
-            'chunked', self._server['request'].version == b'1.1' and self._server['request'].http_keepalive and not no_content
-        )
-
-        if self._server['response'].http_chunked:
-            self._server['response'].append_header(b'Transfer-Encoding: chunked\r\n')
-
-        if self._middlewares['send'][-1][0] is not None:
-            self._server['response'].set_write_callback(
-                lambda : self._handle_middleware(
-                    self._middlewares['send'][-1][0], {**self._middlewares['send'][-1][1], **options})
-            )
-
-        self._server['response'].header = b'HTTP/%s %d %s\r\n' % (self._server['request'].version, *status)
-
-        if is_agen:
-            if no_content:
-                self._server['response'].append_header(b'Connection: close\r\n\r\n')
-            else:
-                if not self._server['response'].http_chunked:
-                    self._server['request'].http_keepalive = False
-
-                if status[0] == 101:
-                    self._server['request'].http_upgrade = True
-
-                self._server['response'].append_header(
-                    b'Content-Type: %s\r\nConnection: %s\r\n\r\n' %
-                    (self._server['response'].get_content_type(), {False: b'keep-alive',
-                                                                   True: b'upgrade'}[status[0] in (101, 426)])
+            if b'connection' in self._request.headers:
+                if self._request.headers[b'connection'].lower().find(b'close') == -1:
+                    self._request.http_keepalive = True
+            elif self._request.version == b'1.1':
+                self._request.http_keepalive = True
+
+            if b'transfer-encoding' in self._request.headers or b'content-length' in self._request.headers:
+                # assuming a request with a body, such as POST
+                if b'content-type' in self._request.headers:
+                    self._request.content_type = self._request.headers[b'content-type'].lower()
+
+                if b'transfer-encoding' in self._request.headers:
+                    if self._request.version == b'1.0':
+                        raise BadRequest
+
+                    self._request.transfer_encoding = self._request.headers[b'transfer-encoding'].lower()
+
+                if b'content-length' in self._request.headers:
+                    if self._request.transfer_encoding.find(b'chunked') > -1:
+                        raise BadRequest
+
+                    self._request.content_length = int(self._request.headers[b'content-length'])
+                elif self._request.version == b'1.0':
+                    raise BadRequest
+
+                if b'expect' in self._request.headers and self._request.headers[b'expect'].lower() == b'100-continue':
+                    self._request.http_continue = True
+
+                # the initial body that accompanies the header
+                await self.put_to_queue(
+                    data[header_size + 4:], queue=self._queue[0], transport=self._transport, rate=self._options['upload_rate']
                 )
 
-            if self._server['request'].method == b'HEAD' or no_content:
-                await self._server['response'].write(None)
-                return
-
-            self.set_watermarks(high=options['buffer_size'] * 4, low=options['buffer_size'] // 2)
-            await self._server['response'].write(
-                data, rate=options['rate'], buffer_size=options['buffer_size']
-            )
-
-            while True:
-                try:
-                    data = await agen.__anext__()
-
-                    await self._server['response'].write(
-                        data, rate=options['rate'], buffer_size=options['buffer_size']
-                    )
-                except StopAsyncIteration:
-                    await self._server['response'].write(b'', throttle=False)
-                    break
-        else:
-            encoding = ('utf-8',)
-
-            if isinstance(data, tuple):
-                data, *encoding = (*data, 'utf-8')
-
-            if isinstance(data, str):
-                data = data.encode(encoding=encoding[0])
-
-            if no_content or data == b'':
-                self._server['response'].append_header(b'Connection: close\r\n\r\n')
-            else:
-                if self._server['response'].http_chunked:
-                    self._server['response'].append_header(b'Content-Type: %s\r\nConnection: keep-alive\r\n\r\n'
-                                                           % self._server['response'].get_content_type())
-                else:
-                    self._server['response'].append_header(
-                        b'Content-Type: %s\r\nContent-Length: %d\r\nConnection: %s\r\n\r\n' % (
-                        self._server['response'].get_content_type(), len(data), {
-                            True: b'keep-alive',
-                            False: b'close'}[self._server['request'].http_keepalive])
-                    )
-
-            if data == b'' or self._server['request'].method == b'HEAD' or no_content:
-                await self._server['response'].write(None)
-                return
-
-            self.set_watermarks(high=options['buffer_size'] * 4, low=options['buffer_size'] // 2)
-            await self._server['response'].write(data, rate=options['rate'], buffer_size=options['buffer_size'])
-            await self._server['response'].write(b'', throttle=False)
-
-        await self._server['response'].send(None)
-
-    async def header_received(self, request, response):
-        self._server['request'] = request
-        self._server['response'] = response
-
-        if self._server['context']._on_connect is not None:
-            await self._server['context']._on_connect
-            self._server['context']._on_connect = None
+            await self.header_received()
+        except Exception as exc:
+            if not isinstance(exc, HTTPException):
+                exc = InternalServerError(cause=exc)
+
+            await self.handle_exception(exc)
+
+    def data_received(self, data):
+        if self._data is not None:
+            self._data.extend(data)
+            header_size = self._data.find(b'\r\n\r\n')
+
+            if -1 < header_size <= 8192:
+                self._transport.pause_reading()
+
+                # got header, clear either the request or keepalive timeout
+                for i in self._timeout_waiters:
+                    if i != 'send' and not self._timeout_waiters[i].done():
+                        self._timeout_waiters[i].set_result(None)
+
+                self.tasks.append(self._loop.create_task(self._handle_request_header(self._data, header_size)))
+            elif header_size > 8192:
+                self._options['logger'].info('request header too large')
+                self._transport.abort()
+            elif not (header_size == -1 and len(self._data) <= 8192):
+                self._options['logger'].info('bad request')
+                self._transport.abort()
 
-        options = self._server['context'].options
-
-        for middleware in self._middlewares['request']:
-            options = await self._handle_middleware(middleware[0], {**middleware[1], **options})
-
-            if not isinstance(options, dict):
-                return
-
-        if not request.is_valid:
-            # bad request
-            await self._handle_response(self._route_handlers[0][0][1], {**self._route_handlers[0][0][2], **options})
             return
 
-        if request.query_string != b'':
-            self._server['request'].query = parse_qs(request.query_string.decode(encoding='latin-1'))
-
-        p = request.path.strip(b'/')
-
-        if p == b'':
-            ri = 1
-        else:
-            ri = b'%d#%s' % (p.count(b'/') + 2, p[:(p + b'/').find(b'/')])
-
-        if ri in self._route_handlers:
-            for (pattern, func, kwargs) in self._route_handlers[ri]:
-                m = pattern.search(request.url)
+        self._transport.pause_reading()
+        self._loop.create_task(
+            self.put_to_queue(data, queue=self._queue[0], transport=self._transport, rate=self._options['upload_rate'])
+        )
 
-                if m:
-                    await self._handle_continue()
+    def eof_received(self):
+        self._queue[0].put_nowait(None)
 
-                    matches = m.groupdict()
+    def resume_writing(self):
+        if 'send' in self._timeout_waiters and not self._timeout_waiters['send'].done():
+            self._timeout_waiters['send'].set_result(None)
+
+    def set_watermarks(self, high=65536, low=8192):
+        if self._transport is not None:
+            self._watermarks['high'] = high
+            self._watermarks['low'] = low
+
+            self._transport.set_write_buffer_limits(high=high, low=low)
+
+    async def _send_data(self):
+        while self._queue[1] is not None:
+            try:
+                data = await self._queue[1].get()
+                self._queue[1].task_done()
+
+                if data is None:
+                    # close the transport, unless keepalive is enabled
+                    if self._request is not None:
+                        if self._request.http_keepalive and self._data is None:
+                            self._handle_keepalive()
+                            continue
 
-                    if not matches:
-                        matches = m.groups()
+                        self._request.clear_body()
 
-                    self._server['request'].params['path'] = matches
+                    if self._transport.can_write_eof():
+                        self._transport.write_eof()
 
-                    await self._handle_response(func, {**kwargs, **options})
+                    self._transport.close()
                     return
-        else:
-            for i, (pattern, func, kwargs) in enumerate(self._route_handlers[-1]):
-                m = pattern.search(request.url)
-
-                if m:
-                    if ri in self._route_handlers:
-                        self._route_handlers[ri].append((pattern, func, kwargs))
-                    else:
-                        self._route_handlers[ri] = [(pattern, func, kwargs)]
 
-                    await self._handle_continue()
+                # send data
+                write_buffer_size = self._transport.get_write_buffer_size()
 
-                    matches = m.groupdict()
+                if write_buffer_size > self._watermarks['high']:
+                    self._options['logger'].info(
+                        '{:d} exceeds the current watermark limits (high={:d}, low={:d})'.format(write_buffer_size,
+                                                                                                 self._watermarks['high'],
+                                                                                                 self._watermarks['low'])
+                    )
+                    self._timeout_waiters['send'] = self._loop.create_future()
 
-                    if not matches:
-                        matches = m.groups()
+                    await self.set_timeout(self._timeout_waiters['send'], timeout_cb=self.send_timeout)
 
-                    self._server['request'].params['path'] = matches
+                    if self._transport is None:
+                        return
 
-                    await self._handle_response(func, {**kwargs, **options})
-                    del self._route_handlers[-1][i]
-                    return
+                self._transport.write(data)
+            except asyncio.CancelledError:
+                pass
+            except Exception as exc:
+                if self._transport is not None:
+                    self._transport.abort()
+                    self.print_exception(exc)
+
+    def _handle_keepalive(self):
+        for i, task in enumerate(self.tasks):
+            if callable(task):
+                continue
+
+            try:
+                exc = task.exception()
+
+                if exc:
+                    self.print_exception(exc)
+
+                del self.tasks[i]
+            except asyncio.InvalidStateError:
+                pass
+
+        if not self._request.http_continue:
+            self._data = bytearray()
+            self._request.clear_body()
+
+        self._timeout_waiters['keepalive'] = self._loop.create_future()
+
+        self.tasks.append(self._loop.create_task(self.set_timeout(self._timeout_waiters['keepalive'],
+                                                                  timeout=self._options['keepalive_timeout'],
+                                                                  timeout_cb=self.keepalive_timeout)))
+        self._transport.resume_reading()
 
-        # not found
-        await self._handle_response(self._route_handlers[0][1][1], {**self._route_handlers[0][1][2], **options})
+    def connection_lost(self, exc):
+        for task in self.tasks:
+            if callable(task):
+                task()
+                continue
+
+            try:
+                exc = task.exception()
+
+                if exc:
+                    self.print_exception(exc)
+            except asyncio.InvalidStateError:
+                task.cancel()
+
+        self._options['_pool'].put({
+            'queue': (asyncio.Queue(), asyncio.Queue())
+        })
+
+        self._transport = None
+        self._queue = (None, None)
+        self._request = None
+        self._response = None
+        self._data = None
```

### Comparing `tremolo-0.0.95/tremolo/lib/h1parser/parse_header.py` & `tremolo-0.0.96/tremolo/lib/h1parser/parse_header.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.95/tremolo/lib/http_exception.py` & `tremolo-0.0.96/tremolo/lib/http_exception.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.95/tremolo/lib/http_request.py` & `tremolo-0.0.96/tremolo/lib/http_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,36 +2,37 @@
 
 from urllib.parse import parse_qs, parse_qsl
 
 from .http_exception import BadRequest, PayloadTooLarge, RequestTimeout
 from .request import Request
 
 class HTTPRequest(Request):
-    def __init__(self, protocol):
+    def __init__(self, protocol, header):
         super().__init__(protocol)
 
-        self.is_valid = protocol.header.is_valid_request
-        self.headers = protocol.header.headers
-        self.host = protocol.header.gethost()
+        self.header = header
+        self.headers = header.headers
+        self.is_valid = header.is_valid_request
+        self.host = header.gethost()
 
         if isinstance(self.host, list):
             self.host = self.host[0]
 
-        self.method = protocol.header.getmethod().upper()
-        self.url = protocol.header.geturl()
+        self.method = header.getmethod().upper()
+        self.url = header.geturl()
         path_size = self.url.find(b'?')
 
         if path_size == -1:
             self.path = self.url
             self.query_string = b''
         else:
             self.path = self.url[:path_size]
             self.query_string = self.url[path_size + 1:]
 
-        self.version = protocol.header.getversion()
+        self.version = header.getversion()
 
         if self.version != b'1.0':
             self.version = b'1.1'
 
         self._content_length = -1
         self._content_type = b'application/octet-stream'
         self._transfer_encoding = b'none'
@@ -260,15 +261,15 @@
 
                     paused = False
                 else:
                     body = header[header_size + 4:]
                     info = {}
 
                     if header_size <= 8192 and header.startswith(b'--%s\r\n' % boundary):
-                        header = self.protocol.header.parse(header, header_size=header_size).getheaders()
+                        header = self.header.parse(header, header_size=header_size).getheaders()
 
                         if b'content-disposition' in header:
                             for k, v in parse_qsl(header[b'content-disposition']
                                     .replace(b'; ', b'&').replace(b';', b'&').decode(encoding='latin-1')):
                                 info[k] = v.strip('"')
 
                         if b'content-length' in header:
```

### Comparing `tremolo-0.0.95/tremolo/lib/http_response.py` & `tremolo-0.0.96/tremolo/lib/http_response.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.95/tremolo/lib/object_pool.py` & `tremolo-0.0.96/tremolo/lib/object_pool.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 # Copyright (c) 2023 nggit
 
 import asyncio
 
-from .h1parser import ParseHeader
-
 class ObjectPool:
     def __init__(self, pool_size, logger):
         self._pool_size = pool_size
         self._pools = []
         self._logger = logger
 
         for _ in range(pool_size):
             self._pools.append(self._create())
 
     def _create(self):
         return {
-            'header': ParseHeader(),
             'queue': (asyncio.Queue(), asyncio.Queue())
         }
 
     def get(self):
         try:
             return self._pools.pop()
         except IndexError:
```

### Comparing `tremolo-0.0.95/tremolo/lib/request.py` & `tremolo-0.0.96/tremolo/lib/request.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.95/tremolo/lib/response.py` & `tremolo-0.0.96/tremolo/lib/response.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.95/tremolo/tremolo.py` & `tremolo-0.0.96/tremolo/tremolo.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.95/tremolo.egg-info/PKG-INFO` & `tremolo-0.0.96/tremolo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tremolo
-Version: 0.0.95
+Version: 0.0.96
 Summary: Tremolo is a stream-oriented, asynchronous web server/framework written in pure Python
 Home-page: https://github.com/nggit/tremolo
 Author: nggit
 Author-email: contact@anggit.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tremolo-0.0.95/tremolo.egg-info/SOURCES.txt` & `tremolo-0.0.96/tremolo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

