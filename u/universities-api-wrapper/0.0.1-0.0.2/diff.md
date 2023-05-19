# Comparing `tmp/universities-api-wrapper-0.0.1.tar.gz` & `tmp/universities-api-wrapper-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "universities-api-wrapper-0.0.1.tar", last modified: Wed Mar  8 23:16:04 2023, max compression
+gzip compressed data, was "universities-api-wrapper-0.0.2.tar", last modified: Fri May 19 23:37:43 2023, max compression
```

## Comparing `universities-api-wrapper-0.0.1.tar` & `universities-api-wrapper-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 juha      (1000) juha      (1000)        0 2023-03-08 23:16:04.054969 universities-api-wrapper-0.0.1/
--rw-r--r--   0 juha      (1000) juha      (1000)     1076 2023-02-27 23:06:02.000000 universities-api-wrapper-0.0.1/LICENSE.txt
--rw-r--r--   0 juha      (1000) juha      (1000)      782 2023-03-08 23:16:04.054969 universities-api-wrapper-0.0.1/PKG-INFO
--rw-r--r--   0 juha      (1000) juha      (1000)     1598 2023-03-06 22:55:48.000000 universities-api-wrapper-0.0.1/README.md
--rw-r--r--   0 juha      (1000) juha      (1000)       79 2023-03-08 23:16:04.054969 universities-api-wrapper-0.0.1/setup.cfg
--rw-r--r--   0 juha      (1000) juha      (1000)     1097 2023-03-08 23:12:54.000000 universities-api-wrapper-0.0.1/setup.py
-drwxr-xr-x   0 juha      (1000) juha      (1000)        0 2023-03-08 23:16:04.050969 universities-api-wrapper-0.0.1/universities_api_wrapper/
--rw-r--r--   0 juha      (1000) juha      (1000)     1868 2023-03-01 23:33:37.000000 universities-api-wrapper-0.0.1/universities_api_wrapper/__init__.py
-drwxr-xr-x   0 juha      (1000) juha      (1000)        0 2023-03-08 23:16:04.053969 universities-api-wrapper-0.0.1/universities_api_wrapper.egg-info/
--rw-r--r--   0 juha      (1000) juha      (1000)      782 2023-03-08 23:16:03.000000 universities-api-wrapper-0.0.1/universities_api_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 juha      (1000) juha      (1000)      316 2023-03-08 23:16:03.000000 universities-api-wrapper-0.0.1/universities_api_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 juha      (1000) juha      (1000)        1 2023-03-08 23:16:03.000000 universities-api-wrapper-0.0.1/universities_api_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 juha      (1000) juha      (1000)       14 2023-03-08 23:16:03.000000 universities-api-wrapper-0.0.1/universities_api_wrapper.egg-info/requires.txt
--rw-r--r--   0 juha      (1000) juha      (1000)       25 2023-03-08 23:16:03.000000 universities-api-wrapper-0.0.1/universities_api_wrapper.egg-info/top_level.txt
+drwxr-xr-x   0 juha      (1000) juha      (1000)        0 2023-05-19 23:37:43.189533 universities-api-wrapper-0.0.2/
+-rw-r--r--   0 juha      (1000) juha      (1000)     1076 2023-02-27 23:06:02.000000 universities-api-wrapper-0.0.2/LICENSE.txt
+-rw-r--r--   0 juha      (1000) juha      (1000)      746 2023-05-19 23:37:43.190533 universities-api-wrapper-0.0.2/PKG-INFO
+-rw-r--r--   0 juha      (1000) juha      (1000)     2038 2023-04-18 23:02:26.000000 universities-api-wrapper-0.0.2/README.md
+-rw-r--r--   0 juha      (1000) juha      (1000)      106 2023-05-19 23:37:43.190533 universities-api-wrapper-0.0.2/setup.cfg
+-rw-r--r--   0 juha      (1000) juha      (1000)     1097 2023-05-19 23:28:21.000000 universities-api-wrapper-0.0.2/setup.py
+drwxr-xr-x   0 juha      (1000) juha      (1000)        0 2023-05-19 23:37:43.185533 universities-api-wrapper-0.0.2/tests/
+-rw-r--r--   0 juha      (1000) juha      (1000)     1618 2023-04-18 23:02:26.000000 universities-api-wrapper-0.0.2/tests/test_universities_api_wrapper.py
+drwxr-xr-x   0 juha      (1000) juha      (1000)        0 2023-05-19 23:37:43.186533 universities-api-wrapper-0.0.2/universities_api_wrapper/
+-rw-r--r--   0 juha      (1000) juha      (1000)     1956 2023-04-18 23:02:26.000000 universities-api-wrapper-0.0.2/universities_api_wrapper/__init__.py
+drwxr-xr-x   0 juha      (1000) juha      (1000)        0 2023-05-19 23:37:43.189533 universities-api-wrapper-0.0.2/universities_api_wrapper.egg-info/
+-rw-r--r--   0 juha      (1000) juha      (1000)      746 2023-05-19 23:37:42.000000 universities-api-wrapper-0.0.2/universities_api_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 juha      (1000) juha      (1000)      355 2023-05-19 23:37:43.000000 universities-api-wrapper-0.0.2/universities_api_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 juha      (1000) juha      (1000)        1 2023-05-19 23:37:42.000000 universities-api-wrapper-0.0.2/universities_api_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 juha      (1000) juha      (1000)       14 2023-05-19 23:37:42.000000 universities-api-wrapper-0.0.2/universities_api_wrapper.egg-info/requires.txt
+-rw-r--r--   0 juha      (1000) juha      (1000)       25 2023-05-19 23:37:42.000000 universities-api-wrapper-0.0.2/universities_api_wrapper.egg-info/top_level.txt
```

### Comparing `universities-api-wrapper-0.0.1/LICENSE.txt` & `universities-api-wrapper-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `universities-api-wrapper-0.0.1/PKG-INFO` & `universities-api-wrapper-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 Metadata-Version: 2.1
 Name: universities-api-wrapper
-Version: 0.0.1
+Version: 0.0.2
 Summary: Universities API Wrapper
 Home-page: https://github.com/jremes-foss/universities-api-wrapper/
+Download-URL: https://github.com/jremes-foss/universities-api-wrapper/archive/refs/tags/0.0.2.tar.gz
 Author: Juha Remes
 Author-email: jremes@outlook.com
-License: UNKNOWN
-Download-URL: https://github.com/jremes-foss/universities-api-wrapper/archive/refs/tags/0.0.1.tar.gz
 Keywords: python,api,wrapper,education,universities
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 License-File: LICENSE.txt
 
 Python package for consuming universities-domains-list API
-
```

### Comparing `universities-api-wrapper-0.0.1/README.md` & `universities-api-wrapper-0.0.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Universities API Wrapper
+[![Downloads](https://static.pepy.tech/badge/universities-api-wrapper)](https://pepy.tech/project/universities-api-wrapper)
 
-This is a small API wrapper designed to consume [Universities API](https://github.com/Hipo/university-domains-list-api) from Python command line. API consumer was built as a project to build first Python library. 
+This is a small API wrapper designed to consume [Universities API](https://github.com/Hipo/university-domains-list-api) by [Hipo](http://hipolabs.com/). from Python command line. API consumer was built as a project to build first Python library.
 
 ## Requirements
 
 This package requires [requests](https://pypi.org/project/requests/) package to function properly.
 
 ## Installation
 
@@ -16,34 +17,46 @@
 python setup.py install
 ```
 
 ### PyPI installation
 
 Alternatively, you can install package via PyPI `pip` package manager.
 
+```bash
+pip install universities-api-wrapper
+```
+
 ## Usage
 
 Once installed, you can use wrapper the following way. First, instantiate the library.
 
 ```python
 from universities_api_wrapper import HipolabsUniversitiesAPI
 ```
 
 Then initialize the client. If you are using local connection only:
 
 ```python
 client = HipolabsUniversitiesAPI("local")
 ```
 
+By default, local connector is attempting to connect port `8080/tcp`.
+
 Alternatively, if you wish to use remote connection:
 
 ```python
 client = HipolabsUniversitiesAPI("remote")
 ```
 
+If you wish to use alternative port, for example, `8888/tcp`, you can invoke connector like this:
+
+```python
+client = HipolabsUniversitiesAPI("remote", 8888)
+```
+
 If you pass anything else, library will raise `UniversitiesAPIError`.
 
 Client has now been initialized. Let's start searching.
 
 ### Search by Country
 
 ```python
```

### Comparing `universities-api-wrapper-0.0.1/setup.py` & `universities-api-wrapper-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Universities API Wrapper'
 LONG_DESCRIPTION = 'Python package for consuming universities-domains-list API'
 
 # Setting up
 setup(
         name="universities-api-wrapper",
         version=VERSION,
         author="Juha Remes",
         author_email="jremes@outlook.com",
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         packages=find_packages(),
         url='https://github.com/jremes-foss/universities-api-wrapper/',
-        download_url='https://github.com/jremes-foss/universities-api-wrapper/archive/refs/tags/0.0.1.tar.gz',
+        download_url='https://github.com/jremes-foss/universities-api-wrapper/archive/refs/tags/0.0.2.tar.gz',
         install_requires=['requests', 'mock'],
         keywords=['python', 'api', 'wrapper', 'education', 'universities'],
         classifiers= [
             "Development Status :: 3 - Alpha",
             "Intended Audience :: Education",
             "Programming Language :: Python :: 2",
             "Programming Language :: Python :: 3",
```

### Comparing `universities-api-wrapper-0.0.1/universities_api_wrapper/__init__.py` & `universities-api-wrapper-0.0.2/universities_api_wrapper/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,25 +6,26 @@
 from requests import Response
 
 # Set up logger
 logging.basicConfig(level="INFO")
 logger = logging.getLogger(__name__)
 
 class HipolabsUniversitiesAPI:
-    """ Main class for API wrapper"""
-    def __init__(self, method):
+    """ Main class for API wrapper. """
+    def __init__(self, method, port=8080):
         self.method = method
+        self.port = port if port is not None else 8080
 
     @staticmethod
-    def _get_method(method):
+    def _get_method(method, port):
         """ Selects the connection method, either remote or local. """
         if method == 'remote':
             return "http://universities.hipolabs.com/search"
         elif method == "local":
-            return "http://127.0.0.1:5000/search"
+            return f"http://127.0.0.1:{port}/search"
         else:
             raise UniversitiesAPIError("Unknown method!")
 
     @staticmethod
     def _check_online(response: Response) -> None:
         """ Checks if API endpoint is online. """
         if response.status_code != 200:
@@ -36,15 +37,15 @@
     def endpoints():
         """ Returns endpoints of universities API. """
         return ["name", "country"]
 
     def search(self, country=None, name=None) -> dict:
         """ This method searches by name and country. """
 
-        base_url = self._get_method(self.method)
+        base_url = self._get_method(self.method, self.port)
 
         if not country and not name:
             raise ValueError("Please provide valid university name or country.")
         elif not name:
             url = f"{base_url}?country={country.lower()}"
         elif not country:
             url = f"{base_url}?name={name.lower()}"
```

### Comparing `universities-api-wrapper-0.0.1/universities_api_wrapper.egg-info/PKG-INFO` & `universities-api-wrapper-0.0.2/universities_api_wrapper.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 Metadata-Version: 2.1
 Name: universities-api-wrapper
-Version: 0.0.1
+Version: 0.0.2
 Summary: Universities API Wrapper
 Home-page: https://github.com/jremes-foss/universities-api-wrapper/
+Download-URL: https://github.com/jremes-foss/universities-api-wrapper/archive/refs/tags/0.0.2.tar.gz
 Author: Juha Remes
 Author-email: jremes@outlook.com
-License: UNKNOWN
-Download-URL: https://github.com/jremes-foss/universities-api-wrapper/archive/refs/tags/0.0.1.tar.gz
 Keywords: python,api,wrapper,education,universities
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 License-File: LICENSE.txt
 
 Python package for consuming universities-domains-list API
-
```

