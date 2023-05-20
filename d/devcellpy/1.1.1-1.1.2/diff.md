# Comparing `tmp/devcellpy-1.1.1.tar.gz` & `tmp/devcellpy-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devcellpy-1.1.1.tar", last modified: Thu May 11 05:14:13 2023, max compression
+gzip compressed data, was "devcellpy-1.1.2.tar", last modified: Sat May 20 19:02:47 2023, max compression
```

## Comparing `devcellpy-1.1.1.tar` & `devcellpy-1.1.2.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxr-xr-x   0 vivian     (501) staff       (20)        0 2023-05-11 05:14:13.076004 devcellpy-1.1.1/
--rw-r--r--   0 vivian     (501) staff       (20)     1063 2022-08-21 02:13:40.000000 devcellpy-1.1.1/LICENSE.txt
--rw-r--r--   0 vivian     (501) staff       (20)     2505 2023-05-11 05:14:13.075261 devcellpy-1.1.1/PKG-INFO
--rw-r--r--   0 vivian     (501) staff       (20)     1665 2022-08-21 02:13:49.000000 devcellpy-1.1.1/README.md
-drwxr-xr-x   0 vivian     (501) staff       (20)        0 2023-05-11 05:14:13.068657 devcellpy-1.1.1/devcellpy/
--rw-r--r--   0 vivian     (501) staff       (20)       78 2023-05-11 05:08:29.000000 devcellpy-1.1.1/devcellpy/__init__.py
--rw-r--r--   0 vivian     (501) staff       (20)      379 2023-05-11 04:53:11.000000 devcellpy-1.1.1/devcellpy/config.py
--rw-r--r--   0 vivian     (501) staff       (20)     2469 2023-05-11 04:53:32.000000 devcellpy-1.1.1/devcellpy/featurerank.py
--rw-r--r--   0 vivian     (501) staff       (20)     1211 2023-05-11 04:53:49.000000 devcellpy-1.1.1/devcellpy/helpers.py
--rw-r--r--   0 vivian     (501) staff       (20)      529 2023-05-11 04:54:07.000000 devcellpy-1.1.1/devcellpy/importing_modules.py
--rw-r--r--   0 vivian     (501) staff       (20)    30565 2023-05-11 04:54:29.000000 devcellpy-1.1.1/devcellpy/layer.py
--rw-r--r--   0 vivian     (501) staff       (20)    10295 2023-05-11 04:54:49.000000 devcellpy-1.1.1/devcellpy/main.py
--rw-r--r--   0 vivian     (501) staff       (20)     7806 2023-05-11 04:55:11.000000 devcellpy-1.1.1/devcellpy/predict.py
--rw-r--r--   0 vivian     (501) staff       (20)     1656 2023-05-11 04:55:41.000000 devcellpy-1.1.1/devcellpy/setup.py
--rw-r--r--   0 vivian     (501) staff       (20)     6344 2023-05-11 04:56:13.000000 devcellpy-1.1.1/devcellpy/train.py
-drwxr-xr-x   0 vivian     (501) staff       (20)        0 2023-05-11 05:14:13.074403 devcellpy-1.1.1/devcellpy.egg-info/
--rw-r--r--   0 vivian     (501) staff       (20)     2505 2023-05-11 05:14:13.000000 devcellpy-1.1.1/devcellpy.egg-info/PKG-INFO
--rw-r--r--   0 vivian     (501) staff       (20)      445 2023-05-11 05:14:13.000000 devcellpy-1.1.1/devcellpy.egg-info/SOURCES.txt
--rw-r--r--   0 vivian     (501) staff       (20)        1 2023-05-11 05:14:13.000000 devcellpy-1.1.1/devcellpy.egg-info/dependency_links.txt
--rw-r--r--   0 vivian     (501) staff       (20)       55 2023-05-11 05:14:13.000000 devcellpy-1.1.1/devcellpy.egg-info/entry_points.txt
--rw-r--r--   0 vivian     (501) staff       (20)       41 2023-05-11 05:14:13.000000 devcellpy-1.1.1/devcellpy.egg-info/requires.txt
--rw-r--r--   0 vivian     (501) staff       (20)       10 2023-05-11 05:14:13.000000 devcellpy-1.1.1/devcellpy.egg-info/top_level.txt
--rw-r--r--   0 vivian     (501) staff       (20)       38 2023-05-11 05:14:13.076199 devcellpy-1.1.1/setup.cfg
--rw-r--r--   0 vivian     (501) staff       (20)     1428 2023-05-11 04:57:25.000000 devcellpy-1.1.1/setup.py
+drwxr-xr-x   0 vivian     (501) staff       (20)        0 2023-05-20 19:02:47.289306 devcellpy-1.1.2/
+-rw-r--r--   0 vivian     (501) staff       (20)     1063 2022-08-21 02:13:40.000000 devcellpy-1.1.2/LICENSE.txt
+-rw-r--r--   0 vivian     (501) staff       (20)     2505 2023-05-20 19:02:47.289013 devcellpy-1.1.2/PKG-INFO
+-rw-r--r--   0 vivian     (501) staff       (20)     1665 2022-08-21 02:13:49.000000 devcellpy-1.1.2/README.md
+drwxr-xr-x   0 vivian     (501) staff       (20)        0 2023-05-20 19:02:47.285803 devcellpy-1.1.2/devcellpy/
+-rw-r--r--   0 vivian     (501) staff       (20)        0 2023-05-20 18:58:00.000000 devcellpy-1.1.2/devcellpy/__init__.py
+-rw-r--r--   0 vivian     (501) staff       (20)    10275 2023-05-20 18:58:25.000000 devcellpy-1.1.2/devcellpy/__main__.py
+-rw-r--r--   0 vivian     (501) staff       (20)      380 2023-05-20 18:58:49.000000 devcellpy-1.1.2/devcellpy/config.py
+-rw-r--r--   0 vivian     (501) staff       (20)     2471 2023-05-20 18:59:06.000000 devcellpy-1.1.2/devcellpy/featurerank.py
+-rw-r--r--   0 vivian     (501) staff       (20)     1201 2023-05-20 18:59:27.000000 devcellpy-1.1.2/devcellpy/helpers.py
+-rw-r--r--   0 vivian     (501) staff       (20)      529 2023-05-20 18:59:47.000000 devcellpy-1.1.2/devcellpy/importing_modules.py
+-rw-r--r--   0 vivian     (501) staff       (20)    30567 2023-05-20 19:00:09.000000 devcellpy-1.1.2/devcellpy/layer.py
+-rw-r--r--   0 vivian     (501) staff       (20)     7808 2023-05-20 19:00:30.000000 devcellpy-1.1.2/devcellpy/predict.py
+-rw-r--r--   0 vivian     (501) staff       (20)     6347 2023-05-20 19:00:48.000000 devcellpy-1.1.2/devcellpy/train.py
+drwxr-xr-x   0 vivian     (501) staff       (20)        0 2023-05-20 19:02:47.288650 devcellpy-1.1.2/devcellpy.egg-info/
+-rw-r--r--   0 vivian     (501) staff       (20)     2505 2023-05-20 19:02:47.000000 devcellpy-1.1.2/devcellpy.egg-info/PKG-INFO
+-rw-r--r--   0 vivian     (501) staff       (20)      430 2023-05-20 19:02:47.000000 devcellpy-1.1.2/devcellpy.egg-info/SOURCES.txt
+-rw-r--r--   0 vivian     (501) staff       (20)        1 2023-05-20 19:02:47.000000 devcellpy-1.1.2/devcellpy.egg-info/dependency_links.txt
+-rw-r--r--   0 vivian     (501) staff       (20)       55 2023-05-20 19:02:47.000000 devcellpy-1.1.2/devcellpy.egg-info/entry_points.txt
+-rw-r--r--   0 vivian     (501) staff       (20)       41 2023-05-20 19:02:47.000000 devcellpy-1.1.2/devcellpy.egg-info/requires.txt
+-rw-r--r--   0 vivian     (501) staff       (20)       10 2023-05-20 19:02:47.000000 devcellpy-1.1.2/devcellpy.egg-info/top_level.txt
+-rw-r--r--   0 vivian     (501) staff       (20)       38 2023-05-20 19:02:47.289398 devcellpy-1.1.2/setup.cfg
+-rw-r--r--   0 vivian     (501) staff       (20)     1428 2023-05-20 19:01:18.000000 devcellpy-1.1.2/setup.py
```

### Comparing `devcellpy-1.1.1/LICENSE.txt` & `devcellpy-1.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `devcellpy-1.1.1/PKG-INFO` & `devcellpy-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devcellpy
-Version: 1.1.1
+Version: 1.1.2
 Summary: DevCellPy is a Python package designed for hierarchical multilayered classification of cells based on single-cell RNA-sequencing (scRNA-seq). It implements the machine learning algorithm Extreme Gradient Boost (XGBoost) (Chen and Guestrin, 2016) to automatically predict cell identities across complex permutations of layers and sublayers of annotation.
 Home-page: https://github.com/DevCellPy-Team/DevCellPy
 Author: Francisco Galdos and Sidra Xu
 Author-email: <fxgaldos@stanford.edu> and <sidraxu@stanford.edu>
 License: MIT
 Keywords: python,cardiology,scRNA,genetics,machine learning,biology,bioinformatics,devcellpy
 Classifier: Intended Audience :: Science/Research
```

### Comparing `devcellpy-1.1.1/README.md` & `devcellpy-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `devcellpy-1.1.1/devcellpy/featurerank.py` & `devcellpy-1.1.2/devcellpy/featurerank.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-from importing_modules import *
-import config
-import helpers
+from .importing_modules import *
+from . import config, helpers
 
 def check_featurerankingfiles(train_normexpr, train_metadata, layer_paths, frsplit):
     passed = True
     if not os.path.exists(train_normexpr):
         print('ERROR: Given normalized expression data file for training does not exist')
         passed = False
     if not os.path.exists(train_metadata):
```

### Comparing `devcellpy-1.1.1/devcellpy/helpers.py` & `devcellpy-1.1.2/devcellpy/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from importing_modules import *
+from .config import *
 
 # Converts the normalized expression csv into a pkl
 # Expression CSV file must contain genes as row names, samples as column names
 # First column name (cell A1) is 'gene'
 def csv2pkl(csvpath):
     tp = pd.read_csv(csvpath, iterator=True, chunksize=1000)
     norm_express = pd.concat(tp, ignore_index=True)
```

### Comparing `devcellpy-1.1.1/devcellpy/importing_modules.py` & `devcellpy-1.1.2/devcellpy/importing_modules.py`

 * *Files identical despite different names*

### Comparing `devcellpy-1.1.1/devcellpy/layer.py` & `devcellpy-1.1.2/devcellpy/layer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-from importing_modules import *
-import config
-import helpers
+from .importing_modules import *
+from . import config, helpers
 
 # Object for each layer of the model
 # Contains methods for subsetting data according to the metadata and label info files,
 #                      dividing subsetted data 90-10 and 10 fold cv,
 #                      finetuning and training each layer, calculating metrics and SHAP feature ranking,
 #                      outputting final model for validation
 # Keeps track of all outputted files, stores paths and names in instance variables
```

### Comparing `devcellpy-1.1.1/devcellpy/main.py` & `devcellpy-1.1.2/devcellpy/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
-from importing_modules import *
-import config as config
-import train
-import predict
-import featurerank
+from .importing_modules import *
+from . import config, train, predict, featurerank
 
 # Ensures given files satisfy one of the possible pathways provided by devcellpy
 # Ensures user input for train or predict matches file inputs
 # Certain files must appear together for training and/or validation to proceed
 def check_combinations(user_train, user_predictOne, user_predictAll, user_fr, train_normexpr, labelinfo, train_metadata, testsplit,
                        rejection_cutoff, val_normexpr, val_metadata, layer_paths, frsplit):
     passed = True
```

### Comparing `devcellpy-1.1.1/devcellpy/predict.py` & `devcellpy-1.1.2/devcellpy/predict.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-from importing_modules import *
-import config
-import helpers
+from .importing_modules import *
+from . import config, helpers
 
 # Ensures all the user given variables for predictOne or predictAll exist and are in the correct format
 def check_predictionfiles(val_normexpr, val_metadata, layer_paths):
     passed = True
     if not os.path.exists(val_normexpr):
         print('ERROR: Given validation normalized expression data file for prediction does not exist')
         passed = False
```

### Comparing `devcellpy-1.1.1/devcellpy/train.py` & `devcellpy-1.1.2/devcellpy/train.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from importing_modules import *
-import config
-import helpers
-from layer import Layer
+from .importing_modules import *
+from . import config, helpers
+from .layer import Layer
 
 # Ensures all the user given variables for training exist or are in bounds
 def check_trainingfiles(train_normexpr, labelinfo, train_metadata, testsplit, rejection_cutoff):
     passed = True
     if not os.path.exists(train_normexpr):
         print('ERROR: Given normalized expression data file for training does not exist')
         passed = False
```

### Comparing `devcellpy-1.1.1/devcellpy.egg-info/PKG-INFO` & `devcellpy-1.1.2/devcellpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devcellpy
-Version: 1.1.1
+Version: 1.1.2
 Summary: DevCellPy is a Python package designed for hierarchical multilayered classification of cells based on single-cell RNA-sequencing (scRNA-seq). It implements the machine learning algorithm Extreme Gradient Boost (XGBoost) (Chen and Guestrin, 2016) to automatically predict cell identities across complex permutations of layers and sublayers of annotation.
 Home-page: https://github.com/DevCellPy-Team/DevCellPy
 Author: Francisco Galdos and Sidra Xu
 Author-email: <fxgaldos@stanford.edu> and <sidraxu@stanford.edu>
 License: MIT
 Keywords: python,cardiology,scRNA,genetics,machine learning,biology,bioinformatics,devcellpy
 Classifier: Intended Audience :: Science/Research
```

### Comparing `devcellpy-1.1.1/setup.py` & `devcellpy-1.1.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '1.1.1'
+VERSION = '1.1.2'
 DESCRIPTION = 'DevCellPy is a Python package designed for hierarchical multilayered classification of cells based on single-cell RNA-sequencing (scRNA-seq). It implements the machine learning algorithm Extreme Gradient Boost (XGBoost) (Chen and Guestrin, 2016) to automatically predict cell identities across complex permutations of layers and sublayers of annotation.'
 
 HERE = pathlib.Path(__file__).parent
 
 README = (HERE / "README.md").read_text()
 
 setup(
```

