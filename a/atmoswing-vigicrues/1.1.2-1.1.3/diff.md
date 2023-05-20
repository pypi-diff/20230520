# Comparing `tmp/atmoswing-vigicrues-1.1.2.tar.gz` & `tmp/atmoswing-vigicrues-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atmoswing-vigicrues-1.1.2.tar", last modified: Tue May 16 22:22:26 2023, max compression
+gzip compressed data, was "atmoswing-vigicrues-1.1.3.tar", last modified: Sat May 20 13:18:21 2023, max compression
```

## Comparing `atmoswing-vigicrues-1.1.2.tar` & `atmoswing-vigicrues-1.1.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:22:26.529282 atmoswing-vigicrues-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-16 22:22:06.000000 atmoswing-vigicrues-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-05-16 22:22:26.529282 atmoswing-vigicrues-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-16 22:22:06.000000 atmoswing-vigicrues-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-16 22:22:06.000000 atmoswing-vigicrues-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-16 22:22:26.529282 atmoswing-vigicrues-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-16 22:22:06.000000 atmoswing-vigicrues-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:22:26.521282 atmoswing-vigicrues-1.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:22:26.525282 atmoswing-vigicrues-1.1.2/src/atmoswing_vigicrues/
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-16 22:22:06.000000 atmoswing-vigicrues-1.1.2/src/atmoswing_vigicrues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-16 22:22:06.000000 atmoswing-vigicrues-1.1.2/src/atmoswing_vigicrues/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11414 2023-05-16 22:22:06.000000 atmoswing-vigicrues-1.1.2/src/atmoswing_vigicrues/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:22:26.525282 atmoswing-vigicrues-1.1.2/src/atmoswing_vigicrues/disseminations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 22:22:06.000000 atmoswing-vigicrues-1.1.2/src/atmoswing_vigicrues/disseminations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-16 22:22:06.000000 atmoswing-vigicrues-1.1.2/src/atmoswing_vigicrues/disseminations/dissemination.py
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-05-16 22:22:06.000000 atmoswing-vigicrues-1.1.2/src/atmoswing_vigicrues/disseminations/transfer_sftp_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-05-16 22:22:06.000000 atmoswing-vigicrues-1.1.2/src/atmoswing_vigicrues/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-16 22:22:06.000000 atmoswing-vigicrues-1.1.2/src/atmoswing_vigicrues/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:22:26.525282 atmoswing-vigicrues-1.1.2/src/atmoswing_vigicrues/postactions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 22:22:06.000000 atmoswing-vigicrues-1.1.2/src/atmoswing_vigicrues/postactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12451 2023-05-16 22:22:06.000000 atmoswing-vigicrues-1.1.2/src/atmoswing_vigicrues/postactions/export_bdapbp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8460 2023-05-16 22:22:06.000000 atmoswing-vigicrues-1.1.2/src/atmoswing_vigicrues/postactions/export_prv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-16 22:22:06.000000 atmoswing-vigicrues-1.1.2/src/atmoswing_vigicrues/postactions/postaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:22:26.529282 atmoswing-vigicrues-1.1.2/src/atmoswing_vigicrues/preactions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 22:22:06.000000 atmoswing-vigicrues-1.1.2/src/atmoswing_vigicrues/preactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8123 2023-05-16 22:22:06.000000 atmoswing-vigicrues-1.1.2/src/atmoswing_vigicrues/preactions/download_gfs.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-16 22:22:06.000000 atmoswing-vigicrues-1.1.2/src/atmoswing_vigicrues/preactions/preaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     8105 2023-05-16 22:22:06.000000 atmoswing-vigicrues-1.1.2/src/atmoswing_vigicrues/preactions/transfer_sftp_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-05-16 22:22:06.000000 atmoswing-vigicrues-1.1.2/src/atmoswing_vigicrues/preactions/transform_ecmwf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-05-16 22:22:06.000000 atmoswing-vigicrues-1.1.2/src/atmoswing_vigicrues/preactions/transform_gfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-05-16 22:22:06.000000 atmoswing-vigicrues-1.1.2/src/atmoswing_vigicrues/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:22:26.525282 atmoswing-vigicrues-1.1.2/src/atmoswing_vigicrues.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-05-16 22:22:26.000000 atmoswing-vigicrues-1.1.2/src/atmoswing_vigicrues.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-16 22:22:26.000000 atmoswing-vigicrues-1.1.2/src/atmoswing_vigicrues.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 22:22:26.000000 atmoswing-vigicrues-1.1.2/src/atmoswing_vigicrues.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-16 22:22:26.000000 atmoswing-vigicrues-1.1.2/src/atmoswing_vigicrues.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-16 22:22:26.000000 atmoswing-vigicrues-1.1.2/src/atmoswing_vigicrues.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:22:26.529282 atmoswing-vigicrues-1.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-05-16 22:22:06.000000 atmoswing-vigicrues-1.1.2/tests/test_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-05-16 22:22:06.000000 atmoswing-vigicrues-1.1.2/tests/test_download_gfs.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-16 22:22:06.000000 atmoswing-vigicrues-1.1.2/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-16 22:22:06.000000 atmoswing-vigicrues-1.1.2/tests/test_export_bdapbp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-16 22:22:06.000000 atmoswing-vigicrues-1.1.2/tests/test_export_prv.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-16 22:22:06.000000 atmoswing-vigicrues-1.1.2/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-16 22:22:06.000000 atmoswing-vigicrues-1.1.2/tests/test_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-05-16 22:22:06.000000 atmoswing-vigicrues-1.1.2/tests/test_transfer_sftp_in.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-16 22:22:06.000000 atmoswing-vigicrues-1.1.2/tests/test_transfer_sftp_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-16 22:22:06.000000 atmoswing-vigicrues-1.1.2/tests/test_transform_gfs.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-16 22:22:06.000000 atmoswing-vigicrues-1.1.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:18:21.041803 atmoswing-vigicrues-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-05-20 13:18:21.041803 atmoswing-vigicrues-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-20 13:18:21.045803 atmoswing-vigicrues-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:18:21.037803 atmoswing-vigicrues-1.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:18:21.037803 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11414 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:18:21.041803 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/disseminations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/disseminations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/disseminations/dissemination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/disseminations/transfer_sftp_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:18:21.041803 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/postactions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/postactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12451 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/postactions/export_bdapbp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8460 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/postactions/export_prv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/postactions/postaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:18:21.041803 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/preactions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/preactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8123 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/preactions/download_gfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/preactions/preaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8105 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/preactions/transfer_sftp_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/preactions/transform_ecmwf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/preactions/transform_gfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:18:21.041803 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-05-20 13:18:21.000000 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-20 13:18:21.000000 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 13:18:21.000000 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-20 13:18:21.000000 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-20 13:18:21.000000 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:18:21.041803 atmoswing-vigicrues-1.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/tests/test_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/tests/test_download_gfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/tests/test_export_bdapbp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/tests/test_export_prv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/tests/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/tests/test_transfer_sftp_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/tests/test_transfer_sftp_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/tests/test_transform_gfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/tests/test_utils.py
```

### Comparing `atmoswing-vigicrues-1.1.2/LICENSE` & `atmoswing-vigicrues-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.2/PKG-INFO` & `atmoswing-vigicrues-1.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atmoswing-vigicrues
-Version: 1.1.2
+Version: 1.1.3
 Summary: Package to integrate AtmoSwing in the Vigicrues network.
 Author: Pascal Horton
 Author-email: Pascal Horton <pascal.horton@terranum.ch>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `atmoswing-vigicrues-1.1.2/README.md` & `atmoswing-vigicrues-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.2/pyproject.toml` & `atmoswing-vigicrues-1.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "atmoswing-vigicrues"
-version = "1.1.2"
+version = "1.1.3"
 authors = [
   { name="Pascal Horton", email="pascal.horton@terranum.ch" },
 ]
 description = "Package to integrate AtmoSwing in the Vigicrues network."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `atmoswing-vigicrues-1.1.2/src/atmoswing_vigicrues/__init__.py` & `atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/__init__.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.2/src/atmoswing_vigicrues/__main__.py` & `atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/__main__.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.2/src/atmoswing_vigicrues/controller.py` & `atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/controller.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.2/src/atmoswing_vigicrues/disseminations/dissemination.py` & `atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/disseminations/dissemination.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.2/src/atmoswing_vigicrues/disseminations/transfer_sftp_out.py` & `atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/disseminations/transfer_sftp_out.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.2/src/atmoswing_vigicrues/exceptions.py` & `atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/exceptions.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.2/src/atmoswing_vigicrues/options.py` & `atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/options.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.2/src/atmoswing_vigicrues/postactions/export_bdapbp.py` & `atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/postactions/export_bdapbp.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.2/src/atmoswing_vigicrues/postactions/export_prv.py` & `atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/postactions/export_prv.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.2/src/atmoswing_vigicrues/postactions/postaction.py` & `atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/postactions/postaction.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.2/src/atmoswing_vigicrues/preactions/download_gfs.py` & `atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/preactions/download_gfs.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.2/src/atmoswing_vigicrues/preactions/preaction.py` & `atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/preactions/preaction.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.2/src/atmoswing_vigicrues/preactions/transfer_sftp_in.py` & `atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/preactions/transfer_sftp_in.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.2/src/atmoswing_vigicrues/preactions/transform_ecmwf.py` & `atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/preactions/transform_ecmwf.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.2/src/atmoswing_vigicrues/preactions/transform_gfs.py` & `atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/preactions/transform_gfs.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.2/src/atmoswing_vigicrues/utils.py` & `atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/utils.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.2/src/atmoswing_vigicrues.egg-info/PKG-INFO` & `atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atmoswing-vigicrues
-Version: 1.1.2
+Version: 1.1.3
 Summary: Package to integrate AtmoSwing in the Vigicrues network.
 Author: Pascal Horton
 Author-email: Pascal Horton <pascal.horton@terranum.ch>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `atmoswing-vigicrues-1.1.2/src/atmoswing_vigicrues.egg-info/SOURCES.txt` & `atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.2/tests/test_controller.py` & `atmoswing-vigicrues-1.1.3/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.2/tests/test_download_gfs.py` & `atmoswing-vigicrues-1.1.3/tests/test_download_gfs.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.2/tests/test_exceptions.py` & `atmoswing-vigicrues-1.1.3/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.2/tests/test_export_bdapbp.py` & `atmoswing-vigicrues-1.1.3/tests/test_export_bdapbp.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.2/tests/test_export_prv.py` & `atmoswing-vigicrues-1.1.3/tests/test_export_prv.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.2/tests/test_options.py` & `atmoswing-vigicrues-1.1.3/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.2/tests/test_transfer_sftp_in.py` & `atmoswing-vigicrues-1.1.3/tests/test_transfer_sftp_in.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.2/tests/test_transfer_sftp_out.py` & `atmoswing-vigicrues-1.1.3/tests/test_transfer_sftp_out.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.2/tests/test_transform_gfs.py` & `atmoswing-vigicrues-1.1.3/tests/test_transform_gfs.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.2/tests/test_utils.py` & `atmoswing-vigicrues-1.1.3/tests/test_utils.py`

 * *Files identical despite different names*

