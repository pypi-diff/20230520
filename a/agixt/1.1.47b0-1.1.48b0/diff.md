# Comparing `tmp/agixt-1.1.47b0.tar.gz` & `tmp/agixt-1.1.48b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agixt-1.1.47b0.tar", last modified: Sat May 20 14:25:36 2023, max compression
+gzip compressed data, was "agixt-1.1.48b0.tar", last modified: Sat May 20 17:59:04 2023, max compression
```

## Comparing `agixt-1.1.47b0.tar` & `agixt-1.1.48b0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:25:36.452568 agixt-1.1.47b0/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-20 14:25:25.000000 agixt-1.1.47b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-20 14:25:25.000000 agixt-1.1.47b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    19140 2023-05-20 14:25:36.452568 agixt-1.1.47b0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:25:36.448568 agixt-1.1.47b0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    18683 2023-05-20 14:25:25.000000 agixt-1.1.47b0/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-20 14:25:25.000000 agixt-1.1.47b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 14:25:36.452568 agixt-1.1.47b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-20 14:25:25.000000 agixt-1.1.47b0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:25:36.448568 agixt-1.1.47b0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:25:36.452568 agixt-1.1.47b0/src/agixt/
--rw-r--r--   0 runner    (1001) docker     (123)    25091 2023-05-20 14:25:25.000000 agixt-1.1.47b0/src/agixt/AGiXT.py
--rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-05-20 14:25:25.000000 agixt-1.1.47b0/src/agixt/Chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-05-20 14:25:25.000000 agixt-1.1.47b0/src/agixt/Commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:25:36.452568 agixt-1.1.47b0/src/agixt/Config/
--rw-r--r--   0 runner    (1001) docker     (123)    13461 2023-05-20 14:25:25.000000 agixt-1.1.47b0/src/agixt/Config/Agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-20 14:25:25.000000 agixt-1.1.47b0/src/agixt/Config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-20 14:25:25.000000 agixt-1.1.47b0/src/agixt/CustomPrompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-05-20 14:25:25.000000 agixt-1.1.47b0/src/agixt/Embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-05-20 14:25:25.000000 agixt-1.1.47b0/src/agixt/Memories.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-20 14:25:25.000000 agixt-1.1.47b0/src/agixt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13588 2023-05-20 14:25:25.000000 agixt-1.1.47b0/src/agixt/app.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-05-20 14:25:25.000000 agixt-1.1.47b0/src/agixt/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:25:36.452568 agixt-1.1.47b0/src/agixt/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-20 14:25:25.000000 agixt-1.1.47b0/src/agixt/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-20 14:25:25.000000 agixt-1.1.47b0/src/agixt/provider/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-20 14:25:25.000000 agixt-1.1.47b0/src/agixt/provider/bard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-20 14:25:25.000000 agixt-1.1.47b0/src/agixt/provider/bing.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-20 14:25:25.000000 agixt-1.1.47b0/src/agixt/provider/fastchat.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-20 14:25:25.000000 agixt-1.1.47b0/src/agixt/provider/gpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-05-20 14:25:25.000000 agixt-1.1.47b0/src/agixt/provider/gpt4free.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-20 14:25:25.000000 agixt-1.1.47b0/src/agixt/provider/gpugpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-20 14:25:25.000000 agixt-1.1.47b0/src/agixt/provider/huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-20 14:25:25.000000 agixt-1.1.47b0/src/agixt/provider/kobold.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-20 14:25:25.000000 agixt-1.1.47b0/src/agixt/provider/llamacpp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-20 14:25:25.000000 agixt-1.1.47b0/src/agixt/provider/oobabooga.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-20 14:25:25.000000 agixt-1.1.47b0/src/agixt/provider/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-20 14:25:25.000000 agixt-1.1.47b0/src/agixt/provider/palm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-20 14:25:25.000000 agixt-1.1.47b0/src/agixt/provider/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-20 14:25:25.000000 agixt-1.1.47b0/src/agixt/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-20 14:25:25.000000 agixt-1.1.47b0/src/agixt/smartchat.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-20 14:25:25.000000 agixt-1.1.47b0/src/agixt/smartinstruct.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-20 14:25:25.000000 agixt-1.1.47b0/src/agixt/streamlit.py
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-20 14:25:25.000000 agixt-1.1.47b0/src/agixt/version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:25:36.452568 agixt-1.1.47b0/src/agixt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19140 2023-05-20 14:25:36.000000 agixt-1.1.47b0/src/agixt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-20 14:25:36.000000 agixt-1.1.47b0/src/agixt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 14:25:36.000000 agixt-1.1.47b0/src/agixt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-20 14:25:36.000000 agixt-1.1.47b0/src/agixt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-20 14:25:36.000000 agixt-1.1.47b0/src/agixt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:59:04.752268 agixt-1.1.48b0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-20 17:58:52.000000 agixt-1.1.48b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-20 17:58:52.000000 agixt-1.1.48b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    18794 2023-05-20 17:59:04.752268 agixt-1.1.48b0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:59:04.748268 agixt-1.1.48b0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    18337 2023-05-20 17:58:52.000000 agixt-1.1.48b0/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-20 17:58:52.000000 agixt-1.1.48b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 17:59:04.752268 agixt-1.1.48b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-20 17:58:52.000000 agixt-1.1.48b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:59:04.748268 agixt-1.1.48b0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:59:04.748268 agixt-1.1.48b0/src/agixt/
+-rw-r--r--   0 runner    (1001) docker     (123)    25177 2023-05-20 17:58:52.000000 agixt-1.1.48b0/src/agixt/AGiXT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-05-20 17:58:52.000000 agixt-1.1.48b0/src/agixt/Chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-05-20 17:58:52.000000 agixt-1.1.48b0/src/agixt/Commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:59:04.752268 agixt-1.1.48b0/src/agixt/Config/
+-rw-r--r--   0 runner    (1001) docker     (123)    13461 2023-05-20 17:58:52.000000 agixt-1.1.48b0/src/agixt/Config/Agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-20 17:58:52.000000 agixt-1.1.48b0/src/agixt/Config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-20 17:58:52.000000 agixt-1.1.48b0/src/agixt/CustomPrompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-05-20 17:58:52.000000 agixt-1.1.48b0/src/agixt/Embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-05-20 17:58:52.000000 agixt-1.1.48b0/src/agixt/Memories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-20 17:58:52.000000 agixt-1.1.48b0/src/agixt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13588 2023-05-20 17:58:52.000000 agixt-1.1.48b0/src/agixt/app.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-05-20 17:58:52.000000 agixt-1.1.48b0/src/agixt/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:59:04.752268 agixt-1.1.48b0/src/agixt/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-20 17:58:52.000000 agixt-1.1.48b0/src/agixt/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-20 17:58:52.000000 agixt-1.1.48b0/src/agixt/provider/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-20 17:58:52.000000 agixt-1.1.48b0/src/agixt/provider/bard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-20 17:58:52.000000 agixt-1.1.48b0/src/agixt/provider/bing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-20 17:58:52.000000 agixt-1.1.48b0/src/agixt/provider/fastchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-20 17:58:52.000000 agixt-1.1.48b0/src/agixt/provider/gpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-05-20 17:58:52.000000 agixt-1.1.48b0/src/agixt/provider/gpt4free.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-20 17:58:52.000000 agixt-1.1.48b0/src/agixt/provider/gpugpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-20 17:58:52.000000 agixt-1.1.48b0/src/agixt/provider/huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-20 17:58:52.000000 agixt-1.1.48b0/src/agixt/provider/kobold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-20 17:58:52.000000 agixt-1.1.48b0/src/agixt/provider/llamacpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-20 17:58:52.000000 agixt-1.1.48b0/src/agixt/provider/oobabooga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-20 17:58:52.000000 agixt-1.1.48b0/src/agixt/provider/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-20 17:58:52.000000 agixt-1.1.48b0/src/agixt/provider/palm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-20 17:58:52.000000 agixt-1.1.48b0/src/agixt/provider/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-20 17:58:52.000000 agixt-1.1.48b0/src/agixt/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-20 17:58:52.000000 agixt-1.1.48b0/src/agixt/smartchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-20 17:58:52.000000 agixt-1.1.48b0/src/agixt/smartinstruct.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-20 17:58:52.000000 agixt-1.1.48b0/src/agixt/streamlit.py
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-20 17:58:52.000000 agixt-1.1.48b0/src/agixt/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:59:04.752268 agixt-1.1.48b0/src/agixt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18794 2023-05-20 17:59:04.000000 agixt-1.1.48b0/src/agixt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-20 17:59:04.000000 agixt-1.1.48b0/src/agixt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 17:59:04.000000 agixt-1.1.48b0/src/agixt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-20 17:59:04.000000 agixt-1.1.48b0/src/agixt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-20 17:59:04.000000 agixt-1.1.48b0/src/agixt.egg-info/top_level.txt
```

### Comparing `agixt-1.1.47b0/LICENSE` & `agixt-1.1.48b0/LICENSE`

 * *Files identical despite different names*

### Comparing `agixt-1.1.47b0/PKG-INFO` & `agixt-1.1.48b0/docs/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,41 +1,29 @@
-Metadata-Version: 2.1
-Name: agixt
-Version: 1.1.47b0
-Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
-Author: Josh XT
-Author-email: josh@devxt.com
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # AGiXT
-
 ![RELEASE](https://img.shields.io/github/v/release/Josh-XT/AGiXT?label=Release%20Version&style=plastic) 
 [![STATUS](https://img.shields.io/badge/status-beta-blue?label=Release%20Status&style=plastic)](https://github.com/josh-xt/AGiXT) 
 [![LICENSE: MIT](https://img.shields.io/github/license/Josh-XT/AGiXT?label=License&style=plastic)](https://github.com/Josh-XT/AGiXT/blob/main/LICENSE) 
 ![DOCKER](https://img.shields.io/github/actions/workflow/status/Josh-XT/AGiXT/publish-docker.yml?branch=main&label=Docker&style=plastic) [![CODESTYLE](https://img.shields.io/badge/code%20style-Black-black?branch=main&label=Code%20Style&style=plastic)](https://black.readthedocs.io/en/stable/the_black_code_style/index.html)
 
 [![GitHub](https://img.shields.io/badge/GitHub-Frontend_Repository-grey?logo=github&style=plastic)](https://github.com/JamesonRGrieve/Agent-LLM-Frontend)
 
 [![Contribute](https://img.shields.io/github/issues/Josh-XT/AGiXT/help%20wanted?color=purple&label=Quick%20Contribute%20Backend&logo=github&style=plastic)](https://github.com/Josh-XT/AGiXT/labels/help%20wanted) 
 [![Contribute](https://img.shields.io/github/issues/JamesonRGrieve/Agent-LLM-Frontend/help%20wanted?color=purple&label=Quick%20Contribute%20Frontend&logo=github&style=plastic)](https://github.com/JamesonRGrieve/Agent-LLM-Frontend/labels/help%20wanted) 
 [![Discord](https://img.shields.io/discord/1097720481970397356?label=Discord&logo=discord&logoColor=white&style=plastic&color=5865f2)](https://discord.gg/d3TkHRZcjD) 
 [![Twitter](https://img.shields.io/badge/Twitter-Follow_@AGi_XT-blue?logo=twitter&style=plastic)](https://twitter.com/AGi_XT) 
 [![EMail](https://img.shields.io/badge/E--Mail-Outreach_&_Media-5865f2?logo=gmail&style=plastic)](https://twitter.com/AGi_XT) 
 
+![Logo](AGiXT.svg)
+
 Please use the outreach email for media, sponsorship, or to contact us for other miscellaneous purposes. 
 
 **Do not** send us emails with troubleshooting requests, feature requests or bug reports, please direct those to [GitHub Issues](https://github.com/Josh-XT/AGiXT/issues) or [Discord](https://discord.gg/d3TkHRZcjD).
 
 AGiXT is an Artificial Intelligence Automation Platform designed to power efficient AI instruction management across multiple providers. Our agents are equipped with adaptive memory, and this versatile solution offers a powerful plugin system that supports a wide range of commands, including web browsing. With growing support for numerous AI providers and models, AGiXT is constantly evolving to empower diverse applications.
 
-![image](https://user-images.githubusercontent.com/102809327/234344654-a1a4201b-594b-4a00-ac78-279a2e5bbe43.png)
-
-![image](https://user-images.githubusercontent.com/102809327/235532233-72f291a7-0633-435f-b72c-7f56bce682d8.png)
 
 ## ⚠️ Run this in Docker or a Virtual Machine!
 You're welcome to disregard this message, but if you do and the AI decides that the best course of action for its task is to build a command to format your entire computer, that is on you.  Understand that this is given full unrestricted terminal access by design and that we have no intentions of building any safeguards.  This project intends to stay light weight and versatile for the best possible research outcomes.
 
 See also [SECURITY.md](1-Getting started/SECURITY.MD)
 
 ## ⚠️ Monitor Your Usage!
@@ -87,16 +75,15 @@
   - [Key Features 🗝️](#key-features-️)
   - [Web Application Features](#web-application-features)
   - [Run with Docker](#run-with-docker)
     - [Linux or Windows](#linux-or-windows)
     - [Windows Docker Desktop (streamlit only example)](#windows-docker-desktop-streamlit-only-example)
     - [Development using docker](#development-using-docker)
   - [Manual Install from source (unsupported)](#manual-install-from-source-unsupported)
-    - [Back End](#back-end)
-    - [Front End](#front-end)
+    - [Streamlit App Locally](#streamlit-app-locally)
   - [Configuration](#configuration)
   - [API Endpoints](#api-endpoints)
   - [Extending Functionality](#extending-functionality)
     - [Updating Requirements](#updating-requirements)
     - [Commands](#commands)
     - [AI Providers](#ai-providers)
   - [Documentation](#documentation)
@@ -163,53 +150,41 @@
 Run all available services
 `docker compose --profile all up`
 
 - AGiXT-frontend http://localhost:3000
 - streamlit-UI http://localhost:8501
 
 ### Windows Docker Desktop (streamlit only example)
-
-![On Windows Docker Desktop](Docker-desktop-win-setting-streamlit.png)
-
+- Container Name: AGiXT
+- Host Port: 8501:8501/tcp
 
 ### Development using docker
 ```
 docker compose --profile all -f docker-compose.yml -f docker-compose.dev.yaml up
 ```
 
 * mounts dev space into container - happy building 
 
 
 ## Manual Install from source (unsupported)
 
 As a reminder, this can be dangerous to run locally depending on what commands you give your agents access to.  [⚠️ Run this in Docker or a Virtual Machine!](#️-run-this-in-docker-or-a-virtual-machine)
 
-### Back End
+### Streamlit App Locally
 
 Clone the repository for the AGiXT back end and start it.
 
 ```
 git clone https://github.com/Josh-XT/AGiXT
 cd AGiXT/src/agixt
 pip install -r requirements.txt
-python app.py
-```
-
-### Front End
-
-Clone the repository for the AGiXT front end in a separate terminal and start it.
-
-```
-git clone https://github.com/JamesonRGrieve/Agent-LLM-Frontend --recurse-submodules 
-cd Agent-LLM-Frontend
-yarn install
-yarn dev
+streamlit run streamlit.py
 ```
 
-Access the web interface at http://localhost:3000
+Access the web interface at http://localhost:8501
 
 ## Configuration
 
 AGiXT utilizes a `.env` configuration file to store AI language model settings, API keys, and other options. Use the supplied `.env.example` as a template to create your personalized `.env` file. Configuration settings include:
 
 - **WORKING_DIRECTORY**: Set the agent's working directory.
 - **EXTENSIONS_SETTINGS**: Configure settings for OpenAI, Hugging Face, Selenium, Twitter, and GitHub.
@@ -217,14 +192,19 @@
 
 For a detailed explanation of each setting, refer to the `.env.example` file provided in the repository.
 
 ## API Endpoints
 
 AGiXT provides several API endpoints for managing agents, prompts and chains.
 
+If you're not running with Docker, the back end can be run with:
+```
+python src/agixt/app.py
+```
+
 To learn more about the API endpoints and their usage, visit the API documentation at 
 - [Swagger](http://localhost:7437)
 - [Redoc](http://localhost:7437/redoc)
 
 This documentation is hosted locally and the frontend must be running for these links to work.
 
 ## Extending Functionality
```

### Comparing `agixt-1.1.47b0/docs/README.md` & `agixt-1.1.48b0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,39 @@
-# AGiXT
+Metadata-Version: 2.1
+Name: agixt
+Version: 1.1.48b0
+Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
+Author: Josh XT
+Author-email: josh@devxt.com
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
 
+# AGiXT
 ![RELEASE](https://img.shields.io/github/v/release/Josh-XT/AGiXT?label=Release%20Version&style=plastic) 
 [![STATUS](https://img.shields.io/badge/status-beta-blue?label=Release%20Status&style=plastic)](https://github.com/josh-xt/AGiXT) 
 [![LICENSE: MIT](https://img.shields.io/github/license/Josh-XT/AGiXT?label=License&style=plastic)](https://github.com/Josh-XT/AGiXT/blob/main/LICENSE) 
 ![DOCKER](https://img.shields.io/github/actions/workflow/status/Josh-XT/AGiXT/publish-docker.yml?branch=main&label=Docker&style=plastic) [![CODESTYLE](https://img.shields.io/badge/code%20style-Black-black?branch=main&label=Code%20Style&style=plastic)](https://black.readthedocs.io/en/stable/the_black_code_style/index.html)
 
 [![GitHub](https://img.shields.io/badge/GitHub-Frontend_Repository-grey?logo=github&style=plastic)](https://github.com/JamesonRGrieve/Agent-LLM-Frontend)
 
 [![Contribute](https://img.shields.io/github/issues/Josh-XT/AGiXT/help%20wanted?color=purple&label=Quick%20Contribute%20Backend&logo=github&style=plastic)](https://github.com/Josh-XT/AGiXT/labels/help%20wanted) 
 [![Contribute](https://img.shields.io/github/issues/JamesonRGrieve/Agent-LLM-Frontend/help%20wanted?color=purple&label=Quick%20Contribute%20Frontend&logo=github&style=plastic)](https://github.com/JamesonRGrieve/Agent-LLM-Frontend/labels/help%20wanted) 
 [![Discord](https://img.shields.io/discord/1097720481970397356?label=Discord&logo=discord&logoColor=white&style=plastic&color=5865f2)](https://discord.gg/d3TkHRZcjD) 
 [![Twitter](https://img.shields.io/badge/Twitter-Follow_@AGi_XT-blue?logo=twitter&style=plastic)](https://twitter.com/AGi_XT) 
 [![EMail](https://img.shields.io/badge/E--Mail-Outreach_&_Media-5865f2?logo=gmail&style=plastic)](https://twitter.com/AGi_XT) 
 
+![Logo](AGiXT.svg)
+
 Please use the outreach email for media, sponsorship, or to contact us for other miscellaneous purposes. 
 
 **Do not** send us emails with troubleshooting requests, feature requests or bug reports, please direct those to [GitHub Issues](https://github.com/Josh-XT/AGiXT/issues) or [Discord](https://discord.gg/d3TkHRZcjD).
 
 AGiXT is an Artificial Intelligence Automation Platform designed to power efficient AI instruction management across multiple providers. Our agents are equipped with adaptive memory, and this versatile solution offers a powerful plugin system that supports a wide range of commands, including web browsing. With growing support for numerous AI providers and models, AGiXT is constantly evolving to empower diverse applications.
 
-![image](https://user-images.githubusercontent.com/102809327/234344654-a1a4201b-594b-4a00-ac78-279a2e5bbe43.png)
-
-![image](https://user-images.githubusercontent.com/102809327/235532233-72f291a7-0633-435f-b72c-7f56bce682d8.png)
 
 ## ⚠️ Run this in Docker or a Virtual Machine!
 You're welcome to disregard this message, but if you do and the AI decides that the best course of action for its task is to build a command to format your entire computer, that is on you.  Understand that this is given full unrestricted terminal access by design and that we have no intentions of building any safeguards.  This project intends to stay light weight and versatile for the best possible research outcomes.
 
 See also [SECURITY.md](1-Getting started/SECURITY.MD)
 
 ## ⚠️ Monitor Your Usage!
@@ -77,16 +85,15 @@
   - [Key Features 🗝️](#key-features-️)
   - [Web Application Features](#web-application-features)
   - [Run with Docker](#run-with-docker)
     - [Linux or Windows](#linux-or-windows)
     - [Windows Docker Desktop (streamlit only example)](#windows-docker-desktop-streamlit-only-example)
     - [Development using docker](#development-using-docker)
   - [Manual Install from source (unsupported)](#manual-install-from-source-unsupported)
-    - [Back End](#back-end)
-    - [Front End](#front-end)
+    - [Streamlit App Locally](#streamlit-app-locally)
   - [Configuration](#configuration)
   - [API Endpoints](#api-endpoints)
   - [Extending Functionality](#extending-functionality)
     - [Updating Requirements](#updating-requirements)
     - [Commands](#commands)
     - [AI Providers](#ai-providers)
   - [Documentation](#documentation)
@@ -153,53 +160,41 @@
 Run all available services
 `docker compose --profile all up`
 
 - AGiXT-frontend http://localhost:3000
 - streamlit-UI http://localhost:8501
 
 ### Windows Docker Desktop (streamlit only example)
-
-![On Windows Docker Desktop](Docker-desktop-win-setting-streamlit.png)
-
+- Container Name: AGiXT
+- Host Port: 8501:8501/tcp
 
 ### Development using docker
 ```
 docker compose --profile all -f docker-compose.yml -f docker-compose.dev.yaml up
 ```
 
 * mounts dev space into container - happy building 
 
 
 ## Manual Install from source (unsupported)
 
 As a reminder, this can be dangerous to run locally depending on what commands you give your agents access to.  [⚠️ Run this in Docker or a Virtual Machine!](#️-run-this-in-docker-or-a-virtual-machine)
 
-### Back End
+### Streamlit App Locally
 
 Clone the repository for the AGiXT back end and start it.
 
 ```
 git clone https://github.com/Josh-XT/AGiXT
 cd AGiXT/src/agixt
 pip install -r requirements.txt
-python app.py
-```
-
-### Front End
-
-Clone the repository for the AGiXT front end in a separate terminal and start it.
-
-```
-git clone https://github.com/JamesonRGrieve/Agent-LLM-Frontend --recurse-submodules 
-cd Agent-LLM-Frontend
-yarn install
-yarn dev
+streamlit run streamlit.py
 ```
 
-Access the web interface at http://localhost:3000
+Access the web interface at http://localhost:8501
 
 ## Configuration
 
 AGiXT utilizes a `.env` configuration file to store AI language model settings, API keys, and other options. Use the supplied `.env.example` as a template to create your personalized `.env` file. Configuration settings include:
 
 - **WORKING_DIRECTORY**: Set the agent's working directory.
 - **EXTENSIONS_SETTINGS**: Configure settings for OpenAI, Hugging Face, Selenium, Twitter, and GitHub.
@@ -207,14 +202,19 @@
 
 For a detailed explanation of each setting, refer to the `.env.example` file provided in the repository.
 
 ## API Endpoints
 
 AGiXT provides several API endpoints for managing agents, prompts and chains.
 
+If you're not running with Docker, the back end can be run with:
+```
+python src/agixt/app.py
+```
+
 To learn more about the API endpoints and their usage, visit the API documentation at 
 - [Swagger](http://localhost:7437)
 - [Redoc](http://localhost:7437/redoc)
 
 This documentation is hosted locally and the frontend must be running for these links to work.
 
 ## Extending Functionality
```

### Comparing `agixt-1.1.47b0/setup.py` & `agixt-1.1.48b0/setup.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.47b0/src/agixt/AGiXT.py` & `agixt-1.1.48b0/src/agixt/AGiXT.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,17 +98,20 @@
         if prompt == "":
             prompt = task
         else:
             prompt = cp.get_prompt(prompt_name=prompt, model=self.CFG.AI_MODEL)
         if top_results == 0:
             context = "None"
         else:
-            context = self.memories.context_agent(
-                query=task, top_results_num=top_results
-            )
+            try:
+                context = self.memories.context_agent(
+                    query=task, top_results_num=top_results
+                )
+            except:
+                context = "None."
         command_list = self.get_commands_string()
         formatted_prompt = self.custom_format(
             prompt,
             task=task,
             agent_name=self.agent_name,
             COMMANDS=command_list,
             context=context,
```

### Comparing `agixt-1.1.47b0/src/agixt/Chain.py` & `agixt-1.1.48b0/src/agixt/Chain.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.47b0/src/agixt/Commands.py` & `agixt-1.1.48b0/src/agixt/Commands.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.47b0/src/agixt/Config/Agent.py` & `agixt-1.1.48b0/src/agixt/Config/Agent.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.47b0/src/agixt/Config/__init__.py` & `agixt-1.1.48b0/src/agixt/Config/__init__.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.47b0/src/agixt/CustomPrompt.py` & `agixt-1.1.48b0/src/agixt/CustomPrompt.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.47b0/src/agixt/Embedding.py` & `agixt-1.1.48b0/src/agixt/Embedding.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.47b0/src/agixt/Memories.py` & `agixt-1.1.48b0/src/agixt/Memories.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,16 @@
             )
         except Exception as e:
             print(f"Failed to store memory: {e}")
 
     def store_result(self, task_name: str, result: str):
         if result:
             timestamp = datetime.now()  # current time as datetime object
+            if not isinstance(result, str):
+                result = str(result)
             chunks = self.chunk_content(result, task_name)
             for chunk in chunks:
                 result_id = self.generate_id(chunk, timestamp.isoformat())
                 self.store_memory(
                     result_id,
                     chunk,
                     {
```

### Comparing `agixt-1.1.47b0/src/agixt/app.py` & `agixt-1.1.48b0/src/agixt/app.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.47b0/src/agixt/provider/__init__.py` & `agixt-1.1.48b0/src/agixt/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.47b0/src/agixt/provider/azure.py` & `agixt-1.1.48b0/src/agixt/provider/azure.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.47b0/src/agixt/provider/bing.py` & `agixt-1.1.48b0/src/agixt/provider/bing.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.47b0/src/agixt/provider/fastchat.py` & `agixt-1.1.48b0/src/agixt/provider/fastchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.47b0/src/agixt/provider/gpt4all.py` & `agixt-1.1.48b0/src/agixt/provider/gpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.47b0/src/agixt/provider/gpt4free.py` & `agixt-1.1.48b0/src/agixt/provider/gpt4free.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import gpt4free
 import time
-import itertools
 
 
 class Gpt4freeProvider:
     def __init__(
         self,
         AI_MODEL: str = "gpt-4",
         AI_TEMPERATURE: float = 0.7,
@@ -12,39 +11,50 @@
         **kwargs,
     ):
         self.requirements = ["gpt4free"]
         self.AI_MODEL = AI_MODEL
         self.AI_TEMPERATURE = AI_TEMPERATURE
         self.MAX_TOKENS = MAX_TOKENS
         self.FAILED_PROVIDERS = []
-        self.providers = itertools.cycle(["DeepAI", "Useless", "You"])
+        self.providers = gpt4free.Provider._member_names_
+        self.providers.sort()
 
     def instruct(self, prompt, tokens: int = 0):
-        provider = next(self.providers)
-        try:
-            if provider not in self.FAILED_PROVIDERS:
-                response = gpt4free.Completion.create(
-                    getattr(gpt4free.Provider, provider),
-                    prompt=prompt,
-                )
-                if "text" in response:
-                    response = response["text"]
-                if "status" in response and response["status"] == "Fail":
-                    self.FAILED_PROVIDERS.append(provider)
-                    print(f"Failed to use {provider}")
-                    response = self.instruct(prompt, tokens)
-                if response == "Unable to fetch the response, Please try again.":
-                    self.FAILED_PROVIDERS.append(provider)
-                    print(f"Failed to use {provider}")
-                    response = self.instruct(prompt, tokens)
-            return response
-        except:
-            print(f"Failed to use {provider}")
-            self.FAILED_PROVIDERS.append(provider)
-            if (
-                len(self.FAILED_PROVIDERS) == 3
-            ):  # adjust this value to the number of your providers
+        final_response = None
+        while final_response is None:
+            for provider in self.providers:
+                if provider not in self.FAILED_PROVIDERS:
+                    try:
+                        response = gpt4free.Completion.create(
+                            getattr(gpt4free.Provider, provider),
+                            prompt=prompt,
+                        )
+                        if "text" in response:
+                            final_response = response["text"]
+                        if "status" in response and response["status"] == "Fail":
+                            self.FAILED_PROVIDERS.append(provider)
+                            print(f"Failed to use {provider}")
+                            final_response = None
+                        elif (
+                            response
+                            == "Unable to fetch the response, Please try again."
+                        ):
+                            self.FAILED_PROVIDERS.append(provider)
+                            print(f"Failed to use {provider}")
+                            final_response = None
+                        else:
+                            final_response = response
+                    except:
+                        print(f"Failed to use {provider}")
+                        self.FAILED_PROVIDERS.append(provider)
+                        final_response = None
+
+                if final_response:
+                    if len(final_response) > 1:
+                        return final_response
+
+            if len(self.FAILED_PROVIDERS) == len(self.providers):
                 self.FAILED_PROVIDERS = []
-                print("All providers failed, trying again in 10 seconds")
+                print(
+                    "All providers failed, sleeping for 10 seconds before trying again..."
+                )
                 time.sleep(10)
-            response = self.instruct(prompt, tokens)
-            return response
```

### Comparing `agixt-1.1.47b0/src/agixt/provider/gpugpt4all.py` & `agixt-1.1.48b0/src/agixt/provider/gpugpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.47b0/src/agixt/provider/huggingchat.py` & `agixt-1.1.48b0/src/agixt/provider/huggingchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.47b0/src/agixt/provider/kobold.py` & `agixt-1.1.48b0/src/agixt/provider/kobold.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.47b0/src/agixt/provider/llamacpp.py` & `agixt-1.1.48b0/src/agixt/provider/llamacpp.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.47b0/src/agixt/provider/oobabooga.py` & `agixt-1.1.48b0/src/agixt/provider/oobabooga.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.47b0/src/agixt/provider/openai.py` & `agixt-1.1.48b0/src/agixt/provider/openai.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.47b0/src/agixt/provider/palm.py` & `agixt-1.1.48b0/src/agixt/provider/palm.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.47b0/src/agixt/provider/transformer.py` & `agixt-1.1.48b0/src/agixt/provider/transformer.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.47b0/src/agixt/requirements.txt` & `agixt-1.1.48b0/src/agixt/requirements.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.47b0/src/agixt/smartchat.py` & `agixt-1.1.48b0/src/agixt/smartchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.47b0/src/agixt/smartinstruct.py` & `agixt-1.1.48b0/src/agixt/smartinstruct.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.47b0/src/agixt.egg-info/PKG-INFO` & `agixt-1.1.48b0/src/agixt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.1.47b0
+Version: 1.1.48b0
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # AGiXT
-
 ![RELEASE](https://img.shields.io/github/v/release/Josh-XT/AGiXT?label=Release%20Version&style=plastic) 
 [![STATUS](https://img.shields.io/badge/status-beta-blue?label=Release%20Status&style=plastic)](https://github.com/josh-xt/AGiXT) 
 [![LICENSE: MIT](https://img.shields.io/github/license/Josh-XT/AGiXT?label=License&style=plastic)](https://github.com/Josh-XT/AGiXT/blob/main/LICENSE) 
 ![DOCKER](https://img.shields.io/github/actions/workflow/status/Josh-XT/AGiXT/publish-docker.yml?branch=main&label=Docker&style=plastic) [![CODESTYLE](https://img.shields.io/badge/code%20style-Black-black?branch=main&label=Code%20Style&style=plastic)](https://black.readthedocs.io/en/stable/the_black_code_style/index.html)
 
 [![GitHub](https://img.shields.io/badge/GitHub-Frontend_Repository-grey?logo=github&style=plastic)](https://github.com/JamesonRGrieve/Agent-LLM-Frontend)
 
 [![Contribute](https://img.shields.io/github/issues/Josh-XT/AGiXT/help%20wanted?color=purple&label=Quick%20Contribute%20Backend&logo=github&style=plastic)](https://github.com/Josh-XT/AGiXT/labels/help%20wanted) 
 [![Contribute](https://img.shields.io/github/issues/JamesonRGrieve/Agent-LLM-Frontend/help%20wanted?color=purple&label=Quick%20Contribute%20Frontend&logo=github&style=plastic)](https://github.com/JamesonRGrieve/Agent-LLM-Frontend/labels/help%20wanted) 
 [![Discord](https://img.shields.io/discord/1097720481970397356?label=Discord&logo=discord&logoColor=white&style=plastic&color=5865f2)](https://discord.gg/d3TkHRZcjD) 
 [![Twitter](https://img.shields.io/badge/Twitter-Follow_@AGi_XT-blue?logo=twitter&style=plastic)](https://twitter.com/AGi_XT) 
 [![EMail](https://img.shields.io/badge/E--Mail-Outreach_&_Media-5865f2?logo=gmail&style=plastic)](https://twitter.com/AGi_XT) 
 
+![Logo](AGiXT.svg)
+
 Please use the outreach email for media, sponsorship, or to contact us for other miscellaneous purposes. 
 
 **Do not** send us emails with troubleshooting requests, feature requests or bug reports, please direct those to [GitHub Issues](https://github.com/Josh-XT/AGiXT/issues) or [Discord](https://discord.gg/d3TkHRZcjD).
 
 AGiXT is an Artificial Intelligence Automation Platform designed to power efficient AI instruction management across multiple providers. Our agents are equipped with adaptive memory, and this versatile solution offers a powerful plugin system that supports a wide range of commands, including web browsing. With growing support for numerous AI providers and models, AGiXT is constantly evolving to empower diverse applications.
 
-![image](https://user-images.githubusercontent.com/102809327/234344654-a1a4201b-594b-4a00-ac78-279a2e5bbe43.png)
-
-![image](https://user-images.githubusercontent.com/102809327/235532233-72f291a7-0633-435f-b72c-7f56bce682d8.png)
 
 ## ⚠️ Run this in Docker or a Virtual Machine!
 You're welcome to disregard this message, but if you do and the AI decides that the best course of action for its task is to build a command to format your entire computer, that is on you.  Understand that this is given full unrestricted terminal access by design and that we have no intentions of building any safeguards.  This project intends to stay light weight and versatile for the best possible research outcomes.
 
 See also [SECURITY.md](1-Getting started/SECURITY.MD)
 
 ## ⚠️ Monitor Your Usage!
@@ -87,16 +85,15 @@
   - [Key Features 🗝️](#key-features-️)
   - [Web Application Features](#web-application-features)
   - [Run with Docker](#run-with-docker)
     - [Linux or Windows](#linux-or-windows)
     - [Windows Docker Desktop (streamlit only example)](#windows-docker-desktop-streamlit-only-example)
     - [Development using docker](#development-using-docker)
   - [Manual Install from source (unsupported)](#manual-install-from-source-unsupported)
-    - [Back End](#back-end)
-    - [Front End](#front-end)
+    - [Streamlit App Locally](#streamlit-app-locally)
   - [Configuration](#configuration)
   - [API Endpoints](#api-endpoints)
   - [Extending Functionality](#extending-functionality)
     - [Updating Requirements](#updating-requirements)
     - [Commands](#commands)
     - [AI Providers](#ai-providers)
   - [Documentation](#documentation)
@@ -163,53 +160,41 @@
 Run all available services
 `docker compose --profile all up`
 
 - AGiXT-frontend http://localhost:3000
 - streamlit-UI http://localhost:8501
 
 ### Windows Docker Desktop (streamlit only example)
-
-![On Windows Docker Desktop](Docker-desktop-win-setting-streamlit.png)
-
+- Container Name: AGiXT
+- Host Port: 8501:8501/tcp
 
 ### Development using docker
 ```
 docker compose --profile all -f docker-compose.yml -f docker-compose.dev.yaml up
 ```
 
 * mounts dev space into container - happy building 
 
 
 ## Manual Install from source (unsupported)
 
 As a reminder, this can be dangerous to run locally depending on what commands you give your agents access to.  [⚠️ Run this in Docker or a Virtual Machine!](#️-run-this-in-docker-or-a-virtual-machine)
 
-### Back End
+### Streamlit App Locally
 
 Clone the repository for the AGiXT back end and start it.
 
 ```
 git clone https://github.com/Josh-XT/AGiXT
 cd AGiXT/src/agixt
 pip install -r requirements.txt
-python app.py
+streamlit run streamlit.py
 ```
 
-### Front End
-
-Clone the repository for the AGiXT front end in a separate terminal and start it.
-
-```
-git clone https://github.com/JamesonRGrieve/Agent-LLM-Frontend --recurse-submodules 
-cd Agent-LLM-Frontend
-yarn install
-yarn dev
-```
-
-Access the web interface at http://localhost:3000
+Access the web interface at http://localhost:8501
 
 ## Configuration
 
 AGiXT utilizes a `.env` configuration file to store AI language model settings, API keys, and other options. Use the supplied `.env.example` as a template to create your personalized `.env` file. Configuration settings include:
 
 - **WORKING_DIRECTORY**: Set the agent's working directory.
 - **EXTENSIONS_SETTINGS**: Configure settings for OpenAI, Hugging Face, Selenium, Twitter, and GitHub.
@@ -217,14 +202,19 @@
 
 For a detailed explanation of each setting, refer to the `.env.example` file provided in the repository.
 
 ## API Endpoints
 
 AGiXT provides several API endpoints for managing agents, prompts and chains.
 
+If you're not running with Docker, the back end can be run with:
+```
+python src/agixt/app.py
+```
+
 To learn more about the API endpoints and their usage, visit the API documentation at 
 - [Swagger](http://localhost:7437)
 - [Redoc](http://localhost:7437/redoc)
 
 This documentation is hosted locally and the frontend must be running for these links to work.
 
 ## Extending Functionality
```

### Comparing `agixt-1.1.47b0/src/agixt.egg-info/SOURCES.txt` & `agixt-1.1.48b0/src/agixt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.47b0/src/agixt.egg-info/requires.txt` & `agixt-1.1.48b0/src/agixt.egg-info/requires.txt`

 * *Files identical despite different names*

