# Comparing `tmp/popodds-0.6.2.tar.gz` & `tmp/popodds-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "popodds-0.6.2.tar", last modified: Tue Mar 28 13:35:23 2023, max compression
+gzip compressed data, was "popodds-0.7.0.tar", last modified: Fri May 19 22:59:38 2023, max compression
```

## Comparing `popodds-0.6.2.tar` & `popodds-0.7.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 mdm988   (1344792526) domain users (1344200513)        0 2023-03-28 13:35:23.237666 popodds-0.6.2/
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)     1070 2022-07-27 10:52:18.000000 popodds-0.6.2/LICENSE
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)     1364 2023-03-28 13:35:23.237666 popodds-0.6.2/PKG-INFO
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)     1056 2023-03-20 15:42:02.000000 popodds-0.6.2/README.md
-drwxr-xr-x   0 mdm988   (1344792526) domain users (1344200513)        0 2023-03-28 13:35:23.237666 popodds-0.6.2/popodds/
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)    12134 2023-03-28 13:33:52.000000 popodds-0.6.2/popodds/__init__.py
-drwxr-xr-x   0 mdm988   (1344792526) domain users (1344200513)        0 2023-03-28 13:35:23.237666 popodds-0.6.2/popodds.egg-info/
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)     1364 2023-03-28 13:35:23.000000 popodds-0.6.2/popodds.egg-info/PKG-INFO
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)      200 2023-03-28 13:35:23.000000 popodds-0.6.2/popodds.egg-info/SOURCES.txt
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)        1 2023-03-28 13:35:23.000000 popodds-0.6.2/popodds.egg-info/dependency_links.txt
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)       19 2023-03-28 13:35:23.000000 popodds-0.6.2/popodds.egg-info/requires.txt
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)        8 2023-03-28 13:35:23.000000 popodds-0.6.2/popodds.egg-info/top_level.txt
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)       38 2023-03-28 13:35:23.237666 popodds-0.6.2/setup.cfg
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)      604 2023-03-28 13:34:13.000000 popodds-0.6.2/setup.py
+drwxr-xr-x   0 mdm988   (1344792526) domain users (1344200513)        0 2023-05-19 22:59:38.164780 popodds-0.7.0/
+-rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)     1070 2023-05-19 22:44:33.000000 popodds-0.7.0/LICENSE
+-rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)     1364 2023-05-19 22:59:38.164780 popodds-0.7.0/PKG-INFO
+-rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)     1056 2023-05-19 22:44:33.000000 popodds-0.7.0/README.md
+drwxr-xr-x   0 mdm988   (1344792526) domain users (1344200513)        0 2023-05-19 22:59:38.160780 popodds-0.7.0/popodds/
+-rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)       50 2023-05-19 22:49:03.000000 popodds-0.7.0/popodds/__init__.py
+-rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)     4693 2023-05-19 22:58:10.000000 popodds-0.7.0/popodds/detection.py
+-rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)    12135 2023-05-19 22:49:16.000000 popodds-0.7.0/popodds/popodds.py
+drwxr-xr-x   0 mdm988   (1344792526) domain users (1344200513)        0 2023-05-19 22:59:38.164780 popodds-0.7.0/popodds.egg-info/
+-rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)     1364 2023-05-19 22:59:38.000000 popodds-0.7.0/popodds.egg-info/PKG-INFO
+-rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)      240 2023-05-19 22:59:38.000000 popodds-0.7.0/popodds.egg-info/SOURCES.txt
+-rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)        1 2023-05-19 22:59:38.000000 popodds-0.7.0/popodds.egg-info/dependency_links.txt
+-rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)       19 2023-05-19 22:59:38.000000 popodds-0.7.0/popodds.egg-info/requires.txt
+-rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)        8 2023-05-19 22:59:38.000000 popodds-0.7.0/popodds.egg-info/top_level.txt
+-rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)       38 2023-05-19 22:59:38.164780 popodds-0.7.0/setup.cfg
+-rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)      604 2023-05-19 22:59:14.000000 popodds-0.7.0/setup.py
```

### Comparing `popodds-0.6.2/LICENSE` & `popodds-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `popodds-0.6.2/PKG-INFO` & `popodds-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: popodds
-Version: 0.6.2
+Version: 0.7.0
 Summary: Simple package for Bayesian model comparison.
 Home-page: https://github.com/mdmould/popodds
 Author: Matthew Mould
 Author-email: mattdmould@gmail.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `popodds-0.6.2/README.md` & `popodds-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `popodds-0.6.2/popodds/__init__.py` & `popodds-0.7.0/popodds/popodds.py`

 * *Files 0% similar despite different names*

```diff
@@ -338,7 +338,8 @@
     box_model = np.all((bounds[0] < model) * (model < bounds[1]), axis=0)
     box_prior = np.all((bounds[0] < prior) * (prior < bounds[1]), axis=0)
 
     return (
         (np.sum(box_model) / np.shape(model)[-1]) /
         (np.sum(box_prior) / np.shape(prior)[-1])
         )
+
```

### Comparing `popodds-0.6.2/popodds.egg-info/PKG-INFO` & `popodds-0.7.0/popodds.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: popodds
-Version: 0.6.2
+Version: 0.7.0
 Summary: Simple package for Bayesian model comparison.
 Home-page: https://github.com/mdmould/popodds
 Author: Matthew Mould
 Author-email: mattdmould@gmail.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `popodds-0.6.2/setup.py` & `popodds-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 name = 'popodds'
-version = '0.6.2'
+version = '0.7.0'
 
 with open('README.md', 'r') as f:
     long_description = f.read().strip()
 
 setup(
     name=name,
     version=version,
```

