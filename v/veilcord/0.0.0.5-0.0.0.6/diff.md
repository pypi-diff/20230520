# Comparing `tmp/veilcord-0.0.0.5.tar.gz` & `tmp/veilcord-0.0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "veilcord-0.0.0.5.tar", last modified: Fri May 19 23:27:43 2023, max compression
+gzip compressed data, was "veilcord-0.0.0.6.tar", last modified: Sat May 20 00:13:37 2023, max compression
```

## Comparing `veilcord-0.0.0.5.tar` & `veilcord-0.0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 23:27:43.655725 veilcord-0.0.0.5/
--rw-rw-rw-   0        0        0     1085 2023-05-08 01:47:46.000000 veilcord-0.0.0.5/LICENSE
--rw-rw-rw-   0        0        0     1926 2023-05-19 23:27:43.655725 veilcord-0.0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      748 2023-05-17 01:51:11.000000 veilcord-0.0.0.5/README.md
--rw-rw-rw-   0        0        0       86 2023-05-08 02:01:12.000000 veilcord-0.0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-19 23:27:43.655725 veilcord-0.0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1603 2023-05-19 23:27:09.000000 veilcord-0.0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-19 23:27:43.649379 veilcord-0.0.0.5/veilcord/
--rw-rw-rw-   0        0        0    13742 2023-05-19 23:27:30.000000 veilcord-0.0.0.5/veilcord/__init__.py
--rw-rw-rw-   0        0        0    10092 2023-05-19 23:26:56.000000 veilcord-0.0.0.5/veilcord/verification.py
-drwxrwxrwx   0        0        0        0 2023-05-19 23:27:43.654727 veilcord-0.0.0.5/veilcord.egg-info/
--rw-rw-rw-   0        0        0     1926 2023-05-19 23:27:43.000000 veilcord-0.0.0.5/veilcord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2023-05-19 23:27:43.000000 veilcord-0.0.0.5/veilcord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 23:27:43.000000 veilcord-0.0.0.5/veilcord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-05-19 23:27:43.000000 veilcord-0.0.0.5/veilcord.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-19 23:27:43.000000 veilcord-0.0.0.5/veilcord.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-20 00:13:37.198341 veilcord-0.0.0.6/
+-rw-rw-rw-   0        0        0     1085 2023-05-08 01:47:46.000000 veilcord-0.0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     2614 2023-05-20 00:13:37.198341 veilcord-0.0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1436 2023-05-19 23:47:05.000000 veilcord-0.0.0.6/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-08 02:01:12.000000 veilcord-0.0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-20 00:13:37.198341 veilcord-0.0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1603 2023-05-19 23:50:54.000000 veilcord-0.0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 00:13:37.184870 veilcord-0.0.0.6/veilcord/
+-rw-rw-rw-   0        0        0    13990 2023-05-20 00:06:07.000000 veilcord-0.0.0.6/veilcord/__init__.py
+-rw-rw-rw-   0        0        0    10385 2023-05-20 00:12:31.000000 veilcord-0.0.0.6/veilcord/verification.py
+drwxrwxrwx   0        0        0        0 2023-05-20 00:13:37.197343 veilcord-0.0.0.6/veilcord.egg-info/
+-rw-rw-rw-   0        0        0     2614 2023-05-20 00:13:37.000000 veilcord-0.0.0.6/veilcord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-05-20 00:13:37.000000 veilcord-0.0.0.6/veilcord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 00:13:37.000000 veilcord-0.0.0.6/veilcord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-05-20 00:13:37.000000 veilcord-0.0.0.6/veilcord.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-20 00:13:37.000000 veilcord-0.0.0.6/veilcord.egg-info/top_level.txt
```

### Comparing `veilcord-0.0.0.5/LICENSE` & `veilcord-0.0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `veilcord-0.0.0.5/setup.py` & `veilcord-0.0.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #! /usr/bin/env python
 
 from setuptools import setup, find_packages
 
-vers = "0.0.0.5"
+vers = "0.0.0.6"
     
 setup(name="veilcord",
       version=vers,
       description="VeilCord // vast#1337",
       long_description_content_type="text/markdown",
       long_description=open("README.md", encoding="utf-8").read(),
       packages=find_packages(exclude=['tests']),
```

### Comparing `veilcord-0.0.0.5/veilcord/__init__.py` & `veilcord-0.0.0.6/veilcord/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 from .verification import *
 from terminut import printf as print
 from re import search
 from colorama import Fore
+from os import system
 
 __author__ = "github.com/imvast"                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   ;_0110001001101111011011110110110001110101011100110110010101100100011000100110010101100110011011110111001001100101=False
+__title__ = 'VeilCord'                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           ;print("MADE BY VAST DONT CHANGE CREDITS U QUEER") if __author__ != "github.com/imvast" else None                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     
+__version__ = '0.0.0.6a'
 if _0110001001101111011011110110110001110101011100110110010101100100011000100110010101100110011011110111001001100101==False:print("(*) Welcome. This was made by github.com/imvast.",showTimestamp=False)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               ;_0110001001101111011011110110110001110101011100110110010101100100011000100110010101100110011011110111001001100101=True
 
-__title__ = 'VeilCord'                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           ;print("MADE BY VAST DONT CHANGE CREDITS U QUEER") if __author__ != "github.com/imvast" else None                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     
-__version__ = '0.0.0.5a'
 
-CURRENT_VERSION = '0.0.0.69'
+import requests
+response = requests.get('https://pypi.org/project/veilcord/').text
+CURRENT_VERSION = str(response.split('<h1 class="package-header__name">\n        veilcord ')[1].split('\n')[0])
 
 
 if __version__ < CURRENT_VERSION:
     print(
         f"[VeilCord] Version Out-of-Date. Please upgrade by using: \"python.exe -m pip install -U veilcord\"", 
         mainCol=Fore.RED,
         showTimestamp=False
     )
+    system('python.exe -m pip install -U veilcord  -q')
 
 
 def getCode(invite):
     """Extracts the code from a Discord invite link"""
     code_regex = r"(?:(?:http:\/\/|https:\/\/)?discord\.gg\/|discordapp\.com\/invite\/|discord\.com\/invite\/)?([a-zA-Z0-9-]+)"
     match = search(code_regex, invite)
     if match:
```

### Comparing `veilcord-0.0.0.5/veilcord/verification.py` & `veilcord-0.0.0.6/veilcord/verification.py`

 * *Files 3% similar despite different names*

```diff
@@ -215,37 +215,43 @@
         ws.send(
             dumps(message)
         )
         for _ in range(5):
             try:
                 result = loads(ws.recv())
             except:
-                print("probably invalid token")
+                print("(!) Error Getting WS (probably invalid token)")
             if "heartbeat_interval" in dumps(result):
                 rpbeat = result["d"].get("heartbeat_interval")
-                # print(f"(~) HB: {rpbeat}")
+                print(f"(~) HB: {rpbeat}")
             if "session_id" in dumps(result):
                 session_id = result['d'].get("session_id")
+                if not keepAlive: return session_id
                 Globals.session_id = session_id
                 # print(f"(~) SessionID: {session_id}")
                 break
                 
         if keepAlive:
             while Globals.sessionOn:
                 sleep(rpbeat / 1000)
                 ws.send(dumps({"op":1,"d":10}))
                 # print(f"(*) Sent HB.")
             
 
     def getSession(self, token: str, type: int = 1, keepAlive: bool = False):
-        if keepAlive: print("[WARN] KeepAlive is expirimental")
-        t1 = Thread(target=self._penis, args=[token, type, keepAlive])
-        Globals.sessionThread = t1
-        t1.start()
-        while Globals.session_id is None:
-            sleep(0.1)
-        return Globals.session_id
+        if keepAlive: 
+            print("[WARN] KeepAlive is expirimental")
+            t1 = Thread(target=self._penis, args=[token, type, keepAlive])
+            Globals.sessionThread = t1
+            t1.start()
+            while Globals.session_id is None:
+                sleep(0.1)
+            return Globals.session_id
+        else:
+            return self._penis(token, type, keepAlive)
     
     def closeSession(self, token):
         Globals.sessionOn = False
+        if Globals.sessionThread is None:
+            return print("(!) Cannot close an unopened session.")
         Globals.sessionThread.join()
         return
```

