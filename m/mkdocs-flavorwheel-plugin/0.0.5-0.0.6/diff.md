# Comparing `tmp/mkdocs-flavorwheel-plugin-0.0.5.tar.gz` & `tmp/mkdocs-flavorwheel-plugin-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-flavorwheel-plugin-0.0.5.tar", last modified: Sat May 20 13:26:52 2023, max compression
+gzip compressed data, was "mkdocs-flavorwheel-plugin-0.0.6.tar", last modified: Sat May 20 13:32:42 2023, max compression
```

## Comparing `mkdocs-flavorwheel-plugin-0.0.5.tar` & `mkdocs-flavorwheel-plugin-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 pappmico   (501) staff       (20)        0 2023-05-20 13:26:52.151210 mkdocs-flavorwheel-plugin-0.0.5/
--rw-r--r--   0 pappmico   (501) staff       (20)     1053 2023-05-16 15:47:51.000000 mkdocs-flavorwheel-plugin-0.0.5/LICENSE
--rw-r--r--   0 pappmico   (501) staff       (20)      724 2023-05-20 13:26:52.151083 mkdocs-flavorwheel-plugin-0.0.5/PKG-INFO
--rw-r--r--   0 pappmico   (501) staff       (20)      967 2023-05-16 11:07:41.000000 mkdocs-flavorwheel-plugin-0.0.5/README.md
-drwxr-xr-x   0 pappmico   (501) staff       (20)        0 2023-05-20 13:26:52.150149 mkdocs-flavorwheel-plugin-0.0.5/mkdocs_flavorwheel_plugin/
--rw-r--r--   0 pappmico   (501) staff       (20)        0 2023-05-16 11:07:41.000000 mkdocs-flavorwheel-plugin-0.0.5/mkdocs_flavorwheel_plugin/__init__.py
--rw-r--r--   0 pappmico   (501) staff       (20)      708 2023-05-18 11:21:16.000000 mkdocs-flavorwheel-plugin-0.0.5/mkdocs_flavorwheel_plugin/plugin.py
-drwxr-xr-x   0 pappmico   (501) staff       (20)        0 2023-05-20 13:26:52.150914 mkdocs-flavorwheel-plugin-0.0.5/mkdocs_flavorwheel_plugin.egg-info/
--rw-r--r--   0 pappmico   (501) staff       (20)      724 2023-05-20 13:26:52.000000 mkdocs-flavorwheel-plugin-0.0.5/mkdocs_flavorwheel_plugin.egg-info/PKG-INFO
--rw-r--r--   0 pappmico   (501) staff       (20)      396 2023-05-20 13:26:52.000000 mkdocs-flavorwheel-plugin-0.0.5/mkdocs_flavorwheel_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 pappmico   (501) staff       (20)        1 2023-05-20 13:26:52.000000 mkdocs-flavorwheel-plugin-0.0.5/mkdocs_flavorwheel_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 pappmico   (501) staff       (20)       96 2023-05-20 13:26:52.000000 mkdocs-flavorwheel-plugin-0.0.5/mkdocs_flavorwheel_plugin.egg-info/entry_points.txt
--rw-r--r--   0 pappmico   (501) staff       (20)       14 2023-05-20 13:26:52.000000 mkdocs-flavorwheel-plugin-0.0.5/mkdocs_flavorwheel_plugin.egg-info/requires.txt
--rw-r--r--   0 pappmico   (501) staff       (20)       26 2023-05-20 13:26:52.000000 mkdocs-flavorwheel-plugin-0.0.5/mkdocs_flavorwheel_plugin.egg-info/top_level.txt
--rw-r--r--   0 pappmico   (501) staff       (20)       38 2023-05-20 13:26:52.151242 mkdocs-flavorwheel-plugin-0.0.5/setup.cfg
--rw-r--r--   0 pappmico   (501) staff       (20)     1066 2023-05-20 13:26:27.000000 mkdocs-flavorwheel-plugin-0.0.5/setup.py
+drwxr-xr-x   0 pappmico   (501) staff       (20)        0 2023-05-20 13:32:42.571573 mkdocs-flavorwheel-plugin-0.0.6/
+-rw-r--r--   0 pappmico   (501) staff       (20)     1053 2023-05-16 15:47:51.000000 mkdocs-flavorwheel-plugin-0.0.6/LICENSE
+-rw-r--r--   0 pappmico   (501) staff       (20)      724 2023-05-20 13:32:42.571465 mkdocs-flavorwheel-plugin-0.0.6/PKG-INFO
+-rw-r--r--   0 pappmico   (501) staff       (20)      967 2023-05-16 11:07:41.000000 mkdocs-flavorwheel-plugin-0.0.6/README.md
+drwxr-xr-x   0 pappmico   (501) staff       (20)        0 2023-05-20 13:32:42.570539 mkdocs-flavorwheel-plugin-0.0.6/mkdocs_flavorwheel_plugin/
+-rw-r--r--   0 pappmico   (501) staff       (20)        0 2023-05-16 11:07:41.000000 mkdocs-flavorwheel-plugin-0.0.6/mkdocs_flavorwheel_plugin/__init__.py
+-rw-r--r--   0 pappmico   (501) staff       (20)      708 2023-05-18 11:21:16.000000 mkdocs-flavorwheel-plugin-0.0.6/mkdocs_flavorwheel_plugin/plugin.py
+drwxr-xr-x   0 pappmico   (501) staff       (20)        0 2023-05-20 13:32:42.571316 mkdocs-flavorwheel-plugin-0.0.6/mkdocs_flavorwheel_plugin.egg-info/
+-rw-r--r--   0 pappmico   (501) staff       (20)      724 2023-05-20 13:32:42.000000 mkdocs-flavorwheel-plugin-0.0.6/mkdocs_flavorwheel_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 pappmico   (501) staff       (20)      396 2023-05-20 13:32:42.000000 mkdocs-flavorwheel-plugin-0.0.6/mkdocs_flavorwheel_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 pappmico   (501) staff       (20)        1 2023-05-20 13:32:42.000000 mkdocs-flavorwheel-plugin-0.0.6/mkdocs_flavorwheel_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 pappmico   (501) staff       (20)       96 2023-05-20 13:32:42.000000 mkdocs-flavorwheel-plugin-0.0.6/mkdocs_flavorwheel_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 pappmico   (501) staff       (20)       14 2023-05-20 13:32:42.000000 mkdocs-flavorwheel-plugin-0.0.6/mkdocs_flavorwheel_plugin.egg-info/requires.txt
+-rw-r--r--   0 pappmico   (501) staff       (20)       26 2023-05-20 13:32:42.000000 mkdocs-flavorwheel-plugin-0.0.6/mkdocs_flavorwheel_plugin.egg-info/top_level.txt
+-rw-r--r--   0 pappmico   (501) staff       (20)       38 2023-05-20 13:32:42.571603 mkdocs-flavorwheel-plugin-0.0.6/setup.cfg
+-rw-r--r--   0 pappmico   (501) staff       (20)     1066 2023-05-20 13:31:56.000000 mkdocs-flavorwheel-plugin-0.0.6/setup.py
```

### Comparing `mkdocs-flavorwheel-plugin-0.0.5/LICENSE` & `mkdocs-flavorwheel-plugin-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-flavorwheel-plugin-0.0.5/PKG-INFO` & `mkdocs-flavorwheel-plugin-0.0.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-flavorwheel-plugin
-Version: 0.0.5
+Version: 0.0.6
 Summary: MkDocs plugin
 Home-page: 
 Author: Mico Papp
 Author-email: papp.mico@gmail.com
 License: MIT
 Keywords: mkdocs
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mkdocs-flavorwheel-plugin-0.0.5/README.md` & `mkdocs-flavorwheel-plugin-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-flavorwheel-plugin-0.0.5/mkdocs_flavorwheel_plugin/plugin.py` & `mkdocs-flavorwheel-plugin-0.0.6/mkdocs_flavorwheel_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs-flavorwheel-plugin-0.0.5/mkdocs_flavorwheel_plugin.egg-info/PKG-INFO` & `mkdocs-flavorwheel-plugin-0.0.6/mkdocs_flavorwheel_plugin.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-flavorwheel-plugin
-Version: 0.0.5
+Version: 0.0.6
 Summary: MkDocs plugin
 Home-page: 
 Author: Mico Papp
 Author-email: papp.mico@gmail.com
 License: MIT
 Keywords: mkdocs
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mkdocs-flavorwheel-plugin-0.0.5/setup.py` & `mkdocs-flavorwheel-plugin-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='mkdocs-flavorwheel-plugin',
-    version='0.0.5',
+    version='0.0.6',
     description='MkDocs plugin',
     long_description='',
     keywords='mkdocs',
     url='',
     author='Mico Papp',
     author_email='papp.mico@gmail.com',
     license='MIT',
```

