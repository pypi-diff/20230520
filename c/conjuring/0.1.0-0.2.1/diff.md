# Comparing `tmp/conjuring-0.1.0.tar.gz` & `tmp/conjuring-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conjuring-0.1.0.tar", max compression
+gzip compressed data, was "conjuring-0.2.1.tar", max compression
```

## Comparing `conjuring-0.1.0.tar` & `conjuring-0.2.1.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0     1040 2023-05-19 23:48:19.089703 conjuring-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-19 23:48:19.089703 conjuring-0.1.0/src/conjuring/__init__.py
--rw-r--r--   0        0        0      541 2023-05-19 23:48:19.089703 conjuring-0.1.0/src/conjuring/colors.py
--rw-r--r--   0        0        0      313 2023-05-19 23:48:19.089703 conjuring-0.1.0/src/conjuring/constants.py
--rw-r--r--   0        0        0     9079 2023-05-19 23:48:19.093704 conjuring-0.1.0/src/conjuring/grimoire.py
--rw-r--r--   0        0        0        0 2023-05-19 23:48:19.093704 conjuring-0.1.0/src/conjuring/spells/__init__.py
--rw-r--r--   0        0        0     2207 2023-05-19 23:48:19.093704 conjuring-0.1.0/src/conjuring/spells/aws.py
--rw-r--r--   0        0        0     3001 2023-05-19 23:48:19.093704 conjuring-0.1.0/src/conjuring/spells/blanket.py
--rw-r--r--   0        0        0     1437 2023-05-19 23:48:19.093704 conjuring-0.1.0/src/conjuring/spells/conjuring.py
--rw-r--r--   0        0        0     1078 2023-05-19 23:48:19.093704 conjuring-0.1.0/src/conjuring/spells/default.py
--rw-r--r--   0        0        0     1239 2023-05-19 23:48:19.093704 conjuring-0.1.0/src/conjuring/spells/docker.py
--rw-r--r--   0        0        0     1725 2023-05-19 23:48:19.093704 conjuring-0.1.0/src/conjuring/spells/duplicity.py
--rw-r--r--   0        0        0      470 2023-05-19 23:48:19.093704 conjuring-0.1.0/src/conjuring/spells/empty.py
--rw-r--r--   0        0        0     1000 2023-05-19 23:48:19.093704 conjuring-0.1.0/src/conjuring/spells/fork.py
--rw-r--r--   0        0        0    14739 2023-05-19 23:48:19.093704 conjuring-0.1.0/src/conjuring/spells/git.py
--rw-r--r--   0        0        0     1008 2023-05-19 23:48:19.093704 conjuring-0.1.0/src/conjuring/spells/jrnl.py
--rw-r--r--   0        0        0     2851 2023-05-19 23:48:19.093704 conjuring-0.1.0/src/conjuring/spells/k8s.py
--rw-r--r--   0        0        0     7044 2023-05-19 23:48:19.093704 conjuring-0.1.0/src/conjuring/spells/media.py
--rw-r--r--   0        0        0      764 2023-05-19 23:48:19.093704 conjuring-0.1.0/src/conjuring/spells/mkdocs.py
--rw-r--r--   0        0        0     2695 2023-05-19 23:48:19.093704 conjuring-0.1.0/src/conjuring/spells/mr.py
--rw-r--r--   0        0        0      824 2023-05-19 23:48:19.093704 conjuring-0.1.0/src/conjuring/spells/onedrive.py
--rw-r--r--   0        0        0    11455 2023-05-19 23:48:19.093704 conjuring-0.1.0/src/conjuring/spells/paperless.py
--rw-r--r--   0        0        0     2721 2023-05-19 23:48:19.093704 conjuring-0.1.0/src/conjuring/spells/pre_commit.py
--rw-r--r--   0        0        0     6741 2023-05-19 23:48:19.093704 conjuring-0.1.0/src/conjuring/spells/py.py
--rw-r--r--   0        0        0     1092 2023-05-19 23:48:19.093704 conjuring-0.1.0/src/conjuring/spells/shell.py
--rw-r--r--   0        0        0     1882 2023-05-19 23:48:19.093704 conjuring-0.1.0/src/conjuring/visibility.py
--rw-r--r--   0        0        0      545 1970-01-01 00:00:00.000000 conjuring-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1481 2023-05-20 00:33:29.136280 conjuring-0.2.1/docs/README.md
+-rw-r--r--   0        0        0     1576 2023-05-20 00:33:29.136280 conjuring-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-20 00:33:29.136280 conjuring-0.2.1/src/conjuring/__init__.py
+-rw-r--r--   0        0        0      541 2023-05-20 00:33:29.136280 conjuring-0.2.1/src/conjuring/colors.py
+-rw-r--r--   0        0        0      313 2023-05-20 00:33:29.136280 conjuring-0.2.1/src/conjuring/constants.py
+-rw-r--r--   0        0        0     9079 2023-05-20 00:33:29.136280 conjuring-0.2.1/src/conjuring/grimoire.py
+-rw-r--r--   0        0        0        0 2023-05-20 00:33:29.136280 conjuring-0.2.1/src/conjuring/spells/__init__.py
+-rw-r--r--   0        0        0     2207 2023-05-20 00:33:29.136280 conjuring-0.2.1/src/conjuring/spells/aws.py
+-rw-r--r--   0        0        0     3001 2023-05-20 00:33:29.136280 conjuring-0.2.1/src/conjuring/spells/blanket.py
+-rw-r--r--   0        0        0     1437 2023-05-20 00:33:29.136280 conjuring-0.2.1/src/conjuring/spells/conjuring.py
+-rw-r--r--   0        0        0     1078 2023-05-20 00:33:29.136280 conjuring-0.2.1/src/conjuring/spells/default.py
+-rw-r--r--   0        0        0     1239 2023-05-20 00:33:29.136280 conjuring-0.2.1/src/conjuring/spells/docker.py
+-rw-r--r--   0        0        0     1725 2023-05-20 00:33:29.136280 conjuring-0.2.1/src/conjuring/spells/duplicity.py
+-rw-r--r--   0        0        0      470 2023-05-20 00:33:29.136280 conjuring-0.2.1/src/conjuring/spells/empty.py
+-rw-r--r--   0        0        0     1000 2023-05-20 00:33:29.136280 conjuring-0.2.1/src/conjuring/spells/fork.py
+-rw-r--r--   0        0        0    14739 2023-05-20 00:33:29.140280 conjuring-0.2.1/src/conjuring/spells/git.py
+-rw-r--r--   0        0        0     1008 2023-05-20 00:33:29.140280 conjuring-0.2.1/src/conjuring/spells/jrnl.py
+-rw-r--r--   0        0        0     2851 2023-05-20 00:33:29.140280 conjuring-0.2.1/src/conjuring/spells/k8s.py
+-rw-r--r--   0        0        0     7044 2023-05-20 00:33:29.140280 conjuring-0.2.1/src/conjuring/spells/media.py
+-rw-r--r--   0        0        0      764 2023-05-20 00:33:29.140280 conjuring-0.2.1/src/conjuring/spells/mkdocs.py
+-rw-r--r--   0        0        0     2695 2023-05-20 00:33:29.140280 conjuring-0.2.1/src/conjuring/spells/mr.py
+-rw-r--r--   0        0        0      824 2023-05-20 00:33:29.140280 conjuring-0.2.1/src/conjuring/spells/onedrive.py
+-rw-r--r--   0        0        0    11455 2023-05-20 00:33:29.140280 conjuring-0.2.1/src/conjuring/spells/paperless.py
+-rw-r--r--   0        0        0     2721 2023-05-20 00:33:29.140280 conjuring-0.2.1/src/conjuring/spells/pre_commit.py
+-rw-r--r--   0        0        0     6741 2023-05-20 00:33:29.140280 conjuring-0.2.1/src/conjuring/spells/py.py
+-rw-r--r--   0        0        0     1092 2023-05-20 00:33:29.140280 conjuring-0.2.1/src/conjuring/spells/shell.py
+-rw-r--r--   0        0        0     1882 2023-05-20 00:33:29.140280 conjuring-0.2.1/src/conjuring/visibility.py
+-rw-r--r--   0        0        0     2599 1970-01-01 00:00:00.000000 conjuring-0.2.1/PKG-INFO
```

### Comparing `conjuring-0.1.0/src/conjuring/colors.py` & `conjuring-0.2.1/src/conjuring/colors.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.1.0/src/conjuring/grimoire.py` & `conjuring-0.2.1/src/conjuring/grimoire.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.1.0/src/conjuring/spells/aws.py` & `conjuring-0.2.1/src/conjuring/spells/aws.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.1.0/src/conjuring/spells/blanket.py` & `conjuring-0.2.1/src/conjuring/spells/blanket.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.1.0/src/conjuring/spells/conjuring.py` & `conjuring-0.2.1/src/conjuring/spells/conjuring.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.1.0/src/conjuring/spells/default.py` & `conjuring-0.2.1/src/conjuring/spells/default.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.1.0/src/conjuring/spells/docker.py` & `conjuring-0.2.1/src/conjuring/spells/docker.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.1.0/src/conjuring/spells/duplicity.py` & `conjuring-0.2.1/src/conjuring/spells/duplicity.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.1.0/src/conjuring/spells/fork.py` & `conjuring-0.2.1/src/conjuring/spells/fork.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.1.0/src/conjuring/spells/git.py` & `conjuring-0.2.1/src/conjuring/spells/git.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.1.0/src/conjuring/spells/jrnl.py` & `conjuring-0.2.1/src/conjuring/spells/jrnl.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.1.0/src/conjuring/spells/k8s.py` & `conjuring-0.2.1/src/conjuring/spells/k8s.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.1.0/src/conjuring/spells/media.py` & `conjuring-0.2.1/src/conjuring/spells/media.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.1.0/src/conjuring/spells/mkdocs.py` & `conjuring-0.2.1/src/conjuring/spells/mkdocs.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.1.0/src/conjuring/spells/mr.py` & `conjuring-0.2.1/src/conjuring/spells/mr.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.1.0/src/conjuring/spells/onedrive.py` & `conjuring-0.2.1/src/conjuring/spells/onedrive.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.1.0/src/conjuring/spells/paperless.py` & `conjuring-0.2.1/src/conjuring/spells/paperless.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.1.0/src/conjuring/spells/pre_commit.py` & `conjuring-0.2.1/src/conjuring/spells/pre_commit.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.1.0/src/conjuring/spells/py.py` & `conjuring-0.2.1/src/conjuring/spells/py.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.1.0/src/conjuring/spells/shell.py` & `conjuring-0.2.1/src/conjuring/spells/shell.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.1.0/src/conjuring/visibility.py` & `conjuring-0.2.1/src/conjuring/visibility.py`

 * *Files identical despite different names*

