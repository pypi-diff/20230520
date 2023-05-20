# Comparing `tmp/myfuncs-0.1.5.tar.gz` & `tmp/myfuncs-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myfuncs-0.1.5.tar", last modified: Sat May 20 07:17:39 2023, max compression
+gzip compressed data, was "myfuncs-0.1.6.tar", last modified: Sat May 20 09:17:28 2023, max compression
```

## Comparing `myfuncs-0.1.5.tar` & `myfuncs-0.1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 work       (501) staff       (20)        0 2023-05-20 07:17:39.652139 myfuncs-0.1.5/
--rw-r--r--   0 work       (501) staff       (20)     1068 2023-05-13 16:42:37.000000 myfuncs-0.1.5/LICENSE
--rw-r--r--   0 work       (501) staff       (20)     2426 2023-05-20 07:17:39.651967 myfuncs-0.1.5/PKG-INFO
--rw-r--r--   0 work       (501) staff       (20)     1687 2023-05-13 21:07:45.000000 myfuncs-0.1.5/README.md
-drwxr-xr-x   0 work       (501) staff       (20)        0 2023-05-20 07:17:39.651270 myfuncs-0.1.5/myfuncs/
--rw-r--r--   0 work       (501) staff       (20)       21 2023-05-13 18:23:34.000000 myfuncs-0.1.5/myfuncs/__init__.py
--rw-r--r--   0 work       (501) staff       (20)     3891 2023-05-20 03:36:35.000000 myfuncs-0.1.5/myfuncs/funcs.py
-drwxr-xr-x   0 work       (501) staff       (20)        0 2023-05-20 07:17:39.651776 myfuncs-0.1.5/myfuncs.egg-info/
--rw-r--r--   0 work       (501) staff       (20)     2426 2023-05-20 07:17:39.000000 myfuncs-0.1.5/myfuncs.egg-info/PKG-INFO
--rw-r--r--   0 work       (501) staff       (20)      187 2023-05-20 07:17:39.000000 myfuncs-0.1.5/myfuncs.egg-info/SOURCES.txt
--rw-r--r--   0 work       (501) staff       (20)        1 2023-05-20 07:17:39.000000 myfuncs-0.1.5/myfuncs.egg-info/dependency_links.txt
--rw-r--r--   0 work       (501) staff       (20)        8 2023-05-20 07:17:39.000000 myfuncs-0.1.5/myfuncs.egg-info/top_level.txt
--rw-r--r--   0 work       (501) staff       (20)       38 2023-05-20 07:17:39.652180 myfuncs-0.1.5/setup.cfg
--rw-r--r--   0 work       (501) staff       (20)      916 2023-05-20 07:17:18.000000 myfuncs-0.1.5/setup.py
+drwxr-xr-x   0 work       (501) staff       (20)        0 2023-05-20 09:17:28.530643 myfuncs-0.1.6/
+-rw-r--r--   0 work       (501) staff       (20)     1068 2023-05-13 16:42:37.000000 myfuncs-0.1.6/LICENSE
+-rw-r--r--   0 work       (501) staff       (20)     2426 2023-05-20 09:17:28.530526 myfuncs-0.1.6/PKG-INFO
+-rw-r--r--   0 work       (501) staff       (20)     1687 2023-05-13 21:07:45.000000 myfuncs-0.1.6/README.md
+drwxr-xr-x   0 work       (501) staff       (20)        0 2023-05-20 09:17:28.529927 myfuncs-0.1.6/myfuncs/
+-rw-r--r--   0 work       (501) staff       (20)       21 2023-05-13 18:23:34.000000 myfuncs-0.1.6/myfuncs/__init__.py
+-rw-r--r--   0 work       (501) staff       (20)     4331 2023-05-20 09:12:09.000000 myfuncs-0.1.6/myfuncs/funcs.py
+drwxr-xr-x   0 work       (501) staff       (20)        0 2023-05-20 09:17:28.530368 myfuncs-0.1.6/myfuncs.egg-info/
+-rw-r--r--   0 work       (501) staff       (20)     2426 2023-05-20 09:17:28.000000 myfuncs-0.1.6/myfuncs.egg-info/PKG-INFO
+-rw-r--r--   0 work       (501) staff       (20)      187 2023-05-20 09:17:28.000000 myfuncs-0.1.6/myfuncs.egg-info/SOURCES.txt
+-rw-r--r--   0 work       (501) staff       (20)        1 2023-05-20 09:17:28.000000 myfuncs-0.1.6/myfuncs.egg-info/dependency_links.txt
+-rw-r--r--   0 work       (501) staff       (20)        8 2023-05-20 09:17:28.000000 myfuncs-0.1.6/myfuncs.egg-info/top_level.txt
+-rw-r--r--   0 work       (501) staff       (20)       38 2023-05-20 09:17:28.530681 myfuncs-0.1.6/setup.cfg
+-rw-r--r--   0 work       (501) staff       (20)      916 2023-05-20 09:17:23.000000 myfuncs-0.1.6/setup.py
```

### Comparing `myfuncs-0.1.5/LICENSE` & `myfuncs-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `myfuncs-0.1.5/PKG-INFO` & `myfuncs-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfuncs
-Version: 0.1.5
+Version: 0.1.6
 Summary: Personal utility functions that I use across different codebases.
 Home-page: https://github.com/cc-d/myfuncs
 Author: Cary Carter
 Author-email: ccarterdev@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `myfuncs-0.1.5/README.md` & `myfuncs-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `myfuncs-0.1.5/myfuncs/funcs.py` & `myfuncs-0.1.6/myfuncs/funcs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 import os
 import re
 import time
 import inspect
+import random
+import string
 from datetime import datetime
 from functools import wraps
 from typing import Any, Callable, Optional, TypeVar, Union
 
 import logging
 
 logger = logging.getLogger(__name__)
 
 T = TypeVar("T", bound=Callable[..., Any])
 
+ASCII_CHARS = string.ascii_letters + string.ascii_lowercase + string.ascii_uppercase
+
 
 def trunc_str(string: str, max_length: int) -> str:
     """
     Truncates a string if its length exceeds the specified maximum length.
     If the string is truncated, it appends '...' to indicate the truncation.
 
     Args:
@@ -95,14 +99,32 @@
                 # Log the message using the specified level.
                 logger.log(level_int, log_message)
 
             return result
         return wrapper
     return decorator
 
+
+@logf()
+def ran_str(length: int) -> str:
+    """ Returns a string of random ascii characters of n length
+
+    Args:
+        length (int): length of returned str
+
+    Returns:
+        str: random char string of n length
+    """
+    s = ''
+    for i in range(0, length):
+        s += random.choice(ASCII_CHARS)
+    return s
+
+
+
 @logf()
 def get_asctime() -> str:
     """Returns the current time in the same format as logging %(asctime)s
 
 
     Returns:
         str: current asctime
```

### Comparing `myfuncs-0.1.5/myfuncs.egg-info/PKG-INFO` & `myfuncs-0.1.6/myfuncs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfuncs
-Version: 0.1.5
+Version: 0.1.6
 Summary: Personal utility functions that I use across different codebases.
 Home-page: https://github.com/cc-d/myfuncs
 Author: Cary Carter
 Author-email: ccarterdev@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `myfuncs-0.1.5/setup.py` & `myfuncs-0.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfuncs',
-    version='0.1.5',
+    version='0.1.6',
     packages=find_packages(),
     install_requires=[],
     author='Cary Carter',
     author_email='ccarterdev@gmail.com',
     description='Personal utility functions that I use across different codebases.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

