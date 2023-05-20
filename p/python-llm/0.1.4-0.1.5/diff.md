# Comparing `tmp/python-llm-0.1.4.tar.gz` & `tmp/python-llm-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-llm-0.1.4.tar", last modified: Sun May 14 23:04:38 2023, max compression
+gzip compressed data, was "python-llm-0.1.5.tar", last modified: Sat May 20 16:42:29 2023, max compression
```

## Comparing `python-llm-0.1.4.tar` & `python-llm-0.1.5.tar`

### file list

```diff
@@ -1,23 +1,27 @@
-drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-14 23:04:38.403267 python-llm-0.1.4/
--rw-r--r--   0 danielgross   (501) staff       (20)     1069 2023-03-30 14:06:17.000000 python-llm-0.1.4/LICENSE
--rw-r--r--   0 danielgross   (501) staff       (20)     1735 2023-05-14 23:04:38.403165 python-llm-0.1.4/PKG-INFO
--rw-r--r--   0 danielgross   (501) staff       (20)     1458 2023-05-14 22:59:17.000000 python-llm-0.1.4/README.md
-drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-14 23:04:38.401872 python-llm-0.1.4/llm/
--rw-r--r--   0 danielgross   (501) staff       (20)       69 2023-05-13 13:51:59.000000 python-llm-0.1.4/llm/__init__.py
-drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-14 23:04:38.402170 python-llm-0.1.4/llm/api/
--rw-r--r--   0 danielgross   (501) staff       (20)        0 2023-03-29 19:17:50.000000 python-llm-0.1.4/llm/api/__init__.py
--rw-r--r--   0 danielgross   (501) staff       (20)     2376 2023-05-14 14:49:00.000000 python-llm-0.1.4/llm/api/claude.py
--rw-r--r--   0 danielgross   (501) staff       (20)      980 2023-03-30 14:01:26.000000 python-llm-0.1.4/llm/api/openaiapi.py
--rw-r--r--   0 danielgross   (501) staff       (20)     2384 2023-05-14 14:49:01.000000 python-llm-0.1.4/llm/main.py
--rw-r--r--   0 danielgross   (501) staff       (20)     1781 2023-05-13 13:24:32.000000 python-llm-0.1.4/llm/util.py
-drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-14 23:04:38.402762 python-llm-0.1.4/python_llm.egg-info/
--rw-r--r--   0 danielgross   (501) staff       (20)     1735 2023-05-14 23:04:38.000000 python-llm-0.1.4/python_llm.egg-info/PKG-INFO
--rw-r--r--   0 danielgross   (501) staff       (20)      336 2023-05-14 23:04:38.000000 python-llm-0.1.4/python_llm.egg-info/SOURCES.txt
--rw-r--r--   0 danielgross   (501) staff       (20)        1 2023-05-14 23:04:38.000000 python-llm-0.1.4/python_llm.egg-info/dependency_links.txt
--rw-r--r--   0 danielgross   (501) staff       (20)      146 2023-05-14 23:04:38.000000 python-llm-0.1.4/python_llm.egg-info/requires.txt
--rw-r--r--   0 danielgross   (501) staff       (20)        4 2023-05-14 23:04:38.000000 python-llm-0.1.4/python_llm.egg-info/top_level.txt
--rw-r--r--   0 danielgross   (501) staff       (20)       38 2023-05-14 23:04:38.403297 python-llm-0.1.4/setup.cfg
--rw-r--r--   0 danielgross   (501) staff       (20)      650 2023-05-14 23:04:32.000000 python-llm-0.1.4/setup.py
-drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-14 23:04:38.403006 python-llm-0.1.4/tests/
--rw-r--r--   0 danielgross   (501) staff       (20)     2749 2023-05-14 22:54:04.000000 python-llm-0.1.4/tests/test_claude.py
--rw-r--r--   0 danielgross   (501) staff       (20)     2097 2023-05-14 22:53:48.000000 python-llm-0.1.4/tests/test_openai.py
+drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-20 16:42:29.462185 python-llm-0.1.5/
+-rw-r--r--   0 danielgross   (501) staff       (20)     1069 2023-03-30 14:06:17.000000 python-llm-0.1.5/LICENSE
+-rw-r--r--   0 danielgross   (501) staff       (20)     1969 2023-05-20 16:42:29.462080 python-llm-0.1.5/PKG-INFO
+-rw-r--r--   0 danielgross   (501) staff       (20)     1692 2023-05-20 16:36:33.000000 python-llm-0.1.5/README.md
+drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-20 16:42:29.460333 python-llm-0.1.5/llm/
+-rw-r--r--   0 danielgross   (501) staff       (20)       81 2023-05-20 15:11:39.000000 python-llm-0.1.5/llm/__init__.py
+drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-20 16:42:29.460628 python-llm-0.1.5/llm/api/
+-rw-r--r--   0 danielgross   (501) staff       (20)        0 2023-03-29 19:17:50.000000 python-llm-0.1.5/llm/api/__init__.py
+-rw-r--r--   0 danielgross   (501) staff       (20)     2387 2023-05-20 16:23:02.000000 python-llm-0.1.5/llm/api/anthropicapi.py
+-rw-r--r--   0 danielgross   (501) staff       (20)     1651 2023-05-20 16:32:24.000000 python-llm-0.1.5/llm/api/openaiapi.py
+-rw-r--r--   0 danielgross   (501) staff       (20)     3899 2023-05-20 16:23:54.000000 python-llm-0.1.5/llm/main.py
+drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-20 16:42:29.460964 python-llm-0.1.5/llm/utils/
+-rw-r--r--   0 danielgross   (501) staff       (20)        0 2023-05-20 11:50:33.000000 python-llm-0.1.5/llm/utils/__init__.py
+-rw-r--r--   0 danielgross   (501) staff       (20)     3200 2023-05-20 11:56:01.000000 python-llm-0.1.5/llm/utils/apikeys.py
+-rw-r--r--   0 danielgross   (501) staff       (20)     2322 2023-05-20 16:23:40.000000 python-llm-0.1.5/llm/utils/parsing.py
+drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-20 16:42:29.461598 python-llm-0.1.5/python_llm.egg-info/
+-rw-r--r--   0 danielgross   (501) staff       (20)     1969 2023-05-20 16:42:29.000000 python-llm-0.1.5/python_llm.egg-info/PKG-INFO
+-rw-r--r--   0 danielgross   (501) staff       (20)      424 2023-05-20 16:42:29.000000 python-llm-0.1.5/python_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 danielgross   (501) staff       (20)        1 2023-05-20 16:42:29.000000 python-llm-0.1.5/python_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 danielgross   (501) staff       (20)      167 2023-05-20 16:42:29.000000 python-llm-0.1.5/python_llm.egg-info/requires.txt
+-rw-r--r--   0 danielgross   (501) staff       (20)        4 2023-05-20 16:42:29.000000 python-llm-0.1.5/python_llm.egg-info/top_level.txt
+-rw-r--r--   0 danielgross   (501) staff       (20)       38 2023-05-20 16:42:29.462220 python-llm-0.1.5/setup.cfg
+-rw-r--r--   0 danielgross   (501) staff       (20)      650 2023-05-20 16:42:25.000000 python-llm-0.1.5/setup.py
+drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-20 16:42:29.461946 python-llm-0.1.5/tests/
+-rw-r--r--   0 danielgross   (501) staff       (20)     3263 2023-05-20 14:37:34.000000 python-llm-0.1.5/tests/test_anthropic.py
+-rw-r--r--   0 danielgross   (501) staff       (20)      853 2023-05-20 16:32:05.000000 python-llm-0.1.5/tests/test_multi_stream.py
+-rw-r--r--   0 danielgross   (501) staff       (20)     3292 2023-05-20 14:37:34.000000 python-llm-0.1.5/tests/test_openai.py
```

### Comparing `python-llm-0.1.4/LICENSE` & `python-llm-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `python-llm-0.1.4/llm/api/claude.py` & `python-llm-0.1.5/llm/api/anthropicapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import requests
 import anthropic
-from llm.util import api_keys
+
+from llm.utils.apikeys import api_keys
 
 
 BASE_URL = "https://api.anthropic.com"
 
 
 def client():
     return anthropic.Client(api_keys["anthropic"])
@@ -65,15 +66,15 @@
         model=engine,
         max_tokens_to_sample=max_tokens_to_sample,
         **kwargs
     )
     return resp["completion"]
 
 
-async def stream_chat(messages, engine="claude-v1", system=None, max_tokens_to_sample=30, **kwargs):
+async def stream_chat(messages, engine="claude-v1", system=None, max_tokens_to_sample=100, **kwargs):
     c = client()
     prompt = format_chat_messages(messages)
     response = await c.acompletion_stream(
         prompt=prompt,
         stop_sequences=[anthropic.HUMAN_PROMPT],
         max_tokens_to_sample=max_tokens_to_sample,
         model=engine,
```

### Comparing `python-llm-0.1.4/llm/api/openaiapi.py` & `python-llm-0.1.5/llm/api/openaiapi.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,52 @@
 """Implement the OpenAI API."""
 
+from llm.utils.parsing import structure_chat
 import openai
 import logging
 
-from llm import util
+logger = logging.getLogger(__name__)
 
 
-def complete(prompt, engine="text-davinci-003", **kwargs):
+def complete(prompt, engine, **kwargs):
     """Complete text using the OpenAI API."""
     if engine.startswith("gpt-3.5") or engine.startswith("gpt-4"):
-        return chat(util.structure_chat([prompt]), engine=engine, **kwargs)
-    logging.debug(f"Completing with {engine} using prompt: {prompt}")
+        return chat(structure_chat([prompt]), engine=engine, **kwargs)
+    logger.debug(f"Completing with {engine} using prompt: {prompt}")
     return openai.Completion.create(
         engine=engine,
         prompt=prompt,
         **kwargs
-    ).choices[0].text.strip()
+    ).choices[0].text
 
 
-def chat(messages, system=None, engine="gpt-3.5-turbo", **kwargs):
+def chat(messages, engine, system=None, **kwargs):
     """Chat with the OpenAI API."""
+    if engine.startswith("text-"):
+        raise ValueError(
+            f"Cannot issue a ChatCompletion with engine {engine}.")
     if system is not None:
         messages = [{"role": "system", "content": system}] + messages
-    logging.debug(f"Chatting with {engine} using messages: {messages}")
+    logger.debug(f"Chatting with {engine} using messages: {messages}")
     response = openai.ChatCompletion.create(
         model=engine,
         messages=messages,
         **kwargs
     )
-    return response.choices[0].message.content.strip()
+    return response.choices[0].message.content
+
+
+async def stream_chat(messages, engine, system=None, **kwargs):
+    """Chat with the OpenAI API."""
+    if system is not None:
+        messages = [{"role": "system", "content": system}] + messages
+    logger.debug(f"Chatting with {engine} using messages: {messages}")
+
+    result = openai.ChatCompletion.create(
+        model=engine,
+        messages=messages,
+        stream=True,
+        **kwargs
+    )
+    for chunk in result:
+        if chunk.choices[0].delta.get('content') != None:
+            yield chunk.choices[0].delta.content
```

### Comparing `python-llm-0.1.4/setup.py` & `python-llm-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = f.read().splitlines()
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name='python-llm',
-    version='0.1.4',
+    version='0.1.5',
     author='Daniel Gross',
     author_email='d@dcgross.com',
     description='An LLM wrapper for Humans',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_namespace_packages(include=['llm', 'llm.*']),
     url="https://github.com/danielgross/python-llm",
```

### Comparing `python-llm-0.1.4/tests/test_claude.py` & `python-llm-0.1.5/tests/test_openai.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,55 +1,69 @@
 import unittest
-import llm
+import asynctest
 import os
 import vcr
-import asynctest
+import llm
+import logging
 
 # Only get API keys if they exist
-_key = open(os.path.expanduser("~/.anthropic")).read().strip() if os.path.exists(
-    os.path.expanduser("~/.anthropic")) else 'test'
-llm.set_api_key(anthropic=_key)
+_key = open(os.path.expanduser("~/.openai")).read().strip() if os.path.exists(
+    os.path.expanduser("~/.openai")) else 'test'
+llm.set_api_key(openai=_key)
 
-class TestClaudeCompletions(unittest.TestCase):
 
-    @vcr.use_cassette("tests/fixtures/claude/test_completion.yaml", filter_headers=['authorization', 'x-api-key'])
+class TestOpenAICompletions(unittest.TestCase):
+
+    @vcr.use_cassette("tests/fixtures/openai/test_completion.yaml", filter_headers=['authorization'])
     def test_completion(self):
-        prompt = "Hello, my name is"
+        prompt = "2+2 is how much? Good question, I think 2+2="
         completion = llm.complete(
-            prompt, engine="anthropic:claude-v1", max_tokens_to_sample=1).strip()
-        self.assertTrue(completion.startswith("Claude"))
+            prompt, engine="openai:text-davinci-002", max_tokens=1)
+        self.assertEqual(completion, "4")
 
-    @vcr.use_cassette("tests/fixtures/claude/test_simple_chat.yaml", filter_headers=['authorization', 'x-api-key'])
+    @vcr.use_cassette("tests/fixtures/openai/test_simple_chat.yaml", filter_headers=['authorization', 'x-api-key'])
     def test_simple_chat(self):
-        self.assertEqual(llm.chat(["What is 2+2? Reply with just one number and no punctuation."], engine="anthropic:claude-v1"), "4")
+        self.assertEqual(llm.chat(
+            ["What is 2+2? Reply with just one number and no punctuaction."], engine="openai:gpt-3.5-turbo"), "4")
+
+    @vcr.use_cassette("tests/fixtures/openai/test_completion_chat_model.yaml", filter_headers=['authorization'])
+    def test_completion_chat_model(self):
+        """Test that we can use a chat model for completion."""
+        prompt = "Hello, my name is"
+        completion = llm.complete(
+            prompt, engine="openai:gpt-3.5-turbo", max_tokens=1)
+        # Assert we only got one extra word that is capitalized
+        self.assertEqual(len(completion.split(' ')), 1)
+        self.assertTrue(completion[0].isupper(), completion)
 
-    @vcr.use_cassette("tests/fixtures/claude/test_chat.yaml", filter_headers=['authorization', 'x-api-key'])
+    @vcr.use_cassette("tests/fixtures/openai/test_chat.yaml", filter_headers=['authorization'])
     def test_chat(self):
-        messages = ["what is your favorite cat breed?", "I like tabbies.",
-                    "And what about dogs? Reply with punctuation."]
-        response = llm.chat(messages, engine="anthropic:claude-v1")
-        self.assertTrue(response[0] != " ",
-                        "Response should not start with a space.")
+        messages = ["hello", "how are you?", "I'm good, thanks."]
+        response = llm.chat(messages, engine="openai:gpt-3.5-turbo")
         # Make sure the response is sorta directionally correct, e.g. has more than 3 words and some punctuation.
         self.assertTrue(len(response.split(' ')) > 3)
         self.assertTrue(
-            '.' in response or '!' in response or '?' in response or ',' in response, response)
+            '.' in response or '!' in response or '?' in response, response)
 
 
-class TestClaudeStreaming(asynctest.TestCase):
+class TestOpenAIStreaming(asynctest.TestCase):
 
-    # TODO: I am not sure this really works? It passes but I'm a little suspicious.
-    @vcr.use_cassette("tests/fixtures/claude/test_streaming_chat.yaml", filter_headers=['authorization', 'x-api-key'])
-    async def test_streaming_chat(self):
+    @vcr.use_cassette("tests/fixtures/openai/test_streaming_chat_method_full.yaml", filter_headers=['authorization', 'x-api-key'])
+    async def test_streaming_chat_method_full(self):
         messages = ["what is your favorite cat breed?", "I like tabbies.",
-                    "And what about dogs? Reply with punctuation."]
+                    "And what about dogs?"]
         responses = []
-        async for response in llm.stream_chat(messages, engine="anthropic:claude-v1"):
+        async for response in llm.stream_chat(messages, engine="openai:gpt-3.5-turbo", stream_method="full"):
             responses.append(response)
         final_response = responses[-1]
-        self.assertTrue(response[0] != " ",
-                        "Response should not start with a space.")
-        # Make sure we're not repeating ourselves within this final response.
-        self.assertTrue(final_response[:5] not in final_response[5:])
-        self.assertTrue(len(final_response.split(' ')) > 3)
         self.assertTrue(
-            '.' in response or '!' in response or '?' in response, response)
+            'Labrador Retriever, German Shepherd, Golden Retriever, Bulldog, Beagle' in final_response)
+
+    @vcr.use_cassette("tests/fixtures/openai/test_streaming_chat_method_delta.yaml", filter_headers=['authorization', 'x-api-key'])
+    async def test_streaming_chat_method_delta(self):
+        messages = ["what is your favorite cat breed?", "I like tabbies.",
+                    "And what about dogs?"]
+        responses = []
+        async for response in llm.stream_chat(messages, engine="openai:gpt-3.5-turbo", stream_method="delta"):
+            responses.append(response)
+        self.assertEqual(responses[0], 'As')
+        self.assertEqual(responses[1], ' an')
```

