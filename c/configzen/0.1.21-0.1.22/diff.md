# Comparing `tmp/configzen-0.1.21.tar.gz` & `tmp/configzen-0.1.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configzen-0.1.21.tar", max compression
+gzip compressed data, was "configzen-0.1.22.tar", max compression
```

## Comparing `configzen-0.1.21.tar` & `configzen-0.1.22.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      216 2023-05-17 21:14:40.122071 configzen-0.1.21/configzen/__init__.py
--rw-r--r--   0        0        0      904 2023-05-19 14:41:10.408896 configzen-0.1.21/configzen/__main__.py
--rw-r--r--   0        0        0    52979 2023-05-19 22:51:22.835958 configzen-0.1.21/configzen/config.py
--rw-r--r--   0        0        0     2470 2023-05-19 16:49:24.141768 configzen-0.1.21/configzen/errors.py
--rw-r--r--   0        0        0    18794 2023-05-19 22:51:21.557867 configzen-0.1.21/configzen/processor.py
--rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.1.21/configzen/py.typed
--rw-r--r--   0        0        0      777 2023-05-19 17:03:50.493938 configzen-0.1.21/configzen/typedefs.py
--rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.1.21/LICENSE
--rw-r--r--   0        0        0     1687 2023-05-19 22:49:39.596706 configzen-0.1.21/pyproject.toml
--rw-r--r--   0        0        0     7150 2023-05-19 22:44:45.534902 configzen-0.1.21/README.md
--rw-r--r--   0        0        0     7841 1970-01-01 00:00:00.000000 configzen-0.1.21/PKG-INFO
+-rw-r--r--   0        0        0      216 2023-05-17 21:14:40.122071 configzen-0.1.22/configzen/__init__.py
+-rw-r--r--   0        0        0      904 2023-05-19 14:41:10.408896 configzen-0.1.22/configzen/__main__.py
+-rw-r--r--   0        0        0    52979 2023-05-19 22:51:22.835958 configzen-0.1.22/configzen/config.py
+-rw-r--r--   0        0        0     2470 2023-05-19 16:49:24.141768 configzen-0.1.22/configzen/errors.py
+-rw-r--r--   0        0        0    18850 2023-05-19 22:54:26.664063 configzen-0.1.22/configzen/processor.py
+-rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.1.22/configzen/py.typed
+-rw-r--r--   0        0        0      777 2023-05-19 17:03:50.493938 configzen-0.1.22/configzen/typedefs.py
+-rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.1.22/LICENSE
+-rw-r--r--   0        0        0     1687 2023-05-19 22:54:47.228053 configzen-0.1.22/pyproject.toml
+-rw-r--r--   0        0        0     7150 2023-05-19 22:44:45.534902 configzen-0.1.22/README.md
+-rw-r--r--   0        0        0     7841 1970-01-01 00:00:00.000000 configzen-0.1.22/PKG-INFO
```

### Comparing `configzen-0.1.21/configzen/__main__.py` & `configzen-0.1.22/configzen/__main__.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.21/configzen/config.py` & `configzen-0.1.22/configzen/config.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.21/configzen/errors.py` & `configzen-0.1.22/configzen/errors.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.21/configzen/processor.py` & `configzen-0.1.22/configzen/processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -631,10 +631,13 @@
                 if counterpart_value != value:
                     overrides[key] = counterpart_value
                     del substituted_values[key]
 
         if substituted_values:
             arguments = [] if route is None else [route]
             substitution_directive = cls.directive(Directives.EXTEND, arguments)
-            state |= {substitution_directive: context.loader.resource}
+            state |= (
+                {substitution_directive: context.loader.resource}
+                | state
+            )
 
         state |= overrides
```

### Comparing `configzen-0.1.21/configzen/typedefs.py` & `configzen-0.1.22/configzen/typedefs.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.21/LICENSE` & `configzen-0.1.22/LICENSE`

 * *Files identical despite different names*

### Comparing `configzen-0.1.21/pyproject.toml` & `configzen-0.1.22/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "configzen"
-version = "0.1.21"
+version = "0.1.22"
 description = "The easiest way to manage configuration files in Python"
 authors = ["bswck <bswck.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `configzen-0.1.21/README.md` & `configzen-0.1.22/README.md`

 * *Files identical despite different names*

### Comparing `configzen-0.1.21/PKG-INFO` & `configzen-0.1.22/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configzen
-Version: 0.1.21
+Version: 0.1.22
 Summary: The easiest way to manage configuration files in Python
 License: MIT
 Author: bswck
 Author-email: bswck.dev@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

