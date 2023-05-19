# Comparing `tmp/melexis-i2c-stick-0.1.1.tar.gz` & `tmp/melexis-i2c-stick-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "melexis-i2c-stick-0.1.1.tar", last modified: Fri May 19 19:18:00 2023, max compression
+gzip compressed data, was "melexis-i2c-stick-0.1.2.tar", last modified: Fri May 19 21:48:58 2023, max compression
```

## Comparing `melexis-i2c-stick-0.1.1.tar` & `melexis-i2c-stick-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:18:00.206321 melexis-i2c-stick-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-19 19:17:46.000000 melexis-i2c-stick-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-19 19:17:46.000000 melexis-i2c-stick-0.1.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-19 19:18:00.206321 melexis-i2c-stick-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-19 19:17:46.000000 melexis-i2c-stick-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:18:00.206321 melexis-i2c-stick-0.1.1/melexis_i2c_stick.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-19 19:18:00.000000 melexis-i2c-stick-0.1.1/melexis_i2c_stick.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-19 19:18:00.000000 melexis-i2c-stick-0.1.1/melexis_i2c_stick.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 19:18:00.000000 melexis-i2c-stick-0.1.1/melexis_i2c_stick.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-19 19:18:00.000000 melexis-i2c-stick-0.1.1/melexis_i2c_stick.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 19:18:00.000000 melexis-i2c-stick-0.1.1/melexis_i2c_stick.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-19 19:18:00.206321 melexis-i2c-stick-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-05-19 19:17:46.000000 melexis-i2c-stick-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:48:58.960343 melexis-i2c-stick-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-19 21:48:47.000000 melexis-i2c-stick-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-19 21:48:47.000000 melexis-i2c-stick-0.1.2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-19 21:48:58.960343 melexis-i2c-stick-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-19 21:48:47.000000 melexis-i2c-stick-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:48:58.960343 melexis-i2c-stick-0.1.2/melexis_i2c_stick.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-19 21:48:58.000000 melexis-i2c-stick-0.1.2/melexis_i2c_stick.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-19 21:48:58.000000 melexis-i2c-stick-0.1.2/melexis_i2c_stick.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 21:48:58.000000 melexis-i2c-stick-0.1.2/melexis_i2c_stick.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 21:48:58.000000 melexis-i2c-stick-0.1.2/melexis_i2c_stick.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-19 21:48:58.000000 melexis-i2c-stick-0.1.2/melexis_i2c_stick.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 21:48:58.000000 melexis-i2c-stick-0.1.2/melexis_i2c_stick.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-19 21:48:58.960343 melexis-i2c-stick-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-19 21:48:47.000000 melexis-i2c-stick-0.1.2/setup.py
```

### Comparing `melexis-i2c-stick-0.1.1/LICENSE` & `melexis-i2c-stick-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `melexis-i2c-stick-0.1.1/PKG-INFO` & `melexis-i2c-stick-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Metadata-Version: 2.1
 Name: melexis-i2c-stick
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python package for I2C Stick
 Home-page: https://github.com/melexis/i2c-stick
-Download-URL: https://github.com/melexis/i2c-stick/archive/melexis-i2c-stick-py-V0.1.1.tar.gz
 License: Apache License, Version 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
```

### Comparing `melexis-i2c-stick-0.1.1/melexis_i2c_stick.egg-info/PKG-INFO` & `melexis-i2c-stick-0.1.2/melexis_i2c_stick.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Metadata-Version: 2.1
 Name: melexis-i2c-stick
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python package for I2C Stick
 Home-page: https://github.com/melexis/i2c-stick
-Download-URL: https://github.com/melexis/i2c-stick/archive/melexis-i2c-stick-py-V0.1.1.tar.gz
 License: Apache License, Version 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
```

### Comparing `melexis-i2c-stick-0.1.1/setup.py` & `melexis-i2c-stick-0.1.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 import sys
 import platform
 from setuptools import find_namespace_packages
 
 
-version='0.1.1'
+version='0.1.2'
 
 requires = ['bincopy>=17.14.5',
             'pyserial>=3.5',
             ]
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
@@ -24,15 +24,14 @@
     version=version,
     description='Python package for I2C Stick',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='Apache License, Version 2.0',
     install_requires=requires,
     url = 'https://github.com/melexis/i2c-stick',   # Provide either the link to your github or to your website
-    download_url = 'https://github.com/melexis/i2c-stick/archive/melexis-i2c-stick-py-V'+version+'.tar.gz',
     packages=find_namespace_packages(include=['mynamespace.*']),
     classifiers=[
         # complete classifier list: http://pypi.python.org/pypi?%3Aaction=list_classifiers
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: Microsoft :: Windows',
@@ -44,8 +43,9 @@
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Topic :: Utilities',
     ],
+    zip_safe=False,
 )
```

