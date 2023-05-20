# Comparing `tmp/scratchattach-1.1.5.tar.gz` & `tmp/scratchattach-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratchattach-1.1.5.tar", last modified: Sun May  7 17:33:08 2023, max compression
+gzip compressed data, was "scratchattach-1.1.6.tar", last modified: Sat May 20 15:27:15 2023, max compression
```

## Comparing `scratchattach-1.1.5.tar` & `scratchattach-1.1.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 17:33:08.802517 scratchattach-1.1.5/
--rw-rw-rw-   0        0        0    22055 2023-05-07 17:33:08.800522 scratchattach-1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0    20740 2023-05-07 17:32:19.000000 scratchattach-1.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-07 17:33:08.764230 scratchattach-1.1.5/scratchattach/
--rw-rw-rw-   0        0        0      167 2023-05-04 16:19:46.000000 scratchattach-1.1.5/scratchattach/__init__.py
--rw-rw-rw-   0        0        0    12798 2023-05-04 17:35:55.000000 scratchattach-1.1.5/scratchattach/_cloud.py
--rw-rw-rw-   0        0        0    15496 2023-05-04 17:24:58.000000 scratchattach-1.1.5/scratchattach/_cloud_requests.py
--rw-rw-rw-   0        0        0     1797 2023-05-04 16:19:46.000000 scratchattach-1.1.5/scratchattach/_encoder.py
--rw-rw-rw-   0        0        0      888 2023-05-07 17:01:33.000000 scratchattach-1.1.5/scratchattach/_exceptions.py
--rw-rw-rw-   0        0        0     6542 2023-05-04 16:19:46.000000 scratchattach-1.1.5/scratchattach/_forum.py
--rw-rw-rw-   0        0        0    18157 2023-05-07 17:16:17.000000 scratchattach-1.1.5/scratchattach/_project.py
--rw-rw-rw-   0        0        0    17923 2023-05-04 16:19:46.000000 scratchattach-1.1.5/scratchattach/_session.py
--rw-rw-rw-   0        0        0     9646 2023-05-07 17:16:12.000000 scratchattach-1.1.5/scratchattach/_studio.py
--rw-rw-rw-   0        0        0    25434 2023-05-07 17:30:43.000000 scratchattach-1.1.5/scratchattach/_user.py
-drwxrwxrwx   0        0        0        0 2023-05-07 17:33:08.797518 scratchattach-1.1.5/scratchattach.egg-info/
--rw-rw-rw-   0        0        0    22055 2023-05-07 17:33:08.000000 scratchattach-1.1.5/scratchattach.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      464 2023-05-07 17:33:08.000000 scratchattach-1.1.5/scratchattach.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 17:33:08.000000 scratchattach-1.1.5/scratchattach.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-05-07 17:33:08.000000 scratchattach-1.1.5/scratchattach.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-07 17:33:08.000000 scratchattach-1.1.5/scratchattach.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-07 17:33:08.802517 scratchattach-1.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1112 2023-05-07 17:32:47.000000 scratchattach-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 15:27:15.134757 scratchattach-1.1.6/
+-rw-rw-rw-   0        0        0    22055 2023-05-20 15:27:15.132676 scratchattach-1.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0    20740 2023-05-07 17:32:19.000000 scratchattach-1.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-20 15:27:15.064044 scratchattach-1.1.6/scratchattach/
+-rw-rw-rw-   0        0        0      167 2023-05-04 16:19:46.000000 scratchattach-1.1.6/scratchattach/__init__.py
+-rw-rw-rw-   0        0        0    12776 2023-05-20 15:26:23.000000 scratchattach-1.1.6/scratchattach/_cloud.py
+-rw-rw-rw-   0        0        0    15496 2023-05-04 17:24:58.000000 scratchattach-1.1.6/scratchattach/_cloud_requests.py
+-rw-rw-rw-   0        0        0     1797 2023-05-04 16:19:46.000000 scratchattach-1.1.6/scratchattach/_encoder.py
+-rw-rw-rw-   0        0        0      888 2023-05-07 17:01:33.000000 scratchattach-1.1.6/scratchattach/_exceptions.py
+-rw-rw-rw-   0        0        0     6542 2023-05-04 16:19:46.000000 scratchattach-1.1.6/scratchattach/_forum.py
+-rw-rw-rw-   0        0        0    18157 2023-05-07 17:16:17.000000 scratchattach-1.1.6/scratchattach/_project.py
+-rw-rw-rw-   0        0        0    17923 2023-05-04 16:19:46.000000 scratchattach-1.1.6/scratchattach/_session.py
+-rw-rw-rw-   0        0        0     9646 2023-05-07 17:16:12.000000 scratchattach-1.1.6/scratchattach/_studio.py
+-rw-rw-rw-   0        0        0    25434 2023-05-07 17:30:43.000000 scratchattach-1.1.6/scratchattach/_user.py
+drwxrwxrwx   0        0        0        0 2023-05-20 15:27:15.128687 scratchattach-1.1.6/scratchattach.egg-info/
+-rw-rw-rw-   0        0        0    22055 2023-05-20 15:27:14.000000 scratchattach-1.1.6/scratchattach.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2023-05-20 15:27:14.000000 scratchattach-1.1.6/scratchattach.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 15:27:14.000000 scratchattach-1.1.6/scratchattach.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-05-20 15:27:14.000000 scratchattach-1.1.6/scratchattach.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-20 15:27:14.000000 scratchattach-1.1.6/scratchattach.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-20 15:27:15.135875 scratchattach-1.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1112 2023-05-20 15:26:45.000000 scratchattach-1.1.6/setup.py
```

### Comparing `scratchattach-1.1.5/PKG-INFO` & `scratchattach-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchattach
-Version: 1.1.5
+Version: 1.1.6
 Summary: An Scratch API Wrapper for scratch.mit.edu
 Home-page: https://github.com/TimMcCool/scratchattach
 Author: TimMcCool
 Author-email: timmccool.scratch@gmail.com
 Keywords: scratch api,scratchattach,scratch api python,scratch python,scratch for python,scratch,scratch cloud,scratch cloud variables,scratch bot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `scratchattach-1.1.5/README.md` & `scratchattach-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `scratchattach-1.1.5/scratchattach/_cloud.py` & `scratchattach-1.1.6/scratchattach/_cloud.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #----- Cloud interactions
-from numpy import var
 import websocket
 import json
 import requests
 from threading import Thread
 import time
 from . import _exceptions
 import traceback
```

### Comparing `scratchattach-1.1.5/scratchattach/_cloud_requests.py` & `scratchattach-1.1.6/scratchattach/_cloud_requests.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.1.5/scratchattach/_encoder.py` & `scratchattach-1.1.6/scratchattach/_encoder.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.1.5/scratchattach/_exceptions.py` & `scratchattach-1.1.6/scratchattach/_exceptions.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.1.5/scratchattach/_forum.py` & `scratchattach-1.1.6/scratchattach/_forum.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.1.5/scratchattach/_project.py` & `scratchattach-1.1.6/scratchattach/_project.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.1.5/scratchattach/_session.py` & `scratchattach-1.1.6/scratchattach/_session.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.1.5/scratchattach/_studio.py` & `scratchattach-1.1.6/scratchattach/_studio.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.1.5/scratchattach/_user.py` & `scratchattach-1.1.6/scratchattach/_user.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.1.5/scratchattach.egg-info/PKG-INFO` & `scratchattach-1.1.6/scratchattach.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchattach
-Version: 1.1.5
+Version: 1.1.6
 Summary: An Scratch API Wrapper for scratch.mit.edu
 Home-page: https://github.com/TimMcCool/scratchattach
 Author: TimMcCool
 Author-email: timmccool.scratch@gmail.com
 Keywords: scratch api,scratchattach,scratch api python,scratch python,scratch for python,scratch,scratch cloud,scratch cloud variables,scratch bot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `scratchattach-1.1.5/setup.py` & `scratchattach-1.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '1.1.5'
+VERSION = '1.1.6'
 DESCRIPTION = 'An Scratch API Wrapper for scratch.mit.edu'
 LONG_DESCRIPTION = DESCRIPTION
 
 # Setting up
 setup(
     name="scratchattach",
     version=VERSION,
```

