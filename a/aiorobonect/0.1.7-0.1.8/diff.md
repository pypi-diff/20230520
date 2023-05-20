# Comparing `tmp/aiorobonect-0.1.7.tar.gz` & `tmp/aiorobonect-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiorobonect-0.1.7.tar", last modified: Tue May 16 09:38:19 2023, max compression
+gzip compressed data, was "aiorobonect-0.1.8.tar", last modified: Sat May 20 15:57:04 2023, max compression
```

## Comparing `aiorobonect-0.1.7.tar` & `aiorobonect-0.1.8.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:38:19.097599 aiorobonect-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-16 09:37:54.000000 aiorobonect-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-16 09:38:19.097599 aiorobonect-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-16 09:37:54.000000 aiorobonect-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:38:19.097599 aiorobonect-0.1.7/aiorobonect/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-16 09:37:54.000000 aiorobonect-0.1.7/aiorobonect/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1257 2023-05-16 09:37:54.000000 aiorobonect-0.1.7/aiorobonect/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-16 09:37:54.000000 aiorobonect-0.1.7/aiorobonect/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-05-16 09:37:54.000000 aiorobonect-0.1.7/aiorobonect/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-16 09:37:54.000000 aiorobonect-0.1.7/aiorobonect/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:38:19.097599 aiorobonect-0.1.7/aiorobonect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-16 09:38:19.000000 aiorobonect-0.1.7/aiorobonect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-16 09:38:19.000000 aiorobonect-0.1.7/aiorobonect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 09:38:19.000000 aiorobonect-0.1.7/aiorobonect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 09:38:19.000000 aiorobonect-0.1.7/aiorobonect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-16 09:38:19.000000 aiorobonect-0.1.7/aiorobonect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 09:38:19.097599 aiorobonect-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-16 09:37:57.000000 aiorobonect-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 15:57:04.060212 aiorobonect-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-20 15:56:44.000000 aiorobonect-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-05-20 15:57:04.060212 aiorobonect-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-05-20 15:56:44.000000 aiorobonect-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 15:57:04.056212 aiorobonect-0.1.8/aiorobonect/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-20 15:56:44.000000 aiorobonect-0.1.8/aiorobonect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-05-20 15:56:44.000000 aiorobonect-0.1.8/aiorobonect/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-20 15:56:44.000000 aiorobonect-0.1.8/aiorobonect/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-20 15:56:44.000000 aiorobonect-0.1.8/aiorobonect/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 15:57:04.056212 aiorobonect-0.1.8/aiorobonect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-05-20 15:57:04.000000 aiorobonect-0.1.8/aiorobonect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-20 15:57:04.000000 aiorobonect-0.1.8/aiorobonect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 15:57:04.000000 aiorobonect-0.1.8/aiorobonect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-20 15:57:04.000000 aiorobonect-0.1.8/aiorobonect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-20 15:57:04.000000 aiorobonect-0.1.8/aiorobonect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 15:57:04.060212 aiorobonect-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-20 15:56:47.000000 aiorobonect-0.1.8/setup.py
```

### Comparing `aiorobonect-0.1.7/LICENSE` & `aiorobonect-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `aiorobonect-0.1.7/aiorobonect/rest.py` & `aiorobonect-0.1.8/aiorobonect/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     def __init__(self, host, username, password, transform_json=False) -> None:
         """Initialize the Communication API to get data."""
         self.auth = None
         self.host = host
         self.username = username
         self.password = password
         self.session = None
+        self.sleeping = None
         self.transform_json = transform_json
         if username is not None and password is not None:
             self.auth = aiohttp.BasicAuth(login=username, password=password)
 
     def session_start(self):
         """Start the aiohttp session."""
         if self.session:
@@ -64,22 +65,26 @@
             if response.status >= 400:
                 await self.session_close()
                 response.raise_for_status()
         if self.transform_json:
             return transform_json_to_single_depth(result)
         return result
 
-    async def async_cmds(self, commands=None) -> list[dict]:
+    async def async_cmds(self, commands=None, bypass_sleeping=False) -> list[dict]:
         """Send command to mower."""
         self.session_start()
         result = []
-        for cmd in commands:
-            result.append({cmd: await self.async_cmd(cmd)})
+        result.append({"status": await self.state()})
+        if not self.sleeping or bypass_sleeping:
+            for cmd in commands:
+                result.append({cmd: await self.async_cmd(cmd)})
         await self.session_close()
         return result
 
     async def state(self) -> list[dict]:
         """Send status command to mower."""
         self.session_start()
         result = await self.async_cmd("status")
+        self.sleeping = result.get("status").get("status") == 17
+        print(result.json)
         await self.session_close()
         return result
```

### Comparing `aiorobonect-0.1.7/setup.py` & `aiorobonect-0.1.8/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,9 +16,9 @@
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     install_requires=[val.strip() for val in open("requirements.txt")],
-    version="v0.1.7",
+    version="v0.1.8",
 )
```

