# Comparing `tmp/soral-data-test-0.0.3.tar.gz` & `tmp/soral-data-test-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soral-data-test-0.0.3.tar", last modified: Fri May 19 21:37:34 2023, max compression
+gzip compressed data, was "soral-data-test-0.0.4.tar", last modified: Sat May 20 18:47:31 2023, max compression
```

## Comparing `soral-data-test-0.0.3.tar` & `soral-data-test-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 21:37:34.473996 soral-data-test-0.0.3/
--rw-rw-rw-   0 root         (0) root         (0)      150 2023-05-18 10:04:46.000000 soral-data-test-0.0.3/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-05-19 21:37:34.000000 soral-data-test-0.0.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      632 2023-05-19 21:37:34.473996 soral-data-test-0.0.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      315 2023-05-18 10:04:46.000000 soral-data-test-0.0.3/README.rst
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-19 21:37:34.473996 soral-data-test-0.0.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2294 2023-05-18 10:04:46.000000 soral-data-test-0.0.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 21:37:34.473996 soral-data-test-0.0.3/soral_data_test/
--rw-rw-rw-   0 root         (0) root         (0)       95 2023-05-19 21:34:54.000000 soral-data-test-0.0.3/soral_data_test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      249 2023-05-19 21:34:54.000000 soral-data-test-0.0.3/soral_data_test/data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 21:37:34.473996 soral-data-test-0.0.3/soral_data_test.egg-info/
--rw-r--r--   0 root         (0) root         (0)      632 2023-05-19 21:37:34.000000 soral-data-test-0.0.3/soral_data_test.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      251 2023-05-19 21:37:34.000000 soral-data-test-0.0.3/soral_data_test.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 21:37:34.000000 soral-data-test-0.0.3/soral_data_test.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-05-19 21:37:34.000000 soral-data-test-0.0.3/soral_data_test.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 18:47:31.686873 soral-data-test-0.0.4/
+-rw-rw-rw-   0 root         (0) root         (0)      150 2023-05-18 10:04:46.000000 soral-data-test-0.0.4/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-05-20 18:47:31.000000 soral-data-test-0.0.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      632 2023-05-20 18:47:31.686873 soral-data-test-0.0.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      315 2023-05-18 10:04:46.000000 soral-data-test-0.0.4/README.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-20 18:47:31.686873 soral-data-test-0.0.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2294 2023-05-18 10:04:46.000000 soral-data-test-0.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 18:47:31.686873 soral-data-test-0.0.4/soral_data_test/
+-rw-rw-rw-   0 root         (0) root         (0)       95 2023-05-20 18:46:27.000000 soral-data-test-0.0.4/soral_data_test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      281 2023-05-20 18:46:27.000000 soral-data-test-0.0.4/soral_data_test/data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 18:47:31.686873 soral-data-test-0.0.4/soral_data_test.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      632 2023-05-20 18:47:31.000000 soral-data-test-0.0.4/soral_data_test.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      251 2023-05-20 18:47:31.000000 soral-data-test-0.0.4/soral_data_test.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-20 18:47:31.000000 soral-data-test-0.0.4/soral_data_test.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-05-20 18:47:31.000000 soral-data-test-0.0.4/soral_data_test.egg-info/top_level.txt
```

### Comparing `soral-data-test-0.0.3/PKG-INFO` & `soral-data-test-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: soral-data-test
-Version: 0.0.3
+Version: 0.0.4
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/soral-data-test/0.0.3/index.html
+Home-page: https://develop.x-i-a.com/docs/soral-data-test/0.0.4/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

### Comparing `soral-data-test-0.0.3/setup.py` & `soral-data-test-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `soral-data-test-0.0.3/soral_data_test.egg-info/PKG-INFO` & `soral-data-test-0.0.4/soral_data_test.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: soral-data-test
-Version: 0.0.3
+Version: 0.0.4
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/soral-data-test/0.0.3/index.html
+Home-page: https://develop.x-i-a.com/docs/soral-data-test/0.0.4/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

