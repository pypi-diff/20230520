# Comparing `tmp/hermescloud-0.0.4.tar.gz` & `tmp/hermescloud-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hermescloud-0.0.4.tar", last modified: Fri May 19 23:42:53 2023, max compression
+gzip compressed data, was "hermescloud-0.0.5.tar", last modified: Sat May 20 10:27:13 2023, max compression
```

## Comparing `hermescloud-0.0.4.tar` & `hermescloud-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 tristan    (501) staff       (20)        0 2023-05-19 23:42:53.640891 hermescloud-0.0.4/
--rw-r--r--   0 tristan    (501) staff       (20)     1064 2023-05-06 23:54:25.000000 hermescloud-0.0.4/LICENSE
--rw-r--r--   0 tristan    (501) staff       (20)    13108 2023-05-19 23:42:53.641444 hermescloud-0.0.4/PKG-INFO
--rw-r--r--   0 tristan    (501) staff       (20)    12570 2023-05-19 22:42:11.000000 hermescloud-0.0.4/README.md
--rw-r--r--   0 tristan    (501) staff       (20)       86 2023-05-06 23:49:25.000000 hermescloud-0.0.4/pyproject.toml
--rw-r--r--   0 tristan    (501) staff       (20)      663 2023-05-19 23:42:53.643008 hermescloud-0.0.4/setup.cfg
-drwxr-xr-x   0 tristan    (501) staff       (20)        0 2023-05-19 23:42:53.622709 hermescloud-0.0.4/src/
-drwxr-xr-x   0 tristan    (501) staff       (20)        0 2023-05-19 23:42:53.634865 hermescloud-0.0.4/src/hermescloud/
--rw-r--r--   0 tristan    (501) staff       (20)       20 2023-05-19 23:39:47.000000 hermescloud-0.0.4/src/hermescloud/__init__.py
--rw-r--r--   0 tristan    (501) staff       (20)     7153 2023-05-19 23:41:32.000000 hermescloud-0.0.4/src/hermescloud/cache.py
--rw-r--r--   0 tristan    (501) staff       (20)      177 2023-05-19 23:15:37.000000 hermescloud-0.0.4/src/hermescloud/utils.py
-drwxr-xr-x   0 tristan    (501) staff       (20)        0 2023-05-19 23:42:53.640231 hermescloud-0.0.4/src/hermescloud.egg-info/
--rw-r--r--   0 tristan    (501) staff       (20)    13108 2023-05-19 23:42:53.000000 hermescloud-0.0.4/src/hermescloud.egg-info/PKG-INFO
--rw-r--r--   0 tristan    (501) staff       (20)      276 2023-05-19 23:42:53.000000 hermescloud-0.0.4/src/hermescloud.egg-info/SOURCES.txt
--rw-r--r--   0 tristan    (501) staff       (20)        1 2023-05-19 23:42:53.000000 hermescloud-0.0.4/src/hermescloud.egg-info/dependency_links.txt
--rw-r--r--   0 tristan    (501) staff       (20)       12 2023-05-19 23:42:53.000000 hermescloud-0.0.4/src/hermescloud.egg-info/top_level.txt
+drwxr-xr-x   0 tristan    (501) staff       (20)        0 2023-05-20 10:27:13.765195 hermescloud-0.0.5/
+-rw-r--r--   0 tristan    (501) staff       (20)     1064 2023-05-06 23:54:25.000000 hermescloud-0.0.5/LICENSE
+-rw-r--r--   0 tristan    (501) staff       (20)    13108 2023-05-20 10:27:13.765621 hermescloud-0.0.5/PKG-INFO
+-rw-r--r--   0 tristan    (501) staff       (20)    12570 2023-05-19 22:42:11.000000 hermescloud-0.0.5/README.md
+-rw-r--r--   0 tristan    (501) staff       (20)       86 2023-05-06 23:49:25.000000 hermescloud-0.0.5/pyproject.toml
+-rw-r--r--   0 tristan    (501) staff       (20)      663 2023-05-20 10:27:13.770496 hermescloud-0.0.5/setup.cfg
+drwxr-xr-x   0 tristan    (501) staff       (20)        0 2023-05-20 10:27:13.745459 hermescloud-0.0.5/src/
+drwxr-xr-x   0 tristan    (501) staff       (20)        0 2023-05-20 10:27:13.756919 hermescloud-0.0.5/src/hermescloud/
+-rw-r--r--   0 tristan    (501) staff       (20)       20 2023-05-19 23:39:47.000000 hermescloud-0.0.5/src/hermescloud/__init__.py
+-rw-r--r--   0 tristan    (501) staff       (20)     8104 2023-05-20 09:58:15.000000 hermescloud-0.0.5/src/hermescloud/cache.py
+-rw-r--r--   0 tristan    (501) staff       (20)      177 2023-05-19 23:15:37.000000 hermescloud-0.0.5/src/hermescloud/utils.py
+drwxr-xr-x   0 tristan    (501) staff       (20)        0 2023-05-20 10:27:13.764349 hermescloud-0.0.5/src/hermescloud.egg-info/
+-rw-r--r--   0 tristan    (501) staff       (20)    13108 2023-05-20 10:27:13.000000 hermescloud-0.0.5/src/hermescloud.egg-info/PKG-INFO
+-rw-r--r--   0 tristan    (501) staff       (20)      276 2023-05-20 10:27:13.000000 hermescloud-0.0.5/src/hermescloud.egg-info/SOURCES.txt
+-rw-r--r--   0 tristan    (501) staff       (20)        1 2023-05-20 10:27:13.000000 hermescloud-0.0.5/src/hermescloud.egg-info/dependency_links.txt
+-rw-r--r--   0 tristan    (501) staff       (20)       12 2023-05-20 10:27:13.000000 hermescloud-0.0.5/src/hermescloud.egg-info/top_level.txt
```

### Comparing `hermescloud-0.0.4/LICENSE` & `hermescloud-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hermescloud-0.0.4/PKG-INFO` & `hermescloud-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hermescloud
-Version: 0.0.4
+Version: 0.0.5
 Summary: Extremely fast full-text-search algorithm and caching system
 Home-page: https://github.com/realTristan/Hermes
 Author: Tristan Simpson
 Author-email: heytristaann@gmail.com
 Project-URL: Bug Tracker, https://github.com/realTristan/Hermes/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hermescloud-0.0.4/README.md` & `hermescloud-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `hermescloud-0.0.4/setup.cfg` & `hermescloud-0.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hermescloud
-version = 0.0.4
+version = 0.0.5
 author = Tristan Simpson
 author_email = heytristaann@gmail.com
 description = Extremely fast full-text-search algorithm and caching system
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/realTristan/Hermes
 project_urls =
```

### Comparing `hermescloud-0.0.4/src/hermescloud/cache.py` & `hermescloud-0.0.5/src/hermescloud/cache.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,218 +17,264 @@
     # Set a value in the cache
     def set(self, key: str, value: dict[str, typing.Any]) -> dict:
         # convert the value to a json string
         json_value: str = json.dumps(value)
         # base64 encode the value
         b64_value: str = Utils.tob64(json_value)
         # send the request
-        self.ws.send(json.dumps({
+        r: int = self.ws.send(json.dumps({
             "function": "cache.set",
             "key": key, 
             "value": b64_value,
         }))
-        return json.loads(self.ws.recv())
+        if r:
+            return json.loads(self.ws.recv())
+        return {}
     
     # Get a value from the cache
     def get(self, key: str) -> dict:
         # send the request
-        self.ws.send(json.dumps({
+        r: int = self.ws.send(json.dumps({
             "function": "cache.get",
             "key": key
         }))
-        return json.loads(self.ws.recv())
+        if r:
+            return json.loads(self.ws.recv())
+        return {}
     
     # Delete a value from the cache
     def delete(self, key: str) -> dict:
         # send the request
-        self.ws.send(json.dumps({
+        r: int = self.ws.send(json.dumps({
             "function": "cache.delete",
             "key": key
         }))
-        return json.loads(self.ws.recv())
+        if r:
+            return json.loads(self.ws.recv())
+        return {}
     
     # Get all keys in the cache
     def keys(self) -> dict:
         # send the request
-        self.ws.send(json.dumps({
+        r: int = self.ws.send(json.dumps({
             "function": "cache.keys"
         }))
-        return json.loads(self.ws.recv())
+        if r:
+            return json.loads(self.ws.recv())
+        return {}
     
     # Get all values in the cache
     def values(self) -> dict:
         # send the request
-        self.ws.send(json.dumps({
+        r: int = self.ws.send(json.dumps({
             "function": "cache.values"
         }))
-        return json.loads(self.ws.recv())
+        if r:
+            return json.loads(self.ws.recv())
+        return {}
     
     # Get the cache length
     def length(self) -> dict:
         # send the request
-        self.ws.send(json.dumps({
+        r: int = self.ws.send(json.dumps({
             "function": "cache.length"
         }))
-        return json.loads(self.ws.recv())
+        if r:
+            return json.loads(self.ws.recv())
+        return {}
     
     # Clear the cache
     def clean(self) -> dict:
         # send the request
-        self.ws.send(json.dumps({
+        r = self.ws.send(json.dumps({
             "function": "cache.clean"
         }))
-        return json.loads(self.ws.recv())
+        if r:
+            return json.loads(self.ws.recv())
+        return {}
     
     # Get the cache info
     def info(self) -> str:
         # send the request
-        self.ws.send(json.dumps({
+        r =  self.ws.send(json.dumps({
             "function": "cache.info"
         }))
-        return self.ws.recv()
+        if r:
+            return self.ws.recv()
+        return ""
     
     # Get cache info for testing
     def info_testing(self) -> str:
         # send the request
-        self.ws.send(json.dumps({
+        r = self.ws.send(json.dumps({
             "function": "cache.info.testing"
         }))
-        return self.ws.recv()
+        if r:
+            return self.ws.recv()
+        return ""
     
     # Check if value exists in the cache
     def exists(self, key: str) -> dict:
         # send the request
-        self.ws.send(json.dumps({
+        r = self.ws.send(json.dumps({
             "function": "cache.exists",
             "key": key
         }))
-        return json.loads(self.ws.recv())
+        if r:
+            return json.loads(self.ws.recv())
+        return {}
     
     # Intialize the full text cache
     def ft_init(self, maxbytes: int, maxlength: int) -> dict:
         # send the request
-        self.ws.send(json.dumps({
+        r = self.ws.send(json.dumps({
             "function": "ft.init",
             "maxbytes": maxbytes,
             "maxlength": maxlength
         }))
-        return json.loads(self.ws.recv())
+        if r:
+            return json.loads(self.ws.recv())
+        return {}
     
     # Clean the full text cache
     def ft_clean(self) -> dict:
         # send the request
-        self.ws.send(json.dumps({
+        r = self.ws.send(json.dumps({
             "function": "ft.clean"
         }))
-        return json.loads(self.ws.recv())
+        if r:
+            return json.loads(self.ws.recv())
+        return {}
     
     # Search the full text cache
     def ft_search(self, query: str, strict: bool, limit: int, schema: dict[str, bool]) -> dict:
         # convert the schema to a json string
         json_schema: str = json.dumps(schema)
         # base64 encode the schema
         b64_schema: str = Utils.tob64(json_schema)
         # send the request
-        self.ws.send(json.dumps({
+        r = self.ws.send(json.dumps({
             "function": "ft.search",
             "query": query,
             "strict": strict,
             "limit": limit,
             "schema": b64_schema
         }))
-        return json.loads(self.ws.recv())
+        if r:
+            return json.loads(self.ws.recv())
+        return {}
     
     # Search one word in the full text cache
     def ft_search_one(self, query: str, strict: bool, limit: int) -> dict:
         # send the request
-        self.ws.send(json.dumps({
+        r = self.ws.send(json.dumps({
             "function": "ft.search.one",
             "query": query,
             "strict": strict,
             "limit": limit
         }))
-        return json.loads(self.ws.recv())
+        if r:
+            return json.loads(self.ws.recv())
+        return {}
     
     # Search value in the full text cache
     def ft_search_values(self, query: str, limit: int, schema: dict[str, bool]) -> dict:
         # convert the schema to a json string
         json_schema: str = json.dumps(schema)
         # base64 encode the schema
         b64_schema: str = Utils.tob64(json_schema)
         # send the request
-        self.ws.send(json.dumps({
+        r = self.ws.send(json.dumps({
             "function": "ft.search.values",
             "query": query,
             "limit": limit,
             "schema": b64_schema
         }))
-        return json.loads(self.ws.recv())
+        if r:
+            return json.loads(self.ws.recv())
+        return {}
     
     # Search values with a key in the full text cache
     def ft_search_with_key(self, query: str, key: str, limit: int) -> dict:
         # send the request
-        self.ws.send(json.dumps({
+        r = self.ws.send(json.dumps({
             "function": "ft.search.withkey",
             "query": query,
             "key": key,
             "limit": limit
         }))
-        return json.loads(self.ws.recv())
+        if r:
+            return json.loads(self.ws.recv())
+        return {}
     
     # Set the max bytes of the full text cache
     def ft_set_max_bytes(self, max_bytes: int) -> dict:
         # send the request
-        self.ws.send(json.dumps({
+        r = self.ws.send(json.dumps({
             "function": "ft.maxbytes.set",
             "maxbytes": max_bytes
         }))
-        return json.loads(self.ws.recv())
+        if r:
+            return json.loads(self.ws.recv())
+        return {}
     
     # Set the max length of the full text storage
     def ft_set_max_length(self, max_length: int) -> dict:
         # send the request
-        self.ws.send(json.dumps({
+        r = self.ws.send(json.dumps({
             "function": "ft.maxlength.set",
             "maxlength": max_length
         }))
-        return json.loads(self.ws.recv())
+        if r:
+            return json.loads(self.ws.recv())
+        return {}
     
     # Get the full text storage
     def ft_storage(self) -> dict:
         # send the request
-        self.ws.send(json.dumps({
+        r = self.ws.send(json.dumps({
             "function": "ft.storage"
         }))
-        return json.loads(self.ws.recv())
+        if r:
+            return json.loads(self.ws.recv())
+        return {}
     
     # Get the full text storage size
     def ft_size(self) -> dict:
         # send the request
-        self.ws.send(json.dumps({
+        r = self.ws.send(json.dumps({
             "function": "ft.storage.size"
         }))
-        return json.loads(self.ws.recv())
+        if r:
+            return json.loads(self.ws.recv())
+        return {}
     
     # Get the full text storage length
     def ft_length(self) -> dict:
         # send the request
-        self.ws.send(json.dumps({
+        r = self.ws.send(json.dumps({
             "function": "ft.storage.length"
         }))
-        return json.loads(self.ws.recv())
+        if r:
+            return json.loads(self.ws.recv())
+        return {}
     
     # Get whether the full text cache is initialized
     def ft_initialized(self) -> dict:
         # send the request
-        self.ws.send(json.dumps({
+        r = self.ws.send(json.dumps({
             "function": "ft.initialized"
         }))
-        return json.loads(self.ws.recv())
+        if r:
+            return json.loads(self.ws.recv())
+        return {}
 
     # Sequence the ft indices
     def ft_sequence(self) -> dict:
         # send the request
-        self.ws.send(json.dumps({
+        r = self.ws.send(json.dumps({
             "function": "ft.indices.sequence"
         }))
-        return json.loads(self.ws.recv())
+        if r:
+            return json.loads(self.ws.recv())
+        return {}
```

### Comparing `hermescloud-0.0.4/src/hermescloud.egg-info/PKG-INFO` & `hermescloud-0.0.5/src/hermescloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hermescloud
-Version: 0.0.4
+Version: 0.0.5
 Summary: Extremely fast full-text-search algorithm and caching system
 Home-page: https://github.com/realTristan/Hermes
 Author: Tristan Simpson
 Author-email: heytristaann@gmail.com
 Project-URL: Bug Tracker, https://github.com/realTristan/Hermes/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

