# Comparing `tmp/PyDeepLX-1.0.2.tar.gz` & `tmp/PyDeepLX-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyDeepLX-1.0.2.tar", last modified: Sat May 20 19:55:55 2023, max compression
+gzip compressed data, was "PyDeepLX-1.0.3.tar", last modified: Sat May 20 20:12:20 2023, max compression
```

## Comparing `PyDeepLX-1.0.2.tar` & `PyDeepLX-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-05-20 19:55:55.473302 PyDeepLX-1.0.2/
--rw-r--r--   0 vincent    (501) staff       (20)     1076 2023-04-26 16:41:03.000000 PyDeepLX-1.0.2/LICENSE
--rw-r--r--   0 vincent    (501) staff       (20)     2570 2023-05-20 19:55:55.473083 PyDeepLX-1.0.2/PKG-INFO
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-05-20 19:55:55.472157 PyDeepLX-1.0.2/PyDeepLX/
--rw-r--r--   0 vincent    (501) staff       (20)     3952 2023-05-20 19:50:47.000000 PyDeepLX-1.0.2/PyDeepLX/PyDeepLX.py
--rw-r--r--   0 vincent    (501) staff       (20)      258 2023-04-26 17:58:27.000000 PyDeepLX-1.0.2/PyDeepLX/__init__.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-05-20 19:55:55.472904 PyDeepLX-1.0.2/PyDeepLX.egg-info/
--rw-r--r--   0 vincent    (501) staff       (20)     2570 2023-05-20 19:55:55.000000 PyDeepLX-1.0.2/PyDeepLX.egg-info/PKG-INFO
--rw-r--r--   0 vincent    (501) staff       (20)      258 2023-05-20 19:55:55.000000 PyDeepLX-1.0.2/PyDeepLX.egg-info/SOURCES.txt
--rw-r--r--   0 vincent    (501) staff       (20)        1 2023-05-20 19:55:55.000000 PyDeepLX-1.0.2/PyDeepLX.egg-info/dependency_links.txt
--rw-r--r--   0 vincent    (501) staff       (20)        1 2023-05-20 19:55:24.000000 PyDeepLX-1.0.2/PyDeepLX.egg-info/not-zip-safe
--rw-r--r--   0 vincent    (501) staff       (20)       24 2023-05-20 19:55:55.000000 PyDeepLX-1.0.2/PyDeepLX.egg-info/requires.txt
--rw-r--r--   0 vincent    (501) staff       (20)        9 2023-05-20 19:55:55.000000 PyDeepLX-1.0.2/PyDeepLX.egg-info/top_level.txt
--rw-r--r--   0 vincent    (501) staff       (20)     1512 2023-05-20 19:43:13.000000 PyDeepLX-1.0.2/README.md
--rw-r--r--   0 vincent    (501) staff       (20)       38 2023-05-20 19:55:55.473338 PyDeepLX-1.0.2/setup.cfg
--rw-r--r--   0 vincent    (501) staff       (20)     1628 2023-05-20 19:54:59.000000 PyDeepLX-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:12:20.717016 PyDeepLX-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-20 20:12:06.000000 PyDeepLX-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-20 20:12:20.717016 PyDeepLX-1.0.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:12:20.713016 PyDeepLX-1.0.3/PyDeepLX/
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-05-20 20:12:06.000000 PyDeepLX-1.0.3/PyDeepLX/PyDeepLX.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-20 20:12:06.000000 PyDeepLX-1.0.3/PyDeepLX/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:12:20.717016 PyDeepLX-1.0.3/PyDeepLX.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-20 20:12:20.000000 PyDeepLX-1.0.3/PyDeepLX.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-20 20:12:20.000000 PyDeepLX-1.0.3/PyDeepLX.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 20:12:20.000000 PyDeepLX-1.0.3/PyDeepLX.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 20:12:20.000000 PyDeepLX-1.0.3/PyDeepLX.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-20 20:12:20.000000 PyDeepLX-1.0.3/PyDeepLX.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-20 20:12:20.000000 PyDeepLX-1.0.3/PyDeepLX.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-20 20:12:06.000000 PyDeepLX-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 20:12:20.717016 PyDeepLX-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-20 20:12:06.000000 PyDeepLX-1.0.3/setup.py
```

### Comparing `PyDeepLX-1.0.2/LICENSE` & `PyDeepLX-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PyDeepLX-1.0.2/PKG-INFO` & `PyDeepLX-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyDeepLX
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Python package for unlimited DeepL translation
 Home-page: https://github.com/OwO-Network/PyDeepLX
 Author: missuo
 Author-email: i@yyt.moe
 License: MIT
 Platform: any
 Classifier: Environment :: Web Environment
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyDeepLX Version: 1.0.2 Summary: A Python package
+Metadata-Version: 2.1 Name: PyDeepLX Version: 1.0.3 Summary: A Python package
 for unlimited DeepL translation Home-page: https://github.com/OwO-Network/
 PyDeepLX Author: missuo Author-email: i@yyt.moe License: MIT Platform: any
 Classifier: Environment :: Web Environment Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.3 Classifier: Programming
 Language :: Python :: 3.4 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `PyDeepLX-1.0.2/PyDeepLX/PyDeepLX.py` & `PyDeepLX-1.0.3/PyDeepLX/PyDeepLX.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 Author: Vincent Young
 Date: 2023-04-27 00:44:01
 LastEditors: Vincent Young
-LastEditTime: 2023-05-21 03:50:47
+LastEditTime: 2023-05-21 03:58:18
 FilePath: /PyDeepLX/PyDeepLX/PyDeepLX.py
 Telegram: https://t.me/missuo
 
 Copyright © 2023 by Vincent, All Rights Reserved. 
 '''
 import random
 import time
@@ -93,15 +93,15 @@
     if (id+5) % 29 == 0 or (id+3) % 13 == 0:
         postDataStr = postDataStr.replace(
             "\"method\":\"", "\"method\" : \"", -1)
     else:
         postDataStr = postDataStr.replace(
             "\"method\":\"", "\"method\": \"", -1)
         
-    # Add proxy (e.g. proxies='socks5://127.0.0.1:9150')
+    # Add proxy (e.g. proxies='socks5://127.0.0.1:7890')
     with httpx.Client(proxies=proxies) as client:
         resp = client.post(url=deeplAPI, data=postDataStr, headers=headers)
         respStatusCode = resp.status_code
         respText = resp.text
         respJson = json.loads(respText)
         targetTextArray = []
         if respStatusCode == 200:
```

### Comparing `PyDeepLX-1.0.2/PyDeepLX.egg-info/PKG-INFO` & `PyDeepLX-1.0.3/PyDeepLX.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyDeepLX
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Python package for unlimited DeepL translation
 Home-page: https://github.com/OwO-Network/PyDeepLX
 Author: missuo
 Author-email: i@yyt.moe
 License: MIT
 Platform: any
 Classifier: Environment :: Web Environment
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyDeepLX Version: 1.0.2 Summary: A Python package
+Metadata-Version: 2.1 Name: PyDeepLX Version: 1.0.3 Summary: A Python package
 for unlimited DeepL translation Home-page: https://github.com/OwO-Network/
 PyDeepLX Author: missuo Author-email: i@yyt.moe License: MIT Platform: any
 Classifier: Environment :: Web Environment Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.3 Classifier: Programming
 Language :: Python :: 3.4 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `PyDeepLX-1.0.2/README.md` & `PyDeepLX-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `PyDeepLX-1.0.2/setup.py` & `PyDeepLX-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 '''
 Author: Vincent Young
 Date: 2023-04-27 00:42:10
 LastEditors: Vincent Young
-LastEditTime: 2023-05-21 03:54:59
+LastEditTime: 2023-05-21 04:10:41
 FilePath: /PyDeepLX/setup.py
 Telegram: https://t.me/missuo
 
 Copyright © 2023 by Vincent, All Rights Reserved. 
 '''
 from setuptools import setup, find_packages
 
 with open("README.md","r") as fh:
     long_description = fh.read()
 
 setup(
     name="PyDeepLX",
     author="missuo",
-    version="1.0.2",
+    version="1.0.3",
     license='MIT',
     long_description= long_description,
     long_description_content_type="text/markdown",
     author_email="i@yyt.moe",
     description="A Python package for unlimited DeepL translation",
     url='https://github.com/OwO-Network/PyDeepLX',
     packages=find_packages(),
```

