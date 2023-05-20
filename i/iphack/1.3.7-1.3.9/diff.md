# Comparing `tmp/iphack-1.3.7.tar.gz` & `tmp/iphack-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iphack-1.3.7.tar", last modified: Sat May 20 12:31:16 2023, max compression
+gzip compressed data, was "iphack-1.3.9.tar", last modified: Sat May 20 20:02:11 2023, max compression
```

## Comparing `iphack-1.3.7.tar` & `iphack-1.3.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwx------   0 u0_a314  (10314) u0_a314  (10314)        0 2023-05-20 12:31:16.953552 iphack-1.3.7/
--rw-------   0 u0_a314  (10314) u0_a314  (10314)     7433 2023-05-20 12:31:16.953552 iphack-1.3.7/PKG-INFO
--rw-------   0 u0_a314  (10314) u0_a314  (10314)     5913 2023-05-20 12:30:35.000000 iphack-1.3.7/README.md
-drwx------   0 u0_a314  (10314) u0_a314  (10314)        0 2023-05-20 12:31:16.949552 iphack-1.3.7/iphack/
--rw-------   0 u0_a314  (10314) u0_a314  (10314)       95 2023-01-30 09:40:16.000000 iphack-1.3.7/iphack/__init__.py
--rw-------   0 u0_a314  (10314) u0_a314  (10314)    44383 2023-05-20 12:30:53.000000 iphack-1.3.7/iphack/iphack.py
-drwx------   0 u0_a314  (10314) u0_a314  (10314)        0 2023-05-20 12:31:16.953552 iphack-1.3.7/iphack.egg-info/
--rw-------   0 u0_a314  (10314) u0_a314  (10314)     7433 2023-05-20 12:31:16.000000 iphack-1.3.7/iphack.egg-info/PKG-INFO
--rw-------   0 u0_a314  (10314) u0_a314  (10314)      213 2023-05-20 12:31:16.000000 iphack-1.3.7/iphack.egg-info/SOURCES.txt
--rw-------   0 u0_a314  (10314) u0_a314  (10314)        1 2023-05-20 12:31:16.000000 iphack-1.3.7/iphack.egg-info/dependency_links.txt
--rw-------   0 u0_a314  (10314) u0_a314  (10314)       65 2023-05-20 12:31:16.000000 iphack-1.3.7/iphack.egg-info/requires.txt
--rw-------   0 u0_a314  (10314) u0_a314  (10314)        7 2023-05-20 12:31:16.000000 iphack-1.3.7/iphack.egg-info/top_level.txt
--rw-------   0 u0_a314  (10314) u0_a314  (10314)       79 2023-05-20 12:31:16.953552 iphack-1.3.7/setup.cfg
--rw-------   0 u0_a314  (10314) u0_a314  (10314)     2293 2023-05-20 12:30:46.000000 iphack-1.3.7/setup.py
+drwx------   0 u0_a314  (10314) u0_a314  (10314)        0 2023-05-20 20:02:11.476457 iphack-1.3.9/
+-rw-------   0 u0_a314  (10314) u0_a314  (10314)     7433 2023-05-20 20:02:11.476457 iphack-1.3.9/PKG-INFO
+-rw-------   0 u0_a314  (10314) u0_a314  (10314)     5913 2023-05-20 12:30:35.000000 iphack-1.3.9/README.md
+drwx------   0 u0_a314  (10314) u0_a314  (10314)        0 2023-05-20 20:02:11.472458 iphack-1.3.9/iphack/
+-rw-------   0 u0_a314  (10314) u0_a314  (10314)       95 2023-01-30 09:40:16.000000 iphack-1.3.9/iphack/__init__.py
+-rw-------   0 u0_a314  (10314) u0_a314  (10314)    44383 2023-05-20 20:01:23.000000 iphack-1.3.9/iphack/iphack.py
+drwx------   0 u0_a314  (10314) u0_a314  (10314)        0 2023-05-20 20:02:11.476457 iphack-1.3.9/iphack.egg-info/
+-rw-------   0 u0_a314  (10314) u0_a314  (10314)     7433 2023-05-20 20:02:11.000000 iphack-1.3.9/iphack.egg-info/PKG-INFO
+-rw-------   0 u0_a314  (10314) u0_a314  (10314)      213 2023-05-20 20:02:11.000000 iphack-1.3.9/iphack.egg-info/SOURCES.txt
+-rw-------   0 u0_a314  (10314) u0_a314  (10314)        1 2023-05-20 20:02:11.000000 iphack-1.3.9/iphack.egg-info/dependency_links.txt
+-rw-------   0 u0_a314  (10314) u0_a314  (10314)       65 2023-05-20 20:02:11.000000 iphack-1.3.9/iphack.egg-info/requires.txt
+-rw-------   0 u0_a314  (10314) u0_a314  (10314)        7 2023-05-20 20:02:11.000000 iphack-1.3.9/iphack.egg-info/top_level.txt
+-rw-------   0 u0_a314  (10314) u0_a314  (10314)       79 2023-05-20 20:02:11.476457 iphack-1.3.9/setup.cfg
+-rw-------   0 u0_a314  (10314) u0_a314  (10314)     2293 2023-05-20 20:01:59.000000 iphack-1.3.9/setup.py
```

### Comparing `iphack-1.3.7/PKG-INFO` & `iphack-1.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iphack
-Version: 1.3.7
+Version: 1.3.9
 Summary: the most ideal tool for finding out information about IP, etc.
 Home-page: https://github.com/mishakorzik/IpHack
 Author: MishaKorzhik_He1Zen
 Author-email: developer.mishakorzhik@gmail.com
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/mishakorzik/IpHack/issues
 Project-URL: Sponsor, https://www.buymeacoffee.com/misakorzik
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iphack Version: 1.3.7 Summary: the most ideal tool
+Metadata-Version: 2.1 Name: iphack Version: 1.3.9 Summary: the most ideal tool
 for finding out information about IP, etc. Home-page: https://github.com/
 mishakorzik/IpHack Author: MishaKorzhik_He1Zen Author-email:
 developer.mishakorzhik@gmail.com License: Apache 2.0 Project-URL: Bug Tracker,
 https://github.com/mishakorzik/IpHack/issues Project-URL: Sponsor, https://
 www.buymeacoffee.com/misakorzik Keywords:
 ip,address,iphack,ips,pypi,pip,dns,router,ipv4,ipv6,public,ip-
 address,isp,location,lookup,iplookup,inquiry,tor,anon Classifier: Development
```

### Comparing `iphack-1.3.7/README.md` & `iphack-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `iphack-1.3.7/iphack/iphack.py` & `iphack-1.3.9/iphack/iphack.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 red = '\033[31m'
 yellow = '\033[93m'
 lgreen = '\033[92m'
 clear = '\033[0m'
 bold = '\033[01m'
 cyan = '\033[96m'
-version = "1.3.7"
+version = "1.3.9"
 referer_list = ["https://www.google.com/", "https://www.youtube.com/", "https://www.twitter.com/", "https://www.discord.com/", "https://www.tiktok.com/", "https://www.instagram.com/", "https://check-host.net/", "https://github.com", "https://gitlab.com", "https://he1zen.rf.gd"]
 
 major = str(sys.version_info.major)
 minor = str(sys.version_info.minor)
 path = str(sys.exec_prefix+"/lib/python"+major+"."+minor+"/site-packages/iphack/")
 
 global log
@@ -379,15 +379,15 @@
         port = int(get["mailport"])
         check = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         check.connect((ip, port))
         find = str(find)
         check.sendall(bytes("get|domain,ip|info|"+find,'UTF-8'))
         try:
             check.settimeout(10)
-            code = check.recv(2048)
+            code = check.recv(4096)
             get = code.decode('utf-8')
             if get == "-":
                 print("no results")
             else:
                 get = get.replace(",", "/")
                 print(get)
         except:
```

### Comparing `iphack-1.3.7/iphack.egg-info/PKG-INFO` & `iphack-1.3.9/iphack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iphack
-Version: 1.3.7
+Version: 1.3.9
 Summary: the most ideal tool for finding out information about IP, etc.
 Home-page: https://github.com/mishakorzik/IpHack
 Author: MishaKorzhik_He1Zen
 Author-email: developer.mishakorzhik@gmail.com
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/mishakorzik/IpHack/issues
 Project-URL: Sponsor, https://www.buymeacoffee.com/misakorzik
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iphack Version: 1.3.7 Summary: the most ideal tool
+Metadata-Version: 2.1 Name: iphack Version: 1.3.9 Summary: the most ideal tool
 for finding out information about IP, etc. Home-page: https://github.com/
 mishakorzik/IpHack Author: MishaKorzhik_He1Zen Author-email:
 developer.mishakorzhik@gmail.com License: Apache 2.0 Project-URL: Bug Tracker,
 https://github.com/mishakorzik/IpHack/issues Project-URL: Sponsor, https://
 www.buymeacoffee.com/misakorzik Keywords:
 ip,address,iphack,ips,pypi,pip,dns,router,ipv4,ipv6,public,ip-
 address,isp,location,lookup,iplookup,inquiry,tor,anon Classifier: Development
```

### Comparing `iphack-1.3.7/setup.py` & `iphack-1.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Reads the content of your README.md into a variable to be used in the setup below
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='iphack',  # should match the package folder
     packages=['iphack'],  # should match the package folder
-    version='1.3.7',  # important for updates
+    version='1.3.9',  # important for updates
     python_requires=">=3.4",
     license='Apache 2.0',  # should match your chosen license
     description='the most ideal tool for finding out information about IP, etc.',
     long_description=long_description,  # loads your README.md
     long_description_content_type="text/markdown",  # README.md is of type 'markdown'
     author='MishaKorzhik_He1Zen',
     author_email='developer.mishakorzhik@gmail.com',
```

