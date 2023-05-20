# Comparing `tmp/QSCOUT-gatemodels-1.1.1.tar.gz` & `tmp/QSCOUT-gatemodels-1.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/tmp/build-jaqal/qscout-gatemodels/dist/.tmp-advos_oc/QSCOUT-gatemodels-1.1.1.tar", last modified: Wed Mar 29 16:24:32 2023, max compression
+gzip compressed data, was "/tmp/build-jaqal/qscout-gatemodels/dist/.tmp-tiobknl0/QSCOUT-gatemodels-1.2.0a1.tar", last modified: Fri May 19 23:36:28 2023, max compression
```

## Comparing `QSCOUT-gatemodels-1.1.1.tar` & `QSCOUT-gatemodels-1.2.0a1.tar`

### file list

```diff
@@ -1,26 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:24:32.000000 QSCOUT-gatemodels-1.1.1/
--rw-rw-r--   0 root         (0) root         (0)    11358 2023-03-29 15:59:03.000000 QSCOUT-gatemodels-1.1.1/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      197 2023-03-29 15:59:03.000000 QSCOUT-gatemodels-1.1.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     2154 2023-03-29 16:24:32.000000 QSCOUT-gatemodels-1.1.1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     1333 2023-03-29 15:59:03.000000 QSCOUT-gatemodels-1.1.1/README.md
--rw-rw-r--   0 root         (0) root         (0)      111 2023-03-29 15:59:03.000000 QSCOUT-gatemodels-1.1.1/pyproject.toml
--rw-rw-r--   0 root         (0) root         (0)     1165 2023-03-29 16:24:32.000000 QSCOUT-gatemodels-1.1.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:24:32.000000 QSCOUT-gatemodels-1.1.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:24:32.000000 QSCOUT-gatemodels-1.1.1/src/QSCOUT_gatemodels.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2154 2023-03-29 16:24:32.000000 QSCOUT-gatemodels-1.1.1/src/QSCOUT_gatemodels.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      456 2023-03-29 16:24:32.000000 QSCOUT-gatemodels-1.1.1/src/QSCOUT_gatemodels.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-29 16:24:32.000000 QSCOUT-gatemodels-1.1.1/src/QSCOUT_gatemodels.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-29 16:24:32.000000 QSCOUT-gatemodels-1.1.1/src/QSCOUT_gatemodels.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-03-29 16:24:32.000000 QSCOUT-gatemodels-1.1.1/src/QSCOUT_gatemodels.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:24:32.000000 QSCOUT-gatemodels-1.1.1/src/qscout/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:24:32.000000 QSCOUT-gatemodels-1.1.1/src/qscout/v1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:24:32.000000 QSCOUT-gatemodels-1.1.1/src/qscout/v1/std/
--rw-rw-r--   0 root         (0) root         (0)     5434 2023-03-29 15:59:03.000000 QSCOUT-gatemodels-1.1.1/src/qscout/v1/std/jaqal_gates.py
--rw-rw-r--   0 root         (0) root         (0)     5051 2023-03-29 15:59:03.000000 QSCOUT-gatemodels-1.1.1/src/qscout/v1/std/noisy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:24:32.000000 QSCOUT-gatemodels-1.1.1/src/qscout/v1/std/stretched/
--rw-rw-r--   0 root         (0) root         (0)      494 2023-03-29 15:59:03.000000 QSCOUT-gatemodels-1.1.1/src/qscout/v1/std/stretched/jaqal_gates.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:24:32.000000 QSCOUT-gatemodels-1.1.1/tests/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-29 15:59:03.000000 QSCOUT-gatemodels-1.1.1/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:24:32.000000 QSCOUT-gatemodels-1.1.1/tests/parser/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-29 15:59:03.000000 QSCOUT-gatemodels-1.1.1/tests/parser/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8190 2023-03-29 15:59:03.000000 QSCOUT-gatemodels-1.1.1/tests/parser/test_jaqalpup_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:28.000000 QSCOUT-gatemodels-1.2.0a1/
+-rw-rw-r--   0 root         (0) root         (0)    11358 2023-05-19 20:38:38.000000 QSCOUT-gatemodels-1.2.0a1/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      197 2023-05-19 20:38:38.000000 QSCOUT-gatemodels-1.2.0a1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     2156 2023-05-19 23:36:28.000000 QSCOUT-gatemodels-1.2.0a1/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     1333 2023-05-19 20:38:38.000000 QSCOUT-gatemodels-1.2.0a1/README.md
+-rw-rw-r--   0 root         (0) root         (0)      111 2023-05-19 20:38:38.000000 QSCOUT-gatemodels-1.2.0a1/pyproject.toml
+-rw-rw-r--   0 root         (0) root         (0)     1169 2023-05-19 23:36:28.000000 QSCOUT-gatemodels-1.2.0a1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:28.000000 QSCOUT-gatemodels-1.2.0a1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:28.000000 QSCOUT-gatemodels-1.2.0a1/src/QSCOUT_gatemodels.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2156 2023-05-19 23:36:28.000000 QSCOUT-gatemodels-1.2.0a1/src/QSCOUT_gatemodels.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      599 2023-05-19 23:36:28.000000 QSCOUT-gatemodels-1.2.0a1/src/QSCOUT_gatemodels.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 23:36:28.000000 QSCOUT-gatemodels-1.2.0a1/src/QSCOUT_gatemodels.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2023-05-19 23:36:28.000000 QSCOUT-gatemodels-1.2.0a1/src/QSCOUT_gatemodels.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-19 23:36:28.000000 QSCOUT-gatemodels-1.2.0a1/src/QSCOUT_gatemodels.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:28.000000 QSCOUT-gatemodels-1.2.0a1/src/qscout/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:28.000000 QSCOUT-gatemodels-1.2.0a1/src/qscout/v1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:28.000000 QSCOUT-gatemodels-1.2.0a1/src/qscout/v1/std/
+-rw-rw-r--   0 root         (0) root         (0)     3205 2023-05-19 20:38:38.000000 QSCOUT-gatemodels-1.2.0a1/src/qscout/v1/std/jaqal_action.py
+-rw-rw-r--   0 root         (0) root         (0)     2740 2023-05-19 20:38:38.000000 QSCOUT-gatemodels-1.2.0a1/src/qscout/v1/std/jaqal_gates.py
+-rw-rw-r--   0 root         (0) root         (0)     5076 2023-05-19 20:38:38.000000 QSCOUT-gatemodels-1.2.0a1/src/qscout/v1/std/noisy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:28.000000 QSCOUT-gatemodels-1.2.0a1/src/qscout/v1/std/stretched/
+-rw-rw-r--   0 root         (0) root         (0)      167 2023-05-19 20:38:38.000000 QSCOUT-gatemodels-1.2.0a1/src/qscout/v1/std/stretched/jaqal_action.py
+-rw-rw-r--   0 root         (0) root         (0)      890 2023-05-19 20:38:38.000000 QSCOUT-gatemodels-1.2.0a1/src/qscout/v1/std/stretched/jaqal_gates.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:28.000000 QSCOUT-gatemodels-1.2.0a1/src/qscout/v1/zz/
+-rw-rw-r--   0 root         (0) root         (0)      781 2023-05-19 20:38:38.000000 QSCOUT-gatemodels-1.2.0a1/src/qscout/v1/zz/jaqal_action.py
+-rw-rw-r--   0 root         (0) root         (0)      762 2023-05-19 20:38:38.000000 QSCOUT-gatemodels-1.2.0a1/src/qscout/v1/zz/jaqal_gates.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:28.000000 QSCOUT-gatemodels-1.2.0a1/tests/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-19 20:38:38.000000 QSCOUT-gatemodels-1.2.0a1/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:28.000000 QSCOUT-gatemodels-1.2.0a1/tests/parser/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-19 20:38:38.000000 QSCOUT-gatemodels-1.2.0a1/tests/parser/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8190 2023-05-19 20:38:38.000000 QSCOUT-gatemodels-1.2.0a1/tests/parser/test_jaqalpup_parser.py
```

### Comparing `QSCOUT-gatemodels-1.1.1/LICENSE` & `QSCOUT-gatemodels-1.2.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `QSCOUT-gatemodels-1.1.1/PKG-INFO` & `QSCOUT-gatemodels-1.2.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QSCOUT-gatemodels
-Version: 1.1.1
+Version: 1.2.0a1
 Summary: QSCOUT Gate Models
 Home-page: https://qscout.sandia.gov
 Author: Benjamin C. A. Morrison, Jay Wesley Van Der Wall, Daniel Lobser, Antonio Russo, Kenneth Rudinger, Peter Maunz
 Author-email: qscout@sandia.gov
 License: Apache
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `QSCOUT-gatemodels-1.1.1/README.md` & `QSCOUT-gatemodels-1.2.0a1/README.md`

 * *Files identical despite different names*

### Comparing `QSCOUT-gatemodels-1.1.1/setup.cfg` & `QSCOUT-gatemodels-1.2.0a1/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 name = QSCOUT-gatemodels
 author = Benjamin C. A. Morrison, Jay Wesley Van Der Wall, Daniel Lobser, Antonio Russo, Kenneth Rudinger, Peter Maunz
 author_email = qscout@sandia.gov
 description = QSCOUT Gate Models
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = Apache
-version = 1.1.1
+version = 1.2.0a1
 home_page = https://qscout.sandia.gov
 classifiers = 
 	Development Status :: 4 - Beta
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3
 	Topic :: Scientific/Engineering :: Physics
@@ -18,15 +18,15 @@
 	Operating System :: MacOS :: MacOS X
 	Operating System :: Unix
 
 [options]
 packages = find_namespace:
 package_dir = 
 	=src
-install_requires = JaqalPaq>=1.1.1; numpy
+install_requires = JaqalPaq>=1.2.0a1; numpy
 python_requires = >=3.6.5
 platforms = any
 
 [options.packages.find]
 include = 
 	qscout
 	qscout.*
```

### Comparing `QSCOUT-gatemodels-1.1.1/src/QSCOUT_gatemodels.egg-info/PKG-INFO` & `QSCOUT-gatemodels-1.2.0a1/src/QSCOUT_gatemodels.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QSCOUT-gatemodels
-Version: 1.1.1
+Version: 1.2.0a1
 Summary: QSCOUT Gate Models
 Home-page: https://qscout.sandia.gov
 Author: Benjamin C. A. Morrison, Jay Wesley Van Der Wall, Daniel Lobser, Antonio Russo, Kenneth Rudinger, Peter Maunz
 Author-email: qscout@sandia.gov
 License: Apache
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `QSCOUT-gatemodels-1.1.1/src/qscout/v1/std/noisy.py` & `QSCOUT-gatemodels-1.2.0a1/src/qscout/v1/std/noisy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # Copyright 2020 National Technology & Engineering Solutions of Sandia, LLC (NTESS).
 # Under the terms of Contract DE-NA0003525 with NTESS, the U.S. Government retains
 # certain rights in this software.
 from numpy import abs, diag, pi, kron
 
 import pygsti
 
-from .jaqal_gates import U_R, U_Rz, U_MS, ALL_GATES
+from .jaqal_gates import ALL_GATES
+from .jaqal_action import U_R, U_Rz, U_MS
 from .stretched import jaqal_gates as stretched
 from jaqalpaq.emulator.pygsti import AbstractNoisyNativeEmulator
 
 
 class SNLToy1(AbstractNoisyNativeEmulator):
     """Version 1 error model of the QSCOUT native gates."""
```

### Comparing `QSCOUT-gatemodels-1.1.1/tests/parser/test_jaqalpup_parser.py` & `QSCOUT-gatemodels-1.2.0a1/tests/parser/test_jaqalpup_parser.py`

 * *Files identical despite different names*

