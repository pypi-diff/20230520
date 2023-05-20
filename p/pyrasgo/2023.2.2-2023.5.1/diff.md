# Comparing `tmp/pyrasgo-2023.2.2.tar.gz` & `tmp/pyrasgo-2023.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyrasgo-2023.2.2.tar", last modified: Mon Feb 27 20:32:44 2023, max compression
+gzip compressed data, was "pyrasgo-2023.5.1.tar", last modified: Sat May 20 12:52:04 2023, max compression
```

## Comparing `pyrasgo-2023.2.2.tar` & `pyrasgo-2023.5.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:32:44.000000 pyrasgo-2023.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    34283 2023-02-27 20:32:17.000000 pyrasgo-2023.2.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-02-27 20:32:44.000000 pyrasgo-2023.2.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:32:44.000000 pyrasgo-2023.2.2/pyrasgo/
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-02-27 20:32:17.000000 pyrasgo-2023.2.2/pyrasgo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:32:44.000000 pyrasgo-2023.2.2/pyrasgo/api/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-02-27 20:32:17.000000 pyrasgo-2023.2.2/pyrasgo/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7623 2023-02-27 20:32:17.000000 pyrasgo-2023.2.2/pyrasgo/api/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9157 2023-02-27 20:32:17.000000 pyrasgo-2023.2.2/pyrasgo/api/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-02-27 20:32:17.000000 pyrasgo-2023.2.2/pyrasgo/api/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     7730 2023-02-27 20:32:17.000000 pyrasgo-2023.2.2/pyrasgo/api/get.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-02-27 20:32:17.000000 pyrasgo-2023.2.2/pyrasgo/api/login.py
--rw-r--r--   0 runner    (1001) docker     (123)    24822 2023-02-27 20:32:17.000000 pyrasgo-2023.2.2/pyrasgo/api/publish.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-02-27 20:32:17.000000 pyrasgo-2023.2.2/pyrasgo/api/read.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-02-27 20:32:17.000000 pyrasgo-2023.2.2/pyrasgo/api/session.py
--rw-r--r--   0 runner    (1001) docker     (123)    12802 2023-02-27 20:32:17.000000 pyrasgo-2023.2.2/pyrasgo/api/update.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-02-27 20:32:17.000000 pyrasgo-2023.2.2/pyrasgo/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-02-27 20:32:17.000000 pyrasgo-2023.2.2/pyrasgo/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-02-27 20:32:17.000000 pyrasgo-2023.2.2/pyrasgo/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-02-27 20:32:17.000000 pyrasgo-2023.2.2/pyrasgo/imports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:32:44.000000 pyrasgo-2023.2.2/pyrasgo/primitives/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-02-27 20:32:17.000000 pyrasgo-2023.2.2/pyrasgo/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35379 2023-02-27 20:32:17.000000 pyrasgo-2023.2.2/pyrasgo/primitives/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-02-27 20:32:17.000000 pyrasgo-2023.2.2/pyrasgo/primitives/dbt.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-02-27 20:32:17.000000 pyrasgo-2023.2.2/pyrasgo/rasgo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:32:44.000000 pyrasgo-2023.2.2/pyrasgo/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-02-27 20:32:17.000000 pyrasgo-2023.2.2/pyrasgo/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-02-27 20:32:17.000000 pyrasgo-2023.2.2/pyrasgo/schemas/attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-02-27 20:32:17.000000 pyrasgo-2023.2.2/pyrasgo/schemas/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-02-27 20:32:17.000000 pyrasgo-2023.2.2/pyrasgo/schemas/dataset_column.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-02-27 20:32:17.000000 pyrasgo-2023.2.2/pyrasgo/schemas/dw.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-02-27 20:32:17.000000 pyrasgo-2023.2.2/pyrasgo/schemas/dw_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-02-27 20:32:17.000000 pyrasgo-2023.2.2/pyrasgo/schemas/dw_operation_set.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-02-27 20:32:17.000000 pyrasgo-2023.2.2/pyrasgo/schemas/dw_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-02-27 20:32:17.000000 pyrasgo-2023.2.2/pyrasgo/schemas/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-02-27 20:32:17.000000 pyrasgo-2023.2.2/pyrasgo/schemas/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-02-27 20:32:17.000000 pyrasgo-2023.2.2/pyrasgo/schemas/offline.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-02-27 20:32:17.000000 pyrasgo-2023.2.2/pyrasgo/schemas/organization.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-02-27 20:32:17.000000 pyrasgo-2023.2.2/pyrasgo/schemas/status_tracking.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-02-27 20:32:17.000000 pyrasgo-2023.2.2/pyrasgo/schemas/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-02-27 20:32:17.000000 pyrasgo-2023.2.2/pyrasgo/schemas/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:32:44.000000 pyrasgo-2023.2.2/pyrasgo/storage/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-02-27 20:32:17.000000 pyrasgo-2023.2.2/pyrasgo/storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:32:44.000000 pyrasgo-2023.2.2/pyrasgo/storage/dataframe/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 20:32:17.000000 pyrasgo-2023.2.2/pyrasgo/storage/dataframe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-02-27 20:32:17.000000 pyrasgo-2023.2.2/pyrasgo/storage/dataframe/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:32:44.000000 pyrasgo-2023.2.2/pyrasgo/storage/datawarehouse/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-02-27 20:32:17.000000 pyrasgo-2023.2.2/pyrasgo/storage/datawarehouse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9080 2023-02-27 20:32:17.000000 pyrasgo-2023.2.2/pyrasgo/storage/datawarehouse/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-02-27 20:32:17.000000 pyrasgo-2023.2.2/pyrasgo/storage/datawarehouse/connect.py
--rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-02-27 20:32:17.000000 pyrasgo-2023.2.2/pyrasgo/storage/datawarehouse/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-02-27 20:32:17.000000 pyrasgo-2023.2.2/pyrasgo/storage/datawarehouse/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:32:44.000000 pyrasgo-2023.2.2/pyrasgo/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 20:32:17.000000 pyrasgo-2023.2.2/pyrasgo/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12314 2023-02-27 20:32:17.000000 pyrasgo-2023.2.2/pyrasgo/utils/dbt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-02-27 20:32:17.000000 pyrasgo-2023.2.2/pyrasgo/utils/naming.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-02-27 20:32:17.000000 pyrasgo-2023.2.2/pyrasgo/utils/polling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-02-27 20:32:17.000000 pyrasgo-2023.2.2/pyrasgo/utils/rendering.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-02-27 20:32:17.000000 pyrasgo-2023.2.2/pyrasgo/utils/versioning.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-27 20:32:17.000000 pyrasgo-2023.2.2/pyrasgo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:32:44.000000 pyrasgo-2023.2.2/pyrasgo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-02-27 20:32:44.000000 pyrasgo-2023.2.2/pyrasgo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-02-27 20:32:44.000000 pyrasgo-2023.2.2/pyrasgo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 20:32:44.000000 pyrasgo-2023.2.2/pyrasgo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-02-27 20:32:44.000000 pyrasgo-2023.2.2/pyrasgo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-27 20:32:44.000000 pyrasgo-2023.2.2/pyrasgo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-27 20:32:44.000000 pyrasgo-2023.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-02-27 20:32:17.000000 pyrasgo-2023.2.2/setup.py
+drwxr-xr-x   0 griff      (501) staff       (20)        0 2023-05-20 12:52:04.825736 pyrasgo-2023.5.1/
+-rw-r--r--   0 griff      (501) staff       (20)    34283 2021-10-06 02:27:09.000000 pyrasgo-2023.5.1/LICENSE.md
+-rw-r--r--   0 griff      (501) staff       (20)     3314 2023-05-20 12:52:04.825116 pyrasgo-2023.5.1/PKG-INFO
+drwxr-xr-x   0 griff      (501) staff       (20)        0 2023-05-20 12:52:04.792845 pyrasgo-2023.5.1/pyrasgo/
+-rw-r--r--   0 griff      (501) staff       (20)     1464 2022-09-03 12:15:07.000000 pyrasgo-2023.5.1/pyrasgo/__init__.py
+drwxr-xr-x   0 griff      (501) staff       (20)        0 2023-05-20 12:52:04.803153 pyrasgo-2023.5.1/pyrasgo/api/
+-rw-r--r--   0 griff      (501) staff       (20)      256 2022-09-01 15:43:46.000000 pyrasgo-2023.5.1/pyrasgo/api/__init__.py
+-rw-r--r--   0 griff      (501) staff       (20)     7420 2023-05-19 17:40:37.000000 pyrasgo-2023.5.1/pyrasgo/api/connection.py
+-rw-r--r--   0 griff      (501) staff       (20)     9157 2023-02-22 15:21:03.000000 pyrasgo-2023.5.1/pyrasgo/api/create.py
+-rw-r--r--   0 griff      (501) staff       (20)     2069 2022-09-16 17:20:05.000000 pyrasgo-2023.5.1/pyrasgo/api/delete.py
+-rw-r--r--   0 griff      (501) staff       (20)     7730 2023-02-22 15:21:03.000000 pyrasgo-2023.5.1/pyrasgo/api/get.py
+-rw-r--r--   0 griff      (501) staff       (20)     1191 2022-05-27 20:04:54.000000 pyrasgo-2023.5.1/pyrasgo/api/login.py
+-rw-r--r--   0 griff      (501) staff       (20)    24822 2023-05-19 17:40:37.000000 pyrasgo-2023.5.1/pyrasgo/api/publish.py
+-rw-r--r--   0 griff      (501) staff       (20)     3094 2022-11-04 13:28:05.000000 pyrasgo-2023.5.1/pyrasgo/api/read.py
+-rw-r--r--   0 griff      (501) staff       (20)     3364 2023-05-19 17:40:37.000000 pyrasgo-2023.5.1/pyrasgo/api/session.py
+-rw-r--r--   0 griff      (501) staff       (20)    12802 2023-02-22 15:21:03.000000 pyrasgo-2023.5.1/pyrasgo/api/update.py
+-rw-r--r--   0 griff      (501) staff       (20)      426 2022-09-03 12:12:56.000000 pyrasgo-2023.5.1/pyrasgo/config.py
+-rw-r--r--   0 griff      (501) staff       (20)      229 2022-09-03 12:12:56.000000 pyrasgo-2023.5.1/pyrasgo/constants.py
+-rw-r--r--   0 griff      (501) staff       (20)     1927 2022-09-03 12:12:56.000000 pyrasgo-2023.5.1/pyrasgo/errors.py
+-rw-r--r--   0 griff      (501) staff       (20)     1286 2022-05-27 20:04:54.000000 pyrasgo-2023.5.1/pyrasgo/imports.py
+drwxr-xr-x   0 griff      (501) staff       (20)        0 2023-05-20 12:52:04.805770 pyrasgo-2023.5.1/pyrasgo/primitives/
+-rw-r--r--   0 griff      (501) staff       (20)      131 2022-05-08 14:56:11.000000 pyrasgo-2023.5.1/pyrasgo/primitives/__init__.py
+-rw-r--r--   0 griff      (501) staff       (20)    35379 2023-02-22 15:21:03.000000 pyrasgo-2023.5.1/pyrasgo/primitives/dataset.py
+-rw-r--r--   0 griff      (501) staff       (20)     3589 2022-07-13 03:49:35.000000 pyrasgo-2023.5.1/pyrasgo/primitives/dbt.py
+-rw-r--r--   0 griff      (501) staff       (20)      497 2022-09-03 12:12:56.000000 pyrasgo-2023.5.1/pyrasgo/rasgo.py
+drwxr-xr-x   0 griff      (501) staff       (20)        0 2023-05-20 12:52:04.815698 pyrasgo-2023.5.1/pyrasgo/schemas/
+-rw-r--r--   0 griff      (501) staff       (20)      823 2023-02-22 15:21:03.000000 pyrasgo-2023.5.1/pyrasgo/schemas/__init__.py
+-rw-r--r--   0 griff      (501) staff       (20)      132 2022-11-01 17:50:09.000000 pyrasgo-2023.5.1/pyrasgo/schemas/attributes.py
+-rw-r--r--   0 griff      (501) staff       (20)     5931 2023-04-18 14:42:47.000000 pyrasgo-2023.5.1/pyrasgo/schemas/dataset.py
+-rw-r--r--   0 griff      (501) staff       (20)      809 2022-11-01 19:39:21.000000 pyrasgo-2023.5.1/pyrasgo/schemas/dataset_column.py
+-rw-r--r--   0 griff      (501) staff       (20)      341 2022-04-25 20:21:05.000000 pyrasgo-2023.5.1/pyrasgo/schemas/dw.py
+-rw-r--r--   0 griff      (501) staff       (20)     2296 2023-02-22 15:21:03.000000 pyrasgo-2023.5.1/pyrasgo/schemas/dw_operation.py
+-rw-r--r--   0 griff      (501) staff       (20)     3865 2023-04-18 14:42:47.000000 pyrasgo-2023.5.1/pyrasgo/schemas/dw_operation_set.py
+-rw-r--r--   0 griff      (501) staff       (20)      940 2022-09-16 17:20:05.000000 pyrasgo-2023.5.1/pyrasgo/schemas/dw_table.py
+-rw-r--r--   0 griff      (501) staff       (20)      156 2023-02-22 15:21:03.000000 pyrasgo-2023.5.1/pyrasgo/schemas/enums.py
+-rw-r--r--   0 griff      (501) staff       (20)     3683 2022-11-13 14:11:46.000000 pyrasgo-2023.5.1/pyrasgo/schemas/metric.py
+-rw-r--r--   0 griff      (501) staff       (20)     2526 2023-02-22 15:21:03.000000 pyrasgo-2023.5.1/pyrasgo/schemas/offline.py
+-rw-r--r--   0 griff      (501) staff       (20)       76 2021-07-14 13:06:35.000000 pyrasgo-2023.5.1/pyrasgo/schemas/organization.py
+-rw-r--r--   0 griff      (501) staff       (20)      214 2022-04-21 23:22:30.000000 pyrasgo-2023.5.1/pyrasgo/schemas/status_tracking.py
+-rw-r--r--   0 griff      (501) staff       (20)     2603 2023-01-24 03:07:22.000000 pyrasgo-2023.5.1/pyrasgo/schemas/transform.py
+-rw-r--r--   0 griff      (501) staff       (20)      795 2023-01-24 01:16:51.000000 pyrasgo-2023.5.1/pyrasgo/schemas/user.py
+drwxr-xr-x   0 griff      (501) staff       (20)        0 2023-05-20 12:52:04.816182 pyrasgo-2023.5.1/pyrasgo/storage/
+-rw-r--r--   0 griff      (501) staff       (20)       56 2022-05-27 20:04:54.000000 pyrasgo-2023.5.1/pyrasgo/storage/__init__.py
+drwxr-xr-x   0 griff      (501) staff       (20)        0 2023-05-20 12:52:04.817059 pyrasgo-2023.5.1/pyrasgo/storage/dataframe/
+-rw-r--r--   0 griff      (501) staff       (20)        0 2021-07-14 13:06:35.000000 pyrasgo-2023.5.1/pyrasgo/storage/dataframe/__init__.py
+-rw-r--r--   0 griff      (501) staff       (20)     4306 2022-05-27 20:04:54.000000 pyrasgo-2023.5.1/pyrasgo/storage/dataframe/utils.py
+drwxr-xr-x   0 griff      (501) staff       (20)        0 2023-05-20 12:52:04.820675 pyrasgo-2023.5.1/pyrasgo/storage/datawarehouse/
+-rw-r--r--   0 griff      (501) staff       (20)      170 2022-05-27 20:04:54.000000 pyrasgo-2023.5.1/pyrasgo/storage/datawarehouse/__init__.py
+-rw-r--r--   0 griff      (501) staff       (20)     9197 2023-05-19 17:40:37.000000 pyrasgo-2023.5.1/pyrasgo/storage/datawarehouse/bigquery.py
+-rw-r--r--   0 griff      (501) staff       (20)      786 2022-05-27 20:04:54.000000 pyrasgo-2023.5.1/pyrasgo/storage/datawarehouse/connect.py
+-rw-r--r--   0 griff      (501) staff       (20)     8023 2023-05-19 17:40:37.000000 pyrasgo-2023.5.1/pyrasgo/storage/datawarehouse/snowflake.py
+-rw-r--r--   0 griff      (501) staff       (20)     1499 2022-07-13 03:49:35.000000 pyrasgo-2023.5.1/pyrasgo/storage/datawarehouse/utils.py
+drwxr-xr-x   0 griff      (501) staff       (20)        0 2023-05-20 12:52:04.823977 pyrasgo-2023.5.1/pyrasgo/utils/
+-rw-r--r--   0 griff      (501) staff       (20)        0 2022-04-21 18:08:01.000000 pyrasgo-2023.5.1/pyrasgo/utils/__init__.py
+-rw-r--r--   0 griff      (501) staff       (20)    12314 2022-09-03 12:26:54.000000 pyrasgo-2023.5.1/pyrasgo/utils/dbt.py
+-rw-r--r--   0 griff      (501) staff       (20)     6500 2022-11-04 14:53:42.000000 pyrasgo-2023.5.1/pyrasgo/utils/naming.py
+-rw-r--r--   0 griff      (501) staff       (20)     2612 2023-02-22 15:21:03.000000 pyrasgo-2023.5.1/pyrasgo/utils/polling.py
+-rw-r--r--   0 griff      (501) staff       (20)     4252 2023-02-06 12:07:15.000000 pyrasgo-2023.5.1/pyrasgo/utils/rendering.py
+-rw-r--r--   0 griff      (501) staff       (20)      883 2022-04-25 20:21:05.000000 pyrasgo-2023.5.1/pyrasgo/utils/versioning.py
+-rw-r--r--   0 griff      (501) staff       (20)       25 2023-05-19 17:40:37.000000 pyrasgo-2023.5.1/pyrasgo/version.py
+drwxr-xr-x   0 griff      (501) staff       (20)        0 2023-05-20 12:52:04.797168 pyrasgo-2023.5.1/pyrasgo.egg-info/
+-rw-r--r--   0 griff      (501) staff       (20)     3314 2023-05-20 12:52:04.000000 pyrasgo-2023.5.1/pyrasgo.egg-info/PKG-INFO
+-rw-r--r--   0 griff      (501) staff       (20)     1508 2023-05-20 12:52:04.000000 pyrasgo-2023.5.1/pyrasgo.egg-info/SOURCES.txt
+-rw-r--r--   0 griff      (501) staff       (20)        1 2023-05-20 12:52:04.000000 pyrasgo-2023.5.1/pyrasgo.egg-info/dependency_links.txt
+-rw-r--r--   0 griff      (501) staff       (20)      304 2023-05-20 12:52:04.000000 pyrasgo-2023.5.1/pyrasgo.egg-info/requires.txt
+-rw-r--r--   0 griff      (501) staff       (20)        8 2023-05-20 12:52:04.000000 pyrasgo-2023.5.1/pyrasgo.egg-info/top_level.txt
+-rw-r--r--   0 griff      (501) staff       (20)       38 2023-05-20 12:52:04.826288 pyrasgo-2023.5.1/setup.cfg
+-rw-r--r--   0 griff      (501) staff       (20)     2303 2022-11-01 20:07:10.000000 pyrasgo-2023.5.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyrasgo-2023.2.2/LICENSE.md` & `pyrasgo-2023.5.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyrasgo-2023.2.2/PKG-INFO` & `pyrasgo-2023.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrasgo
-Version: 2023.2.2
+Version: 2023.5.1
 Summary: Python interface to the Rasgo API.
 Home-page: https://www.rasgoml.com/
 Author: Patrick Dougherty
 Author-email: patrick@rasgoml.com
 License: GNU Affero General Public License v3 or later (AGPLv3+)
 Project-URL: Documentation, https://docs.rasgoml.com
 Project-URL: Source, https://github.com/rasgointelligence/RasgoSDKPython
```

### Comparing `pyrasgo-2023.2.2/pyrasgo/__init__.py` & `pyrasgo-2023.5.1/pyrasgo/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrasgo-2023.2.2/pyrasgo/api/connection.py` & `pyrasgo-2023.5.1/pyrasgo/api/connection.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,33 +15,30 @@
     """
 
     def __init__(self, api_key=None):
         if api_key:
             self._api_key = api_key
 
     def _default_dw_namespace(self) -> Dict:
-        dw_creds = self._profile.get("dw_creds")
-        organization = self._profile.get("organization")
-        if not dw_creds or not organization:
+        if not self._dc:
             raise errors.DWCredentialsWarning("Your user profile is missing critical information. Contact Rasgo.")
         return {
-            'database': organization.get("database", dw_creds.get("project")),
-            'schema': organization.get("schema", dw_creds.get("dataset")),
+            "database": self._dc.get("database", self._dc.get("project")),
+            "schema": self._dc.get("schema", self._dc.get("dataset")),
         }
 
     def _dw_type(self) -> str:
-        org = self._profile.get('organization')
-        if not org:
+        if not self._dc:
             raise errors.DWCredentialsWarning("Your user profile is missing critical information. Contact Rasgo.")
-        return org.get('cloudDataWarehouse', org.get('dw_type'))
+        return self._dc.get("dw_type")
 
     def _url(self, resource, api_version=None):
-        if '/' == resource[0]:
+        if "/" == resource[0]:
             resource = resource[1:]
-        protocol = 'http' if self._environment.value == 'localhost' else 'https'
+        protocol = "http" if self._environment.value == "localhost" else "https"
         return f"{protocol}://{self._environment.value}/{'' if api_version is None else f'v{api_version}/'}{resource}"
 
     def find(self, resource, equality_filters):
         search_strings = []
         for k, v in equality_filters.items():
             filter_str = k + "||$eq||" + v
             search_strings.append(filter_str)
```

### Comparing `pyrasgo-2023.2.2/pyrasgo/api/create.py` & `pyrasgo-2023.5.1/pyrasgo/api/create.py`

 * *Files identical despite different names*

### Comparing `pyrasgo-2023.2.2/pyrasgo/api/delete.py` & `pyrasgo-2023.5.1/pyrasgo/api/delete.py`

 * *Files identical despite different names*

### Comparing `pyrasgo-2023.2.2/pyrasgo/api/get.py` & `pyrasgo-2023.5.1/pyrasgo/api/get.py`

 * *Files identical despite different names*

### Comparing `pyrasgo-2023.2.2/pyrasgo/api/login.py` & `pyrasgo-2023.5.1/pyrasgo/api/login.py`

 * *Files identical despite different names*

### Comparing `pyrasgo-2023.2.2/pyrasgo/api/publish.py` & `pyrasgo-2023.5.1/pyrasgo/api/publish.py`

 * *Files 1% similar despite different names*

```diff
@@ -379,15 +379,15 @@
                     "To update the Dataset referenced by this fqtn, please omit or change your resource_key arg. "
                     "To update the Dataset referenced by this resource_key, please omit or change your fqtn arg."
                 )
 
         ds_to_update = ds_matched_on_rk or ds_matched_on_fqtn
         if ds_to_update:
             # Users should only be able to overwrite datasets in their own organization
-            if ds_to_update._api_dataset.organization_id != self.api._profile.get("organizationId"):
+            if ds_to_update._api_dataset.organization_id != self.api._profile["organization"]["id"]:
                 raise errors.RasgoRuleViolation(
                     f"Dataset {ds_to_update.id} already exists. This API key does not have permission to replace it."
                 )
             if if_exists == "fail":
                 raise errors.ParameterValueError(
                     message=f"Dataset {ds_to_update.id} already exists, and {if_exists} was passed for `if_exists`. "
                     "Please confirm the resource_key & fqtn or choose another value for `if_exists`"
```

### Comparing `pyrasgo-2023.2.2/pyrasgo/api/read.py` & `pyrasgo-2023.5.1/pyrasgo/api/read.py`

 * *Files identical despite different names*

### Comparing `pyrasgo-2023.2.2/pyrasgo/api/session.py` & `pyrasgo-2023.5.1/pyrasgo/api/session.py`

 * *Files 11% similar despite different names*

```diff
@@ -31,57 +31,68 @@
     @classmethod
     def from_environment(cls):
         return cls(os.getenv("RASGO_DOMAIN", cls.PRODUCTION))
 
     @property
     def app_path(self):
         if self == self.PRODUCTION:
-            return 'https://app.rasgoml.com'
+            return "https://app.rasgoml.com"
         if self == self.STAGING:
-            return 'https://dev.rasgoml.com'
+            return "https://staging.rasgoml.com"
         if self == self.LOCAL:
-            return 'http://localhost:9000'
+            return "http://localhost:9000"
 
 
 class SessionMeta(type):
     _api_key = None
     _profile = None
+    _dc = None
     _environment = None
 
     def __new__(mcs, name, bases, dct):
         new = super().__new__(mcs, name, bases, dct)
-        logging.debug(f'Starting the session for user')
+        logging.debug("Starting the session for user")
         new._environment = Environment.from_environment()
         new._api_key = mcs._api_key or None
         new._profile = mcs._profile or None
+        new._dc = mcs._dc or None
         return new
 
     def __call__(cls, *args, **kwargs):
         if SessionMeta._api_key is None:
             api_key = kwargs.pop("api_key", None)
             if not api_key:
                 raise InvalidApiKeyException("Must provide an API key to access the endpoint")
             SessionMeta._api_key = api_key
         if SessionMeta._environment is None:
             SessionMeta._environment = Environment.from_environment()
-        if SessionMeta._profile is None:
-            protocol = 'http' if SessionMeta._environment.value == 'localhost' else 'https'
-            response = requests.get(
-                f"{protocol}://{SessionMeta._environment.value}/v1/users/me",
+        if SessionMeta._profile is None or SessionMeta._dc is None:
+            protocol = "http" if SessionMeta._environment.value == "localhost" else "https"
+            profile_response = requests.get(
+                f"{protocol}://{SessionMeta._environment.value}/v2/users/current-user",
                 headers=generate_headers(SessionMeta._api_key),
+                timeout=25,
+            )
+            dc_response = requests.get(
+                f"{protocol}://{SessionMeta._environment.value}/v2/users/dw-credentials",
+                headers=generate_headers(SessionMeta._api_key),
+                timeout=25,
             )
             try:
-                response.raise_for_status()
+                profile_response.raise_for_status()
+                dc_response.raise_for_status()
             except HTTPError:
                 raise InvalidApiKeyException(
                     f"The API key provided ({SessionMeta._api_key[:5]}...{SessionMeta._api_key[-5:]}) is not valid."
                 )
-            SessionMeta._profile = response.json()
+            SessionMeta._profile = profile_response.json()
+            SessionMeta._dc = dc_response.json()
         cls._api_key = SessionMeta._api_key
         cls._profile = SessionMeta._profile
+        cls._dc = SessionMeta._dc
         cls._environment = SessionMeta._environment
         return type.__call__(cls, *args, **kwargs)
 
 
 class Session(metaclass=SessionMeta):
     pass
```

### Comparing `pyrasgo-2023.2.2/pyrasgo/api/update.py` & `pyrasgo-2023.5.1/pyrasgo/api/update.py`

 * *Files identical despite different names*

### Comparing `pyrasgo-2023.2.2/pyrasgo/errors.py` & `pyrasgo-2023.5.1/pyrasgo/errors.py`

 * *Files identical despite different names*

### Comparing `pyrasgo-2023.2.2/pyrasgo/imports.py` & `pyrasgo-2023.5.1/pyrasgo/imports.py`

 * *Files identical despite different names*

### Comparing `pyrasgo-2023.2.2/pyrasgo/primitives/dataset.py` & `pyrasgo-2023.5.1/pyrasgo/primitives/dataset.py`

 * *Files identical despite different names*

### Comparing `pyrasgo-2023.2.2/pyrasgo/primitives/dbt.py` & `pyrasgo-2023.5.1/pyrasgo/primitives/dbt.py`

 * *Files identical despite different names*

### Comparing `pyrasgo-2023.2.2/pyrasgo/schemas/__init__.py` & `pyrasgo-2023.5.1/pyrasgo/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrasgo-2023.2.2/pyrasgo/schemas/dataset.py` & `pyrasgo-2023.5.1/pyrasgo/schemas/dataset.py`

 * *Files identical despite different names*

### Comparing `pyrasgo-2023.2.2/pyrasgo/schemas/dataset_column.py` & `pyrasgo-2023.5.1/pyrasgo/schemas/dataset_column.py`

 * *Files identical despite different names*

### Comparing `pyrasgo-2023.2.2/pyrasgo/schemas/dw_operation.py` & `pyrasgo-2023.5.1/pyrasgo/schemas/dw_operation.py`

 * *Files identical despite different names*

### Comparing `pyrasgo-2023.2.2/pyrasgo/schemas/dw_operation_set.py` & `pyrasgo-2023.5.1/pyrasgo/schemas/dw_operation_set.py`

 * *Files identical despite different names*

### Comparing `pyrasgo-2023.2.2/pyrasgo/schemas/dw_table.py` & `pyrasgo-2023.5.1/pyrasgo/schemas/dw_table.py`

 * *Files identical despite different names*

### Comparing `pyrasgo-2023.2.2/pyrasgo/schemas/metric.py` & `pyrasgo-2023.5.1/pyrasgo/schemas/metric.py`

 * *Files identical despite different names*

### Comparing `pyrasgo-2023.2.2/pyrasgo/schemas/offline.py` & `pyrasgo-2023.5.1/pyrasgo/schemas/offline.py`

 * *Files identical despite different names*

### Comparing `pyrasgo-2023.2.2/pyrasgo/schemas/transform.py` & `pyrasgo-2023.5.1/pyrasgo/schemas/transform.py`

 * *Files identical despite different names*

### Comparing `pyrasgo-2023.2.2/pyrasgo/schemas/user.py` & `pyrasgo-2023.5.1/pyrasgo/schemas/user.py`

 * *Files identical despite different names*

### Comparing `pyrasgo-2023.2.2/pyrasgo/storage/dataframe/utils.py` & `pyrasgo-2023.5.1/pyrasgo/storage/dataframe/utils.py`

 * *Files identical despite different names*

### Comparing `pyrasgo-2023.2.2/pyrasgo/storage/datawarehouse/bigquery.py` & `pyrasgo-2023.5.1/pyrasgo/storage/datawarehouse/bigquery.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,17 +27,19 @@
     def __init__(self):
         if bq is None:
             raise errors.PackageDependencyWarning(
                 "Missing a required python package to run BigQuery. "
                 "Please download the BigQuery package by running: "
                 "pip install pyrasgo[bigquery]"
             )
-        _creds = self.profile.get("dw_creds")
+        _creds = self._dc
         if not _creds:
             raise errors.DWCredentialsWarning("Your user is missing credentials, please contact Rasgo.")
+        if self._profile.get("isSso", False):
+            raise errors.DWCredentialsWarning("PyRasgo does not support SSO connections.")
         self._connection: bq.Client = None
         self._credentials: bq.Credentials = None
         self._key = _creds.get("json_key")
         self.default_database = _creds.get("project")
         self.default_schema = _creds.get("dataset")
 
     @property
```

### Comparing `pyrasgo-2023.2.2/pyrasgo/storage/datawarehouse/connect.py` & `pyrasgo-2023.5.1/pyrasgo/storage/datawarehouse/connect.py`

 * *Files identical despite different names*

### Comparing `pyrasgo-2023.2.2/pyrasgo/storage/datawarehouse/snowflake.py` & `pyrasgo-2023.5.1/pyrasgo/storage/datawarehouse/snowflake.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,50 +14,57 @@
 from pyrasgo.storage.dataframe import utils as dfutils
 from pyrasgo import errors
 from pyrasgo.imports import sf_connector, write_pandas
 from pyrasgo.schemas.enums import DataWarehouseType
 from pyrasgo.storage.datawarehouse import utils
 
 
+def unobscure(obscured: bytes) -> bytes:
+    import zlib
+    from base64 import urlsafe_b64decode
+
+    return zlib.decompress(urlsafe_b64decode(obscured)).decode()
+
+
 class SnowflakeDataWarehouse(Session):
     """
     Snowflake DataWarehouse Class
     """
 
     def __init__(self):
         if not sf_connector:
             raise errors.PackageDependencyWarning(
                 "Missing a required python package to run Snowflake. "
                 "Please download the Snowflake package by running: "
                 "pip install pyrasgo[snowflake]"
             )
 
-        _creds = self.profile.get("dw_creds")
-        _organization = self.profile.get("organization")
+        _creds = self._dc
         if not _creds:
             raise errors.DWCredentialsWarning("Your user is missing credentials, please contact Rasgo.")
-
+        if self._profile.get("isSso", False):
+            raise errors.DWCredentialsWarning("PyRasgo does not support SSO connections.")
         self._connection: sf_connector.SnowflakeConnection = None
         self._credentials: dict = {
             "user": _creds.get("user"),
-            "password": _creds.get("password"),
-            "role": _creds.get("role", _organization.get("role")),
-            "account": _creds.get("account", _organization.get("account")),
-            "database": _creds.get("database", _organization.get("database")),
-            "schema": _creds.get("schema", _organization.get("schema")),
-            "warehouse": _creds.get("warehouse", _organization.get("warehouse")),
+            "password": unobscure(_creds.get("password")),
+            "role": _creds.get("role"),
+            "account": _creds.get("account"),
+            "database": _creds.get("database"),
+            "schema": _creds.get("schema"),
+            "warehouse": _creds.get("warehouse"),
             "application": "rasgo",
             "session_parameters": {
                 "QUERY_TAG": "rasgo_python_sdk",
                 "TIMESTAMP_NTZ_OUTPUT_FORMAT": "YYYY-MM-DD HH24:MI:SS.FF3",
                 "TIMESTAMP_OUTPUT_FORMAT": "YYYY-MM-DD HH24:MI:SS.FF3 TZHTZM",
             },
         }
-        self.default_database = _organization.get("database")
-        self.default_schema = _organization.get("schema")
+        self.default_database = _creds.get("database")
+        self.default_schema = _creds.get("schema")
 
     @property
     def connection(self) -> 'sf_connector.SnowflakeConnection':
         """
         Returns a connection to Snowflake
         """
         if not self._connection:
```

### Comparing `pyrasgo-2023.2.2/pyrasgo/storage/datawarehouse/utils.py` & `pyrasgo-2023.5.1/pyrasgo/storage/datawarehouse/utils.py`

 * *Files identical despite different names*

### Comparing `pyrasgo-2023.2.2/pyrasgo/utils/dbt.py` & `pyrasgo-2023.5.1/pyrasgo/utils/dbt.py`

 * *Files identical despite different names*

### Comparing `pyrasgo-2023.2.2/pyrasgo/utils/naming.py` & `pyrasgo-2023.5.1/pyrasgo/utils/naming.py`

 * *Files identical despite different names*

### Comparing `pyrasgo-2023.2.2/pyrasgo/utils/polling.py` & `pyrasgo-2023.5.1/pyrasgo/utils/polling.py`

 * *Files identical despite different names*

### Comparing `pyrasgo-2023.2.2/pyrasgo/utils/rendering.py` & `pyrasgo-2023.5.1/pyrasgo/utils/rendering.py`

 * *Files identical despite different names*

### Comparing `pyrasgo-2023.2.2/pyrasgo/utils/versioning.py` & `pyrasgo-2023.5.1/pyrasgo/utils/versioning.py`

 * *Files identical despite different names*

### Comparing `pyrasgo-2023.2.2/pyrasgo.egg-info/PKG-INFO` & `pyrasgo-2023.5.1/pyrasgo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrasgo
-Version: 2023.2.2
+Version: 2023.5.1
 Summary: Python interface to the Rasgo API.
 Home-page: https://www.rasgoml.com/
 Author: Patrick Dougherty
 Author-email: patrick@rasgoml.com
 License: GNU Affero General Public License v3 or later (AGPLv3+)
 Project-URL: Documentation, https://docs.rasgoml.com
 Project-URL: Source, https://github.com/rasgointelligence/RasgoSDKPython
```

### Comparing `pyrasgo-2023.2.2/pyrasgo.egg-info/SOURCES.txt` & `pyrasgo-2023.5.1/pyrasgo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrasgo-2023.2.2/setup.py` & `pyrasgo-2023.5.1/setup.py`

 * *Files identical despite different names*

