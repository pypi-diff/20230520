# Comparing `tmp/bosch-control-panel-cc880p-3.1.1.tar.gz` & `tmp/bosch-control-panel-cc880p-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bosch-control-panel-cc880p-3.1.1.tar", last modified: Sat May 20 12:35:47 2023, max compression
+gzip compressed data, was "bosch-control-panel-cc880p-3.1.2.tar", last modified: Sat May 20 15:46:23 2023, max compression
```

## Comparing `bosch-control-panel-cc880p-3.1.1.tar` & `bosch-control-panel-cc880p-3.1.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:35:47.373360 bosch-control-panel-cc880p-3.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-05-20 12:35:33.000000 bosch-control-panel-cc880p-3.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21111 2023-05-20 12:35:47.373360 bosch-control-panel-cc880p-3.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20428 2023-05-20 12:35:33.000000 bosch-control-panel-cc880p-3.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-20 12:35:33.000000 bosch-control-panel-cc880p-3.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-20 12:35:47.373360 bosch-control-panel-cc880p-3.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:35:47.369360 bosch-control-panel-cc880p-3.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:35:47.369360 bosch-control-panel-cc880p-3.1.1/src/bosch/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:35:47.369360 bosch-control-panel-cc880p-3.1.1/src/bosch/control_panel/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:35:47.373360 bosch-control-panel-cc880p-3.1.1/src/bosch/control_panel/cc880p/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 12:35:33.000000 bosch-control-panel-cc880p-3.1.1/src/bosch/control_panel/cc880p/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:35:47.373360 bosch-control-panel-cc880p-3.1.1/src/bosch/control_panel/cc880p/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 12:35:33.000000 bosch-control-panel-cc880p-3.1.1/src/bosch/control_panel/cc880p/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-05-20 12:35:33.000000 bosch-control-panel-cc880p-3.1.1/src/bosch/control_panel/cc880p/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-20 12:35:33.000000 bosch-control-panel-cc880p-3.1.1/src/bosch/control_panel/cc880p/cli/cmds.py
--rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-05-20 12:35:33.000000 bosch-control-panel-cc880p-3.1.1/src/bosch/control_panel/cc880p/cli/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    18509 2023-05-20 12:35:33.000000 bosch-control-panel-cc880p-3.1.1/src/bosch/control_panel/cc880p/cp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:35:47.373360 bosch-control-panel-cc880p-3.1.1/src/bosch/control_panel/cc880p/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 12:35:33.000000 bosch-control-panel-cc880p-3.1.1/src/bosch/control_panel/cc880p/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-20 12:35:33.000000 bosch-control-panel-cc880p-3.1.1/src/bosch/control_panel/cc880p/models/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-20 12:35:33.000000 bosch-control-panel-cc880p-3.1.1/src/bosch/control_panel/cc880p/models/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-20 12:35:33.000000 bosch-control-panel-cc880p-3.1.1/src/bosch/control_panel/cc880p/models/cp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-05-20 12:35:33.000000 bosch-control-panel-cc880p-3.1.1/src/bosch/control_panel/cc880p/models/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-05-20 12:35:33.000000 bosch-control-panel-cc880p-3.1.1/src/bosch/control_panel/cc880p/models/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-20 12:35:33.000000 bosch-control-panel-cc880p-3.1.1/src/bosch/control_panel/cc880p/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-20 12:35:33.000000 bosch-control-panel-cc880p-3.1.1/src/bosch/control_panel/cc880p/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:35:47.373360 bosch-control-panel-cc880p-3.1.1/src/bosch_control_panel_cc880p.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21111 2023-05-20 12:35:47.000000 bosch-control-panel-cc880p-3.1.1/src/bosch_control_panel_cc880p.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-20 12:35:47.000000 bosch-control-panel-cc880p-3.1.1/src/bosch_control_panel_cc880p.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 12:35:47.000000 bosch-control-panel-cc880p-3.1.1/src/bosch_control_panel_cc880p.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-20 12:35:47.000000 bosch-control-panel-cc880p-3.1.1/src/bosch_control_panel_cc880p.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-20 12:35:47.000000 bosch-control-panel-cc880p-3.1.1/src/bosch_control_panel_cc880p.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-20 12:35:47.000000 bosch-control-panel-cc880p-3.1.1/src/bosch_control_panel_cc880p.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 15:46:23.563196 bosch-control-panel-cc880p-3.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-05-20 15:46:11.000000 bosch-control-panel-cc880p-3.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21111 2023-05-20 15:46:23.563196 bosch-control-panel-cc880p-3.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20428 2023-05-20 15:46:11.000000 bosch-control-panel-cc880p-3.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-20 15:46:11.000000 bosch-control-panel-cc880p-3.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-20 15:46:23.563196 bosch-control-panel-cc880p-3.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 15:46:23.559196 bosch-control-panel-cc880p-3.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 15:46:23.555196 bosch-control-panel-cc880p-3.1.2/src/bosch/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 15:46:23.555196 bosch-control-panel-cc880p-3.1.2/src/bosch/control_panel/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 15:46:23.559196 bosch-control-panel-cc880p-3.1.2/src/bosch/control_panel/cc880p/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 15:46:11.000000 bosch-control-panel-cc880p-3.1.2/src/bosch/control_panel/cc880p/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 15:46:23.559196 bosch-control-panel-cc880p-3.1.2/src/bosch/control_panel/cc880p/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 15:46:11.000000 bosch-control-panel-cc880p-3.1.2/src/bosch/control_panel/cc880p/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-05-20 15:46:11.000000 bosch-control-panel-cc880p-3.1.2/src/bosch/control_panel/cc880p/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-20 15:46:11.000000 bosch-control-panel-cc880p-3.1.2/src/bosch/control_panel/cc880p/cli/cmds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-05-20 15:46:11.000000 bosch-control-panel-cc880p-3.1.2/src/bosch/control_panel/cc880p/cli/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18830 2023-05-20 15:46:11.000000 bosch-control-panel-cc880p-3.1.2/src/bosch/control_panel/cc880p/cp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 15:46:23.559196 bosch-control-panel-cc880p-3.1.2/src/bosch/control_panel/cc880p/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 15:46:11.000000 bosch-control-panel-cc880p-3.1.2/src/bosch/control_panel/cc880p/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-20 15:46:11.000000 bosch-control-panel-cc880p-3.1.2/src/bosch/control_panel/cc880p/models/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-20 15:46:11.000000 bosch-control-panel-cc880p-3.1.2/src/bosch/control_panel/cc880p/models/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-20 15:46:11.000000 bosch-control-panel-cc880p-3.1.2/src/bosch/control_panel/cc880p/models/cp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-05-20 15:46:11.000000 bosch-control-panel-cc880p-3.1.2/src/bosch/control_panel/cc880p/models/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-05-20 15:46:11.000000 bosch-control-panel-cc880p-3.1.2/src/bosch/control_panel/cc880p/models/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-20 15:46:11.000000 bosch-control-panel-cc880p-3.1.2/src/bosch/control_panel/cc880p/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-20 15:46:11.000000 bosch-control-panel-cc880p-3.1.2/src/bosch/control_panel/cc880p/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 15:46:23.563196 bosch-control-panel-cc880p-3.1.2/src/bosch_control_panel_cc880p.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21111 2023-05-20 15:46:23.000000 bosch-control-panel-cc880p-3.1.2/src/bosch_control_panel_cc880p.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-20 15:46:23.000000 bosch-control-panel-cc880p-3.1.2/src/bosch_control_panel_cc880p.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 15:46:23.000000 bosch-control-panel-cc880p-3.1.2/src/bosch_control_panel_cc880p.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-20 15:46:23.000000 bosch-control-panel-cc880p-3.1.2/src/bosch_control_panel_cc880p.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-20 15:46:23.000000 bosch-control-panel-cc880p-3.1.2/src/bosch_control_panel_cc880p.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-20 15:46:23.000000 bosch-control-panel-cc880p-3.1.2/src/bosch_control_panel_cc880p.egg-info/top_level.txt
```

### Comparing `bosch-control-panel-cc880p-3.1.1/LICENSE` & `bosch-control-panel-cc880p-3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bosch-control-panel-cc880p-3.1.1/PKG-INFO` & `bosch-control-panel-cc880p-3.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bosch-control-panel-cc880p
-Version: 3.1.1
+Version: 3.1.2
 Summary: Library to interface with the old CC880p Bosch COntrol Panels
 Home-page: https://github.com/hgomes88/bosch-control-panel-cc880p
 Author: Hugo Gomes
 Author-email: hgomes88@gmail.com
 Project-URL: Tracker, https://github.com/hgomes88/bosch-control-panel-cc880p/issues
 Project-URL: Download, https://pypi.org/project/bosch-control-panel-cc880p/
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bosch-control-panel-cc880p Version: 3.1.1 Summary:
+Metadata-Version: 2.1 Name: bosch-control-panel-cc880p Version: 3.1.2 Summary:
 Library to interface with the old CC880p Bosch COntrol Panels Home-page: https:
 //github.com/hgomes88/bosch-control-panel-cc880p Author: Hugo Gomes Author-
 email: hgomes88@gmail.com Project-URL: Tracker, https://github.com/hgomes88/
 bosch-control-panel-cc880p/issues Project-URL: Download, https://pypi.org/
 project/bosch-control-panel-cc880p/ Classifier: Programming Language :: Python
 :: 3 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.8 Description-Content-
```

### Comparing `bosch-control-panel-cc880p-3.1.1/README.md` & `bosch-control-panel-cc880p-3.1.2/README.md`

 * *Files identical despite different names*

### Comparing `bosch-control-panel-cc880p-3.1.1/setup.cfg` & `bosch-control-panel-cc880p-3.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `bosch-control-panel-cc880p-3.1.1/src/bosch/control_panel/cc880p/cli/cli.py` & `bosch-control-panel-cc880p-3.1.2/src/bosch/control_panel/cc880p/cli/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,20 +50,26 @@
         print(f'Control Panel availability is: {cp}')
     elif isinstance(cp, Time):
         print(f'Control Panel time is: {cp}')
 
     return True
 
 
+async def _wait_for_connection(cp: CP):
+    while not cp.connected:
+        await asyncio.sleep(1.0)
+
+
 async def run_listen_mode(cp: CP):
     """Run the control panel in listen mode."""
     cp.add_data_listener(data_listener)
     cp.add_control_panel_listener(cp_listener)
     while True:
         try:
+            await asyncio.wait_for(_wait_for_connection(cp), timeout=3.0)
             await cp.get_status()
         except BaseException:
             logging.exception('Error:')
         finally:
             await asyncio.sleep(1)
```

### Comparing `bosch-control-panel-cc880p-3.1.1/src/bosch/control_panel/cc880p/cli/cmds.py` & `bosch-control-panel-cc880p-3.1.2/src/bosch/control_panel/cc880p/cli/cmds.py`

 * *Files identical despite different names*

### Comparing `bosch-control-panel-cc880p-3.1.1/src/bosch/control_panel/cc880p/cli/parser.py` & `bosch-control-panel-cc880p-3.1.2/src/bosch/control_panel/cc880p/cli/parser.py`

 * *Files identical despite different names*

### Comparing `bosch-control-panel-cc880p-3.1.1/src/bosch/control_panel/cc880p/cp.py` & `bosch-control-panel-cc880p-3.1.2/src/bosch/control_panel/cc880p/cp.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         # Streamreader
         self._reader: Optional[asyncio.StreamReader] = None
         # Streamwriter
         self._writer: Optional[asyncio.StreamWriter] = None
         # Connected
         self._connected: bool = False
         # Reconnection task
-        self._reconnection_task: Optional[Task] = None
+        self._conn_task: Optional[Task] = None
 
         # Lock
         self._lock = asyncio.Lock()
 
         # Listeners to be called whenever the control panel state is changed
         self._control_panel_listeners: List[ControlPanelListener] = []
         # Listeners to be called whenever the there's new data
@@ -117,26 +117,20 @@
     @property
     def connected(self) -> bool:
         """Report whether the connection to the alarm is established."""
         return self._connected
 
     async def start(self) -> 'CP':
         """Establish the connection to the control panel."""
-        # Open the connection to the control panel
-        await self._connect()
-        self._reconnection_task = asyncio.create_task(self._reconnection())
+        await self._start_connection_task()
         return self
 
     async def stop(self) -> 'CP':
         """Stop the connection to the control panel."""
-        if self._reconnection_task:
-            self._reconnection_task.cancel()
-            self._reconnection_task = None
-        async with self._lock:
-            await self._close_connection()
+        await self._stop_connection_task()
         return self
 
     def add_control_panel_listener(self, listener: ControlPanelListener):
         """Add a listener function to listen for any change in the alarm."""
         self._control_panel_listeners.append(listener)
 
     def add_data_listener(self, listener: DataListener):
@@ -242,44 +236,50 @@
             bytes:
                 Response of the message sent to the control panel or None
                 otherwise
         """
         resp = None
         available = False
 
-        async with self._lock:
-            try:
-                resp = await self._send(message, n_resp_bytes, timeout)
-            except asyncio.exceptions.TimeoutError:
-                _LOGGER.warning('Message not received on time')
-                await self._close_connection()
-                raise
-            except asyncio.IncompleteReadError:
-                _LOGGER.warning('Message not received.')
-                raise
-            except EOFError:
-                _LOGGER.warning('Connection EOF')
-                raise
-            except (OSError):
-                _LOGGER.warning('Connection failed')
-                await self._close_connection()
-                raise
-            except BaseException as ex:
-                _LOGGER.warning('Unexpected Error: %s', ex)
-                raise
-            else:
-                available = True
-                return resp
-            finally:
-                if self.control_panel.availability.available != available:
-                    self.control_panel.availability.available = available
-                    for listener in self._control_panel_listeners:
-                        asyncio.create_task(
-                            listener(0, self.control_panel.availability)
-                        )
+        if self.connected:
+            async with self._lock:
+                try:
+                    resp = await self._send(message, n_resp_bytes, timeout)
+                except asyncio.exceptions.TimeoutError:
+                    _LOGGER.warning('Message not received on time')
+                    raise
+                except asyncio.IncompleteReadError:
+                    _LOGGER.warning('Message not received.')
+                    raise
+                except EOFError:
+                    _LOGGER.warning('Connection EOF')
+                    raise
+                except (OSError):
+                    _LOGGER.warning('Connection failed')
+                    await self._close_connection()
+                    raise
+                except BaseException as ex:
+                    _LOGGER.warning('Unexpected Error: %s', ex)
+                    raise
+                else:
+                    available = True
+                    return resp
+                finally:
+                    await self._update_availability(available)
+        else:
+            await self._update_availability(available)
+            raise ConnectionError('Not Connected')
+
+    async def _update_availability(self, available: bool = True):
+        if self.control_panel.availability.available != available:
+            self.control_panel.availability.available = available
+            for listener in self._control_panel_listeners:
+                asyncio.create_task(
+                    listener(0, self.control_panel.availability)
+                )
 
     async def _connect(self):
         async with self._lock:
             _LOGGER.info('Connecting to control panel...')
             try:
                 await self._close_connection()
                 await self._open_connection()
@@ -351,15 +351,15 @@
                     )
                 if not data:
                     raise asyncio.IncompleteReadError(data, 32)
                 return data
             else:
                 raise EOFError()
         else:
-            raise ConnectionError('Connection not established')
+            raise ConnectionError('Not Connected')
 
     def _encode_key(self, key: str) -> int:
         # Is a number between 0 and 9
         if key.isdigit() and int(key) in range(0, 10):
             return int(key)
         elif key == '*':
             return 0x1B
@@ -392,15 +392,15 @@
 
             if self._is_status_msg(data):
                 self._handle_status_msg(data)
 
             for listener in self._data_listeners:
                 asyncio.create_task(listener(data))
         else:
-            _LOGGER.warn('No Data Received!!!')
+            _LOGGER.warning('No Data Received!!!')
 
     @classmethod
     def _is_status_msg(cls, data: bytes):
 
         if bytes([data[0]]) != bytes.fromhex(StatusResponse.code):
             return False
 
@@ -513,17 +513,27 @@
             self._control_panel.time.time = time
 
             for listener in self._control_panel_listeners:
                 asyncio.create_task(listener(0, self._control_panel.time))
 
             _LOGGER.info('Time updated %s', self._control_panel.time)
 
-    async def _reconnection(self):
+    async def _start_connection_task(self):
+        self._conn_task = asyncio.create_task(self._connection_task())
+
+    async def _stop_connection_task(self):
+        if self._conn_task:
+            self._conn_task.cancel()
+            self._conn_task = None
+        async with self._lock:
+            await self._close_connection()
+
+    async def _connection_task(self):
         while True:
             try:
                 if not self.connected:
-                    _LOGGER.info('Reconnecting')
+                    _LOGGER.info('Connecting')
                     await self._connect()
             except BaseException:
-                _LOGGER.error('Reconnection failed')
+                _LOGGER.error('Connection failed')
             finally:
                 await asyncio.sleep(3)
```

### Comparing `bosch-control-panel-cc880p-3.1.1/src/bosch/control_panel/cc880p/models/cp.py` & `bosch-control-panel-cc880p-3.1.2/src/bosch/control_panel/cc880p/models/cp.py`

 * *Files identical despite different names*

### Comparing `bosch-control-panel-cc880p-3.1.1/src/bosch/control_panel/cc880p/models/requests.py` & `bosch-control-panel-cc880p-3.1.2/src/bosch/control_panel/cc880p/models/requests.py`

 * *Files identical despite different names*

### Comparing `bosch-control-panel-cc880p-3.1.1/src/bosch/control_panel/cc880p/models/responses.py` & `bosch-control-panel-cc880p-3.1.2/src/bosch/control_panel/cc880p/models/responses.py`

 * *Files identical despite different names*

### Comparing `bosch-control-panel-cc880p-3.1.1/src/bosch/control_panel/cc880p/utils.py` & `bosch-control-panel-cc880p-3.1.2/src/bosch/control_panel/cc880p/utils.py`

 * *Files identical despite different names*

### Comparing `bosch-control-panel-cc880p-3.1.1/src/bosch_control_panel_cc880p.egg-info/PKG-INFO` & `bosch-control-panel-cc880p-3.1.2/src/bosch_control_panel_cc880p.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bosch-control-panel-cc880p
-Version: 3.1.1
+Version: 3.1.2
 Summary: Library to interface with the old CC880p Bosch COntrol Panels
 Home-page: https://github.com/hgomes88/bosch-control-panel-cc880p
 Author: Hugo Gomes
 Author-email: hgomes88@gmail.com
 Project-URL: Tracker, https://github.com/hgomes88/bosch-control-panel-cc880p/issues
 Project-URL: Download, https://pypi.org/project/bosch-control-panel-cc880p/
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bosch-control-panel-cc880p Version: 3.1.1 Summary:
+Metadata-Version: 2.1 Name: bosch-control-panel-cc880p Version: 3.1.2 Summary:
 Library to interface with the old CC880p Bosch COntrol Panels Home-page: https:
 //github.com/hgomes88/bosch-control-panel-cc880p Author: Hugo Gomes Author-
 email: hgomes88@gmail.com Project-URL: Tracker, https://github.com/hgomes88/
 bosch-control-panel-cc880p/issues Project-URL: Download, https://pypi.org/
 project/bosch-control-panel-cc880p/ Classifier: Programming Language :: Python
 :: 3 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.8 Description-Content-
```

### Comparing `bosch-control-panel-cc880p-3.1.1/src/bosch_control_panel_cc880p.egg-info/SOURCES.txt` & `bosch-control-panel-cc880p-3.1.2/src/bosch_control_panel_cc880p.egg-info/SOURCES.txt`

 * *Files identical despite different names*

