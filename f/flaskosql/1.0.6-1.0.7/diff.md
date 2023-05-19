# Comparing `tmp/flaskosql-1.0.6.tar.gz` & `tmp/flaskosql-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flaskosql-1.0.6.tar", last modified: Fri May 19 23:39:04 2023, max compression
+gzip compressed data, was "flaskosql-1.0.7.tar", last modified: Fri May 19 23:50:14 2023, max compression
```

## Comparing `flaskosql-1.0.6.tar` & `flaskosql-1.0.7.tar`

### file list

```diff
@@ -1,19 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 23:39:04.043144 flaskosql-1.0.6/
--rw-rw-rw-   0        0        0        0 2023-05-19 18:59:18.000000 flaskosql-1.0.6/LICENSE
--rw-rw-rw-   0        0        0      800 2023-05-19 23:39:04.042174 flaskosql-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-05-19 18:59:18.000000 flaskosql-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 23:39:04.015136 flaskosql-1.0.6/flaskosql/
--rw-rw-rw-   0        0        0        0 2023-05-19 19:34:12.000000 flaskosql-1.0.6/flaskosql/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 23:39:04.039094 flaskosql-1.0.6/flaskosql/columns/
--rw-rw-rw-   0        0        0        0 2023-05-19 23:35:36.000000 flaskosql-1.0.6/flaskosql/columns/__init__.py
--rw-rw-rw-   0        0        0      887 2023-05-19 23:21:47.000000 flaskosql-1.0.6/flaskosql/columns/field.py
--rw-rw-rw-   0        0        0      631 2023-05-19 19:33:50.000000 flaskosql-1.0.6/flaskosql/db.py
--rw-rw-rw-   0        0        0     6475 2023-05-19 23:35:57.000000 flaskosql-1.0.6/flaskosql/model.py
-drwxrwxrwx   0        0        0        0 2023-05-19 23:39:04.032065 flaskosql-1.0.6/flaskosql.egg-info/
--rw-rw-rw-   0        0        0      800 2023-05-19 23:39:03.000000 flaskosql-1.0.6/flaskosql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      304 2023-05-19 23:39:03.000000 flaskosql-1.0.6/flaskosql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 23:39:03.000000 flaskosql-1.0.6/flaskosql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-19 23:39:03.000000 flaskosql-1.0.6/flaskosql.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-19 23:39:03.000000 flaskosql-1.0.6/flaskosql.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-19 23:39:04.044112 flaskosql-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1209 2023-05-19 23:38:22.000000 flaskosql-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 23:50:14.141264 flaskosql-1.0.7/
+-rw-rw-rw-   0        0        0        0 2023-05-19 18:59:18.000000 flaskosql-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0      800 2023-05-19 23:50:14.140909 flaskosql-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-05-19 18:59:18.000000 flaskosql-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-19 23:50:14.121193 flaskosql-1.0.7/flaskosql/
+-rw-rw-rw-   0        0        0       72 2023-05-19 23:49:53.000000 flaskosql-1.0.7/flaskosql/__init__.py
+-rw-rw-rw-   0        0        0      631 2023-05-19 19:33:50.000000 flaskosql-1.0.7/flaskosql/db.py
+-rw-rw-rw-   0        0        0      887 2023-05-19 23:21:47.000000 flaskosql-1.0.7/flaskosql/field.py
+-rw-rw-rw-   0        0        0     6467 2023-05-19 23:45:23.000000 flaskosql-1.0.7/flaskosql/model.py
+drwxrwxrwx   0        0        0        0 2023-05-19 23:50:14.137267 flaskosql-1.0.7/flaskosql.egg-info/
+-rw-rw-rw-   0        0        0      800 2023-05-19 23:50:13.000000 flaskosql-1.0.7/flaskosql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-05-19 23:50:13.000000 flaskosql-1.0.7/flaskosql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 23:50:13.000000 flaskosql-1.0.7/flaskosql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-19 23:50:13.000000 flaskosql-1.0.7/flaskosql.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-19 23:50:13.000000 flaskosql-1.0.7/flaskosql.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-19 23:50:14.142385 flaskosql-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1209 2023-05-19 23:50:05.000000 flaskosql-1.0.7/setup.py
```

### Comparing `flaskosql-1.0.6/PKG-INFO` & `flaskosql-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flaskosql
-Version: 1.0.6
+Version: 1.0.7
 Summary: ORM for ORACLE DB for FLASK API 
 Author: Ashraf khabar
 Author-email: <khabarachraf@gmail.com>
 Keywords: python,orm,api,oracle,database,flask
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `flaskosql-1.0.6/flaskosql/columns/field.py` & `flaskosql-1.0.7/flaskosql/field.py`

 * *Files identical despite different names*

### Comparing `flaskosql-1.0.6/flaskosql/db.py` & `flaskosql-1.0.7/flaskosql/db.py`

 * *Files identical despite different names*

### Comparing `flaskosql-1.0.6/flaskosql/model.py` & `flaskosql-1.0.7/flaskosql/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import cx_Oracle
-from columns.field import Field
+from field import Field
 
 class Model:
     _connection = None
     
     # Constructor : it takes two arguments (self ("this" in other languages and *kwargs wich can be translated to string of values))
     def __init__(self, **kwargs):
         # Initialize the object with provided attributes
```

### Comparing `flaskosql-1.0.6/flaskosql.egg-info/PKG-INFO` & `flaskosql-1.0.7/flaskosql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flaskosql
-Version: 1.0.6
+Version: 1.0.7
 Summary: ORM for ORACLE DB for FLASK API 
 Author: Ashraf khabar
 Author-email: <khabarachraf@gmail.com>
 Keywords: python,orm,api,oracle,database,flask
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `flaskosql-1.0.6/setup.py` & `flaskosql-1.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.6'
+VERSION = '1.0.7'
 DESCRIPTION = 'ORM for ORACLE DB for FLASK API '
 LONG_DESCRIPTION = 'An ORM that allow us to connect with the ORACLE DB using OOP concept, plus the interaction with the database in order to create a rest API using FLASK framwork '
 
 # Setting up
 setup(
     name="flaskosql",
     version=VERSION,
```

