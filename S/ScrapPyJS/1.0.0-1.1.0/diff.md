# Comparing `tmp/ScrapPyJS-1.0.0.tar.gz` & `tmp/ScrapPyJS-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ScrapPyJS-1.0.0.tar", last modified: Sat May 20 07:28:12 2023, max compression
+gzip compressed data, was "ScrapPyJS-1.1.0.tar", last modified: Sat May 20 19:53:40 2023, max compression
```

## Comparing `ScrapPyJS-1.0.0.tar` & `ScrapPyJS-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 07:28:12.325847 ScrapPyJS-1.0.0/
--rw-rw-rw-   0        0        0     1095 2023-05-20 07:18:49.000000 ScrapPyJS-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     3616 2023-05-20 07:28:12.325847 ScrapPyJS-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2953 2023-05-20 07:24:13.000000 ScrapPyJS-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-20 07:28:12.311159 ScrapPyJS-1.0.0/ScrapPyJS/
--rw-rw-rw-   0        0        0       39 2023-05-20 07:23:22.000000 ScrapPyJS-1.0.0/ScrapPyJS/__init__.py
--rw-rw-rw-   0        0        0     4004 2023-05-20 07:23:00.000000 ScrapPyJS-1.0.0/ScrapPyJS/scrappy.py
-drwxrwxrwx   0        0        0        0 2023-05-20 07:28:12.325847 ScrapPyJS-1.0.0/ScrapPyJS.egg-info/
--rw-rw-rw-   0        0        0     3616 2023-05-20 07:28:12.000000 ScrapPyJS-1.0.0/ScrapPyJS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-05-20 07:28:12.000000 ScrapPyJS-1.0.0/ScrapPyJS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 07:28:12.000000 ScrapPyJS-1.0.0/ScrapPyJS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-20 07:28:12.000000 ScrapPyJS-1.0.0/ScrapPyJS.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-20 07:28:12.000000 ScrapPyJS-1.0.0/ScrapPyJS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-20 07:28:12.325847 ScrapPyJS-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1141 2023-05-20 07:21:38.000000 ScrapPyJS-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 19:53:40.142109 ScrapPyJS-1.1.0/
+-rw-rw-rw-   0        0        0     1095 2023-05-20 07:18:49.000000 ScrapPyJS-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     4293 2023-05-20 19:53:40.139718 ScrapPyJS-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3559 2023-05-20 19:25:37.000000 ScrapPyJS-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-20 19:53:40.126247 ScrapPyJS-1.1.0/ScrapPyJS/
+-rw-rw-rw-   0        0        0       39 2023-05-20 07:23:22.000000 ScrapPyJS-1.1.0/ScrapPyJS/__init__.py
+-rw-rw-rw-   0        0        0     6719 2023-05-20 19:50:34.000000 ScrapPyJS-1.1.0/ScrapPyJS/scrappy.py
+drwxrwxrwx   0        0        0        0 2023-05-20 19:53:40.134693 ScrapPyJS-1.1.0/ScrapPyJS.egg-info/
+-rw-rw-rw-   0        0        0     4293 2023-05-20 19:53:39.000000 ScrapPyJS-1.1.0/ScrapPyJS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-05-20 19:53:39.000000 ScrapPyJS-1.1.0/ScrapPyJS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 19:53:39.000000 ScrapPyJS-1.1.0/ScrapPyJS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-20 19:53:39.000000 ScrapPyJS-1.1.0/ScrapPyJS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-20 19:53:39.000000 ScrapPyJS-1.1.0/ScrapPyJS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-20 19:53:40.143125 ScrapPyJS-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1234 2023-05-20 19:43:43.000000 ScrapPyJS-1.1.0/setup.py
```

### Comparing `ScrapPyJS-1.0.0/LICENSE` & `ScrapPyJS-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ScrapPyJS-1.0.0/setup.py` & `ScrapPyJS-1.1.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,30 +3,33 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = 'An easy to use web scrapping library via JS scripts'
 LONG_DESCRIPTION = 'A package that allows to scrapp data from Web pages by running JS scripts from python.'
 
 # Setting up
 setup(
     name="ScrapPyJS",
     version=VERSION,
     author="Hind Sagar Biswas",
     author_email="<hindsbhk@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
-    install_requires=['selenium'],
-    keywords=['python', 'web scrapping', 'scrap'],
+    install_requires=['selenium', 'tqdm'],
+    extras_require={
+        "dev": ["pytest>=7.0", "twine>=4.0.2"],
+    },
+    keywords=['python', 'web scrapping', 'scrape data'],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
```

