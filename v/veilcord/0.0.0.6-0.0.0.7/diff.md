# Comparing `tmp/veilcord-0.0.0.6.tar.gz` & `tmp/veilcord-0.0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "veilcord-0.0.0.6.tar", last modified: Sat May 20 00:13:37 2023, max compression
+gzip compressed data, was "veilcord-0.0.0.7.tar", last modified: Sat May 20 00:35:36 2023, max compression
```

## Comparing `veilcord-0.0.0.6.tar` & `veilcord-0.0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 00:13:37.198341 veilcord-0.0.0.6/
--rw-rw-rw-   0        0        0     1085 2023-05-08 01:47:46.000000 veilcord-0.0.0.6/LICENSE
--rw-rw-rw-   0        0        0     2614 2023-05-20 00:13:37.198341 veilcord-0.0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1436 2023-05-19 23:47:05.000000 veilcord-0.0.0.6/README.md
--rw-rw-rw-   0        0        0       86 2023-05-08 02:01:12.000000 veilcord-0.0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-20 00:13:37.198341 veilcord-0.0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1603 2023-05-19 23:50:54.000000 veilcord-0.0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-20 00:13:37.184870 veilcord-0.0.0.6/veilcord/
--rw-rw-rw-   0        0        0    13990 2023-05-20 00:06:07.000000 veilcord-0.0.0.6/veilcord/__init__.py
--rw-rw-rw-   0        0        0    10385 2023-05-20 00:12:31.000000 veilcord-0.0.0.6/veilcord/verification.py
-drwxrwxrwx   0        0        0        0 2023-05-20 00:13:37.197343 veilcord-0.0.0.6/veilcord.egg-info/
--rw-rw-rw-   0        0        0     2614 2023-05-20 00:13:37.000000 veilcord-0.0.0.6/veilcord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2023-05-20 00:13:37.000000 veilcord-0.0.0.6/veilcord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 00:13:37.000000 veilcord-0.0.0.6/veilcord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-05-20 00:13:37.000000 veilcord-0.0.0.6/veilcord.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-20 00:13:37.000000 veilcord-0.0.0.6/veilcord.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-20 00:35:36.892375 veilcord-0.0.0.7/
+-rw-rw-rw-   0        0        0     1085 2023-05-08 01:47:46.000000 veilcord-0.0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     2614 2023-05-20 00:35:36.892375 veilcord-0.0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1436 2023-05-19 23:47:05.000000 veilcord-0.0.0.7/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-08 02:01:12.000000 veilcord-0.0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-20 00:35:36.892375 veilcord-0.0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1603 2023-05-20 00:34:59.000000 veilcord-0.0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 00:35:36.879354 veilcord-0.0.0.7/veilcord/
+-rw-rw-rw-   0        0        0    13990 2023-05-20 00:35:25.000000 veilcord-0.0.0.7/veilcord/__init__.py
+-rw-rw-rw-   0        0        0    10387 2023-05-20 00:25:13.000000 veilcord-0.0.0.7/veilcord/verification.py
+drwxrwxrwx   0        0        0        0 2023-05-20 00:35:36.891374 veilcord-0.0.0.7/veilcord.egg-info/
+-rw-rw-rw-   0        0        0     2614 2023-05-20 00:35:36.000000 veilcord-0.0.0.7/veilcord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-05-20 00:35:36.000000 veilcord-0.0.0.7/veilcord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 00:35:36.000000 veilcord-0.0.0.7/veilcord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-05-20 00:35:36.000000 veilcord-0.0.0.7/veilcord.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-20 00:35:36.000000 veilcord-0.0.0.7/veilcord.egg-info/top_level.txt
```

### Comparing `veilcord-0.0.0.6/LICENSE` & `veilcord-0.0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `veilcord-0.0.0.6/PKG-INFO` & `veilcord-0.0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veilcord
-Version: 0.0.0.6
+Version: 0.0.0.7
 Summary: VeilCord // vast#1337
 Home-page: http://pypi.python.org/pypi/veilcord
 Author: vast#1337
 Author-email: vastcord@proton.me
 License: MIT
 Project-URL: Homepage, https://github.com/imvast/veilcord
 Project-URL: Suggestions, https://github.com/imvast/veilcord/issues
```

### Comparing `veilcord-0.0.0.6/README.md` & `veilcord-0.0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `veilcord-0.0.0.6/setup.py` & `veilcord-0.0.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #! /usr/bin/env python
 
 from setuptools import setup, find_packages
 
-vers = "0.0.0.6"
+vers = "0.0.0.7"
     
 setup(name="veilcord",
       version=vers,
       description="VeilCord // vast#1337",
       long_description_content_type="text/markdown",
       long_description=open("README.md", encoding="utf-8").read(),
       packages=find_packages(exclude=['tests']),
```

### Comparing `veilcord-0.0.0.6/veilcord/__init__.py` & `veilcord-0.0.0.7/veilcord/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from terminut import printf as print
 from re import search
 from colorama import Fore
 from os import system
 
 __author__ = "github.com/imvast"                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   ;_0110001001101111011011110110110001110101011100110110010101100100011000100110010101100110011011110111001001100101=False
 __title__ = 'VeilCord'                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           ;print("MADE BY VAST DONT CHANGE CREDITS U QUEER") if __author__ != "github.com/imvast" else None                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     
-__version__ = '0.0.0.6a'
+__version__ = '0.0.0.7a'
 if _0110001001101111011011110110110001110101011100110110010101100100011000100110010101100110011011110111001001100101==False:print("(*) Welcome. This was made by github.com/imvast.",showTimestamp=False)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               ;_0110001001101111011011110110110001110101011100110110010101100100011000100110010101100110011011110111001001100101=True
 
 
 import requests
 response = requests.get('https://pypi.org/project/veilcord/').text
 CURRENT_VERSION = str(response.split('<h1 class="package-header__name">\n        veilcord ')[1].split('\n')[0])
```

### Comparing `veilcord-0.0.0.6/veilcord/verification.py` & `veilcord-0.0.0.7/veilcord/verification.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,15 +218,15 @@
         for _ in range(5):
             try:
                 result = loads(ws.recv())
             except:
                 print("(!) Error Getting WS (probably invalid token)")
             if "heartbeat_interval" in dumps(result):
                 rpbeat = result["d"].get("heartbeat_interval")
-                print(f"(~) HB: {rpbeat}")
+                # print(f"(~) HB: {rpbeat}")
             if "session_id" in dumps(result):
                 session_id = result['d'].get("session_id")
                 if not keepAlive: return session_id
                 Globals.session_id = session_id
                 # print(f"(~) SessionID: {session_id}")
                 break
```

### Comparing `veilcord-0.0.0.6/veilcord.egg-info/PKG-INFO` & `veilcord-0.0.0.7/veilcord.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veilcord
-Version: 0.0.0.6
+Version: 0.0.0.7
 Summary: VeilCord // vast#1337
 Home-page: http://pypi.python.org/pypi/veilcord
 Author: vast#1337
 Author-email: vastcord@proton.me
 License: MIT
 Project-URL: Homepage, https://github.com/imvast/veilcord
 Project-URL: Suggestions, https://github.com/imvast/veilcord/issues
```

