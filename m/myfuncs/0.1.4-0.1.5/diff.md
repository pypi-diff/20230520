# Comparing `tmp/myfuncs-0.1.4.tar.gz` & `tmp/myfuncs-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myfuncs-0.1.4.tar", last modified: Sat May 13 21:11:12 2023, max compression
+gzip compressed data, was "myfuncs-0.1.5.tar", last modified: Sat May 20 07:17:39 2023, max compression
```

## Comparing `myfuncs-0.1.4.tar` & `myfuncs-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 work       (501) staff       (20)        0 2023-05-13 21:11:12.466416 myfuncs-0.1.4/
--rw-r--r--   0 work       (501) staff       (20)     1068 2023-05-13 16:42:37.000000 myfuncs-0.1.4/LICENSE
--rw-r--r--   0 work       (501) staff       (20)     2426 2023-05-13 21:11:12.466290 myfuncs-0.1.4/PKG-INFO
--rw-r--r--   0 work       (501) staff       (20)     1687 2023-05-13 21:07:45.000000 myfuncs-0.1.4/README.md
-drwxr-xr-x   0 work       (501) staff       (20)        0 2023-05-13 21:11:12.465480 myfuncs-0.1.4/myfuncs/
--rw-r--r--   0 work       (501) staff       (20)       21 2023-05-13 18:23:34.000000 myfuncs-0.1.4/myfuncs/__init__.py
--rw-r--r--   0 work       (501) staff       (20)     3349 2023-05-13 19:26:19.000000 myfuncs-0.1.4/myfuncs/funcs.py
-drwxr-xr-x   0 work       (501) staff       (20)        0 2023-05-13 21:11:12.466129 myfuncs-0.1.4/myfuncs.egg-info/
--rw-r--r--   0 work       (501) staff       (20)     2426 2023-05-13 21:11:12.000000 myfuncs-0.1.4/myfuncs.egg-info/PKG-INFO
--rw-r--r--   0 work       (501) staff       (20)      187 2023-05-13 21:11:12.000000 myfuncs-0.1.4/myfuncs.egg-info/SOURCES.txt
--rw-r--r--   0 work       (501) staff       (20)        1 2023-05-13 21:11:12.000000 myfuncs-0.1.4/myfuncs.egg-info/dependency_links.txt
--rw-r--r--   0 work       (501) staff       (20)        8 2023-05-13 21:11:12.000000 myfuncs-0.1.4/myfuncs.egg-info/top_level.txt
--rw-r--r--   0 work       (501) staff       (20)       38 2023-05-13 21:11:12.466457 myfuncs-0.1.4/setup.cfg
--rw-r--r--   0 work       (501) staff       (20)      916 2023-05-13 21:09:15.000000 myfuncs-0.1.4/setup.py
+drwxr-xr-x   0 work       (501) staff       (20)        0 2023-05-20 07:17:39.652139 myfuncs-0.1.5/
+-rw-r--r--   0 work       (501) staff       (20)     1068 2023-05-13 16:42:37.000000 myfuncs-0.1.5/LICENSE
+-rw-r--r--   0 work       (501) staff       (20)     2426 2023-05-20 07:17:39.651967 myfuncs-0.1.5/PKG-INFO
+-rw-r--r--   0 work       (501) staff       (20)     1687 2023-05-13 21:07:45.000000 myfuncs-0.1.5/README.md
+drwxr-xr-x   0 work       (501) staff       (20)        0 2023-05-20 07:17:39.651270 myfuncs-0.1.5/myfuncs/
+-rw-r--r--   0 work       (501) staff       (20)       21 2023-05-13 18:23:34.000000 myfuncs-0.1.5/myfuncs/__init__.py
+-rw-r--r--   0 work       (501) staff       (20)     3891 2023-05-20 03:36:35.000000 myfuncs-0.1.5/myfuncs/funcs.py
+drwxr-xr-x   0 work       (501) staff       (20)        0 2023-05-20 07:17:39.651776 myfuncs-0.1.5/myfuncs.egg-info/
+-rw-r--r--   0 work       (501) staff       (20)     2426 2023-05-20 07:17:39.000000 myfuncs-0.1.5/myfuncs.egg-info/PKG-INFO
+-rw-r--r--   0 work       (501) staff       (20)      187 2023-05-20 07:17:39.000000 myfuncs-0.1.5/myfuncs.egg-info/SOURCES.txt
+-rw-r--r--   0 work       (501) staff       (20)        1 2023-05-20 07:17:39.000000 myfuncs-0.1.5/myfuncs.egg-info/dependency_links.txt
+-rw-r--r--   0 work       (501) staff       (20)        8 2023-05-20 07:17:39.000000 myfuncs-0.1.5/myfuncs.egg-info/top_level.txt
+-rw-r--r--   0 work       (501) staff       (20)       38 2023-05-20 07:17:39.652180 myfuncs-0.1.5/setup.cfg
+-rw-r--r--   0 work       (501) staff       (20)      916 2023-05-20 07:17:18.000000 myfuncs-0.1.5/setup.py
```

### Comparing `myfuncs-0.1.4/LICENSE` & `myfuncs-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `myfuncs-0.1.4/PKG-INFO` & `myfuncs-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfuncs
-Version: 0.1.4
+Version: 0.1.5
 Summary: Personal utility functions that I use across different codebases.
 Home-page: https://github.com/cc-d/myfuncs
 Author: Cary Carter
 Author-email: ccarterdev@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `myfuncs-0.1.4/README.md` & `myfuncs-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `myfuncs-0.1.4/myfuncs/funcs.py` & `myfuncs-0.1.5/myfuncs/funcs.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,40 +9,47 @@
 import logging
 
 logger = logging.getLogger(__name__)
 
 T = TypeVar("T", bound=Callable[..., Any])
 
 
-def get_asctime() -> str:
-    """Returns the current time in the same format as logging %(asctime)s
+def trunc_str(string: str, max_length: int) -> str:
+    """
+    Truncates a string if its length exceeds the specified maximum length.
+    If the string is truncated, it appends '...' to indicate the truncation.
 
+    Args:
+        string (str): The string to truncate.
+        max_length (int): The maximum length of the truncated string.
 
     Returns:
-        str: current asctime
+        str: The truncated string.
     """
-    now = datetime.now()
-    return now.strftime(f"%Y-%m-%d %H:%M:%S")
+    if len(string) > max_length:
+        return string[:max_length - 3] + "..."
+    return string
+
 
 def logf(
     level: Optional[Union[int, str]] = logging.DEBUG,
     log_args: bool = True,
     log_return: bool = True,
-    max_vlen: int = 1000,
+    max_str_len: int = 1000,
     measure_time: bool = True
 ) -> Callable[[T], T]:
     """
     A decorator that logs the execution time, function name, arguments, keyword arguments,
     and return value of a function using a specified log level.
 
     Args:
         level (Union[int, str], optional): The log level to use for logging. Defaults to logging.DEBUG.
         log_args (bool, optional): Should the function arguments be logged? Defaults to True.
         log_return (bool, optional): Should function return be logged? Defaults to True.
-        max_vlen (int, optional): Maximum length of the logged arguments and return values. Defaults to 1000.
+        max_str_len (int, optional): Maximum length of the logged arguments and return values. Defaults to 1000.
         measure_time (bool, optional): Should the function execution time be measured? Defaults to True.
 
     Returns:
         Callable[[T], T]: The wrapped function.
     """
     if isinstance(level, str):
         level_int = logging.getLevelName(level.upper())
@@ -53,15 +60,15 @@
         @wraps(func)
         def wrapper(*args: Any, **kwargs: Any) -> Any:
             # Start the timer if required and execute the function.
             start_time = time.time() if measure_time else None
 
             # Log function arguments if required
             if log_args:
-                arg_str = f"{func.__name__}() | {str(args)[:max_vlen]} {str(kwargs)[:max_vlen]}"
+                arg_str = f"{func.__name__}() | {str(args)[:max_str_len]} {str(kwargs)[:max_str_len]}"
             else:
                 arg_str = f"{func.__name__}()"
 
             logger.log(level_int, arg_str)
 
             # Execute the function
             result = func(*args, **kwargs)
@@ -70,31 +77,42 @@
                 end_time = time.time()
                 # Calculate the execution time and format the log message.
                 exec_time = end_time - start_time
                 exec_time_str = f"{exec_time:.5f}s"
 
             # Log the return value and execution time if required
             if log_return and measure_time:
-                result_str = str(result)[:max_vlen]
+                result_str = trunc_str(str(result), max_str_len)
                 log_message = f"{func.__name__}() {exec_time_str} | {result_str}"
             elif log_return:
-                result_str = str(result)[:max_vlen]
+                result_str = trunc_str(str(result), max_str_len)
                 log_message = f"{func.__name__}() | {result_str}"
             elif measure_time:
                 log_message = f"{func.__name__}() {exec_time_str}"
             else:
                 log_message = None
 
             if log_message is not None:
                 # Log the message using the specified level.
                 logger.log(level_int, log_message)
 
             return result
         return wrapper
     return decorator
 
+@logf()
+def get_asctime() -> str:
+    """Returns the current time in the same format as logging %(asctime)s
+
+
+    Returns:
+        str: current asctime
+    """
+    now = datetime.now()
+    return now.strftime(f"%Y-%m-%d %H:%M:%S")
+
 
 @logf()
 def valid_uuid(string):
     regex = re.compile(
         r'^[0-9a-f]{8}-[0-9a-f]{4}-[1-5][0-9a-f]{3}-[0-9a-f]{4}-[0-9a-f]{12}$')
     return bool(regex.match(string))
```

### Comparing `myfuncs-0.1.4/myfuncs.egg-info/PKG-INFO` & `myfuncs-0.1.5/myfuncs.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfuncs
-Version: 0.1.4
+Version: 0.1.5
 Summary: Personal utility functions that I use across different codebases.
 Home-page: https://github.com/cc-d/myfuncs
 Author: Cary Carter
 Author-email: ccarterdev@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `myfuncs-0.1.4/setup.py` & `myfuncs-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfuncs',
-    version='0.1.4',
+    version='0.1.5',
     packages=find_packages(),
     install_requires=[],
     author='Cary Carter',
     author_email='ccarterdev@gmail.com',
     description='Personal utility functions that I use across different codebases.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

