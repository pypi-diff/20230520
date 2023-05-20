# Comparing `tmp/cdk-redisdb-0.0.22.tar.gz` & `tmp/cdk-redisdb-0.0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-redisdb-0.0.22.tar", last modified: Tue Apr 25 04:42:41 2023, max compression
+gzip compressed data, was "cdk-redisdb-0.0.23.tar", last modified: Sat May 20 09:07:20 2023, max compression
```

## Comparing `cdk-redisdb-0.0.22.tar` & `cdk-redisdb-0.0.23.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:42:41.353387 cdk-redisdb-0.0.22/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-25 04:42:27.000000 cdk-redisdb-0.0.22/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-25 04:42:27.000000 cdk-redisdb-0.0.22/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-04-25 04:42:41.353387 cdk-redisdb-0.0.22/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-04-25 04:42:27.000000 cdk-redisdb-0.0.22/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-25 04:42:27.000000 cdk-redisdb-0.0.22/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 04:42:41.353387 cdk-redisdb-0.0.22/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-25 04:42:27.000000 cdk-redisdb-0.0.22/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:42:41.349387 cdk-redisdb-0.0.22/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:42:41.353387 cdk-redisdb-0.0.22/src/cdk_redisdb/
--rw-r--r--   0 runner    (1001) docker     (123)    48408 2023-04-25 04:42:27.000000 cdk-redisdb-0.0.22/src/cdk_redisdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:42:41.353387 cdk-redisdb-0.0.22/src/cdk_redisdb/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-25 04:42:27.000000 cdk-redisdb-0.0.22/src/cdk_redisdb/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25933 2023-04-25 04:42:27.000000 cdk-redisdb-0.0.22/src/cdk_redisdb/_jsii/cdk-redisdb@0.0.22.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 04:42:27.000000 cdk-redisdb-0.0.22/src/cdk_redisdb/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:42:41.353387 cdk-redisdb-0.0.22/src/cdk_redisdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-04-25 04:42:41.000000 cdk-redisdb-0.0.22/src/cdk_redisdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-25 04:42:41.000000 cdk-redisdb-0.0.22/src/cdk_redisdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 04:42:41.000000 cdk-redisdb-0.0.22/src/cdk_redisdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-25 04:42:41.000000 cdk-redisdb-0.0.22/src/cdk_redisdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-25 04:42:41.000000 cdk-redisdb-0.0.22/src/cdk_redisdb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:07:20.837144 cdk-redisdb-0.0.23/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-20 09:07:04.000000 cdk-redisdb-0.0.23/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-20 09:07:04.000000 cdk-redisdb-0.0.23/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-20 09:07:20.837144 cdk-redisdb-0.0.23/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-05-20 09:07:04.000000 cdk-redisdb-0.0.23/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-20 09:07:04.000000 cdk-redisdb-0.0.23/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 09:07:20.837144 cdk-redisdb-0.0.23/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-20 09:07:04.000000 cdk-redisdb-0.0.23/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:07:20.833144 cdk-redisdb-0.0.23/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:07:20.837144 cdk-redisdb-0.0.23/src/cdk_redisdb/
+-rw-r--r--   0 runner    (1001) docker     (123)    48408 2023-05-20 09:07:04.000000 cdk-redisdb-0.0.23/src/cdk_redisdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:07:20.837144 cdk-redisdb-0.0.23/src/cdk_redisdb/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-20 09:07:04.000000 cdk-redisdb-0.0.23/src/cdk_redisdb/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25935 2023-05-20 09:07:04.000000 cdk-redisdb-0.0.23/src/cdk_redisdb/_jsii/cdk-redisdb@0.0.23.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 09:07:04.000000 cdk-redisdb-0.0.23/src/cdk_redisdb/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:07:20.837144 cdk-redisdb-0.0.23/src/cdk_redisdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-20 09:07:20.000000 cdk-redisdb-0.0.23/src/cdk_redisdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-20 09:07:20.000000 cdk-redisdb-0.0.23/src/cdk_redisdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 09:07:20.000000 cdk-redisdb-0.0.23/src/cdk_redisdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-20 09:07:20.000000 cdk-redisdb-0.0.23/src/cdk_redisdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-20 09:07:20.000000 cdk-redisdb-0.0.23/src/cdk_redisdb.egg-info/top_level.txt
```

### Comparing `cdk-redisdb-0.0.22/LICENSE` & `cdk-redisdb-0.0.23/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-redisdb-0.0.22/PKG-INFO` & `cdk-redisdb-0.0.23/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-redisdb
-Version: 0.0.22
+Version: 0.0.23
 Summary: Simple & featureful Redis on AWS - Elasticache Replication Group & MemoryDB with a unified API
 Home-page: https://github.com/forkfork/cdk-redisdb.git
 Author: Timothy Downs<timothydowns@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/forkfork/cdk-redisdb.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-redisdb-0.0.22/README.md` & `cdk-redisdb-0.0.23/README.md`

 * *Files identical despite different names*

### Comparing `cdk-redisdb-0.0.22/setup.py` & `cdk-redisdb-0.0.23/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-redisdb",
-    "version": "0.0.22",
+    "version": "0.0.23",
     "description": "Simple & featureful Redis on AWS - Elasticache Replication Group & MemoryDB with a unified API",
     "license": "Apache-2.0",
     "url": "https://github.com/forkfork/cdk-redisdb.git",
     "long_description_content_type": "text/markdown",
     "author": "Timothy Downs<timothydowns@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "cdk_redisdb",
         "cdk_redisdb._jsii"
     ],
     "package_data": {
         "cdk_redisdb._jsii": [
-            "cdk-redisdb@0.0.22.jsii.tgz"
+            "cdk-redisdb@0.0.23.jsii.tgz"
         ],
         "cdk_redisdb": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "aws-cdk-lib>=2.76.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.80.0, <2.0.0",
+        "jsii>=1.81.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `cdk-redisdb-0.0.22/src/cdk_redisdb/__init__.py` & `cdk-redisdb-0.0.23/src/cdk_redisdb/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-redisdb-0.0.22/src/cdk_redisdb.egg-info/PKG-INFO` & `cdk-redisdb-0.0.23/src/cdk_redisdb.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-redisdb
-Version: 0.0.22
+Version: 0.0.23
 Summary: Simple & featureful Redis on AWS - Elasticache Replication Group & MemoryDB with a unified API
 Home-page: https://github.com/forkfork/cdk-redisdb.git
 Author: Timothy Downs<timothydowns@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/forkfork/cdk-redisdb.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

