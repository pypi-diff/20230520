# Comparing `tmp/PyDistances-0.0.3.tar.gz` & `tmp/PyDistances-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyDistances-0.0.3.tar", last modified: Sat May 20 11:24:40 2023, max compression
+gzip compressed data, was "PyDistances-0.0.4.tar", last modified: Sat May 20 11:46:58 2023, max compression
```

## Comparing `PyDistances-0.0.3.tar` & `PyDistances-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 11:24:40.204213 PyDistances-0.0.3/
--rw-rw-rw-   0        0        0     1091 2023-05-13 15:25:04.000000 PyDistances-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     1033 2023-05-20 11:24:40.203218 PyDistances-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-20 11:24:40.190597 PyDistances-0.0.3/PyDistances/
--rw-rw-rw-   0        0        0       40 2023-05-20 10:58:09.000000 PyDistances-0.0.3/PyDistances/__init__.py
--rw-rw-rw-   0        0        0     1110 2023-05-20 11:21:03.000000 PyDistances-0.0.3/PyDistances/distances.py
-drwxrwxrwx   0        0        0        0 2023-05-20 11:24:40.202215 PyDistances-0.0.3/PyDistances.egg-info/
--rw-rw-rw-   0        0        0     1033 2023-05-20 11:24:40.000000 PyDistances-0.0.3/PyDistances.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      215 2023-05-20 11:24:40.000000 PyDistances-0.0.3/PyDistances.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 11:24:40.000000 PyDistances-0.0.3/PyDistances.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-05-20 11:24:40.000000 PyDistances-0.0.3/PyDistances.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      304 2023-05-20 11:02:56.000000 PyDistances-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-20 11:24:40.204213 PyDistances-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1002 2023-05-20 11:24:26.000000 PyDistances-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 11:46:58.164046 PyDistances-0.0.4/
+-rw-rw-rw-   0        0        0     1091 2023-05-13 15:25:04.000000 PyDistances-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1033 2023-05-20 11:46:58.163047 PyDistances-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-20 11:46:58.152077 PyDistances-0.0.4/PyDistances/
+-rw-rw-rw-   0        0        0       40 2023-05-20 10:58:09.000000 PyDistances-0.0.4/PyDistances/__init__.py
+-rw-rw-rw-   0        0        0     1110 2023-05-20 11:21:03.000000 PyDistances-0.0.4/PyDistances/distances.py
+drwxrwxrwx   0        0        0        0 2023-05-20 11:46:58.161053 PyDistances-0.0.4/PyDistances.egg-info/
+-rw-rw-rw-   0        0        0     1033 2023-05-20 11:46:57.000000 PyDistances-0.0.4/PyDistances.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-05-20 11:46:58.000000 PyDistances-0.0.4/PyDistances.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 11:46:57.000000 PyDistances-0.0.4/PyDistances.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-20 11:46:57.000000 PyDistances-0.0.4/PyDistances.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-20 11:46:57.000000 PyDistances-0.0.4/PyDistances.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      304 2023-05-20 11:02:56.000000 PyDistances-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-20 11:46:58.164046 PyDistances-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1070 2023-05-20 11:46:22.000000 PyDistances-0.0.4/setup.py
```

### Comparing `PyDistances-0.0.3/LICENSE` & `PyDistances-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `PyDistances-0.0.3/PKG-INFO` & `PyDistances-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyDistances
-Version: 0.0.3
+Version: 0.0.4
 Summary: This is a package for computing distances among observations of statistical variables, such as: Euclidean, Minkowski, Canberra, Pearson, Mahalanobis, Robust Mahalanobis, Gower, Generalized Gower and Related Metric Scaling (RelMS). A total of 41 statistical distances can be computed.
 Home-page: https://github.com/FabioScielzoOrtiz/Distances_Package
 Author: Fabio Scielzo Ortiz
 Author-email: fabioscielzo98@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PyDistances-0.0.3/PyDistances/distances.py` & `PyDistances-0.0.4/PyDistances/distances.py`

 * *Files identical despite different names*

### Comparing `PyDistances-0.0.3/PyDistances.egg-info/PKG-INFO` & `PyDistances-0.0.4/PyDistances.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyDistances
-Version: 0.0.3
+Version: 0.0.4
 Summary: This is a package for computing distances among observations of statistical variables, such as: Euclidean, Minkowski, Canberra, Pearson, Mahalanobis, Robust Mahalanobis, Gower, Generalized Gower and Related Metric Scaling (RelMS). A total of 41 statistical distances can be computed.
 Home-page: https://github.com/FabioScielzoOrtiz/Distances_Package
 Author: Fabio Scielzo Ortiz
 Author-email: fabioscielzo98@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PyDistances-0.0.3/setup.py` & `PyDistances-0.0.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="PyDistances",
-    version="0.0.3",
+    version="0.0.4",
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
-    python_requires=">=3.7",
+    install_requires=[
+        'pandas',
+        'numpy'
+     ],
+    python_requires=">=3.7"
 )
```

