# Comparing `tmp/flaskosql-1.1.10.tar.gz` & `tmp/flaskosql-1.2.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flaskosql-1.1.10.tar", last modified: Sat May 20 00:29:44 2023, max compression
+gzip compressed data, was "flaskosql-1.2.10.tar", last modified: Sat May 20 00:30:39 2023, max compression
```

## Comparing `flaskosql-1.1.10.tar` & `flaskosql-1.2.10.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 00:29:44.253454 flaskosql-1.1.10/
--rw-rw-rw-   0        0        0        0 2023-05-19 18:59:18.000000 flaskosql-1.1.10/LICENSE
--rw-rw-rw-   0        0        0     4913 2023-05-20 00:29:44.250432 flaskosql-1.1.10/PKG-INFO
--rw-rw-rw-   0        0        0     4218 2023-05-20 00:29:16.000000 flaskosql-1.1.10/README.md
-drwxrwxrwx   0        0        0        0 2023-05-20 00:29:44.222456 flaskosql-1.1.10/flaskosql/
--rw-rw-rw-   0        0        0        0 2023-05-19 23:56:14.000000 flaskosql-1.1.10/flaskosql/__init__.py
--rw-rw-rw-   0        0        0      631 2023-05-19 19:33:50.000000 flaskosql-1.1.10/flaskosql/db.py
--rw-rw-rw-   0        0        0      887 2023-05-19 23:21:47.000000 flaskosql-1.1.10/flaskosql/field.py
--rw-rw-rw-   0        0        0     6477 2023-05-19 23:55:04.000000 flaskosql-1.1.10/flaskosql/model.py
-drwxrwxrwx   0        0        0        0 2023-05-20 00:29:44.245439 flaskosql-1.1.10/flaskosql.egg-info/
--rw-rw-rw-   0        0        0     4913 2023-05-20 00:29:43.000000 flaskosql-1.1.10/flaskosql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-05-20 00:29:44.000000 flaskosql-1.1.10/flaskosql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 00:29:43.000000 flaskosql-1.1.10/flaskosql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-20 00:29:43.000000 flaskosql-1.1.10/flaskosql.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-20 00:29:43.000000 flaskosql-1.1.10/flaskosql.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-20 00:29:44.254452 flaskosql-1.1.10/setup.cfg
--rw-rw-rw-   0        0        0     1210 2023-05-20 00:29:31.000000 flaskosql-1.1.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 00:30:39.908074 flaskosql-1.2.10/
+-rw-rw-rw-   0        0        0        0 2023-05-19 18:59:18.000000 flaskosql-1.2.10/LICENSE
+-rw-rw-rw-   0        0        0     4877 2023-05-20 00:30:39.906405 flaskosql-1.2.10/PKG-INFO
+-rw-rw-rw-   0        0        0     4182 2023-05-20 00:30:22.000000 flaskosql-1.2.10/README.md
+drwxrwxrwx   0        0        0        0 2023-05-20 00:30:39.877640 flaskosql-1.2.10/flaskosql/
+-rw-rw-rw-   0        0        0        0 2023-05-19 23:56:14.000000 flaskosql-1.2.10/flaskosql/__init__.py
+-rw-rw-rw-   0        0        0      631 2023-05-19 19:33:50.000000 flaskosql-1.2.10/flaskosql/db.py
+-rw-rw-rw-   0        0        0      887 2023-05-19 23:21:47.000000 flaskosql-1.2.10/flaskosql/field.py
+-rw-rw-rw-   0        0        0     6477 2023-05-19 23:55:04.000000 flaskosql-1.2.10/flaskosql/model.py
+drwxrwxrwx   0        0        0        0 2023-05-20 00:30:39.901045 flaskosql-1.2.10/flaskosql.egg-info/
+-rw-rw-rw-   0        0        0     4877 2023-05-20 00:30:39.000000 flaskosql-1.2.10/flaskosql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-05-20 00:30:39.000000 flaskosql-1.2.10/flaskosql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 00:30:39.000000 flaskosql-1.2.10/flaskosql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-20 00:30:39.000000 flaskosql-1.2.10/flaskosql.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-20 00:30:39.000000 flaskosql-1.2.10/flaskosql.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-20 00:30:39.909044 flaskosql-1.2.10/setup.cfg
+-rw-rw-rw-   0        0        0     1210 2023-05-20 00:30:32.000000 flaskosql-1.2.10/setup.py
```

### Comparing `flaskosql-1.1.10/PKG-INFO` & `flaskosql-1.2.10/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: flaskosql
-Version: 1.1.10
+Version: 1.2.10
 Summary: ORM for ORACLE DB for FLASK API 
 Author: Ashraf khabar
 Author-email: <khabarachraf@gmail.com>
 Keywords: python,orm,api,oracle,database,flask
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-# <center style="color:#963">FlaskoSQL</center>
+# FlaskoSQL
 
 
 [![PyPI version](https://badge.fury.io/py/package-name.svg)](https://badge.fury.io/py/package-name) [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 
 Description
 -----------
```

### Comparing `flaskosql-1.1.10/README.md` & `flaskosql-1.2.10/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# <center style="color:#963">FlaskoSQL</center>
+# FlaskoSQL
 
 
 [![PyPI version](https://badge.fury.io/py/package-name.svg)](https://badge.fury.io/py/package-name) [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 
 Description
 -----------
```

### Comparing `flaskosql-1.1.10/flaskosql/db.py` & `flaskosql-1.2.10/flaskosql/db.py`

 * *Files identical despite different names*

### Comparing `flaskosql-1.1.10/flaskosql/field.py` & `flaskosql-1.2.10/flaskosql/field.py`

 * *Files identical despite different names*

### Comparing `flaskosql-1.1.10/flaskosql/model.py` & `flaskosql-1.2.10/flaskosql/model.py`

 * *Files identical despite different names*

### Comparing `flaskosql-1.1.10/flaskosql.egg-info/PKG-INFO` & `flaskosql-1.2.10/flaskosql.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: flaskosql
-Version: 1.1.10
+Version: 1.2.10
 Summary: ORM for ORACLE DB for FLASK API 
 Author: Ashraf khabar
 Author-email: <khabarachraf@gmail.com>
 Keywords: python,orm,api,oracle,database,flask
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-# <center style="color:#963">FlaskoSQL</center>
+# FlaskoSQL
 
 
 [![PyPI version](https://badge.fury.io/py/package-name.svg)](https://badge.fury.io/py/package-name) [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 
 Description
 -----------
```

### Comparing `flaskosql-1.1.10/setup.py` & `flaskosql-1.2.10/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.1.10'
+VERSION = '1.2.10'
 DESCRIPTION = 'ORM for ORACLE DB for FLASK API '
 LONG_DESCRIPTION = 'An ORM that allow us to connect with the ORACLE DB using OOP concept, plus the interaction with the database in order to create a rest API using FLASK framwork '
 
 # Setting up
 setup(
     name="flaskosql",
     version=VERSION,
```

