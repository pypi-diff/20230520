# Comparing `tmp/typing_aliases-1.0.0.tar.gz` & `tmp/typing_aliases-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typing_aliases-1.0.0.tar", max compression
+gzip compressed data, was "typing_aliases-1.1.0.tar", max compression
```

## Comparing `typing_aliases-1.0.0.tar` & `typing_aliases-1.1.0.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1092 2022-11-26 19:17:45.397773 typing_aliases-1.0.0/LICENSE
--rw-r--r--   0        0        0     3112 2022-11-26 19:17:45.397773 typing_aliases-1.0.0/README.md
--rw-r--r--   0        0        0     3041 2022-11-26 19:17:45.397773 typing_aliases-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1946 2022-11-26 19:17:45.397773 typing_aliases-1.0.0/typing_aliases/__init__.py
--rw-r--r--   0        0        0        0 2022-11-26 19:17:45.397773 typing_aliases-1.0.0/typing_aliases/py.typed
--rw-r--r--   0        0        0     3586 2022-11-26 19:17:45.397773 typing_aliases-1.0.0/typing_aliases/typing.py
--rw-r--r--   0        0        0     3860 1970-01-01 00:00:00.000000 typing_aliases-1.0.0/setup.py
--rw-r--r--   0        0        0     4282 1970-01-01 00:00:00.000000 typing_aliases-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-05-20 19:05:48.395093 typing_aliases-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2809 2023-05-20 19:05:48.395093 typing_aliases-1.1.0/README.md
+-rw-r--r--   0        0        0     2657 2023-05-20 19:05:48.395093 typing_aliases-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4600 2023-05-20 19:05:48.395093 typing_aliases-1.1.0/typing_aliases/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-20 19:05:48.395093 typing_aliases-1.1.0/typing_aliases/py.typed
+-rw-r--r--   0        0        0    16879 2023-05-20 19:05:48.395093 typing_aliases-1.1.0/typing_aliases/typing.py
+-rw-r--r--   0        0        0     3985 1970-01-01 00:00:00.000000 typing_aliases-1.1.0/PKG-INFO
```

### Comparing `typing_aliases-1.0.0/LICENSE` & `typing_aliases-1.1.0/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022-present, Nikita Tikhonov (nekitdev)
+Copyright (c) 2023-present, Nikita Tikhonov (nekitdev)
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `typing_aliases-1.0.0/README.md` & `typing_aliases-1.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 [![License][License Badge]][License]
 [![Version][Version Badge]][Package]
 [![Downloads][Downloads Badge]][Package]
 [![Discord][Discord Badge]][Discord]
 
 [![Documentation][Documentation Badge]][Documentation]
 [![Check][Check Badge]][Actions]
-[![Test][Test Badge]][Actions]
-[![Coverage][Coverage Badge]][Coverage]
 
 > *Various type aliases.*
 
 ## Installing
 
 **Python 3.7 or above is required.**
 
@@ -40,15 +38,15 @@
 $ poetry add typing-aliases
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-typing-aliases = "^1.0.0"
+typing-aliases = "^1.1.0"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.typing-aliases]
 git = "https://github.com/nekitdev/typing-aliases.git"
@@ -90,19 +88,16 @@
 [Code of Conduct]: https://github.com/nekitdev/typing-aliases/blob/main/CODE_OF_CONDUCT.md
 [Contributing Guide]: https://github.com/nekitdev/typing-aliases/blob/main/CONTRIBUTING.md
 [Security]: https://github.com/nekitdev/typing-aliases/blob/main/SECURITY.md
 
 [License]: https://github.com/nekitdev/typing-aliases/blob/main/LICENSE
 
 [Package]: https://pypi.org/project/typing-aliases
-[Coverage]: https://codecov.io/gh/nekitdev/typing-aliases
 [Documentation]: https://nekitdev.github.io/typing-aliases
 
 [Discord Badge]: https://img.shields.io/badge/chat-discord-5865f2
 [License Badge]: https://img.shields.io/pypi/l/typing-aliases
 [Version Badge]: https://img.shields.io/pypi/v/typing-aliases
 [Downloads Badge]: https://img.shields.io/pypi/dm/typing-aliases
 
 [Documentation Badge]: https://github.com/nekitdev/typing-aliases/workflows/docs/badge.svg
 [Check Badge]: https://github.com/nekitdev/typing-aliases/workflows/check/badge.svg
-[Test Badge]: https://github.com/nekitdev/typing-aliases/workflows/test/badge.svg
-[Coverage Badge]: https://codecov.io/gh/nekitdev/typing-aliases/branch/main/graph/badge.svg
```

### Comparing `typing_aliases-1.0.0/pyproject.toml` & `typing_aliases-1.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "typing-aliases"
-version = "1.0.0"
+version = "1.1.0"
 description = "Various type aliases."
 authors = ["nekitdev"]
 license = "MIT"
 
 readme = "README.md"
 
 homepage = "https://github.com/nekitdev/typing-aliases"
 repository = "https://github.com/nekitdev/typing-aliases"
 documentation = "https://nekitdev.github.io/typing-aliases"
 
-keywords = ["python", "typing"]
+keywords = ["python", "typing", "alias"]
 
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Topic :: Utilities",
     "Typing :: Typed",
@@ -28,83 +28,61 @@
 
 [[tool.poetry.packages]]
 include = "typing_aliases"
 
 [tool.poetry.dependencies]
 python = ">= 3.7"
 
-typing-extensions = ">= 4.3.0"
+typing-extensions = ">= 4.5.0"
 
 [tool.poetry.group.format]
 optional = true
 
 [tool.poetry.group.format.dependencies]
-black = "22.8.0"
+black = "23.3.0"
+flake8-pyproject = "1.2.3"
+
+[tool.poetry.group.format.dependencies.flake8]
+version = "6.0.0"
+python = ">= 3.8.1"
 
 [tool.poetry.group.format.dependencies.isort]
-version = "5.10.1"
-python = "^3.7"
+version = "5.12.0"
+python = ">= 3.8"
 
 [tool.poetry.group.check]
 optional = true
 
 [tool.poetry.group.check.dependencies]
-mypy = "0.991"
-
-[tool.poetry.group.test]
-optional = true
-
-[tool.poetry.group.test.dependencies]
-pytest = "7.1.3"
-pytest-cov = "3.0.0"
+mypy = "1.3.0"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
-mkdocs = "1.3.1"
-mkdocs-material = "8.5.3"
+mkdocs = "1.4.3"
+mkdocs-material = "9.1.14"
 
 [tool.poetry.group.docs.dependencies.mkdocstrings]
-version = "0.19.0"
+version = "0.21.2"
 extras = ["python"]
 
 [tool.poetry.group.dev.dependencies]
-changelogging = "1.0.0"
+changelogging = "1.2.0"
 
 [tool.black]
 line_length = 100
 
+[tool.flake8]
+max_line_length = 100
+
 [tool.isort]
 line_length = 100
 profile = "black"
 
-[tool.pytest.ini_options]
-addopts = "--cov typing_aliases"
-testpaths = ["tests"]
-
-[tool.coverage.run]
-source = ["typing_aliases"]
-
-[tool.coverage.report]
-ignore_errors = true
-exclude_lines = [
-    "pragma: never",
-    "pragma: no cover",
-    "if TYPE_CHECKING",
-    "@overload",
-    "@abstractmethod",
-    "raise NotImplementedError",
-    "raise AssertionError",
-    "def __repr__",
-]
-
-[tool.coverage.html]
-directory = "coverage"
-
 [tool.mypy]
 show_column_numbers = true
 
 disallow_any_decorated = true
 disallow_any_generics = true
 warn_return_any = true
 
@@ -122,17 +100,17 @@
 
 warn_no_return = true
 warn_unreachable = true
 
 warn_redundant_casts = true
 warn_unused_ignores = false  # compatibility
 
-[tool.changelog]
+[tool.changelogging]
 name = "typing-aliases"
-version = "1.0.0"
+version = "1.1.0"
 url = "https://github.com/nekitdev/typing-aliases"
 directory = "changes"
 output = "CHANGELOG.md"
 
 start_string = "<!-- changelogging: start -->"
 
 title_format = "{version} ({date})"
@@ -141,9 +119,9 @@
 bullet = "-"
 wrap = true
 wrap_size = 100
 
 display = ["feature", "change", "fix", "security", "deprecation", "removal", "internal"]
 
 [build-system]
-requires = ["poetry-core >= 1.3.2"]
+requires = ["poetry-core >= 1.5.2"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `typing_aliases-1.0.0/PKG-INFO` & `typing_aliases-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: typing-aliases
-Version: 1.0.0
+Version: 1.1.0
 Summary: Various type aliases.
 Home-page: https://github.com/nekitdev/typing-aliases
 License: MIT
-Keywords: python,typing
+Keywords: python,typing,alias
 Author: nekitdev
 Requires-Python: >=3.7
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
-Requires-Dist: typing-extensions (>=4.3.0)
+Requires-Dist: typing-extensions (>=4.5.0)
 Project-URL: Documentation, https://nekitdev.github.io/typing-aliases
 Project-URL: Discord, https://nekit.dev/discord
 Project-URL: Funding, https://patreon.com/nekitdev
 Project-URL: Issues, https://github.com/nekitdev/typing-aliases/issues
 Project-URL: Repository, https://github.com/nekitdev/typing-aliases
 Description-Content-Type: text/markdown
 
@@ -32,16 +32,14 @@
 [![License][License Badge]][License]
 [![Version][Version Badge]][Package]
 [![Downloads][Downloads Badge]][Package]
 [![Discord][Discord Badge]][Discord]
 
 [![Documentation][Documentation Badge]][Documentation]
 [![Check][Check Badge]][Actions]
-[![Test][Test Badge]][Actions]
-[![Coverage][Coverage Badge]][Coverage]
 
 > *Various type aliases.*
 
 ## Installing
 
 **Python 3.7 or above is required.**
 
@@ -69,15 +67,15 @@
 $ poetry add typing-aliases
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-typing-aliases = "^1.0.0"
+typing-aliases = "^1.1.0"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.typing-aliases]
 git = "https://github.com/nekitdev/typing-aliases.git"
@@ -119,20 +117,17 @@
 [Code of Conduct]: https://github.com/nekitdev/typing-aliases/blob/main/CODE_OF_CONDUCT.md
 [Contributing Guide]: https://github.com/nekitdev/typing-aliases/blob/main/CONTRIBUTING.md
 [Security]: https://github.com/nekitdev/typing-aliases/blob/main/SECURITY.md
 
 [License]: https://github.com/nekitdev/typing-aliases/blob/main/LICENSE
 
 [Package]: https://pypi.org/project/typing-aliases
-[Coverage]: https://codecov.io/gh/nekitdev/typing-aliases
 [Documentation]: https://nekitdev.github.io/typing-aliases
 
 [Discord Badge]: https://img.shields.io/badge/chat-discord-5865f2
 [License Badge]: https://img.shields.io/pypi/l/typing-aliases
 [Version Badge]: https://img.shields.io/pypi/v/typing-aliases
 [Downloads Badge]: https://img.shields.io/pypi/dm/typing-aliases
 
 [Documentation Badge]: https://github.com/nekitdev/typing-aliases/workflows/docs/badge.svg
 [Check Badge]: https://github.com/nekitdev/typing-aliases/workflows/check/badge.svg
-[Test Badge]: https://github.com/nekitdev/typing-aliases/workflows/test/badge.svg
-[Coverage Badge]: https://codecov.io/gh/nekitdev/typing-aliases/branch/main/graph/badge.svg
```

