# Comparing `tmp/tap_dbt-0.5.1a1.tar.gz` & `tmp/tap_dbt-0.6.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_dbt-0.5.1a1.tar", max compression
+gzip compressed data, was "tap_dbt-0.6.0a1.tar", max compression
```

## Comparing `tap_dbt-0.5.1a1.tar` & `tap_dbt-0.6.0a1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11357 2023-04-17 19:55:15.889690 tap_dbt-0.5.1a1/LICENSE
--rw-r--r--   0        0        0     4899 2023-04-17 19:55:15.889690 tap_dbt-0.5.1a1/README.md
--rw-r--r--   0        0        0     1615 2023-04-17 19:55:31.785910 tap_dbt-0.5.1a1/pyproject.toml
--rw-r--r--   0        0        0       40 2023-04-17 19:55:15.889690 tap_dbt-0.5.1a1/tap_dbt/__init__.py
--rw-r--r--   0        0        0     2360 2023-04-17 19:55:15.889690 tap_dbt-0.5.1a1/tap_dbt/client.py
--rw-r--r--   0        0        0     1780 2023-04-17 19:55:15.889690 tap_dbt-0.5.1a1/tap_dbt/schemas/accounts.json
--rw-r--r--   0        0        0     2264 2023-04-17 19:55:15.889690 tap_dbt-0.5.1a1/tap_dbt/schemas/jobs.json
--rw-r--r--   0        0        0     1821 2023-04-17 19:55:15.889690 tap_dbt-0.5.1a1/tap_dbt/schemas/projects.json
--rw-r--r--   0        0        0     3368 2023-04-17 19:55:15.889690 tap_dbt-0.5.1a1/tap_dbt/schemas/runs.json
--rw-r--r--   0        0        0     3538 2023-04-17 19:55:15.889690 tap_dbt-0.5.1a1/tap_dbt/streams.py
--rw-r--r--   0        0        0     2033 2023-04-17 19:55:15.889690 tap_dbt-0.5.1a1/tap_dbt/tap.py
--rw-r--r--   0        0        0     5795 1970-01-01 00:00:00.000000 tap_dbt-0.5.1a1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-19 22:32:03.917137 tap_dbt-0.6.0a1/LICENSE
+-rw-r--r--   0        0        0     4899 2023-05-19 22:32:03.917137 tap_dbt-0.6.0a1/README.md
+-rw-r--r--   0        0        0     1651 2023-05-19 22:32:20.177365 tap_dbt-0.6.0a1/pyproject.toml
+-rw-r--r--   0        0        0       40 2023-05-19 22:32:03.917137 tap_dbt-0.6.0a1/tap_dbt/__init__.py
+-rw-r--r--   0        0        0     2360 2023-05-19 22:32:03.917137 tap_dbt-0.6.0a1/tap_dbt/client.py
+-rw-r--r--   0        0        0     1780 2023-05-19 22:32:03.917137 tap_dbt-0.6.0a1/tap_dbt/schemas/accounts.json
+-rw-r--r--   0        0        0     2264 2023-05-19 22:32:03.917137 tap_dbt-0.6.0a1/tap_dbt/schemas/jobs.json
+-rw-r--r--   0        0        0     1821 2023-05-19 22:32:03.917137 tap_dbt-0.6.0a1/tap_dbt/schemas/projects.json
+-rw-r--r--   0        0        0     3368 2023-05-19 22:32:03.917137 tap_dbt-0.6.0a1/tap_dbt/schemas/runs.json
+-rw-r--r--   0        0        0     3538 2023-05-19 22:32:03.917137 tap_dbt-0.6.0a1/tap_dbt/streams.py
+-rw-r--r--   0        0        0     2033 2023-05-19 22:32:03.917137 tap_dbt-0.6.0a1/tap_dbt/tap.py
+-rw-r--r--   0        0        0     5795 1970-01-01 00:00:00.000000 tap_dbt-0.6.0a1/PKG-INFO
```

### Comparing `tap_dbt-0.5.1a1/LICENSE` & `tap_dbt-0.6.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `tap_dbt-0.5.1a1/README.md` & `tap_dbt-0.6.0a1/README.md`

 * *Files identical despite different names*

### Comparing `tap_dbt-0.5.1a1/pyproject.toml` & `tap_dbt-0.6.0a1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,45 +1,43 @@
 [build-system]
-build-backend = "poetry.core.masonry.api"
-requires = [
-  "poetry-core>=1.5",
-]
-
-[tool.black]
-line-length = 88
-
-[tool.isort]
-profile = "black"
-multi_line_output = 3 # Vertical Hanging Indent
-src_paths = "tap_dbt"
+requires = ["poetry-core==1.6.0", "poetry-dynamic-versioning"]
+build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "tap-dbt"
-version = "0.5.1a1"
+version = "0.6.0a1"
 description = "Singer tap for dbt, built with the Singer SDK."
 license = "Apache-2.0"
 authors = ["Edgar Ramírez Mondragón <edgarrm358@sample.com>"]
 maintainers = ["Edgar Ramírez Mondragón <edgarrm358@sample.com>"]
 readme = "README.md"
 repository = "https://github.com/edgarrmondragon/tap-dbt"
 keywords = ["singer.io", "elt", "dbt", "singer-sdk"]
 
 [tool.poetry.dependencies]
 python = "<3.12,>=3.7.1"
 pyyaml = "^6.0"
-singer-sdk = "==0.24.0"
+singer-sdk = "==0.27.0"
 
 [tool.poetry.group.dev.dependencies]
 faker = ">=17.6,<19.0"
 pytest = "^7.2.2"
 responses = "^0.23.1"
 
 [tool.poetry.scripts]
 tap-dbt = 'tap_dbt.tap:cli'
 
+[tool.black]
+line-length = 88
+
+[tool.isort]
+profile = "black"
+multi_line_output = 3 # Vertical Hanging Indent
+src_paths = "tap_dbt"
+
 [tool.poetry-dynamic-versioning]
 enable = false
 format-jinja = """
     {%- if distance == 0 -%}
         {{ serialize_pep440(base, stage, revision) }}
     {%- elif revision is not none -%}
         {{ serialize_pep440(base, stage, revision + 1, dev=distance, metadata=[commit]) }}
```

### Comparing `tap_dbt-0.5.1a1/tap_dbt/client.py` & `tap_dbt-0.6.0a1/tap_dbt/client.py`

 * *Files identical despite different names*

### Comparing `tap_dbt-0.5.1a1/tap_dbt/schemas/accounts.json` & `tap_dbt-0.6.0a1/tap_dbt/schemas/accounts.json`

 * *Files identical despite different names*

### Comparing `tap_dbt-0.5.1a1/tap_dbt/schemas/jobs.json` & `tap_dbt-0.6.0a1/tap_dbt/schemas/jobs.json`

 * *Files identical despite different names*

### Comparing `tap_dbt-0.5.1a1/tap_dbt/schemas/projects.json` & `tap_dbt-0.6.0a1/tap_dbt/schemas/projects.json`

 * *Files identical despite different names*

### Comparing `tap_dbt-0.5.1a1/tap_dbt/schemas/runs.json` & `tap_dbt-0.6.0a1/tap_dbt/schemas/runs.json`

 * *Files identical despite different names*

### Comparing `tap_dbt-0.5.1a1/tap_dbt/streams.py` & `tap_dbt-0.6.0a1/tap_dbt/streams.py`

 * *Files identical despite different names*

### Comparing `tap_dbt-0.5.1a1/tap_dbt/tap.py` & `tap_dbt-0.6.0a1/tap_dbt/tap.py`

 * *Files identical despite different names*

### Comparing `tap_dbt-0.5.1a1/PKG-INFO` & `tap_dbt-0.6.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-dbt
-Version: 0.5.1a1
+Version: 0.6.0a1
 Summary: Singer tap for dbt, built with the Singer SDK.
 Home-page: https://github.com/edgarrmondragon/tap-dbt
 License: Apache-2.0
 Keywords: singer.io,elt,dbt,singer-sdk
 Author: Edgar Ramírez Mondragón
 Author-email: edgarrm358@sample.com
 Maintainer: Edgar Ramírez Mondragón
@@ -13,15 +13,15 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pyyaml (>=6.0,<7.0)
-Requires-Dist: singer-sdk (==0.24.0)
+Requires-Dist: singer-sdk (==0.27.0)
 Project-URL: Repository, https://github.com/edgarrmondragon/tap-dbt
 Description-Content-Type: text/markdown
 
 # tap-dbt
 
 [![PyPI](https://img.shields.io/pypi/v/tap-dbt.svg?color=blue)](https://pypi.org/project/tap-dbt/)
 [![Python versions](https://img.shields.io/pypi/pyversions/tap-dbt.svg)](https://pypi.org/project/tap-dbt/)
```

