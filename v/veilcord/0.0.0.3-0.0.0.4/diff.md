# Comparing `tmp/veilcord-0.0.0.3.tar.gz` & `tmp/veilcord-0.0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "veilcord-0.0.0.3.tar", last modified: Fri May 19 00:07:38 2023, max compression
+gzip compressed data, was "veilcord-0.0.0.4.tar", last modified: Fri May 19 23:22:34 2023, max compression
```

## Comparing `veilcord-0.0.0.3.tar` & `veilcord-0.0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 00:07:38.548392 veilcord-0.0.0.3/
--rw-rw-rw-   0        0        0     1085 2023-05-08 01:47:46.000000 veilcord-0.0.0.3/LICENSE
--rw-rw-rw-   0        0        0     1926 2023-05-19 00:07:38.547393 veilcord-0.0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      748 2023-05-17 01:51:11.000000 veilcord-0.0.0.3/README.md
--rw-rw-rw-   0        0        0       86 2023-05-08 02:01:12.000000 veilcord-0.0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-19 00:07:38.548392 veilcord-0.0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1603 2023-05-19 00:03:30.000000 veilcord-0.0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-19 00:07:38.540409 veilcord-0.0.0.3/veilcord/
--rw-rw-rw-   0        0        0    13740 2023-05-19 00:06:20.000000 veilcord-0.0.0.3/veilcord/__init__.py
--rw-rw-rw-   0        0        0     7885 2023-05-18 23:58:49.000000 veilcord-0.0.0.3/veilcord/verification.py
-drwxrwxrwx   0        0        0        0 2023-05-19 00:07:38.546396 veilcord-0.0.0.3/veilcord.egg-info/
--rw-rw-rw-   0        0        0     1926 2023-05-19 00:07:38.000000 veilcord-0.0.0.3/veilcord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2023-05-19 00:07:38.000000 veilcord-0.0.0.3/veilcord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 00:07:38.000000 veilcord-0.0.0.3/veilcord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-05-19 00:07:38.000000 veilcord-0.0.0.3/veilcord.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-19 00:07:38.000000 veilcord-0.0.0.3/veilcord.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 23:22:34.272407 veilcord-0.0.0.4/
+-rw-rw-rw-   0        0        0     1085 2023-05-08 01:47:46.000000 veilcord-0.0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1926 2023-05-19 23:22:34.271107 veilcord-0.0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      748 2023-05-17 01:51:11.000000 veilcord-0.0.0.4/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-08 02:01:12.000000 veilcord-0.0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-19 23:22:34.272407 veilcord-0.0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1603 2023-05-19 23:21:21.000000 veilcord-0.0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 23:22:34.265600 veilcord-0.0.0.4/veilcord/
+-rw-rw-rw-   0        0        0    13776 2023-05-19 23:21:28.000000 veilcord-0.0.0.4/veilcord/__init__.py
+-rw-rw-rw-   0        0        0     9959 2023-05-19 23:20:56.000000 veilcord-0.0.0.4/veilcord/verification.py
+drwxrwxrwx   0        0        0        0 2023-05-19 23:22:34.271107 veilcord-0.0.0.4/veilcord.egg-info/
+-rw-rw-rw-   0        0        0     1926 2023-05-19 23:22:34.000000 veilcord-0.0.0.4/veilcord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-05-19 23:22:34.000000 veilcord-0.0.0.4/veilcord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 23:22:34.000000 veilcord-0.0.0.4/veilcord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-05-19 23:22:34.000000 veilcord-0.0.0.4/veilcord.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-19 23:22:34.000000 veilcord-0.0.0.4/veilcord.egg-info/top_level.txt
```

### Comparing `veilcord-0.0.0.3/LICENSE` & `veilcord-0.0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `veilcord-0.0.0.3/PKG-INFO` & `veilcord-0.0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veilcord
-Version: 0.0.0.3
+Version: 0.0.0.4
 Summary: VeilCord // vast#1337
 Home-page: http://pypi.python.org/pypi/veilcord
 Author: vast#1337
 Author-email: vastcord@proton.me
 License: MIT
 Project-URL: Homepage, https://github.com/imvast/veilcord
 Project-URL: Suggestions, https://github.com/imvast/veilcord/issues
```

### Comparing `veilcord-0.0.0.3/README.md` & `veilcord-0.0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `veilcord-0.0.0.3/setup.py` & `veilcord-0.0.0.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #! /usr/bin/env python
 
 from setuptools import setup, find_packages
 
-vers = "0.0.0.3"
+vers = "0.0.0.4"
     
 setup(name="veilcord",
       version=vers,
       description="VeilCord // vast#1337",
       long_description_content_type="text/markdown",
       long_description=open("README.md", encoding="utf-8").read(),
       packages=find_packages(exclude=['tests']),
```

### Comparing `veilcord-0.0.0.3/veilcord/__init__.py` & `veilcord-0.0.0.4/veilcord/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 from colorama import Fore
 
 __author__ = "github.com/imvast"                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   ;_0110001001101111011011110110110001110101011100110110010101100100011000100110010101100110011011110111001001100101=False
 if _0110001001101111011011110110110001110101011100110110010101100100011000100110010101100110011011110111001001100101==False:print("(*) Welcome. This was made by github.com/imvast.",showTimestamp=False)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               ;_0110001001101111011011110110110001110101011100110110010101100100011000100110010101100110011011110111001001100101=True
 
 __title__ = 'terminut'
 __author__ = 'github.com/imvast'                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            ;print("MADE BY VAST DONT CHANGE CREDITS U QUEER") if __author__ != "github.com/imvast" else None                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     
-__version__ = '0.0.0.3a'
+__version__ = '0.0.0.4a'
 
-CURRENT_VERSION = '0.0.0.3'
+CURRENT_VERSION = '0.0.0.4'
 
 
 if __version__ < CURRENT_VERSION:
     print(
         f"[VeilCord] Version Out-of-Date. Please upgrade by using: \"python.exe -m pip install -U veilcord\"", 
         mainCol=Fore.RED,
         showTimestamp=False
@@ -27,8 +27,11 @@
     match = search(code_regex, invite)
     if match:
         try:
             return match.group(1)
         except:
             return match.group(0)
     else:
-        return None
+        return None
+    
+def getBuildNum():
+    pass
```

### Comparing `veilcord-0.0.0.3/veilcord/verification.py` & `veilcord-0.0.0.4/veilcord/verification.py`

 * *Files 16% similar despite different names*

```diff
@@ -128,55 +128,102 @@
         else: raise ValueError("An invalid type for getFingerprint() was provided. Acceptable values: ['browser', 'mobile']")
         response = self.session.get('https://discord.com/api/v9/experiments', headers=headers)
         if withCookies:
             return response.json().get("fingerprint"), response.cookies
         return response.json().get("fingerprint")
 
 
-    def _penis(self, token):
+    def _penis(self, token, type):
         ws = WebSocket()
         ws.connect("wss://gateway.discord.gg/?encoding=json&v=9")
-
-        message = {
-            "op":2,
-            "d":{
-                "token":"MTEwNzM2NTQwMzUyMjUwNjc1Mg.G-IBXS.Ru5GP-alRQx5HRtabMC5ZmT0dfNTs_ahCJYgtc",
-                "capabilities":8189,
+        if type == 1:
+            message = {
+                "op":2,
+                "d":{
+                    "token":token,
+                    "capabilities":8189,
+                    "properties":{
+                        "os":"Windows",
+                        "browser":"Chrome",
+                        "device":"",
+                        "system_locale":"en-US",
+                        "browser_user_agent":"Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36",
+                        "browser_version":"113.0.0.0",
+                        "os_version":"10",
+                        "referrer":"",
+                        "referring_domain":"",
+                        "referrer_current":"","referring_domain_current":"","release_channel":"stable",
+                        "client_build_number":199356,"client_event_source":None,
+                        "design_id":0
+                    },
+                    "presence":{
+                        "status":"online",
+                        "since":0,"activities":[],"afk":False
+                    },
+                    "compress":False,
+                    "client_state":{
+                        "guild_versions":{},"highest_last_message_id":"0","read_state_version":0,
+                        "user_guild_settings_version":-1,"user_settings_version":-1,"private_channels_version":"0",
+                        "api_code_version":0
+                    }
+                }
+            }
+        elif type == 2:
+            message = {
+            "op": 2,
+            "d": {
+                "token": token,
+                "capabilities": 8189,
                 "properties":{
-                    "os":"Windows",
-                    "browser":"Chrome",
+                    "os": "Windows",
+                    "browser": "Discord Client",
                     "device":"",
-                    "system_locale":"en-US",
-                    "browser_user_agent":"Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36",
-                    "browser_version":"113.0.0.0",
-                    "os_version":"10",
-                    "referrer":"",
-                    "referring_domain":"",
-                    "referrer_current":"","referring_domain_current":"","release_channel":"stable",
-                    "client_build_number":199356,"client_event_source":None,
-                    "design_id":0
+                    "system_locale": "en-US",
+                    "browser_user_agent": "Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) discord/1.0.9013 Chrome/108.0.5359.215 Electron/22.3.2 Safari/537.36",
+                    "browser_version": "22.3.2",
+                    "client_version": "1.0.9013",
+                    "os_version": "10.0.22621",
+                    "os_arch": "x64",
+                    "referrer":" ",
+                    "referring_domain": "",
+                    "referrer_current": "",
+                    "referring_domain_current": "",
+                    "release_channel": "stable",
+                    "client_build_number": 199357,
+                    "native_build_number": 32266,
+                    "client_event_source": None,
+                    "design_id": 0
                 },
                 "presence":{
-                    "status":"online",
-                    "since":0,"activities":[],"afk":False
-                },
+                        "status":"online",
+                        "since":0,"activities":[],"afk":False
+                    },
                 "compress":False,
                 "client_state":{
-                    "guild_versions":{},"highest_last_message_id":"0","read_state_version":0,
-                    "user_guild_settings_version":-1,"user_settings_version":-1,"private_channels_version":"0",
+                    "guild_versions":{},
+                    "highest_last_message_id":"0",
+                    "read_state_version":0,
+                    "user_guild_settings_version":-1,
+                    "user_settings_version":-1,
+                    "private_channels_version":"0",
                     "api_code_version":0
                 }
             }
         }
+        else:
+            raise ValueError("Invalid type provided. [1,2]")
 
         ws.send(
             dumps(message)
         )
         for _ in range(5):
-            result = loads(ws.recv())
+            try:
+                result = loads(ws.recv())
+            except:
+                print("probably invalid token")
             if "heartbeat_interval" in dumps(result):
                 rpbeat = result["d"].get("heartbeat_interval")
                 # print(f"(~) HB: {rpbeat}")
             if "session_id" in dumps(result):
                 session_id = result['d'].get("session_id")
                 Globals.session_id = session_id
                 # print(f"(~) SessionID: {session_id}")
@@ -185,16 +232,16 @@
                 
         while Globals.sessionOn:
             sleep(rpbeat / 1000)
             ws.send(dumps({"op":1,"d":10}))
             # print(f"(*) Sent HB.")
             
 
-    def getSession(self, token):
-        t1 = Thread(target=self._penis, args=[token])
+    def getSession(self, token: str, type: int = 1):
+        t1 = Thread(target=self._penis, args=[token, type])
         Globals.sessionThread = t1
         t1.start()
         while Globals.session_id is None:
             sleep(0.1)
         return Globals.session_id
     
     def closeSession(self, token):
```

### Comparing `veilcord-0.0.0.3/veilcord.egg-info/PKG-INFO` & `veilcord-0.0.0.4/veilcord.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veilcord
-Version: 0.0.0.3
+Version: 0.0.0.4
 Summary: VeilCord // vast#1337
 Home-page: http://pypi.python.org/pypi/veilcord
 Author: vast#1337
 Author-email: vastcord@proton.me
 License: MIT
 Project-URL: Homepage, https://github.com/imvast/veilcord
 Project-URL: Suggestions, https://github.com/imvast/veilcord/issues
```

