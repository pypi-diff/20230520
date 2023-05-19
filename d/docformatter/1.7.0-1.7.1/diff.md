# Comparing `tmp/docformatter-1.7.0.tar.gz` & `tmp/docformatter-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docformatter-1.7.0.tar", max compression
+gzip compressed data, was "docformatter-1.7.1.tar", max compression
```

## Comparing `docformatter-1.7.0.tar` & `docformatter-1.7.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1061 2022-07-29 13:50:28.414095 docformatter-1.7.0/LICENSE
--rw-r--r--   0        0        0     6593 2023-05-03 00:53:18.139711 docformatter-1.7.0/README.rst
--rw-r--r--   0        0        0     6026 2023-05-15 00:27:42.297884 docformatter-1.7.0/pyproject.toml
--rw-r--r--   0        0        0     1539 2023-04-12 22:55:21.288454 docformatter-1.7.0/src/docformatter/__init__.py
--rwxr-xr-x   0        0        0     6095 2023-05-05 16:25:39.896748 docformatter-1.7.0/src/docformatter/__main__.py
--rw-r--r--   0        0        0     1191 2023-05-15 00:27:42.297884 docformatter-1.7.0/src/docformatter/__pkginfo__.py
--rw-r--r--   0        0        0    12789 2023-05-05 16:25:39.896748 docformatter-1.7.0/src/docformatter/configuration.py
--rw-r--r--   0        0        0     3654 2023-04-12 22:55:21.317454 docformatter-1.7.0/src/docformatter/encode.py
--rw-r--r--   0        0        0    20851 2023-05-05 16:25:39.896748 docformatter-1.7.0/src/docformatter/format.py
--rw-r--r--   0        0        0     6611 2023-05-02 23:18:37.457940 docformatter-1.7.0/src/docformatter/strings.py
--rw-r--r--   0        0        0    15288 2023-05-15 00:27:42.298884 docformatter-1.7.0/src/docformatter/syntax.py
--rw-r--r--   0        0        0     4573 2023-04-28 16:27:48.980570 docformatter-1.7.0/src/docformatter/util.py
--rw-r--r--   0        0        0     7811 1970-01-01 00:00:00.000000 docformatter-1.7.0/setup.py
--rw-r--r--   0        0        0     8254 1970-01-01 00:00:00.000000 docformatter-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2022-07-29 13:50:28.414095 docformatter-1.7.1/LICENSE
+-rw-r--r--   0        0        0     6864 2023-05-18 11:03:05.743440 docformatter-1.7.1/README.rst
+-rw-r--r--   0        0        0     6191 2023-05-19 22:27:01.721656 docformatter-1.7.1/pyproject.toml
+-rw-r--r--   0        0        0     1614 2023-05-17 01:35:37.310713 docformatter-1.7.1/src/docformatter/__init__.py
+-rwxr-xr-x   0        0        0     6251 2023-05-18 11:03:05.744440 docformatter-1.7.1/src/docformatter/__main__.py
+-rw-r--r--   0        0        0     1191 2023-05-19 22:27:01.722656 docformatter-1.7.1/src/docformatter/__pkginfo__.py
+-rw-r--r--   0        0        0    13256 2023-05-17 01:35:37.310713 docformatter-1.7.1/src/docformatter/configuration.py
+-rw-r--r--   0        0        0     3654 2023-04-12 22:55:21.317454 docformatter-1.7.1/src/docformatter/encode.py
+-rw-r--r--   0        0        0    20564 2023-05-17 01:35:37.310713 docformatter-1.7.1/src/docformatter/format.py
+-rw-r--r--   0        0        0     6998 2023-05-17 01:35:37.310713 docformatter-1.7.1/src/docformatter/strings.py
+-rw-r--r--   0        0        0    23741 2023-05-19 22:01:42.795215 docformatter-1.7.1/src/docformatter/syntax.py
+-rw-r--r--   0        0        0     4573 2023-04-28 16:27:48.980570 docformatter-1.7.1/src/docformatter/util.py
+-rw-r--r--   0        0        0     8115 1970-01-01 00:00:00.000000 docformatter-1.7.1/setup.py
+-rw-r--r--   0        0        0     8557 1970-01-01 00:00:00.000000 docformatter-1.7.1/PKG-INFO
```

### Comparing `docformatter-1.7.0/LICENSE` & `docformatter-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `docformatter-1.7.0/README.rst` & `docformatter-1.7.1/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -59,32 +59,40 @@
 
 ``docformatter`` also handles some of the PEP 8 conventions.
 
 - Don't write string literals that rely on significant trailing
   whitespace. Such trailing whitespace is visually indistinguishable
   and some editors (or more recently, reindent.py) will trim them.
 
+``docformatter`` formats docstrings compatible with ``black`` when passed the
+``--black`` option.
+
+``docformatter`` formats field lists that use Epytext or Sphinx styles.
+
 See the the full documentation at `read-the-docs`_, especially the
 `requirements`_ section for a more detailed discussion of PEP 257 and other
 requirements.
 
 .. _read-the-docs: https://docformatter.readthedocs.io
 .. _requirements: https://docformatter.readthedocs.io/en/latest/requirements.html
 
 Installation
 ============
 
 From pip::
 
     $ pip install --upgrade docformatter
 
-Or, if you want to use pyproject.toml to configure docformatter::
+Or, if you want to use pyproject.toml to configure docformatter and you're using
+Python < 3.11::
 
     $ pip install --upgrade docformatter[tomli]
 
+With Python >=3.11, ``tomllib`` from the standard library is used.
+
 Or, if you want to use a release candidate (or any other tag)::
 
     $ pip install git+https://github.com/PyCQA/docformatter.git@<RC_TAG>
 
 Where <RC_TAG> is the release candidate tag you'd like to install.  Release
 candidate tags will have the format v1.6.0-rc1  Release candidates will also be
 made available as a Github Release.
```

### Comparing `docformatter-1.7.0/pyproject.toml` & `docformatter-1.7.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "docformatter"
-version = "1.7.0"
+version = "1.7.1"
 description = "Formats docstrings to follow PEP 257"
 authors = ["Steven Myint"]
 maintainers = [
     "Doyle Rowland <doyle.rowland@reliaqual.com>",
 ]
 license = "Expat"
 readme = "README.rst"
@@ -30,15 +30,15 @@
       ]
 packages = [{include = "docformatter", from = "src"}]
 include = ["LICENSE"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 charset_normalizer = "^3.0.0"
-tomli = {version = "^2.0.0", optional = true}
+tomli = {version = "^2.0.0", python = "<3.11", optional = true}
 untokenize = "^0.1.1"
 
 [tool.poetry.dev-dependencies]
 autopep8 = "^2.0.0"
 black = "^22.0.0"
 coverage = {extras = ["toml"], version = "^6.4.0"}
 isort = "^5.10.0"
@@ -48,14 +48,15 @@
 pydocstyle = "^6.1.1"
 pylint = [
     {version = "^2.12.0", python = "<3.7.2"},
     {version = "^2.14.0", python = ">=3.7.2"},
 ]
 pytest = "^7.1.0"
 pytest-cov = "^4.0.0"
+ruff = "^0.0.267"
 rstcheck = "^6.1.0"
 tox = "<4.0.0"
 Sphinx = [
     {version = "5.3.0", python = "<3.8"},
     {version = "^6.0.0", python = ">=3.8"},
 ]
 twine = "^4.0.0"
@@ -130,15 +131,15 @@
 ]
 show_missing = true
 
 [tool.coverage.xml]
 output = 'coverage.xml'
 
 [tool.black]
-line-length = 79
+line-length = 88
 target-version = ['py37', 'py38', 'py39', 'py310', 'py311']
 include = '\.pyi?$'
 exclude = '''
 /(
     \.eggs
   | \.git
   | \.hg
@@ -160,15 +161,26 @@
 import_heading_stdlib = 'Standard Library Imports'
 import_heading_thirdparty = 'Third Party Imports'
 multi_line_output = 3
 include_trailing_comma = true
 force_grid_wrap = 0
 use_parentheses = true
 ensure_newline_before_comments = true
-line_length = 79
+line_length = 88
+
+[tool.rstcheck]
+report = "warning"
+ignore_directives = [
+	"automodule",
+	"tabularcolumns",
+	"toctree",
+]
+ignore_roles = [
+	"numref",
+]
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 envlist =
     py37
     py38
@@ -238,20 +250,20 @@
 
 [testenv:style]
 description = run autoformatters and style checkers
 deps =
     charset_normalizer
     pycodestyle
     pydocstyle
-    pylint
+    ruff
     rstcheck
     toml
     untokenize
 commands =
     pip install -U pip
     pip install .
     docformatter --black --recursive {toxinidir}/src/docformatter
     pycodestyle --exclude=.git,.tox,*.pyc,*.pyo,build,dist,*.egg-info,config,docs,locale,tests,tools --ignore=C326,C330,E121,E123,E126,E133,E203,E242,E265,E402,W503,W504 --format=pylint --max-line-length=88 {toxinidir}/src/docformatter
     pydocstyle {toxinidir}/src/docformatter
-    pylint --rcfile={toxinidir}/pyproject.toml {toxinidir}/src/docformatter
+    ruff check --select "PL" --select "F" {toxinidir}/src/docformatter
     rstcheck --report-level=1 {toxinidir}/README.rst
 """
```

### Comparing `docformatter-1.7.0/src/docformatter/__init__.py` & `docformatter-1.7.1/src/docformatter/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # SOFTWARE.
 """This is the docformatter package."""
 
 __all__ = ["__version__"]
 
 # docformatter Local Imports
 from .__pkginfo__ import __version__
-from .strings import *
-from .syntax import *
-from .util import *
+from .strings import *  # noqa F403
+from .syntax import *  # noqa F403
+from .util import *  # noqa F403
 
 # Have isort skip these they require the functions above.
-from .configuration import Configurater  # isort: skip
-from .encode import Encoder  # isort: skip
-from .format import Formatter, FormatResult  # isort: skip
+from .configuration import Configurater  # isort: skip # noqa F401
+from .encode import Encoder  # isort: skip # noqa F401
+from .format import Formatter, FormatResult  # isort: skip # noqa F401
```

### Comparing `docformatter-1.7.0/src/docformatter/__main__.py` & `docformatter-1.7.1/src/docformatter/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,20 +20,15 @@
 # BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN
 # ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 """Formats docstrings to follow PEP 257."""
 
 
-from __future__ import (
-    absolute_import,
-    division,
-    print_function,
-    unicode_literals,
-)
+from __future__ import absolute_import, division, print_function, unicode_literals
 
 # Standard Library Imports
 import contextlib
 import signal
 import sys
 
 # docformatter Package Imports
@@ -67,14 +62,17 @@
   -e [EXCLUDE ...], --exclude [EXCLUDE ...]
                         in recursive mode, exclude directories and files by
                         names
   -n [NON-CAP ...], --non-cap [NON-CAP ...]
                         list of words not to capitalize when they appear as the
                         first word in the summary
 
+  -s style, --style style
+                        the docstring style to use when formatting parameter
+                        lists.  One of epytext, sphinx. (default: sphinx)
   --black               make formatting compatible with standard black options
                         (default: False)
   --wrap-summaries length
                         wrap long summary lines at this length; set to 0 to
                         disable wrapping (default: 79, 88 with --black option)
   --wrap-descriptions length
                         wrap descriptions at this length; set to 0 to disable
```

### Comparing `docformatter-1.7.0/src/docformatter/__pkginfo__.py` & `docformatter-1.7.1/src/docformatter/__pkginfo__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 # NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS
 # BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN
 # ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 """Package information for docformatter."""
 
-__version__ = "1.7.0"
+__version__ = "1.7.1"
```

### Comparing `docformatter-1.7.0/src/docformatter/configuration.py` & `docformatter-1.7.1/src/docformatter/configuration.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,49 +19,58 @@
 # NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS
 # BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN
 # ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 """This module provides docformatter's Configurater class."""
 
+
 # Standard Library Imports
 import argparse
+import contextlib
 import os
+import sys
 from configparser import ConfigParser
 from typing import Dict, List, Union
 
-try:
-    # Third Party Imports
-    import tomli
-
-    TOMLI_INSTALLED = True
-except ImportError:
-    TOMLI_INSTALLED = False
+TOMLLIB_INSTALLED = False
+TOMLI_INSTALLED = False
+with contextlib.suppress(ImportError):
+    if sys.version_info >= (3, 11):
+        # Standard Library Imports
+        import tomllib
+
+        TOMLLIB_INSTALLED = True
+    else:
+        # Third Party Imports
+        import tomli
+
+        TOMLI_INSTALLED = True
 
 # docformatter Package Imports
 from docformatter import __pkginfo__
 
 
 class Configurater:
     """Read and store all the docformatter configuration information."""
 
-    parser = None
+    parser: argparse.ArgumentParser = argparse.ArgumentParser()
     """Parser object."""
 
     flargs_dct: Dict[str, Union[bool, float, int, str]] = {}
     """Dictionary of configuration file arguments."""
 
     configuration_file_lst = [
         "pyproject.toml",
         "setup.cfg",
         "tox.ini",
     ]
     """List of supported configuration files."""
 
-    args: argparse.Namespace = None
+    args: argparse.Namespace = argparse.Namespace()
 
     def __init__(self, args: List[Union[bool, int, str]]) -> None:
         """Initialize a Configurater class instance.
 
         Parameters
         ----------
         args : list
@@ -71,17 +80,15 @@
         self.config_file = ""
         self.parser = argparse.ArgumentParser(
             description=__doc__,
             prog="docformatter",
         )
 
         try:
-            self.config_file = self.args_lst[
-                self.args_lst.index("--config") + 1
-            ]
+            self.config_file = self.args_lst[self.args_lst.index("--config") + 1]
         except ValueError:
             for _configuration_file in self.configuration_file_lst:
                 if os.path.isfile(_configuration_file):
                     self.config_file = f"./{_configuration_file}"
                     break
 
         if os.path.isfile(self.config_file):
@@ -112,16 +119,15 @@
             help="when used with `--check` or `--in-place`, also what changes "
             "would be made",
         )
         self.parser.add_argument(
             "-r",
             "--recursive",
             action="store_true",
-            default=self.flargs_dct.get("recursive", "false").lower()
-            == "true",
+            default=self.flargs_dct.get("recursive", "false").lower() == "true",
             help="drill down directories recursively",
         )
         self.parser.add_argument(
             "-e",
             "--exclude",
             nargs="*",
             default=self.flargs_dct.get("exclude", None),
@@ -155,42 +161,44 @@
             _default_pre_summary_space = "true"
         else:
             _default_wrap_summaries = 79
             _default_wrap_descriptions = 72
             _default_pre_summary_space = "false"
 
         self.parser.add_argument(
+            "-s",
+            "--style",
+            default=self.flargs_dct.get("style", "sphinx"),
+            help="name of the docstring style to use when formatting "
+            "parameter lists (default: sphinx)",
+        )
+        self.parser.add_argument(
             "--wrap-summaries",
-            default=int(
-                self.flargs_dct.get("wrap-summaries", _default_wrap_summaries)
-            ),
+            default=int(self.flargs_dct.get("wrap-summaries", _default_wrap_summaries)),
             type=int,
             metavar="length",
             help="wrap long summary lines at this length; "
             "set to 0 to disable wrapping (default: 79, 88 with --black "
             "option)",
         )
         self.parser.add_argument(
             "--wrap-descriptions",
             default=int(
-                self.flargs_dct.get(
-                    "wrap-descriptions", _default_wrap_descriptions
-                )
+                self.flargs_dct.get("wrap-descriptions", _default_wrap_descriptions)
             ),
             type=int,
             metavar="length",
             help="wrap descriptions at this length; "
             "set to 0 to disable wrapping (default: 72, 88 with --black "
             "option)",
         )
         self.parser.add_argument(
             "--force-wrap",
             action="store_true",
-            default=self.flargs_dct.get("force-wrap", "false").lower()
-            == "true",
+            default=self.flargs_dct.get("force-wrap", "false").lower() == "true",
             help="force descriptions to be wrapped even if it may "
             "result in a mess (default: False)",
         )
         self.parser.add_argument(
             "--tab-width",
             type=int,
             dest="tab_width",
@@ -217,33 +225,28 @@
         self.parser.add_argument(
             "--pre-summary-space",
             action="store_true",
             default=self.flargs_dct.get(
                 "pre-summary-space", _default_pre_summary_space
             ).lower()
             == "true",
-            help="add a space after the opening triple quotes "
-            "(default: False)",
+            help="add a space after the opening triple quotes " "(default: False)",
         )
         self.parser.add_argument(
             "--make-summary-multi-line",
             action="store_true",
-            default=self.flargs_dct.get(
-                "make-summary-multi-line", "false"
-            ).lower()
+            default=self.flargs_dct.get("make-summary-multi-line", "false").lower()
             == "true",
             help="add a newline before and after the summary of a one-line "
             "docstring (default: False)",
         )
         self.parser.add_argument(
             "--close-quotes-on-newline",
             action="store_true",
-            default=self.flargs_dct.get(
-                "close-quotes-on-newline", "false"
-            ).lower()
+            default=self.flargs_dct.get("close-quotes-on-newline", "false").lower()
             == "true",
             help="place closing triple quotes on a new-line when a "
             "one-line docstring wraps to two or more lines "
             "(default: False)",
         )
         self.parser.add_argument(
             "--range",
@@ -264,16 +267,15 @@
             nargs=2,
             help="apply docformatter to docstrings of given length range "
             "(default: None)",
         )
         self.parser.add_argument(
             "--non-strict",
             action="store_true",
-            default=self.flargs_dct.get("non-strict", "false").lower()
-            == "true",
+            default=self.flargs_dct.get("non-strict", "false").lower() == "true",
             help="don't strictly follow reST syntax to identify lists (see "
             "issue #67) (default: False)",
         )
         self.parser.add_argument(
             "--config",
             default=self.config_file,
             help="path to file containing docformatter options",
@@ -298,17 +300,15 @@
                 self.parser.error(
                     "First value of --range should be less than or equal "
                     "to the second"
                 )
 
         if self.args.length_range:
             if self.args.length_range[0] <= 0:
-                self.parser.error(
-                    "--docstring-length must be positive numbers"
-                )
+                self.parser.error("--docstring-length must be positive numbers")
             if self.args.length_range[0] > self.args.length_range[1]:
                 self.parser.error(
                     "First value of --docstring-length should be less "
                     "than or equal to the second"
                 )
 
     def _do_read_configuration_file(self) -> None:
@@ -317,32 +317,38 @@
         for f in self.configuration_file_lst:
             if argfile == f:
                 break
 
         fullpath, ext = os.path.splitext(self.config_file)
         filename = os.path.basename(fullpath)
 
-        if ext == ".toml" and TOMLI_INSTALLED and filename == "pyproject":
+        if (
+            ext == ".toml"
+            and (TOMLI_INSTALLED or TOMLLIB_INSTALLED)
+            and filename == "pyproject"
+        ):
             self._do_read_toml_configuration()
 
         if (ext == ".cfg" and filename == "setup") or (
             ext == ".ini" and filename == "tox"
         ):
             self._do_read_parser_configuration()
 
     def _do_read_toml_configuration(self) -> None:
         """Load configuration information from a *.toml file."""
         with open(self.config_file, "rb") as f:
-            config = tomli.load(f)
+            if TOMLI_INSTALLED:
+                config = tomli.load(f)
+            elif TOMLLIB_INSTALLED:
+                config = tomllib.load(f)
 
         result = config.get("tool", {}).get("docformatter", None)
         if result is not None:
             self.flargs_dct = {
-                k: v if isinstance(v, list) else str(v)
-                for k, v in result.items()
+                k: v if isinstance(v, list) else str(v) for k, v in result.items()
             }
 
     def _do_read_parser_configuration(self) -> None:
         """Load configuration information from a *.cfg or *.ini file."""
         config = ConfigParser()
         config.read(self.config_file)
```

### Comparing `docformatter-1.7.0/src/docformatter/encode.py` & `docformatter-1.7.1/src/docformatter/encode.py`

 * *Files identical despite different names*

### Comparing `docformatter-1.7.0/src/docformatter/format.py` & `docformatter-1.7.1/src/docformatter/format.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,27 +61,25 @@
     Returns
     -------
     modified_tokens: list
         The list of tokens with any blank lines following a variable
         definition removed.
     """
     for _idx, _token in enumerate(modified_tokens):
-        if _token[0] == 3:
+        if _token[0] == 3:  # noqa PLR2004
             j = 1
 
             # Remove newline between variable definition and docstring
             # unless it's separating a docstring from:
             #     * A previous docstring.
             #     * The file's shebang.
             #     * The import section.
             while (
                 modified_tokens[_idx - j][4] == "\n"
-                and not (
-                    modified_tokens[_idx - j - 1][4].strip().endswith('"""')
-                )
+                and not (modified_tokens[_idx - j - 1][4].strip().endswith('"""'))
                 and not modified_tokens[_idx - j - 1][4].startswith("#!/")
                 and "import" not in modified_tokens[_idx - j - 1][4]
             ):
                 modified_tokens.pop(_idx - j)
                 j += 1
 
             # Remove newline between class, method, and function
@@ -116,31 +114,25 @@
         j = 1
         _num_blank_lines = 0
         while modified_tokens[_idx - j][4] == "\n":
             j += 1
             _num_blank_lines += 1
 
         with contextlib.suppress(IndexError):
-            _is_definition = (
-                _token[4].lstrip().startswith(("class ", "def ", "@"))
-            )
-            _is_docstring = (
-                modified_tokens[_idx - 2][4].strip().endswith('"""')
-            )
+            _is_definition = _token[4].lstrip().startswith(("class ", "def ", "@"))
+            _is_docstring = modified_tokens[_idx - 2][4].strip().endswith('"""')
             _after_definition = (
                 modified_tokens[_idx - _num_blank_lines - 4][4]
                 .lstrip()
                 .startswith(("class", "def", "@"))
             )
             _after_docstring = modified_tokens[_idx - 5][4].strip().endswith(
                 '"""'
             ) or modified_tokens[_idx - 5][4].strip().startswith('"""')
-            _comment_follows = re.search(
-                r"\"\"\" *#", modified_tokens[_idx - 4][4]
-            )
+            _comment_follows = re.search(r"\"\"\" *#", modified_tokens[_idx - 4][4])
 
             if (
                 _token[0] == 1
                 and not _is_definition
                 and not _is_docstring
                 and not _comment_follows
                 and _after_definition
@@ -333,17 +325,15 @@
 
         Parameters
         ----------
         source: str
             The text from the source file.
         """
         try:
-            _original_newline = self.encodor.do_find_newline(
-                source.splitlines(True)
-            )
+            _original_newline = self.encodor.do_find_newline(source.splitlines(True))
             _code = self._format_code(source)
 
             return _strings.normalize_line_endings(
                 _code.splitlines(True), _original_newline
             )
         except (tokenize.TokenError, IndentationError):
             return source
@@ -367,17 +357,15 @@
         if not source:
             return source
 
         if self.args.line_range is not None:
             assert self.args.line_range[0] > 0 and self.args.line_range[1] > 0
 
         if self.args.length_range is not None:
-            assert (
-                self.args.length_range[0] > 0 and self.args.length_range[1] > 0
-            )
+            assert self.args.length_range[0] > 0 and self.args.length_range[1] > 0
 
         modified_tokens = []
 
         sio = io.StringIO(source)
         previous_token_type = None
         only_comments_so_far = True
 
@@ -385,59 +373,52 @@
             for (
                 token_type,
                 token_string,
                 start,
                 end,
                 line,
             ) in tokenize.generate_tokens(sio.readline):
+                _token_string = token_string
                 if (
                     token_type == tokenize.STRING
                     and token_string.startswith(self.QUOTE_TYPES)
                     and (
                         previous_token_type == tokenize.INDENT
                         or previous_token_type == tokenize.NEWLINE
                         or only_comments_so_far
                     )
-                    and _util.is_in_range(
-                        self.args.line_range, start[0], end[0]
-                    )
+                    and _util.is_in_range(self.args.line_range, start[0], end[0])
                     and _util.has_correct_length(
                         self.args.length_range, start[0], end[0]
                     )
                 ):
                     indentation = " " * (len(line) - len(line.lstrip()))
-                    token_string = self._do_format_docstring(
+                    _token_string = self._do_format_docstring(
                         indentation,
                         token_string,
                     )
 
                 if token_type not in [
                     tokenize.COMMENT,
                     tokenize.NEWLINE,
                     tokenize.NL,
                 ]:
                     only_comments_so_far = False
 
                 previous_token_type = token_type
-                modified_tokens.append(
-                    (token_type, token_string, start, end, line)
-                )
+                modified_tokens.append((token_type, _token_string, start, end, line))
 
-            modified_tokens = _do_remove_blank_lines_after_definitions(
-                modified_tokens
-            )
-            modified_tokens = _do_remove_blank_lines_after_docstring(
-                modified_tokens
-            )
+            modified_tokens = _do_remove_blank_lines_after_definitions(modified_tokens)
+            modified_tokens = _do_remove_blank_lines_after_docstring(modified_tokens)
 
             return untokenize.untokenize(modified_tokens)
         except tokenize.TokenError:
             return source
 
-    def _do_format_docstring(
+    def _do_format_docstring(  # noqa PLR0911
         self,
         indentation: str,
         docstring: str,
     ) -> str:
         """Return formatted version of docstring.
 
         Parameters
@@ -475,24 +456,22 @@
         with contextlib.suppress(IndexError):
             if _links[0][0] == 0 and _links[0][1] == len(contents):
                 return docstring
 
         summary, description = _strings.split_summary_and_description(contents)
 
         # Leave docstrings with underlined summaries alone.
-        if (
-            _syntax.remove_section_header(description).strip()
-            != description.strip()
-        ):
+        if _syntax.remove_section_header(description).strip() != description.strip():
             return docstring
 
         if not self.args.force_wrap and (
             _syntax.is_some_sort_of_list(
                 summary,
                 self.args.non_strict,
+                self.args.style,
             )
             or _syntax.do_find_directives(summary)
         ):
             # Something is probably not right with the splitting.
             return docstring
 
         # Compensate for textwrap counting each tab in indentation as 1
@@ -590,33 +569,30 @@
         -------
         formatted_docstring : str
             The formatted docstring.
         """
         # Compensate for triple quotes by temporarily prepending 3 spaces.
         # This temporary prepending is undone below.
         initial_indent = (
-            indentation
-            if self.args.pre_summary_newline
-            else 3 * " " + indentation
-        )
-        pre_summary = (
-            "\n" + indentation if self.args.pre_summary_newline else ""
+            indentation if self.args.pre_summary_newline else 3 * " " + indentation
         )
+        pre_summary = "\n" + indentation if self.args.pre_summary_newline else ""
         summary = _syntax.wrap_summary(
             _strings.normalize_summary(summary, self.args.non_cap),
             wrap_length=self.args.wrap_summaries,
             initial_indent=initial_indent,
             subsequent_indent=indentation,
         ).lstrip()
         description = _syntax.wrap_description(
             description,
             indentation=indentation,
             wrap_length=self.args.wrap_descriptions,
             force_wrap=self.args.force_wrap,
             strict=self.args.non_strict,
+            style=self.args.style,
         )
         post_description = "\n" if self.args.post_description_blank else ""
         return f'''\
 {open_quote}{pre_summary}{summary}
 
 {description}{post_description}
 {indentation}"""\
@@ -653,10 +629,9 @@
                 ].strip(), quote.replace("'", '"')
             elif docstring.startswith(quote) and docstring.endswith(quote):
                 return docstring.split(quote, 1)[1].rsplit(quote, 1)[
                     0
                 ].strip(), quote.replace("'", '"')
 
         raise ValueError(
-            "docformatter only handles triple-quoted (single or double) "
-            "strings"
+            "docformatter only handles triple-quoted (single or double) " "strings"
         )
```

### Comparing `docformatter-1.7.0/src/docformatter/strings.py` & `docformatter-1.7.1/src/docformatter/strings.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,18 +23,18 @@
 # SOFTWARE.
 """This module provides docformatter string functions."""
 
 
 # Standard Library Imports
 import contextlib
 import re
-from typing import List
+from typing import List, Match, Optional, Union
 
 
-def find_shortest_indentation(lines):
+def find_shortest_indentation(lines: List[str]) -> str:
     """Determine the shortest indentation in a list of lines.
 
     Parameters
     ----------
     lines : list
         A list of lines to check indentation.
 
@@ -54,57 +54,69 @@
             _indent = line[:non_whitespace_index]
             if indentation is None or len(_indent) < len(indentation):
                 indentation = _indent
 
     return indentation or ""
 
 
-def is_probably_beginning_of_sentence(line):
+def is_probably_beginning_of_sentence(line: str) -> Union[Match[str], None, bool]:
     """Determine if the line begins a sentence.
 
     Parameters
     ----------
-    line:
+    line : str
         The line to be tested.
 
     Returns
     -------
-    is_beginning: bool
+    is_beginning : bool
         True if this token is the beginning of a sentence.
     """
     # Check heuristically for a parameter list.
     for token in ["@", "-", r"\*"]:
         if re.search(rf"\s{token}\s", line):
             return True
 
     stripped_line = line.strip()
     is_beginning_of_sentence = re.match(r"^[-@\)]", stripped_line)
     is_pydoc_ref = re.match(r"^:\w+:", stripped_line)
 
     return is_beginning_of_sentence and not is_pydoc_ref
 
 
-def normalize_line(line, newline):
+def normalize_line(line: str, newline: str) -> str:
     """Return line with fixed ending, if ending was present in line.
 
     Otherwise, does nothing.
+
+    Parameters
+    ----------
+    line : str
+        The line to normalize.
+    newline : str
+        The newline character to use for line endings.
+
+    Returns
+    -------
+    normalized_line : str
+        The supplied line with line endings replaced by the newline.
     """
     stripped = line.rstrip("\n\r")
     return stripped + newline if stripped != line else line
 
 
 def normalize_line_endings(lines, newline):
     """Return fixed line endings.
 
     All lines will be modified to use the most common line ending.
     """
     return "".join([normalize_line(line, newline) for line in lines])
 
 
-def normalize_summary(summary: str, noncap: List[str] = None) -> str:
+def normalize_summary(summary: str, noncap: Optional[List[str]] = None) -> str:
     """Return normalized docstring summary.
 
     A normalized docstring summary will have the first word capitalized and
     a period at the end.
 
     Parameters
     ----------
@@ -157,15 +169,15 @@
     rest = text
     delimiter = ""
     previous_delimiter = ""
 
     while rest:
         split = re.split(r"(\s)", rest, maxsplit=1)
         word = split[0]
-        if len(split) == 3:
+        if len(split) == 3:  # noqa PLR2004
             delimiter = split[1]
             rest = split[2]
         else:
             assert len(split) == 1
             delimiter = ""
             rest = ""
 
@@ -207,12 +219,11 @@
             )
 
     # Break on first sentence.
     split = split_first_sentence(contents)
     if split[0].strip() and split[1].strip():
         return (
             split[0].strip(),
-            find_shortest_indentation(split[1].splitlines()[1:])
-            + split[1].strip(),
+            find_shortest_indentation(split[1].splitlines()[1:]) + split[1].strip(),
         )
 
     return contents, ""
```

### Comparing `docformatter-1.7.0/src/docformatter/util.py` & `docformatter-1.7.1/src/docformatter/util.py`

 * *Files identical despite different names*

### Comparing `docformatter-1.7.0/setup.py` & `docformatter-1.7.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['charset_normalizer>=3.0.0,<4.0.0', 'untokenize>=0.1.1,<0.2.0']
 
 extras_require = \
-{'tomli': ['tomli>=2.0.0,<3.0.0']}
+{'tomli:python_version < "3.11"': ['tomli>=2.0.0,<3.0.0']}
 
 entry_points = \
 {'console_scripts': ['docformatter = docformatter.__main__:main']}
 
 setup_kwargs = {
     'name': 'docformatter',
-    'version': '1.7.0',
+    'version': '1.7.1',
     'description': 'Formats docstrings to follow PEP 257',
-    'long_description': '============\ndocformatter\n============\n\n.. |CI| image:: https://img.shields.io/github/actions/workflow/status/PyCQA/docformatter/ci.yml?branch=master\n    :target: https://github.com/PyCQA/docformatter/actions/workflows/ci.yml\n.. |COVERALLS| image:: https://img.shields.io/coveralls/github/PyCQA/docformatter\n    :target: https://coveralls.io/github/PyCQA/docformatter\n.. |CONTRIBUTORS| image:: https://img.shields.io/github/contributors/PyCQA/docformatter\n    :target: https://github.com/PyCQA/docformatter/graphs/contributors\n.. |COMMIT| image:: https://img.shields.io/github/last-commit/PyCQA/docformatter\n.. |BLACK| image:: https://img.shields.io/badge/%20style-black-000000.svg\n    :target: https://github.com/psf/black\n.. |ISORT| image:: https://img.shields.io/badge/%20imports-isort-%231674b1\n    :target: https://pycqa.github.io/isort/\n.. |SELF| image:: https://img.shields.io/badge/%20formatter-docformatter-fedcba.svg\n    :target: https://github.com/PyCQA/docformatter\n.. |SPHINXSTYLE| image:: https://img.shields.io/badge/%20style-sphinx-0a507a.svg\n    :target: https://www.sphinx-doc.org/en/master/usage/index.html\n.. |NUMPSTYLE| image:: https://img.shields.io/badge/%20style-numpy-459db9.svg\n    :target: https://numpydoc.readthedocs.io/en/latest/format.html\n.. |GOOGSTYLE| image:: https://img.shields.io/badge/%20style-google-3666d6.svg\n    :target: https://google.github.io/styleguide/pyguide.html#s3.8-comments-and-docstrings\n\n.. |VERSION| image:: https://img.shields.io/pypi/v/docformatter\n.. |LICENSE| image:: https://img.shields.io/pypi/l/docformatter\n.. |PYVERS| image:: https://img.shields.io/pypi/pyversions/docformatter\n.. |PYMAT| image:: https://img.shields.io/pypi/format/docformatter\n.. |DD| image:: https://img.shields.io/pypi/dd/docformatter\n.. |PRE| image:: https://img.shields.io/github/v/release/PyCQA/docformatter?include_prereleases\n\n+----------------+----------------------------------------------------------+\n| **Code**       + |BLACK| |ISORT|                                          +\n+----------------+----------------------------------------------------------+\n| **Docstrings** + |SELF| |NUMPSTYLE|                                       +\n+----------------+----------------------------------------------------------+\n| **GitHub**     + |CI| |CONTRIBUTORS| |COMMIT| |PRE|                       +\n+----------------+----------------------------------------------------------+\n| **PyPi**       + |VERSION| |LICENSE| |PYVERS| |PYMAT| |DD|                +\n+----------------+----------------------------------------------------------+\n\nFormats docstrings to follow `PEP 257`_.\n\n.. _`PEP 257`: http://www.python.org/dev/peps/pep-0257/\n\nFeatures\n========\n\n``docformatter`` automatically formats docstrings to follow a subset of the PEP\n257 conventions. Below are the relevant items quoted from PEP 257.\n\n- For consistency, always use triple double quotes around docstrings.\n- Triple quotes are used even though the string fits on one line.\n- Multi-line docstrings consist of a summary line just like a one-line\n  docstring, followed by a blank line, followed by a more elaborate\n  description.\n- Unless the entire docstring fits on a line, place the closing quotes\n  on a line by themselves.\n\n``docformatter`` also handles some of the PEP 8 conventions.\n\n- Don\'t write string literals that rely on significant trailing\n  whitespace. Such trailing whitespace is visually indistinguishable\n  and some editors (or more recently, reindent.py) will trim them.\n\nSee the the full documentation at `read-the-docs`_, especially the\n`requirements`_ section for a more detailed discussion of PEP 257 and other\nrequirements.\n\n.. _read-the-docs: https://docformatter.readthedocs.io\n.. _requirements: https://docformatter.readthedocs.io/en/latest/requirements.html\n\nInstallation\n============\n\nFrom pip::\n\n    $ pip install --upgrade docformatter\n\nOr, if you want to use pyproject.toml to configure docformatter::\n\n    $ pip install --upgrade docformatter[tomli]\n\nOr, if you want to use a release candidate (or any other tag)::\n\n    $ pip install git+https://github.com/PyCQA/docformatter.git@<RC_TAG>\n\nWhere <RC_TAG> is the release candidate tag you\'d like to install.  Release\ncandidate tags will have the format v1.6.0-rc1  Release candidates will also be\nmade available as a Github Release.\n\nExample\n=======\n\nAfter running::\n\n    $ docformatter --in-place example.py\n\nthis code\n\n.. code-block:: python\n\n    """   Here are some examples.\n\n        This module docstring should be dedented."""\n\n\n    def launch_rocket():\n        """Launch\n    the\n    rocket. Go colonize space."""\n\n\n    def factorial(x):\n        \'\'\'\n\n        Return x factorial.\n\n        This uses math.factorial.\n\n        \'\'\'\n        import math\n        return math.factorial(x)\n\n\n    def print_factorial(x):\n        """Print x factorial"""\n        print(factorial(x))\n\n\n    def main():\n        """Main\n        function"""\n        print_factorial(5)\n        if factorial(10):\n            launch_rocket()\n\n\ngets formatted into this\n\n.. code-block:: python\n\n    """Here are some examples.\n\n    This module docstring should be dedented.\n    """\n\n\n    def launch_rocket():\n        """Launch the rocket.\n\n        Go colonize space.\n        """\n\n\n    def factorial(x):\n        """Return x factorial.\n\n        This uses math.factorial.\n        """\n        import math\n        return math.factorial(x)\n\n\n    def print_factorial(x):\n        """Print x factorial."""\n        print(factorial(x))\n\n\n    def main():\n        """Main function."""\n        print_factorial(5)\n        if factorial(10):\n            launch_rocket()\n\nMarketing\n=========\nDo you use *docformatter*?  What style docstrings do you use?  Add some badges to your project\'s **README** and let everyone know.\n\n|SELF|\n\n.. code-block::\n\n    .. image:: https://img.shields.io/badge/%20formatter-docformatter-fedcba.svg\n        :target: https://github.com/PyCQA/docformatter\n\n|SPHINXSTYLE|\n\n.. code-block::\n\n    .. image:: https://img.shields.io/badge/%20style-sphinx-0a507a.svg\n        :target: https://www.sphinx-doc.org/en/master/usage/index.html\n\n|NUMPSTYLE|\n\n.. code-block::\n\n    .. image:: https://img.shields.io/badge/%20style-numpy-459db9.svg\n        :target: https://numpydoc.readthedocs.io/en/latest/format.html\n\n|GOOGSTYLE|\n\n.. code-block::\n\n    .. image:: https://img.shields.io/badge/%20style-google-3666d6.svg\n        :target: https://google.github.io/styleguide/pyguide.html#s3.8-comments-and-docstrings\n\nIssues\n======\n\nBugs and patches can be reported on the `GitHub page`_.\n\n.. _`GitHub page`: https://github.com/PyCQA/docformatter/issues\n',
+    'long_description': '============\ndocformatter\n============\n\n.. |CI| image:: https://img.shields.io/github/actions/workflow/status/PyCQA/docformatter/ci.yml?branch=master\n    :target: https://github.com/PyCQA/docformatter/actions/workflows/ci.yml\n.. |COVERALLS| image:: https://img.shields.io/coveralls/github/PyCQA/docformatter\n    :target: https://coveralls.io/github/PyCQA/docformatter\n.. |CONTRIBUTORS| image:: https://img.shields.io/github/contributors/PyCQA/docformatter\n    :target: https://github.com/PyCQA/docformatter/graphs/contributors\n.. |COMMIT| image:: https://img.shields.io/github/last-commit/PyCQA/docformatter\n.. |BLACK| image:: https://img.shields.io/badge/%20style-black-000000.svg\n    :target: https://github.com/psf/black\n.. |ISORT| image:: https://img.shields.io/badge/%20imports-isort-%231674b1\n    :target: https://pycqa.github.io/isort/\n.. |SELF| image:: https://img.shields.io/badge/%20formatter-docformatter-fedcba.svg\n    :target: https://github.com/PyCQA/docformatter\n.. |SPHINXSTYLE| image:: https://img.shields.io/badge/%20style-sphinx-0a507a.svg\n    :target: https://www.sphinx-doc.org/en/master/usage/index.html\n.. |NUMPSTYLE| image:: https://img.shields.io/badge/%20style-numpy-459db9.svg\n    :target: https://numpydoc.readthedocs.io/en/latest/format.html\n.. |GOOGSTYLE| image:: https://img.shields.io/badge/%20style-google-3666d6.svg\n    :target: https://google.github.io/styleguide/pyguide.html#s3.8-comments-and-docstrings\n\n.. |VERSION| image:: https://img.shields.io/pypi/v/docformatter\n.. |LICENSE| image:: https://img.shields.io/pypi/l/docformatter\n.. |PYVERS| image:: https://img.shields.io/pypi/pyversions/docformatter\n.. |PYMAT| image:: https://img.shields.io/pypi/format/docformatter\n.. |DD| image:: https://img.shields.io/pypi/dd/docformatter\n.. |PRE| image:: https://img.shields.io/github/v/release/PyCQA/docformatter?include_prereleases\n\n+----------------+----------------------------------------------------------+\n| **Code**       + |BLACK| |ISORT|                                          +\n+----------------+----------------------------------------------------------+\n| **Docstrings** + |SELF| |NUMPSTYLE|                                       +\n+----------------+----------------------------------------------------------+\n| **GitHub**     + |CI| |CONTRIBUTORS| |COMMIT| |PRE|                       +\n+----------------+----------------------------------------------------------+\n| **PyPi**       + |VERSION| |LICENSE| |PYVERS| |PYMAT| |DD|                +\n+----------------+----------------------------------------------------------+\n\nFormats docstrings to follow `PEP 257`_.\n\n.. _`PEP 257`: http://www.python.org/dev/peps/pep-0257/\n\nFeatures\n========\n\n``docformatter`` automatically formats docstrings to follow a subset of the PEP\n257 conventions. Below are the relevant items quoted from PEP 257.\n\n- For consistency, always use triple double quotes around docstrings.\n- Triple quotes are used even though the string fits on one line.\n- Multi-line docstrings consist of a summary line just like a one-line\n  docstring, followed by a blank line, followed by a more elaborate\n  description.\n- Unless the entire docstring fits on a line, place the closing quotes\n  on a line by themselves.\n\n``docformatter`` also handles some of the PEP 8 conventions.\n\n- Don\'t write string literals that rely on significant trailing\n  whitespace. Such trailing whitespace is visually indistinguishable\n  and some editors (or more recently, reindent.py) will trim them.\n\n``docformatter`` formats docstrings compatible with ``black`` when passed the\n``--black`` option.\n\n``docformatter`` formats field lists that use Epytext or Sphinx styles.\n\nSee the the full documentation at `read-the-docs`_, especially the\n`requirements`_ section for a more detailed discussion of PEP 257 and other\nrequirements.\n\n.. _read-the-docs: https://docformatter.readthedocs.io\n.. _requirements: https://docformatter.readthedocs.io/en/latest/requirements.html\n\nInstallation\n============\n\nFrom pip::\n\n    $ pip install --upgrade docformatter\n\nOr, if you want to use pyproject.toml to configure docformatter and you\'re using\nPython < 3.11::\n\n    $ pip install --upgrade docformatter[tomli]\n\nWith Python >=3.11, ``tomllib`` from the standard library is used.\n\nOr, if you want to use a release candidate (or any other tag)::\n\n    $ pip install git+https://github.com/PyCQA/docformatter.git@<RC_TAG>\n\nWhere <RC_TAG> is the release candidate tag you\'d like to install.  Release\ncandidate tags will have the format v1.6.0-rc1  Release candidates will also be\nmade available as a Github Release.\n\nExample\n=======\n\nAfter running::\n\n    $ docformatter --in-place example.py\n\nthis code\n\n.. code-block:: python\n\n    """   Here are some examples.\n\n        This module docstring should be dedented."""\n\n\n    def launch_rocket():\n        """Launch\n    the\n    rocket. Go colonize space."""\n\n\n    def factorial(x):\n        \'\'\'\n\n        Return x factorial.\n\n        This uses math.factorial.\n\n        \'\'\'\n        import math\n        return math.factorial(x)\n\n\n    def print_factorial(x):\n        """Print x factorial"""\n        print(factorial(x))\n\n\n    def main():\n        """Main\n        function"""\n        print_factorial(5)\n        if factorial(10):\n            launch_rocket()\n\n\ngets formatted into this\n\n.. code-block:: python\n\n    """Here are some examples.\n\n    This module docstring should be dedented.\n    """\n\n\n    def launch_rocket():\n        """Launch the rocket.\n\n        Go colonize space.\n        """\n\n\n    def factorial(x):\n        """Return x factorial.\n\n        This uses math.factorial.\n        """\n        import math\n        return math.factorial(x)\n\n\n    def print_factorial(x):\n        """Print x factorial."""\n        print(factorial(x))\n\n\n    def main():\n        """Main function."""\n        print_factorial(5)\n        if factorial(10):\n            launch_rocket()\n\nMarketing\n=========\nDo you use *docformatter*?  What style docstrings do you use?  Add some badges to your project\'s **README** and let everyone know.\n\n|SELF|\n\n.. code-block::\n\n    .. image:: https://img.shields.io/badge/%20formatter-docformatter-fedcba.svg\n        :target: https://github.com/PyCQA/docformatter\n\n|SPHINXSTYLE|\n\n.. code-block::\n\n    .. image:: https://img.shields.io/badge/%20style-sphinx-0a507a.svg\n        :target: https://www.sphinx-doc.org/en/master/usage/index.html\n\n|NUMPSTYLE|\n\n.. code-block::\n\n    .. image:: https://img.shields.io/badge/%20style-numpy-459db9.svg\n        :target: https://numpydoc.readthedocs.io/en/latest/format.html\n\n|GOOGSTYLE|\n\n.. code-block::\n\n    .. image:: https://img.shields.io/badge/%20style-google-3666d6.svg\n        :target: https://google.github.io/styleguide/pyguide.html#s3.8-comments-and-docstrings\n\nIssues\n======\n\nBugs and patches can be reported on the `GitHub page`_.\n\n.. _`GitHub page`: https://github.com/PyCQA/docformatter/issues\n',
     'author': 'Steven Myint',
     'author_email': 'None',
     'maintainer': 'Doyle Rowland',
     'maintainer_email': 'doyle.rowland@reliaqual.com',
     'url': 'https://github.com/PyCQA/docformatter',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `docformatter-1.7.0/PKG-INFO` & `docformatter-1.7.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docformatter
-Version: 1.7.0
+Version: 1.7.1
 Summary: Formats docstrings to follow PEP 257
 Home-page: https://github.com/PyCQA/docformatter
 License: Expat
 Keywords: PEP 257,pep257,style,formatter,docstrings
 Author: Steven Myint
 Maintainer: Doyle Rowland
 Maintainer-email: doyle.rowland@reliaqual.com
@@ -26,15 +26,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Provides-Extra: tomli
 Requires-Dist: charset_normalizer (>=3.0.0,<4.0.0)
-Requires-Dist: tomli (>=2.0.0,<3.0.0) ; extra == "tomli"
+Requires-Dist: tomli (>=2.0.0,<3.0.0) ; (python_version < "3.11") and (extra == "tomli")
 Requires-Dist: untokenize (>=0.1.1,<0.2.0)
 Project-URL: Documentation, https://github.com/PyCQA/docformatter
 Project-URL: Repository, https://github.com/PyCQA/docformatter
 Description-Content-Type: text/x-rst
 
 ============
 docformatter
@@ -97,32 +97,40 @@
 
 ``docformatter`` also handles some of the PEP 8 conventions.
 
 - Don't write string literals that rely on significant trailing
   whitespace. Such trailing whitespace is visually indistinguishable
   and some editors (or more recently, reindent.py) will trim them.
 
+``docformatter`` formats docstrings compatible with ``black`` when passed the
+``--black`` option.
+
+``docformatter`` formats field lists that use Epytext or Sphinx styles.
+
 See the the full documentation at `read-the-docs`_, especially the
 `requirements`_ section for a more detailed discussion of PEP 257 and other
 requirements.
 
 .. _read-the-docs: https://docformatter.readthedocs.io
 .. _requirements: https://docformatter.readthedocs.io/en/latest/requirements.html
 
 Installation
 ============
 
 From pip::
 
     $ pip install --upgrade docformatter
 
-Or, if you want to use pyproject.toml to configure docformatter::
+Or, if you want to use pyproject.toml to configure docformatter and you're using
+Python < 3.11::
 
     $ pip install --upgrade docformatter[tomli]
 
+With Python >=3.11, ``tomllib`` from the standard library is used.
+
 Or, if you want to use a release candidate (or any other tag)::
 
     $ pip install git+https://github.com/PyCQA/docformatter.git@<RC_TAG>
 
 Where <RC_TAG> is the release candidate tag you'd like to install.  Release
 candidate tags will have the format v1.6.0-rc1  Release candidates will also be
 made available as a Github Release.
```

