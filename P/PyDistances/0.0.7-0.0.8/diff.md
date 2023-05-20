# Comparing `tmp/PyDistances-0.0.7.tar.gz` & `tmp/PyDistances-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyDistances-0.0.7.tar", last modified: Sat May 20 12:08:02 2023, max compression
+gzip compressed data, was "PyDistances-0.0.8.tar", last modified: Sat May 20 14:12:11 2023, max compression
```

## Comparing `PyDistances-0.0.7.tar` & `PyDistances-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 12:08:02.096574 PyDistances-0.0.7/
--rw-rw-rw-   0        0        0     1091 2023-05-13 15:25:04.000000 PyDistances-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     1069 2023-05-20 12:08:02.095577 PyDistances-0.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-20 12:08:02.080616 PyDistances-0.0.7/PyDistances/
--rw-rw-rw-   0        0        0       40 2023-05-20 10:58:09.000000 PyDistances-0.0.7/PyDistances/__init__.py
--rw-rw-rw-   0        0        0     1132 2023-05-20 12:06:12.000000 PyDistances-0.0.7/PyDistances/distances.py
-drwxrwxrwx   0        0        0        0 2023-05-20 12:08:02.093582 PyDistances-0.0.7/PyDistances.egg-info/
--rw-rw-rw-   0        0        0     1069 2023-05-20 12:08:01.000000 PyDistances-0.0.7/PyDistances.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-05-20 12:08:01.000000 PyDistances-0.0.7/PyDistances.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 12:08:01.000000 PyDistances-0.0.7/PyDistances.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-20 12:08:01.000000 PyDistances-0.0.7/PyDistances.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-20 12:08:01.000000 PyDistances-0.0.7/PyDistances.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      340 2023-05-20 11:51:44.000000 PyDistances-0.0.7/README.md
--rw-rw-rw-   0        0        0       42 2023-05-20 12:08:02.097571 PyDistances-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1045 2023-05-20 12:07:56.000000 PyDistances-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 14:12:11.896569 PyDistances-0.0.8/
+-rw-rw-rw-   0        0        0     1091 2023-05-13 15:25:04.000000 PyDistances-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     1069 2023-05-20 14:12:11.895574 PyDistances-0.0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-20 14:12:11.884371 PyDistances-0.0.8/PyDistances/
+-rw-rw-rw-   0        0        0      536 2023-05-20 14:08:13.000000 PyDistances-0.0.8/PyDistances/__init__.py
+-rw-rw-rw-   0        0        0    52586 2023-05-20 14:04:02.000000 PyDistances-0.0.8/PyDistances/distances.py
+drwxrwxrwx   0        0        0        0 2023-05-20 14:12:11.893577 PyDistances-0.0.8/PyDistances.egg-info/
+-rw-rw-rw-   0        0        0     1069 2023-05-20 14:12:11.000000 PyDistances-0.0.8/PyDistances.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-05-20 14:12:11.000000 PyDistances-0.0.8/PyDistances.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 14:12:11.000000 PyDistances-0.0.8/PyDistances.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-20 14:12:11.000000 PyDistances-0.0.8/PyDistances.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-20 14:12:11.000000 PyDistances-0.0.8/PyDistances.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      340 2023-05-20 11:51:44.000000 PyDistances-0.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-20 14:12:11.897567 PyDistances-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1045 2023-05-20 14:12:07.000000 PyDistances-0.0.8/setup.py
```

### Comparing `PyDistances-0.0.7/LICENSE` & `PyDistances-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `PyDistances-0.0.7/PKG-INFO` & `PyDistances-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyDistances
-Version: 0.0.7
+Version: 0.0.8
 Summary: This is a package for computing distances among observations of statistical variables, such as: Euclidean, Minkowski, Canberra, Pearson, Mahalanobis, Robust Mahalanobis, Gower, Generalized Gower and Related Metric Scaling (RelMS). A total of 41 statistical distances can be computed.
 Home-page: https://github.com/FabioScielzoOrtiz/Distances_Package
 Author: Fabio Scielzo Ortiz
 Author-email: fabioscielzo98@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PyDistances-0.0.7/PyDistances.egg-info/PKG-INFO` & `PyDistances-0.0.8/PyDistances.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyDistances
-Version: 0.0.7
+Version: 0.0.8
 Summary: This is a package for computing distances among observations of statistical variables, such as: Euclidean, Minkowski, Canberra, Pearson, Mahalanobis, Robust Mahalanobis, Gower, Generalized Gower and Related Metric Scaling (RelMS). A total of 41 statistical distances can be computed.
 Home-page: https://github.com/FabioScielzoOrtiz/Distances_Package
 Author: Fabio Scielzo Ortiz
 Author-email: fabioscielzo98@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PyDistances-0.0.7/setup.py` & `PyDistances-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="PyDistances",
-    version="0.0.7",
+    version="0.0.8",
     author="Fabio Scielzo Ortiz",
     author_email="fabioscielzo98@gmail.com",
     description="This is a package for computing distances among observations of statistical variables, such as: Euclidean, Minkowski, Canberra, Pearson, Mahalanobis, Robust Mahalanobis, Gower, Generalized Gower and Related Metric Scaling (RelMS). A total of 41 statistical distances can be computed.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/FabioScielzoOrtiz/Distances_Package",  # add your project URL here
     packages=find_packages(),
```

