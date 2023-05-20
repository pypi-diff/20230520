# Comparing `tmp/tryceratops-2.2.0.tar.gz` & `tmp/tryceratops-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tryceratops-2.2.0.tar", max compression
+gzip compressed data, was "tryceratops-2.3.0.tar", max compression
```

## Comparing `tryceratops-2.2.0.tar` & `tryceratops-2.3.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1084 2023-05-20 10:03:31.429943 tryceratops-2.2.0/LICENSE
--rw-r--r--   0        0        0     6203 2023-05-20 10:03:57.613667 tryceratops-2.2.0/README.md
--rw-r--r--   0        0        0     2243 2023-05-20 10:03:57.665665 tryceratops-2.2.0/pyproject.toml
--rw-r--r--   0        0        0       69 2023-05-20 10:03:57.613667 tryceratops-2.2.0/src/tryceratops/__init__.py
--rw-r--r--   0        0        0     2220 2023-05-20 10:03:31.433943 tryceratops-2.2.0/src/tryceratops/__main__.py
--rw-r--r--   0        0        0     1130 2023-05-20 10:03:31.433943 tryceratops-2.2.0/src/tryceratops/analyzers/__init__.py
--rw-r--r--   0        0        0     1754 2023-05-20 10:03:31.433943 tryceratops-2.2.0/src/tryceratops/analyzers/base.py
--rw-r--r--   0        0        0     5624 2023-05-20 10:03:31.433943 tryceratops-2.2.0/src/tryceratops/analyzers/call.py
--rw-r--r--   0        0        0     1584 2023-05-20 10:03:31.433943 tryceratops-2.2.0/src/tryceratops/analyzers/classdefs.py
--rw-r--r--   0        0        0     2154 2023-05-20 10:03:31.433943 tryceratops-2.2.0/src/tryceratops/analyzers/conditional.py
--rw-r--r--   0        0        0     6385 2023-05-20 10:03:31.433943 tryceratops-2.2.0/src/tryceratops/analyzers/exception_block.py
--rw-r--r--   0        0        0      350 2023-05-20 10:03:31.433943 tryceratops-2.2.0/src/tryceratops/analyzers/exceptions.py
--rw-r--r--   0        0        0     1192 2023-05-20 10:03:31.433943 tryceratops-2.2.0/src/tryceratops/analyzers/try_block.py
--rw-r--r--   0        0        0       50 2023-05-20 10:03:31.433943 tryceratops-2.2.0/src/tryceratops/files/__init__.py
--rw-r--r--   0        0        0     3618 2023-05-20 10:03:31.433943 tryceratops-2.2.0/src/tryceratops/files/discovery.py
--rw-r--r--   0        0        0     1454 2023-05-20 10:03:31.433943 tryceratops-2.2.0/src/tryceratops/files/parser.py
--rw-r--r--   0        0        0     3476 2023-05-20 10:03:31.433943 tryceratops-2.2.0/src/tryceratops/filters.py
--rw-r--r--   0        0        0      601 2023-05-20 10:03:31.433943 tryceratops-2.2.0/src/tryceratops/fixers/__init__.py
--rw-r--r--   0        0        0     2713 2023-05-20 10:03:31.433943 tryceratops-2.2.0/src/tryceratops/fixers/base.py
--rw-r--r--   0        0        0     2772 2023-05-20 10:03:31.433943 tryceratops-2.2.0/src/tryceratops/fixers/exception_block.py
--rw-r--r--   0        0        0      361 2023-05-20 10:03:31.433943 tryceratops-2.2.0/src/tryceratops/fixers/exceptions.py
--rw-r--r--   0        0        0     2129 2023-05-20 10:03:31.433943 tryceratops-2.2.0/src/tryceratops/flake_plugin.py
--rw-r--r--   0        0        0     2723 2023-05-20 10:03:31.433943 tryceratops-2.2.0/src/tryceratops/interfaces.py
--rw-r--r--   0        0        0      165 2023-05-20 10:03:31.433943 tryceratops-2.2.0/src/tryceratops/processors.py
--rw-r--r--   0        0        0     3038 2023-05-20 10:03:31.433943 tryceratops-2.2.0/src/tryceratops/runners.py
--rw-r--r--   0        0        0     1065 2023-05-20 10:03:31.433943 tryceratops-2.2.0/src/tryceratops/settings.py
--rw-r--r--   0        0        0      740 2023-05-20 10:03:31.433943 tryceratops-2.2.0/src/tryceratops/types.py
--rw-r--r--   0        0        0      108 2023-05-20 10:03:31.433943 tryceratops-2.2.0/src/tryceratops/violations/__init__.py
--rw-r--r--   0        0        0     1610 2023-05-20 10:03:31.433943 tryceratops-2.2.0/src/tryceratops/violations/codes.py
--rw-r--r--   0        0        0     1773 2023-05-20 10:03:31.433943 tryceratops-2.2.0/src/tryceratops/violations/violations.py
--rw-r--r--   0        0        0     7403 1970-01-01 00:00:00.000000 tryceratops-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-05-20 11:15:32.105742 tryceratops-2.3.0/LICENSE
+-rw-r--r--   0        0        0     6243 2023-05-20 11:16:05.812017 tryceratops-2.3.0/README.md
+-rw-r--r--   0        0        0     2243 2023-05-20 11:16:05.868020 tryceratops-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0       69 2023-05-20 11:16:05.812017 tryceratops-2.3.0/src/tryceratops/__init__.py
+-rw-r--r--   0        0        0     2227 2023-05-20 11:15:32.109743 tryceratops-2.3.0/src/tryceratops/__main__.py
+-rw-r--r--   0        0        0     1185 2023-05-20 11:15:32.109743 tryceratops-2.3.0/src/tryceratops/analyzers/__init__.py
+-rw-r--r--   0        0        0     1865 2023-05-20 11:15:32.109743 tryceratops-2.3.0/src/tryceratops/analyzers/base.py
+-rw-r--r--   0        0        0     5624 2023-05-20 11:15:32.109743 tryceratops-2.3.0/src/tryceratops/analyzers/call.py
+-rw-r--r--   0        0        0     2398 2023-05-20 11:15:32.109743 tryceratops-2.3.0/src/tryceratops/analyzers/classdefs.py
+-rw-r--r--   0        0        0     2154 2023-05-20 11:15:32.109743 tryceratops-2.3.0/src/tryceratops/analyzers/conditional.py
+-rw-r--r--   0        0        0     6385 2023-05-20 11:15:32.109743 tryceratops-2.3.0/src/tryceratops/analyzers/exception_block.py
+-rw-r--r--   0        0        0      350 2023-05-20 11:15:32.109743 tryceratops-2.3.0/src/tryceratops/analyzers/exceptions.py
+-rw-r--r--   0        0        0     1192 2023-05-20 11:15:32.109743 tryceratops-2.3.0/src/tryceratops/analyzers/try_block.py
+-rw-r--r--   0        0        0       50 2023-05-20 11:15:32.109743 tryceratops-2.3.0/src/tryceratops/files/__init__.py
+-rw-r--r--   0        0        0     3618 2023-05-20 11:15:32.109743 tryceratops-2.3.0/src/tryceratops/files/discovery.py
+-rw-r--r--   0        0        0     1455 2023-05-20 11:15:32.109743 tryceratops-2.3.0/src/tryceratops/files/parser.py
+-rw-r--r--   0        0        0      602 2023-05-20 11:15:32.109743 tryceratops-2.3.0/src/tryceratops/fixers/__init__.py
+-rw-r--r--   0        0        0     2713 2023-05-20 11:15:32.113743 tryceratops-2.3.0/src/tryceratops/fixers/base.py
+-rw-r--r--   0        0        0     2772 2023-05-20 11:15:32.113743 tryceratops-2.3.0/src/tryceratops/fixers/exception_block.py
+-rw-r--r--   0        0        0      361 2023-05-20 11:15:32.113743 tryceratops-2.3.0/src/tryceratops/fixers/exceptions.py
+-rw-r--r--   0        0        0     2130 2023-05-20 11:15:32.113743 tryceratops-2.3.0/src/tryceratops/flake_plugin.py
+-rw-r--r--   0        0        0     2729 2023-05-20 11:15:32.113743 tryceratops-2.3.0/src/tryceratops/interfaces.py
+-rw-r--r--   0        0        0     1065 2023-05-20 11:15:32.113743 tryceratops-2.3.0/src/tryceratops/logging_config.py
+-rw-r--r--   0        0        0      165 2023-05-20 11:15:32.113743 tryceratops-2.3.0/src/tryceratops/processors.py
+-rw-r--r--   0        0        0     3039 2023-05-20 11:15:32.113743 tryceratops-2.3.0/src/tryceratops/runners.py
+-rw-r--r--   0        0        0     3629 2023-05-20 11:15:32.113743 tryceratops-2.3.0/src/tryceratops/settings.py
+-rw-r--r--   0        0        0      791 2023-05-20 11:15:32.113743 tryceratops-2.3.0/src/tryceratops/types.py
+-rw-r--r--   0        0        0      108 2023-05-20 11:15:32.113743 tryceratops-2.3.0/src/tryceratops/violations/__init__.py
+-rw-r--r--   0        0        0     1745 2023-05-20 11:15:32.113743 tryceratops-2.3.0/src/tryceratops/violations/codes.py
+-rw-r--r--   0        0        0     2403 2023-05-20 11:15:32.113743 tryceratops-2.3.0/src/tryceratops/violations/violations.py
+-rw-r--r--   0        0        0     7443 1970-01-01 00:00:00.000000 tryceratops-2.3.0/PKG-INFO
```

### Comparing `tryceratops-2.2.0/LICENSE` & `tryceratops-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tryceratops-2.2.0/README.md` & `tryceratops-2.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -131,25 +131,26 @@
 
 ```toml
 [tool.tryceratops]
 exclude = ["samples"]
 ignore = ["TRY002", "TRY200", "TRY300"]
 experimental = false
 check_pickable = false
+allowed_base_exceptions = ["MyAppBase"]
 ```
 
 CLI flags always overwrite the config file.
 
 ## Pre-commit
 
 If you wish to use pre-commit, add this:
 
 ```yaml
   - repo: https://github.com/guilatrova/tryceratops
-    rev: v2.2.0
+    rev: v2.3.0
     hooks:
       - id: tryceratops
 ```
 
 ## Show your style
 
 [![try/except style: tryceratops](https://img.shields.io/badge/try%2Fexcept%20style-tryceratops%20%F0%9F%A6%96%E2%9C%A8-black)](https://github.com/guilatrova/tryceratops)
```

### Comparing `tryceratops-2.2.0/pyproject.toml` & `tryceratops-2.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tryceratops"
-version = "2.2.0"
+version = "2.3.0"
 description = "Prevent Exception Handling AntiPatterns"
 authors = ["Guilherme Latrova <hello@guilatrova.dev>"]
 license = "MIT"
 keywords = ["lint", "try", "except"]
 readme = "README.md"
 homepage = "https://github.com/guilatrova/tryceratops"
 repository = "https://github.com/guilatrova/tryceratops"
```

### Comparing `tryceratops-2.2.0/src/tryceratops/__main__.py` & `tryceratops-2.3.0/src/tryceratops/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import click
 import logging.config
 from typing import Tuple
 
 import tryceratops
 from tryceratops.files import FileDiscovery, load_config
-from tryceratops.filters import GlobalSettings
 from tryceratops.interfaces import CliInterface
+from tryceratops.logging_config import LOGGING_CONFIG
 from tryceratops.runners import Runner
-from tryceratops.settings import LOGGING_CONFIG
+from tryceratops.settings import GlobalSettings
 from tryceratops.violations import CODE_CHOICES
 
 runner = Runner()
 discovery = FileDiscovery()
 interface = CliInterface(runner, discovery)
 logger = logging.getLogger("tryceratops")
```

### Comparing `tryceratops-2.2.0/src/tryceratops/analyzers/__init__.py` & `tryceratops-2.3.0/src/tryceratops/analyzers/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,35 +2,36 @@
 
 from typing import TYPE_CHECKING, Set, Type
 
 from . import call, classdefs, conditional, exception_block, try_block
 from .base import BaseAnalyzer
 
 if TYPE_CHECKING:
-    from tryceratops.filters import GlobalSettings
+    from tryceratops.settings import GlobalSettings
 
 
 ANALYZER_CLASSES: Set[Type[BaseAnalyzer]] = {
     call.CallTooManyAnalyzer,
     call.CallRaiseVanillaAnalyzer,
     call.CallRaiseLongArgsAnalyzer,
     call.CallAvoidCheckingToContinueAnalyzer,
     conditional.PreferTypeErrorAnalyzer,
     classdefs.NonPickableAnalyzer,
+    classdefs.InheritFromBaseAnalyzer,
     exception_block.ExceptReraiseWithoutCauseAnalyzer,
     exception_block.ExceptVerboseReraiseAnalyzer,
     exception_block.ExceptBroadPassAnalyzer,
     exception_block.LogErrorAnalyzer,
     exception_block.LogObjectAnalyzer,
     exception_block.UselessTryExceptAnalyzer,
     try_block.TryConsiderElseAnalyzer,
     try_block.TryShouldntRaiseAnalyzer,
 }
 
 
 def get_analyzer_chain(global_settings: GlobalSettings) -> Set[BaseAnalyzer]:
     analyzers = {
-        analyzercls()
+        analyzercls(global_settings)
         for analyzercls in ANALYZER_CLASSES
         if global_settings.should_run_processor(analyzercls)
     }
     return analyzers
```

### Comparing `tryceratops-2.2.0/src/tryceratops/analyzers/base.py` & `tryceratops-2.3.0/src/tryceratops/analyzers/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 import ast
+import typing as t
 from abc import ABC, abstractmethod
-from typing import Any, Callable, List, Protocol, Type
 
 from tryceratops.processors import Processor
+from tryceratops.settings import GlobalSettings
 from tryceratops.violations import Violation
 
 from .exceptions import AnalyzerVisitException
 
 
 class BaseAnalyzer(ABC, Processor, ast.NodeVisitor):
-    violation_type: Type[Violation] = Violation
+    violation_type: t.Type[Violation] = Violation
 
-    def __init__(self) -> None:
-        self.violations: List[Violation] = []
+    def __init__(self, settings: t.Optional[GlobalSettings] = None) -> None:
+        self.violations: t.List[Violation] = []
+        self._settings = settings
 
-    def _mark_violation(self, *nodes: ast.AST, **kwargs: Any) -> None:  # noqa: ANN401
+    def _mark_violation(self, *nodes: ast.AST, **kwargs: t.Any) -> None:  # noqa: ANN401
         klass = self.violation_type
         for node in nodes:
             violation = klass.build(self.filename, self.violation_code, node, **kwargs)
             self.violations.append(violation)
 
-    def check(self, tree: ast.AST, filename: str) -> List[Violation]:
+    def check(self, tree: ast.AST, filename: str) -> t.List[Violation]:
         self.filename = filename
         self.violations = []
 
         self.visit(tree)
 
         return self.violations
 
 
-class StmtBodyProtocol(Protocol):
-    body: List[ast.stmt]
+class StmtBodyProtocol(t.Protocol):
+    body: t.List[ast.stmt]
 
 
-def visit_error_handler(func: Callable[[BaseAnalyzer, Any], Any]):  # noqa: ANN201
-    def _func(instance: Any, node: ast.stmt) -> None:  # noqa: ANN401
+def visit_error_handler(func: t.Callable[[BaseAnalyzer, t.Any], t.Any]):  # noqa: ANN201
+    def _func(instance: t.Any, node: ast.stmt) -> None:  # noqa: ANN401
         try:
             return func(instance, node)
         except Exception as ex:
             raise AnalyzerVisitException(node) from ex
 
     return _func
```

### Comparing `tryceratops-2.2.0/src/tryceratops/analyzers/call.py` & `tryceratops-2.3.0/src/tryceratops/analyzers/call.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.2.0/src/tryceratops/analyzers/classdefs.py` & `tryceratops-2.3.0/src/tryceratops/analyzers/classdefs.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import ast
 import typing as t
 
+from tryceratops.settings import GlobalSettings
 from tryceratops.violations import codes
+from tryceratops.violations.violations import InheritFromNonBaseViolation
 
 from .base import BaseAnalyzer, visit_error_handler
 
 
 class NonPickableAnalyzer(BaseAnalyzer):
     violation_code = codes.NON_PICKABLE_CLASS
 
@@ -40,7 +42,26 @@
         if (
             len(remaining_args) > 0
             or second_arg.annotation
             and getattr(second_arg.annotation, "id", None) != "str"
         ):
             # Pickle would break for non string args or for more than 1 arg
             self._mark_violation(node)
+
+
+class InheritFromBaseAnalyzer(BaseAnalyzer):
+    violation_code = codes.ALLOWED_BASE_EXCEPTION
+    violation_type = InheritFromNonBaseViolation
+
+    @visit_error_handler
+    def visit_ClassDef(self, node: ast.ClassDef) -> t.Any:
+        is_exc = any([base for base in node.bases if getattr(base, "id", None) == "Exception"])
+        if is_exc is False:
+            return self.generic_visit(node)
+
+        settings = t.cast(GlobalSettings, self._settings)
+        if node.name not in settings.allowed_base_exceptions:
+            self._mark_violation(
+                node,
+                class_name=node.name,
+                allowed_bases=settings.allowed_base_exceptions,
+            )
```

### Comparing `tryceratops-2.2.0/src/tryceratops/analyzers/conditional.py` & `tryceratops-2.3.0/src/tryceratops/analyzers/conditional.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.2.0/src/tryceratops/analyzers/exception_block.py` & `tryceratops-2.3.0/src/tryceratops/analyzers/exception_block.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.2.0/src/tryceratops/analyzers/try_block.py` & `tryceratops-2.3.0/src/tryceratops/analyzers/try_block.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.2.0/src/tryceratops/files/discovery.py` & `tryceratops-2.3.0/src/tryceratops/files/discovery.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.2.0/src/tryceratops/files/parser.py` & `tryceratops-2.3.0/src/tryceratops/files/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import ast
 import re
 import tokenize
 from typing import Generator, Iterable, TextIO, Tuple
 
-from tryceratops.filters import FileFilter, IgnoreViolation
+from tryceratops.settings import FileFilter, IgnoreViolation
 
 IGNORE_TRYCERATOPS_TOKEN = "noqa"
 IGNORE_TOKEN_PATT = r"noqa(: ?((TRY\d{3},? ?)+))?"
 
 
 def _build_ignore_line(match: re.Match, location: Tuple[int, int]) -> IgnoreViolation:
     lineno, _ = location
```

### Comparing `tryceratops-2.2.0/src/tryceratops/filters.py` & `tryceratops-2.3.0/src/tryceratops/settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
-from typing import TYPE_CHECKING, Iterable, Optional, Type
+from typing import TYPE_CHECKING, Iterable, Optional, Set, Type
 
 from tryceratops.processors import Processor
 from tryceratops.violations import Violation
 from tryceratops.violations.codes import NON_PICKABLE_CLASS
 
 if TYPE_CHECKING:
     from tryceratops.types import PyprojectConfig
@@ -51,14 +51,16 @@
     Represents a filter applied to the runner
     (i.e. which processes to run, and what files to ignore).
     """
 
     include_experimental: bool
     ignore_violations: Iterable[str]
     exclude_dirs: Iterable[str]
+    allowed_base_exceptions: Set[str]
+
     check_pickable: bool = False
     autofix: bool = False
 
     def _self_check(self) -> None:
         self.exclude_dirs = [excluded for excluded in self.exclude_dirs if excluded]
 
     def __post_init__(self) -> None:
@@ -90,16 +92,17 @@
     @classmethod
     def create_from_config(cls, config: PyprojectConfig) -> GlobalSettings:
         experimental = config.get("experimental", False)
         ignore = config.get("ignore", [])
         exclude = config.get("exclude", [])
         autofix = config.get("autofix", False)
         check_pickable = config.get("check_pickable", False)
+        allowed_base_exceptions = set(config.get("allowed_base_exceptions", set()))
 
-        return cls(experimental, ignore, exclude, check_pickable, autofix)
+        return cls(experimental, ignore, exclude, allowed_base_exceptions, check_pickable, autofix)
 
     def overwrite_from_cli(
         self,
         include_experimental: bool,
         ignore_violations: Iterable[str],
         exclude_dirs: Iterable[str],
         autofix: bool,
```

### Comparing `tryceratops-2.2.0/src/tryceratops/fixers/__init__.py` & `tryceratops-2.3.0/src/tryceratops/fixers/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from typing import TYPE_CHECKING, Set, Type
 
 from .base import BaseFixer
 from .exception_block import LoggerErrorFixer, RaiseWithoutCauseFixer, VerboseReraiseFixer
 
 if TYPE_CHECKING:
-    from tryceratops.filters import GlobalSettings
+    from tryceratops.settings import GlobalSettings
 
 FIXER_CLASSES: Set[Type[BaseFixer]] = {
     RaiseWithoutCauseFixer,
     VerboseReraiseFixer,
     LoggerErrorFixer,
 }
```

### Comparing `tryceratops-2.2.0/src/tryceratops/fixers/base.py` & `tryceratops-2.3.0/src/tryceratops/fixers/base.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.2.0/src/tryceratops/fixers/exception_block.py` & `tryceratops-2.3.0/src/tryceratops/fixers/exception_block.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.2.0/src/tryceratops/flake_plugin.py` & `tryceratops-2.3.0/src/tryceratops/flake_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import ast
 import importlib.metadata
 from tokenize import TokenInfo
 from typing import Any, Generator, Iterable, List, Tuple, Type
 
 from tryceratops.files.discovery import load_config
 from tryceratops.files.parser import parse_ignore_tokens
-from tryceratops.filters import FileFilter, GlobalSettings
 from tryceratops.runners import Runner
+from tryceratops.settings import FileFilter, GlobalSettings
 from tryceratops.violations.violations import Violation
 
 PACKAGE_NAME = "tryceratops"
 GLOBAL_DUMMY_FILTER = GlobalSettings(
     include_experimental=False, ignore_violations=[], exclude_dirs=[], autofix=False
 )
 FLAKE8_VIOLATION_TYPE = Tuple[int, int, str, Type[Any]]
```

### Comparing `tryceratops-2.2.0/src/tryceratops/interfaces.py` & `tryceratops-2.3.0/src/tryceratops/interfaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import os
 import sys
 from enum import IntEnum
 
 from rich import print
 
 from tryceratops.files.discovery import FileDiscovery
+from tryceratops.logging_config import ERROR_LOG_FILENAME
 from tryceratops.runners import Runner
-from tryceratops.settings import ERROR_LOG_FILENAME
 from tryceratops.violations import Violation
 
 
 class ExitCodes(IntEnum):
     SUCCESS = 0
     LINT_BROKEN = 1
     UNPROCESSED_FILE = 2
```

### Comparing `tryceratops-2.2.0/src/tryceratops/runners.py` & `tryceratops-2.3.0/src/tryceratops/runners.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import ast
 import logging
 from dataclasses import dataclass
 from typing import List, Set, Type
 
 from tryceratops.analyzers import BaseAnalyzer, get_analyzer_chain
-from tryceratops.filters import FileFilter, GlobalSettings
 from tryceratops.fixers import BaseFixer, get_fixers_chain
 from tryceratops.processors import Processor
+from tryceratops.settings import FileFilter, GlobalSettings
 from tryceratops.types import ParsedFilesType
 from tryceratops.violations import Violation
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
```

### Comparing `tryceratops-2.2.0/src/tryceratops/settings.py` & `tryceratops-2.3.0/src/tryceratops/logging_config.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.2.0/src/tryceratops/types.py` & `tryceratops-2.3.0/src/tryceratops/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import ast
 import typing as t
 import typing_extensions as te
 
-from tryceratops.filters import FileFilter
+from tryceratops.settings import FileFilter
 
 ParsedFileType = t.Tuple[str, ast.AST, FileFilter]
 ParsedFilesType = t.Collection[ParsedFileType]
 
 
 class PyprojectConfig(t.TypedDict):
     """
@@ -17,7 +17,8 @@
     """
 
     exclude: te.NotRequired[t.List[str]]
     ignore: te.NotRequired[t.List[str]]
     experimental: te.NotRequired[bool]
     autofix: te.NotRequired[bool]
     check_pickable: te.NotRequired[bool]
+    allowed_base_exceptions: te.NotRequired[bool]
```

### Comparing `tryceratops-2.2.0/src/tryceratops/violations/codes.py` & `tryceratops-2.3.0/src/tryceratops/violations/codes.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 RAISE_VANILLA_CLASS = ("TRY002", "Create your own exception")
 RAISE_VANILLA_ARGS = (
     "TRY003",
     "Avoid specifying long messages outside the exception class",
 )
 PREFER_TYPE_ERROR = ("TRY004", "Prefer TypeError exception for invalid type")
 NON_PICKABLE_CLASS = ("TRY005", "Define __reduce__ to make exception pickable")
+ALLOWED_BASE_EXCEPTION = (
+    "TRY006",
+    "Class '{}' should inherit from any of your defined base exceptions: {}",
+)
 
 # TRY1xx - General
 CHECK_TO_CONTINUE = (
     "TRY100",
     "Don't check to continue, make callable '{}' raise a exception instead",
 )
 TOO_MANY_TRY = ("TRY101", "Too many try blocks in your function")
@@ -33,14 +37,15 @@
 
 CODE_CHOICES = {
     # TRY0xx - Exceptions
     "TRY002",
     "TRY003",
     "TRY004",
     "TRY005",
+    "TRY006",
     # TRY1xx - General
     "TRY100",
     "TRY101",
     # TRY2xx - Except
     "TRY200",
     "TRY201",
     "TRY202",
```

### Comparing `tryceratops-2.2.0/src/tryceratops/violations/violations.py` & `tryceratops-2.3.0/src/tryceratops/violations/violations.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import ast
 from dataclasses import dataclass
-from typing import Any, Optional, Tuple
+from typing import Any, Optional, Set, Tuple
 
 
 @dataclass
 class Violation:
     code: str
     line: int
     col: int
@@ -64,7 +64,28 @@
         if except_node is None:
             raise ValueError("except_node")
 
         code, msg = vio_details
         return cls(
             code, node.lineno, node.col_offset, msg, filename, node, except_node, exception_name
         )
+
+
+@dataclass
+class InheritFromNonBaseViolation(Violation):
+    @classmethod
+    def build(
+        cls,
+        filename: str,
+        vio_details: Tuple[str, str],
+        node: ast.AST,
+        class_name: Optional[str] = None,
+        allowed_bases: Optional[Set[str]] = None,
+        *args: Any,  # noqa: ANN401
+        **kwargs: Any,  # noqa: ANN401
+    ) -> InheritFromNonBaseViolation:
+        code, msg_base = vio_details
+
+        allowed_msg = ", ".join(allowed_bases or set())
+        msg = msg_base.format(class_name or "", allowed_msg)
+
+        return cls(code, node.lineno, node.col_offset, msg, filename, node)
```

### Comparing `tryceratops-2.2.0/PKG-INFO` & `tryceratops-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tryceratops
-Version: 2.2.0
+Version: 2.3.0
 Summary: Prevent Exception Handling AntiPatterns
 Home-page: https://github.com/guilatrova/tryceratops
 License: MIT
 Keywords: lint,try,except
 Author: Guilherme Latrova
 Author-email: hello@guilatrova.dev
 Requires-Python: >=3.8.1,<4.0
@@ -160,25 +160,26 @@
 
 ```toml
 [tool.tryceratops]
 exclude = ["samples"]
 ignore = ["TRY002", "TRY200", "TRY300"]
 experimental = false
 check_pickable = false
+allowed_base_exceptions = ["MyAppBase"]
 ```
 
 CLI flags always overwrite the config file.
 
 ## Pre-commit
 
 If you wish to use pre-commit, add this:
 
 ```yaml
   - repo: https://github.com/guilatrova/tryceratops
-    rev: v2.2.0
+    rev: v2.3.0
     hooks:
       - id: tryceratops
 ```
 
 ## Show your style
 
 [![try/except style: tryceratops](https://img.shields.io/badge/try%2Fexcept%20style-tryceratops%20%F0%9F%A6%96%E2%9C%A8-black)](https://github.com/guilatrova/tryceratops)
```

