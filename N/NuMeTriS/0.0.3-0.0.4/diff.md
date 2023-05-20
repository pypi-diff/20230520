# Comparing `tmp/NuMeTriS-0.0.3.tar.gz` & `tmp/NuMeTriS-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NuMeTriS-0.0.3.tar", last modified: Sat May 20 13:12:19 2023, max compression
+gzip compressed data, was "NuMeTriS-0.0.4.tar", last modified: Sat May 20 13:42:16 2023, max compression
```

## Comparing `NuMeTriS-0.0.3.tar` & `NuMeTriS-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 mars      (1000) mars      (1000)        0 2023-05-20 13:12:19.478137 NuMeTriS-0.0.3/
--rw-rw-r--   0 mars      (1000) mars      (1000)     9408 2023-05-20 13:12:19.478137 NuMeTriS-0.0.3/PKG-INFO
--rw-rw-r--   0 mars      (1000) mars      (1000)     8444 2023-05-20 13:07:37.000000 NuMeTriS-0.0.3/README.md
--rw-rw-r--   0 mars      (1000) mars      (1000)     1380 2023-05-20 13:11:54.000000 NuMeTriS-0.0.3/pyproject.toml
--rw-rw-r--   0 mars      (1000) mars      (1000)       38 2023-05-20 13:12:19.478137 NuMeTriS-0.0.3/setup.cfg
--rw-rw-r--   0 mars      (1000) mars      (1000)      136 2023-03-17 16:51:36.000000 NuMeTriS-0.0.3/setup.py
-drwxrwxr-x   0 mars      (1000) mars      (1000)        0 2023-05-20 13:12:19.474137 NuMeTriS-0.0.3/src/
-drwxrwxr-x   0 mars      (1000) mars      (1000)        0 2023-05-20 13:12:19.474137 NuMeTriS-0.0.3/src/NuMeTriS/
--rwxrwxrwx   0 mars      (1000) mars      (1000)    23127 2023-03-20 12:59:10.000000 NuMeTriS-0.0.3/src/NuMeTriS/Graph_Class.py
--rw-rw-r--   0 mars      (1000) mars      (1000)    69485 2023-03-20 12:55:12.000000 NuMeTriS-0.0.3/src/NuMeTriS/Utility_Functions.py
--rwxrwxrwx   0 mars      (1000) mars      (1000)      183 2023-03-20 12:55:34.000000 NuMeTriS-0.0.3/src/NuMeTriS/__init__.py
-drwxrwxr-x   0 mars      (1000) mars      (1000)        0 2023-05-20 13:12:19.474137 NuMeTriS-0.0.3/src/NuMeTriS.egg-info/
--rw-rw-r--   0 mars      (1000) mars      (1000)     9408 2023-05-20 13:12:19.000000 NuMeTriS-0.0.3/src/NuMeTriS.egg-info/PKG-INFO
--rw-rw-r--   0 mars      (1000) mars      (1000)      387 2023-05-20 13:12:19.000000 NuMeTriS-0.0.3/src/NuMeTriS.egg-info/SOURCES.txt
--rw-rw-r--   0 mars      (1000) mars      (1000)        1 2023-05-20 13:12:19.000000 NuMeTriS-0.0.3/src/NuMeTriS.egg-info/dependency_links.txt
--rw-rw-r--   0 mars      (1000) mars      (1000)       94 2023-05-20 13:12:19.000000 NuMeTriS-0.0.3/src/NuMeTriS.egg-info/requires.txt
--rw-rw-r--   0 mars      (1000) mars      (1000)        9 2023-05-20 13:12:19.000000 NuMeTriS-0.0.3/src/NuMeTriS.egg-info/top_level.txt
-drwxrwxr-x   0 mars      (1000) mars      (1000)        0 2023-05-20 13:12:19.478137 NuMeTriS-0.0.3/tests/
--rw-rw-r--   0 mars      (1000) mars      (1000)      693 2023-03-20 12:55:59.000000 NuMeTriS-0.0.3/tests/test_DBCM.py
--rw-rw-r--   0 mars      (1000) mars      (1000)      703 2023-03-20 12:56:04.000000 NuMeTriS-0.0.3/tests/test_DBCM_CReMa.py
--rw-rw-r--   0 mars      (1000) mars      (1000)      693 2023-03-20 12:56:13.000000 NuMeTriS-0.0.3/tests/test_RBCM.py
--rw-rw-r--   0 mars      (1000) mars      (1000)      703 2023-03-20 12:56:08.000000 NuMeTriS-0.0.3/tests/test_RBCM_CRWCM.py
+drwxrwxr-x   0 mars      (1000) mars      (1000)        0 2023-05-20 13:42:16.614215 NuMeTriS-0.0.4/
+-rw-rw-r--   0 mars      (1000) mars      (1000)     9412 2023-05-20 13:42:16.614215 NuMeTriS-0.0.4/PKG-INFO
+-rw-rw-r--   0 mars      (1000) mars      (1000)     8448 2023-05-20 13:38:27.000000 NuMeTriS-0.0.4/README.md
+-rw-rw-r--   0 mars      (1000) mars      (1000)     1380 2023-05-20 13:39:38.000000 NuMeTriS-0.0.4/pyproject.toml
+-rw-rw-r--   0 mars      (1000) mars      (1000)       38 2023-05-20 13:42:16.614215 NuMeTriS-0.0.4/setup.cfg
+-rw-rw-r--   0 mars      (1000) mars      (1000)      136 2023-03-17 16:51:36.000000 NuMeTriS-0.0.4/setup.py
+drwxrwxr-x   0 mars      (1000) mars      (1000)        0 2023-05-20 13:42:16.610215 NuMeTriS-0.0.4/src/
+drwxrwxr-x   0 mars      (1000) mars      (1000)        0 2023-05-20 13:42:16.614215 NuMeTriS-0.0.4/src/NuMeTriS/
+-rwxrwxrwx   0 mars      (1000) mars      (1000)    23127 2023-03-20 12:59:10.000000 NuMeTriS-0.0.4/src/NuMeTriS/Graph_Class.py
+-rw-rw-r--   0 mars      (1000) mars      (1000)    69485 2023-03-20 12:55:12.000000 NuMeTriS-0.0.4/src/NuMeTriS/Utility_Functions.py
+-rwxrwxrwx   0 mars      (1000) mars      (1000)      183 2023-03-20 12:55:34.000000 NuMeTriS-0.0.4/src/NuMeTriS/__init__.py
+drwxrwxr-x   0 mars      (1000) mars      (1000)        0 2023-05-20 13:42:16.614215 NuMeTriS-0.0.4/src/NuMeTriS.egg-info/
+-rw-rw-r--   0 mars      (1000) mars      (1000)     9412 2023-05-20 13:42:16.000000 NuMeTriS-0.0.4/src/NuMeTriS.egg-info/PKG-INFO
+-rw-rw-r--   0 mars      (1000) mars      (1000)      387 2023-05-20 13:42:16.000000 NuMeTriS-0.0.4/src/NuMeTriS.egg-info/SOURCES.txt
+-rw-rw-r--   0 mars      (1000) mars      (1000)        1 2023-05-20 13:42:16.000000 NuMeTriS-0.0.4/src/NuMeTriS.egg-info/dependency_links.txt
+-rw-rw-r--   0 mars      (1000) mars      (1000)       94 2023-05-20 13:42:16.000000 NuMeTriS-0.0.4/src/NuMeTriS.egg-info/requires.txt
+-rw-rw-r--   0 mars      (1000) mars      (1000)        9 2023-05-20 13:42:16.000000 NuMeTriS-0.0.4/src/NuMeTriS.egg-info/top_level.txt
+drwxrwxr-x   0 mars      (1000) mars      (1000)        0 2023-05-20 13:42:16.614215 NuMeTriS-0.0.4/tests/
+-rw-rw-r--   0 mars      (1000) mars      (1000)      693 2023-03-20 12:55:59.000000 NuMeTriS-0.0.4/tests/test_DBCM.py
+-rw-rw-r--   0 mars      (1000) mars      (1000)      703 2023-03-20 12:56:04.000000 NuMeTriS-0.0.4/tests/test_DBCM_CReMa.py
+-rw-rw-r--   0 mars      (1000) mars      (1000)      693 2023-03-20 12:56:13.000000 NuMeTriS-0.0.4/tests/test_RBCM.py
+-rw-rw-r--   0 mars      (1000) mars      (1000)      703 2023-03-20 12:56:08.000000 NuMeTriS-0.0.4/tests/test_RBCM_CRWCM.py
```

### Comparing `NuMeTriS-0.0.3/PKG-INFO` & `NuMeTriS-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NuMeTriS
-Version: 0.0.3
+Version: 0.0.4
 Summary: NuMeTris is a package for Maximum-Entropy models for triadic pattern detection. It contains known models such as DBCM and RBCM for binary motif analysis, and contain mixture models such as DBCM+CReMa and RBCM+CRWCM for weighted triadic motif analysis. The models are solved and routine are present for numeric ensemble generation and the computation of the triadic z-scores for triadic sub-graph occurrence, average flux and intensity.
 Author-email: Marzio Di Vece <marzio.divece@imtlucca.it>
 Project-URL: Homepage, https://github.com/MarsMDK/NuMeTriS
 Keywords: maximum entropy methods,network motifs,pattern detection,graph,network,entropy
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -29,15 +29,15 @@
 
 When using the module for your scientific research please consider citing:
 
 
 ```
     @misc{divece_2023_commodity,
       title = {Commodity-specific triads in the Dutch inter-industry production network},
-      author = {Di Vece, Marzio and Pijpers, Frank P. and Squartini, Tiziano},
+      author = {Di Vece, Marzio and Pijpers, Frank P. and Garlaschelli, Diego},
       year={2023},
       eprint={forthcoming},
       archivePrefix={arXiv},
       primaryClass={physics.soc-ph}
     }
 
 ```
@@ -175,10 +175,10 @@
 ## Credits
 
 *Author*:
 
 [Marzio Di Vece](https://www.imtlucca.it/it/marzio.divece) (a.k.a. [MarsMDK](https://github.com/MarsMDK))
 
 *Acknowledgments*:
-The module was developed under the supervision of [Diego Garlaschelli](https://www.imtlucca.it/en/diego.garlaschelli) and [Frank Pijpers](https://www.uva.nl/profiel/p/i/f.p.pijpers/f.p.pijpers.html).
+The module was developed under the supervision of [Diego Garlaschelli](https://www.imtlucca.it/en/diego.garlaschelli) and [Frank P. Pijpers](https://www.uva.nl/profiel/p/i/f.p.pijpers/f.p.pijpers.html).
 It was developed at [IMT School for Advanced Studies Lucca](https://www.imtlucca.it/en) and [Statistics Netherlands](https://www.cbs.nl/en-gb) and
 supported by the Italian ‘Programma di Attività Integrata’ (PAI) project ‘Prosociality, Cognition and Peer Effects’ (Pro.Co.P.E.), funded by IMT School for Advanced Studies.
```

### Comparing `NuMeTriS-0.0.3/README.md` & `NuMeTriS-0.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 When using the module for your scientific research please consider citing:
 
 
 ```
     @misc{divece_2023_commodity,
       title = {Commodity-specific triads in the Dutch inter-industry production network},
-      author = {Di Vece, Marzio and Pijpers, Frank P. and Squartini, Tiziano},
+      author = {Di Vece, Marzio and Pijpers, Frank P. and Garlaschelli, Diego},
       year={2023},
       eprint={forthcoming},
       archivePrefix={arXiv},
       primaryClass={physics.soc-ph}
     }
 
 ```
@@ -161,10 +161,10 @@
 ## Credits
 
 *Author*:
 
 [Marzio Di Vece](https://www.imtlucca.it/it/marzio.divece) (a.k.a. [MarsMDK](https://github.com/MarsMDK))
 
 *Acknowledgments*:
-The module was developed under the supervision of [Diego Garlaschelli](https://www.imtlucca.it/en/diego.garlaschelli) and [Frank Pijpers](https://www.uva.nl/profiel/p/i/f.p.pijpers/f.p.pijpers.html).
+The module was developed under the supervision of [Diego Garlaschelli](https://www.imtlucca.it/en/diego.garlaschelli) and [Frank P. Pijpers](https://www.uva.nl/profiel/p/i/f.p.pijpers/f.p.pijpers.html).
 It was developed at [IMT School for Advanced Studies Lucca](https://www.imtlucca.it/en) and [Statistics Netherlands](https://www.cbs.nl/en-gb) and
 supported by the Italian ‘Programma di Attività Integrata’ (PAI) project ‘Prosociality, Cognition and Peer Effects’ (Pro.Co.P.E.), funded by IMT School for Advanced Studies.
```

### Comparing `NuMeTriS-0.0.3/pyproject.toml` & `NuMeTriS-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2.0","wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "NuMeTriS"
-version = "0.0.3"
+version = "0.0.4"
 description = "NuMeTris is a package for Maximum-Entropy models for triadic pattern detection. It contains known models such as DBCM and RBCM for binary motif analysis, and contain mixture models such as DBCM+CReMa and RBCM+CRWCM for weighted triadic motif analysis. The models are solved and routine are present for numeric ensemble generation and the computation of the triadic z-scores for triadic sub-graph occurrence, average flux and intensity."
 readme = "README.md"
 license = {file = "GNU General Public License v3"}
 authors = [{ name = "Marzio Di Vece", email = "marzio.divece@imtlucca.it" }]
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python :: 3.9",
```

### Comparing `NuMeTriS-0.0.3/src/NuMeTriS/Graph_Class.py` & `NuMeTriS-0.0.4/src/NuMeTriS/Graph_Class.py`

 * *Files identical despite different names*

### Comparing `NuMeTriS-0.0.3/src/NuMeTriS/Utility_Functions.py` & `NuMeTriS-0.0.4/src/NuMeTriS/Utility_Functions.py`

 * *Files identical despite different names*

### Comparing `NuMeTriS-0.0.3/src/NuMeTriS.egg-info/PKG-INFO` & `NuMeTriS-0.0.4/src/NuMeTriS.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NuMeTriS
-Version: 0.0.3
+Version: 0.0.4
 Summary: NuMeTris is a package for Maximum-Entropy models for triadic pattern detection. It contains known models such as DBCM and RBCM for binary motif analysis, and contain mixture models such as DBCM+CReMa and RBCM+CRWCM for weighted triadic motif analysis. The models are solved and routine are present for numeric ensemble generation and the computation of the triadic z-scores for triadic sub-graph occurrence, average flux and intensity.
 Author-email: Marzio Di Vece <marzio.divece@imtlucca.it>
 Project-URL: Homepage, https://github.com/MarsMDK/NuMeTriS
 Keywords: maximum entropy methods,network motifs,pattern detection,graph,network,entropy
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -29,15 +29,15 @@
 
 When using the module for your scientific research please consider citing:
 
 
 ```
     @misc{divece_2023_commodity,
       title = {Commodity-specific triads in the Dutch inter-industry production network},
-      author = {Di Vece, Marzio and Pijpers, Frank P. and Squartini, Tiziano},
+      author = {Di Vece, Marzio and Pijpers, Frank P. and Garlaschelli, Diego},
       year={2023},
       eprint={forthcoming},
       archivePrefix={arXiv},
       primaryClass={physics.soc-ph}
     }
 
 ```
@@ -175,10 +175,10 @@
 ## Credits
 
 *Author*:
 
 [Marzio Di Vece](https://www.imtlucca.it/it/marzio.divece) (a.k.a. [MarsMDK](https://github.com/MarsMDK))
 
 *Acknowledgments*:
-The module was developed under the supervision of [Diego Garlaschelli](https://www.imtlucca.it/en/diego.garlaschelli) and [Frank Pijpers](https://www.uva.nl/profiel/p/i/f.p.pijpers/f.p.pijpers.html).
+The module was developed under the supervision of [Diego Garlaschelli](https://www.imtlucca.it/en/diego.garlaschelli) and [Frank P. Pijpers](https://www.uva.nl/profiel/p/i/f.p.pijpers/f.p.pijpers.html).
 It was developed at [IMT School for Advanced Studies Lucca](https://www.imtlucca.it/en) and [Statistics Netherlands](https://www.cbs.nl/en-gb) and
 supported by the Italian ‘Programma di Attività Integrata’ (PAI) project ‘Prosociality, Cognition and Peer Effects’ (Pro.Co.P.E.), funded by IMT School for Advanced Studies.
```

### Comparing `NuMeTriS-0.0.3/tests/test_DBCM.py` & `NuMeTriS-0.0.4/tests/test_DBCM.py`

 * *Files identical despite different names*

### Comparing `NuMeTriS-0.0.3/tests/test_DBCM_CReMa.py` & `NuMeTriS-0.0.4/tests/test_DBCM_CReMa.py`

 * *Files identical despite different names*

### Comparing `NuMeTriS-0.0.3/tests/test_RBCM.py` & `NuMeTriS-0.0.4/tests/test_RBCM.py`

 * *Files identical despite different names*

### Comparing `NuMeTriS-0.0.3/tests/test_RBCM_CRWCM.py` & `NuMeTriS-0.0.4/tests/test_RBCM_CRWCM.py`

 * *Files identical despite different names*

