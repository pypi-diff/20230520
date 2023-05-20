# Comparing `tmp/paper-qa-1.6.2.tar.gz` & `tmp/paper-qa-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paper-qa-1.6.2.tar", last modified: Thu May 18 03:15:18 2023, max compression
+gzip compressed data, was "paper-qa-1.6.3.tar", last modified: Sat May 20 06:41:14 2023, max compression
```

## Comparing `paper-qa-1.6.2.tar` & `paper-qa-1.6.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:15:18.664700 paper-qa-1.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-18 03:14:41.000000 paper-qa-1.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12585 2023-05-18 03:15:18.664700 paper-qa-1.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12150 2023-05-18 03:14:41.000000 paper-qa-1.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:15:18.660700 paper-qa-1.6.2/paper_qa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12585 2023-05-18 03:15:18.000000 paper-qa-1.6.2/paper_qa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-18 03:15:18.000000 paper-qa-1.6.2/paper_qa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 03:15:18.000000 paper-qa-1.6.2/paper_qa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-18 03:15:18.000000 paper-qa-1.6.2/paper_qa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-18 03:15:18.000000 paper-qa-1.6.2/paper_qa.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:15:18.664700 paper-qa-1.6.2/paperqa/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 03:14:41.000000 paper-qa-1.6.2/paperqa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-05-18 03:14:41.000000 paper-qa-1.6.2/paperqa/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:15:18.664700 paper-qa-1.6.2/paperqa/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-18 03:14:41.000000 paper-qa-1.6.2/paperqa/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-05-18 03:14:41.000000 paper-qa-1.6.2/paperqa/contrib/zotero.py
--rw-r--r--   0 runner    (1001) docker     (123)    20515 2023-05-18 03:14:41.000000 paper-qa-1.6.2/paperqa/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-18 03:14:41.000000 paper-qa-1.6.2/paperqa/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-05-18 03:14:41.000000 paper-qa-1.6.2/paperqa/qaprompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-05-18 03:14:41.000000 paper-qa-1.6.2/paperqa/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-18 03:14:41.000000 paper-qa-1.6.2/paperqa/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-18 03:14:41.000000 paper-qa-1.6.2/paperqa/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-18 03:14:41.000000 paper-qa-1.6.2/paperqa/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 03:15:18.664700 paper-qa-1.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-18 03:14:41.000000 paper-qa-1.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:15:18.664700 paper-qa-1.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    11729 2023-05-18 03:14:41.000000 paper-qa-1.6.2/tests/test_paperqa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:41:14.458464 paper-qa-1.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-20 06:40:38.000000 paper-qa-1.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12585 2023-05-20 06:41:14.458464 paper-qa-1.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12150 2023-05-20 06:40:38.000000 paper-qa-1.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:41:14.454464 paper-qa-1.6.3/paper_qa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12585 2023-05-20 06:41:14.000000 paper-qa-1.6.3/paper_qa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-20 06:41:14.000000 paper-qa-1.6.3/paper_qa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 06:41:14.000000 paper-qa-1.6.3/paper_qa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-20 06:41:14.000000 paper-qa-1.6.3/paper_qa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-20 06:41:14.000000 paper-qa-1.6.3/paper_qa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:41:14.454464 paper-qa-1.6.3/paperqa/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-20 06:40:38.000000 paper-qa-1.6.3/paperqa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-05-20 06:40:38.000000 paper-qa-1.6.3/paperqa/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:41:14.454464 paper-qa-1.6.3/paperqa/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-20 06:40:38.000000 paper-qa-1.6.3/paperqa/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-05-20 06:40:38.000000 paper-qa-1.6.3/paperqa/contrib/zotero.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20314 2023-05-20 06:40:38.000000 paper-qa-1.6.3/paperqa/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-20 06:40:38.000000 paper-qa-1.6.3/paperqa/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-05-20 06:40:38.000000 paper-qa-1.6.3/paperqa/qaprompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-05-20 06:40:38.000000 paper-qa-1.6.3/paperqa/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-20 06:40:38.000000 paper-qa-1.6.3/paperqa/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-20 06:40:38.000000 paper-qa-1.6.3/paperqa/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-20 06:40:38.000000 paper-qa-1.6.3/paperqa/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 06:41:14.458464 paper-qa-1.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-20 06:40:38.000000 paper-qa-1.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:41:14.454464 paper-qa-1.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    12935 2023-05-20 06:40:38.000000 paper-qa-1.6.3/tests/test_paperqa.py
```

### Comparing `paper-qa-1.6.2/LICENSE` & `paper-qa-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `paper-qa-1.6.2/PKG-INFO` & `paper-qa-1.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 1.6.2
+Version: 1.6.3
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paper-qa-1.6.2/README.md` & `paper-qa-1.6.3/README.md`

 * *Files identical despite different names*

### Comparing `paper-qa-1.6.2/paper_qa.egg-info/PKG-INFO` & `paper-qa-1.6.3/paper_qa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 1.6.2
+Version: 1.6.3
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paper-qa-1.6.2/paperqa/agent.py` & `paper-qa-1.6.3/paperqa/agent.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.6.2/paperqa/contrib/zotero.py` & `paper-qa-1.6.3/paperqa/contrib/zotero.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.6.2/paperqa/docs.py` & `paper-qa-1.6.3/paperqa/docs.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,21 +108,19 @@
         # first check to see if we already have this document
         # this way we don't make api call to create citation on file we already have
         hash = md5sum(path)
         if hash in [d["hash"] for d in self.docs]:
             raise ValueError(f"Document {path} already in collection.")
 
         if citation is None:
-            cite_chain = make_chain(
-                prompt=citation_prompt, llm=self.summary_llm)
+            cite_chain = make_chain(prompt=citation_prompt, llm=self.summary_llm)
             # peak first chunk
             texts, _ = read_doc(path, "", "", chunk_chars=chunk_chars)
             if len(texts) == 0:
-                raise ValueError(
-                    f"Could not read document {path}. Is it empty?")
+                raise ValueError(f"Could not read document {path}. Is it empty?")
             citation = cite_chain.run(texts[0])
             if len(citation) < 3 or "Unknown" in citation or "insufficient" in citation:
                 citation = f"Unknown, {os.path.basename(path)}, {datetime.now().year}"
 
         if key is None:
             # get first name and year from citation
             try:
@@ -134,16 +132,15 @@
                 )
             try:
                 year = re.search(r"(\d{4})", citation).group(1)
             except AttributeError:
                 year = ""
             key = f"{author}{year}"
         key = self.get_unique_key(key)
-        texts, metadata = read_doc(
-            path, citation, key, chunk_chars=chunk_chars)
+        texts, metadata = read_doc(path, citation, key, chunk_chars=chunk_chars)
         # loose check to see if document was loaded
         #
         if len("".join(texts)) < 10 or (
             not disable_check and not maybe_is_text("".join(texts))
         ):
             raise ValueError(
                 f"This does not look like a text document: {path}. Path disable_check to ignore this error."
@@ -212,78 +209,78 @@
                 len(doc["texts"]),
                 doc["metadata"][0]["dockey"],
                 doc["metadata"][0]["citation"],
             )
             for doc in self.docs
         ]
 
-    async def adoc_match(self, query: str, k: int = 25, callbacks: List[AsyncCallbackHandler] = []) -> List[str]:
+    async def adoc_match(
+        self, query: str, k: int = 25, callbacks: List[AsyncCallbackHandler] = []
+    ) -> List[str]:
         """Return a list of documents that match the query."""
         if len(self.docs) == 0:
             return ""
         if self._doc_index is None:
             texts = [doc["metadata"][0]["citation"] for doc in self.docs]
-            metadatas = [{"key": doc["metadata"][0]["dockey"]}
-                         for doc in self.docs]
+            metadatas = [{"key": doc["metadata"][0]["dockey"]} for doc in self.docs]
             self._doc_index = FAISS.from_texts(
                 texts, metadatas=metadatas, embedding=self.embeddings
             )
         docs = self._doc_index.max_marginal_relevance_search(query, k=k)
         chain = make_chain(select_paper_prompt, self.summary_llm)
         papers = [f"{d.metadata['key']}: {d.page_content}" for d in docs]
-        result = await chain.arun(instructions=query, papers="\n".join(papers),
-                                  callbacks=callbacks)
+        result = await chain.arun(
+            instructions=query, papers="\n".join(papers), callbacks=callbacks
+        )
         return result
 
-
-    def doc_match(self, query: str, k: int = 25, callbacks: List[AsyncCallbackHandler] = []) -> List[str]:
+    def doc_match(
+        self, query: str, k: int = 25, callbacks: List[AsyncCallbackHandler] = []
+    ) -> List[str]:
         """Return a list of documents that match the query."""
         if len(self.docs) == 0:
             return ""
         if self._doc_index is None:
             texts = [doc["metadata"][0]["citation"] for doc in self.docs]
-            metadatas = [{"key": doc["metadata"][0]["dockey"]}
-                         for doc in self.docs]
+            metadatas = [{"key": doc["metadata"][0]["dockey"]} for doc in self.docs]
             self._doc_index = FAISS.from_texts(
                 texts, metadatas=metadatas, embedding=self.embeddings
             )
         docs = self._doc_index.max_marginal_relevance_search(query, k=k)
         chain = make_chain(select_paper_prompt, self.summary_llm)
         papers = [f"{d.metadata['key']}: {d.page_content}" for d in docs]
-        result = chain.run(instructions=query, papers="\n".join(papers),
-                                  callbacks=callbacks)
+        result = chain.run(
+            instructions=query, papers="\n".join(papers), callbacks=callbacks
+        )
         return result
-            
+
     def __getstate__(self):
         state = self.__dict__.copy()
         if self._faiss_index is not None:
             state["_faiss_index"].save_local(self.index_path)
         del state["_faiss_index"]
         del state["_doc_index"]
         return state
 
     def __setstate__(self, state):
         self.__dict__.update(state)
         try:
-            self._faiss_index = FAISS.load_local(
-                self.index_path, self.embeddings)
+            self._faiss_index = FAISS.load_local(self.index_path, self.embeddings)
         except:
             # they use some special exception type, but I don't want to import it
             self._faiss_index = None
         if not hasattr(self, "_doc_index"):
             self._doc_index = None
         self.update_llm(None, None)
 
     def _build_faiss_index(self):
         if self._faiss_index is None:
-            texts = reduce(lambda x, y: x + y,
-                           [doc["texts"] for doc in self.docs], [])
+            texts = reduce(lambda x, y: x + y, [doc["texts"] for doc in self.docs], [])
             text_embeddings = reduce(
-                lambda x, y: x + y, [doc["text_embeddings"]
-                                     for doc in self.docs], []
+                lambda x, y: x + y, [doc["text_embeddings"] for doc in self.docs], []
             )
             metadatas = reduce(
                 lambda x, y: x + y, [doc["metadata"] for doc in self.docs], []
             )
             self._faiss_index = FAISS.from_embeddings(
                 # wow adding list to the zip was tricky
                 text_embeddings=list(zip(texts, text_embeddings)),
@@ -364,15 +361,15 @@
                     question=answer.question,
                     context_str=doc.page_content,
                     citation=doc.metadata["citation"],
                     callbacks=callbacks,
                 ),
                 text=doc.page_content,
             )
-            if "Not applicable" not in c.context:
+            if "not applicable" not in c.context.casefold():
                 return c, callbacks[0]
             return None, None
 
         results = await asyncio.gather(*[process(doc) for doc in docs])
         # filter out failures
         results = [r for r in results if r[0] is not None]
         answer.tokens += sum([cb.total_tokens for _, cb in results])
@@ -486,15 +483,15 @@
         passages = dict()
         if len(context_str) < 10:
             answer_text = (
                 "I cannot answer this question due to insufficient information."
             )
         else:
             cb = OpenAICallbackHandler()
-            callbacks = [OpenAICallbackHandler()] + get_callbacks("answer")
+            callbacks = [cb] + get_callbacks("answer")
             qa_chain = make_chain(qa_prompt, self.llm)
             answer_text = await qa_chain.arun(
                 question=query,
                 context_str=context_str,
                 length=length_prompt,
                 callbacks=callbacks,
             )
```

### Comparing `paper-qa-1.6.2/paperqa/qaprompts.py` & `paper-qa-1.6.3/paperqa/qaprompts.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import copy
 from datetime import datetime
 from typing import Any, Dict, List, Optional
 
 import langchain.prompts as prompts
 from langchain.callbacks.manager import AsyncCallbackManagerForChainRun
 from langchain.chains import LLMChain
 from langchain.chat_models import ChatOpenAI
@@ -30,15 +31,15 @@
     template="Write an answer ({length}) "
     "for the question below based on the provided context. "
     "If the context provides insufficient information, "
     'reply "I cannot answer". '
     "For each sentence in your answer, indicate which sources most support it "
     "via valid citation markers at the end of sentences, like (Example2012). "
     "Answer in an unbiased, comprehensive, and scholarly tone. "
-    "Complete your answer with a concluding 1-2 sentences, which may be opinionated. "
+    "If the question is subjective, provide an opinionated answer in the concluding 1-2 sentences. "
     "Use Markdown for formatting code or text, and try to use direct quotes to support arguments.\n\n"
     "{context_str}\n"
     "Question: {question}\n"
     "Answer: ",
 )
 
 
@@ -93,14 +94,15 @@
             return self.generate(input_list, run_manager=run_manager)
 
 
 def make_chain(prompt, llm):
     if type(llm) == ChatOpenAI:
         system_message_prompt = SystemMessage(
             content="You are a scholarly researcher that answers in an unbiased, concise, scholarly tone. "
-            "You sometimes refuse to answer if there is insufficient information.",
+            "You sometimes refuse to answer if there is insufficient information. "
+            "If there are potentially ambiguous terms or acronyms, first define them. ",
         )
         human_message_prompt = HumanMessagePromptTemplate(prompt=prompt)
         prompt = ChatPromptTemplate.from_messages(
             [system_message_prompt, human_message_prompt]
         )
     return FallbackLLMChain(prompt=prompt, llm=llm)
```

### Comparing `paper-qa-1.6.2/paperqa/readers.py` & `paper-qa-1.6.3/paperqa/readers.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.6.2/paperqa/types.py` & `paper-qa-1.6.3/paperqa/types.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.6.2/paperqa/utils.py` & `paper-qa-1.6.3/paperqa/utils.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.6.2/setup.py` & `paper-qa-1.6.3/setup.py`

 * *Files identical despite different names*

### Comparing `paper-qa-1.6.2/tests/test_paperqa.py` & `paper-qa-1.6.3/tests/test_paperqa.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,54 +1,89 @@
 import os
 import pickle
+from typing import Any
 from unittest import IsolatedAsyncioTestCase
 
 import requests
+from langchain.callbacks.base import AsyncCallbackHandler
 from langchain.llms import OpenAI
 from langchain.llms.fake import FakeListLLM
 
 import paperqa
 from paperqa.utils import strings_similarity
 
 
+class TestHandler(AsyncCallbackHandler):
+    async def on_llm_new_token(self, token: str, **kwargs: Any) -> None:
+        print(token)
+
+
 def test_maybe_is_text():
     assert paperqa.maybe_is_text(
         "This is a test. The sample conc. was 1.0 mM (at 245 ^F)"
     )
     assert not paperqa.maybe_is_text("\\C0\\C0\\B1\x00")
     # get front page of wikipedia
-    r = requests.get(
-        "https://en.wikipedia.org/wiki/National_Flag_of_Canada_Day")
+    r = requests.get("https://en.wikipedia.org/wiki/National_Flag_of_Canada_Day")
     assert paperqa.maybe_is_text(r.text)
 
     # now force it to contain lots of weird encoding
     bad_text = r.text.encode("latin1", "ignore").decode("utf-16", "ignore")
     assert not paperqa.maybe_is_text(bad_text)
 
 
 def test_docs():
     doc_path = "example.txt"
     with open(doc_path, "w", encoding="utf-8") as f:
         # get front page of wikipedia
-        r = requests.get(
-            "https://en.wikipedia.org/wiki/National_Flag_of_Canada_Day")
+        r = requests.get("https://en.wikipedia.org/wiki/National_Flag_of_Canada_Day")
         f.write(r.text)
     llm = OpenAI(temperature=0.1, model_name="text-ada-001")
     docs = paperqa.Docs(llm=llm)
     docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
     assert docs.docs[0]["key"] == "Wiki2023"
     os.remove(doc_path)
 
 
+class TokenTest(IsolatedAsyncioTestCase):
+    async def test_token_count(self):
+        doc_path = "example.txt"
+        with open(doc_path, "w", encoding="utf-8") as f:
+            # get wiki page about politician
+            r = requests.get(
+                "https://en.wikipedia.org/wiki/Frederick_Bates_(politician)"
+            )
+            f.write(r.text)
+        docs = paperqa.Docs()
+
+        docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
+        os.remove(doc_path)
+        doc_path = "example2.txt"
+        with open(doc_path, "w", encoding="utf-8") as f:
+            # get wiki page about politician
+            r = requests.get(
+                "https://en.wikipedia.org/wiki/Frederick_Bates_(politician)"
+            )
+            f.write(r.text)
+            f.write("\n")  # so we don't have same hash
+        docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed tomorrow")
+        os.remove(doc_path)
+        answer = await docs.aquery(
+            "What is Frederick Bates's greatest accomplishment?",
+            get_callbacks=lambda x: [TestHandler()],
+        )
+        assert answer.tokens > 100
+        assert answer.cost > 0.01
+
+
 def test_evidence():
     doc_path = "example.txt"
     with open(doc_path, "w", encoding="utf-8") as f:
         # get wiki page about politician
-        r = requests.get(
-            "https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
+        r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
         f.write(r.text)
     docs = paperqa.Docs()
     docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
     evidence = docs.get_evidence(
         paperqa.Answer("For which state was he a governor"), k=1, max_sources=1
     )
     print(evidence.contexts[0].context, evidence.context)
@@ -56,16 +91,15 @@
     os.remove(doc_path)
 
 
 def test_query():
     doc_path = "example.txt"
     with open(doc_path, "w", encoding="utf-8") as f:
         # get wiki page about politician
-        r = requests.get(
-            "https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
+        r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
         f.write(r.text)
     docs = paperqa.Docs()
     docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
     docs.query("What is Frederick Bates's greatest accomplishment?")
     os.remove(doc_path)
 
 
@@ -84,29 +118,27 @@
         os.remove(doc_path)
 
 
 def test_doc_match():
     doc_path = "example.txt"
     with open(doc_path, "w", encoding="utf-8") as f:
         # get wiki page about politician
-        r = requests.get(
-            "https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
+        r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
         f.write(r.text)
     docs = paperqa.Docs()
     docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
     docs.doc_match("What is Frederick Bates's greatest accomplishment?")
     os.remove(doc_path)
 
 
 def test_docs_pickle():
     doc_path = "example.txt"
     with open(doc_path, "w", encoding="utf-8") as f:
         # get front page of wikipedia
-        r = requests.get(
-            "https://en.wikipedia.org/wiki/National_Flag_of_Canada_Day")
+        r = requests.get("https://en.wikipedia.org/wiki/National_Flag_of_Canada_Day")
         f.write(r.text)
     llm = OpenAI(temperature=0.0, model_name="text-babbage-001")
     docs = paperqa.Docs(llm=llm)
     docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now", chunk_chars=1000)
     docs_pickle = pickle.dumps(docs)
     docs2 = pickle.loads(docs_pickle)
     docs2.update_llm(llm)
@@ -161,16 +193,15 @@
     os.remove(doc_path)
 
 
 def test_bad_context():
     doc_path = "example.html"
     with open(doc_path, "w", encoding="utf-8") as f:
         # get wiki page about politician
-        r = requests.get(
-            "https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
+        r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
         f.write(r.text)
     docs = paperqa.Docs()
     docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
     answer = docs.query(
         "What year was Barack Obama born?",
         length_prompt="about 20 words",
     )
@@ -178,16 +209,15 @@
     os.remove(doc_path)
 
 
 def test_repeat_keys():
     doc_path = "example.txt"
     with open(doc_path, "w", encoding="utf-8") as f:
         # get wiki page about politician
-        r = requests.get(
-            "https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
+        r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
         f.write(r.text)
     docs = paperqa.Docs(llm=OpenAI(temperature=0.0, model_name="text-ada-001"))
     docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
     try:
         docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
     except ValueError:
         pass
@@ -209,39 +239,36 @@
     os.remove(doc_path)
     os.remove(doc_path2)
 
 
 def test_pdf_reader():
     tests_dir = os.path.dirname(os.path.abspath(__file__))
     doc_path = os.path.join(tests_dir, "paper.pdf")
-    docs = paperqa.Docs(llm=OpenAI(
-        temperature=0.0, model_name="text-curie-001"))
+    docs = paperqa.Docs(llm=OpenAI(temperature=0.0, model_name="text-curie-001"))
     docs.add(doc_path, "Wellawatte et al, XAI Review, 2023")
     answer = docs.query("Are counterfactuals actionable?")
     assert "yes" in answer.answer or "Yes" in answer.answer
 
 
 def test_prompt_length():
     doc_path = "example.txt"
     with open(doc_path, "w", encoding="utf-8") as f:
         # get wiki page about politician
-        r = requests.get(
-            "https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
+        r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
         f.write(r.text)
     docs = paperqa.Docs()
     docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
     docs.query("What is the name of the politician?", length_prompt="25 words")
 
 
 def test_doc_preview():
     doc_path = "example.txt"
     with open(doc_path, "w", encoding="utf-8") as f:
         # get wiki page about politician
-        r = requests.get(
-            "https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
+        r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
         f.write(r.text)
     docs = paperqa.Docs(llm=OpenAI(temperature=0.0, model_name="text-ada-001"))
     docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
     assert len(docs.doc_previews()) == 1
 
 
 def test_code():
@@ -253,32 +280,30 @@
     docs.query("What function tests the preview?")
 
 
 def test_citation():
     doc_path = "example.txt"
     with open(doc_path, "w", encoding="utf-8") as f:
         # get wiki page about politician
-        r = requests.get(
-            "https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
+        r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
         f.write(r.text)
     docs = paperqa.Docs()
     docs.add(doc_path)
     assert (
         list(docs.docs)[0]["metadata"][0]["key"] == "Wikipedia2023"
         or list(docs.docs)[0]["metadata"][0]["key"] == "Frederick2023"
     )
 
 
 def test_dockey_filter():
     """Test that we can filter evidence with dockeys"""
     doc_path = "example2.txt"
     with open(doc_path, "w", encoding="utf-8") as f:
         # get wiki page about politician
-        r = requests.get(
-            "https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
+        r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
         f.write(r.text)
     docs = paperqa.Docs()
     docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
     # add with new dockey
     with open("example.txt", "w", encoding="utf-8") as f:
         f.write(r.text)
         f.write("\n")  # so we don't have same hash
@@ -288,16 +313,15 @@
 
 
 def test_query_filter():
     """Test that we can filter evidence with in query"""
     doc_path = "example2.txt"
     with open(doc_path, "w", encoding="utf-8") as f:
         # get wiki page about politician
-        r = requests.get(
-            "https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
+        r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
         f.write(r.text)
     docs = paperqa.Docs()
     docs.add(
         doc_path,
         "Information about Fredrick Bates, WikiMedia Foundation, 2023, Accessed now",
     )
     # add with new dockey
@@ -311,16 +335,15 @@
 
 def test_nonopenai_model():
     responses = ["This is a test", "This is another test"] * 50
     model = FakeListLLM(responses=responses)
     doc_path = "example.txt"
     with open(doc_path, "w", encoding="utf-8") as f:
         # get wiki page about politician
-        r = requests.get(
-            "https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
+        r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
         f.write(r.text)
     docs = paperqa.Docs(llm=model)
     docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
     answer = docs.query("What country is Bates from?")
 
 
 def test_agent():
```

