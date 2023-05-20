# Comparing `tmp/flanautils-1.7.1.tar.gz` & `tmp/flanautils-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flanautils-1.7.1.tar", last modified: Sat May  6 18:46:02 2023, max compression
+gzip compressed data, was "flanautils-1.7.2.tar", last modified: Sat May 20 04:34:07 2023, max compression
```

## Comparing `flanautils-1.7.1.tar` & `flanautils-1.7.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:46:02.574962 flanautils-1.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-06 18:45:48.000000 flanautils-1.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-06 18:46:02.574962 flanautils-1.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-06 18:45:48.000000 flanautils-1.7.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:46:02.570962 flanautils-1.7.1/flanautils/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-06 18:45:48.000000 flanautils-1.7.1/flanautils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-05-06 18:45:48.000000 flanautils-1.7.1/flanautils/asyncs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15682 2023-05-06 18:45:48.000000 flanautils-1.7.1/flanautils/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:46:02.570962 flanautils-1.7.1/flanautils/data_structures/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-06 18:45:48.000000 flanautils-1.7.1/flanautils/data_structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-05-06 18:45:48.000000 flanautils-1.7.1/flanautils/data_structures/bi_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)    10550 2023-05-06 18:45:48.000000 flanautils-1.7.1/flanautils/data_structures/ordered_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-05-06 18:45:48.000000 flanautils-1.7.1/flanautils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-06 18:45:48.000000 flanautils-1.7.1/flanautils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-05-06 18:45:48.000000 flanautils-1.7.1/flanautils/iterables.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-06 18:45:48.000000 flanautils-1.7.1/flanautils/maths.py
--rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-05-06 18:45:48.000000 flanautils-1.7.1/flanautils/medias.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:46:02.570962 flanautils-1.7.1/flanautils/models/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-06 18:45:48.000000 flanautils-1.7.1/flanautils/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25248 2023-05-06 18:45:48.000000 flanautils-1.7.1/flanautils/models/bases.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-06 18:45:48.000000 flanautils-1.7.1/flanautils/models/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-06 18:45:48.000000 flanautils-1.7.1/flanautils/models/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-06 18:45:48.000000 flanautils-1.7.1/flanautils/models/media.py
--rw-r--r--   0 runner    (1001) docker     (123)    11334 2023-05-06 18:45:48.000000 flanautils-1.7.1/flanautils/models/plotly_charts.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-06 18:45:48.000000 flanautils-1.7.1/flanautils/models/score_match.py
--rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-05-06 18:45:48.000000 flanautils-1.7.1/flanautils/models/time_units.py
--rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-05-06 18:45:48.000000 flanautils-1.7.1/flanautils/oss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-06 18:45:48.000000 flanautils-1.7.1/flanautils/requests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:46:02.570962 flanautils-1.7.1/flanautils/resources/
--rw-r--r--   0 runner    (1001) docker     (123)  3602215 2023-05-06 18:45:48.000000 flanautils-1.7.1/flanautils/resources/plotly_es.js
--rw-r--r--   0 runner    (1001) docker     (123)    14597 2023-05-06 18:45:48.000000 flanautils-1.7.1/flanautils/strings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:46:02.570962 flanautils-1.7.1/flanautils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-06 18:46:02.000000 flanautils-1.7.1/flanautils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-06 18:46:02.000000 flanautils-1.7.1/flanautils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 18:46:02.000000 flanautils-1.7.1/flanautils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-06 18:46:02.000000 flanautils-1.7.1/flanautils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-06 18:46:02.000000 flanautils-1.7.1/flanautils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-06 18:45:48.000000 flanautils-1.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-06 18:46:02.574962 flanautils-1.7.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:46:02.574962 flanautils-1.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-06 18:45:48.000000 flanautils-1.7.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 04:34:07.338575 flanautils-1.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-20 04:33:49.000000 flanautils-1.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-20 04:34:07.338575 flanautils-1.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-20 04:33:49.000000 flanautils-1.7.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 04:34:07.330575 flanautils-1.7.2/flanautils/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-20 04:33:49.000000 flanautils-1.7.2/flanautils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-05-20 04:33:49.000000 flanautils-1.7.2/flanautils/asyncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15682 2023-05-20 04:33:49.000000 flanautils-1.7.2/flanautils/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 04:34:07.334575 flanautils-1.7.2/flanautils/data_structures/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-20 04:33:49.000000 flanautils-1.7.2/flanautils/data_structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-05-20 04:33:49.000000 flanautils-1.7.2/flanautils/data_structures/bi_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10550 2023-05-20 04:33:49.000000 flanautils-1.7.2/flanautils/data_structures/ordered_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-20 04:33:49.000000 flanautils-1.7.2/flanautils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-05-20 04:33:49.000000 flanautils-1.7.2/flanautils/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-05-20 04:33:49.000000 flanautils-1.7.2/flanautils/iterables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-20 04:33:49.000000 flanautils-1.7.2/flanautils/maths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-05-20 04:33:49.000000 flanautils-1.7.2/flanautils/medias.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 04:34:07.334575 flanautils-1.7.2/flanautils/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-20 04:33:49.000000 flanautils-1.7.2/flanautils/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25248 2023-05-20 04:33:49.000000 flanautils-1.7.2/flanautils/models/bases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-20 04:33:49.000000 flanautils-1.7.2/flanautils/models/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-20 04:33:49.000000 flanautils-1.7.2/flanautils/models/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-20 04:33:49.000000 flanautils-1.7.2/flanautils/models/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11334 2023-05-20 04:33:49.000000 flanautils-1.7.2/flanautils/models/plotly_charts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-20 04:33:49.000000 flanautils-1.7.2/flanautils/models/score_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-05-20 04:33:49.000000 flanautils-1.7.2/flanautils/models/time_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-05-20 04:33:49.000000 flanautils-1.7.2/flanautils/oss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-05-20 04:33:49.000000 flanautils-1.7.2/flanautils/requests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 04:34:07.334575 flanautils-1.7.2/flanautils/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)  3602215 2023-05-20 04:33:49.000000 flanautils-1.7.2/flanautils/resources/plotly_es.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14597 2023-05-20 04:33:49.000000 flanautils-1.7.2/flanautils/strings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 04:34:07.330575 flanautils-1.7.2/flanautils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-20 04:34:07.000000 flanautils-1.7.2/flanautils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-20 04:34:07.000000 flanautils-1.7.2/flanautils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 04:34:07.000000 flanautils-1.7.2/flanautils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-20 04:34:07.000000 flanautils-1.7.2/flanautils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-20 04:34:07.000000 flanautils-1.7.2/flanautils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-20 04:33:49.000000 flanautils-1.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-20 04:34:07.338575 flanautils-1.7.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 04:34:07.338575 flanautils-1.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-20 04:33:49.000000 flanautils-1.7.2/tests/test_utils.py
```

### Comparing `flanautils-1.7.1/LICENSE` & `flanautils-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flanautils-1.7.1/PKG-INFO` & `flanautils-1.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flanautils
-Version: 1.7.1
+Version: 1.7.2
 Summary: Set of utilities of all kinds to develop python projects.
 Home-page: https://github.com/AlberLC/flanautils
 Author: AlberLC
 Project-URL: Bug Tracker, https://github.com/AlberLC/flanautils/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `flanautils-1.7.1/README.rst` & `flanautils-1.7.2/README.rst`

 * *Files identical despite different names*

### Comparing `flanautils-1.7.1/flanautils/asyncs.py` & `flanautils-1.7.2/flanautils/asyncs.py`

 * *Files identical despite different names*

### Comparing `flanautils-1.7.1/flanautils/constants.py` & `flanautils-1.7.2/flanautils/constants.py`

 * *Files identical despite different names*

### Comparing `flanautils-1.7.1/flanautils/data_structures/bi_dict.py` & `flanautils-1.7.2/flanautils/data_structures/bi_dict.py`

 * *Files identical despite different names*

### Comparing `flanautils-1.7.1/flanautils/data_structures/ordered_set.py` & `flanautils-1.7.2/flanautils/data_structures/ordered_set.py`

 * *Files identical despite different names*

### Comparing `flanautils-1.7.1/flanautils/decorators.py` & `flanautils-1.7.2/flanautils/functions.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,28 +3,35 @@
 import inspect
 import timeit
 from typing import Any, Callable, Iterable, Type
 
 from flanautils import iterables
 
 
+def is_function(func: Any) -> bool:
+    if isinstance(func, functools.partial):
+        func = func.func
+
+    return inspect.isfunction(func) or inspect.ismethod(func)
+
+
 # --------------------------------------------------------- #
 # -------------------- META DECORATORS -------------------- #
 # --------------------------------------------------------- #
 def shift_args_if_called(func_: Callable = None, *, exclude_self_types: str | Type | Iterable[str | Type] = (), globals_: dict = None) -> Callable:
     """Decorator for decorators that shifts the arguments depending on whether the decorator is called or not."""
 
-    if func_ is not None and not inspect.isfunction(func_) and not inspect.ismethod(func_):
+    if func_ is not None and not is_function(func_):
         func_, exclude_self_types, globals_ = iterables.shift_function_args(func_, exclude_self_types, globals_, func=shift_args_if_called)
 
-    def decorator(func):
+    def decorator(func: Callable):
         @functools.wraps(func)
         def wrapper(*args, **kwargs):
             self, args = iterables.separate_self_from_args(args, exclude_self_types, globals_)
-            if args and args[0] is not None and not inspect.isfunction(args[0]) and not inspect.ismethod(args[0]):
+            if args and args[0] is not None and not is_function(args[0]):
                 args = iterables.shift_function_args(*args, func=func)
 
             if self:
                 return func(self, *args, **kwargs)
             else:
                 return func(*args, **kwargs)
 
@@ -91,15 +98,15 @@
     return decorator(func_) if func_ else decorator
 
 
 @shift_args_if_called
 def time_it(func_: Callable = None, /, n_executions=1) -> Callable:
     """Decorator that prints the seconds it takes for the function to run."""
 
-    def decorator(func):
+    def decorator(func: Callable):
         @functools.wraps(func)
         def wrapper(*args, **kwargs):
             new_template = f"""def inner(_it, _timer{{init}}):
                                    {{setup}}
                                    _t0 = _timer()
                                    for _i in _it:
                                        result = {{stmt}}
```

### Comparing `flanautils-1.7.1/flanautils/iterables.py` & `flanautils-1.7.2/flanautils/iterables.py`

 * *Files 3% similar despite different names*

```diff
@@ -133,19 +133,19 @@
         nonlocal current_depth
 
         if depth_ is not None:
             current_depth += 1
 
         for arg_ in args_:
             if (
-                    isinstance(arg_, Iterable)
-                    and
-                    not isinstance(arg_, (str, bytes))
-                    and
-                    (depth_ is None or current_depth < depth_)
+                isinstance(arg_, Iterable)
+                and
+                not isinstance(arg_, (str, bytes))
+                and
+                (depth_ is None or current_depth < depth_)
             ):
                 yield from flatten_generator(*arg_, depth_=depth_)
                 if depth_ is not None:
                     current_depth -= 1
             else:
                 yield arg_
 
@@ -179,14 +179,17 @@
     [2.0, 2.5, 3.0, 3.5, 4.0, 4.5]
     >>> list(frange(2, 5, 0.5, include_last=True))
     [2.0, 2.5, 3.0, 3.5, 4.0, 4.5, 5.0]
     >>> list(frange(3, 5, 0.2))
     [3.0, 3.2, 3.4000000000000004, 3.6000000000000005, 3.8000000000000007, 4.000000000000001, 4.200000000000001, 4.400000000000001, 4.600000000000001, 4.800000000000002]
     """
 
+    if step == 0:
+        raise ValueError('step must not be zero')
+
     match start, stop:
         case [(int() | float()) as stop, None]:
             start = 0
         case [(int() | float()) as stop, bool(include_last)]:
             start = 0
 
     step_sign = maths.sign(step)
@@ -250,16 +253,11 @@
 
 def shift_function_args(*args, func: Callable = None, first_arg_default: Any = None) -> tuple:
     """
     Shift received arguments one position to the right, taking into account the possible default value of the first
     argument.
     """
 
-    match func, first_arg_default:
-        case func, _ if isinstance(func, Callable):
-            first_arg_default = next(iter(inspect.signature(func).parameters.values())).default
-        case _, first_arg_default:
-            pass
-        case _:
-            raise TypeError('bad arguments')
+    if isinstance(func, Callable):
+        first_arg_default = next(iter(inspect.signature(func).parameters.values())).default
 
     return None if first_arg_default is inspect.Parameter.empty else first_arg_default, *args
```

### Comparing `flanautils-1.7.1/flanautils/medias.py` & `flanautils-1.7.2/flanautils/medias.py`

 * *Files identical despite different names*

### Comparing `flanautils-1.7.1/flanautils/models/bases.py` & `flanautils-1.7.2/flanautils/models/bases.py`

 * *Files identical despite different names*

### Comparing `flanautils-1.7.1/flanautils/models/database.py` & `flanautils-1.7.2/flanautils/models/database.py`

 * *Files identical despite different names*

### Comparing `flanautils-1.7.1/flanautils/models/enums.py` & `flanautils-1.7.2/flanautils/models/enums.py`

 * *Files identical despite different names*

### Comparing `flanautils-1.7.1/flanautils/models/media.py` & `flanautils-1.7.2/flanautils/models/media.py`

 * *Files identical despite different names*

### Comparing `flanautils-1.7.1/flanautils/models/plotly_charts.py` & `flanautils-1.7.2/flanautils/models/plotly_charts.py`

 * *Files identical despite different names*

### Comparing `flanautils-1.7.1/flanautils/models/score_match.py` & `flanautils-1.7.2/flanautils/models/score_match.py`

 * *Files identical despite different names*

### Comparing `flanautils-1.7.1/flanautils/models/time_units.py` & `flanautils-1.7.2/flanautils/models/time_units.py`

 * *Files identical despite different names*

### Comparing `flanautils-1.7.1/flanautils/oss.py` & `flanautils-1.7.2/flanautils/oss.py`

 * *Files identical despite different names*

### Comparing `flanautils-1.7.1/flanautils/requests.py` & `flanautils-1.7.2/flanautils/requests.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,44 @@
 import asyncio
 import functools
 import html
 import random
 
 import aiohttp
 import aiohttp.client_exceptions
+import browser_cookie3
 import yarl
 
 from flanautils import constants
 from flanautils.exceptions import ResponseError
 from flanautils.models.enums import HTTPMethod
 
 
+def browser_cookies(domain: str, ignore_expired=True) -> list[dict]:
+    cookies = []
+
+    for cookie in browser_cookie3.chrome(domain_name=domain):
+        cookie_vars = vars(cookie)
+        if ignore_expired and 'expires' in cookie_vars and not cookie_vars['expires']:
+            continue
+
+        cookie_dict = {}
+        for k, v in cookie_vars.items():
+            if k.startswith('_'):
+                cookie_dict |= v
+                continue
+
+            if k == 'secure':
+                v = bool(v)
+            cookie_dict[k] = v
+        cookies.append(cookie_dict)
+
+    return cookies
+
+
 async def request(
     http_method: HTTPMethod,
     url: str,
     params: dict = None,
     headers: dict = None,
     data: dict = None,
     session: aiohttp.ClientSession = None,
```

### Comparing `flanautils-1.7.1/flanautils/resources/plotly_es.js` & `flanautils-1.7.2/flanautils/resources/plotly_es.js`

 * *Files identical despite different names*

### Comparing `flanautils-1.7.1/flanautils/strings.py` & `flanautils-1.7.2/flanautils/strings.py`

 * *Files identical despite different names*

### Comparing `flanautils-1.7.1/flanautils.egg-info/PKG-INFO` & `flanautils-1.7.2/flanautils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flanautils
-Version: 1.7.1
+Version: 1.7.2
 Summary: Set of utilities of all kinds to develop python projects.
 Home-page: https://github.com/AlberLC/flanautils
 Author: AlberLC
 Project-URL: Bug Tracker, https://github.com/AlberLC/flanautils/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `flanautils-1.7.1/flanautils.egg-info/SOURCES.txt` & `flanautils-1.7.2/flanautils.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 LICENSE
 README.rst
 pyproject.toml
 setup.cfg
 flanautils/__init__.py
 flanautils/asyncs.py
 flanautils/constants.py
-flanautils/decorators.py
 flanautils/exceptions.py
+flanautils/functions.py
 flanautils/iterables.py
 flanautils/maths.py
 flanautils/medias.py
 flanautils/oss.py
 flanautils/requests.py
 flanautils/strings.py
 flanautils.egg-info/PKG-INFO
```

### Comparing `flanautils-1.7.1/setup.cfg` & `flanautils-1.7.2/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = flanautils
-version = v1.7.1
+version = v1.7.2
 author = AlberLC
 description = Set of utilities of all kinds to develop python projects.
 long_description = file: README.rst
 url = https://github.com/AlberLC/flanautils
 project_urls = 
 	Bug Tracker = https://github.com/AlberLC/flanautils/issues
 classifiers = 
@@ -14,14 +14,16 @@
 
 [options]
 packages = find_namespace:
 include_package_data = True
 python_requires = >=3.10
 install_requires = 
 	aiohttp
+	browser_cookie3
+	jeepney
 	jellyfish
 	pymongo
 	plotly
 	sympy
 	kaleido
 
 [options.packages.find]
```

### Comparing `flanautils-1.7.1/tests/test_utils.py` & `flanautils-1.7.2/tests/test_utils.py`

 * *Files identical despite different names*

