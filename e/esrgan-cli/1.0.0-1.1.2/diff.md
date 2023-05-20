# Comparing `tmp/esrgan-cli-1.0.0.tar.gz` & `tmp/esrgan-cli-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esrgan-cli-1.0.0.tar", last modified: Thu May 18 06:38:29 2023, max compression
+gzip compressed data, was "esrgan-cli-1.1.2.tar", last modified: Sat May 20 02:18:49 2023, max compression
```

## Comparing `esrgan-cli-1.0.0.tar` & `esrgan-cli-1.1.2.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:38:29.110358 esrgan-cli-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      135 2023-05-18 06:38:29.110358 esrgan-cli-1.0.0/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)      603 2023-05-18 06:36:17.000000 esrgan-cli-1.0.0/esrgan.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 06:38:29.110358 esrgan-cli-1.0.0/esrgan_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)      135 2023-05-18 06:38:28.000000 esrgan-cli-1.0.0/esrgan_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      241 2023-05-18 06:38:28.000000 esrgan-cli-1.0.0/esrgan_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 06:38:28.000000 esrgan-cli-1.0.0/esrgan_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-05-18 06:38:28.000000 esrgan-cli-1.0.0/esrgan_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-18 06:38:28.000000 esrgan-cli-1.0.0/esrgan_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-18 06:38:28.000000 esrgan-cli-1.0.0/esrgan_cli.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      530 2023-05-18 06:36:28.000000 esrgan-cli-1.0.0/esrgan_client.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-18 06:38:29.110358 esrgan-cli-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      376 2023-05-18 06:38:17.000000 esrgan-cli-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 02:18:49.697708 esrgan-cli-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-20 02:18:36.000000 esrgan-cli-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-20 02:18:49.697708 esrgan-cli-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-20 02:18:36.000000 esrgan-cli-1.1.2/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      603 2023-05-20 02:18:36.000000 esrgan-cli-1.1.2/esrgan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 02:18:49.697708 esrgan-cli-1.1.2/esrgan_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-20 02:18:49.000000 esrgan-cli-1.1.2/esrgan_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-20 02:18:49.000000 esrgan-cli-1.1.2/esrgan_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 02:18:49.000000 esrgan-cli-1.1.2/esrgan_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-20 02:18:49.000000 esrgan-cli-1.1.2/esrgan_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-20 02:18:49.000000 esrgan-cli-1.1.2/esrgan_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-20 02:18:49.000000 esrgan-cli-1.1.2/esrgan_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-20 02:18:36.000000 esrgan-cli-1.1.2/esrgan_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 02:18:49.697708 esrgan-cli-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-20 02:18:36.000000 esrgan-cli-1.1.2/setup.py
```

### Comparing `esrgan-cli-1.0.0/esrgan.py` & `esrgan-cli-1.1.2/esrgan.py`

 * *Files identical despite different names*

### Comparing `esrgan-cli-1.0.0/esrgan_client.py` & `esrgan-cli-1.1.2/esrgan_client.py`

 * *Files identical despite different names*

