# Comparing `tmp/dbtdocgen_rutryk-0.0.7.tar.gz` & `tmp/dbtdocgen_rutryk-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbtdocgen_rutryk-0.0.7.tar", last modified: Sat May 20 16:38:40 2023, max compression
+gzip compressed data, was "dbtdocgen_rutryk-0.0.8.tar", last modified: Sat May 20 16:44:38 2023, max compression
```

## Comparing `dbtdocgen_rutryk-0.0.7.tar` & `dbtdocgen_rutryk-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 16:38:40.805122 dbtdocgen_rutryk-0.0.7/
--rw-rw-rw-   0        0        0     1091 2023-05-20 16:16:45.000000 dbtdocgen_rutryk-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      579 2023-05-20 16:38:40.804122 dbtdocgen_rutryk-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      194 2023-05-20 16:24:13.000000 dbtdocgen_rutryk-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-20 16:38:40.791255 dbtdocgen_rutryk-0.0.7/dbtdocgen_rutryk/
--rw-rw-rw-   0        0        0        0 2023-05-20 16:16:45.000000 dbtdocgen_rutryk-0.0.7/dbtdocgen_rutryk/__init__.py
--rw-rw-rw-   0        0        0     1744 2023-05-20 16:36:29.000000 dbtdocgen_rutryk-0.0.7/dbtdocgen_rutryk/dbtdocgen.py
-drwxrwxrwx   0        0        0        0 2023-05-20 16:38:40.801789 dbtdocgen_rutryk-0.0.7/dbtdocgen_rutryk.egg-info/
--rw-rw-rw-   0        0        0      579 2023-05-20 16:38:40.000000 dbtdocgen_rutryk-0.0.7/dbtdocgen_rutryk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2023-05-20 16:38:40.000000 dbtdocgen_rutryk-0.0.7/dbtdocgen_rutryk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 16:38:40.000000 dbtdocgen_rutryk-0.0.7/dbtdocgen_rutryk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-05-20 16:38:40.000000 dbtdocgen_rutryk-0.0.7/dbtdocgen_rutryk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-05-20 16:38:40.000000 dbtdocgen_rutryk-0.0.7/dbtdocgen_rutryk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-20 16:38:40.000000 dbtdocgen_rutryk-0.0.7/dbtdocgen_rutryk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      448 2023-05-20 16:36:52.000000 dbtdocgen_rutryk-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-20 16:38:40.806123 dbtdocgen_rutryk-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      306 2023-05-20 16:36:56.000000 dbtdocgen_rutryk-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 16:44:38.800483 dbtdocgen_rutryk-0.0.8/
+-rw-rw-rw-   0        0        0     1091 2023-05-20 16:16:45.000000 dbtdocgen_rutryk-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      398 2023-05-20 16:44:38.799475 dbtdocgen_rutryk-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       15 2023-05-20 16:43:24.000000 dbtdocgen_rutryk-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-20 16:44:38.785814 dbtdocgen_rutryk-0.0.8/dbtdocgen_rutryk/
+-rw-rw-rw-   0        0        0        0 2023-05-20 16:16:45.000000 dbtdocgen_rutryk-0.0.8/dbtdocgen_rutryk/__init__.py
+-rw-rw-rw-   0        0        0     1744 2023-05-20 16:36:29.000000 dbtdocgen_rutryk-0.0.8/dbtdocgen_rutryk/dbtdocgen.py
+drwxrwxrwx   0        0        0        0 2023-05-20 16:44:38.797967 dbtdocgen_rutryk-0.0.8/dbtdocgen_rutryk.egg-info/
+-rw-rw-rw-   0        0        0      398 2023-05-20 16:44:38.000000 dbtdocgen_rutryk-0.0.8/dbtdocgen_rutryk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2023-05-20 16:44:38.000000 dbtdocgen_rutryk-0.0.8/dbtdocgen_rutryk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 16:44:38.000000 dbtdocgen_rutryk-0.0.8/dbtdocgen_rutryk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-05-20 16:44:38.000000 dbtdocgen_rutryk-0.0.8/dbtdocgen_rutryk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-05-20 16:44:38.000000 dbtdocgen_rutryk-0.0.8/dbtdocgen_rutryk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-20 16:44:38.000000 dbtdocgen_rutryk-0.0.8/dbtdocgen_rutryk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      448 2023-05-20 16:44:33.000000 dbtdocgen_rutryk-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-20 16:44:38.800483 dbtdocgen_rutryk-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      306 2023-05-20 16:44:29.000000 dbtdocgen_rutryk-0.0.8/setup.py
```

### Comparing `dbtdocgen_rutryk-0.0.7/LICENSE` & `dbtdocgen_rutryk-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dbtdocgen_rutryk-0.0.7/dbtdocgen_rutryk/dbtdocgen.py` & `dbtdocgen_rutryk-0.0.8/dbtdocgen_rutryk/dbtdocgen.py`

 * *Files identical despite different names*

