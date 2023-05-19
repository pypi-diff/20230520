# Comparing `tmp/eigenrules-0.1.8.tar.gz` & `tmp/eigenrules-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eigenrules-0.1.8.tar", max compression
+gzip compressed data, was "eigenrules-0.1.9.tar", max compression
```

## Comparing `eigenrules-0.1.8.tar` & `eigenrules-0.1.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2023-03-31 19:13:19.747869 eigenrules-0.1.8/LICENSE
--rw-r--r--   0        0        0      213 2023-03-31 19:13:19.747869 eigenrules-0.1.8/README.md
--rw-r--r--   0        0        0      164 2023-03-31 19:13:19.747869 eigenrules-0.1.8/eigenrules/__init__.py
--rw-r--r--   0        0        0     6049 2023-03-31 19:13:19.747869 eigenrules-0.1.8/eigenrules/eigendata.py
--rw-r--r--   0        0        0      206 2023-03-31 19:13:19.747869 eigenrules-0.1.8/eigenrules/exceptions.py
--rw-r--r--   0        0        0     1450 2023-03-31 19:13:19.747869 eigenrules-0.1.8/eigenrules/schemas.py
--rw-r--r--   0        0        0      696 2023-03-31 19:13:19.811870 eigenrules-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      832 1970-01-01 00:00:00.000000 eigenrules-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-01 14:56:56.886948 eigenrules-0.1.9/LICENSE
+-rw-r--r--   0        0        0      213 2023-04-01 14:56:56.886948 eigenrules-0.1.9/README.md
+-rw-r--r--   0        0        0      164 2023-04-01 14:56:56.886948 eigenrules-0.1.9/eigenrules/__init__.py
+-rw-r--r--   0        0        0     6049 2023-04-01 14:56:56.886948 eigenrules-0.1.9/eigenrules/eigendata.py
+-rw-r--r--   0        0        0      206 2023-04-01 14:56:56.886948 eigenrules-0.1.9/eigenrules/exceptions.py
+-rw-r--r--   0        0        0     1450 2023-04-01 14:56:56.886948 eigenrules-0.1.9/eigenrules/schemas.py
+-rw-r--r--   0        0        0      703 2023-04-01 14:56:56.950953 eigenrules-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      881 1970-01-01 00:00:00.000000 eigenrules-0.1.9/PKG-INFO
```

### Comparing `eigenrules-0.1.8/LICENSE` & `eigenrules-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `eigenrules-0.1.8/eigenrules/eigendata.py` & `eigenrules-0.1.9/eigenrules/eigendata.py`

 * *Files identical despite different names*

### Comparing `eigenrules-0.1.8/eigenrules/schemas.py` & `eigenrules-0.1.9/eigenrules/schemas.py`

 * *Files identical despite different names*

### Comparing `eigenrules-0.1.8/pyproject.toml` & `eigenrules-0.1.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "eigenrules"
-version = "0.1.8"
+version = "0.1.9"
 description = "Client library to communicate with eigendata ML systems"
 authors = ["bjornaer <max@eigendata.ai>"]
 license = "Apache 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.9"
 pandas = "^1.5.3"
 requests = "^2.28.2"
 numpy = "^1.24.2"
 pydantic = "^1.10.6"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
@@ -22,15 +22,15 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
-target-version = ['py310', 'py311']
+target-version = ['py39', 'py310', 'py311']
 exclude = '''
 (
   /(
     \.mypy_cache
   )/
 )
 '''
```

### Comparing `eigenrules-0.1.8/PKG-INFO` & `eigenrules-0.1.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: eigenrules
-Version: 0.1.8
+Version: 0.1.9
 Summary: Client library to communicate with eigendata ML systems
 License: Apache 2.0
 Author: bjornaer
 Author-email: max@eigendata.ai
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: pydantic (>=1.10.6,<2.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Description-Content-Type: text/markdown
```

