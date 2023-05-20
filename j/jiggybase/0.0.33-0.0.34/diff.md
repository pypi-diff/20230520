# Comparing `tmp/jiggybase-0.0.33.tar.gz` & `tmp/jiggybase-0.0.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jiggybase-0.0.33.tar", last modified: Mon May 15 16:48:36 2023, max compression
+gzip compressed data, was "jiggybase-0.0.34.tar", last modified: Sat May 20 00:43:09 2023, max compression
```

## Comparing `jiggybase-0.0.33.tar` & `jiggybase-0.0.34.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-15 16:48:36.214019 jiggybase-0.0.33/
--rw-r--r--   0 wsk        (501) staff       (20)    11357 2023-04-10 04:07:02.000000 jiggybase-0.0.33/LICENSE
--rw-r--r--   0 wsk        (501) staff       (20)     6813 2023-05-15 16:48:36.213659 jiggybase-0.0.33/PKG-INFO
--rw-r--r--   0 wsk        (501) staff       (20)     6279 2023-05-15 02:51:01.000000 jiggybase-0.0.33/README.md
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-15 16:48:36.205687 jiggybase-0.0.33/jiggybase/
--rw-r--r--   0 wsk        (501) staff       (20)       30 2023-04-28 15:28:30.000000 jiggybase-0.0.33/jiggybase/__init__.py
--rw-r--r--   0 wsk        (501) staff       (20)      989 2023-05-15 14:54:50.000000 jiggybase-0.0.33/jiggybase/chat_stream.py
--rw-r--r--   0 wsk        (501) staff       (20)     2403 2023-05-15 15:21:13.000000 jiggybase-0.0.33/jiggybase/client.py
--rw-r--r--   0 wsk        (501) staff       (20)    10503 2023-05-15 16:47:12.000000 jiggybase-0.0.33/jiggybase/collection.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-15 16:48:36.208539 jiggybase-0.0.33/jiggybase/examples/
--rw-r--r--   0 wsk        (501) staff       (20)     1378 2023-05-15 15:42:51.000000 jiggybase-0.0.33/jiggybase/examples/chat_completion.py
--rw-r--r--   0 wsk        (501) staff       (20)      295 2023-05-15 15:35:06.000000 jiggybase-0.0.33/jiggybase/examples/chat_completion_stream.py
--rwxr-xr-x   0 wsk        (501) staff       (20)     3381 2023-05-05 04:06:34.000000 jiggybase-0.0.33/jiggybase/examples/jiggybase_upload.py
--rw-r--r--   0 wsk        (501) staff       (20)     1361 2023-05-03 07:37:11.000000 jiggybase-0.0.33/jiggybase/examples/upload_email_example.py
--rw-r--r--   0 wsk        (501) staff       (20)     5705 2023-05-15 15:27:23.000000 jiggybase-0.0.33/jiggybase/jiggybase_session.py
--rw-r--r--   0 wsk        (501) staff       (20)     1187 2023-03-30 18:09:13.000000 jiggybase-0.0.33/jiggybase/login.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-15 16:48:36.212966 jiggybase-0.0.33/jiggybase/models/
--rw-r--r--   0 wsk        (501) staff       (20)      273 2023-04-26 01:37:49.000000 jiggybase-0.0.33/jiggybase/models/__init__.py
--rw-r--r--   0 wsk        (501) staff       (20)     1236 2023-04-10 05:17:32.000000 jiggybase-0.0.33/jiggybase/models/auth.py
--rw-r--r--   0 wsk        (501) staff       (20)     2767 2023-05-15 16:07:13.000000 jiggybase-0.0.33/jiggybase/models/chat.py
--rw-r--r--   0 wsk        (501) staff       (20)      188 2023-05-15 03:37:46.000000 jiggybase-0.0.33/jiggybase/models/chatmodel.py
--rw-r--r--   0 wsk        (501) staff       (20)     1322 2023-04-10 16:54:34.000000 jiggybase-0.0.33/jiggybase/models/chunk.py
--rw-r--r--   0 wsk        (501) staff       (20)     4240 2023-04-20 21:45:37.000000 jiggybase-0.0.33/jiggybase/models/collection.py
--rw-r--r--   0 wsk        (501) staff       (20)      454 2023-04-23 05:06:00.000000 jiggybase-0.0.33/jiggybase/models/embedding.py
--rw-r--r--   0 wsk        (501) staff       (20)      696 2023-04-10 04:48:20.000000 jiggybase-0.0.33/jiggybase/models/metadata.py
--rw-r--r--   0 wsk        (501) staff       (20)     2214 2023-04-10 04:58:39.000000 jiggybase-0.0.33/jiggybase/models/org.py
--rw-r--r--   0 wsk        (501) staff       (20)     3166 2023-05-14 15:04:22.000000 jiggybase-0.0.33/jiggybase/models/plugin.py
--rw-r--r--   0 wsk        (501) staff       (20)     3415 2023-05-04 23:56:42.000000 jiggybase-0.0.33/jiggybase/models/plugin_config.py
--rw-r--r--   0 wsk        (501) staff       (20)     2834 2023-04-22 23:44:02.000000 jiggybase-0.0.33/jiggybase/models/prompt.py
--rw-r--r--   0 wsk        (501) staff       (20)     3012 2023-04-11 17:29:49.000000 jiggybase-0.0.33/jiggybase/models/providers.py
--rw-r--r--   0 wsk        (501) staff       (20)     1820 2023-04-17 16:14:19.000000 jiggybase-0.0.33/jiggybase/models/user.py
--rw-r--r--   0 wsk        (501) staff       (20)     4600 2023-04-29 15:22:54.000000 jiggybase-0.0.33/jiggybase/org.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-15 16:48:36.207380 jiggybase-0.0.33/jiggybase.egg-info/
--rw-r--r--   0 wsk        (501) staff       (20)     6813 2023-05-15 16:48:36.000000 jiggybase-0.0.33/jiggybase.egg-info/PKG-INFO
--rw-r--r--   0 wsk        (501) staff       (20)      960 2023-05-15 16:48:36.000000 jiggybase-0.0.33/jiggybase.egg-info/SOURCES.txt
--rw-r--r--   0 wsk        (501) staff       (20)        1 2023-05-15 16:48:36.000000 jiggybase-0.0.33/jiggybase.egg-info/dependency_links.txt
--rw-r--r--   0 wsk        (501) staff       (20)       78 2023-05-15 16:48:36.000000 jiggybase-0.0.33/jiggybase.egg-info/entry_points.txt
--rw-r--r--   0 wsk        (501) staff       (20)       32 2023-05-15 16:48:36.000000 jiggybase-0.0.33/jiggybase.egg-info/requires.txt
--rw-r--r--   0 wsk        (501) staff       (20)       10 2023-05-15 16:48:36.000000 jiggybase-0.0.33/jiggybase.egg-info/top_level.txt
--rw-r--r--   0 wsk        (501) staff       (20)      752 2023-05-15 16:47:19.000000 jiggybase-0.0.33/pyproject.toml
--rw-r--r--   0 wsk        (501) staff       (20)       38 2023-05-15 16:48:36.214116 jiggybase-0.0.33/setup.cfg
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-15 16:48:36.213260 jiggybase-0.0.33/test/
--rw-r--r--   0 wsk        (501) staff       (20)      830 2023-04-28 15:38:35.000000 jiggybase-0.0.33/test/test.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-20 00:43:09.325658 jiggybase-0.0.34/
+-rw-r--r--   0 wsk        (501) staff       (20)    11357 2023-04-10 04:07:02.000000 jiggybase-0.0.34/LICENSE
+-rw-r--r--   0 wsk        (501) staff       (20)     6813 2023-05-20 00:43:09.325201 jiggybase-0.0.34/PKG-INFO
+-rw-r--r--   0 wsk        (501) staff       (20)     6279 2023-05-15 02:51:01.000000 jiggybase-0.0.34/README.md
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-20 00:43:09.316613 jiggybase-0.0.34/jiggybase/
+-rw-r--r--   0 wsk        (501) staff       (20)       30 2023-04-28 15:28:30.000000 jiggybase-0.0.34/jiggybase/__init__.py
+-rw-r--r--   0 wsk        (501) staff       (20)      989 2023-05-15 14:54:50.000000 jiggybase-0.0.34/jiggybase/chat_stream.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2317 2023-05-16 01:07:05.000000 jiggybase-0.0.34/jiggybase/client.py
+-rw-r--r--   0 wsk        (501) staff       (20)    11142 2023-05-19 02:24:06.000000 jiggybase-0.0.34/jiggybase/collection.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-20 00:43:09.319562 jiggybase-0.0.34/jiggybase/examples/
+-rw-r--r--   0 wsk        (501) staff       (20)     1378 2023-05-15 15:42:51.000000 jiggybase-0.0.34/jiggybase/examples/chat_completion.py
+-rw-r--r--   0 wsk        (501) staff       (20)      295 2023-05-15 15:35:06.000000 jiggybase-0.0.34/jiggybase/examples/chat_completion_stream.py
+-rwxr-xr-x   0 wsk        (501) staff       (20)     3381 2023-05-05 04:06:34.000000 jiggybase-0.0.34/jiggybase/examples/jiggybase_upload.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1361 2023-05-03 07:37:11.000000 jiggybase-0.0.34/jiggybase/examples/upload_email_example.py
+-rw-r--r--   0 wsk        (501) staff       (20)     5705 2023-05-15 15:27:23.000000 jiggybase-0.0.34/jiggybase/jiggybase_session.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1187 2023-03-30 18:09:13.000000 jiggybase-0.0.34/jiggybase/login.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-20 00:43:09.324322 jiggybase-0.0.34/jiggybase/models/
+-rw-r--r--   0 wsk        (501) staff       (20)      273 2023-04-26 01:37:49.000000 jiggybase-0.0.34/jiggybase/models/__init__.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1236 2023-04-10 05:17:32.000000 jiggybase-0.0.34/jiggybase/models/auth.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2767 2023-05-15 16:07:13.000000 jiggybase-0.0.34/jiggybase/models/chat.py
+-rw-r--r--   0 wsk        (501) staff       (20)      188 2023-05-15 03:37:46.000000 jiggybase-0.0.34/jiggybase/models/chatmodel.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1322 2023-04-10 16:54:34.000000 jiggybase-0.0.34/jiggybase/models/chunk.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4240 2023-04-20 21:45:37.000000 jiggybase-0.0.34/jiggybase/models/collection.py
+-rw-r--r--   0 wsk        (501) staff       (20)      454 2023-04-23 05:06:00.000000 jiggybase-0.0.34/jiggybase/models/embedding.py
+-rw-r--r--   0 wsk        (501) staff       (20)      696 2023-04-10 04:48:20.000000 jiggybase-0.0.34/jiggybase/models/metadata.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2214 2023-04-10 04:58:39.000000 jiggybase-0.0.34/jiggybase/models/org.py
+-rw-r--r--   0 wsk        (501) staff       (20)     3206 2023-05-20 00:39:05.000000 jiggybase-0.0.34/jiggybase/models/plugin.py
+-rw-r--r--   0 wsk        (501) staff       (20)     3415 2023-05-04 23:56:42.000000 jiggybase-0.0.34/jiggybase/models/plugin_config.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2834 2023-04-22 23:44:02.000000 jiggybase-0.0.34/jiggybase/models/prompt.py
+-rw-r--r--   0 wsk        (501) staff       (20)     3012 2023-04-11 17:29:49.000000 jiggybase-0.0.34/jiggybase/models/providers.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1820 2023-04-17 16:14:19.000000 jiggybase-0.0.34/jiggybase/models/user.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4600 2023-04-29 15:22:54.000000 jiggybase-0.0.34/jiggybase/org.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-20 00:43:09.318302 jiggybase-0.0.34/jiggybase.egg-info/
+-rw-r--r--   0 wsk        (501) staff       (20)     6813 2023-05-20 00:43:09.000000 jiggybase-0.0.34/jiggybase.egg-info/PKG-INFO
+-rw-r--r--   0 wsk        (501) staff       (20)      960 2023-05-20 00:43:09.000000 jiggybase-0.0.34/jiggybase.egg-info/SOURCES.txt
+-rw-r--r--   0 wsk        (501) staff       (20)        1 2023-05-20 00:43:09.000000 jiggybase-0.0.34/jiggybase.egg-info/dependency_links.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       78 2023-05-20 00:43:09.000000 jiggybase-0.0.34/jiggybase.egg-info/entry_points.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       32 2023-05-20 00:43:09.000000 jiggybase-0.0.34/jiggybase.egg-info/requires.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       10 2023-05-20 00:43:09.000000 jiggybase-0.0.34/jiggybase.egg-info/top_level.txt
+-rw-r--r--   0 wsk        (501) staff       (20)      752 2023-05-20 00:39:32.000000 jiggybase-0.0.34/pyproject.toml
+-rw-r--r--   0 wsk        (501) staff       (20)       38 2023-05-20 00:43:09.325782 jiggybase-0.0.34/setup.cfg
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-20 00:43:09.324625 jiggybase-0.0.34/test/
+-rw-r--r--   0 wsk        (501) staff       (20)      830 2023-04-28 15:38:35.000000 jiggybase-0.0.34/test/test.py
```

### Comparing `jiggybase-0.0.33/LICENSE` & `jiggybase-0.0.34/LICENSE`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.33/PKG-INFO` & `jiggybase-0.0.34/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jiggybase
-Version: 0.0.33
+Version: 0.0.34
 Summary: Client for Jiggy AI JiggyBase, including ChatGPT Retriever Plugins
 Author-email: Bill Kish <bk@jiggy.ai>
 Project-URL: Homepage, https://github.com/jiggy-ai/jiggybase
 Project-URL: Bug Tracker, https://github.com/jiggy-ai/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `jiggybase-0.0.33/README.md` & `jiggybase-0.0.34/README.md`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.33/jiggybase/chat_stream.py` & `jiggybase-0.0.34/jiggybase/chat_stream.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.33/jiggybase/client.py` & `jiggybase-0.0.34/jiggybase/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -50,29 +50,24 @@
         resp = self.session.post("/orgs", json={"name":name})
         return Org(self.session, **resp.json())
 
     def collections(self) -> List[Collection]:
         """
         return all Collections in all Orgs that the user is a member of
         """
-        collections = []
-        for org in self.orgs():
-            for collection in org.collections():
-                collections.append(collection)
-        return collections
-
+        resp = self.session.get("/collections")
+        return [Collection(self.session, **c) for c in resp.json()]
+   
     def collection_names(self) -> List[Collection]:
         """
         return the unique collection name for all collections in all Orgs that the user is a member of
         """
-        names = []
-        for org in self.orgs():
-            for collection in org.collections():
-                names.append(collection.name)
-        return names
+        return [c.name for c in self.collections()]
             
-    def collection(self, name : str) -> Collection:
-        for org in self.orgs():
-            for collection in org.collections():
-                if collection.name == name:
-                    return collection
+    def collection(self, name : str) -> Collection:        
+        """
+        return a collection of the specified name
+        """
+        for collection in self.collections():
+            if collection.name == name or collection.display_name.lower() == name.lower():
+                return collection
         raise ValueError(f'Collection "{name}" not found')
```

### Comparing `jiggybase-0.0.33/jiggybase/collection.py` & `jiggybase-0.0.34/jiggybase/collection.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 from pydantic import BaseModel, Field, BaseConfig, HttpUrl
 from enum import Enum
 from .models import collection, CollectionChatConfig, PatchCollectionChatConfig
 from .jiggybase_session import JiggyBaseSession
 from .models import UpsertResponse,  Query, QueryRequest, QueryResponse, UpsertRequest, Document, DocumentChunk, DeleteRequest, DeleteResponse, DocumentMetadataFilter, DocChunksResponse
 from .models import Message, CompletionRequest, ChatCompletion, ChatUsage
 from .chat_stream import extract_content_from_sse_bytes
+from .models import ExtractMetadataConfig
+
 
 from typing import Union, List
 class PluginAuthType(Enum):
     bearer :str = "bearer"
     none   :str = "none"
     oauth  :str = "oauth"
 
@@ -212,8 +214,21 @@
                                max_tokens  = max_tokens,
                                temperature = temperature,
                                stream      = True)
         rsp = self.chat_session.post("/chat/completions", model=cr, stream=True)
         for line in rsp.iter_lines():
             if line:  # filter out keep-alive newlines        
                 yield extract_content_from_sse_bytes(line)
-                
+
+    def get_extract_metadata_config(self):
+        """
+        Get the metadata configuration for this collection.
+        """
+        rsp = self.session.get(f"/orgs/{self.org_id}/collections/{self.id}/extract_metadata_config")
+        return ExtractMetadataConfig(**rsp.json())
+
+    def patch_extract_metadata_config(self, config: ExtractMetadataConfig):
+        """
+        Get the metadata configuration for this collection.
+        """
+        rsp = self.session.patch(f"/orgs/{self.org_id}/collections/{self.id}/extract_metadata_config", model=config)
+        return ExtractMetadataConfig(**rsp.json())
```

### Comparing `jiggybase-0.0.33/jiggybase/examples/chat_completion.py` & `jiggybase-0.0.34/jiggybase/examples/chat_completion.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.33/jiggybase/examples/jiggybase_upload.py` & `jiggybase-0.0.34/jiggybase/examples/jiggybase_upload.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.33/jiggybase/examples/upload_email_example.py` & `jiggybase-0.0.34/jiggybase/examples/upload_email_example.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.33/jiggybase/jiggybase_session.py` & `jiggybase-0.0.34/jiggybase/jiggybase_session.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.33/jiggybase/login.py` & `jiggybase-0.0.34/jiggybase/login.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.33/jiggybase/models/auth.py` & `jiggybase-0.0.34/jiggybase/models/auth.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.33/jiggybase/models/chat.py` & `jiggybase-0.0.34/jiggybase/models/chat.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.33/jiggybase/models/chunk.py` & `jiggybase-0.0.34/jiggybase/models/chunk.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.33/jiggybase/models/collection.py` & `jiggybase-0.0.34/jiggybase/models/collection.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.33/jiggybase/models/metadata.py` & `jiggybase-0.0.34/jiggybase/models/metadata.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.33/jiggybase/models/org.py` & `jiggybase-0.0.34/jiggybase/models/org.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.33/jiggybase/models/plugin.py` & `jiggybase-0.0.34/jiggybase/models/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
 class DocumentChunk(BaseModel):
     id: Optional[str] = None
     text: str
     metadata: DocumentChunkMetadata
     embedding: Optional[list[float]] = None
     token_count: Optional[int] = None
+    reference_url: Optional[str] = None
 
     def __str__(self):
         if len(self.text) > 100:
             text = self.text[:100] + '...'
         else: 
             text = self.text
         text = text.replace('\n', ' ')
```

### Comparing `jiggybase-0.0.33/jiggybase/models/plugin_config.py` & `jiggybase-0.0.34/jiggybase/models/plugin_config.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.33/jiggybase/models/prompt.py` & `jiggybase-0.0.34/jiggybase/models/prompt.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.33/jiggybase/models/providers.py` & `jiggybase-0.0.34/jiggybase/models/providers.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.33/jiggybase/models/user.py` & `jiggybase-0.0.34/jiggybase/models/user.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.33/jiggybase/org.py` & `jiggybase-0.0.34/jiggybase/org.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.33/jiggybase.egg-info/PKG-INFO` & `jiggybase-0.0.34/jiggybase.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jiggybase
-Version: 0.0.33
+Version: 0.0.34
 Summary: Client for Jiggy AI JiggyBase, including ChatGPT Retriever Plugins
 Author-email: Bill Kish <bk@jiggy.ai>
 Project-URL: Homepage, https://github.com/jiggy-ai/jiggybase
 Project-URL: Bug Tracker, https://github.com/jiggy-ai/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `jiggybase-0.0.33/jiggybase.egg-info/SOURCES.txt` & `jiggybase-0.0.34/jiggybase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.33/pyproject.toml` & `jiggybase-0.0.34/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jiggybase"
-version = "0.0.33"
+version = "0.0.34"
 authors = [
   { name="Bill Kish", email="bk@jiggy.ai" },
 ]
 dependencies=['loguru', 'pydantic[email]', 'requests']
 description = "Client for Jiggy AI JiggyBase, including ChatGPT Retriever Plugins"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `jiggybase-0.0.33/test/test.py` & `jiggybase-0.0.34/test/test.py`

 * *Files identical despite different names*

