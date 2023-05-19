# Comparing `tmp/sha256bit-0.0.1.tar.gz` & `tmp/sha256bit-0.0.3.tar.gz`

## Comparing `sha256bit-0.0.1.tar` & `sha256bit-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rwxr-xr-x   0        0        0       44 2020-02-02 00:00:00.000000 sha256bit-0.0.1/publish_to_pypi
--rw-r--r--   0        0        0     5874 2020-02-02 00:00:00.000000 sha256bit-0.0.1/sha256bit/__init__.py
--rwxr-xr-x   0        0        0  3364551 2020-02-02 00:00:00.000000 sha256bit-0.0.1/test/SHA256LongMsg.rsp
--rwxr-xr-x   0        0        0    80540 2020-02-02 00:00:00.000000 sha256bit-0.0.1/test/SHA256ShortMsg.rsp
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 sha256bit-0.0.1/test/__init__.py
--rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 sha256bit-0.0.1/test/test.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 sha256bit-0.0.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 sha256bit-0.0.1/LICENSE
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 sha256bit-0.0.1/README.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 sha256bit-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 sha256bit-0.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0       44 2020-02-02 00:00:00.000000 sha256bit-0.0.3/publish_to_pypi
+-rw-r--r--   0        0        0     5874 2020-02-02 00:00:00.000000 sha256bit-0.0.3/sha256bit/__init__.py
+-rwxr-xr-x   0        0        0  3364551 2020-02-02 00:00:00.000000 sha256bit-0.0.3/test/SHA256LongMsg.rsp
+-rwxr-xr-x   0        0        0    80540 2020-02-02 00:00:00.000000 sha256bit-0.0.3/test/SHA256ShortMsg.rsp
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 sha256bit-0.0.3/test/__init__.py
+-rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 sha256bit-0.0.3/test/test.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 sha256bit-0.0.3/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 sha256bit-0.0.3/LICENSE
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 sha256bit-0.0.3/README.md
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 sha256bit-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 sha256bit-0.0.3/PKG-INFO
```

### Comparing `sha256bit-0.0.1/sha256bit/__init__.py` & `sha256bit-0.0.3/sha256bit/__init__.py`

 * *Files identical despite different names*

### Comparing `sha256bit-0.0.1/test/SHA256LongMsg.rsp` & `sha256bit-0.0.3/test/SHA256LongMsg.rsp`

 * *Files identical despite different names*

### Comparing `sha256bit-0.0.1/test/SHA256ShortMsg.rsp` & `sha256bit-0.0.3/test/SHA256ShortMsg.rsp`

 * *Files identical despite different names*

### Comparing `sha256bit-0.0.1/test/test.py` & `sha256bit-0.0.3/test/test.py`

 * *Files identical despite different names*

### Comparing `sha256bit-0.0.1/.gitignore` & `sha256bit-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `sha256bit-0.0.1/LICENSE` & `sha256bit-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sha256bit-0.0.1/pyproject.toml` & `sha256bit-0.0.3/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 [build-system]
-requires = ["hatchling"]
+requires = ["hatchling", "hatch-vcs"]
 build-backend = "hatchling.build"
 
+[tool.hatch.version]
+source = "vcs"
+
 [project]
 name = "sha256bit"
-version = "0.0.1"
+dynamic = ["version"]
 authors = [
   { name="Sebastien Riou", email="" },
 ]
 description = "SHA256 with bit granularity for message input length"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/sebastien-riou/sha256bit"
-"Bug Tracker" = "https://github.com/sebastien-riou/sha256bit/issues"
+"Bug Tracker" = "https://github.com/sebastien-riou/sha256bit/issues"
+
```

### Comparing `sha256bit-0.0.1/PKG-INFO` & `sha256bit-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sha256bit
-Version: 0.0.1
+Version: 0.0.3
 Summary: SHA256 with bit granularity for message input length
 Project-URL: Homepage, https://github.com/sebastien-riou/sha256bit
 Project-URL: Bug Tracker, https://github.com/sebastien-riou/sha256bit/issues
 Author: Sebastien Riou
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

