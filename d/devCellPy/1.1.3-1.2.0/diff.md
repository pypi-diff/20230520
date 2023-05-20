# Comparing `tmp/devCellPy-1.1.3.tar.gz` & `tmp/devCellPy-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devCellPy-1.1.3.tar", last modified: Sat May 20 19:35:24 2023, max compression
+gzip compressed data, was "devCellPy-1.2.0.tar", last modified: Sat May 20 19:46:28 2023, max compression
```

## Comparing `devCellPy-1.1.3.tar` & `devCellPy-1.2.0.tar`

### file list

```diff
@@ -1,23 +1,22 @@
-drwxr-xr-x   0 vivian     (501) staff       (20)        0 2023-05-20 19:35:24.750545 devCellPy-1.1.3/
--rw-r--r--   0 vivian     (501) staff       (20)     1063 2022-08-21 02:13:40.000000 devCellPy-1.1.3/LICENSE.txt
--rw-r--r--   0 vivian     (501) staff       (20)     2505 2023-05-20 19:35:24.750182 devCellPy-1.1.3/PKG-INFO
--rw-r--r--   0 vivian     (501) staff       (20)     1665 2022-08-21 02:13:49.000000 devCellPy-1.1.3/README.md
-drwxr-xr-x   0 vivian     (501) staff       (20)        0 2023-05-20 19:35:24.747214 devCellPy-1.1.3/devCellPy/
--rw-r--r--   0 vivian     (501) staff       (20)        0 2023-05-20 18:58:00.000000 devCellPy-1.1.3/devCellPy/__init__.py
--rw-r--r--   0 vivian     (501) staff       (20)    10275 2023-05-20 18:58:25.000000 devCellPy-1.1.3/devCellPy/__main__.py
--rw-r--r--   0 vivian     (501) staff       (20)      380 2023-05-20 18:58:49.000000 devCellPy-1.1.3/devCellPy/config.py
--rw-r--r--   0 vivian     (501) staff       (20)     2471 2023-05-20 18:59:06.000000 devCellPy-1.1.3/devCellPy/featurerank.py
--rw-r--r--   0 vivian     (501) staff       (20)     1201 2023-05-20 18:59:27.000000 devCellPy-1.1.3/devCellPy/helpers.py
--rw-r--r--   0 vivian     (501) staff       (20)      529 2023-05-20 18:59:47.000000 devCellPy-1.1.3/devCellPy/importing_modules.py
--rw-r--r--   0 vivian     (501) staff       (20)    30567 2023-05-20 19:00:09.000000 devCellPy-1.1.3/devCellPy/layer.py
--rw-r--r--   0 vivian     (501) staff       (20)     7808 2023-05-20 19:00:30.000000 devCellPy-1.1.3/devCellPy/predict.py
--rw-r--r--   0 vivian     (501) staff       (20)     6347 2023-05-20 19:00:48.000000 devCellPy-1.1.3/devCellPy/train.py
-drwxr-xr-x   0 vivian     (501) staff       (20)        0 2023-05-20 19:35:24.749835 devCellPy-1.1.3/devCellPy.egg-info/
--rw-r--r--   0 vivian     (501) staff       (20)     2505 2023-05-20 19:35:24.000000 devCellPy-1.1.3/devCellPy.egg-info/PKG-INFO
--rw-r--r--   0 vivian     (501) staff       (20)      430 2023-05-20 19:35:24.000000 devCellPy-1.1.3/devCellPy.egg-info/SOURCES.txt
--rw-r--r--   0 vivian     (501) staff       (20)        1 2023-05-20 19:35:24.000000 devCellPy-1.1.3/devCellPy.egg-info/dependency_links.txt
--rw-r--r--   0 vivian     (501) staff       (20)       54 2023-05-20 19:35:24.000000 devCellPy-1.1.3/devCellPy.egg-info/entry_points.txt
--rw-r--r--   0 vivian     (501) staff       (20)       41 2023-05-20 19:35:24.000000 devCellPy-1.1.3/devCellPy.egg-info/requires.txt
--rw-r--r--   0 vivian     (501) staff       (20)       10 2023-05-20 19:35:24.000000 devCellPy-1.1.3/devCellPy.egg-info/top_level.txt
--rw-r--r--   0 vivian     (501) staff       (20)       38 2023-05-20 19:35:24.750681 devCellPy-1.1.3/setup.cfg
--rw-r--r--   0 vivian     (501) staff       (20)     1427 2023-05-20 19:34:08.000000 devCellPy-1.1.3/setup.py
+drwxr-xr-x   0 vivian     (501) staff       (20)        0 2023-05-20 19:46:28.502220 devCellPy-1.2.0/
+-rw-r--r--   0 vivian     (501) staff       (20)     1063 2022-08-21 02:13:40.000000 devCellPy-1.2.0/LICENSE.txt
+-rw-r--r--   0 vivian     (501) staff       (20)      756 2023-05-20 19:46:28.501551 devCellPy-1.2.0/PKG-INFO
+-rw-r--r--   0 vivian     (501) staff       (20)     1665 2022-08-21 02:13:49.000000 devCellPy-1.2.0/README.md
+drwxr-xr-x   0 vivian     (501) staff       (20)        0 2023-05-20 19:46:28.498659 devCellPy-1.2.0/devCellPy/
+-rw-r--r--   0 vivian     (501) staff       (20)        0 2023-05-20 18:58:00.000000 devCellPy-1.2.0/devCellPy/__init__.py
+-rw-r--r--   0 vivian     (501) staff       (20)    10275 2023-05-20 18:58:25.000000 devCellPy-1.2.0/devCellPy/__main__.py
+-rw-r--r--   0 vivian     (501) staff       (20)      380 2023-05-20 18:58:49.000000 devCellPy-1.2.0/devCellPy/config.py
+-rw-r--r--   0 vivian     (501) staff       (20)     2471 2023-05-20 18:59:06.000000 devCellPy-1.2.0/devCellPy/featurerank.py
+-rw-r--r--   0 vivian     (501) staff       (20)     1201 2023-05-20 18:59:27.000000 devCellPy-1.2.0/devCellPy/helpers.py
+-rw-r--r--   0 vivian     (501) staff       (20)      529 2023-05-20 18:59:47.000000 devCellPy-1.2.0/devCellPy/importing_modules.py
+-rw-r--r--   0 vivian     (501) staff       (20)    30567 2023-05-20 19:00:09.000000 devCellPy-1.2.0/devCellPy/layer.py
+-rw-r--r--   0 vivian     (501) staff       (20)     7808 2023-05-20 19:00:30.000000 devCellPy-1.2.0/devCellPy/predict.py
+-rw-r--r--   0 vivian     (501) staff       (20)     6347 2023-05-20 19:00:48.000000 devCellPy-1.2.0/devCellPy/train.py
+drwxr-xr-x   0 vivian     (501) staff       (20)        0 2023-05-20 19:46:28.500901 devCellPy-1.2.0/devCellPy.egg-info/
+-rw-r--r--   0 vivian     (501) staff       (20)      756 2023-05-20 19:46:28.000000 devCellPy-1.2.0/devCellPy.egg-info/PKG-INFO
+-rw-r--r--   0 vivian     (501) staff       (20)      398 2023-05-20 19:46:28.000000 devCellPy-1.2.0/devCellPy.egg-info/SOURCES.txt
+-rw-r--r--   0 vivian     (501) staff       (20)        1 2023-05-20 19:46:28.000000 devCellPy-1.2.0/devCellPy.egg-info/dependency_links.txt
+-rw-r--r--   0 vivian     (501) staff       (20)       54 2023-05-20 19:46:28.000000 devCellPy-1.2.0/devCellPy.egg-info/entry_points.txt
+-rw-r--r--   0 vivian     (501) staff       (20)       10 2023-05-20 19:46:28.000000 devCellPy-1.2.0/devCellPy.egg-info/top_level.txt
+-rw-r--r--   0 vivian     (501) staff       (20)       38 2023-05-20 19:46:28.502431 devCellPy-1.2.0/setup.cfg
+-rw-r--r--   0 vivian     (501) staff       (20)     1095 2023-05-20 19:46:08.000000 devCellPy-1.2.0/setup.py
```

### Comparing `devCellPy-1.1.3/LICENSE.txt` & `devCellPy-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `devCellPy-1.1.3/PKG-INFO` & `devCellPy-1.2.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: devCellPy
-Version: 1.1.3
-Summary: DevCellPy is a Python package designed for hierarchical multilayered classification of cells based on single-cell RNA-sequencing (scRNA-seq). It implements the machine learning algorithm Extreme Gradient Boost (XGBoost) (Chen and Guestrin, 2016) to automatically predict cell identities across complex permutations of layers and sublayers of annotation.
-Home-page: https://github.com/DevCellPy-Team/DevCellPy
-Author: Francisco Galdos and Sidra Xu
-Author-email: <fxgaldos@stanford.edu> and <sidraxu@stanford.edu>
-License: MIT
-Keywords: python,cardiology,scRNA,genetics,machine learning,biology,bioinformatics,devcellpy
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 ## DevCellPy
 DevCellPy is a Python package designed for hierarchical multilayered classification of cells based on single-cell RNA-sequencing (scRNA-seq). It implements the machine learning algorithm Extreme Gradient Boost (XGBoost) (Chen and Guestrin, 2016) to automatically predict cell identities across complex permutations of layers and sublayers of annotation.
 
 Given DevCellPy's highly customizable classification scheme, users can input the annotation hierarchy of their scRNA-seq datasets into DevCellPy to guide the automatic classification and prediction of cells according to the provided hierarchy. DevCellPy allows users to designate any identity at each layer of classification and is not constrained by cell type——for example, assigning timepoint as one of the annotation layers allows for cell identity predictions at that layer to be conditioned on the age of the cells. In addition to hierarchical cell classification, DevCellPy implements the SHapley Additive exPlanations (SHAP) package (Lundberg etal, 2020), which provides the user with interpretability methods for the model and determines the positive and negative gene predictors of cell identities across all annotation layers.
 
 We provide a comprehensive tutorial on DevCellPy's usage as well as overall concepts in its design in the tutorial folder of the DevCellPy GitHub.
```

### Comparing `devCellPy-1.1.3/devCellPy/__main__.py` & `devCellPy-1.2.0/devCellPy/__main__.py`

 * *Files identical despite different names*

### Comparing `devCellPy-1.1.3/devCellPy/featurerank.py` & `devCellPy-1.2.0/devCellPy/featurerank.py`

 * *Files identical despite different names*

### Comparing `devCellPy-1.1.3/devCellPy/helpers.py` & `devCellPy-1.2.0/devCellPy/helpers.py`

 * *Files identical despite different names*

### Comparing `devCellPy-1.1.3/devCellPy/importing_modules.py` & `devCellPy-1.2.0/devCellPy/importing_modules.py`

 * *Files identical despite different names*

### Comparing `devCellPy-1.1.3/devCellPy/layer.py` & `devCellPy-1.2.0/devCellPy/layer.py`

 * *Files identical despite different names*

### Comparing `devCellPy-1.1.3/devCellPy/predict.py` & `devCellPy-1.2.0/devCellPy/predict.py`

 * *Files identical despite different names*

### Comparing `devCellPy-1.1.3/devCellPy/train.py` & `devCellPy-1.2.0/devCellPy/train.py`

 * *Files identical despite different names*

