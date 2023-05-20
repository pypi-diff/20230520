# Comparing `tmp/archetesting-0.0.2.tar.gz` & `tmp/archetesting-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archetesting-0.0.2.tar", last modified: Sun Feb  5 18:14:32 2023, max compression
+gzip compressed data, was "archetesting-0.0.3.tar", last modified: Sat May 20 13:56:52 2023, max compression
```

## Comparing `archetesting-0.0.2.tar` & `archetesting-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-02-05 18:14:32.720034 archetesting-0.0.2/
--rw-rw-rw-   0        0        0       83 2023-02-05 18:12:19.000000 archetesting-0.0.2/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1072 2023-02-05 17:27:44.000000 archetesting-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0       26 2023-02-05 17:24:15.000000 archetesting-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      721 2023-02-05 18:14:32.720034 archetesting-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       68 2023-02-05 17:06:36.000000 archetesting-0.0.2/README.txt
-drwxrwxrwx   0        0        0        0 2023-02-05 18:14:32.711032 archetesting-0.0.2/archetesting/
--rw-rw-rw-   0        0        0      135 2023-02-05 17:05:37.000000 archetesting-0.0.2/archetesting/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-05 18:14:32.719033 archetesting-0.0.2/archetesting.egg-info/
--rw-rw-rw-   0        0        0      721 2023-02-05 18:14:32.000000 archetesting-0.0.2/archetesting.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2023-02-05 18:14:32.000000 archetesting-0.0.2/archetesting.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-05 18:14:32.000000 archetesting-0.0.2/archetesting.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-02-05 18:14:32.000000 archetesting-0.0.2/archetesting.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-05 18:14:32.720034 archetesting-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      643 2023-02-05 18:14:30.000000 archetesting-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 13:56:52.524920 archetesting-0.0.3/
+-rw-rw-rw-   0        0        0      103 2023-05-20 13:54:34.000000 archetesting-0.0.3/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1072 2023-02-05 17:27:44.000000 archetesting-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0       26 2023-02-05 17:24:15.000000 archetesting-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      741 2023-05-20 13:56:52.524920 archetesting-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       68 2023-02-05 17:06:36.000000 archetesting-0.0.3/README.txt
+drwxrwxrwx   0        0        0        0 2023-05-20 13:56:52.509916 archetesting-0.0.3/archetesting/
+-rw-rw-rw-   0        0        0      220 2023-05-20 13:56:40.000000 archetesting-0.0.3/archetesting/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-20 13:56:52.523919 archetesting-0.0.3/archetesting.egg-info/
+-rw-rw-rw-   0        0        0      741 2023-05-20 13:56:52.000000 archetesting-0.0.3/archetesting.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-05-20 13:56:52.000000 archetesting-0.0.3/archetesting.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 13:56:52.000000 archetesting-0.0.3/archetesting.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-20 13:56:52.000000 archetesting-0.0.3/archetesting.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-20 13:56:52.525920 archetesting-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      643 2023-05-20 13:54:18.000000 archetesting-0.0.3/setup.py
```

### Comparing `archetesting-0.0.2/LICENSE.txt` & `archetesting-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `archetesting-0.0.2/PKG-INFO` & `archetesting-0.0.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 1.1
 Name: archetesting
-Version: 0.0.2
+Version: 0.0.3
 Summary: This is the testing library
 Home-page: UNKNOWN
 Author: Arche
 Author-email: rkdyava@gmail.com
 License: UNKNOWN
 Description: This is the application for adding and subsstracting the two numbers
         
         Chnage LOG
         ==========
         
         
-        0.0.1 (05/02/2023)
+        0.0.3 (05/02/2023)
         ------------------
-        - First Release
+        - 3rd Release and added numpy as np
 Keywords: add
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `archetesting-0.0.2/archetesting.egg-info/PKG-INFO` & `archetesting-0.0.3/archetesting.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 1.1
 Name: archetesting
-Version: 0.0.2
+Version: 0.0.3
 Summary: This is the testing library
 Home-page: UNKNOWN
 Author: Arche
 Author-email: rkdyava@gmail.com
 License: UNKNOWN
 Description: This is the application for adding and subsstracting the two numbers
         
         Chnage LOG
         ==========
         
         
-        0.0.1 (05/02/2023)
+        0.0.3 (05/02/2023)
         ------------------
-        - First Release
+        - 3rd Release and added numpy as np
 Keywords: add
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `archetesting-0.0.2/setup.py` & `archetesting-0.0.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 ]
 
 setup(
 
 name = 'archetesting',
-version='0.0.2',
+version='0.0.3',
 description='This is the testing library',
 long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
 url='',
 author='Arche',
 author_email='rkdyava@gmail.com',
 classifiers=classifiers,
 keywords='add',
```

