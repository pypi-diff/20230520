# Comparing `tmp/archeSetup-0.0.4.tar.gz` & `tmp/archeSetup-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archeSetup-0.0.4.tar", last modified: Sat May 20 14:07:13 2023, max compression
+gzip compressed data, was "archeSetup-0.0.5.tar", last modified: Sat May 20 14:14:57 2023, max compression
```

## Comparing `archeSetup-0.0.4.tar` & `archeSetup-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 14:07:13.268304 archeSetup-0.0.4/
--rw-rw-rw-   0        0        0      101 2023-05-20 13:46:17.000000 archeSetup-0.0.4/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1072 2023-05-20 12:20:31.000000 archeSetup-0.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0       26 2023-05-20 12:18:33.000000 archeSetup-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0      769 2023-05-20 14:07:13.268304 archeSetup-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       74 2023-05-20 13:47:05.000000 archeSetup-0.0.4/README.txt
-drwxrwxrwx   0        0        0        0 2023-05-20 14:07:13.258302 archeSetup-0.0.4/archeInitialze/
--rw-rw-rw-   0        0        0      221 2023-05-20 14:05:44.000000 archeSetup-0.0.4/archeInitialze/__init__.py
--rw-rw-rw-   0        0        0     1119 2023-05-20 13:47:35.000000 archeSetup-0.0.4/archeInitialze/initApp.py
-drwxrwxrwx   0        0        0        0 2023-05-20 14:07:13.267304 archeSetup-0.0.4/archeSetup.egg-info/
--rw-rw-rw-   0        0        0      769 2023-05-20 14:07:13.000000 archeSetup-0.0.4/archeSetup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2023-05-20 14:07:13.000000 archeSetup-0.0.4/archeSetup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 14:07:13.000000 archeSetup-0.0.4/archeSetup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-20 14:07:13.000000 archeSetup-0.0.4/archeSetup.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-20 14:07:13.268304 archeSetup-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      667 2023-05-20 14:07:07.000000 archeSetup-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 14:14:57.421974 archeSetup-0.0.5/
+-rw-rw-rw-   0        0        0       99 2023-05-20 14:12:07.000000 archeSetup-0.0.5/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1072 2023-05-20 12:20:31.000000 archeSetup-0.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0       26 2023-05-20 12:18:33.000000 archeSetup-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      767 2023-05-20 14:14:57.421974 archeSetup-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       74 2023-05-20 13:47:05.000000 archeSetup-0.0.5/README.txt
+drwxrwxrwx   0        0        0        0 2023-05-20 14:14:57.407971 archeSetup-0.0.5/archeSetup/
+-rw-rw-rw-   0        0        0      221 2023-05-20 14:14:30.000000 archeSetup-0.0.5/archeSetup/__init__.py
+-rw-rw-rw-   0        0        0     1119 2023-05-20 13:47:35.000000 archeSetup-0.0.5/archeSetup/initApp.py
+drwxrwxrwx   0        0        0        0 2023-05-20 14:14:57.420974 archeSetup-0.0.5/archeSetup.egg-info/
+-rw-rw-rw-   0        0        0      767 2023-05-20 14:14:57.000000 archeSetup-0.0.5/archeSetup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2023-05-20 14:14:57.000000 archeSetup-0.0.5/archeSetup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 14:14:57.000000 archeSetup-0.0.5/archeSetup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-20 14:14:57.000000 archeSetup-0.0.5/archeSetup.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-20 14:14:57.422975 archeSetup-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      667 2023-05-20 14:14:45.000000 archeSetup-0.0.5/setup.py
```

### Comparing `archeSetup-0.0.4/LICENSE.txt` & `archeSetup-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `archeSetup-0.0.4/PKG-INFO` & `archeSetup-0.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 1.1
 Name: archeSetup
-Version: 0.0.4
+Version: 0.0.5
 Summary: This is the setup for the basic Application library
 Home-page: UNKNOWN
 Author: Arche
 Author-email: rkdyava@gmail.com
 License: UNKNOWN
 Description: This is the  initialisation of the application and it will be use as check
         
         Chnage LOG
         ==========
         
         
-        0.0.3 (20/05/2023)
+        0.0.4 (20/05/2023)
         ------------------
-        - third  Release after bug fixing
+        - 4th  Release after bug fixing
 Keywords: Setup
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `archeSetup-0.0.4/archeInitialze/initApp.py` & `archeSetup-0.0.5/archeSetup/initApp.py`

 * *Files identical despite different names*

### Comparing `archeSetup-0.0.4/archeSetup.egg-info/PKG-INFO` & `archeSetup-0.0.5/archeSetup.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 1.1
 Name: archeSetup
-Version: 0.0.4
+Version: 0.0.5
 Summary: This is the setup for the basic Application library
 Home-page: UNKNOWN
 Author: Arche
 Author-email: rkdyava@gmail.com
 License: UNKNOWN
 Description: This is the  initialisation of the application and it will be use as check
         
         Chnage LOG
         ==========
         
         
-        0.0.3 (20/05/2023)
+        0.0.4 (20/05/2023)
         ------------------
-        - third  Release after bug fixing
+        - 4th  Release after bug fixing
 Keywords: Setup
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `archeSetup-0.0.4/setup.py` & `archeSetup-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 ]
 
 setup(
 
 name = 'archeSetup',
-version='0.0.4',
+version='0.0.5',
 description='This is the setup for the basic Application library',
 long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
 url='',
 author='Arche',
 author_email='rkdyava@gmail.com',
 classifiers=classifiers,
 keywords='Setup',
```

