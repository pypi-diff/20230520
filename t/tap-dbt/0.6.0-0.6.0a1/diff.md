# Comparing `tmp/tap_dbt-0.6.0.tar.gz` & `tmp/tap_dbt-0.6.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_dbt-0.6.0.tar", max compression
+gzip compressed data, was "tap_dbt-0.6.0a1.tar", max compression
```

## Comparing `tap_dbt-0.6.0.tar` & `tap_dbt-0.6.0a1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11357 2023-05-19 23:17:01.565922 tap_dbt-0.6.0/LICENSE
--rw-r--r--   0        0        0     4723 2023-05-19 23:17:01.565922 tap_dbt-0.6.0/README.md
--rw-r--r--   0        0        0     1654 2023-05-19 23:17:29.914133 tap_dbt-0.6.0/pyproject.toml
--rw-r--r--   0        0        0       40 2023-05-19 23:17:01.565922 tap_dbt-0.6.0/tap_dbt/__init__.py
--rw-r--r--   0        0        0     2360 2023-05-19 23:17:01.565922 tap_dbt-0.6.0/tap_dbt/client.py
--rw-r--r--   0        0        0     1780 2023-05-19 23:17:01.565922 tap_dbt-0.6.0/tap_dbt/schemas/accounts.json
--rw-r--r--   0        0        0     2264 2023-05-19 23:17:01.565922 tap_dbt-0.6.0/tap_dbt/schemas/jobs.json
--rw-r--r--   0        0        0     1821 2023-05-19 23:17:01.565922 tap_dbt-0.6.0/tap_dbt/schemas/projects.json
--rw-r--r--   0        0        0     3368 2023-05-19 23:17:01.565922 tap_dbt-0.6.0/tap_dbt/schemas/runs.json
--rw-r--r--   0        0        0     3538 2023-05-19 23:17:01.565922 tap_dbt-0.6.0/tap_dbt/streams.py
--rw-r--r--   0        0        0     2033 2023-05-19 23:17:01.565922 tap_dbt-0.6.0/tap_dbt/tap.py
--rw-r--r--   0        0        0     5617 1970-01-01 00:00:00.000000 tap_dbt-0.6.0/PKG-INFO
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

### Comparing `tap_dbt-0.6.0/LICENSE` & `tap_dbt-0.6.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `tap_dbt-0.6.0/README.md` & `tap_dbt-0.6.0a1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # tap-dbt
 
 [![PyPI](https://img.shields.io/pypi/v/tap-dbt.svg?color=blue)](https://pypi.org/project/tap-dbt/)
 [![Python versions](https://img.shields.io/pypi/pyversions/tap-dbt.svg)](https://pypi.org/project/tap-dbt/)
 [![Singer](https://img.shields.io/badge/Singer-Tap-purple.svg)](https://hub.meltano.com/taps/dbt)
+[![TestPyPI](https://github.com/edgarrmondragon/tap-dbt/actions/workflows/test-pypi.yml/badge.svg)](https://github.com/edgarrmondragon/tap-dbt/actions/workflows/test-pypi.yml)
 [![Test Tap](https://github.com/edgarrmondragon/tap-dbt/actions/workflows/test-tap.yml/badge.svg)](https://github.com/edgarrmondragon/tap-dbt/actions/workflows/test-tap.yml)
 
 `tap-dbt` is a Singer tap for the [dbt Cloud API v2][dbtcloud].
 
 Built with the [Singer SDK][sdk].
 
 - [Installation](#Installation)
```

### Comparing `tap_dbt-0.6.0/pyproject.toml` & `tap_dbt-0.6.0a1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 [build-system]
+requires = ["poetry-core==1.6.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
-requires = [
-  "poetry-core==1.6",
-  "poetry-dynamic-versioning",
-]
 
 [tool.poetry]
 name = "tap-dbt"
-version = "0.6.0"
+version = "0.6.0a1"
 description = "Singer tap for dbt, built with the Singer SDK."
 license = "Apache-2.0"
 authors = ["Edgar Ramírez Mondragón <edgarrm358@sample.com>"]
 maintainers = ["Edgar Ramírez Mondragón <edgarrm358@sample.com>"]
 readme = "README.md"
 repository = "https://github.com/edgarrmondragon/tap-dbt"
 keywords = ["singer.io", "elt", "dbt", "singer-sdk"]
```

### Comparing `tap_dbt-0.6.0/tap_dbt/client.py` & `tap_dbt-0.6.0a1/tap_dbt/client.py`

 * *Files identical despite different names*

### Comparing `tap_dbt-0.6.0/tap_dbt/schemas/accounts.json` & `tap_dbt-0.6.0a1/tap_dbt/schemas/accounts.json`

 * *Files identical despite different names*

### Comparing `tap_dbt-0.6.0/tap_dbt/schemas/jobs.json` & `tap_dbt-0.6.0a1/tap_dbt/schemas/jobs.json`

 * *Files identical despite different names*

### Comparing `tap_dbt-0.6.0/tap_dbt/schemas/projects.json` & `tap_dbt-0.6.0a1/tap_dbt/schemas/projects.json`

 * *Files identical despite different names*

### Comparing `tap_dbt-0.6.0/tap_dbt/schemas/runs.json` & `tap_dbt-0.6.0a1/tap_dbt/schemas/runs.json`

 * *Files identical despite different names*

### Comparing `tap_dbt-0.6.0/tap_dbt/streams.py` & `tap_dbt-0.6.0a1/tap_dbt/streams.py`

 * *Files identical despite different names*

### Comparing `tap_dbt-0.6.0/tap_dbt/tap.py` & `tap_dbt-0.6.0a1/tap_dbt/tap.py`

 * *Files identical despite different names*

### Comparing `tap_dbt-0.6.0/PKG-INFO` & `tap_dbt-0.6.0a1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-dbt
-Version: 0.6.0
+Version: 0.6.0a1
 Summary: Singer tap for dbt, built with the Singer SDK.
 Home-page: https://github.com/edgarrmondragon/tap-dbt
 License: Apache-2.0
 Keywords: singer.io,elt,dbt,singer-sdk
 Author: Edgar Ramírez Mondragón
 Author-email: edgarrm358@sample.com
 Maintainer: Edgar Ramírez Mondragón
@@ -22,14 +22,15 @@
 Description-Content-Type: text/markdown
 
 # tap-dbt
 
 [![PyPI](https://img.shields.io/pypi/v/tap-dbt.svg?color=blue)](https://pypi.org/project/tap-dbt/)
 [![Python versions](https://img.shields.io/pypi/pyversions/tap-dbt.svg)](https://pypi.org/project/tap-dbt/)
 [![Singer](https://img.shields.io/badge/Singer-Tap-purple.svg)](https://hub.meltano.com/taps/dbt)
+[![TestPyPI](https://github.com/edgarrmondragon/tap-dbt/actions/workflows/test-pypi.yml/badge.svg)](https://github.com/edgarrmondragon/tap-dbt/actions/workflows/test-pypi.yml)
 [![Test Tap](https://github.com/edgarrmondragon/tap-dbt/actions/workflows/test-tap.yml/badge.svg)](https://github.com/edgarrmondragon/tap-dbt/actions/workflows/test-tap.yml)
 
 `tap-dbt` is a Singer tap for the [dbt Cloud API v2][dbtcloud].
 
 Built with the [Singer SDK][sdk].
 
 - [Installation](#Installation)
```

