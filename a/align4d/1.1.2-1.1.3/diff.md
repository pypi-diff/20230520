# Comparing `tmp/align4d-1.1.2.tar.gz` & `tmp/align4d-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "align4d-1.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "align4d-1.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `align4d-1.1.2.tar` & `align4d-1.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    12277 2023-05-20 16:54:37.703041 align4d-1.1.2/README.md
--rw-r--r--   0        0        0      822 2023-05-20 16:55:57.147854 align4d-1.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-22 15:58:38.000000 align4d-1.1.2/src/align4d/__init__.py
--rw-r--r--   0        0        0     4646 2023-05-20 16:07:52.747761 align4d-1.1.2/src/align4d/align.py
--rw-r--r--   0        0        0    68096 2023-05-06 20:40:24.892372 align4d-1.1.2/src/align4d/align4d.cp310-win_amd64.pyd
--rw-r--r--   0        0        0   170842 2023-05-09 00:37:12.092411 align4d-1.1.2/src/align4d/align4d.cpython-310-darwin.so
--rw-r--r--   0        0        0  1981216 2023-05-06 20:45:55.257222 align4d-1.1.2/src/align4d/align4d.cpython-310-x86_64-linux-gnu.so
--rw-r--r--   0        0        0     1126 2023-05-09 01:39:20.296078 align4d-1.1.2/src/align4d/align4d.py
--rw-r--r--   0        0        0    13002 1970-01-01 00:00:00.000000 align4d-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0    12277 2023-05-20 17:20:37.817649 align4d-1.1.3/README.md
+-rw-r--r--   0        0        0      822 2023-05-20 17:26:13.839158 align4d-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-02-22 15:58:38.000000 align4d-1.1.3/src/align4d/__init__.py
+-rw-r--r--   0        0        0     4646 2023-05-20 16:07:52.747761 align4d-1.1.3/src/align4d/align.py
+-rw-r--r--   0        0        0    68096 2023-05-06 20:40:24.892372 align4d-1.1.3/src/align4d/align4d.cp310-win_amd64.pyd
+-rw-r--r--   0        0        0   170842 2023-05-09 00:37:12.092411 align4d-1.1.3/src/align4d/align4d.cpython-310-darwin.so
+-rw-r--r--   0        0        0  1981216 2023-05-06 20:45:55.257222 align4d-1.1.3/src/align4d/align4d.cpython-310-x86_64-linux-gnu.so
+-rw-r--r--   0        0        0     1126 2023-05-09 01:39:20.296078 align4d-1.1.3/src/align4d/align4d.py
+-rw-r--r--   0        0        0    13002 1970-01-01 00:00:00.000000 align4d-1.1.3/PKG-INFO
```

### Comparing `align4d-1.1.2/README.md` & `align4d-1.1.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,15 @@
 ```
 
 Sample output from `align()` : 
 
 ```python
 # content in align_result
 {
-		"hypothesis": ['ok', 'I', 'am', 'a', 'fish.', 'Are', 'you?', 'Hello', 'there.', 'How', 'are', 'you?', 'ok'],
+    "hypothesis": ['ok', 'I', 'am', 'a', 'fish.', 'Are', 'you?', 'Hello', 'there.', 'How', 'are', 'you?', 'ok'],
     "reference": {
         "A": ['', 'I', 'am', 'a', 'fish.', '', '', '', '', '', '', '', ''],
         "B": ['okay.', '', '', '', '', '', '', '', '', '', '', '', ''],
         "C": ['', '', '', '', '', 'Are', 'you?', '', '', '', '', '', ''],
         "D": ['', '', '', '', '', '', '', 'Hello', 'there.', '', '', '', ''],
         "E": ['', '', '', '', '', '', '', '', '', 'How', 'are', 'you?', '']
     }
@@ -194,15 +194,15 @@
         ["A", "I am a fish. "],
         ["B", "okay. "],
         ["C", "Are you? "],
         ["D", "Hello there. "],
         ["E", "How are you? "]
 ]
 align_result = align.align(hypothesis, reference)
-align_indices = align4d.get_token_match_result(align_result)
+align_indices = align.get_token_match_result(align_result)
 print(align_indices)
 ```
 
 The return value is a dictionary containing list of integers that shows the mapping between tokens from separated reference to hypothesis. The integers are the indices of the tokens in reference sequence map to the hypothesis sequence (for example, the first token in sequence “C” is mapped to the token in hypothesis with index 5).
 
 ```python
 # possible output
```

### Comparing `align4d-1.1.2/pyproject.toml` & `align4d-1.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core>=3.4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "align4d"
-version = "1.1.2"
+version = "1.1.3"
 authors = [
   { name="Peilin Wu", email="pwu54@emory.edu" },
 ]
 description = "align4d: Multi-sequence alignment tools for aligning ASR and Speaker Diarization result"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `align4d-1.1.2/src/align4d/align.py` & `align4d-1.1.3/src/align4d/align.py`

 * *Files identical despite different names*

### Comparing `align4d-1.1.2/src/align4d/align4d.cpython-310-darwin.so` & `align4d-1.1.3/src/align4d/align4d.cpython-310-darwin.so`

 * *Files identical despite different names*

### Comparing `align4d-1.1.2/src/align4d/align4d.cpython-310-x86_64-linux-gnu.so` & `align4d-1.1.3/src/align4d/align4d.cpython-310-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `align4d-1.1.2/src/align4d/align4d.py` & `align4d-1.1.3/src/align4d/align4d.py`

 * *Files identical despite different names*

### Comparing `align4d-1.1.2/PKG-INFO` & `align4d-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: align4d
-Version: 1.1.2
+Version: 1.1.3
 Summary: align4d: Multi-sequence alignment tools for aligning ASR and Speaker Diarization result
 Author-email: Peilin Wu <pwu54@emory.edu>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
@@ -149,15 +149,15 @@
 ```
 
 Sample output from `align()` : 
 
 ```python
 # content in align_result
 {
-		"hypothesis": ['ok', 'I', 'am', 'a', 'fish.', 'Are', 'you?', 'Hello', 'there.', 'How', 'are', 'you?', 'ok'],
+    "hypothesis": ['ok', 'I', 'am', 'a', 'fish.', 'Are', 'you?', 'Hello', 'there.', 'How', 'are', 'you?', 'ok'],
     "reference": {
         "A": ['', 'I', 'am', 'a', 'fish.', '', '', '', '', '', '', '', ''],
         "B": ['okay.', '', '', '', '', '', '', '', '', '', '', '', ''],
         "C": ['', '', '', '', '', 'Are', 'you?', '', '', '', '', '', ''],
         "D": ['', '', '', '', '', '', '', 'Hello', 'there.', '', '', '', ''],
         "E": ['', '', '', '', '', '', '', '', '', 'How', 'are', 'you?', '']
     }
@@ -210,15 +210,15 @@
         ["A", "I am a fish. "],
         ["B", "okay. "],
         ["C", "Are you? "],
         ["D", "Hello there. "],
         ["E", "How are you? "]
 ]
 align_result = align.align(hypothesis, reference)
-align_indices = align4d.get_token_match_result(align_result)
+align_indices = align.get_token_match_result(align_result)
 print(align_indices)
 ```
 
 The return value is a dictionary containing list of integers that shows the mapping between tokens from separated reference to hypothesis. The integers are the indices of the tokens in reference sequence map to the hypothesis sequence (for example, the first token in sequence “C” is mapped to the token in hypothesis with index 5).
 
 ```python
 # possible output
```

