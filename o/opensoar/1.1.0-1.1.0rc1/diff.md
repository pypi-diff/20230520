# Comparing `tmp/opensoar-1.1.0.tar.gz` & `tmp/opensoar-1.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opensoar-1.1.0.tar", last modified: Sat May 20 10:21:12 2023, max compression
+gzip compressed data, was "opensoar-1.1.0rc1.tar", last modified: Sat May 20 10:15:30 2023, max compression
```

## Comparing `opensoar-1.1.0.tar` & `opensoar-1.1.0rc1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:21:12.481548 opensoar-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-20 10:20:39.000000 opensoar-1.1.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-20 10:20:39.000000 opensoar-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-20 10:20:39.000000 opensoar-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-20 10:21:12.481548 opensoar-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-20 10:20:39.000000 opensoar-1.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:21:12.473548 opensoar-1.1.0/opensoar/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-20 10:20:39.000000 opensoar-1.1.0/opensoar/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:21:12.477548 opensoar-1.1.0/opensoar/competition/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-20 10:20:39.000000 opensoar-1.1.0/opensoar/competition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-20 10:20:39.000000 opensoar-1.1.0/opensoar/competition/competition_day.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-20 10:20:39.000000 opensoar-1.1.0/opensoar/competition/competitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-05-20 10:20:39.000000 opensoar-1.1.0/opensoar/competition/daily_results_page.py
--rw-r--r--   0 runner    (1001) docker     (123)    13848 2023-05-20 10:20:39.000000 opensoar-1.1.0/opensoar/competition/soaringspot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-05-20 10:20:39.000000 opensoar-1.1.0/opensoar/competition/strepla.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:21:12.477548 opensoar-1.1.0/opensoar/task/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-20 10:20:39.000000 opensoar-1.1.0/opensoar/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15799 2023-05-20 10:20:39.000000 opensoar-1.1.0/opensoar/task/aat.py
--rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-05-20 10:20:39.000000 opensoar-1.1.0/opensoar/task/race_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     6845 2023-05-20 10:20:39.000000 opensoar-1.1.0/opensoar/task/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-05-20 10:20:39.000000 opensoar-1.1.0/opensoar/task/trip.py
--rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-05-20 10:20:39.000000 opensoar-1.1.0/opensoar/task/waypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:21:12.477548 opensoar-1.1.0/opensoar/thermals/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-20 10:20:39.000000 opensoar-1.1.0/opensoar/thermals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-05-20 10:20:39.000000 opensoar-1.1.0/opensoar/thermals/flight_phases.py
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-05-20 10:20:39.000000 opensoar-1.1.0/opensoar/thermals/pysoar_thermal_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:21:12.477548 opensoar-1.1.0/opensoar/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-20 10:20:39.000000 opensoar-1.1.0/opensoar/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-05-20 10:20:39.000000 opensoar-1.1.0/opensoar/utilities/geojson_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-05-20 10:20:39.000000 opensoar-1.1.0/opensoar/utilities/helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-20 10:20:39.000000 opensoar-1.1.0/opensoar/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:21:12.473548 opensoar-1.1.0/opensoar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-20 10:21:12.000000 opensoar-1.1.0/opensoar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-20 10:21:12.000000 opensoar-1.1.0/opensoar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 10:21:12.000000 opensoar-1.1.0/opensoar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-20 10:21:12.000000 opensoar-1.1.0/opensoar.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-20 10:21:12.000000 opensoar-1.1.0/opensoar.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 10:21:12.481548 opensoar-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-20 10:20:39.000000 opensoar-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:21:12.473548 opensoar-1.1.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:21:12.477548 opensoar-1.1.0/tests/competition/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 10:20:39.000000 opensoar-1.1.0/tests/competition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7140 2023-05-20 10:20:39.000000 opensoar-1.1.0/tests/competition/test_soaringspot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-20 10:20:39.000000 opensoar-1.1.0/tests/competition/test_strepla.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:21:12.481548 opensoar-1.1.0/tests/task/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 10:20:39.000000 opensoar-1.1.0/tests/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-20 10:20:39.000000 opensoar-1.1.0/tests/task/helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-20 10:20:39.000000 opensoar-1.1.0/tests/task/test_aat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-05-20 10:20:39.000000 opensoar-1.1.0/tests/task/test_aat_trip.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-05-20 10:20:39.000000 opensoar-1.1.0/tests/task/test_race_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-20 10:20:39.000000 opensoar-1.1.0/tests/task/test_trip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-05-20 10:20:39.000000 opensoar-1.1.0/tests/task/test_waypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:21:12.481548 opensoar-1.1.0/tests/thermals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 10:20:39.000000 opensoar-1.1.0/tests/thermals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-05-20 10:20:39.000000 opensoar-1.1.0/tests/thermals/test_flight_phases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:21:12.481548 opensoar-1.1.0/tests/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 10:20:39.000000 opensoar-1.1.0/tests/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-05-20 10:20:39.000000 opensoar-1.1.0/tests/utilities/test_helper_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:15:30.505873 opensoar-1.1.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-20 10:15:05.000000 opensoar-1.1.0rc1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-20 10:15:05.000000 opensoar-1.1.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-20 10:15:05.000000 opensoar-1.1.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-20 10:15:30.505873 opensoar-1.1.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-20 10:15:05.000000 opensoar-1.1.0rc1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:15:30.501873 opensoar-1.1.0rc1/opensoar/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-20 10:15:05.000000 opensoar-1.1.0rc1/opensoar/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:15:30.501873 opensoar-1.1.0rc1/opensoar/competition/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-20 10:15:05.000000 opensoar-1.1.0rc1/opensoar/competition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-20 10:15:05.000000 opensoar-1.1.0rc1/opensoar/competition/competition_day.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-20 10:15:05.000000 opensoar-1.1.0rc1/opensoar/competition/competitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-05-20 10:15:05.000000 opensoar-1.1.0rc1/opensoar/competition/daily_results_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13848 2023-05-20 10:15:05.000000 opensoar-1.1.0rc1/opensoar/competition/soaringspot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-05-20 10:15:05.000000 opensoar-1.1.0rc1/opensoar/competition/strepla.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:15:30.505873 opensoar-1.1.0rc1/opensoar/task/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-20 10:15:05.000000 opensoar-1.1.0rc1/opensoar/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15799 2023-05-20 10:15:05.000000 opensoar-1.1.0rc1/opensoar/task/aat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-05-20 10:15:05.000000 opensoar-1.1.0rc1/opensoar/task/race_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6845 2023-05-20 10:15:05.000000 opensoar-1.1.0rc1/opensoar/task/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-05-20 10:15:05.000000 opensoar-1.1.0rc1/opensoar/task/trip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-05-20 10:15:05.000000 opensoar-1.1.0rc1/opensoar/task/waypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:15:30.505873 opensoar-1.1.0rc1/opensoar/thermals/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-20 10:15:05.000000 opensoar-1.1.0rc1/opensoar/thermals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-05-20 10:15:05.000000 opensoar-1.1.0rc1/opensoar/thermals/flight_phases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-05-20 10:15:05.000000 opensoar-1.1.0rc1/opensoar/thermals/pysoar_thermal_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:15:30.505873 opensoar-1.1.0rc1/opensoar/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-20 10:15:05.000000 opensoar-1.1.0rc1/opensoar/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-05-20 10:15:05.000000 opensoar-1.1.0rc1/opensoar/utilities/geojson_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-05-20 10:15:05.000000 opensoar-1.1.0rc1/opensoar/utilities/helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-20 10:15:05.000000 opensoar-1.1.0rc1/opensoar/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:15:30.501873 opensoar-1.1.0rc1/opensoar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-20 10:15:30.000000 opensoar-1.1.0rc1/opensoar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-20 10:15:30.000000 opensoar-1.1.0rc1/opensoar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 10:15:30.000000 opensoar-1.1.0rc1/opensoar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-20 10:15:30.000000 opensoar-1.1.0rc1/opensoar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-20 10:15:30.000000 opensoar-1.1.0rc1/opensoar.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 10:15:30.505873 opensoar-1.1.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-20 10:15:05.000000 opensoar-1.1.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:15:30.501873 opensoar-1.1.0rc1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:15:30.505873 opensoar-1.1.0rc1/tests/competition/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 10:15:05.000000 opensoar-1.1.0rc1/tests/competition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7140 2023-05-20 10:15:05.000000 opensoar-1.1.0rc1/tests/competition/test_soaringspot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-20 10:15:05.000000 opensoar-1.1.0rc1/tests/competition/test_strepla.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:15:30.505873 opensoar-1.1.0rc1/tests/task/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 10:15:05.000000 opensoar-1.1.0rc1/tests/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-20 10:15:05.000000 opensoar-1.1.0rc1/tests/task/helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-20 10:15:05.000000 opensoar-1.1.0rc1/tests/task/test_aat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-05-20 10:15:05.000000 opensoar-1.1.0rc1/tests/task/test_aat_trip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-05-20 10:15:05.000000 opensoar-1.1.0rc1/tests/task/test_race_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-20 10:15:05.000000 opensoar-1.1.0rc1/tests/task/test_trip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-05-20 10:15:05.000000 opensoar-1.1.0rc1/tests/task/test_waypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:15:30.505873 opensoar-1.1.0rc1/tests/thermals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 10:15:05.000000 opensoar-1.1.0rc1/tests/thermals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-05-20 10:15:05.000000 opensoar-1.1.0rc1/tests/thermals/test_flight_phases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:15:30.505873 opensoar-1.1.0rc1/tests/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 10:15:05.000000 opensoar-1.1.0rc1/tests/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-05-20 10:15:05.000000 opensoar-1.1.0rc1/tests/utilities/test_helper_functions.py
```

### Comparing `opensoar-1.1.0/CHANGELOG.rst` & `opensoar-1.1.0rc1/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `opensoar-1.1.0/LICENSE` & `opensoar-1.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `opensoar-1.1.0/PKG-INFO` & `opensoar-1.1.0rc1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opensoar
-Version: 1.1.0
+Version: 1.1.0rc1
 Summary: Open source python library for glider flight analysis
 Home-page: https://github.com/glidergeek/opensoar
 License: MIT
 License-File: LICENSE
 
 OpenSoar
 ========
```

### Comparing `opensoar-1.1.0/README.rst` & `opensoar-1.1.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `opensoar-1.1.0/opensoar/competition/competition_day.py` & `opensoar-1.1.0rc1/opensoar/competition/competition_day.py`

 * *Files identical despite different names*

### Comparing `opensoar-1.1.0/opensoar/competition/competitor.py` & `opensoar-1.1.0rc1/opensoar/competition/competitor.py`

 * *Files identical despite different names*

### Comparing `opensoar-1.1.0/opensoar/competition/daily_results_page.py` & `opensoar-1.1.0rc1/opensoar/competition/daily_results_page.py`

 * *Files identical despite different names*

### Comparing `opensoar-1.1.0/opensoar/competition/soaringspot.py` & `opensoar-1.1.0rc1/opensoar/competition/soaringspot.py`

 * *Files identical despite different names*

### Comparing `opensoar-1.1.0/opensoar/competition/strepla.py` & `opensoar-1.1.0rc1/opensoar/competition/strepla.py`

 * *Files identical despite different names*

### Comparing `opensoar-1.1.0/opensoar/task/aat.py` & `opensoar-1.1.0rc1/opensoar/task/aat.py`

 * *Files identical despite different names*

### Comparing `opensoar-1.1.0/opensoar/task/race_task.py` & `opensoar-1.1.0rc1/opensoar/task/race_task.py`

 * *Files identical despite different names*

### Comparing `opensoar-1.1.0/opensoar/task/task.py` & `opensoar-1.1.0rc1/opensoar/task/task.py`

 * *Files identical despite different names*

### Comparing `opensoar-1.1.0/opensoar/task/trip.py` & `opensoar-1.1.0rc1/opensoar/task/trip.py`

 * *Files identical despite different names*

### Comparing `opensoar-1.1.0/opensoar/task/waypoint.py` & `opensoar-1.1.0rc1/opensoar/task/waypoint.py`

 * *Files identical despite different names*

### Comparing `opensoar-1.1.0/opensoar/thermals/flight_phases.py` & `opensoar-1.1.0rc1/opensoar/thermals/flight_phases.py`

 * *Files identical despite different names*

### Comparing `opensoar-1.1.0/opensoar/thermals/pysoar_thermal_detector.py` & `opensoar-1.1.0rc1/opensoar/thermals/pysoar_thermal_detector.py`

 * *Files identical despite different names*

### Comparing `opensoar-1.1.0/opensoar/utilities/geojson_serializers.py` & `opensoar-1.1.0rc1/opensoar/utilities/geojson_serializers.py`

 * *Files identical despite different names*

### Comparing `opensoar-1.1.0/opensoar/utilities/helper_functions.py` & `opensoar-1.1.0rc1/opensoar/utilities/helper_functions.py`

 * *Files identical despite different names*

### Comparing `opensoar-1.1.0/opensoar.egg-info/PKG-INFO` & `opensoar-1.1.0rc1/opensoar.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opensoar
-Version: 1.1.0
+Version: 1.1.0rc1
 Summary: Open source python library for glider flight analysis
 Home-page: https://github.com/glidergeek/opensoar
 License: MIT
 License-File: LICENSE
 
 OpenSoar
 ========
```

### Comparing `opensoar-1.1.0/opensoar.egg-info/SOURCES.txt` & `opensoar-1.1.0rc1/opensoar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opensoar-1.1.0/setup.py` & `opensoar-1.1.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `opensoar-1.1.0/tests/competition/test_soaringspot.py` & `opensoar-1.1.0rc1/tests/competition/test_soaringspot.py`

 * *Files identical despite different names*

### Comparing `opensoar-1.1.0/tests/competition/test_strepla.py` & `opensoar-1.1.0rc1/tests/competition/test_strepla.py`

 * *Files identical despite different names*

### Comparing `opensoar-1.1.0/tests/task/test_aat.py` & `opensoar-1.1.0rc1/tests/task/test_aat.py`

 * *Files identical despite different names*

### Comparing `opensoar-1.1.0/tests/task/test_aat_trip.py` & `opensoar-1.1.0rc1/tests/task/test_aat_trip.py`

 * *Files identical despite different names*

### Comparing `opensoar-1.1.0/tests/task/test_race_task.py` & `opensoar-1.1.0rc1/tests/task/test_race_task.py`

 * *Files identical despite different names*

### Comparing `opensoar-1.1.0/tests/task/test_trip.py` & `opensoar-1.1.0rc1/tests/task/test_trip.py`

 * *Files identical despite different names*

### Comparing `opensoar-1.1.0/tests/task/test_waypoint.py` & `opensoar-1.1.0rc1/tests/task/test_waypoint.py`

 * *Files identical despite different names*

### Comparing `opensoar-1.1.0/tests/thermals/test_flight_phases.py` & `opensoar-1.1.0rc1/tests/thermals/test_flight_phases.py`

 * *Files identical despite different names*

### Comparing `opensoar-1.1.0/tests/utilities/test_helper_functions.py` & `opensoar-1.1.0rc1/tests/utilities/test_helper_functions.py`

 * *Files identical despite different names*

