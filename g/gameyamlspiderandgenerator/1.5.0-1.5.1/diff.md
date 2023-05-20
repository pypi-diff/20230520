# Comparing `tmp/gameyamlspiderandgenerator-1.5.0.tar.gz` & `tmp/gameyamlspiderandgenerator-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gameyamlspiderandgenerator-1.5.0.tar", max compression
+gzip compressed data, was "gameyamlspiderandgenerator-1.5.1.tar", max compression
```

## Comparing `gameyamlspiderandgenerator-1.5.0.tar` & `gameyamlspiderandgenerator-1.5.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rwxr-xr-x   0        0        0     1069 2023-05-05 11:54:39.050499 gameyamlspiderandgenerator-1.5.0/LICENSE
--rwxr-xr-x   0        0        0     1321 2023-05-05 11:54:39.050733 gameyamlspiderandgenerator-1.5.0/README.md
--rwxr-xr-x   0        0        0      568 2023-05-05 11:54:39.052482 gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/__init__.py
--rwxr-xr-x   0        0        0     1751 2023-05-05 11:54:39.052734 gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/__main__.py
--rwxr-xr-x   0        0        0      753 2023-05-05 11:54:39.052963 gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/exception.py
--rwxr-xr-x   0        0        0       52 2023-05-05 11:54:39.054143 gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/hook/__init__.py
--rwxr-xr-x   0        0        0      235 2023-05-19 14:05:11.849031 gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/hook/_base.py
--rwxr-xr-x   0        0        0      901 2023-05-19 15:02:18.997930 gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/hook/openai.py
--rwxr-xr-x   0        0        0     3879 2023-05-19 14:09:35.954441 gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/hook/search.py
--rwxr-xr-x   0        0        0      559 2023-05-19 14:05:11.679558 gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/hook/validate.py
--rwxr-xr-x   0        0        0       56 2023-05-05 11:54:39.055255 gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/plugin/__init__.py
--rwxr-xr-x   0        0        0     3163 2023-05-19 15:02:38.731415 gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/plugin/_base.py
--rwxr-xr-x   0        0        0     7203 2023-05-14 14:53:55.250700 gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/plugin/itchio.py
--rwxr-xr-x   0        0        0     7700 2023-05-05 14:39:08.992543 gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/plugin/steam.py
--rwxr-xr-x   0        0        0        0 2023-05-05 11:54:39.056470 gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/util/__init__.py
--rwxr-xr-x   0        0        0     1461 2023-05-05 11:54:39.056789 gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/util/config.py
--rwxr-xr-x   0        0        0     1472 2023-05-05 14:39:08.993151 gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/util/fgi.py
--rwxr-xr-x   0        0        0     1953 2023-05-05 14:39:08.995558 gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/util/fgi_yaml.py
--rwxr-xr-x   0        0        0     1944 2023-05-05 11:54:39.057708 gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/util/plugin_manager.py
--rwxr-xr-x   0        0        0     2611 2023-05-05 11:54:39.066258 gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/util/spider.py
--rwxr-xr-x   0        0        0      264 2023-05-19 13:17:24.010025 gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/util/thread.py
--rwxr-xr-x   0        0        0      719 2023-05-19 15:05:19.437639 gameyamlspiderandgenerator-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     2449 1970-01-01 00:00:00.000000 gameyamlspiderandgenerator-1.5.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1069 2023-05-05 11:54:39.050499 gameyamlspiderandgenerator-1.5.1/LICENSE
+-rwxr-xr-x   0        0        0     1332 2023-05-20 00:09:25.451593 gameyamlspiderandgenerator-1.5.1/README.md
+-rwxr-xr-x   0        0        0      568 2023-05-05 11:54:39.052482 gameyamlspiderandgenerator-1.5.1/gameyamlspiderandgenerator/__init__.py
+-rwxr-xr-x   0        0        0     1751 2023-05-05 11:54:39.052734 gameyamlspiderandgenerator-1.5.1/gameyamlspiderandgenerator/__main__.py
+-rwxr-xr-x   0        0        0      753 2023-05-05 11:54:39.052963 gameyamlspiderandgenerator-1.5.1/gameyamlspiderandgenerator/exception.py
+-rwxr-xr-x   0        0        0       52 2023-05-05 11:54:39.054143 gameyamlspiderandgenerator-1.5.1/gameyamlspiderandgenerator/hook/__init__.py
+-rwxr-xr-x   0        0        0      235 2023-05-19 14:05:11.849031 gameyamlspiderandgenerator-1.5.1/gameyamlspiderandgenerator/hook/_base.py
+-rwxr-xr-x   0        0        0      901 2023-05-19 15:02:18.997930 gameyamlspiderandgenerator-1.5.1/gameyamlspiderandgenerator/hook/openai.py
+-rwxr-xr-x   0        0        0     3879 2023-05-19 14:09:35.954441 gameyamlspiderandgenerator-1.5.1/gameyamlspiderandgenerator/hook/search.py
+-rwxr-xr-x   0        0        0      559 2023-05-19 14:05:11.679558 gameyamlspiderandgenerator-1.5.1/gameyamlspiderandgenerator/hook/validate.py
+-rwxr-xr-x   0        0        0       56 2023-05-05 11:54:39.055255 gameyamlspiderandgenerator-1.5.1/gameyamlspiderandgenerator/plugin/__init__.py
+-rwxr-xr-x   0        0        0     3163 2023-05-19 15:02:38.731415 gameyamlspiderandgenerator-1.5.1/gameyamlspiderandgenerator/plugin/_base.py
+-rwxr-xr-x   0        0        0     7203 2023-05-14 14:53:55.250700 gameyamlspiderandgenerator-1.5.1/gameyamlspiderandgenerator/plugin/itchio.py
+-rwxr-xr-x   0        0        0     7700 2023-05-05 14:39:08.992543 gameyamlspiderandgenerator-1.5.1/gameyamlspiderandgenerator/plugin/steam.py
+-rwxr-xr-x   0        0        0        0 2023-05-05 11:54:39.056470 gameyamlspiderandgenerator-1.5.1/gameyamlspiderandgenerator/util/__init__.py
+-rwxr-xr-x   0        0        0     1461 2023-05-05 11:54:39.056789 gameyamlspiderandgenerator-1.5.1/gameyamlspiderandgenerator/util/config.py
+-rwxr-xr-x   0        0        0     1837 2023-05-20 00:08:47.482214 gameyamlspiderandgenerator-1.5.1/gameyamlspiderandgenerator/util/fgi.py
+-rwxr-xr-x   0        0        0     1953 2023-05-05 14:39:08.995558 gameyamlspiderandgenerator-1.5.1/gameyamlspiderandgenerator/util/fgi_yaml.py
+-rwxr-xr-x   0        0        0     1944 2023-05-05 11:54:39.057708 gameyamlspiderandgenerator-1.5.1/gameyamlspiderandgenerator/util/plugin_manager.py
+-rwxr-xr-x   0        0        0     2611 2023-05-05 11:54:39.066258 gameyamlspiderandgenerator-1.5.1/gameyamlspiderandgenerator/util/spider.py
+-rwxr-xr-x   0        0        0      264 2023-05-19 13:17:24.010025 gameyamlspiderandgenerator-1.5.1/gameyamlspiderandgenerator/util/thread.py
+-rwxr-xr-x   0        0        0      719 2023-05-20 00:14:54.182457 gameyamlspiderandgenerator-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     2460 1970-01-01 00:00:00.000000 gameyamlspiderandgenerator-1.5.1/PKG-INFO
```

### Comparing `gameyamlspiderandgenerator-1.5.0/LICENSE` & `gameyamlspiderandgenerator-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.0/README.md` & `gameyamlspiderandgenerator-1.5.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 ```yaml
 plugin:
   - steam
   - itchio
 hook:
   - search
   - validate
+# - openai
 # if you don't want to set proxy, please fill in {}
 # http: socks5://127.0.0.1:7891
 # https: socks5://127.0.0.1:7891
 proxy: { }
 gitToken: 'your token'
 api:
   google-play: a714b00383f0662a61b2e382d55c685f17015617aa7048972da58a756fb75e90
```

### Comparing `gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/__init__.py` & `gameyamlspiderandgenerator-1.5.1/gameyamlspiderandgenerator/__init__.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/__main__.py` & `gameyamlspiderandgenerator-1.5.1/gameyamlspiderandgenerator/__main__.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/exception.py` & `gameyamlspiderandgenerator-1.5.1/gameyamlspiderandgenerator/exception.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/hook/openai.py` & `gameyamlspiderandgenerator-1.5.1/gameyamlspiderandgenerator/hook/openai.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/hook/search.py` & `gameyamlspiderandgenerator-1.5.1/gameyamlspiderandgenerator/hook/search.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/hook/validate.py` & `gameyamlspiderandgenerator-1.5.1/gameyamlspiderandgenerator/hook/validate.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/plugin/_base.py` & `gameyamlspiderandgenerator-1.5.1/gameyamlspiderandgenerator/plugin/_base.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/plugin/itchio.py` & `gameyamlspiderandgenerator-1.5.1/gameyamlspiderandgenerator/plugin/itchio.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/plugin/steam.py` & `gameyamlspiderandgenerator-1.5.1/gameyamlspiderandgenerator/plugin/steam.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/util/config.py` & `gameyamlspiderandgenerator-1.5.1/gameyamlspiderandgenerator/util/config.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/util/fgi.py` & `gameyamlspiderandgenerator-1.5.1/gameyamlspiderandgenerator/util/fgi.py`

 * *Files 17% similar despite different names*

```diff
@@ -42,7 +42,24 @@
 ]
 default_config = {'api': {'apple': 'a714b00383f0662a61b2e382d55c685f17015617aa7048972da58a756fb75e90',
                           'google-play': 'a714b00383f0662a61b2e382d55c685f17015617aa7048972da58a756fb75e90'},
                   'gitToken': 'your token',
                   'hook': ['search'],
                   'plugin': ['steam', 'itchio'],
                   'proxy': {}}
+template_dict = {
+    "name": 'NAME',
+    "brief-description": 'BRIEF-DESC',
+    "description": 'DESC',
+    "description-format": "markdown",
+    "authors": [],
+    "tags": {
+        "type": [],
+        "lang": [],
+        "platform": [],
+        "publish": [],
+        "misc": [],
+    },
+    "links": [],
+    "thumbnail": 'THUMBNAIL.PNG',
+    "screenshots": [],
+}
```

### Comparing `gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/util/fgi_yaml.py` & `gameyamlspiderandgenerator-1.5.1/gameyamlspiderandgenerator/util/fgi_yaml.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/util/plugin_manager.py` & `gameyamlspiderandgenerator-1.5.1/gameyamlspiderandgenerator/util/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.0/gameyamlspiderandgenerator/util/spider.py` & `gameyamlspiderandgenerator-1.5.1/gameyamlspiderandgenerator/util/spider.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.0/pyproject.toml` & `gameyamlspiderandgenerator-1.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gameyamlspiderandgenerator"
-version = "1.5.0"
+version = "1.5.1"
 description = "A useful tool for generating Furrygameindex yaml files"
 authors = ["kaesinol"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `gameyamlspiderandgenerator-1.5.0/PKG-INFO` & `gameyamlspiderandgenerator-1.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gameyamlspiderandgenerator
-Version: 1.5.0
+Version: 1.5.1
 Summary: A useful tool for generating Furrygameindex yaml files
 License: MIT
 Author: kaesinol
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -38,14 +38,15 @@
 ```yaml
 plugin:
   - steam
   - itchio
 hook:
   - search
   - validate
+# - openai
 # if you don't want to set proxy, please fill in {}
 # http: socks5://127.0.0.1:7891
 # https: socks5://127.0.0.1:7891
 proxy: { }
 gitToken: 'your token'
 api:
   google-play: a714b00383f0662a61b2e382d55c685f17015617aa7048972da58a756fb75e90
```

