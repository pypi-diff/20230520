# Comparing `tmp/agixt-1.1.49b0.tar.gz` & `tmp/agixt-1.1.50b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agixt-1.1.49b0.tar", last modified: Sat May 20 18:36:23 2023, max compression
+gzip compressed data, was "agixt-1.1.50b0.tar", last modified: Sat May 20 20:56:22 2023, max compression
```

## Comparing `agixt-1.1.49b0.tar` & `agixt-1.1.50b0.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:36:23.039126 agixt-1.1.49b0/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-20 18:36:12.000000 agixt-1.1.49b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-20 18:36:12.000000 agixt-1.1.49b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    18794 2023-05-20 18:36:23.039126 agixt-1.1.49b0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:36:23.035126 agixt-1.1.49b0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    18337 2023-05-20 18:36:12.000000 agixt-1.1.49b0/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-20 18:36:12.000000 agixt-1.1.49b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 18:36:23.039126 agixt-1.1.49b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-20 18:36:12.000000 agixt-1.1.49b0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:36:23.035126 agixt-1.1.49b0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:36:23.035126 agixt-1.1.49b0/src/agixt/
--rw-r--r--   0 runner    (1001) docker     (123)    25177 2023-05-20 18:36:12.000000 agixt-1.1.49b0/src/agixt/AGiXT.py
--rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-05-20 18:36:12.000000 agixt-1.1.49b0/src/agixt/Chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-05-20 18:36:12.000000 agixt-1.1.49b0/src/agixt/Commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:36:23.039126 agixt-1.1.49b0/src/agixt/Config/
--rw-r--r--   0 runner    (1001) docker     (123)    13461 2023-05-20 18:36:12.000000 agixt-1.1.49b0/src/agixt/Config/Agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-20 18:36:12.000000 agixt-1.1.49b0/src/agixt/Config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-20 18:36:12.000000 agixt-1.1.49b0/src/agixt/CustomPrompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-05-20 18:36:12.000000 agixt-1.1.49b0/src/agixt/Embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-05-20 18:36:12.000000 agixt-1.1.49b0/src/agixt/Memories.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-20 18:36:12.000000 agixt-1.1.49b0/src/agixt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13588 2023-05-20 18:36:12.000000 agixt-1.1.49b0/src/agixt/app.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-05-20 18:36:12.000000 agixt-1.1.49b0/src/agixt/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:36:23.039126 agixt-1.1.49b0/src/agixt/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-20 18:36:12.000000 agixt-1.1.49b0/src/agixt/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-20 18:36:12.000000 agixt-1.1.49b0/src/agixt/provider/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-20 18:36:12.000000 agixt-1.1.49b0/src/agixt/provider/bard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-20 18:36:12.000000 agixt-1.1.49b0/src/agixt/provider/bing.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-20 18:36:12.000000 agixt-1.1.49b0/src/agixt/provider/fastchat.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-20 18:36:12.000000 agixt-1.1.49b0/src/agixt/provider/gpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-05-20 18:36:12.000000 agixt-1.1.49b0/src/agixt/provider/gpt4free.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-20 18:36:12.000000 agixt-1.1.49b0/src/agixt/provider/gpugpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-20 18:36:12.000000 agixt-1.1.49b0/src/agixt/provider/huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-20 18:36:12.000000 agixt-1.1.49b0/src/agixt/provider/kobold.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-20 18:36:12.000000 agixt-1.1.49b0/src/agixt/provider/llamacpp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-20 18:36:12.000000 agixt-1.1.49b0/src/agixt/provider/oobabooga.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-20 18:36:12.000000 agixt-1.1.49b0/src/agixt/provider/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-20 18:36:12.000000 agixt-1.1.49b0/src/agixt/provider/palm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-20 18:36:12.000000 agixt-1.1.49b0/src/agixt/provider/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-20 18:36:12.000000 agixt-1.1.49b0/src/agixt/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-20 18:36:12.000000 agixt-1.1.49b0/src/agixt/smartchat.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-20 18:36:12.000000 agixt-1.1.49b0/src/agixt/smartinstruct.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-20 18:36:12.000000 agixt-1.1.49b0/src/agixt/streamlit.py
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-20 18:36:12.000000 agixt-1.1.49b0/src/agixt/version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:36:23.035126 agixt-1.1.49b0/src/agixt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18794 2023-05-20 18:36:23.000000 agixt-1.1.49b0/src/agixt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-20 18:36:23.000000 agixt-1.1.49b0/src/agixt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 18:36:23.000000 agixt-1.1.49b0/src/agixt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-20 18:36:23.000000 agixt-1.1.49b0/src/agixt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-20 18:36:23.000000 agixt-1.1.49b0/src/agixt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:56:22.801755 agixt-1.1.50b0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-20 20:56:05.000000 agixt-1.1.50b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-20 20:56:05.000000 agixt-1.1.50b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    18794 2023-05-20 20:56:22.801755 agixt-1.1.50b0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:56:22.793754 agixt-1.1.50b0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    18337 2023-05-20 20:56:05.000000 agixt-1.1.50b0/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-20 20:56:05.000000 agixt-1.1.50b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 20:56:22.801755 agixt-1.1.50b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-20 20:56:05.000000 agixt-1.1.50b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:56:22.793754 agixt-1.1.50b0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:56:22.797755 agixt-1.1.50b0/src/agixt/
+-rw-r--r--   0 runner    (1001) docker     (123)    25177 2023-05-20 20:56:05.000000 agixt-1.1.50b0/src/agixt/AGiXT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-05-20 20:56:05.000000 agixt-1.1.50b0/src/agixt/Chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-05-20 20:56:05.000000 agixt-1.1.50b0/src/agixt/Commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:56:22.797755 agixt-1.1.50b0/src/agixt/Config/
+-rw-r--r--   0 runner    (1001) docker     (123)    13461 2023-05-20 20:56:05.000000 agixt-1.1.50b0/src/agixt/Config/Agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-20 20:56:05.000000 agixt-1.1.50b0/src/agixt/Config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-20 20:56:05.000000 agixt-1.1.50b0/src/agixt/CustomPrompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-05-20 20:56:05.000000 agixt-1.1.50b0/src/agixt/Embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-05-20 20:56:05.000000 agixt-1.1.50b0/src/agixt/Memories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-20 20:56:05.000000 agixt-1.1.50b0/src/agixt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13588 2023-05-20 20:56:05.000000 agixt-1.1.50b0/src/agixt/app.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-05-20 20:56:05.000000 agixt-1.1.50b0/src/agixt/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:56:22.801755 agixt-1.1.50b0/src/agixt/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-20 20:56:05.000000 agixt-1.1.50b0/src/agixt/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-20 20:56:05.000000 agixt-1.1.50b0/src/agixt/provider/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-20 20:56:05.000000 agixt-1.1.50b0/src/agixt/provider/bard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-20 20:56:05.000000 agixt-1.1.50b0/src/agixt/provider/bing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-20 20:56:05.000000 agixt-1.1.50b0/src/agixt/provider/claude.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-20 20:56:05.000000 agixt-1.1.50b0/src/agixt/provider/fastchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-20 20:56:05.000000 agixt-1.1.50b0/src/agixt/provider/gpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-20 20:56:05.000000 agixt-1.1.50b0/src/agixt/provider/gpt4free.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-20 20:56:05.000000 agixt-1.1.50b0/src/agixt/provider/gpugpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-20 20:56:05.000000 agixt-1.1.50b0/src/agixt/provider/huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-20 20:56:05.000000 agixt-1.1.50b0/src/agixt/provider/kobold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-20 20:56:05.000000 agixt-1.1.50b0/src/agixt/provider/llamacpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-20 20:56:05.000000 agixt-1.1.50b0/src/agixt/provider/oobabooga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-20 20:56:05.000000 agixt-1.1.50b0/src/agixt/provider/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-20 20:56:05.000000 agixt-1.1.50b0/src/agixt/provider/palm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-20 20:56:05.000000 agixt-1.1.50b0/src/agixt/provider/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-20 20:56:05.000000 agixt-1.1.50b0/src/agixt/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-20 20:56:05.000000 agixt-1.1.50b0/src/agixt/smartchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-20 20:56:05.000000 agixt-1.1.50b0/src/agixt/smartinstruct.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-20 20:56:05.000000 agixt-1.1.50b0/src/agixt/streamlit.py
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-20 20:56:05.000000 agixt-1.1.50b0/src/agixt/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:56:22.797755 agixt-1.1.50b0/src/agixt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18794 2023-05-20 20:56:22.000000 agixt-1.1.50b0/src/agixt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-20 20:56:22.000000 agixt-1.1.50b0/src/agixt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 20:56:22.000000 agixt-1.1.50b0/src/agixt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-20 20:56:22.000000 agixt-1.1.50b0/src/agixt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-20 20:56:22.000000 agixt-1.1.50b0/src/agixt.egg-info/top_level.txt
```

### Comparing `agixt-1.1.49b0/LICENSE` & `agixt-1.1.50b0/LICENSE`

 * *Files identical despite different names*

### Comparing `agixt-1.1.49b0/PKG-INFO` & `agixt-1.1.50b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.1.49b0
+Version: 1.1.50b0
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `agixt-1.1.49b0/docs/README.md` & `agixt-1.1.50b0/docs/README.md`

 * *Files identical despite different names*

### Comparing `agixt-1.1.49b0/setup.py` & `agixt-1.1.50b0/setup.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.49b0/src/agixt/AGiXT.py` & `agixt-1.1.50b0/src/agixt/AGiXT.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.49b0/src/agixt/Chain.py` & `agixt-1.1.50b0/src/agixt/Chain.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.49b0/src/agixt/Commands.py` & `agixt-1.1.50b0/src/agixt/Commands.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.49b0/src/agixt/Config/Agent.py` & `agixt-1.1.50b0/src/agixt/Config/Agent.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.49b0/src/agixt/Config/__init__.py` & `agixt-1.1.50b0/src/agixt/Config/__init__.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.49b0/src/agixt/CustomPrompt.py` & `agixt-1.1.50b0/src/agixt/CustomPrompt.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.49b0/src/agixt/Embedding.py` & `agixt-1.1.50b0/src/agixt/Embedding.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.49b0/src/agixt/Memories.py` & `agixt-1.1.50b0/src/agixt/Memories.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.49b0/src/agixt/app.py` & `agixt-1.1.50b0/src/agixt/app.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.49b0/src/agixt/provider/__init__.py` & `agixt-1.1.50b0/src/agixt/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.49b0/src/agixt/provider/azure.py` & `agixt-1.1.50b0/src/agixt/provider/azure.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.49b0/src/agixt/provider/bing.py` & `agixt-1.1.50b0/src/agixt/provider/bing.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.49b0/src/agixt/provider/fastchat.py` & `agixt-1.1.50b0/src/agixt/provider/fastchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.49b0/src/agixt/provider/gpt4all.py` & `agixt-1.1.50b0/src/agixt/provider/gpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.49b0/src/agixt/provider/gpt4free.py` & `agixt-1.1.50b0/src/agixt/provider/gpt4free.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,22 +31,22 @@
                         if response:
                             if "text" in response:
                                 final_response = response["text"]
                             if "status" in response and response["status"] == "Fail":
                                 self.FAILED_PROVIDERS.append(provider)
                                 print(f"Failed to use {provider}")
                                 final_response = None
-                            elif (
+                            if (
                                 response
                                 == "Unable to fetch the response, Please try again."
                             ):
                                 self.FAILED_PROVIDERS.append(provider)
                                 print(f"Failed to use {provider}")
                                 final_response = None
-                            else:
+                            if final_response == None:
                                 final_response = response
                     if final_response:
                         if len(final_response) > 1:
                             return final_response
                 except:
                     print(f"Failed to use {provider}")
                     self.FAILED_PROVIDERS.append(provider)
```

### Comparing `agixt-1.1.49b0/src/agixt/provider/gpugpt4all.py` & `agixt-1.1.50b0/src/agixt/provider/gpugpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.49b0/src/agixt/provider/huggingchat.py` & `agixt-1.1.50b0/src/agixt/provider/huggingchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.49b0/src/agixt/provider/kobold.py` & `agixt-1.1.50b0/src/agixt/provider/kobold.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.49b0/src/agixt/provider/llamacpp.py` & `agixt-1.1.50b0/src/agixt/provider/llamacpp.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.49b0/src/agixt/provider/oobabooga.py` & `agixt-1.1.50b0/src/agixt/provider/oobabooga.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.49b0/src/agixt/provider/openai.py` & `agixt-1.1.50b0/src/agixt/provider/openai.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.49b0/src/agixt/provider/palm.py` & `agixt-1.1.50b0/src/agixt/provider/palm.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.49b0/src/agixt/provider/transformer.py` & `agixt-1.1.50b0/src/agixt/provider/transformer.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.49b0/src/agixt/requirements.txt` & `agixt-1.1.50b0/src/agixt/requirements.txt`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 git+https://github.com/huggingface/transformers
 sentence-transformers
 llama-cpp-python==0.1.48
 accelerate
 nomic
 ####
 argparse
+anthropic
 beautifulsoup4
 captcha-solver
 docker
 duckduckgo_search==2.9.5
 fastapi
 uvicorn
 gitpython
```

### Comparing `agixt-1.1.49b0/src/agixt/smartchat.py` & `agixt-1.1.50b0/src/agixt/smartchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.49b0/src/agixt/smartinstruct.py` & `agixt-1.1.50b0/src/agixt/smartinstruct.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.49b0/src/agixt.egg-info/PKG-INFO` & `agixt-1.1.50b0/src/agixt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.1.49b0
+Version: 1.1.50b0
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `agixt-1.1.49b0/src/agixt.egg-info/SOURCES.txt` & `agixt-1.1.50b0/src/agixt.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 src/agixt.egg-info/top_level.txt
 src/agixt/Config/Agent.py
 src/agixt/Config/__init__.py
 src/agixt/provider/__init__.py
 src/agixt/provider/azure.py
 src/agixt/provider/bard.py
 src/agixt/provider/bing.py
+src/agixt/provider/claude.py
 src/agixt/provider/fastchat.py
 src/agixt/provider/gpt4all.py
 src/agixt/provider/gpt4free.py
 src/agixt/provider/gpugpt4all.py
 src/agixt/provider/huggingchat.py
 src/agixt/provider/kobold.py
 src/agixt/provider/llamacpp.py
```

### Comparing `agixt-1.1.49b0/src/agixt.egg-info/requires.txt` & `agixt-1.1.50b0/src/agixt.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 chromadb
 sentence-transformers
 llama-cpp-python==0.1.48
 accelerate
 nomic
 argparse
+anthropic
 beautifulsoup4
 captcha-solver
 docker
 duckduckgo_search==2.9.5
 fastapi
 uvicorn
 gitpython
```

