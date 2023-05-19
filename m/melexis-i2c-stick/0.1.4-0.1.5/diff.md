# Comparing `tmp/melexis-i2c-stick-0.1.4.tar.gz` & `tmp/melexis-i2c-stick-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "melexis-i2c-stick-0.1.4.tar", last modified: Fri May 19 22:41:36 2023, max compression
+gzip compressed data, was "melexis-i2c-stick-0.1.5.tar", last modified: Fri May 19 23:26:43 2023, max compression
```

## Comparing `melexis-i2c-stick-0.1.4.tar` & `melexis-i2c-stick-0.1.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:41:36.391993 melexis-i2c-stick-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-19 22:41:18.000000 melexis-i2c-stick-0.1.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-19 22:41:18.000000 melexis-i2c-stick-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-19 22:41:18.000000 melexis-i2c-stick-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-19 22:41:18.000000 melexis-i2c-stick-0.1.4/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-19 22:41:36.391993 melexis-i2c-stick-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-19 22:41:18.000000 melexis-i2c-stick-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:41:36.391993 melexis-i2c-stick-0.1.4/melexis/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:41:36.391993 melexis-i2c-stick-0.1.4/melexis/i2c_stick/
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-19 22:41:18.000000 melexis-i2c-stick-0.1.4/melexis/i2c_stick/I2CStick.py
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-05-19 22:41:18.000000 melexis-i2c-stick-0.1.4/melexis/i2c_stick/MemoryFile.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-19 22:41:18.000000 melexis-i2c-stick-0.1.4/melexis/i2c_stick/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:41:36.391993 melexis-i2c-stick-0.1.4/melexis_i2c_stick.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-19 22:41:36.000000 melexis-i2c-stick-0.1.4/melexis_i2c_stick.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-19 22:41:36.000000 melexis-i2c-stick-0.1.4/melexis_i2c_stick.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 22:41:36.000000 melexis-i2c-stick-0.1.4/melexis_i2c_stick.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 22:41:36.000000 melexis-i2c-stick-0.1.4/melexis_i2c_stick.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-19 22:41:36.000000 melexis-i2c-stick-0.1.4/melexis_i2c_stick.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-19 22:41:18.000000 melexis-i2c-stick-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 22:41:36.391993 melexis-i2c-stick-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 23:26:43.611360 melexis-i2c-stick-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-19 23:26:24.000000 melexis-i2c-stick-0.1.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-19 23:26:24.000000 melexis-i2c-stick-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-19 23:26:24.000000 melexis-i2c-stick-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-19 23:26:24.000000 melexis-i2c-stick-0.1.5/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-19 23:26:43.611360 melexis-i2c-stick-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-19 23:26:24.000000 melexis-i2c-stick-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 23:26:43.607360 melexis-i2c-stick-0.1.5/melexis/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 23:26:43.607360 melexis-i2c-stick-0.1.5/melexis/i2c_stick/
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-19 23:26:24.000000 melexis-i2c-stick-0.1.5/melexis/i2c_stick/I2CStick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-05-19 23:26:24.000000 melexis-i2c-stick-0.1.5/melexis/i2c_stick/MemoryFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-19 23:26:24.000000 melexis-i2c-stick-0.1.5/melexis/i2c_stick/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 23:26:43.611360 melexis-i2c-stick-0.1.5/melexis_i2c_stick.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-19 23:26:43.000000 melexis-i2c-stick-0.1.5/melexis_i2c_stick.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-19 23:26:43.000000 melexis-i2c-stick-0.1.5/melexis_i2c_stick.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 23:26:43.000000 melexis-i2c-stick-0.1.5/melexis_i2c_stick.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 23:26:43.000000 melexis-i2c-stick-0.1.5/melexis_i2c_stick.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-19 23:26:43.000000 melexis-i2c-stick-0.1.5/melexis_i2c_stick.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-19 23:26:24.000000 melexis-i2c-stick-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 23:26:43.611360 melexis-i2c-stick-0.1.5/setup.cfg
```

### Comparing `melexis-i2c-stick-0.1.4/CONTRIBUTING.md` & `melexis-i2c-stick-0.1.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `melexis-i2c-stick-0.1.4/LICENSE` & `melexis-i2c-stick-0.1.5/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-   Copyright 2020 Melexis
+   Copyright 2023 Melexis
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
      http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `melexis-i2c-stick-0.1.4/PKG-INFO` & `melexis-i2c-stick-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: melexis-i2c-stick
-Version: 0.1.4
+Version: 0.1.5
 Summary: Melexis I2C Stick, python interface
 Author-email: Karel Vanroye <kva@melexis.com>
-License:    Copyright 2020 Melexis
+License:    Copyright 2023 Melexis
         
            Licensed under the Apache License, Version 2.0 (the "License");
            you may not use this file except in compliance with the License.
            You may obtain a copy of the License at
         
              http://www.apache.org/licenses/LICENSE-2.0
         
@@ -18,15 +18,15 @@
            limitations under the License.
         
 Project-URL: Homepage, https://github.com/melexis/i2c-stick
 Keywords: Melexis,I2C,sensors,demo
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
+Requires-Python: >=3.3
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 License-File: NOTICE
 
 # melexis-i2c-stick-py
```

### Comparing `melexis-i2c-stick-0.1.4/melexis/i2c_stick/I2CStick.py` & `melexis-i2c-stick-0.1.5/melexis/i2c_stick/I2CStick.py`

 * *Files identical despite different names*

### Comparing `melexis-i2c-stick-0.1.4/melexis/i2c_stick/MemoryFile.py` & `melexis-i2c-stick-0.1.5/melexis/i2c_stick/MemoryFile.py`

 * *Files identical despite different names*

### Comparing `melexis-i2c-stick-0.1.4/melexis_i2c_stick.egg-info/PKG-INFO` & `melexis-i2c-stick-0.1.5/melexis_i2c_stick.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: melexis-i2c-stick
-Version: 0.1.4
+Version: 0.1.5
 Summary: Melexis I2C Stick, python interface
 Author-email: Karel Vanroye <kva@melexis.com>
-License:    Copyright 2020 Melexis
+License:    Copyright 2023 Melexis
         
            Licensed under the Apache License, Version 2.0 (the "License");
            you may not use this file except in compliance with the License.
            You may obtain a copy of the License at
         
              http://www.apache.org/licenses/LICENSE-2.0
         
@@ -18,15 +18,15 @@
            limitations under the License.
         
 Project-URL: Homepage, https://github.com/melexis/i2c-stick
 Keywords: Melexis,I2C,sensors,demo
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
+Requires-Python: >=3.3
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 License-File: NOTICE
 
 # melexis-i2c-stick-py
```

### Comparing `melexis-i2c-stick-0.1.4/pyproject.toml` & `melexis-i2c-stick-0.1.5/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 # pyproject.toml
 
+# Learn more about package building configurations: https://realpython.com/pypi-publish-python-package/
+
 [build-system]
 requires      = ["setuptools>=63.2.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "melexis-i2c-stick"
-version = "0.1.4"
+version = "0.1.5"
 description = "Melexis I2C Stick, python interface"
 readme = "README.md"
 authors = [{ name = "Karel Vanroye", email = "kva@melexis.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["Melexis", "I2C", "sensors", "demo"]
 dependencies = [
     'bincopy>=17.14.5',
     'pyserial>=3.5',
 ]
-requires-python = ">=3.9"
+requires-python = ">=3.3"
 
 [project.optional-dependencies]
 dev = []
 
 [project.urls]
 Homepage = "https://github.com/melexis/i2c-stick"
 
 # [project.scripts]
 # melexis_i2c_stick = "melexis.i2c_stick.__main__:main"
 
 
 [tool.bumpver]
-current_version = "0.1.4"
+current_version = "0.1.5"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = false
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

