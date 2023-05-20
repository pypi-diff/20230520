# Comparing `tmp/json_timeseries-0.1.2.tar.gz` & `tmp/json_timeseries-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json_timeseries-0.1.2.tar", last modified: Wed May 10 03:33:49 2023, max compression
+gzip compressed data, was "json_timeseries-0.1.3.tar", last modified: Sat May 20 08:18:50 2023, max compression
```

## Comparing `json_timeseries-0.1.2.tar` & `json_timeseries-0.1.3.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxr-xr-x   0 slavapisarevskiy   (501) staff       (20)        0 2023-05-10 03:33:49.899918 json_timeseries-0.1.2/
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)     1857 2023-05-07 05:16:13.000000 json_timeseries-0.1.2/.gitignore
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)      550 2023-05-09 07:47:05.000000 json_timeseries-0.1.2/.readthedocs.yml
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)     1074 2023-03-28 00:27:02.000000 json_timeseries-0.1.2/LICENSE
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)     4523 2023-05-10 03:33:49.900226 json_timeseries-0.1.2/PKG-INFO
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)     3640 2023-05-09 11:10:18.000000 json_timeseries-0.1.2/README.md
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)      197 2023-05-09 12:11:35.000000 json_timeseries-0.1.2/build.sh
-drwxr-xr-x   0 slavapisarevskiy   (501) staff       (20)        0 2023-05-10 03:33:49.865345 json_timeseries-0.1.2/docs/
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)      634 2023-05-07 04:38:02.000000 json_timeseries-0.1.2/docs/Makefile
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)     1180 2023-05-09 12:16:22.000000 json_timeseries-0.1.2/docs/conf.py
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)      532 2023-05-08 11:47:16.000000 json_timeseries-0.1.2/docs/index.rst
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)      800 2023-05-07 04:38:02.000000 json_timeseries-0.1.2/docs/make.bat
-drwxr-xr-x   0 slavapisarevskiy   (501) staff       (20)        0 2023-05-10 03:33:49.823971 json_timeseries-0.1.2/docs/source/
-drwxr-xr-x   0 slavapisarevskiy   (501) staff       (20)        0 2023-05-10 03:33:49.869922 json_timeseries-0.1.2/docs/source/api/
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)      304 2023-05-09 07:18:07.000000 json_timeseries-0.1.2/docs/source/api/jts.rst
-drwxr-xr-x   0 slavapisarevskiy   (501) staff       (20)        0 2023-05-10 03:33:49.882420 json_timeseries-0.1.2/json_timeseries/
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)      128 2023-05-09 07:13:32.000000 json_timeseries-0.1.2/json_timeseries/__init__.py
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)     8509 2023-05-09 07:19:41.000000 json_timeseries-0.1.2/json_timeseries/jts.py
-drwxr-xr-x   0 slavapisarevskiy   (501) staff       (20)        0 2023-05-10 03:33:49.892206 json_timeseries-0.1.2/json_timeseries.egg-info/
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)     4523 2023-05-10 03:33:49.000000 json_timeseries-0.1.2/json_timeseries.egg-info/PKG-INFO
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)      469 2023-05-10 03:33:49.000000 json_timeseries-0.1.2/json_timeseries.egg-info/SOURCES.txt
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)        1 2023-05-10 03:33:49.000000 json_timeseries-0.1.2/json_timeseries.egg-info/dependency_links.txt
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)       16 2023-05-10 03:33:49.000000 json_timeseries-0.1.2/json_timeseries.egg-info/requires.txt
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)       22 2023-05-10 03:33:49.000000 json_timeseries-0.1.2/json_timeseries.egg-info/top_level.txt
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)       99 2023-05-08 12:17:32.000000 json_timeseries-0.1.2/pyproject.toml
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)       15 2023-05-07 12:04:18.000000 json_timeseries-0.1.2/requirements.txt
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)     1049 2023-05-10 03:33:49.903355 json_timeseries-0.1.2/setup.cfg
-drwxr-xr-x   0 slavapisarevskiy   (501) staff       (20)        0 2023-05-10 03:33:49.899123 json_timeseries-0.1.2/tests/
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)        0 2023-03-30 00:31:15.000000 json_timeseries-0.1.2/tests/__init__.py
--rw-r--r--   0 slavapisarevskiy   (501) staff       (20)    11640 2023-05-09 07:12:59.000000 json_timeseries-0.1.2/tests/test_json_timeseries.py
+drwxr-xr-x   0 slavapisarevskiy   (501) staff       (20)        0 2023-05-20 08:18:50.312203 json_timeseries-0.1.3/
+-rw-r--r--   0 slavapisarevskiy   (501) staff       (20)     1857 2023-05-07 05:16:13.000000 json_timeseries-0.1.3/.gitignore
+-rw-r--r--   0 slavapisarevskiy   (501) staff       (20)      592 2023-05-14 11:48:03.000000 json_timeseries-0.1.3/.readthedocs.yml
+-rw-r--r--   0 slavapisarevskiy   (501) staff       (20)     1074 2023-03-28 00:27:02.000000 json_timeseries-0.1.3/LICENSE
+-rw-r--r--   0 slavapisarevskiy   (501) staff       (20)     5024 2023-05-20 08:18:50.312816 json_timeseries-0.1.3/PKG-INFO
+-rw-r--r--   0 slavapisarevskiy   (501) staff       (20)     4142 2023-05-14 11:43:08.000000 json_timeseries-0.1.3/README.md
+-rw-r--r--   0 slavapisarevskiy   (501) staff       (20)      126 2023-05-20 08:17:50.000000 json_timeseries-0.1.3/build.sh
+drwxr-xr-x   0 slavapisarevskiy   (501) staff       (20)        0 2023-05-20 08:18:50.260610 json_timeseries-0.1.3/docs/
+-rw-r--r--   0 slavapisarevskiy   (501) staff       (20)      634 2023-05-07 04:38:02.000000 json_timeseries-0.1.3/docs/Makefile
+-rw-r--r--   0 slavapisarevskiy   (501) staff       (20)     1185 2023-05-14 10:33:09.000000 json_timeseries-0.1.3/docs/conf.py
+-rw-r--r--   0 slavapisarevskiy   (501) staff       (20)      518 2023-05-14 11:54:21.000000 json_timeseries-0.1.3/docs/index.rst
+-rw-r--r--   0 slavapisarevskiy   (501) staff       (20)      800 2023-05-07 04:38:02.000000 json_timeseries-0.1.3/docs/make.bat
+-rw-r--r--   0 slavapisarevskiy   (501) staff       (20)       16 2023-05-14 11:48:31.000000 json_timeseries-0.1.3/docs/requirements.txt
+drwxr-xr-x   0 slavapisarevskiy   (501) staff       (20)        0 2023-05-20 08:18:50.269828 json_timeseries-0.1.3/docs/source/
+drwxr-xr-x   0 slavapisarevskiy   (501) staff       (20)        0 2023-05-20 08:18:50.277924 json_timeseries-0.1.3/docs/source/api/
+-rw-r--r--   0 slavapisarevskiy   (501) staff       (20)      311 2023-05-14 10:42:36.000000 json_timeseries-0.1.3/docs/source/api/jts.rst
+-rw-r--r--   0 slavapisarevskiy   (501) staff       (20)       31 2023-05-14 10:41:37.000000 json_timeseries-0.1.3/docs/source/readme.rst
+drwxr-xr-x   0 slavapisarevskiy   (501) staff       (20)        0 2023-05-20 08:18:50.285117 json_timeseries-0.1.3/json_timeseries/
+-rw-r--r--   0 slavapisarevskiy   (501) staff       (20)      128 2023-05-09 07:13:32.000000 json_timeseries-0.1.3/json_timeseries/__init__.py
+-rw-r--r--   0 slavapisarevskiy   (501) staff       (20)     9005 2023-05-20 08:16:54.000000 json_timeseries-0.1.3/json_timeseries/jts.py
+drwxr-xr-x   0 slavapisarevskiy   (501) staff       (20)        0 2023-05-20 08:18:50.304065 json_timeseries-0.1.3/json_timeseries.egg-info/
+-rw-r--r--   0 slavapisarevskiy   (501) staff       (20)     5024 2023-05-20 08:18:50.000000 json_timeseries-0.1.3/json_timeseries.egg-info/PKG-INFO
+-rw-r--r--   0 slavapisarevskiy   (501) staff       (20)      514 2023-05-20 08:18:50.000000 json_timeseries-0.1.3/json_timeseries.egg-info/SOURCES.txt
+-rw-r--r--   0 slavapisarevskiy   (501) staff       (20)        1 2023-05-20 08:18:50.000000 json_timeseries-0.1.3/json_timeseries.egg-info/dependency_links.txt
+-rw-r--r--   0 slavapisarevskiy   (501) staff       (20)       16 2023-05-20 08:18:50.000000 json_timeseries-0.1.3/json_timeseries.egg-info/requires.txt
+-rw-r--r--   0 slavapisarevskiy   (501) staff       (20)       22 2023-05-20 08:18:50.000000 json_timeseries-0.1.3/json_timeseries.egg-info/top_level.txt
+-rw-r--r--   0 slavapisarevskiy   (501) staff       (20)       99 2023-05-08 12:17:32.000000 json_timeseries-0.1.3/pyproject.toml
+-rw-r--r--   0 slavapisarevskiy   (501) staff       (20)       15 2023-05-07 12:04:18.000000 json_timeseries-0.1.3/requirements.txt
+-rw-r--r--   0 slavapisarevskiy   (501) staff       (20)     1049 2023-05-20 08:18:50.322976 json_timeseries-0.1.3/setup.cfg
+drwxr-xr-x   0 slavapisarevskiy   (501) staff       (20)        0 2023-05-20 08:18:50.309816 json_timeseries-0.1.3/tests/
+-rw-r--r--   0 slavapisarevskiy   (501) staff       (20)        0 2023-03-30 00:31:15.000000 json_timeseries-0.1.3/tests/__init__.py
+-rw-r--r--   0 slavapisarevskiy   (501) staff       (20)    11646 2023-05-20 08:15:14.000000 json_timeseries-0.1.3/tests/test_json_timeseries.py
```

### Comparing `json_timeseries-0.1.2/.gitignore` & `json_timeseries-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `json_timeseries-0.1.2/.readthedocs.yml` & `json_timeseries-0.1.3/.readthedocs.yml`

 * *Files 16% similar despite different names*

```diff
@@ -16,8 +16,9 @@
 # Optionally build your docs in additional formats such as PDF and ePub
 formats: all
 
 # ReadTheDocs.io need to install the dependencies to be able
 # to build the documentation automatically.
 python:
   install:
-    - requirements: requirements.txt
+    - requirements: requirements.txt
+    - requirements: docs/requirements.txt
```

### Comparing `json_timeseries-0.1.2/LICENSE` & `json_timeseries-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `json_timeseries-0.1.2/PKG-INFO` & `json_timeseries-0.1.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,13 @@
-Metadata-Version: 2.1
-Name: json_timeseries
-Version: 0.1.2
-Summary: JSON-TimeSeries (JTS specification) handling library
-Home-page: https://github.com/slaxor505/json-timeseries-py
-Author: Slava Pisarevskiy
-Author-email: slava@plantbook.io
-License: MIT
-Project-URL: Documentation, https://json-timeseries-py.readthedocs.io
-Project-URL: Source, https://github.com/slaxor505/json-timeseries-py
-Project-URL: Specification, https://docs.eagle.io/en/latest/reference/historic/jts.html
-Keywords: json,timeseries,iot,jts
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
+# JSON Time Series
 
-# JSON - time series
-JSON Time Series (JTS specification) handling Python library
+[![Documentation Status](https://readthedocs.org/projects/json-timeseries-py/badge/?version=latest)](https://json-timeseries-py.readthedocs.io/en/latest/?badge=latest)
+[![PyPI version](https://badge.fury.io/py/json-timeseries.svg)](https://badge.fury.io/py/json-timeseries)
 
-# Time Series
-
-> Time Series data construction, manipulation and serialisation.
+[JSON Time Series](https://docs.eagle.io/en/latest/reference/historic/jts.html) (JTS specification) handling Python library - Time Series data construction, manipulation and serialisation.
 
 ## Installation
 
 ```shell
 pip install json-timeseries
 ```
 
@@ -105,19 +83,19 @@
 - `timestamp`: date object. Type of datetime. e.g.`datetime.now()`
 - `value` *(optional)*:  number, string, date, null
 - `quality` *(optional)*: number (quality code) associated with value
 - `annotation` (optional): string description or comment related to the record
 
 ### Methods 
 
-See full documentation.
+See [full documentation](https://json-timeseries-py.readthedocs.io).
 
 ### Properties
 
-See full documentation.
+See [full documentation](https://json-timeseries-py.readthedocs.io).
 
 
 
 ## JTS Document
 
 `JtsDocument` is a class for outputting `TimeSeries` in 
 [JSON Time Series](https://docs.eagle.io/en/latest/reference/historic/jts.html) document format.
@@ -132,15 +110,15 @@
 
 ### Options
 
 - `series`: array of `TimeSeries` to include in JTS Document
 
 ### Methods 
 
-See full documentation.
+See [full documentation](https://json-timeseries-py.readthedocs.io).
 
 ### Properties
 
-See full documentation.
+See [full documentation](https://json-timeseries-py.readthedocs.io).
 
 ## License
 MIT
```

### Comparing `json_timeseries-0.1.2/docs/Makefile` & `json_timeseries-0.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `json_timeseries-0.1.2/docs/conf.py` & `json_timeseries-0.1.3/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 copyright = '2023, Slava Pisarevskiy'
 author = 'Slava Pisarevskiy'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
-    'recommonmark',
     'sphinx.ext.autodoc',
-    'sphinx.ext.viewcode'
+    'sphinx.ext.viewcode',
+    'sphinx_mdinclude',
 ]
 
 templates_path = ['_templates']
 exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
```

### Comparing `json_timeseries-0.1.2/docs/make.bat` & `json_timeseries-0.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `json_timeseries-0.1.2/json_timeseries/jts.py` & `json_timeseries-0.1.3/json_timeseries/jts.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,21 +4,31 @@
 from typing import Union, List
 
 from dateutil import parser
 
 TimeSeriesDataType = ('NUMBER', 'TEXT', 'TIME', 'COORDINATES')
 
 
-
 class TsRecord:
     """
-    Record of TimeSeries object
+    A record of TimeSeries object
+
+    :param timestamp: Timestamp
+    :type timestamp: datetime
+    :param value: Value
+    :type value: Union[float, str, int]
+    :param quality: Quality
+    :type quality: int
+    :param annotation: Annotation
+    :type annotation: str
     """
+
     def __init__(self, timestamp: datetime, value: Union[float, str, int], quality: int = None,
                  annotation: str = None):
+        # TODO 1: enforce value types
         self.timestamp = timestamp
         self.value = value
         self.quality = quality
         self.annotation = annotation
 
 
 def __datetimeconverter(m):
@@ -57,14 +67,17 @@
         else:
             raise TypeError("'records' value must be TsRecord or List[TsRecord]")
 
     # def __eq__(self, other):
     #     return self.__dict__ is other.__dict__
 
     def insert(self, records: Union[TsRecord, List[TsRecord]]):
+        """
+        Insert single or multiple records
+        """
 
         if isinstance(records, list):
             self.records.extend(records)
         # single instance
         else:
             self.records.append(records)
 
@@ -76,18 +89,19 @@
     #     pass
 
     def __len__(self):
         return self.records.__len__()
 
     def toJSON(self) -> str:
         """
-        Outputs JSON string
+        Outputs formatted JSON
         """
         return json.dumps(self, default=__datetimeconverter)
 
+
 # TODO METHODS to implement
 #
 #   def get_timestamps:
 #
 #   public sort (): TimeSeries<Type> {
 #
 #   public clone (): TimeSeries<Type> {
@@ -96,26 +110,27 @@
 #
 #   private valueToJSON (value: Type | undefined): Type | undefined | string | null {
 #
 #   private cloneRecords (records: ITimeSeriesRecord<Type>[]): ITimeSeriesRecord<Type>[] {
 
 
 class JtsDocument:
+    pass
+
+
+class JtsDocument:
     """
     JTS document object
 
     :raise [TypeError]: [Value of 'series' must be types of TimeSeries or List[TimeSeries]]
     """
 
     """
     TODO Methods to implement
 
-    // Output as stringified JSON
-    jtsDocument.toString()
-
     // Clone document (also clones series)
     jtsDocument.clone()
 
     // Create a new jtsDocument from JSON
     const jtsDocument = JtsDocument.from('{"docType": "jts", ...}')
 
     Properties
@@ -155,19 +170,30 @@
         # single instance
         else:
             self.series.append(series)
 
     def __len__(self):
         return self.series.__len__()
 
-    def toJSON(self) -> str:
+    def toJSON(self) -> dict:
         """
-        Output as formatted JSON
+        Output as dictionary of JSON structure
+        :return: Python dictionary of JSON structure
+        :rtype: dict
         """
-        return json.dumps(self.__build())
+        # return json.dumps(self.__build())
+        return self.__build()
+
+    def toJSONString(self):
+        """
+        Output as stringified JSON (json.dumps)
+        :return: Output as stringified JSON
+        :rtype: str
+        """
+        return json.dumps(self.toJSON())
 
     def __build(self):
         doc = dict(docType='jts',
                    version=self.version)
 
         data = self.__get_data()
         if not data:
@@ -237,15 +263,19 @@
 
         if r.annotation:
             column["a"] = r.annotation
 
         return column
 
     @staticmethod
-    def fromJSON(json_str):
+    def fromJSON(json_str: str) -> JtsDocument:
+        """
+        Create a new jtsDocument from JSON
+        """
+
         json_obj = json.loads(json_str)
 
         jts_doc = JtsDocument(version=json_obj.get('version'))
 
         # build series from header columns
         for idx, c in json_obj['header']["columns"].items():
             jts_doc.addSeries(TimeSeries(
@@ -273,19 +303,11 @@
                 #     raise Exception("Data columns do not match Header columns")
 
         return jts_doc
 
     def getSeries(self, identifier: str) -> TimeSeries:
         """
         Get series by id
-        :param identifier: 
-        :type identifier: 
-        :return: 
-        :rtype: 
         """
 
-
+        # TODO: return list of found series
         return next((x for x in self.series if x.identifier == identifier), None)
-
-# TODO check if I need extra methods then publish and rewrite OPB API using the library
-# TODO all type hints of public API
-# TODO DOCS - read.me from eagle rewrite and any necessary docs
```

### Comparing `json_timeseries-0.1.2/json_timeseries.egg-info/PKG-INFO` & `json_timeseries-0.1.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: json-timeseries
-Version: 0.1.2
+Name: json_timeseries
+Version: 0.1.3
 Summary: JSON-TimeSeries (JTS specification) handling library
 Home-page: https://github.com/slaxor505/json-timeseries-py
 Author: Slava Pisarevskiy
 Author-email: slava@plantbook.io
 License: MIT
 Project-URL: Documentation, https://json-timeseries-py.readthedocs.io
 Project-URL: Source, https://github.com/slaxor505/json-timeseries-py
@@ -16,20 +16,20 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# JSON - time series
-JSON Time Series (JTS specification) handling Python library
+# JSON Time Series
 
-# Time Series
+[![Documentation Status](https://readthedocs.org/projects/json-timeseries-py/badge/?version=latest)](https://json-timeseries-py.readthedocs.io/en/latest/?badge=latest)
+[![PyPI version](https://badge.fury.io/py/json-timeseries.svg)](https://badge.fury.io/py/json-timeseries)
 
-> Time Series data construction, manipulation and serialisation.
+[JSON Time Series](https://docs.eagle.io/en/latest/reference/historic/jts.html) (JTS specification) handling Python library - Time Series data construction, manipulation and serialisation.
 
 ## Installation
 
 ```shell
 pip install json-timeseries
 ```
 
@@ -105,19 +105,19 @@
 - `timestamp`: date object. Type of datetime. e.g.`datetime.now()`
 - `value` *(optional)*:  number, string, date, null
 - `quality` *(optional)*: number (quality code) associated with value
 - `annotation` (optional): string description or comment related to the record
 
 ### Methods 
 
-See full documentation.
+See [full documentation](https://json-timeseries-py.readthedocs.io).
 
 ### Properties
 
-See full documentation.
+See [full documentation](https://json-timeseries-py.readthedocs.io).
 
 
 
 ## JTS Document
 
 `JtsDocument` is a class for outputting `TimeSeries` in 
 [JSON Time Series](https://docs.eagle.io/en/latest/reference/historic/jts.html) document format.
@@ -132,15 +132,15 @@
 
 ### Options
 
 - `series`: array of `TimeSeries` to include in JTS Document
 
 ### Methods 
 
-See full documentation.
+See [full documentation](https://json-timeseries-py.readthedocs.io).
 
 ### Properties
 
-See full documentation.
+See [full documentation](https://json-timeseries-py.readthedocs.io).
 
 ## License
 MIT
```

### Comparing `json_timeseries-0.1.2/setup.cfg` & `json_timeseries-0.1.3/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = json_timeseries
-version = 0.1.2
+version = 0.1.3
 author = Slava Pisarevskiy
 author_email = slava@plantbook.io
 description = JSON-TimeSeries (JTS specification) handling library
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/slaxor505/json-timeseries-py
 keywords = json, timeseries, iot, jts
```

### Comparing `json_timeseries-0.1.2/tests/test_json_timeseries.py` & `json_timeseries-0.1.3/tests/test_json_timeseries.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,15 @@
                 }
             ]
         }
         """)
 
         jts_str = t.substitute(ONE_MINUTE_AGO=self.ONE_MINUTE_AGO.isoformat(),
                                NOW=self.NOW.isoformat())
-        jts_payload = jts_document.toJSON()
+        jts_payload = jts_document.toJSONString()
         self.assertEqual(jts_payload, json.dumps(json.loads(jts_str)))
 
     def test_fromJSON(self):
         timeseries1 = TimeSeries(identifier='series_1', name='Series 1', data_type='NUMBER', records=[
             TsRecord(**{"timestamp": self.ONE_MINUTE_AGO, "value": '1.23', "quality": 192, "annotation": 'comment'}),
             TsRecord(**{"timestamp": self.NOW, "value": '2.34', "quality": 245, "annotation": 'comment number 2'})]
                                  )
```

