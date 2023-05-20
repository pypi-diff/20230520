# Comparing `tmp/dbtdocgen_rutryk-0.0.1.tar.gz` & `tmp/dbtdocgen_rutryk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbtdocgen_rutryk-0.0.1.tar", last modified: Sat May 20 15:02:02 2023, max compression
+gzip compressed data, was "dbtdocgen_rutryk-0.0.2.tar", last modified: Sat May 20 15:45:10 2023, max compression
```

## Comparing `dbtdocgen_rutryk-0.0.1.tar` & `dbtdocgen_rutryk-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 patrykpacholek   (501) staff       (20)        0 2023-05-20 15:02:02.857066 dbtdocgen_rutryk-0.0.1/
--rw-r--r--   0 patrykpacholek   (501) staff       (20)      190 2023-05-20 15:02:02.854607 dbtdocgen_rutryk-0.0.1/PKG-INFO
--rw-r--r--   0 patrykpacholek   (501) staff       (20)       11 2023-05-20 14:45:53.000000 dbtdocgen_rutryk-0.0.1/README.md
-drwxr-xr-x   0 patrykpacholek   (501) staff       (20)        0 2023-05-20 15:02:02.853084 dbtdocgen_rutryk-0.0.1/dbtdocgen_rutryk.egg-info/
--rw-r--r--   0 patrykpacholek   (501) staff       (20)      190 2023-05-20 15:02:02.000000 dbtdocgen_rutryk-0.0.1/dbtdocgen_rutryk.egg-info/PKG-INFO
--rw-r--r--   0 patrykpacholek   (501) staff       (20)      266 2023-05-20 15:02:02.000000 dbtdocgen_rutryk-0.0.1/dbtdocgen_rutryk.egg-info/SOURCES.txt
--rw-r--r--   0 patrykpacholek   (501) staff       (20)        1 2023-05-20 15:02:02.000000 dbtdocgen_rutryk-0.0.1/dbtdocgen_rutryk.egg-info/dependency_links.txt
--rw-r--r--   0 patrykpacholek   (501) staff       (20)       90 2023-05-20 15:02:02.000000 dbtdocgen_rutryk-0.0.1/dbtdocgen_rutryk.egg-info/entry_points.txt
--rw-r--r--   0 patrykpacholek   (501) staff       (20)        6 2023-05-20 15:02:02.000000 dbtdocgen_rutryk-0.0.1/dbtdocgen_rutryk.egg-info/requires.txt
--rw-r--r--   0 patrykpacholek   (501) staff       (20)        1 2023-05-20 15:02:02.000000 dbtdocgen_rutryk-0.0.1/dbtdocgen_rutryk.egg-info/top_level.txt
--rw-r--r--   0 patrykpacholek   (501) staff       (20)      437 2023-05-20 14:49:14.000000 dbtdocgen_rutryk-0.0.1/pyproject.toml
--rw-r--r--   0 patrykpacholek   (501) staff       (20)       38 2023-05-20 15:02:02.857214 dbtdocgen_rutryk-0.0.1/setup.cfg
+drwxr-xr-x   0 patrykpacholek   (501) staff       (20)        0 2023-05-20 15:45:10.706681 dbtdocgen_rutryk-0.0.2/
+-rw-r--r--   0 patrykpacholek   (501) staff       (20)      190 2023-05-20 15:45:10.706277 dbtdocgen_rutryk-0.0.2/PKG-INFO
+-rw-r--r--   0 patrykpacholek   (501) staff       (20)      192 2023-05-20 15:41:31.000000 dbtdocgen_rutryk-0.0.2/README.md
+drwxr-xr-x   0 patrykpacholek   (501) staff       (20)        0 2023-05-20 15:45:10.705612 dbtdocgen_rutryk-0.0.2/dbtdocgen_rutryk.egg-info/
+-rw-r--r--   0 patrykpacholek   (501) staff       (20)      190 2023-05-20 15:45:10.000000 dbtdocgen_rutryk-0.0.2/dbtdocgen_rutryk.egg-info/PKG-INFO
+-rw-r--r--   0 patrykpacholek   (501) staff       (20)      266 2023-05-20 15:45:10.000000 dbtdocgen_rutryk-0.0.2/dbtdocgen_rutryk.egg-info/SOURCES.txt
+-rw-r--r--   0 patrykpacholek   (501) staff       (20)        1 2023-05-20 15:45:10.000000 dbtdocgen_rutryk-0.0.2/dbtdocgen_rutryk.egg-info/dependency_links.txt
+-rw-r--r--   0 patrykpacholek   (501) staff       (20)       90 2023-05-20 15:45:10.000000 dbtdocgen_rutryk-0.0.2/dbtdocgen_rutryk.egg-info/entry_points.txt
+-rw-r--r--   0 patrykpacholek   (501) staff       (20)        6 2023-05-20 15:45:10.000000 dbtdocgen_rutryk-0.0.2/dbtdocgen_rutryk.egg-info/requires.txt
+-rw-r--r--   0 patrykpacholek   (501) staff       (20)        1 2023-05-20 15:45:10.000000 dbtdocgen_rutryk-0.0.2/dbtdocgen_rutryk.egg-info/top_level.txt
+-rw-r--r--   0 patrykpacholek   (501) staff       (20)      437 2023-05-20 15:42:21.000000 dbtdocgen_rutryk-0.0.2/pyproject.toml
+-rw-r--r--   0 patrykpacholek   (501) staff       (20)       38 2023-05-20 15:45:10.706780 dbtdocgen_rutryk-0.0.2/setup.cfg
```

