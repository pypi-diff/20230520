# Comparing `tmp/econuker-1.0.0.tar.gz` & `tmp/econuker-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "econuker-1.0.0.tar", last modified: Sat May 20 00:21:48 2023, max compression
+gzip compressed data, was "econuker-1.0.1.tar", last modified: Sat May 20 00:50:30 2023, max compression
```

## Comparing `econuker-1.0.0.tar` & `econuker-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 00:21:48.458214 econuker-1.0.0/
--rw-rw-rw-   0        0        0      819 2023-05-20 00:21:48.457215 econuker-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1361 2023-05-20 00:05:55.000000 econuker-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-20 00:21:48.449215 econuker-1.0.0/econuker/
--rw-rw-rw-   0        0        0     1368 2023-05-19 23:47:34.000000 econuker-1.0.0/econuker/Exceptions.py
--rw-rw-rw-   0        0        0      104 2023-05-20 00:09:50.000000 econuker-1.0.0/econuker/__init__.py
--rw-rw-rw-   0        0        0    14766 2023-05-20 00:21:18.000000 econuker-1.0.0/econuker/async_client.py
--rw-rw-rw-   0        0        0    14255 2023-05-20 00:19:32.000000 econuker-1.0.0/econuker/client.py
-drwxrwxrwx   0        0        0        0 2023-05-20 00:21:48.455214 econuker-1.0.0/econuker.egg-info/
--rw-rw-rw-   0        0        0      819 2023-05-20 00:21:48.000000 econuker-1.0.0/econuker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-05-20 00:21:48.000000 econuker-1.0.0/econuker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 00:21:48.000000 econuker-1.0.0/econuker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-20 00:21:48.000000 econuker-1.0.0/econuker.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-20 00:21:48.000000 econuker-1.0.0/econuker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-20 00:21:48.458214 econuker-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1037 2023-05-20 00:13:40.000000 econuker-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 00:50:30.465647 econuker-1.0.1/
+-rw-rw-rw-   0        0        0      819 2023-05-20 00:50:30.459652 econuker-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1363 2023-05-20 00:27:36.000000 econuker-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-20 00:50:30.091457 econuker-1.0.1/econuker/
+-rw-rw-rw-   0        0        0     1368 2023-05-19 23:47:34.000000 econuker-1.0.1/econuker/Exceptions.py
+-rw-rw-rw-   0        0        0      104 2023-05-20 00:09:50.000000 econuker-1.0.1/econuker/__init__.py
+-rw-rw-rw-   0        0        0    14765 2023-05-20 00:48:01.000000 econuker-1.0.1/econuker/async_client.py
+-rw-rw-rw-   0        0        0    14264 2023-05-20 00:48:27.000000 econuker-1.0.1/econuker/client.py
+drwxrwxrwx   0        0        0        0 2023-05-20 00:50:30.432663 econuker-1.0.1/econuker.egg-info/
+-rw-rw-rw-   0        0        0      819 2023-05-20 00:50:27.000000 econuker-1.0.1/econuker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-05-20 00:50:28.000000 econuker-1.0.1/econuker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 00:50:27.000000 econuker-1.0.1/econuker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-20 00:50:27.000000 econuker-1.0.1/econuker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-20 00:50:27.000000 econuker-1.0.1/econuker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-20 00:50:30.466643 econuker-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1037 2023-05-20 00:49:23.000000 econuker-1.0.1/setup.py
```

### Comparing `econuker-1.0.0/PKG-INFO` & `econuker-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: econuker
-Version: 1.0.0
+Version: 1.0.1
 Summary: API wrapper for https://api.econuker.xyz
 Home-page: https://github.com/EcoNuker/EcoNuker-API-Python/
 Author: YumYummity
 Author-email: 034nop@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Internet :: WWW/HTTP
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 
 A Python library for interacting with EcoNuker's API.
```

### Comparing `econuker-1.0.0/README.md` & `econuker-1.0.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 EcoNuker-API is a Python library for interacting with the EcoNuker API, which provides tools for managing and controlling Eco servers.
 
 ## Installation
 
 You can install the EcoNuker-API library using pip:
 
-`pip install econuker-api`
+`pip install econuker`
 
 ## Usage
 
 WARNING: The MAIN API is not available for use until June 1, 2023.
 
 Please use the BETA version. Beta=True.
 
@@ -25,15 +25,15 @@
 if __name__ == "__main__":
     client = Client(auth_token=authtoken, beta=beta)
     status = client.status()
     print(status.name)
 ```
 
 ### Async Example
-```
+```python
 # Python Async Example
 from econuker import AsyncClient
 beta = True # False
 authtoken = None # "your auth token here"
 
 if __name__ == "__main__":
     client = AsyncClient(auth_token=authtoken, beta=beta)
```

### Comparing `econuker-1.0.0/econuker/Exceptions.py` & `econuker-1.0.1/econuker/Exceptions.py`

 * *Files identical despite different names*

### Comparing `econuker-1.0.0/econuker/async_client.py` & `econuker-1.0.1/econuker/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import aiohttp, asyncio, requests
 from econuker.Exceptions import Forbidden, Unauthorized, NotFound, InternalServerError, RateLimited, EconukerException, InvalidAuthToken
 
 
-async def _handle_error(self, response):
+async def _handle_error(response):
     """
     Handles the error responses from API requests.
 
     Args:
         response (aiohttp.ClientResponse): The response object from the API request.
 
     Raises:
@@ -326,15 +326,15 @@
             self.id: str = list(data.keys())[0]
             self.name: str = self._data[0]
             self.rarity: str = self._data[1]
             self.description: str = self._data[2]
             self.desc: str = self._data[2]
             self.aliases: list = self._data[3]
             self._extradata: str = self._data[4]
-            self.price: ItemPrice = self.ItemPrice(self._data[5])
+            self.price: self.ItemPrice = self.ItemPrice(self._data[5])
             self.price.worth: str = self._data[6]
 
     async def fetch_items(self, hidden: bool = True) -> ItemsResult:
         """
         Fetches all items.
 
         Args:
```

### Comparing `econuker-1.0.0/econuker/client.py` & `econuker-1.0.1/econuker/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import requests
 from econuker.Exceptions import Forbidden, Unauthorized, NotFound, InternalServerError, RateLimited, EconukerException, InvalidAuthToken
 
 
-def _handle_error(self, response):
+def _handle_error(response):
     """
     Handles the error responses from API requests.
 
     Args:
         response (requests.Response): The response object from the API request.
 
     Raises:
@@ -224,15 +224,15 @@
                     self.id = data["id"]
                     self.nick = data.get("nick")
                     self.profile = data.get("profile")
 
             self._raw: dict = data
             self.id: str = data["id"]
             self.name: str = data["name"]
-            self.owner: Owner = Owner(data["owner"])
+            self.owner: self.Owner = self.Owner(data["owner"])
             self.url: str = data["vanity_url"]
             self.verified: bool = data["verified"]
             self.created_at: int = data["created_at"]
             self.timezone: str = data["timezone"]
             self.slug: str = data["slug"]
             self.about: str = data["about"]
     
@@ -324,15 +324,15 @@
             self.id: str = list(data.keys())[0]
             self.name: str = self._data[0]
             self.rarity: str = self._data[1]
             self.description: str = self._data[2]
             self.desc: str = self._data[2]
             self.aliases: list = self._data[3]
             self._extradata: str = self._data[4]
-            self.price: ItemPrice = self.ItemPrice(self._data[5])
+            self.price: self.ItemPrice = self.ItemPrice(self._data[5])
             self.price.worth: str = self._data[6]
 
     def fetch_items(self, hidden:bool=True) -> ItemsResult:
         """
         Fetches all items.
 
         Args:
```

### Comparing `econuker-1.0.0/econuker.egg-info/PKG-INFO` & `econuker-1.0.1/econuker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: econuker
-Version: 1.0.0
+Version: 1.0.1
 Summary: API wrapper for https://api.econuker.xyz
 Home-page: https://github.com/EcoNuker/EcoNuker-API-Python/
 Author: YumYummity
 Author-email: 034nop@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Internet :: WWW/HTTP
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 
 A Python library for interacting with EcoNuker's API.
```

### Comparing `econuker-1.0.0/setup.py` & `econuker-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='econuker',
-    version='1.0.0',
+    version='1.0.1',
     author='YumYummity',
     author_email='034nop@gmail.com',
     description='API wrapper for https://api.econuker.xyz',
     long_description='A Python library for interacting with EcoNuker\'s API.',
     url='https://github.com/EcoNuker/EcoNuker-API-Python/',
     packages=find_packages(),
     classifiers=[
@@ -17,13 +17,13 @@
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Topic :: Internet :: WWW/HTTP',
     ],
-    python_requires='>=3.8',
+    python_requires='>=3.9',
     install_requires=[
         'requests',
         'aiohttp'
     ],
 )
```

