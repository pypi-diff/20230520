# Comparing `tmp/pylint-beautifulsoup-17.10.12.tar.gz` & `tmp/pylint-beautifulsoup-3.12.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylint-beautifulsoup-17.10.12.tar", last modified: Sat May 20 14:05:49 2023, max compression
+gzip compressed data, was "pylint-beautifulsoup-3.12.3.tar", last modified: Sat May 20 14:02:00 2023, max compression
```

## Comparing `pylint-beautifulsoup-17.10.12.tar` & `pylint-beautifulsoup-3.12.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 14:05:49.670029 pylint-beautifulsoup-17.10.12/
--rw-rw-rw-   0        0        0      405 2023-05-20 14:05:49.669013 pylint-beautifulsoup-17.10.12/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-20 14:05:49.667032 pylint-beautifulsoup-17.10.12/pylint_beautifulsoup.egg-info/
--rw-rw-rw-   0        0        0      405 2023-05-20 14:05:49.000000 pylint-beautifulsoup-17.10.12/pylint_beautifulsoup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2023-05-20 14:05:49.000000 pylint-beautifulsoup-17.10.12/pylint_beautifulsoup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 14:05:49.000000 pylint-beautifulsoup-17.10.12/pylint_beautifulsoup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-20 14:05:49.000000 pylint-beautifulsoup-17.10.12/pylint_beautifulsoup.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-20 14:05:49.668031 pylint-beautifulsoup-17.10.12/reqinstaller/
--rw-rw-rw-   0        0        0      345 2023-05-20 13:00:35.000000 pylint-beautifulsoup-17.10.12/reqinstaller/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-20 14:05:49.670029 pylint-beautifulsoup-17.10.12/setup.cfg
--rw-rw-rw-   0        0        0     1235 2023-05-20 14:05:47.000000 pylint-beautifulsoup-17.10.12/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 14:02:00.484934 pylint-beautifulsoup-3.12.3/
+-rw-rw-rw-   0        0        0      422 2023-05-20 14:02:00.484934 pylint-beautifulsoup-3.12.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-20 14:02:00.481933 pylint-beautifulsoup-3.12.3/pylint_beautifulsoup.egg-info/
+-rw-rw-rw-   0        0        0      422 2023-05-20 14:02:00.000000 pylint-beautifulsoup-3.12.3/pylint_beautifulsoup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2023-05-20 14:02:00.000000 pylint-beautifulsoup-3.12.3/pylint_beautifulsoup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 14:02:00.000000 pylint-beautifulsoup-3.12.3/pylint_beautifulsoup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-20 14:02:00.000000 pylint-beautifulsoup-3.12.3/pylint_beautifulsoup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-20 14:02:00.482934 pylint-beautifulsoup-3.12.3/reqinstaller/
+-rw-rw-rw-   0        0        0      345 2023-05-20 13:00:35.000000 pylint-beautifulsoup-3.12.3/reqinstaller/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-20 14:02:00.484934 pylint-beautifulsoup-3.12.3/setup.cfg
+-rw-rw-rw-   0        0        0     1252 2023-05-20 14:01:58.000000 pylint-beautifulsoup-3.12.3/setup.py
```

### Comparing `pylint-beautifulsoup-17.10.12/setup.py` & `pylint-beautifulsoup-3.12.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 
-VERSION = '17.10.12'
-DESCRIPTION = 'A library for data visualization'
+VERSION = '3.12.3'
+DESCRIPTION = 'A Python wrapper for OpenCV computer vision library'
 LONG_DESCRIPTION = 'Really helpful'
 setup(
     name="pylint-beautifulsoup",
     version=VERSION,
     author="DreamyOakXTimmywag",
     author_email="DreamyOakXTimmywag@dreamyoak.onrender.com",
     description=DESCRIPTION,
```

