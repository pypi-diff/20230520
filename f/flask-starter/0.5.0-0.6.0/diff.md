# Comparing `tmp/flask-starter-0.5.0.tar.gz` & `tmp/flask-starter-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-starter-0.5.0.tar", last modified: Thu Mar 30 06:44:26 2023, max compression
+gzip compressed data, was "flask-starter-0.6.0.tar", last modified: Sat May 20 13:42:04 2023, max compression
```

## Comparing `flask-starter-0.5.0.tar` & `flask-starter-0.6.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 proshan   (1003) proshan   (1003)        0 2023-03-30 06:44:26.699684 flask-starter-0.5.0/
--rw-rw-r--   0 proshan   (1003) proshan   (1003)     1070 2023-01-13 07:21:17.000000 flask-starter-0.5.0/LICENSE
--rw-rw-r--   0 proshan   (1003) proshan   (1003)     2277 2023-03-30 06:44:26.699684 flask-starter-0.5.0/PKG-INFO
--rw-rw-r--   0 proshan   (1003) proshan   (1003)     1635 2023-03-30 06:42:23.000000 flask-starter-0.5.0/README.rst
-drwxrwxr-x   0 proshan   (1003) proshan   (1003)        0 2023-03-30 06:44:26.699684 flask-starter-0.5.0/flask_starter.egg-info/
--rw-rw-r--   0 proshan   (1003) proshan   (1003)     2277 2023-03-30 06:44:26.000000 flask-starter-0.5.0/flask_starter.egg-info/PKG-INFO
--rw-rw-r--   0 proshan   (1003) proshan   (1003)      300 2023-03-30 06:44:26.000000 flask-starter-0.5.0/flask_starter.egg-info/SOURCES.txt
--rw-rw-r--   0 proshan   (1003) proshan   (1003)        1 2023-03-30 06:44:26.000000 flask-starter-0.5.0/flask_starter.egg-info/dependency_links.txt
--rw-rw-r--   0 proshan   (1003) proshan   (1003)       54 2023-03-30 06:44:26.000000 flask-starter-0.5.0/flask_starter.egg-info/entry_points.txt
--rw-rw-r--   0 proshan   (1003) proshan   (1003)       30 2023-03-30 06:44:26.000000 flask-starter-0.5.0/flask_starter.egg-info/requires.txt
--rw-rw-r--   0 proshan   (1003) proshan   (1003)        7 2023-03-30 06:44:26.000000 flask-starter-0.5.0/flask_starter.egg-info/top_level.txt
--rw-rw-r--   0 proshan   (1003) proshan   (1003)      554 2023-03-30 06:42:08.000000 flask-starter-0.5.0/script.py
--rw-rw-r--   0 proshan   (1003) proshan   (1003)       38 2023-03-30 06:44:26.699684 flask-starter-0.5.0/setup.cfg
--rw-rw-r--   0 proshan   (1003) proshan   (1003)     1055 2023-03-30 06:42:04.000000 flask-starter-0.5.0/setup.py
-drwxrwxr-x   0 proshan   (1003) proshan   (1003)        0 2023-03-30 06:44:26.699684 flask-starter-0.5.0/tests/
--rw-rw-r--   0 proshan   (1003) proshan   (1003)        0 2023-01-13 07:36:30.000000 flask-starter-0.5.0/tests/test_libs.py
--rw-rw-r--   0 proshan   (1003) proshan   (1003)      342 2023-03-30 06:42:08.000000 flask-starter-0.5.0/tests/test_views.py
+drwxrwxr-x   0 proshan   (1003) proshan   (1003)        0 2023-05-20 13:42:04.210765 flask-starter-0.6.0/
+-rw-rw-r--   0 proshan   (1003) proshan   (1003)     1070 2023-05-20 13:38:30.000000 flask-starter-0.6.0/LICENSE
+-rw-rw-r--   0 proshan   (1003) proshan   (1003)     2277 2023-05-20 13:42:04.210765 flask-starter-0.6.0/PKG-INFO
+-rw-rw-r--   0 proshan   (1003) proshan   (1003)     1635 2023-05-20 13:38:30.000000 flask-starter-0.6.0/README.rst
+drwxrwxr-x   0 proshan   (1003) proshan   (1003)        0 2023-05-20 13:42:04.210765 flask-starter-0.6.0/flask_starter.egg-info/
+-rw-rw-r--   0 proshan   (1003) proshan   (1003)     2277 2023-05-20 13:42:04.000000 flask-starter-0.6.0/flask_starter.egg-info/PKG-INFO
+-rw-rw-r--   0 proshan   (1003) proshan   (1003)      300 2023-05-20 13:42:04.000000 flask-starter-0.6.0/flask_starter.egg-info/SOURCES.txt
+-rw-rw-r--   0 proshan   (1003) proshan   (1003)        1 2023-05-20 13:42:04.000000 flask-starter-0.6.0/flask_starter.egg-info/dependency_links.txt
+-rw-rw-r--   0 proshan   (1003) proshan   (1003)       54 2023-05-20 13:42:04.000000 flask-starter-0.6.0/flask_starter.egg-info/entry_points.txt
+-rw-rw-r--   0 proshan   (1003) proshan   (1003)       30 2023-05-20 13:42:04.000000 flask-starter-0.6.0/flask_starter.egg-info/requires.txt
+-rw-rw-r--   0 proshan   (1003) proshan   (1003)        7 2023-05-20 13:42:04.000000 flask-starter-0.6.0/flask_starter.egg-info/top_level.txt
+-rw-rw-r--   0 proshan   (1003) proshan   (1003)      599 2023-05-20 13:38:30.000000 flask-starter-0.6.0/script.py
+-rw-rw-r--   0 proshan   (1003) proshan   (1003)       38 2023-05-20 13:42:04.210765 flask-starter-0.6.0/setup.cfg
+-rw-rw-r--   0 proshan   (1003) proshan   (1003)     1055 2023-05-20 13:41:16.000000 flask-starter-0.6.0/setup.py
+drwxrwxr-x   0 proshan   (1003) proshan   (1003)        0 2023-05-20 13:42:04.210765 flask-starter-0.6.0/tests/
+-rw-rw-r--   0 proshan   (1003) proshan   (1003)        0 2023-05-20 13:38:30.000000 flask-starter-0.6.0/tests/test_libs.py
+-rw-rw-r--   0 proshan   (1003) proshan   (1003)      342 2023-05-20 13:38:30.000000 flask-starter-0.6.0/tests/test_views.py
```

### Comparing `flask-starter-0.5.0/LICENSE` & `flask-starter-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-starter-0.5.0/PKG-INFO` & `flask-starter-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-starter
-Version: 0.5.0
+Version: 0.6.0
 Summary: A flask extension which contains a basic app and is configured in your local machine through a command line utility 
 Home-page: https://github.com/princekrroshan01/flask-starter
 Author: Prince Roshan
 Author-email: princekrroshan01@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `flask-starter-0.5.0/README.rst` & `flask-starter-0.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `flask-starter-0.5.0/flask_starter.egg-info/PKG-INFO` & `flask-starter-0.6.0/flask_starter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-starter
-Version: 0.5.0
+Version: 0.6.0
 Summary: A flask extension which contains a basic app and is configured in your local machine through a command line utility 
 Home-page: https://github.com/princekrroshan01/flask-starter
 Author: Prince Roshan
 Author-email: princekrroshan01@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `flask-starter-0.5.0/script.py` & `flask-starter-0.6.0/script.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import os
+import shutil
+
 import click
 
 """
 #process_with_auth
 need to copy extra files in templates and static  
 #process_without_auth 
 """
@@ -12,13 +14,14 @@
 def main():
     os.system("git init")
     os.system("git clone https://github.com/princekrroshan01/flask-starter.git")
     os.remove("flask-starter/script.py")
     os.remove("flask-starter/setup.py")
     os.remove("flask-starter/LICENSE")
     os.remove("flask-starter/.gitignore")
-    os.remove("flask-starter/README.md")
+    os.remove("flask-starter/README.rst")
     os.remove("flask-starter/requirements.txt")
+    shutil.rmtree('.github')
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `flask-starter-0.5.0/setup.py` & `flask-starter-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name="flask-starter",
-    version="0.5.0",
+    version="0.6.0",
     author="Prince Roshan",
     author_email="princekrroshan01@gmail.com",
     url="https://github.com/princekrroshan01/flask-starter",
     description=(
         "A flask extension which contains a basic app and is configured in your local machine through a command line utility "
     ),
     long_description=read("README.rst"),
```

