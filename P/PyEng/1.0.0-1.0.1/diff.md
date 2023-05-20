# Comparing `tmp/PyEng-1.0.0.tar.gz` & `tmp/PyEng-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyEng-1.0.0.tar", last modified: Sat May 20 14:19:37 2023, max compression
+gzip compressed data, was "PyEng-1.0.1.tar", last modified: Sat May 20 15:26:04 2023, max compression
```

## Comparing `PyEng-1.0.0.tar` & `PyEng-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 14:19:37.055426 PyEng-1.0.0/
--rw-rw-rw-   0        0        0     1091 2023-05-16 07:22:16.000000 PyEng-1.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0       76 2023-05-20 14:00:41.000000 PyEng-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2475 2023-05-20 14:19:37.054392 PyEng-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-20 14:19:36.991560 PyEng-1.0.0/PyEng/
--rw-rw-rw-   0        0        0     1624 2023-05-20 14:16:55.000000 PyEng-1.0.0/PyEng/Words.py
--rw-rw-rw-   0        0        0       55 2023-05-20 14:01:19.000000 PyEng-1.0.0/PyEng/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-20 14:19:37.002567 PyEng-1.0.0/PyEng/data/
--rw-rw-rw-   0        0        0 22970019 2023-05-20 13:53:02.000000 PyEng-1.0.0/PyEng/data/dictionary.json
-drwxrwxrwx   0        0        0        0 2023-05-20 14:19:37.000623 PyEng-1.0.0/PyEng.egg-info/
--rw-rw-rw-   0        0        0     2475 2023-05-20 14:19:36.000000 PyEng-1.0.0/PyEng.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2023-05-20 14:19:36.000000 PyEng-1.0.0/PyEng.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 14:19:36.000000 PyEng-1.0.0/PyEng.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-20 14:19:36.000000 PyEng-1.0.0/PyEng.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2003 2023-05-20 13:46:17.000000 PyEng-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-20 14:19:37.056388 PyEng-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      854 2023-05-20 13:44:47.000000 PyEng-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 15:26:04.727933 PyEng-1.0.1/
+-rw-rw-rw-   0        0        0     1091 2023-05-16 07:22:16.000000 PyEng-1.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       76 2023-05-20 14:00:41.000000 PyEng-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2475 2023-05-20 15:26:04.726936 PyEng-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-20 15:26:04.653131 PyEng-1.0.1/PyEng/
+-rw-rw-rw-   0        0        0     1669 2023-05-20 14:36:30.000000 PyEng-1.0.1/PyEng/Words.py
+-rw-rw-rw-   0        0        0       55 2023-05-20 14:01:19.000000 PyEng-1.0.1/PyEng/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-20 15:26:04.668093 PyEng-1.0.1/PyEng/data/
+-rw-rw-rw-   0        0        0 22970019 2023-05-20 13:53:02.000000 PyEng-1.0.1/PyEng/data/dictionary.json
+drwxrwxrwx   0        0        0        0 2023-05-20 15:26:04.666098 PyEng-1.0.1/PyEng.egg-info/
+-rw-rw-rw-   0        0        0     2475 2023-05-20 15:26:04.000000 PyEng-1.0.1/PyEng.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2023-05-20 15:26:04.000000 PyEng-1.0.1/PyEng.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 15:26:04.000000 PyEng-1.0.1/PyEng.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-20 15:26:04.000000 PyEng-1.0.1/PyEng.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2003 2023-05-20 15:24:53.000000 PyEng-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-20 15:26:04.728929 PyEng-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      854 2023-05-20 15:24:56.000000 PyEng-1.0.1/setup.py
```

### Comparing `PyEng-1.0.0/LICENSE.txt` & `PyEng-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyEng-1.0.0/PKG-INFO` & `PyEng-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyEng
-Version: 1.0.0
+Version: 1.0.1
 Summary: PyEng is a general-purpose Python module that contains functions related to the English language.
 Home-page: https://github.com/Anikethc/PyEng
 Download-URL: https://pypi.org/project/PyEng
 Author: Aniketh Chavare
 Author-email: anikethchavare@outlook.com
 License: MIT
 Keywords: English
@@ -18,15 +18,15 @@
 PyEng is a general-purpose Python module that contains functions related to the English language.
 
 Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pyeng-docs).
 
 ## Module Information
 
 **Name** - PyEng</br>
-**Version** - 1.0.0</br>
+**Version** - 1.0.1</br>
 **Description** - PyEng is a general-purpose Python module that contains functions related to the English language.</br>
 **Author** - Aniketh Chavare</br>
 **GitHub URL** - [https://github.com/Anikethc/PyEng](https://github.com/Anikethc/PyEng)</br>
 **Pypi.org URL** - [https://pypi.org/project/PyEng](https://pypi.org/project/PyEng)</br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pyeng-docs](https://aniketh-chavare.gitbook.io/pyeng-docs)
 
 ## License
```

### Comparing `PyEng-1.0.0/PyEng/Words.py` & `PyEng-1.0.1/PyEng/Words.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # PyEng - Words
 
+''' This is the "Words" sub-module. '''
+
 # Imports
 import os
 from difflib import get_close_matches
 import json
 
 # Set Directory
 directory = os.path.dirname(os.path.realpath(__file__))
@@ -43,8 +45,8 @@
 
         # Check if Anagram
         if (lengthOfStrings(string1, string2) and sortStrings(string1, string2)):
             return True
         else:
             return False
     else:
-        raise Exception("The 'string1' and 'string2' arguments must be a string.")
+        raise Exception("The 'string1' and 'string2' arguments must be a string.")
```

### Comparing `PyEng-1.0.0/PyEng/data/dictionary.json` & `PyEng-1.0.1/PyEng/data/dictionary.json`

 * *Files identical despite different names*

### Comparing `PyEng-1.0.0/PyEng.egg-info/PKG-INFO` & `PyEng-1.0.1/PyEng.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyEng
-Version: 1.0.0
+Version: 1.0.1
 Summary: PyEng is a general-purpose Python module that contains functions related to the English language.
 Home-page: https://github.com/Anikethc/PyEng
 Download-URL: https://pypi.org/project/PyEng
 Author: Aniketh Chavare
 Author-email: anikethchavare@outlook.com
 License: MIT
 Keywords: English
@@ -18,15 +18,15 @@
 PyEng is a general-purpose Python module that contains functions related to the English language.
 
 Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pyeng-docs).
 
 ## Module Information
 
 **Name** - PyEng</br>
-**Version** - 1.0.0</br>
+**Version** - 1.0.1</br>
 **Description** - PyEng is a general-purpose Python module that contains functions related to the English language.</br>
 **Author** - Aniketh Chavare</br>
 **GitHub URL** - [https://github.com/Anikethc/PyEng](https://github.com/Anikethc/PyEng)</br>
 **Pypi.org URL** - [https://pypi.org/project/PyEng](https://pypi.org/project/PyEng)</br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pyeng-docs](https://aniketh-chavare.gitbook.io/pyeng-docs)
 
 ## License
```

### Comparing `PyEng-1.0.0/README.md` & `PyEng-1.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 PyEng is a general-purpose Python module that contains functions related to the English language.
 
 Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pyeng-docs).
 
 ## Module Information
 
 **Name** - PyEng</br>
-**Version** - 1.0.0</br>
+**Version** - 1.0.1</br>
 **Description** - PyEng is a general-purpose Python module that contains functions related to the English language.</br>
 **Author** - Aniketh Chavare</br>
 **GitHub URL** - [https://github.com/Anikethc/PyEng](https://github.com/Anikethc/PyEng)</br>
 **Pypi.org URL** - [https://pypi.org/project/PyEng](https://pypi.org/project/PyEng)</br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pyeng-docs](https://aniketh-chavare.gitbook.io/pyeng-docs)
 
 ## License
```

### Comparing `PyEng-1.0.0/setup.py` & `PyEng-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # README.md
 with open("README.md") as readme_file:
     README = readme_file.read()
 
 # Setup Arguements
 setup_args = dict (
     name="PyEng",
-    version="1.0.0",
+    version="1.0.1",
     description="PyEng is a general-purpose Python module that contains functions related to the English language.",
     long_description_content_type="text/markdown",
     long_description=README,
     license="MIT",
     packages=find_packages(),
     include_package_data=True,
     author="Aniketh Chavare",
```

