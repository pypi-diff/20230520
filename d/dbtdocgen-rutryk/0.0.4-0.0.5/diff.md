# Comparing `tmp/dbtdocgen_rutryk-0.0.4.tar.gz` & `tmp/dbtdocgen_rutryk-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbtdocgen_rutryk-0.0.4.tar", last modified: Sat May 20 15:57:04 2023, max compression
+gzip compressed data, was "dbtdocgen_rutryk-0.0.5.tar", last modified: Sat May 20 16:01:10 2023, max compression
```

## Comparing `dbtdocgen_rutryk-0.0.4.tar` & `dbtdocgen_rutryk-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxr-xr-x   0 patrykpacholek   (501) staff       (20)        0 2023-05-20 15:57:04.388218 dbtdocgen_rutryk-0.0.4/
--rw-r--r--   0 patrykpacholek   (501) staff       (20)      190 2023-05-20 15:57:04.336482 dbtdocgen_rutryk-0.0.4/PKG-INFO
--rw-r--r--   0 patrykpacholek   (501) staff       (20)      192 2023-05-20 15:41:31.000000 dbtdocgen_rutryk-0.0.4/README.md
-drwxr-xr-x   0 patrykpacholek   (501) staff       (20)        0 2023-05-20 15:57:04.335720 dbtdocgen_rutryk-0.0.4/dbtdocgen_rutryk.egg-info/
--rw-r--r--   0 patrykpacholek   (501) staff       (20)      190 2023-05-20 15:57:04.000000 dbtdocgen_rutryk-0.0.4/dbtdocgen_rutryk.egg-info/PKG-INFO
--rw-r--r--   0 patrykpacholek   (501) staff       (20)      275 2023-05-20 15:57:04.000000 dbtdocgen_rutryk-0.0.4/dbtdocgen_rutryk.egg-info/SOURCES.txt
--rw-r--r--   0 patrykpacholek   (501) staff       (20)        1 2023-05-20 15:57:04.000000 dbtdocgen_rutryk-0.0.4/dbtdocgen_rutryk.egg-info/dependency_links.txt
--rw-r--r--   0 patrykpacholek   (501) staff       (20)       90 2023-05-20 15:57:04.000000 dbtdocgen_rutryk-0.0.4/dbtdocgen_rutryk.egg-info/entry_points.txt
--rw-r--r--   0 patrykpacholek   (501) staff       (20)        6 2023-05-20 15:57:04.000000 dbtdocgen_rutryk-0.0.4/dbtdocgen_rutryk.egg-info/requires.txt
--rw-r--r--   0 patrykpacholek   (501) staff       (20)        1 2023-05-20 15:57:04.000000 dbtdocgen_rutryk-0.0.4/dbtdocgen_rutryk.egg-info/top_level.txt
--rw-r--r--   0 patrykpacholek   (501) staff       (20)      437 2023-05-20 15:56:37.000000 dbtdocgen_rutryk-0.0.4/pyproject.toml
--rw-r--r--   0 patrykpacholek   (501) staff       (20)       38 2023-05-20 15:57:04.388393 dbtdocgen_rutryk-0.0.4/setup.cfg
--rw-r--r--   0 patrykpacholek   (501) staff       (20)      294 2023-05-20 15:56:37.000000 dbtdocgen_rutryk-0.0.4/setup.py
+drwxr-xr-x   0 patrykpacholek   (501) staff       (20)        0 2023-05-20 16:01:10.763580 dbtdocgen_rutryk-0.0.5/
+-rw-r--r--   0 patrykpacholek   (501) staff       (20)      190 2023-05-20 16:01:10.761002 dbtdocgen_rutryk-0.0.5/PKG-INFO
+-rw-r--r--   0 patrykpacholek   (501) staff       (20)      192 2023-05-20 15:41:31.000000 dbtdocgen_rutryk-0.0.5/README.md
+drwxr-xr-x   0 patrykpacholek   (501) staff       (20)        0 2023-05-20 16:01:10.748628 dbtdocgen_rutryk-0.0.5/dbtdocgen_rutryk/
+-rw-r--r--   0 patrykpacholek   (501) staff       (20)        0 2023-05-20 14:43:00.000000 dbtdocgen_rutryk-0.0.5/dbtdocgen_rutryk/__init__.py
+-rw-r--r--   0 patrykpacholek   (501) staff       (20)     1663 2023-05-20 15:43:18.000000 dbtdocgen_rutryk-0.0.5/dbtdocgen_rutryk/dbtdocgen.py
+drwxr-xr-x   0 patrykpacholek   (501) staff       (20)        0 2023-05-20 16:01:10.760202 dbtdocgen_rutryk-0.0.5/dbtdocgen_rutryk.egg-info/
+-rw-r--r--   0 patrykpacholek   (501) staff       (20)      190 2023-05-20 16:01:10.000000 dbtdocgen_rutryk-0.0.5/dbtdocgen_rutryk.egg-info/PKG-INFO
+-rw-r--r--   0 patrykpacholek   (501) staff       (20)      334 2023-05-20 16:01:10.000000 dbtdocgen_rutryk-0.0.5/dbtdocgen_rutryk.egg-info/SOURCES.txt
+-rw-r--r--   0 patrykpacholek   (501) staff       (20)        1 2023-05-20 16:01:10.000000 dbtdocgen_rutryk-0.0.5/dbtdocgen_rutryk.egg-info/dependency_links.txt
+-rw-r--r--   0 patrykpacholek   (501) staff       (20)       90 2023-05-20 16:01:10.000000 dbtdocgen_rutryk-0.0.5/dbtdocgen_rutryk.egg-info/entry_points.txt
+-rw-r--r--   0 patrykpacholek   (501) staff       (20)        6 2023-05-20 16:01:10.000000 dbtdocgen_rutryk-0.0.5/dbtdocgen_rutryk.egg-info/requires.txt
+-rw-r--r--   0 patrykpacholek   (501) staff       (20)       17 2023-05-20 16:01:10.000000 dbtdocgen_rutryk-0.0.5/dbtdocgen_rutryk.egg-info/top_level.txt
+-rw-r--r--   0 patrykpacholek   (501) staff       (20)      437 2023-05-20 16:00:17.000000 dbtdocgen_rutryk-0.0.5/pyproject.toml
+-rw-r--r--   0 patrykpacholek   (501) staff       (20)       38 2023-05-20 16:01:10.763724 dbtdocgen_rutryk-0.0.5/setup.cfg
+-rw-r--r--   0 patrykpacholek   (501) staff       (20)      294 2023-05-20 16:00:39.000000 dbtdocgen_rutryk-0.0.5/setup.py
```

