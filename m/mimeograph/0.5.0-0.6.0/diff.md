# Comparing `tmp/mimeograph-0.5.0.tar.gz` & `tmp/mimeograph-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mimeograph-0.5.0.tar", last modified: Fri May 12 09:59:04 2023, max compression
+gzip compressed data, was "mimeograph-0.6.0.tar", last modified: Sat May 20 16:31:41 2023, max compression
```

## Comparing `mimeograph-0.5.0.tar` & `mimeograph-0.6.0.tar`

### file list

```diff
@@ -1,80 +1,84 @@
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-12 09:59:04.042522 mimeograph-0.5.0/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1075 2023-03-13 05:35:12.000000 mimeograph-0.5.0/LICENSE
--rw-rw-r--   0 tom       (1000) tom       (1000)       30 2023-05-11 05:33:09.000000 mimeograph-0.5.0/MANIFEST.in
--rw-rw-r--   0 tom       (1000) tom       (1000)    23377 2023-05-12 09:59:04.042522 mimeograph-0.5.0/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)    21021 2023-05-12 09:42:23.000000 mimeograph-0.5.0/README.md
--rw-rw-r--   0 tom       (1000) tom       (1000)     3692 2023-05-12 09:58:54.000000 mimeograph-0.5.0/pyproject.toml
--rw-rw-r--   0 tom       (1000) tom       (1000)       38 2023-05-12 09:59:04.042522 mimeograph-0.5.0/setup.cfg
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-12 09:59:04.034522 mimeograph-0.5.0/src/
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-12 09:59:04.034522 mimeograph-0.5.0/src/mimeo/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1327 2023-05-12 09:58:54.000000 mimeograph-0.5.0/src/mimeo/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      408 2023-05-11 13:41:23.000000 mimeograph-0.5.0/src/mimeo/__main__.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-12 09:59:04.034522 mimeograph-0.5.0/src/mimeo/cli/
--rw-rw-r--   0 tom       (1000) tom       (1000)      761 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/cli/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1660 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/cli/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     4283 2023-05-12 09:42:23.000000 mimeograph-0.5.0/src/mimeo/cli/job.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    17274 2023-05-12 09:58:54.000000 mimeograph-0.5.0/src/mimeo/cli/parsers.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-12 09:59:04.034522 mimeograph-0.5.0/src/mimeo/config/
--rw-rw-r--   0 tom       (1000) tom       (1000)      589 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/config/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     3111 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/config/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    28118 2023-05-12 09:42:23.000000 mimeograph-0.5.0/src/mimeo/config/mimeo_config.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-12 09:59:04.038522 mimeograph-0.5.0/src/mimeo/consumers/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1322 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/consumers/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1402 2023-05-12 09:42:23.000000 mimeograph-0.5.0/src/mimeo/consumers/consumer.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2135 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/consumers/consumer_factory.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2364 2023-05-12 09:42:23.000000 mimeograph-0.5.0/src/mimeo/consumers/file_consumer.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     3032 2023-05-12 09:42:23.000000 mimeograph-0.5.0/src/mimeo/consumers/http_consumer.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1018 2023-05-12 09:42:23.000000 mimeograph-0.5.0/src/mimeo/consumers/raw_consumer.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-12 09:59:04.038522 mimeograph-0.5.0/src/mimeo/context/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1001 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/context/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     4261 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/context/decorators.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5087 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/context/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    16065 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/context/mimeo_context.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5091 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/context/mimeo_context_manager.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2888 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/context/mimeo_iteration.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-12 09:59:04.038522 mimeograph-0.5.0/src/mimeo/database/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1533 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/database/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5515 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/database/cities.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5763 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/database/countries.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2120 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/database/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5479 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/database/first_names.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2192 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/database/last_names.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     8025 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/database/mimeo_db.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-12 09:59:04.038522 mimeograph-0.5.0/src/mimeo/generators/
--rw-rw-r--   0 tom       (1000) tom       (1000)      981 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/generators/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1117 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/generators/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2685 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/generators/generator.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1640 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/generators/generator_factory.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    24152 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/generators/xml_generator.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-12 09:59:04.038522 mimeograph-0.5.0/src/mimeo/logging/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1364 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/logging/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1743 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/logging/filters.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-12 09:59:04.038522 mimeograph-0.5.0/src/mimeo/meta/
--rw-rw-r--   0 tom       (1000) tom       (1000)      652 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/meta/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     4028 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/meta/alive.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      651 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/meta/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1525 2023-05-12 09:42:23.000000 mimeograph-0.5.0/src/mimeo/mimeo.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-12 09:59:04.042522 mimeograph-0.5.0/src/mimeo/resources/
--rw-rw-r--   0 tom       (1000) tom       (1000)      357 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/resources/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)  1541655 2023-05-08 08:24:08.000000 mimeograph-0.5.0/src/mimeo/resources/cities.csv
--rw-rw-r--   0 tom       (1000) tom       (1000)     4205 2023-05-08 08:24:08.000000 mimeograph-0.5.0/src/mimeo/resources/countries.csv
--rw-rw-r--   0 tom       (1000) tom       (1000)      778 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/resources/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    66313 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/resources/forenames.csv
--rw-rw-r--   0 tom       (1000) tom       (1000)      719 2023-03-31 04:40:40.000000 mimeograph-0.5.0/src/mimeo/resources/logging.yaml
--rw-rw-r--   0 tom       (1000) tom       (1000)  1197769 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/resources/surnames.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)     1030 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/tools.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-12 09:59:04.042522 mimeograph-0.5.0/src/mimeo/utils/
--rw-rw-r--   0 tom       (1000) tom       (1000)     2063 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/utils/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1412 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/utils/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    24474 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/utils/mimeo_utils.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    20016 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/utils/renderers.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-12 09:59:04.042522 mimeograph-0.5.0/src/mimeograph.egg-info/
--rw-rw-r--   0 tom       (1000) tom       (1000)    23377 2023-05-12 09:59:04.000000 mimeograph-0.5.0/src/mimeograph.egg-info/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)     1854 2023-05-12 09:59:04.000000 mimeograph-0.5.0/src/mimeograph.egg-info/SOURCES.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        1 2023-05-12 09:59:04.000000 mimeograph-0.5.0/src/mimeograph.egg-info/dependency_links.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       46 2023-05-12 09:59:04.000000 mimeograph-0.5.0/src/mimeograph.egg-info/entry_points.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)      212 2023-05-12 09:59:04.000000 mimeograph-0.5.0/src/mimeograph.egg-info/requires.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        6 2023-05-12 09:59:04.000000 mimeograph-0.5.0/src/mimeograph.egg-info/top_level.txt
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-12 09:59:04.042522 mimeograph-0.5.0/tests/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1828 2023-05-12 09:42:23.000000 mimeograph-0.5.0/tests/test_mimeograph.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      514 2023-05-11 05:33:09.000000 mimeograph-0.5.0/tests/test_tools.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-20 16:31:41.902028 mimeograph-0.6.0/
+-rw-r--r--   0 tom        (501) staff       (20)     1075 2023-03-12 16:41:41.000000 mimeograph-0.6.0/LICENSE
+-rw-r--r--   0 tom        (501) staff       (20)       30 2023-05-09 15:53:05.000000 mimeograph-0.6.0/MANIFEST.in
+-rw-r--r--   0 tom        (501) staff       (20)    26854 2023-05-20 16:31:41.901820 mimeograph-0.6.0/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)    24498 2023-05-17 16:22:49.000000 mimeograph-0.6.0/README.md
+-rw-r--r--   0 tom        (501) staff       (20)     3768 2023-05-20 16:30:13.000000 mimeograph-0.6.0/pyproject.toml
+-rw-r--r--   0 tom        (501) staff       (20)       38 2023-05-20 16:31:41.902087 mimeograph-0.6.0/setup.cfg
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-20 16:31:41.879002 mimeograph-0.6.0/src/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-20 16:31:41.880912 mimeograph-0.6.0/src/mimeo/
+-rw-r--r--   0 tom        (501) staff       (20)     1327 2023-05-20 16:30:13.000000 mimeograph-0.6.0/src/mimeo/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      408 2023-05-09 15:53:05.000000 mimeograph-0.6.0/src/mimeo/__main__.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-20 16:31:41.882493 mimeograph-0.6.0/src/mimeo/cli/
+-rw-r--r--   0 tom        (501) staff       (20)      761 2023-05-09 15:53:05.000000 mimeograph-0.6.0/src/mimeo/cli/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     2290 2023-05-17 16:22:49.000000 mimeograph-0.6.0/src/mimeo/cli/exc.py
+-rw-r--r--   0 tom        (501) staff       (20)     4408 2023-05-17 16:22:49.000000 mimeograph-0.6.0/src/mimeo/cli/job.py
+-rw-r--r--   0 tom        (501) staff       (20)    16721 2023-05-20 16:30:13.000000 mimeograph-0.6.0/src/mimeo/cli/parsers.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-20 16:31:41.883461 mimeograph-0.6.0/src/mimeo/config/
+-rw-r--r--   0 tom        (501) staff       (20)      691 2023-05-17 16:22:49.000000 mimeograph-0.6.0/src/mimeo/config/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     5718 2023-05-17 16:22:49.000000 mimeograph-0.6.0/src/mimeo/config/constants.py
+-rw-r--r--   0 tom        (501) staff       (20)    10653 2023-05-20 16:17:22.000000 mimeograph-0.6.0/src/mimeo/config/exc.py
+-rw-r--r--   0 tom        (501) staff       (20)    23424 2023-05-20 16:17:22.000000 mimeograph-0.6.0/src/mimeo/config/mimeo_config.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-20 16:31:41.885840 mimeograph-0.6.0/src/mimeo/consumers/
+-rw-r--r--   0 tom        (501) staff       (20)     1322 2023-05-09 15:53:05.000000 mimeograph-0.6.0/src/mimeo/consumers/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     1402 2023-05-13 05:35:39.000000 mimeograph-0.6.0/src/mimeo/consumers/consumer.py
+-rw-r--r--   0 tom        (501) staff       (20)     2131 2023-05-17 16:22:49.000000 mimeograph-0.6.0/src/mimeo/consumers/consumer_factory.py
+-rw-r--r--   0 tom        (501) staff       (20)     2364 2023-05-13 05:35:39.000000 mimeograph-0.6.0/src/mimeo/consumers/file_consumer.py
+-rw-r--r--   0 tom        (501) staff       (20)     3032 2023-05-13 05:35:39.000000 mimeograph-0.6.0/src/mimeo/consumers/http_consumer.py
+-rw-r--r--   0 tom        (501) staff       (20)     1018 2023-05-13 05:35:39.000000 mimeograph-0.6.0/src/mimeo/consumers/raw_consumer.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-20 16:31:41.887511 mimeograph-0.6.0/src/mimeo/context/
+-rw-r--r--   0 tom        (501) staff       (20)     1001 2023-05-09 15:53:05.000000 mimeograph-0.6.0/src/mimeo/context/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     4261 2023-05-09 15:53:05.000000 mimeograph-0.6.0/src/mimeo/context/decorators.py
+-rw-r--r--   0 tom        (501) staff       (20)     5087 2023-05-09 15:53:05.000000 mimeograph-0.6.0/src/mimeo/context/exc.py
+-rw-r--r--   0 tom        (501) staff       (20)    18138 2023-05-20 16:17:22.000000 mimeograph-0.6.0/src/mimeo/context/mimeo_context.py
+-rw-r--r--   0 tom        (501) staff       (20)     5111 2023-05-17 16:22:49.000000 mimeograph-0.6.0/src/mimeo/context/mimeo_context_manager.py
+-rw-r--r--   0 tom        (501) staff       (20)     2888 2023-05-09 15:53:05.000000 mimeograph-0.6.0/src/mimeo/context/mimeo_iteration.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-20 16:31:41.889805 mimeograph-0.6.0/src/mimeo/database/
+-rw-r--r--   0 tom        (501) staff       (20)     1805 2023-05-17 16:22:49.000000 mimeograph-0.6.0/src/mimeo/database/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     5507 2023-05-17 16:22:49.000000 mimeograph-0.6.0/src/mimeo/database/cities.py
+-rw-r--r--   0 tom        (501) staff       (20)     5775 2023-05-17 16:22:49.000000 mimeograph-0.6.0/src/mimeo/database/countries.py
+-rw-r--r--   0 tom        (501) staff       (20)     5613 2023-05-17 16:22:49.000000 mimeograph-0.6.0/src/mimeo/database/currencies.py
+-rw-r--r--   0 tom        (501) staff       (20)     6200 2023-05-20 16:17:22.000000 mimeograph-0.6.0/src/mimeo/database/exc.py
+-rw-r--r--   0 tom        (501) staff       (20)     5471 2023-05-17 16:22:49.000000 mimeograph-0.6.0/src/mimeo/database/first_names.py
+-rw-r--r--   0 tom        (501) staff       (20)     2180 2023-05-17 16:22:49.000000 mimeograph-0.6.0/src/mimeo/database/last_names.py
+-rw-r--r--   0 tom        (501) staff       (20)    10209 2023-05-17 16:22:49.000000 mimeograph-0.6.0/src/mimeo/database/mimeo_db.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-20 16:31:41.890918 mimeograph-0.6.0/src/mimeo/generators/
+-rw-r--r--   0 tom        (501) staff       (20)      981 2023-05-13 05:35:39.000000 mimeograph-0.6.0/src/mimeo/generators/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     1117 2023-05-13 05:35:39.000000 mimeograph-0.6.0/src/mimeo/generators/exc.py
+-rw-r--r--   0 tom        (501) staff       (20)     2685 2023-05-09 15:53:05.000000 mimeograph-0.6.0/src/mimeo/generators/generator.py
+-rw-r--r--   0 tom        (501) staff       (20)     1654 2023-05-17 16:22:49.000000 mimeograph-0.6.0/src/mimeo/generators/generator_factory.py
+-rw-r--r--   0 tom        (501) staff       (20)    24157 2023-05-17 16:22:49.000000 mimeograph-0.6.0/src/mimeo/generators/xml_generator.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-20 16:31:41.891411 mimeograph-0.6.0/src/mimeo/logging/
+-rw-r--r--   0 tom        (501) staff       (20)     1364 2023-05-09 15:53:05.000000 mimeograph-0.6.0/src/mimeo/logging/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     1743 2023-05-09 15:53:05.000000 mimeograph-0.6.0/src/mimeo/logging/filters.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-20 16:31:41.892087 mimeograph-0.6.0/src/mimeo/meta/
+-rw-r--r--   0 tom        (501) staff       (20)      652 2023-05-09 15:53:05.000000 mimeograph-0.6.0/src/mimeo/meta/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     4033 2023-05-17 16:22:49.000000 mimeograph-0.6.0/src/mimeo/meta/alive.py
+-rw-r--r--   0 tom        (501) staff       (20)      656 2023-05-17 16:22:49.000000 mimeograph-0.6.0/src/mimeo/meta/exc.py
+-rw-r--r--   0 tom        (501) staff       (20)     1525 2023-05-13 05:35:39.000000 mimeograph-0.6.0/src/mimeo/mimeo.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-20 16:31:41.896837 mimeograph-0.6.0/src/mimeo/resources/
+-rw-r--r--   0 tom        (501) staff       (20)      362 2023-05-17 16:22:49.000000 mimeograph-0.6.0/src/mimeo/resources/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)  1541655 2023-03-30 16:49:35.000000 mimeograph-0.6.0/src/mimeo/resources/cities.csv
+-rw-r--r--   0 tom        (501) staff       (20)     1467 2023-05-17 16:22:49.000000 mimeograph-0.6.0/src/mimeo/resources/constants.yaml
+-rw-r--r--   0 tom        (501) staff       (20)     4205 2023-03-30 16:49:35.000000 mimeograph-0.6.0/src/mimeo/resources/countries.csv
+-rw-r--r--   0 tom        (501) staff       (20)     7268 2023-05-17 16:22:49.000000 mimeograph-0.6.0/src/mimeo/resources/currencies.csv
+-rw-r--r--   0 tom        (501) staff       (20)      783 2023-05-17 16:22:49.000000 mimeograph-0.6.0/src/mimeo/resources/exc.py
+-rw-r--r--   0 tom        (501) staff       (20)    66313 2023-05-09 15:53:05.000000 mimeograph-0.6.0/src/mimeo/resources/forenames.csv
+-rw-r--r--   0 tom        (501) staff       (20)      719 2023-03-30 16:49:35.000000 mimeograph-0.6.0/src/mimeo/resources/logging.yaml
+-rw-r--r--   0 tom        (501) staff       (20)  1197769 2023-05-09 15:53:05.000000 mimeograph-0.6.0/src/mimeo/resources/surnames.txt
+-rw-r--r--   0 tom        (501) staff       (20)     1035 2023-05-17 16:22:49.000000 mimeograph-0.6.0/src/mimeo/tools.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-20 16:31:41.899729 mimeograph-0.6.0/src/mimeo/utils/
+-rw-r--r--   0 tom        (501) staff       (20)     2193 2023-05-17 16:22:49.000000 mimeograph-0.6.0/src/mimeo/utils/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     6226 2023-05-20 16:17:22.000000 mimeograph-0.6.0/src/mimeo/utils/exc.py
+-rw-r--r--   0 tom        (501) staff       (20)    29122 2023-05-20 16:17:22.000000 mimeograph-0.6.0/src/mimeo/utils/mimeo_utils.py
+-rw-r--r--   0 tom        (501) staff       (20)    20118 2023-05-20 16:17:22.000000 mimeograph-0.6.0/src/mimeo/utils/renderers.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-20 16:31:41.900924 mimeograph-0.6.0/src/mimeograph.egg-info/
+-rw-r--r--   0 tom        (501) staff       (20)    26854 2023-05-20 16:31:41.000000 mimeograph-0.6.0/src/mimeograph.egg-info/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)     1987 2023-05-20 16:31:41.000000 mimeograph-0.6.0/src/mimeograph.egg-info/SOURCES.txt
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-05-20 16:31:41.000000 mimeograph-0.6.0/src/mimeograph.egg-info/dependency_links.txt
+-rw-r--r--   0 tom        (501) staff       (20)       46 2023-05-20 16:31:41.000000 mimeograph-0.6.0/src/mimeograph.egg-info/entry_points.txt
+-rw-r--r--   0 tom        (501) staff       (20)      212 2023-05-20 16:31:41.000000 mimeograph-0.6.0/src/mimeograph.egg-info/requires.txt
+-rw-r--r--   0 tom        (501) staff       (20)        6 2023-05-20 16:31:41.000000 mimeograph-0.6.0/src/mimeograph.egg-info/top_level.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-20 16:31:41.901434 mimeograph-0.6.0/tests/
+-rw-r--r--   0 tom        (501) staff       (20)     1828 2023-05-13 05:35:39.000000 mimeograph-0.6.0/tests/test_mimeograph.py
+-rw-r--r--   0 tom        (501) staff       (20)      502 2023-05-20 16:17:22.000000 mimeograph-0.6.0/tests/test_tools.py
```

### Comparing `mimeograph-0.5.0/LICENSE` & `mimeograph-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mimeograph-0.5.0/PKG-INFO` & `mimeograph-0.6.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,7 @@
-Metadata-Version: 2.1
-Name: mimeograph
-Version: 0.5.0
-Summary: Generate data based on a simple template
-Author-email: "T.A. Programming Svcs." <tomasz.maciej.aniolowski@gmail.com>
-License: MIT License
-        
-        Copyright (c) 2023 Tomasz Aniołowski
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: GitHub, https://github.com/TomaszAniolowski/mimeo
-Keywords: mimeograph,mimeo,generate,generator,data,xml
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Database
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Testing
-Classifier: Topic :: Utilities
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: test
-License-File: LICENSE
-
 # Mimeo (Mimeograph)
 
 [![License](https://img.shields.io/github/license/TomaszAniolowski/mimeo?label=License&style=plastic)](https://github.com/TomaszAniolowski/mimeo/blob/develop/LICENSE)
 [![Version](https://img.shields.io/pypi/v/mimeograph?color=blue&label=PyPI&style=plastic)](https://pypi.org/project/mimeograph/)
 [![Python](https://img.shields.io/pypi/pyversions/mimeograph?label=Python&style=plastic)](https://www.python.org/)  
 [![Build](https://img.shields.io/github/actions/workflow/status/TomaszAniolowski/mimeo/test.yml?color=brightgreen&label=Test%20Mimeo&style=plastic)](https://github.com/TomaszAniolowski/mimeo/actions/workflows/test.yml?query=branch%3Amain)
 [![Code Coverage](https://img.shields.io/badge/Code%20Coverage-100%25-brightgreen?style=plastic)](https://github.com/TomaszAniolowski/mimeo/actions/workflows/coverage_badge.yml?query=branch%3Amain)
@@ -236,15 +186,14 @@
 #### Mimeo Environment
 
 To make `http` output directory easier to use, mimeo allows you to configure Mimeo Environments.
 They are configured in a JSON file (by default: mimeo.envs.json) and support the following output details:
 - `protocol`
 - `host`
 - `port`
-- `auth`
 - `username`
 - `password`
 
 Example
 ```json
 {
     "local": {
@@ -253,15 +202,14 @@
         "username": "admin",
         "password": "admin"
     },
     "dev": {
         "protocol": "https",
         "host": "11.111.11.111",
         "port": 8000,
-        "auth": "digest",
         "username": "some-user",
         "password": "some-password"
     }
 }
 ```
 
 To use a specific Mimeo Environment you can use the following commands:
@@ -352,14 +300,18 @@
 
 You can use several predefined functions to generate data. They can be used in a _raw_ format or _parametrized_.
 
 ##### Random String
 
 Generates a random string value.
 
+| Parameter | Supported values | Default |
+|:---------:|:----------------:|:-------:|
+|  length   |      `int`       |  `20`   |
+
 ###### Raw
 
 Uses the default length: 20 characters.
 
 ```json
 {
   "randomstring": "{random_str}"
@@ -381,14 +333,19 @@
 }
 ```
 
 ##### Random Integer
 
 Generates a random integer value between `start` and `limit` parameters (inclusive).
 
+| Parameter | Supported values | Default |
+|:---------:|:----------------:|:-------:|
+|   start   |      `int`       |   `1`   |
+|   limit   |      `int`       |  `100`  |
+
 ###### Raw
 
 Uses the default start (1) and limit (100) values.
 
 ```json
 {
   "randominteger": "{random_int}"
@@ -424,14 +381,18 @@
 ```
 
 ##### Random Item
 
 Generates a random value from items provided.  
 NOTICE: The raw form of this Mimeo Util will generate a blank string value (as same as no items parametrized).
 
+| Parameter | Supported values | Default |
+|:---------:|:----------------:|:-------:|
+|   items   |      `list`      | `[""]`  |
+
 ###### Parametrized
 
 ```json
 {
   "random": {
     "_mimeo_util": {
       "_name": "random_item",
@@ -441,14 +402,18 @@
 }
 ```
 
 ##### Date
 
 Generates a date value in format `YYYY-MM-DD`.
 
+| Parameter  | Supported values | Default |
+|:----------:|:----------------:|:-------:|
+| days_delta |      `int`       |   `0`   |
+
 ###### Raw
 
 Uses the today's date.
 
 ```json
 {
   "Today": "{date}"
@@ -476,14 +441,21 @@
 }
 ```
 
 ##### Date Time
 
 Generates a date time value in format `YYYY-MM-DD'T'HH:mm:SS`.
 
+|   Parameter   | Supported values | Default |
+|:-------------:|:----------------:|:-------:|
+|  days_delta   |      `int`       |   `0`   |
+|  hours_delta  |      `int`       |   `0`   |
+| minutes_delta |      `int`       |   `0`   |
+| seconds_delta |      `int`       |   `0`   |
+
 ###### Raw
 
 Uses the current timestamp.
 
 ```json
 {
   "Now": "{date_time}"
@@ -508,14 +480,18 @@
 }
 ```
 
 ##### Auto Increment
 
 Generates a next integer in context of a model (in nested templates it will use a separated context).
 
+| Parameter | Supported values | Default  |
+|:---------:|:----------------:|:--------:|
+|  pattern  |      `str`       | `{:05d}` |
+
 ###### Raw
 
 Uses a default pattern: **{:05d}** (an integer with 5 leading zeros).
 
 ```json
 {
   "ID": "{auto_increment}"
@@ -537,14 +513,18 @@
 }
 ```
 
 ##### Current Iteration
 
 Generates a value of the current iteration in a Mimeo Template context.
 
+| Parameter | Supported values |      Default      |
+|:---------:|:----------------:|:-----------------:|
+|  context  |      `str`       | a current context |
+
 ###### Raw
 
 Uses the current context.
 
 ```json
 {
   "ID": "{curr_iter}"
@@ -566,14 +546,19 @@
 }
 ```
 
 ##### Key
 
 Generates a key unique across all Mimeo Models and being the same within a single Mimeo Model context.
 
+| Parameter | Supported values |              Default               |
+|:---------:|:----------------:|:----------------------------------:|
+|  context  |      `str`       |         a current context          |
+| iteration |      `int`       | a current iteration of the context |
+
 ###### Raw
 
 Uses a key from the current context and iteration.
 
 ```json
 {
   "ID": "{key}"
@@ -583,28 +568,33 @@
 ###### Parametrized
 
 Uses a key from the specific context and iteration.  
 When context is indicated and iteration is not, then the current iteration **of the indicated context** is being used.
 
 ```json
 {
-  "SomeEntity": {
+  "SomeEntity2": {
     "_mimeo_util": {
       "_name": "key",
       "context": "SomeEntity",
       "iteration": "{curr_iter}"
     }
   }
 }
 ```
 
 ##### City
 
 Generates a city name.
 
+| Parameter | Supported values | Default |
+|:---------:|:----------------:|:-------:|
+|  unique   |      `bool`      | `True`  |
+|  country  |      `str`       | `None`  |
+
 ###### Raw
 
 By default city names will be unique across a Mimeo Context.
 
 ```json
 {
   "City": "{city}"
@@ -651,14 +641,20 @@
 }
 ```
 
 ##### Country
 
 Generates a country name (by default), iso2 or iso3.
 
+| Parameter |       Supported values       | Default  |
+|:---------:|:----------------------------:|:--------:|
+|  unique   |            `bool`            |  `True`  |
+|   value   | `"name"`, `"iso3"`, `"iso2"` | `"name"` |
+|  country  |            `str`             |  `None`  |
+
 ###### Raw
 
 By default country names will be unique across a Mimeo Context.
 
 ```json
 {
   "Country": "{country}"
@@ -708,18 +704,89 @@
       "value": "iso2",
       "country": "United Kingdom"
     }
   }
 }
 ```
 
+##### Currency
+
+Generates a currency code (by default) or name.
+
+| Parameter |  Supported values  | Default  |
+|:---------:|:------------------:|:--------:|
+|  unique   |       `bool`       | `False`  |
+|   value   | `"code"`, `"name"` | `"code"` |
+|  country  |       `str`        |  `None`  |
+
+###### Raw
+
+By default city names will _NOT_ be unique across a Mimeo Context.
+
+```json
+{
+  "Currency": "{currency}"
+}
+```
+
+###### Parametrized
+
+It can generate:
+- unique currencies
+- currency name instead of code
+- currency code or name of a specific country (using iso3, iso2 or name)
+
+When the `country` param is provided then the `unique` flag is ignored.
+
+```json
+{
+  "UniqueCurrencyCode": {
+    "_mimeo_util": {
+      "_name": "currency",
+      "unique": true
+    }
+  },
+  "CurrencyName": {
+    "_mimeo_util": {
+      "_name": "currency",
+      "value": "name"
+    }
+  },
+  "CurrencyCodeForCountryISO3": {
+    "_mimeo_util": {
+      "_name": "currency",
+      "country": "GBR"
+    }
+  },
+  "CurrencyNameForCountryISO2": {
+    "_mimeo_util": {
+      "_name": "currency",
+      "value": "name",
+      "country": "GB"
+    }
+  },
+  "CurrencyNameForCountryName": {
+    "_mimeo_util": {
+      "_name": "currency",
+      "value": "name",
+      "country": "United Kingdom"
+    }
+  }
+}
+```
+
 ##### First Name
 
 Generates a first name.
 
+| Parameter |      Supported values      | Default  |
+|:---------:|:--------------------------:|:--------:|
+|  unique   |           `bool`           |  `True`  |
+|    sex    | `M`, `Male`, `F`, `Female` |  `None`  |
+
 ###### Raw
 
 By default first names will be unique across a Mimeo Context.
 
 ```json
 {
   "FirstName": "{first_name}"
@@ -760,14 +827,18 @@
 }
 ```
 
 ##### Last Name
 
 Generates a last name.
 
+| Parameter | Supported values | Default  |
+|:---------:|:----------------:|:--------:|
+|  unique   |      `bool`      |  `True`  |
+
 ###### Raw
 
 By default last names will be unique across a Mimeo Context.
 
 ```json
 {
   "LastName": "{last_name}"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mimeograph-0.5.0/README.md` & `mimeograph-0.6.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,57 @@
+Metadata-Version: 2.1
+Name: mimeograph
+Version: 0.6.0
+Summary: Generate data based on a simple template
+Author-email: "T.A. Programming Svcs." <tomasz.maciej.aniolowski@gmail.com>
+License: MIT License
+        
+        Copyright (c) 2023 Tomasz Aniołowski
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: GitHub, https://github.com/TomaszAniolowski/mimeo
+Keywords: mimeograph,mimeo,generate,generator,data,xml
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Database
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: Utilities
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: test
+License-File: LICENSE
+
 # Mimeo (Mimeograph)
 
 [![License](https://img.shields.io/github/license/TomaszAniolowski/mimeo?label=License&style=plastic)](https://github.com/TomaszAniolowski/mimeo/blob/develop/LICENSE)
 [![Version](https://img.shields.io/pypi/v/mimeograph?color=blue&label=PyPI&style=plastic)](https://pypi.org/project/mimeograph/)
 [![Python](https://img.shields.io/pypi/pyversions/mimeograph?label=Python&style=plastic)](https://www.python.org/)  
 [![Build](https://img.shields.io/github/actions/workflow/status/TomaszAniolowski/mimeo/test.yml?color=brightgreen&label=Test%20Mimeo&style=plastic)](https://github.com/TomaszAniolowski/mimeo/actions/workflows/test.yml?query=branch%3Amain)
 [![Code Coverage](https://img.shields.io/badge/Code%20Coverage-100%25-brightgreen?style=plastic)](https://github.com/TomaszAniolowski/mimeo/actions/workflows/coverage_badge.yml?query=branch%3Amain)
@@ -186,15 +236,14 @@
 #### Mimeo Environment
 
 To make `http` output directory easier to use, mimeo allows you to configure Mimeo Environments.
 They are configured in a JSON file (by default: mimeo.envs.json) and support the following output details:
 - `protocol`
 - `host`
 - `port`
-- `auth`
 - `username`
 - `password`
 
 Example
 ```json
 {
     "local": {
@@ -203,15 +252,14 @@
         "username": "admin",
         "password": "admin"
     },
     "dev": {
         "protocol": "https",
         "host": "11.111.11.111",
         "port": 8000,
-        "auth": "digest",
         "username": "some-user",
         "password": "some-password"
     }
 }
 ```
 
 To use a specific Mimeo Environment you can use the following commands:
@@ -302,14 +350,18 @@
 
 You can use several predefined functions to generate data. They can be used in a _raw_ format or _parametrized_.
 
 ##### Random String
 
 Generates a random string value.
 
+| Parameter | Supported values | Default |
+|:---------:|:----------------:|:-------:|
+|  length   |      `int`       |  `20`   |
+
 ###### Raw
 
 Uses the default length: 20 characters.
 
 ```json
 {
   "randomstring": "{random_str}"
@@ -331,14 +383,19 @@
 }
 ```
 
 ##### Random Integer
 
 Generates a random integer value between `start` and `limit` parameters (inclusive).
 
+| Parameter | Supported values | Default |
+|:---------:|:----------------:|:-------:|
+|   start   |      `int`       |   `1`   |
+|   limit   |      `int`       |  `100`  |
+
 ###### Raw
 
 Uses the default start (1) and limit (100) values.
 
 ```json
 {
   "randominteger": "{random_int}"
@@ -374,14 +431,18 @@
 ```
 
 ##### Random Item
 
 Generates a random value from items provided.  
 NOTICE: The raw form of this Mimeo Util will generate a blank string value (as same as no items parametrized).
 
+| Parameter | Supported values | Default |
+|:---------:|:----------------:|:-------:|
+|   items   |      `list`      | `[""]`  |
+
 ###### Parametrized
 
 ```json
 {
   "random": {
     "_mimeo_util": {
       "_name": "random_item",
@@ -391,14 +452,18 @@
 }
 ```
 
 ##### Date
 
 Generates a date value in format `YYYY-MM-DD`.
 
+| Parameter  | Supported values | Default |
+|:----------:|:----------------:|:-------:|
+| days_delta |      `int`       |   `0`   |
+
 ###### Raw
 
 Uses the today's date.
 
 ```json
 {
   "Today": "{date}"
@@ -426,14 +491,21 @@
 }
 ```
 
 ##### Date Time
 
 Generates a date time value in format `YYYY-MM-DD'T'HH:mm:SS`.
 
+|   Parameter   | Supported values | Default |
+|:-------------:|:----------------:|:-------:|
+|  days_delta   |      `int`       |   `0`   |
+|  hours_delta  |      `int`       |   `0`   |
+| minutes_delta |      `int`       |   `0`   |
+| seconds_delta |      `int`       |   `0`   |
+
 ###### Raw
 
 Uses the current timestamp.
 
 ```json
 {
   "Now": "{date_time}"
@@ -458,14 +530,18 @@
 }
 ```
 
 ##### Auto Increment
 
 Generates a next integer in context of a model (in nested templates it will use a separated context).
 
+| Parameter | Supported values | Default  |
+|:---------:|:----------------:|:--------:|
+|  pattern  |      `str`       | `{:05d}` |
+
 ###### Raw
 
 Uses a default pattern: **{:05d}** (an integer with 5 leading zeros).
 
 ```json
 {
   "ID": "{auto_increment}"
@@ -487,14 +563,18 @@
 }
 ```
 
 ##### Current Iteration
 
 Generates a value of the current iteration in a Mimeo Template context.
 
+| Parameter | Supported values |      Default      |
+|:---------:|:----------------:|:-----------------:|
+|  context  |      `str`       | a current context |
+
 ###### Raw
 
 Uses the current context.
 
 ```json
 {
   "ID": "{curr_iter}"
@@ -516,14 +596,19 @@
 }
 ```
 
 ##### Key
 
 Generates a key unique across all Mimeo Models and being the same within a single Mimeo Model context.
 
+| Parameter | Supported values |              Default               |
+|:---------:|:----------------:|:----------------------------------:|
+|  context  |      `str`       |         a current context          |
+| iteration |      `int`       | a current iteration of the context |
+
 ###### Raw
 
 Uses a key from the current context and iteration.
 
 ```json
 {
   "ID": "{key}"
@@ -533,28 +618,33 @@
 ###### Parametrized
 
 Uses a key from the specific context and iteration.  
 When context is indicated and iteration is not, then the current iteration **of the indicated context** is being used.
 
 ```json
 {
-  "SomeEntity": {
+  "SomeEntity2": {
     "_mimeo_util": {
       "_name": "key",
       "context": "SomeEntity",
       "iteration": "{curr_iter}"
     }
   }
 }
 ```
 
 ##### City
 
 Generates a city name.
 
+| Parameter | Supported values | Default |
+|:---------:|:----------------:|:-------:|
+|  unique   |      `bool`      | `True`  |
+|  country  |      `str`       | `None`  |
+
 ###### Raw
 
 By default city names will be unique across a Mimeo Context.
 
 ```json
 {
   "City": "{city}"
@@ -601,14 +691,20 @@
 }
 ```
 
 ##### Country
 
 Generates a country name (by default), iso2 or iso3.
 
+| Parameter |       Supported values       | Default  |
+|:---------:|:----------------------------:|:--------:|
+|  unique   |            `bool`            |  `True`  |
+|   value   | `"name"`, `"iso3"`, `"iso2"` | `"name"` |
+|  country  |            `str`             |  `None`  |
+
 ###### Raw
 
 By default country names will be unique across a Mimeo Context.
 
 ```json
 {
   "Country": "{country}"
@@ -658,18 +754,89 @@
       "value": "iso2",
       "country": "United Kingdom"
     }
   }
 }
 ```
 
+##### Currency
+
+Generates a currency code (by default) or name.
+
+| Parameter |  Supported values  | Default  |
+|:---------:|:------------------:|:--------:|
+|  unique   |       `bool`       | `False`  |
+|   value   | `"code"`, `"name"` | `"code"` |
+|  country  |       `str`        |  `None`  |
+
+###### Raw
+
+By default city names will _NOT_ be unique across a Mimeo Context.
+
+```json
+{
+  "Currency": "{currency}"
+}
+```
+
+###### Parametrized
+
+It can generate:
+- unique currencies
+- currency name instead of code
+- currency code or name of a specific country (using iso3, iso2 or name)
+
+When the `country` param is provided then the `unique` flag is ignored.
+
+```json
+{
+  "UniqueCurrencyCode": {
+    "_mimeo_util": {
+      "_name": "currency",
+      "unique": true
+    }
+  },
+  "CurrencyName": {
+    "_mimeo_util": {
+      "_name": "currency",
+      "value": "name"
+    }
+  },
+  "CurrencyCodeForCountryISO3": {
+    "_mimeo_util": {
+      "_name": "currency",
+      "country": "GBR"
+    }
+  },
+  "CurrencyNameForCountryISO2": {
+    "_mimeo_util": {
+      "_name": "currency",
+      "value": "name",
+      "country": "GB"
+    }
+  },
+  "CurrencyNameForCountryName": {
+    "_mimeo_util": {
+      "_name": "currency",
+      "value": "name",
+      "country": "United Kingdom"
+    }
+  }
+}
+```
+
 ##### First Name
 
 Generates a first name.
 
+| Parameter |      Supported values      | Default  |
+|:---------:|:--------------------------:|:--------:|
+|  unique   |           `bool`           |  `True`  |
+|    sex    | `M`, `Male`, `F`, `Female` |  `None`  |
+
 ###### Raw
 
 By default first names will be unique across a Mimeo Context.
 
 ```json
 {
   "FirstName": "{first_name}"
@@ -710,14 +877,18 @@
 }
 ```
 
 ##### Last Name
 
 Generates a last name.
 
+| Parameter | Supported values | Default  |
+|:---------:|:----------------:|:--------:|
+|  unique   |      `bool`      |  `True`  |
+
 ###### Raw
 
 By default last names will be unique across a Mimeo Context.
 
 ```json
 {
   "LastName": "{last_name}"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mimeograph-0.5.0/pyproject.toml` & `mimeograph-0.6.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mimeograph"
-version = "0.5.0"
+version = "0.6.0"
 description = "Generate data based on a simple template"
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [{ name = "T.A. Programming Svcs.", email = "tomasz.maciej.aniolowski@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
@@ -60,19 +60,19 @@
     "pytest-asyncio"
 ]
 
 [project.scripts]
 mimeo = "mimeo.__main__:main"
 
 [tool.bumpver]
-current_version = "0.5.0"
+current_version = "0.6.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} to {new_version}"
 commit          = true
-tag             = true
+tag             = false
 push            = false
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = ['current_version = "{version}"', 'version = "{version}"']
 "src/mimeo/__init__.py" = ["{version}"]
 "src/mimeo/cli/parsers.py" = ["{version}"]
 
@@ -95,15 +95,18 @@
     "src/mimeo/cli/__init__.py",
     "src/mimeo/consumers/__init__.py",
     "src/mimeo/context/__init__.py",
     "src/mimeo/generators/__init__.py"
 ]
 
 [tool.ruff]
-select = ["F", "E", "W", "C90", "N", "D", "UP", "B", "A", "COM", "C4", "EM", "EXE", "ISC", "G", "PIE", "T20", "PT", "Q", "RSE", "RET", "SLF", "SIM", "ARG", "PTH", "ERA", "PD", "PGH", "PL", "TRY", "RUF"]
+select = [
+    "F", "E", "W", "C90", "N", "D", "UP", "B", "A", "COM", "C4", "EM", "EXE", "ISC", "G", "PIE", "T20",
+    "PT", "Q", "RSE", "RET", "SLF", "SIM", "ARG", "PTH", "ERA", "PD", "PGH", "PL", "TRY", "RUF", "FLY"
+]
 ignore = []
 exclude = [
     ".git",
     ".github",
     ".idea",
     ".pytest_cache",
     ".ruff_cache",
@@ -125,14 +128,15 @@
 
 [tool.ruff.per-file-ignores]
 "scripts/*" = [
     "T20" # allow for print in scripts
 ]
 "tests/*" = [
     "D", # disable pydocstyle for tests
+    "EM101", # allow string literals in exceptions' tests
     "PLC1901", # allow comparison to blank string in tests
     "PLR2004" # allow magic values in tests
 ]
 "src/mimeo/consumers/raw_consumer.py" = [
     "T20" # allow for print in raw consumer
 ]
 "src/mimeo/logging/filters.py" = [
```

### Comparing `mimeograph-0.5.0/src/mimeo/__init__.py` & `mimeograph-0.6.0/src/mimeo/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,9 +44,9 @@
     from mimeo import MimeoConfig, Mimeograph
 """
 from __future__ import annotations
 
 from .config import MimeoConfig
 from .mimeo import Mimeograph
 
-__version__ = "0.5.0"
+__version__ = "0.6.0"
 __all__ = ["MimeoConfig", "Mimeograph"]
```

### Comparing `mimeograph-0.5.0/src/mimeo/cli/__init__.py` & `mimeograph-0.6.0/src/mimeo/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.5.0/src/mimeo/cli/exc.py` & `mimeograph-0.6.0/src/mimeo/cli/exc.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,45 @@
 """The Mimeo CLI Exceptions module.
 
 It contains all custom exceptions related to Mimeo CLI:
+    * PathNotFoundError
+        A custom Exception class for not found path.
     * EnvironmentNotFoundError
         A custom Exception class for not found environment.
     * EnvironmentsFileNotFoundError
         A custom Exception class for not found environments file.
 """
 
 
 from __future__ import annotations
 
 
+class PathNotFoundError(Exception):
+    """A custom Exception class for not found path.
+
+    Raised while attempting to access a Mimeo Config file or directory that doesn't
+    exist.
+    """
+
+    def __init__(
+            self,
+            path: str,
+    ):
+        """Initialize PathNotFoundError exception with details.
+
+        Extends Exception constructor with a custom message.
+
+        Parameters
+        ----------
+        path : str
+            A non existing path
+        """
+        super().__init__(f"No such file or directory [{path}]")
+
+
 class EnvironmentNotFoundError(Exception):
     """A custom Exception class for not found environment.
 
     Raised while attempting to access an environment that does not exist.
     """
 
     def __init__(
```

### Comparing `mimeograph-0.5.0/src/mimeo/cli/job.py` & `mimeograph-0.6.0/src/mimeo/cli/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import logging
 from argparse import Namespace
 from os import walk
 from pathlib import Path
 
 from mimeo import MimeoConfig, Mimeograph
 from mimeo.cli import MimeoArgumentParser, MimeoConfigParser
+from mimeo.cli.exc import PathNotFoundError
 
 logger = logging.getLogger(__name__)
 
 
 class MimeoJob:
     """A class representing a single Mimeo processing job.
 
@@ -90,17 +91,19 @@
             A list of file paths
         """
         file_paths = []
         for file_path in paths:
             if Path(file_path).is_dir():
                 for dir_path, _, file_names in walk(file_path):
                     for file_name in file_names:
-                        file_paths.append(f"{dir_path}/{file_name}")
+                        file_paths.append(Path(f"{dir_path}/{file_name}"))
             elif Path(file_path).is_file():
-                file_paths.append(file_path)
+                file_paths.append(Path(file_path))
+            else:
+                raise PathNotFoundError(file_path)
         return file_paths
 
     @classmethod
     def _get_mimeo_config(
             cls,
             config_path: str,
             args: Namespace,
```

### Comparing `mimeograph-0.5.0/src/mimeo/cli/parsers.py` & `mimeograph-0.6.0/src/mimeo/cli/parsers.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import logging
 from argparse import ArgumentParser, Namespace
 from pathlib import Path
 
 from mimeo import MimeoConfig
 from mimeo.cli.exc import (EnvironmentNotFoundError,
                            EnvironmentsFileNotFoundError)
+from mimeo.config import constants as cc
 
 logger = logging.getLogger(__name__)
 
 DEFAULT_ENVS_PATH = "mimeo.envs.json"
 
 
 class MimeoArgumentParser(ArgumentParser):
@@ -95,15 +96,15 @@
             self,
     ):
         """Add positional arguments."""
         self.add_argument(
             "-v",
             "--version",
             action="version",
-            version="%(prog)s v0.5.0")
+            version="%(prog)s v0.6.0")
         self.add_argument(
             "paths",
             nargs="+",
             type=str,
             help="take paths to Mimeo Configuration files")
 
     def _add_mimeo_configuration_arguments(
@@ -217,71 +218,59 @@
 
     Methods
     -------
     parse_config() -> MimeoConfig
         Parse a Mimeo Configuration using Mimeo arguments.
     """
 
-    _ENVIRONMENT_PROPS = [MimeoConfig.OUTPUT_PROTOCOL_KEY,
-                          MimeoConfig.OUTPUT_HOST_KEY,
-                          MimeoConfig.OUTPUT_PORT_KEY,
-                          MimeoConfig.OUTPUT_USERNAME_KEY,
-                          MimeoConfig.OUTPUT_PASSWORD_KEY]
+    _ENVIRONMENT_PROPS = [cc.OUTPUT_PROTOCOL_KEY,
+                          cc.OUTPUT_HOST_KEY,
+                          cc.OUTPUT_PORT_KEY,
+                          cc.OUTPUT_USERNAME_KEY,
+                          cc.OUTPUT_PASSWORD_KEY]
 
     _ENTRY_PATH_KEY = "entry_path"
     _GET_VALUE_KEY = "get_value"
     _ARGS_MAPPING = {
         "output": {
-            "entry_path": [MimeoConfig.OUTPUT_KEY,
-                           MimeoConfig.OUTPUT_DIRECTION_KEY],
+            "entry_path": [cc.OUTPUT_KEY, cc.OUTPUT_DIRECTION_KEY],
         },
         "xml_declaration": {
-            "entry_path": [MimeoConfig.OUTPUT_KEY,
-                           MimeoConfig.OUTPUT_XML_DECLARATION_KEY],
+            "entry_path": [cc.OUTPUT_KEY, cc.OUTPUT_XML_DECLARATION_KEY],
             "get_value": lambda arg: arg.lower() == "true",
         },
         "indent": {
-            "entry_path": [MimeoConfig.OUTPUT_KEY,
-                           MimeoConfig.OUTPUT_INDENT_KEY],
+            "entry_path": [cc.OUTPUT_KEY, cc.OUTPUT_INDENT_KEY],
         },
         "directory": {
-            "entry_path": [MimeoConfig.OUTPUT_KEY,
-                           MimeoConfig.OUTPUT_DIRECTORY_PATH_KEY],
+            "entry_path": [cc.OUTPUT_KEY, cc.OUTPUT_DIRECTORY_PATH_KEY],
         },
         "file": {
-            "entry_path": [MimeoConfig.OUTPUT_KEY,
-                           MimeoConfig.OUTPUT_FILE_NAME_KEY],
+            "entry_path": [cc.OUTPUT_KEY, cc.OUTPUT_FILE_NAME_KEY],
         },
         "http_method": {
-            "entry_path": [MimeoConfig.OUTPUT_KEY,
-                           MimeoConfig.OUTPUT_METHOD_KEY],
+            "entry_path": [cc.OUTPUT_KEY, cc.OUTPUT_METHOD_KEY],
         },
         "http_protocol": {
-            "entry_path": [MimeoConfig.OUTPUT_KEY,
-                           MimeoConfig.OUTPUT_PROTOCOL_KEY],
+            "entry_path": [cc.OUTPUT_KEY, cc.OUTPUT_PROTOCOL_KEY],
         },
         "http_host": {
-            "entry_path": [MimeoConfig.OUTPUT_KEY,
-                           MimeoConfig.OUTPUT_HOST_KEY],
+            "entry_path": [cc.OUTPUT_KEY, cc.OUTPUT_HOST_KEY],
         },
         "http_port": {
-            "entry_path": [MimeoConfig.OUTPUT_KEY,
-                           MimeoConfig.OUTPUT_PORT_KEY],
+            "entry_path": [cc.OUTPUT_KEY, cc.OUTPUT_PORT_KEY],
         },
         "http_endpoint": {
-            "entry_path": [MimeoConfig.OUTPUT_KEY,
-                           MimeoConfig.OUTPUT_ENDPOINT_KEY],
+            "entry_path": [cc.OUTPUT_KEY, cc.OUTPUT_ENDPOINT_KEY],
         },
         "http_user": {
-            "entry_path": [MimeoConfig.OUTPUT_KEY,
-                           MimeoConfig.OUTPUT_USERNAME_KEY],
+            "entry_path": [cc.OUTPUT_KEY, cc.OUTPUT_USERNAME_KEY],
         },
         "http_password": {
-            "entry_path": [MimeoConfig.OUTPUT_KEY,
-                           MimeoConfig.OUTPUT_PASSWORD_KEY],
+            "entry_path": [cc.OUTPUT_KEY, cc.OUTPUT_PASSWORD_KEY],
         },
     }
 
     def __init__(
             self,
             config: dict,
             args: Namespace,
@@ -416,15 +405,15 @@
         -------
         config : dict
             An overwritten Mimeo Configuration.
         """
         for prop in cls._ENVIRONMENT_PROPS:
             value = env.get(prop)
             if value is not None:
-                config_entry_path = [MimeoConfig.OUTPUT_KEY, prop]
+                config_entry_path = [cc.OUTPUT_KEY, prop]
                 config = cls._overwrite_config_entry(config, config_entry_path, value)
         return config
 
     @classmethod
     def _overwrite_config_entry(
             cls,
             config_entry: dict,
```

### Comparing `mimeograph-0.5.0/src/mimeo/config/__init__.py` & `mimeograph-0.6.0/src/mimeo/config/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 """The Mimeo Configuration package.
 
 It contains the following modules:
 * mimeo_config
     The Mimeo Configuration module
+* constants
+    The Mimeo Configuration Constants module
 * exc
     The Mimeo Configuration Exceptions module
 
 The Mimeo Configuration package exports a class representing
 root Mimeo Configuration component:
 * MimeoConfig
     A MimeoDTO class representing Mimeo Configuration
 
 To use this package, simply import it:
     from mimeo.config import MimeoConfig
+    from mimeo.config import constants as cc
     from mimeo.config.exc import UnsupportedPropertyValueError
 """
 from __future__ import annotations
 
 from .mimeo_config import MimeoConfig
 
 __all__ = ["MimeoConfig"]
```

### Comparing `mimeograph-0.5.0/src/mimeo/config/mimeo_config.py` & `mimeograph-0.6.0/src/mimeo/config/mimeo_config.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     * MimeoModel
         A MimeoDTO class representing Mimeo Model
 """
 from __future__ import annotations
 
 import re
 
+from mimeo.config import constants as cc
 from mimeo.config.exc import (InvalidIndentError, InvalidMimeoConfigError,
                               InvalidMimeoModelError,
                               InvalidMimeoTemplateError, InvalidVarsError,
                               MissingRequiredPropertyError,
                               UnsupportedPropertyValueError)
 from mimeo.logging import setup_logging
 
@@ -59,149 +60,37 @@
 
 
 class MimeoConfig(MimeoDTO):
     """A MimeoDTO class representing Mimeo Configuration.
 
     It is a python representation of a Mimeo Configuration file / dictionary.
 
-    Attributes
-    ----------
-    OUTPUT_KEY : str
-        A Mimeo Configuration output details key
-    OUTPUT_DIRECTION_KEY : str
-        A Mimeo Configuration output direction key
-    OUTPUT_FORMAT_KEY : str
-        A Mimeo Configuration output format key
-    OUTPUT_XML_DECLARATION_KEY : str
-        A Mimeo Configuration xml declaration key
-    OUTPUT_INDENT_KEY : str
-        A Mimeo Configuration indent key
-    OUTPUT_DIRECTORY_PATH_KEY : str
-        A Mimeo Configuration output directory path key
-    OUTPUT_FILE_NAME_KEY : str
-        A Mimeo Configuration output file name key
-    OUTPUT_METHOD_KEY : str
-        A Mimeo Configuration http method key
-    OUTPUT_PROTOCOL_KEY : str
-        A Mimeo Configuration http protocol key
-    OUTPUT_HOST_KEY : str
-        A Mimeo Configuration http host key
-    OUTPUT_PORT_KEY : str
-        A Mimeo Configuration http port key
-    OUTPUT_ENDPOINT_KEY : str
-        A Mimeo Configuration http endpoint key
-    OUTPUT_USERNAME_KEY : str
-        A Mimeo Configuration http username key
-    OUTPUT_PASSWORD_KEY : str
-        A Mimeo Configuration http password key
-    VARS_KEY : str
-        A Mimeo Configuration vars key
-    TEMPLATES_KEY : str
-        A Mimeo Configuration templates key
-    TEMPLATES_COUNT_KEY : str
-        A Mimeo Configuration template's count key
-    TEMPLATES_MODEL_KEY : str
-        A Mimeo Configuration template's model key
-    MODEL_CONTEXT_KEY : str
-        A Mimeo Configuration model's context name key
-    MODEL_ATTRIBUTES_KEY : str
-        A Mimeo Configuration attributes key (for nodes' attributes)
-    MODEL_VALUE_KEY : str
-        A Mimeo Configuration value key (for nodes' value)
-    MODEL_MIMEO_UTIL_KEY : str
-        A Mimeo Configuration Mimeo Util key
-    MODEL_MIMEO_UTIL_NAME_KEY : str
-        A Mimeo Configuration Mimeo Util's name key
-    SUPPORTED_OUTPUT_FORMATS : set
-        A set of supported output formats
-    OUTPUT_DIRECTION_FILE : str
-        The 'file' output direction
-    OUTPUT_DIRECTION_STD_OUT : str
-        The 'stdout' output direction
-    OUTPUT_DIRECTION_HTTP : str
-        The 'http' output direction
-    OUTPUT_DIRECTION_HTTP_REQUEST_POST : str
-        The 'POST' http request method
-    OUTPUT_DIRECTION_HTTP_REQUEST_PUT : str
-        The 'PUT' http request method
-    SUPPORTED_OUTPUT_DIRECTIONS : set
-        List of supported output directions
-    SUPPORTED_REQUEST_METHODS : set
-        List of supported http request methods
-    REQUIRED_HTTP_DETAILS : set
-        List of required http request output direction details
-
     output : MimeoOutput, default {}
         A Mimeo Output Details settings
     vars : dict, default {}
         A Mimeo Configuration vars setting
     templates : list
         A Mimeo Templates setting
     """
 
-    OUTPUT_KEY = "output"
-    OUTPUT_DIRECTION_KEY = "direction"
-    OUTPUT_FORMAT_KEY = "format"
-    OUTPUT_XML_DECLARATION_KEY = "xml_declaration"
-    OUTPUT_INDENT_KEY = "indent"
-    OUTPUT_DIRECTORY_PATH_KEY = "directory_path"
-    OUTPUT_FILE_NAME_KEY = "file_name"
-    OUTPUT_METHOD_KEY = "method"
-    OUTPUT_PROTOCOL_KEY = "protocol"
-    OUTPUT_HOST_KEY = "host"
-    OUTPUT_PORT_KEY = "port"
-    OUTPUT_ENDPOINT_KEY = "endpoint"
-    OUTPUT_USERNAME_KEY = "username"
-    OUTPUT_PASSWORD_KEY = "password"
-    VARS_KEY = "vars"
-    TEMPLATES_KEY = "_templates_"
-    TEMPLATES_COUNT_KEY = "count"
-    TEMPLATES_MODEL_KEY = "model"
-    MODEL_CONTEXT_KEY = "context"
-    MODEL_ATTRIBUTES_KEY = "_attrs"
-    MODEL_VALUE_KEY = "_value"
-    MODEL_MIMEO_UTIL_KEY = "_mimeo_util"
-    MODEL_MIMEO_UTIL_NAME_KEY = "_name"
-
-    OUTPUT_FORMAT_XML = "xml"
-
-    OUTPUT_DIRECTION_FILE = "file"
-    OUTPUT_DIRECTION_STD_OUT = "stdout"
-    OUTPUT_DIRECTION_HTTP = "http"
-
-    OUTPUT_DIRECTION_HTTP_REQUEST_POST = "POST"
-    OUTPUT_DIRECTION_HTTP_REQUEST_PUT = "PUT"
-
-    SUPPORTED_OUTPUT_FORMATS = (OUTPUT_FORMAT_XML,)
-
-    SUPPORTED_OUTPUT_DIRECTIONS = (OUTPUT_DIRECTION_STD_OUT,
-                                   OUTPUT_DIRECTION_FILE,
-                                   OUTPUT_DIRECTION_HTTP)
-    SUPPORTED_REQUEST_METHODS = (OUTPUT_DIRECTION_HTTP_REQUEST_POST,
-                                 OUTPUT_DIRECTION_HTTP_REQUEST_PUT)
-    REQUIRED_HTTP_DETAILS = (OUTPUT_HOST_KEY,
-                             OUTPUT_ENDPOINT_KEY,
-                             OUTPUT_USERNAME_KEY,
-                             OUTPUT_PASSWORD_KEY)
-
     def __init__(
             self,
             config: dict,
     ):
         """Initialize MimeoConfig class.
 
         Extends MimeoDTO constructor.
 
         Parameters
         ----------
         config : dict
             A source config dictionary
         """
         super().__init__(config)
-        self.output = MimeoOutput(config.get(self.OUTPUT_KEY, {}))
+        self.output = MimeoOutput(config.get(cc.OUTPUT_KEY, {}))
         self.vars = self._get_vars(config)
         self.templates = self._get_templates(config)
 
     @classmethod
     def _get_vars(
             cls,
             config: dict,
@@ -222,28 +111,22 @@
         ------
         InvalidVarsError
             If (1) the vars key does not point to a dictionary or
             (2) some variable's name does not start with a letter,
             is not SNAKE_UPPER_CASE with possible digits or
             (3) some variable's value points to non-atomic value nor Mimeo Util
         """
-        variables = config.get(MimeoConfig.VARS_KEY, {})
+        variables = config.get(cc.VARS_KEY, {})
         if not isinstance(variables, dict):
-            msg = f"vars property does not store an object: {variables}"
-            raise InvalidVarsError(msg)
+            raise InvalidVarsError(InvalidVarsError.Code.ERR_1, vars=variables)
         for var, val in variables.items():
-            if not re.match(r"^[A-Z][A-Z_0-9]*$", var):
-                msg = (f"Provided var [{var}] is invalid "
-                       f"(you can use upper-cased name with underscore and digits, "
-                       f"starting with a letter)!")
-                raise InvalidVarsError(msg)
             if isinstance(val, (list, dict)) and not cls._is_mimeo_util_object(val):
-                msg = (f"Provided var [{var}] is invalid "
-                       f"(you can use ony atomic values and Mimeo Utils)!")
-                raise InvalidVarsError(msg)
+                raise InvalidVarsError(InvalidVarsError.Code.ERR_2, var=var)
+            if not re.match(r"^[A-Z][A-Z_0-9]*$", var):
+                raise InvalidVarsError(InvalidVarsError.Code.ERR_3, var=var)
         return variables
 
     @classmethod
     def _get_templates(
             cls,
             config: dict,
     ) -> list:
@@ -257,27 +140,27 @@
         Returns
         -------
         list
             A Mimeo Templates list
 
         Raises
         ------
-        IncorrectMimeoConfig
+        InvalidMimeoConfigError
             If (1) the source dictionary does not include the _templates_ key or
             (2) the _templates_ key does not point to a list
         """
-        templates = config.get(cls.TEMPLATES_KEY)
+        templates = config.get(cc.TEMPLATES_KEY)
         if templates is None:
-            msg = f"No templates in the Mimeo Config: {config}"
-            raise InvalidMimeoConfigError(msg)
+            raise InvalidMimeoConfigError(InvalidMimeoConfigError.Code.ERR_1,
+                                          config=config)
         if not isinstance(templates, list):
-            msg = f"_templates_ property does not store an array: {config}"
-            raise InvalidMimeoConfigError(msg)
+            raise InvalidMimeoConfigError(InvalidMimeoConfigError.Code.ERR_2,
+                                          config=config)
         return [MimeoTemplate(template)
-                for template in config.get(cls.TEMPLATES_KEY)]
+                for template in config.get(cc.TEMPLATES_KEY)]
 
     @classmethod
     def _is_mimeo_util_object(
             cls,
             obj: dict,
     ) -> bool:
         """Verify if the object is a Mimeo Util.
@@ -291,15 +174,15 @@
         -------
         bool
             True if the object is a dictionary having only one key: _mimeo_util.
             Otherwise, False.
         """
         return (isinstance(obj, dict) and
                 len(obj) == 1 and
-                cls.MODEL_MIMEO_UTIL_KEY in obj)
+                cc.MODEL_MIMEO_UTIL_KEY in obj)
 
 
 class MimeoOutput(MimeoDTO):
     """A MimeoDTO class representing Mimeo Output Details.
 
     It is a python representation of a Mimeo Output Details configuration node.
 
@@ -323,16 +206,14 @@
         The configured http output protocol
     host : str
         The configured http output host
     port : str
         The configured http output port
     endpoint : str
         The configured http output endpoint
-    auth : str, default 'basic'
-        The configured http output auth method
     username : str
         The configured http output username
     password : str
         The configured http output password
     """
 
     def __init__(
@@ -348,15 +229,15 @@
         output : dict
             A source config output details dictionary
         """
         super().__init__(output)
         self.direction = self._get_direction(output)
         self._validate_output(self.direction, output)
         self.format = self._get_format(output)
-        self.xml_declaration = output.get(MimeoConfig.OUTPUT_XML_DECLARATION_KEY, False)
+        self.xml_declaration = output.get(cc.OUTPUT_XML_DECLARATION_KEY, False)
         self.indent = self._get_indent(output)
         self.directory_path = self._get_directory_path(self.direction, output)
         self.file_name = self._get_file_name(self.direction, output, self.format)
         self.method = self._get_method(self.direction, output)
         self.protocol = self._get_protocol(self.direction, output)
         self.host = self._get_host(self.direction, output)
         self.port = self._get_port(self.direction, output)
@@ -381,22 +262,20 @@
             The configured output direction
 
         Raises
         ------
         UnsupportedPropertyValueError
             If the configured output direction is not supported
         """
-        direction = output.get(
-            MimeoConfig.OUTPUT_DIRECTION_KEY,
-            MimeoConfig.OUTPUT_DIRECTION_FILE)
-        if direction not in MimeoConfig.SUPPORTED_OUTPUT_DIRECTIONS:
+        direction = output.get(cc.OUTPUT_DIRECTION_KEY, cc.OUTPUT_DIRECTION_FILE)
+        if direction not in cc.SUPPORTED_OUTPUT_DIRECTIONS:
             raise UnsupportedPropertyValueError(
-                MimeoConfig.OUTPUT_DIRECTION_KEY,
+                cc.OUTPUT_DIRECTION_KEY,
                 direction,
-                MimeoConfig.SUPPORTED_OUTPUT_DIRECTIONS)
+                cc.SUPPORTED_OUTPUT_DIRECTIONS)
         return direction
 
     @staticmethod
     def _get_format(
             config: dict,
     ) -> str:
         """Extract an output format from the source dictionary.
@@ -412,22 +291,20 @@
             The customized output format or 'xml' by default
 
         Raises
         ------
         UnsupportedPropertyValueError
             If the customized output format is not supported
         """
-        output_format = config.get(
-            MimeoConfig.OUTPUT_FORMAT_KEY,
-            MimeoConfig.OUTPUT_FORMAT_XML)
-        if output_format not in MimeoConfig.SUPPORTED_OUTPUT_FORMATS:
+        output_format = config.get(cc.OUTPUT_FORMAT_KEY, cc.OUTPUT_FORMAT_XML)
+        if output_format not in cc.SUPPORTED_OUTPUT_FORMATS:
             raise UnsupportedPropertyValueError(
-                MimeoConfig.OUTPUT_FORMAT_KEY,
+                cc.OUTPUT_FORMAT_KEY,
                 output_format,
-                MimeoConfig.SUPPORTED_OUTPUT_FORMATS)
+                cc.SUPPORTED_OUTPUT_FORMATS)
         return output_format
 
     @staticmethod
     def _get_indent(
             config: dict,
     ) -> int:
         """Extract an indent value from the source dictionary.
@@ -443,15 +320,15 @@
             The customized indent or 0 by default
 
         Raises
         ------
         InvalidIndentError
             If the customized indent is lower than zero
         """
-        indent = config.get(MimeoConfig.OUTPUT_INDENT_KEY, 0)
+        indent = config.get(cc.OUTPUT_INDENT_KEY, 0)
         if indent < 0:
             raise InvalidIndentError(indent)
         return indent
 
     @staticmethod
     def _get_directory_path(
             direction: str,
@@ -471,16 +348,16 @@
         Returns
         -------
         str | None
             The configured output directory path when the output direction is 'file'.
             Otherwise, None. If the 'directory_path' setting is missing returns
             'mimeo-output' by default.
         """
-        if direction == MimeoConfig.OUTPUT_DIRECTION_FILE:
-            return output.get(MimeoConfig.OUTPUT_DIRECTORY_PATH_KEY, "mimeo-output")
+        if direction == cc.OUTPUT_DIRECTION_FILE:
+            return output.get(cc.OUTPUT_DIRECTORY_PATH_KEY, "mimeo-output")
         return None
 
     @staticmethod
     def _get_file_name(
             direction: str,
             output: dict,
             output_format: str,
@@ -499,16 +376,16 @@
         Returns
         -------
         str | None
             The configured output file name template when the output direction is
             'file'. Otherwise, None. If the 'file_name' setting is missing returns
             'mimeo-output-{}.{output_format}' by default.
         """
-        if direction == MimeoConfig.OUTPUT_DIRECTION_FILE:
-            file_name = output.get(MimeoConfig.OUTPUT_FILE_NAME_KEY, "mimeo-output")
+        if direction == cc.OUTPUT_DIRECTION_FILE:
+            file_name = output.get(cc.OUTPUT_FILE_NAME_KEY, "mimeo-output")
             return f"{file_name}-{'{}'}.{output_format}"
         return None
 
     @staticmethod
     def _get_method(
             direction: str,
             output: dict,
@@ -526,25 +403,28 @@
 
         Returns
         -------
         method: str | None
             The configured HTTP request method when the output direction is 'http'.
             Otherwise, None. If the 'method' setting is missing returns
             'POST' by default.
+
+        Raises
+        ------
+        UnsupportedPropertyValueError
+            If the configured request method is not supported
         """
         method = None
-        if direction == MimeoConfig.OUTPUT_DIRECTION_HTTP:
-            method = output.get(
-                MimeoConfig.OUTPUT_METHOD_KEY,
-                MimeoConfig.OUTPUT_DIRECTION_HTTP_REQUEST_POST)
-            if method not in MimeoConfig.SUPPORTED_REQUEST_METHODS:
+        if direction == cc.OUTPUT_DIRECTION_HTTP:
+            method = output.get(cc.OUTPUT_METHOD_KEY, cc.OUTPUT_HTTP_REQUEST_POST)
+            if method not in cc.SUPPORTED_REQUEST_METHODS:
                 raise UnsupportedPropertyValueError(
-                    MimeoConfig.OUTPUT_METHOD_KEY,
+                    cc.OUTPUT_METHOD_KEY,
                     method,
-                    MimeoConfig.SUPPORTED_REQUEST_METHODS)
+                    cc.SUPPORTED_REQUEST_METHODS)
         return method
 
     @staticmethod
     def _get_protocol(
             direction: str,
             output: dict,
     ) -> str | None:
@@ -561,19 +441,29 @@
 
         Returns
         -------
         str | None
             The configured HTTP request method when the output direction is 'http'.
             Otherwise, None. If the 'protocol' setting is missing returns
             'http' by default.
+
+        Raises
+        ------
+        UnsupportedPropertyValueError
+            If the configured request protocol is not supported
         """
-        if direction == MimeoConfig.OUTPUT_DIRECTION_HTTP:
-            return output.get(MimeoConfig.OUTPUT_PROTOCOL_KEY,
-                              MimeoConfig.OUTPUT_DIRECTION_HTTP)
-        return None
+        protocol = None
+        if direction == cc.OUTPUT_DIRECTION_HTTP:
+            protocol = output.get(cc.OUTPUT_PROTOCOL_KEY, cc.OUTPUT_PROTOCOL_HTTP)
+            if protocol not in cc.SUPPORTED_REQUEST_PROTOCOLS:
+                raise UnsupportedPropertyValueError(
+                    cc.OUTPUT_PROTOCOL_KEY,
+                    protocol,
+                    cc.SUPPORTED_REQUEST_PROTOCOLS)
+        return protocol
 
     @staticmethod
     def _get_host(
             direction: str,
             output: dict,
     ) -> str | None:
         """Extract an HTTP host from the source dictionary.
@@ -589,16 +479,16 @@
 
         Returns
         -------
         str | None
             The configured HTTP host when the output direction is 'http'.
             Otherwise, None.
         """
-        if direction == MimeoConfig.OUTPUT_DIRECTION_HTTP:
-            return output.get(MimeoConfig.OUTPUT_HOST_KEY)
+        if direction == cc.OUTPUT_DIRECTION_HTTP:
+            return output.get(cc.OUTPUT_HOST_KEY)
         return None
 
     @staticmethod
     def _get_port(
             direction: str,
             output: dict,
     ) -> str | None:
@@ -615,16 +505,16 @@
 
         Returns
         -------
         str | None
             The configured HTTP port when the output direction is 'http'.
             Otherwise, None.
         """
-        if direction == MimeoConfig.OUTPUT_DIRECTION_HTTP:
-            return output.get(MimeoConfig.OUTPUT_PORT_KEY)
+        if direction == cc.OUTPUT_DIRECTION_HTTP:
+            return output.get(cc.OUTPUT_PORT_KEY)
         return None
 
     @staticmethod
     def _get_endpoint(
             direction: str,
             output: dict,
     ) -> str | None:
@@ -641,16 +531,16 @@
 
         Returns
         -------
         str | None
             The configured HTTP request method when the output direction is 'http'.
             Otherwise, None.
         """
-        if direction == MimeoConfig.OUTPUT_DIRECTION_HTTP:
-            return output.get(MimeoConfig.OUTPUT_ENDPOINT_KEY)
+        if direction == cc.OUTPUT_DIRECTION_HTTP:
+            return output.get(cc.OUTPUT_ENDPOINT_KEY)
         return None
 
     @staticmethod
     def _get_username(
             direction: str,
             output: dict,
     ) -> str | None:
@@ -667,16 +557,16 @@
 
         Returns
         -------
         str | None
             The configured username when the output direction is 'http'.
             Otherwise, None.
         """
-        if direction == MimeoConfig.OUTPUT_DIRECTION_HTTP:
-            return output.get(MimeoConfig.OUTPUT_USERNAME_KEY)
+        if direction == cc.OUTPUT_DIRECTION_HTTP:
+            return output.get(cc.OUTPUT_USERNAME_KEY)
         return None
 
     @staticmethod
     def _get_password(
             direction: str,
             output: dict,
     ) -> str | None:
@@ -693,16 +583,16 @@
 
         Returns
         -------
         str | None
             The configured password when the output direction is 'http'.
             Otherwise, None.
         """
-        if direction == MimeoConfig.OUTPUT_DIRECTION_HTTP:
-            return output.get(MimeoConfig.OUTPUT_PASSWORD_KEY)
+        if direction == cc.OUTPUT_DIRECTION_HTTP:
+            return output.get(cc.OUTPUT_PASSWORD_KEY)
         return None
 
     @staticmethod
     def _validate_output(
             direction: str,
             output: dict,
     ) -> None:
@@ -720,23 +610,21 @@
 
         Raises
         ------
         MissingRequiredPropertyError
             If the output details doesn't include all required settings
             for the direction
         """
-        if direction == MimeoConfig.OUTPUT_DIRECTION_HTTP:
+        if direction == cc.OUTPUT_DIRECTION_HTTP:
             missing_details = []
-            for detail in MimeoConfig.REQUIRED_HTTP_DETAILS:
+            for detail in cc.REQUIRED_HTTP_DETAILS:
                 if detail not in output:
                     missing_details.append(detail)
             if len(missing_details) > 0:
-                details_str = ", ".join(missing_details)
-                msg = f"Missing required fields is HTTP output details: {details_str}"
-                raise MissingRequiredPropertyError(msg)
+                raise MissingRequiredPropertyError(missing_details)
 
 
 class MimeoTemplate(MimeoDTO):
     """A MimeoDTO class representing Mimeo Template.
 
     It is a python representation of a Mimeo Template configuration node.
 
@@ -759,39 +647,39 @@
         Parameters
         ----------
         template : dict
             A source config template dictionary
         """
         super().__init__(template)
         self._validate_template(template)
-        self.count = template.get(MimeoConfig.TEMPLATES_COUNT_KEY)
-        self.model = MimeoModel(template.get(MimeoConfig.TEMPLATES_MODEL_KEY))
+        self.count = template.get(cc.TEMPLATES_COUNT_KEY)
+        self.model = MimeoModel(template.get(cc.TEMPLATES_MODEL_KEY))
 
     @staticmethod
     def _validate_template(
             template: dict,
     ) -> None:
         """Validate template in the source dictionary.
 
         Parameters
         ----------
         template : dict
             A source config template dictionary
 
         Raises
         ------
-        IncorrectMimeoTemplate
+        InvalidMimeoTemplateError
             If the source config doesn't include count or model properties
         """
-        if MimeoConfig.TEMPLATES_COUNT_KEY not in template:
-            msg = f"No count value in the Mimeo Template: {template}"
-            raise InvalidMimeoTemplateError(msg)
-        if MimeoConfig.TEMPLATES_MODEL_KEY not in template:
-            msg = f"No model data in the Mimeo Template: {template}"
-            raise InvalidMimeoTemplateError(msg)
+        if cc.TEMPLATES_COUNT_KEY not in template:
+            prop_name = "count"
+            raise InvalidMimeoTemplateError(prop_name, template)
+        if cc.TEMPLATES_MODEL_KEY not in template:
+            prop_name = "model"
+            raise InvalidMimeoTemplateError(prop_name, template)
 
 
 class MimeoModel(MimeoDTO):
     """A MimeoDTO class representing Mimeo Model.
 
     It is a python representation of a Mimeo Model configuration node.
 
@@ -837,24 +725,22 @@
         Returns
         -------
         str
             The configured root node's tag
 
         Raises
         ------
-        IncorrectMimeoModel
+        InvalidMimeoModelError
             If the source config has no or more than one root nodes
         """
         model_keys = list(filter(MimeoModel._is_not_configuration_key, iter(model)))
         if len(model_keys) == 0:
-            msg = f"No root data in Mimeo Model: {model}"
-            raise InvalidMimeoModelError(msg)
+            raise InvalidMimeoModelError(InvalidMimeoModelError.Code.ERR_1, model=model)
         if len(model_keys) > 1:
-            msg = f"Multiple root data in Mimeo Model: {model}"
-            raise InvalidMimeoModelError(msg)
+            raise InvalidMimeoModelError(InvalidMimeoModelError.Code.ERR_2, model=model)
         return model_keys[0]
 
     @staticmethod
     def _get_context_name(
             model: dict,
             root_name: str,
     ) -> str:
@@ -871,21 +757,20 @@
         -------
         str
             The configured context name.
             If the 'context' setting is missing returns root name by default
 
         Raises
         ------
-        IncorrectMimeoModel
+        InvalidMimeoModelError
             If the source config has a context name not being a string value
         """
-        context_name = model.get(MimeoConfig.MODEL_CONTEXT_KEY, root_name)
+        context_name = model.get(cc.MODEL_CONTEXT_KEY, root_name)
         if not isinstance(context_name, str):
-            msg = f"Invalid context name in Mimeo Model (not a string value): {model}"
-            raise InvalidMimeoModelError(msg)
+            raise InvalidMimeoModelError(InvalidMimeoModelError.Code.ERR_3, model=model)
         return context_name
 
     @staticmethod
     def _is_not_configuration_key(
             dict_key: str,
     ) -> bool:
         """Verify if the dictionary key is a configuration one.
@@ -896,8 +781,8 @@
             A dictionary key to verify
 
         Returns
         -------
         bool
             True if the key is 'context', otherwise False
         """
-        return dict_key not in [MimeoConfig.MODEL_CONTEXT_KEY]
+        return dict_key not in [cc.MODEL_CONTEXT_KEY]
```

### Comparing `mimeograph-0.5.0/src/mimeo/consumers/__init__.py` & `mimeograph-0.6.0/src/mimeo/consumers/__init__.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.5.0/src/mimeo/consumers/consumer.py` & `mimeograph-0.6.0/src/mimeo/consumers/consumer.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.5.0/src/mimeo/consumers/consumer_factory.py` & `mimeograph-0.6.0/src/mimeo/consumers/consumer_factory.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 It exports only one class:
     * ConsumerFactory
         A Factory class instantiating a Consumer based on Mimeo Config.
 """
 from __future__ import annotations
 
+from mimeo.config import constants as cc
 from mimeo.config.exc import UnsupportedPropertyValueError
 from mimeo.config.mimeo_config import MimeoConfig
 from mimeo.consumers import Consumer, FileConsumer, HttpConsumer, RawConsumer
 
 
 class ConsumerFactory:
     """A Factory class instantiating a Consumer based on Mimeo Config.
@@ -27,17 +28,17 @@
 
     Methods
     -------
     get_consumer(mimeo_config: MimeoConfig) -> Consumer
         Initialize a Consumer based on the Mimeo Output Direction.
     """
 
-    FILE_DIRECTION = MimeoConfig.OUTPUT_DIRECTION_FILE
-    STD_OUT_DIRECTION = MimeoConfig.OUTPUT_DIRECTION_STD_OUT
-    HTTP_DIRECTION = MimeoConfig.OUTPUT_DIRECTION_HTTP
+    FILE_DIRECTION = cc.OUTPUT_DIRECTION_FILE
+    STD_OUT_DIRECTION = cc.OUTPUT_DIRECTION_STD_OUT
+    HTTP_DIRECTION = cc.OUTPUT_DIRECTION_HTTP
 
     @staticmethod
     def get_consumer(
             mimeo_config: MimeoConfig,
     ) -> Consumer:
         """Initialize a Consumer based on the Mimeo Output Direction.
 
@@ -60,10 +61,10 @@
         if direction == ConsumerFactory.STD_OUT_DIRECTION:
             return RawConsumer()
         if direction == ConsumerFactory.FILE_DIRECTION:
             return FileConsumer(mimeo_config.output)
         if direction == ConsumerFactory.HTTP_DIRECTION:
             return HttpConsumer(mimeo_config.output)
         raise UnsupportedPropertyValueError(
-            MimeoConfig.OUTPUT_DIRECTION_KEY,
+            cc.OUTPUT_DIRECTION_KEY,
             direction,
-            MimeoConfig.SUPPORTED_OUTPUT_DIRECTIONS)
+            cc.SUPPORTED_OUTPUT_DIRECTIONS)
```

### Comparing `mimeograph-0.5.0/src/mimeo/consumers/file_consumer.py` & `mimeograph-0.6.0/src/mimeo/consumers/file_consumer.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.5.0/src/mimeo/consumers/http_consumer.py` & `mimeograph-0.6.0/src/mimeo/consumers/http_consumer.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.5.0/src/mimeo/consumers/raw_consumer.py` & `mimeograph-0.6.0/src/mimeo/consumers/raw_consumer.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.5.0/src/mimeo/context/__init__.py` & `mimeograph-0.6.0/src/mimeo/context/__init__.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.5.0/src/mimeo/context/decorators.py` & `mimeograph-0.6.0/src/mimeo/context/decorators.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.5.0/src/mimeo/context/exc.py` & `mimeograph-0.6.0/src/mimeo/context/exc.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.5.0/src/mimeo/context/mimeo_context.py` & `mimeograph-0.6.0/src/mimeo/context/mimeo_context.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,14 +47,16 @@
         Return a specific iteration from the context.
     clear_iterations()
         Clear out all context iterations.
     next_country_index() -> int
         Provide next unique country index.
     next_city_index(country: str = None) -> int
         Provide next unique city index.
+    next_currency_index() -> int
+        Provide next unique currency index.
     next_first_name_index(sex: str = None) -> int
         Provide next unique first name index.
     next_last_name_index() -> int
         Provide next unique last name index.
     """
 
     _ALL = "_ALL_"
@@ -73,14 +75,15 @@
             A context name
         """
         self.name = name
         self._id = 0
         self._iterations = []
         self._countries_indexes = None
         self._cities_indexes = {}
+        self._currencies_indexes = None
         self._first_names_indexes = {}
         self._last_names_indexes = None
 
     def next_id(
             self,
     ) -> int:
         """Increment an identifier and return the current (incremented) one.
@@ -258,26 +261,54 @@
         Returns
         -------
         int
             Next unique city identifier
 
         Raises
         ------
-        CountryNotFound
+        DataNotFoundError
             If database does not contain any cities for the provided
             `country`
         OutOfStockError
             If all cities' indexes have been consumed already
         """
         country = country if country is not None else MimeoContext._ALL
         self._initialize_cities_indexes(country)
         self._validate_cities(country)
 
         return self._cities_indexes[country][MimeoContext._INDEXES].pop()
 
+    def next_currency_index(
+            self,
+    ) -> int:
+        """Provide next unique currency index.
+
+        When used for the first time in the specific context
+        it populates internal currencies' indexes list. This approach
+        ensures country uniqueness without time-consuming operations.
+        Each time it verifies if the internal list still contains some
+        indexes.
+        This method is used by the Currency Mimeo Util to get a currency
+        entry at a specific index in database.
+
+        Returns
+        -------
+        int
+            Next unique currency identifier
+
+        Raises
+        ------
+        OutOfStockError
+            If all currencies' indexes have been consumed already
+        """
+        self._initialize_currencies_indexes()
+        self._validate_currencies()
+
+        return self._currencies_indexes.pop()
+
     def next_first_name_index(
             self,
             sex: str = None,
     ) -> int:
         """Provide next unique first name index.
 
         When used for the first time in the specific context
@@ -361,35 +392,49 @@
         """Initialize cities' indexes with unique integers.
 
         The list length and range depends on the number of city
         records in database for the `country`.
 
         Raises
         ------
-        CountryNotFound
+        DataNotFoundError
             If database does not contain any cities for the provided
             `country`
         """
         if country not in self._cities_indexes:
             if country == MimeoContext._ALL:
                 num_of_entries = MimeoDB.NUM_OF_CITIES
             else:
                 country_cities = MimeoDB().get_cities_of(country)
                 num_of_entries = len(country_cities)
                 if num_of_entries == 0:
-                    msg = (f"Mimeo database doesn't contain any cities "
-                           f"of provided country [{country}].")
-                    raise DataNotFoundError(msg)
+                    raise DataNotFoundError(DataNotFoundError.Code.ERR_2,
+                                            data="city",
+                                            param_name="country",
+                                            param_val=country)
 
             cities_indexes = random.sample(range(num_of_entries), num_of_entries)
             self._cities_indexes[country] = {
                 MimeoContext._INITIAL_COUNT: num_of_entries,
                 MimeoContext._INDEXES: cities_indexes,
             }
 
+    def _initialize_currencies_indexes(
+            self,
+    ):
+        """Initialize currencies' indexes with unique integers.
+
+        The list length and range depends on the number of currency
+        records in database.
+        """
+        if self._currencies_indexes is None:
+            num_of_entries = MimeoDB.NUM_OF_CURRENCIES
+            currencies_indexes = random.sample(range(num_of_entries), num_of_entries)
+            self._currencies_indexes = currencies_indexes
+
     def _initialize_first_names_indexes(
             self,
             sex: str,
     ):
         """Initialize first names' indexes with integers.
 
         The list length and range depends on the number of first name
@@ -433,17 +478,17 @@
 
         Raises
         ------
         OutOfStockError
             If all countries' indexes have been consumed already
         """
         if len(self._countries_indexes) == 0:
-            msg = (f"No more unique values, "
-                   f"database contain only {MimeoDB.NUM_OF_COUNTRIES} countries.")
-            raise OutOfStockError(msg)
+            raise OutOfStockError(OutOfStockError.Code.ERR_1,
+                                  num=MimeoDB.NUM_OF_COUNTRIES,
+                                  data="countries")
 
     def _validate_cities(
             self,
             country: str,
     ):
         """Verify if all cities' indexes have been consumed.
 
@@ -451,20 +496,36 @@
         ------
         OutOfStockError
             If all cities' indexes have been consumed already
         """
         if len(self._cities_indexes[country][MimeoContext._INDEXES]) == 0:
             init_count = self._cities_indexes[country][MimeoContext._INITIAL_COUNT]
             if country == MimeoContext._ALL:
-                msg = (f"No more unique values, "
-                       f"database contain only {init_count} cities.")
-            else:
-                msg = (f"No more unique values, "
-                       f"database contain only {init_count} cities of {country}.")
-            raise OutOfStockError(msg)
+                raise OutOfStockError(OutOfStockError.Code.ERR_1,
+                                      num=init_count,
+                                      data="cities")
+            raise OutOfStockError(OutOfStockError.Code.ERR_2,
+                                  num=init_count,
+                                  data="cities",
+                                  param_val=country)
+
+    def _validate_currencies(
+            self,
+    ):
+        """Verify if all currencies' indexes have been consumed.
+
+        Raises
+        ------
+        OutOfStockError
+            If all currencies' indexes have been consumed already
+        """
+        if len(self._currencies_indexes) == 0:
+            raise OutOfStockError(OutOfStockError.Code.ERR_1,
+                                  num=MimeoDB.NUM_OF_CURRENCIES,
+                                  data="currencies")
 
     def _validate_first_names(
             self,
             sex: str,
     ):
         """Verify if all first names' indexes have been consumed.
 
@@ -472,29 +533,30 @@
         ------
         OutOfStockError
             If all first names' indexes have been consumed already
         """
         if len(self._first_names_indexes[sex][MimeoContext._INDEXES]) == 0:
             init_count = self._first_names_indexes[sex][MimeoContext._INITIAL_COUNT]
             if sex == MimeoContext._ALL:
-                msg = (f"No more unique values, "
-                       f"database contain only {init_count} first names.")
+                sex_info = ""
+            elif sex == "M":
+                sex_info = "male "
             else:
-                sex_info = "male" if sex == "M" else "female"
-                msg = (f"No more unique values, "
-                       f"database contain only {init_count} {sex_info} first names.")
-            raise OutOfStockError(msg)
+                sex_info = "female "
+            raise OutOfStockError(OutOfStockError.Code.ERR_1,
+                                  num=init_count,
+                                  data=f"{sex_info}first names")
 
     def _validate_last_names(
             self,
     ):
         """Verify if all last names' indexes have been consumed.
 
         Raises
         ------
         OutOfStockError
             If all last names' indexes have been consumed already
         """
         if len(self._last_names_indexes) == 0:
-            msg = (f"No more unique values, "
-                   f"database contain only {MimeoDB.NUM_OF_LAST_NAMES} last names.")
-            raise OutOfStockError(msg)
+            raise OutOfStockError(OutOfStockError.Code.ERR_1,
+                                  num=MimeoDB.NUM_OF_LAST_NAMES,
+                                  data="last names")
```

### Comparing `mimeograph-0.5.0/src/mimeo/context/mimeo_context_manager.py` & `mimeograph-0.6.0/src/mimeo/context/mimeo_context_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,15 @@
         Returns
         -------
         MimeoContext
             A specific Mimeo Context
 
         Raises
         ------
-        InstanceNotAlive
+        InstanceNotAliveError
             If the MimeoContextManager instance is not alive
         """
         super().assert_alive()
         if context not in self._contexts:
             self._contexts[context] = MimeoContext(context)
         return self._contexts[context]
 
@@ -134,15 +134,15 @@
         Returns
         -------
         MimeoContext
             The current Mimeo Context
 
         Raises
         ------
-        InstanceNotAlive
+        InstanceNotAliveError
             If the MimeoContextManager instance is not alive
         """
         super().assert_alive()
         return self._current_context
 
     def set_current_context(
             self,
@@ -153,15 +153,15 @@
         Parameters
         ----------
         context : MimeoContext
             A Mimeo Context to be set as the current one
 
         Raises
         ------
-        InstanceNotAlive
+        InstanceNotAliveError
             If the MimeoContextManager instance is not alive
         """
         super().assert_alive()
         self._current_context = context
 
     def get_var(
             self,
@@ -177,15 +177,15 @@
         Returns
         -------
         value : str | int | bool | dict
             The Mimeo Var value
 
         Raises
         ------
-        InstanceNotAlive
+        InstanceNotAliveError
             If the MimeoContextManager instance is not alive
         VarNotFoundError
             If the Mimeo Var with the `variable_name` provided does not
             exist
         """
         super().assert_alive()
         value = self._vars.get(variable_name)
```

### Comparing `mimeograph-0.5.0/src/mimeo/context/mimeo_iteration.py` & `mimeograph-0.6.0/src/mimeo/context/mimeo_iteration.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.5.0/src/mimeo/database/__init__.py` & `mimeograph-0.6.0/src/mimeo/database/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,54 +5,63 @@
 It contains the following modules:
 * mimeo_db
     The Mimeo Database module.
 * cities
     The Cities module.
 * countries
     The Countries module.
+* currencies
+    The Currencies module.
 * first_names
     The First Names module.
 * last_names
     The Last Names module.
 * exc
     The Mimeo Database Exceptions module.
 
 The Mimeo Context package exports the following classes:
 * MimeoDB
     Facade class exposing READ operations on all Mimeo CSV data.
 * CitiesDB
     Class exposing READ operations on cities CSV data.
 * CountriesDB
     Class exposing READ operations on countries CSV data.
+* CurrenciesDB
+    Class exposing READ operations on currencies CSV data.
 * FirstNamesDB
     Class exposing READ operations on forenames CSV data.
 * LastNamesDB
     Class exposing READ operations on surnames CSV data.
 * City
     DTO class representing a single row in cities CSV data.
 * Country
     DTO class representing a single row in countries CSV data.
+* Currency
+    DTO class representing a single row in currencies CSV data.
 * FirstName
     DTO class representing a single row in forenames CSV data.
 
 To use this package, simply import the desired class:
     from mimeo.database import MimeoDB
     from mimeo.database.exc import DataNotFoundError
 """
 from __future__ import annotations
 
 from .cities import CitiesDB, City
 from .countries import CountriesDB, Country
+from .currencies import CurrenciesDB, Currency
 from .first_names import FirstName, FirstNamesDB
 from .last_names import LastNamesDB
 from .mimeo_db import MimeoDB
 
 __all__ = [
     "City",
     "Country",
+    "Currency",
     "FirstName",
     "CitiesDB",
     "CountriesDB",
+    "CurrenciesDB",
     "FirstNamesDB",
     "LastNamesDB",
     "MimeoDB",
 ]
```

### Comparing `mimeograph-0.5.0/src/mimeo/database/cities.py` & `mimeograph-0.6.0/src/mimeo/database/cities.py`

 * *Files 10% similar despite different names*

```diff
@@ -129,15 +129,15 @@
             A specific city
 
         Raises
         ------
         InvalidIndexError
             If the provided `index` is out of bounds
         """
-        cities = self._get_cities()
+        cities = CitiesDB._get_cities()
         try:
             return cities[index]
         except IndexError:
             last_index = CitiesDB.NUM_OF_RECORDS-1
             raise InvalidIndexError(index, last_index) from IndexError
 
     def get_cities_of(
@@ -152,28 +152,27 @@
             A country ISO3 code to filter cities
 
         Returns
         -------
         list[City]
             List of cities filtered by country
         """
-        return self._get_country_cities(country_iso3).copy()
+        return CitiesDB._get_country_cities(country_iso3).copy()
 
-    @classmethod
     def get_cities(
-            cls,
+            self,
     ) -> list[City]:
         """Get all cities.
 
         Returns
         -------
         list[City]
             List of all cities
         """
-        return cls._get_cities().copy()
+        return CitiesDB._get_cities().copy()
 
     @classmethod
     def _get_country_cities(
             cls,
             country_iso3: str,
     ) -> list[City]:
         """Get cities of a specific country from cache.
@@ -218,10 +217,10 @@
 
     @classmethod
     def _get_cities_df(
             cls,
     ) -> pandas.DataFrame:
         """Load cities CSV data and save in internal class attribute."""
         if cls._CITIES_DF is None:
-            data = tools.get_resource(CitiesDB._CITIES_DB)
+            data = tools.get_resource(cls._CITIES_DB)
             cls._CITIES_DF = pandas.read_csv(data)
         return cls._CITIES_DF
```

### Comparing `mimeograph-0.5.0/src/mimeo/database/countries.py` & `mimeograph-0.6.0/src/mimeo/database/countries.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,15 +125,15 @@
             A specific country
 
         Raises
         ------
         InvalidIndexError
             If the provided `index` is out of bounds
         """
-        countries = self._get_countries()
+        countries = CountriesDB._get_countries()
         try:
             return countries[index]
         except IndexError:
             last_index = CountriesDB.NUM_OF_RECORDS-1
             raise InvalidIndexError(index, last_index) from IndexError
 
     def get_country_by_iso_3(
@@ -148,15 +148,15 @@
             An ISO3 code to find a country
 
         Returns
         -------
         Country
             A specific country or None
         """
-        countries = self._get_countries()
+        countries = CountriesDB._get_countries()
         return next(filter(lambda country: country.iso_3 == iso_3, countries), None)
 
     def get_country_by_iso_2(
             self,
             iso_2: str,
     ) -> Country:
         """Get a country having a specific ISO2 code.
@@ -167,15 +167,15 @@
             An ISO2 code to find a country
 
         Returns
         -------
         Country
             A specific country or None
         """
-        countries = self._get_countries()
+        countries = CountriesDB._get_countries()
         return next(filter(lambda country: country.iso_2 == iso_2, countries), None)
 
     def get_country_by_name(
             self,
             name: str,
     ) -> Country:
         """Get a country having a specific name.
@@ -186,29 +186,28 @@
             A name to find a country
 
         Returns
         -------
         Country
             A specific country or None
         """
-        countries = self._get_countries()
+        countries = CountriesDB._get_countries()
         return next(filter(lambda country: country.name == name, countries), None)
 
-    @classmethod
     def get_countries(
-            cls,
+            self,
     ) -> list[Country]:
         """Get all countries.
 
         Returns
         -------
         list[Country]
             List of all countries
         """
-        return cls._get_countries().copy()
+        return CountriesDB._get_countries().copy()
 
     @classmethod
     def _get_countries(
             cls,
     ) -> list[Country]:
         """Get all countries from cache.
 
@@ -227,10 +226,10 @@
 
     @classmethod
     def _get_countries_df(
             cls,
     ) -> pandas.DataFrame:
         """Load countries CSV data and save in internal class attribute."""
         if cls._COUNTRIES_DF is None:
-            data = tools.get_resource(CountriesDB._COUNTRIES_DB)
+            data = tools.get_resource(cls._COUNTRIES_DB)
             cls._COUNTRIES_DF = pandas.read_csv(data)
         return cls._COUNTRIES_DF
```

### Comparing `mimeograph-0.5.0/src/mimeo/database/first_names.py` & `mimeograph-0.6.0/src/mimeo/database/first_names.py`

 * *Files 10% similar despite different names*

```diff
@@ -114,15 +114,15 @@
             A specific first name
 
         Raises
         ------
         InvalidIndexError
             If the provided `index` is out of bounds
         """
-        first_names = self.__get_first_names()
+        first_names = FirstNamesDB._get_first_names()
         try:
             return first_names[index]
         except IndexError:
             last_index = FirstNamesDB.NUM_OF_RECORDS-1
             raise InvalidIndexError(index, last_index) from IndexError
 
     def get_first_names_by_sex(
@@ -144,31 +144,30 @@
         Raises
         ------
         InvalidSexError
             If the provided `sex` value is not supported
         """
         if sex not in FirstNamesDB.__SUPPORTED_SEX:
             raise InvalidSexError(FirstNamesDB.__SUPPORTED_SEX)
-        return self.__get_first_names_by_sex(sex).copy()
+        return FirstNamesDB._get_first_names_by_sex(sex).copy()
 
-    @classmethod
     def get_first_names(
-            cls,
+            self,
     ) -> list[FirstName]:
         """Get all first names.
 
         Returns
         -------
         list[FirstName]
             List of all first names
         """
-        return cls.__get_first_names().copy()
+        return FirstNamesDB._get_first_names().copy()
 
     @classmethod
-    def __get_first_names_by_sex(
+    def _get_first_names_by_sex(
             cls,
             sex: str,
     ) -> list[FirstName]:
         """Get first names for a specific sex from cache.
 
         The first names list for sex is initialized for the first time
         and cached in internal class attribute.
@@ -180,39 +179,39 @@
 
         Returns
         -------
         list[FirstName]
             List of first names filtered by sex
         """
         if sex not in cls.__NAMES_FOR_SEX:
-            first_names = cls.__get_first_names()
+            first_names = cls._get_first_names()
             cls.__NAMES_FOR_SEX[sex] = list(filter(lambda n: n.sex == sex, first_names))
         return cls.__NAMES_FOR_SEX[sex]
 
     @classmethod
-    def __get_first_names(
+    def _get_first_names(
             cls,
     ) -> list[FirstName]:
         """Get all first names from cache.
 
         The first names list is initialized for the first time and
         cached in internal class attribute.
 
         Returns
         -------
         list[FirstName]
             List of all first names
         """
         if cls.__FIRST_NAMES is None:
             cls.__FIRST_NAMES = [FirstName(row.NAME, row.SEX)
-                                 for row in cls.__get_first_names_df().itertuples()]
+                                 for row in cls._get_first_names_df().itertuples()]
         return cls.__FIRST_NAMES
 
     @classmethod
-    def __get_first_names_df(
+    def _get_first_names_df(
             cls,
     ) -> pandas.DataFrame:
         """Load forenames CSV data and save in internal class attribute."""
         if cls.__FIRST_NAMES_DF is None:
-            data = tools.get_resource(FirstNamesDB.__FIRST_NAMES_DB)
+            data = tools.get_resource(cls.__FIRST_NAMES_DB)
             cls.__FIRST_NAMES_DF = pandas.read_csv(data)
         return cls.__FIRST_NAMES_DF
```

### Comparing `mimeograph-0.5.0/src/mimeo/database/last_names.py` & `mimeograph-0.6.0/src/mimeo/database/last_names.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,45 +47,44 @@
             A last name
 
         Raises
         ------
         InvalidIndexError
             If the provided `index` is out of bounds
         """
-        last_names = self.__get_last_names()
+        last_names = LastNamesDB._get_last_names()
         try:
             return last_names[index]
         except IndexError:
             last_index = LastNamesDB.NUM_OF_RECORDS-1
             raise InvalidIndexError(index, last_index) from IndexError
 
-    @classmethod
     def get_last_names(
-            cls,
+            self,
     ) -> list[str]:
         """Get all last names.
 
         Returns
         -------
         list[str]
             List of all last names
         """
-        return cls.__get_last_names().copy()
+        return LastNamesDB._get_last_names().copy()
 
     @classmethod
-    def __get_last_names(
+    def _get_last_names(
             cls,
     ) -> list:
         """Get all last names from cache.
 
         The last names list is initialized for the first time and
         cached in internal class attribute.
 
         Returns
         -------
         list[str]
             List of all last names
         """
         if cls._LAST_NAMES is None:
-            with tools.get_resource(LastNamesDB._LAST_NAMES_DB) as last_names:
+            with tools.get_resource(cls._LAST_NAMES_DB) as last_names:
                 cls._LAST_NAMES = [line.rstrip() for line in last_names.readlines()]
         return cls._LAST_NAMES
```

### Comparing `mimeograph-0.5.0/src/mimeo/database/mimeo_db.py` & `mimeograph-0.6.0/src/mimeo/database/mimeo_db.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,47 +2,56 @@
 
 It exports a class related to all Mimeo CSV data:
     * MimeoDB
         Facade class exposing READ operations on all Mimeo CSV data.
 """
 from __future__ import annotations
 
-from mimeo.database import (CitiesDB, City, CountriesDB, Country, FirstName,
-                            FirstNamesDB, LastNamesDB)
+from mimeo.database import (CitiesDB, City, CountriesDB, Country, CurrenciesDB,
+                            Currency, FirstName, FirstNamesDB, LastNamesDB)
 
 
 class MimeoDB:
     """Facade class exposing READ operations on all Mimeo CSV data.
 
     It combines all attributes and methods exposed by downstream
     classes:
     - CitiesDB
     - CountriesDB
+    - CurrenciesDB
     - FirstNamesDB
     - LastNamesDB
 
     Attributes
     ----------
     NUM_OF_CITIES : int
         A number of rows in cities CSV data
     NUM_OF_COUNTRIES : int
         A number of rows in countries CSV data
+    NUM_OF_CURRENCIES : int
+        A number of rows in currencies CSV data
     NUM_OF_FIRST_NAMES : int
         A number of rows in forenames CSV data
     NUM_OF_LAST_NAMES : int
         A number of rows in surnames CSV data
 
     Methods
     -------
     get_cities() -> list[City]
         Get all cities.
     get_cities_of(country: str) -> list[City]
         Get cities of a specific country.
     get_city_at(index: int) -> City
         Get a city at `index` position.
+    get_currencies() -> list[Currency]
+        Get all currencies.
+    get_currency_at(index: int) -> Currency
+        Get a currency at `index` position.
+    get_currency_of(country: str) -> Currency | None
+        Get a currency at `index` position.
     get_countries() -> list[Country]
         Get all countries.
     get_country_at(index: int) -> Country
         Get a country at `index` position.
     get_country_by_iso_3(iso_3: str) -> Country
         Get a country having a specific ISO3 code.
     get_country_by_iso_3(iso_2: str) -> Country
@@ -59,36 +68,38 @@
         Get all last names.
     get_last_name_at(index: int) -> str
         Get a last name at `index` position.
     """
 
     NUM_OF_CITIES = CitiesDB.NUM_OF_RECORDS
     NUM_OF_COUNTRIES = CountriesDB.NUM_OF_RECORDS
+    NUM_OF_CURRENCIES = CurrenciesDB.NUM_OF_RECORDS
     NUM_OF_FIRST_NAMES = FirstNamesDB.NUM_OF_RECORDS
     NUM_OF_LAST_NAMES = LastNamesDB.NUM_OF_RECORDS
 
     def __init__(
             self,
     ):
-        self.__cities_db = CitiesDB()
-        self.__countries_db = CountriesDB()
-        self.__first_names_db = FirstNamesDB()
-        self.__last_names_db = LastNamesDB()
+        self._cities_db = CitiesDB()
+        self._countries_db = CountriesDB()
+        self._currencies_db = CurrenciesDB()
+        self._first_names_db = FirstNamesDB()
+        self._last_names_db = LastNamesDB()
 
     def get_cities(
             self,
     ) -> list[City]:
         """Get all cities.
 
         Returns
         -------
         list[City]
             List of all cities
         """
-        return self.__cities_db.get_cities()
+        return self._cities_db.get_cities()
 
     def get_cities_of(
             self,
             country: str,
     ) -> list[City]:
         """Get cities of a specific country.
 
@@ -110,15 +121,15 @@
         """
         countries = filter(
             lambda c: country in [c.iso_3, c.iso_2, c.name],
             self.get_countries())
         country = next(countries, None)
         if country is None:
             return []
-        return self.__cities_db.get_cities_of(country.iso_3)
+        return self._cities_db.get_cities_of(country.iso_3)
 
     def get_city_at(
             self,
             index: int,
     ) -> City:
         """Get a city at `index` position.
 
@@ -133,27 +144,92 @@
             A specific city
 
         Raises
         ------
         InvalidIndexError
             If the provided `index` is out of bounds
         """
-        return self.__cities_db.get_city_at(index)
+        return self._cities_db.get_city_at(index)
+
+    def get_currencies(
+            self,
+    ) -> list[Currency]:
+        """Get all currencies.
+
+        Returns
+        -------
+        list[Currency]
+            List of all currencies
+        """
+        return self._currencies_db.get_currencies()
+
+    def get_currency_at(
+            self,
+            index: int,
+    ) -> Currency:
+        """Get a currency at `index` position.
+
+        Parameters
+        ----------
+        index : int
+            A currency row index
+
+        Returns
+        -------
+        Currency
+            A specific currency
+
+        Raises
+        ------
+        InvalidIndexError
+            If the provided `index` is out of bounds
+        """
+        return self._currencies_db.get_currency_at(index)
+
+    def get_currency_of(
+            self,
+            country: str,
+    ) -> Currency | None:
+        """Get a currency of a specific country.
+
+        In contrast to CurrenciesDB.get_currency_of() method it combines
+        CurrenciesDB and CountriesDB to allow for any country detail
+        providing. It can be ISO3 code, ISO2 code and name.
+        First it will find the specific country and extract its
+        name to use in CurrenciesDB.get_currency_of() call.
+
+        Parameters
+        ----------
+        country : str
+            A country ISO3 / ISO2 code or name to filter currency
+
+        Returns
+        -------
+        Currency
+            A currency used in a specific country
+        """
+        countries = filter(
+            lambda c: country in [c.iso_3, c.iso_2, c.name],
+            self.get_countries())
+        country = next(countries, None)
+        if country is None:
+            return None
+        return self._currencies_db.get_currency_of(country.name)
 
     def get_countries(
             self,
     ) -> list[Country]:
         """Get all countries.
 
         Returns
         -------
         list[Country]
             List of all countries
         """
-        return self.__countries_db.get_countries()
+        return self._countries_db.get_countries()
 
     def get_country_at(
             self,
             index: int,
     ) -> Country:
         """Get a country at `index` position.
 
@@ -168,15 +244,15 @@
             A specific country
 
         Raises
         ------
         InvalidIndexError
             If the provided `index` is out of bounds
         """
-        return self.__countries_db.get_country_at(index)
+        return self._countries_db.get_country_at(index)
 
     def get_country_by_iso_3(
             self,
             iso_3: str,
     ) -> Country:
         """Get a country having a specific ISO3 code.
 
@@ -186,15 +262,15 @@
             An ISO3 code to find a country
 
         Returns
         -------
         Country
             A specific country or None
         """
-        return self.__countries_db.get_country_by_iso_3(iso_3)
+        return self._countries_db.get_country_by_iso_3(iso_3)
 
     def get_country_by_iso_2(
             self,
             iso_2: str,
     ) -> Country:
         """Get a country having a specific ISO2 code.
 
@@ -204,15 +280,15 @@
             An ISO2 code to find a country
 
         Returns
         -------
         Country
             A specific country or None
         """
-        return self.__countries_db.get_country_by_iso_2(iso_2)
+        return self._countries_db.get_country_by_iso_2(iso_2)
 
     def get_country_by_name(
             self,
             name: str,
     ) -> Country:
         """Get a country having a specific name.
 
@@ -222,27 +298,27 @@
             A name to find a country
 
         Returns
         -------
         Country
             A specific country or None
         """
-        return self.__countries_db.get_country_by_name(name)
+        return self._countries_db.get_country_by_name(name)
 
     def get_first_names(
             self,
     ) -> list[FirstName]:
         """Get all first names.
 
         Returns
         -------
         list[FirstName]
             List of all first names
         """
-        return self.__first_names_db.get_first_names()
+        return self._first_names_db.get_first_names()
 
     def get_first_names_by_sex(
             self,
             sex: str,
     ) -> list[FirstName]:
         """Get first names for a specific sex.
 
@@ -257,15 +333,15 @@
             List of first names filtered by sex
 
         Raises
         ------
         InvalidSexError
             If the provided `sex` value is not supported
         """
-        return self.__first_names_db.get_first_names_by_sex(sex)
+        return self._first_names_db.get_first_names_by_sex(sex)
 
     def get_first_name_at(
             self,
             index: int,
     ) -> FirstName:
         """Get a first name at `index` position.
 
@@ -280,27 +356,27 @@
             A specific first name
 
         Raises
         ------
         InvalidIndexError
             If the provided `index` is out of bounds
         """
-        return self.__first_names_db.get_first_name_at(index)
+        return self._first_names_db.get_first_name_at(index)
 
     def get_last_names(
             self,
     ) -> list[str]:
         """Get all last names.
 
         Returns
         -------
         list[str]
             List of all last names
         """
-        return self.__last_names_db.get_last_names()
+        return self._last_names_db.get_last_names()
 
     def get_last_name_at(
             self,
             index: int,
     ) -> str:
         """Get a last name at `index` position.
 
@@ -315,8 +391,8 @@
             A last name
 
         Raises
         ------
         InvalidIndexError
             If the provided `index` is out of bounds
         """
-        return self.__last_names_db.get_last_name_at(index)
+        return self._last_names_db.get_last_name_at(index)
```

### Comparing `mimeograph-0.5.0/src/mimeo/generators/__init__.py` & `mimeograph-0.6.0/src/mimeo/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.5.0/src/mimeo/generators/exc.py` & `mimeograph-0.6.0/src/mimeo/generators/exc.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.5.0/src/mimeo/generators/generator.py` & `mimeograph-0.6.0/src/mimeo/generators/generator.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.5.0/src/mimeo/generators/generator_factory.py` & `mimeograph-0.6.0/src/mimeo/generators/generator_factory.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 It exports only one class:
     * GeneratorFactory
         A Factory class instantiating a Generator based on Mimeo Config.
 """
 from __future__ import annotations
 
+from mimeo.config import constants as cc
 from mimeo.config.exc import UnsupportedPropertyValueError
 from mimeo.config.mimeo_config import MimeoConfig
 from mimeo.generators import Generator, XMLGenerator
 
 
 class GeneratorFactory:
     """A Factory class instantiating a Generator based on Mimeo Config.
@@ -24,15 +25,15 @@
 
     Methods
     -------
     get_generator(mimeo_config: MimeoConfig) -> Generator
         Initialize a Generator based on the Mimeo Output Format.
     """
 
-    XML = MimeoConfig.OUTPUT_FORMAT_XML
+    XML = cc.OUTPUT_FORMAT_XML
 
     @staticmethod
     def get_generator(
             mimeo_config: MimeoConfig,
     ) -> Generator:
         """Initialize a Generator based on the Mimeo Output Format.
 
@@ -51,10 +52,10 @@
         UnsupportedPropertyValueError
             If the output format is not supported
         """
         output_format = mimeo_config.output.format
         if output_format == GeneratorFactory.XML:
             return XMLGenerator(mimeo_config)
         raise UnsupportedPropertyValueError(
-            MimeoConfig.OUTPUT_FORMAT_KEY,
+            cc.OUTPUT_FORMAT_KEY,
             output_format,
-            MimeoConfig.SUPPORTED_OUTPUT_FORMATS)
+            cc.SUPPORTED_OUTPUT_FORMATS)
```

### Comparing `mimeograph-0.5.0/src/mimeo/generators/xml_generator.py` & `mimeograph-0.6.0/src/mimeo/generators/xml_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from __future__ import annotations
 
 import logging
 import xml.etree.ElementTree as ElemTree
 from typing import Iterator
 from xml.dom import minidom
 
+from mimeo.config import constants as cc
 from mimeo.config.mimeo_config import MimeoConfig, MimeoTemplate
 from mimeo.context import MimeoContext
 from mimeo.context.decorators import (mimeo_clear_iterations, mimeo_context,
                                       mimeo_context_switch,
                                       mimeo_next_iteration)
 from mimeo.generators import Generator
 from mimeo.generators.exc import UnsupportedStructureError
@@ -272,18 +273,18 @@
         tag = element_meta["tag"]
         value = element_meta["value"]
         attrs = element_meta["attrs"]
         is_mimeo_util = MimeoRenderer.is_parametrized_mimeo_util(value)
         is_special_field = MimeoRenderer.is_special_field(tag)
         if is_special_field:
             tag = MimeoRenderer.get_special_field_name(tag)
-        if isinstance(value, dict) and MimeoConfig.MODEL_ATTRIBUTES_KEY in value:
+        if isinstance(value, dict) and cc.MODEL_ATTRIBUTES_KEY in value:
             value = dict(value)
-            attrs = value.pop(MimeoConfig.MODEL_ATTRIBUTES_KEY)
-            value = value.get(MimeoConfig.MODEL_VALUE_KEY, value)
+            attrs = value.pop(cc.MODEL_ATTRIBUTES_KEY)
+            value = value.get(cc.MODEL_VALUE_KEY, value)
         if attrs is None:
             attrs = {}
 
         return cls._element_meta(
             tag,
             value,
             attrs,
@@ -342,15 +343,15 @@
             If a special field value is dict or list
         SpecialFieldNotFoundError
             If a special field does not exist.
         """
         if isinstance(element_meta["value"], dict):
             func = cls._process_dict_value
         elif (isinstance(element_meta["value"], list) and
-              element_meta["tag"] != MimeoConfig.TEMPLATES_KEY):
+              element_meta["tag"] != cc.TEMPLATES_KEY):
             func = cls._process_list_value
         else:
             func = cls._process_templates_value
         return func(parent, element_meta)
 
     @classmethod
     def _process_dict_value(
```

### Comparing `mimeograph-0.5.0/src/mimeo/logging/__init__.py` & `mimeograph-0.6.0/src/mimeo/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.5.0/src/mimeo/logging/filters.py` & `mimeograph-0.6.0/src/mimeo/logging/filters.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.5.0/src/mimeo/meta/__init__.py` & `mimeograph-0.6.0/src/mimeo/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.5.0/src/mimeo/meta/alive.py` & `mimeograph-0.6.0/src/mimeo/meta/alive.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,15 @@
         Returns
         -------
         bool
             True
 
         Raises
         ------
-        InstanceNotAlive
+        InstanceNotAliveError
             If the instance is not alive
         """
         if not self.is_alive():
             raise InstanceNotAliveError
         return self.is_alive()
 
     def is_alive(
```

### Comparing `mimeograph-0.5.0/src/mimeo/meta/exc.py` & `mimeograph-0.6.0/src/mimeo/meta/exc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """The Mimeo Meta Exceptions module.
 
 It contains all custom exceptions related to useful abstract classes:
-    * InstanceNotAlive
+    * InstanceNotAliveError
         A custom Exception class for using non-alive instance.
 """
 
 
 from __future__ import annotations
```

### Comparing `mimeograph-0.5.0/src/mimeo/mimeo.py` & `mimeograph-0.6.0/src/mimeo/mimeo.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.5.0/src/mimeo/resources/cities.csv` & `mimeograph-0.6.0/src/mimeo/resources/cities.csv`

 * *Files identical despite different names*

### Comparing `mimeograph-0.5.0/src/mimeo/resources/countries.csv` & `mimeograph-0.6.0/src/mimeo/resources/countries.csv`

 * *Files identical despite different names*

### Comparing `mimeograph-0.5.0/src/mimeo/resources/exc.py` & `mimeograph-0.6.0/src/mimeo/resources/exc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """The Mimeo Resources Exceptions module.
 
 It contains all custom exceptions related to Mimeo resources:
-    * ResourceNotFound
+    * ResourceNotFoundError
         A custom Exception class for a not found resource.
 """
 
 
 from __future__ import annotations
```

### Comparing `mimeograph-0.5.0/src/mimeo/resources/forenames.csv` & `mimeograph-0.6.0/src/mimeo/resources/forenames.csv`

 * *Files identical despite different names*

### Comparing `mimeograph-0.5.0/src/mimeo/resources/logging.yaml` & `mimeograph-0.6.0/src/mimeo/resources/logging.yaml`

 * *Files identical despite different names*

### Comparing `mimeograph-0.5.0/src/mimeo/resources/surnames.txt` & `mimeograph-0.6.0/src/mimeo/resources/surnames.txt`

 * *Files identical despite different names*

### Comparing `mimeograph-0.5.0/src/mimeo/tools.py` & `mimeograph-0.6.0/src/mimeo/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,14 @@
     Returns
     -------
     TextIO
         A Mimeo resource
 
     Raises
     ------
-    ResourceNotFound
+    ResourceNotFoundError
         If the resource does not exist
     """
     try:
         return pkg_resources.open_text(data, resource_name)
     except FileNotFoundError:
         raise ResourceNotFoundError(resource_name) from FileNotFoundError
```

### Comparing `mimeograph-0.5.0/src/mimeo/utils/__init__.py` & `mimeograph-0.6.0/src/mimeo/utils/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -27,29 +27,32 @@
     A MimeoUtil implementation rendering a current iteration ID.
 * KeyUtil
     A MimeoUtil implementation rendering a unique identifier.
 * CityUtil
     A MimeoUtil implementation rendering city names.
 * CountryUtil
     A MimeoUtil implementation rendering country details.
+* CurrencyUtil
+    A MimeoUtil implementation rendering currency details.
 * FirstNameUtil
     A MimeoUtil implementation rendering forenames.
 * LastNameUtil
     A MimeoUtil implementation rendering surnames.
 * MimeoRenderer
     A Facade class rendering Mimeo Utils, Vars and Special Fields.
 
 To use this package, simply import the desired class:
     from mimeo.utils import MimeoRenderer
 """
 from __future__ import annotations
 
 from .mimeo_utils import (AutoIncrementUtil, CityUtil, CountryUtil,
-                          CurrentIterationUtil, DateTimeUtil, DateUtil,
-                          FirstNameUtil, KeyUtil, LastNameUtil, MimeoUtil,
-                          RandomIntegerUtil, RandomItemUtil, RandomStringUtil)
+                          CurrencyUtil, CurrentIterationUtil, DateTimeUtil,
+                          DateUtil, FirstNameUtil, KeyUtil, LastNameUtil,
+                          MimeoUtil, RandomIntegerUtil, RandomItemUtil,
+                          RandomStringUtil)
 from .renderers import MimeoRenderer
 
-__all__ = ["AutoIncrementUtil", "CityUtil", "CountryUtil", "CurrentIterationUtil",
-           "DateTimeUtil", "DateUtil", "FirstNameUtil", "KeyUtil", "LastNameUtil",
-           "MimeoUtil", "RandomIntegerUtil", "RandomItemUtil", "RandomStringUtil",
-           "MimeoRenderer"]
+__all__ = ["AutoIncrementUtil", "CityUtil", "CountryUtil", "CurrencyUtil",
+           "CurrentIterationUtil", "DateTimeUtil", "DateUtil", "FirstNameUtil",
+           "KeyUtil", "LastNameUtil", "MimeoUtil", "RandomIntegerUtil",
+           "RandomItemUtil", "RandomStringUtil", "MimeoRenderer"]
```

### Comparing `mimeograph-0.5.0/src/mimeo/utils/mimeo_utils.py` & `mimeograph-0.6.0/src/mimeo/utils/mimeo_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,14 +19,16 @@
         A MimeoUtil implementation rendering a current iteration ID.
     * KeyUtil
         A MimeoUtil implementation rendering a unique identifier.
     * CityUtil
         A MimeoUtil implementation rendering city names.
     * CountryUtil
         A MimeoUtil implementation rendering country details.
+    * CurrencyUtil
+        A MimeoUtil implementation rendering currency details.
     * FirstNameUtil
         A MimeoUtil implementation rendering forenames.
     * LastNameUtil
         A MimeoUtil implementation rendering surnames.
 """
 from __future__ import annotations
 
@@ -34,15 +36,15 @@
 import string
 from abc import ABCMeta, abstractmethod
 from datetime import date, datetime, timedelta
 from typing import Any
 
 from mimeo.context import MimeoContext, MimeoContextManager
 from mimeo.context.decorators import mimeo_context
-from mimeo.database import Country, MimeoDB
+from mimeo.database import Country, Currency, MimeoDB
 from mimeo.database.exc import DataNotFoundError, InvalidSexError
 from mimeo.utils.exc import InvalidValueError
 
 
 class MimeoUtil(metaclass=ABCMeta):
     """A superclass for all Mimeo Utils.
 
@@ -125,15 +127,24 @@
     ) -> str:
         """Render a random string value.
 
         Returns
         -------
         str
             A random string value
+
+        Raises
+        ------
+        InvalidValueError
+            If the length param is negative
         """
+        if self._length < 0:
+            raise InvalidValueError(InvalidValueError.Code.ERR_1,
+                                    util=self.KEY,
+                                    length=self._length)
         return "".join(random.choice(string.ascii_letters) for _ in range(self._length))
 
 
 class RandomIntegerUtil(MimeoUtil):
     """A MimeoUtil implementation rendering a random integer value.
 
     Methods
@@ -174,15 +185,25 @@
     ) -> int:
         """Render a random integer value.
 
         Returns
         -------
         int
             A random integer value
+
+        Raises
+        ------
+        InvalidValueError
+            If the limit param is lower than start
         """
+        if self._start > self._limit:
+            raise InvalidValueError(InvalidValueError.Code.ERR_2,
+                                    util=self.KEY,
+                                    limit=self._limit,
+                                    start=self._start)
         return random.randrange(self._start, self._limit + 1)
 
 
 class RandomItemUtil(MimeoUtil):
     """A MimeoUtil implementation rendering a random item.
 
     Methods
@@ -386,25 +407,27 @@
         Returns
         -------
         str
             An auto incremented identifier in a parametrized format
 
         Raises
         ------
-        InvalidValue
+        InvalidValueError
             If the pattern is not a string value
         """
         try:
             identifier = context.next_id()
             return self._pattern.format(identifier)
         except AttributeError:
             context.prev_id()
-            msg = (f"The {self.KEY} Mimeo Util require a string value for the pattern "
-                   f"parameter and was: [{self._pattern}].")
-            raise InvalidValueError(msg) from AttributeError
+            raise InvalidValueError(InvalidValueError.Code.ERR_3,
+                                    util=self.KEY,
+                                    type="string",
+                                    param_name="pattern",
+                                    param_val=self._pattern) from AttributeError
 
 
 class CurrentIterationUtil(MimeoUtil):
     """A MimeoUtil implementation rendering a current iteration ID.
 
     It is a Mimeo Context-dependent Mimeo Util. Rendered ID value is
     pulled from the Context.
@@ -611,17 +634,18 @@
             else:
                 index = random.randrange(MimeoDB.NUM_OF_CITIES)
             city = self._MIMEO_DB.get_city_at(index)
         else:
             country_cities = self._MIMEO_DB.get_cities_of(self._country)
             country_cities_count = len(country_cities)
             if country_cities_count == 0:
-                msg = (f"Mimeo database doesn't contain any cities "
-                       f"of provided country [{self._country}].")
-                raise DataNotFoundError(msg)
+                raise DataNotFoundError(DataNotFoundError.Code.ERR_2,
+                                        data="city",
+                                        param_name="country",
+                                        param_val=self._country)
 
             if self._unique:
                 index = context.next_city_index(self._country)
             else:
                 index = random.randrange(country_cities_count)
             city = country_cities[index]
 
@@ -633,28 +657,29 @@
 
     It is a Mimeo Context-dependent Mimeo Util only when parametrized
     to generate unique country names.
 
     Methods
     -------
     render
-        Render a country name.
+        Render a country detail (name, ISO3 or ISO2 code).
 
     Attributes
     ----------
     KEY : str
         A Mimeo Util key
     """
 
     KEY = "country"
 
-    __VALUE_NAME = "name"
-    __VALUE_ISO3 = "iso3"
-    __VALUE_ISO2 = "iso2"
-    __MIMEO_DB = MimeoDB()
+    _VALUE_NAME = "name"
+    _VALUE_ISO3 = "iso3"
+    _VALUE_ISO2 = "iso2"
+    _SUPPORTED_VALUES = (_VALUE_NAME, _VALUE_ISO3, _VALUE_ISO2)
+    _MIMEO_DB = MimeoDB()
 
     def __init__(
             self,
             value: str = None,
             unique: bool = True,
             country: str = None,
             **kwargs,
@@ -670,15 +695,15 @@
             Indicates if rendered country names will be unique across
             a Mimeo Context
         country : str, default None
             A one country detail to get its other detail
         kwargs : dict
             Arbitrary keyword arguments (ignored)
         """
-        self._value = value if value is not None else self.__VALUE_NAME
+        self._value = value if value is not None else self._VALUE_NAME
         self._unique = unique
         self._country = country
 
     @mimeo_context
     def render(
             self,
             context: MimeoContext = None,
@@ -701,53 +726,165 @@
         Returns
         -------
         str
             A country detail
 
         Raises
         ------
-        InvalidValue
-            If the `country` parameter value is not supported
+        InvalidValueError
+            If the `value` parameter value is not supported
         OutOfStockError
             If all unique countries have been consumed already
         DataNotFoundError
             If database does not contain the provided `country`
         """
-        if self._value == self.__VALUE_NAME:
+        if self._value == self._VALUE_NAME:
             return self._get_country(context).name
-        if self._value == self.__VALUE_ISO3:
+        if self._value == self._VALUE_ISO3:
             return self._get_country(context).iso_3
-        if self._value == self.__VALUE_ISO2:
+        if self._value == self._VALUE_ISO2:
             return self._get_country(context).iso_2
-        msg = (f"The country Mimeo Util does not support a value [{self._value}]. "
-               f"Supported values are: {self.__VALUE_NAME} (default), "
-               f"{self.__VALUE_ISO3}, {self.__VALUE_ISO2}.")
-        raise InvalidValueError(msg)
+        raise InvalidValueError(InvalidValueError.Code.ERR_4,
+                                util=self.KEY,
+                                value=self._value,
+                                supported_values=self._SUPPORTED_VALUES)
 
     def _get_country(
             self,
             context: MimeoContext,
     ) -> Country:
         if self._country is not None:
-            countries = self.__MIMEO_DB.get_countries()
+            countries = self._MIMEO_DB.get_countries()
             country_found = next(
                 filter(lambda c: self._country in [c.name, c.iso_3, c.iso_2],
                        countries),
                 None,
             )
             if country_found is None:
-                msg = f"Mimeo database doesn't contain a country [{self._country}]."
-                raise DataNotFoundError(msg)
+                raise DataNotFoundError(DataNotFoundError.Code.ERR_1,
+                                        data="country",
+                                        value=self._country)
             return country_found
 
         if self._unique:
             index = context.next_country_index()
         else:
             index = random.randrange(MimeoDB.NUM_OF_COUNTRIES)
-        return self.__MIMEO_DB.get_country_at(index)
+        return self._MIMEO_DB.get_country_at(index)
+
+
+class CurrencyUtil(MimeoUtil):
+    """A MimeoUtil implementation rendering currency details.
+
+    It is a Mimeo Context-dependent Mimeo Util only when parametrized
+    to generate unique currency codes.
+
+    Methods
+    -------
+    render
+        Render a currency detail (code or name).
+
+    Attributes
+    ----------
+    KEY : str
+        A Mimeo Util key
+    """
+
+    KEY = "currency"
+
+    _VALUE_CODE = "code"
+    _VALUE_NAME = "name"
+    _SUPPORTED_VALUES = (_VALUE_CODE, _VALUE_NAME)
+    _MIMEO_DB = MimeoDB()
+
+    def __init__(
+            self,
+            value: str = None,
+            unique: bool = False,
+            country: str = None,
+            **kwargs,
+    ):
+        """Initialize CurrencyUtil class.
+
+        Parameters
+        ----------
+        value : str, default 'code'
+            Indicates which currency detail should be rendered:
+            code or name.
+        unique : bool, default False
+            Indicates if rendered currency codes will be unique across
+            a Mimeo Context
+        country : str, default None
+            A country of which the currency should be rendered
+        kwargs : dict
+            Arbitrary keyword arguments (ignored)
+        """
+        self._value = value if value is not None else self._VALUE_CODE
+        self._unique = unique
+        self._country = country
+
+    @mimeo_context
+    def render(
+            self,
+            context: MimeoContext = None,
+    ) -> str:
+        """Render a currency code.
+
+        By default, Currency Mimeo Util generates a non-unique currency code across
+        a Mimeo Context. If `value` is parametrized, then it will render a specific
+        currency detail (code or name). This Mimeo Util allows you to provide
+        a `country` to get a currency being used there. When `country` is parametrized,
+        then the 'unique' parameter is ignored.
+
+        Parameters
+        ----------
+        context : MimeoContext, default None
+            A current Mimeo Context injected by a decorator
+
+        Returns
+        -------
+        str
+            A currency code
+
+        Raises
+        ------
+        InvalidValueError
+            If the `value` parameter value is not supported
+        OutOfStockError
+            If all unique currencies have been consumed already
+        DataNotFoundError
+            If database does not contain a currency of the provided `country`
+        """
+        if self._value == self._VALUE_CODE:
+            return self._get_currency(context).code
+        if self._value == self._VALUE_NAME:
+            return self._get_currency(context).name
+        raise InvalidValueError(InvalidValueError.Code.ERR_4,
+                                util=self.KEY,
+                                value=self._value,
+                                supported_values=self._SUPPORTED_VALUES)
+
+    def _get_currency(
+            self,
+            context: MimeoContext,
+    ) -> Currency:
+        if self._country is None:
+            if self._unique:
+                index = context.next_currency_index()
+            else:
+                index = random.randrange(MimeoDB.NUM_OF_CURRENCIES)
+            currency = self._MIMEO_DB.get_currency_at(index)
+        else:
+            currency = self._MIMEO_DB.get_currency_of(self._country)
+            if currency is None:
+                raise DataNotFoundError(DataNotFoundError.Code.ERR_2,
+                                        data="currency",
+                                        param_name="country",
+                                        param_val=self._country)
+        return currency
 
 
 class FirstNameUtil(MimeoUtil):
     """A MimeoUtil implementation rendering forenames.
 
     It is a Mimeo Context-dependent Mimeo Util only when parametrized
     to generate unique forenames.
```

### Comparing `mimeograph-0.5.0/src/mimeo/utils/renderers.py` & `mimeograph-0.6.0/src/mimeo/utils/renderers.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,21 +13,22 @@
 """
 from __future__ import annotations
 
 import logging
 import re
 from typing import Any
 
-from mimeo.config import MimeoConfig
+from mimeo.config import constants as cc
 from mimeo.context import MimeoContext, MimeoContextManager
 from mimeo.context.decorators import mimeo_context
 from mimeo.utils import (AutoIncrementUtil, CityUtil, CountryUtil,
-                         CurrentIterationUtil, DateTimeUtil, DateUtil,
-                         FirstNameUtil, KeyUtil, LastNameUtil, MimeoUtil,
-                         RandomIntegerUtil, RandomItemUtil, RandomStringUtil)
+                         CurrencyUtil, CurrentIterationUtil, DateTimeUtil,
+                         DateUtil, FirstNameUtil, KeyUtil, LastNameUtil,
+                         MimeoUtil, RandomIntegerUtil, RandomItemUtil,
+                         RandomStringUtil)
 from mimeo.utils.exc import InvalidMimeoUtilError, NotASpecialFieldError
 
 logger = logging.getLogger(__name__)
 
 
 class UtilsRenderer:
     """A class rendering Mimeo Utils.
@@ -49,14 +50,15 @@
         DateUtil.KEY: DateUtil,
         DateTimeUtil.KEY: DateTimeUtil,
         AutoIncrementUtil.KEY: AutoIncrementUtil,
         CurrentIterationUtil.KEY: CurrentIterationUtil,
         KeyUtil.KEY: KeyUtil,
         CityUtil.KEY: CityUtil,
         CountryUtil.KEY: CountryUtil,
+        CurrencyUtil.KEY: CurrencyUtil,
         FirstNameUtil.KEY: FirstNameUtil,
         LastNameUtil.KEY: LastNameUtil,
     }
     _INSTANCES = {}
 
     @classmethod
     def render_raw(
@@ -73,21 +75,19 @@
         Returns
         -------
         Any
             Rendered Mimeo Util value.
 
         Raises
         ------
-        InvalidMimeoUtil
+        InvalidMimeoUtilError
             If the Mimeo Util name does not match any existing Mimeo
             Util.
         """
-        return cls.render_parametrized({
-            MimeoConfig.MODEL_MIMEO_UTIL_NAME_KEY: mimeo_util_key,
-        })
+        return cls.render_parametrized({cc.MODEL_MIMEO_UTIL_NAME_KEY: mimeo_util_key})
 
     @classmethod
     def render_parametrized(
             cls,
             mimeo_util_config: dict,
     ) -> Any:
         """Render a Mimeo Util in a parametrized form.
@@ -100,19 +100,19 @@
         Returns
         -------
         Any
             Rendered Mimeo Util value.
 
         Raises
         ------
-        InvalidMimeoUtil
+        InvalidMimeoUtilError
             If the Mimeo Util configuration does not include Mimeo
             Util name, or the parametrized name does not match any
             existing Mimeo Util.
-        InvalidValue
+        InvalidValueError
             If a Mimeo Util is incorrectly parametrized.
         InvalidSexError
             If the First Name Mimeo Util has not supported `sex`
             parameter value assigned.
         """
         logger.fine("Rendering a mimeo util [%s]", mimeo_util_config)
         mimeo_util = cls._get_mimeo_util(mimeo_util_config)
@@ -137,15 +137,15 @@
         Returns
         -------
         MimeoUtil
             A Mimeo Util instance
 
         Raises
         ------
-        InvalidMimeoUtil
+        InvalidMimeoUtilError
             If the Mimeo Util configuration does not include Mimeo
             Util name, or the parametrized name does not match any
             existing Mimeo Util.
         """
         cache_key = cls._generate_cache_key(config)
         if cache_key not in cls._INSTANCES:
             return cls._instantiate_mimeo_util(cache_key, config)
@@ -192,15 +192,15 @@
         Returns
         -------
         MimeoUtil
             A Mimeo Util instance
 
         Raises
         ------
-        InvalidMimeoUtil
+        InvalidMimeoUtilError
             If the Mimeo Util configuration does not include Mimeo
             Util name, or the parametrized name does not match any
             existing Mimeo Util.
         """
         mimeo_util_name = cls.get_mimeo_util_name(config)
         mimeo_util = cls.MIMEO_UTILS.get(mimeo_util_name)(**config)
         cls._INSTANCES[cache_key] = mimeo_util
@@ -221,26 +221,26 @@
         Returns
         -------
         str
             A Mimeo Util name
 
         Raises
         ------
-        InvalidMimeoUtil
+        InvalidMimeoUtilError
             If the Mimeo Util configuration does not include Mimeo
             Util name, or the parametrized name does not match any
             existing Mimeo Util.
         """
-        mimeo_util_name = config.get(MimeoConfig.MODEL_MIMEO_UTIL_NAME_KEY)
+        mimeo_util_name = config.get(cc.MODEL_MIMEO_UTIL_NAME_KEY)
         if mimeo_util_name is None:
-            msg = f"Missing Mimeo Util name in configuration [{config}]!"
-            raise InvalidMimeoUtilError(msg)
+            code = InvalidMimeoUtilError.Code.ERR_1
+            raise InvalidMimeoUtilError(code, config=config)
         if mimeo_util_name not in cls.MIMEO_UTILS:
-            msg = f"No such Mimeo Util [{mimeo_util_name}]!"
-            raise InvalidMimeoUtilError(msg)
+            code = InvalidMimeoUtilError.Code.ERR_2
+            raise InvalidMimeoUtilError(code, name=mimeo_util_name)
         return mimeo_util_name
 
 
 class VarsRenderer:
     """A class rendering Mimeo Vars.
 
     It contains only a class method.
@@ -266,15 +266,15 @@
         Returns
         -------
         Any
             A variable value
 
         Raises
         ------
-        InstanceNotAlive
+        InstanceNotAliveError
             If the MimeoContextManager instance is not alive
         VarNotFoundError
             If the Mimeo Var with the `var` provided does not exist
         """
         logger.fine("Rendering a variable [%s]", var)
         return MimeoContextManager().get_var(var)
 
@@ -360,15 +360,15 @@
         Returns
         -------
         str
             A special field name
 
         Raises
         ------
-        NotASpecialField
+        NotASpecialFieldError
             If the `wrapped_field_name` is not of form {:FIELD_NAME:}
         """
         if not cls.is_special_field(wrapped_field_name):
             raise NotASpecialFieldError(wrapped_field_name)
 
         return wrapped_field_name[2:][:-2]
 
@@ -430,15 +430,15 @@
         -------
         bool
             True if the value is a dictionary having only one key,
             "_mimeo_util". Otherwise, False.
         """
         return (isinstance(value, dict) and
                 len(value) == 1 and
-                MimeoConfig.MODEL_MIMEO_UTIL_KEY in value)
+                cc.MODEL_MIMEO_UTIL_KEY in value)
 
     @classmethod
     def render(
             cls,
             value: Any,
     ) -> Any:
         """Render a value.
@@ -460,24 +460,24 @@
         Returns
         -------
         Any
             A rendered value
 
         Raises
         ------
-        InstanceNotAlive
+        InstanceNotAliveError
             If the MimeoContextManager instance is not alive
         UninitializedContextIterationError
             If no iteration has been initialized yet for the context
         VarNotFoundError
             If the Mimeo Var does not exist
-        InvalidMimeoUtil
+        InvalidMimeoUtilError
             If the Mimeo Util node has missing _name property, or it
             does not match any Mimeo Util.
-        InvalidValue
+        InvalidValueError
             If Mimeo Util node is incorrectly parametrized
         OutOfStockError
             If all unique values have been consumed already
         DataNotFoundError
             If database does not contain the expected value
         InvalidSexError
             If the First Name Mimeo Util has not supported `sex`
@@ -578,15 +578,15 @@
         Returns
         -------
         Any
             A rendered value
 
         Raises
         ------
-        InstanceNotAlive
+        InstanceNotAliveError
             If the MimeoContextManager instance is not alive
         VarNotFoundError
             If the Mimeo Var with the `var` provided does not exist
         """
         match = next(cls._VARS_PATTERN.finditer(value))
         wrapped_var = match.group(1)
         r_val = VarsRenderer.render(wrapped_var[1:][:-1])
@@ -643,25 +643,25 @@
         Returns
         -------
         Any
             A rendered value
 
         Raises
         ------
-        InvalidValue
+        InvalidValueError
             If a Mimeo Util is incorrectly parametrized.
         OutOfStockError
             If all unique values have been consumed already
         DataNotFoundError
             If database does not contain the expected value
         InvalidSexError
             If the First Name Mimeo Util has not supported `sex`
             parameter value assigned.
         """
-        mimeo_util = value[MimeoConfig.MODEL_MIMEO_UTIL_KEY]
+        mimeo_util = value[cc.MODEL_MIMEO_UTIL_KEY]
         mimeo_util = cls._render_mimeo_util_parameters(mimeo_util)
         logger.fine("Pre-rendered mimeo util [%s]", mimeo_util)
         r_val = UtilsRenderer.render_parametrized(mimeo_util)
         return cls.render(r_val)
 
     @classmethod
     def _render_mimeo_util_parameters(
@@ -678,15 +678,15 @@
         Returns
         -------
         dict
             A Mimeo Util with pre-rendered parameters
 
         Raises
         ------
-        InvalidValue
+        InvalidValueError
             If a Mimeo Util is incorrectly parametrized.
         OutOfStockError
             If all unique values have been consumed already
         DataNotFoundError
             If database does not contain the expected value
         InvalidSexError
             If the First Name Mimeo Util has not supported `sex`
```

### Comparing `mimeograph-0.5.0/src/mimeograph.egg-info/PKG-INFO` & `mimeograph-0.6.0/src/mimeograph.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mimeograph
-Version: 0.5.0
+Version: 0.6.0
 Summary: Generate data based on a simple template
 Author-email: "T.A. Programming Svcs." <tomasz.maciej.aniolowski@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Tomasz Aniołowski
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -236,15 +236,14 @@
 #### Mimeo Environment
 
 To make `http` output directory easier to use, mimeo allows you to configure Mimeo Environments.
 They are configured in a JSON file (by default: mimeo.envs.json) and support the following output details:
 - `protocol`
 - `host`
 - `port`
-- `auth`
 - `username`
 - `password`
 
 Example
 ```json
 {
     "local": {
@@ -253,15 +252,14 @@
         "username": "admin",
         "password": "admin"
     },
     "dev": {
         "protocol": "https",
         "host": "11.111.11.111",
         "port": 8000,
-        "auth": "digest",
         "username": "some-user",
         "password": "some-password"
     }
 }
 ```
 
 To use a specific Mimeo Environment you can use the following commands:
@@ -352,14 +350,18 @@
 
 You can use several predefined functions to generate data. They can be used in a _raw_ format or _parametrized_.
 
 ##### Random String
 
 Generates a random string value.
 
+| Parameter | Supported values | Default |
+|:---------:|:----------------:|:-------:|
+|  length   |      `int`       |  `20`   |
+
 ###### Raw
 
 Uses the default length: 20 characters.
 
 ```json
 {
   "randomstring": "{random_str}"
@@ -381,14 +383,19 @@
 }
 ```
 
 ##### Random Integer
 
 Generates a random integer value between `start` and `limit` parameters (inclusive).
 
+| Parameter | Supported values | Default |
+|:---------:|:----------------:|:-------:|
+|   start   |      `int`       |   `1`   |
+|   limit   |      `int`       |  `100`  |
+
 ###### Raw
 
 Uses the default start (1) and limit (100) values.
 
 ```json
 {
   "randominteger": "{random_int}"
@@ -424,14 +431,18 @@
 ```
 
 ##### Random Item
 
 Generates a random value from items provided.  
 NOTICE: The raw form of this Mimeo Util will generate a blank string value (as same as no items parametrized).
 
+| Parameter | Supported values | Default |
+|:---------:|:----------------:|:-------:|
+|   items   |      `list`      | `[""]`  |
+
 ###### Parametrized
 
 ```json
 {
   "random": {
     "_mimeo_util": {
       "_name": "random_item",
@@ -441,14 +452,18 @@
 }
 ```
 
 ##### Date
 
 Generates a date value in format `YYYY-MM-DD`.
 
+| Parameter  | Supported values | Default |
+|:----------:|:----------------:|:-------:|
+| days_delta |      `int`       |   `0`   |
+
 ###### Raw
 
 Uses the today's date.
 
 ```json
 {
   "Today": "{date}"
@@ -476,14 +491,21 @@
 }
 ```
 
 ##### Date Time
 
 Generates a date time value in format `YYYY-MM-DD'T'HH:mm:SS`.
 
+|   Parameter   | Supported values | Default |
+|:-------------:|:----------------:|:-------:|
+|  days_delta   |      `int`       |   `0`   |
+|  hours_delta  |      `int`       |   `0`   |
+| minutes_delta |      `int`       |   `0`   |
+| seconds_delta |      `int`       |   `0`   |
+
 ###### Raw
 
 Uses the current timestamp.
 
 ```json
 {
   "Now": "{date_time}"
@@ -508,14 +530,18 @@
 }
 ```
 
 ##### Auto Increment
 
 Generates a next integer in context of a model (in nested templates it will use a separated context).
 
+| Parameter | Supported values | Default  |
+|:---------:|:----------------:|:--------:|
+|  pattern  |      `str`       | `{:05d}` |
+
 ###### Raw
 
 Uses a default pattern: **{:05d}** (an integer with 5 leading zeros).
 
 ```json
 {
   "ID": "{auto_increment}"
@@ -537,14 +563,18 @@
 }
 ```
 
 ##### Current Iteration
 
 Generates a value of the current iteration in a Mimeo Template context.
 
+| Parameter | Supported values |      Default      |
+|:---------:|:----------------:|:-----------------:|
+|  context  |      `str`       | a current context |
+
 ###### Raw
 
 Uses the current context.
 
 ```json
 {
   "ID": "{curr_iter}"
@@ -566,14 +596,19 @@
 }
 ```
 
 ##### Key
 
 Generates a key unique across all Mimeo Models and being the same within a single Mimeo Model context.
 
+| Parameter | Supported values |              Default               |
+|:---------:|:----------------:|:----------------------------------:|
+|  context  |      `str`       |         a current context          |
+| iteration |      `int`       | a current iteration of the context |
+
 ###### Raw
 
 Uses a key from the current context and iteration.
 
 ```json
 {
   "ID": "{key}"
@@ -583,28 +618,33 @@
 ###### Parametrized
 
 Uses a key from the specific context and iteration.  
 When context is indicated and iteration is not, then the current iteration **of the indicated context** is being used.
 
 ```json
 {
-  "SomeEntity": {
+  "SomeEntity2": {
     "_mimeo_util": {
       "_name": "key",
       "context": "SomeEntity",
       "iteration": "{curr_iter}"
     }
   }
 }
 ```
 
 ##### City
 
 Generates a city name.
 
+| Parameter | Supported values | Default |
+|:---------:|:----------------:|:-------:|
+|  unique   |      `bool`      | `True`  |
+|  country  |      `str`       | `None`  |
+
 ###### Raw
 
 By default city names will be unique across a Mimeo Context.
 
 ```json
 {
   "City": "{city}"
@@ -651,14 +691,20 @@
 }
 ```
 
 ##### Country
 
 Generates a country name (by default), iso2 or iso3.
 
+| Parameter |       Supported values       | Default  |
+|:---------:|:----------------------------:|:--------:|
+|  unique   |            `bool`            |  `True`  |
+|   value   | `"name"`, `"iso3"`, `"iso2"` | `"name"` |
+|  country  |            `str`             |  `None`  |
+
 ###### Raw
 
 By default country names will be unique across a Mimeo Context.
 
 ```json
 {
   "Country": "{country}"
@@ -708,18 +754,89 @@
       "value": "iso2",
       "country": "United Kingdom"
     }
   }
 }
 ```
 
+##### Currency
+
+Generates a currency code (by default) or name.
+
+| Parameter |  Supported values  | Default  |
+|:---------:|:------------------:|:--------:|
+|  unique   |       `bool`       | `False`  |
+|   value   | `"code"`, `"name"` | `"code"` |
+|  country  |       `str`        |  `None`  |
+
+###### Raw
+
+By default city names will _NOT_ be unique across a Mimeo Context.
+
+```json
+{
+  "Currency": "{currency}"
+}
+```
+
+###### Parametrized
+
+It can generate:
+- unique currencies
+- currency name instead of code
+- currency code or name of a specific country (using iso3, iso2 or name)
+
+When the `country` param is provided then the `unique` flag is ignored.
+
+```json
+{
+  "UniqueCurrencyCode": {
+    "_mimeo_util": {
+      "_name": "currency",
+      "unique": true
+    }
+  },
+  "CurrencyName": {
+    "_mimeo_util": {
+      "_name": "currency",
+      "value": "name"
+    }
+  },
+  "CurrencyCodeForCountryISO3": {
+    "_mimeo_util": {
+      "_name": "currency",
+      "country": "GBR"
+    }
+  },
+  "CurrencyNameForCountryISO2": {
+    "_mimeo_util": {
+      "_name": "currency",
+      "value": "name",
+      "country": "GB"
+    }
+  },
+  "CurrencyNameForCountryName": {
+    "_mimeo_util": {
+      "_name": "currency",
+      "value": "name",
+      "country": "United Kingdom"
+    }
+  }
+}
+```
+
 ##### First Name
 
 Generates a first name.
 
+| Parameter |      Supported values      | Default  |
+|:---------:|:--------------------------:|:--------:|
+|  unique   |           `bool`           |  `True`  |
+|    sex    | `M`, `Male`, `F`, `Female` |  `None`  |
+
 ###### Raw
 
 By default first names will be unique across a Mimeo Context.
 
 ```json
 {
   "FirstName": "{first_name}"
@@ -760,14 +877,18 @@
 }
 ```
 
 ##### Last Name
 
 Generates a last name.
 
+| Parameter | Supported values | Default  |
+|:---------:|:----------------:|:--------:|
+|  unique   |      `bool`      |  `True`  |
+
 ###### Raw
 
 By default last names will be unique across a Mimeo Context.
 
 ```json
 {
   "LastName": "{last_name}"
```

### Comparing `mimeograph-0.5.0/src/mimeograph.egg-info/SOURCES.txt` & `mimeograph-0.6.0/src/mimeograph.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 src/mimeo/mimeo.py
 src/mimeo/tools.py
 src/mimeo/cli/__init__.py
 src/mimeo/cli/exc.py
 src/mimeo/cli/job.py
 src/mimeo/cli/parsers.py
 src/mimeo/config/__init__.py
+src/mimeo/config/constants.py
 src/mimeo/config/exc.py
 src/mimeo/config/mimeo_config.py
 src/mimeo/consumers/__init__.py
 src/mimeo/consumers/consumer.py
 src/mimeo/consumers/consumer_factory.py
 src/mimeo/consumers/file_consumer.py
 src/mimeo/consumers/http_consumer.py
@@ -24,14 +25,15 @@
 src/mimeo/context/exc.py
 src/mimeo/context/mimeo_context.py
 src/mimeo/context/mimeo_context_manager.py
 src/mimeo/context/mimeo_iteration.py
 src/mimeo/database/__init__.py
 src/mimeo/database/cities.py
 src/mimeo/database/countries.py
+src/mimeo/database/currencies.py
 src/mimeo/database/exc.py
 src/mimeo/database/first_names.py
 src/mimeo/database/last_names.py
 src/mimeo/database/mimeo_db.py
 src/mimeo/generators/__init__.py
 src/mimeo/generators/exc.py
 src/mimeo/generators/generator.py
@@ -40,15 +42,17 @@
 src/mimeo/logging/__init__.py
 src/mimeo/logging/filters.py
 src/mimeo/meta/__init__.py
 src/mimeo/meta/alive.py
 src/mimeo/meta/exc.py
 src/mimeo/resources/__init__.py
 src/mimeo/resources/cities.csv
+src/mimeo/resources/constants.yaml
 src/mimeo/resources/countries.csv
+src/mimeo/resources/currencies.csv
 src/mimeo/resources/exc.py
 src/mimeo/resources/forenames.csv
 src/mimeo/resources/logging.yaml
 src/mimeo/resources/surnames.txt
 src/mimeo/utils/__init__.py
 src/mimeo/utils/exc.py
 src/mimeo/utils/mimeo_utils.py
```

### Comparing `mimeograph-0.5.0/tests/test_mimeograph.py` & `mimeograph-0.6.0/tests/test_mimeograph.py`

 * *Files identical despite different names*

