# Comparing `tmp/pysparse-array-1.0.0.tar.gz` & `tmp/pysparse-array-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysparse-array-1.0.0.tar", last modified: Sat May 20 08:09:43 2023, max compression
+gzip compressed data, was "pysparse-array-1.0.1.tar", last modified: Sat May 20 10:17:23 2023, max compression
```

## Comparing `pysparse-array-1.0.0.tar` & `pysparse-array-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-20 08:09:43.345474 pysparse-array-1.0.0/
--rw-r--r--   0 thomasfrost   (502) staff       (20)     2327 2023-05-20 08:08:18.000000 pysparse-array-1.0.0/HISTORY.md
--rw-r--r--   0 thomasfrost   (502) staff       (20)     1060 2023-05-15 14:53:09.000000 pysparse-array-1.0.0/LICENSE.txt
--rw-r--r--   0 thomasfrost   (502) staff       (20)       19 2023-05-16 11:11:47.000000 pysparse-array-1.0.0/MANIFEST.in
--rw-r--r--   0 thomasfrost   (502) staff       (20)     5374 2023-05-20 08:09:43.343218 pysparse-array-1.0.0/PKG-INFO
--rw-r--r--   0 thomasfrost   (502) staff       (20)     4669 2023-05-20 08:08:43.000000 pysparse-array-1.0.0/README.md
--rw-r--r--   0 thomasfrost   (502) staff       (20)      773 2023-05-20 08:08:31.000000 pysparse-array-1.0.0/pyproject.toml
-drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-20 08:09:43.233800 pysparse-array-1.0.0/pysparse_array.egg-info/
--rw-r--r--   0 thomasfrost   (502) staff       (20)     5374 2023-05-20 08:09:43.000000 pysparse-array-1.0.0/pysparse_array.egg-info/PKG-INFO
--rw-r--r--   0 thomasfrost   (502) staff       (20)      311 2023-05-20 08:09:43.000000 pysparse-array-1.0.0/pysparse_array.egg-info/SOURCES.txt
--rw-r--r--   0 thomasfrost   (502) staff       (20)        1 2023-05-20 08:09:43.000000 pysparse-array-1.0.0/pysparse_array.egg-info/dependency_links.txt
--rw-r--r--   0 thomasfrost   (502) staff       (20)       41 2023-05-20 08:09:43.000000 pysparse-array-1.0.0/pysparse_array.egg-info/requires.txt
--rw-r--r--   0 thomasfrost   (502) staff       (20)        7 2023-05-20 08:09:43.000000 pysparse-array-1.0.0/pysparse_array.egg-info/top_level.txt
--rw-r--r--   0 thomasfrost   (502) staff       (20)       38 2023-05-20 08:09:43.345846 pysparse-array-1.0.0/setup.cfg
--rw-r--r--   0 thomasfrost   (502) staff       (20)      708 2023-05-20 08:08:56.000000 pysparse-array-1.0.0/setup.py
-drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-20 08:09:43.337401 pysparse-array-1.0.0/sparse/
--rw-r--r--   0 thomasfrost   (502) staff       (20)      113 2023-05-16 11:47:08.000000 pysparse-array-1.0.0/sparse/__init__.py
--rw-r--r--   0 thomasfrost   (502) staff       (20)     9878 2023-05-20 06:51:45.000000 pysparse-array-1.0.0/sparse/array_api.py
--rw-r--r--   0 thomasfrost   (502) staff       (20)     7627 2023-05-20 06:59:53.000000 pysparse-array-1.0.0/sparse/core.py
+drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-20 10:17:23.048390 pysparse-array-1.0.1/
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     2402 2023-05-20 10:16:18.000000 pysparse-array-1.0.1/HISTORY.md
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     1060 2023-05-15 14:53:09.000000 pysparse-array-1.0.1/LICENSE.txt
+-rw-r--r--   0 thomasfrost   (502) staff       (20)       19 2023-05-16 11:11:47.000000 pysparse-array-1.0.1/MANIFEST.in
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     5374 2023-05-20 10:17:23.047244 pysparse-array-1.0.1/PKG-INFO
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     4669 2023-05-20 08:08:43.000000 pysparse-array-1.0.1/README.md
+-rw-r--r--   0 thomasfrost   (502) staff       (20)      763 2023-05-20 10:15:49.000000 pysparse-array-1.0.1/pyproject.toml
+drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-20 10:17:23.020548 pysparse-array-1.0.1/pysparse_array.egg-info/
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     5374 2023-05-20 10:17:22.000000 pysparse-array-1.0.1/pysparse_array.egg-info/PKG-INFO
+-rw-r--r--   0 thomasfrost   (502) staff       (20)      311 2023-05-20 10:17:22.000000 pysparse-array-1.0.1/pysparse_array.egg-info/SOURCES.txt
+-rw-r--r--   0 thomasfrost   (502) staff       (20)        1 2023-05-20 10:17:22.000000 pysparse-array-1.0.1/pysparse_array.egg-info/dependency_links.txt
+-rw-r--r--   0 thomasfrost   (502) staff       (20)       34 2023-05-20 10:17:22.000000 pysparse-array-1.0.1/pysparse_array.egg-info/requires.txt
+-rw-r--r--   0 thomasfrost   (502) staff       (20)        7 2023-05-20 10:17:22.000000 pysparse-array-1.0.1/pysparse_array.egg-info/top_level.txt
+-rw-r--r--   0 thomasfrost   (502) staff       (20)       38 2023-05-20 10:17:23.048476 pysparse-array-1.0.1/setup.cfg
+-rw-r--r--   0 thomasfrost   (502) staff       (20)      708 2023-05-20 10:16:43.000000 pysparse-array-1.0.1/setup.py
+drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-20 10:17:23.044133 pysparse-array-1.0.1/sparse/
+-rw-r--r--   0 thomasfrost   (502) staff       (20)      113 2023-05-16 11:47:08.000000 pysparse-array-1.0.1/sparse/__init__.py
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     9878 2023-05-20 06:51:45.000000 pysparse-array-1.0.1/sparse/array_api.py
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     7627 2023-05-20 06:59:53.000000 pysparse-array-1.0.1/sparse/core.py
```

### Comparing `pysparse-array-1.0.0/HISTORY.md` & `pysparse-array-1.0.1/HISTORY.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 #Changelog
 
 All notable changes to the `PySparse` package will be documented in this file.
 
 ## [Unreleased]
 
+## [1.0.1] - 2023-05-20
+
+### Fixed
+- Small dependencies bug, now resolved
+
 ## [1.0.0] - 2023-05-20
 
 ### Added
 - Additional "coords_dictionary" file included, which replaces the previous find_indices function and introduces significant loading speed-up of 2-3x. This version is not backwards compatible with arrays encoded using v0.*
 
 ### Fixed
 - N/A
```

### Comparing `pysparse-array-1.0.0/LICENSE.txt` & `pysparse-array-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pysparse-array-1.0.0/PKG-INFO` & `pysparse-array-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysparse-array
-Version: 1.0.0
+Version: 1.0.1
 Summary: A package that enables on-the-fly encoding and decoding of large NumPy arrays as Sparse binaries.
 Home-page: https://github.com/tdgfrost/PySparse
 Download-URL: https://pypi.org/project/pysparse-array/
 Author: Thomas Frost
 Author-email: Thomas Frost <tdgfrost@gmail.com>
 Project-URL: Homepage, https://github.com/tdgfrost/PySparse
 Project-URL: Bug Tracker, https://github.com/tdgfrost/PySparse/issues
```

### Comparing `pysparse-array-1.0.0/README.md` & `pysparse-array-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pysparse-array-1.0.0/pyproject.toml` & `pysparse-array-1.0.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "pysparse-array"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
 	{ name="Thomas Frost", email="tdgfrost@gmail.com" },
 ]
 description = "A package that enables on-the-fly encoding and decoding of large NumPy arrays as Sparse binaries."
 readme = "README.md"
 requires-python = ">=3.8.0"
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"License :: OSI Approved :: MIT License",
 	"Operating System :: OS Independent",
 ]
-dependencies = ['numpy>=1.18.0', 'numba>=0.49.0, <0.57', 'pickle']
+dependencies = ['numpy>=1.18.0', 'numba>=0.49.0, <0.57']
 
 [dynamic]
 keywords = ["PySparse", "SparseArray"]
 license = "MIT"
 
 [project.urls]
 "Homepage" = "https://github.com/tdgfrost/PySparse"
```

### Comparing `pysparse-array-1.0.0/pysparse_array.egg-info/PKG-INFO` & `pysparse-array-1.0.1/pysparse_array.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysparse-array
-Version: 1.0.0
+Version: 1.0.1
 Summary: A package that enables on-the-fly encoding and decoding of large NumPy arrays as Sparse binaries.
 Home-page: https://github.com/tdgfrost/PySparse
 Download-URL: https://pypi.org/project/pysparse-array/
 Author: Thomas Frost
 Author-email: Thomas Frost <tdgfrost@gmail.com>
 Project-URL: Homepage, https://github.com/tdgfrost/PySparse
 Project-URL: Bug Tracker, https://github.com/tdgfrost/PySparse/issues
```

### Comparing `pysparse-array-1.0.0/setup.py` & `pysparse-array-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme_file.read()
 
 with open('HISTORY.md') as history_file:
     HISTORY = history_file.read()
 
 setup_args = dict(
     name='pysparse-array',
-    version='1.0.0',
+    version='1.0.1',
     description='Package to encode and decode large OOM numpy arrays as Sparse binaries',
     long_description_content_type="text/markdown",
     long_description=README + '\n\n' + HISTORY,
     packages=find_packages(),
     author='Thomas Frost',
     author_email='tdgfrost@gmail.com',
     url='https://github.com/tdgfrost/PySparse',
```

### Comparing `pysparse-array-1.0.0/sparse/array_api.py` & `pysparse-array-1.0.1/sparse/array_api.py`

 * *Files identical despite different names*

### Comparing `pysparse-array-1.0.0/sparse/core.py` & `pysparse-array-1.0.1/sparse/core.py`

 * *Files identical despite different names*

