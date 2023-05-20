# Comparing `tmp/agixt-1.1.43b0.tar.gz` & `tmp/agixt-1.1.44b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agixt-1.1.43b0.tar", last modified: Fri May 19 22:19:22 2023, max compression
+gzip compressed data, was "agixt-1.1.44b0.tar", last modified: Sat May 20 02:53:46 2023, max compression
```

## Comparing `agixt-1.1.43b0.tar` & `agixt-1.1.44b0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:19:22.365368 agixt-1.1.43b0/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-19 22:19:11.000000 agixt-1.1.43b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-19 22:19:11.000000 agixt-1.1.43b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    19243 2023-05-19 22:19:22.365368 agixt-1.1.43b0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:19:22.357368 agixt-1.1.43b0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    18786 2023-05-19 22:19:11.000000 agixt-1.1.43b0/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-19 22:19:11.000000 agixt-1.1.43b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 22:19:22.365368 agixt-1.1.43b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-19 22:19:11.000000 agixt-1.1.43b0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:19:22.357368 agixt-1.1.43b0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:19:22.361368 agixt-1.1.43b0/src/agixt/
--rw-r--r--   0 runner    (1001) docker     (123)    27224 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/AGiXT.py
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/Chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/Commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:19:22.361368 agixt-1.1.43b0/src/agixt/Config/
--rw-r--r--   0 runner    (1001) docker     (123)    13354 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/Config/Agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/Config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/CustomPrompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/Embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/Memories.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13588 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/app.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:19:22.365368 agixt-1.1.43b0/src/agixt/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/provider/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/provider/bard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/provider/bing.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/provider/fastchat.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/provider/gpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/provider/gpt4free.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/provider/gpugpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/provider/huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/provider/kobold.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/provider/llamacpp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/provider/oobabooga.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/provider/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/provider/palm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/provider/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/smartchat.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/smartinstruct.py
--rw-r--r--   0 runner    (1001) docker     (123)    33055 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/streamlit.py
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-19 22:19:11.000000 agixt-1.1.43b0/src/agixt/version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:19:22.361368 agixt-1.1.43b0/src/agixt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19243 2023-05-19 22:19:22.000000 agixt-1.1.43b0/src/agixt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-19 22:19:22.000000 agixt-1.1.43b0/src/agixt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 22:19:22.000000 agixt-1.1.43b0/src/agixt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-19 22:19:22.000000 agixt-1.1.43b0/src/agixt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-19 22:19:22.000000 agixt-1.1.43b0/src/agixt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 02:53:46.896667 agixt-1.1.44b0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-20 02:53:32.000000 agixt-1.1.44b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-20 02:53:32.000000 agixt-1.1.44b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    19140 2023-05-20 02:53:46.896667 agixt-1.1.44b0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 02:53:46.892667 agixt-1.1.44b0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    18683 2023-05-20 02:53:32.000000 agixt-1.1.44b0/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-20 02:53:32.000000 agixt-1.1.44b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 02:53:46.896667 agixt-1.1.44b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-20 02:53:32.000000 agixt-1.1.44b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 02:53:46.892667 agixt-1.1.44b0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 02:53:46.892667 agixt-1.1.44b0/src/agixt/
+-rw-r--r--   0 runner    (1001) docker     (123)    25128 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/AGiXT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/Chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/Commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 02:53:46.896667 agixt-1.1.44b0/src/agixt/Config/
+-rw-r--r--   0 runner    (1001) docker     (123)    13352 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/Config/Agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/Config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/CustomPrompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/Embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/Memories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13588 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/app.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 02:53:46.896667 agixt-1.1.44b0/src/agixt/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/provider/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/provider/bard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/provider/bing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/provider/fastchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/provider/gpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/provider/gpt4free.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/provider/gpugpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/provider/huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/provider/kobold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/provider/llamacpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/provider/oobabooga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/provider/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/provider/palm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/provider/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/smartchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/smartinstruct.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33053 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/streamlit.py
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 02:53:46.896667 agixt-1.1.44b0/src/agixt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19140 2023-05-20 02:53:46.000000 agixt-1.1.44b0/src/agixt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-20 02:53:46.000000 agixt-1.1.44b0/src/agixt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 02:53:46.000000 agixt-1.1.44b0/src/agixt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-20 02:53:46.000000 agixt-1.1.44b0/src/agixt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-20 02:53:46.000000 agixt-1.1.44b0/src/agixt.egg-info/top_level.txt
```

### Comparing `agixt-1.1.43b0/LICENSE` & `agixt-1.1.44b0/LICENSE`

 * *Files identical despite different names*

### Comparing `agixt-1.1.43b0/PKG-INFO` & `agixt-1.1.44b0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.1.43b0
+Version: 1.1.44b0
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # AGiXT
 
 ![RELEASE](https://img.shields.io/github/v/release/Josh-XT/AGiXT?label=Release%20Version&style=plastic) 
 [![STATUS](https://img.shields.io/badge/status-beta-blue?label=Release%20Status&style=plastic)](https://github.com/josh-xt/AGiXT) 
 [![LICENSE: MIT](https://img.shields.io/github/license/Josh-XT/AGiXT?label=License&style=plastic)](https://github.com/Josh-XT/AGiXT/blob/main/LICENSE) 
 ![DOCKER](https://img.shields.io/github/actions/workflow/status/Josh-XT/AGiXT/publish-docker.yml?branch=main&label=Docker&style=plastic) [![CODESTYLE](https://img.shields.io/badge/code%20style-Black-black?branch=main&label=Code%20Style&style=plastic)](https://black.readthedocs.io/en/stable/the_black_code_style/index.html)
 
-[![GitHub](https://img.shields.io/badge/GitHub-Frontend_Repository-grey?logo=github&style=plastic)](https://github.com/JamesonRGrieve/AGiXT-Frontend)
+[![GitHub](https://img.shields.io/badge/GitHub-Frontend_Repository-grey?logo=github&style=plastic)](https://github.com/JamesonRGrieve/Agent-LLM-Frontend)
 
 [![Contribute](https://img.shields.io/github/issues/Josh-XT/AGiXT/help%20wanted?color=purple&label=Quick%20Contribute%20Backend&logo=github&style=plastic)](https://github.com/Josh-XT/AGiXT/labels/help%20wanted) 
-[![Contribute](https://img.shields.io/github/issues/JamesonRGrieve/AGiXT-Frontend/help%20wanted?color=purple&label=Quick%20Contribute%20Frontend&logo=github&style=plastic)](https://github.com/JamesonRGrieve/AGiXT-Frontend/labels/help%20wanted) 
+[![Contribute](https://img.shields.io/github/issues/JamesonRGrieve/Agent-LLM-Frontend/help%20wanted?color=purple&label=Quick%20Contribute%20Frontend&logo=github&style=plastic)](https://github.com/JamesonRGrieve/Agent-LLM-Frontend/labels/help%20wanted) 
 [![Discord](https://img.shields.io/discord/1097720481970397356?label=Discord&logo=discord&logoColor=white&style=plastic&color=5865f2)](https://discord.gg/d3TkHRZcjD) 
-[![Twitter](https://img.shields.io/badge/Twitter-Follow_@AGiXT-blue?logo=twitter&style=plastic)](https://twitter.com/AGiXT) 
-[![FacebookGroup](https://img.shields.io/badge/Facebook-Join_Our_Group-blue?logo=facebook&style=plastic)](https://www.facebook.com/groups/AGiXT)
-[![EMail](https://img.shields.io/badge/E--Mail-Outreach_&_Media-5865f2?logo=gmail&style=plastic)](https://twitter.com/AGiXT) 
+[![Twitter](https://img.shields.io/badge/Twitter-Follow_@AGi_XT-blue?logo=twitter&style=plastic)](https://twitter.com/AGi_XT) 
+[![EMail](https://img.shields.io/badge/E--Mail-Outreach_&_Media-5865f2?logo=gmail&style=plastic)](https://twitter.com/AGi_XT) 
 
 Please use the outreach email for media, sponsorship, or to contact us for other miscellaneous purposes. 
 
 **Do not** send us emails with troubleshooting requests, feature requests or bug reports, please direct those to [GitHub Issues](https://github.com/Josh-XT/AGiXT/issues) or [Discord](https://discord.gg/d3TkHRZcjD).
 
 AGiXT is an Artificial Intelligence Automation Platform designed to power efficient AI instruction management across multiple providers. Our agents are equipped with adaptive memory, and this versatile solution offers a powerful plugin system that supports a wide range of commands, including web browsing. With growing support for numerous AI providers and models, AGiXT is constantly evolving to empower diverse applications.
 
@@ -186,26 +185,26 @@
 
 ### Back End
 
 Clone the repository for the AGiXT back end and start it.
 
 ```
 git clone https://github.com/Josh-XT/AGiXT
-cd AGiXT
+cd AGiXT/src/agixt
 pip install -r requirements.txt
 python app.py
 ```
 
 ### Front End
 
 Clone the repository for the AGiXT front end in a separate terminal and start it.
 
 ```
-git clone https://github.com/JamesonRGrieve/AGiXT-Frontend --recurse-submodules 
-cd AGiXT-Frontend
+git clone https://github.com/JamesonRGrieve/Agent-LLM-Frontend --recurse-submodules 
+cd Agent-LLM-Frontend
 yarn install
 yarn dev
 ```
 
 Access the web interface at http://localhost:3000
 
 ## Configuration
@@ -253,18 +252,18 @@
 
 In `docs/` folder. Can be used to generate static html output. See `deploy-docs` section in [Publish Workflow](/.github/workflows/python-publish.yml) howto build with honkit.
 
 ## Contributing
 
 [![Contribute](https://img.shields.io/github/issues/Josh-XT/AGiXT/help%20wanted?color=purple&label=Quick%20Contribute&logo=github&style=plastic)](https://github.com/Josh-XT/AGiXT/labels/help%20wanted) 
 
-We welcome contributions to AGiXT! If you're interested in contributing, please check out our [contributions guide](https://github.com/Josh-XT/AGiXT/tree/main/.github/CONTRIBUTING.md) the [open issues on the backend](https://github.com/Josh-XT/AGiXT/issues), [open issues on the frontend](https://github.com/JamesonRGrieve/AGiXT-Frontend/issues) and [pull requests](https://github.com/Josh-XT/AGiXT/pulls), submit a [pull request](https://github.com/Josh-XT/AGiXT/pulls/new), or [suggest new features](https://github.com/Josh-XT/AGiXT/issues/new). To stay updated on the project's progress, [![Twitter](https://img.shields.io/badge/Twitter-Follow_@AGiXT-blue?logo=twitter&style=plastic)](https://twitter.com/AGiXT), [![Twitter](https://img.shields.io/badge/Twitter-Follow_@Josh_XT-blue?logo=twitter&style=plastic)](https://twitter.com/Josh_XT) and [![Twitter](https://img.shields.io/badge/Twitter-Follow_@JamesonRGrieve-blue?logo=twitter&style=plastic)](https://twitter.com/JamesonRGrieve). Also feel free to join our [![Discord](https://img.shields.io/discord/1097720481970397356?label=Discord&logo=discord&logoColor=white&style=plastic&color=5865f2)](https://discord.gg/d3TkHRZcjD).
+We welcome contributions to AGiXT! If you're interested in contributing, please check out our [contributions guide](https://github.com/Josh-XT/AGiXT/tree/main/.github/CONTRIBUTING.md) the [open issues on the backend](https://github.com/Josh-XT/AGiXT/issues), [open issues on the frontend](https://github.com/JamesonRGrieve/Agent-LLM-Frontend/issues) and [pull requests](https://github.com/Josh-XT/AGiXT/pulls), submit a [pull request](https://github.com/Josh-XT/AGiXT/pulls/new), or [suggest new features](https://github.com/Josh-XT/AGiXT/issues/new). To stay updated on the project's progress, [![Twitter](https://img.shields.io/badge/Twitter-Follow_@AGi_XT-blue?logo=twitter&style=plastic)](https://twitter.com/AGi_XT), [![Twitter](https://img.shields.io/badge/Twitter-Follow_@Josh_XT-blue?logo=twitter&style=plastic)](https://twitter.com/Josh_XT) and [![Twitter](https://img.shields.io/badge/Twitter-Follow_@JamesonRGrieve-blue?logo=twitter&style=plastic)](https://twitter.com/JamesonRGrieve). Also feel free to join our [![Discord](https://img.shields.io/discord/1097720481970397356?label=Discord&logo=discord&logoColor=white&style=plastic&color=5865f2)](https://discord.gg/d3TkHRZcjD).
 
 ## Donations and Sponsorships
-We appreciate any support for AGiXT's development, including donations, sponsorships, and any other kind of assistance. If you would like to support us, please contact us through our [![EMail](https://img.shields.io/badge/E--Mail-Outreach_&_Media-5865f2?logo=gmail&style=plastic)](https://twitter.com/AGiXT) , [![Discord](https://img.shields.io/discord/1097720481970397356?label=Discord&logo=discord&logoColor=white&style=plastic&color=5865f2)](https://discord.gg/d3TkHRZcjD) or [![Twitter](https://img.shields.io/badge/Twitter-Follow_@AGiXT-blue?logo=twitter&style=plastic)](https://twitter.com/AGiXT).
+We appreciate any support for AGiXT's development, including donations, sponsorships, and any other kind of assistance. If you would like to support us, please contact us through our [![EMail](https://img.shields.io/badge/E--Mail-Outreach_&_Media-5865f2?logo=gmail&style=plastic)](https://twitter.com/AGi_XT) , [![Discord](https://img.shields.io/discord/1097720481970397356?label=Discord&logo=discord&logoColor=white&style=plastic&color=5865f2)](https://discord.gg/d3TkHRZcjD) or [![Twitter](https://img.shields.io/badge/Twitter-Follow_@AGi_XT-blue?logo=twitter&style=plastic)](https://twitter.com/AGi_XT).
 
 We're always looking for ways to improve AGiXT and make it more useful for our users. Your support will help us continue to develop and enhance the application. Thank you for considering to support us!
 
 ## Our Team 🧑‍💻
 | Josh (@Josh-XT)                    | James (@JamesonRGrieve) | 
 |-----------------------------------|-----------------------------------|
 |[![GitHub](https://img.shields.io/badge/GitHub-Follow_@Josh--XT-white?logo=github&style=plastic)](https://github.com/Josh-XT)|[![GitHub](https://img.shields.io/badge/GitHub-Follow_@JamesonRGrieve-white?logo=github&style=plastic)](https://github.com/JamesonRGrieve)|
```

### Comparing `agixt-1.1.43b0/docs/README.md` & `agixt-1.1.44b0/src/agixt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,31 @@
+Metadata-Version: 2.1
+Name: agixt
+Version: 1.1.44b0
+Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
+Author: Josh XT
+Author-email: josh@devxt.com
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # AGiXT
 
 ![RELEASE](https://img.shields.io/github/v/release/Josh-XT/AGiXT?label=Release%20Version&style=plastic) 
 [![STATUS](https://img.shields.io/badge/status-beta-blue?label=Release%20Status&style=plastic)](https://github.com/josh-xt/AGiXT) 
 [![LICENSE: MIT](https://img.shields.io/github/license/Josh-XT/AGiXT?label=License&style=plastic)](https://github.com/Josh-XT/AGiXT/blob/main/LICENSE) 
 ![DOCKER](https://img.shields.io/github/actions/workflow/status/Josh-XT/AGiXT/publish-docker.yml?branch=main&label=Docker&style=plastic) [![CODESTYLE](https://img.shields.io/badge/code%20style-Black-black?branch=main&label=Code%20Style&style=plastic)](https://black.readthedocs.io/en/stable/the_black_code_style/index.html)
 
-[![GitHub](https://img.shields.io/badge/GitHub-Frontend_Repository-grey?logo=github&style=plastic)](https://github.com/JamesonRGrieve/AGiXT-Frontend)
+[![GitHub](https://img.shields.io/badge/GitHub-Frontend_Repository-grey?logo=github&style=plastic)](https://github.com/JamesonRGrieve/Agent-LLM-Frontend)
 
 [![Contribute](https://img.shields.io/github/issues/Josh-XT/AGiXT/help%20wanted?color=purple&label=Quick%20Contribute%20Backend&logo=github&style=plastic)](https://github.com/Josh-XT/AGiXT/labels/help%20wanted) 
-[![Contribute](https://img.shields.io/github/issues/JamesonRGrieve/AGiXT-Frontend/help%20wanted?color=purple&label=Quick%20Contribute%20Frontend&logo=github&style=plastic)](https://github.com/JamesonRGrieve/AGiXT-Frontend/labels/help%20wanted) 
+[![Contribute](https://img.shields.io/github/issues/JamesonRGrieve/Agent-LLM-Frontend/help%20wanted?color=purple&label=Quick%20Contribute%20Frontend&logo=github&style=plastic)](https://github.com/JamesonRGrieve/Agent-LLM-Frontend/labels/help%20wanted) 
 [![Discord](https://img.shields.io/discord/1097720481970397356?label=Discord&logo=discord&logoColor=white&style=plastic&color=5865f2)](https://discord.gg/d3TkHRZcjD) 
-[![Twitter](https://img.shields.io/badge/Twitter-Follow_@AGiXT-blue?logo=twitter&style=plastic)](https://twitter.com/AGiXT) 
-[![FacebookGroup](https://img.shields.io/badge/Facebook-Join_Our_Group-blue?logo=facebook&style=plastic)](https://www.facebook.com/groups/AGiXT)
-[![EMail](https://img.shields.io/badge/E--Mail-Outreach_&_Media-5865f2?logo=gmail&style=plastic)](https://twitter.com/AGiXT) 
+[![Twitter](https://img.shields.io/badge/Twitter-Follow_@AGi_XT-blue?logo=twitter&style=plastic)](https://twitter.com/AGi_XT) 
+[![EMail](https://img.shields.io/badge/E--Mail-Outreach_&_Media-5865f2?logo=gmail&style=plastic)](https://twitter.com/AGi_XT) 
 
 Please use the outreach email for media, sponsorship, or to contact us for other miscellaneous purposes. 
 
 **Do not** send us emails with troubleshooting requests, feature requests or bug reports, please direct those to [GitHub Issues](https://github.com/Josh-XT/AGiXT/issues) or [Discord](https://discord.gg/d3TkHRZcjD).
 
 AGiXT is an Artificial Intelligence Automation Platform designed to power efficient AI instruction management across multiple providers. Our agents are equipped with adaptive memory, and this versatile solution offers a powerful plugin system that supports a wide range of commands, including web browsing. With growing support for numerous AI providers and models, AGiXT is constantly evolving to empower diverse applications.
 
@@ -176,26 +185,26 @@
 
 ### Back End
 
 Clone the repository for the AGiXT back end and start it.
 
 ```
 git clone https://github.com/Josh-XT/AGiXT
-cd AGiXT
+cd AGiXT/src/agixt
 pip install -r requirements.txt
 python app.py
 ```
 
 ### Front End
 
 Clone the repository for the AGiXT front end in a separate terminal and start it.
 
 ```
-git clone https://github.com/JamesonRGrieve/AGiXT-Frontend --recurse-submodules 
-cd AGiXT-Frontend
+git clone https://github.com/JamesonRGrieve/Agent-LLM-Frontend --recurse-submodules 
+cd Agent-LLM-Frontend
 yarn install
 yarn dev
 ```
 
 Access the web interface at http://localhost:3000
 
 ## Configuration
@@ -243,18 +252,18 @@
 
 In `docs/` folder. Can be used to generate static html output. See `deploy-docs` section in [Publish Workflow](/.github/workflows/python-publish.yml) howto build with honkit.
 
 ## Contributing
 
 [![Contribute](https://img.shields.io/github/issues/Josh-XT/AGiXT/help%20wanted?color=purple&label=Quick%20Contribute&logo=github&style=plastic)](https://github.com/Josh-XT/AGiXT/labels/help%20wanted) 
 
-We welcome contributions to AGiXT! If you're interested in contributing, please check out our [contributions guide](https://github.com/Josh-XT/AGiXT/tree/main/.github/CONTRIBUTING.md) the [open issues on the backend](https://github.com/Josh-XT/AGiXT/issues), [open issues on the frontend](https://github.com/JamesonRGrieve/AGiXT-Frontend/issues) and [pull requests](https://github.com/Josh-XT/AGiXT/pulls), submit a [pull request](https://github.com/Josh-XT/AGiXT/pulls/new), or [suggest new features](https://github.com/Josh-XT/AGiXT/issues/new). To stay updated on the project's progress, [![Twitter](https://img.shields.io/badge/Twitter-Follow_@AGiXT-blue?logo=twitter&style=plastic)](https://twitter.com/AGiXT), [![Twitter](https://img.shields.io/badge/Twitter-Follow_@Josh_XT-blue?logo=twitter&style=plastic)](https://twitter.com/Josh_XT) and [![Twitter](https://img.shields.io/badge/Twitter-Follow_@JamesonRGrieve-blue?logo=twitter&style=plastic)](https://twitter.com/JamesonRGrieve). Also feel free to join our [![Discord](https://img.shields.io/discord/1097720481970397356?label=Discord&logo=discord&logoColor=white&style=plastic&color=5865f2)](https://discord.gg/d3TkHRZcjD).
+We welcome contributions to AGiXT! If you're interested in contributing, please check out our [contributions guide](https://github.com/Josh-XT/AGiXT/tree/main/.github/CONTRIBUTING.md) the [open issues on the backend](https://github.com/Josh-XT/AGiXT/issues), [open issues on the frontend](https://github.com/JamesonRGrieve/Agent-LLM-Frontend/issues) and [pull requests](https://github.com/Josh-XT/AGiXT/pulls), submit a [pull request](https://github.com/Josh-XT/AGiXT/pulls/new), or [suggest new features](https://github.com/Josh-XT/AGiXT/issues/new). To stay updated on the project's progress, [![Twitter](https://img.shields.io/badge/Twitter-Follow_@AGi_XT-blue?logo=twitter&style=plastic)](https://twitter.com/AGi_XT), [![Twitter](https://img.shields.io/badge/Twitter-Follow_@Josh_XT-blue?logo=twitter&style=plastic)](https://twitter.com/Josh_XT) and [![Twitter](https://img.shields.io/badge/Twitter-Follow_@JamesonRGrieve-blue?logo=twitter&style=plastic)](https://twitter.com/JamesonRGrieve). Also feel free to join our [![Discord](https://img.shields.io/discord/1097720481970397356?label=Discord&logo=discord&logoColor=white&style=plastic&color=5865f2)](https://discord.gg/d3TkHRZcjD).
 
 ## Donations and Sponsorships
-We appreciate any support for AGiXT's development, including donations, sponsorships, and any other kind of assistance. If you would like to support us, please contact us through our [![EMail](https://img.shields.io/badge/E--Mail-Outreach_&_Media-5865f2?logo=gmail&style=plastic)](https://twitter.com/AGiXT) , [![Discord](https://img.shields.io/discord/1097720481970397356?label=Discord&logo=discord&logoColor=white&style=plastic&color=5865f2)](https://discord.gg/d3TkHRZcjD) or [![Twitter](https://img.shields.io/badge/Twitter-Follow_@AGiXT-blue?logo=twitter&style=plastic)](https://twitter.com/AGiXT).
+We appreciate any support for AGiXT's development, including donations, sponsorships, and any other kind of assistance. If you would like to support us, please contact us through our [![EMail](https://img.shields.io/badge/E--Mail-Outreach_&_Media-5865f2?logo=gmail&style=plastic)](https://twitter.com/AGi_XT) , [![Discord](https://img.shields.io/discord/1097720481970397356?label=Discord&logo=discord&logoColor=white&style=plastic&color=5865f2)](https://discord.gg/d3TkHRZcjD) or [![Twitter](https://img.shields.io/badge/Twitter-Follow_@AGi_XT-blue?logo=twitter&style=plastic)](https://twitter.com/AGi_XT).
 
 We're always looking for ways to improve AGiXT and make it more useful for our users. Your support will help us continue to develop and enhance the application. Thank you for considering to support us!
 
 ## Our Team 🧑‍💻
 | Josh (@Josh-XT)                    | James (@JamesonRGrieve) | 
 |-----------------------------------|-----------------------------------|
 |[![GitHub](https://img.shields.io/badge/GitHub-Follow_@Josh--XT-white?logo=github&style=plastic)](https://github.com/Josh-XT)|[![GitHub](https://img.shields.io/badge/GitHub-Follow_@JamesonRGrieve-white?logo=github&style=plastic)](https://github.com/JamesonRGrieve)|
```

### Comparing `agixt-1.1.43b0/setup.py` & `agixt-1.1.44b0/setup.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.43b0/src/agixt/AGiXT.py` & `agixt-1.1.44b0/src/agixt/AGiXT.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from typing import List, Dict
 from Config.Agent import Agent
 from datetime import datetime
 from playwright.async_api import async_playwright
 from duckduckgo_search import ddg
 from Commands import Commands
 import json
-from json.decoder import JSONDecodeError
 from CustomPrompt import CustomPrompt
 from Memories import Memories
 import asyncio
 import pandas as pd
 import docx2txt
 import pdfplumber
 from urllib.parse import urlparse
@@ -164,15 +163,18 @@
                 **kwargs,
             )
         self.response = self.CFG.instruct(formatted_prompt, tokens=tokens)
         # Handle commands if the prompt contains the {COMMANDS} placeholder
         # We handle command injection that DOESN'T allow command execution by using {command_list} in the prompt
         if "{COMMANDS}" in unformatted_prompt:
             self.response = self.execution_agent(
-                execution_response=self.response, task=task, **kwargs
+                execution_response=self.response,
+                task=task,
+                context_results=context_results,
+                **kwargs,
             )
         print(f"Response: {self.response}")
         self.memories.store_result(task, self.response)
         self.CFG.log_interaction("USER", task)
         self.CFG.log_interaction(self.agent_name, self.response)
         return self.response
 
@@ -328,15 +330,15 @@
                     content = f.read()
             self.memories.store_result(task_name=task, result=content)
             return True
         except:
             return False
 
     # Worker Sub-Agents
-    def validation_agent(self, task, execution_response, **kwargs):
+    def validation_agent(self, task, execution_response, context_results, **kwargs):
         try:
             pattern = regex.compile(r"\{(?:[^{}]|(?R))*\}")
             cleaned_json = pattern.findall(execution_response)
             if len(cleaned_json) == 0:
                 return False
             if isinstance(cleaned_json, list):
                 cleaned_json = cleaned_json[0]
@@ -349,34 +351,44 @@
             if context_results != 0:
                 context_results = context_results - 1
             else:
                 context_results = 0
             execution_response = self.run(
                 task=task, context_results=context_results, **kwargs
             )
-            return self.validation_agent(task, execution_response, **kwargs)
+            return self.validation_agent(
+                task, execution_response, context_results, **kwargs
+            )
 
     def revalidation_agent(
-        self, task, command_name, command_args, command_output, **kwargs
+        self,
+        task,
+        command_name,
+        command_args,
+        command_output,
+        context_results,
+        **kwargs,
     ):
         print(
             f"Command {command_name} did not execute as expected with args {command_args}. Trying again.."
         )
         revalidate = self.run(
             task=task,
             prompt="ValidationFailed",
             command_name=command_name,
             command_args=command_args,
             command_output=command_output,
             **kwargs,
         )
-        return self.execution_agent(revalidate, task, **kwargs)
+        return self.execution_agent(revalidate, task, context_results, **kwargs)
 
-    def execution_agent(self, execution_response, task, **kwargs):
-        validated_response = self.validation_agent(task, execution_response, **kwargs)
+    def execution_agent(self, execution_response, task, context_results, **kwargs):
+        validated_response = self.validation_agent(
+            task, execution_response, context_results, **kwargs
+        )
         try:
             for command_name, command_args in validated_response["commands"].items():
                 # Search for the command in the available_commands list, and if found, use the command's name attribute for execution
                 if command_name is not None:
                     for available_command in self.available_commands:
                         if command_name in [
                             available_command["friendly_name"],
@@ -624,55 +636,14 @@
             self.update_output_list(f"\nNew Tasks:\n\n{new_tasks}\n")
             for new_task in new_tasks:
                 new_task.update({"task_id": len(self.task_list) + 1})
                 self.task_list.append(new_task)
             self.prioritization_agent()
         self.update_output_list("All tasks completed or stopped.")
 
-    def run_chain_step(self, step_data_list):
-        for step_data in step_data_list:
-            for prompt_type, prompt in step_data.items():
-                if prompt_type == "instruction":
-                    self.run(prompt, prompt="instruct")
-                elif prompt_type == "chat":
-                    self.run(prompt, prompt="chat")
-                elif prompt_type == "smart_instruct":
-                    self.smart_instruct(task=prompt, shots=3)
-                elif prompt_type == "smart_chat":
-                    self.smart_chat(task=prompt, shots=3)
-                elif prompt_type == "task":
-                    self.run_task(prompt)
-                elif prompt_type == "command":
-                    command = prompt.strip()
-                    command_name, command_args = None, {}
-                    # Extract command name and arguments using regex
-                    command_regex = re.search(r"(\w+)\((.*)\)", command)
-                    if command_regex:
-                        command_name, args_str = command_regex.groups()
-                        if args_str:
-                            # Parse arguments string into a dictionary
-                            args_str = args_str.replace("'", '"')
-                            args_str = args_str.replace("None", "null")
-                            try:
-                                command_args = json.loads(args_str)
-                            except JSONDecodeError as e:
-                                # error parsing args, send command_name to None so trying to execute command won't crash
-                                command_name = None
-                                print(f"Error: {e}")
-
-                    # Search for the command in the available_commands list, and if found, use the command's name attribute for execution
-                    if command_name is not None:
-                        for available_command in self.available_commands:
-                            if available_command["friendly_name"] == command_name:
-                                command_name = available_command["name"]
-                                break
-                        self.commands.execute_command(command_name, command_args)
-                else:
-                    self.run(task=prompt, prompt=prompt_type)
-
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("--task", type=str, default="Write a tweet about AI.")
     parser.add_argument("--agent_name", type=str, default="AGiXT")
     parser.add_argument("--option", type=str, default="")
     parser.add_argument("--shots", type=int, default=3)
```

### Comparing `agixt-1.1.43b0/src/agixt/Commands.py` & `agixt-1.1.44b0/src/agixt/Commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import importlib
 import os
 from inspect import signature, Parameter
 from Config.Agent import Agent
 
 
 class Commands:
-    def __init__(self, agent_name: str = "XTAgent", load_commands_flag: bool = True):
+    def __init__(self, agent_name: str = "AGiXT", load_commands_flag: bool = True):
         if agent_name == "undefined":
-            self.agent_name = "XTAgent"
+            self.agent_name = "AGiXT"
         else:
             self.agent_name = agent_name
         self.CFG = Agent(self.agent_name)
         self.agent_folder = self.CFG.create_agent_folder(self.agent_name)
         # self.agent_config_file = self.CFG.create_agent_config_file(self.agent_folder)
         self.agent_config = self.CFG.load_agent_config(self.agent_name)
         if load_commands_flag:
```

### Comparing `agixt-1.1.43b0/src/agixt/Config/Agent.py` & `agixt-1.1.44b0/src/agixt/Config/Agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 load_dotenv()
 
 
 class Agent(Config):
     def __init__(self, agent_name=None):
         # General Configuration
-        self.AGENT_NAME = agent_name if agent_name is not None else "XTAgent"
+        self.AGENT_NAME = agent_name if agent_name is not None else "AGiXT"
         # Need to get the following from the agent config file:
         self.AGENT_CONFIG = self.get_agent_config()
         # AI Configuration
         if "settings" in self.AGENT_CONFIG:
             self.PROVIDER_SETTINGS = self.AGENT_CONFIG["settings"]
             if "provider" in self.PROVIDER_SETTINGS:
                 self.AI_PROVIDER = self.PROVIDER_SETTINGS["provider"]
```

### Comparing `agixt-1.1.43b0/src/agixt/Config/__init__.py` & `agixt-1.1.44b0/src/agixt/Config/__init__.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.43b0/src/agixt/CustomPrompt.py` & `agixt-1.1.44b0/src/agixt/CustomPrompt.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.43b0/src/agixt/Embedding.py` & `agixt-1.1.44b0/src/agixt/Embedding.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.43b0/src/agixt/Memories.py` & `agixt-1.1.44b0/src/agixt/Memories.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from hashlib import sha256
 from Embedding import Embedding
 from datetime import datetime
 from collections import Counter
 
 
 class Memories:
-    def __init__(self, AGENT_NAME: str = "XTAgent", AgentConfig=None, nlp=None):
+    def __init__(self, AGENT_NAME: str = "AGiXT", AgentConfig=None, nlp=None):
         self.AGENT_NAME = AGENT_NAME
         self.CFG = AgentConfig
         self.nlp = nlp if nlp else self.load_spacy_model()
         self.nlp.max_length = 999999999999999999999999999999999
         embedder = Embedding(CFG=AgentConfig)
         self.embedding_function = embedder.embed
         self.chunk_size = embedder.chunk_size
```

### Comparing `agixt-1.1.43b0/src/agixt/app.py` & `agixt-1.1.44b0/src/agixt/app.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.43b0/src/agixt/provider/__init__.py` & `agixt-1.1.44b0/src/agixt/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.43b0/src/agixt/provider/azure.py` & `agixt-1.1.44b0/src/agixt/provider/azure.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.43b0/src/agixt/provider/bing.py` & `agixt-1.1.44b0/src/agixt/provider/bing.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.43b0/src/agixt/provider/fastchat.py` & `agixt-1.1.44b0/src/agixt/provider/fastchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.43b0/src/agixt/provider/gpt4all.py` & `agixt-1.1.44b0/src/agixt/provider/gpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.43b0/src/agixt/provider/gpt4free.py` & `agixt-1.1.44b0/src/agixt/provider/gpt4free.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.43b0/src/agixt/provider/gpugpt4all.py` & `agixt-1.1.44b0/src/agixt/provider/gpugpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.43b0/src/agixt/provider/huggingchat.py` & `agixt-1.1.44b0/src/agixt/provider/huggingchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.43b0/src/agixt/provider/kobold.py` & `agixt-1.1.44b0/src/agixt/provider/kobold.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.43b0/src/agixt/provider/llamacpp.py` & `agixt-1.1.44b0/src/agixt/provider/llamacpp.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.43b0/src/agixt/provider/oobabooga.py` & `agixt-1.1.44b0/src/agixt/provider/oobabooga.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.43b0/src/agixt/provider/openai.py` & `agixt-1.1.44b0/src/agixt/provider/openai.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.43b0/src/agixt/provider/palm.py` & `agixt-1.1.44b0/src/agixt/provider/palm.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.43b0/src/agixt/provider/transformer.py` & `agixt-1.1.44b0/src/agixt/provider/transformer.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.43b0/src/agixt/requirements.txt` & `agixt-1.1.44b0/src/agixt/requirements.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.43b0/src/agixt/smartchat.py` & `agixt-1.1.44b0/src/agixt/smartchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.43b0/src/agixt/smartinstruct.py` & `agixt-1.1.44b0/src/agixt/smartinstruct.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.43b0/src/agixt/streamlit.py` & `agixt-1.1.44b0/src/agixt/streamlit.py`

 * *Files 0% similar despite different names*

```diff
@@ -306,15 +306,15 @@
                     if chat["sender"] == "User":
                         st.markdown(
                             f'<div style="text-align: left; margin-bottom: 5px;"><strong>User:</strong> {chat["message"]}</div>',
                             unsafe_allow_html=True,
                         )
                     else:
                         st.markdown(
-                            f'<div style="text-align: right; margin-bottom: 5px;"><strong>Agent:</strong> {chat["message"]}</div>',
+                            f'<div style="text-align: left; margin-bottom: 5px;"><strong>Agent:</strong> {chat["message"]}</div>',
                             unsafe_allow_html=True,
                         )
 
     if agent_name:
         learn_file_upload = st.file_uploader("Upload a file to learn from")
         learn_file_path = ""
         if learn_file_upload is not None:
@@ -396,15 +396,15 @@
                     if instruct["sender"] == "User":
                         st.markdown(
                             f'<div style="text-align: left; margin-bottom: 5px;"><strong>User:</strong> {instruct["message"]}</div>',
                             unsafe_allow_html=True,
                         )
                     else:
                         st.markdown(
-                            f'<div style="text-align: right; margin-bottom: 5px;"><strong>Agent:</strong> {instruct["message"]}</div>',
+                            f'<div style="text-align: left; margin-bottom: 5px;"><strong>Agent:</strong> {instruct["message"]}</div>',
                             unsafe_allow_html=True,
                         )
 
     if agent_name:
         learn_file_upload = st.file_uploader("Upload a file to learn from")
         learn_file_path = ""
         if learn_file_upload is not None:
```

### Comparing `agixt-1.1.43b0/src/agixt.egg-info/PKG-INFO` & `agixt-1.1.44b0/docs/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,21 @@
-Metadata-Version: 2.1
-Name: agixt
-Version: 1.1.43b0
-Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
-Author: Josh XT
-Author-email: josh@devxt.com
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # AGiXT
 
 ![RELEASE](https://img.shields.io/github/v/release/Josh-XT/AGiXT?label=Release%20Version&style=plastic) 
 [![STATUS](https://img.shields.io/badge/status-beta-blue?label=Release%20Status&style=plastic)](https://github.com/josh-xt/AGiXT) 
 [![LICENSE: MIT](https://img.shields.io/github/license/Josh-XT/AGiXT?label=License&style=plastic)](https://github.com/Josh-XT/AGiXT/blob/main/LICENSE) 
 ![DOCKER](https://img.shields.io/github/actions/workflow/status/Josh-XT/AGiXT/publish-docker.yml?branch=main&label=Docker&style=plastic) [![CODESTYLE](https://img.shields.io/badge/code%20style-Black-black?branch=main&label=Code%20Style&style=plastic)](https://black.readthedocs.io/en/stable/the_black_code_style/index.html)
 
-[![GitHub](https://img.shields.io/badge/GitHub-Frontend_Repository-grey?logo=github&style=plastic)](https://github.com/JamesonRGrieve/AGiXT-Frontend)
+[![GitHub](https://img.shields.io/badge/GitHub-Frontend_Repository-grey?logo=github&style=plastic)](https://github.com/JamesonRGrieve/Agent-LLM-Frontend)
 
 [![Contribute](https://img.shields.io/github/issues/Josh-XT/AGiXT/help%20wanted?color=purple&label=Quick%20Contribute%20Backend&logo=github&style=plastic)](https://github.com/Josh-XT/AGiXT/labels/help%20wanted) 
-[![Contribute](https://img.shields.io/github/issues/JamesonRGrieve/AGiXT-Frontend/help%20wanted?color=purple&label=Quick%20Contribute%20Frontend&logo=github&style=plastic)](https://github.com/JamesonRGrieve/AGiXT-Frontend/labels/help%20wanted) 
+[![Contribute](https://img.shields.io/github/issues/JamesonRGrieve/Agent-LLM-Frontend/help%20wanted?color=purple&label=Quick%20Contribute%20Frontend&logo=github&style=plastic)](https://github.com/JamesonRGrieve/Agent-LLM-Frontend/labels/help%20wanted) 
 [![Discord](https://img.shields.io/discord/1097720481970397356?label=Discord&logo=discord&logoColor=white&style=plastic&color=5865f2)](https://discord.gg/d3TkHRZcjD) 
-[![Twitter](https://img.shields.io/badge/Twitter-Follow_@AGiXT-blue?logo=twitter&style=plastic)](https://twitter.com/AGiXT) 
-[![FacebookGroup](https://img.shields.io/badge/Facebook-Join_Our_Group-blue?logo=facebook&style=plastic)](https://www.facebook.com/groups/AGiXT)
-[![EMail](https://img.shields.io/badge/E--Mail-Outreach_&_Media-5865f2?logo=gmail&style=plastic)](https://twitter.com/AGiXT) 
+[![Twitter](https://img.shields.io/badge/Twitter-Follow_@AGi_XT-blue?logo=twitter&style=plastic)](https://twitter.com/AGi_XT) 
+[![EMail](https://img.shields.io/badge/E--Mail-Outreach_&_Media-5865f2?logo=gmail&style=plastic)](https://twitter.com/AGi_XT) 
 
 Please use the outreach email for media, sponsorship, or to contact us for other miscellaneous purposes. 
 
 **Do not** send us emails with troubleshooting requests, feature requests or bug reports, please direct those to [GitHub Issues](https://github.com/Josh-XT/AGiXT/issues) or [Discord](https://discord.gg/d3TkHRZcjD).
 
 AGiXT is an Artificial Intelligence Automation Platform designed to power efficient AI instruction management across multiple providers. Our agents are equipped with adaptive memory, and this versatile solution offers a powerful plugin system that supports a wide range of commands, including web browsing. With growing support for numerous AI providers and models, AGiXT is constantly evolving to empower diverse applications.
 
@@ -186,26 +175,26 @@
 
 ### Back End
 
 Clone the repository for the AGiXT back end and start it.
 
 ```
 git clone https://github.com/Josh-XT/AGiXT
-cd AGiXT
+cd AGiXT/src/agixt
 pip install -r requirements.txt
 python app.py
 ```
 
 ### Front End
 
 Clone the repository for the AGiXT front end in a separate terminal and start it.
 
 ```
-git clone https://github.com/JamesonRGrieve/AGiXT-Frontend --recurse-submodules 
-cd AGiXT-Frontend
+git clone https://github.com/JamesonRGrieve/Agent-LLM-Frontend --recurse-submodules 
+cd Agent-LLM-Frontend
 yarn install
 yarn dev
 ```
 
 Access the web interface at http://localhost:3000
 
 ## Configuration
@@ -253,18 +242,18 @@
 
 In `docs/` folder. Can be used to generate static html output. See `deploy-docs` section in [Publish Workflow](/.github/workflows/python-publish.yml) howto build with honkit.
 
 ## Contributing
 
 [![Contribute](https://img.shields.io/github/issues/Josh-XT/AGiXT/help%20wanted?color=purple&label=Quick%20Contribute&logo=github&style=plastic)](https://github.com/Josh-XT/AGiXT/labels/help%20wanted) 
 
-We welcome contributions to AGiXT! If you're interested in contributing, please check out our [contributions guide](https://github.com/Josh-XT/AGiXT/tree/main/.github/CONTRIBUTING.md) the [open issues on the backend](https://github.com/Josh-XT/AGiXT/issues), [open issues on the frontend](https://github.com/JamesonRGrieve/AGiXT-Frontend/issues) and [pull requests](https://github.com/Josh-XT/AGiXT/pulls), submit a [pull request](https://github.com/Josh-XT/AGiXT/pulls/new), or [suggest new features](https://github.com/Josh-XT/AGiXT/issues/new). To stay updated on the project's progress, [![Twitter](https://img.shields.io/badge/Twitter-Follow_@AGiXT-blue?logo=twitter&style=plastic)](https://twitter.com/AGiXT), [![Twitter](https://img.shields.io/badge/Twitter-Follow_@Josh_XT-blue?logo=twitter&style=plastic)](https://twitter.com/Josh_XT) and [![Twitter](https://img.shields.io/badge/Twitter-Follow_@JamesonRGrieve-blue?logo=twitter&style=plastic)](https://twitter.com/JamesonRGrieve). Also feel free to join our [![Discord](https://img.shields.io/discord/1097720481970397356?label=Discord&logo=discord&logoColor=white&style=plastic&color=5865f2)](https://discord.gg/d3TkHRZcjD).
+We welcome contributions to AGiXT! If you're interested in contributing, please check out our [contributions guide](https://github.com/Josh-XT/AGiXT/tree/main/.github/CONTRIBUTING.md) the [open issues on the backend](https://github.com/Josh-XT/AGiXT/issues), [open issues on the frontend](https://github.com/JamesonRGrieve/Agent-LLM-Frontend/issues) and [pull requests](https://github.com/Josh-XT/AGiXT/pulls), submit a [pull request](https://github.com/Josh-XT/AGiXT/pulls/new), or [suggest new features](https://github.com/Josh-XT/AGiXT/issues/new). To stay updated on the project's progress, [![Twitter](https://img.shields.io/badge/Twitter-Follow_@AGi_XT-blue?logo=twitter&style=plastic)](https://twitter.com/AGi_XT), [![Twitter](https://img.shields.io/badge/Twitter-Follow_@Josh_XT-blue?logo=twitter&style=plastic)](https://twitter.com/Josh_XT) and [![Twitter](https://img.shields.io/badge/Twitter-Follow_@JamesonRGrieve-blue?logo=twitter&style=plastic)](https://twitter.com/JamesonRGrieve). Also feel free to join our [![Discord](https://img.shields.io/discord/1097720481970397356?label=Discord&logo=discord&logoColor=white&style=plastic&color=5865f2)](https://discord.gg/d3TkHRZcjD).
 
 ## Donations and Sponsorships
-We appreciate any support for AGiXT's development, including donations, sponsorships, and any other kind of assistance. If you would like to support us, please contact us through our [![EMail](https://img.shields.io/badge/E--Mail-Outreach_&_Media-5865f2?logo=gmail&style=plastic)](https://twitter.com/AGiXT) , [![Discord](https://img.shields.io/discord/1097720481970397356?label=Discord&logo=discord&logoColor=white&style=plastic&color=5865f2)](https://discord.gg/d3TkHRZcjD) or [![Twitter](https://img.shields.io/badge/Twitter-Follow_@AGiXT-blue?logo=twitter&style=plastic)](https://twitter.com/AGiXT).
+We appreciate any support for AGiXT's development, including donations, sponsorships, and any other kind of assistance. If you would like to support us, please contact us through our [![EMail](https://img.shields.io/badge/E--Mail-Outreach_&_Media-5865f2?logo=gmail&style=plastic)](https://twitter.com/AGi_XT) , [![Discord](https://img.shields.io/discord/1097720481970397356?label=Discord&logo=discord&logoColor=white&style=plastic&color=5865f2)](https://discord.gg/d3TkHRZcjD) or [![Twitter](https://img.shields.io/badge/Twitter-Follow_@AGi_XT-blue?logo=twitter&style=plastic)](https://twitter.com/AGi_XT).
 
 We're always looking for ways to improve AGiXT and make it more useful for our users. Your support will help us continue to develop and enhance the application. Thank you for considering to support us!
 
 ## Our Team 🧑‍💻
 | Josh (@Josh-XT)                    | James (@JamesonRGrieve) | 
 |-----------------------------------|-----------------------------------|
 |[![GitHub](https://img.shields.io/badge/GitHub-Follow_@Josh--XT-white?logo=github&style=plastic)](https://github.com/Josh-XT)|[![GitHub](https://img.shields.io/badge/GitHub-Follow_@JamesonRGrieve-white?logo=github&style=plastic)](https://github.com/JamesonRGrieve)|
```

### Comparing `agixt-1.1.43b0/src/agixt.egg-info/SOURCES.txt` & `agixt-1.1.44b0/src/agixt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.43b0/src/agixt.egg-info/requires.txt` & `agixt-1.1.44b0/src/agixt.egg-info/requires.txt`

 * *Files identical despite different names*

