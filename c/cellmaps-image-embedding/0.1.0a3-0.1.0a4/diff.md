# Comparing `tmp/cellmaps_image_embedding-0.1.0a3.tar.gz` & `tmp/cellmaps_image_embedding-0.1.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cellmaps_image_embedding-0.1.0a3.tar", last modified: Thu May 18 23:32:47 2023, max compression
+gzip compressed data, was "dist/cellmaps_image_embedding-0.1.0a4.tar", last modified: Sat May 20 00:03:35 2023, max compression
```

## Comparing `cellmaps_image_embedding-0.1.0a3.tar` & `cellmaps_image_embedding-0.1.0a4.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-18 23:32:47.061797 cellmaps_image_embedding-0.1.0a3/
--rw-r--r--   0 churas     (504) staff       (20)      160 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a3/AUTHORS.rst
--rw-r--r--   0 churas     (504) staff       (20)     3731 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a3/CONTRIBUTING.rst
--rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-18 23:31:36.000000 cellmaps_image_embedding-0.1.0a3/HISTORY.rst
--rw-r--r--   0 churas     (504) staff       (20)     1102 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a3/LICENSE
--rw-r--r--   0 churas     (504) staff       (20)      262 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a3/MANIFEST.in
--rw-r--r--   0 churas     (504) staff       (20)     5619 2023-05-18 23:32:47.061962 cellmaps_image_embedding-0.1.0a3/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     3609 2023-05-18 23:24:53.000000 cellmaps_image_embedding-0.1.0a3/README.rst
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-18 23:32:47.051977 cellmaps_image_embedding-0.1.0a3/cellmaps_image_embedding/
--rw-r--r--   0 churas     (504) staff       (20)      304 2023-05-18 23:32:17.000000 cellmaps_image_embedding-0.1.0a3/cellmaps_image_embedding/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     6272 2023-05-18 23:18:31.000000 cellmaps_image_embedding-0.1.0a3/cellmaps_image_embedding/cellmaps_image_embeddingcmd.py
--rw-r--r--   0 churas     (504) staff       (20)     4718 2023-05-15 22:13:15.000000 cellmaps_image_embedding-0.1.0a3/cellmaps_image_embedding/dataset.py
--rw-r--r--   0 churas     (504) staff       (20)      143 2023-03-30 21:25:53.000000 cellmaps_image_embedding-0.1.0a3/cellmaps_image_embedding/exceptions.py
--rw-r--r--   0 churas     (504) staff       (20)     7602 2023-05-16 19:18:42.000000 cellmaps_image_embedding-0.1.0a3/cellmaps_image_embedding/models.py
--rw-r--r--   0 churas     (504) staff       (20)    15943 2023-05-18 23:21:18.000000 cellmaps_image_embedding-0.1.0a3/cellmaps_image_embedding/runner.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-18 23:32:47.053247 cellmaps_image_embedding-0.1.0a3/cellmaps_image_embedding.egg-info/
--rw-r--r--   0 churas     (504) staff       (20)     5619 2023-05-18 23:32:46.000000 cellmaps_image_embedding-0.1.0a3/cellmaps_image_embedding.egg-info/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     1207 2023-05-18 23:32:47.000000 cellmaps_image_embedding-0.1.0a3/cellmaps_image_embedding.egg-info/SOURCES.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-18 23:32:46.000000 cellmaps_image_embedding-0.1.0a3/cellmaps_image_embedding.egg-info/dependency_links.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-18 23:32:46.000000 cellmaps_image_embedding-0.1.0a3/cellmaps_image_embedding.egg-info/not-zip-safe
--rw-r--r--   0 churas     (504) staff       (20)      121 2023-05-18 23:32:46.000000 cellmaps_image_embedding-0.1.0a3/cellmaps_image_embedding.egg-info/requires.txt
--rw-r--r--   0 churas     (504) staff       (20)       25 2023-05-18 23:32:46.000000 cellmaps_image_embedding-0.1.0a3/cellmaps_image_embedding.egg-info/top_level.txt
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-18 23:32:47.058873 cellmaps_image_embedding-0.1.0a3/docs/
--rw-r--r--   0 churas     (504) staff       (20)      625 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a3/docs/Makefile
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-18 23:32:47.048284 cellmaps_image_embedding-0.1.0a3/docs/_build/
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-18 23:32:47.048353 cellmaps_image_embedding-0.1.0a3/docs/_build/html/
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-18 23:32:47.059771 cellmaps_image_embedding-0.1.0a3/docs/_build/html/_static/
--rw-r--r--   0 churas     (504) staff       (20)      286 2023-05-02 22:49:28.000000 cellmaps_image_embedding-0.1.0a3/docs/_build/html/_static/file.png
--rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_image_embedding-0.1.0a3/docs/_build/html/_static/minus.png
--rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_image_embedding-0.1.0a3/docs/_build/html/_static/plus.png
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a3/docs/authors.rst
--rw-r--r--   0 churas     (504) staff       (20)     1234 2023-05-18 23:15:22.000000 cellmaps_image_embedding-0.1.0a3/docs/cellmaps_image_embedding.rst
--rwxr-xr-x   0 churas     (504) staff       (20)     6131 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a3/docs/conf.py
--rw-r--r--   0 churas     (504) staff       (20)       33 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a3/docs/contributing.rst
--rw-r--r--   0 churas     (504) staff       (20)      174 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a3/docs/devbranches.rst
--rw-r--r--   0 churas     (504) staff       (20)      292 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a3/docs/developer.rst
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a3/docs/history.rst
--rw-r--r--   0 churas     (504) staff       (20)      986 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a3/docs/index.rst
--rw-r--r--   0 churas     (504) staff       (20)     1254 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a3/docs/installation.rst
--rw-r--r--   0 churas     (504) staff       (20)      472 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a3/docs/integrationtesting.rst
--rw-r--r--   0 churas     (504) staff       (20)      822 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a3/docs/make.bat
--rw-r--r--   0 churas     (504) staff       (20)       83 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a3/docs/modules.rst
--rw-r--r--   0 churas     (504) staff       (20)     4424 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a3/docs/newrelease.rst
--rw-r--r--   0 churas     (504) staff       (20)      794 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a3/docs/pypircfile.rst
--rw-r--r--   0 churas     (504) staff       (20)      739 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a3/docs/usage.rst
--rw-r--r--   0 churas     (504) staff       (20)      817 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a3/docs/versioningscheme.rst
--rw-r--r--   0 churas     (504) staff       (20)      407 2023-05-18 23:32:47.062715 cellmaps_image_embedding-0.1.0a3/setup.cfg
--rw-r--r--   0 churas     (504) staff       (20)     2272 2023-05-18 23:26:41.000000 cellmaps_image_embedding-0.1.0a3/setup.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-18 23:32:47.061526 cellmaps_image_embedding-0.1.0a3/tests/
--rw-r--r--   0 churas     (504) staff       (20)       79 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a3/tests/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     1630 2023-05-08 16:58:10.000000 cellmaps_image_embedding-0.1.0a3/tests/test_cellmaps_image_embeddingcmd.py
--rw-r--r--   0 churas     (504) staff       (20)     1394 2023-05-15 20:45:32.000000 cellmaps_image_embedding-0.1.0a3/tests/test_cellmaps_image_embeddingrunner.py
--rw-r--r--   0 churas     (504) staff       (20)      821 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a3/tests/test_integration_cellmaps_image_embedding.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-20 00:03:35.240467 cellmaps_image_embedding-0.1.0a4/
+-rw-r--r--   0 churas     (504) staff       (20)      160 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a4/AUTHORS.rst
+-rw-r--r--   0 churas     (504) staff       (20)     3731 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a4/CONTRIBUTING.rst
+-rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-18 23:31:36.000000 cellmaps_image_embedding-0.1.0a4/HISTORY.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1102 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a4/LICENSE
+-rw-r--r--   0 churas     (504) staff       (20)      262 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a4/MANIFEST.in
+-rw-r--r--   0 churas     (504) staff       (20)     5619 2023-05-20 00:03:35.240666 cellmaps_image_embedding-0.1.0a4/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     3609 2023-05-18 23:24:53.000000 cellmaps_image_embedding-0.1.0a4/README.rst
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-20 00:03:35.230225 cellmaps_image_embedding-0.1.0a4/cellmaps_image_embedding/
+-rw-r--r--   0 churas     (504) staff       (20)      304 2023-05-20 00:03:03.000000 cellmaps_image_embedding-0.1.0a4/cellmaps_image_embedding/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)     6272 2023-05-18 23:18:31.000000 cellmaps_image_embedding-0.1.0a4/cellmaps_image_embedding/cellmaps_image_embeddingcmd.py
+-rw-r--r--   0 churas     (504) staff       (20)     4718 2023-05-15 22:13:15.000000 cellmaps_image_embedding-0.1.0a4/cellmaps_image_embedding/dataset.py
+-rw-r--r--   0 churas     (504) staff       (20)      143 2023-03-30 21:25:53.000000 cellmaps_image_embedding-0.1.0a4/cellmaps_image_embedding/exceptions.py
+-rw-r--r--   0 churas     (504) staff       (20)     7602 2023-05-16 19:18:42.000000 cellmaps_image_embedding-0.1.0a4/cellmaps_image_embedding/models.py
+-rw-r--r--   0 churas     (504) staff       (20)    15944 2023-05-19 23:52:50.000000 cellmaps_image_embedding-0.1.0a4/cellmaps_image_embedding/runner.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-20 00:03:35.231833 cellmaps_image_embedding-0.1.0a4/cellmaps_image_embedding.egg-info/
+-rw-r--r--   0 churas     (504) staff       (20)     5619 2023-05-20 00:03:35.000000 cellmaps_image_embedding-0.1.0a4/cellmaps_image_embedding.egg-info/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     1207 2023-05-20 00:03:35.000000 cellmaps_image_embedding-0.1.0a4/cellmaps_image_embedding.egg-info/SOURCES.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-20 00:03:35.000000 cellmaps_image_embedding-0.1.0a4/cellmaps_image_embedding.egg-info/dependency_links.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-20 00:03:35.000000 cellmaps_image_embedding-0.1.0a4/cellmaps_image_embedding.egg-info/not-zip-safe
+-rw-r--r--   0 churas     (504) staff       (20)      121 2023-05-20 00:03:35.000000 cellmaps_image_embedding-0.1.0a4/cellmaps_image_embedding.egg-info/requires.txt
+-rw-r--r--   0 churas     (504) staff       (20)       25 2023-05-20 00:03:35.000000 cellmaps_image_embedding-0.1.0a4/cellmaps_image_embedding.egg-info/top_level.txt
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-20 00:03:35.237736 cellmaps_image_embedding-0.1.0a4/docs/
+-rw-r--r--   0 churas     (504) staff       (20)      625 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a4/docs/Makefile
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-20 00:03:35.225128 cellmaps_image_embedding-0.1.0a4/docs/_build/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-20 00:03:35.225210 cellmaps_image_embedding-0.1.0a4/docs/_build/html/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-20 00:03:35.238696 cellmaps_image_embedding-0.1.0a4/docs/_build/html/_static/
+-rw-r--r--   0 churas     (504) staff       (20)      286 2023-05-02 22:49:28.000000 cellmaps_image_embedding-0.1.0a4/docs/_build/html/_static/file.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_image_embedding-0.1.0a4/docs/_build/html/_static/minus.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_image_embedding-0.1.0a4/docs/_build/html/_static/plus.png
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a4/docs/authors.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1234 2023-05-18 23:15:22.000000 cellmaps_image_embedding-0.1.0a4/docs/cellmaps_image_embedding.rst
+-rwxr-xr-x   0 churas     (504) staff       (20)     6131 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a4/docs/conf.py
+-rw-r--r--   0 churas     (504) staff       (20)       33 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a4/docs/contributing.rst
+-rw-r--r--   0 churas     (504) staff       (20)      174 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a4/docs/devbranches.rst
+-rw-r--r--   0 churas     (504) staff       (20)      292 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a4/docs/developer.rst
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a4/docs/history.rst
+-rw-r--r--   0 churas     (504) staff       (20)      986 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a4/docs/index.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1254 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a4/docs/installation.rst
+-rw-r--r--   0 churas     (504) staff       (20)      472 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a4/docs/integrationtesting.rst
+-rw-r--r--   0 churas     (504) staff       (20)      822 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a4/docs/make.bat
+-rw-r--r--   0 churas     (504) staff       (20)       83 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a4/docs/modules.rst
+-rw-r--r--   0 churas     (504) staff       (20)     4424 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a4/docs/newrelease.rst
+-rw-r--r--   0 churas     (504) staff       (20)      794 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a4/docs/pypircfile.rst
+-rw-r--r--   0 churas     (504) staff       (20)      739 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a4/docs/usage.rst
+-rw-r--r--   0 churas     (504) staff       (20)      817 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a4/docs/versioningscheme.rst
+-rw-r--r--   0 churas     (504) staff       (20)      407 2023-05-20 00:03:35.241265 cellmaps_image_embedding-0.1.0a4/setup.cfg
+-rw-r--r--   0 churas     (504) staff       (20)     2272 2023-05-18 23:26:41.000000 cellmaps_image_embedding-0.1.0a4/setup.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-20 00:03:35.240120 cellmaps_image_embedding-0.1.0a4/tests/
+-rw-r--r--   0 churas     (504) staff       (20)       79 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a4/tests/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)     1630 2023-05-08 16:58:10.000000 cellmaps_image_embedding-0.1.0a4/tests/test_cellmaps_image_embeddingcmd.py
+-rw-r--r--   0 churas     (504) staff       (20)     1394 2023-05-15 20:45:32.000000 cellmaps_image_embedding-0.1.0a4/tests/test_cellmaps_image_embeddingrunner.py
+-rw-r--r--   0 churas     (504) staff       (20)      821 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a4/tests/test_integration_cellmaps_image_embedding.py
```

### Comparing `cellmaps_image_embedding-0.1.0a3/CONTRIBUTING.rst` & `cellmaps_image_embedding-0.1.0a4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a3/LICENSE` & `cellmaps_image_embedding-0.1.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a3/PKG-INFO` & `cellmaps_image_embedding-0.1.0a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmaps_image_embedding
-Version: 0.1.0a3
+Version: 0.1.0a4
 Summary: A tool to generate embeddings from HPA IF images
 Home-page: https://github.com/idekerlab/cellmaps_image_embedding
 Author: Gege Qian
 Author-email: geqian@ucsd.edu
 License: MIT license
 Description: =========================
         cellmaps_image_embedding
```

### Comparing `cellmaps_image_embedding-0.1.0a3/README.rst` & `cellmaps_image_embedding-0.1.0a4/README.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a3/cellmaps_image_embedding/cellmaps_image_embeddingcmd.py` & `cellmaps_image_embedding-0.1.0a4/cellmaps_image_embedding/cellmaps_image_embeddingcmd.py`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a3/cellmaps_image_embedding/dataset.py` & `cellmaps_image_embedding-0.1.0a4/cellmaps_image_embedding/dataset.py`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a3/cellmaps_image_embedding/models.py` & `cellmaps_image_embedding-0.1.0a4/cellmaps_image_embedding/models.py`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a3/cellmaps_image_embedding/runner.py` & `cellmaps_image_embedding-0.1.0a4/cellmaps_image_embedding/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
     `Densenet <https://github.com/CellProfiling/densenet>`__
     code and no memory leaks
 
     """
     def __init__(self, inputdir, dimensions=1024,
                  outdir=None,
                  model_path=None,
-                 suffix='jpg'):
+                 suffix='.jpg'):
         """
         Constructor
 
         :param inputdir: Directory where red, blue, green, and yellow
                          image directories reside
         :type inputdir: str
         :param dimensions: Desired size of output embedding vector
```

### Comparing `cellmaps_image_embedding-0.1.0a3/cellmaps_image_embedding.egg-info/PKG-INFO` & `cellmaps_image_embedding-0.1.0a4/cellmaps_image_embedding.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmaps-image-embedding
-Version: 0.1.0a3
+Version: 0.1.0a4
 Summary: A tool to generate embeddings from HPA IF images
 Home-page: https://github.com/idekerlab/cellmaps_image_embedding
 Author: Gege Qian
 Author-email: geqian@ucsd.edu
 License: MIT license
 Description: =========================
         cellmaps_image_embedding
```

### Comparing `cellmaps_image_embedding-0.1.0a3/cellmaps_image_embedding.egg-info/SOURCES.txt` & `cellmaps_image_embedding-0.1.0a4/cellmaps_image_embedding.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a3/docs/Makefile` & `cellmaps_image_embedding-0.1.0a4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a3/docs/cellmaps_image_embedding.rst` & `cellmaps_image_embedding-0.1.0a4/docs/cellmaps_image_embedding.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a3/docs/conf.py` & `cellmaps_image_embedding-0.1.0a4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a3/docs/index.rst` & `cellmaps_image_embedding-0.1.0a4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a3/docs/installation.rst` & `cellmaps_image_embedding-0.1.0a4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a3/docs/make.bat` & `cellmaps_image_embedding-0.1.0a4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a3/docs/newrelease.rst` & `cellmaps_image_embedding-0.1.0a4/docs/newrelease.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a3/docs/pypircfile.rst` & `cellmaps_image_embedding-0.1.0a4/docs/pypircfile.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a3/docs/usage.rst` & `cellmaps_image_embedding-0.1.0a4/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a3/docs/versioningscheme.rst` & `cellmaps_image_embedding-0.1.0a4/docs/versioningscheme.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a3/setup.py` & `cellmaps_image_embedding-0.1.0a4/setup.py`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a3/tests/test_cellmaps_image_embeddingcmd.py` & `cellmaps_image_embedding-0.1.0a4/tests/test_cellmaps_image_embeddingcmd.py`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a3/tests/test_cellmaps_image_embeddingrunner.py` & `cellmaps_image_embedding-0.1.0a4/tests/test_cellmaps_image_embeddingrunner.py`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a3/tests/test_integration_cellmaps_image_embedding.py` & `cellmaps_image_embedding-0.1.0a4/tests/test_integration_cellmaps_image_embedding.py`

 * *Files identical despite different names*

