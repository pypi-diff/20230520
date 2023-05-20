# Comparing `tmp/chap-0.2.0.tar.gz` & `tmp/chap-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chap-0.2.0.tar", last modified: Tue Apr  4 14:48:25 2023, max compression
+gzip compressed data, was "chap-0.3.0.tar", last modified: Sat May 20 17:22:15 2023, max compression
```

## Comparing `chap-0.2.0.tar` & `chap-0.3.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:48:25.057102 chap-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:48:25.049102 chap-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:48:25.053102 chap-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-04 14:48:08.000000 chap-0.2.0/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-04 14:48:08.000000 chap-0.2.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-04 14:48:08.000000 chap-0.2.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-04 14:48:08.000000 chap-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-04 14:48:08.000000 chap-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-04 14:48:08.000000 chap-0.2.0/.pylintrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:48:25.053102 chap-0.2.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-04-04 14:48:08.000000 chap-0.2.0/LICENSES/CC0-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-04 14:48:08.000000 chap-0.2.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-04 14:48:08.000000 chap-0.2.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-04-04 14:48:25.057102 chap-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-04 14:48:08.000000 chap-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   343634 2023-04-04 14:48:08.000000 chap-0.2.0/chap.gif
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-04 14:48:08.000000 chap-0.2.0/chap.gif.license
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-04-04 14:48:08.000000 chap-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-04 14:48:08.000000 chap-0.2.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 14:48:25.057102 chap-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:48:25.053102 chap-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:48:25.053102 chap-0.2.0/src/chap/
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-04 14:48:08.000000 chap-0.2.0/src/chap/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-04 14:48:24.000000 chap-0.2.0/src/chap/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:48:25.057102 chap-0.2.0/src/chap/backends/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-04 14:48:08.000000 chap-0.2.0/src/chap/backends/lorem.py
--rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-04-04 14:48:08.000000 chap-0.2.0/src/chap/backends/openai_chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-04-04 14:48:08.000000 chap-0.2.0/src/chap/backends/textgen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:48:25.057102 chap-0.2.0/src/chap/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-04-04 14:48:08.000000 chap-0.2.0/src/chap/commands/ask.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-04 14:48:08.000000 chap-0.2.0/src/chap/commands/cat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-04-04 14:48:08.000000 chap-0.2.0/src/chap/commands/grep.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-04-04 14:48:08.000000 chap-0.2.0/src/chap/commands/import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-04 14:48:08.000000 chap-0.2.0/src/chap/commands/render.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-04 14:48:08.000000 chap-0.2.0/src/chap/commands/tui.css
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-04-04 14:48:08.000000 chap-0.2.0/src/chap/commands/tui.py
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-04 14:48:08.000000 chap-0.2.0/src/chap/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-04 14:48:08.000000 chap-0.2.0/src/chap/key.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-04-04 14:48:08.000000 chap-0.2.0/src/chap/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:48:25.057102 chap-0.2.0/src/chap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-04-04 14:48:25.000000 chap-0.2.0/src/chap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-04 14:48:25.000000 chap-0.2.0/src/chap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 14:48:25.000000 chap-0.2.0/src/chap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-04 14:48:25.000000 chap-0.2.0/src/chap.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-04 14:48:25.000000 chap-0.2.0/src/chap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-04 14:48:25.000000 chap-0.2.0/src/chap.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:22:15.730757 chap-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:22:15.726757 chap-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:22:15.726757 chap-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-20 17:21:55.000000 chap-0.3.0/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-20 17:21:55.000000 chap-0.3.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-20 17:21:55.000000 chap-0.3.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-20 17:21:55.000000 chap-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-20 17:21:55.000000 chap-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-20 17:21:55.000000 chap-0.3.0/.pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:22:15.726757 chap-0.3.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-05-20 17:21:55.000000 chap-0.3.0/LICENSES/CC0-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-20 17:21:55.000000 chap-0.3.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-20 17:21:55.000000 chap-0.3.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-05-20 17:22:15.730757 chap-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-20 17:21:55.000000 chap-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   336717 2023-05-20 17:21:55.000000 chap-0.3.0/chap.gif
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-20 17:21:55.000000 chap-0.3.0/chap.gif.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-20 17:21:55.000000 chap-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-20 17:21:55.000000 chap-0.3.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 17:22:15.730757 chap-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:22:15.726757 chap-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:22:15.726757 chap-0.3.0/src/chap/
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-20 17:21:55.000000 chap-0.3.0/src/chap/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-20 17:22:15.000000 chap-0.3.0/src/chap/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:22:15.730757 chap-0.3.0/src/chap/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-20 17:21:55.000000 chap-0.3.0/src/chap/backends/lorem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-05-20 17:21:55.000000 chap-0.3.0/src/chap/backends/openai_chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-05-20 17:21:55.000000 chap-0.3.0/src/chap/backends/textgen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:22:15.730757 chap-0.3.0/src/chap/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-05-20 17:21:55.000000 chap-0.3.0/src/chap/commands/ask.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-20 17:21:55.000000 chap-0.3.0/src/chap/commands/cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-20 17:21:55.000000 chap-0.3.0/src/chap/commands/grep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-05-20 17:21:55.000000 chap-0.3.0/src/chap/commands/import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-20 17:21:55.000000 chap-0.3.0/src/chap/commands/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-20 17:21:55.000000 chap-0.3.0/src/chap/commands/tui.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-05-20 17:21:55.000000 chap-0.3.0/src/chap/commands/tui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-20 17:21:55.000000 chap-0.3.0/src/chap/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-20 17:21:55.000000 chap-0.3.0/src/chap/key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-20 17:21:55.000000 chap-0.3.0/src/chap/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:22:15.730757 chap-0.3.0/src/chap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-05-20 17:22:15.000000 chap-0.3.0/src/chap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-20 17:22:15.000000 chap-0.3.0/src/chap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 17:22:15.000000 chap-0.3.0/src/chap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-20 17:22:15.000000 chap-0.3.0/src/chap.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-20 17:22:15.000000 chap-0.3.0/src/chap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-20 17:22:15.000000 chap-0.3.0/src/chap.egg-info/top_level.txt
```

### Comparing `chap-0.2.0/.github/workflows/codeql.yml` & `chap-0.3.0/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `chap-0.2.0/.github/workflows/release.yml` & `chap-0.3.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `chap-0.2.0/.github/workflows/test.yml` & `chap-0.3.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `chap-0.2.0/.pre-commit-config.yaml` & `chap-0.3.0/.pre-commit-config.yaml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -18,19 +18,19 @@
       exclude: tests
   -   id: trailing-whitespace
       exclude: tests
 - repo: https://github.com/fsfe/reuse-tool
   rev: v1.1.2
   hooks:
   - id: reuse
-- repo: https://github.com/pycqa/pylint
-  rev: v2.17.0
-  hooks:
-  - id: pylint
-    additional_dependencies: [click,dataclasses_json,httpx,lorem-text,'textual>=0.18.0',websockets]
-    args: ['--source-roots', 'src']
 - repo: https://github.com/pycqa/isort
   rev: 5.12.0
   hooks:
     - id: isort
       name: isort (python)
       args: ['--profile', 'black']
+- repo: https://github.com/pycqa/pylint
+  rev: v2.17.0
+  hooks:
+  - id: pylint
+    additional_dependencies: [click,dataclasses_json,httpx,lorem-text,'textual>=0.18.0',websockets]
+    args: ['--source-roots', 'src']
```

### Comparing `chap-0.2.0/LICENSES/CC0-1.0.txt` & `chap-0.3.0/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `chap-0.2.0/LICENSES/MIT.txt` & `chap-0.3.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `chap-0.2.0/LICENSES/Unlicense.txt` & `chap-0.3.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `chap-0.2.0/PKG-INFO` & `chap-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chap
-Version: 0.2.0
+Version: 0.3.0
 Summary: Interact with the OpenAI ChatGPT API (and other text generators)
 Author-email: Jeff Epler <jepler@gmail.com>
 Project-URL: homepage, https://github.com/jepler/chap
 Project-URL: repository, https://github.com/jepler/chap
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: PyPy
```

### Comparing `chap-0.2.0/README.md` & `chap-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `chap-0.2.0/pyproject.toml` & `chap-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `chap-0.2.0/src/chap/backends/lorem.py` & `chap-0.3.0/src/chap/backends/lorem.py`

 * *Files identical despite different names*

### Comparing `chap-0.2.0/src/chap/backends/openai_chatgpt.py` & `chap-0.3.0/src/chap/backends/openai_chatgpt.py`

 * *Files identical despite different names*

### Comparing `chap-0.2.0/src/chap/backends/textgen.py` & `chap-0.3.0/src/chap/backends/textgen.py`

 * *Files identical despite different names*

### Comparing `chap-0.2.0/src/chap/commands/ask.py` & `chap-0.3.0/src/chap/commands/ask.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,15 @@
 @click.option("--new-session", "-n", type=click.Path(exists=False), default=None)
 @click.option("--system-message", "-S", type=str, default=None)
 @click.option("--backend", "-b", type=str, default="openai_chatgpt")
 @click.argument("prompt", nargs=-1, required=True)
 def main(
     continue_session, last, new_session, system_message, prompt, backend
 ):  # pylint: disable=too-many-arguments
+    """Ask a question (command-line argument is passed as prompt)"""
     if bool(continue_session) + bool(last) + bool(new_session) > 1:
         raise SystemExit(
             "--continue-session, --last and --new_session are mutually exclusive"
         )
 
     api = get_api(backend)
```

### Comparing `chap-0.2.0/src/chap/commands/cat.py` & `chap-0.3.0/src/chap/commands/cat.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from ..session import Session
 
 
 @click.command
 @click.option("--session", "-s", type=click.Path(exists=True), default=None)
 @click.option("--last", is_flag=True)
 def main(session, last):
+    """Print session in plaintext"""
     if bool(session) + bool(last) != 1:
         raise SystemExit("Specify either --session, or --last")
 
     if last:
         session = last_session_path()
     with open(session, "r", encoding="utf-8") as f:
         session = Session.from_json(f.read())  # pylint: disable=no-member
```

### Comparing `chap-0.2.0/src/chap/commands/grep.py` & `chap-0.3.0/src/chap/commands/grep.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 
 
 @click.command
 @click.option("--ignore-case", "-i", is_flag=True)
 @click.option("--fixed-strings", "--literal", "-F", is_flag=True)
 @click.argument("pattern", nargs=1, required=True)
 def main(ignore_case, fixed_strings, pattern):
+    """Search sessions for pattern"""
     console = rich.get_console()
     if fixed_strings:
         pattern = re.escape(pattern)
 
     rx = re.compile(pattern, re.I if ignore_case else 0)
     last_file = None
     for f, m in list_files_matching_rx(rx, ignore_case):
```

### Comparing `chap-0.2.0/src/chap/commands/import.py` & `chap-0.3.0/src/chap/commands/import.py`

 * *Files identical despite different names*

### Comparing `chap-0.2.0/src/chap/commands/render.py` & `chap-0.3.0/src/chap/commands/render.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     return m
 
 
 @click.command
 @click.option("--session", "-s", type=click.Path(exists=True), default=None)
 @click.option("--last", is_flag=True)
 def main(session, last):
+    """Print session with formatting"""
     if bool(session) + bool(last) != 1:
         raise SystemExit("Specify either --session, or --last")
 
     if last:
         session = last_session_path()
     with open(session, "r", encoding="utf-8") as f:
         session = Session.from_json(f.read())  # pylint: disable=no-member
```

### Comparing `chap-0.2.0/src/chap/commands/tui.css` & `chap-0.3.0/src/chap/commands/tui.css`

 * *Files identical despite different names*

### Comparing `chap-0.2.0/src/chap/commands/tui.py` & `chap-0.3.0/src/chap/commands/tui.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import subprocess
 import sys
 
 import click
 from markdown_it import MarkdownIt
 from textual.app import App
 from textual.binding import Binding
-from textual.containers import Container
+from textual.containers import Container, VerticalScroll
 from textual.widgets import Footer, Input, Markdown
 
 from ..core import get_api, last_session_path, new_session_path
 from ..session import Assistant, Session, User
 
 
 def parser_factory():
@@ -54,15 +54,15 @@
     @property
     def container(self):
         return self.query_one("#content")
 
     def compose(self):
         yield Footer()
         yield Input(placeholder="Prompt")
-        yield Container(Container(id="pad"), id="content")
+        yield VerticalScroll(Container(id="pad"), id="content")
 
     async def on_mount(self) -> None:
         await self.container.mount_all(
             [markdown_for_step(step) for step in self.session.session], before="#pad"
         )
         # self.scrollview.scroll_y = self.scrollview.get_content_height()
         self.scroll_end()
@@ -117,14 +117,15 @@
 @click.command
 @click.option("--continue-session", "-s", type=click.Path(exists=True), default=None)
 @click.option("--last", is_flag=True)
 @click.option("--new-session", "-n", type=click.Path(exists=False), default=None)
 @click.option("--system-message", "-S", type=str, default=None)
 @click.option("--backend", "-b", type=str, default="openai_chatgpt")
 def main(continue_session, last, new_session, system_message, backend):
+    """Start interactive terminal user interface session"""
     if bool(continue_session) + bool(last) + bool(new_session) > 1:
         raise SystemExit(
             "--continue-session, --last and --new_session are mutually exclusive"
         )
 
     api = get_api(backend)
```

### Comparing `chap-0.2.0/src/chap/core.py` & `chap-0.3.0/src/chap/core.py`

 * *Files identical despite different names*

### Comparing `chap-0.2.0/src/chap/key.py` & `chap-0.3.0/src/chap/key.py`

 * *Files identical despite different names*

### Comparing `chap-0.2.0/src/chap/session.py` & `chap-0.3.0/src/chap/session.py`

 * *Files identical despite different names*

### Comparing `chap-0.2.0/src/chap.egg-info/PKG-INFO` & `chap-0.3.0/src/chap.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chap
-Version: 0.2.0
+Version: 0.3.0
 Summary: Interact with the OpenAI ChatGPT API (and other text generators)
 Author-email: Jeff Epler <jepler@gmail.com>
 Project-URL: homepage, https://github.com/jepler/chap
 Project-URL: repository, https://github.com/jepler/chap
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: PyPy
```

### Comparing `chap-0.2.0/src/chap.egg-info/SOURCES.txt` & `chap-0.3.0/src/chap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

