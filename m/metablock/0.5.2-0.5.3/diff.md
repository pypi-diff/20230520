# Comparing `tmp/metablock-0.5.2.tar.gz` & `tmp/metablock-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metablock-0.5.2.tar", max compression
+gzip compressed data, was "metablock-0.5.3.tar", max compression
```

## Comparing `metablock-0.5.2.tar` & `metablock-0.5.3.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1482 2023-04-07 10:33:56.321380 metablock-0.5.2/LICENSE
--rw-r--r--   0        0        0      502 2023-04-07 10:33:56.321380 metablock-0.5.2/metablock/__init__.py
--rw-r--r--   0        0        0     4119 2023-04-07 10:33:56.321380 metablock-0.5.2/metablock/client.py
--rw-r--r--   0        0        0     7937 2023-04-07 10:33:56.321380 metablock-0.5.2/metablock/components.py
--rw-r--r--   0        0        0      540 2023-04-07 10:33:56.321380 metablock-0.5.2/metablock/extensions.py
--rw-r--r--   0        0        0     1850 2023-04-07 10:33:56.325380 metablock-0.5.2/metablock/orgs.py
--rw-r--r--   0        0        0     3029 2023-04-07 10:33:56.325380 metablock-0.5.2/metablock/spaces.py
--rw-r--r--   0        0        0     1350 2023-04-07 10:33:56.325380 metablock-0.5.2/metablock/user.py
--rw-r--r--   0        0        0      531 2023-04-07 10:33:56.325380 metablock-0.5.2/metablock/utils.py
--rw-r--r--   0        0        0      584 2023-04-07 10:33:56.325380 metablock-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     1010 2023-04-07 10:33:56.325380 metablock-0.5.2/readme.md
--rw-r--r--   0        0        0     1472 1970-01-01 00:00:00.000000 metablock-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1482 2023-05-20 10:27:45.002933 metablock-0.5.3/LICENSE
+-rw-r--r--   0        0        0      502 2023-05-20 10:27:45.002933 metablock-0.5.3/metablock/__init__.py
+-rw-r--r--   0        0        0     4119 2023-05-20 10:27:45.002933 metablock-0.5.3/metablock/client.py
+-rw-r--r--   0        0        0     7937 2023-05-20 10:27:45.002933 metablock-0.5.3/metablock/components.py
+-rw-r--r--   0        0        0      540 2023-05-20 10:27:45.002933 metablock-0.5.3/metablock/extensions.py
+-rw-r--r--   0        0        0     1850 2023-05-20 10:27:45.002933 metablock-0.5.3/metablock/orgs.py
+-rw-r--r--   0        0        0        0 2023-05-20 10:27:45.002933 metablock-0.5.3/metablock/py.typed
+-rw-r--r--   0        0        0     3029 2023-05-20 10:27:45.006933 metablock-0.5.3/metablock/spaces.py
+-rw-r--r--   0        0        0     1350 2023-05-20 10:27:45.006933 metablock-0.5.3/metablock/user.py
+-rw-r--r--   0        0        0      531 2023-05-20 10:27:45.006933 metablock-0.5.3/metablock/utils.py
+-rw-r--r--   0        0        0      564 2023-05-20 10:27:45.006933 metablock-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     1010 2023-05-20 10:27:45.006933 metablock-0.5.3/readme.md
+-rw-r--r--   0        0        0     1472 1970-01-01 00:00:00.000000 metablock-0.5.3/PKG-INFO
```

### Comparing `metablock-0.5.2/LICENSE` & `metablock-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `metablock-0.5.2/metablock/client.py` & `metablock-0.5.3/metablock/client.py`

 * *Files identical despite different names*

### Comparing `metablock-0.5.2/metablock/components.py` & `metablock-0.5.3/metablock/components.py`

 * *Files identical despite different names*

### Comparing `metablock-0.5.2/metablock/extensions.py` & `metablock-0.5.3/metablock/extensions.py`

 * *Files identical despite different names*

### Comparing `metablock-0.5.2/metablock/orgs.py` & `metablock-0.5.3/metablock/orgs.py`

 * *Files identical despite different names*

### Comparing `metablock-0.5.2/metablock/spaces.py` & `metablock-0.5.3/metablock/spaces.py`

 * *Files identical despite different names*

### Comparing `metablock-0.5.2/metablock/user.py` & `metablock-0.5.3/metablock/user.py`

 * *Files identical despite different names*

### Comparing `metablock-0.5.2/metablock/utils.py` & `metablock-0.5.3/metablock/utils.py`

 * *Files identical despite different names*

### Comparing `metablock-0.5.2/pyproject.toml` & `metablock-0.5.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 [tool.poetry]
 name = "metablock"
-version = "0.5.2"
+version = "0.5.3"
 description = "Metablock cloud python client"
 authors = ["Luca <luca@quantmind.com>"]
 license = "BSD"
 readme = "readme.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
 aiohttp = "^3.8.3"
 
 [tool.poetry.group.dev.dependencies]
 pytest-asyncio = "^0.21.0"
 pytest = "^7.0.1"
 pytest-cov = "^4.0.0"
-mypy = "^1.2.0"
+mypy = "^1.3.0"
 black = "^23.3.0"
 isort = "^5.11.3"
 flake8 = "^6.0.0"
 flake8-builtins = "^2.0.1"
-codecov = "^2.1.12"
 python-dotenv = "^1.0.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `metablock-0.5.2/readme.md` & `metablock-0.5.3/readme.md`

 * *Files identical despite different names*

### Comparing `metablock-0.5.2/PKG-INFO` & `metablock-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metablock
-Version: 0.5.2
+Version: 0.5.3
 Summary: Metablock cloud python client
 License: BSD
 Author: Luca
 Author-email: luca@quantmind.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

