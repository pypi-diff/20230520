# Comparing `tmp/hf_hub_ctranslate2-2.0.7.tar.gz` & `tmp/hf_hub_ctranslate2-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hf_hub_ctranslate2-2.0.7.tar", last modified: Sat May 20 00:06:29 2023, max compression
+gzip compressed data, was "hf_hub_ctranslate2-2.0.8.tar", last modified: Sat May 20 00:36:46 2023, max compression
```

## Comparing `hf_hub_ctranslate2-2.0.7.tar` & `hf_hub_ctranslate2-2.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:06:29.373404 hf_hub_ctranslate2-2.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-20 00:06:20.000000 hf_hub_ctranslate2-2.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-20 00:06:29.373404 hf_hub_ctranslate2-2.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-05-20 00:06:20.000000 hf_hub_ctranslate2-2.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:06:29.373404 hf_hub_ctranslate2-2.0.7/hf_hub_ctranslate2/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-20 00:06:20.000000 hf_hub_ctranslate2-2.0.7/hf_hub_ctranslate2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15455 2023-05-20 00:06:20.000000 hf_hub_ctranslate2-2.0.7/hf_hub_ctranslate2/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:06:29.373404 hf_hub_ctranslate2-2.0.7/hf_hub_ctranslate2/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 00:06:20.000000 hf_hub_ctranslate2-2.0.7/hf_hub_ctranslate2/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-20 00:06:20.000000 hf_hub_ctranslate2-2.0.7/hf_hub_ctranslate2/util/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:06:29.373404 hf_hub_ctranslate2-2.0.7/hf_hub_ctranslate2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-20 00:06:29.000000 hf_hub_ctranslate2-2.0.7/hf_hub_ctranslate2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-20 00:06:29.000000 hf_hub_ctranslate2-2.0.7/hf_hub_ctranslate2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 00:06:29.000000 hf_hub_ctranslate2-2.0.7/hf_hub_ctranslate2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-20 00:06:29.000000 hf_hub_ctranslate2-2.0.7/hf_hub_ctranslate2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-20 00:06:29.000000 hf_hub_ctranslate2-2.0.7/hf_hub_ctranslate2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-20 00:06:20.000000 hf_hub_ctranslate2-2.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 00:06:29.373404 hf_hub_ctranslate2-2.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-20 00:06:20.000000 hf_hub_ctranslate2-2.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:06:29.373404 hf_hub_ctranslate2-2.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-20 00:06:20.000000 hf_hub_ctranslate2-2.0.7/tests/test_translate.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-20 00:06:20.000000 hf_hub_ctranslate2-2.0.7/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:36:46.713046 hf_hub_ctranslate2-2.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-20 00:36:37.000000 hf_hub_ctranslate2-2.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-20 00:36:46.713046 hf_hub_ctranslate2-2.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-05-20 00:36:37.000000 hf_hub_ctranslate2-2.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:36:46.713046 hf_hub_ctranslate2-2.0.8/hf_hub_ctranslate2/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-20 00:36:37.000000 hf_hub_ctranslate2-2.0.8/hf_hub_ctranslate2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15568 2023-05-20 00:36:37.000000 hf_hub_ctranslate2-2.0.8/hf_hub_ctranslate2/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:36:46.713046 hf_hub_ctranslate2-2.0.8/hf_hub_ctranslate2/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 00:36:37.000000 hf_hub_ctranslate2-2.0.8/hf_hub_ctranslate2/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-20 00:36:37.000000 hf_hub_ctranslate2-2.0.8/hf_hub_ctranslate2/util/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:36:46.713046 hf_hub_ctranslate2-2.0.8/hf_hub_ctranslate2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-20 00:36:46.000000 hf_hub_ctranslate2-2.0.8/hf_hub_ctranslate2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-20 00:36:46.000000 hf_hub_ctranslate2-2.0.8/hf_hub_ctranslate2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 00:36:46.000000 hf_hub_ctranslate2-2.0.8/hf_hub_ctranslate2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-20 00:36:46.000000 hf_hub_ctranslate2-2.0.8/hf_hub_ctranslate2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-20 00:36:46.000000 hf_hub_ctranslate2-2.0.8/hf_hub_ctranslate2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-20 00:36:37.000000 hf_hub_ctranslate2-2.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 00:36:46.713046 hf_hub_ctranslate2-2.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-20 00:36:37.000000 hf_hub_ctranslate2-2.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:36:46.713046 hf_hub_ctranslate2-2.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-20 00:36:37.000000 hf_hub_ctranslate2-2.0.8/tests/test_translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-20 00:36:37.000000 hf_hub_ctranslate2-2.0.8/tests/test_version.py
```

### Comparing `hf_hub_ctranslate2-2.0.7/LICENSE` & `hf_hub_ctranslate2-2.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hf_hub_ctranslate2-2.0.7/PKG-INFO` & `hf_hub_ctranslate2-2.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hf_hub_ctranslate2
-Version: 2.0.7
+Version: 2.0.8
 Summary: Connecting Transfromers on HuggingfaceHub with Ctranslate2 
 Home-page: https://github.com/michaelfeil/hf-hub-ctranslate2
 Author: Michael Feil
 License: MIT
 Project-URL: Bug Tracker, https://github.com/michaelfeil/hf-hub-ctranslate2/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hf_hub_ctranslate2-2.0.7/README.md` & `hf_hub_ctranslate2-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `hf_hub_ctranslate2-2.0.7/hf_hub_ctranslate2/translate.py` & `hf_hub_ctranslate2-2.0.8/hf_hub_ctranslate2/translate.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,18 +110,19 @@
             tokenizer,
             hub_kwargs,
         )
 
     def _forward(self, *args, **kwds):
         return self.model.translate_batch(*args, **kwds)
     
-    def tokenize_decode(self, tokens_out, *args):
+    def tokenize_decode(self, tokens_out, *args, **kwargs):
         return [
             self.tokenizer.decode(
-                self.tokenizer.convert_tokens_to_ids(tokens_out[i].hypotheses[0])
+                self.tokenizer.convert_tokens_to_ids(tokens_out[i].hypotheses[0]),
+                *args, **kwargs
             )
             for i in range(len(tokens_out))
         ]
 
     def generate(self, text: Union[str, List[str]], encode_tok_kwargs={}, decode_tok_kwargs={}, *forward_args, **forward_kwds: Any):
         """_summary_
 
@@ -203,18 +204,19 @@
         tokens = []
         src_lang = kwargs.pop("src_lang")
         for t, src_language in zip(text, src_lang):
             self.tokenizer.src_lang = src_language
             tokens.append(self.tokenizer.convert_ids_to_tokens(self.tokenizer.encode(t)))
         return tokens
     
-    def tokenize_decode(self, tokens_out, *args):
+    def tokenize_decode(self, tokens_out, *args, **kwargs):
         return [
             self.tokenizer.decode(
-                self.tokenizer.convert_tokens_to_ids(tokens_out[i].hypotheses[0][1:])
+                self.tokenizer.convert_tokens_to_ids(tokens_out[i].hypotheses[0][1:]),
+                *args, **kwargs
             )
             for i in range(len(tokens_out))
         ]
 
     def generate(self, text: Union[str, List[str]], src_lang: Union[str, List[str]], tgt_lang: Union[str, List[str]], *forward_args, **forward_kwds: Any):
         """_summary_
 
@@ -289,17 +291,17 @@
             tokenizer,
             hub_kwargs,
         )
 
     def _forward(self, *args, **kwds):
         return self.model.generate_batch(*args, **kwds)
         
-    def tokenize_decode(self, tokens_out, *args):
+    def tokenize_decode(self, tokens_out, *args, **kwargs):
         return [
-            self.tokenizer.decode(tokens_out[i].sequences_ids[0])
+            self.tokenizer.decode(tokens_out[i].sequences_ids[0], *args, **kwargs)
             for i in range(len(tokens_out))
         ]
 
         
     def generate(self, text: Union[str, List[str]], encode_tok_kwargs={}, decode_tok_kwargs={},  *forward_args, **forward_kwds: Any):
         """_summary_
```

### Comparing `hf_hub_ctranslate2-2.0.7/hf_hub_ctranslate2/util/utils.py` & `hf_hub_ctranslate2-2.0.8/hf_hub_ctranslate2/util/utils.py`

 * *Files identical despite different names*

### Comparing `hf_hub_ctranslate2-2.0.7/hf_hub_ctranslate2.egg-info/PKG-INFO` & `hf_hub_ctranslate2-2.0.8/hf_hub_ctranslate2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hf-hub-ctranslate2
-Version: 2.0.7
+Version: 2.0.8
 Summary: Connecting Transfromers on HuggingfaceHub with Ctranslate2 
 Home-page: https://github.com/michaelfeil/hf-hub-ctranslate2
 Author: Michael Feil
 License: MIT
 Project-URL: Bug Tracker, https://github.com/michaelfeil/hf-hub-ctranslate2/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hf_hub_ctranslate2-2.0.7/setup.py` & `hf_hub_ctranslate2-2.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `hf_hub_ctranslate2-2.0.7/tests/test_translate.py` & `hf_hub_ctranslate2-2.0.8/tests/test_translate.py`

 * *Files identical despite different names*

