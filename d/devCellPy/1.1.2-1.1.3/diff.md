# Comparing `tmp/devcellpy-1.1.2.tar.gz` & `tmp/devCellPy-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devcellpy-1.1.2.tar", last modified: Sat May 20 19:02:47 2023, max compression
+gzip compressed data, was "devCellPy-1.1.3.tar", last modified: Sat May 20 19:35:24 2023, max compression
```

## Comparing `devcellpy-1.1.2.tar` & `devCellPy-1.1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 vivian     (501) staff       (20)        0 2023-05-20 19:02:47.289306 devcellpy-1.1.2/
--rw-r--r--   0 vivian     (501) staff       (20)     1063 2022-08-21 02:13:40.000000 devcellpy-1.1.2/LICENSE.txt
--rw-r--r--   0 vivian     (501) staff       (20)     2505 2023-05-20 19:02:47.289013 devcellpy-1.1.2/PKG-INFO
--rw-r--r--   0 vivian     (501) staff       (20)     1665 2022-08-21 02:13:49.000000 devcellpy-1.1.2/README.md
-drwxr-xr-x   0 vivian     (501) staff       (20)        0 2023-05-20 19:02:47.285803 devcellpy-1.1.2/devcellpy/
--rw-r--r--   0 vivian     (501) staff       (20)        0 2023-05-20 18:58:00.000000 devcellpy-1.1.2/devcellpy/__init__.py
--rw-r--r--   0 vivian     (501) staff       (20)    10275 2023-05-20 18:58:25.000000 devcellpy-1.1.2/devcellpy/__main__.py
--rw-r--r--   0 vivian     (501) staff       (20)      380 2023-05-20 18:58:49.000000 devcellpy-1.1.2/devcellpy/config.py
--rw-r--r--   0 vivian     (501) staff       (20)     2471 2023-05-20 18:59:06.000000 devcellpy-1.1.2/devcellpy/featurerank.py
--rw-r--r--   0 vivian     (501) staff       (20)     1201 2023-05-20 18:59:27.000000 devcellpy-1.1.2/devcellpy/helpers.py
--rw-r--r--   0 vivian     (501) staff       (20)      529 2023-05-20 18:59:47.000000 devcellpy-1.1.2/devcellpy/importing_modules.py
--rw-r--r--   0 vivian     (501) staff       (20)    30567 2023-05-20 19:00:09.000000 devcellpy-1.1.2/devcellpy/layer.py
--rw-r--r--   0 vivian     (501) staff       (20)     7808 2023-05-20 19:00:30.000000 devcellpy-1.1.2/devcellpy/predict.py
--rw-r--r--   0 vivian     (501) staff       (20)     6347 2023-05-20 19:00:48.000000 devcellpy-1.1.2/devcellpy/train.py
-drwxr-xr-x   0 vivian     (501) staff       (20)        0 2023-05-20 19:02:47.288650 devcellpy-1.1.2/devcellpy.egg-info/
--rw-r--r--   0 vivian     (501) staff       (20)     2505 2023-05-20 19:02:47.000000 devcellpy-1.1.2/devcellpy.egg-info/PKG-INFO
--rw-r--r--   0 vivian     (501) staff       (20)      430 2023-05-20 19:02:47.000000 devcellpy-1.1.2/devcellpy.egg-info/SOURCES.txt
--rw-r--r--   0 vivian     (501) staff       (20)        1 2023-05-20 19:02:47.000000 devcellpy-1.1.2/devcellpy.egg-info/dependency_links.txt
--rw-r--r--   0 vivian     (501) staff       (20)       55 2023-05-20 19:02:47.000000 devcellpy-1.1.2/devcellpy.egg-info/entry_points.txt
--rw-r--r--   0 vivian     (501) staff       (20)       41 2023-05-20 19:02:47.000000 devcellpy-1.1.2/devcellpy.egg-info/requires.txt
--rw-r--r--   0 vivian     (501) staff       (20)       10 2023-05-20 19:02:47.000000 devcellpy-1.1.2/devcellpy.egg-info/top_level.txt
--rw-r--r--   0 vivian     (501) staff       (20)       38 2023-05-20 19:02:47.289398 devcellpy-1.1.2/setup.cfg
--rw-r--r--   0 vivian     (501) staff       (20)     1428 2023-05-20 19:01:18.000000 devcellpy-1.1.2/setup.py
+drwxr-xr-x   0 vivian     (501) staff       (20)        0 2023-05-20 19:35:24.750545 devCellPy-1.1.3/
+-rw-r--r--   0 vivian     (501) staff       (20)     1063 2022-08-21 02:13:40.000000 devCellPy-1.1.3/LICENSE.txt
+-rw-r--r--   0 vivian     (501) staff       (20)     2505 2023-05-20 19:35:24.750182 devCellPy-1.1.3/PKG-INFO
+-rw-r--r--   0 vivian     (501) staff       (20)     1665 2022-08-21 02:13:49.000000 devCellPy-1.1.3/README.md
+drwxr-xr-x   0 vivian     (501) staff       (20)        0 2023-05-20 19:35:24.747214 devCellPy-1.1.3/devCellPy/
+-rw-r--r--   0 vivian     (501) staff       (20)        0 2023-05-20 18:58:00.000000 devCellPy-1.1.3/devCellPy/__init__.py
+-rw-r--r--   0 vivian     (501) staff       (20)    10275 2023-05-20 18:58:25.000000 devCellPy-1.1.3/devCellPy/__main__.py
+-rw-r--r--   0 vivian     (501) staff       (20)      380 2023-05-20 18:58:49.000000 devCellPy-1.1.3/devCellPy/config.py
+-rw-r--r--   0 vivian     (501) staff       (20)     2471 2023-05-20 18:59:06.000000 devCellPy-1.1.3/devCellPy/featurerank.py
+-rw-r--r--   0 vivian     (501) staff       (20)     1201 2023-05-20 18:59:27.000000 devCellPy-1.1.3/devCellPy/helpers.py
+-rw-r--r--   0 vivian     (501) staff       (20)      529 2023-05-20 18:59:47.000000 devCellPy-1.1.3/devCellPy/importing_modules.py
+-rw-r--r--   0 vivian     (501) staff       (20)    30567 2023-05-20 19:00:09.000000 devCellPy-1.1.3/devCellPy/layer.py
+-rw-r--r--   0 vivian     (501) staff       (20)     7808 2023-05-20 19:00:30.000000 devCellPy-1.1.3/devCellPy/predict.py
+-rw-r--r--   0 vivian     (501) staff       (20)     6347 2023-05-20 19:00:48.000000 devCellPy-1.1.3/devCellPy/train.py
+drwxr-xr-x   0 vivian     (501) staff       (20)        0 2023-05-20 19:35:24.749835 devCellPy-1.1.3/devCellPy.egg-info/
+-rw-r--r--   0 vivian     (501) staff       (20)     2505 2023-05-20 19:35:24.000000 devCellPy-1.1.3/devCellPy.egg-info/PKG-INFO
+-rw-r--r--   0 vivian     (501) staff       (20)      430 2023-05-20 19:35:24.000000 devCellPy-1.1.3/devCellPy.egg-info/SOURCES.txt
+-rw-r--r--   0 vivian     (501) staff       (20)        1 2023-05-20 19:35:24.000000 devCellPy-1.1.3/devCellPy.egg-info/dependency_links.txt
+-rw-r--r--   0 vivian     (501) staff       (20)       54 2023-05-20 19:35:24.000000 devCellPy-1.1.3/devCellPy.egg-info/entry_points.txt
+-rw-r--r--   0 vivian     (501) staff       (20)       41 2023-05-20 19:35:24.000000 devCellPy-1.1.3/devCellPy.egg-info/requires.txt
+-rw-r--r--   0 vivian     (501) staff       (20)       10 2023-05-20 19:35:24.000000 devCellPy-1.1.3/devCellPy.egg-info/top_level.txt
+-rw-r--r--   0 vivian     (501) staff       (20)       38 2023-05-20 19:35:24.750681 devCellPy-1.1.3/setup.cfg
+-rw-r--r--   0 vivian     (501) staff       (20)     1427 2023-05-20 19:34:08.000000 devCellPy-1.1.3/setup.py
```

### Comparing `devcellpy-1.1.2/LICENSE.txt` & `devCellPy-1.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `devcellpy-1.1.2/PKG-INFO` & `devCellPy-1.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: devcellpy
-Version: 1.1.2
+Name: devCellPy
+Version: 1.1.3
 Summary: DevCellPy is a Python package designed for hierarchical multilayered classification of cells based on single-cell RNA-sequencing (scRNA-seq). It implements the machine learning algorithm Extreme Gradient Boost (XGBoost) (Chen and Guestrin, 2016) to automatically predict cell identities across complex permutations of layers and sublayers of annotation.
 Home-page: https://github.com/DevCellPy-Team/DevCellPy
 Author: Francisco Galdos and Sidra Xu
 Author-email: <fxgaldos@stanford.edu> and <sidraxu@stanford.edu>
 License: MIT
 Keywords: python,cardiology,scRNA,genetics,machine learning,biology,bioinformatics,devcellpy
 Classifier: Intended Audience :: Science/Research
```

### Comparing `devcellpy-1.1.2/README.md` & `devCellPy-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `devcellpy-1.1.2/devcellpy/__main__.py` & `devCellPy-1.1.3/devCellPy/__main__.py`

 * *Files identical despite different names*

### Comparing `devcellpy-1.1.2/devcellpy/featurerank.py` & `devCellPy-1.1.3/devCellPy/featurerank.py`

 * *Files identical despite different names*

### Comparing `devcellpy-1.1.2/devcellpy/helpers.py` & `devCellPy-1.1.3/devCellPy/helpers.py`

 * *Files identical despite different names*

### Comparing `devcellpy-1.1.2/devcellpy/importing_modules.py` & `devCellPy-1.1.3/devCellPy/importing_modules.py`

 * *Files identical despite different names*

### Comparing `devcellpy-1.1.2/devcellpy/layer.py` & `devCellPy-1.1.3/devCellPy/layer.py`

 * *Files identical despite different names*

### Comparing `devcellpy-1.1.2/devcellpy/predict.py` & `devCellPy-1.1.3/devCellPy/predict.py`

 * *Files identical despite different names*

### Comparing `devcellpy-1.1.2/devcellpy/train.py` & `devCellPy-1.1.3/devCellPy/train.py`

 * *Files identical despite different names*

### Comparing `devcellpy-1.1.2/devcellpy.egg-info/PKG-INFO` & `devCellPy-1.1.3/devCellPy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: devcellpy
-Version: 1.1.2
+Name: devCellPy
+Version: 1.1.3
 Summary: DevCellPy is a Python package designed for hierarchical multilayered classification of cells based on single-cell RNA-sequencing (scRNA-seq). It implements the machine learning algorithm Extreme Gradient Boost (XGBoost) (Chen and Guestrin, 2016) to automatically predict cell identities across complex permutations of layers and sublayers of annotation.
 Home-page: https://github.com/DevCellPy-Team/DevCellPy
 Author: Francisco Galdos and Sidra Xu
 Author-email: <fxgaldos@stanford.edu> and <sidraxu@stanford.edu>
 License: MIT
 Keywords: python,cardiology,scRNA,genetics,machine learning,biology,bioinformatics,devcellpy
 Classifier: Intended Audience :: Science/Research
```

### Comparing `devcellpy-1.1.2/setup.py` & `devCellPy-1.1.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import pathlib
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '1.1.2'
+VERSION = '1.1.3'
 DESCRIPTION = 'DevCellPy is a Python package designed for hierarchical multilayered classification of cells based on single-cell RNA-sequencing (scRNA-seq). It implements the machine learning algorithm Extreme Gradient Boost (XGBoost) (Chen and Guestrin, 2016) to automatically predict cell identities across complex permutations of layers and sublayers of annotation.'
 
 HERE = pathlib.Path(__file__).parent
 
 README = (HERE / "README.md").read_text()
 
 setup(
-    name="devcellpy",
+    name="devCellPy",
     version=VERSION,
     author = "Francisco Galdos and Sidra Xu",
     author_email="<fxgaldos@stanford.edu> and <sidraxu@stanford.edu>",
     description=DESCRIPTION,
     long_description=README,
     long_description_content_type="text/markdown",
     packages=find_packages(),
@@ -27,14 +27,14 @@
         "shap",
         "scanpy"],
     url="https://github.com/DevCellPy-Team/DevCellPy",
     license='MIT',
     keywords=["python","cardiology","scRNA","genetics","machine learning","biology","bioinformatics","devcellpy"],
     classifiers=["Intended Audience :: Science/Research","Programming Language :: Python"],
     include_package_data=True,
-    entry_points={
-        "console_scripts": [
-            "devcellpy=devcellpy.devcellpy:main",
-        ]
+    entry_points = {
+        'console_scripts': [
+            'devCellPy = devCellPy.__main__:main'
+        ],
     }
-    
+
     )
```

