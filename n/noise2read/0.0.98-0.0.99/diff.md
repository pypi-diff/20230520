# Comparing `tmp/noise2read-0.0.98.tar.gz` & `tmp/noise2read-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noise2read-0.0.98.tar", last modified: Sat May 20 01:50:08 2023, max compression
+gzip compressed data, was "noise2read-0.0.99.tar", last modified: Sat May 20 11:19:23 2023, max compression
```

## Comparing `noise2read-0.0.98.tar` & `noise2read-0.0.99.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-20 01:50:08.596423 noise2read-0.0.98/
--rw-r--r--   0 pping    (55472) Research  (5010)     1068 2023-04-20 03:30:20.000000 noise2read-0.0.98/LICENSE
--rw-r--r--   0 pping    (55472) Research  (5010)     5951 2023-05-20 01:50:08.597701 noise2read-0.0.98/PKG-INFO
--rw-r--r--   0 pping    (55472) Research  (5010)     5531 2023-05-13 12:21:26.000000 noise2read-0.0.98/README.rst
--rw-r--r--   0 pping    (55472) Research  (5010)       90 2023-04-20 03:30:20.000000 noise2read-0.0.98/pyproject.toml
--rw-r--r--   0 pping    (55472) Research  (5010)      999 2023-05-20 01:50:08.600505 noise2read-0.0.98/setup.cfg
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-20 01:50:08.446620 noise2read-0.0.98/src/
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-20 01:50:08.544130 noise2read-0.0.98/src/noise2read/
--rw-r--r--   0 pping    (55472) Research  (5010)      182 2023-05-20 01:46:09.000000 noise2read-0.0.98/src/noise2read/__init__.py
--rw-r--r--   0 pping    (55472) Research  (5010)    13443 2023-05-16 08:27:41.000000 noise2read-0.0.98/src/noise2read/classifier.py
--rw-r--r--   0 pping    (55472) Research  (5010)    17347 2023-05-19 00:55:32.000000 noise2read-0.0.98/src/noise2read/config.py
--rw-r--r--   0 pping    (55472) Research  (5010)     2701 2023-04-20 03:30:20.000000 noise2read-0.0.98/src/noise2read/coverage.py
--rw-r--r--   0 pping    (55472) Research  (5010)    70175 2023-04-20 03:30:20.000000 noise2read-0.0.98/src/noise2read/data_analysis.py
--rw-r--r--   0 pping    (55472) Research  (5010)    56513 2023-05-19 00:52:07.000000 noise2read-0.0.98/src/noise2read/data_generation.py
--rw-r--r--   0 pping    (55472) Research  (5010)    11534 2023-05-17 00:24:07.000000 noise2read-0.0.98/src/noise2read/data_preprocessing.py
--rw-r--r--   0 pping    (55472) Research  (5010)    30052 2023-05-14 01:00:24.000000 noise2read-0.0.98/src/noise2read/encoding.py
--rw-r--r--   0 pping    (55472) Research  (5010)    30703 2023-05-18 23:59:43.000000 noise2read-0.0.98/src/noise2read/error_orrection.py
--rw-r--r--   0 pping    (55472) Research  (5010)    16773 2023-04-20 03:30:20.000000 noise2read-0.0.98/src/noise2read/isolates_correction.py
--rw-r--r--   0 pping    (55472) Research  (5010)    26351 2023-05-16 13:42:25.000000 noise2read-0.0.98/src/noise2read/noise2read.py
--rw-r--r--   0 pping    (55472) Research  (5010)    39127 2023-05-20 01:49:53.000000 noise2read-0.0.98/src/noise2read/reads2vectors.py
--rw-r--r--   0 pping    (55472) Research  (5010)    18547 2023-05-17 00:19:59.000000 noise2read-0.0.98/src/noise2read/simulation.py
--rw-r--r--   0 pping    (55472) Research  (5010)     3475 2023-04-20 03:30:20.000000 noise2read-0.0.98/src/noise2read/umitest.py
--rw-r--r--   0 pping    (55472) Research  (5010)    15905 2023-04-20 03:30:20.000000 noise2read-0.0.98/src/noise2read/utils.py
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-20 01:50:08.579004 noise2read-0.0.98/src/noise2read.egg-info/
--rw-r--r--   0 pping    (55472) Research  (5010)     5951 2023-05-20 01:50:08.000000 noise2read-0.0.98/src/noise2read.egg-info/PKG-INFO
--rw-r--r--   0 pping    (55472) Research  (5010)      837 2023-05-20 01:50:08.000000 noise2read-0.0.98/src/noise2read.egg-info/SOURCES.txt
--rw-r--r--   0 pping    (55472) Research  (5010)        1 2023-05-20 01:50:08.000000 noise2read-0.0.98/src/noise2read.egg-info/dependency_links.txt
--rw-r--r--   0 pping    (55472) Research  (5010)       58 2023-05-20 01:50:08.000000 noise2read-0.0.98/src/noise2read.egg-info/entry_points.txt
--rw-r--r--   0 pping    (55472) Research  (5010)        1 2023-04-20 03:31:42.000000 noise2read-0.0.98/src/noise2read.egg-info/not-zip-safe
--rw-r--r--   0 pping    (55472) Research  (5010)      217 2023-05-20 01:50:08.000000 noise2read-0.0.98/src/noise2read.egg-info/requires.txt
--rw-r--r--   0 pping    (55472) Research  (5010)       11 2023-05-20 01:50:08.000000 noise2read-0.0.98/src/noise2read.egg-info/top_level.txt
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-20 01:50:08.591917 noise2read-0.0.98/tests/
--rw-r--r--   0 pping    (55472) Research  (5010)     3641 2023-04-20 03:30:20.000000 noise2read-0.0.98/tests/test_data_generation.py
--rw-r--r--   0 pping    (55472) Research  (5010)      985 2023-04-20 03:30:20.000000 noise2read-0.0.98/tests/test_reads2vector.py
--rw-r--r--   0 pping    (55472) Research  (5010)     4216 2023-04-20 03:30:20.000000 noise2read-0.0.98/tests/test_utils.py
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-20 11:19:23.204498 noise2read-0.0.99/
+-rw-r--r--   0 pping    (55472) Research  (5010)     1068 2023-04-20 03:30:20.000000 noise2read-0.0.99/LICENSE
+-rw-r--r--   0 pping    (55472) Research  (5010)     5951 2023-05-20 11:19:23.205778 noise2read-0.0.99/PKG-INFO
+-rw-r--r--   0 pping    (55472) Research  (5010)     5531 2023-05-13 12:21:26.000000 noise2read-0.0.99/README.rst
+-rw-r--r--   0 pping    (55472) Research  (5010)       90 2023-04-20 03:30:20.000000 noise2read-0.0.99/pyproject.toml
+-rw-r--r--   0 pping    (55472) Research  (5010)      999 2023-05-20 11:19:23.209031 noise2read-0.0.99/setup.cfg
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-20 11:19:22.998820 noise2read-0.0.99/src/
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-20 11:19:23.115871 noise2read-0.0.99/src/noise2read/
+-rw-r--r--   0 pping    (55472) Research  (5010)      182 2023-05-20 11:18:03.000000 noise2read-0.0.99/src/noise2read/__init__.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    13443 2023-05-16 08:27:41.000000 noise2read-0.0.99/src/noise2read/classifier.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    17347 2023-05-19 00:55:32.000000 noise2read-0.0.99/src/noise2read/config.py
+-rw-r--r--   0 pping    (55472) Research  (5010)     2701 2023-04-20 03:30:20.000000 noise2read-0.0.99/src/noise2read/coverage.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    70175 2023-04-20 03:30:20.000000 noise2read-0.0.99/src/noise2read/data_analysis.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    56593 2023-05-20 11:17:32.000000 noise2read-0.0.99/src/noise2read/data_generation.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    11534 2023-05-17 00:24:07.000000 noise2read-0.0.99/src/noise2read/data_preprocessing.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    30052 2023-05-14 01:00:24.000000 noise2read-0.0.99/src/noise2read/encoding.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    30703 2023-05-18 23:59:43.000000 noise2read-0.0.99/src/noise2read/error_orrection.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    16773 2023-04-20 03:30:20.000000 noise2read-0.0.99/src/noise2read/isolates_correction.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    26351 2023-05-16 13:42:25.000000 noise2read-0.0.99/src/noise2read/noise2read.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    39127 2023-05-20 01:49:53.000000 noise2read-0.0.99/src/noise2read/reads2vectors.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    18547 2023-05-17 00:19:59.000000 noise2read-0.0.99/src/noise2read/simulation.py
+-rw-r--r--   0 pping    (55472) Research  (5010)     3475 2023-04-20 03:30:20.000000 noise2read-0.0.99/src/noise2read/umitest.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    15905 2023-04-20 03:30:20.000000 noise2read-0.0.99/src/noise2read/utils.py
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-20 11:19:23.183814 noise2read-0.0.99/src/noise2read.egg-info/
+-rw-r--r--   0 pping    (55472) Research  (5010)     5951 2023-05-20 11:19:22.000000 noise2read-0.0.99/src/noise2read.egg-info/PKG-INFO
+-rw-r--r--   0 pping    (55472) Research  (5010)      837 2023-05-20 11:19:22.000000 noise2read-0.0.99/src/noise2read.egg-info/SOURCES.txt
+-rw-r--r--   0 pping    (55472) Research  (5010)        1 2023-05-20 11:19:22.000000 noise2read-0.0.99/src/noise2read.egg-info/dependency_links.txt
+-rw-r--r--   0 pping    (55472) Research  (5010)       58 2023-05-20 11:19:22.000000 noise2read-0.0.99/src/noise2read.egg-info/entry_points.txt
+-rw-r--r--   0 pping    (55472) Research  (5010)        1 2023-04-20 03:31:42.000000 noise2read-0.0.99/src/noise2read.egg-info/not-zip-safe
+-rw-r--r--   0 pping    (55472) Research  (5010)      217 2023-05-20 11:19:22.000000 noise2read-0.0.99/src/noise2read.egg-info/requires.txt
+-rw-r--r--   0 pping    (55472) Research  (5010)       11 2023-05-20 11:19:22.000000 noise2read-0.0.99/src/noise2read.egg-info/top_level.txt
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-20 11:19:23.198973 noise2read-0.0.99/tests/
+-rw-r--r--   0 pping    (55472) Research  (5010)     3641 2023-04-20 03:30:20.000000 noise2read-0.0.99/tests/test_data_generation.py
+-rw-r--r--   0 pping    (55472) Research  (5010)      985 2023-04-20 03:30:20.000000 noise2read-0.0.99/tests/test_reads2vector.py
+-rw-r--r--   0 pping    (55472) Research  (5010)     4216 2023-04-20 03:30:20.000000 noise2read-0.0.99/tests/test_utils.py
```

### Comparing `noise2read-0.0.98/LICENSE` & `noise2read-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.98/PKG-INFO` & `noise2read-0.0.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noise2read
-Version: 0.0.98
+Version: 0.0.99
 Summary: Turn noise to read
 Home-page: https://github.com/Jappy0/noise2read
 Author: Penagyao Ping
 Author-email: ping.pengyao@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `noise2read-0.0.98/README.rst` & `noise2read-0.0.99/README.rst`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.98/setup.cfg` & `noise2read-0.0.99/setup.cfg`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.98/src/noise2read/classifier.py` & `noise2read-0.0.99/src/noise2read/classifier.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.98/src/noise2read/config.py` & `noise2read-0.0.99/src/noise2read/config.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.98/src/noise2read/coverage.py` & `noise2read-0.0.99/src/noise2read/coverage.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.98/src/noise2read/data_analysis.py` & `noise2read-0.0.99/src/noise2read/data_analysis.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.98/src/noise2read/data_generation.py` & `noise2read-0.0.99/src/noise2read/data_generation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # @Author: Pengyao Ping
 # @Date:   2023-01-16 15:52:44
 # @Last Modified by:   Pengyao Ping
-# @Last Modified time: 2023-05-19 10:52:07
+# @Last Modified time: 2023-05-20 21:17:32
 
 import editdistance
 import networkx as nx
 import os
 import csv
 from tqdm import tqdm
 from noise2read.utils import *
@@ -193,15 +193,15 @@
         # isolated negative samples
         negative_df = self.extract_isolated_negatives(graph, edit_dis)
         # ambiguous errors
         if edit_dis == 1 and self.config.high_ambiguous: #
             # high_ambiguous_df = self.extract_high_ambiguous_errs(subgraphs)
             genuine_df, ambiguous_df, high_ambiguous_df = self.extract_genuine_ambi_errs(graph, edit_dis)
             return genuine_df, negative_df, ambiguous_df, high_ambiguous_df
-        else:
+        elif edit_dis == 1 or edit_dis == 2:
             genuine_df, ambiguous_df = self.extract_genuine_ambi_errs(graph, edit_dis)
             return genuine_df, negative_df, ambiguous_df
 
     def extract_umi_genuine_errs(self):  
         """
         extract genuine errors from umi graph
 
@@ -392,17 +392,17 @@
         if self.config.verbose:
             genuine_df.to_csv(genuine_csv, index=False)  
             ambiguous_df.to_csv(ambiguous_csv, index=False) 
             if self.config.high_ambiguous:   
                 high_ambiguous_csv = self.config.result_dir + "high_ambiguous_1nt.csv"
                 high_ambiguous_df.to_csv(high_ambiguous_csv, index=False)  
         self.logger.info("Done!")
-        if self.config.high_ambiguous:
+        if edit_dis == 1 and self.config.high_ambiguous:
             return genuine_df, ambiguous_df, high_ambiguous_df
-        else:
+        elif edit_dis == 1 or edit_dis == 2:
             return genuine_df, ambiguous_df
 
     def add_genu_sample(self, shared_obs, i):
         """
         add samples to pd DataFrame
 
         Args:
```

### Comparing `noise2read-0.0.98/src/noise2read/data_preprocessing.py` & `noise2read-0.0.99/src/noise2read/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.98/src/noise2read/encoding.py` & `noise2read-0.0.99/src/noise2read/encoding.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.98/src/noise2read/error_orrection.py` & `noise2read-0.0.99/src/noise2read/error_orrection.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.98/src/noise2read/isolates_correction.py` & `noise2read-0.0.99/src/noise2read/isolates_correction.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.98/src/noise2read/noise2read.py` & `noise2read-0.0.99/src/noise2read/noise2read.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.98/src/noise2read/reads2vectors.py` & `noise2read-0.0.99/src/noise2read/reads2vectors.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.98/src/noise2read/simulation.py` & `noise2read-0.0.99/src/noise2read/simulation.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.98/src/noise2read/umitest.py` & `noise2read-0.0.99/src/noise2read/umitest.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.98/src/noise2read/utils.py` & `noise2read-0.0.99/src/noise2read/utils.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.98/src/noise2read.egg-info/PKG-INFO` & `noise2read-0.0.99/src/noise2read.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noise2read
-Version: 0.0.98
+Version: 0.0.99
 Summary: Turn noise to read
 Home-page: https://github.com/Jappy0/noise2read
 Author: Penagyao Ping
 Author-email: ping.pengyao@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `noise2read-0.0.98/src/noise2read.egg-info/SOURCES.txt` & `noise2read-0.0.99/src/noise2read.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.98/tests/test_data_generation.py` & `noise2read-0.0.99/tests/test_data_generation.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.98/tests/test_reads2vector.py` & `noise2read-0.0.99/tests/test_reads2vector.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.98/tests/test_utils.py` & `noise2read-0.0.99/tests/test_utils.py`

 * *Files identical despite different names*

