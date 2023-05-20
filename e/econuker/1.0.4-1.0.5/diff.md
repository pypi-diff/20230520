# Comparing `tmp/econuker-1.0.4.tar.gz` & `tmp/econuker-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "econuker-1.0.4.tar", last modified: Sat May 20 01:51:33 2023, max compression
+gzip compressed data, was "econuker-1.0.5.tar", last modified: Sat May 20 01:55:10 2023, max compression
```

## Comparing `econuker-1.0.4.tar` & `econuker-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 01:51:33.234233 econuker-1.0.4/
--rw-rw-rw-   0        0        0      819 2023-05-20 01:51:33.234233 econuker-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2612 2023-05-20 01:22:57.000000 econuker-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-20 01:51:33.226232 econuker-1.0.4/econuker/
--rw-rw-rw-   0        0        0     1368 2023-05-19 23:47:34.000000 econuker-1.0.4/econuker/Exceptions.py
--rw-rw-rw-   0        0        0      104 2023-05-20 00:09:50.000000 econuker-1.0.4/econuker/__init__.py
--rw-rw-rw-   0        0        0    14431 2023-05-20 01:50:55.000000 econuker-1.0.4/econuker/async_client.py
--rw-rw-rw-   0        0        0    13922 2023-05-20 01:51:03.000000 econuker-1.0.4/econuker/client.py
-drwxrwxrwx   0        0        0        0 2023-05-20 01:51:33.232232 econuker-1.0.4/econuker.egg-info/
--rw-rw-rw-   0        0        0      819 2023-05-20 01:51:33.000000 econuker-1.0.4/econuker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-05-20 01:51:33.000000 econuker-1.0.4/econuker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 01:51:33.000000 econuker-1.0.4/econuker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-20 01:51:33.000000 econuker-1.0.4/econuker.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-20 01:51:33.000000 econuker-1.0.4/econuker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-20 01:51:33.234233 econuker-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1037 2023-05-20 01:50:43.000000 econuker-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 01:55:10.973782 econuker-1.0.5/
+-rw-rw-rw-   0        0        0      819 2023-05-20 01:55:10.972761 econuker-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2612 2023-05-20 01:22:57.000000 econuker-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-20 01:55:10.965749 econuker-1.0.5/econuker/
+-rw-rw-rw-   0        0        0     1368 2023-05-19 23:47:34.000000 econuker-1.0.5/econuker/Exceptions.py
+-rw-rw-rw-   0        0        0      104 2023-05-20 00:09:50.000000 econuker-1.0.5/econuker/__init__.py
+-rw-rw-rw-   0        0        0    14446 2023-05-20 01:54:12.000000 econuker-1.0.5/econuker/async_client.py
+-rw-rw-rw-   0        0        0    13937 2023-05-20 01:53:50.000000 econuker-1.0.5/econuker/client.py
+drwxrwxrwx   0        0        0        0 2023-05-20 01:55:10.971750 econuker-1.0.5/econuker.egg-info/
+-rw-rw-rw-   0        0        0      819 2023-05-20 01:55:10.000000 econuker-1.0.5/econuker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-05-20 01:55:10.000000 econuker-1.0.5/econuker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 01:55:10.000000 econuker-1.0.5/econuker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-20 01:55:10.000000 econuker-1.0.5/econuker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-20 01:55:10.000000 econuker-1.0.5/econuker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-20 01:55:10.973782 econuker-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1037 2023-05-20 01:54:54.000000 econuker-1.0.5/setup.py
```

### Comparing `econuker-1.0.4/PKG-INFO` & `econuker-1.0.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: econuker
-Version: 1.0.4
+Version: 1.0.5
 Summary: API wrapper for https://api.econuker.xyz
 Home-page: https://github.com/EcoNuker/EcoNuker-API-Python/
 Author: YumYummity
 Author-email: 034nop@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `econuker-1.0.4/README.md` & `econuker-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `econuker-1.0.4/econuker/Exceptions.py` & `econuker-1.0.5/econuker/Exceptions.py`

 * *Files identical despite different names*

### Comparing `econuker-1.0.4/econuker/async_client.py` & `econuker-1.0.5/econuker/async_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,24 +105,25 @@
         self.auth_token: str = auth_token
         self.base_url: str = "https://beta.econuker.xyz/api" if beta else "https://api.econuker.xyz"
         self.auth_level: str = None
 
         if not beta:
             raise EconukerException("Main API is not available at this moment.")
 
-        def __check_verify(self, auth_token) -> Token:
+        def __check_verify(self) -> Token:
             """
             Verifies an authentication token.
 
             Args:
                 auth_token (str): The authentication token to verify.
 
             Returns:
                 Token: A Token object if the token is valid, False otherwise.
             """
+            auth_token = self.auth_token
             url = self.base_url + f"/auth/verify/{auth_token}"
             response = requests.get(url)
             if response.status_code == 200:
                 data = response.json()
                 self.auth_token = data["token"]
                 self.auth_level = data["authlevel"]
                 return Token(self.auth_token, self.auth_level, data)
@@ -130,15 +131,15 @@
                 return False
             else:
                 _handle_error(response)
     
         self.__check_verify = lambda: __check_verify(self)
 
         if self.auth_token is not None:
-            token = self.__check_verify(self.auth_token)
+            token = self.__check_verify()
             if token is False:
                 raise InvalidAuthToken("Invalid auth_token provided.")
             else:
                 self.auth_level = token.authlevel
 
 
     async def ping(self) -> bool:
```

### Comparing `econuker-1.0.4/econuker/client.py` & `econuker-1.0.5/econuker/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,24 +104,25 @@
         self.auth_token: str = auth_token
         self.base_url: str = "https://beta.econuker.xyz/api" if beta else "https://api.econuker.xyz"
         self.auth_level: str = None
 
         if not beta:
             raise EconukerException("Main API is not available at this moment.")
 
-        def __check_verify(self, auth_token) -> Token:
+        def __check_verify(self) -> Token:
             """
             Verifies an authentication token.
 
             Args:
                 auth_token (str): The authentication token to verify.
 
             Returns:
                 Token: A Token object if the token is valid, False otherwise.
             """
+            auth_token = self.auth_token
             url = self.base_url + f"/auth/verify/{auth_token}"
             response = requests.get(url)
             if response.status_code == 200:
                 data = response.json()
                 self.auth_token = data["token"]
                 self.auth_level = data["authlevel"]
                 return Token(self.auth_token, self.auth_level, data)
@@ -129,15 +130,15 @@
                 return False
             else:
                 _handle_error(response)
     
         self.__check_verify = lambda: __check_verify(self)
 
         if self.auth_token is not None:
-            token = self.__check_verify(self.auth_token)
+            token = self.__check_verify()
             if token is False:
                 raise InvalidAuthToken("Invalid auth_token provided.")
             else:
                 self.auth_level = token.authlevel
 
     class StatusData:
         """
```

### Comparing `econuker-1.0.4/econuker.egg-info/PKG-INFO` & `econuker-1.0.5/econuker.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: econuker
-Version: 1.0.4
+Version: 1.0.5
 Summary: API wrapper for https://api.econuker.xyz
 Home-page: https://github.com/EcoNuker/EcoNuker-API-Python/
 Author: YumYummity
 Author-email: 034nop@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `econuker-1.0.4/setup.py` & `econuker-1.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='econuker',
-    version='1.0.4',
+    version='1.0.5',
     author='YumYummity',
     author_email='034nop@gmail.com',
     description='API wrapper for https://api.econuker.xyz',
     long_description='A Python library for interacting with EcoNuker\'s API.',
     url='https://github.com/EcoNuker/EcoNuker-API-Python/',
     packages=find_packages(),
     classifiers=[
```

