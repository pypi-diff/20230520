# Comparing `tmp/dbtdocgen_rutryk-0.0.2.tar.gz` & `tmp/dbtdocgen_rutryk-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbtdocgen_rutryk-0.0.2.tar", last modified: Sat May 20 15:45:10 2023, max compression
+gzip compressed data, was "dbtdocgen_rutryk-0.0.3.tar", last modified: Sat May 20 15:52:41 2023, max compression
```

## Comparing `dbtdocgen_rutryk-0.0.2.tar` & `dbtdocgen_rutryk-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 patrykpacholek   (501) staff       (20)        0 2023-05-20 15:45:10.706681 dbtdocgen_rutryk-0.0.2/
--rw-r--r--   0 patrykpacholek   (501) staff       (20)      190 2023-05-20 15:45:10.706277 dbtdocgen_rutryk-0.0.2/PKG-INFO
--rw-r--r--   0 patrykpacholek   (501) staff       (20)      192 2023-05-20 15:41:31.000000 dbtdocgen_rutryk-0.0.2/README.md
-drwxr-xr-x   0 patrykpacholek   (501) staff       (20)        0 2023-05-20 15:45:10.705612 dbtdocgen_rutryk-0.0.2/dbtdocgen_rutryk.egg-info/
--rw-r--r--   0 patrykpacholek   (501) staff       (20)      190 2023-05-20 15:45:10.000000 dbtdocgen_rutryk-0.0.2/dbtdocgen_rutryk.egg-info/PKG-INFO
--rw-r--r--   0 patrykpacholek   (501) staff       (20)      266 2023-05-20 15:45:10.000000 dbtdocgen_rutryk-0.0.2/dbtdocgen_rutryk.egg-info/SOURCES.txt
--rw-r--r--   0 patrykpacholek   (501) staff       (20)        1 2023-05-20 15:45:10.000000 dbtdocgen_rutryk-0.0.2/dbtdocgen_rutryk.egg-info/dependency_links.txt
--rw-r--r--   0 patrykpacholek   (501) staff       (20)       90 2023-05-20 15:45:10.000000 dbtdocgen_rutryk-0.0.2/dbtdocgen_rutryk.egg-info/entry_points.txt
--rw-r--r--   0 patrykpacholek   (501) staff       (20)        6 2023-05-20 15:45:10.000000 dbtdocgen_rutryk-0.0.2/dbtdocgen_rutryk.egg-info/requires.txt
--rw-r--r--   0 patrykpacholek   (501) staff       (20)        1 2023-05-20 15:45:10.000000 dbtdocgen_rutryk-0.0.2/dbtdocgen_rutryk.egg-info/top_level.txt
--rw-r--r--   0 patrykpacholek   (501) staff       (20)      437 2023-05-20 15:42:21.000000 dbtdocgen_rutryk-0.0.2/pyproject.toml
--rw-r--r--   0 patrykpacholek   (501) staff       (20)       38 2023-05-20 15:45:10.706780 dbtdocgen_rutryk-0.0.2/setup.cfg
+drwxr-xr-x   0 patrykpacholek   (501) staff       (20)        0 2023-05-20 15:52:41.943833 dbtdocgen_rutryk-0.0.3/
+-rw-r--r--   0 patrykpacholek   (501) staff       (20)      190 2023-05-20 15:52:41.870751 dbtdocgen_rutryk-0.0.3/PKG-INFO
+-rw-r--r--   0 patrykpacholek   (501) staff       (20)      192 2023-05-20 15:41:31.000000 dbtdocgen_rutryk-0.0.3/README.md
+drwxr-xr-x   0 patrykpacholek   (501) staff       (20)        0 2023-05-20 15:52:41.868603 dbtdocgen_rutryk-0.0.3/dbtdocgen_rutryk.egg-info/
+-rw-r--r--   0 patrykpacholek   (501) staff       (20)      190 2023-05-20 15:52:41.000000 dbtdocgen_rutryk-0.0.3/dbtdocgen_rutryk.egg-info/PKG-INFO
+-rw-r--r--   0 patrykpacholek   (501) staff       (20)      266 2023-05-20 15:52:41.000000 dbtdocgen_rutryk-0.0.3/dbtdocgen_rutryk.egg-info/SOURCES.txt
+-rw-r--r--   0 patrykpacholek   (501) staff       (20)        1 2023-05-20 15:52:41.000000 dbtdocgen_rutryk-0.0.3/dbtdocgen_rutryk.egg-info/dependency_links.txt
+-rw-r--r--   0 patrykpacholek   (501) staff       (20)       90 2023-05-20 15:52:41.000000 dbtdocgen_rutryk-0.0.3/dbtdocgen_rutryk.egg-info/entry_points.txt
+-rw-r--r--   0 patrykpacholek   (501) staff       (20)        6 2023-05-20 15:52:41.000000 dbtdocgen_rutryk-0.0.3/dbtdocgen_rutryk.egg-info/requires.txt
+-rw-r--r--   0 patrykpacholek   (501) staff       (20)        1 2023-05-20 15:52:41.000000 dbtdocgen_rutryk-0.0.3/dbtdocgen_rutryk.egg-info/top_level.txt
+-rw-r--r--   0 patrykpacholek   (501) staff       (20)      437 2023-05-20 15:52:12.000000 dbtdocgen_rutryk-0.0.3/pyproject.toml
+-rw-r--r--   0 patrykpacholek   (501) staff       (20)       38 2023-05-20 15:52:41.944080 dbtdocgen_rutryk-0.0.3/setup.cfg
```

