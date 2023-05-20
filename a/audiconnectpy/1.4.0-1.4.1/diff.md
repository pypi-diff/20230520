# Comparing `tmp/audiconnectpy-1.4.0.tar.gz` & `tmp/audiconnectpy-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiconnectpy-1.4.0.tar", last modified: Sat May 20 14:13:59 2023, max compression
+gzip compressed data, was "audiconnectpy-1.4.1.tar", last modified: Sat May 20 15:41:55 2023, max compression
```

## Comparing `audiconnectpy-1.4.0.tar` & `audiconnectpy-1.4.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:13:59.288046 audiconnectpy-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-20 14:13:45.000000 audiconnectpy-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-20 14:13:45.000000 audiconnectpy-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-20 14:13:59.288046 audiconnectpy-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-05-20 14:13:45.000000 audiconnectpy-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:13:59.288046 audiconnectpy-1.4.0/audiconnectpy/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-20 14:13:45.000000 audiconnectpy-1.4.0/audiconnectpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-05-20 14:13:45.000000 audiconnectpy-1.4.0/audiconnectpy/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    22837 2023-05-20 14:13:45.000000 audiconnectpy-1.4.0/audiconnectpy/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-20 14:13:45.000000 audiconnectpy-1.4.0/audiconnectpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-05-20 14:13:45.000000 audiconnectpy-1.4.0/audiconnectpy/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    27196 2023-05-20 14:13:45.000000 audiconnectpy-1.4.0/audiconnectpy/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    32074 2023-05-20 14:13:45.000000 audiconnectpy-1.4.0/audiconnectpy/services.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:13:59.288046 audiconnectpy-1.4.0/audiconnectpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-20 14:13:59.000000 audiconnectpy-1.4.0/audiconnectpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-20 14:13:59.000000 audiconnectpy-1.4.0/audiconnectpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 14:13:59.000000 audiconnectpy-1.4.0/audiconnectpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 14:13:59.000000 audiconnectpy-1.4.0/audiconnectpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-20 14:13:59.000000 audiconnectpy-1.4.0/audiconnectpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-20 14:13:45.000000 audiconnectpy-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 14:13:59.288046 audiconnectpy-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-20 14:13:57.000000 audiconnectpy-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:13:59.288046 audiconnectpy-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-20 14:13:45.000000 audiconnectpy-1.4.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 15:41:55.196634 audiconnectpy-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-20 15:41:45.000000 audiconnectpy-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-20 15:41:45.000000 audiconnectpy-1.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-20 15:41:55.196634 audiconnectpy-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-05-20 15:41:45.000000 audiconnectpy-1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 15:41:55.196634 audiconnectpy-1.4.1/audiconnectpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-20 15:41:45.000000 audiconnectpy-1.4.1/audiconnectpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-05-20 15:41:45.000000 audiconnectpy-1.4.1/audiconnectpy/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22837 2023-05-20 15:41:45.000000 audiconnectpy-1.4.1/audiconnectpy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-20 15:41:45.000000 audiconnectpy-1.4.1/audiconnectpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-05-20 15:41:45.000000 audiconnectpy-1.4.1/audiconnectpy/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26807 2023-05-20 15:41:45.000000 audiconnectpy-1.4.1/audiconnectpy/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32074 2023-05-20 15:41:45.000000 audiconnectpy-1.4.1/audiconnectpy/services.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 15:41:55.196634 audiconnectpy-1.4.1/audiconnectpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-20 15:41:55.000000 audiconnectpy-1.4.1/audiconnectpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-20 15:41:55.000000 audiconnectpy-1.4.1/audiconnectpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 15:41:55.000000 audiconnectpy-1.4.1/audiconnectpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 15:41:55.000000 audiconnectpy-1.4.1/audiconnectpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-20 15:41:55.000000 audiconnectpy-1.4.1/audiconnectpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-20 15:41:45.000000 audiconnectpy-1.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 15:41:55.196634 audiconnectpy-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-20 15:41:54.000000 audiconnectpy-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 15:41:55.196634 audiconnectpy-1.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-20 15:41:45.000000 audiconnectpy-1.4.1/tests/__init__.py
```

### Comparing `audiconnectpy-1.4.0/LICENSE` & `audiconnectpy-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.4.0/PKG-INFO` & `audiconnectpy-1.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 1.4.0
+Version: 1.4.1
 Summary: Provides asynchronous authentication and access to Audi Connect
 Home-page: https://github.com/cyr-ius/audiconnectpy/tree/master/audiconnectpy
 Author: cyr-ius
 Author-email: cyr-ius@ipocus.net
 License: GPL-3
 Keywords: connect,async
 Classifier: Programming Language :: Python
```

### Comparing `audiconnectpy-1.4.0/README.md` & `audiconnectpy-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.4.0/audiconnectpy/api.py` & `audiconnectpy-1.4.1/audiconnectpy/api.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.4.0/audiconnectpy/auth.py` & `audiconnectpy-1.4.1/audiconnectpy/auth.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.4.0/audiconnectpy/helpers.py` & `audiconnectpy-1.4.1/audiconnectpy/helpers.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.4.0/audiconnectpy/models.py` & `audiconnectpy-1.4.1/audiconnectpy/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -552,16 +552,14 @@
                     )
             except HttpRequestError as error:
                 _LOGGER.error(
                     "Unable to obtain the vehicle  status report of %s: %s",
                     self.vin,
                     str(error).rstrip("\n"),
                 )
-            else:
-                self.support_vehicle = result.is_supported
 
     @retry(exceptions=TimeoutExceededError, tries=3, delay=2)
     async def async_update_position(self) -> None:
         """Update vehicle position."""
         if self.support_position is not False:
             try:
                 result = await self._audi_service.async_get_stored_position(self.vin)
@@ -579,16 +577,14 @@
                     )
             except HttpRequestError as error:
                 _LOGGER.error(
                     "Unable to obtain the vehicle position of %s: %s",
                     self.vin,
                     str(error).rstrip("\n"),
                 )
-            else:
-                self.support_position = result.is_supported
 
     @retry(exceptions=TimeoutExceededError, tries=3, delay=2)
     async def async_update_climater(self) -> None:
         """Update vehicle climater."""
         if self.support_climater is not False:
             try:
                 result = await self._audi_service.async_get_climater(self.vin)
@@ -605,16 +601,14 @@
                     )
             except HttpRequestError as error:
                 _LOGGER.error(
                     "Unable to obtain the vehicle climatisation state for %s: %s",
                     self.vin,
                     str(error).rstrip("\n"),
                 )
-            else:
-                self.support_climater = result.is_supported
 
     @retry(exceptions=TimeoutExceededError, tries=3, delay=2)
     async def async_update_preheater(self) -> None:
         """Update vehicle preheater."""
         if self.support_preheater is not False:
             try:
                 result = await self._audi_service.async_get_preheater(self.vin)
@@ -631,16 +625,14 @@
                     )
             except HttpRequestError as error:
                 _LOGGER.error(
                     "Unable to obtain the vehicle preheater state for %s: %s",
                     self.vin,
                     str(error).rstrip("\n"),
                 )
-            else:
-                self.support_preheater = result.is_supported
 
     @retry(exceptions=TimeoutExceededError, tries=3, delay=2)
     async def async_update_charger(self) -> None:
         """Update vehicle charger."""
         if self.support_charger is not False:
             try:
                 result = await self._audi_service.async_get_charger(self.vin)
@@ -657,16 +649,14 @@
                     )
             except HttpRequestError as error:
                 _LOGGER.error(
                     "Unable to obtain the vehicle charger state for %s: %s",
                     self.vin,
                     str(error).rstrip("\n"),
                 )
-            else:
-                self.support_charger = result.is_supported
 
     @retry(exceptions=TimeoutExceededError, tries=3, delay=2)
     async def async_update_tripdata(
         self, kind: Literal["short", "long", "cyclic"]
     ) -> None:
         """Update vehicle trip."""
         if getattr(self, f"support_trip_{kind}") is not False:
```

### Comparing `audiconnectpy-1.4.0/audiconnectpy/services.py` & `audiconnectpy-1.4.1/audiconnectpy/services.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.4.0/audiconnectpy.egg-info/PKG-INFO` & `audiconnectpy-1.4.1/audiconnectpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 1.4.0
+Version: 1.4.1
 Summary: Provides asynchronous authentication and access to Audi Connect
 Home-page: https://github.com/cyr-ius/audiconnectpy/tree/master/audiconnectpy
 Author: cyr-ius
 Author-email: cyr-ius@ipocus.net
 License: GPL-3
 Keywords: connect,async
 Classifier: Programming Language :: Python
```

### Comparing `audiconnectpy-1.4.0/pyproject.toml` & `audiconnectpy-1.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.4.0/setup.py` & `audiconnectpy-1.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Get the long description from the README file
 with open(os.path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name="audiconnectpy",
-    version="1.4.0",
+    version="1.4.1",
     packages=find_packages(),
     author="cyr-ius",
     author_email="cyr-ius@ipocus.net",
     description="Provides asynchronous authentication and access to Audi Connect",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=["aiohttp>=3.8.1", "beautifulsoup4>=4.11.2"],
```

