# Comparing `tmp/fastai-datasets-0.0.5.tar.gz` & `tmp/fastai-datasets-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastai-datasets-0.0.5.tar", last modified: Thu May 18 08:47:32 2023, max compression
+gzip compressed data, was "fastai-datasets-0.0.6.tar", last modified: Sat May 20 11:11:38 2023, max compression
```

## Comparing `fastai-datasets-0.0.5.tar` & `fastai-datasets-0.0.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-05-18 08:47:32.214201 fastai-datasets-0.0.5/
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)    35149 2023-04-13 22:08:00.000000 fastai-datasets-0.0.5/LICENSE
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      111 2023-04-13 22:08:00.000000 fastai-datasets-0.0.5/MANIFEST.in
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     5493 2023-05-18 08:47:32.214201 fastai-datasets-0.0.5/PKG-INFO
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     3895 2023-05-15 14:03:48.000000 fastai-datasets-0.0.5/README.md
-drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-05-18 08:47:32.214201 fastai-datasets-0.0.5/fastai_datasets/
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      313 2023-05-18 08:47:21.000000 fastai-datasets-0.0.5/fastai_datasets/__init__.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)    12255 2023-05-18 08:47:21.000000 fastai-datasets-0.0.5/fastai_datasets/_modidx.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      172 2023-04-14 23:03:52.000000 fastai-datasets-0.0.5/fastai_datasets/all.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      461 2023-05-18 08:47:21.000000 fastai-datasets-0.0.5/fastai_datasets/cifar10.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      615 2023-05-18 08:47:21.000000 fastai-datasets-0.0.5/fastai_datasets/imagenette.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     4575 2023-05-18 08:47:21.000000 fastai-datasets-0.0.5/fastai_datasets/lfw.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      858 2023-05-18 08:47:21.000000 fastai-datasets-0.0.5/fastai_datasets/mnist.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     3675 2023-05-18 08:47:21.000000 fastai-datasets-0.0.5/fastai_datasets/pairs.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     5827 2023-05-18 08:47:21.000000 fastai-datasets-0.0.5/fastai_datasets/patches.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      796 2023-05-18 08:47:21.000000 fastai-datasets-0.0.5/fastai_datasets/pfr.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     1877 2023-05-18 08:47:21.000000 fastai-datasets-0.0.5/fastai_datasets/utils.py
-drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-05-18 08:47:32.214201 fastai-datasets-0.0.5/fastai_datasets.egg-info/
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     5493 2023-05-18 08:47:32.000000 fastai-datasets-0.0.5/fastai_datasets.egg-info/PKG-INFO
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      608 2023-05-18 08:47:32.000000 fastai-datasets-0.0.5/fastai_datasets.egg-info/SOURCES.txt
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)        1 2023-05-18 08:47:32.000000 fastai-datasets-0.0.5/fastai_datasets.egg-info/dependency_links.txt
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       73 2023-05-18 08:47:32.000000 fastai-datasets-0.0.5/fastai_datasets.egg-info/entry_points.txt
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)        1 2023-04-13 22:13:24.000000 fastai-datasets-0.0.5/fastai_datasets.egg-info/not-zip-safe
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       30 2023-05-18 08:47:32.000000 fastai-datasets-0.0.5/fastai_datasets.egg-info/requires.txt
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       16 2023-05-18 08:47:32.000000 fastai-datasets-0.0.5/fastai_datasets.egg-info/top_level.txt
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      991 2023-05-18 08:46:47.000000 fastai-datasets-0.0.5/settings.ini
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       38 2023-05-18 08:47:32.214201 fastai-datasets-0.0.5/setup.cfg
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     2560 2023-04-13 22:08:00.000000 fastai-datasets-0.0.5/setup.py
+drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-05-20 11:11:38.643440 fastai-datasets-0.0.6/
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)    35149 2023-04-13 22:08:00.000000 fastai-datasets-0.0.6/LICENSE
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      111 2023-04-13 22:08:00.000000 fastai-datasets-0.0.6/MANIFEST.in
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     5419 2023-05-20 11:11:38.643440 fastai-datasets-0.0.6/PKG-INFO
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     3821 2023-05-20 11:10:54.000000 fastai-datasets-0.0.6/README.md
+drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-05-20 11:11:38.639440 fastai-datasets-0.0.6/fastai_datasets/
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      313 2023-05-20 11:11:30.000000 fastai-datasets-0.0.6/fastai_datasets/__init__.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)    12255 2023-05-20 11:11:30.000000 fastai-datasets-0.0.6/fastai_datasets/_modidx.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      172 2023-04-14 23:03:52.000000 fastai-datasets-0.0.6/fastai_datasets/all.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      461 2023-05-20 11:11:30.000000 fastai-datasets-0.0.6/fastai_datasets/cifar10.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      947 2023-05-20 11:11:30.000000 fastai-datasets-0.0.6/fastai_datasets/imagenette.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     4575 2023-05-20 11:11:30.000000 fastai-datasets-0.0.6/fastai_datasets/lfw.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      882 2023-05-20 11:11:30.000000 fastai-datasets-0.0.6/fastai_datasets/mnist.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     3761 2023-05-20 11:11:30.000000 fastai-datasets-0.0.6/fastai_datasets/pairs.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     5827 2023-05-20 11:11:30.000000 fastai-datasets-0.0.6/fastai_datasets/patches.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      796 2023-05-20 11:11:30.000000 fastai-datasets-0.0.6/fastai_datasets/pfr.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     1877 2023-05-20 11:11:30.000000 fastai-datasets-0.0.6/fastai_datasets/utils.py
+drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-05-20 11:11:38.639440 fastai-datasets-0.0.6/fastai_datasets.egg-info/
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     5419 2023-05-20 11:11:38.000000 fastai-datasets-0.0.6/fastai_datasets.egg-info/PKG-INFO
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      608 2023-05-20 11:11:38.000000 fastai-datasets-0.0.6/fastai_datasets.egg-info/SOURCES.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)        1 2023-05-20 11:11:38.000000 fastai-datasets-0.0.6/fastai_datasets.egg-info/dependency_links.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       73 2023-05-20 11:11:38.000000 fastai-datasets-0.0.6/fastai_datasets.egg-info/entry_points.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)        1 2023-04-13 22:13:24.000000 fastai-datasets-0.0.6/fastai_datasets.egg-info/not-zip-safe
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       30 2023-05-20 11:11:38.000000 fastai-datasets-0.0.6/fastai_datasets.egg-info/requires.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       16 2023-05-20 11:11:38.000000 fastai-datasets-0.0.6/fastai_datasets.egg-info/top_level.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      991 2023-05-20 11:10:39.000000 fastai-datasets-0.0.6/settings.ini
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       38 2023-05-20 11:11:38.643440 fastai-datasets-0.0.6/setup.cfg
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     2560 2023-04-13 22:08:00.000000 fastai-datasets-0.0.6/setup.py
```

### Comparing `fastai-datasets-0.0.5/LICENSE` & `fastai-datasets-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fastai-datasets-0.0.5/fastai_datasets/_modidx.py` & `fastai-datasets-0.0.6/fastai_datasets/_modidx.py`

 * *Files identical despite different names*

### Comparing `fastai-datasets-0.0.5/fastai_datasets/lfw.py` & `fastai-datasets-0.0.6/fastai_datasets/lfw.py`

 * *Files identical despite different names*

### Comparing `fastai-datasets-0.0.5/fastai_datasets/mnist.py` & `fastai-datasets-0.0.6/fastai_datasets/mnist.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 from fastai.vision.all import *
 
 import fastai_datasets.patches
 
 # %% ../nbs/mnist.ipynb 4
 def MNIST(sample=False):
     return DataBlock(
-        blocks=(ImageBlock, CategoryBlock),
+        blocks=(ImageBlock(PILImageBW), CategoryBlock),
         get_items=get_image_files,
         get_y=parent_label,
         splitter=GrandparentSplitter('training', 'testing') if not sample else GrandparentSplitter()
     ).datasets(untar_data(URLs.MNIST if not sample else URLs.MNIST_SAMPLE))
 
 def TinyMNIST():
     return DataBlock(
-        blocks=(ImageBlock, CategoryBlock),
+        blocks=(ImageBlock(PILImageBW), CategoryBlock),
         get_items=partial(get_image_files, folders=['train', 'valid']),
         get_y=parent_label,
         splitter=GrandparentSplitter(),
     ).datasets(untar_data(URLs.MNIST_TINY))
```

### Comparing `fastai-datasets-0.0.5/fastai_datasets/pairs.py` & `fastai-datasets-0.0.6/fastai_datasets/pairs.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,18 +15,20 @@
 
 # %% ../nbs/pairs.ipynb 3
 class ImagePair(fastuple):
     """Adds showing functionality to fastai's `fastuple`"""
     @classmethod
     def create(cls, fns): return cls(tuple(PILImage.create(f) for f in fns))
     
-    def show(self, ctx=None, **kwargs): 
+    def show(self, ctx=None, **kwargs):
         t1,t2 = ToTensor()(self)
-        line = t1.new_zeros(t1.shape[0], t1.shape[1], 1)
-        return show_image(torch.cat([t1,line,t2], dim=2), ctx=ctx, **kwargs)
+        assert type(t1) == type(t2)
+        line = t1.new_zeros((t1.shape[0], t1.shape[1], 1))
+        joint_image = torch.cat([t1,line,t2], dim=2).as_subclass(type(t1))
+        return joint_image.show(ctx=ctx, **kwargs)
 
 class Sameness(Categorize):
     """Converts boolean/binary labels into "Not Same"/"Same" labels"""
     def __init__(self):
         super().__init__(['Not Same', 'Same'], sort=False)
 
     def encodes(self, o: Union[bool, int]):
```

### Comparing `fastai-datasets-0.0.5/fastai_datasets/patches.py` & `fastai-datasets-0.0.6/fastai_datasets/patches.py`

 * *Files identical despite different names*

### Comparing `fastai-datasets-0.0.5/fastai_datasets/pfr.py` & `fastai-datasets-0.0.6/fastai_datasets/pfr.py`

 * *Files identical despite different names*

### Comparing `fastai-datasets-0.0.5/fastai_datasets/utils.py` & `fastai-datasets-0.0.6/fastai_datasets/utils.py`

 * *Files identical despite different names*

### Comparing `fastai-datasets-0.0.5/fastai_datasets.egg-info/SOURCES.txt` & `fastai-datasets-0.0.6/fastai_datasets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastai-datasets-0.0.5/settings.ini` & `fastai-datasets-0.0.6/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = fastai-datasets
 lib_name = %(repo)s
-version = 0.0.5
+version = 0.0.6
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = fastai_datasets
```

### Comparing `fastai-datasets-0.0.5/setup.py` & `fastai-datasets-0.0.6/setup.py`

 * *Files identical despite different names*

