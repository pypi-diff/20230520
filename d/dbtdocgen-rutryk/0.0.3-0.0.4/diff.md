# Comparing `tmp/dbtdocgen_rutryk-0.0.3.tar.gz` & `tmp/dbtdocgen_rutryk-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbtdocgen_rutryk-0.0.3.tar", last modified: Sat May 20 15:52:41 2023, max compression
+gzip compressed data, was "dbtdocgen_rutryk-0.0.4.tar", last modified: Sat May 20 15:57:04 2023, max compression
```

## Comparing `dbtdocgen_rutryk-0.0.3.tar` & `dbtdocgen_rutryk-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 patrykpacholek   (501) staff       (20)        0 2023-05-20 15:52:41.943833 dbtdocgen_rutryk-0.0.3/
--rw-r--r--   0 patrykpacholek   (501) staff       (20)      190 2023-05-20 15:52:41.870751 dbtdocgen_rutryk-0.0.3/PKG-INFO
--rw-r--r--   0 patrykpacholek   (501) staff       (20)      192 2023-05-20 15:41:31.000000 dbtdocgen_rutryk-0.0.3/README.md
-drwxr-xr-x   0 patrykpacholek   (501) staff       (20)        0 2023-05-20 15:52:41.868603 dbtdocgen_rutryk-0.0.3/dbtdocgen_rutryk.egg-info/
--rw-r--r--   0 patrykpacholek   (501) staff       (20)      190 2023-05-20 15:52:41.000000 dbtdocgen_rutryk-0.0.3/dbtdocgen_rutryk.egg-info/PKG-INFO
--rw-r--r--   0 patrykpacholek   (501) staff       (20)      266 2023-05-20 15:52:41.000000 dbtdocgen_rutryk-0.0.3/dbtdocgen_rutryk.egg-info/SOURCES.txt
--rw-r--r--   0 patrykpacholek   (501) staff       (20)        1 2023-05-20 15:52:41.000000 dbtdocgen_rutryk-0.0.3/dbtdocgen_rutryk.egg-info/dependency_links.txt
--rw-r--r--   0 patrykpacholek   (501) staff       (20)       90 2023-05-20 15:52:41.000000 dbtdocgen_rutryk-0.0.3/dbtdocgen_rutryk.egg-info/entry_points.txt
--rw-r--r--   0 patrykpacholek   (501) staff       (20)        6 2023-05-20 15:52:41.000000 dbtdocgen_rutryk-0.0.3/dbtdocgen_rutryk.egg-info/requires.txt
--rw-r--r--   0 patrykpacholek   (501) staff       (20)        1 2023-05-20 15:52:41.000000 dbtdocgen_rutryk-0.0.3/dbtdocgen_rutryk.egg-info/top_level.txt
--rw-r--r--   0 patrykpacholek   (501) staff       (20)      437 2023-05-20 15:52:12.000000 dbtdocgen_rutryk-0.0.3/pyproject.toml
--rw-r--r--   0 patrykpacholek   (501) staff       (20)       38 2023-05-20 15:52:41.944080 dbtdocgen_rutryk-0.0.3/setup.cfg
+drwxr-xr-x   0 patrykpacholek   (501) staff       (20)        0 2023-05-20 15:57:04.388218 dbtdocgen_rutryk-0.0.4/
+-rw-r--r--   0 patrykpacholek   (501) staff       (20)      190 2023-05-20 15:57:04.336482 dbtdocgen_rutryk-0.0.4/PKG-INFO
+-rw-r--r--   0 patrykpacholek   (501) staff       (20)      192 2023-05-20 15:41:31.000000 dbtdocgen_rutryk-0.0.4/README.md
+drwxr-xr-x   0 patrykpacholek   (501) staff       (20)        0 2023-05-20 15:57:04.335720 dbtdocgen_rutryk-0.0.4/dbtdocgen_rutryk.egg-info/
+-rw-r--r--   0 patrykpacholek   (501) staff       (20)      190 2023-05-20 15:57:04.000000 dbtdocgen_rutryk-0.0.4/dbtdocgen_rutryk.egg-info/PKG-INFO
+-rw-r--r--   0 patrykpacholek   (501) staff       (20)      275 2023-05-20 15:57:04.000000 dbtdocgen_rutryk-0.0.4/dbtdocgen_rutryk.egg-info/SOURCES.txt
+-rw-r--r--   0 patrykpacholek   (501) staff       (20)        1 2023-05-20 15:57:04.000000 dbtdocgen_rutryk-0.0.4/dbtdocgen_rutryk.egg-info/dependency_links.txt
+-rw-r--r--   0 patrykpacholek   (501) staff       (20)       90 2023-05-20 15:57:04.000000 dbtdocgen_rutryk-0.0.4/dbtdocgen_rutryk.egg-info/entry_points.txt
+-rw-r--r--   0 patrykpacholek   (501) staff       (20)        6 2023-05-20 15:57:04.000000 dbtdocgen_rutryk-0.0.4/dbtdocgen_rutryk.egg-info/requires.txt
+-rw-r--r--   0 patrykpacholek   (501) staff       (20)        1 2023-05-20 15:57:04.000000 dbtdocgen_rutryk-0.0.4/dbtdocgen_rutryk.egg-info/top_level.txt
+-rw-r--r--   0 patrykpacholek   (501) staff       (20)      437 2023-05-20 15:56:37.000000 dbtdocgen_rutryk-0.0.4/pyproject.toml
+-rw-r--r--   0 patrykpacholek   (501) staff       (20)       38 2023-05-20 15:57:04.388393 dbtdocgen_rutryk-0.0.4/setup.cfg
+-rw-r--r--   0 patrykpacholek   (501) staff       (20)      294 2023-05-20 15:56:37.000000 dbtdocgen_rutryk-0.0.4/setup.py
```

