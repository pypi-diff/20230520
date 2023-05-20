# Comparing `tmp/apeek-0.0.1.tar.gz` & `tmp/apeek-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apeek-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "apeek-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `apeek-0.0.1.tar` & `apeek-0.1.0.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0      231 2023-05-20 00:42:15.969484 apeek-0.0.1/README.md
--rw-r--r--   0        0        0     2910 2023-05-20 00:42:15.969484 apeek-0.0.1/apeek/__init__.py
--rw-r--r--   0        0        0     1761 2023-05-20 00:42:15.969484 apeek-0.0.1/apeek/__main__.py
--rw-r--r--   0        0        0     1635 2023-05-20 00:42:15.973484 apeek-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1148 1970-01-01 00:00:00.000000 apeek-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2653 2023-05-20 03:19:21.967235 apeek-0.1.0/README.md
+-rw-r--r--   0        0        0     1325 2023-05-20 03:19:21.967235 apeek-0.1.0/apeek/__init__.py
+-rw-r--r--   0        0        0     2423 2023-05-20 03:19:21.967235 apeek-0.1.0/apeek/__main__.py
+-rw-r--r--   0        0        0     2246 2023-05-20 03:19:21.967235 apeek-0.1.0/apeek/waveform.py
+-rw-r--r--   0        0        0     1635 2023-05-20 03:19:21.967235 apeek-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3570 1970-01-01 00:00:00.000000 apeek-0.1.0/PKG-INFO
```

### Comparing `apeek-0.0.1/pyproject.toml` & `apeek-0.1.0/pyproject.toml`

 * *Files identical despite different names*

