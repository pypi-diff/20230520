# Comparing `tmp/tastytrade-1.0.tar.gz` & `tmp/tastytrade-5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tastytrade-1.0.tar", last modified: Wed Apr 19 01:41:36 2023, max compression
+gzip compressed data, was "tastytrade-5.0.tar", last modified: Sat May 20 06:11:59 2023, max compression
```

## Comparing `tastytrade-1.0.tar` & `tastytrade-5.0.tar`

### file list

```diff
@@ -1,31 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:41:36.262296 tastytrade-1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-19 01:41:25.000000 tastytrade-1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-19 01:41:36.262296 tastytrade-1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-19 01:41:25.000000 tastytrade-1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 01:41:36.262296 tastytrade-1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-19 01:41:25.000000 tastytrade-1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:41:36.262296 tastytrade-1.0/tastytrade/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-19 01:41:25.000000 tastytrade-1.0/tastytrade/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-04-19 01:41:25.000000 tastytrade-1.0/tastytrade/account.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:41:36.262296 tastytrade-1.0/tastytrade/dxfeed/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-19 01:41:25.000000 tastytrade-1.0/tastytrade/dxfeed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-19 01:41:25.000000 tastytrade-1.0/tastytrade/dxfeed/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-19 01:41:25.000000 tastytrade-1.0/tastytrade/dxfeed/greeks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-19 01:41:25.000000 tastytrade-1.0/tastytrade/dxfeed/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-19 01:41:25.000000 tastytrade-1.0/tastytrade/dxfeed/quote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-04-19 01:41:25.000000 tastytrade-1.0/tastytrade/dxfeed/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-19 01:41:25.000000 tastytrade-1.0/tastytrade/dxfeed/theoprice.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-19 01:41:25.000000 tastytrade-1.0/tastytrade/dxfeed/trade.py
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-04-19 01:41:25.000000 tastytrade-1.0/tastytrade/option.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-04-19 01:41:25.000000 tastytrade-1.0/tastytrade/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-19 01:41:25.000000 tastytrade-1.0/tastytrade/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-19 01:41:25.000000 tastytrade-1.0/tastytrade/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-04-19 01:41:25.000000 tastytrade-1.0/tastytrade/streamer.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-19 01:41:25.000000 tastytrade-1.0/tastytrade/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-04-19 01:41:25.000000 tastytrade-1.0/tastytrade/watchlists.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 01:41:36.262296 tastytrade-1.0/tastytrade.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-19 01:41:36.000000 tastytrade-1.0/tastytrade.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-19 01:41:36.000000 tastytrade-1.0/tastytrade.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 01:41:36.000000 tastytrade-1.0/tastytrade.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-19 01:41:36.000000 tastytrade-1.0/tastytrade.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-19 01:41:36.000000 tastytrade-1.0/tastytrade.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:11:59.488858 tastytrade-5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-20 06:11:49.000000 tastytrade-5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7463 2023-05-20 06:11:59.488858 tastytrade-5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7177 2023-05-20 06:11:49.000000 tastytrade-5.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 06:11:59.488858 tastytrade-5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-20 06:11:49.000000 tastytrade-5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:11:59.484858 tastytrade-5.0/tastytrade/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-20 06:11:49.000000 tastytrade-5.0/tastytrade/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34247 2023-05-20 06:11:49.000000 tastytrade-5.0/tastytrade/account.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:11:59.488858 tastytrade-5.0/tastytrade/dxfeed/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-20 06:11:49.000000 tastytrade-5.0/tastytrade/dxfeed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-20 06:11:49.000000 tastytrade-5.0/tastytrade/dxfeed/candle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-20 06:11:49.000000 tastytrade-5.0/tastytrade/dxfeed/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-20 06:11:49.000000 tastytrade-5.0/tastytrade/dxfeed/greeks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-20 06:11:49.000000 tastytrade-5.0/tastytrade/dxfeed/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-20 06:11:49.000000 tastytrade-5.0/tastytrade/dxfeed/quote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-20 06:11:49.000000 tastytrade-5.0/tastytrade/dxfeed/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-20 06:11:49.000000 tastytrade-5.0/tastytrade/dxfeed/theoprice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-20 06:11:49.000000 tastytrade-5.0/tastytrade/dxfeed/trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30051 2023-05-20 06:11:49.000000 tastytrade-5.0/tastytrade/instruments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-05-20 06:11:49.000000 tastytrade-5.0/tastytrade/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9056 2023-05-20 06:11:49.000000 tastytrade-5.0/tastytrade/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-20 06:11:49.000000 tastytrade-5.0/tastytrade/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-05-20 06:11:49.000000 tastytrade-5.0/tastytrade/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18754 2023-05-20 06:11:49.000000 tastytrade-5.0/tastytrade/streamer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-20 06:11:49.000000 tastytrade-5.0/tastytrade/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-05-20 06:11:49.000000 tastytrade-5.0/tastytrade/watchlists.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:11:59.488858 tastytrade-5.0/tastytrade.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7463 2023-05-20 06:11:59.000000 tastytrade-5.0/tastytrade.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-20 06:11:59.000000 tastytrade-5.0/tastytrade.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 06:11:59.000000 tastytrade-5.0/tastytrade.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-20 06:11:59.000000 tastytrade-5.0/tastytrade.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-20 06:11:59.000000 tastytrade-5.0/tastytrade.egg-info/top_level.txt
```

### Comparing `tastytrade-1.0/LICENSE` & `tastytrade-5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tastytrade-1.0/setup.py` & `tastytrade-5.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from setuptools import find_packages, setup
 
 from tastytrade import VERSION
 
 
-f = open('README.md', 'r')
+f = open('README.rst', 'r')
 LONG_DESCRIPTION = f.read()
 f.close()
 
 setup(
     name='tastytrade',
     version=VERSION,
-    description='An unofficial API for Tastytrade!',
+    description='An unofficial SDK for Tastytrade!',
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     author='Graeme Holliday',
     author_email='graeme.holliday@pm.me',
     url='https://github.com/tastyware/tastytrade',
     license='Apache',
     install_requires=[
-        'aiohttp<4',
         'requests<3',
-        'tastyworks-aiocometd>=1.0',
-        'dataclasses'
+        'dataclasses',
+        'websockets>=11.0.3',
+        'pydantic>=1.10.7'
     ],
     packages=find_packages(exclude=['ez_setup', 'tests*']),
     include_package_data=True,
 )
```

### Comparing `tastytrade-1.0/tastytrade/dxfeed/greeks.py` & `tastytrade-5.0/tastytrade/dxfeed/greeks.py`

 * *Files identical despite different names*

### Comparing `tastytrade-1.0/tastytrade/dxfeed/profile.py` & `tastytrade-5.0/tastytrade/dxfeed/profile.py`

 * *Files identical despite different names*

### Comparing `tastytrade-1.0/tastytrade/dxfeed/quote.py` & `tastytrade-5.0/tastytrade/dxfeed/quote.py`

 * *Files identical despite different names*

### Comparing `tastytrade-1.0/tastytrade/dxfeed/summary.py` & `tastytrade-5.0/tastytrade/dxfeed/summary.py`

 * *Files identical despite different names*

### Comparing `tastytrade-1.0/tastytrade/dxfeed/theoprice.py` & `tastytrade-5.0/tastytrade/dxfeed/theoprice.py`

 * *Files identical despite different names*

### Comparing `tastytrade-1.0/tastytrade/dxfeed/trade.py` & `tastytrade-5.0/tastytrade/dxfeed/trade.py`

 * *Files identical despite different names*

### Comparing `tastytrade-1.0/tastytrade.egg-info/SOURCES.txt` & `tastytrade-5.0/tastytrade.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 LICENSE
-README.md
+README.rst
 setup.py
 tastytrade/__init__.py
 tastytrade/account.py
-tastytrade/option.py
+tastytrade/instruments.py
+tastytrade/metrics.py
 tastytrade/order.py
 tastytrade/search.py
 tastytrade/session.py
 tastytrade/streamer.py
 tastytrade/utils.py
 tastytrade/watchlists.py
 tastytrade.egg-info/PKG-INFO
 tastytrade.egg-info/SOURCES.txt
 tastytrade.egg-info/dependency_links.txt
 tastytrade.egg-info/requires.txt
 tastytrade.egg-info/top_level.txt
 tastytrade/dxfeed/__init__.py
+tastytrade/dxfeed/candle.py
 tastytrade/dxfeed/event.py
 tastytrade/dxfeed/greeks.py
 tastytrade/dxfeed/profile.py
 tastytrade/dxfeed/quote.py
 tastytrade/dxfeed/summary.py
 tastytrade/dxfeed/theoprice.py
 tastytrade/dxfeed/trade.py
```

