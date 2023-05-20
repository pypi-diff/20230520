# Comparing `tmp/embedbase-1.1.8.tar.gz` & `tmp/embedbase-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedbase-1.1.8.tar", max compression
+gzip compressed data, was "embedbase-1.1.9.tar", max compression
```

## Comparing `embedbase-1.1.8.tar` & `embedbase-1.1.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1069 2023-05-20 07:25:48.328072 embedbase-1.1.8/LICENSE
--rw-r--r--   0        0        0     4905 2023-05-20 07:25:48.328072 embedbase-1.1.8/README.md
--rw-r--r--   0        0        0      121 2023-05-20 07:25:48.444070 embedbase-1.1.8/embedbase/__init__.py
--rw-r--r--   0        0        0     1716 2023-05-20 07:25:48.444070 embedbase-1.1.8/embedbase/__main__.py
--rw-r--r--   0        0        0      976 2023-05-20 07:25:48.444070 embedbase-1.1.8/embedbase/api.py
--rw-r--r--   0        0        0    17880 2023-05-20 07:25:48.444070 embedbase-1.1.8/embedbase/app.py
--rw-r--r--   0        0        0       88 2023-05-20 07:25:48.444070 embedbase-1.1.8/embedbase/database/__init__.py
--rw-r--r--   0        0        0     3400 2023-05-20 07:25:48.444070 embedbase-1.1.8/embedbase/database/base.py
--rw-r--r--   0        0        0     6218 2023-05-20 07:25:48.444070 embedbase-1.1.8/embedbase/database/memory_db.py
--rw-r--r--   0        0        0    10189 2023-05-20 07:25:48.444070 embedbase-1.1.8/embedbase/database/postgres_db.py
--rw-r--r--   0        0        0     7579 2023-05-20 07:25:48.444070 embedbase-1.1.8/embedbase/database/supabase_db.py
--rw-r--r--   0        0        0       77 2023-05-20 07:25:48.444070 embedbase-1.1.8/embedbase/embedding/__init__.py
--rw-r--r--   0        0        0      858 2023-05-20 07:25:48.444070 embedbase-1.1.8/embedbase/embedding/base.py
--rw-r--r--   0        0        0     1237 2023-05-20 07:25:48.444070 embedbase-1.1.8/embedbase/embedding/cohere.py
--rw-r--r--   0        0        0     2059 2023-05-20 07:25:48.444070 embedbase-1.1.8/embedbase/embedding/openai.py
--rw-r--r--   0        0        0     1551 2023-05-20 07:25:48.444070 embedbase-1.1.8/embedbase/firebase_auth.py
--rw-r--r--   0        0        0      690 2023-05-20 07:25:48.444070 embedbase-1.1.8/embedbase/logging_utils.py
--rw-r--r--   0        0        0      955 2023-05-20 07:25:48.444070 embedbase-1.1.8/embedbase/models.py
--rw-r--r--   0        0        0     1285 2023-05-20 07:25:48.444070 embedbase-1.1.8/embedbase/settings.py
--rw-r--r--   0        0        0     3208 2023-05-20 07:25:48.444070 embedbase-1.1.8/embedbase/strings.py
--rw-r--r--   0        0        0      301 2023-05-20 07:25:48.444070 embedbase-1.1.8/embedbase/supabase_auth.py
--rw-r--r--   0        0        0     3867 2023-05-20 07:25:48.444070 embedbase-1.1.8/embedbase/utils.py
--rw-r--r--   0        0        0     3666 2023-05-20 07:25:48.448070 embedbase-1.1.8/pyproject.toml
--rw-r--r--   0        0        0     6138 1970-01-01 00:00:00.000000 embedbase-1.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-20 09:06:52.366709 embedbase-1.1.9/LICENSE
+-rw-r--r--   0        0        0     4905 2023-05-20 09:06:52.366709 embedbase-1.1.9/README.md
+-rw-r--r--   0        0        0      121 2023-05-20 09:06:52.498710 embedbase-1.1.9/embedbase/__init__.py
+-rw-r--r--   0        0        0     1716 2023-05-20 09:06:52.498710 embedbase-1.1.9/embedbase/__main__.py
+-rw-r--r--   0        0        0      976 2023-05-20 09:06:52.498710 embedbase-1.1.9/embedbase/api.py
+-rw-r--r--   0        0        0    17884 2023-05-20 09:06:52.498710 embedbase-1.1.9/embedbase/app.py
+-rw-r--r--   0        0        0       88 2023-05-20 09:06:52.498710 embedbase-1.1.9/embedbase/database/__init__.py
+-rw-r--r--   0        0        0     3406 2023-05-20 09:06:52.498710 embedbase-1.1.9/embedbase/database/base.py
+-rw-r--r--   0        0        0     6220 2023-05-20 09:06:52.498710 embedbase-1.1.9/embedbase/database/memory_db.py
+-rw-r--r--   0        0        0    10191 2023-05-20 09:06:52.498710 embedbase-1.1.9/embedbase/database/postgres_db.py
+-rw-r--r--   0        0        0     7585 2023-05-20 09:06:52.498710 embedbase-1.1.9/embedbase/database/supabase_db.py
+-rw-r--r--   0        0        0       77 2023-05-20 09:06:52.498710 embedbase-1.1.9/embedbase/embedding/__init__.py
+-rw-r--r--   0        0        0      858 2023-05-20 09:06:52.502710 embedbase-1.1.9/embedbase/embedding/base.py
+-rw-r--r--   0        0        0     1237 2023-05-20 09:06:52.502710 embedbase-1.1.9/embedbase/embedding/cohere.py
+-rw-r--r--   0        0        0     2059 2023-05-20 09:06:52.502710 embedbase-1.1.9/embedbase/embedding/openai.py
+-rw-r--r--   0        0        0     1551 2023-05-20 09:06:52.502710 embedbase-1.1.9/embedbase/firebase_auth.py
+-rw-r--r--   0        0        0      690 2023-05-20 09:06:52.502710 embedbase-1.1.9/embedbase/logging_utils.py
+-rw-r--r--   0        0        0      955 2023-05-20 09:06:52.502710 embedbase-1.1.9/embedbase/models.py
+-rw-r--r--   0        0        0     1285 2023-05-20 09:06:52.502710 embedbase-1.1.9/embedbase/settings.py
+-rw-r--r--   0        0        0     3208 2023-05-20 09:06:52.502710 embedbase-1.1.9/embedbase/strings.py
+-rw-r--r--   0        0        0      301 2023-05-20 09:06:52.502710 embedbase-1.1.9/embedbase/supabase_auth.py
+-rw-r--r--   0        0        0     3867 2023-05-20 09:06:52.502710 embedbase-1.1.9/embedbase/utils.py
+-rw-r--r--   0        0        0     3666 2023-05-20 09:06:52.502710 embedbase-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0     6138 1970-01-01 00:00:00.000000 embedbase-1.1.9/PKG-INFO
```

### Comparing `embedbase-1.1.8/LICENSE` & `embedbase-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.8/README.md` & `embedbase-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.8/embedbase/__main__.py` & `embedbase-1.1.9/embedbase/__main__.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.8/embedbase/api.py` & `embedbase-1.1.9/embedbase/api.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.8/embedbase/app.py` & `embedbase-1.1.9/embedbase/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -469,23 +469,23 @@
                 **self._base_return(),
                 "datasets": [e.dict() for e in datasets],
             },
         )
 
     # TODO where filter for list?
     async def list(
-        self, request: Request, dataset_id: str, page: int = 0, limit: int = 100
+        self, request: Request, dataset_id: str, offset: int = 0, limit: int = 100
     ):
         """
         Return a list of documents in the dataset.
         As a large language model, you can use this endpoint to see what documents you have
         and how many documents are in each.
         """
         user_id = get_user_id(request)
-        documents = await self.db.list(dataset_id, user_id, page, limit)
+        documents = await self.db.list(dataset_id, user_id, offset, limit)
         return JSONResponse(
             status_code=status.HTTP_200_OK,
             content={
                 **self._base_return(dataset_id),
                 "documents": [e.dict() for e in documents],
             },
         )
```

### Comparing `embedbase-1.1.8/embedbase/database/base.py` & `embedbase-1.1.9/embedbase/database/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,19 +114,19 @@
         raise NotImplementedError
 
     @abstractmethod
     async def list(
         self,
         dataset_id: str,
         user_id: Optional[str] = None,
-        page: int = 0,
+        offset: int = 0,
         limit: int = 100,
     ) -> List[Document]:
         """
         Returns a list of Documents in a dataset
         :param dataset_id: dataset id
         :param user_id: user id
-        :param page: page
+        :param offset: offset
         :param limit: limit
         :return: list of documents
         """
         raise NotImplementedError
```

### Comparing `embedbase-1.1.8/embedbase/database/memory_db.py` & `embedbase-1.1.9/embedbase/database/memory_db.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,11 +179,11 @@
         for doc_id in doc_ids_to_remove:
             del self.storage[doc_id]
 
     async def list(
         self,
         dataset_id: str,
         user_id: Optional[str] = None,
-        page: int = 0,
+        offset: int = 0,
         limit: int = 100,
     ) -> List[Document]:
         raise NotImplementedError
```

### Comparing `embedbase-1.1.8/embedbase/database/postgres_db.py` & `embedbase-1.1.9/embedbase/database/postgres_db.py`

 * *Files 1% similar despite different names*

```diff
@@ -311,11 +311,11 @@
             )
         return data
 
     async def list(
         self,
         dataset_id: str,
         user_id: Optional[str] = None,
-        page: int = 0,
+        offset: int = 0,
         limit: int = 100,
     ) -> List[Document]:
         raise NotImplementedError
```

### Comparing `embedbase-1.1.8/embedbase/database/supabase_db.py` & `embedbase-1.1.9/embedbase/database/supabase_db.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,21 +203,21 @@
             for row in data
         ]
 
     async def list(
         self,
         dataset_id: str,
         user_id: Optional[str] = None,
-        page: int = 0,
+        offset: int = 0,
         limit: int = 100,
     ) -> List[Document]:
         req = self.supabase.table("documents").select("*").eq("dataset_id", dataset_id)
         if user_id:
             req = req.eq("user_id", user_id)
-        req = req.range(page * limit, (page + 1) * limit)
+        req = req.range(offset * limit, (offset + 1) * limit)
         data = req.execute().data
         return [
             Document(
                 id=row["id"],
                 data=row["data"],
                 embedding=ast.literal_eval(row["embedding"]),
                 hash=row["hash"],
```

### Comparing `embedbase-1.1.8/embedbase/embedding/base.py` & `embedbase-1.1.9/embedbase/embedding/base.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.8/embedbase/embedding/cohere.py` & `embedbase-1.1.9/embedbase/embedding/cohere.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.8/embedbase/embedding/openai.py` & `embedbase-1.1.9/embedbase/embedding/openai.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.8/embedbase/firebase_auth.py` & `embedbase-1.1.9/embedbase/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.8/embedbase/logging_utils.py` & `embedbase-1.1.9/embedbase/logging_utils.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.8/embedbase/models.py` & `embedbase-1.1.9/embedbase/models.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.8/embedbase/settings.py` & `embedbase-1.1.9/embedbase/settings.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.8/embedbase/strings.py` & `embedbase-1.1.9/embedbase/strings.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.8/embedbase/utils.py` & `embedbase-1.1.9/embedbase/utils.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.8/pyproject.toml` & `embedbase-1.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "embedbase"
-version = "1.1.8"
+version = "1.1.9"
 description = "Open-source API & SDK to integrate your data and easily hook them up to LLMs."
 readme = "README.md"
 authors = ["Different AI <louis@embedbase.xyz>"]
 license = "MIT"
 repository = "https://github.com/different-ai/embedbase"
 homepage = "https://github.com/different-ai/embedbase"
 keywords = ["embeddings", "machine learning", "artificial intelligence", "llm"]
```

### Comparing `embedbase-1.1.8/PKG-INFO` & `embedbase-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedbase
-Version: 1.1.8
+Version: 1.1.9
 Summary: Open-source API & SDK to integrate your data and easily hook them up to LLMs.
 Home-page: https://github.com/different-ai/embedbase
 License: MIT
 Keywords: embeddings,machine learning,artificial intelligence,llm
 Author: Different AI
 Author-email: louis@embedbase.xyz
 Requires-Python: >=3.8,<4.0
```

