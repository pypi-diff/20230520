# Comparing `tmp/api_sap-0.0.2.tar.gz` & `tmp/api_sap-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "api_sap-0.0.2.tar", last modified: Sat May 20 14:12:03 2023, max compression
+gzip compressed data, was "api_sap-0.0.3.tar", last modified: Sat May 20 14:29:13 2023, max compression
```

## Comparing `api_sap-0.0.2.tar` & `api_sap-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 14:12:03.728513 api_sap-0.0.2/
--rw-rw-rw-   0        0        0     1075 2023-05-20 12:58:20.000000 api_sap-0.0.2/LICENCE
--rw-rw-rw-   0        0        0      428 2023-05-20 14:12:03.717578 api_sap-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      113 2023-05-20 13:14:53.000000 api_sap-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-20 14:12:03.677669 api_sap-0.0.2/api_sap.egg-info/
--rw-rw-rw-   0        0        0      428 2023-05-20 14:12:03.000000 api_sap-0.0.2/api_sap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2023-05-20 14:12:03.000000 api_sap-0.0.2/api_sap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 14:12:03.000000 api_sap-0.0.2/api_sap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-05-20 14:12:03.000000 api_sap-0.0.2/api_sap.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-20 14:12:03.000000 api_sap-0.0.2/api_sap.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-20 14:12:03.701793 api_sap-0.0.2/py_sap/
--rw-rw-rw-   0        0        0       25 2023-05-19 23:13:01.000000 api_sap-0.0.2/py_sap/__init__.py
--rw-rw-rw-   0        0        0    29082 2023-05-08 18:17:20.000000 api_sap-0.0.2/py_sap/py_sap.py
--rw-rw-rw-   0        0        0       42 2023-05-20 14:12:03.728513 api_sap-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      784 2023-05-20 14:04:45.000000 api_sap-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 14:29:13.028168 api_sap-0.0.3/
+-rw-rw-rw-   0        0        0     1075 2023-05-20 12:58:20.000000 api_sap-0.0.3/LICENCE
+-rw-rw-rw-   0        0        0      434 2023-05-20 14:29:13.020828 api_sap-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      119 2023-05-20 14:26:04.000000 api_sap-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-20 14:29:12.984611 api_sap-0.0.3/api_sap.egg-info/
+-rw-rw-rw-   0        0        0      434 2023-05-20 14:29:12.000000 api_sap-0.0.3/api_sap.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2023-05-20 14:29:12.000000 api_sap-0.0.3/api_sap.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 14:29:12.000000 api_sap-0.0.3/api_sap.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-05-20 14:29:12.000000 api_sap-0.0.3/api_sap.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-20 14:29:12.000000 api_sap-0.0.3/api_sap.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-20 14:29:13.007152 api_sap-0.0.3/py_sap/
+-rw-rw-rw-   0        0        0       25 2023-05-19 23:13:01.000000 api_sap-0.0.3/py_sap/__init__.py
+-rw-rw-rw-   0        0        0    29082 2023-05-08 18:17:20.000000 api_sap-0.0.3/py_sap/py_sap.py
+-rw-rw-rw-   0        0        0       42 2023-05-20 14:29:13.028668 api_sap-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      784 2023-05-20 14:26:43.000000 api_sap-0.0.3/setup.py
```

### Comparing `api_sap-0.0.2/LICENCE` & `api_sap-0.0.3/LICENCE`

 * *Files identical despite different names*

### Comparing `api_sap-0.0.2/py_sap/py_sap.py` & `api_sap-0.0.3/py_sap/py_sap.py`

 * *Files identical despite different names*

### Comparing `api_sap-0.0.2/setup.py` & `api_sap-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     """
     with open('README.md', 'r', encoding="utf-8") as arq:
         return arq.read()
 
 
 setup(
     name='api_sap',
-    version='0.0.2',
+    version='0.0.3',
     license='MIT License',
     author='Wilton Melo',
     long_description=readme(),
     requires_python='>=3.9.13',
     long_description_content_type='text/markdown',
     author_email='pmelo.wilton@gmail.com',
     keywords=['api sap', 'SAP', 'conectar ao SAP'],
```

