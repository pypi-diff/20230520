# Comparing `tmp/eot-0.0.6.tar.gz` & `tmp/eot-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eot-0.0.6.tar", last modified: Tue Oct 18 00:26:47 2022, max compression
+gzip compressed data, was "eot-0.0.7.tar", last modified: Sat May 20 00:46:47 2023, max compression
```

## Comparing `eot-0.0.6.tar` & `eot-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 00:26:47.363581 eot-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (121)      574 2022-10-18 00:26:47.363581 eot-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-10-18 00:26:28.000000 eot-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 00:26:47.359581 eot-0.0.6/pkg/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 00:26:47.363581 eot-0.0.6/pkg/eot/
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-10-18 00:26:38.000000 eot-0.0.6/pkg/eot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-10-18 00:26:38.000000 eot-0.0.6/pkg/eot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1217 2022-10-18 00:26:38.000000 eot-0.0.6/pkg/eot/eot.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 00:26:47.363581 eot-0.0.6/pkg/eot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      574 2022-10-18 00:26:47.000000 eot-0.0.6/pkg/eot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      277 2022-10-18 00:26:47.000000 eot-0.0.6/pkg/eot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-18 00:26:47.000000 eot-0.0.6/pkg/eot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-10-18 00:26:47.000000 eot-0.0.6/pkg/eot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-10-18 00:26:47.000000 eot-0.0.6/pkg/eot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-10-18 00:26:47.000000 eot-0.0.6/pkg/eot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-10-18 00:26:38.000000 eot-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      737 2022-10-18 00:26:47.363581 eot-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:46:47.143196 eot-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-20 00:46:47.143196 eot-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-20 00:46:25.000000 eot-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:46:47.139196 eot-0.0.7/pkg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:46:47.143196 eot-0.0.7/pkg/eot/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-20 00:46:36.000000 eot-0.0.7/pkg/eot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-20 00:46:36.000000 eot-0.0.7/pkg/eot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-20 00:46:36.000000 eot-0.0.7/pkg/eot/eot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:46:47.143196 eot-0.0.7/pkg/eot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-20 00:46:47.000000 eot-0.0.7/pkg/eot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-20 00:46:47.000000 eot-0.0.7/pkg/eot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 00:46:47.000000 eot-0.0.7/pkg/eot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-20 00:46:47.000000 eot-0.0.7/pkg/eot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-20 00:46:47.000000 eot-0.0.7/pkg/eot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-20 00:46:36.000000 eot-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-20 00:46:47.143196 eot-0.0.7/setup.cfg
```

### Comparing `eot-0.0.6/PKG-INFO` & `eot-0.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eot
-Version: 0.0.6
+Version: 0.0.7
 Summary: Eons Official Time
 Home-page: https://github.com/eons-dev/bin_eot
 Author: eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/bin_eot/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eot-0.0.6/pkg/eot/eot.py` & `eot-0.0.7/pkg/eot/eot.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-import eons
 from datetime import datetime
 
 ######## START CONTENT ########
 
-class EOT(eons.Executor):
+class EOT():
 	def __init__(self):
 		super().__init__(name="Eons Official Time", descriptionStr="A stardate implementation")
 
-
 	#RETURNS the current time as a stardate with 8 decimal point precision.
 	@staticmethod
 	def GetStardate():
 		now = datetime.utcnow()
 		year = now.year
 		day_of_year = now.timetuple().tm_yday
 		hour = now.hour
@@ -33,11 +31,10 @@
 		stardate = year + decimal
 
 		# print("stardate for", year, day_of_year, hour)
 		# print("error:", error, "in hours:", error_hours)
 		return stardate
 
 	#Called when executing this as a functor.
-	#Required method from eons.Executor. See that class for more details.
-	def Function(this):
+	def __call__(this):
 		print(EOT.GetStardate())
```

### Comparing `eot-0.0.6/pkg/eot.egg-info/PKG-INFO` & `eot-0.0.7/pkg/eot.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eot
-Version: 0.0.6
+Version: 0.0.7
 Summary: Eons Official Time
 Home-page: https://github.com/eons-dev/bin_eot
 Author: eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/bin_eot/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

