# Comparing `tmp/logica-1.3.2.tar.gz` & `tmp/logica-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/logica-1.3.2.tar", last modified: Mon Oct 12 16:24:26 2020, max compression
+gzip compressed data, was "dist/logica-1.3.9.tar", last modified: Wed Oct 14 21:05:58 2020, max compression
```

## Comparing `logica-1.3.2.tar` & `logica-1.3.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 evgenys  (95425) primarygroup (89939)        0 2020-10-12 16:24:26.000000 logica-1.3.2/
--rw-r--r--   0 evgenys  (95425) primarygroup (89939)     6415 2020-10-12 16:24:26.000000 logica-1.3.2/PKG-INFO
-drwxr-xr-x   0 evgenys  (95425) primarygroup (89939)        0 2020-10-12 16:24:26.000000 logica-1.3.2/logica.egg-info/
--rw-r--r--   0 evgenys  (95425) primarygroup (89939)     6415 2020-10-12 16:24:25.000000 logica-1.3.2/logica.egg-info/PKG-INFO
--rw-r--r--   0 evgenys  (95425) primarygroup (89939)      633 2020-10-12 16:24:25.000000 logica-1.3.2/logica.egg-info/SOURCES.txt
--rw-r--r--   0 evgenys  (95425) primarygroup (89939)       51 2020-10-12 16:24:25.000000 logica-1.3.2/logica.egg-info/entry_points.txt
--rw-r--r--   0 evgenys  (95425) primarygroup (89939)        7 2020-10-12 16:24:25.000000 logica-1.3.2/logica.egg-info/top_level.txt
--rw-r--r--   0 evgenys  (95425) primarygroup (89939)        1 2020-10-12 16:24:25.000000 logica-1.3.2/logica.egg-info/dependency_links.txt
--rw-r--r--   0 evgenys  (95425) primarygroup (89939)      657 2020-10-12 16:24:09.000000 logica-1.3.2/setup.py
-drwxr-xr-x   0 evgenys  (95425) primarygroup (89939)        0 2020-10-12 16:24:26.000000 logica-1.3.2/logica/
-drwxr-xr-x   0 evgenys  (95425) primarygroup (89939)        0 2020-10-12 16:24:26.000000 logica-1.3.2/logica/parser_py/
--rwxr-xr-x   0 evgenys  (95425) primarygroup (89939)    47666 2020-10-12 04:14:56.000000 logica-1.3.2/logica/parser_py/parse.py
-drwxr-xr-x   0 evgenys  (95425) primarygroup (89939)        0 2020-10-12 16:24:26.000000 logica-1.3.2/logica/integration_tests/
--rwxr-xr-x   0 evgenys  (95425) primarygroup (89939)     5508 2020-10-12 04:14:56.000000 logica-1.3.2/logica/integration_tests/run_tests.py
-drwxr-xr-x   0 evgenys  (95425) primarygroup (89939)        0 2020-10-12 16:24:26.000000 logica-1.3.2/logica/integration_tests/import_tests/
--rwxr-xr-x   0 evgenys  (95425) primarygroup (89939)     1806 2020-10-12 04:14:56.000000 logica-1.3.2/logica/integration_tests/import_tests/run_tests.py
--rwxr-xr-x   0 evgenys  (95425) primarygroup (89939)     3291 2020-10-12 04:14:56.000000 logica-1.3.2/logica/colab_logica.py
-drwxr-xr-x   0 evgenys  (95425) primarygroup (89939)        0 2020-10-12 16:24:26.000000 logica-1.3.2/logica/common/
--rw-r--r--   0 evgenys  (95425) primarygroup (89939)     2839 2020-10-12 04:14:56.000000 logica-1.3.2/logica/common/logica_lib.py
--rwxr-xr-x   0 evgenys  (95425) primarygroup (89939)     1386 2020-10-12 04:14:56.000000 logica-1.3.2/logica/common/color.py
--rw-r--r--   0 evgenys  (95425) primarygroup (89939)     2470 2020-10-12 04:14:56.000000 logica-1.3.2/logica/common/logica_test.py
-drwxr-xr-x   0 evgenys  (95425) primarygroup (89939)        0 2020-10-12 16:24:26.000000 logica-1.3.2/logica/common/data/
--rwxr-xr-x   0 evgenys  (95425) primarygroup (89939)    11596 2020-10-12 04:14:56.000000 logica-1.3.2/logica/common/data/processed_functions.py
--rwxr-xr-x   0 evgenys  (95425) primarygroup (89939)     1186 2020-10-12 04:14:56.000000 logica-1.3.2/logica/run_all_tests.py
-drwxr-xr-x   0 evgenys  (95425) primarygroup (89939)        0 2020-10-12 16:24:26.000000 logica-1.3.2/logica/compiler/
--rwxr-xr-x   0 evgenys  (95425) primarygroup (89939)    10908 2020-10-12 04:14:56.000000 logica-1.3.2/logica/compiler/functors.py
--rwxr-xr-x   0 evgenys  (95425) primarygroup (89939)    41814 2020-10-12 04:14:56.000000 logica-1.3.2/logica/compiler/universe.py
--rwxr-xr-x   0 evgenys  (95425) primarygroup (89939)    26320 2020-10-12 04:14:56.000000 logica-1.3.2/logica/compiler/rule_translate.py
--rwxr-xr-x   0 evgenys  (95425) primarygroup (89939)     1989 2020-10-12 04:14:56.000000 logica-1.3.2/logica/compiler/dialects.py
--rwxr-xr-x   0 evgenys  (95425) primarygroup (89939)    20245 2020-10-12 04:14:56.000000 logica-1.3.2/logica/compiler/expr_translate.py
--rw-r--r--   0 evgenys  (95425) primarygroup (89939)       74 2020-10-12 06:53:47.000000 logica-1.3.2/logica/__main__.py
--rwxr-xr-x   0 evgenys  (95425) primarygroup (89939)     5845 2020-10-12 15:42:32.000000 logica-1.3.2/logica/logica.py
--rw-r--r--   0 evgenys  (95425) primarygroup (89939)       38 2020-10-12 16:24:26.000000 logica-1.3.2/setup.cfg
+drwxr-xr-x   0 evgenys  (95425) primarygroup (89939)        0 2020-10-14 21:05:58.000000 logica-1.3.9/
+-rw-r--r--   0 evgenys  (95425) primarygroup (89939)     9334 2020-10-14 21:05:58.000000 logica-1.3.9/PKG-INFO
+drwxr-xr-x   0 evgenys  (95425) primarygroup (89939)        0 2020-10-14 21:05:58.000000 logica-1.3.9/logica.egg-info/
+-rw-r--r--   0 evgenys  (95425) primarygroup (89939)     9334 2020-10-14 21:05:57.000000 logica-1.3.9/logica.egg-info/PKG-INFO
+-rw-r--r--   0 evgenys  (95425) primarygroup (89939)      633 2020-10-14 21:05:57.000000 logica-1.3.9/logica.egg-info/SOURCES.txt
+-rw-r--r--   0 evgenys  (95425) primarygroup (89939)       51 2020-10-14 21:05:57.000000 logica-1.3.9/logica.egg-info/entry_points.txt
+-rw-r--r--   0 evgenys  (95425) primarygroup (89939)        7 2020-10-14 21:05:57.000000 logica-1.3.9/logica.egg-info/top_level.txt
+-rw-r--r--   0 evgenys  (95425) primarygroup (89939)        1 2020-10-14 21:05:57.000000 logica-1.3.9/logica.egg-info/dependency_links.txt
+-rw-r--r--   0 evgenys  (95425) primarygroup (89939)      657 2020-10-14 21:05:47.000000 logica-1.3.9/setup.py
+drwxr-xr-x   0 evgenys  (95425) primarygroup (89939)        0 2020-10-14 21:05:58.000000 logica-1.3.9/logica/
+drwxr-xr-x   0 evgenys  (95425) primarygroup (89939)        0 2020-10-14 21:05:58.000000 logica-1.3.9/logica/parser_py/
+-rwxr-xr-x   0 evgenys  (95425) primarygroup (89939)    47666 2020-10-14 21:04:24.000000 logica-1.3.9/logica/parser_py/parse.py
+drwxr-xr-x   0 evgenys  (95425) primarygroup (89939)        0 2020-10-14 21:05:58.000000 logica-1.3.9/logica/integration_tests/
+-rwxr-xr-x   0 evgenys  (95425) primarygroup (89939)     5508 2020-10-14 21:04:24.000000 logica-1.3.9/logica/integration_tests/run_tests.py
+drwxr-xr-x   0 evgenys  (95425) primarygroup (89939)        0 2020-10-14 21:05:58.000000 logica-1.3.9/logica/integration_tests/import_tests/
+-rwxr-xr-x   0 evgenys  (95425) primarygroup (89939)     1806 2020-10-14 21:04:23.000000 logica-1.3.9/logica/integration_tests/import_tests/run_tests.py
+-rwxr-xr-x   0 evgenys  (95425) primarygroup (89939)     3781 2020-10-14 21:04:23.000000 logica-1.3.9/logica/colab_logica.py
+drwxr-xr-x   0 evgenys  (95425) primarygroup (89939)        0 2020-10-14 21:05:58.000000 logica-1.3.9/logica/common/
+-rw-r--r--   0 evgenys  (95425) primarygroup (89939)     2839 2020-10-14 21:04:23.000000 logica-1.3.9/logica/common/logica_lib.py
+-rwxr-xr-x   0 evgenys  (95425) primarygroup (89939)     1386 2020-10-14 21:04:23.000000 logica-1.3.9/logica/common/color.py
+-rw-r--r--   0 evgenys  (95425) primarygroup (89939)     2470 2020-10-14 21:04:23.000000 logica-1.3.9/logica/common/logica_test.py
+drwxr-xr-x   0 evgenys  (95425) primarygroup (89939)        0 2020-10-14 21:05:58.000000 logica-1.3.9/logica/common/data/
+-rwxr-xr-x   0 evgenys  (95425) primarygroup (89939)    11596 2020-10-14 21:04:23.000000 logica-1.3.9/logica/common/data/processed_functions.py
+-rwxr-xr-x   0 evgenys  (95425) primarygroup (89939)     1186 2020-10-14 21:04:24.000000 logica-1.3.9/logica/run_all_tests.py
+drwxr-xr-x   0 evgenys  (95425) primarygroup (89939)        0 2020-10-14 21:05:58.000000 logica-1.3.9/logica/compiler/
+-rwxr-xr-x   0 evgenys  (95425) primarygroup (89939)    10908 2020-10-14 21:04:23.000000 logica-1.3.9/logica/compiler/functors.py
+-rwxr-xr-x   0 evgenys  (95425) primarygroup (89939)    41814 2020-10-14 21:04:23.000000 logica-1.3.9/logica/compiler/universe.py
+-rwxr-xr-x   0 evgenys  (95425) primarygroup (89939)    26320 2020-10-14 21:04:23.000000 logica-1.3.9/logica/compiler/rule_translate.py
+-rwxr-xr-x   0 evgenys  (95425) primarygroup (89939)     1989 2020-10-14 21:04:23.000000 logica-1.3.9/logica/compiler/dialects.py
+-rwxr-xr-x   0 evgenys  (95425) primarygroup (89939)    20245 2020-10-14 21:04:23.000000 logica-1.3.9/logica/compiler/expr_translate.py
+-rw-r--r--   0 evgenys  (95425) primarygroup (89939)      670 2020-10-14 21:04:30.000000 logica-1.3.9/logica/__main__.py
+-rwxr-xr-x   0 evgenys  (95425) primarygroup (89939)     5845 2020-10-14 21:04:24.000000 logica-1.3.9/logica/logica.py
+-rw-r--r--   0 evgenys  (95425) primarygroup (89939)       38 2020-10-14 21:05:58.000000 logica-1.3.9/setup.cfg
```

### Comparing `logica-1.3.2/logica.egg-info/SOURCES.txt` & `logica-1.3.9/logica.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `logica-1.3.2/setup.py` & `logica-1.3.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("logica/README.md", "r") as f:
   long_description = f.read()
 
 setuptools.setup(
   name = "logica",
-  version = "1.3.2",
+  version = "1.3.9",
   author = "Evgeny Skvortsov",
   author_email = "logica@evgeny.ninja",
   description = "Logica language.",
   long_description = long_description,
   long_description_content_type = "text/markdown",
   url="https://github.com/evgskv/logica",
   packages=setuptools.find_namespace_packages(),
```

### Comparing `logica-1.3.2/logica/parser_py/parse.py` & `logica-1.3.9/logica/parser_py/parse.py`

 * *Files identical despite different names*

### Comparing `logica-1.3.2/logica/integration_tests/run_tests.py` & `logica-1.3.9/logica/integration_tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `logica-1.3.2/logica/integration_tests/import_tests/run_tests.py` & `logica-1.3.9/logica/integration_tests/import_tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `logica-1.3.2/logica/colab_logica.py` & `logica-1.3.9/logica/colab_logica.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,29 +27,45 @@
 from IPython.display import display
 
 import pandas
 
 from .parser_py import parse
 
 from google.cloud import bigquery
+from google.colab import auth
 from google.colab import widgets
 
 
 PROJECT = None
 
 DB_CONNECTION = None
 
+USER_AUTHENTICATED = False
+
 def SetProject(project):
   global PROJECT
   PROJECT = project
 
 def SetDbConnection(connection):
   global DB_CONNECTION
   DB_CONNECTION = connection
 
+def EnsureAuthenticatedUser():
+  global USER_AUTHENTICATED
+  global PROJECT
+  if USER_AUTHENTICATED:
+    return
+  auth.authenticate_user()
+  if PROJECT is None:
+    print("Please enter project_id to use for BigQuery querries.")
+    PROJECT = input()
+    print("project_id is set to %s" % PROJECT)
+    print("You can change it with logica.colab_logica.SetProject command.")
+  USER_AUTHENTICATED = True
+
 
 @register_cell_magic
 def logica(line, cell):
   Logica(line, cell, run_query=True)
 
 
 def ParseList(line):
@@ -59,14 +75,15 @@
   else:
     predicates = [p.strip() for p in line.split(',')]
   return predicates
 
 
 def RunSQL(sql, engine):
   if engine == 'bigquery':
+    EnsureAuthenticatedUser()
     client = bigquery.Client(project=PROJECT)
     return client.query(sql).to_dataframe()
   elif engine == 'psql':
     return pandas.read_sql(sql, DB_CONNECTION)
   else:
     raise Exception('Logica colab only supports BigQuery and PostgreSQL '
                     'for now.')
```

### Comparing `logica-1.3.2/logica/common/logica_lib.py` & `logica-1.3.9/logica/common/logica_lib.py`

 * *Files identical despite different names*

### Comparing `logica-1.3.2/logica/common/color.py` & `logica-1.3.9/logica/common/color.py`

 * *Files identical despite different names*

### Comparing `logica-1.3.2/logica/common/logica_test.py` & `logica-1.3.9/logica/common/logica_test.py`

 * *Files identical despite different names*

### Comparing `logica-1.3.2/logica/common/data/processed_functions.py` & `logica-1.3.9/logica/common/data/processed_functions.py`

 * *Files identical despite different names*

### Comparing `logica-1.3.2/logica/run_all_tests.py` & `logica-1.3.9/logica/run_all_tests.py`

 * *Files identical despite different names*

### Comparing `logica-1.3.2/logica/compiler/functors.py` & `logica-1.3.9/logica/compiler/functors.py`

 * *Files identical despite different names*

### Comparing `logica-1.3.2/logica/compiler/universe.py` & `logica-1.3.9/logica/compiler/universe.py`

 * *Files identical despite different names*

### Comparing `logica-1.3.2/logica/compiler/rule_translate.py` & `logica-1.3.9/logica/compiler/rule_translate.py`

 * *Files identical despite different names*

### Comparing `logica-1.3.2/logica/compiler/dialects.py` & `logica-1.3.9/logica/compiler/dialects.py`

 * *Files identical despite different names*

### Comparing `logica-1.3.2/logica/compiler/expr_translate.py` & `logica-1.3.9/logica/compiler/expr_translate.py`

 * *Files identical despite different names*

### Comparing `logica-1.3.2/logica/logica.py` & `logica-1.3.9/logica/logica.py`

 * *Files identical despite different names*

