# Comparing `tmp/command_line_loom-0.0.4.tar.gz` & `tmp/command_line_loom-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "command_line_loom-0.0.4.tar", max compression
+gzip compressed data, was "command_line_loom-0.0.5.tar", max compression
```

## Comparing `command_line_loom-0.0.4.tar` & `command_line_loom-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1070 2023-05-18 18:19:49.972930 command_line_loom-0.0.4/LICENSE
--rw-r--r--   0        0        0     4466 2023-05-19 21:06:05.942638 command_line_loom-0.0.4/README.md
--rw-r--r--   0        0        0        7 2023-05-19 13:37:16.686088 command_line_loom-0.0.4/cll/__init__.py
--rw-r--r--   0        0        0     1555 2023-05-19 13:37:16.690088 command_line_loom-0.0.4/cll/__main__.py
--rw-r--r--   0        0        0     7645 2023-05-19 21:14:40.199467 command_line_loom-0.0.4/cll/app.py
--rw-r--r--   0        0        0     7358 2023-05-20 12:28:46.515322 command_line_loom-0.0.4/cll/config.py
--rw-r--r--   0        0        0      217 2023-05-19 13:37:16.690088 command_line_loom-0.0.4/cll/data_structs/__init__.py
--rw-r--r--   0        0        0    11532 2023-05-19 18:53:41.708355 command_line_loom-0.0.4/cll/data_structs/data_structs.py
--rw-r--r--   0        0        0     9817 2023-05-19 21:14:40.199467 command_line_loom-0.0.4/cll/data_structs/loom_index.py
--rw-r--r--   0        0        0     2493 2023-05-19 17:01:41.546225 command_line_loom-0.0.4/cll/data_structs/node.py
--rwxr-xr-x   0        0        0     4133 2023-05-20 12:28:46.515322 command_line_loom-0.0.4/cll/encoder.py
--rw-r--r--   0        0        0     1025 2023-05-19 13:37:16.690088 command_line_loom-0.0.4/cll/io.py
--rw-r--r--   0        0        0     2381 2023-05-19 21:14:40.203467 command_line_loom-0.0.4/cll/store.py
--rw-r--r--   0        0        0     7963 2023-05-19 21:14:40.203467 command_line_loom-0.0.4/cll/templater.py
--rw-r--r--   0        0        0    15809 2023-05-20 12:28:46.515322 command_line_loom-0.0.4/cll/tree.py
--rw-r--r--   0        0        0     1052 2023-05-20 12:28:48.275313 command_line_loom-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     5480 1970-01-01 00:00:00.000000 command_line_loom-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-18 18:19:49.972930 command_line_loom-0.0.5/LICENSE
+-rw-r--r--   0        0        0     4466 2023-05-19 21:06:05.942638 command_line_loom-0.0.5/README.md
+-rw-r--r--   0        0        0        7 2023-05-19 13:37:16.686088 command_line_loom-0.0.5/cll/__init__.py
+-rw-r--r--   0        0        0     1555 2023-05-19 13:37:16.690088 command_line_loom-0.0.5/cll/__main__.py
+-rw-r--r--   0        0        0     7645 2023-05-19 21:14:40.199467 command_line_loom-0.0.5/cll/app.py
+-rw-r--r--   0        0        0     7358 2023-05-20 12:28:46.515322 command_line_loom-0.0.5/cll/config.py
+-rw-r--r--   0        0        0      217 2023-05-19 13:37:16.690088 command_line_loom-0.0.5/cll/data_structs/__init__.py
+-rw-r--r--   0        0        0    11532 2023-05-19 18:53:41.708355 command_line_loom-0.0.5/cll/data_structs/data_structs.py
+-rw-r--r--   0        0        0     9817 2023-05-19 21:14:40.199467 command_line_loom-0.0.5/cll/data_structs/loom_index.py
+-rw-r--r--   0        0        0     2493 2023-05-19 17:01:41.546225 command_line_loom-0.0.5/cll/data_structs/node.py
+-rwxr-xr-x   0        0        0     4133 2023-05-20 12:28:46.515322 command_line_loom-0.0.5/cll/encoder.py
+-rw-r--r--   0        0        0     1025 2023-05-19 13:37:16.690088 command_line_loom-0.0.5/cll/io.py
+-rw-r--r--   0        0        0     2381 2023-05-19 21:14:40.203467 command_line_loom-0.0.5/cll/store.py
+-rw-r--r--   0        0        0     7963 2023-05-19 21:14:40.203467 command_line_loom-0.0.5/cll/templater.py
+-rw-r--r--   0        0        0    15809 2023-05-20 12:28:46.515322 command_line_loom-0.0.5/cll/tree.py
+-rw-r--r--   0        0        0     1052 2023-05-20 12:55:16.435098 command_line_loom-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     5480 1970-01-01 00:00:00.000000 command_line_loom-0.0.5/PKG-INFO
```

### Comparing `command_line_loom-0.0.4/LICENSE` & `command_line_loom-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `command_line_loom-0.0.4/README.md` & `command_line_loom-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `command_line_loom-0.0.4/cll/__main__.py` & `command_line_loom-0.0.5/cll/__main__.py`

 * *Files identical despite different names*

### Comparing `command_line_loom-0.0.4/cll/app.py` & `command_line_loom-0.0.5/cll/app.py`

 * *Files identical despite different names*

### Comparing `command_line_loom-0.0.4/cll/config.py` & `command_line_loom-0.0.5/cll/config.py`

 * *Files identical despite different names*

### Comparing `command_line_loom-0.0.4/cll/data_structs/data_structs.py` & `command_line_loom-0.0.5/cll/data_structs/data_structs.py`

 * *Files identical despite different names*

### Comparing `command_line_loom-0.0.4/cll/data_structs/loom_index.py` & `command_line_loom-0.0.5/cll/data_structs/loom_index.py`

 * *Files identical despite different names*

### Comparing `command_line_loom-0.0.4/cll/data_structs/node.py` & `command_line_loom-0.0.5/cll/data_structs/node.py`

 * *Files identical despite different names*

### Comparing `command_line_loom-0.0.4/cll/encoder.py` & `command_line_loom-0.0.5/cll/encoder.py`

 * *Files identical despite different names*

### Comparing `command_line_loom-0.0.4/cll/io.py` & `command_line_loom-0.0.5/cll/io.py`

 * *Files identical despite different names*

### Comparing `command_line_loom-0.0.4/cll/store.py` & `command_line_loom-0.0.5/cll/store.py`

 * *Files identical despite different names*

### Comparing `command_line_loom-0.0.4/cll/templater.py` & `command_line_loom-0.0.5/cll/templater.py`

 * *Files identical despite different names*

### Comparing `command_line_loom-0.0.4/cll/tree.py` & `command_line_loom-0.0.5/cll/tree.py`

 * *Files identical despite different names*

### Comparing `command_line_loom-0.0.4/pyproject.toml` & `command_line_loom-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "command-line-loom"
-version = "0.0.4"
+version = "0.0.5"
 description = ""
 authors = ["fergus <fergusfettes@gmail.com>"]
 homepage = "https://github.com/fergusfettes/command-line-loom"
 readme = "README.md"
 packages = [{include = "cll"}]
 
 [tool.poetry.dependencies]
@@ -16,15 +16,15 @@
 turbo-text-transformer-prompts = "^0.1.10"
 python-dotenv = "^1.0.0"
 click-shell = "^2.1"
 typer = "^0.9.0"
 rich = "^13.3.5"
 iterfzf = "^0.5.0.20.0"
 llama-index = "^0.6.8"
-typer-shell = "^0.1.4"
+typer-shell = "^0.1.6"
 networkx = "^3.1"
 
 [tool.poetry.group.dev.dependencies]
 ipdb = "^0.13.11"
 ipython = "^8.10.0"
 memory-profiler = "^0.61.0"
```

### Comparing `command_line_loom-0.0.4/PKG-INFO` & `command_line_loom-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: command-line-loom
-Version: 0.0.4
+Version: 0.0.5
 Summary: 
 Home-page: https://github.com/fergusfettes/command-line-loom
 Author: fergus
 Author-email: fergusfettes@gmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -18,15 +18,15 @@
 Requires-Dist: openai (>=0.27.0,<0.28.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: rich (>=13.3.5,<14.0.0)
 Requires-Dist: tiktoken (>=0.3.0,<0.4.0)
 Requires-Dist: turbo-text-transformer-prompts (>=0.1.10,<0.2.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
-Requires-Dist: typer-shell (>=0.1.4,<0.2.0)
+Requires-Dist: typer-shell (>=0.1.6,<0.2.0)
 Description-Content-Type: text/markdown
 
 # Command Line Loom
 
 Command Line Loom is a Python command-line tool for generating text using OpenAI's GPT-3 and other models. It includes a modular model system that allows for easy integration of new models and customization of existing ones.
 
 Includes templates, look in the [Turbo Text Transformer Prompts](https://github.com/fergusfettes/turbo-text-transformer-prompts) repository for more documentation and to find a list of the templates!
```

