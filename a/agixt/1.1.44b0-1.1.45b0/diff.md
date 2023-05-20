# Comparing `tmp/agixt-1.1.44b0.tar.gz` & `tmp/agixt-1.1.45b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agixt-1.1.44b0.tar", last modified: Sat May 20 02:53:46 2023, max compression
+gzip compressed data, was "agixt-1.1.45b0.tar", last modified: Sat May 20 03:11:50 2023, max compression
```

## Comparing `agixt-1.1.44b0.tar` & `agixt-1.1.45b0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 02:53:46.896667 agixt-1.1.44b0/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-20 02:53:32.000000 agixt-1.1.44b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-20 02:53:32.000000 agixt-1.1.44b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    19140 2023-05-20 02:53:46.896667 agixt-1.1.44b0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 02:53:46.892667 agixt-1.1.44b0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    18683 2023-05-20 02:53:32.000000 agixt-1.1.44b0/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-20 02:53:32.000000 agixt-1.1.44b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 02:53:46.896667 agixt-1.1.44b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-20 02:53:32.000000 agixt-1.1.44b0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 02:53:46.892667 agixt-1.1.44b0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 02:53:46.892667 agixt-1.1.44b0/src/agixt/
--rw-r--r--   0 runner    (1001) docker     (123)    25128 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/AGiXT.py
--rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/Chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/Commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 02:53:46.896667 agixt-1.1.44b0/src/agixt/Config/
--rw-r--r--   0 runner    (1001) docker     (123)    13352 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/Config/Agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/Config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/CustomPrompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/Embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/Memories.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13588 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/app.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 02:53:46.896667 agixt-1.1.44b0/src/agixt/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/provider/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/provider/bard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/provider/bing.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/provider/fastchat.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/provider/gpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/provider/gpt4free.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/provider/gpugpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/provider/huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/provider/kobold.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/provider/llamacpp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/provider/oobabooga.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/provider/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/provider/palm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/provider/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/smartchat.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/smartinstruct.py
--rw-r--r--   0 runner    (1001) docker     (123)    33053 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/streamlit.py
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-20 02:53:32.000000 agixt-1.1.44b0/src/agixt/version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 02:53:46.896667 agixt-1.1.44b0/src/agixt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19140 2023-05-20 02:53:46.000000 agixt-1.1.44b0/src/agixt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-20 02:53:46.000000 agixt-1.1.44b0/src/agixt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 02:53:46.000000 agixt-1.1.44b0/src/agixt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-20 02:53:46.000000 agixt-1.1.44b0/src/agixt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-20 02:53:46.000000 agixt-1.1.44b0/src/agixt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:11:50.547690 agixt-1.1.45b0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-20 03:11:36.000000 agixt-1.1.45b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-20 03:11:36.000000 agixt-1.1.45b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    19140 2023-05-20 03:11:50.547690 agixt-1.1.45b0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:11:50.539690 agixt-1.1.45b0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    18683 2023-05-20 03:11:36.000000 agixt-1.1.45b0/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-20 03:11:36.000000 agixt-1.1.45b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 03:11:50.547690 agixt-1.1.45b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-20 03:11:36.000000 agixt-1.1.45b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:11:50.539690 agixt-1.1.45b0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:11:50.543690 agixt-1.1.45b0/src/agixt/
+-rw-r--r--   0 runner    (1001) docker     (123)    25091 2023-05-20 03:11:36.000000 agixt-1.1.45b0/src/agixt/AGiXT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-05-20 03:11:36.000000 agixt-1.1.45b0/src/agixt/Chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-05-20 03:11:36.000000 agixt-1.1.45b0/src/agixt/Commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:11:50.543690 agixt-1.1.45b0/src/agixt/Config/
+-rw-r--r--   0 runner    (1001) docker     (123)    13352 2023-05-20 03:11:36.000000 agixt-1.1.45b0/src/agixt/Config/Agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-20 03:11:36.000000 agixt-1.1.45b0/src/agixt/Config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-20 03:11:36.000000 agixt-1.1.45b0/src/agixt/CustomPrompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-05-20 03:11:36.000000 agixt-1.1.45b0/src/agixt/Embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-05-20 03:11:36.000000 agixt-1.1.45b0/src/agixt/Memories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-20 03:11:36.000000 agixt-1.1.45b0/src/agixt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13588 2023-05-20 03:11:36.000000 agixt-1.1.45b0/src/agixt/app.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-05-20 03:11:36.000000 agixt-1.1.45b0/src/agixt/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:11:50.547690 agixt-1.1.45b0/src/agixt/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-20 03:11:36.000000 agixt-1.1.45b0/src/agixt/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-20 03:11:36.000000 agixt-1.1.45b0/src/agixt/provider/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-20 03:11:36.000000 agixt-1.1.45b0/src/agixt/provider/bard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-20 03:11:36.000000 agixt-1.1.45b0/src/agixt/provider/bing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-20 03:11:36.000000 agixt-1.1.45b0/src/agixt/provider/fastchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-20 03:11:36.000000 agixt-1.1.45b0/src/agixt/provider/gpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-20 03:11:36.000000 agixt-1.1.45b0/src/agixt/provider/gpt4free.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-20 03:11:36.000000 agixt-1.1.45b0/src/agixt/provider/gpugpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-20 03:11:36.000000 agixt-1.1.45b0/src/agixt/provider/huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-20 03:11:36.000000 agixt-1.1.45b0/src/agixt/provider/kobold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-20 03:11:36.000000 agixt-1.1.45b0/src/agixt/provider/llamacpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-20 03:11:36.000000 agixt-1.1.45b0/src/agixt/provider/oobabooga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-20 03:11:36.000000 agixt-1.1.45b0/src/agixt/provider/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-20 03:11:36.000000 agixt-1.1.45b0/src/agixt/provider/palm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-20 03:11:36.000000 agixt-1.1.45b0/src/agixt/provider/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-20 03:11:36.000000 agixt-1.1.45b0/src/agixt/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-20 03:11:36.000000 agixt-1.1.45b0/src/agixt/smartchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-20 03:11:36.000000 agixt-1.1.45b0/src/agixt/smartinstruct.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33053 2023-05-20 03:11:36.000000 agixt-1.1.45b0/src/agixt/streamlit.py
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-20 03:11:36.000000 agixt-1.1.45b0/src/agixt/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:11:50.543690 agixt-1.1.45b0/src/agixt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19140 2023-05-20 03:11:50.000000 agixt-1.1.45b0/src/agixt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-20 03:11:50.000000 agixt-1.1.45b0/src/agixt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 03:11:50.000000 agixt-1.1.45b0/src/agixt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-20 03:11:50.000000 agixt-1.1.45b0/src/agixt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-20 03:11:50.000000 agixt-1.1.45b0/src/agixt.egg-info/top_level.txt
```

### Comparing `agixt-1.1.44b0/LICENSE` & `agixt-1.1.45b0/LICENSE`

 * *Files identical despite different names*

### Comparing `agixt-1.1.44b0/PKG-INFO` & `agixt-1.1.45b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.1.44b0
+Version: 1.1.45b0
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `agixt-1.1.44b0/docs/README.md` & `agixt-1.1.45b0/docs/README.md`

 * *Files identical despite different names*

### Comparing `agixt-1.1.44b0/setup.py` & `agixt-1.1.45b0/setup.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.44b0/src/agixt/AGiXT.py` & `agixt-1.1.45b0/src/agixt/AGiXT.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,18 +22,18 @@
 def run_asyncio_coroutine(coro):
     loop = asyncio.new_event_loop()
     asyncio.set_event_loop(loop)
     return loop.run_until_complete(coro)
 
 
 class AGiXT:
-    def __init__(self, agent_name: str = "AGiXT", primary_objective=None):
+    def __init__(self, agent_name: str = "AGiXT"):
         self.agent_name = agent_name
         self.CFG = Agent(self.agent_name)
-        self.primary_objective = primary_objective
+        self.primary_objective = None
         self.task_list = deque([])
         self.commands = Commands(self.agent_name)
         self.available_commands = self.commands.get_available_commands()
         self.agent_config = self.CFG.load_agent_config(self.agent_name)
         self.output_list = []
         self.memories = Memories(self.agent_name, self.CFG)
         self.stop_running_event = None
```

### Comparing `agixt-1.1.44b0/src/agixt/Chain.py` & `agixt-1.1.45b0/src/agixt/Chain.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import json
-from . import AGiXT
+from AGiXT import AGiXT
 import argparse
-from . import CustomPrompt
-from . import Commands
+from CustomPrompt import CustomPrompt
+from Commands import Commands
 
 
 class Chain:
     def get_chain(self, chain_name):
         with open(os.path.join("chains", f"{chain_name}.json"), "r") as f:
             chain_data = json.load(f)
         return chain_data
@@ -86,44 +86,41 @@
     def run_chain_step(self, step):
         if step:
             if "prompt_type" in step:
                 prompt_type = step["prompt_type"]
                 prompt = step["prompt"]
                 agent_name = step["agent_name"]
                 try:
-                    prompt_name = prompt["prompt_name"]
-                    prompt = {k: v for k, v in prompt.items() if k != "prompt_name"}
-                    prompt_content = CustomPrompt().get_prompt(prompt_name)
-                except:
-                    prompt_name = ""
-                try:
                     command_name = prompt["command_name"]
                     prompt = {k: v for k, v in prompt.items() if k != "command_name"}
                 except:
                     command_name = ""
+                if prompt_type == "Command":
+                    return Commands(agent_name=agent_name).execute_command(
+                        command_name, prompt
+                    )
+                try:
+                    prompt_name = prompt["prompt_name"]
+                    prompt = {k: v for k, v in prompt.items() if k != "prompt_name"}
+                    prompt_content = CustomPrompt().get_prompt(prompt_name)
+                    agent = AGiXT(agent_name)
+                except:
+                    return None
                 if prompt_type == "Prompt":
-                    result = AGiXT(agent_name).run(
+                    result = agent.run(
                         task=prompt_content, prompt=prompt_name, **prompt
                     )
-                elif prompt_type == "Command":
-                    result = Commands(agent_name=agent_name).execute_command(
-                        command_name, prompt
-                    )
                 elif prompt_type == "Chain":
                     result = self.run_chain(prompt["chain_name"])
                 elif prompt_type == "Smart Instruct":
-                    result = AGiXT(agent_name).smart_instruct(
-                        task=prompt_content, **prompt
-                    )
+                    result = agent.smart_instruct(task=prompt_content, **prompt)
                 elif prompt_type == "Smart Chat":
-                    result = AGiXT(agent_name).smart_chat(task=prompt_content, **prompt)
+                    result = agent.smart_chat(task=prompt_content, **prompt)
                 elif prompt_type == "Task":
-                    result = AGiXT(
-                        agent_name, primary_objective=prompt_content
-                    ).run_task(objective=prompt_content, **prompt)
+                    result = agent.run_task(objective=prompt_content, **prompt)
         if result:
             return result
         else:
             return None
 
 
 if __name__ == "__main__":
```

### Comparing `agixt-1.1.44b0/src/agixt/Commands.py` & `agixt-1.1.45b0/src/agixt/Commands.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.44b0/src/agixt/Config/Agent.py` & `agixt-1.1.45b0/src/agixt/Config/Agent.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.44b0/src/agixt/Config/__init__.py` & `agixt-1.1.45b0/src/agixt/Config/__init__.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.44b0/src/agixt/CustomPrompt.py` & `agixt-1.1.45b0/src/agixt/CustomPrompt.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.44b0/src/agixt/Embedding.py` & `agixt-1.1.45b0/src/agixt/Embedding.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.44b0/src/agixt/Memories.py` & `agixt-1.1.45b0/src/agixt/Memories.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.44b0/src/agixt/app.py` & `agixt-1.1.45b0/src/agixt/app.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.44b0/src/agixt/provider/__init__.py` & `agixt-1.1.45b0/src/agixt/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.44b0/src/agixt/provider/azure.py` & `agixt-1.1.45b0/src/agixt/provider/azure.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.44b0/src/agixt/provider/bing.py` & `agixt-1.1.45b0/src/agixt/provider/bing.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.44b0/src/agixt/provider/fastchat.py` & `agixt-1.1.45b0/src/agixt/provider/fastchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.44b0/src/agixt/provider/gpt4all.py` & `agixt-1.1.45b0/src/agixt/provider/gpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.44b0/src/agixt/provider/gpt4free.py` & `agixt-1.1.45b0/src/agixt/provider/gpt4free.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.44b0/src/agixt/provider/gpugpt4all.py` & `agixt-1.1.45b0/src/agixt/provider/gpugpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.44b0/src/agixt/provider/huggingchat.py` & `agixt-1.1.45b0/src/agixt/provider/huggingchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.44b0/src/agixt/provider/kobold.py` & `agixt-1.1.45b0/src/agixt/provider/kobold.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.44b0/src/agixt/provider/llamacpp.py` & `agixt-1.1.45b0/src/agixt/provider/llamacpp.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.44b0/src/agixt/provider/oobabooga.py` & `agixt-1.1.45b0/src/agixt/provider/oobabooga.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.44b0/src/agixt/provider/openai.py` & `agixt-1.1.45b0/src/agixt/provider/openai.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.44b0/src/agixt/provider/palm.py` & `agixt-1.1.45b0/src/agixt/provider/palm.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.44b0/src/agixt/provider/transformer.py` & `agixt-1.1.45b0/src/agixt/provider/transformer.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.44b0/src/agixt/requirements.txt` & `agixt-1.1.45b0/src/agixt/requirements.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.44b0/src/agixt/smartchat.py` & `agixt-1.1.45b0/src/agixt/smartchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.44b0/src/agixt/smartinstruct.py` & `agixt-1.1.45b0/src/agixt/smartinstruct.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.44b0/src/agixt/streamlit.py` & `agixt-1.1.45b0/src/agixt/streamlit.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.44b0/src/agixt.egg-info/PKG-INFO` & `agixt-1.1.45b0/src/agixt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.1.44b0
+Version: 1.1.45b0
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `agixt-1.1.44b0/src/agixt.egg-info/SOURCES.txt` & `agixt-1.1.45b0/src/agixt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.44b0/src/agixt.egg-info/requires.txt` & `agixt-1.1.45b0/src/agixt.egg-info/requires.txt`

 * *Files identical despite different names*

