# Comparing `tmp/osgiservicebridge-1.5.2.tar.gz` & `tmp/osgiservicebridge-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osgiservicebridge-1.5.2.tar", last modified: Sat May 20 00:03:47 2023, max compression
+gzip compressed data, was "osgiservicebridge-1.5.3.tar", last modified: Sat May 20 04:26:34 2023, max compression
```

## Comparing `osgiservicebridge-1.5.2.tar` & `osgiservicebridge-1.5.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 00:03:47.536032 osgiservicebridge-1.5.2/
--rw-rw-rw-   0        0        0    11558 2019-03-24 04:27:06.000000 osgiservicebridge-1.5.2/LICENSE
--rw-rw-rw-   0        0        0     1268 2023-05-20 00:03:47.536032 osgiservicebridge-1.5.2/PKG-INFO
--rw-rw-rw-   0        0        0      276 2023-05-19 20:02:04.000000 osgiservicebridge-1.5.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-20 00:03:47.499713 osgiservicebridge-1.5.2/java/
--rw-rw-rw-   0        0        0  2778718 2023-05-19 19:42:54.000000 osgiservicebridge-1.5.2/java/py4j-remoteservicesprovider_2.11.0.zip
--rw-rw-rw-   0        0        0       99 2023-05-19 23:48:27.000000 osgiservicebridge-1.5.2/pyproject.toml
--rw-rw-rw-   0        0        0       74 2023-05-20 00:03:47.538037 osgiservicebridge-1.5.2/setup.cfg
--rw-rw-rw-   0        0        0     4751 2023-05-19 23:53:23.000000 osgiservicebridge-1.5.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-20 00:03:47.491421 osgiservicebridge-1.5.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-20 00:03:47.511026 osgiservicebridge-1.5.2/src/osgiservicebridge/
--rw-rw-rw-   0        0        0    17269 2023-05-17 22:26:05.000000 osgiservicebridge-1.5.2/src/osgiservicebridge/__init__.py
--rw-rw-rw-   0        0        0    49609 2023-05-18 23:34:21.000000 osgiservicebridge-1.5.2/src/osgiservicebridge/bridge.py
--rw-rw-rw-   0        0        0     2475 2023-05-17 22:27:56.000000 osgiservicebridge-1.5.2/src/osgiservicebridge/exporter_pb2.py
--rw-rw-rw-   0        0        0    11085 2023-05-17 22:26:05.000000 osgiservicebridge-1.5.2/src/osgiservicebridge/flatbuf.py
--rw-rw-rw-   0        0        0    31593 2023-05-17 22:30:57.000000 osgiservicebridge-1.5.2/src/osgiservicebridge/protobuf.py
--rw-rw-rw-   0        0        0       20 2023-05-20 00:03:06.000000 osgiservicebridge-1.5.2/src/osgiservicebridge/version.py
-drwxrwxrwx   0        0        0        0 2023-05-20 00:03:47.535035 osgiservicebridge-1.5.2/src/osgiservicebridge.egg-info/
--rw-rw-rw-   0        0        0     1268 2023-05-20 00:03:47.000000 osgiservicebridge-1.5.2/src/osgiservicebridge.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      524 2023-05-20 00:03:47.000000 osgiservicebridge-1.5.2/src/osgiservicebridge.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 00:03:47.000000 osgiservicebridge-1.5.2/src/osgiservicebridge.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-05-20 00:03:47.000000 osgiservicebridge-1.5.2/src/osgiservicebridge.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-20 00:03:47.000000 osgiservicebridge-1.5.2/src/osgiservicebridge.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-20 04:26:34.597157 osgiservicebridge-1.5.3/
+-rw-rw-rw-   0        0        0    11558 2019-03-24 04:27:06.000000 osgiservicebridge-1.5.3/LICENSE
+-rw-rw-rw-   0        0        0     1268 2023-05-20 04:26:34.598155 osgiservicebridge-1.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2023-05-19 20:02:04.000000 osgiservicebridge-1.5.3/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-20 04:26:34.572025 osgiservicebridge-1.5.3/java/
+-rw-rw-rw-   0        0        0  2778718 2023-05-19 19:42:54.000000 osgiservicebridge-1.5.3/java/py4j-remoteservicesprovider_2.11.0.zip
+-rw-rw-rw-   0        0        0       99 2023-05-19 23:48:27.000000 osgiservicebridge-1.5.3/pyproject.toml
+-rw-rw-rw-   0        0        0       74 2023-05-20 04:26:34.599233 osgiservicebridge-1.5.3/setup.cfg
+-rw-rw-rw-   0        0        0     4751 2023-05-20 04:26:07.000000 osgiservicebridge-1.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 04:26:34.560702 osgiservicebridge-1.5.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-20 04:26:34.581017 osgiservicebridge-1.5.3/src/osgiservicebridge/
+-rw-rw-rw-   0        0        0    17269 2023-05-17 22:26:05.000000 osgiservicebridge-1.5.3/src/osgiservicebridge/__init__.py
+-rw-rw-rw-   0        0        0    49609 2023-05-18 23:34:21.000000 osgiservicebridge-1.5.3/src/osgiservicebridge/bridge.py
+-rw-rw-rw-   0        0        0     2475 2023-05-17 22:27:56.000000 osgiservicebridge-1.5.3/src/osgiservicebridge/exporter_pb2.py
+-rw-rw-rw-   0        0        0    11085 2023-05-17 22:26:05.000000 osgiservicebridge-1.5.3/src/osgiservicebridge/flatbuf.py
+-rw-rw-rw-   0        0        0    31593 2023-05-17 22:30:57.000000 osgiservicebridge-1.5.3/src/osgiservicebridge/protobuf.py
+-rw-rw-rw-   0        0        0       20 2023-05-20 04:24:07.000000 osgiservicebridge-1.5.3/src/osgiservicebridge/version.py
+drwxrwxrwx   0        0        0        0 2023-05-20 04:26:34.597157 osgiservicebridge-1.5.3/src/osgiservicebridge.egg-info/
+-rw-rw-rw-   0        0        0     1268 2023-05-20 04:26:34.000000 osgiservicebridge-1.5.3/src/osgiservicebridge.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      524 2023-05-20 04:26:34.000000 osgiservicebridge-1.5.3/src/osgiservicebridge.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 04:26:34.000000 osgiservicebridge-1.5.3/src/osgiservicebridge.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-05-20 04:26:34.000000 osgiservicebridge-1.5.3/src/osgiservicebridge.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-20 04:26:34.000000 osgiservicebridge-1.5.3/src/osgiservicebridge.egg-info/top_level.txt
```

### Comparing `osgiservicebridge-1.5.2/LICENSE` & `osgiservicebridge-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `osgiservicebridge-1.5.2/PKG-INFO` & `osgiservicebridge-1.5.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osgiservicebridge
-Version: 1.5.2
+Version: 1.5.3
 Summary: OSGi services implemented in Python
 Home-page: https://github.com/ECF/Py4j-RemoteServicesProvider
 Author: Scott Lewis
 Author-email: scottslewis@gmail.com
 License: Apache Software License
 Keywords: Java Python OSGi development
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `osgiservicebridge-1.5.2/java/py4j-remoteservicesprovider_2.11.0.zip` & `osgiservicebridge-1.5.3/java/py4j-remoteservicesprovider_2.11.0.zip`

 * *Files identical despite different names*

### Comparing `osgiservicebridge-1.5.2/setup.py` & `osgiservicebridge-1.5.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     # this:
     #   py_modules=["my_module"],
 
     # List run-time dependencies here.  These will be installed by pip when
     # your project is installed. For an analysis of "install_requires" vs pip's
     # requirements files see:
     # https://packaging.python.org/en/latest/requirements.html
-    install_requires=['py4j>=0.10.9.7','protobuf==3.22.2'],
+    install_requires=['py4j>=0.10.9.7','protobuf==4.22.5'],
 
     # List additional groups of dependencies here (e.g. development
     # dependencies). You can install these using the following syntax,
     # for example:
     # $ pip install -e .[dev,test]
     #extras_require={
     #    'dev': ['check-manifest'],
```

### Comparing `osgiservicebridge-1.5.2/src/osgiservicebridge/__init__.py` & `osgiservicebridge-1.5.3/src/osgiservicebridge/__init__.py`

 * *Files identical despite different names*

### Comparing `osgiservicebridge-1.5.2/src/osgiservicebridge/bridge.py` & `osgiservicebridge-1.5.3/src/osgiservicebridge/bridge.py`

 * *Files identical despite different names*

### Comparing `osgiservicebridge-1.5.2/src/osgiservicebridge/exporter_pb2.py` & `osgiservicebridge-1.5.3/src/osgiservicebridge/exporter_pb2.py`

 * *Files identical despite different names*

### Comparing `osgiservicebridge-1.5.2/src/osgiservicebridge/flatbuf.py` & `osgiservicebridge-1.5.3/src/osgiservicebridge/flatbuf.py`

 * *Files identical despite different names*

### Comparing `osgiservicebridge-1.5.2/src/osgiservicebridge/protobuf.py` & `osgiservicebridge-1.5.3/src/osgiservicebridge/protobuf.py`

 * *Files identical despite different names*

### Comparing `osgiservicebridge-1.5.2/src/osgiservicebridge.egg-info/PKG-INFO` & `osgiservicebridge-1.5.3/src/osgiservicebridge.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osgiservicebridge
-Version: 1.5.2
+Version: 1.5.3
 Summary: OSGi services implemented in Python
 Home-page: https://github.com/ECF/Py4j-RemoteServicesProvider
 Author: Scott Lewis
 Author-email: scottslewis@gmail.com
 License: Apache Software License
 Keywords: Java Python OSGi development
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `osgiservicebridge-1.5.2/src/osgiservicebridge.egg-info/SOURCES.txt` & `osgiservicebridge-1.5.3/src/osgiservicebridge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

