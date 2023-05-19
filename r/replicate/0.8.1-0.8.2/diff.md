# Comparing `tmp/replicate-0.8.1.tar.gz` & `tmp/replicate-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "replicate-0.8.1.tar", last modified: Wed Apr 12 14:16:04 2023, max compression
+gzip compressed data, was "replicate-0.8.2.tar", last modified: Fri May 19 22:45:52 2023, max compression
```

## Comparing `replicate-0.8.1.tar` & `replicate-0.8.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:16:04.991200 replicate-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-04-12 14:15:53.000000 replicate-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18309 2023-04-12 14:16:04.987200 replicate-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-04-12 14:15:53.000000 replicate-0.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-12 14:15:53.000000 replicate-0.8.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:16:04.987200 replicate-0.8.1/replicate/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-12 14:15:53.000000 replicate-0.8.1/replicate/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-12 14:15:53.000000 replicate-0.8.1/replicate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-12 14:15:53.000000 replicate-0.8.1/replicate/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-04-12 14:15:53.000000 replicate-0.8.1/replicate/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-12 14:15:53.000000 replicate-0.8.1/replicate/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-12 14:15:53.000000 replicate-0.8.1/replicate/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-12 14:15:53.000000 replicate-0.8.1/replicate/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-12 14:15:53.000000 replicate-0.8.1/replicate/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-12 14:15:53.000000 replicate-0.8.1/replicate/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-04-12 14:15:53.000000 replicate-0.8.1/replicate/prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-12 14:15:53.000000 replicate-0.8.1/replicate/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-04-12 14:15:53.000000 replicate-0.8.1/replicate/training.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-04-12 14:15:53.000000 replicate-0.8.1/replicate/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:16:04.987200 replicate-0.8.1/replicate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18309 2023-04-12 14:16:04.000000 replicate-0.8.1/replicate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-12 14:16:04.000000 replicate-0.8.1/replicate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 14:16:04.000000 replicate-0.8.1/replicate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-12 14:16:04.000000 replicate-0.8.1/replicate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-12 14:16:04.000000 replicate-0.8.1/replicate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 14:16:04.991200 replicate-0.8.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:16:04.987200 replicate-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9693 2023-04-12 14:15:53.000000 replicate-0.8.1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-12 14:15:53.000000 replicate-0.8.1/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-04-12 14:15:53.000000 replicate-0.8.1/tests/test_prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-04-12 14:15:53.000000 replicate-0.8.1/tests/test_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-04-12 14:15:53.000000 replicate-0.8.1/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:45:52.357302 replicate-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-05-19 22:45:41.000000 replicate-0.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18624 2023-05-19 22:45:52.353302 replicate-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-05-19 22:45:41.000000 replicate-0.8.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-19 22:45:41.000000 replicate-0.8.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:45:52.353302 replicate-0.8.2/replicate/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-19 22:45:41.000000 replicate-0.8.2/replicate/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-19 22:45:41.000000 replicate-0.8.2/replicate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-19 22:45:41.000000 replicate-0.8.2/replicate/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-05-19 22:45:41.000000 replicate-0.8.2/replicate/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-05-19 22:45:41.000000 replicate-0.8.2/replicate/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-19 22:45:41.000000 replicate-0.8.2/replicate/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-19 22:45:41.000000 replicate-0.8.2/replicate/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-19 22:45:41.000000 replicate-0.8.2/replicate/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-19 22:45:41.000000 replicate-0.8.2/replicate/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-05-19 22:45:41.000000 replicate-0.8.2/replicate/prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-19 22:45:41.000000 replicate-0.8.2/replicate/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-19 22:45:41.000000 replicate-0.8.2/replicate/training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-05-19 22:45:41.000000 replicate-0.8.2/replicate/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:45:52.353302 replicate-0.8.2/replicate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18624 2023-05-19 22:45:52.000000 replicate-0.8.2/replicate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-19 22:45:52.000000 replicate-0.8.2/replicate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 22:45:52.000000 replicate-0.8.2/replicate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-19 22:45:52.000000 replicate-0.8.2/replicate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-19 22:45:52.000000 replicate-0.8.2/replicate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 22:45:52.357302 replicate-0.8.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:45:52.353302 replicate-0.8.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9693 2023-05-19 22:45:41.000000 replicate-0.8.2/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-19 22:45:41.000000 replicate-0.8.2/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-05-19 22:45:41.000000 replicate-0.8.2/tests/test_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-05-19 22:45:41.000000 replicate-0.8.2/tests/test_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-05-19 22:45:41.000000 replicate-0.8.2/tests/test_version.py
```

### Comparing `replicate-0.8.1/LICENSE` & `replicate-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `replicate-0.8.1/PKG-INFO` & `replicate-0.8.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: replicate
-Version: 0.8.1
+Version: 0.8.2
 Summary: Python client for Replicate
 Author: Replicate, Inc.
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -213,14 +213,19 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 # Replicate Python client
 
 This is a Python client for [Replicate](https://replicate.com). It lets you run models from your Python code or Jupyter notebook, and do various other things on Replicate.
 
+> **👋** Check out an interactive version of this tutorial on [Google Colab](https://colab.research.google.com/drive/1K91q4p-OhL96FHBAVLsv9FlwFdu6Pn3c).
+>
+>  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1K91q4p-OhL96FHBAVLsv9FlwFdu6Pn3c)
+
+
 ## Install
 
 ```sh
 pip install replicate
 ```
 
 ## Authenticate
@@ -376,15 +381,15 @@
 
 ```python
 import replicate
 from urllib.request import urlretrieve
 
 model = replicate.models.get("stability-ai/stable-diffusion")
 version = model.versions.get("27b93a2413e7f36cd83da926f3656280b2931564ff050bf9575f1fdf9bcd7478")
-out = version.predict(prompt="wavy colorful abstract patterns, cgsociety"
+out = version.predict(prompt="wavy colorful abstract patterns, cgsociety")
 urlretrieve(out[0], "/tmp/out.png")
 background = Image.open("/tmp/out.png")
 ```
 
 ## Development
 
 See [CONTRIBUTING.md](CONTRIBUTING.md)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `replicate-0.8.1/README.md` & `replicate-0.8.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 # Replicate Python client
 
 This is a Python client for [Replicate](https://replicate.com). It lets you run models from your Python code or Jupyter notebook, and do various other things on Replicate.
 
+> **👋** Check out an interactive version of this tutorial on [Google Colab](https://colab.research.google.com/drive/1K91q4p-OhL96FHBAVLsv9FlwFdu6Pn3c).
+>
+>  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1K91q4p-OhL96FHBAVLsv9FlwFdu6Pn3c)
+
+
 ## Install
 
 ```sh
 pip install replicate
 ```
 
 ## Authenticate
@@ -161,15 +166,15 @@
 
 ```python
 import replicate
 from urllib.request import urlretrieve
 
 model = replicate.models.get("stability-ai/stable-diffusion")
 version = model.versions.get("27b93a2413e7f36cd83da926f3656280b2931564ff050bf9575f1fdf9bcd7478")
-out = version.predict(prompt="wavy colorful abstract patterns, cgsociety"
+out = version.predict(prompt="wavy colorful abstract patterns, cgsociety")
 urlretrieve(out[0], "/tmp/out.png")
 background = Image.open("/tmp/out.png")
 ```
 
 ## Development
 
 See [CONTRIBUTING.md](CONTRIBUTING.md)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `replicate-0.8.1/pyproject.toml` & `replicate-0.8.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "replicate"
-version = "0.8.1"
+version = "0.8.2"
 description = "Python client for Replicate"
 readme = "README.md"
 license = { file = "LICENSE" }
 authors = [{ name = "Replicate, Inc." }]
 requires-python = ">=3.8"
 dependencies = ["packaging", "pydantic>1", "requests>2"]
 optional-dependencies = { dev = [
```

### Comparing `replicate-0.8.1/replicate/base_model.py` & `replicate-0.8.2/replicate/base_model.py`

 * *Files identical despite different names*

### Comparing `replicate-0.8.1/replicate/client.py` & `replicate-0.8.2/replicate/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import re
 from json import JSONDecodeError
 from typing import Any, Dict, Iterator, Optional, Union
 
 import requests
 from requests.adapters import HTTPAdapter, Retry
+from requests.cookies import RequestsCookieJar
 
 from replicate.__about__ import __version__
 from replicate.exceptions import ModelError, ReplicateError
 from replicate.model import ModelCollection
 from replicate.prediction import PredictionCollection
 from replicate.training import TrainingCollection
 
@@ -21,15 +22,15 @@
         self.api_token = api_token
         self.base_url = os.environ.get(
             "REPLICATE_API_BASE_URL", "https://api.replicate.com"
         )
         self.poll_interval = float(os.environ.get("REPLICATE_POLL_INTERVAL", "0.5"))
 
         # TODO: make thread safe
-        self.read_session = requests.Session()
+        self.read_session = _create_session()
         read_retries = Retry(
             total=5,
             backoff_factor=2,
             # Only retry 500s on GET so we don't unintionally mutute data
             allowed_methods=["GET"],
             # https://support.cloudflare.com/hc/en-us/articles/115003011431-Troubleshooting-Cloudflare-5XX-errors
             status_forcelist=[
@@ -46,15 +47,15 @@
                 526,
                 527,
             ],
         )
         self.read_session.mount("http://", HTTPAdapter(max_retries=read_retries))
         self.read_session.mount("https://", HTTPAdapter(max_retries=read_retries))
 
-        self.write_session = requests.Session()
+        self.write_session = _create_session()
         write_retries = Retry(
             total=5,
             backoff_factor=2,
             allowed_methods=["POST", "PUT"],
             # Only retry POST/PUT requests on rate limits, so we don't unintionally mutute data
             status_forcelist=[429],
         )
@@ -80,15 +81,15 @@
                 pass
             raise ReplicateError(f"HTTP error: {resp.status_code, resp.reason}")
         return resp
 
     def _headers(self) -> Dict[str, str]:
         return {
             "Authorization": f"Token {self._api_token()}",
-            "User-Agent": f"replicate-python@{__version__}",
+            "User-Agent": f"replicate-python/{__version__}",
         }
 
     def _api_token(self) -> str:
         token = self.api_token
         # Evaluate lazily in case environment variable is set with dotenv, or something
         if token is None:
             token = os.environ.get("REPLICATE_API_TOKEN")
@@ -134,7 +135,25 @@
         ):
             return prediction.output_iterator()
 
         prediction.wait()
         if prediction.status == "failed":
             raise ModelError(prediction.error)
         return prediction.output
+
+
+class _NonpersistentCookieJar(RequestsCookieJar):
+    """
+    A cookie jar that doesn't persist cookies between requests.
+    """
+
+    def set(self, name, value, **kwargs) -> None:
+        return
+
+    def set_cookie(self, cookie, *args, **kwargs) -> None:
+        return
+
+
+def _create_session() -> requests.Session:
+    s = requests.Session()
+    s.cookies = _NonpersistentCookieJar()
+    return s
```

### Comparing `replicate-0.8.1/replicate/collection.py` & `replicate-0.8.2/replicate/collection.py`

 * *Files identical despite different names*

### Comparing `replicate-0.8.1/replicate/files.py` & `replicate-0.8.2/replicate/files.py`

 * *Files identical despite different names*

### Comparing `replicate-0.8.1/replicate/json.py` & `replicate-0.8.2/replicate/json.py`

 * *Files identical despite different names*

### Comparing `replicate-0.8.1/replicate/model.py` & `replicate-0.8.2/replicate/model.py`

 * *Files identical despite different names*

### Comparing `replicate-0.8.1/replicate/prediction.py` & `replicate-0.8.2/replicate/prediction.py`

 * *Files identical despite different names*

### Comparing `replicate-0.8.1/replicate/schema.py` & `replicate-0.8.2/replicate/schema.py`

 * *Files identical despite different names*

### Comparing `replicate-0.8.1/replicate/training.py` & `replicate-0.8.2/replicate/training.py`

 * *Files identical despite different names*

### Comparing `replicate-0.8.1/replicate/version.py` & `replicate-0.8.2/replicate/version.py`

 * *Files identical despite different names*

### Comparing `replicate-0.8.1/replicate.egg-info/PKG-INFO` & `replicate-0.8.2/replicate.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: replicate
-Version: 0.8.1
+Version: 0.8.2
 Summary: Python client for Replicate
 Author: Replicate, Inc.
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -213,14 +213,19 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 # Replicate Python client
 
 This is a Python client for [Replicate](https://replicate.com). It lets you run models from your Python code or Jupyter notebook, and do various other things on Replicate.
 
+> **👋** Check out an interactive version of this tutorial on [Google Colab](https://colab.research.google.com/drive/1K91q4p-OhL96FHBAVLsv9FlwFdu6Pn3c).
+>
+>  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1K91q4p-OhL96FHBAVLsv9FlwFdu6Pn3c)
+
+
 ## Install
 
 ```sh
 pip install replicate
 ```
 
 ## Authenticate
@@ -376,15 +381,15 @@
 
 ```python
 import replicate
 from urllib.request import urlretrieve
 
 model = replicate.models.get("stability-ai/stable-diffusion")
 version = model.versions.get("27b93a2413e7f36cd83da926f3656280b2931564ff050bf9575f1fdf9bcd7478")
-out = version.predict(prompt="wavy colorful abstract patterns, cgsociety"
+out = version.predict(prompt="wavy colorful abstract patterns, cgsociety")
 urlretrieve(out[0], "/tmp/out.png")
 background = Image.open("/tmp/out.png")
 ```
 
 ## Development
 
 See [CONTRIBUTING.md](CONTRIBUTING.md)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `replicate-0.8.1/replicate.egg-info/SOURCES.txt` & `replicate-0.8.2/replicate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `replicate-0.8.1/tests/test_client.py` & `replicate-0.8.2/tests/test_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     client = Client(api_token="abc123")
     model = client.models.get("test/model")
 
     responses.get(
         "https://api.replicate.com/v1/models/test/model/versions",
         match=[
             matchers.header_matcher({"Authorization": "Token abc123"}),
-            matchers.header_matcher({"User-Agent": f"replicate-python@{__version__}"}),
+            matchers.header_matcher({"User-Agent": f"replicate-python/{__version__}"}),
         ],
         json={"results": []},
     )
 
     model.versions.list()
```

### Comparing `replicate-0.8.1/tests/test_model.py` & `replicate-0.8.2/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `replicate-0.8.1/tests/test_prediction.py` & `replicate-0.8.2/tests/test_prediction.py`

 * *Files identical despite different names*

### Comparing `replicate-0.8.1/tests/test_training.py` & `replicate-0.8.2/tests/test_training.py`

 * *Files identical despite different names*

### Comparing `replicate-0.8.1/tests/test_version.py` & `replicate-0.8.2/tests/test_version.py`

 * *Files identical despite different names*

