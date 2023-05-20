# Comparing `tmp/bytez-0.1.90.tar.gz` & `tmp/bytez-0.1.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bytez-0.1.90.tar", last modified: Sat May 20 01:50:51 2023, max compression
+gzip compressed data, was "bytez-0.1.91.tar", last modified: Sat May 20 01:52:44 2023, max compression
```

## Comparing `bytez-0.1.90.tar` & `bytez-0.1.91.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 01:50:51.628621 bytez-0.1.90/
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      409 2023-05-20 01:50:51.628621 bytez-0.1.90/PKG-INFO
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)       73 2023-03-26 07:05:33.000000 bytez-0.1.90/README.md
-drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 01:50:51.628621 bytez-0.1.90/bytez/
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)       38 2023-05-14 20:59:27.000000 bytez-0.1.90/bytez/__init__.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)   106186 2023-05-20 01:50:51.000000 bytez-0.1.90/bytez/exports.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)     1152 2023-05-17 01:52:53.000000 bytez-0.1.90/bytez/model.py
-drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 01:50:51.628621 bytez-0.1.90/bytez/tasks/
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-14 21:00:59.000000 bytez-0.1.90/bytez/tasks/__init__.py
-drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 01:50:51.628621 bytez-0.1.90/bytez/tasks/language_modelling/
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 01:50:51.000000 bytez-0.1.90/bytez/tasks/language_modelling/__init__.py
-drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 01:50:51.628621 bytez-0.1.90/bytez/tasks/language_modelling/_models/
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 01:50:51.000000 bytez-0.1.90/bytez/tasks/language_modelling/_models/__init__.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)     1384 2023-05-20 01:50:51.000000 bytez-0.1.90/bytez/tasks/language_modelling/_models/blinkdl_rwkv_lm.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)     1438 2023-05-17 01:53:53.000000 bytez-0.1.90/bytez/tasks/language_modelling/_models/hazyresearch_h3.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      357 2023-05-20 01:50:51.000000 bytez-0.1.90/bytez/tasks/language_modelling/models.py
-drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 01:50:51.628621 bytez-0.1.90/bytez/tasks/style_transfer/
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-14 21:02:57.000000 bytez-0.1.90/bytez/tasks/style_transfer/__init__.py
-drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 01:50:51.628621 bytez-0.1.90/bytez/tasks/style_transfer/_models/
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-14 21:02:59.000000 bytez-0.1.90/bytez/tasks/style_transfer/_models/__init__.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      761 2023-05-14 20:47:16.000000 bytez-0.1.90/bytez/tasks/style_transfer/_models/cmd_style_transfer.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      686 2023-05-14 20:47:16.000000 bytez-0.1.90/bytez/tasks/style_transfer/_models/fast_style_transfer.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      706 2023-05-14 20:47:16.000000 bytez-0.1.90/bytez/tasks/style_transfer/_models/tensorflow_fast_style.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      547 2023-05-14 20:47:16.000000 bytez-0.1.90/bytez/tasks/style_transfer/models.py
-drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 01:50:51.628621 bytez-0.1.90/bytez/tasks/super_resolution/
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-14 21:01:49.000000 bytez-0.1.90/bytez/tasks/super_resolution/__init__.py
-drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 01:50:51.628621 bytez-0.1.90/bytez/tasks/super_resolution/_models/
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-14 21:02:22.000000 bytez-0.1.90/bytez/tasks/super_resolution/_models/__init__.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)     2478 2023-05-14 20:58:15.000000 bytez-0.1.90/bytez/tasks/super_resolution/_models/holmes_alan_dsrvae.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      224 2023-05-14 20:58:15.000000 bytez-0.1.90/bytez/tasks/super_resolution/models.py
-drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 01:50:51.628621 bytez-0.1.90/bytez/tasks/text_summarization/
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-15 21:02:31.000000 bytez-0.1.90/bytez/tasks/text_summarization/__init__.py
-drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 01:50:51.628621 bytez-0.1.90/bytez/tasks/text_summarization/_models/
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-15 21:02:31.000000 bytez-0.1.90/bytez/tasks/text_summarization/_models/__init__.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      803 2023-05-14 21:13:12.000000 bytez-0.1.90/bytez/tasks/text_summarization/_models/chriskhanhtran_bert_extractive_summarization.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)     1079 2023-05-15 21:02:31.000000 bytez-0.1.90/bytez/tasks/text_summarization/_models/dmmiller612_bert_extractive_summarizer.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      564 2023-05-20 01:50:06.000000 bytez-0.1.90/bytez/tasks/text_summarization/models.py
-drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 01:50:51.628621 bytez-0.1.90/bytez.egg-info/
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      409 2023-05-20 01:50:51.000000 bytez-0.1.90/bytez.egg-info/PKG-INFO
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)     1276 2023-05-20 01:50:51.000000 bytez-0.1.90/bytez.egg-info/SOURCES.txt
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        1 2023-05-20 01:50:51.000000 bytez-0.1.90/bytez.egg-info/dependency_links.txt
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)       70 2023-05-20 01:50:51.000000 bytez-0.1.90/bytez.egg-info/requires.txt
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        6 2023-05-20 01:50:51.000000 bytez-0.1.90/bytez.egg-info/top_level.txt
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)       38 2023-05-20 01:50:51.628621 bytez-0.1.90/setup.cfg
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      663 2023-05-20 01:50:51.000000 bytez-0.1.90/setup.py
+drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 01:52:44.039034 bytez-0.1.91/
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      409 2023-05-20 01:52:44.039034 bytez-0.1.91/PKG-INFO
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)       73 2023-03-26 07:05:33.000000 bytez-0.1.91/README.md
+drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 01:52:44.039034 bytez-0.1.91/bytez/
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)       38 2023-05-14 20:59:27.000000 bytez-0.1.91/bytez/__init__.py
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)   106186 2023-05-20 01:52:43.000000 bytez-0.1.91/bytez/exports.py
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)     1152 2023-05-17 01:52:53.000000 bytez-0.1.91/bytez/model.py
+drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 01:52:44.039034 bytez-0.1.91/bytez/tasks/
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-14 21:00:59.000000 bytez-0.1.91/bytez/tasks/__init__.py
+drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 01:52:44.039034 bytez-0.1.91/bytez/tasks/language_modelling/
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 01:52:43.000000 bytez-0.1.91/bytez/tasks/language_modelling/__init__.py
+drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 01:52:44.039034 bytez-0.1.91/bytez/tasks/language_modelling/_models/
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 01:52:43.000000 bytez-0.1.91/bytez/tasks/language_modelling/_models/__init__.py
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)     1376 2023-05-20 01:52:43.000000 bytez-0.1.91/bytez/tasks/language_modelling/_models/blinkdl_rwkv_lm.py
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)     1438 2023-05-17 01:53:53.000000 bytez-0.1.91/bytez/tasks/language_modelling/_models/hazyresearch_h3.py
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      357 2023-05-20 01:50:51.000000 bytez-0.1.91/bytez/tasks/language_modelling/models.py
+drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 01:52:44.039034 bytez-0.1.91/bytez/tasks/style_transfer/
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-14 21:02:57.000000 bytez-0.1.91/bytez/tasks/style_transfer/__init__.py
+drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 01:52:44.039034 bytez-0.1.91/bytez/tasks/style_transfer/_models/
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-14 21:02:59.000000 bytez-0.1.91/bytez/tasks/style_transfer/_models/__init__.py
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      761 2023-05-14 20:47:16.000000 bytez-0.1.91/bytez/tasks/style_transfer/_models/cmd_style_transfer.py
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      686 2023-05-14 20:47:16.000000 bytez-0.1.91/bytez/tasks/style_transfer/_models/fast_style_transfer.py
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      706 2023-05-14 20:47:16.000000 bytez-0.1.91/bytez/tasks/style_transfer/_models/tensorflow_fast_style.py
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      547 2023-05-14 20:47:16.000000 bytez-0.1.91/bytez/tasks/style_transfer/models.py
+drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 01:52:44.039034 bytez-0.1.91/bytez/tasks/super_resolution/
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-14 21:01:49.000000 bytez-0.1.91/bytez/tasks/super_resolution/__init__.py
+drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 01:52:44.039034 bytez-0.1.91/bytez/tasks/super_resolution/_models/
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-14 21:02:22.000000 bytez-0.1.91/bytez/tasks/super_resolution/_models/__init__.py
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)     2478 2023-05-14 20:58:15.000000 bytez-0.1.91/bytez/tasks/super_resolution/_models/holmes_alan_dsrvae.py
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      224 2023-05-14 20:58:15.000000 bytez-0.1.91/bytez/tasks/super_resolution/models.py
+drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 01:52:44.039034 bytez-0.1.91/bytez/tasks/text_summarization/
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-15 21:02:31.000000 bytez-0.1.91/bytez/tasks/text_summarization/__init__.py
+drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 01:52:44.039034 bytez-0.1.91/bytez/tasks/text_summarization/_models/
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-15 21:02:31.000000 bytez-0.1.91/bytez/tasks/text_summarization/_models/__init__.py
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      803 2023-05-14 21:13:12.000000 bytez-0.1.91/bytez/tasks/text_summarization/_models/chriskhanhtran_bert_extractive_summarization.py
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)     1079 2023-05-15 21:02:31.000000 bytez-0.1.91/bytez/tasks/text_summarization/_models/dmmiller612_bert_extractive_summarizer.py
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      564 2023-05-20 01:50:06.000000 bytez-0.1.91/bytez/tasks/text_summarization/models.py
+drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 01:52:44.039034 bytez-0.1.91/bytez.egg-info/
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      409 2023-05-20 01:52:44.000000 bytez-0.1.91/bytez.egg-info/PKG-INFO
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)     1276 2023-05-20 01:52:44.000000 bytez-0.1.91/bytez.egg-info/SOURCES.txt
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        1 2023-05-20 01:52:44.000000 bytez-0.1.91/bytez.egg-info/dependency_links.txt
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)       70 2023-05-20 01:52:44.000000 bytez-0.1.91/bytez.egg-info/requires.txt
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        6 2023-05-20 01:52:44.000000 bytez-0.1.91/bytez.egg-info/top_level.txt
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)       38 2023-05-20 01:52:44.039034 bytez-0.1.91/setup.cfg
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      663 2023-05-20 01:52:43.000000 bytez-0.1.91/setup.py
```

### Comparing `bytez-0.1.90/bytez/exports.py` & `bytez-0.1.91/bytez/exports.py`

 * *Files identical despite different names*

### Comparing `bytez-0.1.90/bytez/model.py` & `bytez-0.1.91/bytez/model.py`

 * *Files identical despite different names*

### Comparing `bytez-0.1.90/bytez/tasks/language_modelling/_models/blinkdl_rwkv_lm.py` & `bytez-0.1.91/bytez/tasks/language_modelling/_models/blinkdl_rwkv_lm.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,12 +16,12 @@
                       
                       top_p_newline (float, optional): Control the "safeness" of the generated text at newline characters. Lower values generate safer text. Defaults to 0.9.
             
                     Returns:
                         str: The generated text as a string.
         """
 
-        request_params = {'input_text': 'input_text', 'temperature': 'temperature', 'top_p': 'top_p', 'top_p_newline': 'top_p_newline'}
+        request_params = {'input_text': input_text, 'temperature': temperature, 'top_p': top_p, 'top_p_newline': top_p_newline}
 
         url = 'https://blinkdl-rwkv-lm-tfhmsoxnpq-uc.a.run.app'
 
         return self._Model__inference(url=url, request_params=request_params)
```

### Comparing `bytez-0.1.90/bytez/tasks/language_modelling/_models/hazyresearch_h3.py` & `bytez-0.1.91/bytez/tasks/language_modelling/_models/hazyresearch_h3.py`

 * *Files identical despite different names*

### Comparing `bytez-0.1.90/bytez/tasks/style_transfer/_models/cmd_style_transfer.py` & `bytez-0.1.91/bytez/tasks/style_transfer/_models/cmd_style_transfer.py`

 * *Files identical despite different names*

### Comparing `bytez-0.1.90/bytez/tasks/style_transfer/_models/fast_style_transfer.py` & `bytez-0.1.91/bytez/tasks/style_transfer/_models/fast_style_transfer.py`

 * *Files identical despite different names*

### Comparing `bytez-0.1.90/bytez/tasks/style_transfer/_models/tensorflow_fast_style.py` & `bytez-0.1.91/bytez/tasks/style_transfer/_models/tensorflow_fast_style.py`

 * *Files identical despite different names*

### Comparing `bytez-0.1.90/bytez/tasks/style_transfer/models.py` & `bytez-0.1.91/bytez/tasks/style_transfer/models.py`

 * *Files identical despite different names*

### Comparing `bytez-0.1.90/bytez/tasks/super_resolution/_models/holmes_alan_dsrvae.py` & `bytez-0.1.91/bytez/tasks/super_resolution/_models/holmes_alan_dsrvae.py`

 * *Files identical despite different names*

### Comparing `bytez-0.1.90/bytez/tasks/text_summarization/_models/chriskhanhtran_bert_extractive_summarization.py` & `bytez-0.1.91/bytez/tasks/text_summarization/_models/chriskhanhtran_bert_extractive_summarization.py`

 * *Files identical despite different names*

### Comparing `bytez-0.1.90/bytez/tasks/text_summarization/_models/dmmiller612_bert_extractive_summarizer.py` & `bytez-0.1.91/bytez/tasks/text_summarization/_models/dmmiller612_bert_extractive_summarizer.py`

 * *Files identical despite different names*

### Comparing `bytez-0.1.90/bytez/tasks/text_summarization/models.py` & `bytez-0.1.91/bytez/tasks/text_summarization/models.py`

 * *Files identical despite different names*

### Comparing `bytez-0.1.90/bytez.egg-info/SOURCES.txt` & `bytez-0.1.91/bytez.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bytez-0.1.90/setup.py` & `bytez-0.1.91/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 packages = find_packages()
 
 
 setup(
     name='bytez',
-    version='0.1.90',
+    version='0.1.91',
     packages=packages,
     install_requires=[
         'charset-normalizer==3.1.0',
         'idna==3.4',
         'requests==2.28.2',
         'urllib3==1.26.15',
     ],
```

