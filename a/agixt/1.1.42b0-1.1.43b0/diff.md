# Comparing `tmp/agixt-1.1.42b0.tar.gz` & `tmp/agixt-1.1.43b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agixt-1.1.42b0.tar", last modified: Fri May 19 22:09:51 2023, max compression
+gzip compressed data, was "agixt-1.1.43b0.tar", last modified: Fri May 19 22:19:22 2023, max compression
```

## Comparing `agixt-1.1.42b0.tar` & `agixt-1.1.43b0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:51.060380 agixt-1.1.42b0/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-19 22:09:40.000000 agixt-1.1.42b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-19 22:09:40.000000 agixt-1.1.42b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    19243 2023-05-19 22:09:51.060380 agixt-1.1.42b0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:51.056380 agixt-1.1.42b0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    18786 2023-05-19 22:09:40.000000 agixt-1.1.42b0/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-19 22:09:40.000000 agixt-1.1.42b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 22:09:51.060380 agixt-1.1.42b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-19 22:09:40.000000 agixt-1.1.42b0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:51.056380 agixt-1.1.42b0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:51.060380 agixt-1.1.42b0/src/agixt/
--rw-r--r--   0 runner    (1001) docker     (123)    27224 2023-05-19 22:09:40.000000 agixt-1.1.42b0/src/agixt/AGiXT.py
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-05-19 22:09:40.000000 agixt-1.1.42b0/src/agixt/Chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-05-19 22:09:40.000000 agixt-1.1.42b0/src/agixt/Commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:51.060380 agixt-1.1.42b0/src/agixt/Config/
--rw-r--r--   0 runner    (1001) docker     (123)    13354 2023-05-19 22:09:40.000000 agixt-1.1.42b0/src/agixt/Config/Agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-19 22:09:40.000000 agixt-1.1.42b0/src/agixt/Config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-19 22:09:40.000000 agixt-1.1.42b0/src/agixt/CustomPrompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-05-19 22:09:40.000000 agixt-1.1.42b0/src/agixt/Embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-05-19 22:09:40.000000 agixt-1.1.42b0/src/agixt/Memories.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-19 22:09:40.000000 agixt-1.1.42b0/src/agixt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13588 2023-05-19 22:09:40.000000 agixt-1.1.42b0/src/agixt/app.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-05-19 22:09:40.000000 agixt-1.1.42b0/src/agixt/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:51.060380 agixt-1.1.42b0/src/agixt/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-19 22:09:40.000000 agixt-1.1.42b0/src/agixt/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-19 22:09:40.000000 agixt-1.1.42b0/src/agixt/provider/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-19 22:09:40.000000 agixt-1.1.42b0/src/agixt/provider/bard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-19 22:09:40.000000 agixt-1.1.42b0/src/agixt/provider/bing.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-19 22:09:40.000000 agixt-1.1.42b0/src/agixt/provider/fastchat.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-19 22:09:40.000000 agixt-1.1.42b0/src/agixt/provider/gpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-19 22:09:40.000000 agixt-1.1.42b0/src/agixt/provider/gpt4free.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-19 22:09:40.000000 agixt-1.1.42b0/src/agixt/provider/gpugpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-19 22:09:40.000000 agixt-1.1.42b0/src/agixt/provider/huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-19 22:09:40.000000 agixt-1.1.42b0/src/agixt/provider/kobold.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-19 22:09:40.000000 agixt-1.1.42b0/src/agixt/provider/llamacpp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-19 22:09:40.000000 agixt-1.1.42b0/src/agixt/provider/oobabooga.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-19 22:09:40.000000 agixt-1.1.42b0/src/agixt/provider/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-19 22:09:40.000000 agixt-1.1.42b0/src/agixt/provider/palm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-19 22:09:40.000000 agixt-1.1.42b0/src/agixt/provider/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-19 22:09:40.000000 agixt-1.1.42b0/src/agixt/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-19 22:09:40.000000 agixt-1.1.42b0/src/agixt/smartchat.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-19 22:09:40.000000 agixt-1.1.42b0/src/agixt/smartinstruct.py
--rw-r--r--   0 runner    (1001) docker     (123)    33055 2023-05-19 22:09:40.000000 agixt-1.1.42b0/src/agixt/streamlit.py
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-19 22:09:40.000000 agixt-1.1.42b0/src/agixt/version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:09:51.060380 agixt-1.1.42b0/src/agixt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19243 2023-05-19 22:09:51.000000 agixt-1.1.42b0/src/agixt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-19 22:09:51.000000 agixt-1.1.42b0/src/agixt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 22:09:51.000000 agixt-1.1.42b0/src/agixt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-19 22:09:51.000000 agixt-1.1.42b0/src/agixt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-19 22:09:51.000000 agixt-1.1.42b0/src/agixt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:19:22.365368 agixt-1.1.43b0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-19 22:19:11.000000 agixt-1.1.43b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-19 22:19:11.000000 agixt-1.1.43b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    19243 2023-05-19 22:19:22.365368 agixt-1.1.43b0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:19:22.357368 agixt-1.1.43b0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    18786 2023-05-19 22:19:11.000000 agixt-1.1.43b0/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-19 22:19:11.000000 agixt-1.1.43b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 22:19:22.365368 agixt-1.1.43b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-19 22:19:11.000000 agixt-1.1.43b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:19:22.357368 agixt-1.1.43b0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:19:22.361368 agixt-1.1.43b0/src/agixt/
+-rw-r--r--   0 runner    (1001) docker     (123)    27224 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/AGiXT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/Chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/Commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:19:22.361368 agixt-1.1.43b0/src/agixt/Config/
+-rw-r--r--   0 runner    (1001) docker     (123)    13354 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/Config/Agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/Config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/CustomPrompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/Embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/Memories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13588 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/app.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:19:22.365368 agixt-1.1.43b0/src/agixt/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/provider/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/provider/bard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/provider/bing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/provider/fastchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/provider/gpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/provider/gpt4free.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/provider/gpugpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/provider/huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/provider/kobold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/provider/llamacpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/provider/oobabooga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/provider/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/provider/palm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/provider/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/smartchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/smartinstruct.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33055 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/streamlit.py
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:19:22.361368 agixt-1.1.43b0/src/agixt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19243 2023-05-19 22:19:22.000000 agixt-1.1.43b0/src/agixt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-19 22:19:22.000000 agixt-1.1.43b0/src/agixt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 22:19:22.000000 agixt-1.1.43b0/src/agixt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-19 22:19:22.000000 agixt-1.1.43b0/src/agixt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-19 22:19:22.000000 agixt-1.1.43b0/src/agixt.egg-info/top_level.txt
```

### Comparing `agixt-1.1.42b0/LICENSE` & `agixt-1.1.43b0/LICENSE`

 * *Files identical despite different names*

### Comparing `agixt-1.1.42b0/PKG-INFO` & `agixt-1.1.43b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.1.42b0
+Version: 1.1.43b0
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `agixt-1.1.42b0/docs/README.md` & `agixt-1.1.43b0/docs/README.md`

 * *Files identical despite different names*

### Comparing `agixt-1.1.42b0/setup.py` & `agixt-1.1.43b0/setup.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.42b0/src/agixt/AGiXT.py` & `agixt-1.1.43b0/src/agixt/AGiXT.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.42b0/src/agixt/Chain.py` & `agixt-1.1.43b0/src/agixt/Chain.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.42b0/src/agixt/Commands.py` & `agixt-1.1.43b0/src/agixt/Commands.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.42b0/src/agixt/Config/Agent.py` & `agixt-1.1.43b0/src/agixt/Config/Agent.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.42b0/src/agixt/Config/__init__.py` & `agixt-1.1.43b0/src/agixt/Config/__init__.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.42b0/src/agixt/CustomPrompt.py` & `agixt-1.1.43b0/src/agixt/CustomPrompt.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.42b0/src/agixt/Embedding.py` & `agixt-1.1.43b0/src/agixt/Embedding.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.42b0/src/agixt/Memories.py` & `agixt-1.1.43b0/src/agixt/Memories.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.42b0/src/agixt/app.py` & `agixt-1.1.43b0/src/agixt/app.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.42b0/src/agixt/provider/__init__.py` & `agixt-1.1.43b0/src/agixt/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.42b0/src/agixt/provider/azure.py` & `agixt-1.1.43b0/src/agixt/provider/azure.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.42b0/src/agixt/provider/bing.py` & `agixt-1.1.43b0/src/agixt/provider/bing.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.42b0/src/agixt/provider/fastchat.py` & `agixt-1.1.43b0/src/agixt/provider/fastchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.42b0/src/agixt/provider/gpt4all.py` & `agixt-1.1.43b0/src/agixt/provider/gpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.42b0/src/agixt/provider/gpt4free.py` & `agixt-1.1.43b0/src/agixt/provider/gpt4free.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.42b0/src/agixt/provider/gpugpt4all.py` & `agixt-1.1.43b0/src/agixt/provider/gpugpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.42b0/src/agixt/provider/huggingchat.py` & `agixt-1.1.43b0/src/agixt/provider/huggingchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.42b0/src/agixt/provider/kobold.py` & `agixt-1.1.43b0/src/agixt/provider/kobold.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.42b0/src/agixt/provider/llamacpp.py` & `agixt-1.1.43b0/src/agixt/provider/llamacpp.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.42b0/src/agixt/provider/oobabooga.py` & `agixt-1.1.43b0/src/agixt/provider/oobabooga.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.42b0/src/agixt/provider/openai.py` & `agixt-1.1.43b0/src/agixt/provider/openai.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.42b0/src/agixt/provider/palm.py` & `agixt-1.1.43b0/src/agixt/provider/palm.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.42b0/src/agixt/provider/transformer.py` & `agixt-1.1.43b0/src/agixt/provider/transformer.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.42b0/src/agixt/requirements.txt` & `agixt-1.1.43b0/src/agixt/requirements.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.42b0/src/agixt/smartchat.py` & `agixt-1.1.43b0/src/agixt/smartchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.42b0/src/agixt/smartinstruct.py` & `agixt-1.1.43b0/src/agixt/smartinstruct.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.42b0/src/agixt/streamlit.py` & `agixt-1.1.43b0/src/agixt/streamlit.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.42b0/src/agixt.egg-info/PKG-INFO` & `agixt-1.1.43b0/src/agixt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.1.42b0
+Version: 1.1.43b0
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `agixt-1.1.42b0/src/agixt.egg-info/SOURCES.txt` & `agixt-1.1.43b0/src/agixt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.42b0/src/agixt.egg-info/requires.txt` & `agixt-1.1.43b0/src/agixt.egg-info/requires.txt`

 * *Files identical despite different names*

