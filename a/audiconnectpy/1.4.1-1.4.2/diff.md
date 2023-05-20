# Comparing `tmp/audiconnectpy-1.4.1.tar.gz` & `tmp/audiconnectpy-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiconnectpy-1.4.1.tar", last modified: Sat May 20 15:41:55 2023, max compression
+gzip compressed data, was "audiconnectpy-1.4.2.tar", last modified: Sat May 20 15:50:38 2023, max compression
```

## Comparing `audiconnectpy-1.4.1.tar` & `audiconnectpy-1.4.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 15:41:55.196634 audiconnectpy-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-20 15:41:45.000000 audiconnectpy-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-20 15:41:45.000000 audiconnectpy-1.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-20 15:41:55.196634 audiconnectpy-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-05-20 15:41:45.000000 audiconnectpy-1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 15:41:55.196634 audiconnectpy-1.4.1/audiconnectpy/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-20 15:41:45.000000 audiconnectpy-1.4.1/audiconnectpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-05-20 15:41:45.000000 audiconnectpy-1.4.1/audiconnectpy/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    22837 2023-05-20 15:41:45.000000 audiconnectpy-1.4.1/audiconnectpy/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-20 15:41:45.000000 audiconnectpy-1.4.1/audiconnectpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-05-20 15:41:45.000000 audiconnectpy-1.4.1/audiconnectpy/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    26807 2023-05-20 15:41:45.000000 audiconnectpy-1.4.1/audiconnectpy/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    32074 2023-05-20 15:41:45.000000 audiconnectpy-1.4.1/audiconnectpy/services.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 15:41:55.196634 audiconnectpy-1.4.1/audiconnectpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-20 15:41:55.000000 audiconnectpy-1.4.1/audiconnectpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-20 15:41:55.000000 audiconnectpy-1.4.1/audiconnectpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 15:41:55.000000 audiconnectpy-1.4.1/audiconnectpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 15:41:55.000000 audiconnectpy-1.4.1/audiconnectpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-20 15:41:55.000000 audiconnectpy-1.4.1/audiconnectpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-20 15:41:45.000000 audiconnectpy-1.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 15:41:55.196634 audiconnectpy-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-20 15:41:54.000000 audiconnectpy-1.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 15:41:55.196634 audiconnectpy-1.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-20 15:41:45.000000 audiconnectpy-1.4.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 15:50:38.616926 audiconnectpy-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-20 15:50:28.000000 audiconnectpy-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-20 15:50:28.000000 audiconnectpy-1.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-20 15:50:38.616926 audiconnectpy-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-05-20 15:50:28.000000 audiconnectpy-1.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 15:50:38.616926 audiconnectpy-1.4.2/audiconnectpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-20 15:50:28.000000 audiconnectpy-1.4.2/audiconnectpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-05-20 15:50:28.000000 audiconnectpy-1.4.2/audiconnectpy/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22835 2023-05-20 15:50:28.000000 audiconnectpy-1.4.2/audiconnectpy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-20 15:50:28.000000 audiconnectpy-1.4.2/audiconnectpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-05-20 15:50:28.000000 audiconnectpy-1.4.2/audiconnectpy/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26807 2023-05-20 15:50:28.000000 audiconnectpy-1.4.2/audiconnectpy/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32074 2023-05-20 15:50:28.000000 audiconnectpy-1.4.2/audiconnectpy/services.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 15:50:38.616926 audiconnectpy-1.4.2/audiconnectpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-20 15:50:38.000000 audiconnectpy-1.4.2/audiconnectpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-20 15:50:38.000000 audiconnectpy-1.4.2/audiconnectpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 15:50:38.000000 audiconnectpy-1.4.2/audiconnectpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 15:50:38.000000 audiconnectpy-1.4.2/audiconnectpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-20 15:50:38.000000 audiconnectpy-1.4.2/audiconnectpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-20 15:50:28.000000 audiconnectpy-1.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 15:50:38.620926 audiconnectpy-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-20 15:50:37.000000 audiconnectpy-1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 15:50:38.616926 audiconnectpy-1.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-20 15:50:28.000000 audiconnectpy-1.4.2/tests/__init__.py
```

### Comparing `audiconnectpy-1.4.1/LICENSE` & `audiconnectpy-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.4.1/PKG-INFO` & `audiconnectpy-1.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 1.4.1
+Version: 1.4.2
 Summary: Provides asynchronous authentication and access to Audi Connect
 Home-page: https://github.com/cyr-ius/audiconnectpy/tree/master/audiconnectpy
 Author: cyr-ius
 Author-email: cyr-ius@ipocus.net
 License: GPL-3
 Keywords: connect,async
 Classifier: Programming Language :: Python
```

### Comparing `audiconnectpy-1.4.1/README.md` & `audiconnectpy-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.4.1/audiconnectpy/api.py` & `audiconnectpy-1.4.2/audiconnectpy/api.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.4.1/audiconnectpy/auth.py` & `audiconnectpy-1.4.2/audiconnectpy/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,15 @@
             return response
 
         if "application/json" in content_type:
             rsp = await response.json(loads=json_loads)
         elif (
             headers
             and "application/json" in headers.get("Accept", "")
-            and contents is None
+            and contents == ""
         ):
             _LOGGER.debug("JSON FIX: Accept is JSON but Response is None")
             rsp = ExtendedDict({})
         else:
             rsp = await response.text()
 
         if raw_reply and raw_rsp:
```

### Comparing `audiconnectpy-1.4.1/audiconnectpy/helpers.py` & `audiconnectpy-1.4.2/audiconnectpy/helpers.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.4.1/audiconnectpy/models.py` & `audiconnectpy-1.4.2/audiconnectpy/models.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.4.1/audiconnectpy/services.py` & `audiconnectpy-1.4.2/audiconnectpy/services.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.4.1/audiconnectpy.egg-info/PKG-INFO` & `audiconnectpy-1.4.2/audiconnectpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 1.4.1
+Version: 1.4.2
 Summary: Provides asynchronous authentication and access to Audi Connect
 Home-page: https://github.com/cyr-ius/audiconnectpy/tree/master/audiconnectpy
 Author: cyr-ius
 Author-email: cyr-ius@ipocus.net
 License: GPL-3
 Keywords: connect,async
 Classifier: Programming Language :: Python
```

### Comparing `audiconnectpy-1.4.1/pyproject.toml` & `audiconnectpy-1.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.4.1/setup.py` & `audiconnectpy-1.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Get the long description from the README file
 with open(os.path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name="audiconnectpy",
-    version="1.4.1",
+    version="1.4.2",
     packages=find_packages(),
     author="cyr-ius",
     author_email="cyr-ius@ipocus.net",
     description="Provides asynchronous authentication and access to Audi Connect",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=["aiohttp>=3.8.1", "beautifulsoup4>=4.11.2"],
```

