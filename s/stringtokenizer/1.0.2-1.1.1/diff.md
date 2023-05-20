# Comparing `tmp/stringtokenizer-1.0.2.tar.gz` & `tmp/stringtokenizer-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stringtokenizer-1.0.2.tar", last modified: Thu May 18 09:52:26 2023, max compression
+gzip compressed data, was "stringtokenizer-1.1.1.tar", last modified: Sat May 20 18:10:40 2023, max compression
```

## Comparing `stringtokenizer-1.0.2.tar` & `stringtokenizer-1.1.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0 tanmay    (1000) tanmay    (1000)        0 2023-05-18 09:52:26.884753 stringtokenizer-1.0.2/
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)      222 2023-05-18 09:52:26.884400 stringtokenizer-1.0.2/PKG-INFO
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)       38 2023-05-18 09:52:26.884887 stringtokenizer-1.0.2/setup.cfg
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)      233 2023-05-18 09:51:41.000000 stringtokenizer-1.0.2/setup.py
-drwxrwxrwx   0 tanmay    (1000) tanmay    (1000)        0 2023-05-18 09:52:26.879521 stringtokenizer-1.0.2/stringtokenizer/
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)       46 2023-05-17 18:44:19.000000 stringtokenizer-1.0.2/stringtokenizer/__init__.py
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)     1611 2023-05-18 09:51:18.000000 stringtokenizer-1.0.2/stringtokenizer/stringtokenizer.py
-drwxrwxrwx   0 tanmay    (1000) tanmay    (1000)        0 2023-05-18 09:52:26.883365 stringtokenizer-1.0.2/stringtokenizer.egg-info/
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)      222 2023-05-18 09:52:26.000000 stringtokenizer-1.0.2/stringtokenizer.egg-info/PKG-INFO
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)      227 2023-05-18 09:52:26.000000 stringtokenizer-1.0.2/stringtokenizer.egg-info/SOURCES.txt
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)        1 2023-05-18 09:52:26.000000 stringtokenizer-1.0.2/stringtokenizer.egg-info/dependency_links.txt
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)       16 2023-05-18 09:52:26.000000 stringtokenizer-1.0.2/stringtokenizer.egg-info/top_level.txt
+drwxrwxrwx   0 tanmay    (1000) tanmay    (1000)        0 2023-05-20 18:10:40.592958 stringtokenizer-1.1.1/
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)     1444 2023-05-20 18:10:40.592626 stringtokenizer-1.1.1/PKG-INFO
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)      933 2023-05-20 18:09:24.000000 stringtokenizer-1.1.1/README.md
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)       38 2023-05-20 18:10:40.593043 stringtokenizer-1.1.1/setup.cfg
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)      448 2023-05-20 18:10:31.000000 stringtokenizer-1.1.1/setup.py
+drwxrwxrwx   0 tanmay    (1000) tanmay    (1000)        0 2023-05-20 18:10:40.590321 stringtokenizer-1.1.1/stringtokenizer/
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)       46 2023-05-17 18:44:19.000000 stringtokenizer-1.1.1/stringtokenizer/__init__.py
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)     1611 2023-05-18 09:51:18.000000 stringtokenizer-1.1.1/stringtokenizer/stringtokenizer.py
+drwxrwxrwx   0 tanmay    (1000) tanmay    (1000)        0 2023-05-20 18:10:40.592134 stringtokenizer-1.1.1/stringtokenizer.egg-info/
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)     1444 2023-05-20 18:10:40.000000 stringtokenizer-1.1.1/stringtokenizer.egg-info/PKG-INFO
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)      237 2023-05-20 18:10:40.000000 stringtokenizer-1.1.1/stringtokenizer.egg-info/SOURCES.txt
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)        1 2023-05-20 18:10:40.000000 stringtokenizer-1.1.1/stringtokenizer.egg-info/dependency_links.txt
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)       16 2023-05-20 18:10:40.000000 stringtokenizer-1.1.1/stringtokenizer.egg-info/top_level.txt
```

### Comparing `stringtokenizer-1.0.2/stringtokenizer/stringtokenizer.py` & `stringtokenizer-1.1.1/stringtokenizer/stringtokenizer.py`

 * *Files identical despite different names*

