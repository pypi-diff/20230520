# Comparing `tmp/tidytcells-1.6.0.tar.gz` & `tmp/tidytcells-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidytcells-1.6.0.tar", last modified: Sat Mar 11 19:25:15 2023, max compression
+gzip compressed data, was "tidytcells-1.7.0.tar", last modified: Sat May 20 20:39:04 2023, max compression
```

## Comparing `tidytcells-1.6.0.tar` & `tidytcells-1.7.0.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-03-11 19:25:15.825084 tidytcells-1.6.0/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1068 2022-11-05 19:14:55.000000 tidytcells-1.6.0/LICENSE.txt
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       19 2022-11-06 20:07:03.000000 tidytcells-1.6.0/MANIFEST.in
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2052 2023-03-11 19:25:15.824084 tidytcells-1.6.0/PKG-INFO
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1433 2023-03-05 13:54:54.000000 tidytcells-1.6.0/README.md
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)        5 2023-03-11 19:18:57.000000 tidytcells-1.6.0/VERSION.txt
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       38 2023-03-11 19:25:15.825084 tidytcells-1.6.0/setup.cfg
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1287 2023-03-05 13:54:54.000000 tidytcells-1.6.0/setup.py
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-03-11 19:25:15.815084 tidytcells-1.6.0/src/
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-03-11 19:25:15.817083 tidytcells-1.6.0/src/tidytcells/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       90 2023-03-11 17:56:50.000000 tidytcells-1.6.0/src/tidytcells/__init__.py
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-03-11 19:25:15.821084 tidytcells-1.6.0/src/tidytcells/_resources/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1000 2023-03-11 15:00:51.000000 tidytcells-1.6.0/src/tidytcells/_resources/__init__.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)   611997 2023-02-24 16:40:58.000000 tidytcells-1.6.0/src/tidytcells/_resources/homosapiens_mhc.json
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1295 2023-02-24 16:40:58.000000 tidytcells-1.6.0/src/tidytcells/_resources/homosapiens_mhc_synonyms.json
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    14382 2023-02-24 16:40:58.000000 tidytcells-1.6.0/src/tidytcells/_resources/homosapiens_tcr.json
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     6476 2023-02-24 16:40:58.000000 tidytcells-1.6.0/src/tidytcells/_resources/homosapiens_tcr_synonyms.json
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1031 2023-02-24 20:05:06.000000 tidytcells-1.6.0/src/tidytcells/_resources/musmusculus_mhc.json
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     5344 2023-02-24 20:05:06.000000 tidytcells-1.6.0/src/tidytcells/_resources/musmusculus_mhc_synonyms.json
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    16802 2023-02-24 16:40:58.000000 tidytcells-1.6.0/src/tidytcells/_resources/musmusculus_tcr.json
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-03-11 19:25:15.822084 tidytcells-1.6.0/src/tidytcells/_utils/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)        0 2023-02-24 16:40:58.000000 tidytcells-1.6.0/src/tidytcells/_utils/__init__.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     4231 2023-03-11 17:11:54.000000 tidytcells-1.6.0/src/tidytcells/_utils/abstract_functions.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     3081 2023-03-05 13:54:54.000000 tidytcells-1.6.0/src/tidytcells/_utils/gene_query_engines.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    10869 2023-03-05 13:54:54.000000 tidytcells-1.6.0/src/tidytcells/_utils/gene_standardisers.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      553 2023-03-05 13:54:54.000000 tidytcells-1.6.0/src/tidytcells/_utils/warnings.py
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-03-11 19:25:15.822084 tidytcells-1.6.0/src/tidytcells/aa/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      246 2023-03-11 15:44:14.000000 tidytcells-1.6.0/src/tidytcells/aa/__init__.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1290 2023-03-11 18:51:23.000000 tidytcells-1.6.0/src/tidytcells/aa/_main.py
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-03-11 19:25:15.823083 tidytcells-1.6.0/src/tidytcells/junction/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      248 2023-03-11 15:44:14.000000 tidytcells-1.6.0/src/tidytcells/junction/__init__.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2671 2023-03-11 18:51:23.000000 tidytcells-1.6.0/src/tidytcells/junction/_main.py
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-03-11 19:25:15.823083 tidytcells-1.6.0/src/tidytcells/mhc/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      403 2023-03-05 13:54:54.000000 tidytcells-1.6.0/src/tidytcells/mhc/__init__.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     9630 2023-03-11 19:17:47.000000 tidytcells-1.6.0/src/tidytcells/mhc/_main.py
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-03-11 19:25:15.823083 tidytcells-1.6.0/src/tidytcells/tcr/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      243 2023-03-05 13:54:54.000000 tidytcells-1.6.0/src/tidytcells/tcr/__init__.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     6194 2023-03-11 19:17:38.000000 tidytcells-1.6.0/src/tidytcells/tcr/_main.py
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-03-11 19:25:15.818084 tidytcells-1.6.0/src/tidytcells.egg-info/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2052 2023-03-11 19:25:15.000000 tidytcells-1.6.0/src/tidytcells.egg-info/PKG-INFO
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1184 2023-03-11 19:25:15.000000 tidytcells-1.6.0/src/tidytcells.egg-info/SOURCES.txt
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)        1 2023-03-11 19:25:15.000000 tidytcells-1.6.0/src/tidytcells.egg-info/dependency_links.txt
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       89 2023-03-11 19:25:15.000000 tidytcells-1.6.0/src/tidytcells.egg-info/requires.txt
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       11 2023-03-11 19:25:15.000000 tidytcells-1.6.0/src/tidytcells.egg-info/top_level.txt
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-03-11 19:25:15.824084 tidytcells-1.6.0/tests/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1231 2023-03-11 17:13:55.000000 tidytcells-1.6.0/tests/test_aa.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2021 2023-03-11 17:13:55.000000 tidytcells-1.6.0/tests/test_junction.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     8969 2023-03-05 13:54:54.000000 tidytcells-1.6.0/tests/test_mhc.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     6827 2023-03-05 13:54:54.000000 tidytcells-1.6.0/tests/test_tcr.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-05-20 20:39:04.522236 tidytcells-1.7.0/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1068 2022-11-05 19:14:55.000000 tidytcells-1.7.0/LICENSE.txt
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       19 2022-11-06 20:07:03.000000 tidytcells-1.7.0/MANIFEST.in
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2052 2023-05-20 20:39:04.522236 tidytcells-1.7.0/PKG-INFO
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1433 2023-03-05 13:54:54.000000 tidytcells-1.7.0/README.md
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)        5 2023-05-20 20:34:56.000000 tidytcells-1.7.0/VERSION.txt
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       38 2023-05-20 20:39:04.522236 tidytcells-1.7.0/setup.cfg
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1287 2023-03-05 13:54:54.000000 tidytcells-1.7.0/setup.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-05-20 20:39:04.511236 tidytcells-1.7.0/src/
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-05-20 20:39:04.513236 tidytcells-1.7.0/src/tidytcells/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       90 2023-03-11 19:32:17.000000 tidytcells-1.7.0/src/tidytcells/__init__.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-05-20 20:39:04.518236 tidytcells-1.7.0/src/tidytcells/_resources/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1109 2023-05-20 20:06:21.000000 tidytcells-1.7.0/src/tidytcells/_resources/__init__.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)   611997 2023-02-24 16:40:58.000000 tidytcells-1.7.0/src/tidytcells/_resources/homosapiens_mhc.json
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1295 2023-02-24 16:40:58.000000 tidytcells-1.7.0/src/tidytcells/_resources/homosapiens_mhc_synonyms.json
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    14382 2023-05-20 18:54:56.000000 tidytcells-1.7.0/src/tidytcells/_resources/homosapiens_tcr.json
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    59200 2023-05-20 19:36:11.000000 tidytcells-1.7.0/src/tidytcells/_resources/homosapiens_tcr_aa_sequences.json
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     6476 2023-05-20 18:54:57.000000 tidytcells-1.7.0/src/tidytcells/_resources/homosapiens_tcr_synonyms.json
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1031 2023-02-24 20:05:06.000000 tidytcells-1.7.0/src/tidytcells/_resources/musmusculus_mhc.json
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     5344 2023-02-24 20:05:06.000000 tidytcells-1.7.0/src/tidytcells/_resources/musmusculus_mhc_synonyms.json
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    16802 2023-02-24 16:40:58.000000 tidytcells-1.7.0/src/tidytcells/_resources/musmusculus_tcr.json
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-05-20 20:39:04.519236 tidytcells-1.7.0/src/tidytcells/_utils/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)        0 2023-02-24 16:40:58.000000 tidytcells-1.7.0/src/tidytcells/_utils/__init__.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     4336 2023-05-20 20:12:43.000000 tidytcells-1.7.0/src/tidytcells/_utils/abstract_functions.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     3081 2023-03-05 13:54:54.000000 tidytcells-1.7.0/src/tidytcells/_utils/gene_query_engines.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    10869 2023-03-05 13:54:54.000000 tidytcells-1.7.0/src/tidytcells/_utils/gene_standardisers.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      553 2023-03-05 13:54:54.000000 tidytcells-1.7.0/src/tidytcells/_utils/warnings.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-05-20 20:39:04.519236 tidytcells-1.7.0/src/tidytcells/aa/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      246 2023-03-11 19:32:17.000000 tidytcells-1.7.0/src/tidytcells/aa/__init__.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1290 2023-03-11 19:32:17.000000 tidytcells-1.7.0/src/tidytcells/aa/_main.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-05-20 20:39:04.520236 tidytcells-1.7.0/src/tidytcells/junction/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      248 2023-03-11 19:32:17.000000 tidytcells-1.7.0/src/tidytcells/junction/__init__.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2671 2023-03-11 19:32:17.000000 tidytcells-1.7.0/src/tidytcells/junction/_main.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-05-20 20:39:04.520236 tidytcells-1.7.0/src/tidytcells/mhc/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      403 2023-03-05 13:54:54.000000 tidytcells-1.7.0/src/tidytcells/mhc/__init__.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     9648 2023-03-11 23:17:03.000000 tidytcells-1.7.0/src/tidytcells/mhc/_main.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-05-20 20:39:04.521236 tidytcells-1.7.0/src/tidytcells/tcr/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      260 2023-05-20 20:15:47.000000 tidytcells-1.7.0/src/tidytcells/tcr/__init__.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     8313 2023-05-20 20:17:45.000000 tidytcells-1.7.0/src/tidytcells/tcr/_main.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-05-20 20:39:04.514236 tidytcells-1.7.0/src/tidytcells.egg-info/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2052 2023-05-20 20:39:04.000000 tidytcells-1.7.0/src/tidytcells.egg-info/PKG-INFO
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1244 2023-05-20 20:39:04.000000 tidytcells-1.7.0/src/tidytcells.egg-info/SOURCES.txt
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)        1 2023-05-20 20:39:04.000000 tidytcells-1.7.0/src/tidytcells.egg-info/dependency_links.txt
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       89 2023-05-20 20:39:04.000000 tidytcells-1.7.0/src/tidytcells.egg-info/requires.txt
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       11 2023-05-20 20:39:04.000000 tidytcells-1.7.0/src/tidytcells.egg-info/top_level.txt
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-05-20 20:39:04.521236 tidytcells-1.7.0/tests/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1231 2023-03-11 19:32:17.000000 tidytcells-1.7.0/tests/test_aa.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2021 2023-03-11 19:32:17.000000 tidytcells-1.7.0/tests/test_junction.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     8969 2023-03-05 13:54:54.000000 tidytcells-1.7.0/tests/test_mhc.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     7811 2023-05-20 20:32:03.000000 tidytcells-1.7.0/tests/test_tcr.py
```

### Comparing `tidytcells-1.6.0/LICENSE.txt` & `tidytcells-1.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tidytcells-1.6.0/PKG-INFO` & `tidytcells-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidytcells
-Version: 1.6.0
+Version: 1.7.0
 Summary: Standardise TCR/MHC data.
 Author: Yuta Nagano
 Author-email: yutanagano51@proton.me
 Keywords: immunology,bioinformatics,TCR,MHC,HLA,T cell,IMGT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tidytcells-1.6.0/README.md` & `tidytcells-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `tidytcells-1.6.0/setup.py` & `tidytcells-1.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.6.0/src/tidytcells/_resources/__init__.py` & `tidytcells-1.7.0/src/tidytcells/_resources/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 from pkg_resources import resource_stream as rs
 
 
 with rs(__name__, "homosapiens_tcr.json") as s:
     HOMOSAPIENS_TCR = json.load(s)
 with rs(__name__, "homosapiens_tcr_synonyms.json") as s:
     HOMOSAPIENS_TCR_SYNONYMS = json.load(s)
+with rs(__name__, "homosapiens_tcr_aa_sequences.json") as s:
+    HOMOSAPIENS_TCR_AA_SEQUENCES = json.load(s)
 with rs(__name__, "homosapiens_mhc.json") as s:
     HOMOSAPIENS_MHC = json.load(s)
 with rs(__name__, "homosapiens_mhc_synonyms.json") as s:
     HOMOSAPIENS_MHC_SYNONYMS = json.load(s)
 
 
 with rs(__name__, "musmusculus_tcr.json") as s:
```

### Comparing `tidytcells-1.6.0/src/tidytcells/_resources/homosapiens_mhc.json` & `tidytcells-1.7.0/src/tidytcells/_resources/homosapiens_mhc.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.6.0/src/tidytcells/_resources/homosapiens_mhc_synonyms.json` & `tidytcells-1.7.0/src/tidytcells/_resources/homosapiens_mhc_synonyms.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.6.0/src/tidytcells/_resources/homosapiens_tcr.json` & `tidytcells-1.7.0/src/tidytcells/_resources/homosapiens_tcr.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.6.0/src/tidytcells/_resources/homosapiens_tcr_synonyms.json` & `tidytcells-1.7.0/src/tidytcells/_resources/homosapiens_tcr_synonyms.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.6.0/src/tidytcells/_resources/musmusculus_mhc.json` & `tidytcells-1.7.0/src/tidytcells/_resources/musmusculus_mhc.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.6.0/src/tidytcells/_resources/musmusculus_mhc_synonyms.json` & `tidytcells-1.7.0/src/tidytcells/_resources/musmusculus_mhc_synonyms.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.6.0/src/tidytcells/_resources/musmusculus_tcr.json` & `tidytcells-1.7.0/src/tidytcells/_resources/musmusculus_tcr.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.6.0/src/tidytcells/_utils/abstract_functions.py` & `tidytcells-1.7.0/src/tidytcells/_utils/abstract_functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -95,14 +95,17 @@
             f'precision must be either "allele" or "gene", got {precision}.'
         )
     if not functionality in {"any", "F", "NF", "P", "ORF"}:
         raise ValueError(
             f'functionality must be "any", "F", "NF", "P", or "ORF", got {functionality}.'
         )
 
+    # For backward compatibility, fix CamelCased species
+    species = "".join(species.split()).lower()
+
     if not species in query_engine_dict:
         raise ValueError(f"Unsupported species: {species}. No data available.")
 
     result = query_engine_dict[species].query(
         precision=precision, functionality=functionality
     )
```

### Comparing `tidytcells-1.6.0/src/tidytcells/_utils/gene_query_engines.py` & `tidytcells-1.7.0/src/tidytcells/_utils/gene_query_engines.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.6.0/src/tidytcells/_utils/gene_standardisers.py` & `tidytcells-1.7.0/src/tidytcells/_utils/gene_standardisers.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.6.0/src/tidytcells/_utils/warnings.py` & `tidytcells-1.7.0/src/tidytcells/_utils/warnings.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.6.0/src/tidytcells/aa/_main.py` & `tidytcells-1.7.0/src/tidytcells/aa/_main.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.6.0/src/tidytcells/junction/_main.py` & `tidytcells-1.7.0/src/tidytcells/junction/_main.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.6.0/src/tidytcells/mhc/_main.py` & `tidytcells-1.7.0/src/tidytcells/mhc/_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         Input strings will intelligently be corrected to IMGT-compliant gene symbols.
 
         >>> tt.mhc.standardise("A1")
         'HLA-A*01'
 
         The ``precision`` setting can truncate unnecessary information.
 
-        >>> tt.mhc.standardise("HLA-A*01")
+        >>> tt.mhc.standardise("HLA-A*01", precision="gene")
         'HLA-A'
 
         *Mus musculus* is a supported species.
 
         >>> tt.mhc.standardise("CRW2", species="musmusculus")
         'MH1-M5'
     """
```

### Comparing `tidytcells-1.6.0/src/tidytcells/tcr/_main.py` & `tidytcells-1.7.0/src/tidytcells/tcr/_main.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Utility functions related to TCRs and TCR genes.
 """
 
 
-from typing import FrozenSet, Optional
+from typing import Dict, FrozenSet, Optional
+from .._resources import HOMOSAPIENS_TCR_AA_SEQUENCES
 from .._utils.abstract_functions import standardise_template, query_template
 from .._utils.gene_query_engines import (
     HomoSapiensTCRQueryEngine,
     MusMusculusTCRQueryEngine,
 )
 from .._utils.gene_standardisers import (
     HomoSapiensTCRStandardiser,
@@ -87,15 +88,15 @@
         Input strings will intelligently be corrected to IMGT-compliant gene symbols.
 
         >>> tt.tcr.standardise("aj1")
         'TRAJ1'
 
         The ``precision`` setting can truncate unnecessary information.
 
-        >>> tt.tcr.standardise("TRBV6-4*01")
+        >>> tt.tcr.standardise("TRBV6-4*01", precision="gene")
         'TRBV6-4'
 
         The ``enforce_functional`` setting will cause non-functional genes or alleles to be rejected.
 
         >>> result = tt.tcr.standardise("TRBV1", enforce_functional=True)
         UserWarning: Failed to standardise: "TRBV1" for species homosapiens. Attempted fix "TRBV1" did not meet the standardised format requirements. Ignoring this gene name...
         >>> print(result)
@@ -188,7 +189,63 @@
     return query_template(
         species=species,
         precision=precision,
         functionality=functionality,
         contains=contains,
         query_engine_dict=QUERY_ENGINES,
     )
+
+
+def get_aa_sequence(gene: str, species: str = "homosapiens") -> Dict[str, str]:
+    """
+    Look up the amino acid sequence of a given TCR gene.
+
+    .. topic:: Supported species
+
+        - ``'homosapiens'``
+
+    .. note::
+
+        This function currently only supports V genes.
+        Support for J genes is planned for the future.
+
+    :param gene:
+        Standardised gene name.
+        The gene must be specified to the level of the allele.
+        Note that some genes, notably the non-functional ones, will not have resolvable amino acid sequences.
+    :type gene:
+        ``str``
+    :param species:
+        Species to which the TCR gene in question belongs (see above for supported species).
+        Defaults to ``'homosapiens'``.
+    :type species:
+        ``str``
+
+    :return:
+        A dictionary with keys corresponding to names of different sequence regions within the gene, and values corresponding to their amino acid sequences.
+    :rtype:
+        ``Dict[str, str]``
+
+    .. topic:: Example usage
+
+        Get amino acid sequence information about the human V gene TRBV2*01.
+
+        >>> tt.tcr.get_aa_sequence(gene="TRBV2*01", species="homosapiens")
+        {'CDR1-IMGT': 'SNHLY', 'CDR2-IMGT': 'FYNNEI', 'FR1-IMGT': 'EPEVTQTPSHQVTQMGQEVILRCVPI', 'FR2-IMGT': 'FYWYRQILGQKVEFLVS', 'FR3-IMGT': 'SEKSEIFDDQFSVERPDGSNFTLKIRSTKLEDSAMYFC'}
+    """
+    # Type checks
+    if type(gene) != str:
+        raise TypeError(f"gene must be type str, got {gene} ({type(gene)}).")
+    if type(species) != str:
+        raise TypeError(f"species must be type str, got {species} ({type(species)}).")
+
+    # For backward compatibility, fix CamelCased species
+    species = "".join(species.split()).lower()
+
+    # Currently only supports homosapiens
+    if species != "homosapiens":
+        raise ValueError(f"Unsupported species: {species}. No data available.")
+
+    if gene in HOMOSAPIENS_TCR_AA_SEQUENCES:
+        return HOMOSAPIENS_TCR_AA_SEQUENCES[gene]
+
+    raise ValueError(f"No data found for TCR gene {gene} for species {species}.")
```

### Comparing `tidytcells-1.6.0/src/tidytcells.egg-info/PKG-INFO` & `tidytcells-1.7.0/src/tidytcells.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidytcells
-Version: 1.6.0
+Version: 1.7.0
 Summary: Standardise TCR/MHC data.
 Author: Yuta Nagano
 Author-email: yutanagano51@proton.me
 Keywords: immunology,bioinformatics,TCR,MHC,HLA,T cell,IMGT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tidytcells-1.6.0/src/tidytcells.egg-info/SOURCES.txt` & `tidytcells-1.7.0/src/tidytcells.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 src/tidytcells.egg-info/dependency_links.txt
 src/tidytcells.egg-info/requires.txt
 src/tidytcells.egg-info/top_level.txt
 src/tidytcells/_resources/__init__.py
 src/tidytcells/_resources/homosapiens_mhc.json
 src/tidytcells/_resources/homosapiens_mhc_synonyms.json
 src/tidytcells/_resources/homosapiens_tcr.json
+src/tidytcells/_resources/homosapiens_tcr_aa_sequences.json
 src/tidytcells/_resources/homosapiens_tcr_synonyms.json
 src/tidytcells/_resources/musmusculus_mhc.json
 src/tidytcells/_resources/musmusculus_mhc_synonyms.json
 src/tidytcells/_resources/musmusculus_tcr.json
 src/tidytcells/_utils/__init__.py
 src/tidytcells/_utils/abstract_functions.py
 src/tidytcells/_utils/gene_query_engines.py
```

### Comparing `tidytcells-1.6.0/tests/test_aa.py` & `tidytcells-1.7.0/tests/test_aa.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.6.0/tests/test_junction.py` & `tidytcells-1.7.0/tests/test_junction.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.6.0/tests/test_mhc.py` & `tidytcells-1.7.0/tests/test_mhc.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.6.0/tests/test_tcr.py` & `tidytcells-1.7.0/tests/test_tcr.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,7 +208,39 @@
         result = tcr.query(
             species=species, precision=precision, functionality=functionality
         )
 
         assert len(result) == expected_len
         assert expected_in in result
         assert not expected_not_in in result
+
+
+class TestGetAaSequence:
+    @pytest.mark.parametrize(
+        ("gene", "expected"),
+        (
+            (
+                "TRBV2*01",
+                {
+                    "CDR1-IMGT": "SNHLY",
+                    "CDR2-IMGT": "FYNNEI",
+                    "FR1-IMGT": "EPEVTQTPSHQVTQMGQEVILRCVPI",
+                    "FR2-IMGT": "FYWYRQILGQKVEFLVS",
+                    "FR3-IMGT": "SEKSEIFDDQFSVERPDGSNFTLKIRSTKLEDSAMYFC",
+                },
+            ),
+            (
+                "TRAV10*02",
+                {
+                    "CDR1-IMGT": "VSPFSN",
+                    "CDR2-IMGT": "MTFSENT",
+                    "FR1-IMGT": "KNQVEQSPQSLIILEGKNCTLQCNYT",
+                    "FR2-IMGT": "LRWYKQDTGRGPVSLTI",
+                    "FR3-IMGT": "KSNGRYTATLDADTKQSSLHITASQLSDSASYIC",
+                },
+            ),
+        ),
+    )
+    def test_get_aa_sequence(self, gene, expected):
+        result = tcr.get_aa_sequence(gene=gene)
+
+        assert result == expected
```

