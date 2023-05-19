# Comparing `tmp/wait_for_it_to-0.0.8.tar.gz` & `tmp/wait_for_it_to-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wait_for_it_to-0.0.8.tar", last modified: Tue Aug 13 17:35:53 2019, max compression
+gzip compressed data, was "dist/wait_for_it_to-0.0.9.tar", last modified: Thu Aug 15 09:04:06 2019, max compression
```

## Comparing `wait_for_it_to-0.0.8.tar` & `wait_for_it_to-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-13 17:35:53.000000 wait_for_it_to-0.0.8/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3075 2019-08-13 17:35:53.000000 wait_for_it_to-0.0.8/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1873 2019-08-13 17:35:23.000000 wait_for_it_to-0.0.8/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)       79 2019-08-13 17:35:53.000000 wait_for_it_to-0.0.8/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1273 2019-08-13 17:35:23.000000 wait_for_it_to-0.0.8/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-13 17:35:53.000000 wait_for_it_to-0.0.8/wait_for_it_to/
--rw-rw-r--   0 travis    (2000) travis    (2000)      736 2019-08-13 17:35:23.000000 wait_for_it_to-0.0.8/wait_for_it_to/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       81 2019-08-13 17:35:23.000000 wait_for_it_to-0.0.8/wait_for_it_to/_version.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-13 17:35:53.000000 wait_for_it_to-0.0.8/wait_for_it_to.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3075 2019-08-13 17:35:53.000000 wait_for_it_to-0.0.8/wait_for_it_to.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      234 2019-08-13 17:35:53.000000 wait_for_it_to-0.0.8/wait_for_it_to.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-08-13 17:35:53.000000 wait_for_it_to-0.0.8/wait_for_it_to.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       15 2019-08-13 17:35:53.000000 wait_for_it_to-0.0.8/wait_for_it_to.egg-info/top_level.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-15 09:04:06.000000 wait_for_it_to-0.0.9/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3304 2019-08-15 09:04:06.000000 wait_for_it_to-0.0.9/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2038 2019-08-15 09:03:34.000000 wait_for_it_to-0.0.9/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)       79 2019-08-15 09:04:06.000000 wait_for_it_to-0.0.9/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1397 2019-08-15 09:03:34.000000 wait_for_it_to-0.0.9/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-15 09:04:06.000000 wait_for_it_to-0.0.9/wait_for_it_to/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1394 2019-08-15 09:03:34.000000 wait_for_it_to-0.0.9/wait_for_it_to/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       80 2019-08-15 09:03:34.000000 wait_for_it_to-0.0.9/wait_for_it_to/_version.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-15 09:04:06.000000 wait_for_it_to-0.0.9/wait_for_it_to.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3304 2019-08-15 09:04:06.000000 wait_for_it_to-0.0.9/wait_for_it_to.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      234 2019-08-15 09:04:06.000000 wait_for_it_to-0.0.9/wait_for_it_to.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-08-15 09:04:06.000000 wait_for_it_to-0.0.9/wait_for_it_to.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       15 2019-08-15 09:04:06.000000 wait_for_it_to-0.0.9/wait_for_it_to.egg-info/top_level.txt
```

### Comparing `wait_for_it_to-0.0.8/PKG-INFO` & `wait_for_it_to-0.0.9/wait_for_it_to.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 Metadata-Version: 2.1
-Name: wait_for_it_to
-Version: 0.0.8
+Name: wait-for-it-to
+Version: 0.0.9
 Summary: helper library which waits
 Home-page: https://github.com/studioj/wait_for_it/
 Author: Jef Neefs
 Author-email: neefsj@gmail.com
 License: GPL
 Description: # waitforit
-        ## Badges
-        ### Travis Build
+        ### Badges
+        ##### Travis Build
         [![Build Status](https://travis-ci.com/studioj/wait_for_it.svg?branch=master)](https://travis-ci.com/studioj/wait_for_it)
         
-        ### Code and Test Quality
+        ##### Code and Test Quality
         [![codecov](https://codecov.io/gh/studioj/wait_for_it/branch/master/graph/badge.svg)](https://codecov.io/gh/studioj/wait_for_it)
         [![BCH compliance](https://bettercodehub.com/edge/badge/studioj/wait_for_it?branch=master)](https://bettercodehub.com/)
         [![CodeFactor](https://www.codefactor.io/repository/github/studioj/wait_for_it/badge)](https://www.codefactor.io/repository/github/studioj/wait_for_it)
         
-        ### SonarQube
+        ##### SonarQube
         [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=studioj_wait_for_it&metric=alert_status)](https://sonarcloud.io/dashboard?id=studioj_wait_for_it)
         [![Code Smells](https://sonarcloud.io/api/project_badges/measure?project=studioj_wait_for_it&metric=code_smells)](https://sonarcloud.io/dashboard?id=studioj_wait_for_it)
         [![Bugs](https://sonarcloud.io/api/project_badges/measure?project=studioj_wait_for_it&metric=bugs)](https://sonarcloud.io/dashboard?id=studioj_wait_for_it)
         [![Vulnerabilities](https://sonarcloud.io/api/project_badges/measure?project=studioj_wait_for_it&metric=vulnerabilities)](https://sonarcloud.io/dashboard?id=studioj_wait_for_it)
         
+        ##### PyPI
+        
+        ![PyPI - Downloads](https://img.shields.io/pypi/dw/wait_for_it_to?style=flat)
+        
         This is a library for letting your python code wait for a certain action to complete
         
         short example
         
         ```python
         import wait_for_it_to
         def foo():
@@ -39,18 +43,22 @@
         >> wait_for_it_to.be_true(bar)
         Traceback (most recent call last):
           File "<stdin>", line 1, in <module>
           File "..\wait_for_it\wait_for_it_to\__init__.py", line 27, in be_true
             raise TimeoutError(msg)
         TimeoutError: expected something that evaluates to True, but got False instead
         
+        >> wait_for_it_to.be_true(foo, timeout=5)
         ```
         #### Version History
         0.0.7: first release
+        
         0.0.8: adding timeout functionality
+        
+        0.0.9: adding be false
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python
```

### Comparing `wait_for_it_to-0.0.8/README.md` & `wait_for_it_to-0.0.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 # waitforit
-## Badges
-### Travis Build
+### Badges
+##### Travis Build
 [![Build Status](https://travis-ci.com/studioj/wait_for_it.svg?branch=master)](https://travis-ci.com/studioj/wait_for_it)
 
-### Code and Test Quality
+##### Code and Test Quality
 [![codecov](https://codecov.io/gh/studioj/wait_for_it/branch/master/graph/badge.svg)](https://codecov.io/gh/studioj/wait_for_it)
 [![BCH compliance](https://bettercodehub.com/edge/badge/studioj/wait_for_it?branch=master)](https://bettercodehub.com/)
 [![CodeFactor](https://www.codefactor.io/repository/github/studioj/wait_for_it/badge)](https://www.codefactor.io/repository/github/studioj/wait_for_it)
 
-### SonarQube
+##### SonarQube
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=studioj_wait_for_it&metric=alert_status)](https://sonarcloud.io/dashboard?id=studioj_wait_for_it)
 [![Code Smells](https://sonarcloud.io/api/project_badges/measure?project=studioj_wait_for_it&metric=code_smells)](https://sonarcloud.io/dashboard?id=studioj_wait_for_it)
 [![Bugs](https://sonarcloud.io/api/project_badges/measure?project=studioj_wait_for_it&metric=bugs)](https://sonarcloud.io/dashboard?id=studioj_wait_for_it)
 [![Vulnerabilities](https://sonarcloud.io/api/project_badges/measure?project=studioj_wait_for_it&metric=vulnerabilities)](https://sonarcloud.io/dashboard?id=studioj_wait_for_it)
 
+##### PyPI
+
+![PyPI - Downloads](https://img.shields.io/pypi/dw/wait_for_it_to?style=flat)
+
 This is a library for letting your python code wait for a certain action to complete
 
 short example
 
 ```python
 import wait_for_it_to
 def foo():
@@ -31,11 +35,15 @@
 >> wait_for_it_to.be_true(bar)
 Traceback (most recent call last):
   File "<stdin>", line 1, in <module>
   File "..\wait_for_it\wait_for_it_to\__init__.py", line 27, in be_true
     raise TimeoutError(msg)
 TimeoutError: expected something that evaluates to True, but got False instead
 
+>> wait_for_it_to.be_true(foo, timeout=5)
 ```
 #### Version History
 0.0.7: first release
-0.0.8: adding timeout functionality
+
+0.0.8: adding timeout functionality
+
+0.0.9: adding be false
```

### Comparing `wait_for_it_to-0.0.8/setup.py` & `wait_for_it_to-0.0.9/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,25 +5,28 @@
 from wait_for_it_to import __version__
 
 version = __version__
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
+with open('test_requirements.txt') as f:
+    test_requirements = f.read().splitlines()
 
 setup(
     name="wait_for_it_to",
     version=version,
     description="helper library which waits",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Jef Neefs",
     author_email="neefsj@gmail.com",
     url="https://github.com/studioj/wait_for_it/",
     packages=["wait_for_it_to"],
+    tests_require=test_requirements,
     license="GPL",
     platforms="Posix; MacOS X; Windows",
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
```

### Comparing `wait_for_it_to-0.0.8/wait_for_it_to/__init__.py` & `wait_for_it_to-0.0.9/wait_for_it_to/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,18 +12,43 @@
     :param func: an executable object
 
     >>>def foo():
     >>>  return True
     >>>
     >>>wait_for_it_to.be_true(foo)
     >>>wait_for_it_to.be_true(foo, timeout=5)
-    
+
     """
     start = time.time()
     while True:
         result = func()
         if result:
             return True
         if time.time() > start + timeout:
             msg = "expected something that evaluates to True, but got %s instead" % str(result)
             raise TimeoutError(msg)
         time.sleep(0.01)
+
+
+def be_false(func, timeout=10):
+    """
+    waits until func evaluates to False
+    raises an exception when the timeout expires
+
+    :param timeout: a timeout in seconds
+    :param func: an executable object
+
+    >>>def foo():
+    >>>  return False
+    >>>
+    >>>wait_for_it_to.be_false(foo)
+    >>>wait_for_it_to.be_false(foo, timeout=5)
+    """
+    start = time.time()
+    while True:
+        result = func()
+        if not result:
+            return False
+        if time.time() > start + timeout:
+            msg = "expected something that evaluates to True, but got %s instead" % str(result)
+            raise TimeoutError(msg)
+        time.sleep(0.01)
```

### Comparing `wait_for_it_to-0.0.8/wait_for_it_to.egg-info/PKG-INFO` & `wait_for_it_to-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 Metadata-Version: 2.1
-Name: wait-for-it-to
-Version: 0.0.8
+Name: wait_for_it_to
+Version: 0.0.9
 Summary: helper library which waits
 Home-page: https://github.com/studioj/wait_for_it/
 Author: Jef Neefs
 Author-email: neefsj@gmail.com
 License: GPL
 Description: # waitforit
-        ## Badges
-        ### Travis Build
+        ### Badges
+        ##### Travis Build
         [![Build Status](https://travis-ci.com/studioj/wait_for_it.svg?branch=master)](https://travis-ci.com/studioj/wait_for_it)
         
-        ### Code and Test Quality
+        ##### Code and Test Quality
         [![codecov](https://codecov.io/gh/studioj/wait_for_it/branch/master/graph/badge.svg)](https://codecov.io/gh/studioj/wait_for_it)
         [![BCH compliance](https://bettercodehub.com/edge/badge/studioj/wait_for_it?branch=master)](https://bettercodehub.com/)
         [![CodeFactor](https://www.codefactor.io/repository/github/studioj/wait_for_it/badge)](https://www.codefactor.io/repository/github/studioj/wait_for_it)
         
-        ### SonarQube
+        ##### SonarQube
         [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=studioj_wait_for_it&metric=alert_status)](https://sonarcloud.io/dashboard?id=studioj_wait_for_it)
         [![Code Smells](https://sonarcloud.io/api/project_badges/measure?project=studioj_wait_for_it&metric=code_smells)](https://sonarcloud.io/dashboard?id=studioj_wait_for_it)
         [![Bugs](https://sonarcloud.io/api/project_badges/measure?project=studioj_wait_for_it&metric=bugs)](https://sonarcloud.io/dashboard?id=studioj_wait_for_it)
         [![Vulnerabilities](https://sonarcloud.io/api/project_badges/measure?project=studioj_wait_for_it&metric=vulnerabilities)](https://sonarcloud.io/dashboard?id=studioj_wait_for_it)
         
+        ##### PyPI
+        
+        ![PyPI - Downloads](https://img.shields.io/pypi/dw/wait_for_it_to?style=flat)
+        
         This is a library for letting your python code wait for a certain action to complete
         
         short example
         
         ```python
         import wait_for_it_to
         def foo():
@@ -39,18 +43,22 @@
         >> wait_for_it_to.be_true(bar)
         Traceback (most recent call last):
           File "<stdin>", line 1, in <module>
           File "..\wait_for_it\wait_for_it_to\__init__.py", line 27, in be_true
             raise TimeoutError(msg)
         TimeoutError: expected something that evaluates to True, but got False instead
         
+        >> wait_for_it_to.be_true(foo, timeout=5)
         ```
         #### Version History
         0.0.7: first release
+        
         0.0.8: adding timeout functionality
+        
+        0.0.9: adding be false
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python
```

