# Comparing `tmp/embedbase-1.1.7.tar.gz` & `tmp/embedbase-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedbase-1.1.7.tar", max compression
+gzip compressed data, was "embedbase-1.1.8.tar", max compression
```

## Comparing `embedbase-1.1.7.tar` & `embedbase-1.1.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1069 2023-05-17 08:43:33.430248 embedbase-1.1.7/LICENSE
--rw-r--r--   0        0        0     4905 2023-05-17 08:43:33.430248 embedbase-1.1.7/README.md
--rw-r--r--   0        0        0      121 2023-05-17 08:43:33.498248 embedbase-1.1.7/embedbase/__init__.py
--rw-r--r--   0        0        0     1716 2023-05-17 08:43:33.498248 embedbase-1.1.7/embedbase/__main__.py
--rw-r--r--   0        0        0      976 2023-05-17 08:43:33.498248 embedbase-1.1.7/embedbase/api.py
--rw-r--r--   0        0        0    17076 2023-05-17 08:43:33.498248 embedbase-1.1.7/embedbase/app.py
--rw-r--r--   0        0        0       88 2023-05-17 08:43:33.498248 embedbase-1.1.7/embedbase/database/__init__.py
--rw-r--r--   0        0        0     3505 2023-05-17 08:43:33.498248 embedbase-1.1.7/embedbase/database/base.py
--rw-r--r--   0        0        0     5939 2023-05-17 08:43:33.498248 embedbase-1.1.7/embedbase/database/memory_db.py
--rw-r--r--   0        0        0     9903 2023-05-17 08:43:33.498248 embedbase-1.1.7/embedbase/database/postgres_db.py
--rw-r--r--   0        0        0     6873 2023-05-17 08:43:33.498248 embedbase-1.1.7/embedbase/database/supabase_db.py
--rw-r--r--   0        0        0       77 2023-05-17 08:43:33.498248 embedbase-1.1.7/embedbase/embedding/__init__.py
--rw-r--r--   0        0        0      858 2023-05-17 08:43:33.498248 embedbase-1.1.7/embedbase/embedding/base.py
--rw-r--r--   0        0        0     1237 2023-05-17 08:43:33.498248 embedbase-1.1.7/embedbase/embedding/cohere.py
--rw-r--r--   0        0        0     2059 2023-05-17 08:43:33.498248 embedbase-1.1.7/embedbase/embedding/openai.py
--rw-r--r--   0        0        0     1551 2023-05-17 08:43:33.498248 embedbase-1.1.7/embedbase/firebase_auth.py
--rw-r--r--   0        0        0      690 2023-05-17 08:43:33.498248 embedbase-1.1.7/embedbase/logging_utils.py
--rw-r--r--   0        0        0      802 2023-05-17 08:43:33.498248 embedbase-1.1.7/embedbase/models.py
--rw-r--r--   0        0        0     1285 2023-05-17 08:43:33.498248 embedbase-1.1.7/embedbase/settings.py
--rw-r--r--   0        0        0     3208 2023-05-17 08:43:33.498248 embedbase-1.1.7/embedbase/strings.py
--rw-r--r--   0        0        0      301 2023-05-17 08:43:33.498248 embedbase-1.1.7/embedbase/supabase_auth.py
--rw-r--r--   0        0        0     3867 2023-05-17 08:43:33.498248 embedbase-1.1.7/embedbase/utils.py
--rw-r--r--   0        0        0     3666 2023-05-17 08:43:33.502248 embedbase-1.1.7/pyproject.toml
--rw-r--r--   0        0        0     6337 1970-01-01 00:00:00.000000 embedbase-1.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-20 07:25:48.328072 embedbase-1.1.8/LICENSE
+-rw-r--r--   0        0        0     4905 2023-05-20 07:25:48.328072 embedbase-1.1.8/README.md
+-rw-r--r--   0        0        0      121 2023-05-20 07:25:48.444070 embedbase-1.1.8/embedbase/__init__.py
+-rw-r--r--   0        0        0     1716 2023-05-20 07:25:48.444070 embedbase-1.1.8/embedbase/__main__.py
+-rw-r--r--   0        0        0      976 2023-05-20 07:25:48.444070 embedbase-1.1.8/embedbase/api.py
+-rw-r--r--   0        0        0    17880 2023-05-20 07:25:48.444070 embedbase-1.1.8/embedbase/app.py
+-rw-r--r--   0        0        0       88 2023-05-20 07:25:48.444070 embedbase-1.1.8/embedbase/database/__init__.py
+-rw-r--r--   0        0        0     3400 2023-05-20 07:25:48.444070 embedbase-1.1.8/embedbase/database/base.py
+-rw-r--r--   0        0        0     6218 2023-05-20 07:25:48.444070 embedbase-1.1.8/embedbase/database/memory_db.py
+-rw-r--r--   0        0        0    10189 2023-05-20 07:25:48.444070 embedbase-1.1.8/embedbase/database/postgres_db.py
+-rw-r--r--   0        0        0     7579 2023-05-20 07:25:48.444070 embedbase-1.1.8/embedbase/database/supabase_db.py
+-rw-r--r--   0        0        0       77 2023-05-20 07:25:48.444070 embedbase-1.1.8/embedbase/embedding/__init__.py
+-rw-r--r--   0        0        0      858 2023-05-20 07:25:48.444070 embedbase-1.1.8/embedbase/embedding/base.py
+-rw-r--r--   0        0        0     1237 2023-05-20 07:25:48.444070 embedbase-1.1.8/embedbase/embedding/cohere.py
+-rw-r--r--   0        0        0     2059 2023-05-20 07:25:48.444070 embedbase-1.1.8/embedbase/embedding/openai.py
+-rw-r--r--   0        0        0     1551 2023-05-20 07:25:48.444070 embedbase-1.1.8/embedbase/firebase_auth.py
+-rw-r--r--   0        0        0      690 2023-05-20 07:25:48.444070 embedbase-1.1.8/embedbase/logging_utils.py
+-rw-r--r--   0        0        0      955 2023-05-20 07:25:48.444070 embedbase-1.1.8/embedbase/models.py
+-rw-r--r--   0        0        0     1285 2023-05-20 07:25:48.444070 embedbase-1.1.8/embedbase/settings.py
+-rw-r--r--   0        0        0     3208 2023-05-20 07:25:48.444070 embedbase-1.1.8/embedbase/strings.py
+-rw-r--r--   0        0        0      301 2023-05-20 07:25:48.444070 embedbase-1.1.8/embedbase/supabase_auth.py
+-rw-r--r--   0        0        0     3867 2023-05-20 07:25:48.444070 embedbase-1.1.8/embedbase/utils.py
+-rw-r--r--   0        0        0     3666 2023-05-20 07:25:48.448070 embedbase-1.1.8/pyproject.toml
+-rw-r--r--   0        0        0     6138 1970-01-01 00:00:00.000000 embedbase-1.1.8/PKG-INFO
```

### Comparing `embedbase-1.1.7/LICENSE` & `embedbase-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.7/README.md` & `embedbase-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.7/embedbase/__main__.py` & `embedbase-1.1.8/embedbase/__main__.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.7/embedbase/api.py` & `embedbase-1.1.8/embedbase/api.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.7/embedbase/app.py` & `embedbase-1.1.8/embedbase/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -467,14 +467,33 @@
             status_code=status.HTTP_200_OK,
             content={
                 **self._base_return(),
                 "datasets": [e.dict() for e in datasets],
             },
         )
 
+    # TODO where filter for list?
+    async def list(
+        self, request: Request, dataset_id: str, page: int = 0, limit: int = 100
+    ):
+        """
+        Return a list of documents in the dataset.
+        As a large language model, you can use this endpoint to see what documents you have
+        and how many documents are in each.
+        """
+        user_id = get_user_id(request)
+        documents = await self.db.list(dataset_id, user_id, page, limit)
+        return JSONResponse(
+            status_code=status.HTTP_200_OK,
+            content={
+                **self._base_return(dataset_id),
+                "documents": [e.dict() for e in documents],
+            },
+        )
+
     # health check endpoint
     def health(self, _: Request):
         """
         Return the status of the API.
         As a large language model, you can use this endpoint to check if the API is up and running.
         """
         self.logger.info("Health check successful")
@@ -505,11 +524,14 @@
         )
         self.fastapi_app.add_api_route(
             "/v1/{dataset_id}/search", self.semantic_search, methods=["POST"]
         )
         self.fastapi_app.add_api_route(
             "/v1/datasets", self.get_datasets, methods=["GET"]
         )
+        self.fastapi_app.add_api_route(
+            "/v1/{dataset_id}", self.list, methods=["GET"]
+        )
         self.fastapi_app.add_api_route("/health", self.health, methods=["GET"])
         print(embedbase_ascii)
 
         return self.fastapi_app
```

### Comparing `embedbase-1.1.7/embedbase/database/base.py` & `embedbase-1.1.8/embedbase/database/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,29 @@
-from abc import ABC, abstractmethod
 from typing import Coroutine, List, Optional, Union
+
+from abc import ABC, abstractmethod
+
 from pandas import DataFrame
 from pydantic import BaseModel
 
+from embedbase.models import Document
+
 
 # TODO use pydantic validation
 class Dataset(BaseModel):
     dataset_id: str
     documents_count: int
 
 
-class SearchResponse(BaseModel):
+class SearchResponse(Document):
     score: float
-    id: str
-    # data-privacy aware setup avoid storing data on the database
-    # and rather store it on the client side
-    data: Optional[str]
-    hash: str
-    # HACK supabase pgvector returns a string of float '[0.1, 0.2, ...]' not sure its
-    # any inconvenience for now. Let's see if we can fix this later
-    embedding: Union[List[float], str]
-    metadata: Optional[dict]
-
-
-class SelectResponse(BaseModel):
-    id: str
-    # data-privacy aware setup avoid storing data on the database
-    # and rather store it on the client side
-    data: Optional[str]
-    hash: str
-    embedding: Union[List[float], str]
-    metadata: Optional[dict]
+
+
+class SelectResponse(Document):
+    pass
 
 
 class VectorDatabase(ABC):
     """
     Base class for all vector databases
     """
 
@@ -119,7 +108,25 @@
     @abstractmethod
     async def get_datasets(self, user_id: Optional[str] = None) -> List[Dataset]:
         """
         :param user_id: user id
         :return: list of datasets
         """
         raise NotImplementedError
+
+    @abstractmethod
+    async def list(
+        self,
+        dataset_id: str,
+        user_id: Optional[str] = None,
+        page: int = 0,
+        limit: int = 100,
+    ) -> List[Document]:
+        """
+        Returns a list of Documents in a dataset
+        :param dataset_id: dataset id
+        :param user_id: user id
+        :param page: page
+        :param limit: limit
+        :return: list of documents
+        """
+        raise NotImplementedError
```

### Comparing `embedbase-1.1.7/embedbase/database/memory_db.py` & `embedbase-1.1.8/embedbase/database/memory_db.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+from typing import List, Optional
 from embedbase.database.base import (
     Dataset,
     SearchResponse,
     SelectResponse,
     VectorDatabase,
 )
+from embedbase.models import Document
 
 
 # Calculate cosine similarity
 def cosine_similarity(np, a, b):
     return np.dot(a, b) / (np.linalg.norm(a) * np.linalg.norm(b))
 
 
@@ -172,7 +174,16 @@
             doc_id
             for doc_id, doc in self.storage.items()
             if doc["dataset_id"] == dataset_id
             and (user_id is None or doc["user_id"] == user_id)
         ]
         for doc_id in doc_ids_to_remove:
             del self.storage[doc_id]
+
+    async def list(
+        self,
+        dataset_id: str,
+        user_id: Optional[str] = None,
+        page: int = 0,
+        limit: int = 100,
+    ) -> List[Document]:
+        raise NotImplementedError
```

### Comparing `embedbase-1.1.7/embedbase/database/postgres_db.py` & `embedbase-1.1.8/embedbase/database/postgres_db.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-import asyncio
-import json
 from typing import List, Optional
+
+import asyncio
 import itertools
+import json
+
 from pandas import DataFrame, Series
 
 from embedbase.database import VectorDatabase
 from embedbase.database.base import Dataset, SearchResponse, SelectResponse
+from embedbase.models import Document
 
 
 class Postgres(VectorDatabase):
     def __init__(
         self, conn_str="postgresql://postgres:localdb@0.0.0.0/embedbase", **kwargs
     ):
         """
@@ -145,33 +148,33 @@
                     conditions.append(
                         sql.SQL("dataset_id = {}").format(sql.Literal(dataset_id))
                     )
                 if user_id:
                     conditions.append(
                         sql.SQL("user_id = {}").format(sql.Literal(user_id))
                     )
-                return list(self.conn.execute(
-                    sql.SQL(query).format(conditions=sql.SQL(" and ").join(conditions))
-                ))
+                return list(
+                    self.conn.execute(
+                        sql.SQL(query).format(
+                            conditions=sql.SQL(" and ").join(conditions)
+                        )
+                    )
+                )
             except Exception as e:
                 raise e
 
         # we need to run parallel requests with postgres
         n = 50
         docs = []
         if ids:
             elements = [ids[i : i + n] for i in range(0, len(ids), n)]
-            docs = await asyncio.gather(
-                *[_fetch(e, []) for e in elements]
-            )
+            docs = await asyncio.gather(*[_fetch(e, []) for e in elements])
         else:
             elements = [hashes[i : i + n] for i in range(0, len(hashes), n)]
-            docs = await asyncio.gather(
-                *[_fetch([], e) for e in elements]
-            )
+            docs = await asyncio.gather(*[_fetch([], e) for e in elements])
         return [
             SelectResponse(
                 id=row[0],
                 data=row[1],
                 embedding=row[2].tolist(),
                 hash=row[3],
                 metadata=row[4],
@@ -243,15 +246,14 @@
         self,
         vector: List[float],
         top_k: Optional[int],
         dataset_ids: List[str],
         user_id: Optional[str] = None,
         where=None,
     ):
-
         d = {
             "query_embedding": str(vector),
             "similarity_threshold": 0.0,  # TODO: make this configurable
             "match_count": top_k,
             "query_dataset_ids": dataset_ids,
         }
         q = "select * from match_documents(%(query_embedding)s, %(similarity_threshold)s, %(match_count)s, %(query_dataset_ids)s"
@@ -304,7 +306,16 @@
             data.append(
                 Dataset(
                     dataset_id=row[0],
                     documents_count=row[2],
                 )
             )
         return data
+
+    async def list(
+        self,
+        dataset_id: str,
+        user_id: Optional[str] = None,
+        page: int = 0,
+        limit: int = 100,
+    ) -> List[Document]:
+        raise NotImplementedError
```

### Comparing `embedbase-1.1.7/embedbase/database/supabase_db.py` & `embedbase-1.1.8/embedbase/database/supabase_db.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,35 @@
+from typing import List, Optional
+
+import ast
 import asyncio
 import itertools
-from typing import List, Optional
+
 from pandas import DataFrame, Series
+
 from embedbase.database import VectorDatabase
 from embedbase.database.base import Dataset, SearchResponse, SelectResponse
+from embedbase.models import Document
 from embedbase.utils import BatchGenerator
-import ast
+
 
 class Supabase(VectorDatabase):
     """
     Implements a vector database using supabase
     Supabase is an open source Firebase alternative.
     """
 
     def __init__(self, url: str, key: str, **kwargs):
         """
         :param url: supabase url
         :param key: supabase key
         """
         super().__init__(**kwargs)
         try:
-            from supabase import create_client, Client
+            from supabase import Client, create_client
 
             self.supabase: Client = create_client(url, key)
             self.functions = self.supabase.functions()
 
         except ImportError:
             raise ImportError("Please install supabase with `pip install supabase`")
 
@@ -36,15 +41,17 @@
         user_id: Optional[str] = None,
         distinct: bool = True,
     ):
         # either ids or hashes must be provided
         assert ids or hashes, "ids or hashes must be provided"
 
         # raise if both ids and hashes are provided
-        assert not (ids and hashes), "ids and hashes cannot be provided at the same time"
+        assert not (
+            ids and hashes
+        ), "ids and hashes cannot be provided at the same time"
         # TODO not supported yet
 
         async def _fetch(ids, hashes) -> List[dict]:
             try:
                 req = self.supabase.table("documents").select("*")
                 if ids:
                     req = req.in_("id", ids)
@@ -68,22 +75,18 @@
                 raise e
 
         # we need to run parallel requests with supabase
         n = 50
         docs = []
         if ids:
             elements = [ids[i : i + n] for i in range(0, len(ids), n)]
-            docs = await asyncio.gather(
-                *[_fetch(e, []) for e in elements]
-            )
+            docs = await asyncio.gather(*[_fetch(e, []) for e in elements])
         else:
             elements = [hashes[i : i + n] for i in range(0, len(hashes), n)]
-            docs = await asyncio.gather(
-                *[_fetch([], e) for e in elements]
-            )
+            docs = await asyncio.gather(*[_fetch([], e) for e in elements])
         return [
             SelectResponse(
                 id=row["id"],
                 data=row["data"],
                 embedding=ast.literal_eval(row["embedding"]),
                 hash=row["hash"],
                 metadata=row["metadata"],
@@ -153,28 +156,24 @@
         }
         if user_id:
             d["query_user_id"] = user_id
         query = self.supabase.rpc(
             "match_documents",
             d,
         )
-        
+
         if where:
             # raise if where is not a dict
             if not isinstance(where, dict):
                 raise ValueError("currently only dict is supported for where")
             metadata_field = list(where.keys())[0]
             metadata_value = where[metadata_field]
             d["metadata_field"] = metadata_field
             d["metadata_value"] = metadata_value
-        response = (
-            query
-            .execute()
-            .data
-        )
+        response = query.execute().data
         return [
             SearchResponse(
                 id=row["id"],
                 data=row["data"],
                 embedding=ast.literal_eval(row["embedding"]),
                 hash=row["hash"],
                 metadata=row["metadata"],
@@ -199,7 +198,31 @@
         return [
             Dataset(
                 dataset_id=row["dataset_id"],
                 documents_count=row["documents_count"],
             )
             for row in data
         ]
+
+    async def list(
+        self,
+        dataset_id: str,
+        user_id: Optional[str] = None,
+        page: int = 0,
+        limit: int = 100,
+    ) -> List[Document]:
+        req = self.supabase.table("documents").select("*").eq("dataset_id", dataset_id)
+        if user_id:
+            req = req.eq("user_id", user_id)
+        req = req.range(page * limit, (page + 1) * limit)
+        data = req.execute().data
+        return [
+            Document(
+                id=row["id"],
+                data=row["data"],
+                embedding=ast.literal_eval(row["embedding"]),
+                hash=row["hash"],
+                metadata=row["metadata"],
+                dataset_ids=[row["dataset_id"]],
+            )
+            for row in data
+        ]
```

### Comparing `embedbase-1.1.7/embedbase/embedding/base.py` & `embedbase-1.1.8/embedbase/embedding/base.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.7/embedbase/embedding/cohere.py` & `embedbase-1.1.8/embedbase/embedding/cohere.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.7/embedbase/embedding/openai.py` & `embedbase-1.1.8/embedbase/embedding/openai.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.7/embedbase/firebase_auth.py` & `embedbase-1.1.8/embedbase/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.7/embedbase/logging_utils.py` & `embedbase-1.1.8/embedbase/logging_utils.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.7/embedbase/models.py` & `embedbase-1.1.8/embedbase/models.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,45 @@
 from typing import List, Optional, Union
+
 from pydantic import BaseModel
 
-# TODO: response models once stable
 
 class Document(BaseModel):
+    id: str
+    data: Optional[str]
+    hash: str
+    embedding: Union[List[float], str]
+    metadata: Optional[dict]
+    dataset_ids: List[str] = []
+
+
+class AddDocument(BaseModel):
     # data can be
     # - a string - for example  "This is a document"
     # TODO: currently only string is supported (later could be images, audio, multi/cross-modal)
     # etc.
     data: str
     metadata: Optional[dict]
 
 
 class AddRequest(BaseModel):
-    documents: List[Document]
+    documents: List[AddDocument]
     store_data: bool = True
 
+
 class UpdateDocument(BaseModel):
     id: str
     data: Optional[str] = None
     metadata: Optional[dict] = None
 
+
 class UpdateRequest(BaseModel):
     documents: List[UpdateDocument]
 
+
 class DeleteRequest(BaseModel):
     ids: List[str]
 
 
 class SearchRequest(BaseModel):
     query: str
     top_k: int = 6
```

### Comparing `embedbase-1.1.7/embedbase/settings.py` & `embedbase-1.1.8/embedbase/settings.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.7/embedbase/strings.py` & `embedbase-1.1.8/embedbase/strings.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.7/embedbase/utils.py` & `embedbase-1.1.8/embedbase/utils.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.7/pyproject.toml` & `embedbase-1.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "embedbase"
-version = "1.1.7"
+version = "1.1.8"
 description = "Open-source API & SDK to integrate your data and easily hook them up to LLMs."
 readme = "README.md"
 authors = ["Different AI <louis@embedbase.xyz>"]
 license = "MIT"
 repository = "https://github.com/different-ai/embedbase"
 homepage = "https://github.com/different-ai/embedbase"
 keywords = ["embeddings", "machine learning", "artificial intelligence", "llm"]
```

### Comparing `embedbase-1.1.7/PKG-INFO` & `embedbase-1.1.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedbase
-Version: 1.1.7
+Version: 1.1.8
 Summary: Open-source API & SDK to integrate your data and easily hook them up to LLMs.
 Home-page: https://github.com/different-ai/embedbase
 License: MIT
 Keywords: embeddings,machine learning,artificial intelligence,llm
 Author: Different AI
 Author-email: louis@embedbase.xyz
 Requires-Python: >=3.8,<4.0
@@ -12,18 +12,14 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Dist: fastapi (>=0.95.1,<0.96.0)
 Requires-Dist: openai (>=0.27.0,<0.28.0)
 Requires-Dist: pandas (>=1.3.4,<2.0.0)
 Requires-Dist: pydantic_yaml[pyyaml] (>=0.4.0,<0.5.0)
 Requires-Dist: tenacity (>=8.0.1,<9.0.0)
 Requires-Dist: tiktoken (>=0.3.3,<0.4.0)
```

