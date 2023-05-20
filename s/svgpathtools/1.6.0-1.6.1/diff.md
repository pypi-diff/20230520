# Comparing `tmp/svgpathtools-1.6.0.tar.gz` & `tmp/svgpathtools-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svgpathtools-1.6.0.tar", last modified: Mon Feb 13 22:49:44 2023, max compression
+gzip compressed data, was "svgpathtools-1.6.1.tar", last modified: Sat May 20 18:35:44 2023, max compression
```

## Comparing `svgpathtools-1.6.0.tar` & `svgpathtools-1.6.1.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-13 22:49:43.994840 svgpathtools-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (116)     1083 2023-02-13 22:49:35.000000 svgpathtools-1.6.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1086 2023-02-13 22:49:35.000000 svgpathtools-1.6.0/LICENSE2.txt
--rw-r--r--   0 runner    (1001) docker     (116)       51 2023-02-13 22:49:35.000000 svgpathtools-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)    22719 2023-02-13 22:49:43.994840 svgpathtools-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)    21098 2023-02-13 22:49:35.000000 svgpathtools-1.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (116)     1059 2023-02-13 22:49:35.000000 svgpathtools-1.6.0/decorated_ellipse.svg
--rw-r--r--   0 runner    (1001) docker     (116)     1066 2023-02-13 22:49:35.000000 svgpathtools-1.6.0/donate-button.svg
--rw-r--r--   0 runner    (1001) docker     (116)  4504401 2023-02-13 22:49:35.000000 svgpathtools-1.6.0/offset_curves.svg
--rw-r--r--   0 runner    (1001) docker     (116)      774 2023-02-13 22:49:35.000000 svgpathtools-1.6.0/output1.svg
--rw-r--r--   0 runner    (1001) docker     (116)     1528 2023-02-13 22:49:35.000000 svgpathtools-1.6.0/output2.svg
--rw-r--r--   0 runner    (1001) docker     (116)     1044 2023-02-13 22:49:35.000000 svgpathtools-1.6.0/output_intersections.svg
--rw-r--r--   0 runner    (1001) docker     (116)      424 2023-02-13 22:49:35.000000 svgpathtools-1.6.0/path.svg
--rw-r--r--   0 runner    (1001) docker     (116)      106 2023-02-13 22:49:43.994840 svgpathtools-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     2344 2023-02-13 22:49:35.000000 svgpathtools-1.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-13 22:49:43.994840 svgpathtools-1.6.0/svgpathtools/
--rw-r--r--   0 runner    (1001) docker     (116)     1097 2023-02-13 22:49:35.000000 svgpathtools-1.6.0/svgpathtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    14309 2023-02-13 22:49:35.000000 svgpathtools-1.6.0/svgpathtools/bezier.py
--rw-r--r--   0 runner    (1001) docker     (116)    18553 2023-02-13 22:49:35.000000 svgpathtools-1.6.0/svgpathtools/document.py
--rw-r--r--   0 runner    (1001) docker     (116)     2026 2023-02-13 22:49:35.000000 svgpathtools-1.6.0/svgpathtools/misctools.py
--rw-r--r--   0 runner    (1001) docker     (116)     3939 2023-02-13 22:49:35.000000 svgpathtools-1.6.0/svgpathtools/parser.py
--rw-r--r--   0 runner    (1001) docker     (116)   135101 2023-02-13 22:49:35.000000 svgpathtools-1.6.0/svgpathtools/path.py
--rw-r--r--   0 runner    (1001) docker     (116)    18991 2023-02-13 22:49:35.000000 svgpathtools-1.6.0/svgpathtools/paths2svg.py
--rw-r--r--   0 runner    (1001) docker     (116)     2473 2023-02-13 22:49:35.000000 svgpathtools-1.6.0/svgpathtools/polytools.py
--rw-r--r--   0 runner    (1001) docker     (116)     7642 2023-02-13 22:49:35.000000 svgpathtools-1.6.0/svgpathtools/smoothing.py
--rw-r--r--   0 runner    (1001) docker     (116)     7145 2023-02-13 22:49:35.000000 svgpathtools-1.6.0/svgpathtools/svg_io_sax.py
--rw-r--r--   0 runner    (1001) docker     (116)    11331 2023-02-13 22:49:35.000000 svgpathtools-1.6.0/svgpathtools/svg_to_paths.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-13 22:49:43.994840 svgpathtools-1.6.0/svgpathtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)    22719 2023-02-13 22:49:43.000000 svgpathtools-1.6.0/svgpathtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      996 2023-02-13 22:49:43.000000 svgpathtools-1.6.0/svgpathtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-02-13 22:49:43.000000 svgpathtools-1.6.0/svgpathtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       21 2023-02-13 22:49:43.000000 svgpathtools-1.6.0/svgpathtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       13 2023-02-13 22:49:43.000000 svgpathtools-1.6.0/svgpathtools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-13 22:49:43.994840 svgpathtools-1.6.0/test/
--rw-r--r--   0 runner    (1001) docker     (116)      294 2023-02-13 22:49:35.000000 svgpathtools-1.6.0/test/circle.svg
--rw-r--r--   0 runner    (1001) docker     (116)     1074 2023-02-13 22:49:35.000000 svgpathtools-1.6.0/test/display_temp.svg
--rw-r--r--   0 runner    (1001) docker     (116)      304 2023-02-13 22:49:35.000000 svgpathtools-1.6.0/test/ellipse.svg
--rw-r--r--   0 runner    (1001) docker     (116)     3057 2023-02-13 22:49:35.000000 svgpathtools-1.6.0/test/groups.svg
--rw-r--r--   0 runner    (1001) docker     (116)      431 2023-02-13 22:49:35.000000 svgpathtools-1.6.0/test/polygons.svg
--rw-r--r--   0 runner    (1001) docker     (116)      207 2023-02-13 22:49:35.000000 svgpathtools-1.6.0/test/rects.svg
--rw-r--r--   0 runner    (1001) docker     (116)     2674 2023-02-13 22:49:35.000000 svgpathtools-1.6.0/test/test.svg
--rw-r--r--   0 runner    (1001) docker     (116)     1795 2023-02-13 22:49:35.000000 svgpathtools-1.6.0/test/test_bezier.py
--rw-r--r--   0 runner    (1001) docker     (116)     1963 2023-02-13 22:49:35.000000 svgpathtools-1.6.0/test/test_document.py
--rw-r--r--   0 runner    (1001) docker     (116)     3924 2023-02-13 22:49:35.000000 svgpathtools-1.6.0/test/test_generation.py
--rw-r--r--   0 runner    (1001) docker     (116)    10205 2023-02-13 22:49:35.000000 svgpathtools-1.6.0/test/test_groups.py
--rw-r--r--   0 runner    (1001) docker     (116)    13221 2023-02-13 22:49:35.000000 svgpathtools-1.6.0/test/test_parsing.py
--rw-r--r--   0 runner    (1001) docker     (116)   100001 2023-02-13 22:49:35.000000 svgpathtools-1.6.0/test/test_path.py
--rw-r--r--   0 runner    (1001) docker     (116)      759 2023-02-13 22:49:35.000000 svgpathtools-1.6.0/test/test_polytools.py
--rw-r--r--   0 runner    (1001) docker     (116)     1033 2023-02-13 22:49:35.000000 svgpathtools-1.6.0/test/test_sax_groups.py
--rw-r--r--   0 runner    (1001) docker     (116)     4478 2023-02-13 22:49:35.000000 svgpathtools-1.6.0/test/test_svg2paths.py
--rw-r--r--   0 runner    (1001) docker     (116)     1583 2023-02-13 22:49:35.000000 svgpathtools-1.6.0/test/transforms.svg
--rw-r--r--   0 runner    (1001) docker     (116)      815 2023-02-13 22:49:35.000000 svgpathtools-1.6.0/test.svg
--rw-r--r--   0 runner    (1001) docker     (116)     1467 2023-02-13 22:49:35.000000 svgpathtools-1.6.0/vectorframes.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:35:44.937130 svgpathtools-1.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-20 18:35:36.000000 svgpathtools-1.6.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-20 18:35:36.000000 svgpathtools-1.6.1/LICENSE2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-20 18:35:36.000000 svgpathtools-1.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    22663 2023-05-20 18:35:44.937130 svgpathtools-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20991 2023-05-20 18:35:36.000000 svgpathtools-1.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-20 18:35:36.000000 svgpathtools-1.6.1/decorated_ellipse.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-20 18:35:36.000000 svgpathtools-1.6.1/donate-button.svg
+-rw-r--r--   0 runner    (1001) docker     (123)  4504401 2023-05-20 18:35:36.000000 svgpathtools-1.6.1/offset_curves.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-20 18:35:36.000000 svgpathtools-1.6.1/output1.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-20 18:35:36.000000 svgpathtools-1.6.1/output2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-20 18:35:36.000000 svgpathtools-1.6.1/output_intersections.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-20 18:35:36.000000 svgpathtools-1.6.1/path.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-20 18:35:44.937130 svgpathtools-1.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-05-20 18:35:36.000000 svgpathtools-1.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:35:44.933130 svgpathtools-1.6.1/svgpathtools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-20 18:35:36.000000 svgpathtools-1.6.1/svgpathtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14309 2023-05-20 18:35:36.000000 svgpathtools-1.6.1/svgpathtools/bezier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18553 2023-05-20 18:35:36.000000 svgpathtools-1.6.1/svgpathtools/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-20 18:35:36.000000 svgpathtools-1.6.1/svgpathtools/misctools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-05-20 18:35:36.000000 svgpathtools-1.6.1/svgpathtools/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)   135405 2023-05-20 18:35:36.000000 svgpathtools-1.6.1/svgpathtools/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18991 2023-05-20 18:35:36.000000 svgpathtools-1.6.1/svgpathtools/paths2svg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-05-20 18:35:36.000000 svgpathtools-1.6.1/svgpathtools/polytools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-05-20 18:35:36.000000 svgpathtools-1.6.1/svgpathtools/smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-05-20 18:35:36.000000 svgpathtools-1.6.1/svgpathtools/svg_io_sax.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11337 2023-05-20 18:35:36.000000 svgpathtools-1.6.1/svgpathtools/svg_to_paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:35:44.933130 svgpathtools-1.6.1/svgpathtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22663 2023-05-20 18:35:44.000000 svgpathtools-1.6.1/svgpathtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-20 18:35:44.000000 svgpathtools-1.6.1/svgpathtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 18:35:44.000000 svgpathtools-1.6.1/svgpathtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-20 18:35:44.000000 svgpathtools-1.6.1/svgpathtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-20 18:35:44.000000 svgpathtools-1.6.1/svgpathtools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:35:44.937130 svgpathtools-1.6.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-20 18:35:36.000000 svgpathtools-1.6.1/test/circle.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-20 18:35:36.000000 svgpathtools-1.6.1/test/display_temp.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-20 18:35:36.000000 svgpathtools-1.6.1/test/ellipse.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-05-20 18:35:36.000000 svgpathtools-1.6.1/test/groups.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-20 18:35:36.000000 svgpathtools-1.6.1/test/negative-scale.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-20 18:35:36.000000 svgpathtools-1.6.1/test/polygons.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-20 18:35:36.000000 svgpathtools-1.6.1/test/rects.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-05-20 18:35:36.000000 svgpathtools-1.6.1/test/test.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-05-20 18:35:36.000000 svgpathtools-1.6.1/test/test_bezier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-20 18:35:36.000000 svgpathtools-1.6.1/test/test_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-05-20 18:35:36.000000 svgpathtools-1.6.1/test/test_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11605 2023-05-20 18:35:36.000000 svgpathtools-1.6.1/test/test_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13221 2023-05-20 18:35:36.000000 svgpathtools-1.6.1/test/test_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100001 2023-05-20 18:35:36.000000 svgpathtools-1.6.1/test/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-20 18:35:36.000000 svgpathtools-1.6.1/test/test_polytools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-20 18:35:36.000000 svgpathtools-1.6.1/test/test_sax_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-05-20 18:35:36.000000 svgpathtools-1.6.1/test/test_svg2paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-20 18:35:36.000000 svgpathtools-1.6.1/test/transforms.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-20 18:35:36.000000 svgpathtools-1.6.1/test.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-20 18:35:36.000000 svgpathtools-1.6.1/vectorframes.svg
```

### Comparing `svgpathtools-1.6.0/LICENSE.txt` & `svgpathtools-1.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `svgpathtools-1.6.0/LICENSE2.txt` & `svgpathtools-1.6.1/LICENSE2.txt`

 * *Files identical despite different names*

### Comparing `svgpathtools-1.6.0/PKG-INFO` & `svgpathtools-1.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: svgpathtools
-Version: 1.6.0
+Version: 1.6.1
 Summary: A collection of tools for manipulating and analyzing SVG Path objects and Bezier curves.
 Home-page: https://github.com/mathandy/svgpathtools
-Download-URL: https://github.com/mathandy/svgpathtools/releases/download/1.6.0/svgpathtools-1.6.0-py2.py3-none-any.whl
+Download-URL: https://github.com/mathandy/svgpathtools/releases/download/1.6.1/svgpathtools-1.6.1-py2.py3-none-any.whl
 Author: Andy Port
 Author-email: AndyAPort@gmail.com
 License: MIT
 Keywords: svg,svg path,svg.path,bezier,parse svg path,display svg
 Platform: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -18,28 +18,28 @@
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Multimedia :: Graphics :: Editors :: Vector-Based
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 [![Donate](https://img.shields.io/badge/donate-paypal-brightgreen)](https://www.paypal.com/donate?business=4SKJ27AM4EYYA&amp;no_recurring=0&amp;item_name=Support+the+creator+of+svgpathtools?++He%27s+a+student+and+would+appreciate+it.&amp;currency_code=USD)
 ![Python](https://img.shields.io/pypi/pyversions/svgpathtools.svg)
 [![PyPI](https://img.shields.io/pypi/v/svgpathtools)](https://pypi.org/project/svgpathtools/)
-![Build](https://img.shields.io/github/workflow/status/mathandy/svgpathtools/Github%20CI%20Unit%20Testing)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/svgpathtools?color=yellow)](https://pypistats.org/packages/svgpathtools)
 # svgpathtools
 
 
 svgpathtools is a collection of tools for manipulating and analyzing SVG Path objects and Bézier curves.
 
 ## Features
```

### Comparing `svgpathtools-1.6.0/README.md` & `svgpathtools-1.6.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 [![Donate](https://img.shields.io/badge/donate-paypal-brightgreen)](https://www.paypal.com/donate?business=4SKJ27AM4EYYA&amp;no_recurring=0&amp;item_name=Support+the+creator+of+svgpathtools?++He%27s+a+student+and+would+appreciate+it.&amp;currency_code=USD)
 ![Python](https://img.shields.io/pypi/pyversions/svgpathtools.svg)
 [![PyPI](https://img.shields.io/pypi/v/svgpathtools)](https://pypi.org/project/svgpathtools/)
-![Build](https://img.shields.io/github/workflow/status/mathandy/svgpathtools/Github%20CI%20Unit%20Testing)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/svgpathtools?color=yellow)](https://pypistats.org/packages/svgpathtools)
 # svgpathtools
 
 
 svgpathtools is a collection of tools for manipulating and analyzing SVG Path objects and Bézier curves.
 
 ## Features
```

### Comparing `svgpathtools-1.6.0/decorated_ellipse.svg` & `svgpathtools-1.6.1/decorated_ellipse.svg`

 * *Files identical despite different names*

### Comparing `svgpathtools-1.6.0/donate-button.svg` & `svgpathtools-1.6.1/donate-button.svg`

 * *Files identical despite different names*

### Comparing `svgpathtools-1.6.0/offset_curves.svg` & `svgpathtools-1.6.1/offset_curves.svg`

 * *Files identical despite different names*

### Comparing `svgpathtools-1.6.0/output1.svg` & `svgpathtools-1.6.1/output1.svg`

 * *Files identical despite different names*

### Comparing `svgpathtools-1.6.0/output2.svg` & `svgpathtools-1.6.1/output2.svg`

 * *Files identical despite different names*

### Comparing `svgpathtools-1.6.0/output_intersections.svg` & `svgpathtools-1.6.1/output_intersections.svg`

 * *Files identical despite different names*

### Comparing `svgpathtools-1.6.0/setup.py` & `svgpathtools-1.6.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 import codecs
 import os
 
 
-VERSION = '1.6.0'
+VERSION = '1.6.1'
 AUTHOR_NAME = 'Andy Port'
 AUTHOR_EMAIL = 'AndyAPort@gmail.com'
 GITHUB = 'https://github.com/mathandy/svgpathtools'
 
 _here = os.path.abspath(os.path.dirname(__file__))
 
 
@@ -43,14 +43,15 @@
             "Programming Language :: Python :: 2.7",
             "Programming Language :: Python :: 3.5",
             "Programming Language :: Python :: 3.6",
             "Programming Language :: Python :: 3.7",
             "Programming Language :: Python :: 3.8",
             "Programming Language :: Python :: 3.9",
             "Programming Language :: Python :: 3.10",
+            "Programming Language :: Python :: 3.11",
             "Topic :: Multimedia :: Graphics :: Editors :: Vector-Based",
             "Topic :: Scientific/Engineering",
             "Topic :: Scientific/Engineering :: Image Recognition",
             "Topic :: Scientific/Engineering :: Information Analysis",
             "Topic :: Scientific/Engineering :: Mathematics",
             "Topic :: Scientific/Engineering :: Visualization",
             "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `svgpathtools-1.6.0/svgpathtools/__init__.py` & `svgpathtools-1.6.1/svgpathtools/__init__.py`

 * *Files identical despite different names*

### Comparing `svgpathtools-1.6.0/svgpathtools/bezier.py` & `svgpathtools-1.6.1/svgpathtools/bezier.py`

 * *Files identical despite different names*

### Comparing `svgpathtools-1.6.0/svgpathtools/document.py` & `svgpathtools-1.6.1/svgpathtools/document.py`

 * *Files identical despite different names*

### Comparing `svgpathtools-1.6.0/svgpathtools/misctools.py` & `svgpathtools-1.6.1/svgpathtools/misctools.py`

 * *Files identical despite different names*

### Comparing `svgpathtools-1.6.0/svgpathtools/parser.py` & `svgpathtools-1.6.1/svgpathtools/parser.py`

 * *Files identical despite different names*

### Comparing `svgpathtools-1.6.0/svgpathtools/path.py` & `svgpathtools-1.6.1/svgpathtools/path.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,16 +39,16 @@
     str = basestring
 except NameError:
     pass
 
 COMMANDS = set('MmZzLlHhVvCcSsQqTtAa')
 UPPERCASE = set('MZLHVCSQTA')
 
-COMMAND_RE = re.compile("([MmZzLlHhVvCcSsQqTtAa])")
-FLOAT_RE = re.compile("[-+]?[0-9]*\.?[0-9]+(?:[eE][-+]?[0-9]+)?")
+COMMAND_RE = re.compile(r"([MmZzLlHhVvCcSsQqTtAa])")
+FLOAT_RE = re.compile(r"[-+]?[0-9]*\.?[0-9]+(?:[eE][-+]?[0-9]+)?")
 
 # Default Parameters ##########################################################
 
 # path segment .length() parameters for arc length computation
 LENGTH_MIN_DEPTH = 5
 LENGTH_ERROR = 1e-12
 USE_SCIPY_QUAD = True  # for elliptic Arc segment arc length computation
@@ -334,17 +334,21 @@
         new_radius = complex(rx, ry)
 
         xeigvec = eigvecs[:, 0]
         rot = np.degrees(np.arccos(xeigvec[0]))
 
         if new_radius.real == 0 or new_radius.imag == 0 :
             return Line(new_start, new_end)
-        else : 
+        else:
+            if tf[0][0] * tf[1][1] >= 0.0:
+                new_sweep = curve.sweep
+            else:
+                new_sweep = not curve.sweep
             return Arc(new_start, radius=new_radius, rotation=curve.rotation + rot,
-                       large_arc=curve.large_arc, sweep=curve.sweep, end=new_end,
+                       large_arc=curve.large_arc, sweep=new_sweep, end=new_end,
                        autoscale_radius=True)
 
     else:
         raise TypeError("Input `curve` should be a Path, Line, "
                         "QuadraticBezier, CubicBezier, or Arc object.")
 
 
@@ -1390,15 +1394,15 @@
         """Scale transform.  See `scale` function for further explanation."""
         return scale(self, sx=sx, sy=sy, origin=origin)
 
 
 class Arc(object):
     def __init__(self, start, radius, rotation, large_arc, sweep, end,
                  autoscale_radius=True):
-        """
+        r"""
         This should be thought of as a part of an ellipse connecting two
         points on that ellipse, start and end.
         Parameters
         ----------
         start : complex
             The start point of the curve. Note: `start` and `end` cannot be the
             same.  To make a full ellipse or circle, use two `Arc` objects.
@@ -2564,15 +2568,15 @@
         else:
             self._lengths = [each / self._length for each in lengths]
 
     def point(self, pos):
 
         # Shortcuts
         if len(self._segments) == 0:
-            return None
+            raise ValueError("This path contains no segments!")
         if pos == 0.0:
             return self._segments[0].point(pos)
         if pos == 1.0:
             return self._segments[-1].point(pos)
 
         self._calc_lengths()
         # Find which segment the point we search for is located on:
@@ -2581,14 +2585,15 @@
             segment_end = segment_start + self._lengths[index]
             if segment_end >= pos:
                 # This is the segment! How far in on the segment is the point?
                 segment_pos = (pos - segment_start)/(
                     segment_end - segment_start)
                 return segment.point(segment_pos)
             segment_start = segment_end
+        raise RuntimeError("Something has gone wrong.  Could not compute Path.point({}) for path {}".format(pos, self))
 
     def length(self, T0=0, T1=1, error=LENGTH_ERROR, min_depth=LENGTH_MIN_DEPTH):
         self._calc_lengths(error=error, min_depth=min_depth)
         if T0 == 0 and T1 == 1:
             return self._length
         else:
             if len(self) == 1:
```

### Comparing `svgpathtools-1.6.0/svgpathtools/paths2svg.py` & `svgpathtools-1.6.1/svgpathtools/paths2svg.py`

 * *Files identical despite different names*

### Comparing `svgpathtools-1.6.0/svgpathtools/polytools.py` & `svgpathtools-1.6.1/svgpathtools/polytools.py`

 * *Files identical despite different names*

### Comparing `svgpathtools-1.6.0/svgpathtools/smoothing.py` & `svgpathtools-1.6.1/svgpathtools/smoothing.py`

 * *Files identical despite different names*

### Comparing `svgpathtools-1.6.0/svgpathtools/svg_io_sax.py` & `svgpathtools-1.6.1/svgpathtools/svg_io_sax.py`

 * *Files identical despite different names*

### Comparing `svgpathtools-1.6.0/svgpathtools/svg_to_paths.py` & `svgpathtools-1.6.1/svgpathtools/svg_to_paths.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     cy = float(cy)
 
     d = ''
     d += 'M' + str(cx - rx) + ',' + str(cy)
     d += 'a' + str(rx) + ',' + str(ry) + ' 0 1,0 ' + str(2 * rx) + ',0'
     d += 'a' + str(rx) + ',' + str(ry) + ' 0 1,0 ' + str(-2 * rx) + ',0'
 
-    return d
+    return d + 'z'
 
 
 def polyline2pathd(polyline, is_polygon=False):
     """converts the string from a polyline points-attribute to a string for a
     Path object d-attribute"""
     if isinstance(polyline, str):
         points = polyline
```

### Comparing `svgpathtools-1.6.0/svgpathtools.egg-info/PKG-INFO` & `svgpathtools-1.6.1/svgpathtools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: svgpathtools
-Version: 1.6.0
+Version: 1.6.1
 Summary: A collection of tools for manipulating and analyzing SVG Path objects and Bezier curves.
 Home-page: https://github.com/mathandy/svgpathtools
-Download-URL: https://github.com/mathandy/svgpathtools/releases/download/1.6.0/svgpathtools-1.6.0-py2.py3-none-any.whl
+Download-URL: https://github.com/mathandy/svgpathtools/releases/download/1.6.1/svgpathtools-1.6.1-py2.py3-none-any.whl
 Author: Andy Port
 Author-email: AndyAPort@gmail.com
 License: MIT
 Keywords: svg,svg path,svg.path,bezier,parse svg path,display svg
 Platform: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -18,28 +18,28 @@
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Multimedia :: Graphics :: Editors :: Vector-Based
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 [![Donate](https://img.shields.io/badge/donate-paypal-brightgreen)](https://www.paypal.com/donate?business=4SKJ27AM4EYYA&amp;no_recurring=0&amp;item_name=Support+the+creator+of+svgpathtools?++He%27s+a+student+and+would+appreciate+it.&amp;currency_code=USD)
 ![Python](https://img.shields.io/pypi/pyversions/svgpathtools.svg)
 [![PyPI](https://img.shields.io/pypi/v/svgpathtools)](https://pypi.org/project/svgpathtools/)
-![Build](https://img.shields.io/github/workflow/status/mathandy/svgpathtools/Github%20CI%20Unit%20Testing)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/svgpathtools?color=yellow)](https://pypistats.org/packages/svgpathtools)
 # svgpathtools
 
 
 svgpathtools is a collection of tools for manipulating and analyzing SVG Path objects and Bézier curves.
 
 ## Features
```

### Comparing `svgpathtools-1.6.0/svgpathtools.egg-info/SOURCES.txt` & `svgpathtools-1.6.1/svgpathtools.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 svgpathtools.egg-info/dependency_links.txt
 svgpathtools.egg-info/requires.txt
 svgpathtools.egg-info/top_level.txt
 test/circle.svg
 test/display_temp.svg
 test/ellipse.svg
 test/groups.svg
+test/negative-scale.svg
 test/polygons.svg
 test/rects.svg
 test/test.svg
 test/test_bezier.py
 test/test_document.py
 test/test_generation.py
 test/test_groups.py
```

### Comparing `svgpathtools-1.6.0/test/display_temp.svg` & `svgpathtools-1.6.1/test/display_temp.svg`

 * *Files identical despite different names*

### Comparing `svgpathtools-1.6.0/test/groups.svg` & `svgpathtools-1.6.1/test/groups.svg`

 * *Files identical despite different names*

### Comparing `svgpathtools-1.6.0/test/test.svg` & `svgpathtools-1.6.1/test/test.svg`

 * *Files identical despite different names*

### Comparing `svgpathtools-1.6.0/test/test_bezier.py` & `svgpathtools-1.6.1/test/test_bezier.py`

 * *Files identical despite different names*

### Comparing `svgpathtools-1.6.0/test/test_document.py` & `svgpathtools-1.6.1/test/test_document.py`

 * *Files identical despite different names*

### Comparing `svgpathtools-1.6.0/test/test_generation.py` & `svgpathtools-1.6.1/test/test_generation.py`

 * *Files identical despite different names*

### Comparing `svgpathtools-1.6.0/test/test_groups.py` & `svgpathtools-1.6.1/test/test_groups.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 """Tests related to SVG groups.
 
 To run these tests, you can use (from root svgpathtools directory):
 $ python -m unittest test.test_groups.TestGroups.test_group_flatten
 """
 from __future__ import division, absolute_import, print_function
 import unittest
-from svgpathtools import Document, SVG_NAMESPACE, parse_path
+from svgpathtools import Document, SVG_NAMESPACE, parse_path, Line, Arc
 from os.path import join, dirname
 import numpy as np
 
 
+# When an assert fails, show the full error message, don't truncate it.
+unittest.util._MAX_LENGTH = 999999999
+
+
 def get_desired_path(name, paths):
     return next(p for p in paths
                 if p.element.get('{some://testuri}name') == name)
 
 
 class TestGroups(unittest.TestCase):
 
@@ -38,14 +42,30 @@
         v_e = v_s + v_e_relative_vals
 
         actual = get_desired_path(name, paths)
 
         self.check_values(tf.dot(v_s), actual.start)
         self.check_values(tf.dot(v_e), actual.end)
 
+    def test_group_transform(self):
+        # The input svg has a group transform of "scale(1,-1)", which
+        # can mess with Arc sweeps.
+        doc = Document(join(dirname(__file__), 'negative-scale.svg'))
+        path = doc.paths()[0]
+        self.assertEqual(path[0], Line(start=-10j, end=-80j))
+        self.assertEqual(path[1], Arc(start=-80j, radius=(30+30j), rotation=0.0, large_arc=True, sweep=True, end=-140j))
+        self.assertEqual(path[2], Arc(start=-140j, radius=(20+20j), rotation=0.0, large_arc=False, sweep=False, end=-100j))
+        self.assertEqual(path[3], Line(start=-100j, end=(100-100j)))
+        self.assertEqual(path[4], Arc(start=(100-100j), radius=(20+20j), rotation=0.0, large_arc=True, sweep=False, end=(100-140j)))
+        self.assertEqual(path[5], Arc(start=(100-140j), radius=(30+30j), rotation=0.0, large_arc=False, sweep=True, end=(100-80j)))
+        self.assertEqual(path[6], Line(start=(100-80j), end=(100-10j)))
+        self.assertEqual(path[7], Arc(start=(100-10j), radius=(10+10j), rotation=0.0, large_arc=False, sweep=True, end=(90+0j)))
+        self.assertEqual(path[8], Line(start=(90+0j), end=(10+0j)))
+        self.assertEqual(path[9], Arc(start=(10+0j), radius=(10+10j), rotation=0.0, large_arc=False, sweep=True, end=-10j))
+
     def test_group_flatten(self):
         # Test the Document.paths() function against the
         # groups.svg test file.
         # There are 12 paths in that file, with various levels of being
         # nested inside of group transforms.
         # The check_line function is used to reduce the boilerplate,
         # since all the tests are very similar.
```

### Comparing `svgpathtools-1.6.0/test/test_parsing.py` & `svgpathtools-1.6.1/test/test_parsing.py`

 * *Files identical despite different names*

### Comparing `svgpathtools-1.6.0/test/test_path.py` & `svgpathtools-1.6.1/test/test_path.py`

 * *Files identical despite different names*

### Comparing `svgpathtools-1.6.0/test/test_polytools.py` & `svgpathtools-1.6.1/test/test_polytools.py`

 * *Files identical despite different names*

### Comparing `svgpathtools-1.6.0/test/test_sax_groups.py` & `svgpathtools-1.6.1/test/test_sax_groups.py`

 * *Files identical despite different names*

### Comparing `svgpathtools-1.6.0/test/test_svg2paths.py` & `svgpathtools-1.6.1/test/test_svg2paths.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from __future__ import division, absolute_import, print_function
 import unittest
 from svgpathtools import Path, Line, Arc, svg2paths, svgstr2paths
 from io import StringIO
 from io import open  # overrides build-in open for compatibility with python2
+import os
 from os.path import join, dirname
 from sys import version_info
+import tempfile
+import shutil
 
 from svgpathtools.svg_to_paths import rect2pathd
 
 
 class TestSVG2Paths(unittest.TestCase):
     def test_svg2paths_polygons(self):
 
@@ -53,14 +56,34 @@
         path_circle = paths[0]
         path_circle_correct = Path(Arc(50+100j, 50+50j, 0.0, True, False, 150+100j),
                                     Arc(150+100j, 50+50j, 0.0, True, False, 50+100j))
         self.assertTrue(len(path_circle)==2)
         self.assertTrue(path_circle==path_circle_correct)
         self.assertTrue(path_circle.isclosed())
 
+        # test for issue #198 (circles not being closed)
+        svg = u"""<?xml version="1.0" encoding="UTF-8"?>
+        <svg xmlns="http://www.w3.org/2000/svg" xmlns:svg="http://www.w3.org/2000/svg" width="40mm" height="40mm" 
+          viewBox="0 0 40 40" version="1.1">
+            
+          <g id="layer">
+            <circle id="c1" cx="20.000" cy="20.000" r="11.000" />
+            <circle id="c2" cx="20.000" cy="20.000" r="5.15" />
+          </g>
+        </svg>"""
+        tmpdir = tempfile.mkdtemp()
+        svgfile = os.path.join(tmpdir, 'test.svg')
+        with open(svgfile, 'w') as f:
+            f.write(svg)
+        paths, _ = svg2paths(svgfile)
+        self.assertEqual(len(paths), 2)
+        self.assertTrue(paths[0].isclosed())
+        self.assertTrue(paths[1].isclosed())
+        shutil.rmtree(tmpdir)
+
     def test_rect2pathd(self):
         non_rounded = {"x":"10", "y":"10", "width":"100","height":"100"}
         self.assertEqual(rect2pathd(non_rounded), 'M10.0 10.0 L 110.0 10.0 L 110.0 110.0 L 10.0 110.0 z')
         rounded = {"x":"10", "y":"10", "width":"100","height":"100", "rx":"15", "ry": "12"}
         self.assertEqual(rect2pathd(rounded), "M 25.0 10.0 L 95.0 10.0 A 15.0 12.0 0 0 1 110.0 22.0 L 110.0 98.0 A 15.0 12.0 0 0 1 95.0 110.0 L 25.0 110.0 A 15.0 12.0 0 0 1 10.0 98.0 L 10.0 22.0 A 15.0 12.0 0 0 1 25.0 10.0 z")
 
     def test_from_file_path_string(self):
@@ -103,7 +126,11 @@
                   'r', encoding='utf-8') as file:
             # read entire file into string
             file_content = file.read()
 
             paths, _ = svgstr2paths(file_content)
 
             self.assertEqual(len(paths), 2)
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `svgpathtools-1.6.0/test/transforms.svg` & `svgpathtools-1.6.1/test/transforms.svg`

 * *Files identical despite different names*

### Comparing `svgpathtools-1.6.0/test.svg` & `svgpathtools-1.6.1/test.svg`

 * *Files identical despite different names*

### Comparing `svgpathtools-1.6.0/vectorframes.svg` & `svgpathtools-1.6.1/vectorframes.svg`

 * *Files identical despite different names*

