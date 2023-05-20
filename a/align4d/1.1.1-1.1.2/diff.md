# Comparing `tmp/align4d-1.1.1.tar.gz` & `tmp/align4d-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "align4d-1.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "align4d-1.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `align4d-1.1.1.tar` & `align4d-1.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    12459 2023-05-20 16:44:18.162866 align4d-1.1.1/README.md
--rw-r--r--   0        0        0      822 2023-05-20 16:13:04.057429 align4d-1.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-22 15:58:38.000000 align4d-1.1.1/src/align4d/__init__.py
--rw-r--r--   0        0        0     4646 2023-05-20 16:07:52.747761 align4d-1.1.1/src/align4d/align.py
--rw-r--r--   0        0        0    68096 2023-05-06 20:40:24.892372 align4d-1.1.1/src/align4d/align4d.cp310-win_amd64.pyd
--rw-r--r--   0        0        0   170842 2023-05-09 00:37:12.092411 align4d-1.1.1/src/align4d/align4d.cpython-310-darwin.so
--rw-r--r--   0        0        0  1981216 2023-05-06 20:45:55.257222 align4d-1.1.1/src/align4d/align4d.cpython-310-x86_64-linux-gnu.so
--rw-r--r--   0        0        0     1126 2023-05-09 01:39:20.296078 align4d-1.1.1/src/align4d/align4d.py
--rw-r--r--   0        0        0    13184 1970-01-01 00:00:00.000000 align4d-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0    12277 2023-05-20 16:54:37.703041 align4d-1.1.2/README.md
+-rw-r--r--   0        0        0      822 2023-05-20 16:55:57.147854 align4d-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-02-22 15:58:38.000000 align4d-1.1.2/src/align4d/__init__.py
+-rw-r--r--   0        0        0     4646 2023-05-20 16:07:52.747761 align4d-1.1.2/src/align4d/align.py
+-rw-r--r--   0        0        0    68096 2023-05-06 20:40:24.892372 align4d-1.1.2/src/align4d/align4d.cp310-win_amd64.pyd
+-rw-r--r--   0        0        0   170842 2023-05-09 00:37:12.092411 align4d-1.1.2/src/align4d/align4d.cpython-310-darwin.so
+-rw-r--r--   0        0        0  1981216 2023-05-06 20:45:55.257222 align4d-1.1.2/src/align4d/align4d.cpython-310-x86_64-linux-gnu.so
+-rw-r--r--   0        0        0     1126 2023-05-09 01:39:20.296078 align4d-1.1.2/src/align4d/align4d.py
+-rw-r--r--   0        0        0    13002 1970-01-01 00:00:00.000000 align4d-1.1.2/PKG-INFO
```

### Comparing `align4d-1.1.1/README.md` & `align4d-1.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -218,10 +218,8 @@
 ## Troubleshooting
 
 If you encounter any issues while using Align4d, try the following:
 
 1. Make sure you have installed Python version 3.10 or higher.
 2. Make sure you have installed the latest version of Align4d.
 3. Check the input data to make sure it is in the correct format.
-    1. The length of the `reference` and `reference_speaker_label` needs to be the same.
-    2. All the input strings must be encoded in the utf-8 format.
-4. For short conversation (hypothesis length ≤ 100), please use `align_without_segment()`.
+    1. All the input strings must be encoded in the utf-8 format.
```

### Comparing `align4d-1.1.1/pyproject.toml` & `align4d-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core>=3.4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "align4d"
-version = "1.1.1"
+version = "1.1.2"
 authors = [
   { name="Peilin Wu", email="pwu54@emory.edu" },
 ]
 description = "align4d: Multi-sequence alignment tools for aligning ASR and Speaker Diarization result"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `align4d-1.1.1/src/align4d/align.py` & `align4d-1.1.2/src/align4d/align.py`

 * *Files identical despite different names*

### Comparing `align4d-1.1.1/src/align4d/align4d.cpython-310-darwin.so` & `align4d-1.1.2/src/align4d/align4d.cpython-310-darwin.so`

 * *Files identical despite different names*

### Comparing `align4d-1.1.1/src/align4d/align4d.cpython-310-x86_64-linux-gnu.so` & `align4d-1.1.2/src/align4d/align4d.cpython-310-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `align4d-1.1.1/src/align4d/align4d.py` & `align4d-1.1.2/src/align4d/align4d.py`

 * *Files identical despite different names*

### Comparing `align4d-1.1.1/PKG-INFO` & `align4d-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: align4d
-Version: 1.1.1
+Version: 1.1.2
 Summary: align4d: Multi-sequence alignment tools for aligning ASR and Speaker Diarization result
 Author-email: Peilin Wu <pwu54@emory.edu>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
@@ -234,10 +234,8 @@
 ## Troubleshooting
 
 If you encounter any issues while using Align4d, try the following:
 
 1. Make sure you have installed Python version 3.10 or higher.
 2. Make sure you have installed the latest version of Align4d.
 3. Check the input data to make sure it is in the correct format.
-    1. The length of the `reference` and `reference_speaker_label` needs to be the same.
-    2. All the input strings must be encoded in the utf-8 format.
-4. For short conversation (hypothesis length ≤ 100), please use `align_without_segment()`.
+    1. All the input strings must be encoded in the utf-8 format.
```

