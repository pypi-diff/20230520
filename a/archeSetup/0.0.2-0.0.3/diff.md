# Comparing `tmp/archeSetup-0.0.2.tar.gz` & `tmp/archeSetup-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archeSetup-0.0.2.tar", last modified: Sat May 20 13:23:39 2023, max compression
+gzip compressed data, was "archeSetup-0.0.3.tar", last modified: Sat May 20 13:47:09 2023, max compression
```

## Comparing `archeSetup-0.0.2.tar` & `archeSetup-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 13:23:39.809285 archeSetup-0.0.2/
--rw-rw-rw-   0        0        0       84 2023-05-20 13:21:50.000000 archeSetup-0.0.2/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1072 2023-05-20 12:20:31.000000 archeSetup-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0       26 2023-05-20 12:18:33.000000 archeSetup-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      743 2023-05-20 13:23:39.809285 archeSetup-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       71 2023-05-20 13:22:12.000000 archeSetup-0.0.2/README.txt
-drwxrwxrwx   0        0        0        0 2023-05-20 13:23:39.805284 archeSetup-0.0.2/archeInitialze/
--rw-rw-rw-   0        0        0      197 2023-05-20 13:19:18.000000 archeSetup-0.0.2/archeInitialze/_init_.py
--rw-rw-rw-   0        0        0     1152 2023-05-20 13:22:16.000000 archeSetup-0.0.2/archeInitialze/initApp.py
-drwxrwxrwx   0        0        0        0 2023-05-20 13:23:39.808286 archeSetup-0.0.2/archeSetup.egg-info/
--rw-rw-rw-   0        0        0      743 2023-05-20 13:23:39.000000 archeSetup-0.0.2/archeSetup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-05-20 13:23:39.000000 archeSetup-0.0.2/archeSetup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 13:23:39.000000 archeSetup-0.0.2/archeSetup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 13:23:39.000000 archeSetup-0.0.2/archeSetup.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-20 13:23:39.809285 archeSetup-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      661 2023-05-20 13:22:39.000000 archeSetup-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 13:47:09.358274 archeSetup-0.0.3/
+-rw-rw-rw-   0        0        0      101 2023-05-20 13:46:17.000000 archeSetup-0.0.3/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1072 2023-05-20 12:20:31.000000 archeSetup-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0       26 2023-05-20 12:18:33.000000 archeSetup-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      767 2023-05-20 13:47:09.357273 archeSetup-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       74 2023-05-20 13:47:05.000000 archeSetup-0.0.3/README.txt
+drwxrwxrwx   0        0        0        0 2023-05-20 13:47:09.349271 archeSetup-0.0.3/archeInitialze/
+-rw-rw-rw-   0        0        0      221 2023-05-20 13:45:25.000000 archeSetup-0.0.3/archeInitialze/_init_.py
+-rw-rw-rw-   0        0        0     1154 2023-05-20 13:43:11.000000 archeSetup-0.0.3/archeInitialze/initApp.py
+drwxrwxrwx   0        0        0        0 2023-05-20 13:47:09.357273 archeSetup-0.0.3/archeSetup.egg-info/
+-rw-rw-rw-   0        0        0      767 2023-05-20 13:47:09.000000 archeSetup-0.0.3/archeSetup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-05-20 13:47:09.000000 archeSetup-0.0.3/archeSetup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 13:47:09.000000 archeSetup-0.0.3/archeSetup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 13:47:09.000000 archeSetup-0.0.3/archeSetup.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-20 13:47:09.358274 archeSetup-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      665 2023-05-20 13:46:34.000000 archeSetup-0.0.3/setup.py
```

### Comparing `archeSetup-0.0.2/LICENSE.txt` & `archeSetup-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `archeSetup-0.0.2/PKG-INFO` & `archeSetup-0.0.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 1.1
 Name: archeSetup
-Version: 0.0.2
-Summary: This is the setup the basic Application library
+Version: 0.0.3
+Summary: This is the setup for the basic Application library
 Home-page: UNKNOWN
 Author: Arche
 Author-email: rkdyava@gmail.com
 License: UNKNOWN
-Description: This is the application for adding the initilisation of the application
+Description: This is the  initialisation of the application and it will be use as check
         
         Chnage LOG
         ==========
         
         
-        0.0.2 (20/05/2023)
+        0.0.3 (20/05/2023)
         ------------------
-        - second Release
+        - third  Release after bug fixing
 Keywords: add
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `archeSetup-0.0.2/archeInitialze/initApp.py` & `archeSetup-0.0.3/archeInitialze/initApp.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,10 +46,10 @@
     # print(month)
     # print(year)
     # print(key)
     # print(encryption_online)
    
 
 
-ouput = license(1237910791138560)
+# ouput = license(1237910791138560)
 
 # print("the license ouput:", ouput)
```

### Comparing `archeSetup-0.0.2/archeSetup.egg-info/PKG-INFO` & `archeSetup-0.0.3/archeSetup.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 1.1
 Name: archeSetup
-Version: 0.0.2
-Summary: This is the setup the basic Application library
+Version: 0.0.3
+Summary: This is the setup for the basic Application library
 Home-page: UNKNOWN
 Author: Arche
 Author-email: rkdyava@gmail.com
 License: UNKNOWN
-Description: This is the application for adding the initilisation of the application
+Description: This is the  initialisation of the application and it will be use as check
         
         Chnage LOG
         ==========
         
         
-        0.0.2 (20/05/2023)
+        0.0.3 (20/05/2023)
         ------------------
-        - second Release
+        - third  Release after bug fixing
 Keywords: add
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `archeSetup-0.0.2/setup.py` & `archeSetup-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
 
 ]
 
 setup(
 
 name = 'archeSetup',
-version='0.0.2',
-description='This is the setup the basic Application library',
+version='0.0.3',
+description='This is the setup for the basic Application library',
 long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
 url='',
 author='Arche',
 author_email='rkdyava@gmail.com',
 classifiers=classifiers,
 keywords='add',
 packages=find_packages(),
```

