# Comparing `tmp/hf_hub_ctranslate2-2.0.6.tar.gz` & `tmp/hf_hub_ctranslate2-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hf_hub_ctranslate2-2.0.6.tar", last modified: Fri May 19 00:06:26 2023, max compression
+gzip compressed data, was "hf_hub_ctranslate2-2.0.7.tar", last modified: Sat May 20 00:06:29 2023, max compression
```

## Comparing `hf_hub_ctranslate2-2.0.6.tar` & `hf_hub_ctranslate2-2.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:06:26.594873 hf_hub_ctranslate2-2.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-19 00:06:16.000000 hf_hub_ctranslate2-2.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-19 00:06:26.590873 hf_hub_ctranslate2-2.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-05-19 00:06:16.000000 hf_hub_ctranslate2-2.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:06:26.590873 hf_hub_ctranslate2-2.0.6/hf_hub_ctranslate2/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-19 00:06:16.000000 hf_hub_ctranslate2-2.0.6/hf_hub_ctranslate2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14878 2023-05-19 00:06:16.000000 hf_hub_ctranslate2-2.0.6/hf_hub_ctranslate2/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:06:26.590873 hf_hub_ctranslate2-2.0.6/hf_hub_ctranslate2/util/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-19 00:06:16.000000 hf_hub_ctranslate2-2.0.6/hf_hub_ctranslate2/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-19 00:06:16.000000 hf_hub_ctranslate2-2.0.6/hf_hub_ctranslate2/util/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:06:26.590873 hf_hub_ctranslate2-2.0.6/hf_hub_ctranslate2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-19 00:06:26.000000 hf_hub_ctranslate2-2.0.6/hf_hub_ctranslate2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-19 00:06:26.000000 hf_hub_ctranslate2-2.0.6/hf_hub_ctranslate2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 00:06:26.000000 hf_hub_ctranslate2-2.0.6/hf_hub_ctranslate2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-19 00:06:26.000000 hf_hub_ctranslate2-2.0.6/hf_hub_ctranslate2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-19 00:06:26.000000 hf_hub_ctranslate2-2.0.6/hf_hub_ctranslate2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-19 00:06:16.000000 hf_hub_ctranslate2-2.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 00:06:26.594873 hf_hub_ctranslate2-2.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-19 00:06:16.000000 hf_hub_ctranslate2-2.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:06:26.590873 hf_hub_ctranslate2-2.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-05-19 00:06:16.000000 hf_hub_ctranslate2-2.0.6/tests/test_translate.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-19 00:06:16.000000 hf_hub_ctranslate2-2.0.6/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:06:29.373404 hf_hub_ctranslate2-2.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-20 00:06:20.000000 hf_hub_ctranslate2-2.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-20 00:06:29.373404 hf_hub_ctranslate2-2.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-05-20 00:06:20.000000 hf_hub_ctranslate2-2.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:06:29.373404 hf_hub_ctranslate2-2.0.7/hf_hub_ctranslate2/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-20 00:06:20.000000 hf_hub_ctranslate2-2.0.7/hf_hub_ctranslate2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15455 2023-05-20 00:06:20.000000 hf_hub_ctranslate2-2.0.7/hf_hub_ctranslate2/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:06:29.373404 hf_hub_ctranslate2-2.0.7/hf_hub_ctranslate2/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 00:06:20.000000 hf_hub_ctranslate2-2.0.7/hf_hub_ctranslate2/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-20 00:06:20.000000 hf_hub_ctranslate2-2.0.7/hf_hub_ctranslate2/util/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:06:29.373404 hf_hub_ctranslate2-2.0.7/hf_hub_ctranslate2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-20 00:06:29.000000 hf_hub_ctranslate2-2.0.7/hf_hub_ctranslate2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-20 00:06:29.000000 hf_hub_ctranslate2-2.0.7/hf_hub_ctranslate2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 00:06:29.000000 hf_hub_ctranslate2-2.0.7/hf_hub_ctranslate2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-20 00:06:29.000000 hf_hub_ctranslate2-2.0.7/hf_hub_ctranslate2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-20 00:06:29.000000 hf_hub_ctranslate2-2.0.7/hf_hub_ctranslate2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-20 00:06:20.000000 hf_hub_ctranslate2-2.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 00:06:29.373404 hf_hub_ctranslate2-2.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-20 00:06:20.000000 hf_hub_ctranslate2-2.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:06:29.373404 hf_hub_ctranslate2-2.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-20 00:06:20.000000 hf_hub_ctranslate2-2.0.7/tests/test_translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-20 00:06:20.000000 hf_hub_ctranslate2-2.0.7/tests/test_version.py
```

### Comparing `hf_hub_ctranslate2-2.0.6/LICENSE` & `hf_hub_ctranslate2-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hf_hub_ctranslate2-2.0.6/PKG-INFO` & `hf_hub_ctranslate2-2.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hf_hub_ctranslate2
-Version: 2.0.6
+Version: 2.0.7
 Summary: Connecting Transfromers on HuggingfaceHub with Ctranslate2 
 Home-page: https://github.com/michaelfeil/hf-hub-ctranslate2
 Author: Michael Feil
 License: MIT
 Project-URL: Bug Tracker, https://github.com/michaelfeil/hf-hub-ctranslate2/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hf_hub_ctranslate2-2.0.6/README.md` & `hf_hub_ctranslate2-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `hf_hub_ctranslate2-2.0.6/hf_hub_ctranslate2/translate.py` & `hf_hub_ctranslate2-2.0.7/hf_hub_ctranslate2/translate.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,22 +63,22 @@
     def tokenize_encode(self, text, *args, **kwargs):
         return [
             self.tokenizer.convert_ids_to_tokens(self.tokenizer.encode(p)) for p in text
         ]
     def tokenize_decode(self, tokens_out, *args, **kwargs):
         raise NotImplementedError
 
-    def generate(self, text: Union[str, List[str]], encode_kwargs={}, *forward_args, **forward_kwds: Any):
+    def generate(self, text: Union[str, List[str]], encode_kwargs={}, decode_kwargs={}, *forward_args, **forward_kwds: Any):
         orig_type = list
         if isinstance(text, str):
             orig_type = str
             text = [text]
         token_list = self.tokenize_encode(text, **encode_kwargs)
         tokens_out = self._forward(token_list, *forward_args, **forward_kwds)
-        texts_out = self.tokenize_decode(tokens_out)
+        texts_out = self.tokenize_decode(tokens_out, **decode_kwargs)
         if orig_type == str:
             return texts_out[0]
         else:
             return texts_out
 
 
 class TranslatorCT2fromHfHub(CTranslate2ModelfromHuggingfaceHub):
@@ -118,19 +118,21 @@
         return [
             self.tokenizer.decode(
                 self.tokenizer.convert_tokens_to_ids(tokens_out[i].hypotheses[0])
             )
             for i in range(len(tokens_out))
         ]
 
-    def generate(self, text: Union[str, List[str]], *forward_args, **forward_kwds: Any):
+    def generate(self, text: Union[str, List[str]], encode_tok_kwargs={}, decode_tok_kwargs={}, *forward_args, **forward_kwds: Any):
         """_summary_
 
         Args:
             text (Union[str, List[str]]): Input texts
+            encode_tok_kwargs (dict, optional): additional kwargs for tokenizer
+            decode_tok_kwargs (dict, optional): additional kwargs for tokenizer
             max_batch_size (int, optional): Batch size. Defaults to 0.
             batch_type (str, optional): _. Defaults to "examples".
             asynchronous (bool, optional): Only False supported. Defaults to False.
             beam_size (int, optional): _. Defaults to 2.
             patience (float, optional): _. Defaults to 1.
             num_hypotheses (int, optional): _. Defaults to 1.
             length_penalty (float, optional): _. Defaults to 1.
@@ -156,15 +158,15 @@
             sampling_temperature (float, optional): _. Defaults to 1.
             replace_unknowns (bool, optional): _. Defaults to False.
             callback (_type_, optional): _. Defaults to None.
 
         Returns:
             Union[str, List[str]]: text as output, if list, same len as input
         """
-        return super().generate(text, *forward_args, **forward_kwds)
+        return super().generate(text, encode_kwargs=encode_tok_kwargs, decode_kwargs=decode_tok_kwargs, *forward_args, **forward_kwds)
 
 class MultiLingualTranslatorCT2fromHfHub(CTranslate2ModelfromHuggingfaceHub):
     def __init__(
         self,
         model_name_or_path: str,
         device: Literal["cpu", "cuda"] = "cuda",
         device_index=0,
@@ -294,19 +296,21 @@
     def tokenize_decode(self, tokens_out, *args):
         return [
             self.tokenizer.decode(tokens_out[i].sequences_ids[0])
             for i in range(len(tokens_out))
         ]
 
         
-    def generate(self, text: Union[str, List[str]], *forward_args, **forward_kwds: Any):
+    def generate(self, text: Union[str, List[str]], encode_tok_kwargs={}, decode_tok_kwargs={},  *forward_args, **forward_kwds: Any):
         """_summary_
 
         Args:
             text (str | List[str]): Input texts
+            encode_tok_kwargs (dict, optional): additional kwargs for tokenizer
+            decode_tok_kwargs (dict, optional): additional kwargs for tokenizer
             max_batch_size (int, optional): _. Defaults to 0.
             batch_type (str, optional): _. Defaults to 'examples'.
             asynchronous (bool, optional): _. Defaults to False.
             beam_size (int, optional): _. Defaults to 1.
             patience (float, optional): _. Defaults to 1.
             num_hypotheses (int, optional): _. Defaults to 1.
             length_penalty (float, optional): _. Defaults to 1.
@@ -326,9 +330,9 @@
             min_alternative_expansion_prob (float, optional): _. Defaults to 0.
             sampling_topk (int, optional): _. Defaults to 1.
             sampling_temperature (float, optional): _. Defaults to 1.
 
         Returns:
             str | List[str]: text as output, if list, same len as input
         """
-        return super().generate(text, *forward_args, **forward_kwds)
+        return super().generate(text, encode_kwargs=encode_tok_kwargs, decode_kwargs=decode_tok_kwargs,  *forward_args, **forward_kwds)
```

### Comparing `hf_hub_ctranslate2-2.0.6/hf_hub_ctranslate2/util/utils.py` & `hf_hub_ctranslate2-2.0.7/hf_hub_ctranslate2/util/utils.py`

 * *Files identical despite different names*

### Comparing `hf_hub_ctranslate2-2.0.6/hf_hub_ctranslate2.egg-info/PKG-INFO` & `hf_hub_ctranslate2-2.0.7/hf_hub_ctranslate2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hf-hub-ctranslate2
-Version: 2.0.6
+Version: 2.0.7
 Summary: Connecting Transfromers on HuggingfaceHub with Ctranslate2 
 Home-page: https://github.com/michaelfeil/hf-hub-ctranslate2
 Author: Michael Feil
 License: MIT
 Project-URL: Bug Tracker, https://github.com/michaelfeil/hf-hub-ctranslate2/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hf_hub_ctranslate2-2.0.6/setup.py` & `hf_hub_ctranslate2-2.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `hf_hub_ctranslate2-2.0.6/tests/test_translate.py` & `hf_hub_ctranslate2-2.0.7/tests/test_translate.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from hf_hub_ctranslate2 import TranslatorCT2fromHfHub, GeneratorCT2fromHfHub, MultiLingualTranslatorCT2fromHfHub
-from hf_hub_ctranslate2.util import _download_model
+from hf_hub_ctranslate2.util import utils as _utils
 from transformers import AutoTokenizer
 
 
 def test_translator(model_name="michaelfeil/ct2fast-flan-alpaca-base"):
     model = TranslatorCT2fromHfHub(
         model_name_or_path=model_name, device="cpu", compute_type="int8"
     )
@@ -47,15 +47,15 @@
     assert len(outputs[0]) != len(outputs[1])
     assert "flan" in outputs[0].lower()
     for o in outputs:
         assert isinstance(o, str)
 
 
 def test_generator_single(model_name="michaelfeil/ct2fast-pythia-160m"):
-    model_path = _download_model(model_name)
+    model_path = _utils._download_model(model_name)
     tokenizer = AutoTokenizer.from_pretrained(model_path)
 
     model = GeneratorCT2fromHfHub(
         model_name_or_path=model_path,
         device="cpu",
         compute_type="int8",
         tokenizer=tokenizer,
```

