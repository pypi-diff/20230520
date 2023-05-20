# Comparing `tmp/licensio-1.0.0.tar.gz` & `tmp/licensio-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "licensio-1.0.0.tar", max compression
+gzip compressed data, was "licensio-1.1.0.tar", max compression
```

## Comparing `licensio-1.0.0.tar` & `licensio-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1069 2023-05-19 15:22:07.528034 licensio-1.0.0/LICENSE
--rw-r--r--   0        0        0     2880 2023-05-20 07:23:10.837346 licensio-1.0.0/README.md
--rw-r--r--   0        0        0      319 2023-05-19 17:19:45.195455 licensio-1.0.0/licensio/__init__.py
--rw-r--r--   0        0        0     1840 2023-05-19 17:08:02.358905 licensio-1.0.0/licensio/agpl.py
--rw-r--r--   0        0        0     1745 2023-05-19 17:12:35.812943 licensio-1.0.0/licensio/apache.py
--rw-r--r--   0        0        0     2617 2023-05-19 17:13:29.066093 licensio-1.0.0/licensio/bsd.py
--rw-r--r--   0        0        0     1649 2023-05-19 17:08:37.650142 licensio-1.0.0/licensio/cc0.py
--rw-r--r--   0        0        0     2278 2023-05-19 17:14:21.926241 licensio-1.0.0/licensio/epl.py
--rw-r--r--   0        0        0     1754 2023-05-19 17:15:20.515406 licensio-1.0.0/licensio/gnu.py
--rw-r--r--   0        0        0     1837 2023-05-19 17:16:21.369577 licensio-1.0.0/licensio/lgpl.py
--rw-r--r--   0        0        0     2137 2023-05-19 17:10:55.261660 licensio-1.0.0/licensio/mit.py
--rw-r--r--   0        0        0     1556 2023-05-19 17:17:11.396717 licensio-1.0.0/licensio/wtfpl.py
--rw-r--r--   0        0        0      541 2023-05-19 17:28:16.906220 licensio-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3488 1970-01-01 00:00:00.000000 licensio-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-19 15:22:07.528034 licensio-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2900 2023-05-20 08:03:14.778873 licensio-1.1.0/README.md
+-rw-r--r--   0        0        0      319 2023-05-19 17:19:45.195455 licensio-1.1.0/licensio/__init__.py
+-rw-r--r--   0        0        0     1840 2023-05-19 17:08:02.358905 licensio-1.1.0/licensio/agpl.py
+-rw-r--r--   0        0        0     1745 2023-05-19 17:12:35.812943 licensio-1.1.0/licensio/apache.py
+-rw-r--r--   0        0        0     2617 2023-05-19 17:13:29.066093 licensio-1.1.0/licensio/bsd.py
+-rw-r--r--   0        0        0     1649 2023-05-19 17:08:37.650142 licensio-1.1.0/licensio/cc0.py
+-rw-r--r--   0        0        0     2278 2023-05-19 17:14:21.926241 licensio-1.1.0/licensio/epl.py
+-rw-r--r--   0        0        0     1754 2023-05-19 17:15:20.515406 licensio-1.1.0/licensio/gnu.py
+-rw-r--r--   0        0        0     1837 2023-05-19 17:16:21.369577 licensio-1.1.0/licensio/lgpl.py
+-rw-r--r--   0        0        0     2137 2023-05-19 17:10:55.261660 licensio-1.1.0/licensio/mit.py
+-rw-r--r--   0        0        0     1556 2023-05-19 17:17:11.396717 licensio-1.1.0/licensio/wtfpl.py
+-rw-r--r--   0        0        0      541 2023-05-20 08:02:51.744732 licensio-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3508 1970-01-01 00:00:00.000000 licensio-1.1.0/PKG-INFO
```

### Comparing `licensio-1.0.0/LICENSE` & `licensio-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `licensio-1.0.0/README.md` & `licensio-1.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 - DO WHAT THE F*CK YOU WANT TO PUBLIC LICENSE (WTFPL)
 - Creative Commons Zero (CC0)
 
 Each license module provides a function that accepts the year and the name of the person making the dedication and returns the corresponding license statement.
 
 ## Documentation
 
-For detailed documentation, please refer to the [docs](./docs) folder.
+For detailed documentation, please refer to the github repository's [docs](./docs) folder.
 
 The "docs" folder contains individual markdown files for each license module, providing information about the module and usage examples.
 
 
 ## Examples
 For more examples on how to use Licensio, refer to the example code snippets provided in the documentation of each license module.
```

### Comparing `licensio-1.0.0/licensio/agpl.py` & `licensio-1.1.0/licensio/agpl.py`

 * *Files identical despite different names*

### Comparing `licensio-1.0.0/licensio/apache.py` & `licensio-1.1.0/licensio/apache.py`

 * *Files identical despite different names*

### Comparing `licensio-1.0.0/licensio/bsd.py` & `licensio-1.1.0/licensio/bsd.py`

 * *Files identical despite different names*

### Comparing `licensio-1.0.0/licensio/cc0.py` & `licensio-1.1.0/licensio/cc0.py`

 * *Files identical despite different names*

### Comparing `licensio-1.0.0/licensio/epl.py` & `licensio-1.1.0/licensio/epl.py`

 * *Files identical despite different names*

### Comparing `licensio-1.0.0/licensio/gnu.py` & `licensio-1.1.0/licensio/gnu.py`

 * *Files identical despite different names*

### Comparing `licensio-1.0.0/licensio/lgpl.py` & `licensio-1.1.0/licensio/lgpl.py`

 * *Files identical despite different names*

### Comparing `licensio-1.0.0/licensio/mit.py` & `licensio-1.1.0/licensio/mit.py`

 * *Files identical despite different names*

### Comparing `licensio-1.0.0/licensio/wtfpl.py` & `licensio-1.1.0/licensio/wtfpl.py`

 * *Files identical despite different names*

### Comparing `licensio-1.0.0/PKG-INFO` & `licensio-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: licensio
-Version: 1.0.0
+Version: 1.1.0
 Summary: Licensio is a Python library that provides a collection of functions to generate license statements for various open source licenses. It simplifies the process of including license information in your projects by providing ready-to-use license templates.
 License: MIT
 Author: zayedmalick
 Author-email: zayedalmalick@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -53,15 +53,15 @@
 - DO WHAT THE F*CK YOU WANT TO PUBLIC LICENSE (WTFPL)
 - Creative Commons Zero (CC0)
 
 Each license module provides a function that accepts the year and the name of the person making the dedication and returns the corresponding license statement.
 
 ## Documentation
 
-For detailed documentation, please refer to the [docs](./docs) folder.
+For detailed documentation, please refer to the github repository's [docs](./docs) folder.
 
 The "docs" folder contains individual markdown files for each license module, providing information about the module and usage examples.
 
 
 ## Examples
 For more examples on how to use Licensio, refer to the example code snippets provided in the documentation of each license module.
```

