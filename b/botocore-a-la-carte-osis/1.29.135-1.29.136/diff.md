# Comparing `tmp/botocore-a-la-carte-osis-1.29.135.tar.gz` & `tmp/botocore-a-la-carte-osis-1.29.136.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-osis-1.29.135.tar", last modified: Wed May 17 01:18:48 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-osis-1.29.136.tar", last modified: Fri May 19 01:17:56 2023, max compression
```

## Comparing `botocore-a-la-carte-osis-1.29.135.tar` & `botocore-a-la-carte-osis-1.29.136.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:18:48.399294 botocore-a-la-carte-osis-1.29.135/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-05-17 01:18:48.000000 botocore-a-la-carte-osis-1.29.135/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-17 01:18:48.399294 botocore-a-la-carte-osis-1.29.135/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:18:48.395294 botocore-a-la-carte-osis-1.29.135/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:18:48.395294 botocore-a-la-carte-osis-1.29.135/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:18:48.395294 botocore-a-la-carte-osis-1.29.135/botocore/data/osis/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:18:48.399294 botocore-a-la-carte-osis-1.29.135/botocore/data/osis/2022-01-01/
--rw-r--r--   0 runner    (1001) docker     (123)    17616 2023-05-17 01:18:14.000000 botocore-a-la-carte-osis-1.29.135/botocore/data/osis/2022-01-01/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-17 01:18:14.000000 botocore-a-la-carte-osis-1.29.135/botocore/data/osis/2022-01-01/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    37304 2023-05-17 01:18:14.000000 botocore-a-la-carte-osis-1.29.135/botocore/data/osis/2022-01-01/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:18:48.399294 botocore-a-la-carte-osis-1.29.135/botocore_a_la_carte_osis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-17 01:18:48.000000 botocore-a-la-carte-osis-1.29.135/botocore_a_la_carte_osis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-17 01:18:48.000000 botocore-a-la-carte-osis-1.29.135/botocore_a_la_carte_osis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 01:18:48.000000 botocore-a-la-carte-osis-1.29.135/botocore_a_la_carte_osis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-17 01:18:48.000000 botocore-a-la-carte-osis-1.29.135/botocore_a_la_carte_osis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 01:18:48.399294 botocore-a-la-carte-osis-1.29.135/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-17 01:18:48.000000 botocore-a-la-carte-osis-1.29.135/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 01:17:56.943562 botocore-a-la-carte-osis-1.29.136/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-05-19 01:17:56.000000 botocore-a-la-carte-osis-1.29.136/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-19 01:17:56.943562 botocore-a-la-carte-osis-1.29.136/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 01:17:56.939562 botocore-a-la-carte-osis-1.29.136/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 01:17:56.939562 botocore-a-la-carte-osis-1.29.136/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 01:17:56.939562 botocore-a-la-carte-osis-1.29.136/botocore/data/osis/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 01:17:56.939562 botocore-a-la-carte-osis-1.29.136/botocore/data/osis/2022-01-01/
+-rw-r--r--   0 runner    (1001) docker     (123)    17616 2023-05-19 01:17:23.000000 botocore-a-la-carte-osis-1.29.136/botocore/data/osis/2022-01-01/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-19 01:17:23.000000 botocore-a-la-carte-osis-1.29.136/botocore/data/osis/2022-01-01/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    37304 2023-05-19 01:17:23.000000 botocore-a-la-carte-osis-1.29.136/botocore/data/osis/2022-01-01/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 01:17:56.939562 botocore-a-la-carte-osis-1.29.136/botocore_a_la_carte_osis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-19 01:17:56.000000 botocore-a-la-carte-osis-1.29.136/botocore_a_la_carte_osis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-19 01:17:56.000000 botocore-a-la-carte-osis-1.29.136/botocore_a_la_carte_osis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 01:17:56.000000 botocore-a-la-carte-osis-1.29.136/botocore_a_la_carte_osis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-19 01:17:56.000000 botocore-a-la-carte-osis-1.29.136/botocore_a_la_carte_osis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 01:17:56.943562 botocore-a-la-carte-osis-1.29.136/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-19 01:17:56.000000 botocore-a-la-carte-osis-1.29.136/setup.py
```

### Comparing `botocore-a-la-carte-osis-1.29.135/LICENSE.txt` & `botocore-a-la-carte-osis-1.29.136/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-osis-1.29.135/PKG-INFO` & `botocore-a-la-carte-osis-1.29.136/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-osis
-Version: 1.29.135
+Version: 1.29.136
 Summary: osis data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-osis-1.29.135/botocore/data/osis/2022-01-01/endpoint-rule-set-1.json` & `botocore-a-la-carte-osis-1.29.136/botocore/data/osis/2022-01-01/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-osis-1.29.135/botocore/data/osis/2022-01-01/service-2.json` & `botocore-a-la-carte-osis-1.29.136/botocore/data/osis/2022-01-01/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-osis-1.29.135/botocore_a_la_carte_osis.egg-info/PKG-INFO` & `botocore-a-la-carte-osis-1.29.136/botocore_a_la_carte_osis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-osis
-Version: 1.29.135
+Version: 1.29.136
 Summary: osis data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-osis-1.29.135/setup.py` & `botocore-a-la-carte-osis-1.29.136/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-osis',
-    version="1.29.135",
+    version="1.29.136",
     description='osis data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/osis/*/*.json'],
```

