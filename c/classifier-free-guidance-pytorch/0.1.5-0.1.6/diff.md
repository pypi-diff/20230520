# Comparing `tmp/classifier-free-guidance-pytorch-0.1.5.tar.gz` & `tmp/classifier-free-guidance-pytorch-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "classifier-free-guidance-pytorch-0.1.5.tar", last modified: Fri May 19 18:13:00 2023, max compression
+gzip compressed data, was "classifier-free-guidance-pytorch-0.1.6.tar", last modified: Fri May 19 20:58:55 2023, max compression
```

## Comparing `classifier-free-guidance-pytorch-0.1.5.tar` & `classifier-free-guidance-pytorch-0.1.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:13:00.143517 classifier-free-guidance-pytorch-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-19 18:12:49.000000 classifier-free-guidance-pytorch-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-19 18:12:49.000000 classifier-free-guidance-pytorch-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-19 18:13:00.143517 classifier-free-guidance-pytorch-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7434 2023-05-19 18:12:49.000000 classifier-free-guidance-pytorch-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:13:00.139517 classifier-free-guidance-pytorch-0.1.5/classifier_free_guidance_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-19 18:12:49.000000 classifier-free-guidance-pytorch-0.1.5/classifier_free_guidance_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-05-19 18:12:49.000000 classifier-free-guidance-pytorch-0.1.5/classifier_free_guidance_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)    16690 2023-05-19 18:12:49.000000 classifier-free-guidance-pytorch-0.1.5/classifier_free_guidance_pytorch/classifier_free_guidance_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:13:00.139517 classifier-free-guidance-pytorch-0.1.5/classifier_free_guidance_pytorch/data/
--rw-r--r--   0 runner    (1001) docker     (123)  3194984 2023-05-19 18:12:49.000000 classifier-free-guidance-pytorch-0.1.5/classifier_free_guidance_pytorch/data/bpe_simple_vocab_16e6.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-05-19 18:12:49.000000 classifier-free-guidance-pytorch-0.1.5/classifier_free_guidance_pytorch/open_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-05-19 18:12:49.000000 classifier-free-guidance-pytorch-0.1.5/classifier_free_guidance_pytorch/t5.py
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-05-19 18:12:49.000000 classifier-free-guidance-pytorch-0.1.5/classifier_free_guidance_pytorch/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:13:00.139517 classifier-free-guidance-pytorch-0.1.5/classifier_free_guidance_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-19 18:13:00.000000 classifier-free-guidance-pytorch-0.1.5/classifier_free_guidance_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-19 18:13:00.000000 classifier-free-guidance-pytorch-0.1.5/classifier_free_guidance_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 18:13:00.000000 classifier-free-guidance-pytorch-0.1.5/classifier_free_guidance_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-19 18:13:00.000000 classifier-free-guidance-pytorch-0.1.5/classifier_free_guidance_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-19 18:13:00.000000 classifier-free-guidance-pytorch-0.1.5/classifier_free_guidance_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 18:13:00.143517 classifier-free-guidance-pytorch-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-19 18:12:49.000000 classifier-free-guidance-pytorch-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:58:55.732567 classifier-free-guidance-pytorch-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-19 20:58:44.000000 classifier-free-guidance-pytorch-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-19 20:58:44.000000 classifier-free-guidance-pytorch-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-19 20:58:55.732567 classifier-free-guidance-pytorch-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7434 2023-05-19 20:58:44.000000 classifier-free-guidance-pytorch-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:58:55.728567 classifier-free-guidance-pytorch-0.1.6/classifier_free_guidance_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-19 20:58:44.000000 classifier-free-guidance-pytorch-0.1.6/classifier_free_guidance_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-05-19 20:58:44.000000 classifier-free-guidance-pytorch-0.1.6/classifier_free_guidance_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17546 2023-05-19 20:58:44.000000 classifier-free-guidance-pytorch-0.1.6/classifier_free_guidance_pytorch/classifier_free_guidance_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:58:55.728567 classifier-free-guidance-pytorch-0.1.6/classifier_free_guidance_pytorch/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  3194984 2023-05-19 20:58:44.000000 classifier-free-guidance-pytorch-0.1.6/classifier_free_guidance_pytorch/data/bpe_simple_vocab_16e6.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-05-19 20:58:44.000000 classifier-free-guidance-pytorch-0.1.6/classifier_free_guidance_pytorch/open_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-05-19 20:58:44.000000 classifier-free-guidance-pytorch-0.1.6/classifier_free_guidance_pytorch/t5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-05-19 20:58:44.000000 classifier-free-guidance-pytorch-0.1.6/classifier_free_guidance_pytorch/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:58:55.728567 classifier-free-guidance-pytorch-0.1.6/classifier_free_guidance_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-19 20:58:55.000000 classifier-free-guidance-pytorch-0.1.6/classifier_free_guidance_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-19 20:58:55.000000 classifier-free-guidance-pytorch-0.1.6/classifier_free_guidance_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 20:58:55.000000 classifier-free-guidance-pytorch-0.1.6/classifier_free_guidance_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-19 20:58:55.000000 classifier-free-guidance-pytorch-0.1.6/classifier_free_guidance_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-19 20:58:55.000000 classifier-free-guidance-pytorch-0.1.6/classifier_free_guidance_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 20:58:55.732567 classifier-free-guidance-pytorch-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-19 20:58:44.000000 classifier-free-guidance-pytorch-0.1.6/setup.py
```

### Comparing `classifier-free-guidance-pytorch-0.1.5/LICENSE` & `classifier-free-guidance-pytorch-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `classifier-free-guidance-pytorch-0.1.5/PKG-INFO` & `classifier-free-guidance-pytorch-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: classifier-free-guidance-pytorch
-Version: 0.1.5
+Version: 0.1.6
 Summary: Classifier Free Guidance - Pytorch
 Home-page: https://github.com/lucidrains/classifier-free-guidance-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,classifier free guidance,text conditioning and guidance
 Classifier: Development Status :: 4 - Beta
```

### Comparing `classifier-free-guidance-pytorch-0.1.5/README.md` & `classifier-free-guidance-pytorch-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `classifier-free-guidance-pytorch-0.1.5/classifier_free_guidance_pytorch/attend.py` & `classifier-free-guidance-pytorch-0.1.6/classifier_free_guidance_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `classifier-free-guidance-pytorch-0.1.5/classifier_free_guidance_pytorch/classifier_free_guidance_pytorch.py` & `classifier-free-guidance-pytorch-0.1.6/classifier_free_guidance_pytorch/classifier_free_guidance_pytorch.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,29 +84,33 @@
                 texts = kwargs.pop('texts', None)
                 text_embeds = kwargs.pop('text_embeds', None)
 
                 assert not (exists(texts) and exists(text_embeds))
 
                 cond_fns = None
 
+                text_conditioner = getattr(self, text_conditioner_name, None)
+
                 # auto convert texts -> conditioning functions
 
                 if exists(texts) ^ exists(text_embeds):
 
                     assert is_bearable(texts, Optional[List[str]]), f'keyword `{texts_key_name}` must be a list of strings'
 
-                    text_conditioner = getattr(self, text_conditioner_name, None)
                     assert exists(text_conditioner) and is_bearable(text_conditioner, Conditioner), 'text_conditioner must be set on your network with the correct hidden dimensions to be conditioned on'
 
                     cond_drop_prob = kwargs.pop(cond_drop_prob_keyname, None)
 
                     text_condition_input = dict(texts = texts) if exists(texts) else dict(text_embeds = text_embeds)
 
                     cond_fns = text_conditioner(**text_condition_input, cond_drop_prob = cond_drop_prob)
 
+                elif isinstance(text_conditioner, NullConditioner):
+                    cond_fns = text_conditioner()
+
                 kwargs.update(cond_fns = cond_fns)
 
             return fn(self, *args, **kwargs)
 
         # main classifier free guidance logic
 
         if self.training:
@@ -277,14 +281,44 @@
 )
 
 MODEL_TYPES = CONDITION_CONFIG.keys()
 
 class Conditioner(nn.Module):
     pass
 
+# null conditioner
+
+class Identity(nn.Module):
+    def forward(self, t, *args, **kwargs):
+        return t
+
+@beartype
+class NullConditioner(Conditioner):
+    def __init__(
+        self,
+        *,
+        num_null_conditioners: int
+    ):
+        super().__init__()
+        self.cond_fns = tuple(Identity() for _ in range(num_null_conditioners))
+
+        self.register_buffer('_device_param', torch.tensor(0.), persistent = False)
+
+    @property
+    def device(self):
+        return next(self.buffers()).device
+
+    def embed_texts(self, texts: List[str]):
+        assert False, 'null conditioner cannot embed text'
+
+    def forward(self, *args, **kwarg) -> Tuple[Identity, ...]:
+        return self.cond_fns
+
+# text conditioner with FiLM
+
 @beartype
 class TextConditioner(Conditioner):
     def __init__(
         self,
         *,
         hidden_dims: Tuple[int, ...],
         model_types = 't5',
```

### Comparing `classifier-free-guidance-pytorch-0.1.5/classifier_free_guidance_pytorch/data/bpe_simple_vocab_16e6.txt` & `classifier-free-guidance-pytorch-0.1.6/classifier_free_guidance_pytorch/data/bpe_simple_vocab_16e6.txt`

 * *Files identical despite different names*

### Comparing `classifier-free-guidance-pytorch-0.1.5/classifier_free_guidance_pytorch/open_clip.py` & `classifier-free-guidance-pytorch-0.1.6/classifier_free_guidance_pytorch/open_clip.py`

 * *Files identical despite different names*

### Comparing `classifier-free-guidance-pytorch-0.1.5/classifier_free_guidance_pytorch/t5.py` & `classifier-free-guidance-pytorch-0.1.6/classifier_free_guidance_pytorch/t5.py`

 * *Files identical despite different names*

### Comparing `classifier-free-guidance-pytorch-0.1.5/classifier_free_guidance_pytorch/tokenizer.py` & `classifier-free-guidance-pytorch-0.1.6/classifier_free_guidance_pytorch/tokenizer.py`

 * *Files identical despite different names*

### Comparing `classifier-free-guidance-pytorch-0.1.5/classifier_free_guidance_pytorch.egg-info/PKG-INFO` & `classifier-free-guidance-pytorch-0.1.6/classifier_free_guidance_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: classifier-free-guidance-pytorch
-Version: 0.1.5
+Version: 0.1.6
 Summary: Classifier Free Guidance - Pytorch
 Home-page: https://github.com/lucidrains/classifier-free-guidance-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,classifier free guidance,text conditioning and guidance
 Classifier: Development Status :: 4 - Beta
```

### Comparing `classifier-free-guidance-pytorch-0.1.5/classifier_free_guidance_pytorch.egg-info/SOURCES.txt` & `classifier-free-guidance-pytorch-0.1.6/classifier_free_guidance_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `classifier-free-guidance-pytorch-0.1.5/setup.py` & `classifier-free-guidance-pytorch-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'classifier-free-guidance-pytorch',
   packages = find_packages(exclude=[]),
   include_package_data = True,
-  version = '0.1.5',
+  version = '0.1.6',
   license='MIT',
   description = 'Classifier Free Guidance - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/classifier-free-guidance-pytorch',
   keywords = [
```

