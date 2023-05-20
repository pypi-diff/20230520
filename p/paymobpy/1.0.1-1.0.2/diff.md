# Comparing `tmp/paymobpy-1.0.1.tar.gz` & `tmp/paymobpy-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paymobpy-1.0.1.tar", last modified: Sat May 20 16:29:55 2023, max compression
+gzip compressed data, was "paymobpy-1.0.2.tar", last modified: Sat May 20 16:51:06 2023, max compression
```

## Comparing `paymobpy-1.0.1.tar` & `paymobpy-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-20 16:29:55.867656 paymobpy-1.0.1/
--rw-r--r--   0 leondaz    (501) staff       (20)      193 2023-05-20 16:29:55.867539 paymobpy-1.0.1/PKG-INFO
--rw-r--r--   0 leondaz    (501) staff       (20)      113 2023-05-20 16:29:46.000000 paymobpy-1.0.1/README.md
-drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-20 16:29:55.866955 paymobpy-1.0.1/paymobpy/
--rw-r--r--   0 leondaz    (501) staff       (20)     2441 2023-05-20 15:53:26.000000 paymobpy-1.0.1/paymobpy/__init__.py
--rw-r--r--   0 leondaz    (501) staff       (20)      177 2023-05-20 14:43:04.000000 paymobpy-1.0.1/paymobpy/consts.py
--rw-r--r--   0 leondaz    (501) staff       (20)      281 2023-05-20 15:20:58.000000 paymobpy-1.0.1/paymobpy/exceptions.py
--rw-r--r--   0 leondaz    (501) staff       (20)      825 2023-05-20 15:26:08.000000 paymobpy-1.0.1/paymobpy/http_clients.py
--rw-r--r--   0 leondaz    (501) staff       (20)     2493 2023-05-20 16:19:48.000000 paymobpy-1.0.1/paymobpy/schemas.py
-drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-20 16:29:55.867397 paymobpy-1.0.1/paymobpy.egg-info/
--rw-r--r--   0 leondaz    (501) staff       (20)      193 2023-05-20 16:29:55.000000 paymobpy-1.0.1/paymobpy.egg-info/PKG-INFO
--rw-r--r--   0 leondaz    (501) staff       (20)      254 2023-05-20 16:29:55.000000 paymobpy-1.0.1/paymobpy.egg-info/SOURCES.txt
--rw-r--r--   0 leondaz    (501) staff       (20)        1 2023-05-20 16:29:55.000000 paymobpy-1.0.1/paymobpy.egg-info/dependency_links.txt
--rw-r--r--   0 leondaz    (501) staff       (20)        9 2023-05-20 16:29:55.000000 paymobpy-1.0.1/paymobpy.egg-info/top_level.txt
--rw-r--r--   0 leondaz    (501) staff       (20)       38 2023-05-20 16:29:55.867693 paymobpy-1.0.1/setup.cfg
--rw-r--r--   0 leondaz    (501) staff       (20)      275 2023-05-20 16:29:34.000000 paymobpy-1.0.1/setup.py
+drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-20 16:51:06.565174 paymobpy-1.0.2/
+-rw-r--r--   0 leondaz    (501) staff       (20)      193 2023-05-20 16:51:06.565052 paymobpy-1.0.2/PKG-INFO
+-rw-r--r--   0 leondaz    (501) staff       (20)      777 2023-05-20 16:49:04.000000 paymobpy-1.0.2/README.md
+drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-20 16:51:06.564361 paymobpy-1.0.2/paymobpy/
+-rw-r--r--   0 leondaz    (501) staff       (20)     2518 2023-05-20 16:49:46.000000 paymobpy-1.0.2/paymobpy/__init__.py
+-rw-r--r--   0 leondaz    (501) staff       (20)      177 2023-05-20 14:43:04.000000 paymobpy-1.0.2/paymobpy/consts.py
+-rw-r--r--   0 leondaz    (501) staff       (20)      281 2023-05-20 15:20:58.000000 paymobpy-1.0.2/paymobpy/exceptions.py
+-rw-r--r--   0 leondaz    (501) staff       (20)      825 2023-05-20 15:26:08.000000 paymobpy-1.0.2/paymobpy/http_clients.py
+-rw-r--r--   0 leondaz    (501) staff       (20)     2493 2023-05-20 16:19:48.000000 paymobpy-1.0.2/paymobpy/schemas.py
+drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-20 16:51:06.564915 paymobpy-1.0.2/paymobpy.egg-info/
+-rw-r--r--   0 leondaz    (501) staff       (20)      193 2023-05-20 16:51:06.000000 paymobpy-1.0.2/paymobpy.egg-info/PKG-INFO
+-rw-r--r--   0 leondaz    (501) staff       (20)      254 2023-05-20 16:51:06.000000 paymobpy-1.0.2/paymobpy.egg-info/SOURCES.txt
+-rw-r--r--   0 leondaz    (501) staff       (20)        1 2023-05-20 16:51:06.000000 paymobpy-1.0.2/paymobpy.egg-info/dependency_links.txt
+-rw-r--r--   0 leondaz    (501) staff       (20)        9 2023-05-20 16:51:06.000000 paymobpy-1.0.2/paymobpy.egg-info/top_level.txt
+-rw-r--r--   0 leondaz    (501) staff       (20)       38 2023-05-20 16:51:06.565212 paymobpy-1.0.2/setup.cfg
+-rw-r--r--   0 leondaz    (501) staff       (20)      275 2023-05-20 16:50:50.000000 paymobpy-1.0.2/setup.py
```

### Comparing `paymobpy-1.0.1/paymobpy/__init__.py` & `paymobpy-1.0.2/paymobpy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,13 +76,16 @@
                 "integration_id": integration_id,
                 **data.dict(),
             },
         )
 
         return response.json()
 
+    async def close_connection(self):
+        await self._client.aclose()
+
     async def __aenter__(self):
         await self.authenticate()
         return self
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
-        await self._client.aclose()
+        await self.close_connection()
```

### Comparing `paymobpy-1.0.1/paymobpy/http_clients.py` & `paymobpy-1.0.2/paymobpy/http_clients.py`

 * *Files identical despite different names*

### Comparing `paymobpy-1.0.1/paymobpy/schemas.py` & `paymobpy-1.0.2/paymobpy/schemas.py`

 * *Files identical despite different names*

