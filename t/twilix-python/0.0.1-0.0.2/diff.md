# Comparing `tmp/twilix-python-0.0.1.tar.gz` & `tmp/twilix-python-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twilix-python-0.0.1.tar", last modified: Sat May 20 06:00:21 2023, max compression
+gzip compressed data, was "twilix-python-0.0.2.tar", last modified: Sat May 20 13:41:17 2023, max compression
```

## Comparing `twilix-python-0.0.1.tar` & `twilix-python-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-05-20 06:00:21.039960 twilix-python-0.0.1/
--rw-r--r--   0 jackywong   (501) staff       (20)    11357 2023-05-20 02:14:08.000000 twilix-python-0.0.1/LICENSE
--rw-r--r--   0 jackywong   (501) staff       (20)      190 2023-05-20 06:00:21.039799 twilix-python-0.0.1/PKG-INFO
--rw-r--r--   0 jackywong   (501) staff       (20)       37 2023-05-20 02:14:08.000000 twilix-python-0.0.1/README.md
--rw-r--r--   0 jackywong   (501) staff       (20)       38 2023-05-20 06:00:21.040008 twilix-python-0.0.1/setup.cfg
--rw-r--r--   0 jackywong   (501) staff       (20)      380 2023-05-20 05:57:47.000000 twilix-python-0.0.1/setup.py
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-05-20 06:00:21.038218 twilix-python-0.0.1/tests/
--rw-r--r--   0 jackywong   (501) staff       (20)      540 2023-05-20 05:50:18.000000 twilix-python-0.0.1/tests/test_crud.py
--rw-r--r--   0 jackywong   (501) staff       (20)      309 2023-05-20 05:51:22.000000 twilix-python-0.0.1/tests/test_semantic_search.py
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-05-20 06:00:21.038639 twilix-python-0.0.1/twilix/
--rw-r--r--   0 jackywong   (501) staff       (20)     1228 2023-05-20 05:56:33.000000 twilix-python-0.0.1/twilix/__init__.py
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-05-20 06:00:21.039598 twilix-python-0.0.1/twilix_python.egg-info/
--rw-r--r--   0 jackywong   (501) staff       (20)      190 2023-05-20 06:00:21.000000 twilix-python-0.0.1/twilix_python.egg-info/PKG-INFO
--rw-r--r--   0 jackywong   (501) staff       (20)      278 2023-05-20 06:00:21.000000 twilix-python-0.0.1/twilix_python.egg-info/SOURCES.txt
--rw-r--r--   0 jackywong   (501) staff       (20)        1 2023-05-20 06:00:21.000000 twilix-python-0.0.1/twilix_python.egg-info/dependency_links.txt
--rw-r--r--   0 jackywong   (501) staff       (20)       18 2023-05-20 06:00:21.000000 twilix-python-0.0.1/twilix_python.egg-info/requires.txt
--rw-r--r--   0 jackywong   (501) staff       (20)        7 2023-05-20 06:00:21.000000 twilix-python-0.0.1/twilix_python.egg-info/top_level.txt
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-05-20 13:41:17.789842 twilix-python-0.0.2/
+-rw-r--r--   0 jackywong   (501) staff       (20)    11357 2023-05-20 02:14:08.000000 twilix-python-0.0.2/LICENSE
+-rw-r--r--   0 jackywong   (501) staff       (20)      190 2023-05-20 13:41:17.789679 twilix-python-0.0.2/PKG-INFO
+-rw-r--r--   0 jackywong   (501) staff       (20)      133 2023-05-20 11:36:18.000000 twilix-python-0.0.2/README.md
+-rw-r--r--   0 jackywong   (501) staff       (20)       38 2023-05-20 13:41:17.789908 twilix-python-0.0.2/setup.cfg
+-rw-r--r--   0 jackywong   (501) staff       (20)      377 2023-05-20 11:56:48.000000 twilix-python-0.0.2/setup.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-05-20 13:41:17.787953 twilix-python-0.0.2/tests/
+-rw-r--r--   0 jackywong   (501) staff       (20)      516 2023-05-20 11:33:00.000000 twilix-python-0.0.2/tests/test_crud.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      310 2023-05-20 06:21:57.000000 twilix-python-0.0.2/tests/test_semantic_search.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-05-20 13:41:17.788433 twilix-python-0.0.2/twilix/
+-rw-r--r--   0 jackywong   (501) staff       (20)     1448 2023-05-20 11:58:43.000000 twilix-python-0.0.2/twilix/__init__.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-05-20 13:41:17.789487 twilix-python-0.0.2/twilix_python.egg-info/
+-rw-r--r--   0 jackywong   (501) staff       (20)      190 2023-05-20 13:41:17.000000 twilix-python-0.0.2/twilix_python.egg-info/PKG-INFO
+-rw-r--r--   0 jackywong   (501) staff       (20)      278 2023-05-20 13:41:17.000000 twilix-python-0.0.2/twilix_python.egg-info/SOURCES.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)        1 2023-05-20 13:41:17.000000 twilix-python-0.0.2/twilix_python.egg-info/dependency_links.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)       18 2023-05-20 13:41:17.000000 twilix-python-0.0.2/twilix_python.egg-info/requires.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)        7 2023-05-20 13:41:17.000000 twilix-python-0.0.2/twilix_python.egg-info/top_level.txt
```

### Comparing `twilix-python-0.0.1/LICENSE` & `twilix-python-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `twilix-python-0.0.1/tests/test_crud.py` & `twilix-python-0.0.2/tests/test_crud.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,23 +7,17 @@
 
 twilix.api_key = api_key
 
 collection_name = "example2"
 
 docs = [
     {
-        "answer": 'This framework generates embeddings for each input sentence',
+        "answer": "This framework generates embeddings for each input sentence",
     },
     {
-
-        "answer": 'Sentences are passed as a list of string.',
+        "answer": "Sentences are passed as a list of string.",
     },
-    {
-        "answer": 'The quick brown fox jumps over the lazy dog.'
-    }
+    {"answer": "The quick brown fox jumps over the lazy dog."},
 ]
 
-result = twilix.add_objects(
-    collection_name=collection_name,
-    objects=docs
-)
+result = twilix.add_objects(collection_name=collection_name, objects=docs)
 ic(result)
```

