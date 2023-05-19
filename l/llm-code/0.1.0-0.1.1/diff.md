# Comparing `tmp/llm_code-0.1.0.tar.gz` & `tmp/llm_code-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_code-0.1.0.tar", max compression
+gzip compressed data, was "llm_code-0.1.1.tar", max compression
```

## Comparing `llm_code-0.1.0.tar` & `llm_code-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,10 @@
--rw-r--r--   0        0        0     1070 2023-05-19 17:43:32.824715 llm_code-0.1.0/LICENSE
--rw-r--r--   0        0        0     1678 2023-05-19 23:09:48.887270 llm_code-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-19 17:43:32.824978 llm_code-0.1.0/llm_code/__init__.py
--rw-r--r--   0        0        0     2780 2023-05-19 22:57:36.142933 llm_code-0.1.0/llm_code/llm_code.py
--rw-r--r--   0        0        0     3293 2023-05-19 22:57:07.356159 llm_code-0.1.0/llm_code/templates.py
--rw-r--r--   0        0        0     1081 2023-05-19 20:42:43.473739 llm_code-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2607 1970-01-01 00:00:00.000000 llm_code-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-19 17:43:32.824715 llm_code-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1678 2023-05-19 23:09:48.887270 llm_code-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-19 17:43:32.824978 llm_code-0.1.1/llm_code/__init__.py
+-rw-r--r--   0        0        0     2780 2023-05-19 23:23:40.635458 llm_code-0.1.1/llm_code/llm_code.py
+-rw-r--r--   0        0        0     3293 2023-05-19 22:57:07.356159 llm_code-0.1.1/llm_code/templates.py
+-rw-r--r--   0        0        0      161 2023-05-19 18:26:22.445515 llm_code-0.1.1/prompts/coding/system.toml
+-rw-r--r--   0        0        0      613 2023-05-19 18:23:27.578834 llm_code-0.1.1/prompts/coding/user/input.toml
+-rw-r--r--   0        0        0      396 2023-05-19 18:19:43.905655 llm_code-0.1.1/prompts/coding/user/simple.toml
+-rw-r--r--   0        0        0     1113 2023-05-19 23:34:04.560704 llm_code-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2607 1970-01-01 00:00:00.000000 llm_code-0.1.1/PKG-INFO
```

### Comparing `llm_code-0.1.0/LICENSE` & `llm_code-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_code-0.1.0/README.md` & `llm_code-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `llm_code-0.1.0/llm_code/llm_code.py` & `llm_code-0.1.1/llm_code/llm_code.py`

 * *Files identical despite different names*

### Comparing `llm_code-0.1.0/llm_code/templates.py` & `llm_code-0.1.1/llm_code/templates.py`

 * *Files identical despite different names*

### Comparing `llm_code-0.1.0/pyproject.toml` & `llm_code-0.1.1/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "llm-code"
-version = "0.1.0"
+version = "0.1.1"
 description = "An OpenAI LLM based CLI coding assistant."
 authors = ["Rushabh Doshi <radoshi@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "llm_code" }]
 homepage = "https://github.com/radoshi/llm-code"
 repository = "https://github.com/radoshi/llm-code"
 keywords = ["openai", "llm", "cli", "coding", "assistant"]
 classifiers = [
     "Topic :: Software Development",
     "Topic :: Software Development :: Code Generators",
     "Development Status :: 3 - Alpha",
     "Environment :: Console",
 ]
+include = ["prompts/**/*.toml"]
 
 [tool.poetry.scripts]
 llm-code = "llm_code.llm_code:main"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 pydantic = { extras = ["dotenv"], version = "^1.10.7" }
```

### Comparing `llm_code-0.1.0/PKG-INFO` & `llm_code-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-code
-Version: 0.1.0
+Version: 0.1.1
 Summary: An OpenAI LLM based CLI coding assistant.
 Home-page: https://github.com/radoshi/llm-code
 License: MIT
 Keywords: openai,llm,cli,coding,assistant
 Author: Rushabh Doshi
 Author-email: radoshi@gmail.com
 Requires-Python: >=3.11,<4.0
```

