# Comparing `tmp/veilcord-0.0.0.4.tar.gz` & `tmp/veilcord-0.0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "veilcord-0.0.0.4.tar", last modified: Fri May 19 23:22:34 2023, max compression
+gzip compressed data, was "veilcord-0.0.0.5.tar", last modified: Fri May 19 23:27:43 2023, max compression
```

## Comparing `veilcord-0.0.0.4.tar` & `veilcord-0.0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 23:22:34.272407 veilcord-0.0.0.4/
--rw-rw-rw-   0        0        0     1085 2023-05-08 01:47:46.000000 veilcord-0.0.0.4/LICENSE
--rw-rw-rw-   0        0        0     1926 2023-05-19 23:22:34.271107 veilcord-0.0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      748 2023-05-17 01:51:11.000000 veilcord-0.0.0.4/README.md
--rw-rw-rw-   0        0        0       86 2023-05-08 02:01:12.000000 veilcord-0.0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-19 23:22:34.272407 veilcord-0.0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1603 2023-05-19 23:21:21.000000 veilcord-0.0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-19 23:22:34.265600 veilcord-0.0.0.4/veilcord/
--rw-rw-rw-   0        0        0    13776 2023-05-19 23:21:28.000000 veilcord-0.0.0.4/veilcord/__init__.py
--rw-rw-rw-   0        0        0     9959 2023-05-19 23:20:56.000000 veilcord-0.0.0.4/veilcord/verification.py
-drwxrwxrwx   0        0        0        0 2023-05-19 23:22:34.271107 veilcord-0.0.0.4/veilcord.egg-info/
--rw-rw-rw-   0        0        0     1926 2023-05-19 23:22:34.000000 veilcord-0.0.0.4/veilcord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2023-05-19 23:22:34.000000 veilcord-0.0.0.4/veilcord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 23:22:34.000000 veilcord-0.0.0.4/veilcord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-05-19 23:22:34.000000 veilcord-0.0.0.4/veilcord.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-19 23:22:34.000000 veilcord-0.0.0.4/veilcord.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 23:27:43.655725 veilcord-0.0.0.5/
+-rw-rw-rw-   0        0        0     1085 2023-05-08 01:47:46.000000 veilcord-0.0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1926 2023-05-19 23:27:43.655725 veilcord-0.0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      748 2023-05-17 01:51:11.000000 veilcord-0.0.0.5/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-08 02:01:12.000000 veilcord-0.0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-19 23:27:43.655725 veilcord-0.0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1603 2023-05-19 23:27:09.000000 veilcord-0.0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 23:27:43.649379 veilcord-0.0.0.5/veilcord/
+-rw-rw-rw-   0        0        0    13742 2023-05-19 23:27:30.000000 veilcord-0.0.0.5/veilcord/__init__.py
+-rw-rw-rw-   0        0        0    10092 2023-05-19 23:26:56.000000 veilcord-0.0.0.5/veilcord/verification.py
+drwxrwxrwx   0        0        0        0 2023-05-19 23:27:43.654727 veilcord-0.0.0.5/veilcord.egg-info/
+-rw-rw-rw-   0        0        0     1926 2023-05-19 23:27:43.000000 veilcord-0.0.0.5/veilcord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-05-19 23:27:43.000000 veilcord-0.0.0.5/veilcord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 23:27:43.000000 veilcord-0.0.0.5/veilcord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-05-19 23:27:43.000000 veilcord-0.0.0.5/veilcord.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-19 23:27:43.000000 veilcord-0.0.0.5/veilcord.egg-info/top_level.txt
```

### Comparing `veilcord-0.0.0.4/LICENSE` & `veilcord-0.0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `veilcord-0.0.0.4/PKG-INFO` & `veilcord-0.0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veilcord
-Version: 0.0.0.4
+Version: 0.0.0.5
 Summary: VeilCord // vast#1337
 Home-page: http://pypi.python.org/pypi/veilcord
 Author: vast#1337
 Author-email: vastcord@proton.me
 License: MIT
 Project-URL: Homepage, https://github.com/imvast/veilcord
 Project-URL: Suggestions, https://github.com/imvast/veilcord/issues
```

### Comparing `veilcord-0.0.0.4/README.md` & `veilcord-0.0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `veilcord-0.0.0.4/setup.py` & `veilcord-0.0.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #! /usr/bin/env python
 
 from setuptools import setup, find_packages
 
-vers = "0.0.0.4"
+vers = "0.0.0.5"
     
 setup(name="veilcord",
       version=vers,
       description="VeilCord // vast#1337",
       long_description_content_type="text/markdown",
       long_description=open("README.md", encoding="utf-8").read(),
       packages=find_packages(exclude=['tests']),
```

### Comparing `veilcord-0.0.0.4/veilcord/__init__.py` & `veilcord-0.0.0.5/veilcord/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,19 +2,18 @@
 from terminut import printf as print
 from re import search
 from colorama import Fore
 
 __author__ = "github.com/imvast"                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   ;_0110001001101111011011110110110001110101011100110110010101100100011000100110010101100110011011110111001001100101=False
 if _0110001001101111011011110110110001110101011100110110010101100100011000100110010101100110011011110111001001100101==False:print("(*) Welcome. This was made by github.com/imvast.",showTimestamp=False)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               ;_0110001001101111011011110110110001110101011100110110010101100100011000100110010101100110011011110111001001100101=True
 
-__title__ = 'terminut'
-__author__ = 'github.com/imvast'                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            ;print("MADE BY VAST DONT CHANGE CREDITS U QUEER") if __author__ != "github.com/imvast" else None                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     
-__version__ = '0.0.0.4a'
+__title__ = 'VeilCord'                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           ;print("MADE BY VAST DONT CHANGE CREDITS U QUEER") if __author__ != "github.com/imvast" else None                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     
+__version__ = '0.0.0.5a'
 
-CURRENT_VERSION = '0.0.0.4'
+CURRENT_VERSION = '0.0.0.69'
 
 
 if __version__ < CURRENT_VERSION:
     print(
         f"[VeilCord] Version Out-of-Date. Please upgrade by using: \"python.exe -m pip install -U veilcord\"", 
         mainCol=Fore.RED,
         showTimestamp=False
```

### Comparing `veilcord-0.0.0.4/veilcord/verification.py` & `veilcord-0.0.0.5/veilcord/verification.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,15 +128,15 @@
         else: raise ValueError("An invalid type for getFingerprint() was provided. Acceptable values: ['browser', 'mobile']")
         response = self.session.get('https://discord.com/api/v9/experiments', headers=headers)
         if withCookies:
             return response.json().get("fingerprint"), response.cookies
         return response.json().get("fingerprint")
 
 
-    def _penis(self, token, type):
+    def _penis(self, token, type, keepAlive):
         ws = WebSocket()
         ws.connect("wss://gateway.discord.gg/?encoding=json&v=9")
         if type == 1:
             message = {
                 "op":2,
                 "d":{
                     "token":token,
@@ -225,23 +225,24 @@
                 # print(f"(~) HB: {rpbeat}")
             if "session_id" in dumps(result):
                 session_id = result['d'].get("session_id")
                 Globals.session_id = session_id
                 # print(f"(~) SessionID: {session_id}")
                 break
                 
-                
-        while Globals.sessionOn:
-            sleep(rpbeat / 1000)
-            ws.send(dumps({"op":1,"d":10}))
-            # print(f"(*) Sent HB.")
+        if keepAlive:
+            while Globals.sessionOn:
+                sleep(rpbeat / 1000)
+                ws.send(dumps({"op":1,"d":10}))
+                # print(f"(*) Sent HB.")
             
 
-    def getSession(self, token: str, type: int = 1):
-        t1 = Thread(target=self._penis, args=[token, type])
+    def getSession(self, token: str, type: int = 1, keepAlive: bool = False):
+        if keepAlive: print("[WARN] KeepAlive is expirimental")
+        t1 = Thread(target=self._penis, args=[token, type, keepAlive])
         Globals.sessionThread = t1
         t1.start()
         while Globals.session_id is None:
             sleep(0.1)
         return Globals.session_id
     
     def closeSession(self, token):
```

### Comparing `veilcord-0.0.0.4/veilcord.egg-info/PKG-INFO` & `veilcord-0.0.0.5/veilcord.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veilcord
-Version: 0.0.0.4
+Version: 0.0.0.5
 Summary: VeilCord // vast#1337
 Home-page: http://pypi.python.org/pypi/veilcord
 Author: vast#1337
 Author-email: vastcord@proton.me
 License: MIT
 Project-URL: Homepage, https://github.com/imvast/veilcord
 Project-URL: Suggestions, https://github.com/imvast/veilcord/issues
```

