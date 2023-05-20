# Comparing `tmp/mkdocs-flavorwheel-plugin-0.0.3.tar.gz` & `tmp/mkdocs-flavorwheel-plugin-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-flavorwheel-plugin-0.0.3.tar", last modified: Wed May 17 11:27:32 2023, max compression
+gzip compressed data, was "mkdocs-flavorwheel-plugin-0.0.4.tar", last modified: Sat May 20 13:02:27 2023, max compression
```

## Comparing `mkdocs-flavorwheel-plugin-0.0.3.tar` & `mkdocs-flavorwheel-plugin-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 pappmico   (501) staff       (20)        0 2023-05-17 11:27:32.363521 mkdocs-flavorwheel-plugin-0.0.3/
--rw-r--r--   0 pappmico   (501) staff       (20)     1053 2023-05-16 15:47:51.000000 mkdocs-flavorwheel-plugin-0.0.3/LICENSE
--rw-r--r--   0 pappmico   (501) staff       (20)      724 2023-05-17 11:27:32.363403 mkdocs-flavorwheel-plugin-0.0.3/PKG-INFO
--rw-r--r--   0 pappmico   (501) staff       (20)      967 2023-05-16 11:07:41.000000 mkdocs-flavorwheel-plugin-0.0.3/README.md
-drwxr-xr-x   0 pappmico   (501) staff       (20)        0 2023-05-17 11:27:32.362559 mkdocs-flavorwheel-plugin-0.0.3/mkdocs_flavorwheel_plugin/
--rw-r--r--   0 pappmico   (501) staff       (20)        0 2023-05-16 11:07:41.000000 mkdocs-flavorwheel-plugin-0.0.3/mkdocs_flavorwheel_plugin/__init__.py
--rw-r--r--   0 pappmico   (501) staff       (20)     2039 2023-05-16 16:02:39.000000 mkdocs-flavorwheel-plugin-0.0.3/mkdocs_flavorwheel_plugin/plugin.py
-drwxr-xr-x   0 pappmico   (501) staff       (20)        0 2023-05-17 11:27:32.363219 mkdocs-flavorwheel-plugin-0.0.3/mkdocs_flavorwheel_plugin.egg-info/
--rw-r--r--   0 pappmico   (501) staff       (20)      724 2023-05-17 11:27:32.000000 mkdocs-flavorwheel-plugin-0.0.3/mkdocs_flavorwheel_plugin.egg-info/PKG-INFO
--rw-r--r--   0 pappmico   (501) staff       (20)      396 2023-05-17 11:27:32.000000 mkdocs-flavorwheel-plugin-0.0.3/mkdocs_flavorwheel_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 pappmico   (501) staff       (20)        1 2023-05-17 11:27:32.000000 mkdocs-flavorwheel-plugin-0.0.3/mkdocs_flavorwheel_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 pappmico   (501) staff       (20)       96 2023-05-17 11:27:32.000000 mkdocs-flavorwheel-plugin-0.0.3/mkdocs_flavorwheel_plugin.egg-info/entry_points.txt
--rw-r--r--   0 pappmico   (501) staff       (20)       14 2023-05-17 11:27:32.000000 mkdocs-flavorwheel-plugin-0.0.3/mkdocs_flavorwheel_plugin.egg-info/requires.txt
--rw-r--r--   0 pappmico   (501) staff       (20)       26 2023-05-17 11:27:32.000000 mkdocs-flavorwheel-plugin-0.0.3/mkdocs_flavorwheel_plugin.egg-info/top_level.txt
--rw-r--r--   0 pappmico   (501) staff       (20)       38 2023-05-17 11:27:32.363557 mkdocs-flavorwheel-plugin-0.0.3/setup.cfg
--rw-r--r--   0 pappmico   (501) staff       (20)     1066 2023-05-17 11:27:17.000000 mkdocs-flavorwheel-plugin-0.0.3/setup.py
+drwxr-xr-x   0 pappmico   (501) staff       (20)        0 2023-05-20 13:02:27.129004 mkdocs-flavorwheel-plugin-0.0.4/
+-rw-r--r--   0 pappmico   (501) staff       (20)     1053 2023-05-16 15:47:51.000000 mkdocs-flavorwheel-plugin-0.0.4/LICENSE
+-rw-r--r--   0 pappmico   (501) staff       (20)      724 2023-05-20 13:02:27.128875 mkdocs-flavorwheel-plugin-0.0.4/PKG-INFO
+-rw-r--r--   0 pappmico   (501) staff       (20)      967 2023-05-16 11:07:41.000000 mkdocs-flavorwheel-plugin-0.0.4/README.md
+drwxr-xr-x   0 pappmico   (501) staff       (20)        0 2023-05-20 13:02:27.127880 mkdocs-flavorwheel-plugin-0.0.4/mkdocs_flavorwheel_plugin/
+-rw-r--r--   0 pappmico   (501) staff       (20)        0 2023-05-16 11:07:41.000000 mkdocs-flavorwheel-plugin-0.0.4/mkdocs_flavorwheel_plugin/__init__.py
+-rw-r--r--   0 pappmico   (501) staff       (20)      708 2023-05-18 11:21:16.000000 mkdocs-flavorwheel-plugin-0.0.4/mkdocs_flavorwheel_plugin/plugin.py
+drwxr-xr-x   0 pappmico   (501) staff       (20)        0 2023-05-20 13:02:27.128711 mkdocs-flavorwheel-plugin-0.0.4/mkdocs_flavorwheel_plugin.egg-info/
+-rw-r--r--   0 pappmico   (501) staff       (20)      724 2023-05-20 13:02:27.000000 mkdocs-flavorwheel-plugin-0.0.4/mkdocs_flavorwheel_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 pappmico   (501) staff       (20)      396 2023-05-20 13:02:27.000000 mkdocs-flavorwheel-plugin-0.0.4/mkdocs_flavorwheel_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 pappmico   (501) staff       (20)        1 2023-05-20 13:02:27.000000 mkdocs-flavorwheel-plugin-0.0.4/mkdocs_flavorwheel_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 pappmico   (501) staff       (20)       96 2023-05-20 13:02:27.000000 mkdocs-flavorwheel-plugin-0.0.4/mkdocs_flavorwheel_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 pappmico   (501) staff       (20)       14 2023-05-20 13:02:27.000000 mkdocs-flavorwheel-plugin-0.0.4/mkdocs_flavorwheel_plugin.egg-info/requires.txt
+-rw-r--r--   0 pappmico   (501) staff       (20)       26 2023-05-20 13:02:27.000000 mkdocs-flavorwheel-plugin-0.0.4/mkdocs_flavorwheel_plugin.egg-info/top_level.txt
+-rw-r--r--   0 pappmico   (501) staff       (20)       38 2023-05-20 13:02:27.129039 mkdocs-flavorwheel-plugin-0.0.4/setup.cfg
+-rw-r--r--   0 pappmico   (501) staff       (20)     1066 2023-05-17 19:33:26.000000 mkdocs-flavorwheel-plugin-0.0.4/setup.py
```

### Comparing `mkdocs-flavorwheel-plugin-0.0.3/LICENSE` & `mkdocs-flavorwheel-plugin-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-flavorwheel-plugin-0.0.3/PKG-INFO` & `mkdocs-flavorwheel-plugin-0.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-flavorwheel-plugin
-Version: 0.0.3
+Version: 0.0.4
 Summary: MkDocs plugin
 Home-page: 
 Author: Mico Papp
 Author-email: papp.mico@gmail.com
 License: MIT
 Keywords: mkdocs
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mkdocs-flavorwheel-plugin-0.0.3/README.md` & `mkdocs-flavorwheel-plugin-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-flavorwheel-plugin-0.0.3/mkdocs_flavorwheel_plugin.egg-info/PKG-INFO` & `mkdocs-flavorwheel-plugin-0.0.4/mkdocs_flavorwheel_plugin.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-flavorwheel-plugin
-Version: 0.0.3
+Version: 0.0.4
 Summary: MkDocs plugin
 Home-page: 
 Author: Mico Papp
 Author-email: papp.mico@gmail.com
 License: MIT
 Keywords: mkdocs
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mkdocs-flavorwheel-plugin-0.0.3/setup.py` & `mkdocs-flavorwheel-plugin-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='mkdocs-flavorwheel-plugin',
-    version='0.0.3',
+    version='0.0.4',
     description='MkDocs plugin',
     long_description='',
     keywords='mkdocs',
     url='',
     author='Mico Papp',
     author_email='papp.mico@gmail.com',
     license='MIT',
```

