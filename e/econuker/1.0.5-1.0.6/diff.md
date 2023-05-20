# Comparing `tmp/econuker-1.0.5.tar.gz` & `tmp/econuker-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "econuker-1.0.5.tar", last modified: Sat May 20 01:55:10 2023, max compression
+gzip compressed data, was "econuker-1.0.6.tar", last modified: Sat May 20 15:47:10 2023, max compression
```

## Comparing `econuker-1.0.5.tar` & `econuker-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 01:55:10.973782 econuker-1.0.5/
--rw-rw-rw-   0        0        0      819 2023-05-20 01:55:10.972761 econuker-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2612 2023-05-20 01:22:57.000000 econuker-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-20 01:55:10.965749 econuker-1.0.5/econuker/
--rw-rw-rw-   0        0        0     1368 2023-05-19 23:47:34.000000 econuker-1.0.5/econuker/Exceptions.py
--rw-rw-rw-   0        0        0      104 2023-05-20 00:09:50.000000 econuker-1.0.5/econuker/__init__.py
--rw-rw-rw-   0        0        0    14446 2023-05-20 01:54:12.000000 econuker-1.0.5/econuker/async_client.py
--rw-rw-rw-   0        0        0    13937 2023-05-20 01:53:50.000000 econuker-1.0.5/econuker/client.py
-drwxrwxrwx   0        0        0        0 2023-05-20 01:55:10.971750 econuker-1.0.5/econuker.egg-info/
--rw-rw-rw-   0        0        0      819 2023-05-20 01:55:10.000000 econuker-1.0.5/econuker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-05-20 01:55:10.000000 econuker-1.0.5/econuker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 01:55:10.000000 econuker-1.0.5/econuker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-20 01:55:10.000000 econuker-1.0.5/econuker.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-20 01:55:10.000000 econuker-1.0.5/econuker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-20 01:55:10.973782 econuker-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1037 2023-05-20 01:54:54.000000 econuker-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 15:47:10.447713 econuker-1.0.6/
+-rw-rw-rw-   0        0        0      819 2023-05-20 15:47:10.446714 econuker-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2612 2023-05-20 01:22:57.000000 econuker-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-20 15:47:10.437711 econuker-1.0.6/econuker/
+-rw-rw-rw-   0        0        0     1368 2023-05-19 23:47:34.000000 econuker-1.0.6/econuker/Exceptions.py
+-rw-rw-rw-   0        0        0      104 2023-05-20 00:09:50.000000 econuker-1.0.6/econuker/__init__.py
+-rw-rw-rw-   0        0        0    14456 2023-05-20 15:46:49.000000 econuker-1.0.6/econuker/async_client.py
+-rw-rw-rw-   0        0        0    13947 2023-05-20 15:45:37.000000 econuker-1.0.6/econuker/client.py
+drwxrwxrwx   0        0        0        0 2023-05-20 15:47:10.444710 econuker-1.0.6/econuker.egg-info/
+-rw-rw-rw-   0        0        0      819 2023-05-20 15:47:10.000000 econuker-1.0.6/econuker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-05-20 15:47:10.000000 econuker-1.0.6/econuker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 15:47:10.000000 econuker-1.0.6/econuker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-20 15:47:10.000000 econuker-1.0.6/econuker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-20 15:47:10.000000 econuker-1.0.6/econuker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-20 15:47:10.448712 econuker-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1037 2023-05-20 15:47:02.000000 econuker-1.0.6/setup.py
```

### Comparing `econuker-1.0.5/PKG-INFO` & `econuker-1.0.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: econuker
-Version: 1.0.5
+Version: 1.0.6
 Summary: API wrapper for https://api.econuker.xyz
 Home-page: https://github.com/EcoNuker/EcoNuker-API-Python/
 Author: YumYummity
 Author-email: 034nop@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `econuker-1.0.5/README.md` & `econuker-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `econuker-1.0.5/econuker/Exceptions.py` & `econuker-1.0.6/econuker/Exceptions.py`

 * *Files identical despite different names*

### Comparing `econuker-1.0.5/econuker/async_client.py` & `econuker-1.0.6/econuker/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,14 +94,15 @@
     """
     Base AsyncClient class for interacting with the EcoNuker API.
 
     WARNING: Until June 1, 2023, the Main API cannot be used.
 
     Args:
         auth_token (str, optional): The authentication token. Can be None. Must be valid. Defaults to None.
+        
         beta (bool, optional): Whether or not to use the BETA API. Defaults to False.
     """
 
     def __init__(self, auth_token: str = None, beta: bool = False):
         self.auth_token: str = auth_token
         self.base_url: str = "https://beta.econuker.xyz/api" if beta else "https://api.econuker.xyz"
         self.auth_level: str = None
```

### Comparing `econuker-1.0.5/econuker/client.py` & `econuker-1.0.6/econuker/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,14 +93,15 @@
     """
     Base Client class for interacting with the EcoNuker API.
 
     WARNING: Until June 1, 2023, the Main API cannot be used.
 
     Args:
         auth_token (str, optional): The authentication token. Can be None. Must be valid. Defaults to None.
+        
         beta (bool, optional): Whether or not to use the BETA API. Defaults to False.
     """
 
     def __init__(self, auth_token: str = None, beta: bool = False):
         self.auth_token: str = auth_token
         self.base_url: str = "https://beta.econuker.xyz/api" if beta else "https://api.econuker.xyz"
         self.auth_level: str = None
@@ -287,15 +288,15 @@
         if self.auth_level and self.auth_level.lower() not in ["trusted", "admin"]:
             raise Forbidden("Insufficient authorization level to fetch server details.")
         url = self.base_url + f"/server/{id}"
         headers = {"authorization": self.auth_token} if self.auth_token else {}
         response = requests.get(url, headers=headers)
         if response.status_code == 200:
             data = response.json()
-            return self.serverResult(data)
+            return self.ServerResult(data)
         else:
             _handle_error(response)
 
     class ItemsResult:
         """
         ItemsResult object.
```

### Comparing `econuker-1.0.5/econuker.egg-info/PKG-INFO` & `econuker-1.0.6/econuker.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: econuker
-Version: 1.0.5
+Version: 1.0.6
 Summary: API wrapper for https://api.econuker.xyz
 Home-page: https://github.com/EcoNuker/EcoNuker-API-Python/
 Author: YumYummity
 Author-email: 034nop@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `econuker-1.0.5/setup.py` & `econuker-1.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='econuker',
-    version='1.0.5',
+    version='1.0.6',
     author='YumYummity',
     author_email='034nop@gmail.com',
     description='API wrapper for https://api.econuker.xyz',
     long_description='A Python library for interacting with EcoNuker\'s API.',
     url='https://github.com/EcoNuker/EcoNuker-API-Python/',
     packages=find_packages(),
     classifiers=[
```

