# Comparing `tmp/crosscompute-analytics-0.9.4.3.tar.gz` & `tmp/crosscompute-analytics-0.9.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crosscompute-analytics-0.9.4.3.tar", last modified: Mon May  1 17:55:50 2023, max compression
+gzip compressed data, was "crosscompute-analytics-0.9.4.9.tar", last modified: Sat May 20 20:15:04 2023, max compression
```

## Comparing `crosscompute-analytics-0.9.4.3.tar` & `crosscompute-analytics-0.9.4.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-01 17:55:50.641165 crosscompute-analytics-0.9.4.3/
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1976 2023-05-01 17:55:50.642165 crosscompute-analytics-0.9.4.3/PKG-INFO
--rw-r--r--   0 rhh       (1000) rhh       (1000)      755 2023-05-01 17:47:55.000000 crosscompute-analytics-0.9.4.3/README.md
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-01 17:55:50.641165 crosscompute-analytics-0.9.4.3/crosscompute_analytics.egg-info/
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1976 2023-05-01 17:55:50.000000 crosscompute-analytics-0.9.4.3/crosscompute_analytics.egg-info/PKG-INFO
--rw-r--r--   0 rhh       (1000) rhh       (1000)      298 2023-05-01 17:55:50.000000 crosscompute-analytics-0.9.4.3/crosscompute_analytics.egg-info/SOURCES.txt
--rw-r--r--   0 rhh       (1000) rhh       (1000)        1 2023-05-01 17:55:50.000000 crosscompute-analytics-0.9.4.3/crosscompute_analytics.egg-info/dependency_links.txt
--rw-r--r--   0 rhh       (1000) rhh       (1000)      181 2023-05-01 17:55:50.000000 crosscompute-analytics-0.9.4.3/crosscompute_analytics.egg-info/requires.txt
--rw-r--r--   0 rhh       (1000) rhh       (1000)        1 2023-05-01 17:55:50.000000 crosscompute-analytics-0.9.4.3/crosscompute_analytics.egg-info/top_level.txt
--rw-r--r--   0 rhh       (1000) rhh       (1000)        1 2023-05-01 17:42:07.000000 crosscompute-analytics-0.9.4.3/crosscompute_analytics.egg-info/zip-safe
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1431 2023-05-01 17:55:50.642165 crosscompute-analytics-0.9.4.3/setup.cfg
--rw-r--r--   0 rhh       (1000) rhh       (1000)       39 2023-05-01 17:30:54.000000 crosscompute-analytics-0.9.4.3/setup.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-20 20:15:04.781613 crosscompute-analytics-0.9.4.9/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1976 2023-05-20 20:15:04.781613 crosscompute-analytics-0.9.4.9/PKG-INFO
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      755 2023-05-20 20:12:39.000000 crosscompute-analytics-0.9.4.9/README.md
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-05-20 20:15:04.781613 crosscompute-analytics-0.9.4.9/crosscompute_analytics.egg-info/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1976 2023-05-20 20:15:04.000000 crosscompute-analytics-0.9.4.9/crosscompute_analytics.egg-info/PKG-INFO
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      298 2023-05-20 20:15:04.000000 crosscompute-analytics-0.9.4.9/crosscompute_analytics.egg-info/SOURCES.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)        1 2023-05-20 20:15:04.000000 crosscompute-analytics-0.9.4.9/crosscompute_analytics.egg-info/dependency_links.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      214 2023-05-20 20:15:04.000000 crosscompute-analytics-0.9.4.9/crosscompute_analytics.egg-info/requires.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)        1 2023-05-20 20:15:04.000000 crosscompute-analytics-0.9.4.9/crosscompute_analytics.egg-info/top_level.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)        1 2023-05-20 20:15:04.000000 crosscompute-analytics-0.9.4.9/crosscompute_analytics.egg-info/zip-safe
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1465 2023-05-20 20:15:04.782613 crosscompute-analytics-0.9.4.9/setup.cfg
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       39 2023-05-20 20:12:39.000000 crosscompute-analytics-0.9.4.9/setup.py
```

### Comparing `crosscompute-analytics-0.9.4.3/PKG-INFO` & `crosscompute-analytics-0.9.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crosscompute-analytics
-Version: 0.9.4.3
+Version: 0.9.4.9
 Summary: CrossCompute Analytics Software Development Kit
 Home-page: https://crosscompute.com
 Author: CrossCompute Inc.
 Author-email: support@crosscompute.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/crosscompute/crosscompute-analytics/issues
 Project-URL: Documentation, https://docs.crosscompute.com
```

### Comparing `crosscompute-analytics-0.9.4.3/README.md` & `crosscompute-analytics-0.9.4.9/README.md`

 * *Files identical despite different names*

### Comparing `crosscompute-analytics-0.9.4.3/crosscompute_analytics.egg-info/PKG-INFO` & `crosscompute-analytics-0.9.4.9/crosscompute_analytics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crosscompute-analytics
-Version: 0.9.4.3
+Version: 0.9.4.9
 Summary: CrossCompute Analytics Software Development Kit
 Home-page: https://crosscompute.com
 Author: CrossCompute Inc.
 Author-email: support@crosscompute.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/crosscompute/crosscompute-analytics/issues
 Project-URL: Documentation, https://docs.crosscompute.com
```

### Comparing `crosscompute-analytics-0.9.4.3/setup.cfg` & `crosscompute-analytics-0.9.4.9/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = crosscompute-analytics
-version = 0.9.4.3
+version = 0.9.4.9
 description = CrossCompute Analytics Software Development Kit
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://crosscompute.com
 author = CrossCompute Inc.
 author_email = support@crosscompute.com
 license = MIT
@@ -29,21 +29,22 @@
 	Documentation = https://docs.crosscompute.com
 	Source Code = https://github.com/crosscompute/crosscompute-analytics
 
 [options]
 packages = find:
 python_requires = >=3.10
 install_requires = 
-	crosscompute>=0.9.4.3
-	crosscompute-printers-pdf>=0.4.0
-	crosscompute-views-barcode>=0.2.0
-	crosscompute-views-map>=0.2.0
-	ipython
-	jupyterlab>=3.6.3
+	crosscompute>=0.9.4.9
+	crosscompute-printers-pdf>=0.4.1
+	crosscompute-views-map>=0.2.2
+	crosscompute-views-barcode>=0.2.2
+	invisibleroads-macros-web>=0.3.4
 	jupyterlab-crosscompute>=0.2.4
+	jupyterlab==3.6.3
+	ipython
 	pudb
 zip_safe = True
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

