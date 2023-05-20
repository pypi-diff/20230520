# Comparing `tmp/flaskosql-1.0.8.tar.gz` & `tmp/flaskosql-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flaskosql-1.0.8.tar", last modified: Fri May 19 23:55:29 2023, max compression
+gzip compressed data, was "flaskosql-1.0.9.tar", last modified: Fri May 19 23:56:25 2023, max compression
```

## Comparing `flaskosql-1.0.8.tar` & `flaskosql-1.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 23:55:29.916312 flaskosql-1.0.8/
--rw-rw-rw-   0        0        0        0 2023-05-19 18:59:18.000000 flaskosql-1.0.8/LICENSE
--rw-rw-rw-   0        0        0      800 2023-05-19 23:55:29.915321 flaskosql-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-05-19 18:59:18.000000 flaskosql-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 23:55:29.885137 flaskosql-1.0.8/flaskosql/
--rw-rw-rw-   0        0        0       72 2023-05-19 23:49:53.000000 flaskosql-1.0.8/flaskosql/__init__.py
--rw-rw-rw-   0        0        0      631 2023-05-19 19:33:50.000000 flaskosql-1.0.8/flaskosql/db.py
--rw-rw-rw-   0        0        0      887 2023-05-19 23:21:47.000000 flaskosql-1.0.8/flaskosql/field.py
--rw-rw-rw-   0        0        0     6477 2023-05-19 23:55:04.000000 flaskosql-1.0.8/flaskosql/model.py
-drwxrwxrwx   0        0        0        0 2023-05-19 23:55:29.911265 flaskosql-1.0.8/flaskosql.egg-info/
--rw-rw-rw-   0        0        0      800 2023-05-19 23:55:29.000000 flaskosql-1.0.8/flaskosql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-05-19 23:55:29.000000 flaskosql-1.0.8/flaskosql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 23:55:29.000000 flaskosql-1.0.8/flaskosql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-19 23:55:29.000000 flaskosql-1.0.8/flaskosql.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-19 23:55:29.000000 flaskosql-1.0.8/flaskosql.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-19 23:55:29.917310 flaskosql-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1209 2023-05-19 23:55:22.000000 flaskosql-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 23:56:25.096183 flaskosql-1.0.9/
+-rw-rw-rw-   0        0        0        0 2023-05-19 18:59:18.000000 flaskosql-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0      800 2023-05-19 23:56:25.095367 flaskosql-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-05-19 18:59:18.000000 flaskosql-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-19 23:56:25.074596 flaskosql-1.0.9/flaskosql/
+-rw-rw-rw-   0        0        0        0 2023-05-19 23:56:14.000000 flaskosql-1.0.9/flaskosql/__init__.py
+-rw-rw-rw-   0        0        0      631 2023-05-19 19:33:50.000000 flaskosql-1.0.9/flaskosql/db.py
+-rw-rw-rw-   0        0        0      887 2023-05-19 23:21:47.000000 flaskosql-1.0.9/flaskosql/field.py
+-rw-rw-rw-   0        0        0     6477 2023-05-19 23:55:04.000000 flaskosql-1.0.9/flaskosql/model.py
+drwxrwxrwx   0        0        0        0 2023-05-19 23:56:25.091168 flaskosql-1.0.9/flaskosql.egg-info/
+-rw-rw-rw-   0        0        0      800 2023-05-19 23:56:24.000000 flaskosql-1.0.9/flaskosql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-05-19 23:56:24.000000 flaskosql-1.0.9/flaskosql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 23:56:24.000000 flaskosql-1.0.9/flaskosql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-19 23:56:24.000000 flaskosql-1.0.9/flaskosql.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-19 23:56:24.000000 flaskosql-1.0.9/flaskosql.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-19 23:56:25.096183 flaskosql-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1209 2023-05-19 23:56:11.000000 flaskosql-1.0.9/setup.py
```

### Comparing `flaskosql-1.0.8/PKG-INFO` & `flaskosql-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flaskosql
-Version: 1.0.8
+Version: 1.0.9
 Summary: ORM for ORACLE DB for FLASK API 
 Author: Ashraf khabar
 Author-email: <khabarachraf@gmail.com>
 Keywords: python,orm,api,oracle,database,flask
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `flaskosql-1.0.8/flaskosql/db.py` & `flaskosql-1.0.9/flaskosql/db.py`

 * *Files identical despite different names*

### Comparing `flaskosql-1.0.8/flaskosql/field.py` & `flaskosql-1.0.9/flaskosql/field.py`

 * *Files identical despite different names*

### Comparing `flaskosql-1.0.8/flaskosql/model.py` & `flaskosql-1.0.9/flaskosql/model.py`

 * *Files identical despite different names*

### Comparing `flaskosql-1.0.8/flaskosql.egg-info/PKG-INFO` & `flaskosql-1.0.9/flaskosql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flaskosql
-Version: 1.0.8
+Version: 1.0.9
 Summary: ORM for ORACLE DB for FLASK API 
 Author: Ashraf khabar
 Author-email: <khabarachraf@gmail.com>
 Keywords: python,orm,api,oracle,database,flask
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `flaskosql-1.0.8/setup.py` & `flaskosql-1.0.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.8'
+VERSION = '1.0.9'
 DESCRIPTION = 'ORM for ORACLE DB for FLASK API '
 LONG_DESCRIPTION = 'An ORM that allow us to connect with the ORACLE DB using OOP concept, plus the interaction with the database in order to create a rest API using FLASK framwork '
 
 # Setting up
 setup(
     name="flaskosql",
     version=VERSION,
```

