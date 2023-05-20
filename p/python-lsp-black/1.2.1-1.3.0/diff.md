# Comparing `tmp/python-lsp-black-1.2.1.tar.gz` & `tmp/python-lsp-black-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-lsp-black-1.2.1.tar", last modified: Tue Apr 12 11:55:51 2022, max compression
+gzip compressed data, was "python-lsp-black-1.3.0.tar", last modified: Fri May 19 12:16:09 2023, max compression
```

## Comparing `python-lsp-black-1.2.1.tar` & `python-lsp-black-1.3.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 fidel     (1000) fidel     (1000)        0 2022-04-12 11:55:51.957335 python-lsp-black-1.2.1/
--rw-rw-r--   0 fidel     (1000) fidel     (1000)     4791 2022-04-12 11:55:51.961335 python-lsp-black-1.2.1/PKG-INFO
--rw-rw-r--   0 fidel     (1000) fidel     (1000)     3352 2022-04-12 11:51:02.000000 python-lsp-black-1.2.1/README.md
-drwxrwxr-x   0 fidel     (1000) fidel     (1000)        0 2022-04-12 11:55:51.957335 python-lsp-black-1.2.1/pylsp_black/
--rw-rw-r--   0 fidel     (1000) fidel     (1000)        0 2021-05-18 19:58:47.000000 python-lsp-black-1.2.1/pylsp_black/__init__.py
--rw-rw-r--   0 fidel     (1000) fidel     (1000)     6337 2022-04-12 11:51:02.000000 python-lsp-black-1.2.1/pylsp_black/plugin.py
--rw-rw-r--   0 fidel     (1000) fidel     (1000)      160 2022-03-28 13:29:25.000000 python-lsp-black-1.2.1/pyproject.toml
-drwxrwxr-x   0 fidel     (1000) fidel     (1000)        0 2022-04-12 11:55:51.957335 python-lsp-black-1.2.1/python_lsp_black.egg-info/
--rw-rw-r--   0 fidel     (1000) fidel     (1000)     4791 2022-04-12 11:55:51.000000 python-lsp-black-1.2.1/python_lsp_black.egg-info/PKG-INFO
--rw-rw-r--   0 fidel     (1000) fidel     (1000)      331 2022-04-12 11:55:51.000000 python-lsp-black-1.2.1/python_lsp_black.egg-info/SOURCES.txt
--rw-rw-r--   0 fidel     (1000) fidel     (1000)        1 2022-04-12 11:55:51.000000 python-lsp-black-1.2.1/python_lsp_black.egg-info/dependency_links.txt
--rw-rw-r--   0 fidel     (1000) fidel     (1000)       42 2022-04-12 11:55:51.000000 python-lsp-black-1.2.1/python_lsp_black.egg-info/entry_points.txt
--rw-rw-r--   0 fidel     (1000) fidel     (1000)      147 2022-04-12 11:55:51.000000 python-lsp-black-1.2.1/python_lsp_black.egg-info/requires.txt
--rw-rw-r--   0 fidel     (1000) fidel     (1000)       12 2022-04-12 11:55:51.000000 python-lsp-black-1.2.1/python_lsp_black.egg-info/top_level.txt
--rw-rw-r--   0 fidel     (1000) fidel     (1000)     1164 2022-04-12 11:55:51.961335 python-lsp-black-1.2.1/setup.cfg
--rw-rw-r--   0 fidel     (1000) fidel     (1000)       69 2021-05-18 19:58:47.000000 python-lsp-black-1.2.1/setup.py
+drwxrwxr-x   0 fidel     (1000) fidel     (1000)        0 2023-05-19 12:16:09.123677 python-lsp-black-1.3.0/
+-rw-rw-r--   0 fidel     (1000) fidel     (1000)     1119 2021-05-18 19:58:47.000000 python-lsp-black-1.3.0/LICENSE
+-rw-rw-r--   0 fidel     (1000) fidel     (1000)     4114 2023-05-19 12:16:09.123677 python-lsp-black-1.3.0/PKG-INFO
+-rw-rw-r--   0 fidel     (1000) fidel     (1000)     3352 2022-04-12 11:51:02.000000 python-lsp-black-1.3.0/README.md
+drwxrwxr-x   0 fidel     (1000) fidel     (1000)        0 2023-05-19 12:16:09.123677 python-lsp-black-1.3.0/pylsp_black/
+-rw-rw-r--   0 fidel     (1000) fidel     (1000)        0 2021-05-18 19:58:47.000000 python-lsp-black-1.3.0/pylsp_black/__init__.py
+-rw-rw-r--   0 fidel     (1000) fidel     (1000)     6609 2023-05-19 11:41:21.000000 python-lsp-black-1.3.0/pylsp_black/plugin.py
+-rw-rw-r--   0 fidel     (1000) fidel     (1000)      160 2022-03-28 13:29:25.000000 python-lsp-black-1.3.0/pyproject.toml
+drwxrwxr-x   0 fidel     (1000) fidel     (1000)        0 2023-05-19 12:16:09.123677 python-lsp-black-1.3.0/python_lsp_black.egg-info/
+-rw-rw-r--   0 fidel     (1000) fidel     (1000)     4114 2023-05-19 12:16:08.000000 python-lsp-black-1.3.0/python_lsp_black.egg-info/PKG-INFO
+-rw-rw-r--   0 fidel     (1000) fidel     (1000)      339 2023-05-19 12:16:08.000000 python-lsp-black-1.3.0/python_lsp_black.egg-info/SOURCES.txt
+-rw-rw-r--   0 fidel     (1000) fidel     (1000)        1 2023-05-19 12:16:08.000000 python-lsp-black-1.3.0/python_lsp_black.egg-info/dependency_links.txt
+-rw-rw-r--   0 fidel     (1000) fidel     (1000)       42 2023-05-19 12:16:08.000000 python-lsp-black-1.3.0/python_lsp_black.egg-info/entry_points.txt
+-rw-rw-r--   0 fidel     (1000) fidel     (1000)      165 2023-05-19 12:16:08.000000 python-lsp-black-1.3.0/python_lsp_black.egg-info/requires.txt
+-rw-rw-r--   0 fidel     (1000) fidel     (1000)       12 2023-05-19 12:16:08.000000 python-lsp-black-1.3.0/python_lsp_black.egg-info/top_level.txt
+-rw-rw-r--   0 fidel     (1000) fidel     (1000)     1178 2023-05-19 12:16:09.123677 python-lsp-black-1.3.0/setup.cfg
+-rw-rw-r--   0 fidel     (1000) fidel     (1000)       69 2021-05-18 19:58:47.000000 python-lsp-black-1.3.0/setup.py
```

### Comparing `python-lsp-black-1.2.1/PKG-INFO` & `python-lsp-black-1.3.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,105 +1,108 @@
 Metadata-Version: 2.1
 Name: python-lsp-black
-Version: 1.2.1
+Version: 1.3.0
 Summary: Black plugin for the Python LSP Server
 Home-page: https://github.com/python-lsp/python-lsp-black
 Author: Python LSP contributors
 Author-email: f@fidelramos.net
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/python-lsp/python-lsp-black/issues
 Project-URL: Changelog, https://github.com/python-lsp/python-lsp-black/blob/master/CHANGELOG.md
 Project-URL: Source Code, https://github.com/python-lsp/python-lsp-black
-Description: # python-lsp-black
-        
-        [![PyPI](https://img.shields.io/pypi/v/python-lsp-black.svg)](https://pypi.org/project/python-lsp-black) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-        [![Python](https://github.com/python-lsp/python-lsp-black/actions/workflows/python.yml/badge.svg)](https://github.com/python-lsp/python-lsp-black/actions/workflows/python.yml)
-        
-        [Black](https://github.com/psf/black) plugin for the [Python LSP Server](https://github.com/python-lsp/python-lsp-server).
-        
-        ## Install
-        
-        In the same `virtualenv` as `python-lsp-server`:
-        
-        ```shell
-        pip install python-lsp-black
-        ```
-        
-        # Usage
-        
-        This plugin will disable the yapf and autopep8 plugins if installed.
-        
-        - `python-lsp-black` can either format an entire file or just the selected text.
-        - The code will only be formatted if it is syntactically valid Python.
-        - Text selections are treated as if they were a separate Python file.
-          Unfortunately this means you can't format an indented block of code.
-        - `python-lsp-black` will use your project's
-          [pyproject.toml](https://github.com/psf/black#pyprojecttoml) if it has one.
-        - `python-lsp-black` only officially supports the latest stable version of
-          [black](https://github.com/psf/black). An effort is made to keep backwards-compatibility
-          but older black versions will not be actively tested.
-        - The plugin can cache the black configuration that applies to each Python file, this
-          improves performance of the plugin. When configuration caching is enabled any changes to
-          black's configuration will need the LSP server to be restarted. Configuration caching
-          can be disabled with the `cache_config` option, see *Configuration* below.
-        
-        # Configuration
-        
-        The plugin follows [python-lsp-server's
-        configuration](https://github.com/python-lsp/python-lsp-server/#configuration). These are
-        the valid configuration keys:
-        
-        - `pylsp.plugins.black.enabled`: boolean to enable/disable the plugin.
-        - `pylsp.plugins.black.cache_config`: a boolean to enable black configuration caching (see
-          *Usage*). `false` by default.
-        - `pylsp.plugins.black.line_length`: an integer that maps to [black's
-          `max-line-length`](https://black.readthedocs.io/en/stable/the_black_code_style/current_style.html#line-length)
-          setting. Defaults to 88 (same as black's default). This can also be set through black's
-          configuration files, which should be preferred for multi-user projects.
-        - `pylsp.plugins.black.preview`: a boolean to enable or disable [black's `--preview`
-          setting](https://black.readthedocs.io/en/stable/the_black_code_style/future_style.html#preview-style).
-        
-        # Development
-        
-        To install the project for development you need to specify the dev optional dependencies:
-        
-        ```shell
-        python -m venv .venv
-        . .venv/bin/activate
-        pip install -e .[dev]
-        ```
-        
-        This project uses [pre-commit](https://pre-commit.com/) hooks to control code quality,
-        install them to run automatically when creating a git commit, thus avoiding seeing errors
-        when you create a pull request:
-        
-        ```shell
-        pre-commit install
-        ```
-        
-        To run tests:
-        
-        ```shell
-        make test
-        ```
-        
-        To run linters:
-        
-        ```shell
-        make lint  # just a shortcut to pre-commit run -a
-        make <linter_name>  # black, flake8, isort, mypy
-        ```
-        
-        To upgrade the version of the pre-commit hooks:
-        
-        ```shell
-        pre-commit autoupdate
-        # check and git commit changes to .pre-commit-config.yaml
-        ```
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE
+
+# python-lsp-black
+
+[![PyPI](https://img.shields.io/pypi/v/python-lsp-black.svg)](https://pypi.org/project/python-lsp-black) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Python](https://github.com/python-lsp/python-lsp-black/actions/workflows/python.yml/badge.svg)](https://github.com/python-lsp/python-lsp-black/actions/workflows/python.yml)
+
+[Black](https://github.com/psf/black) plugin for the [Python LSP Server](https://github.com/python-lsp/python-lsp-server).
+
+## Install
+
+In the same `virtualenv` as `python-lsp-server`:
+
+```shell
+pip install python-lsp-black
+```
+
+# Usage
+
+This plugin will disable the yapf and autopep8 plugins if installed.
+
+- `python-lsp-black` can either format an entire file or just the selected text.
+- The code will only be formatted if it is syntactically valid Python.
+- Text selections are treated as if they were a separate Python file.
+  Unfortunately this means you can't format an indented block of code.
+- `python-lsp-black` will use your project's
+  [pyproject.toml](https://github.com/psf/black#pyprojecttoml) if it has one.
+- `python-lsp-black` only officially supports the latest stable version of
+  [black](https://github.com/psf/black). An effort is made to keep backwards-compatibility
+  but older black versions will not be actively tested.
+- The plugin can cache the black configuration that applies to each Python file, this
+  improves performance of the plugin. When configuration caching is enabled any changes to
+  black's configuration will need the LSP server to be restarted. Configuration caching
+  can be disabled with the `cache_config` option, see *Configuration* below.
+
+# Configuration
+
+The plugin follows [python-lsp-server's
+configuration](https://github.com/python-lsp/python-lsp-server/#configuration). These are
+the valid configuration keys:
+
+- `pylsp.plugins.black.enabled`: boolean to enable/disable the plugin.
+- `pylsp.plugins.black.cache_config`: a boolean to enable black configuration caching (see
+  *Usage*). `false` by default.
+- `pylsp.plugins.black.line_length`: an integer that maps to [black's
+  `max-line-length`](https://black.readthedocs.io/en/stable/the_black_code_style/current_style.html#line-length)
+  setting. Defaults to 88 (same as black's default). This can also be set through black's
+  configuration files, which should be preferred for multi-user projects.
+- `pylsp.plugins.black.preview`: a boolean to enable or disable [black's `--preview`
+  setting](https://black.readthedocs.io/en/stable/the_black_code_style/future_style.html#preview-style).
+
+# Development
+
+To install the project for development you need to specify the dev optional dependencies:
+
+```shell
+python -m venv .venv
+. .venv/bin/activate
+pip install -e .[dev]
+```
+
+This project uses [pre-commit](https://pre-commit.com/) hooks to control code quality,
+install them to run automatically when creating a git commit, thus avoiding seeing errors
+when you create a pull request:
+
+```shell
+pre-commit install
+```
+
+To run tests:
+
+```shell
+make test
+```
+
+To run linters:
+
+```shell
+make lint  # just a shortcut to pre-commit run -a
+make <linter_name>  # black, flake8, isort, mypy
+```
+
+To upgrade the version of the pre-commit hooks:
+
+```shell
+pre-commit autoupdate
+# check and git commit changes to .pre-commit-config.yaml
+```
+
+
```

### Comparing `python-lsp-black-1.2.1/README.md` & `python-lsp-black-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `python-lsp-black-1.2.1/pylsp_black/plugin.py` & `python-lsp-black-1.3.0/pylsp_black/plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 import logging
 import os
+import sys
 from functools import lru_cache
 from pathlib import Path
 from typing import Dict, Optional
 
 import black
-import toml
 from pylsp import hookimpl
 from pylsp._utils import get_eol_chars
 from pylsp.config.config import Config
 
+if sys.version_info >= (3, 11):
+    import tomllib
+else:
+    import tomli as tomllib
+
 logger = logging.getLogger(__name__)
 
 
 GLOBAL_CONFIG: Optional[Path] = None
 try:
     if os.name == "nt":
         GLOBAL_CONFIG = Path.home() / ".black"
@@ -83,14 +88,16 @@
 
 def format_text(*, text, config):
     mode = black.FileMode(
         target_versions=config["target_version"],
         line_length=config["line_length"],
         is_pyi=config["pyi"],
         string_normalization=not config["skip_string_normalization"],
+        magic_trailing_comma=not config["skip_magic_trailing_comma"],
+        preview=config["preview"],
     )
     try:
         # Black's format_file_contents only works reliably when eols are '\n'. It gives
         # an error for '\r' and produces wrong formatting for '\r\n'. So we replace
         # those eols by '\n' before formatting and restore them afterwards.
         replace_eols = False
         eol_chars = get_eol_chars(text)
@@ -127,14 +134,15 @@
     settings = client_config.plugin_settings("black")
 
     defaults = {
         "line_length": settings.get("line_length", 88),
         "fast": False,
         "pyi": filename.endswith(".pyi"),
         "skip_string_normalization": False,
+        "skip_magic_trailing_comma": False,
         "target_version": set(),
         "preview": settings.get("preview", False),
     }
 
     root = black.find_project_root((filename,))
 
     # Black 22.1.0+ returns a tuple
@@ -148,16 +156,17 @@
             pyproject_filename = GLOBAL_CONFIG
             logger.info("Using global black config at %s", pyproject_filename)
         else:
             logger.info("Using defaults: %r", defaults)
             return defaults
 
     try:
-        pyproject_toml = toml.load(str(pyproject_filename))
-    except (toml.TomlDecodeError, OSError):
+        with open(pyproject_filename, "rb") as f:
+            pyproject_toml = tomllib.load(f)
+    except (tomllib.TOMLDecodeError, OSError):
         logger.warning(
             "Error decoding pyproject.toml, using defaults: %r",
             defaults,
         )
         return defaults
 
     file_config = pyproject_toml.get("tool", {}).get("black", {})
```

### Comparing `python-lsp-black-1.2.1/python_lsp_black.egg-info/PKG-INFO` & `python-lsp-black-1.3.0/python_lsp_black.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,105 +1,108 @@
 Metadata-Version: 2.1
 Name: python-lsp-black
-Version: 1.2.1
+Version: 1.3.0
 Summary: Black plugin for the Python LSP Server
 Home-page: https://github.com/python-lsp/python-lsp-black
 Author: Python LSP contributors
 Author-email: f@fidelramos.net
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/python-lsp/python-lsp-black/issues
 Project-URL: Changelog, https://github.com/python-lsp/python-lsp-black/blob/master/CHANGELOG.md
 Project-URL: Source Code, https://github.com/python-lsp/python-lsp-black
-Description: # python-lsp-black
-        
-        [![PyPI](https://img.shields.io/pypi/v/python-lsp-black.svg)](https://pypi.org/project/python-lsp-black) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-        [![Python](https://github.com/python-lsp/python-lsp-black/actions/workflows/python.yml/badge.svg)](https://github.com/python-lsp/python-lsp-black/actions/workflows/python.yml)
-        
-        [Black](https://github.com/psf/black) plugin for the [Python LSP Server](https://github.com/python-lsp/python-lsp-server).
-        
-        ## Install
-        
-        In the same `virtualenv` as `python-lsp-server`:
-        
-        ```shell
-        pip install python-lsp-black
-        ```
-        
-        # Usage
-        
-        This plugin will disable the yapf and autopep8 plugins if installed.
-        
-        - `python-lsp-black` can either format an entire file or just the selected text.
-        - The code will only be formatted if it is syntactically valid Python.
-        - Text selections are treated as if they were a separate Python file.
-          Unfortunately this means you can't format an indented block of code.
-        - `python-lsp-black` will use your project's
-          [pyproject.toml](https://github.com/psf/black#pyprojecttoml) if it has one.
-        - `python-lsp-black` only officially supports the latest stable version of
-          [black](https://github.com/psf/black). An effort is made to keep backwards-compatibility
-          but older black versions will not be actively tested.
-        - The plugin can cache the black configuration that applies to each Python file, this
-          improves performance of the plugin. When configuration caching is enabled any changes to
-          black's configuration will need the LSP server to be restarted. Configuration caching
-          can be disabled with the `cache_config` option, see *Configuration* below.
-        
-        # Configuration
-        
-        The plugin follows [python-lsp-server's
-        configuration](https://github.com/python-lsp/python-lsp-server/#configuration). These are
-        the valid configuration keys:
-        
-        - `pylsp.plugins.black.enabled`: boolean to enable/disable the plugin.
-        - `pylsp.plugins.black.cache_config`: a boolean to enable black configuration caching (see
-          *Usage*). `false` by default.
-        - `pylsp.plugins.black.line_length`: an integer that maps to [black's
-          `max-line-length`](https://black.readthedocs.io/en/stable/the_black_code_style/current_style.html#line-length)
-          setting. Defaults to 88 (same as black's default). This can also be set through black's
-          configuration files, which should be preferred for multi-user projects.
-        - `pylsp.plugins.black.preview`: a boolean to enable or disable [black's `--preview`
-          setting](https://black.readthedocs.io/en/stable/the_black_code_style/future_style.html#preview-style).
-        
-        # Development
-        
-        To install the project for development you need to specify the dev optional dependencies:
-        
-        ```shell
-        python -m venv .venv
-        . .venv/bin/activate
-        pip install -e .[dev]
-        ```
-        
-        This project uses [pre-commit](https://pre-commit.com/) hooks to control code quality,
-        install them to run automatically when creating a git commit, thus avoiding seeing errors
-        when you create a pull request:
-        
-        ```shell
-        pre-commit install
-        ```
-        
-        To run tests:
-        
-        ```shell
-        make test
-        ```
-        
-        To run linters:
-        
-        ```shell
-        make lint  # just a shortcut to pre-commit run -a
-        make <linter_name>  # black, flake8, isort, mypy
-        ```
-        
-        To upgrade the version of the pre-commit hooks:
-        
-        ```shell
-        pre-commit autoupdate
-        # check and git commit changes to .pre-commit-config.yaml
-        ```
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE
+
+# python-lsp-black
+
+[![PyPI](https://img.shields.io/pypi/v/python-lsp-black.svg)](https://pypi.org/project/python-lsp-black) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Python](https://github.com/python-lsp/python-lsp-black/actions/workflows/python.yml/badge.svg)](https://github.com/python-lsp/python-lsp-black/actions/workflows/python.yml)
+
+[Black](https://github.com/psf/black) plugin for the [Python LSP Server](https://github.com/python-lsp/python-lsp-server).
+
+## Install
+
+In the same `virtualenv` as `python-lsp-server`:
+
+```shell
+pip install python-lsp-black
+```
+
+# Usage
+
+This plugin will disable the yapf and autopep8 plugins if installed.
+
+- `python-lsp-black` can either format an entire file or just the selected text.
+- The code will only be formatted if it is syntactically valid Python.
+- Text selections are treated as if they were a separate Python file.
+  Unfortunately this means you can't format an indented block of code.
+- `python-lsp-black` will use your project's
+  [pyproject.toml](https://github.com/psf/black#pyprojecttoml) if it has one.
+- `python-lsp-black` only officially supports the latest stable version of
+  [black](https://github.com/psf/black). An effort is made to keep backwards-compatibility
+  but older black versions will not be actively tested.
+- The plugin can cache the black configuration that applies to each Python file, this
+  improves performance of the plugin. When configuration caching is enabled any changes to
+  black's configuration will need the LSP server to be restarted. Configuration caching
+  can be disabled with the `cache_config` option, see *Configuration* below.
+
+# Configuration
+
+The plugin follows [python-lsp-server's
+configuration](https://github.com/python-lsp/python-lsp-server/#configuration). These are
+the valid configuration keys:
+
+- `pylsp.plugins.black.enabled`: boolean to enable/disable the plugin.
+- `pylsp.plugins.black.cache_config`: a boolean to enable black configuration caching (see
+  *Usage*). `false` by default.
+- `pylsp.plugins.black.line_length`: an integer that maps to [black's
+  `max-line-length`](https://black.readthedocs.io/en/stable/the_black_code_style/current_style.html#line-length)
+  setting. Defaults to 88 (same as black's default). This can also be set through black's
+  configuration files, which should be preferred for multi-user projects.
+- `pylsp.plugins.black.preview`: a boolean to enable or disable [black's `--preview`
+  setting](https://black.readthedocs.io/en/stable/the_black_code_style/future_style.html#preview-style).
+
+# Development
+
+To install the project for development you need to specify the dev optional dependencies:
+
+```shell
+python -m venv .venv
+. .venv/bin/activate
+pip install -e .[dev]
+```
+
+This project uses [pre-commit](https://pre-commit.com/) hooks to control code quality,
+install them to run automatically when creating a git commit, thus avoiding seeing errors
+when you create a pull request:
+
+```shell
+pre-commit install
+```
+
+To run tests:
+
+```shell
+make test
+```
+
+To run linters:
+
+```shell
+make lint  # just a shortcut to pre-commit run -a
+make <linter_name>  # black, flake8, isort, mypy
+```
+
+To upgrade the version of the pre-commit hooks:
+
+```shell
+pre-commit autoupdate
+# check and git commit changes to .pre-commit-config.yaml
+```
+
+
```

### Comparing `python-lsp-black-1.2.1/setup.cfg` & `python-lsp-black-1.3.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = python-lsp-black
-version = 1.2.1
+version = 1.3.0
 author = Python LSP contributors
 author_email = f@fidelramos.net
 description = Black plugin for the Python LSP Server
 url = https://github.com/python-lsp/python-lsp-black
 long_description = file: README.md
 long_description_content_type = text/markdown
 project_urls = 
@@ -14,22 +14,25 @@
 classifiers = 
 	Programming Language :: Python
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 packages = find:
-install_requires = python-lsp-server>=1.4.0; black>=22.3.0; toml
+install_requires = 
+	python-lsp-server>=1.4.0
+	black>=22.3.0
+	tomli; python_version<'3.11'
 python_requires = >= 3.7
 
 [options.entry_points]
 pylsp = pylsp_black = pylsp_black.plugin
 
 [options.extras_require]
-dev = isort>=5.0; flake8; pre-commit; pytest; mypy; pytest; types-pkg_resources; types-setuptools; types-toml
+dev = isort>=5.0; flake8; pre-commit; pytest; mypy; pytest; types-pkg_resources; types-setuptools
 
 [flake8]
 max-line-length = 88
 ignore = E203
 exclude = 
 	.venv
```

