# Comparing `tmp/embedbase_client-0.1.0.tar.gz` & `tmp/embedbase_client-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedbase_client-0.1.0.tar", max compression
+gzip compressed data, was "embedbase_client-0.1.1.tar", max compression
```

## Comparing `embedbase_client-0.1.0.tar` & `embedbase_client-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,11 @@
--rw-r--r--   0        0        0     1077 2023-04-17 09:49:08.973283 embedbase_client-0.1.0/LICENSE
--rw-r--r--   0        0        0     1102 2023-04-23 10:52:50.878842 embedbase_client-0.1.0/README.md
--rw-r--r--   0        0        0      434 2023-04-23 10:52:50.879295 embedbase_client-0.1.0/embedbase_client/__init__.py
--rw-r--r--   0        0        0     8073 2023-04-25 14:21:18.602349 embedbase_client-0.1.0/embedbase_client/client.py
--rw-r--r--   0        0        0     3531 2023-05-01 08:28:06.529600 embedbase_client-0.1.0/embedbase_client/split.py
--rw-r--r--   0        0        0     3542 2023-04-23 10:52:50.880926 embedbase_client-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2253 1970-01-01 00:00:00.000000 embedbase_client-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-04-17 09:49:08.973283 embedbase_client-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1005 2023-05-12 15:05:38.517672 embedbase_client-0.1.1/README.md
+-rw-r--r--   0        0        0      389 2023-05-20 14:15:09.469578 embedbase_client-0.1.1/embedbase_client/__init__.py
+-rw-r--r--   0        0        0    13892 2023-05-20 15:20:18.079226 embedbase_client-0.1.1/embedbase_client/async_client.py
+-rw-r--r--   0        0        0      913 2023-05-20 14:34:00.754341 embedbase_client-0.1.1/embedbase_client/base.py
+-rw-r--r--   0        0        0       49 2023-05-20 14:19:44.624286 embedbase_client-0.1.1/embedbase_client/errors.py
+-rw-r--r--   0        0        0     1579 2023-05-20 15:10:49.386549 embedbase_client-0.1.1/embedbase_client/model.py
+-rw-r--r--   0        0        0     3388 2023-05-20 15:24:12.182673 embedbase_client-0.1.1/embedbase_client/split.py
+-rw-r--r--   0        0        0    13858 2023-05-20 16:34:08.598970 embedbase_client-0.1.1/embedbase_client/sync_client.py
+-rw-r--r--   0        0        0     3516 2023-05-20 16:13:59.558388 embedbase_client-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2261 1970-01-01 00:00:00.000000 embedbase_client-0.1.1/PKG-INFO
```

### Comparing `embedbase_client-0.1.0/LICENSE` & `embedbase_client-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `embedbase_client-0.1.0/embedbase_client/split.py` & `embedbase_client-0.1.1/embedbase_client/split.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Callable, List, Optional, Tuple, Union
+from typing import List, Optional
 
 from tiktoken import get_encoding
 
 MAX_CHUNK_LENGTH = 8191
 EMBEDDING_ENCODING = "cl100k_base"
 CHUNK_OVERLAP = 0
 
@@ -20,15 +20,14 @@
 
 
 def split_text(
     text: str,
     max_tokens: int = MAX_CHUNK_LENGTH,
     chunk_overlap: int = CHUNK_OVERLAP,
     encoding_name: str = EMBEDDING_ENCODING,
-    callback: Optional[Callable[[SplitTextChunk], None]] = None,
 ) -> List[SplitTextChunk]:
     """
     Split a text into chunks of max_tokens length.
     Depending on the model used, you may want to adjust the max_tokens and chunk_overlap parameters.
     For example, if you use the OpenAI embeddings model, you can use max_tokens of 500 and chunk_overlap of 200.
     While if you use "all-MiniLM-L6-v2" of sentence-transformers, you might use max_tokens of 30 and chunk_overlap of 20
     because the model has a relatively limited input size.
@@ -59,16 +58,14 @@
 
     chunks = []
 
     while start_idx < len(input_ids):
         chunk = tokenizer.decode(chunk_ids)
         chunk_item = SplitTextChunk(chunk, start_idx, cur_idx)
         chunks.append(chunk_item)
-        if callback:
-            callback(chunk_item)
         start_idx += chunk_size - chunk_overlap
         cur_idx = min(start_idx + chunk_size, len(input_ids))
         chunk_ids = input_ids[start_idx:cur_idx]
 
     return chunks
```

### Comparing `embedbase_client-0.1.0/pyproject.toml` & `embedbase_client-0.1.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "embedbase-client"
-version = "0.1.0"
+version = "0.1.1"
 description = "Python client for Embedbase"
 readme = "README.md"
-authors = ["embedbase-client <louis@embedbase.xyz>"]
+authors = ["Different AI <louis@embedbase.xyz>"]
 license = "MIT"
 repository = "https://github.com/different-ai/embedbase/tree/main/sdk/embedbase-py"
 homepage = "https://github.com/different-ai/embedbase/tree/main/sdk/embedbase-py"
 
-# Keywords description https://python-poetry.org/docs/pyproject/#keywords
-keywords = []  #! Update me
+keywords = ["embeddings", "machine learning", "artificial intelligence", "llm"]
 
-# Pypi classifiers: https://pypi.org/classifiers/
-classifiers = [  #! Update me
-  "Development Status :: 3 - Alpha",
-  "Intended Audience :: Developers",
-  "Operating System :: OS Independent",
-  "Topic :: Software Development :: Libraries :: Python Modules",
-  "License :: OSI Approved :: MIT License",
-  "Programming Language :: Python :: 3",
-  "Programming Language :: Python :: 3.8",
-  "Programming Language :: Python :: 3.9",
+classifiers = [
+    "Development Status :: 4 - Beta",
+    "Intended Audience :: Developers",
+    "Topic :: Scientific/Engineering :: Artificial Intelligence",
+    "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 
 # todo: optional dependencies
 tiktoken = "^0.3.3"
 httpx = "^0.24.0"
+pydantic = "^1.10.7"
 
 [tool.poetry.dev-dependencies]
 click = "^7.1.2"
 bandit = "^1.7.1"
 black = {version = "^21.10b0", allow-prereleases = true}
 darglint = "^1.8.1"
 isort = {extras = ["colors"], version = "^5.10.1"}
@@ -49,16 +48,16 @@
 pytest = "^7.3.1"
 pyupgrade = "^2.29.1"
 safety = "^1.10.3"
 coverage = "^6.1.2"
 coverage-badge = "^1.1.0"
 pytest-html = "^3.1.1"
 pytest-cov = "^3.0.0"
-embedbase = "^1.0.4"
-
+embedbase = "^1.1.9"
+pytest-asyncio = "^0.21.0"
 
 [tool.black]
 # https://github.com/psf/black
 target-version = ["py38"]
 line-length = 88
 color = true
```

### Comparing `embedbase_client-0.1.0/PKG-INFO` & `embedbase_client-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: embedbase-client
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python client for Embedbase
 Home-page: https://github.com/different-ai/embedbase/tree/main/sdk/embedbase-py
 License: MIT
-Author: embedbase-client
+Keywords: embeddings,machine learning,artificial intelligence,llm
+Author: Different AI
 Author-email: louis@embedbase.xyz
 Requires-Python: >=3.8,<4.0
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Dist: httpx (>=0.24.0,<0.25.0)
+Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: tiktoken (>=0.3.3,<0.4.0)
 Project-URL: Repository, https://github.com/different-ai/embedbase/tree/main/sdk/embedbase-py
 Description-Content-Type: text/markdown
 
 # embedbase-py
 
 <div align="center">
@@ -41,17 +43,19 @@
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![License](https://img.shields.io/github/license/different-ai/embedbase)](https://github.com/different-ai/embedbase/blob/main/sdk/embedbase-py/LICENSE)
 ![Coverage Report](assets/images/coverage.svg)
 
 
 </div>
 
-This is not an officially launched product and currently lacks documentation. Please use at your own risk. If you are using this library, please let us know by opening an issue or contacting us on [discord](https://discord.gg/pMNeuGrDky).
+If you have any feedback or issues, please let us know by opening an issue or contacting us on [discord](https://discord.gg/pMNeuGrDky).
 
-Please refer to the [documentation](https://docs.embedbase.xyz/sdk-py).
+Please refer to the [documentation](https://docs.embedbase.xyz/sdk).
 
 ## Getting started
 
+To install the Embedbase Python client library, run the following command:
+
 ```bash
-pip install git+https://github.com/different-ai/embedbase.git@main#subdirectory=sdk/embedbase-py
+pip install embedbase-client
 ```
```

#### html2text {}

```diff
@@ -1,32 +1,32 @@
-Metadata-Version: 2.1 Name: embedbase-client Version: 0.1.0 Summary: Python
+Metadata-Version: 2.1 Name: embedbase-client Version: 0.1.1 Summary: Python
 client for Embedbase Home-page: https://github.com/different-ai/embedbase/tree/
-main/sdk/embedbase-py License: MIT Author: embedbase-client Author-email:
+main/sdk/embedbase-py License: MIT Keywords: embeddings,machine
+learning,artificial intelligence,llm Author: Different AI Author-email:
 louis@embedbase.xyz Requires-Python: >=3.8,<4.0 Classifier: Development Status
-:: 3 - Alpha Classifier: Intended Audience :: Developers Classifier: License ::
-OSI Approved :: MIT License Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3
+:: 4 - Beta Classifier: Intended Audience :: Developers Classifier: License ::
+OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Topic :: Software Development ::
-Libraries :: Python Modules Requires-Dist: httpx (>=0.24.0,<0.25.0) Requires-
-Dist: tiktoken (>=0.3.3,<0.4.0) Project-URL: Repository, https://github.com/
-different-ai/embedbase/tree/main/sdk/embedbase-py Description-Content-Type:
-text/markdown # embedbase-py
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Topic :: Scientific/Engineering ::
+Artificial Intelligence Requires-Dist: httpx (>=0.24.0,<0.25.0) Requires-Dist:
+pydantic (>=1.10.7,<2.0.0) Requires-Dist: tiktoken (>=0.3.3,<0.4.0) Project-
+URL: Repository, https://github.com/different-ai/embedbase/tree/main/sdk/
+embedbase-py Description-Content-Type: text/markdown # embedbase-py
  Embedbase-py - Python client for [Embedbase](https://github.com/different-ai/
                                   embedbase)
 
                      â ï¸ Status: Alpha release â ï¸
 
   [Discord] [![Code style: black](https://img.shields.io/badge/code%20style-
      black-000000.svg)](https://github.com/psf/black) [![License](https://
   img.shields.io/github/license/different-ai/embedbase)](https://github.com/
  different-ai/embedbase/blob/main/sdk/embedbase-py/LICENSE) ![Coverage Report]
                          (assets/images/coverage.svg)
-This is not an officially launched product and currently lacks documentation.
-Please use at your own risk. If you are using this library, please let us know
-by opening an issue or contacting us on [discord](https://discord.gg/
-pMNeuGrDky). Please refer to the [documentation](https://docs.embedbase.xyz/
-sdk-py). ## Getting started ```bash pip install git+https://github.com/
-different-ai/embedbase.git@main#subdirectory=sdk/embedbase-py ```
+If you have any feedback or issues, please let us know by opening an issue or
+contacting us on [discord](https://discord.gg/pMNeuGrDky). Please refer to the
+[documentation](https://docs.embedbase.xyz/sdk). ## Getting started To install
+the Embedbase Python client library, run the following command: ```bash pip
+install embedbase-client ```
```

