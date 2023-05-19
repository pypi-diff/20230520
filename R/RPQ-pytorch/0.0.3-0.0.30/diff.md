# Comparing `tmp/RPQ-pytorch-0.0.3.tar.gz` & `tmp/RPQ-pytorch-0.0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RPQ-pytorch-0.0.3.tar", last modified: Fri May 19 21:50:33 2023, max compression
+gzip compressed data, was "RPQ-pytorch-0.0.30.tar", last modified: Fri May 19 22:13:59 2023, max compression
```

## Comparing `RPQ-pytorch-0.0.3.tar` & `RPQ-pytorch-0.0.30.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:50:33.404658 RPQ-pytorch-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-19 21:50:23.000000 RPQ-pytorch-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7635 2023-05-19 21:50:33.404658 RPQ-pytorch-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-05-19 21:50:23.000000 RPQ-pytorch-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:50:33.404658 RPQ-pytorch-0.0.3/RPQ_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7635 2023-05-19 21:50:33.000000 RPQ-pytorch-0.0.3/RPQ_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-19 21:50:33.000000 RPQ-pytorch-0.0.3/RPQ_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 21:50:33.000000 RPQ-pytorch-0.0.3/RPQ_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-19 21:50:33.000000 RPQ-pytorch-0.0.3/RPQ_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-19 21:50:33.000000 RPQ-pytorch-0.0.3/RPQ_pytorch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:50:33.404658 RPQ-pytorch-0.0.3/rpq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 21:50:23.000000 RPQ-pytorch-0.0.3/rpq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 21:50:33.404658 RPQ-pytorch-0.0.3/rpq/models/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-19 21:50:23.000000 RPQ-pytorch-0.0.3/rpq/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57773 2023-05-19 21:50:23.000000 RPQ-pytorch-0.0.3/rpq/models/rpqopt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-05-19 21:50:23.000000 RPQ-pytorch-0.0.3/rpq/models/rpqvit.py
--rw-r--r--   0 runner    (1001) docker     (123)    12165 2023-05-19 21:50:23.000000 RPQ-pytorch-0.0.3/rpq/nn.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-19 21:50:23.000000 RPQ-pytorch-0.0.3/rpq/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 21:50:33.404658 RPQ-pytorch-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-19 21:50:23.000000 RPQ-pytorch-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:13:59.646553 RPQ-pytorch-0.0.30/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-19 22:13:43.000000 RPQ-pytorch-0.0.30/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-05-19 22:13:59.646553 RPQ-pytorch-0.0.30/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-05-19 22:13:43.000000 RPQ-pytorch-0.0.30/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:13:59.642552 RPQ-pytorch-0.0.30/RPQ_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-05-19 22:13:59.000000 RPQ-pytorch-0.0.30/RPQ_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-19 22:13:59.000000 RPQ-pytorch-0.0.30/RPQ_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 22:13:59.000000 RPQ-pytorch-0.0.30/RPQ_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-19 22:13:59.000000 RPQ-pytorch-0.0.30/RPQ_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-19 22:13:59.000000 RPQ-pytorch-0.0.30/RPQ_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:13:59.646553 RPQ-pytorch-0.0.30/rpq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 22:13:43.000000 RPQ-pytorch-0.0.30/rpq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:13:59.646553 RPQ-pytorch-0.0.30/rpq/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-19 22:13:43.000000 RPQ-pytorch-0.0.30/rpq/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57773 2023-05-19 22:13:43.000000 RPQ-pytorch-0.0.30/rpq/models/rpqopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-05-19 22:13:43.000000 RPQ-pytorch-0.0.30/rpq/models/rpqvit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12165 2023-05-19 22:13:43.000000 RPQ-pytorch-0.0.30/rpq/nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-19 22:13:43.000000 RPQ-pytorch-0.0.30/rpq/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 22:13:59.646553 RPQ-pytorch-0.0.30/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-19 22:13:43.000000 RPQ-pytorch-0.0.30/setup.py
```

### Comparing `RPQ-pytorch-0.0.3/LICENSE` & `RPQ-pytorch-0.0.30/LICENSE`

 * *Files identical despite different names*

### Comparing `RPQ-pytorch-0.0.3/PKG-INFO` & `RPQ-pytorch-0.0.30/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RPQ-pytorch
-Version: 0.0.3
+Version: 0.0.30
 Summary: Reverse Product Quantization (RPQ) of weights to reduce static memory usage.
 Home-page: https://github.com/a-kore/RPQ-pytorch
 Author: Ali Kore
 Author-email: akore654@gmail.com
 License: MIT
 Keywords: artificial intelligence,AI,machine learning,deep learning,pytorch,quantization,product quantization,reverse product quantization,memory reduction
 Classifier: Development Status :: 4 - Beta
```

### Comparing `RPQ-pytorch-0.0.3/README.md` & `RPQ-pytorch-0.0.30/README.md`

 * *Files identical despite different names*

### Comparing `RPQ-pytorch-0.0.3/RPQ_pytorch.egg-info/PKG-INFO` & `RPQ-pytorch-0.0.30/RPQ_pytorch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RPQ-pytorch
-Version: 0.0.3
+Version: 0.0.30
 Summary: Reverse Product Quantization (RPQ) of weights to reduce static memory usage.
 Home-page: https://github.com/a-kore/RPQ-pytorch
 Author: Ali Kore
 Author-email: akore654@gmail.com
 License: MIT
 Keywords: artificial intelligence,AI,machine learning,deep learning,pytorch,quantization,product quantization,reverse product quantization,memory reduction
 Classifier: Development Status :: 4 - Beta
```

### Comparing `RPQ-pytorch-0.0.3/rpq/models/rpqopt.py` & `RPQ-pytorch-0.0.30/rpq/models/rpqopt.py`

 * *Files identical despite different names*

### Comparing `RPQ-pytorch-0.0.3/rpq/models/rpqvit.py` & `RPQ-pytorch-0.0.30/rpq/models/rpqvit.py`

 * *Files identical despite different names*

### Comparing `RPQ-pytorch-0.0.3/rpq/nn.py` & `RPQ-pytorch-0.0.30/rpq/nn.py`

 * *Files identical despite different names*

### Comparing `RPQ-pytorch-0.0.3/setup.py` & `RPQ-pytorch-0.0.30/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'RPQ-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.0.3',
+  version = '0.0.30',
   license='MIT',
   description = 'Reverse Product Quantization (RPQ) of weights to reduce static memory usage.',
   author = 'Ali Kore',
   author_email = 'akore654@gmail.com',
   long_description=open('README.md', 'r').read(),
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/a-kore/RPQ-pytorch',
```

