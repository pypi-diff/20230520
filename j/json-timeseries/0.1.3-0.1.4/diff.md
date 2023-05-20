# Comparing `tmp/json_timeseries-0.1.3.tar.gz` & `tmp/json_timeseries-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json_timeseries-0.1.3.tar", last modified: Sat May 20 08:18:50 2023, max compression
+gzip compressed data, was "json_timeseries-0.1.4.tar", last modified: Sat May 20 08:45:54 2023, max compression
```

## Comparing `json_timeseries-0.1.3.tar` & `json_timeseries-0.1.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 slavapisarevskiy   (501) staff       (20)        0 2023-05-20 08:18:50.312203 json_timeseries-0.1.3/
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)     1857 2023-05-07 05:16:13.000000 json_timeseries-0.1.3/.gitignore
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)      592 2023-05-14 11:48:03.000000 json_timeseries-0.1.3/.readthedocs.yml
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)     1074 2023-03-28 00:27:02.000000 json_timeseries-0.1.3/LICENSE
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)     5024 2023-05-20 08:18:50.312816 json_timeseries-0.1.3/PKG-INFO
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)     4142 2023-05-14 11:43:08.000000 json_timeseries-0.1.3/README.md
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)      126 2023-05-20 08:17:50.000000 json_timeseries-0.1.3/build.sh
-drwxr-xr-x   0 slavapisarevskiy   (501) staff       (20)        0 2023-05-20 08:18:50.260610 json_timeseries-0.1.3/docs/
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)      634 2023-05-07 04:38:02.000000 json_timeseries-0.1.3/docs/Makefile
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)     1185 2023-05-14 10:33:09.000000 json_timeseries-0.1.3/docs/conf.py
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)      518 2023-05-14 11:54:21.000000 json_timeseries-0.1.3/docs/index.rst
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)      800 2023-05-07 04:38:02.000000 json_timeseries-0.1.3/docs/make.bat
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)       16 2023-05-14 11:48:31.000000 json_timeseries-0.1.3/docs/requirements.txt
-drwxr-xr-x   0 slavapisarevskiy   (501) staff       (20)        0 2023-05-20 08:18:50.269828 json_timeseries-0.1.3/docs/source/
-drwxr-xr-x   0 slavapisarevskiy   (501) staff       (20)        0 2023-05-20 08:18:50.277924 json_timeseries-0.1.3/docs/source/api/
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)      311 2023-05-14 10:42:36.000000 json_timeseries-0.1.3/docs/source/api/jts.rst
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)       31 2023-05-14 10:41:37.000000 json_timeseries-0.1.3/docs/source/readme.rst
-drwxr-xr-x   0 slavapisarevskiy   (501) staff       (20)        0 2023-05-20 08:18:50.285117 json_timeseries-0.1.3/json_timeseries/
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)      128 2023-05-09 07:13:32.000000 json_timeseries-0.1.3/json_timeseries/__init__.py
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)     9005 2023-05-20 08:16:54.000000 json_timeseries-0.1.3/json_timeseries/jts.py
-drwxr-xr-x   0 slavapisarevskiy   (501) staff       (20)        0 2023-05-20 08:18:50.304065 json_timeseries-0.1.3/json_timeseries.egg-info/
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)     5024 2023-05-20 08:18:50.000000 json_timeseries-0.1.3/json_timeseries.egg-info/PKG-INFO
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)      514 2023-05-20 08:18:50.000000 json_timeseries-0.1.3/json_timeseries.egg-info/SOURCES.txt
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)        1 2023-05-20 08:18:50.000000 json_timeseries-0.1.3/json_timeseries.egg-info/dependency_links.txt
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)       16 2023-05-20 08:18:50.000000 json_timeseries-0.1.3/json_timeseries.egg-info/requires.txt
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)       22 2023-05-20 08:18:50.000000 json_timeseries-0.1.3/json_timeseries.egg-info/top_level.txt
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)       99 2023-05-08 12:17:32.000000 json_timeseries-0.1.3/pyproject.toml
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)       15 2023-05-07 12:04:18.000000 json_timeseries-0.1.3/requirements.txt
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)     1049 2023-05-20 08:18:50.322976 json_timeseries-0.1.3/setup.cfg
-drwxr-xr-x   0 slavapisarevskiy   (501) staff       (20)        0 2023-05-20 08:18:50.309816 json_timeseries-0.1.3/tests/
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)        0 2023-03-30 00:31:15.000000 json_timeseries-0.1.3/tests/__init__.py
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)    11646 2023-05-20 08:15:14.000000 json_timeseries-0.1.3/tests/test_json_timeseries.py
+drwxr-xr-x   0 slavapisarevskiy   (501) staff       (20)        0 2023-05-20 08:45:54.396455 json_timeseries-0.1.4/
+-rw-r--r--   0 slavapisarevskiy   (501) staff       (20)     1857 2023-05-07 05:16:13.000000 json_timeseries-0.1.4/.gitignore
+-rw-r--r--   0 slavapisarevskiy   (501) staff       (20)      592 2023-05-14 11:48:03.000000 json_timeseries-0.1.4/.readthedocs.yml
+-rw-r--r--   0 slavapisarevskiy   (501) staff       (20)     1074 2023-03-28 00:27:02.000000 json_timeseries-0.1.4/LICENSE
+-rw-r--r--   0 slavapisarevskiy   (501) staff       (20)     5024 2023-05-20 08:45:54.396899 json_timeseries-0.1.4/PKG-INFO
+-rw-r--r--   0 slavapisarevskiy   (501) staff       (20)     4142 2023-05-14 11:43:08.000000 json_timeseries-0.1.4/README.md
+-rw-r--r--   0 slavapisarevskiy   (501) staff       (20)      126 2023-05-20 08:17:50.000000 json_timeseries-0.1.4/build.sh
+drwxr-xr-x   0 slavapisarevskiy   (501) staff       (20)        0 2023-05-20 08:45:54.361071 json_timeseries-0.1.4/docs/
+-rw-r--r--   0 slavapisarevskiy   (501) staff       (20)      634 2023-05-07 04:38:02.000000 json_timeseries-0.1.4/docs/Makefile
+-rw-r--r--   0 slavapisarevskiy   (501) staff       (20)     1185 2023-05-14 10:33:09.000000 json_timeseries-0.1.4/docs/conf.py
+-rw-r--r--   0 slavapisarevskiy   (501) staff       (20)      518 2023-05-14 11:54:21.000000 json_timeseries-0.1.4/docs/index.rst
+-rw-r--r--   0 slavapisarevskiy   (501) staff       (20)      800 2023-05-07 04:38:02.000000 json_timeseries-0.1.4/docs/make.bat
+-rw-r--r--   0 slavapisarevskiy   (501) staff       (20)       16 2023-05-14 11:48:31.000000 json_timeseries-0.1.4/docs/requirements.txt
+drwxr-xr-x   0 slavapisarevskiy   (501) staff       (20)        0 2023-05-20 08:45:54.365147 json_timeseries-0.1.4/docs/source/
+drwxr-xr-x   0 slavapisarevskiy   (501) staff       (20)        0 2023-05-20 08:45:54.368336 json_timeseries-0.1.4/docs/source/api/
+-rw-r--r--   0 slavapisarevskiy   (501) staff       (20)      311 2023-05-14 10:42:36.000000 json_timeseries-0.1.4/docs/source/api/jts.rst
+-rw-r--r--   0 slavapisarevskiy   (501) staff       (20)       31 2023-05-14 10:41:37.000000 json_timeseries-0.1.4/docs/source/readme.rst
+drwxr-xr-x   0 slavapisarevskiy   (501) staff       (20)        0 2023-05-20 08:45:54.373315 json_timeseries-0.1.4/json_timeseries/
+-rw-r--r--   0 slavapisarevskiy   (501) staff       (20)      128 2023-05-09 07:13:32.000000 json_timeseries-0.1.4/json_timeseries/__init__.py
+-rw-r--r--   0 slavapisarevskiy   (501) staff       (20)     9014 2023-05-20 08:42:36.000000 json_timeseries-0.1.4/json_timeseries/jts.py
+drwxr-xr-x   0 slavapisarevskiy   (501) staff       (20)        0 2023-05-20 08:45:54.390838 json_timeseries-0.1.4/json_timeseries.egg-info/
+-rw-r--r--   0 slavapisarevskiy   (501) staff       (20)     5024 2023-05-20 08:45:54.000000 json_timeseries-0.1.4/json_timeseries.egg-info/PKG-INFO
+-rw-r--r--   0 slavapisarevskiy   (501) staff       (20)      514 2023-05-20 08:45:54.000000 json_timeseries-0.1.4/json_timeseries.egg-info/SOURCES.txt
+-rw-r--r--   0 slavapisarevskiy   (501) staff       (20)        1 2023-05-20 08:45:54.000000 json_timeseries-0.1.4/json_timeseries.egg-info/dependency_links.txt
+-rw-r--r--   0 slavapisarevskiy   (501) staff       (20)       16 2023-05-20 08:45:54.000000 json_timeseries-0.1.4/json_timeseries.egg-info/requires.txt
+-rw-r--r--   0 slavapisarevskiy   (501) staff       (20)       22 2023-05-20 08:45:54.000000 json_timeseries-0.1.4/json_timeseries.egg-info/top_level.txt
+-rw-r--r--   0 slavapisarevskiy   (501) staff       (20)       99 2023-05-08 12:17:32.000000 json_timeseries-0.1.4/pyproject.toml
+-rw-r--r--   0 slavapisarevskiy   (501) staff       (20)       15 2023-05-07 12:04:18.000000 json_timeseries-0.1.4/requirements.txt
+-rw-r--r--   0 slavapisarevskiy   (501) staff       (20)     1049 2023-05-20 08:45:54.405702 json_timeseries-0.1.4/setup.cfg
+drwxr-xr-x   0 slavapisarevskiy   (501) staff       (20)        0 2023-05-20 08:45:54.395310 json_timeseries-0.1.4/tests/
+-rw-r--r--   0 slavapisarevskiy   (501) staff       (20)        0 2023-03-30 00:31:15.000000 json_timeseries-0.1.4/tests/__init__.py
+-rw-r--r--   0 slavapisarevskiy   (501) staff       (20)    11646 2023-05-20 08:15:14.000000 json_timeseries-0.1.4/tests/test_json_timeseries.py
```

### Comparing `json_timeseries-0.1.3/.gitignore` & `json_timeseries-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `json_timeseries-0.1.3/.readthedocs.yml` & `json_timeseries-0.1.4/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `json_timeseries-0.1.3/LICENSE` & `json_timeseries-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `json_timeseries-0.1.3/PKG-INFO` & `json_timeseries-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json_timeseries
-Version: 0.1.3
+Version: 0.1.4
 Summary: JSON-TimeSeries (JTS specification) handling library
 Home-page: https://github.com/slaxor505/json-timeseries-py
 Author: Slava Pisarevskiy
 Author-email: slava@plantbook.io
 License: MIT
 Project-URL: Documentation, https://json-timeseries-py.readthedocs.io
 Project-URL: Source, https://github.com/slaxor505/json-timeseries-py
```

### Comparing `json_timeseries-0.1.3/README.md` & `json_timeseries-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `json_timeseries-0.1.3/docs/Makefile` & `json_timeseries-0.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `json_timeseries-0.1.3/docs/conf.py` & `json_timeseries-0.1.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `json_timeseries-0.1.3/docs/index.rst` & `json_timeseries-0.1.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `json_timeseries-0.1.3/docs/make.bat` & `json_timeseries-0.1.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `json_timeseries-0.1.3/json_timeseries/jts.py` & `json_timeseries-0.1.4/json_timeseries/jts.py`

 * *Files 0% similar despite different names*

```diff
@@ -173,23 +173,25 @@
 
     def __len__(self):
         return self.series.__len__()
 
     def toJSON(self) -> dict:
         """
         Output as dictionary of JSON structure
+
         :return: Python dictionary of JSON structure
         :rtype: dict
         """
         # return json.dumps(self.__build())
         return self.__build()
 
-    def toJSONString(self):
+    def toJSONString(self) -> str:
         """
         Output as stringified JSON (json.dumps)
+
         :return: Output as stringified JSON
         :rtype: str
         """
         return json.dumps(self.toJSON())
 
     def __build(self):
         doc = dict(docType='jts',
```

### Comparing `json_timeseries-0.1.3/json_timeseries.egg-info/PKG-INFO` & `json_timeseries-0.1.4/json_timeseries.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-timeseries
-Version: 0.1.3
+Version: 0.1.4
 Summary: JSON-TimeSeries (JTS specification) handling library
 Home-page: https://github.com/slaxor505/json-timeseries-py
 Author: Slava Pisarevskiy
 Author-email: slava@plantbook.io
 License: MIT
 Project-URL: Documentation, https://json-timeseries-py.readthedocs.io
 Project-URL: Source, https://github.com/slaxor505/json-timeseries-py
```

### Comparing `json_timeseries-0.1.3/json_timeseries.egg-info/SOURCES.txt` & `json_timeseries-0.1.4/json_timeseries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `json_timeseries-0.1.3/setup.cfg` & `json_timeseries-0.1.4/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = json_timeseries
-version = 0.1.3
+version = 0.1.4
 author = Slava Pisarevskiy
 author_email = slava@plantbook.io
 description = JSON-TimeSeries (JTS specification) handling library
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/slaxor505/json-timeseries-py
 keywords = json, timeseries, iot, jts
```

### Comparing `json_timeseries-0.1.3/tests/test_json_timeseries.py` & `json_timeseries-0.1.4/tests/test_json_timeseries.py`

 * *Files identical despite different names*

