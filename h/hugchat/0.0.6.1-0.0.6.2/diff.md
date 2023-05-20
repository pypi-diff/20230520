# Comparing `tmp/hugchat-0.0.6.1.tar.gz` & `tmp/hugchat-0.0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hugchat-0.0.6.1.tar", last modified: Wed May 17 00:32:20 2023, max compression
+gzip compressed data, was "hugchat-0.0.6.2.tar", last modified: Sat May 20 05:26:05 2023, max compression
```

## Comparing `hugchat-0.0.6.1.tar` & `hugchat-0.0.6.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-17 00:32:20.523693 hugchat-0.0.6.1/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    34523 2023-05-01 00:33:11.000000 hugchat-0.0.6.1/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3829 2023-05-17 00:32:20.519693 hugchat-0.0.6.1/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2809 2023-05-16 00:53:53.000000 hugchat-0.0.6.1/README.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-05-17 00:32:20.523693 hugchat-0.0.6.1/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1436 2023-05-17 00:32:09.000000 hugchat-0.0.6.1/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-17 00:32:20.507692 hugchat-0.0.6.1/src/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-17 00:32:20.515693 hugchat-0.0.6.1/src/hugchat/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-03 15:54:22.000000 hugchat-0.0.6.1/src/hugchat/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      179 2023-05-03 15:54:22.000000 hugchat-0.0.6.1/src/hugchat/cli.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10716 2023-05-17 00:31:10.000000 hugchat-0.0.6.1/src/hugchat/hugchat.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-17 00:32:20.519693 hugchat-0.0.6.1/src/hugchat.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3829 2023-05-17 00:32:20.000000 hugchat-0.0.6.1/src/hugchat.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      266 2023-05-17 00:32:20.000000 hugchat-0.0.6.1/src/hugchat.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-05-17 00:32:20.000000 hugchat-0.0.6.1/src/hugchat.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       27 2023-05-17 00:32:20.000000 hugchat-0.0.6.1/src/hugchat.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        8 2023-05-17 00:32:20.000000 hugchat-0.0.6.1/src/hugchat.egg-info/top_level.txt
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-20 05:26:05.554893 hugchat-0.0.6.2/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    34523 2023-05-01 00:33:11.000000 hugchat-0.0.6.2/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4133 2023-05-20 05:26:05.554893 hugchat-0.0.6.2/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3113 2023-05-20 05:25:35.000000 hugchat-0.0.6.2/README.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-05-20 05:26:05.554893 hugchat-0.0.6.2/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1436 2023-05-20 05:25:10.000000 hugchat-0.0.6.2/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-20 05:26:05.546893 hugchat-0.0.6.2/src/
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-20 05:26:05.550893 hugchat-0.0.6.2/src/hugchat/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-03 15:54:22.000000 hugchat-0.0.6.2/src/hugchat/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      179 2023-05-03 15:54:22.000000 hugchat-0.0.6.2/src/hugchat/cli.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12254 2023-05-20 05:25:35.000000 hugchat-0.0.6.2/src/hugchat/hugchat.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-20 05:26:05.554893 hugchat-0.0.6.2/src/hugchat.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4133 2023-05-20 05:26:05.000000 hugchat-0.0.6.2/src/hugchat.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      266 2023-05-20 05:26:05.000000 hugchat-0.0.6.2/src/hugchat.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-05-20 05:26:05.000000 hugchat-0.0.6.2/src/hugchat.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       27 2023-05-20 05:26:05.000000 hugchat-0.0.6.2/src/hugchat.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        8 2023-05-20 05:26:05.000000 hugchat-0.0.6.2/src/hugchat.egg-info/top_level.txt
```

### Comparing `hugchat-0.0.6.1/LICENSE` & `hugchat-0.0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hugchat-0.0.6.1/PKG-INFO` & `hugchat-0.0.6.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugchat
-Version: 0.0.6.1
+Version: 0.0.6.2
 Summary: A huggingchat python api.
 Home-page: https://github.com/Soulter/hugging-chat-api
 Author: Soulter
 Author-email: 905617992@qq.com
 License: GNU Affero General Public License v3.0
 Project-URL: Bug Report, https://github.com/Soulter/hugging-chat-api/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -104,7 +104,13 @@
 
 Commands in cli mode:
 
 - `/new` : Create and switch to a new conversation.
 - `/ids` : Shows a list of all ID numbers and ID strings in current session.
 - `/switch <id>` : Switches to the ID number passed.
 - `/exit` : Closes CLI environment.
+
+## Disclaimers
+
+This is not an official [Hugging Face](https://huggingface.co/) product. This is a **personal project** and is not affiliated with [Hugging Face](https://huggingface.co/) in any way. Don't sue us.
+
+**Server resources are precious, it is not recommended to request this API frequently.**
```

### Comparing `hugchat-0.0.6.1/README.md` & `hugchat-0.0.6.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -80,7 +80,13 @@
 
 Commands in cli mode:
 
 - `/new` : Create and switch to a new conversation.
 - `/ids` : Shows a list of all ID numbers and ID strings in current session.
 - `/switch <id>` : Switches to the ID number passed.
 - `/exit` : Closes CLI environment.
+
+## Disclaimers
+
+This is not an official [Hugging Face](https://huggingface.co/) product. This is a **personal project** and is not affiliated with [Hugging Face](https://huggingface.co/) in any way. Don't sue us.
+
+**Server resources are precious, it is not recommended to request this API frequently.**
```

### Comparing `hugchat-0.0.6.1/setup.py` & `hugchat-0.0.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_namespace_packages
 from setuptools import setup
 
 setup(
     name="hugchat",
-    version="0.0.6.1",
+    version="0.0.6.2",
     description="A huggingchat python api.",
     long_description=open("README.md", "rt", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Soulter/hugging-chat-api",
     project_urls={
         "Bug Report": "https://github.com/Soulter/hugging-chat-api/issues"
     },
```

### Comparing `hugchat-0.0.6.1/src/hugchat/hugchat.py` & `hugchat-0.0.6.2/src/hugchat/hugchat.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 from requests import Session
 import json
+import os
 import uuid
+import logging
+
 
 class ChatBot:
     
     cookies: dict
     """Cookies for authentication"""
 
     session: Session
@@ -18,14 +21,16 @@
         if cookies is None and cookie_path == "":
             raise Exception("Authentication is required now, but no cookies provided")
         elif cookies is not None and cookie_path != "":
             raise Exception("Both cookies and cookie_path provided")
         
         if cookies is None and cookie_path != "":
             # read cookies from path
+            if not os.path.exists(cookie_path):
+                raise Exception(f"Cookie file {cookie_path} not found. Note: The file must be in JSON format and must contain a list of cookies. See more at https://github.com/Soulter/hugging-chat-api")
             with open(cookie_path, "r") as f:
                 cookies = json.load(f)
 
         # convert cookies to KV format
         if isinstance(cookies, list):
             cookies = {cookie["name"]: cookie["value"] for cookie in cookies}
 
@@ -74,59 +79,72 @@
     #       acts as a pointer to the data in the object.
     #
     # Returns a pointer to this objects list that contains id of conversations.
     def get_conversation_list(self) -> list:
         return list(self.conversation_id_list)
 
     def accept_ethics_modal(self):
+        '''
+        [Deprecated Method]
+        '''
         response = self.session.post(self.hf_base_url + "/chat/settings", headers=self.get_headers(ref=False), cookies=self.get_cookies(), allow_redirects=True, data={
             "ethicsModalAccepted": "true",
             "shareConversationsWithModelAuthors": "true",
             "ethicsModalAcceptedAt": "",
             "activeModel": str(self.active_model)
         })
 
         if response.status_code != 200:
             raise Exception(f"Failed to accept ethics modal with status code {response.status_code}. {response.content.decode()}")
         
         return True
     
     def new_conversation(self) -> str:
+        '''
+        Create a new conversation. Return the new conversation id. You should change the conversation by calling change_conversation() after calling this method.
+        '''
         err_count = 0
 
         # Accept the welcome modal when init.
         # 17/5/2023: This is not required anymore.
         # if not self.accepted_welcome_modal:
         #     self.accept_ethics_modal()
 
         # Create new conversation and get a conversation id.
         resp = ""
         while True:
             try:
                 resp = self.session.post(self.hf_base_url + "/chat/conversation", json={"model": self.active_model}, headers=self.json_header)
                 # print(resp.text)
+                logging.debug(resp.text)
                 cid = json.loads(resp.text)['conversationId']
                 self.conversation_id_list.append(cid)
                 return cid
             
             except BaseException as e:
                 err_count += 1
-                print(f"[Error] Failed to create new conversation. Retrying... ({err_count})")
+                logging.debug(f" Failed to create new conversation. Retrying... ({err_count})")
                 if err_count > 5:
                     raise e
                 continue
     
     def change_conversation(self, conversation_id: str) -> bool:
+        '''
+        Change the current conversation to another one. Need a valid conversation id.
+        '''
         if conversation_id not in self.conversation_id_list:
             raise Exception("Invalid conversation id. Please check conversation id list.")
         self.current_conversation = conversation_id
         return True
     
         
     def summarize_conversation(self, conversation_id: str = None) -> str:
+        '''
+        Return a summary of the conversation.
+        '''
         if conversation_id is None:
             conversation_id = self.current_conversation
         
         headers = self.get_headers()
 
         r = self.session.post(f"{self.hf_base_url}/chat/conversation/{conversation_id}/summarize", headers=headers, cookies=self.get_cookies())
         
@@ -136,14 +154,17 @@
         response = r.json()
         if 'title' in response:
             return response['title']
 
         raise Exception(f"Unknown server response: {response}")
     
     def share_conversation(self, conversation_id: str = None) -> str:
+        '''
+        Return a share link of the conversation.
+        '''
         if conversation_id is None:
             conversation_id = self.current_conversation
 
         headers = self.get_headers()
         
         r = self.session.post(f"{self.hf_base_url}/chat/conversation/{conversation_id}/share", headers=headers, cookies=self.get_cookies())
         
@@ -152,14 +173,30 @@
         
         response = r.json()
         if 'url' in response:
             return response['url']
 
         raise Exception(f"Unknown server response: {response}")
 
+    def delete_conversation(self, conversation_id: str = None) -> bool:
+        '''
+        Delete a HuggingChat conversation by conversation_id.
+        '''
+
+        if conversation_id is None:
+            raise Exception("conversation_id is required.")
+
+        headers = self.get_headers()
+
+        r = self.session.delete(f"{self.hf_base_url}/chat/conversation/{conversation_id}", headers=headers, cookies=self.get_cookies())
+
+        if r.status_code != 200:
+            raise Exception(f"Failed to delete conversation with status code: {r.status_code}")
+        
+
     def chat(
         self,
         text: str,
         temperature: float=0.9,
         top_p: float=0.95,
         repetition_penalty: float=1.2,
         top_k: int=50,
@@ -169,14 +206,17 @@
         stop: list=["</s>"],
         return_full_text: bool=False,
         stream: bool=True,
         use_cache: bool=False,
         is_retry: bool=False,
         retry_count: int=5,
     ):
+        '''
+        Send a message to the current conversation. Return the response text.
+        '''
         if retry_count <= 0:
             raise Exception("the parameter retry_count must be greater than 0.")
         if self.current_conversation == "":
             self.current_conversation = self.new_conversation()
         req_json = {
             "inputs": text,
             "parameters": {
@@ -219,14 +259,15 @@
                         res_text += obj["generated_text"]
                     elif "error" in obj:
                         raise Exception(obj["error"])
             return res_text
 
 def cli():
     print("-------HuggingChat-------")
+    print("Official Site: https://huggingface.co/chat")
     print("1. AI is an area of active research with known problems such as biased generation and misinformation. Do not use this application for high-stakes decisions or advice.\n2. Your conversations will be shared with model authors.\nContinuing to use means that you accept the above points")
     chatbot = ChatBot(cookie_path="cookies.json")
     running = True
     while running:
         question = input("> ")
         if question == "/new":
             cid = chatbot.new_conversation()
```

### Comparing `hugchat-0.0.6.1/src/hugchat.egg-info/PKG-INFO` & `hugchat-0.0.6.2/src/hugchat.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugchat
-Version: 0.0.6.1
+Version: 0.0.6.2
 Summary: A huggingchat python api.
 Home-page: https://github.com/Soulter/hugging-chat-api
 Author: Soulter
 Author-email: 905617992@qq.com
 License: GNU Affero General Public License v3.0
 Project-URL: Bug Report, https://github.com/Soulter/hugging-chat-api/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -104,7 +104,13 @@
 
 Commands in cli mode:
 
 - `/new` : Create and switch to a new conversation.
 - `/ids` : Shows a list of all ID numbers and ID strings in current session.
 - `/switch <id>` : Switches to the ID number passed.
 - `/exit` : Closes CLI environment.
+
+## Disclaimers
+
+This is not an official [Hugging Face](https://huggingface.co/) product. This is a **personal project** and is not affiliated with [Hugging Face](https://huggingface.co/) in any way. Don't sue us.
+
+**Server resources are precious, it is not recommended to request this API frequently.**
```

