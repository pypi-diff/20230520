# Comparing `tmp/archeSetup-0.0.3.tar.gz` & `tmp/archeSetup-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archeSetup-0.0.3.tar", last modified: Sat May 20 13:47:09 2023, max compression
+gzip compressed data, was "archeSetup-0.0.4.tar", last modified: Sat May 20 14:07:13 2023, max compression
```

## Comparing `archeSetup-0.0.3.tar` & `archeSetup-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 13:47:09.358274 archeSetup-0.0.3/
--rw-rw-rw-   0        0        0      101 2023-05-20 13:46:17.000000 archeSetup-0.0.3/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1072 2023-05-20 12:20:31.000000 archeSetup-0.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0       26 2023-05-20 12:18:33.000000 archeSetup-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      767 2023-05-20 13:47:09.357273 archeSetup-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       74 2023-05-20 13:47:05.000000 archeSetup-0.0.3/README.txt
-drwxrwxrwx   0        0        0        0 2023-05-20 13:47:09.349271 archeSetup-0.0.3/archeInitialze/
--rw-rw-rw-   0        0        0      221 2023-05-20 13:45:25.000000 archeSetup-0.0.3/archeInitialze/_init_.py
--rw-rw-rw-   0        0        0     1154 2023-05-20 13:43:11.000000 archeSetup-0.0.3/archeInitialze/initApp.py
-drwxrwxrwx   0        0        0        0 2023-05-20 13:47:09.357273 archeSetup-0.0.3/archeSetup.egg-info/
--rw-rw-rw-   0        0        0      767 2023-05-20 13:47:09.000000 archeSetup-0.0.3/archeSetup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-05-20 13:47:09.000000 archeSetup-0.0.3/archeSetup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 13:47:09.000000 archeSetup-0.0.3/archeSetup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 13:47:09.000000 archeSetup-0.0.3/archeSetup.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-20 13:47:09.358274 archeSetup-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      665 2023-05-20 13:46:34.000000 archeSetup-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 14:07:13.268304 archeSetup-0.0.4/
+-rw-rw-rw-   0        0        0      101 2023-05-20 13:46:17.000000 archeSetup-0.0.4/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1072 2023-05-20 12:20:31.000000 archeSetup-0.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0       26 2023-05-20 12:18:33.000000 archeSetup-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      769 2023-05-20 14:07:13.268304 archeSetup-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       74 2023-05-20 13:47:05.000000 archeSetup-0.0.4/README.txt
+drwxrwxrwx   0        0        0        0 2023-05-20 14:07:13.258302 archeSetup-0.0.4/archeInitialze/
+-rw-rw-rw-   0        0        0      221 2023-05-20 14:05:44.000000 archeSetup-0.0.4/archeInitialze/__init__.py
+-rw-rw-rw-   0        0        0     1119 2023-05-20 13:47:35.000000 archeSetup-0.0.4/archeInitialze/initApp.py
+drwxrwxrwx   0        0        0        0 2023-05-20 14:07:13.267304 archeSetup-0.0.4/archeSetup.egg-info/
+-rw-rw-rw-   0        0        0      769 2023-05-20 14:07:13.000000 archeSetup-0.0.4/archeSetup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-05-20 14:07:13.000000 archeSetup-0.0.4/archeSetup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 14:07:13.000000 archeSetup-0.0.4/archeSetup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-20 14:07:13.000000 archeSetup-0.0.4/archeSetup.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-20 14:07:13.268304 archeSetup-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      667 2023-05-20 14:07:07.000000 archeSetup-0.0.4/setup.py
```

### Comparing `archeSetup-0.0.3/LICENSE.txt` & `archeSetup-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `archeSetup-0.0.3/PKG-INFO` & `archeSetup-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 1.1
 Name: archeSetup
-Version: 0.0.3
+Version: 0.0.4
 Summary: This is the setup for the basic Application library
 Home-page: UNKNOWN
 Author: Arche
 Author-email: rkdyava@gmail.com
 License: UNKNOWN
 Description: This is the  initialisation of the application and it will be use as check
         
         Chnage LOG
         ==========
         
         
         0.0.3 (20/05/2023)
         ------------------
         - third  Release after bug fixing
-Keywords: add
+Keywords: Setup
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `archeSetup-0.0.3/archeInitialze/initApp.py` & `archeSetup-0.0.4/archeInitialze/initApp.py`

 * *Files 16% similar despite different names*

```diff
@@ -46,10 +46,10 @@
     # print(month)
     # print(year)
     # print(key)
     # print(encryption_online)
    
 
 
-# ouput = license(1237910791138560)
+
 
 # print("the license ouput:", ouput)
```

### Comparing `archeSetup-0.0.3/archeSetup.egg-info/PKG-INFO` & `archeSetup-0.0.4/archeSetup.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 1.1
 Name: archeSetup
-Version: 0.0.3
+Version: 0.0.4
 Summary: This is the setup for the basic Application library
 Home-page: UNKNOWN
 Author: Arche
 Author-email: rkdyava@gmail.com
 License: UNKNOWN
 Description: This is the  initialisation of the application and it will be use as check
         
         Chnage LOG
         ==========
         
         
         0.0.3 (20/05/2023)
         ------------------
         - third  Release after bug fixing
-Keywords: add
+Keywords: Setup
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `archeSetup-0.0.3/setup.py` & `archeSetup-0.0.4/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 
 
 ]
 
 setup(
 
 name = 'archeSetup',
-version='0.0.3',
+version='0.0.4',
 description='This is the setup for the basic Application library',
 long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
 url='',
 author='Arche',
 author_email='rkdyava@gmail.com',
 classifiers=classifiers,
-keywords='add',
+keywords='Setup',
 packages=find_packages(),
 install_requires=['']
```

