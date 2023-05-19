# Comparing `tmp/flaskosql-1.0.5.tar.gz` & `tmp/flaskosql-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flaskosql-1.0.5.tar", last modified: Fri May 19 22:16:23 2023, max compression
+gzip compressed data, was "flaskosql-1.0.6.tar", last modified: Fri May 19 23:39:04 2023, max compression
```

## Comparing `flaskosql-1.0.5.tar` & `flaskosql-1.0.6.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 22:16:23.699104 flaskosql-1.0.5/
--rw-rw-rw-   0        0        0        0 2023-05-19 18:59:18.000000 flaskosql-1.0.5/LICENSE
--rw-rw-rw-   0        0        0      799 2023-05-19 22:16:23.697107 flaskosql-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-05-19 18:59:18.000000 flaskosql-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 22:16:23.669105 flaskosql-1.0.5/flaskosql/
--rw-rw-rw-   0        0        0        0 2023-05-19 19:34:12.000000 flaskosql-1.0.5/flaskosql/__init__.py
--rw-rw-rw-   0        0        0      631 2023-05-19 19:33:50.000000 flaskosql-1.0.5/flaskosql/db.py
--rw-rw-rw-   0        0        0      887 2023-05-19 18:59:18.000000 flaskosql-1.0.5/flaskosql/field.py
--rw-rw-rw-   0        0        0     6467 2023-05-19 22:15:36.000000 flaskosql-1.0.5/flaskosql/model.py
-drwxrwxrwx   0        0        0        0 2023-05-19 22:16:23.693136 flaskosql-1.0.5/flaskosql.egg-info/
--rw-rw-rw-   0        0        0      799 2023-05-19 22:16:23.000000 flaskosql-1.0.5/flaskosql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-05-19 22:16:23.000000 flaskosql-1.0.5/flaskosql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 22:16:23.000000 flaskosql-1.0.5/flaskosql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-19 22:16:23.000000 flaskosql-1.0.5/flaskosql.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-19 22:16:23.000000 flaskosql-1.0.5/flaskosql.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-19 22:16:23.699104 flaskosql-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1208 2023-05-19 22:15:58.000000 flaskosql-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 23:39:04.043144 flaskosql-1.0.6/
+-rw-rw-rw-   0        0        0        0 2023-05-19 18:59:18.000000 flaskosql-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0      800 2023-05-19 23:39:04.042174 flaskosql-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-05-19 18:59:18.000000 flaskosql-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-19 23:39:04.015136 flaskosql-1.0.6/flaskosql/
+-rw-rw-rw-   0        0        0        0 2023-05-19 19:34:12.000000 flaskosql-1.0.6/flaskosql/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 23:39:04.039094 flaskosql-1.0.6/flaskosql/columns/
+-rw-rw-rw-   0        0        0        0 2023-05-19 23:35:36.000000 flaskosql-1.0.6/flaskosql/columns/__init__.py
+-rw-rw-rw-   0        0        0      887 2023-05-19 23:21:47.000000 flaskosql-1.0.6/flaskosql/columns/field.py
+-rw-rw-rw-   0        0        0      631 2023-05-19 19:33:50.000000 flaskosql-1.0.6/flaskosql/db.py
+-rw-rw-rw-   0        0        0     6475 2023-05-19 23:35:57.000000 flaskosql-1.0.6/flaskosql/model.py
+drwxrwxrwx   0        0        0        0 2023-05-19 23:39:04.032065 flaskosql-1.0.6/flaskosql.egg-info/
+-rw-rw-rw-   0        0        0      800 2023-05-19 23:39:03.000000 flaskosql-1.0.6/flaskosql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2023-05-19 23:39:03.000000 flaskosql-1.0.6/flaskosql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 23:39:03.000000 flaskosql-1.0.6/flaskosql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-19 23:39:03.000000 flaskosql-1.0.6/flaskosql.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-19 23:39:03.000000 flaskosql-1.0.6/flaskosql.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-19 23:39:04.044112 flaskosql-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1209 2023-05-19 23:38:22.000000 flaskosql-1.0.6/setup.py
```

### Comparing `flaskosql-1.0.5/PKG-INFO` & `flaskosql-1.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: flaskosql
-Version: 1.0.5
-Summary: ORM for ORACLE DB for FLASK API
+Version: 1.0.6
+Summary: ORM for ORACLE DB for FLASK API 
 Author: Ashraf khabar
 Author-email: <khabarachraf@gmail.com>
 Keywords: python,orm,api,oracle,database,flask
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `flaskosql-1.0.5/flaskosql/db.py` & `flaskosql-1.0.6/flaskosql/db.py`

 * *Files identical despite different names*

### Comparing `flaskosql-1.0.5/flaskosql/field.py` & `flaskosql-1.0.6/flaskosql/columns/field.py`

 * *Files identical despite different names*

### Comparing `flaskosql-1.0.5/flaskosql/model.py` & `flaskosql-1.0.6/flaskosql/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import cx_Oracle
-from field import Field
+from columns.field import Field
 
 class Model:
     _connection = None
     
     # Constructor : it takes two arguments (self ("this" in other languages and *kwargs wich can be translated to string of values))
     def __init__(self, **kwargs):
         # Initialize the object with provided attributes
```

### Comparing `flaskosql-1.0.5/flaskosql.egg-info/PKG-INFO` & `flaskosql-1.0.6/flaskosql.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: flaskosql
-Version: 1.0.5
-Summary: ORM for ORACLE DB for FLASK API
+Version: 1.0.6
+Summary: ORM for ORACLE DB for FLASK API 
 Author: Ashraf khabar
 Author-email: <khabarachraf@gmail.com>
 Keywords: python,orm,api,oracle,database,flask
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `flaskosql-1.0.5/setup.py` & `flaskosql-1.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.5'
-DESCRIPTION = 'ORM for ORACLE DB for FLASK API'
+VERSION = '1.0.6'
+DESCRIPTION = 'ORM for ORACLE DB for FLASK API '
 LONG_DESCRIPTION = 'An ORM that allow us to connect with the ORACLE DB using OOP concept, plus the interaction with the database in order to create a rest API using FLASK framwork '
 
 # Setting up
 setup(
     name="flaskosql",
     version=VERSION,
     author="Ashraf khabar",
```

