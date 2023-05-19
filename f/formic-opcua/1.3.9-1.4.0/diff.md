# Comparing `tmp/formic_opcua-1.3.9.tar.gz` & `tmp/formic_opcua-1.4.0.tar.gz`

## Comparing `formic_opcua-1.3.9.tar` & `formic_opcua-1.4.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 formic_opcua-1.3.9/.pre-commit-config.yaml
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 formic_opcua-1.3.9/README.md
--rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 formic_opcua-1.3.9/examples/opcua_client.py
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 formic_opcua-1.3.9/examples/example_configs/opcua_config.yaml
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 formic_opcua-1.3.9/examples/example_configs/opcua_config_1.yaml
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 formic_opcua-1.3.9/examples/example_configs/opcua_config_2.yaml
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 formic_opcua-1.3.9/examples/example_configs/opcua_config_3.yaml
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 formic_opcua-1.3.9/examples/example_configs/opcua_config_4.yaml
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 formic_opcua-1.3.9/examples/example_configs/opcua_config_5.yaml
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 formic_opcua-1.3.9/formic_opcua/__init__.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 formic_opcua-1.3.9/formic_opcua/client/__init__.py
--rw-r--r--   0        0        0    11780 2020-02-02 00:00:00.000000 formic_opcua-1.3.9/formic_opcua/client/async_opcua_client.py
--rw-r--r--   0        0        0    10544 2020-02-02 00:00:00.000000 formic_opcua-1.3.9/formic_opcua/client/opcua_client.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 formic_opcua-1.3.9/formic_opcua/core/__init__.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 formic_opcua-1.3.9/formic_opcua/core/exceptions.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 formic_opcua-1.3.9/formic_opcua/core/parse.py
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 formic_opcua-1.3.9/formic_opcua/core/type_conversions.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 formic_opcua-1.3.9/formic_opcua/scripts/__init__.py
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 formic_opcua-1.3.9/formic_opcua/scripts/formic_opcua_client.py
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 formic_opcua-1.3.9/formic_opcua/scripts/formic_opcua_server.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 formic_opcua-1.3.9/formic_opcua/server/__init__.py
--rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 formic_opcua-1.3.9/formic_opcua/server/opcua_server.py
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 formic_opcua-1.3.9/hooks/add_issue_prefix.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 formic_opcua-1.3.9/tests/__init__.py
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 formic_opcua-1.3.9/tests/test_server_config.py
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 formic_opcua-1.3.9/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 formic_opcua-1.3.9/pyproject.toml
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 formic_opcua-1.3.9/PKG-INFO
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 formic_opcua-1.4.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 formic_opcua-1.4.0/README.md
+-rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 formic_opcua-1.4.0/examples/opcua_client.py
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 formic_opcua-1.4.0/examples/example_configs/opcua_config.yaml
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 formic_opcua-1.4.0/examples/example_configs/opcua_config_1.yaml
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 formic_opcua-1.4.0/examples/example_configs/opcua_config_2.yaml
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 formic_opcua-1.4.0/examples/example_configs/opcua_config_3.yaml
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 formic_opcua-1.4.0/examples/example_configs/opcua_config_4.yaml
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 formic_opcua-1.4.0/examples/example_configs/opcua_config_5.yaml
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 formic_opcua-1.4.0/formic_opcua/__init__.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 formic_opcua-1.4.0/formic_opcua/client/__init__.py
+-rw-r--r--   0        0        0    12221 2020-02-02 00:00:00.000000 formic_opcua-1.4.0/formic_opcua/client/async_opcua_client.py
+-rw-r--r--   0        0        0    10544 2020-02-02 00:00:00.000000 formic_opcua-1.4.0/formic_opcua/client/opcua_client.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 formic_opcua-1.4.0/formic_opcua/core/__init__.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 formic_opcua-1.4.0/formic_opcua/core/exceptions.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 formic_opcua-1.4.0/formic_opcua/core/parse.py
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 formic_opcua-1.4.0/formic_opcua/core/type_conversions.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 formic_opcua-1.4.0/formic_opcua/scripts/__init__.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 formic_opcua-1.4.0/formic_opcua/scripts/formic_opcua_client.py
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 formic_opcua-1.4.0/formic_opcua/scripts/formic_opcua_server.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 formic_opcua-1.4.0/formic_opcua/server/__init__.py
+-rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 formic_opcua-1.4.0/formic_opcua/server/opcua_server.py
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 formic_opcua-1.4.0/hooks/add_issue_prefix.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 formic_opcua-1.4.0/tests/__init__.py
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 formic_opcua-1.4.0/tests/test_server_config.py
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 formic_opcua-1.4.0/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 formic_opcua-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 formic_opcua-1.4.0/PKG-INFO
```

### Comparing `formic_opcua-1.3.9/.pre-commit-config.yaml` & `formic_opcua-1.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.3.9/examples/opcua_client.py` & `formic_opcua-1.4.0/examples/opcua_client.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.3.9/examples/example_configs/opcua_config.yaml` & `formic_opcua-1.4.0/examples/example_configs/opcua_config.yaml`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.3.9/examples/example_configs/opcua_config_1.yaml` & `formic_opcua-1.4.0/examples/example_configs/opcua_config_1.yaml`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.3.9/examples/example_configs/opcua_config_2.yaml` & `formic_opcua-1.4.0/examples/example_configs/opcua_config_2.yaml`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.3.9/formic_opcua/client/async_opcua_client.py` & `formic_opcua-1.4.0/formic_opcua/client/async_opcua_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,19 +20,21 @@
     CONNECTED = 0
     CONNECTING = 1
     DISCONNECTED = 2
 
 
 class AsyncOpcuaClient:
     def __init__(
-        self,
-        server_config_file: str = None,
-        connect_timeout: float = 0.5,
-        url: str = None,
-        uri: str = None,
+            self,
+            server_config_file: str = None,
+            connect_timeout: float = .5,
+            url: str = None,
+            uri: str = None,
+            username: str = None,
+            password: str = None,
     ) -> None:
         if server_config_file is None and (url is None and uri is None):
             error_message = 'No configuration arguments passed to client.'
             logger.critical(error_message)
             raise InvalidClientArgsError(error_message)
 
         if server_config_file is not None and (url is not None or uri is not None):
@@ -53,14 +55,22 @@
         else:
             self._url = url
             self._uri = uri
 
         self._idx = -1
         self._node_path_list: List[str] = []
         self._client = Client(url=self._url)
+
+        self._username = None
+        self._password = None
+
+        if username is not None and password is not None:
+            self._username = username
+            self._password = password
+
         self.connect_timeout = connect_timeout
         self._connection_status = ConnectionStatus.DISCONNECTED
         self._node_map: Dict[str, Tuple] = {}
 
         logger.info(f'Client created with url: {self._url}, and uri: {self._uri}')
 
     async def __aenter__(self):
@@ -78,14 +88,18 @@
         try:
             # if await self._test_server_connection():
             #     logger.info('_connect called but there is a connection to the server.')
             #     self._connection_status =
             #     return
             if await self._disconnect():
                 self._client = Client(url=self._url, timeout=self.connect_timeout)
+                if self._username is not None and self._password is not None:
+                    self._client.set_user(self._username)
+                    self._client.set_password(self._password)
+
             logger.info('Connecting...')
             await self._client.connect()
             logger.info('Connected...')
         except (ConnectionRefusedError, ConnectionError, RuntimeError, RuntimeWarning, TimeoutError):
             logger.error(
                 f'Unable to connect to server. Client expects server to have url: {self._url} and uri: {self._uri}. '
                 f'Server is not running or the configs are not matched with client.'
@@ -110,16 +124,16 @@
         except Exception as e:
             logger.error(f'Unhandled exception while to disconnecting from server. {e} ')
             return False
 
     async def _dfs_mapper(self, node: Node, path: str) -> None:
         browse_path = await node.read_browse_name()
 
-        if browse_path.NamespaceIndex != self._idx and browse_path.NamespaceIndex != 0:
-            return
+        # if browse_path.NamespaceIndex != self._idx and browse_path.NamespaceIndex != 0:
+        #     return
 
         node_class = await node.read_node_class()
         path_to_node = path + '/' + browse_path.Name
 
         # if node_class == NodeClass.Variable and browse_path.NamespaceIndex == self._idx:
         if node_class == NodeClass.Variable:
             # Remove "/Objects/" since this client is intended for reading only custom nodes
@@ -262,19 +276,20 @@
         await asyncio.gather(*future_results.values())
 
         for path, task in future_results.items():
             task_value = task.result()
 
             if task_value is not None:
                 logger.info(f'Successfully read value: {task_value} for path: {path}')
+                results[path] = task_value
             else:
-                # This could happens if there is a disconnect during reading
                 logger.warning(f'Unsuccessful read attempt for path {path}')
-                self._connection_status = ConnectionStatus.DISCONNECTED
-            results[path] = task_value
+
+        if len(results) == 0:
+            self._connection_status = ConnectionStatus.DISCONNECTED
 
         logger.info(f'{results}')
         return results
 
     def identifier_from_string(self, path: str) -> List[str]:
         identifier = [f'{self._idx}:{path_part}' for path_part in path.split('/')]
         return ['0:Objects'] + identifier
```

### Comparing `formic_opcua-1.3.9/formic_opcua/client/opcua_client.py` & `formic_opcua-1.4.0/formic_opcua/client/opcua_client.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.3.9/formic_opcua/core/parse.py` & `formic_opcua-1.4.0/formic_opcua/core/parse.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.3.9/formic_opcua/core/type_conversions.py` & `formic_opcua-1.4.0/formic_opcua/core/type_conversions.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.3.9/formic_opcua/scripts/formic_opcua_client.py` & `formic_opcua-1.4.0/formic_opcua/scripts/formic_opcua_client.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.3.9/formic_opcua/scripts/formic_opcua_server.py` & `formic_opcua-1.4.0/formic_opcua/scripts/formic_opcua_server.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.3.9/formic_opcua/server/opcua_server.py` & `formic_opcua-1.4.0/formic_opcua/server/opcua_server.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.3.9/hooks/add_issue_prefix.py` & `formic_opcua-1.4.0/hooks/add_issue_prefix.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.3.9/tests/test_server_config.py` & `formic_opcua-1.4.0/tests/test_server_config.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.3.9/.gitignore` & `formic_opcua-1.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.3.9/pyproject.toml` & `formic_opcua-1.4.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ['hatchling']
 build-backend = 'hatchling.build'
 
 [project]
 name = 'formic_opcua'
 requires-python = ">=3.8"
-version = "1.3.9"
+version = "1.4.0"
 authors = [
     {name = "Spencer White", email = "swhite@formic.co"},
     {name = "Damian Stempel"},
     {name = "Viachaslau Zakharchuk"}
 
 ]
 dependencies = [
```

