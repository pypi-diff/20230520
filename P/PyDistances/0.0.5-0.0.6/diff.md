# Comparing `tmp/PyDistances-0.0.5.tar.gz` & `tmp/PyDistances-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyDistances-0.0.5.tar", last modified: Sat May 20 11:50:19 2023, max compression
+gzip compressed data, was "PyDistances-0.0.6.tar", last modified: Sat May 20 12:00:58 2023, max compression
```

## Comparing `PyDistances-0.0.5.tar` & `PyDistances-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 11:50:19.887133 PyDistances-0.0.5/
--rw-rw-rw-   0        0        0     1091 2023-05-13 15:25:04.000000 PyDistances-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     1057 2023-05-20 11:50:19.886136 PyDistances-0.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-20 11:50:19.872306 PyDistances-0.0.5/PyDistances/
--rw-rw-rw-   0        0        0       40 2023-05-20 10:58:09.000000 PyDistances-0.0.5/PyDistances/__init__.py
--rw-rw-rw-   0        0        0     1110 2023-05-20 11:21:03.000000 PyDistances-0.0.5/PyDistances/distances.py
-drwxrwxrwx   0        0        0        0 2023-05-20 11:50:19.884139 PyDistances-0.0.5/PyDistances.egg-info/
--rw-rw-rw-   0        0        0     1057 2023-05-20 11:50:19.000000 PyDistances-0.0.5/PyDistances.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-05-20 11:50:19.000000 PyDistances-0.0.5/PyDistances.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 11:50:19.000000 PyDistances-0.0.5/PyDistances.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-20 11:50:19.000000 PyDistances-0.0.5/PyDistances.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-20 11:50:19.000000 PyDistances-0.0.5/PyDistances.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      328 2023-05-20 11:48:39.000000 PyDistances-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-05-20 11:50:19.887133 PyDistances-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1070 2023-05-20 11:49:45.000000 PyDistances-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 12:00:58.494213 PyDistances-0.0.6/
+-rw-rw-rw-   0        0        0     1091 2023-05-13 15:25:04.000000 PyDistances-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     1069 2023-05-20 12:00:58.494213 PyDistances-0.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-20 12:00:58.480251 PyDistances-0.0.6/PyDistances/
+-rw-rw-rw-   0        0        0       40 2023-05-20 10:58:09.000000 PyDistances-0.0.6/PyDistances/__init__.py
+-rw-rw-rw-   0        0        0     1110 2023-05-20 11:21:03.000000 PyDistances-0.0.6/PyDistances/distances.py
+drwxrwxrwx   0        0        0        0 2023-05-20 12:00:58.492219 PyDistances-0.0.6/PyDistances.egg-info/
+-rw-rw-rw-   0        0        0     1069 2023-05-20 12:00:58.000000 PyDistances-0.0.6/PyDistances.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-05-20 12:00:58.000000 PyDistances-0.0.6/PyDistances.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 12:00:58.000000 PyDistances-0.0.6/PyDistances.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-20 12:00:58.000000 PyDistances-0.0.6/PyDistances.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-20 12:00:58.000000 PyDistances-0.0.6/PyDistances.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      340 2023-05-20 11:51:44.000000 PyDistances-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-20 12:00:58.495221 PyDistances-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1065 2023-05-20 11:59:56.000000 PyDistances-0.0.6/setup.py
```

### Comparing `PyDistances-0.0.5/LICENSE` & `PyDistances-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `PyDistances-0.0.5/PKG-INFO` & `PyDistances-0.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: PyDistances
-Version: 0.0.5
+Version: 0.0.6
 Summary: This is a package for computing distances among observations of statistical variables, such as: Euclidean, Minkowski, Canberra, Pearson, Mahalanobis, Robust Mahalanobis, Gower, Generalized Gower and Related Metric Scaling (RelMS). A total of 41 statistical distances can be computed.
 Home-page: https://github.com/FabioScielzoOrtiz/Distances_Package
 Author: Fabio Scielzo Ortiz
 Author-email: fabioscielzo98@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# PyDistances: A Python Distances Package
+# PyDistances: A Statistical Distances Python Package
 
 This is a package for computing distances among observations of statistical variables, such as: Euclidean, Minkowski, Canberra, Pearson, Mahalanobis, Robust Mahalanobis, Gower, Generalized Gower and Related Metric Scaling (RelMS). A total of 41 statistical distances can be computed.
```

### Comparing `PyDistances-0.0.5/PyDistances/distances.py` & `PyDistances-0.0.6/PyDistances/distances.py`

 * *Files identical despite different names*

### Comparing `PyDistances-0.0.5/PyDistances.egg-info/PKG-INFO` & `PyDistances-0.0.6/PyDistances.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: PyDistances
-Version: 0.0.5
+Version: 0.0.6
 Summary: This is a package for computing distances among observations of statistical variables, such as: Euclidean, Minkowski, Canberra, Pearson, Mahalanobis, Robust Mahalanobis, Gower, Generalized Gower and Related Metric Scaling (RelMS). A total of 41 statistical distances can be computed.
 Home-page: https://github.com/FabioScielzoOrtiz/Distances_Package
 Author: Fabio Scielzo Ortiz
 Author-email: fabioscielzo98@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# PyDistances: A Python Distances Package
+# PyDistances: A Statistical Distances Python Package
 
 This is a package for computing distances among observations of statistical variables, such as: Euclidean, Minkowski, Canberra, Pearson, Mahalanobis, Robust Mahalanobis, Gower, Generalized Gower and Related Metric Scaling (RelMS). A total of 41 statistical distances can be computed.
```

### Comparing `PyDistances-0.0.5/setup.py` & `PyDistances-0.0.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from setuptools import setup, find_packages
 
+import numpy as np
+
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="PyDistances",
-    version="0.0.5",
+    version="0.0.6",
     author="Fabio Scielzo Ortiz",
     author_email="fabioscielzo98@gmail.com",
     description="This is a package for computing distances among observations of statistical variables, such as: Euclidean, Minkowski, Canberra, Pearson, Mahalanobis, Robust Mahalanobis, Gower, Generalized Gower and Related Metric Scaling (RelMS). A total of 41 statistical distances can be computed.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/FabioScielzoOrtiz/Distances_Package",  # add your project URL here
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    install_requires=[
-        'pandas',
-        'numpy'
-     ],
+    install_requires=['pandas','numpy'],
     python_requires=">=3.7"
 )
```

