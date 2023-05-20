# Comparing `tmp/eot-0.0.7.tar.gz` & `tmp/eot-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eot-0.0.7.tar", last modified: Sat May 20 00:46:47 2023, max compression
+gzip compressed data, was "eot-0.1.0.tar", last modified: Sat May 20 01:01:35 2023, max compression
```

## Comparing `eot-0.0.7.tar` & `eot-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:46:47.143196 eot-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-20 00:46:47.143196 eot-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-20 00:46:25.000000 eot-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:46:47.139196 eot-0.0.7/pkg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:46:47.143196 eot-0.0.7/pkg/eot/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-20 00:46:36.000000 eot-0.0.7/pkg/eot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-20 00:46:36.000000 eot-0.0.7/pkg/eot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-20 00:46:36.000000 eot-0.0.7/pkg/eot/eot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:46:47.143196 eot-0.0.7/pkg/eot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-20 00:46:47.000000 eot-0.0.7/pkg/eot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-20 00:46:47.000000 eot-0.0.7/pkg/eot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 00:46:47.000000 eot-0.0.7/pkg/eot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-20 00:46:47.000000 eot-0.0.7/pkg/eot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-20 00:46:47.000000 eot-0.0.7/pkg/eot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-20 00:46:36.000000 eot-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-20 00:46:47.143196 eot-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:01:35.155204 eot-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-20 01:01:35.155204 eot-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-20 01:01:14.000000 eot-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:01:35.151204 eot-0.1.0/pkg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:01:35.151204 eot-0.1.0/pkg/eot/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-20 01:01:25.000000 eot-0.1.0/pkg/eot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-20 01:01:25.000000 eot-0.1.0/pkg/eot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-20 01:01:25.000000 eot-0.1.0/pkg/eot/eot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:01:35.151204 eot-0.1.0/pkg/eot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-20 01:01:35.000000 eot-0.1.0/pkg/eot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-20 01:01:35.000000 eot-0.1.0/pkg/eot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 01:01:35.000000 eot-0.1.0/pkg/eot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-20 01:01:35.000000 eot-0.1.0/pkg/eot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-20 01:01:35.000000 eot-0.1.0/pkg/eot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-20 01:01:25.000000 eot-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-20 01:01:35.155204 eot-0.1.0/setup.cfg
```

### Comparing `eot-0.0.7/PKG-INFO` & `eot-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eot
-Version: 0.0.7
+Version: 0.1.0
 Summary: Eons Official Time
 Home-page: https://github.com/eons-dev/bin_eot
 Author: eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/bin_eot/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eot-0.0.7/pkg/eot/eot.py` & `eot-0.1.0/pkg/eot/eot.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 from datetime import datetime
 
 ######## START CONTENT ########
 
 class EOT():
-	def __init__(self):
-		super().__init__(name="Eons Official Time", descriptionStr="A stardate implementation")
-
 	#RETURNS the current time as a stardate with 8 decimal point precision.
 	@staticmethod
 	def GetStardate():
 		now = datetime.utcnow()
 		year = now.year
 		day_of_year = now.timetuple().tm_yday
 		hour = now.hour
```

### Comparing `eot-0.0.7/pkg/eot.egg-info/PKG-INFO` & `eot-0.1.0/pkg/eot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eot
-Version: 0.0.7
+Version: 0.1.0
 Summary: Eons Official Time
 Home-page: https://github.com/eons-dev/bin_eot
 Author: eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/bin_eot/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eot-0.0.7/setup.cfg` & `eot-0.1.0/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = eot
-version = v0.0.7
+version = 0.1.0
 author = eons
 author_email = support@eons.llc
 description = Eons Official Time
 license_files = LICENSE.txt
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/eons-dev/bin_eot
```

