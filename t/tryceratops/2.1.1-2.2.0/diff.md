# Comparing `tmp/tryceratops-2.1.1.tar.gz` & `tmp/tryceratops-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tryceratops-2.1.1.tar", max compression
+gzip compressed data, was "tryceratops-2.2.0.tar", max compression
```

## Comparing `tryceratops-2.1.1.tar` & `tryceratops-2.2.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0     1084 2023-05-18 08:27:50.690437 tryceratops-2.1.1/LICENSE
--rw-r--r--   0        0        0     6179 2023-05-18 08:28:24.286208 tryceratops-2.1.1/README.md
--rw-r--r--   0        0        0     2146 2023-05-18 08:28:24.330208 tryceratops-2.1.1/pyproject.toml
--rw-r--r--   0        0        0       69 2023-05-18 08:28:24.282209 tryceratops-2.1.1/src/tryceratops/__init__.py
--rw-r--r--   0        0        0     2220 2023-05-18 08:27:50.694437 tryceratops-2.1.1/src/tryceratops/__main__.py
--rw-r--r--   0        0        0     1090 2023-05-18 08:27:50.694437 tryceratops-2.1.1/src/tryceratops/analyzers/__init__.py
--rw-r--r--   0        0        0     1746 2023-05-18 08:27:50.694437 tryceratops-2.1.1/src/tryceratops/analyzers/base.py
--rw-r--r--   0        0        0     5616 2023-05-18 08:27:50.694437 tryceratops-2.1.1/src/tryceratops/analyzers/call.py
--rw-r--r--   0        0        0     2154 2023-05-18 08:27:50.694437 tryceratops-2.1.1/src/tryceratops/analyzers/conditional.py
--rw-r--r--   0        0        0     6385 2023-05-18 08:27:50.694437 tryceratops-2.1.1/src/tryceratops/analyzers/exception_block.py
--rw-r--r--   0        0        0      342 2023-05-18 08:27:50.694437 tryceratops-2.1.1/src/tryceratops/analyzers/exceptions.py
--rw-r--r--   0        0        0     1192 2023-05-18 08:27:50.694437 tryceratops-2.1.1/src/tryceratops/analyzers/try_block.py
--rw-r--r--   0        0        0       50 2023-05-18 08:27:50.694437 tryceratops-2.1.1/src/tryceratops/files/__init__.py
--rw-r--r--   0        0        0     3610 2023-05-18 08:27:50.694437 tryceratops-2.1.1/src/tryceratops/files/discovery.py
--rw-r--r--   0        0        0     1454 2023-05-18 08:27:50.694437 tryceratops-2.1.1/src/tryceratops/files/parser.py
--rw-r--r--   0        0        0     3126 2023-05-18 08:27:50.694437 tryceratops-2.1.1/src/tryceratops/filters.py
--rw-r--r--   0        0        0      601 2023-05-18 08:27:50.694437 tryceratops-2.1.1/src/tryceratops/fixers/__init__.py
--rw-r--r--   0        0        0     2653 2023-05-18 08:27:50.694437 tryceratops-2.1.1/src/tryceratops/fixers/base.py
--rw-r--r--   0        0        0     2747 2023-05-18 08:27:50.694437 tryceratops-2.1.1/src/tryceratops/fixers/exception_block.py
--rw-r--r--   0        0        0      353 2023-05-18 08:27:50.694437 tryceratops-2.1.1/src/tryceratops/fixers/exceptions.py
--rw-r--r--   0        0        0     2121 2023-05-18 08:27:50.694437 tryceratops-2.1.1/src/tryceratops/flake_plugin.py
--rw-r--r--   0        0        0     2715 2023-05-18 08:27:50.694437 tryceratops-2.1.1/src/tryceratops/interfaces.py
--rw-r--r--   0        0        0      165 2023-05-18 08:27:50.698437 tryceratops-2.1.1/src/tryceratops/processors.py
--rw-r--r--   0        0        0     3030 2023-05-18 08:27:50.698437 tryceratops-2.1.1/src/tryceratops/runners.py
--rw-r--r--   0        0        0     1065 2023-05-18 08:27:50.698437 tryceratops-2.1.1/src/tryceratops/settings.py
--rw-r--r--   0        0        0      629 2023-05-18 08:27:50.698437 tryceratops-2.1.1/src/tryceratops/types.py
--rw-r--r--   0        0        0      108 2023-05-18 08:27:50.698437 tryceratops-2.1.1/src/tryceratops/violations/__init__.py
--rw-r--r--   0        0        0     1389 2023-05-18 08:27:50.698437 tryceratops-2.1.1/src/tryceratops/violations/codes.py
--rw-r--r--   0        0        0     1773 2023-05-18 08:27:50.698437 tryceratops-2.1.1/src/tryceratops/violations/violations.py
--rw-r--r--   0        0        0     7358 1970-01-01 00:00:00.000000 tryceratops-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-05-20 10:03:31.429943 tryceratops-2.2.0/LICENSE
+-rw-r--r--   0        0        0     6203 2023-05-20 10:03:57.613667 tryceratops-2.2.0/README.md
+-rw-r--r--   0        0        0     2243 2023-05-20 10:03:57.665665 tryceratops-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0       69 2023-05-20 10:03:57.613667 tryceratops-2.2.0/src/tryceratops/__init__.py
+-rw-r--r--   0        0        0     2220 2023-05-20 10:03:31.433943 tryceratops-2.2.0/src/tryceratops/__main__.py
+-rw-r--r--   0        0        0     1130 2023-05-20 10:03:31.433943 tryceratops-2.2.0/src/tryceratops/analyzers/__init__.py
+-rw-r--r--   0        0        0     1754 2023-05-20 10:03:31.433943 tryceratops-2.2.0/src/tryceratops/analyzers/base.py
+-rw-r--r--   0        0        0     5624 2023-05-20 10:03:31.433943 tryceratops-2.2.0/src/tryceratops/analyzers/call.py
+-rw-r--r--   0        0        0     1584 2023-05-20 10:03:31.433943 tryceratops-2.2.0/src/tryceratops/analyzers/classdefs.py
+-rw-r--r--   0        0        0     2154 2023-05-20 10:03:31.433943 tryceratops-2.2.0/src/tryceratops/analyzers/conditional.py
+-rw-r--r--   0        0        0     6385 2023-05-20 10:03:31.433943 tryceratops-2.2.0/src/tryceratops/analyzers/exception_block.py
+-rw-r--r--   0        0        0      350 2023-05-20 10:03:31.433943 tryceratops-2.2.0/src/tryceratops/analyzers/exceptions.py
+-rw-r--r--   0        0        0     1192 2023-05-20 10:03:31.433943 tryceratops-2.2.0/src/tryceratops/analyzers/try_block.py
+-rw-r--r--   0        0        0       50 2023-05-20 10:03:31.433943 tryceratops-2.2.0/src/tryceratops/files/__init__.py
+-rw-r--r--   0        0        0     3618 2023-05-20 10:03:31.433943 tryceratops-2.2.0/src/tryceratops/files/discovery.py
+-rw-r--r--   0        0        0     1454 2023-05-20 10:03:31.433943 tryceratops-2.2.0/src/tryceratops/files/parser.py
+-rw-r--r--   0        0        0     3476 2023-05-20 10:03:31.433943 tryceratops-2.2.0/src/tryceratops/filters.py
+-rw-r--r--   0        0        0      601 2023-05-20 10:03:31.433943 tryceratops-2.2.0/src/tryceratops/fixers/__init__.py
+-rw-r--r--   0        0        0     2713 2023-05-20 10:03:31.433943 tryceratops-2.2.0/src/tryceratops/fixers/base.py
+-rw-r--r--   0        0        0     2772 2023-05-20 10:03:31.433943 tryceratops-2.2.0/src/tryceratops/fixers/exception_block.py
+-rw-r--r--   0        0        0      361 2023-05-20 10:03:31.433943 tryceratops-2.2.0/src/tryceratops/fixers/exceptions.py
+-rw-r--r--   0        0        0     2129 2023-05-20 10:03:31.433943 tryceratops-2.2.0/src/tryceratops/flake_plugin.py
+-rw-r--r--   0        0        0     2723 2023-05-20 10:03:31.433943 tryceratops-2.2.0/src/tryceratops/interfaces.py
+-rw-r--r--   0        0        0      165 2023-05-20 10:03:31.433943 tryceratops-2.2.0/src/tryceratops/processors.py
+-rw-r--r--   0        0        0     3038 2023-05-20 10:03:31.433943 tryceratops-2.2.0/src/tryceratops/runners.py
+-rw-r--r--   0        0        0     1065 2023-05-20 10:03:31.433943 tryceratops-2.2.0/src/tryceratops/settings.py
+-rw-r--r--   0        0        0      740 2023-05-20 10:03:31.433943 tryceratops-2.2.0/src/tryceratops/types.py
+-rw-r--r--   0        0        0      108 2023-05-20 10:03:31.433943 tryceratops-2.2.0/src/tryceratops/violations/__init__.py
+-rw-r--r--   0        0        0     1610 2023-05-20 10:03:31.433943 tryceratops-2.2.0/src/tryceratops/violations/codes.py
+-rw-r--r--   0        0        0     1773 2023-05-20 10:03:31.433943 tryceratops-2.2.0/src/tryceratops/violations/violations.py
+-rw-r--r--   0        0        0     7403 1970-01-01 00:00:00.000000 tryceratops-2.2.0/PKG-INFO
```

### Comparing `tryceratops-2.1.1/LICENSE` & `tryceratops-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tryceratops-2.1.1/README.md` & `tryceratops-2.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -129,26 +129,27 @@
 
 Example:
 
 ```toml
 [tool.tryceratops]
 exclude = ["samples"]
 ignore = ["TRY002", "TRY200", "TRY300"]
-experimental = true
+experimental = false
+check_pickable = false
 ```
 
 CLI flags always overwrite the config file.
 
 ## Pre-commit
 
 If you wish to use pre-commit, add this:
 
 ```yaml
   - repo: https://github.com/guilatrova/tryceratops
-    rev: v2.1.1
+    rev: v2.2.0
     hooks:
       - id: tryceratops
 ```
 
 ## Show your style
 
 [![try/except style: tryceratops](https://img.shields.io/badge/try%2Fexcept%20style-tryceratops%20%F0%9F%A6%96%E2%9C%A8-black)](https://github.com/guilatrova/tryceratops)
```

### Comparing `tryceratops-2.1.1/pyproject.toml` & `tryceratops-2.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tryceratops"
-version = "2.1.1"
+version = "2.2.0"
 description = "Prevent Exception Handling AntiPatterns"
 authors = ["Guilherme Latrova <hello@guilatrova.dev>"]
 license = "MIT"
 keywords = ["lint", "try", "except"]
 readme = "README.md"
 homepage = "https://github.com/guilatrova/tryceratops"
 repository = "https://github.com/guilatrova/tryceratops"
@@ -28,14 +28,15 @@
 
 [tool.poetry.plugins."flake8.extension"]
 TRY = "tryceratops.flake_plugin:TryceratopsAdapterPlugin"
 
 [tool.poetry.urls]
 "Changelog" = "https://github.com/guilatrova/tryceratops/blob/main/CHANGELOG.md"
 
+
 [tool.semantic_release]
 version_variable = [
     "src/tryceratops/__init__.py:__version__"
 ]
 version_toml = [
     "pyproject.toml:tool.poetry.version"
 ]
@@ -45,39 +46,40 @@
 ]
 branch = "main"
 upload_to_pypi = true
 upload_to_release = true
 build_command = "pip install poetry && poetry build"
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = ">=3.8.1,<4.0"
 click = ">=7"
 toml = ">=0.10.2"
 rich = ">=10.14.0"
+typing-extensions = { version = ">=4.5.0", python = "<3.10" }
 
-[tool.poetry.dev-dependencies]
-pytest = "^6.2.4"
-flake8 = "^5.0.4"
-black = "^22.12.0"
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.3.1"
+pytest-cov = "^2.12.1"
+flake8 = "^6.0.0"
+flake8-annotations = "^3.0.1"
+black = "^23.3.0"
 isort = "^5.12.0"
 pre-commit = "^2.13.0"
-astpretty = "^2.1.0"
-pytest-cov = "^2.12.1"
-python-semantic-release = "^7.16.2"
-mypy = "^0.910"
+astpretty = "^3.0.0"
+python-semantic-release = "^7.33.5"
+mypy = "^1.3.0"
 types-toml = "^0.1.3"
-flake8-annotations = "^2.9.0"
 
 [tool.black]
 line-length = 100
 
 [tool.isort]
 profile = "black"
 line_length = 100
-extra_standard_library = ["pytest", "toml", "click"]
+extra_standard_library = ["pytest", "toml", "click", "typing_extensions"]
 
 [tool.mypy]
 python_version = 3.8
 warn_unused_configs = true
 namespace_packages = true
 explicit_package_bases = true
 ignore_missing_imports = true
```

### Comparing `tryceratops-2.1.1/src/tryceratops/__main__.py` & `tryceratops-2.2.0/src/tryceratops/__main__.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.1.1/src/tryceratops/analyzers/__init__.py` & `tryceratops-2.2.0/src/tryceratops/analyzers/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Set, Type, cast
+from typing import TYPE_CHECKING, Set, Type
 
-from . import call, conditional, exception_block, try_block
+from . import call, classdefs, conditional, exception_block, try_block
 from .base import BaseAnalyzer
 
 if TYPE_CHECKING:
     from tryceratops.filters import GlobalSettings
 
 
 ANALYZER_CLASSES: Set[Type[BaseAnalyzer]] = {
     call.CallTooManyAnalyzer,
     call.CallRaiseVanillaAnalyzer,
     call.CallRaiseLongArgsAnalyzer,
     call.CallAvoidCheckingToContinueAnalyzer,
     conditional.PreferTypeErrorAnalyzer,
+    classdefs.NonPickableAnalyzer,
     exception_block.ExceptReraiseWithoutCauseAnalyzer,
     exception_block.ExceptVerboseReraiseAnalyzer,
     exception_block.ExceptBroadPassAnalyzer,
     exception_block.LogErrorAnalyzer,
     exception_block.LogObjectAnalyzer,
     exception_block.UselessTryExceptAnalyzer,
     try_block.TryConsiderElseAnalyzer,
```

### Comparing `tryceratops-2.1.1/src/tryceratops/analyzers/base.py` & `tryceratops-2.2.0/src/tryceratops/analyzers/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from .exceptions import AnalyzerVisitException
 
 
 class BaseAnalyzer(ABC, Processor, ast.NodeVisitor):
     violation_type: Type[Violation] = Violation
 
-    def __init__(self):
+    def __init__(self) -> None:
         self.violations: List[Violation] = []
 
     def _mark_violation(self, *nodes: ast.AST, **kwargs: Any) -> None:  # noqa: ANN401
         klass = self.violation_type
         for node in nodes:
             violation = klass.build(self.filename, self.violation_code, node, **kwargs)
             self.violations.append(violation)
```

### Comparing `tryceratops-2.1.1/src/tryceratops/analyzers/call.py` & `tryceratops-2.2.0/src/tryceratops/analyzers/call.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
                 self._mark_violation(node)
 
 
 class CallAvoidCheckingToContinueAnalyzer(BaseAnalyzer):
     EXPERIMENTAL = True
     violation_code = codes.CHECK_TO_CONTINUE
 
-    def __init__(self):
+    def __init__(self) -> None:
         self.assignments_from_calls: Dict[str, ast.Assign] = {}
         super().__init__()
 
     def _scan_assignments(self, node: StmtBodyProtocol) -> None:
         def is_assigned_from_call(node: ast.stmt) -> bool:
             if isinstance(node, ast.Assign):
                 if isinstance(node.value, ast.Call):
```

### Comparing `tryceratops-2.1.1/src/tryceratops/analyzers/conditional.py` & `tryceratops-2.2.0/src/tryceratops/analyzers/conditional.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.1.1/src/tryceratops/analyzers/exception_block.py` & `tryceratops-2.2.0/src/tryceratops/analyzers/exception_block.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.1.1/src/tryceratops/analyzers/try_block.py` & `tryceratops-2.2.0/src/tryceratops/analyzers/try_block.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.1.1/src/tryceratops/files/discovery.py` & `tryceratops-2.2.0/src/tryceratops/files/discovery.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 class FileParseFailed:
     filename: str
     reason: str
     exception: Exception
 
 
 class FileDiscovery:
-    def __init__(self):
+    def __init__(self) -> None:
         self.failures: List[FileParseFailed] = []
 
     @property
     def had_issues(self) -> bool:
         return len(self.failures) > 0
 
     def _parse_python_files_from_dir(self, dir: str) -> Generator[ParsedFileType, None, None]:
```

### Comparing `tryceratops-2.1.1/src/tryceratops/files/parser.py` & `tryceratops-2.2.0/src/tryceratops/files/parser.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.1.1/src/tryceratops/filters.py` & `tryceratops-2.2.0/src/tryceratops/filters.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Iterable, Optional, Type
 
 from tryceratops.processors import Processor
 from tryceratops.violations import Violation
+from tryceratops.violations.codes import NON_PICKABLE_CLASS
 
 if TYPE_CHECKING:
     from tryceratops.types import PyprojectConfig
 
 
 @dataclass
 class IgnoreViolation:
@@ -50,21 +51,25 @@
     Represents a filter applied to the runner
     (i.e. which processes to run, and what files to ignore).
     """
 
     include_experimental: bool
     ignore_violations: Iterable[str]
     exclude_dirs: Iterable[str]
+    check_pickable: bool = False
     autofix: bool = False
 
     def _self_check(self) -> None:
         self.exclude_dirs = [excluded for excluded in self.exclude_dirs if excluded]
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         self._self_check()
+        if self.check_pickable is False:
+            self.ignore_violations = list(self.ignore_violations)
+            self.ignore_violations.append(NON_PICKABLE_CLASS[0])
 
     @property
     def exclude_experimental(self) -> bool:
         return not self.include_experimental
 
     def should_run_processor(self, processor: Type[Processor]) -> bool:
         code, _ = processor.violation_code
@@ -84,16 +89,17 @@
 
     @classmethod
     def create_from_config(cls, config: PyprojectConfig) -> GlobalSettings:
         experimental = config.get("experimental", False)
         ignore = config.get("ignore", [])
         exclude = config.get("exclude", [])
         autofix = config.get("autofix", False)
+        check_pickable = config.get("check_pickable", False)
 
-        return cls(experimental, ignore, exclude, autofix)
+        return cls(experimental, ignore, exclude, check_pickable, autofix)
 
     def overwrite_from_cli(
         self,
         include_experimental: bool,
         ignore_violations: Iterable[str],
         exclude_dirs: Iterable[str],
         autofix: bool,
```

### Comparing `tryceratops-2.1.1/src/tryceratops/fixers/__init__.py` & `tryceratops-2.2.0/src/tryceratops/fixers/__init__.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.1.1/src/tryceratops/fixers/base.py` & `tryceratops-2.2.0/src/tryceratops/fixers/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from abc import ABC, abstractmethod
 from collections import defaultdict
 from types import TracebackType
 from typing import Dict, Generic, Iterable, List, Optional, Type, TypeVar
 
 from tryceratops.processors import Processor
 from tryceratops.violations import Violation
@@ -9,21 +11,21 @@
 from .exceptions import FixerFixException
 
 ViolationType = TypeVar("ViolationType", bound=Violation)
 GroupedViolations = Dict[str, List[ViolationType]]
 
 
 class FileFixerHandler:
-    def __init__(self, filename: str):
+    def __init__(self, filename: str) -> None:
         self.file = open(filename, "r+", encoding="utf-8")
 
-    def __enter__(self):
+    def __enter__(self) -> FileFixerHandler:
         return self
 
-    def read_lines(self) -> Iterable[str]:
+    def read_lines(self) -> List[str]:
         lines = self.file.readlines()
         self.file.seek(0)
         return lines
 
     def write_fix(self, new_lines: Iterable[str]) -> None:
         self.file.writelines(new_lines)
         self.file.truncate()
```

### Comparing `tryceratops-2.1.1/src/tryceratops/fixers/exception_block.py` & `tryceratops-2.2.0/src/tryceratops/fixers/exception_block.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,52 @@
 import ast
 import re
-from typing import List
+import typing as t
 
 from tryceratops.violations import codes
 from tryceratops.violations.violations import (
     RaiseWithoutCauseViolation,
     VerboseReraiseViolation,
     Violation,
 )
 
 from .base import BaseFixer
 
 
 class VerboseReraiseFixer(BaseFixer[VerboseReraiseViolation]):
     violation_code = codes.VERBOSE_RERAISE
 
-    def perform_fix(self, lines: List[str], violation: VerboseReraiseViolation) -> List[str]:
+    def perform_fix(self, lines: t.List[str], violation: VerboseReraiseViolation) -> t.List[str]:
         all_lines = lines[:]
 
         guilty_line = all_lines[violation.line - 1]
         new_line = re.sub(rf"raise {violation.exception_name}", "raise", guilty_line)
         all_lines[violation.line - 1] = new_line
 
         return all_lines
 
 
 class RaiseWithoutCauseFixer(BaseFixer[RaiseWithoutCauseViolation]):
     violation_code = codes.RERAISE_NO_CAUSE
     exception_name_to_create = "ex"
 
-    def _fix_except_handler(self, all_lines: List[str], offending_node: ast.ExceptHandler) -> None:
+    def _fix_except_handler(
+        self, all_lines: t.List[str], offending_node: ast.ExceptHandler
+    ) -> None:
         line_offset = offending_node.lineno - 1
         offending_line = all_lines[line_offset]
 
         new_line = re.sub(
             r"except (.*):", rf"except \1 as {self.exception_name_to_create}:", offending_line
         )
 
         all_lines[line_offset] = new_line
 
     def _fix_raise_no_cause(
-        self, all_lines: List[str], violation: RaiseWithoutCauseViolation, exception_name: str
+        self, all_lines: t.List[str], violation: RaiseWithoutCauseViolation, exception_name: str
     ) -> None:
         endline = violation.node.end_lineno or violation.line
         is_singleline = violation.line == endline
 
         if is_singleline:
             fix_offset = violation.line - 1
             guilty_line = all_lines[fix_offset]
@@ -52,15 +54,15 @@
         else:
             fix_offset = endline - 1
             guilty_line = all_lines[fix_offset]
             new_line = re.sub(r"(\))(.*)", rf"\1 from {exception_name}\2", guilty_line)
 
         all_lines[fix_offset] = new_line
 
-    def perform_fix(self, lines: List[str], violation: RaiseWithoutCauseViolation) -> List[str]:
+    def perform_fix(self, lines: t.List[str], violation: RaiseWithoutCauseViolation) -> t.List[str]:
         all_lines = lines[:]
         exception_name = violation.exception_name
 
         if exception_name is None:
             self._fix_except_handler(all_lines, violation.except_node)
             exception_name = self.exception_name_to_create
 
@@ -68,15 +70,15 @@
 
         return all_lines
 
 
 class LoggerErrorFixer(BaseFixer[Violation]):
     violation_code = codes.USE_LOGGING_EXCEPTION
 
-    def perform_fix(self, lines: List[str], violation: Violation) -> List[str]:
+    def perform_fix(self, lines: t.List[str], violation: Violation) -> t.List[str]:
         all_lines = lines[:]
 
         guilty_line = all_lines[violation.line - 1]
         new_line = guilty_line.replace(".error(", ".exception(")
         all_lines[violation.line - 1] = new_line
 
         return all_lines
```

### Comparing `tryceratops-2.1.1/src/tryceratops/flake_plugin.py` & `tryceratops-2.2.0/src/tryceratops/flake_plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     version = importlib.metadata.version(PACKAGE_NAME)
 
     def __init__(
         self,
         tree: ast.AST,
         filename: str = "undefined",
         file_tokens: Iterable[TokenInfo] = [],
-    ):
+    ) -> None:
         self._tree = tree
         self._filename = filename
         self._runner = Runner()
 
         ignore_lines = list(parse_ignore_tokens(file_tokens))
         self._file_filter = FileFilter(ignore_lines)
         self._global_settings = self._create_global_settings(filename)
```

### Comparing `tryceratops-2.1.1/src/tryceratops/interfaces.py` & `tryceratops-2.2.0/src/tryceratops/interfaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     descstr = violation.description
     location = f"{violation.filename}:{violation.line}:{violation.col}"
 
     return f"[[yellow]{codestr}[/yellow]] [red]{descstr}[/red] - {location}"
 
 
 class CliInterface:
-    def __init__(self, runner: Runner, discovery: FileDiscovery):
+    def __init__(self, runner: Runner, discovery: FileDiscovery) -> None:
         self.runner = runner
         self.discovery = discovery
 
     def _present_violations(self) -> None:
         for violation in self.runner.violations:
             print(present_violation(violation))
```

### Comparing `tryceratops-2.1.1/src/tryceratops/runners.py` & `tryceratops-2.2.0/src/tryceratops/runners.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 class RuntimeError:
     filename: str
     processor: Type[Processor]
     exception: Exception
 
 
 class Runner:
-    def __init__(self):
+    def __init__(self) -> None:
         self.runtime_errors: List[RuntimeError] = []
         self.violations: List[Violation] = []
         self.analyzed_files = 0
         self.excluded_files = 0
         self.fixed_violations = 0
 
     def _clear(self) -> None:
```

### Comparing `tryceratops-2.1.1/src/tryceratops/settings.py` & `tryceratops-2.2.0/src/tryceratops/settings.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.1.1/src/tryceratops/types.py` & `tryceratops-2.2.0/src/tryceratops/types.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import ast
-from typing import Collection, List, Tuple, TypedDict
+import typing as t
+import typing_extensions as te
 
 from tryceratops.filters import FileFilter
 
-ParsedFileType = Tuple[str, ast.AST, FileFilter]
-ParsedFilesType = Collection[ParsedFileType]
+ParsedFileType = t.Tuple[str, ast.AST, FileFilter]
+ParsedFilesType = t.Collection[ParsedFileType]
 
 
-class PyprojectConfig(TypedDict):
+class PyprojectConfig(t.TypedDict):
     """
     Represents the expected pyproject config to be loaded
         exclude: a list of path patterns to be excluded e.g. [/tests, /fixtures]
         ignore: a list of violations to be completely ignored e.g. [TRY002, TRY300]
         experimental: whether to enable experimental analyzers
     """
 
-    exclude: List[str]
-    ignore: List[str]
-    experimental: bool
-    autofix: bool
+    exclude: te.NotRequired[t.List[str]]
+    ignore: te.NotRequired[t.List[str]]
+    experimental: te.NotRequired[bool]
+    autofix: te.NotRequired[bool]
+    check_pickable: te.NotRequired[bool]
```

### Comparing `tryceratops-2.1.1/src/tryceratops/violations/codes.py` & `tryceratops-2.2.0/src/tryceratops/violations/codes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # TRY0xx - Exceptions
 RAISE_VANILLA_CLASS = ("TRY002", "Create your own exception")
 RAISE_VANILLA_ARGS = (
     "TRY003",
     "Avoid specifying long messages outside the exception class",
 )
 PREFER_TYPE_ERROR = ("TRY004", "Prefer TypeError exception for invalid type")
+NON_PICKABLE_CLASS = ("TRY005", "Define __reduce__ to make exception pickable")
 
 # TRY1xx - General
 CHECK_TO_CONTINUE = (
     "TRY100",
     "Don't check to continue, make callable '{}' raise a exception instead",
 )
 TOO_MANY_TRY = ("TRY101", "Too many try blocks in your function")
@@ -27,20 +28,27 @@
 RAISE_WITHIN_TRY = ("TRY301", "Abstract raise to an inner function")
 
 # TRY4xx - Logging
 USE_LOGGING_EXCEPTION = ("TRY400", "Use logging '.exception' instead of '.error'")
 VERBOSE_LOG_MESSAGE = ("TRY401", "Do not log exception object, give context instead")
 
 CODE_CHOICES = {
+    # TRY0xx - Exceptions
     "TRY002",
     "TRY003",
+    "TRY004",
+    "TRY005",
+    # TRY1xx - General
     "TRY100",
     "TRY101",
+    # TRY2xx - Except
     "TRY200",
     "TRY201",
     "TRY202",
     "TRY203",
+    # TRY3xx - Try
     "TRY300",
     "TRY301",
+    # TRY4xx - Logging
     "TRY400",
     "TRY401",
 }
```

### Comparing `tryceratops-2.1.1/src/tryceratops/violations/violations.py` & `tryceratops-2.2.0/src/tryceratops/violations/violations.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.1.1/PKG-INFO` & `tryceratops-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: tryceratops
-Version: 2.1.1
+Version: 2.2.0
 Summary: Prevent Exception Handling AntiPatterns
 Home-page: https://github.com/guilatrova/tryceratops
 License: MIT
 Keywords: lint,try,except
 Author: Guilherme Latrova
 Author-email: hello@guilatrova.dev
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8.1,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Requires-Dist: click (>=7)
 Requires-Dist: rich (>=10.14.0)
 Requires-Dist: toml (>=0.10.2)
+Requires-Dist: typing-extensions (>=4.5.0) ; python_version < "3.10"
 Project-URL: Changelog, https://github.com/guilatrova/tryceratops/blob/main/CHANGELOG.md
 Project-URL: Repository, https://github.com/guilatrova/tryceratops
 Description-Content-Type: text/markdown
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/guilatrova/tryceratops/main/img/logo.png">
 </p>
@@ -158,26 +158,27 @@
 
 Example:
 
 ```toml
 [tool.tryceratops]
 exclude = ["samples"]
 ignore = ["TRY002", "TRY200", "TRY300"]
-experimental = true
+experimental = false
+check_pickable = false
 ```
 
 CLI flags always overwrite the config file.
 
 ## Pre-commit
 
 If you wish to use pre-commit, add this:
 
 ```yaml
   - repo: https://github.com/guilatrova/tryceratops
-    rev: v2.1.1
+    rev: v2.2.0
     hooks:
       - id: tryceratops
 ```
 
 ## Show your style
 
 [![try/except style: tryceratops](https://img.shields.io/badge/try%2Fexcept%20style-tryceratops%20%F0%9F%A6%96%E2%9C%A8-black)](https://github.com/guilatrova/tryceratops)
```

