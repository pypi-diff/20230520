# Comparing `tmp/pyrovskite-0.0.1.tar.gz` & `tmp/pyrovskite-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrovskite-0.0.1.tar", last modified: Thu May 18 20:37:02 2023, max compression
+gzip compressed data, was "pyrovskite-0.9.0.tar", last modified: Sat May 20 21:41:01 2023, max compression
```

## Comparing `pyrovskite-0.0.1.tar` & `pyrovskite-0.9.0.tar`

### file list

```diff
@@ -1,14 +1,19 @@
-drwxr-xr-x   0 alg       (1000) alg       (1000)        0 2023-05-18 20:37:02.739401 pyrovskite-0.0.1/
--rw-r--r--   0 alg       (1000) alg       (1000)    35149 2023-05-18 20:20:11.000000 pyrovskite-0.0.1/LICENSE
--rw-r--r--   0 alg       (1000) alg       (1000)      806 2023-05-18 20:37:02.739401 pyrovskite-0.0.1/PKG-INFO
--rw-r--r--   0 alg       (1000) alg       (1000)       43 2023-05-18 20:30:45.000000 pyrovskite-0.0.1/README.md
-drwxr-xr-x   0 alg       (1000) alg       (1000)        0 2023-05-18 20:37:02.739401 pyrovskite-0.0.1/pyrovskite/
--rw-r--r--   0 alg       (1000) alg       (1000)        0 2023-05-18 20:29:56.000000 pyrovskite-0.0.1/pyrovskite/__init__.py
-drwxr-xr-x   0 alg       (1000) alg       (1000)        0 2023-05-18 20:37:02.739401 pyrovskite-0.0.1/pyrovskite.egg-info/
--rw-r--r--   0 alg       (1000) alg       (1000)      806 2023-05-18 20:37:02.000000 pyrovskite-0.0.1/pyrovskite.egg-info/PKG-INFO
--rw-r--r--   0 alg       (1000) alg       (1000)      218 2023-05-18 20:37:02.000000 pyrovskite-0.0.1/pyrovskite.egg-info/SOURCES.txt
--rw-r--r--   0 alg       (1000) alg       (1000)        1 2023-05-18 20:37:02.000000 pyrovskite-0.0.1/pyrovskite.egg-info/dependency_links.txt
--rw-r--r--   0 alg       (1000) alg       (1000)       13 2023-05-18 20:37:02.000000 pyrovskite-0.0.1/pyrovskite.egg-info/requires.txt
--rw-r--r--   0 alg       (1000) alg       (1000)       11 2023-05-18 20:37:02.000000 pyrovskite-0.0.1/pyrovskite.egg-info/top_level.txt
--rw-r--r--   0 alg       (1000) alg       (1000)       38 2023-05-18 20:37:02.739401 pyrovskite-0.0.1/setup.cfg
--rw-r--r--   0 alg       (1000) alg       (1000)     1297 2023-05-18 20:36:49.000000 pyrovskite-0.0.1/setup.py
+drwxr-xr-x   0 alg       (1000) alg       (1000)        0 2023-05-20 21:41:01.210535 pyrovskite-0.9.0/
+-rw-r--r--   0 alg       (1000) alg       (1000)    35149 2023-05-18 20:20:11.000000 pyrovskite-0.9.0/LICENSE
+-rw-r--r--   0 alg       (1000) alg       (1000)      802 2023-05-20 21:41:01.210535 pyrovskite-0.9.0/PKG-INFO
+-rw-r--r--   0 alg       (1000) alg       (1000)      722 2023-05-20 20:35:59.000000 pyrovskite-0.9.0/README.md
+drwxr-xr-x   0 alg       (1000) alg       (1000)        0 2023-05-20 21:41:01.210535 pyrovskite-0.9.0/pyrovskite/
+-rw-r--r--   0 alg       (1000) alg       (1000)        0 2023-05-18 20:29:56.000000 pyrovskite-0.9.0/pyrovskite/__init__.py
+-rw-r--r--   0 alg       (1000) alg       (1000)     2621 2023-05-19 21:20:53.000000 pyrovskite-0.9.0/pyrovskite/auxiliary.py
+-rw-r--r--   0 alg       (1000) alg       (1000)    40767 2023-05-20 21:02:44.000000 pyrovskite-0.9.0/pyrovskite/builder.py
+-rw-r--r--   0 alg       (1000) alg       (1000)     6094 2023-05-20 00:03:59.000000 pyrovskite-0.9.0/pyrovskite/geometry.py
+-rw-r--r--   0 alg       (1000) alg       (1000)     9292 2023-05-19 22:31:22.000000 pyrovskite-0.9.0/pyrovskite/io.py
+-rw-r--r--   0 alg       (1000) alg       (1000)    32025 2023-05-20 00:03:44.000000 pyrovskite-0.9.0/pyrovskite/perovskite.py
+drwxr-xr-x   0 alg       (1000) alg       (1000)        0 2023-05-20 21:41:01.210535 pyrovskite-0.9.0/pyrovskite.egg-info/
+-rw-r--r--   0 alg       (1000) alg       (1000)      802 2023-05-20 21:41:01.000000 pyrovskite-0.9.0/pyrovskite.egg-info/PKG-INFO
+-rw-r--r--   0 alg       (1000) alg       (1000)      329 2023-05-20 21:41:01.000000 pyrovskite-0.9.0/pyrovskite.egg-info/SOURCES.txt
+-rw-r--r--   0 alg       (1000) alg       (1000)        1 2023-05-20 21:41:01.000000 pyrovskite-0.9.0/pyrovskite.egg-info/dependency_links.txt
+-rw-r--r--   0 alg       (1000) alg       (1000)       13 2023-05-20 21:41:01.000000 pyrovskite-0.9.0/pyrovskite.egg-info/requires.txt
+-rw-r--r--   0 alg       (1000) alg       (1000)       11 2023-05-20 21:41:01.000000 pyrovskite-0.9.0/pyrovskite.egg-info/top_level.txt
+-rw-r--r--   0 alg       (1000) alg       (1000)       38 2023-05-20 21:41:01.210535 pyrovskite-0.9.0/setup.cfg
+-rw-r--r--   0 alg       (1000) alg       (1000)     1104 2023-05-20 21:40:33.000000 pyrovskite-0.9.0/setup.py
```

### Comparing `pyrovskite-0.0.1/LICENSE` & `pyrovskite-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrovskite-0.0.1/PKG-INFO` & `pyrovskite-0.9.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: pyrovskite
-Version: 0.0.1
+Version: 0.9.0
 Summary: Python package for 2D- and 3D-perovskites
 Author: Robert Stanton, Dhara J. Trivedi
 Author-email: <stantor@clarkson.edu>
 Keywords: python,perovskite,hybrid,electronic structure,DFT,xTB
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
```

### Comparing `pyrovskite-0.0.1/pyrovskite.egg-info/PKG-INFO` & `pyrovskite-0.9.0/pyrovskite.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: pyrovskite
-Version: 0.0.1
+Version: 0.9.0
 Summary: Python package for 2D- and 3D-perovskites
 Author: Robert Stanton, Dhara J. Trivedi
 Author-email: <stantor@clarkson.edu>
 Keywords: python,perovskite,hybrid,electronic structure,DFT,xTB
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
```

### Comparing `pyrovskite-0.0.1/setup.py` & `pyrovskite-0.9.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,11 @@
 from setuptools import setup, find_packages
-# import codecs
 import os
 
-# here = os.path.abspath(os.path.dirname(__file__))
-
-# with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
-    # long_description = "\n" + fh.read()
-
-VERSION = '0.0.1'
+VERSION = '0.9.0'
 DESCRIPTION = 'Python package for 2D- and 3D-perovskites'
 LONG_DESCRIPTION = 'A software package for the high throughput construction, analysis, and featurization of two- and three-dimensional perovskite systems.'
 
 # Setting up
 setup(
     name="pyrovskite",
     version=VERSION,
@@ -21,15 +15,15 @@
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=['pymatgen', 'ase'],
     keywords=['python', 'perovskite', 'hybrid',
         'electronic structure', 'DFT', 'xTB'],
     classifiers=[
-        "Development Status :: 1 - Planning",
+        "Development Status :: 4 - Beta",
         "Programming Language :: Python :: 3",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ]
```

