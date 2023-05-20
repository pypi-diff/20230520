# Comparing `tmp/statml-0.0.1.tar.gz` & `tmp/statml-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statml-0.0.1.tar", last modified: Sat May 20 12:44:41 2023, max compression
+gzip compressed data, was "statml-0.0.3.tar", last modified: Sat May 20 14:12:24 2023, max compression
```

## Comparing `statml-0.0.1.tar` & `statml-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 12:44:41.145370 statml-0.0.1/
--rw-rw-rw-   0        0        0      381 2023-05-20 12:44:41.145370 statml-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       16 2023-05-20 12:40:16.000000 statml-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-20 12:44:41.145370 statml-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      608 2023-05-20 12:44:16.000000 statml-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-20 12:44:41.145370 statml-0.0.1/statml.egg-info/
--rw-rw-rw-   0        0        0      381 2023-05-20 12:44:40.000000 statml-0.0.1/statml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      138 2023-05-20 12:44:41.000000 statml-0.0.1/statml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 12:44:40.000000 statml-0.0.1/statml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 12:44:40.000000 statml-0.0.1/statml.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-20 14:12:24.807168 statml-0.0.3/
+-rw-rw-rw-   0        0        0      381 2023-05-20 14:12:24.807168 statml-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       16 2023-05-20 12:40:16.000000 statml-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-20 14:12:24.807168 statml-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      608 2023-05-20 14:12:10.000000 statml-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 14:12:24.791544 statml-0.0.3/statml/
+-rw-rw-rw-   0        0        0       21 2023-05-20 14:11:59.000000 statml-0.0.3/statml/__init__.py
+-rw-rw-rw-   0        0        0     3538 2023-05-20 14:05:21.000000 statml-0.0.3/statml/playchat.py
+drwxrwxrwx   0        0        0        0 2023-05-20 14:12:24.807168 statml-0.0.3/statml.egg-info/
+-rw-rw-rw-   0        0        0      381 2023-05-20 14:12:24.000000 statml-0.0.3/statml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      176 2023-05-20 14:12:24.000000 statml-0.0.3/statml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 14:12:24.000000 statml-0.0.3/statml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-20 14:12:24.000000 statml-0.0.3/statml.egg-info/top_level.txt
```

### Comparing `statml-0.0.1/setup.py` & `statml-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="statml",
-    version="0.0.1",
+    version="0.0.3",
     author="HaeWoon",
     author_email="likesea7@gmail.com",
     description="stat and ml example",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

