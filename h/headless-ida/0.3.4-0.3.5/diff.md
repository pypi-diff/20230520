# Comparing `tmp/headless-ida-0.3.4.tar.gz` & `tmp/headless-ida-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "headless-ida-0.3.4.tar", last modified: Fri Mar 31 07:27:29 2023, max compression
+gzip compressed data, was "headless-ida-0.3.5.tar", last modified: Sat May 20 06:01:18 2023, max compression
```

## Comparing `headless-ida-0.3.4.tar` & `headless-ida-0.3.5.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 07:27:29.387660 headless-ida-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-03-31 07:27:20.000000 headless-ida-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-03-31 07:27:29.387660 headless-ida-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-03-31 07:27:20.000000 headless-ida-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 07:27:29.387660 headless-ida-0.3.4/headless_ida/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-31 07:27:20.000000 headless-ida-0.3.4/headless_ida/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-03-31 07:27:20.000000 headless-ida-0.3.4/headless_ida/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-03-31 07:27:20.000000 headless-ida-0.3.4/headless_ida/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-03-31 07:27:20.000000 headless-ida-0.3.4/headless_ida/ida_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-03-31 07:27:20.000000 headless-ida-0.3.4/headless_ida/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 07:27:29.387660 headless-ida-0.3.4/headless_ida.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-03-31 07:27:29.000000 headless-ida-0.3.4/headless_ida.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-03-31 07:27:29.000000 headless-ida-0.3.4/headless_ida.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 07:27:29.000000 headless-ida-0.3.4/headless_ida.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-03-31 07:27:29.000000 headless-ida-0.3.4/headless_ida.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-31 07:27:29.000000 headless-ida-0.3.4/headless_ida.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-31 07:27:29.000000 headless-ida-0.3.4/headless_ida.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-03-31 07:27:22.000000 headless-ida-0.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 07:27:29.387660 headless-ida-0.3.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:01:18.669571 headless-ida-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-20 06:01:08.000000 headless-ida-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-05-20 06:01:18.669571 headless-ida-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-05-20 06:01:08.000000 headless-ida-0.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:01:18.669571 headless-ida-0.3.5/headless_ida/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-20 06:01:08.000000 headless-ida-0.3.5/headless_ida/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-20 06:01:08.000000 headless-ida-0.3.5/headless_ida/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-05-20 06:01:08.000000 headless-ida-0.3.5/headless_ida/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-20 06:01:08.000000 headless-ida-0.3.5/headless_ida/ida_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-20 06:01:08.000000 headless-ida-0.3.5/headless_ida/ida_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-05-20 06:01:08.000000 headless-ida-0.3.5/headless_ida/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:01:18.669571 headless-ida-0.3.5/headless_ida.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-05-20 06:01:18.000000 headless-ida-0.3.5/headless_ida.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-20 06:01:18.000000 headless-ida-0.3.5/headless_ida.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 06:01:18.000000 headless-ida-0.3.5/headless_ida.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-20 06:01:18.000000 headless-ida-0.3.5/headless_ida.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-20 06:01:18.000000 headless-ida-0.3.5/headless_ida.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-20 06:01:18.000000 headless-ida-0.3.5/headless_ida.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-20 06:01:10.000000 headless-ida-0.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 06:01:18.669571 headless-ida-0.3.5/setup.cfg
```

### Comparing `headless-ida-0.3.4/LICENSE` & `headless-ida-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `headless-ida-0.3.4/PKG-INFO` & `headless-ida-0.3.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: headless-ida
-Version: 0.3.4
+Version: 0.3.5
 Summary: Headless IDA
 Author-email: Han Dai <pypi@han.do>
 License: MIT License
         
         Copyright (c) 2023 Han Dai
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -55,14 +55,17 @@
 from headless_ida import HeadlessIda
 headlessida = HeadlessIda("/path/to/idat64", "/path/to/binary")
 
 # Import IDA Modules (make sure you have initialized HeadlessIda first)
 import idautils
 import ida_name
 
+# Or Import All IDA Modules at Once (idaapi is not imported by default)
+# from headless_ida.ida_headers import *
+
 # Have Fun
 for func in idautils.Functions():
     print(f"{hex(func)} {ida_name.get_ea_name(func)}")
 ```
 
 ### Use it as a command line tool.
 ```bash
@@ -122,8 +125,9 @@
 # One-liner
 $ headless-ida localhost:1337 /path/to/local/binary -c "import idautils; print(list(idautils.Functions())[0:10])"
 ```
 
 
 # Resources
 - [Headless IDA Examples](https://github.com/DennyDai/headless-ida/tree/main/examples)
-- [IDAPython Documentation](https://www.hex-rays.com/products/ida/support/idapython_docs/)
+- [IDAPython Official Documentation](https://www.hex-rays.com/products/ida/support/idapython_docs/)
+- [IDAPython Official Examples](https://github.com/idapython/src/tree/master/examples)
```

### Comparing `headless-ida-0.3.4/README.md` & `headless-ida-0.3.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,17 @@
 from headless_ida import HeadlessIda
 headlessida = HeadlessIda("/path/to/idat64", "/path/to/binary")
 
 # Import IDA Modules (make sure you have initialized HeadlessIda first)
 import idautils
 import ida_name
 
+# Or Import All IDA Modules at Once (idaapi is not imported by default)
+# from headless_ida.ida_headers import *
+
 # Have Fun
 for func in idautils.Functions():
     print(f"{hex(func)} {ida_name.get_ea_name(func)}")
 ```
 
 ### Use it as a command line tool.
 ```bash
@@ -87,8 +90,9 @@
 # One-liner
 $ headless-ida localhost:1337 /path/to/local/binary -c "import idautils; print(list(idautils.Functions())[0:10])"
 ```
 
 
 # Resources
 - [Headless IDA Examples](https://github.com/DennyDai/headless-ida/tree/main/examples)
-- [IDAPython Documentation](https://www.hex-rays.com/products/ida/support/idapython_docs/)
+- [IDAPython Official Documentation](https://www.hex-rays.com/products/ida/support/idapython_docs/)
+- [IDAPython Official Examples](https://github.com/idapython/src/tree/master/examples)
```

### Comparing `headless-ida-0.3.4/headless_ida/cli.py` & `headless-ida-0.3.5/headless_ida/cli.py`

 * *Files identical despite different names*

### Comparing `headless-ida-0.3.4/headless_ida/client.py` & `headless-ida-0.3.5/headless_ida/client.py`

 * *Files identical despite different names*

### Comparing `headless-ida-0.3.4/headless_ida/ida_script.py` & `headless-ida-0.3.5/headless_ida/ida_script.py`

 * *Files identical despite different names*

### Comparing `headless-ida-0.3.4/headless_ida/server.py` & `headless-ida-0.3.5/headless_ida/server.py`

 * *Files identical despite different names*

### Comparing `headless-ida-0.3.4/headless_ida.egg-info/PKG-INFO` & `headless-ida-0.3.5/headless_ida.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: headless-ida
-Version: 0.3.4
+Version: 0.3.5
 Summary: Headless IDA
 Author-email: Han Dai <pypi@han.do>
 License: MIT License
         
         Copyright (c) 2023 Han Dai
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -55,14 +55,17 @@
 from headless_ida import HeadlessIda
 headlessida = HeadlessIda("/path/to/idat64", "/path/to/binary")
 
 # Import IDA Modules (make sure you have initialized HeadlessIda first)
 import idautils
 import ida_name
 
+# Or Import All IDA Modules at Once (idaapi is not imported by default)
+# from headless_ida.ida_headers import *
+
 # Have Fun
 for func in idautils.Functions():
     print(f"{hex(func)} {ida_name.get_ea_name(func)}")
 ```
 
 ### Use it as a command line tool.
 ```bash
@@ -122,8 +125,9 @@
 # One-liner
 $ headless-ida localhost:1337 /path/to/local/binary -c "import idautils; print(list(idautils.Functions())[0:10])"
 ```
 
 
 # Resources
 - [Headless IDA Examples](https://github.com/DennyDai/headless-ida/tree/main/examples)
-- [IDAPython Documentation](https://www.hex-rays.com/products/ida/support/idapython_docs/)
+- [IDAPython Official Documentation](https://www.hex-rays.com/products/ida/support/idapython_docs/)
+- [IDAPython Official Examples](https://github.com/idapython/src/tree/master/examples)
```

### Comparing `headless-ida-0.3.4/pyproject.toml` & `headless-ida-0.3.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "headless-ida"
-version = "0.3.4"
+version = "0.3.5"
 dependencies = [
     "rpyc",
 ]
 readme = "README.md"
 description = "Headless IDA"
 authors = [
     {name = "Han Dai", email = "pypi@han.do"},
```

