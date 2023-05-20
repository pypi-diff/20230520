# Comparing `tmp/PyDistances-0.0.2.tar.gz` & `tmp/PyDistances-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyDistances-0.0.2.tar", last modified: Sat May 20 11:21:21 2023, max compression
+gzip compressed data, was "PyDistances-0.0.3.tar", last modified: Sat May 20 11:24:40 2023, max compression
```

## Comparing `PyDistances-0.0.2.tar` & `PyDistances-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 11:21:21.632759 PyDistances-0.0.2/
--rw-rw-rw-   0        0        0     1091 2023-05-13 15:25:04.000000 PyDistances-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     1033 2023-05-20 11:21:21.631763 PyDistances-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-20 11:21:21.616803 PyDistances-0.0.2/PyDistances/
--rw-rw-rw-   0        0        0       40 2023-05-20 10:58:09.000000 PyDistances-0.0.2/PyDistances/__init__.py
--rw-rw-rw-   0        0        0     1110 2023-05-20 11:21:03.000000 PyDistances-0.0.2/PyDistances/distances.py
-drwxrwxrwx   0        0        0        0 2023-05-20 11:21:21.629767 PyDistances-0.0.2/PyDistances.egg-info/
--rw-rw-rw-   0        0        0     1033 2023-05-20 11:21:21.000000 PyDistances-0.0.2/PyDistances.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      215 2023-05-20 11:21:21.000000 PyDistances-0.0.2/PyDistances.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 11:21:21.000000 PyDistances-0.0.2/PyDistances.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-05-20 11:21:21.000000 PyDistances-0.0.2/PyDistances.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      304 2023-05-20 11:02:56.000000 PyDistances-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-20 11:21:21.632759 PyDistances-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1002 2023-05-20 11:19:14.000000 PyDistances-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 11:24:40.204213 PyDistances-0.0.3/
+-rw-rw-rw-   0        0        0     1091 2023-05-13 15:25:04.000000 PyDistances-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1033 2023-05-20 11:24:40.203218 PyDistances-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-20 11:24:40.190597 PyDistances-0.0.3/PyDistances/
+-rw-rw-rw-   0        0        0       40 2023-05-20 10:58:09.000000 PyDistances-0.0.3/PyDistances/__init__.py
+-rw-rw-rw-   0        0        0     1110 2023-05-20 11:21:03.000000 PyDistances-0.0.3/PyDistances/distances.py
+drwxrwxrwx   0        0        0        0 2023-05-20 11:24:40.202215 PyDistances-0.0.3/PyDistances.egg-info/
+-rw-rw-rw-   0        0        0     1033 2023-05-20 11:24:40.000000 PyDistances-0.0.3/PyDistances.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      215 2023-05-20 11:24:40.000000 PyDistances-0.0.3/PyDistances.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 11:24:40.000000 PyDistances-0.0.3/PyDistances.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-20 11:24:40.000000 PyDistances-0.0.3/PyDistances.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      304 2023-05-20 11:02:56.000000 PyDistances-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-20 11:24:40.204213 PyDistances-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1002 2023-05-20 11:24:26.000000 PyDistances-0.0.3/setup.py
```

### Comparing `PyDistances-0.0.2/LICENSE` & `PyDistances-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PyDistances-0.0.2/PKG-INFO` & `PyDistances-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyDistances
-Version: 0.0.2
+Version: 0.0.3
 Summary: This is a package for computing distances among observations of statistical variables, such as: Euclidean, Minkowski, Canberra, Pearson, Mahalanobis, Robust Mahalanobis, Gower, Generalized Gower and Related Metric Scaling (RelMS). A total of 41 statistical distances can be computed.
 Home-page: https://github.com/FabioScielzoOrtiz/Distances_Package
 Author: Fabio Scielzo Ortiz
 Author-email: fabioscielzo98@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PyDistances-0.0.2/PyDistances/distances.py` & `PyDistances-0.0.3/PyDistances/distances.py`

 * *Files identical despite different names*

### Comparing `PyDistances-0.0.2/PyDistances.egg-info/PKG-INFO` & `PyDistances-0.0.3/PyDistances.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyDistances
-Version: 0.0.2
+Version: 0.0.3
 Summary: This is a package for computing distances among observations of statistical variables, such as: Euclidean, Minkowski, Canberra, Pearson, Mahalanobis, Robust Mahalanobis, Gower, Generalized Gower and Related Metric Scaling (RelMS). A total of 41 statistical distances can be computed.
 Home-page: https://github.com/FabioScielzoOrtiz/Distances_Package
 Author: Fabio Scielzo Ortiz
 Author-email: fabioscielzo98@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PyDistances-0.0.2/setup.py` & `PyDistances-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="PyDistances",
-    version="0.0.2",
+    version="0.0.3",
     author="Fabio Scielzo Ortiz",
     author_email="fabioscielzo98@gmail.com",
     description="This is a package for computing distances among observations of statistical variables, such as: Euclidean, Minkowski, Canberra, Pearson, Mahalanobis, Robust Mahalanobis, Gower, Generalized Gower and Related Metric Scaling (RelMS). A total of 41 statistical distances can be computed.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/FabioScielzoOrtiz/Distances_Package",  # add your project URL here
     packages=find_packages(),
```

