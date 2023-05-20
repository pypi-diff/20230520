# Comparing `tmp/streamflow-postgresql-0.0.1.tar.gz` & `tmp/streamflow-postgresql-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamflow-postgresql-0.0.1.tar", last modified: Sat May  6 16:20:49 2023, max compression
+gzip compressed data, was "streamflow-postgresql-0.0.2.tar", last modified: Sat May 20 18:13:26 2023, max compression
```

## Comparing `streamflow-postgresql-0.0.1.tar` & `streamflow-postgresql-0.0.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 glassofwhiskey  (1000) glassofwhiskey  (1000)        0 2023-05-06 16:20:49.943488 streamflow-postgresql-0.0.1/
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)     7652 2023-01-25 20:14:18.000000 streamflow-postgresql-0.0.1/LICENSE
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)      151 2023-05-06 08:13:01.000000 streamflow-postgresql-0.0.1/MANIFEST.in
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)     2370 2023-05-06 16:20:49.943488 streamflow-postgresql-0.0.1/PKG-INFO
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)     1184 2023-05-06 08:15:39.000000 streamflow-postgresql-0.0.1/README.md
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)       13 2023-04-22 09:55:51.000000 streamflow-postgresql-0.0.1/bandit-requirements.txt
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)       71 2023-04-30 09:01:56.000000 streamflow-postgresql-0.0.1/lint-requirements.txt
-drwxrwxr-x   0 glassofwhiskey  (1000) glassofwhiskey  (1000)        0 2023-05-06 16:20:49.943488 streamflow-postgresql-0.0.1/postgresql/
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)        0 2023-04-30 18:53:59.000000 streamflow-postgresql-0.0.1/postgresql/__init__.py
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)    24413 2023-05-06 13:57:27.000000 streamflow-postgresql-0.0.1/postgresql/database.py
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)      254 2023-04-30 20:47:45.000000 streamflow-postgresql-0.0.1/postgresql/plugin.py
-drwxrwxr-x   0 glassofwhiskey  (1000) glassofwhiskey  (1000)        0 2023-05-06 16:20:49.943488 streamflow-postgresql-0.0.1/postgresql/schemas/
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)     1013 2023-05-05 18:56:01.000000 streamflow-postgresql-0.0.1/postgresql/schemas/postgresql.json
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)     2025 2023-05-06 13:54:37.000000 streamflow-postgresql-0.0.1/postgresql/schemas/postgresql.sql
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)       18 2023-04-30 19:12:27.000000 streamflow-postgresql-0.0.1/postgresql/version.py
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)     1754 2023-05-06 08:12:38.000000 streamflow-postgresql-0.0.1/pyproject.toml
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)       51 2023-05-06 15:50:01.000000 streamflow-postgresql-0.0.1/requirements.txt
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)       38 2023-05-06 16:20:49.943488 streamflow-postgresql-0.0.1/setup.cfg
-drwxrwxr-x   0 glassofwhiskey  (1000) glassofwhiskey  (1000)        0 2023-05-06 16:20:49.943488 streamflow-postgresql-0.0.1/streamflow_postgresql.egg-info/
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)     2370 2023-05-06 16:20:49.000000 streamflow-postgresql-0.0.1/streamflow_postgresql.egg-info/PKG-INFO
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)      625 2023-05-06 16:20:49.000000 streamflow-postgresql-0.0.1/streamflow_postgresql.egg-info/SOURCES.txt
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)        1 2023-05-06 16:20:49.000000 streamflow-postgresql-0.0.1/streamflow_postgresql.egg-info/dependency_links.txt
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)       84 2023-05-06 16:20:49.000000 streamflow-postgresql-0.0.1/streamflow_postgresql.egg-info/entry_points.txt
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)      239 2023-05-06 16:20:49.000000 streamflow-postgresql-0.0.1/streamflow_postgresql.egg-info/requires.txt
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)       11 2023-05-06 16:20:49.000000 streamflow-postgresql-0.0.1/streamflow_postgresql.egg-info/top_level.txt
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)        1 2023-05-06 15:45:16.000000 streamflow-postgresql-0.0.1/streamflow_postgresql.egg-info/zip-safe
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)       75 2023-05-06 08:12:13.000000 streamflow-postgresql-0.0.1/test-requirements.txt
-drwxrwxr-x   0 glassofwhiskey  (1000) glassofwhiskey  (1000)        0 2023-05-06 16:20:49.943488 streamflow-postgresql-0.0.1/tests/
--rw-rw-r--   0 glassofwhiskey  (1000) glassofwhiskey  (1000)    10836 2023-05-06 08:09:30.000000 streamflow-postgresql-0.0.1/tests/test_persistence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:13:26.691495 streamflow-postgresql-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-20 18:13:09.000000 streamflow-postgresql-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-20 18:13:09.000000 streamflow-postgresql-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-20 18:13:26.691495 streamflow-postgresql-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-05-20 18:13:09.000000 streamflow-postgresql-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-20 18:13:09.000000 streamflow-postgresql-0.0.2/bandit-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-20 18:13:09.000000 streamflow-postgresql-0.0.2/lint-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:13:26.687495 streamflow-postgresql-0.0.2/postgresql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 18:13:09.000000 streamflow-postgresql-0.0.2/postgresql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24413 2023-05-20 18:13:09.000000 streamflow-postgresql-0.0.2/postgresql/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-20 18:13:09.000000 streamflow-postgresql-0.0.2/postgresql/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:13:26.687495 streamflow-postgresql-0.0.2/postgresql/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-20 18:13:09.000000 streamflow-postgresql-0.0.2/postgresql/schemas/postgresql.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-20 18:13:09.000000 streamflow-postgresql-0.0.2/postgresql/schemas/postgresql.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-20 18:13:09.000000 streamflow-postgresql-0.0.2/postgresql/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-20 18:13:09.000000 streamflow-postgresql-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-20 18:13:09.000000 streamflow-postgresql-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 18:13:26.691495 streamflow-postgresql-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:13:26.691495 streamflow-postgresql-0.0.2/streamflow_postgresql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-20 18:13:26.000000 streamflow-postgresql-0.0.2/streamflow_postgresql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-20 18:13:26.000000 streamflow-postgresql-0.0.2/streamflow_postgresql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 18:13:26.000000 streamflow-postgresql-0.0.2/streamflow_postgresql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-20 18:13:26.000000 streamflow-postgresql-0.0.2/streamflow_postgresql.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-20 18:13:26.000000 streamflow-postgresql-0.0.2/streamflow_postgresql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-20 18:13:26.000000 streamflow-postgresql-0.0.2/streamflow_postgresql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 18:13:26.000000 streamflow-postgresql-0.0.2/streamflow_postgresql.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-20 18:13:09.000000 streamflow-postgresql-0.0.2/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:13:26.691495 streamflow-postgresql-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-05-20 18:13:09.000000 streamflow-postgresql-0.0.2/tests/test_persistence.py
```

### Comparing `streamflow-postgresql-0.0.1/LICENSE` & `streamflow-postgresql-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `streamflow-postgresql-0.0.1/PKG-INFO` & `streamflow-postgresql-0.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamflow-postgresql
-Version: 0.0.1
+Version: 0.0.2
 Summary: StreamFlow PostgreSQL plugin
 Author-email: Iacopo Colonnelli <iacopo.colonnelli@unito.it>
 License: LGPL-3.0-or-later
 Project-URL: Package, https://pypi.org/project/streamflow-postgresql
 Project-URL: Repository, https://github.com/alpha-unito/streamflow-postgresql
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
@@ -27,32 +27,32 @@
 Provides-Extra: test
 License-File: LICENSE
 
 # PostgreSQL Plugin for StreamFlow
 
 ## Installation
 
-Simply install the package directory from [this repository](https://github.com/alpha-unito/streamflow-postgresql) using [pip](https://pip.pypa.io/en/stable/). StreamFlow will automatically recognise it as a plugin and load it at each workflow execution.
+Simply install the package directory from [PyPI](https://pypi.org/project/streamflow-postgresql/) using [pip](https://pip.pypa.io/en/stable/). StreamFlow will automatically recognise it as a plugin and load it at each workflow execution.
 
 ```bash
-pip install streamflow-postgresql@git+https://github.com/alpha-unito/streamflow-postgresql
+pip install streamflow-postgresql
 ```
 
 If everything worked correctly, whenever a workflow execution start the following message should be printed in the log:
 
 ```bash
 Successfully registered plugin postgresql.plugin.PostgreSQLStreamFlowPlugin
 ```
 
 ## Usage
 
 This plugin registers a new `Database` component, which extends the StreamFlow `CachedDatabase` class. To declare it, put the following lines inside a `streamflow.yml` configuration file.
 
 ```yaml
 database:
-  type: postgresql
+  type: unito.postgresql
   config:
     dbname: <dbname>               # The name of the database to use
     hostname: <hostname>           # The database hostname or IP address
     password: <password>           # Password to use when connecting to the database
     username: <username>           # Username to use when connecting to the database
 ```
```

### Comparing `streamflow-postgresql-0.0.1/README.md` & `streamflow-postgresql-0.0.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # PostgreSQL Plugin for StreamFlow
 
 ## Installation
 
-Simply install the package directory from [this repository](https://github.com/alpha-unito/streamflow-postgresql) using [pip](https://pip.pypa.io/en/stable/). StreamFlow will automatically recognise it as a plugin and load it at each workflow execution.
+Simply install the package directory from [PyPI](https://pypi.org/project/streamflow-postgresql/) using [pip](https://pip.pypa.io/en/stable/). StreamFlow will automatically recognise it as a plugin and load it at each workflow execution.
 
 ```bash
-pip install streamflow-postgresql@git+https://github.com/alpha-unito/streamflow-postgresql
+pip install streamflow-postgresql
 ```
 
 If everything worked correctly, whenever a workflow execution start the following message should be printed in the log:
 
 ```bash
 Successfully registered plugin postgresql.plugin.PostgreSQLStreamFlowPlugin
 ```
 
 ## Usage
 
 This plugin registers a new `Database` component, which extends the StreamFlow `CachedDatabase` class. To declare it, put the following lines inside a `streamflow.yml` configuration file.
 
 ```yaml
 database:
-  type: postgresql
+  type: unito.postgresql
   config:
     dbname: <dbname>               # The name of the database to use
     hostname: <hostname>           # The database hostname or IP address
     password: <password>           # Password to use when connecting to the database
     username: <username>           # Username to use when connecting to the database
 ```
```

### Comparing `streamflow-postgresql-0.0.1/postgresql/database.py` & `streamflow-postgresql-0.0.2/postgresql/database.py`

 * *Files identical despite different names*

### Comparing `streamflow-postgresql-0.0.1/postgresql/schemas/postgresql.json` & `streamflow-postgresql-0.0.2/postgresql/schemas/postgresql.json`

 * *Files identical despite different names*

### Comparing `streamflow-postgresql-0.0.1/postgresql/schemas/postgresql.sql` & `streamflow-postgresql-0.0.2/postgresql/schemas/postgresql.sql`

 * *Files identical despite different names*

### Comparing `streamflow-postgresql-0.0.1/pyproject.toml` & `streamflow-postgresql-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 dynamic = ["dependencies", "optional-dependencies", "version"]
 
 [project.urls]
 Package = "https://pypi.org/project/streamflow-postgresql"
 Repository = "https://github.com/alpha-unito/streamflow-postgresql"
 
 [project.entry-points]
-"unito.streamflow.plugin" = {postgresql = "postgresql.plugin:PostgreSQLStreamFlowPlugin"}
+"unito.streamflow.plugin" = {"unito.postgresql" = "postgresql.plugin:PostgreSQLStreamFlowPlugin"}
 
 
 [tool.setuptools]
 packages = [
     "postgresql"
 ]
 zip-safe = true
```

### Comparing `streamflow-postgresql-0.0.1/streamflow_postgresql.egg-info/PKG-INFO` & `streamflow-postgresql-0.0.2/streamflow_postgresql.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamflow-postgresql
-Version: 0.0.1
+Version: 0.0.2
 Summary: StreamFlow PostgreSQL plugin
 Author-email: Iacopo Colonnelli <iacopo.colonnelli@unito.it>
 License: LGPL-3.0-or-later
 Project-URL: Package, https://pypi.org/project/streamflow-postgresql
 Project-URL: Repository, https://github.com/alpha-unito/streamflow-postgresql
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
@@ -27,32 +27,32 @@
 Provides-Extra: test
 License-File: LICENSE
 
 # PostgreSQL Plugin for StreamFlow
 
 ## Installation
 
-Simply install the package directory from [this repository](https://github.com/alpha-unito/streamflow-postgresql) using [pip](https://pip.pypa.io/en/stable/). StreamFlow will automatically recognise it as a plugin and load it at each workflow execution.
+Simply install the package directory from [PyPI](https://pypi.org/project/streamflow-postgresql/) using [pip](https://pip.pypa.io/en/stable/). StreamFlow will automatically recognise it as a plugin and load it at each workflow execution.
 
 ```bash
-pip install streamflow-postgresql@git+https://github.com/alpha-unito/streamflow-postgresql
+pip install streamflow-postgresql
 ```
 
 If everything worked correctly, whenever a workflow execution start the following message should be printed in the log:
 
 ```bash
 Successfully registered plugin postgresql.plugin.PostgreSQLStreamFlowPlugin
 ```
 
 ## Usage
 
 This plugin registers a new `Database` component, which extends the StreamFlow `CachedDatabase` class. To declare it, put the following lines inside a `streamflow.yml` configuration file.
 
 ```yaml
 database:
-  type: postgresql
+  type: unito.postgresql
   config:
     dbname: <dbname>               # The name of the database to use
     hostname: <hostname>           # The database hostname or IP address
     password: <password>           # Password to use when connecting to the database
     username: <username>           # Username to use when connecting to the database
 ```
```

### Comparing `streamflow-postgresql-0.0.1/streamflow_postgresql.egg-info/SOURCES.txt` & `streamflow-postgresql-0.0.2/streamflow_postgresql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `streamflow-postgresql-0.0.1/tests/test_persistence.py` & `streamflow-postgresql-0.0.2/tests/test_persistence.py`

 * *Files identical despite different names*

