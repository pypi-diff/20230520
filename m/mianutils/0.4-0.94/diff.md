# Comparing `tmp/mianutils-0.4.tar.gz` & `tmp/mianutils-0.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mianutils-0.4.tar", last modified: Sat May 20 19:12:31 2023, max compression
+gzip compressed data, was "mianutils-0.94.tar", last modified: Thu Sep 22 17:14:16 2022, max compression
```

## Comparing `mianutils-0.4.tar` & `mianutils-0.94.tar`

### file list

```diff
@@ -1,11 +1,9 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 19:12:31.376280 mianutils-0.4/
--rw-rw-rw-   0        0        0      712 2023-05-20 19:12:31.376280 mianutils-0.4/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-20 18:59:06.000000 mianutils-0.4/license.txt
-drwxrwxrwx   0        0        0        0 2023-05-20 19:12:31.374278 mianutils-0.4/mianutils.egg-info/
--rw-rw-rw-   0        0        0      712 2023-05-20 19:12:31.000000 mianutils-0.4/mianutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      194 2023-05-20 19:12:31.000000 mianutils-0.4/mianutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 19:12:31.000000 mianutils-0.4/mianutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-05-20 19:12:31.000000 mianutils-0.4/mianutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-20 19:12:31.000000 mianutils-0.4/mianutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-20 19:12:31.377282 mianutils-0.4/setup.cfg
--rw-rw-rw-   0        0        0     4029 2023-05-20 19:12:13.000000 mianutils-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2022-09-22 17:14:16.023280 mianutils-0.94/
+-rw-rw-rw-   0        0        0      151 2022-09-22 17:14:16.023280 mianutils-0.94/PKG-INFO
+drwxrwxrwx   0        0        0        0 2022-09-22 17:14:16.022282 mianutils-0.94/mianutils.egg-info/
+-rw-rw-rw-   0        0        0      151 2022-09-22 17:14:15.000000 mianutils-0.94/mianutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      150 2022-09-22 17:14:16.000000 mianutils-0.94/mianutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-09-22 17:14:15.000000 mianutils-0.94/mianutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2022-09-22 17:14:15.000000 mianutils-0.94/mianutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      116 2022-09-22 17:14:16.028264 mianutils-0.94/setup.cfg
+-rw-rw-rw-   0        0        0      513 2022-09-22 17:14:03.000000 mianutils-0.94/setup.py
```

