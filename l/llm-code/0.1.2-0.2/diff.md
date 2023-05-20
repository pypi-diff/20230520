# Comparing `tmp/llm_code-0.1.2.tar.gz` & `tmp/llm_code-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_code-0.1.2.tar", max compression
+gzip compressed data, was "llm_code-0.2.tar", max compression
```

## Comparing `llm_code-0.1.2.tar` & `llm_code-0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1070 2023-05-19 17:43:32.824715 llm_code-0.1.2/LICENSE
--rw-r--r--   0        0        0     1833 2023-05-20 05:46:21.650675 llm_code-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-05-19 17:43:32.824978 llm_code-0.1.2/llm_code/__init__.py
--rw-r--r--   0        0        0     2696 2023-05-20 05:32:25.595648 llm_code-0.1.2/llm_code/llm_code.py
--rw-r--r--   0        0        0     3293 2023-05-19 22:57:07.356159 llm_code-0.1.2/llm_code/templates.py
--rw-r--r--   0        0        0      161 2023-05-19 18:26:22.445515 llm_code-0.1.2/prompts/coding/system.toml
--rw-r--r--   0        0        0      613 2023-05-19 18:23:27.578834 llm_code-0.1.2/prompts/coding/user/input.toml
--rw-r--r--   0        0        0      396 2023-05-19 18:19:43.905655 llm_code-0.1.2/prompts/coding/user/simple.toml
--rw-r--r--   0        0        0     1113 2023-05-20 05:46:53.726329 llm_code-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2762 1970-01-01 00:00:00.000000 llm_code-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-19 17:43:32.824715 llm_code-0.2/LICENSE
+-rw-r--r--   0        0        0     1833 2023-05-20 05:46:21.650675 llm_code-0.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-19 17:43:32.824978 llm_code-0.2/llm_code/__init__.py
+-rw-r--r--   0        0        0     2696 2023-05-20 05:32:25.595648 llm_code-0.2/llm_code/llm_code.py
+-rw-r--r--   0        0        0     3293 2023-05-19 22:57:07.356159 llm_code-0.2/llm_code/templates.py
+-rw-r--r--   0        0        0      161 2023-05-19 18:26:22.445515 llm_code-0.2/prompts/coding/system.toml
+-rw-r--r--   0        0        0      613 2023-05-19 18:23:27.578834 llm_code-0.2/prompts/coding/user/input.toml
+-rw-r--r--   0        0        0      396 2023-05-19 18:19:43.905655 llm_code-0.2/prompts/coding/user/simple.toml
+-rw-r--r--   0        0        0     1116 2023-05-20 05:58:54.951619 llm_code-0.2/pyproject.toml
+-rw-r--r--   0        0        0     2765 1970-01-01 00:00:00.000000 llm_code-0.2/PKG-INFO
```

### Comparing `llm_code-0.1.2/LICENSE` & `llm_code-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_code-0.1.2/README.md` & `llm_code-0.2/README.md`

 * *Files identical despite different names*

### Comparing `llm_code-0.1.2/llm_code/llm_code.py` & `llm_code-0.2/llm_code/llm_code.py`

 * *Files identical despite different names*

### Comparing `llm_code-0.1.2/llm_code/templates.py` & `llm_code-0.2/llm_code/templates.py`

 * *Files identical despite different names*

### Comparing `llm_code-0.1.2/prompts/coding/user/input.toml` & `llm_code-0.2/prompts/coding/user/input.toml`

 * *Files identical despite different names*

### Comparing `llm_code-0.1.2/pyproject.toml` & `llm_code-0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "llm-code"
-version = "0.1.2"
+version = "0.2"
 description = "An OpenAI LLM based CLI coding assistant."
-authors = ["Rushabh Doshi <radoshi@gmail.com>"]
+authors = ["Rushabh Doshi <radoshi+pypi@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "llm_code" }]
 homepage = "https://github.com/radoshi/llm-code"
 repository = "https://github.com/radoshi/llm-code"
 keywords = ["openai", "llm", "cli", "coding", "assistant"]
 classifiers = [
```

### Comparing `llm_code-0.1.2/PKG-INFO` & `llm_code-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: llm-code
-Version: 0.1.2
+Version: 0.2
 Summary: An OpenAI LLM based CLI coding assistant.
 Home-page: https://github.com/radoshi/llm-code
 License: MIT
 Keywords: openai,llm,cli,coding,assistant
 Author: Rushabh Doshi
-Author-email: radoshi@gmail.com
+Author-email: radoshi+pypi@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
```

