# Comparing `tmp/matchmeta-2023.4.24.tar.gz` & `tmp/matchmeta-2023.5.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matchmeta-2023.4.24.tar", last modified: Mon Apr 24 10:41:49 2023, max compression
+gzip compressed data, was "matchmeta-2023.5.19.tar", last modified: Sat May 20 00:43:42 2023, max compression
```

## Comparing `matchmeta-2023.4.24.tar` & `matchmeta-2023.5.19.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:41:49.631219 matchmeta-2023.4.24/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-24 10:41:34.000000 matchmeta-2023.4.24/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-04-24 10:41:49.631219 matchmeta-2023.4.24/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-24 10:41:34.000000 matchmeta-2023.4.24/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:41:49.631219 matchmeta-2023.4.24/matchmeta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-04-24 10:41:49.000000 matchmeta-2023.4.24/matchmeta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-24 10:41:49.000000 matchmeta-2023.4.24/matchmeta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 10:41:49.000000 matchmeta-2023.4.24/matchmeta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-24 10:41:49.000000 matchmeta-2023.4.24/matchmeta.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-24 10:41:49.000000 matchmeta-2023.4.24/matchmeta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-24 10:41:49.000000 matchmeta-2023.4.24/matchmeta.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:41:49.631219 matchmeta-2023.4.24/mmi/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-24 10:41:34.000000 matchmeta-2023.4.24/mmi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-24 10:41:34.000000 matchmeta-2023.4.24/mmi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-04-24 10:41:34.000000 matchmeta-2023.4.24/mmi/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 10:41:49.631219 matchmeta-2023.4.24/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-24 10:41:34.000000 matchmeta-2023.4.24/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:43:42.927729 matchmeta-2023.5.19/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-20 00:43:28.000000 matchmeta-2023.5.19/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-20 00:43:42.927729 matchmeta-2023.5.19/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-20 00:43:28.000000 matchmeta-2023.5.19/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:43:42.927729 matchmeta-2023.5.19/matchmeta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-20 00:43:42.000000 matchmeta-2023.5.19/matchmeta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-20 00:43:42.000000 matchmeta-2023.5.19/matchmeta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 00:43:42.000000 matchmeta-2023.5.19/matchmeta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-20 00:43:42.000000 matchmeta-2023.5.19/matchmeta.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-20 00:43:42.000000 matchmeta-2023.5.19/matchmeta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-20 00:43:42.000000 matchmeta-2023.5.19/matchmeta.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:43:42.927729 matchmeta-2023.5.19/mmi/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-20 00:43:28.000000 matchmeta-2023.5.19/mmi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-20 00:43:28.000000 matchmeta-2023.5.19/mmi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-05-20 00:43:28.000000 matchmeta-2023.5.19/mmi/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 00:43:42.927729 matchmeta-2023.5.19/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-20 00:43:28.000000 matchmeta-2023.5.19/setup.py
```

### Comparing `matchmeta-2023.4.24/LICENSE` & `matchmeta-2023.5.19/LICENSE`

 * *Files identical despite different names*

### Comparing `matchmeta-2023.4.24/PKG-INFO` & `matchmeta-2023.5.19/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matchmeta
-Version: 2023.4.24
+Version: 2023.5.19
 Summary: Amazon Linux Triage for Anyone and Everyone
 Home-page: https://github.com/jblukach/mmi
 Author: John Lukach
 Author-email: hello@lukach.io
 License: Apache-2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -12,15 +12,15 @@
 
 # mmi
 
 Amazon Linux default installation now starts with about ```175k+``` directories and files. How do we know which files belong on a particular host during the triage of the operating system?
 
 Review enough systems; you start remembering all those Amazon Linux operating system artifacts, just in time for new directories and filenames to end up in the mix or moved to other locations.
 
-The ```mmi``` command line tool lists the current path’s directories and files based on the user access, which are color-coded to help reduce triage time.
+The ```mmi``` command line tool lists the current path’s directories and files based on user access, which are color-coded to help reduce triage time.
 
 ![MatchMeta.Info CLI Output](MMI.png)
 
 ### Installation
 
 ```
 pip install matchmeta
@@ -34,17 +34,17 @@
 
 ### Color Coded
 
 - :purple_square: Empty File (purple)
 - :green_square: Known File (green)
 - :blue_square: Known Meta (blue)
 - :red_square: Large File (red)
+- :yellow_square: Not Available (yellow)
 - :white_large_square: Partial Meta (grey)
 - :black_large_square: Unknown (black)
-- :yellow_square: Not Available (yellow)
 
 ### GTFOBins
 
 - H for Known SHA256 Hash :red_square: (red)
 - P for Known Full Path :red_square: (red)
 - F for Known File Name :red_square: (red)
```

### Comparing `matchmeta-2023.4.24/README.md` & `matchmeta-2023.5.19/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # mmi
 
 Amazon Linux default installation now starts with about ```175k+``` directories and files. How do we know which files belong on a particular host during the triage of the operating system?
 
 Review enough systems; you start remembering all those Amazon Linux operating system artifacts, just in time for new directories and filenames to end up in the mix or moved to other locations.
 
-The ```mmi``` command line tool lists the current path’s directories and files based on the user access, which are color-coded to help reduce triage time.
+The ```mmi``` command line tool lists the current path’s directories and files based on user access, which are color-coded to help reduce triage time.
 
 ![MatchMeta.Info CLI Output](MMI.png)
 
 ### Installation
 
 ```
 pip install matchmeta
@@ -22,17 +22,17 @@
 
 ### Color Coded
 
 - :purple_square: Empty File (purple)
 - :green_square: Known File (green)
 - :blue_square: Known Meta (blue)
 - :red_square: Large File (red)
+- :yellow_square: Not Available (yellow)
 - :white_large_square: Partial Meta (grey)
 - :black_large_square: Unknown (black)
-- :yellow_square: Not Available (yellow)
 
 ### GTFOBins
 
 - H for Known SHA256 Hash :red_square: (red)
 - P for Known Full Path :red_square: (red)
 - F for Known File Name :red_square: (red)
 
@@ -43,8 +43,8 @@
 - *** for Access Denied :red_square: (red)
 
 ### Local Development
 
 ```
 pip install pybloomfiltermmap3 requests
 python setup.py install --user
-```
+```
```

### Comparing `matchmeta-2023.4.24/matchmeta.egg-info/PKG-INFO` & `matchmeta-2023.5.19/matchmeta.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matchmeta
-Version: 2023.4.24
+Version: 2023.5.19
 Summary: Amazon Linux Triage for Anyone and Everyone
 Home-page: https://github.com/jblukach/mmi
 Author: John Lukach
 Author-email: hello@lukach.io
 License: Apache-2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -12,15 +12,15 @@
 
 # mmi
 
 Amazon Linux default installation now starts with about ```175k+``` directories and files. How do we know which files belong on a particular host during the triage of the operating system?
 
 Review enough systems; you start remembering all those Amazon Linux operating system artifacts, just in time for new directories and filenames to end up in the mix or moved to other locations.
 
-The ```mmi``` command line tool lists the current path’s directories and files based on the user access, which are color-coded to help reduce triage time.
+The ```mmi``` command line tool lists the current path’s directories and files based on user access, which are color-coded to help reduce triage time.
 
 ![MatchMeta.Info CLI Output](MMI.png)
 
 ### Installation
 
 ```
 pip install matchmeta
@@ -34,17 +34,17 @@
 
 ### Color Coded
 
 - :purple_square: Empty File (purple)
 - :green_square: Known File (green)
 - :blue_square: Known Meta (blue)
 - :red_square: Large File (red)
+- :yellow_square: Not Available (yellow)
 - :white_large_square: Partial Meta (grey)
 - :black_large_square: Unknown (black)
-- :yellow_square: Not Available (yellow)
 
 ### GTFOBins
 
 - H for Known SHA256 Hash :red_square: (red)
 - P for Known Full Path :red_square: (red)
 - F for Known File Name :red_square: (red)
```

### Comparing `matchmeta-2023.4.24/mmi/__init__.py` & `matchmeta-2023.5.19/mmi/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 
-__version__ = VERSION = '2023.4.24'
+__version__ = VERSION = '2023.5.19'
 
 __emptyfile__ = EMPTYFILE = '\033[94m{}\033[00m'        ### PURPLE ###
 __knownfile__ = KNOWNFILE = '\033[92m{}\033[00m'        ### GREEN ###
 __knownmeta__ = KNOWNMETA = '\033[96m{}\033[00m'        ### BLUE ###
 __largefile__ = LARGEFILE = '\033[91m{}\033[00m'        ### RED ###
 __nofilehash__ = NOFILEHASH = '\033[93m{}\033[00m'      ### YELLOW ###
 __partialmeta__ = PARTIALMETA = '\033[97m{}\033[00m'    ### GREY ###
 
 __gtfo__ = GTFO = pathlib.Path('/tmp/gtfo.bloom')
-__mmi__ = MMI = pathlib.Path('/tmp/mmi.bloom')
+__mmi__ = MMI = pathlib.Path('/tmp/mmi.bloom')
```

### Comparing `matchmeta-2023.4.24/mmi/cli.py` & `matchmeta-2023.5.19/mmi/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,16 +150,16 @@
         check = await calculate('mmi')
         if check != sha256:
             print('CORRUPTED: /tmp/mmi.bloom')
             sys.exit(1)
     else:
         checked = int(pathlib.Path(update).read_text())
         if now > checked:
-            sha256 = await verify('gtfo')
-            check = await calculate('gtfo')
+            sha256 = await verify('mmi')
+            check = await calculate('mmi')
             if check != sha256:
                 await download('mmi')
                 check = await calculate('mmi')
                 if check != sha256:
                     print('CORRUPTED: /tmp/mmi.bloom')
                     sys.exit(1)
             pathlib.Path(update).write_text(str(now + 3600))
@@ -236,8 +236,8 @@
 
             if str(p.parent) == '/':
                 print(denied+' '+sha256+' '+dir+file)
             else:
                 print(denied+' '+sha256+' '+dir+slash+file)
 
 def main():
-    asyncio.run(start())
+    asyncio.run(start())
```

### Comparing `matchmeta-2023.4.24/setup.py` & `matchmeta-2023.5.19/setup.py`

 * *Files identical despite different names*

