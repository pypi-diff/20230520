# Comparing `tmp/audiconnectpy-1.3.9.tar.gz` & `tmp/audiconnectpy-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiconnectpy-1.3.9.tar", last modified: Sat May 20 13:41:46 2023, max compression
+gzip compressed data, was "audiconnectpy-1.4.0.tar", last modified: Sat May 20 14:13:59 2023, max compression
```

## Comparing `audiconnectpy-1.3.9.tar` & `audiconnectpy-1.4.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:41:46.065297 audiconnectpy-1.3.9/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-20 13:41:36.000000 audiconnectpy-1.3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-20 13:41:36.000000 audiconnectpy-1.3.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-20 13:41:46.061297 audiconnectpy-1.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-05-20 13:41:36.000000 audiconnectpy-1.3.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:41:46.061297 audiconnectpy-1.3.9/audiconnectpy/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-20 13:41:36.000000 audiconnectpy-1.3.9/audiconnectpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-05-20 13:41:36.000000 audiconnectpy-1.3.9/audiconnectpy/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    22837 2023-05-20 13:41:36.000000 audiconnectpy-1.3.9/audiconnectpy/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-20 13:41:36.000000 audiconnectpy-1.3.9/audiconnectpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-05-20 13:41:36.000000 audiconnectpy-1.3.9/audiconnectpy/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    27196 2023-05-20 13:41:36.000000 audiconnectpy-1.3.9/audiconnectpy/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    32069 2023-05-20 13:41:36.000000 audiconnectpy-1.3.9/audiconnectpy/services.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:41:46.061297 audiconnectpy-1.3.9/audiconnectpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-20 13:41:46.000000 audiconnectpy-1.3.9/audiconnectpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-20 13:41:46.000000 audiconnectpy-1.3.9/audiconnectpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 13:41:46.000000 audiconnectpy-1.3.9/audiconnectpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 13:41:46.000000 audiconnectpy-1.3.9/audiconnectpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-20 13:41:46.000000 audiconnectpy-1.3.9/audiconnectpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-20 13:41:36.000000 audiconnectpy-1.3.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 13:41:46.065297 audiconnectpy-1.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-20 13:41:45.000000 audiconnectpy-1.3.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:41:46.061297 audiconnectpy-1.3.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-20 13:41:36.000000 audiconnectpy-1.3.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:13:59.288046 audiconnectpy-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-20 14:13:45.000000 audiconnectpy-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-20 14:13:45.000000 audiconnectpy-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-20 14:13:59.288046 audiconnectpy-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-05-20 14:13:45.000000 audiconnectpy-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:13:59.288046 audiconnectpy-1.4.0/audiconnectpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-20 14:13:45.000000 audiconnectpy-1.4.0/audiconnectpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-05-20 14:13:45.000000 audiconnectpy-1.4.0/audiconnectpy/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22837 2023-05-20 14:13:45.000000 audiconnectpy-1.4.0/audiconnectpy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-20 14:13:45.000000 audiconnectpy-1.4.0/audiconnectpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-05-20 14:13:45.000000 audiconnectpy-1.4.0/audiconnectpy/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27196 2023-05-20 14:13:45.000000 audiconnectpy-1.4.0/audiconnectpy/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32074 2023-05-20 14:13:45.000000 audiconnectpy-1.4.0/audiconnectpy/services.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:13:59.288046 audiconnectpy-1.4.0/audiconnectpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-20 14:13:59.000000 audiconnectpy-1.4.0/audiconnectpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-20 14:13:59.000000 audiconnectpy-1.4.0/audiconnectpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 14:13:59.000000 audiconnectpy-1.4.0/audiconnectpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 14:13:59.000000 audiconnectpy-1.4.0/audiconnectpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-20 14:13:59.000000 audiconnectpy-1.4.0/audiconnectpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-20 14:13:45.000000 audiconnectpy-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 14:13:59.288046 audiconnectpy-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-20 14:13:57.000000 audiconnectpy-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:13:59.288046 audiconnectpy-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-20 14:13:45.000000 audiconnectpy-1.4.0/tests/__init__.py
```

### Comparing `audiconnectpy-1.3.9/LICENSE` & `audiconnectpy-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.3.9/PKG-INFO` & `audiconnectpy-1.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 1.3.9
+Version: 1.4.0
 Summary: Provides asynchronous authentication and access to Audi Connect
 Home-page: https://github.com/cyr-ius/audiconnectpy/tree/master/audiconnectpy
 Author: cyr-ius
 Author-email: cyr-ius@ipocus.net
 License: GPL-3
 Keywords: connect,async
 Classifier: Programming Language :: Python
```

### Comparing `audiconnectpy-1.3.9/README.md` & `audiconnectpy-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.3.9/audiconnectpy/api.py` & `audiconnectpy-1.4.0/audiconnectpy/api.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.3.9/audiconnectpy/auth.py` & `audiconnectpy-1.4.0/audiconnectpy/auth.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.3.9/audiconnectpy/helpers.py` & `audiconnectpy-1.4.0/audiconnectpy/helpers.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.3.9/audiconnectpy/models.py` & `audiconnectpy-1.4.0/audiconnectpy/models.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.3.9/audiconnectpy/services.py` & `audiconnectpy-1.4.0/audiconnectpy/services.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,26 +141,26 @@
 
     async def async_get_tripdata(
         self, vin: str, kind: Literal["short", "long", "cyclic"]
     ) -> tuple[TripDataResponse, TripDataResponse]:
         """Get trip data."""
         if kind not in ["short", "long", "cyclic"]:
             raise AudiException(f"Syntax error, {kind} must be 'short'|'long|'cyclic'")
-        kind.replace("short", "shortTerm").replace("long", "longTerm")
+        knd = kind.replace("short", "shortTerm").replace("long", "longTerm")
         url = await self._async_get_home_region(vin.upper())
         params = {
             "type": "list",
             "from": "1970-01-01T00:00:00Z",
             # "from":(datetime.utcnow() - timedelta(days=365)).strftime("%Y-%m-%dT%H:%M:%SZ"),
             "to": (datetime.utcnow() + timedelta(minutes=90)).strftime(
                 "%Y-%m-%dT%H:%M:%SZ"
             ),
         }
         data = await self._auth.get(
-            f"{url}/bs/tripstatistics/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/tripdata/{kind}",
+            f"{url}/bs/tripstatistics/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/tripdata/{knd}",
             params=params,
         )
         data = data if data else ExtendedDict()
         td_sorted = sorted(
             data.getr("tripDataList.tripData"),
             key=lambda k: k["overallMileage"],  # type: ignore[no-any-return]
             reverse=True,
```

### Comparing `audiconnectpy-1.3.9/audiconnectpy.egg-info/PKG-INFO` & `audiconnectpy-1.4.0/audiconnectpy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 1.3.9
+Version: 1.4.0
 Summary: Provides asynchronous authentication and access to Audi Connect
 Home-page: https://github.com/cyr-ius/audiconnectpy/tree/master/audiconnectpy
 Author: cyr-ius
 Author-email: cyr-ius@ipocus.net
 License: GPL-3
 Keywords: connect,async
 Classifier: Programming Language :: Python
```

### Comparing `audiconnectpy-1.3.9/pyproject.toml` & `audiconnectpy-1.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.3.9/setup.py` & `audiconnectpy-1.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Get the long description from the README file
 with open(os.path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name="audiconnectpy",
-    version="1.3.9",
+    version="1.4.0",
     packages=find_packages(),
     author="cyr-ius",
     author_email="cyr-ius@ipocus.net",
     description="Provides asynchronous authentication and access to Audi Connect",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=["aiohttp>=3.8.1", "beautifulsoup4>=4.11.2"],
```

