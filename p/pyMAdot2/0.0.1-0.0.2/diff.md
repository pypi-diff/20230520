# Comparing `tmp/pyMAdot2-0.0.1.tar.gz` & `tmp/pyMAdot2-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyMAdot2-0.0.1.tar", last modified: Fri May 19 23:34:31 2023, max compression
+gzip compressed data, was "pyMAdot2-0.0.2.tar", last modified: Sat May 20 07:42:35 2023, max compression
```

## Comparing `pyMAdot2-0.0.1.tar` & `pyMAdot2-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 23:34:31.420296 pyMAdot2-0.0.1/
--rw-rw-rw-   0        0        0     1092 2023-05-19 20:10:20.000000 pyMAdot2-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1637 2023-05-19 23:34:31.419297 pyMAdot2-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      981 2023-05-19 23:30:14.000000 pyMAdot2-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 23:34:31.392651 pyMAdot2-0.0.1/pyMAdot2/
--rw-rw-rw-   0        0        0     2655 2023-05-19 23:32:45.000000 pyMAdot2-0.0.1/pyMAdot2/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 23:34:31.418299 pyMAdot2-0.0.1/pyMAdot2.egg-info/
--rw-rw-rw-   0        0        0     1637 2023-05-19 23:34:31.000000 pyMAdot2-0.0.1/pyMAdot2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-05-19 23:34:31.000000 pyMAdot2-0.0.1/pyMAdot2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 23:34:31.000000 pyMAdot2-0.0.1/pyMAdot2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-19 23:34:31.000000 pyMAdot2-0.0.1/pyMAdot2.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-19 23:34:31.000000 pyMAdot2-0.0.1/pyMAdot2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-05-19 23:34:31.000000 pyMAdot2-0.0.1/pyMAdot2.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2023-05-19 23:34:31.420296 pyMAdot2-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1048 2023-05-19 20:17:15.000000 pyMAdot2-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 07:42:35.848591 pyMAdot2-0.0.2/
+-rw-rw-rw-   0        0        0     1092 2023-05-19 20:10:20.000000 pyMAdot2-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1637 2023-05-20 07:42:35.848591 pyMAdot2-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      981 2023-05-19 23:30:14.000000 pyMAdot2-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-20 07:42:35.831592 pyMAdot2-0.0.2/pyMAdot2/
+-rw-rw-rw-   0        0        0     2754 2023-05-20 07:42:18.000000 pyMAdot2-0.0.2/pyMAdot2/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-20 07:42:35.847595 pyMAdot2-0.0.2/pyMAdot2.egg-info/
+-rw-rw-rw-   0        0        0     1637 2023-05-20 07:42:35.000000 pyMAdot2-0.0.2/pyMAdot2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-05-20 07:42:35.000000 pyMAdot2-0.0.2/pyMAdot2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 07:42:35.000000 pyMAdot2-0.0.2/pyMAdot2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-20 07:42:35.000000 pyMAdot2-0.0.2/pyMAdot2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-20 07:42:35.000000 pyMAdot2-0.0.2/pyMAdot2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-05-19 23:34:31.000000 pyMAdot2-0.0.2/pyMAdot2.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-05-20 07:42:35.848591 pyMAdot2-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1048 2023-05-20 07:42:26.000000 pyMAdot2-0.0.2/setup.py
```

### Comparing `pyMAdot2-0.0.1/LICENSE` & `pyMAdot2-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyMAdot2-0.0.1/PKG-INFO` & `pyMAdot2-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyMAdot2
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python library for MA Lighting dot2 console
 Home-page: https://github.com/elektr0nisch/pyMAdot2
 Author: Linus Groschke
 Author-email: linus@elektronisch.dev
 License: MIT
 Platform: any
 Classifier: Intended Audience :: Developers
```

### Comparing `pyMAdot2-0.0.1/README.md` & `pyMAdot2-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyMAdot2-0.0.1/pyMAdot2/__init__.py` & `pyMAdot2-0.0.2/pyMAdot2/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,14 +45,17 @@
         await self.send({"requestType": "close", "session": self.session_id})
         self.listen_task.cancel()
 
     async def listen(self) -> None:
         while True:
             message = await self.ws.receive()
 
+            if self.initialized:
+                await self.send({"session": self.session_id})
+
             if message.type == aiohttp.WSMsgType.TEXT:
                 data = json.loads(message.data)
                 if "status" in data:
                     await self.send({"session": 0})
 
                 if "session" in data:
                     self.session_id = data["session"]
```

### Comparing `pyMAdot2-0.0.1/pyMAdot2.egg-info/PKG-INFO` & `pyMAdot2-0.0.2/pyMAdot2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyMAdot2
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python library for MA Lighting dot2 console
 Home-page: https://github.com/elektr0nisch/pyMAdot2
 Author: Linus Groschke
 Author-email: linus@elektronisch.dev
 License: MIT
 Platform: any
 Classifier: Intended Audience :: Developers
```

### Comparing `pyMAdot2-0.0.1/setup.py` & `pyMAdot2-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Setup module for pyMAdot2."""
 from pathlib import Path
 from setuptools import setup
 
 PROJECT_DIR = Path(__file__).parent.resolve()
 README_FILE = PROJECT_DIR / "README.md"
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 
 setup(
     name='pyMAdot2',
     version=VERSION,
     license="MIT",
     url="https://github.com/elektr0nisch/pyMAdot2",
     author="Linus Groschke",
```

