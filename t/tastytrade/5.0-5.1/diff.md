# Comparing `tmp/tastytrade-5.0.tar.gz` & `tmp/tastytrade-5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tastytrade-5.0.tar", last modified: Sat May 20 06:11:59 2023, max compression
+gzip compressed data, was "tastytrade-5.1.tar", last modified: Sat May 20 16:53:07 2023, max compression
```

## Comparing `tastytrade-5.0.tar` & `tastytrade-5.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:11:59.488858 tastytrade-5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-20 06:11:49.000000 tastytrade-5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7463 2023-05-20 06:11:59.488858 tastytrade-5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7177 2023-05-20 06:11:49.000000 tastytrade-5.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 06:11:59.488858 tastytrade-5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-20 06:11:49.000000 tastytrade-5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:11:59.484858 tastytrade-5.0/tastytrade/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-20 06:11:49.000000 tastytrade-5.0/tastytrade/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34247 2023-05-20 06:11:49.000000 tastytrade-5.0/tastytrade/account.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:11:59.488858 tastytrade-5.0/tastytrade/dxfeed/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-20 06:11:49.000000 tastytrade-5.0/tastytrade/dxfeed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-20 06:11:49.000000 tastytrade-5.0/tastytrade/dxfeed/candle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-20 06:11:49.000000 tastytrade-5.0/tastytrade/dxfeed/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-20 06:11:49.000000 tastytrade-5.0/tastytrade/dxfeed/greeks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-20 06:11:49.000000 tastytrade-5.0/tastytrade/dxfeed/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-20 06:11:49.000000 tastytrade-5.0/tastytrade/dxfeed/quote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-20 06:11:49.000000 tastytrade-5.0/tastytrade/dxfeed/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-20 06:11:49.000000 tastytrade-5.0/tastytrade/dxfeed/theoprice.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-20 06:11:49.000000 tastytrade-5.0/tastytrade/dxfeed/trade.py
--rw-r--r--   0 runner    (1001) docker     (123)    30051 2023-05-20 06:11:49.000000 tastytrade-5.0/tastytrade/instruments.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-05-20 06:11:49.000000 tastytrade-5.0/tastytrade/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     9056 2023-05-20 06:11:49.000000 tastytrade-5.0/tastytrade/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-20 06:11:49.000000 tastytrade-5.0/tastytrade/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-05-20 06:11:49.000000 tastytrade-5.0/tastytrade/session.py
--rw-r--r--   0 runner    (1001) docker     (123)    18754 2023-05-20 06:11:49.000000 tastytrade-5.0/tastytrade/streamer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-20 06:11:49.000000 tastytrade-5.0/tastytrade/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-05-20 06:11:49.000000 tastytrade-5.0/tastytrade/watchlists.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:11:59.488858 tastytrade-5.0/tastytrade.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7463 2023-05-20 06:11:59.000000 tastytrade-5.0/tastytrade.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-20 06:11:59.000000 tastytrade-5.0/tastytrade.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 06:11:59.000000 tastytrade-5.0/tastytrade.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-20 06:11:59.000000 tastytrade-5.0/tastytrade.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-20 06:11:59.000000 tastytrade-5.0/tastytrade.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 16:53:07.861299 tastytrade-5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-20 16:52:54.000000 tastytrade-5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-05-20 16:53:07.861299 tastytrade-5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7177 2023-05-20 16:52:54.000000 tastytrade-5.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 16:53:07.861299 tastytrade-5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-20 16:52:54.000000 tastytrade-5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 16:53:07.857299 tastytrade-5.1/tastytrade/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-20 16:52:54.000000 tastytrade-5.1/tastytrade/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34247 2023-05-20 16:52:54.000000 tastytrade-5.1/tastytrade/account.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 16:53:07.861299 tastytrade-5.1/tastytrade/dxfeed/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-20 16:52:54.000000 tastytrade-5.1/tastytrade/dxfeed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-20 16:52:54.000000 tastytrade-5.1/tastytrade/dxfeed/candle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-20 16:52:54.000000 tastytrade-5.1/tastytrade/dxfeed/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-20 16:52:54.000000 tastytrade-5.1/tastytrade/dxfeed/greeks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-20 16:52:54.000000 tastytrade-5.1/tastytrade/dxfeed/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-20 16:52:54.000000 tastytrade-5.1/tastytrade/dxfeed/quote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-20 16:52:54.000000 tastytrade-5.1/tastytrade/dxfeed/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-20 16:52:54.000000 tastytrade-5.1/tastytrade/dxfeed/theoprice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-20 16:52:54.000000 tastytrade-5.1/tastytrade/dxfeed/trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30051 2023-05-20 16:52:54.000000 tastytrade-5.1/tastytrade/instruments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-05-20 16:52:54.000000 tastytrade-5.1/tastytrade/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9056 2023-05-20 16:52:54.000000 tastytrade-5.1/tastytrade/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-20 16:52:54.000000 tastytrade-5.1/tastytrade/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-05-20 16:52:54.000000 tastytrade-5.1/tastytrade/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18754 2023-05-20 16:52:54.000000 tastytrade-5.1/tastytrade/streamer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-20 16:52:54.000000 tastytrade-5.1/tastytrade/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-05-20 16:52:54.000000 tastytrade-5.1/tastytrade/watchlists.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 16:53:07.861299 tastytrade-5.1/tastytrade.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-05-20 16:53:07.000000 tastytrade-5.1/tastytrade.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-20 16:53:07.000000 tastytrade-5.1/tastytrade.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 16:53:07.000000 tastytrade-5.1/tastytrade.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-20 16:53:07.000000 tastytrade-5.1/tastytrade.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-20 16:53:07.000000 tastytrade-5.1/tastytrade.egg-info/top_level.txt
```

### Comparing `tastytrade-5.0/LICENSE` & `tastytrade-5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tastytrade-5.0/PKG-INFO` & `tastytrade-5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: tastytrade
-Version: 5.0
+Version: 5.1
 Summary: An unofficial SDK for Tastytrade!
 Home-page: https://github.com/tastyware/tastytrade
 Author: Graeme Holliday
 Author-email: graeme.holliday@pm.me
-License: Apache
-Description-Content-Type: text/markdown
+License: MIT
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 .. image:: https://readthedocs.org/projects/tastyworks-api/badge/?version=latest
    :target: https://tastyworks-api.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
 
 .. image:: https://img.shields.io/pypi/v/tastytrade
```

### Comparing `tastytrade-5.0/README.rst` & `tastytrade-5.1/README.rst`

 * *Files identical despite different names*

### Comparing `tastytrade-5.0/setup.py` & `tastytrade-5.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 f.close()
 
 setup(
     name='tastytrade',
     version=VERSION,
     description='An unofficial SDK for Tastytrade!',
     long_description=LONG_DESCRIPTION,
-    long_description_content_type='text/markdown',
+    long_description_content_type='text/x-rst',
     author='Graeme Holliday',
     author_email='graeme.holliday@pm.me',
     url='https://github.com/tastyware/tastytrade',
-    license='Apache',
+    license='MIT',
     install_requires=[
         'requests<3',
         'dataclasses',
         'websockets>=11.0.3',
         'pydantic>=1.10.7'
     ],
     packages=find_packages(exclude=['ez_setup', 'tests*']),
-    include_package_data=True,
+    include_package_data=True
 )
```

### Comparing `tastytrade-5.0/tastytrade/account.py` & `tastytrade-5.1/tastytrade/account.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.0/tastytrade/dxfeed/candle.py` & `tastytrade-5.1/tastytrade/dxfeed/candle.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.0/tastytrade/dxfeed/event.py` & `tastytrade-5.1/tastytrade/dxfeed/event.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.0/tastytrade/dxfeed/greeks.py` & `tastytrade-5.1/tastytrade/dxfeed/greeks.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.0/tastytrade/dxfeed/profile.py` & `tastytrade-5.1/tastytrade/dxfeed/profile.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.0/tastytrade/dxfeed/quote.py` & `tastytrade-5.1/tastytrade/dxfeed/quote.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.0/tastytrade/dxfeed/summary.py` & `tastytrade-5.1/tastytrade/dxfeed/summary.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.0/tastytrade/dxfeed/theoprice.py` & `tastytrade-5.1/tastytrade/dxfeed/theoprice.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.0/tastytrade/dxfeed/trade.py` & `tastytrade-5.1/tastytrade/dxfeed/trade.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.0/tastytrade/instruments.py` & `tastytrade-5.1/tastytrade/instruments.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.0/tastytrade/metrics.py` & `tastytrade-5.1/tastytrade/metrics.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.0/tastytrade/order.py` & `tastytrade-5.1/tastytrade/order.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.0/tastytrade/search.py` & `tastytrade-5.1/tastytrade/search.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.0/tastytrade/session.py` & `tastytrade-5.1/tastytrade/session.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.0/tastytrade/streamer.py` & `tastytrade-5.1/tastytrade/streamer.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.0/tastytrade/utils.py` & `tastytrade-5.1/tastytrade/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         allow_population_by_field_name = True
 
 
 def validate_response(response: Response) -> None:
     """
     Checks if the given code is an error; if so, raises an exception.
 
-    :param json: response to check for errors
+    :param response: response to check for errors
     """
     if response.status_code // 100 != 2:
         content = response.json()['error']
         error_message = f"{content['code']}: {content['message']}"
         errors = content.get('errors')
         if errors is not None:
             for error in errors:
```

### Comparing `tastytrade-5.0/tastytrade/watchlists.py` & `tastytrade-5.1/tastytrade/watchlists.py`

 * *Files identical despite different names*

### Comparing `tastytrade-5.0/tastytrade.egg-info/PKG-INFO` & `tastytrade-5.1/tastytrade.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: tastytrade
-Version: 5.0
+Version: 5.1
 Summary: An unofficial SDK for Tastytrade!
 Home-page: https://github.com/tastyware/tastytrade
 Author: Graeme Holliday
 Author-email: graeme.holliday@pm.me
-License: Apache
-Description-Content-Type: text/markdown
+License: MIT
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 .. image:: https://readthedocs.org/projects/tastyworks-api/badge/?version=latest
    :target: https://tastyworks-api.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
 
 .. image:: https://img.shields.io/pypi/v/tastytrade
```

### Comparing `tastytrade-5.0/tastytrade.egg-info/SOURCES.txt` & `tastytrade-5.1/tastytrade.egg-info/SOURCES.txt`

 * *Files identical despite different names*

