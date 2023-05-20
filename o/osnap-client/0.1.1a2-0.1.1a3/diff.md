# Comparing `tmp/osnap_client-0.1.1a2.tar.gz` & `tmp/osnap_client-0.1.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osnap_client-0.1.1a2.tar", max compression
+gzip compressed data, was "osnap_client-0.1.1a3.tar", max compression
```

## Comparing `osnap_client-0.1.1a2.tar` & `osnap_client-0.1.1a3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    11357 2023-05-17 08:21:07.375494 osnap_client-0.1.1a2/LICENSE
--rw-r--r--   0        0        0     2487 2023-05-17 08:21:07.375494 osnap_client-0.1.1a2/README.md
--rw-r--r--   0        0        0      214 2023-05-17 08:21:07.415495 osnap_client-0.1.1a2/osnap_client/__init__.py
--rw-r--r--   0        0        0     1759 2023-05-17 08:21:07.415495 osnap_client-0.1.1a2/osnap_client/adapters/AdapterBase.py
--rw-r--r--   0        0        0     4525 2023-05-17 08:21:07.415495 osnap_client-0.1.1a2/osnap_client/adapters/DiscordAdapter.py
--rw-r--r--   0        0        0      190 2023-05-17 08:21:07.415495 osnap_client-0.1.1a2/osnap_client/adapters/QueueTaskStruct.py
--rw-r--r--   0        0        0       79 2023-05-17 08:21:07.415495 osnap_client-0.1.1a2/osnap_client/adapters/__init__.py
--rw-r--r--   0        0        0     3681 2023-05-17 08:21:07.415495 osnap_client-0.1.1a2/osnap_client/agents/SwarmAgentBase.py
--rw-r--r--   0        0        0       42 2023-05-17 08:21:07.415495 osnap_client-0.1.1a2/osnap_client/agents/__init__.py
--rw-r--r--   0        0        0      199 2023-05-17 08:21:07.415495 osnap_client-0.1.1a2/osnap_client/core/__init__.py
--rw-r--r--   0        0        0     5934 2023-05-17 08:21:07.415495 osnap_client-0.1.1a2/osnap_client/core/agent.py
--rw-r--r--   0        0        0     1419 2023-05-17 08:21:07.415495 osnap_client-0.1.1a2/osnap_client/core/api.py
--rw-r--r--   0        0        0     1314 2023-05-17 08:21:07.415495 osnap_client-0.1.1a2/osnap_client/core/crypt.py
--rw-r--r--   0        0        0     6296 2023-05-17 08:21:07.415495 osnap_client-0.1.1a2/osnap_client/core/osnap.py
--rw-r--r--   0        0        0       46 2023-05-17 08:21:07.415495 osnap_client-0.1.1a2/osnap_client/pubsub/__init__.py
--rw-r--r--   0        0        0     2666 2023-05-17 08:21:07.415495 osnap_client-0.1.1a2/osnap_client/pubsub/pubsub.py
--rw-r--r--   0        0        0       98 2023-05-17 08:21:07.415495 osnap_client-0.1.1a2/osnap_client/registry/__init__.py
--rw-r--r--   0        0        0     3149 2023-05-17 08:21:07.415495 osnap_client-0.1.1a2/osnap_client/registry/agent_registry.py
--rw-r--r--   0        0        0        0 2023-05-17 08:21:07.415495 osnap_client-0.1.1a2/osnap_client/registry/registry.py
--rw-r--r--   0        0        0     1813 2023-05-17 08:21:07.415495 osnap_client-0.1.1a2/osnap_client/registry/tool_registry.py
--rw-r--r--   0        0        0        0 2023-05-17 08:21:07.415495 osnap_client-0.1.1a2/osnap_client/tools/__init__.py
--rw-r--r--   0        0        0        0 2023-05-17 08:21:07.415495 osnap_client-0.1.1a2/osnap_client/tools/main.py
--rw-r--r--   0        0        0     2449 2023-05-17 08:21:07.415495 osnap_client-0.1.1a2/osnap_client/utils/ai_engines/EngineBase.py
--rw-r--r--   0        0        0     2846 2023-05-17 08:21:07.415495 osnap_client-0.1.1a2/osnap_client/utils/ai_engines/GPTConversEngine.py
--rw-r--r--   0        0        0     2972 2023-05-17 08:21:07.415495 osnap_client-0.1.1a2/osnap_client/utils/ai_engines/LanchainGoogleEngine.py
--rw-r--r--   0        0        0      136 2023-05-17 08:21:07.415495 osnap_client-0.1.1a2/osnap_client/utils/ai_engines/__init__.py
--rw-r--r--   0        0        0     1220 2023-05-17 08:21:07.415495 osnap_client-0.1.1a2/pyproject.toml
--rw-r--r--   0        0        0     3580 1970-01-01 00:00:00.000000 osnap_client-0.1.1a2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-20 16:00:46.197570 osnap_client-0.1.1a3/LICENSE
+-rw-r--r--   0        0        0     2555 2023-05-20 16:00:46.197570 osnap_client-0.1.1a3/README.md
+-rw-r--r--   0        0        0        0 2023-05-20 16:00:46.245571 osnap_client-0.1.1a3/osnap_client/__init__.py
+-rw-r--r--   0        0        0       91 2023-05-20 16:00:46.245571 osnap_client-0.1.1a3/osnap_client/adapters/__init__.py
+-rw-r--r--   0        0        0     1868 2023-05-20 16:00:46.245571 osnap_client-0.1.1a3/osnap_client/adapters/base.py
+-rw-r--r--   0        0        0     4470 2023-05-20 16:00:46.245571 osnap_client-0.1.1a3/osnap_client/adapters/discord_adapter.py
+-rw-r--r--   0        0        0      387 2023-05-20 16:00:46.245571 osnap_client-0.1.1a3/osnap_client/agents/__init__.py
+-rw-r--r--   0        0        0      274 2023-05-20 16:00:46.245571 osnap_client-0.1.1a3/osnap_client/agents/agent_info.py
+-rw-r--r--   0        0        0     3186 2023-05-20 16:00:46.245571 osnap_client-0.1.1a3/osnap_client/agents/base.py
+-rw-r--r--   0        0        0     3696 2023-05-20 16:00:46.245571 osnap_client-0.1.1a3/osnap_client/agents/swarm_agent.py
+-rw-r--r--   0        0        0      158 2023-05-20 16:00:46.245571 osnap_client-0.1.1a3/osnap_client/core/__init__.py
+-rw-r--r--   0        0        0     1419 2023-05-20 16:00:46.245571 osnap_client-0.1.1a3/osnap_client/core/api.py
+-rw-r--r--   0        0        0     1314 2023-05-20 16:00:46.245571 osnap_client-0.1.1a3/osnap_client/core/crypt.py
+-rw-r--r--   0        0        0     6296 2023-05-20 16:00:46.245571 osnap_client-0.1.1a3/osnap_client/core/osnap.py
+-rw-r--r--   0        0        0       46 2023-05-20 16:00:46.245571 osnap_client-0.1.1a3/osnap_client/pubsub/__init__.py
+-rw-r--r--   0        0        0     2725 2023-05-20 16:00:46.245571 osnap_client-0.1.1a3/osnap_client/pubsub/pubsub.py
+-rw-r--r--   0        0        0      117 2023-05-20 16:00:46.245571 osnap_client-0.1.1a3/osnap_client/registry/__init__.py
+-rw-r--r--   0        0        0     3162 2023-05-20 16:00:46.245571 osnap_client-0.1.1a3/osnap_client/registry/agent_registry.py
+-rw-r--r--   0        0        0      309 2023-05-20 16:00:46.245571 osnap_client-0.1.1a3/osnap_client/registry/registry.py
+-rw-r--r--   0        0        0     1825 2023-05-20 16:00:46.245571 osnap_client-0.1.1a3/osnap_client/registry/tool_registry.py
+-rw-r--r--   0        0        0        0 2023-05-20 16:00:46.245571 osnap_client-0.1.1a3/osnap_client/tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-20 16:00:46.245571 osnap_client-0.1.1a3/osnap_client/tools/main.py
+-rw-r--r--   0        0        0     2449 2023-05-20 16:00:46.245571 osnap_client-0.1.1a3/osnap_client/utils/ai_engines/EngineBase.py
+-rw-r--r--   0        0        0     3070 2023-05-20 16:00:46.245571 osnap_client-0.1.1a3/osnap_client/utils/ai_engines/GPTConversEngine.py
+-rw-r--r--   0        0        0     2972 2023-05-20 16:00:46.245571 osnap_client-0.1.1a3/osnap_client/utils/ai_engines/LanchainGoogleEngine.py
+-rw-r--r--   0        0        0      136 2023-05-20 16:00:46.245571 osnap_client-0.1.1a3/osnap_client/utils/ai_engines/__init__.py
+-rw-r--r--   0        0        0     1220 2023-05-20 16:00:46.249570 osnap_client-0.1.1a3/pyproject.toml
+-rw-r--r--   0        0        0     3648 1970-01-01 00:00:00.000000 osnap_client-0.1.1a3/PKG-INFO
```

### Comparing `osnap_client-0.1.1a2/LICENSE` & `osnap_client-0.1.1a3/LICENSE`

 * *Files identical despite different names*

### Comparing `osnap_client-0.1.1a2/README.md` & `osnap_client-0.1.1a3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # OSNAP
 
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![Python Version](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/)
 [![Discord Follow](https://dcbadge.vercel.app/api/server/seKVhCtcAJ?style=flat)](https://discord.gg/seKVhCtcAJ)
 
-The Open Swarm Network Agent Protocol (OSNAP) is a standardized toolkit for building AI agents that interact with each other. Currently, the development and implementation of interacting autonomous AI agents and swarms are highly fragmented, with different projects utilizing various custom-built protocols and communication methods. This lack of standardization can lead to difficulties. OSNAP aims to address these issues by providing a well-defined, standardized toolkit for building and interacting with autonomous AI agents and swarms.
-
 <p align="center">
   <img src="content/logo_midjourney.png" alt="Project logo" width="1080">
 </p>
 
+The Open Swarm Network Agent Protocol (OSNAP) is a standardized toolkit for building AI agents that interact with each other. Currently, the development and implementation of interacting autonomous AI agents and swarms are highly fragmented, with different projects utilizing various custom-built protocols and communication methods. This lack of standardization can lead to difficulties. OSNAP aims to address these issues by providing a well-defined, standardized toolkit for building and interacting with autonomous AI agents and swarms.
+
+
 ## Table of Contents
 - [How to use in your project](#how-to-use-in-your-project)
 - [Examples](#examples)
 - [Architecture Overview](#architecture-overview)
 - [Next-Ups](#next-ups)
 - [How to Contribute](#how-to-contribute)
 
@@ -37,14 +38,16 @@
 The communication is handleded via the DiscordAdapter and the only think you need to do is to implement the logic of the `SwarmAgentBase`.
 
 # Architecture overview
 <p align="center">
   <img src="content/architecture_diagram.png" alt="Project diagram" width="720">
 </p>
 
+## Docker Containers
+[To Example](examples/2_containers/README.md)
 
 # Next-ups
 - make adding new models as easy as possible, including custom deployed ones like llama
 - multi-key support for higher scalability
 
 
 # How to Contribute
```

### Comparing `osnap_client-0.1.1a2/osnap_client/adapters/AdapterBase.py` & `osnap_client-0.1.1a3/osnap_client/adapters/base.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,53 +1,59 @@
 from abc import ABC, abstractmethod
 import asyncio
-from osnap_client.adapters.QueueTaskStruct import QueueTaskStruct
+import functools
+
+from pydantic import BaseModel
+
+
+class QueueTaskStruct(BaseModel):
+    """QueueTaskStruct holds the callback function and the arguments to pass to it."""
+
+    command_type: str
+    data: str
+
 
 class AdapterBase(ABC):
-    """This class stores some basic properties that every adapter should implement.
-    """
+    """This class stores some basic properties that every adapter should implement."""
 
     def __init__(self) -> None:
         self.event_queue = asyncio.Queue()
 
     async def add_to_queue(self, task):
         if not isinstance(task, QueueTaskStruct):
-            raise TypeError(f"Expected a QueueTaskStruct to add to the event_queue, got {type(task)}")
+            raise TypeError(
+                f"Expected a QueueTaskStruct to add to the event_queue, got {type(task)}"
+            )
         await self.event_queue.put(task)
         print(f"Added {task} to the event_queue")
 
     @abstractmethod
     async def on_ready(self) -> QueueTaskStruct:
         """This method is called when the apter is loaded.
         The output is forwarded to the agent through the event queue.
         """
         raise NotImplementedError
-    
+
     @abstractmethod
     async def on_message(self, message: str) -> QueueTaskStruct:
-        """This method is called when the apter is loaded
-        """
+        """This method is called when the apter is loaded"""
         raise NotImplementedError
 
     @abstractmethod
     async def get_users(self):
-        """Returns the information about the users on the server
-        """
+        """Returns the information about the users on the server"""
         raise NotImplementedError
-    
+
     @abstractmethod
     async def send_message(self, message: str, target_channel: str):
-        """This method is called to send a message to a specific channel
-        """
+        """This method is called to send a message to a specific channel"""
         raise NotImplementedError
-    
+
     @abstractmethod
     async def send_dm(self, message: str, target_user: str):
-        """This method is called to send a message to a specific user
-        """
+        """This method is called to send a message to a specific user"""
         raise NotImplementedError
-    
+
     @abstractmethod
     async def start():
-        """This method is called to start the adapter
-        """
-        raise NotImplementedError
+        """This method is called to start the adapter"""
+        raise NotImplementedError
```

### Comparing `osnap_client-0.1.1a2/osnap_client/adapters/DiscordAdapter.py` & `osnap_client-0.1.1a3/osnap_client/adapters/discord_adapter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,48 +1,46 @@
 # discord_adapter.py
 import discord
-from osnap_client.adapters.AdapterBase import AdapterBase
-from osnap_client.adapters.QueueTaskStruct import QueueTaskStruct
+from .base import AdapterBase, QueueTaskStruct
 import asyncio
 
+
 class DiscordAdapter(AdapterBase):
     """This is an adapter that allows the agent to communicate with Discord and receive/send messages.
 
     Args:
     - intents_list (list[str]): A list of intents that the bot will listen to.
     - token (str): The token of the bot that is used to connect to Discord.
     """
-    
+
     def __init__(self, start_server: str, intents_list: list, token: str):
         super().__init__()
         intents = self._unpack_intents(intents_list)
 
         self.adapter_loop = asyncio.new_event_loop()
         self.client = discord.Client(loop=self.adapter_loop, intents=intents)
         self.token = token
         self.start_server_name = start_server
         self.guild = None
 
     async def on_ready(self):
-        """This method is called automatically by the discord library when the bot is ready to start working.
-        """
-        response = QueueTaskStruct(command_type='on_ready', data='')
+        """This method is called automatically by the discord library when the bot is ready to start working."""
+        response = QueueTaskStruct(command_type="on_ready", data="")
         await self.add_to_queue(response)
 
     async def on_message(self, message):
-        """This method is called automatically by the discord library when a message is received.
-        """
+        """This method is called automatically by the discord library when a message is received."""
         if message.author == self.client.user:
             return
-        
+
         message_content = message.content
-        
-        if message.content.startswith('$'):
-            command_name = message_content.split(' ')[0][1:]
-            command_data = ' '.join(message_content.split(' ')[1:])
+
+        if message.content.startswith("$"):
+            command_name = message_content.split(" ")[0][1:]
+            command_data = " ".join(message_content.split(" ")[1:])
             response = QueueTaskStruct(command_type=command_name, data=command_data)
             await self.add_to_queue(response)
 
     async def get_users(self):
         """Returns the information about the users on the server
         # About me is not available in the API: https://stackoverflow.com/questions/68654914/discord-py-get-user-about-me-section
         """
@@ -55,31 +53,37 @@
     async def send_message(self, message: str, target_channel="general"):
         """Sends a message to the specified channel"""
         if self.guild is None:
             self.guild = self._get_start_guild()
 
         # Find the channel by its name
         for channel in self.guild.channels:
-            if channel.name == target_channel and isinstance(channel, discord.TextChannel):
+            if channel.name == target_channel and isinstance(
+                channel, discord.TextChannel
+            ):
                 await channel.send(message)
                 print(f"Sent message {message} to channel {target_channel}")
                 return
 
-        raise ValueError(f"Could not find the channel {target_channel} in the list of channels: {self.guild.channels}.")
-    
+        raise ValueError(
+            f"Could not find the channel {target_channel} in the list of channels: {self.guild.channels}."
+        )
+
     async def send_dm(self, message: str, target_user: str):
         """Sends a direct message to the specified user"""
         if self.guild is None:
             self.guild = self._get_start_guild()
 
         for user in self.client.guild.members:
             if user.name == target_user:
                 await user.send(message)
-        
-        raise ValueError(f"Could not find the user {target_user} in the list of users: {self.guild.members}.")
+
+        raise ValueError(
+            f"Could not find the user {target_user} in the list of users: {self.guild.members}."
+        )
 
     def start(self):
         # adding the methods to the adapter
         self.client.event(self.on_ready)
         self.client.event(self.on_message)
         # need to launch the adapter loop
         self.adapter_loop.run_until_complete(self.client.start(self.token))
@@ -91,18 +95,18 @@
             if hasattr(intents_obj, intent):
                 setattr(intents_obj, intent, True)
             else:
                 raise ValueError(f"Invalid intent: {intent}")
         return intents_obj
 
     def _get_start_guild(self):
-        """In discord api the servers are called guilds.
-        """
+        """In discord api the servers are called guilds."""
         # Find the guild by its name
         target_guild = None
         for guild in self.client.guilds:
             if guild.name == self.start_server_name:
                 target_guild = guild
                 return target_guild
-        
-        raise ValueError(f"Could not find the guild {self.start_server_name} in the list of guilds: {self.client.guilds}. Make sure the bot is added to the server: https://discordpy.readthedocs.io/en/stable/discord.html")
-        
+
+        raise ValueError(
+            f"Could not find the guild {self.start_server_name} in the list of guilds: {self.client.guilds}. Make sure the bot is added to the server: https://discordpy.readthedocs.io/en/stable/discord.html"
+        )
```

### Comparing `osnap_client-0.1.1a2/osnap_client/agents/SwarmAgentBase.py` & `osnap_client-0.1.1a3/osnap_client/agents/swarm_agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,89 +1,97 @@
 from abc import ABC, abstractmethod
 import asyncio
 import time
 import threading
 
-from osnap_client.adapters.AdapterBase import AdapterBase
-from osnap_client.adapters.QueueTaskStruct import QueueTaskStruct
+from osnap_client.adapters import AdapterBase, QueueTaskStruct
+
 
 class SwarmAgentBase(ABC):
     """
     This is a base class that the user needs to implement to define the logic of the bot
     for request handling and sending.
     """
+
     def __init__(self, name: str, description: str, swarm_adapter: AdapterBase) -> None:
         super().__init__()
         self.name = name
         self.description = description
         self.swarm_adapter = swarm_adapter
         self.event_queue = swarm_adapter.event_queue
         self.command_map = {}
 
         # Register "ready" command
         self.command_map["on_ready"] = self.on_ready
-    
+
     def command(self, name: str):
         def decorator(func):
             self.command_map[name] = func
             return func
+
         return decorator
-    
+
     async def on_callback_event_listener(self):
         while True:
             task = None
             try:
                 task = self.event_queue.get_nowait()
             except asyncio.QueueEmpty:
                 time.sleep(0.5)
                 continue
             if not isinstance(task, QueueTaskStruct):
                 raise TypeError(f"Expected a QueueTaskStruct, got {type(task)}")
-            
+
             command = task.command_type
             data = task.data
 
             if command in self.command_map:
                 # check if the adapter loop is running
                 if not self.swarm_adapter.adapter_loop.is_running():
                     print("Adapter loop is not running, starting it now")
                     try:
                         self.start_adapter()
                     except Exception as e:
                         print(f"Error starting adapter: {e}")
                     if not self.swarm_adapter.adapter_loop.is_running():
-                        raise Exception("Adapter loop is still not running after starting it")
-                
+                        raise Exception(
+                            "Adapter loop is still not running after starting it"
+                        )
+
                 try:
-                    asyncio.run_coroutine_threadsafe(self.command_map[command](data), self.swarm_adapter.adapter_loop)
+                    asyncio.run_coroutine_threadsafe(
+                        self.command_map[command](data), self.swarm_adapter.adapter_loop
+                    )
                 except Exception as e:
                     print(f"Error in {command} command: {e}")
             else:
                 print(f"Unknown command: {command}")
 
     def start_adapter(self):
         adapter_thread = threading.Thread(target=self.swarm_adapter.start)
         adapter_thread.start()
 
     async def on_ready(self, data: str):
         """This method is called when the apter is loaded."""
-        self_description = f"Hi everyone!\nName: {self.name}\nDescription: {self.description}"
+        self_description = (
+            f"Hi everyone!\nName: {self.name}\nDescription: {self.description}"
+        )
         await self.swarm_adapter.send_message(self_description, "intros")
 
     def run(self):
         """This method is called to start the bot
-        
+
         Clarification on the event loops. Bear with me here =)
         Ideally we'd like the adapter and the agent to run in the same event loop,
         but both the discord process and the adent process are blocking the event loop.
 
         So we need to split the process into two event loops, one for the agent and one for the adapter.
 
         However, now we cannot await the adapter methods from the agent, because they are running in different event loops.
         Therefore in the agent we need to use the run_coroutine_threadsafe method to run the adapter methods in the adapter event loop.
-        """       
+        """
         # run the adapter in a separate thread
         self.start_adapter()
 
         # run the event listener in the main thread
         agent_loop = asyncio.get_event_loop()
         agent_loop.run_until_complete(self.on_callback_event_listener())
```

### Comparing `osnap_client-0.1.1a2/osnap_client/core/api.py` & `osnap_client-0.1.1a3/osnap_client/core/api.py`

 * *Files identical despite different names*

### Comparing `osnap_client-0.1.1a2/osnap_client/core/crypt.py` & `osnap_client-0.1.1a3/osnap_client/core/crypt.py`

 * *Files identical despite different names*

### Comparing `osnap_client-0.1.1a2/osnap_client/core/osnap.py` & `osnap_client-0.1.1a3/osnap_client/core/osnap.py`

 * *Files identical despite different names*

### Comparing `osnap_client-0.1.1a2/osnap_client/pubsub/pubsub.py` & `osnap_client-0.1.1a3/osnap_client/pubsub/pubsub.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import asyncio
 import os
 import redis.asyncio as redis
 from fastapi import WebSocket
 
+from dotenv import load_dotenv
+load_dotenv(".env.sender")
+
 REDIS_HOST = os.getenv("REDIS_HOST")
 REDIS_PORT = os.getenv("REDIS_PORT")
 REDIS_USERNAME = os.getenv("REDIS_USERNAME")
 REDIS_PASSWORD = os.getenv("REDIS_PASSWORD")
 
 STOPWORD = "STOP"
```

### Comparing `osnap_client-0.1.1a2/osnap_client/registry/agent_registry.py` & `osnap_client-0.1.1a3/osnap_client/registry/agent_registry.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import redis
 import json
 import uuid
 
-from osnap import OSNAPAgent
+from osnap_client.agents import OSNAPBaseAgent
 
 import logging
 
 LOGGER = logging.getLogger(__name__)
 
 
 class AgentRegistry:
@@ -15,45 +15,44 @@
             host=host,
             port=port,
             username=username,
             password=password,
             decode_responses=True,
         )
 
-    def register(self, agent: OSNAPAgent):
+    def register(self, agent: OSNAPBaseAgent):
         return self.get_or_create_agent(agent)
 
     def get_agents(self, scope):
         return self._get_agents_by_scope(scope)
 
     def _get_agents_by_scope(self, scope):
         agent_ids = self.redis_client.smembers(f"scope:{scope}:agents")
         agents = []
         for agent_id in agent_ids:
             agent_data = self.redis_client.hgetall(f"agent:{agent_id}")
             agent = {k: v for k, v in agent_data.items()}
             agents.append(agent)
         return agents
 
-    def get_or_create_agent(self, agent: OSNAPAgent):
+    def get_or_create_agent(self, agent: OSNAPBaseAgent):
         if self.redis_client.hexists(f"agent:{agent.name}", agent.name):
             return self.get_agent(agent.name)
         else:
             agent.id = str(uuid.uuid4())
             self.add_agent(agent)
 
     def get_agent(self, name):
         agent_data = self.redis_client.hget(f"agent:{name}", name)
-        print("agent_data")
         if agent_data:
             agent_data["tools"] = json.loads(agent_data["tools"])
             return agent_data
         return None
 
-    def add_agent(self, agent: OSNAPAgent) -> OSNAPAgent:
+    def add_agent(self, agent: OSNAPBaseAgent) -> OSNAPBaseAgent | None:
         agent_data = {
             "id": agent.id,
             "name": agent.name,
             "description": agent.description,
             "tools": json.dumps(agent.tools),
             "scope": agent.scope,
         }
```

### Comparing `osnap_client-0.1.1a2/osnap_client/registry/tool_registry.py` & `osnap_client-0.1.1a3/osnap_client/registry/tool_registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import redis
 import uuid
 
-from osnap import OSNAPTool
+from osnap_client.core import OSNAPTool
 
 
 class ToolRegistry:
     def __init__(self, host, port, username, password):
         self.redis_client = redis.Redis(
             host=host,
             port=port,
```

### Comparing `osnap_client-0.1.1a2/osnap_client/utils/ai_engines/EngineBase.py` & `osnap_client-0.1.1a3/osnap_client/utils/ai_engines/EngineBase.py`

 * *Files identical despite different names*

### Comparing `osnap_client-0.1.1a2/osnap_client/utils/ai_engines/GPTConversEngine.py` & `osnap_client-0.1.1a3/osnap_client/utils/ai_engines/GPTConversEngine.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 import os
 import openai
 import tiktoken
 
-from osnap.utils.ai_engines.EngineBase import EngineBase
+from osnap_client.utils.ai_engines.EngineBase import EngineBase
+
 
 class GPTConversEngine(EngineBase):
     """
     gpt-4, gpt-4-0314, gpt-4-32k, gpt-4-32k-0314, gpt-3.5-turbo, gpt-3.5-turbo-0301
     """
+
     SUPPORTED_MODELS = [
         "gpt-4",
         "gpt-4-0314",
         "gpt-4-32k",
         "gpt-4-32k-0314",
         "gpt-3.5-turbo",
-        "gpt-3.5-turbo-0301"
+        "gpt-3.5-turbo-0301",
     ]
 
     def __init__(self, model_name: str, temperature: float, max_response_tokens: int):
-
         if model_name not in self.SUPPORTED_MODELS:
-            raise ValueError(f"Model {model_name} is not supported. Supported models are: {self.SUPPORTED_MODELS}")
+            raise ValueError(
+                f"Model {model_name} is not supported. Supported models are: {self.SUPPORTED_MODELS}"
+            )
 
         super().__init__("openai", model_name, temperature, max_response_tokens)
-        
+
         if "OPENAI_API_KEY" not in os.environ:
             raise ValueError("OPENAI_API_KEY environment variable is not set.")
-        
+
         openai.api_key = os.getenv("OPENAI_API_KEY")
         self.tiktoken_encoding = tiktoken.encoding_for_model(model_name)
 
     def call_model(self, conversation, max_tokens=None, temperature=None) -> str:
         """Calls the gpt-3.5 or gpt-4 model to generate a response to a conversation.
 
         Args:
@@ -45,27 +48,38 @@
         if temperature is None:
             temperature = self.temperature
 
         if isinstance(conversation, str):
             conversation = [{"role": "user", "content": conversation}]
 
         if len(conversation) == 0:
-            raise ValueError("Conversation must have at least one message of format: [{'role': 'user', 'content': 'message'}]")
-        
+            raise ValueError(
+                "Conversation must have at least one message of format: [{'role': 'user', 'content': 'message'}]"
+            )
+
         total_len = 0
         for message in conversation:
             if "role" not in message:
-                raise ValueError("Conversation messages must have a format: {'role': 'user', 'content': 'message'}. 'role' is missing.")
+                raise ValueError(
+                    "Conversation messages must have a format: {'role': 'user', 'content': 'message'}. 'role' is missing."
+                )
             if "content" not in message:
-                raise ValueError("Conversation messages must have a format: {'role': 'user', 'content': 'message'}. 'content' is missing.")
-            message["content"] = self.truncate_message(message["content"], self.max_input_length()-total_len-100)
+                raise ValueError(
+                    "Conversation messages must have a format: {'role': 'user', 'content': 'message'}. 'content' is missing."
+                )
+            message["content"] = self.truncate_message(
+                message["content"], self.max_input_length() - total_len - 100
+            )
             new_message_len = len(self.tiktoken_encoding.encode(message["content"]))
             total_len += new_message_len
-        
+
         try:
-            response = openai.ChatCompletion.create(model=self.model_name, messages=conversation, max_tokens=max_tokens, temperature=temperature, n=1)
+            response = openai.ChatCompletion.create(
+                model=self.model_name,
+                messages=conversation,
+                max_tokens=max_tokens,
+                temperature=temperature,
+                n=1,
+            )
         except:
             return ""
         return response["choices"][0]["message"]["content"]
-
-        
-
```

### Comparing `osnap_client-0.1.1a2/osnap_client/utils/ai_engines/LanchainGoogleEngine.py` & `osnap_client-0.1.1a3/osnap_client/utils/ai_engines/LanchainGoogleEngine.py`

 * *Files identical despite different names*

### Comparing `osnap_client-0.1.1a2/pyproject.toml` & `osnap_client-0.1.1a3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "osnap-client"
-version = "0.1.1a2"
+version = "0.1.1a3"
 description = ""
 authors = ["Forrest Murray <FMurray@gmail.com>", "Vlad Samoilov <nicelir1996@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 langchain = ">=0.0.153,<0.1.0"
```

### Comparing `osnap_client-0.1.1a2/PKG-INFO` & `osnap_client-0.1.1a3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osnap-client
-Version: 0.1.1a2
+Version: 0.1.1a3
 Summary: 
 Author: Forrest Murray
 Author-email: FMurray@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -30,20 +30,21 @@
 
 # OSNAP
 
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![Python Version](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/)
 [![Discord Follow](https://dcbadge.vercel.app/api/server/seKVhCtcAJ?style=flat)](https://discord.gg/seKVhCtcAJ)
 
-The Open Swarm Network Agent Protocol (OSNAP) is a standardized toolkit for building AI agents that interact with each other. Currently, the development and implementation of interacting autonomous AI agents and swarms are highly fragmented, with different projects utilizing various custom-built protocols and communication methods. This lack of standardization can lead to difficulties. OSNAP aims to address these issues by providing a well-defined, standardized toolkit for building and interacting with autonomous AI agents and swarms.
-
 <p align="center">
   <img src="content/logo_midjourney.png" alt="Project logo" width="1080">
 </p>
 
+The Open Swarm Network Agent Protocol (OSNAP) is a standardized toolkit for building AI agents that interact with each other. Currently, the development and implementation of interacting autonomous AI agents and swarms are highly fragmented, with different projects utilizing various custom-built protocols and communication methods. This lack of standardization can lead to difficulties. OSNAP aims to address these issues by providing a well-defined, standardized toolkit for building and interacting with autonomous AI agents and swarms.
+
+
 ## Table of Contents
 - [How to use in your project](#how-to-use-in-your-project)
 - [Examples](#examples)
 - [Architecture Overview](#architecture-overview)
 - [Next-Ups](#next-ups)
 - [How to Contribute](#how-to-contribute)
 
@@ -67,14 +68,16 @@
 The communication is handleded via the DiscordAdapter and the only think you need to do is to implement the logic of the `SwarmAgentBase`.
 
 # Architecture overview
 <p align="center">
   <img src="content/architecture_diagram.png" alt="Project diagram" width="720">
 </p>
 
+## Docker Containers
+[To Example](examples/2_containers/README.md)
 
 # Next-ups
 - make adding new models as easy as possible, including custom deployed ones like llama
 - multi-key support for higher scalability
 
 
 # How to Contribute
```

