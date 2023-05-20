# Comparing `tmp/YetAnotherModule-0.0.1.tar.gz` & `tmp/YetAnotherModule-0.0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "YetAnotherModule-0.0.1.tar", last modified: Sat May 20 13:43:19 2023, max compression
+gzip compressed data, was "YetAnotherModule-0.0.1.1.tar", last modified: Sat May 20 16:31:11 2023, max compression
```

## Comparing `YetAnotherModule-0.0.1.tar` & `YetAnotherModule-0.0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:43:19.714459 YetAnotherModule-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-20 13:43:06.000000 YetAnotherModule-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-20 13:43:19.714459 YetAnotherModule-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-20 13:43:06.000000 YetAnotherModule-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:43:19.714459 YetAnotherModule-0.0.1/YAPM/
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-20 13:43:06.000000 YetAnotherModule-0.0.1/YAPM/Matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-20 13:43:06.000000 YetAnotherModule-0.0.1/YAPM/Random.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-20 13:43:06.000000 YetAnotherModule-0.0.1/YAPM/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:43:19.714459 YetAnotherModule-0.0.1/YetAnotherModule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-20 13:43:19.000000 YetAnotherModule-0.0.1/YetAnotherModule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-20 13:43:19.000000 YetAnotherModule-0.0.1/YetAnotherModule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 13:43:19.000000 YetAnotherModule-0.0.1/YetAnotherModule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-20 13:43:19.000000 YetAnotherModule-0.0.1/YetAnotherModule.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 13:43:19.714459 YetAnotherModule-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-20 13:43:06.000000 YetAnotherModule-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 16:31:11.047774 YetAnotherModule-0.0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-20 16:31:00.000000 YetAnotherModule-0.0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-20 16:31:11.047774 YetAnotherModule-0.0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-20 16:31:00.000000 YetAnotherModule-0.0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 16:31:11.047774 YetAnotherModule-0.0.1.1/YAPM/
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-05-20 16:31:00.000000 YetAnotherModule-0.0.1.1/YAPM/Matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-20 16:31:00.000000 YetAnotherModule-0.0.1.1/YAPM/Random.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-20 16:31:00.000000 YetAnotherModule-0.0.1.1/YAPM/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 16:31:11.047774 YetAnotherModule-0.0.1.1/YetAnotherModule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-20 16:31:11.000000 YetAnotherModule-0.0.1.1/YetAnotherModule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-20 16:31:11.000000 YetAnotherModule-0.0.1.1/YetAnotherModule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 16:31:11.000000 YetAnotherModule-0.0.1.1/YetAnotherModule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-20 16:31:11.000000 YetAnotherModule-0.0.1.1/YetAnotherModule.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 16:31:11.047774 YetAnotherModule-0.0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-20 16:31:00.000000 YetAnotherModule-0.0.1.1/setup.py
```

### Comparing `YetAnotherModule-0.0.1/LICENSE` & `YetAnotherModule-0.0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `YetAnotherModule-0.0.1/PKG-INFO` & `YetAnotherModule-0.0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YetAnotherModule
-Version: 0.0.1
+Version: 0.0.1.1
 Summary: Yet Another Python Module.
 Home-page: https://github.com/carson-coder/Yet-Another-Python-Module
 Author: Carson
 Author-email: carsondpool@gmail.com
 License: LICENSE
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `YetAnotherModule-0.0.1/README.md` & `YetAnotherModule-0.0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `YetAnotherModule-0.0.1/YAPM/Random.py` & `YetAnotherModule-0.0.1.1/YAPM/Random.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,31 @@
 from collections.abc import Sequence
 
 #
 # Random Stuff
 #
 
 def RaisesError(code: str, Ignore: Sequence[Exception] = [None,], GlobalVars: dict[str, any] = {}):
-    """Runs the code and returns (True, ReturnValue) if run successfully or (False, Error) if there was an error. Can return (True, Exception) if code raised a ignored error"""
+    """
+    Evaluates the code provited.
+    
+    :param str code: str - The code to eval
+    :param Sequence[Exception] Ignore: Exceptions to ignore
+    :param dict[str, any] GlobalVars: Globals to pass into the eval function
+
+    :returns:
+        - Tuple[True, any] - Code ran without any errors. returns code result.
+        - Tuple[True, Exception] - Code threw a error that is in the Ignored exceptions list
+        - Tuple[False, Exception] - Code threw a error that is not Ignored. 
+    
+    :raises:
+        - ValueError - Ignore isn't a iterable
+        - ValueError - GlobalVars isn't a dict
+        - ValueError - Code isn't a string
+    """
     try: 
         iter(Ignore)
     except ValueError: 
         raise ValueError("Ignore Should be an iterable")
     try: 
         dict(GlobalVars)
     except ValueError:
```

### Comparing `YetAnotherModule-0.0.1/YetAnotherModule.egg-info/PKG-INFO` & `YetAnotherModule-0.0.1.1/YetAnotherModule.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YetAnotherModule
-Version: 0.0.1
+Version: 0.0.1.1
 Summary: Yet Another Python Module.
 Home-page: https://github.com/carson-coder/Yet-Another-Python-Module
 Author: Carson
 Author-email: carsondpool@gmail.com
 License: LICENSE
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

