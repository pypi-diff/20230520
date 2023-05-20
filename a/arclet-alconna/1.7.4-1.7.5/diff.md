# Comparing `tmp/arclet-alconna-1.7.4.tar.gz` & `tmp/arclet-alconna-1.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arclet-alconna-1.7.4.tar", last modified: Thu May 18 17:46:58 2023, max compression
+gzip compressed data, was "arclet-alconna-1.7.5.tar", last modified: Sat May 20 10:54:11 2023, max compression
```

## Comparing `arclet-alconna-1.7.4.tar` & `arclet-alconna-1.7.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524011 arclet-alconna-1.7.4/LICENSE
--rw-r--r--   0        0        0     2810 2023-05-11 05:55:21.918053 arclet-alconna-1.7.4/pyproject.toml
--rw-r--r--   0        0        0     6702 2023-05-11 05:55:23.383958 arclet-alconna-1.7.4/README-EN.md
--rw-r--r--   0        0        0     1084 2023-05-18 17:46:33.704373 arclet-alconna-1.7.4/src/arclet/alconna/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 05:53:44.746150 arclet-alconna-1.7.4/src/arclet/alconna/_internal/__init__.py
--rw-r--r--   0        0        0    17863 2023-05-18 17:26:34.573035 arclet-alconna-1.7.4/src/arclet/alconna/_internal/_analyser.py
--rw-r--r--   0        0        0     8476 2023-05-11 05:53:44.748144 arclet-alconna-1.7.4/src/arclet/alconna/_internal/_argv.py
--rw-r--r--   0        0        0    23162 2023-05-18 17:44:42.865275 arclet-alconna-1.7.4/src/arclet/alconna/_internal/_handlers.py
--rw-r--r--   0        0        0     7811 2023-05-11 05:53:44.749146 arclet-alconna-1.7.4/src/arclet/alconna/_internal/_header.py
--rw-r--r--   0        0        0      837 2023-05-11 05:53:44.749146 arclet-alconna-1.7.4/src/arclet/alconna/_internal/_util.py
--rw-r--r--   0        0        0     1543 2023-05-11 05:54:34.441719 arclet-alconna-1.7.4/src/arclet/alconna/action.py
--rw-r--r--   0        0        0    14429 2023-05-11 05:55:00.317381 arclet-alconna-1.7.4/src/arclet/alconna/args.py
--rw-r--r--   0        0        0     1499 2023-05-11 05:53:44.752371 arclet-alconna-1.7.4/src/arclet/alconna/argv.py
--rw-r--r--   0        0        0    15660 2023-05-11 05:55:01.638197 arclet-alconna-1.7.4/src/arclet/alconna/arparma.py
--rw-r--r--   0        0        0    13248 2023-05-11 05:55:02.886909 arclet-alconna-1.7.4/src/arclet/alconna/base.py
--rw-r--r--   0        0        0     1889 2023-05-11 05:55:04.954858 arclet-alconna-1.7.4/src/arclet/alconna/builtin.py
--rw-r--r--   0        0        0     4867 2023-05-11 05:53:44.757144 arclet-alconna-1.7.4/src/arclet/alconna/completion.py
--rw-r--r--   0        0        0     4465 2023-05-11 05:55:07.597153 arclet-alconna-1.7.4/src/arclet/alconna/config.py
--rw-r--r--   0        0        0    14029 2023-05-12 11:11:57.973132 arclet-alconna-1.7.4/src/arclet/alconna/core.py
--rw-r--r--   0        0        0     2617 2023-05-11 05:55:14.716787 arclet-alconna-1.7.4/src/arclet/alconna/duplication.py
--rw-r--r--   0        0        0     1009 2023-05-11 05:55:16.833416 arclet-alconna-1.7.4/src/arclet/alconna/exceptions.py
--rw-r--r--   0        0        0    11287 2023-05-11 05:55:17.442184 arclet-alconna-1.7.4/src/arclet/alconna/formatter.py
--rw-r--r--   0        0        0       99 2023-05-11 05:53:44.763145 arclet-alconna-1.7.4/src/arclet/alconna/i18n/.config.json
--rw-r--r--   0        0        0     3565 2023-05-11 05:53:44.764143 arclet-alconna-1.7.4/src/arclet/alconna/i18n/en-US.json
--rw-r--r--   0        0        0     3602 2023-05-11 05:53:44.764143 arclet-alconna-1.7.4/src/arclet/alconna/i18n/zh-CN.json
--rw-r--r--   0        0        0    16956 2023-05-11 05:55:18.044404 arclet-alconna-1.7.4/src/arclet/alconna/manager.py
--rw-r--r--   0        0        0     1484 2023-05-11 05:55:18.667097 arclet-alconna-1.7.4/src/arclet/alconna/model.py
--rw-r--r--   0        0        0     1943 2023-05-11 05:55:19.651541 arclet-alconna-1.7.4/src/arclet/alconna/model.pyi
--rw-r--r--   0        0        0     3940 2023-05-11 05:55:20.308191 arclet-alconna-1.7.4/src/arclet/alconna/output.py
--rw-r--r--   0        0        0        0 2023-05-11 05:53:44.769149 arclet-alconna-1.7.4/src/arclet/alconna/py.typed
--rw-r--r--   0        0        0     5815 2023-05-11 05:55:25.933152 arclet-alconna-1.7.4/src/arclet/alconna/stub.py
--rw-r--r--   0        0        0     3586 2023-05-11 05:55:26.563876 arclet-alconna-1.7.4/src/arclet/alconna/typing.py
--rw-r--r--   0        0        0     3246 2023-05-11 05:53:44.772143 arclet-alconna-1.7.4/tests/analyser_test.py
--rw-r--r--   0        0        0     7583 2023-05-11 05:53:44.773143 arclet-alconna-1.7.4/tests/args_test.py
--rw-r--r--   0        0        0     2167 2023-05-11 05:55:03.459296 arclet-alconna-1.7.4/tests/base_test.py
--rw-r--r--   0        0        0     3113 2023-05-11 05:53:44.774144 arclet-alconna-1.7.4/tests/components_test.py
--rw-r--r--   0        0        0     1199 2023-05-11 05:53:44.774144 arclet-alconna-1.7.4/tests/config_test.py
--rw-r--r--   0        0        0    23995 2023-05-18 17:37:11.008952 arclet-alconna-1.7.4/tests/core_test.py
--rw-r--r--   0        0        0      505 2023-05-11 05:53:44.775105 arclet-alconna-1.7.4/tests/util_test.py
--rw-r--r--   0        0        0     7363 1970-01-01 00:00:00.000000 arclet-alconna-1.7.4/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524011 arclet-alconna-1.7.5/LICENSE
+-rw-r--r--   0        0        0     2810 2023-05-11 05:55:21.918053 arclet-alconna-1.7.5/pyproject.toml
+-rw-r--r--   0        0        0     6702 2023-05-11 05:55:23.383958 arclet-alconna-1.7.5/README-EN.md
+-rw-r--r--   0        0        0     1084 2023-05-19 14:58:51.597031 arclet-alconna-1.7.5/src/arclet/alconna/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 05:53:44.746150 arclet-alconna-1.7.5/src/arclet/alconna/_internal/__init__.py
+-rw-r--r--   0        0        0    17863 2023-05-19 14:58:51.598030 arclet-alconna-1.7.5/src/arclet/alconna/_internal/_analyser.py
+-rw-r--r--   0        0        0     8476 2023-05-11 05:53:44.748144 arclet-alconna-1.7.5/src/arclet/alconna/_internal/_argv.py
+-rw-r--r--   0        0        0    23361 2023-05-19 14:58:51.599030 arclet-alconna-1.7.5/src/arclet/alconna/_internal/_handlers.py
+-rw-r--r--   0        0        0     9971 2023-05-19 14:58:51.600030 arclet-alconna-1.7.5/src/arclet/alconna/_internal/_header.py
+-rw-r--r--   0        0        0      837 2023-05-11 05:53:44.749146 arclet-alconna-1.7.5/src/arclet/alconna/_internal/_util.py
+-rw-r--r--   0        0        0     1543 2023-05-11 05:54:34.441719 arclet-alconna-1.7.5/src/arclet/alconna/action.py
+-rw-r--r--   0        0        0    14429 2023-05-11 05:55:00.317381 arclet-alconna-1.7.5/src/arclet/alconna/args.py
+-rw-r--r--   0        0        0     1499 2023-05-11 05:53:44.752371 arclet-alconna-1.7.5/src/arclet/alconna/argv.py
+-rw-r--r--   0        0        0    15660 2023-05-11 05:55:01.638197 arclet-alconna-1.7.5/src/arclet/alconna/arparma.py
+-rw-r--r--   0        0        0    13248 2023-05-11 05:55:02.886909 arclet-alconna-1.7.5/src/arclet/alconna/base.py
+-rw-r--r--   0        0        0     1889 2023-05-11 05:55:04.954858 arclet-alconna-1.7.5/src/arclet/alconna/builtin.py
+-rw-r--r--   0        0        0     4867 2023-05-11 05:53:44.757144 arclet-alconna-1.7.5/src/arclet/alconna/completion.py
+-rw-r--r--   0        0        0     4465 2023-05-11 05:55:07.597153 arclet-alconna-1.7.5/src/arclet/alconna/config.py
+-rw-r--r--   0        0        0    14061 2023-05-19 14:58:51.601035 arclet-alconna-1.7.5/src/arclet/alconna/core.py
+-rw-r--r--   0        0        0     2617 2023-05-11 05:55:14.716787 arclet-alconna-1.7.5/src/arclet/alconna/duplication.py
+-rw-r--r--   0        0        0     1009 2023-05-11 05:55:16.833416 arclet-alconna-1.7.5/src/arclet/alconna/exceptions.py
+-rw-r--r--   0        0        0    11287 2023-05-11 05:55:17.442184 arclet-alconna-1.7.5/src/arclet/alconna/formatter.py
+-rw-r--r--   0        0        0       99 2023-05-11 05:53:44.763145 arclet-alconna-1.7.5/src/arclet/alconna/i18n/.config.json
+-rw-r--r--   0        0        0     3638 2023-05-19 14:58:51.602031 arclet-alconna-1.7.5/src/arclet/alconna/i18n/en-US.json
+-rw-r--r--   0        0        0     3687 2023-05-19 14:58:51.603034 arclet-alconna-1.7.5/src/arclet/alconna/i18n/zh-CN.json
+-rw-r--r--   0        0        0    16956 2023-05-11 05:55:18.044404 arclet-alconna-1.7.5/src/arclet/alconna/manager.py
+-rw-r--r--   0        0        0     1484 2023-05-11 05:55:18.667097 arclet-alconna-1.7.5/src/arclet/alconna/model.py
+-rw-r--r--   0        0        0     1943 2023-05-11 05:55:19.651541 arclet-alconna-1.7.5/src/arclet/alconna/model.pyi
+-rw-r--r--   0        0        0     3940 2023-05-11 05:55:20.308191 arclet-alconna-1.7.5/src/arclet/alconna/output.py
+-rw-r--r--   0        0        0        0 2023-05-11 05:53:44.769149 arclet-alconna-1.7.5/src/arclet/alconna/py.typed
+-rw-r--r--   0        0        0     5815 2023-05-11 05:55:25.933152 arclet-alconna-1.7.5/src/arclet/alconna/stub.py
+-rw-r--r--   0        0        0     3586 2023-05-11 05:55:26.563876 arclet-alconna-1.7.5/src/arclet/alconna/typing.py
+-rw-r--r--   0        0        0     3246 2023-05-11 05:53:44.772143 arclet-alconna-1.7.5/tests/analyser_test.py
+-rw-r--r--   0        0        0     7583 2023-05-11 05:53:44.773143 arclet-alconna-1.7.5/tests/args_test.py
+-rw-r--r--   0        0        0     2167 2023-05-11 05:55:03.459296 arclet-alconna-1.7.5/tests/base_test.py
+-rw-r--r--   0        0        0     3113 2023-05-11 05:53:44.774144 arclet-alconna-1.7.5/tests/components_test.py
+-rw-r--r--   0        0        0     1199 2023-05-11 05:53:44.774144 arclet-alconna-1.7.5/tests/config_test.py
+-rw-r--r--   0        0        0    23995 2023-05-19 14:58:51.604030 arclet-alconna-1.7.5/tests/core_test.py
+-rw-r--r--   0        0        0      505 2023-05-11 05:53:44.775105 arclet-alconna-1.7.5/tests/util_test.py
+-rw-r--r--   0        0        0     7363 1970-01-01 00:00:00.000000 arclet-alconna-1.7.5/PKG-INFO
```

### Comparing `arclet-alconna-1.7.4/LICENSE` & `arclet-alconna-1.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.4/pyproject.toml` & `arclet-alconna-1.7.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
 ]
-version = "1.7.4"
+version = "1.7.5"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 documentation = "https://arcletproject.github.io/docs/alconna/tutorial"
 repository = "https://github.com/ArcletProject/Alconna"
```

### Comparing `arclet-alconna-1.7.4/README-EN.md` & `arclet-alconna-1.7.5/README-EN.md`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.4/src/arclet/alconna/__init__.py` & `arclet-alconna-1.7.5/src/arclet/alconna/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,12 +17,12 @@
 from .builtin import set_default
 from .model import OptionResult, SubcommandResult, HeadResult
 from .output import output_manager
 from .formatter import TextFormatter
 from .duplication import Duplication
 from .stub import ArgsStub, OptionStub, SubcommandStub
 
-__version__ = "1.7.4"
+__version__ = "1.7.5"
 
 # backward compatibility
 Arpamar = Arparma
 DataCollectionContainer = Argv
```

### Comparing `arclet-alconna-1.7.4/src/arclet/alconna/_internal/_analyser.py` & `arclet-alconna-1.7.5/src/arclet/alconna/_internal/_analyser.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.4/src/arclet/alconna/_internal/_argv.py` & `arclet-alconna-1.7.5/src/arclet/alconna/_internal/_argv.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.4/src/arclet/alconna/_internal/_handlers.py` & `arclet-alconna-1.7.5/src/arclet/alconna/_internal/_handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -453,24 +453,26 @@
 
     Returns:
         HeadResult: 分析结果
     """
     content = header.content
     mapping = header.mapping
     head_text, _str = argv.next()
-    if content.__class__ is TPattern and _str:
-        if mat := content.fullmatch(head_text):
+    if _str:
+        if content.__class__ is set and head_text in content:
+            return HeadResult(head_text, head_text, True, fixes=mapping)
+        elif content.__class__ is TPattern and (mat := content.fullmatch(head_text)):
             return HeadResult(head_text, head_text, True, mat.groupdict(), mapping)
-        if header.compact and (mat := content.match(head_text)):
+        if header.compact and content.__class__ in (set, TPattern) and (mat := header.compact_pattern.match(head_text)):
             argv.rollback(head_text[len(mat[0]):], replace=True)
             return HeadResult(mat[0], mat[0], True, mat.groupdict(), mapping)
-    elif isinstance(content, BasePattern):
+    if isinstance(content, BasePattern):
         if (val := content.exec(head_text, Empty)).success:
             return HeadResult(head_text, val.value, True, fixes=mapping)
-        if header.compact and (val := content.prefixed().exec(head_text, Empty)).success:
+        if header.compact and (val := header.compact_pattern.exec(head_text, Empty)).success:
             if _str:
                 argv.rollback(head_text[len(str(val.value)):], replace=True)
             return HeadResult(val.value, val.value, True, fixes=mapping)
 
     may_cmd, _m_str = argv.next()
     if content.__class__ is list and _m_str:
         for pair in content:
```

### Comparing `arclet-alconna-1.7.4/src/arclet/alconna/_internal/_header.py` & `arclet-alconna-1.7.5/src/arclet/alconna/_internal/_header.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,25 +3,24 @@
 import re
 from copy import deepcopy
 from inspect import isclass
 from typing import Any, Callable
 
 from nepattern import BasePattern, UnionPattern, all_patterns, type_parser
 from nepattern.util import TPattern
-from tarina import Empty
+from tarina import Empty, lang
 
 from ..typing import TPrefixes
 
 
-def handle_bracket(name: str):
+def handle_bracket(name: str, mapping: dict):
     """处理字符串中的括号对并转为正则表达式"""
     pattern_map = all_patterns()
-    mapping = {}
     if len(parts := re.split(r"(\{.*?})", name)) <= 1:
-        return name, mapping
+        return name, False
     for i, part in enumerate(parts):
         if not part:
             continue
         if part.startswith("{") and part.endswith("}"):
             res = part[1:-1].split(":")
             if not res or (len(res) > 1 and not res[1] and not res[0]):
                 parts[i] = ".+?"
@@ -32,160 +31,201 @@
                     i
                 ] = f"{pattern_map[res[1]].pattern if res[1] in pattern_map else res[1]}"
             elif res[1] in pattern_map:
                 mapping[res[0]] = pattern_map[res[1]]
                 parts[i] = f"(?P<{res[0]}>{pattern_map[res[1]].pattern})"
             else:
                 parts[i] = f"(?P<{res[0]}>{res[1]})"
-    return "".join(parts), mapping
+    return "".join(parts), True
 
 
 class Pair:
     """用于匹配前缀和命令的配对"""
-    __slots__ = ("prefix", "pattern", "is_prefix_pat")
+    __slots__ = ("prefix", "pattern", "is_prefix_pat", "gd_supplier", "_match")
 
-    def __init__(self, prefix: Any, pattern: TPattern):
+    def __init__(self, prefix: Any, pattern: TPattern | str):
         self.prefix = prefix
         self.pattern = pattern
         self.is_prefix_pat = isinstance(self.prefix, BasePattern)
+        if isinstance(self.pattern, str):
+            self.gd_supplier = lambda mat: None
 
-    def match(self, prefix: Any, command: str, pbfn: Callable[..., ...], comp: bool):
-        if not (mat := self.pattern.fullmatch(command)):
-            if comp and (mat := self.pattern.match(command)):
-                pbfn(command[len(mat[0]):], replace=True)
-                command = mat[0]
-            else:
-                return
-        if self.is_prefix_pat and (val := self.prefix.exec(prefix, Empty)).success:
-            return (prefix, command), (val.value, command), True, mat.groupdict()
-        if not isclass(prefix) and prefix == self.prefix or prefix.__class__ == self.prefix:
-            return (prefix, command), (prefix, command), True, mat.groupdict()
+            def _match(command: str, pbfn: Callable[..., ...], comp: bool):
+                if command == self.pattern:
+                    return command, None
+                if comp and command.startswith(self.pattern):
+                    pbfn(command[len(self.pattern):], replace=True)
+                    return self.pattern, None
+                return None, None
+
+        else:
+            self.gd_supplier = lambda mat: mat.groupdict()
+
+            def _match(command: str, pbfn: Callable[..., ...], comp: bool):
+                if mat := self.pattern.fullmatch(command):
+                    return command, mat
+                if comp and (mat := self.pattern.match(command)):
+                    pbfn(command[len(mat[0]):], replace=True)
+                    return mat[0], mat
+                return None, None
+        self._match = _match
+
+    def match(self, _pf: Any, command: str, pbfn: Callable[..., ...], comp: bool):
+        cmd, mat = self._match(command, pbfn, comp)
+        if cmd is None:
+            return
+        if self.is_prefix_pat and (val := self.prefix.exec(_pf, Empty)).success:
+            return (_pf, command), (val.value, command), True, self.gd_supplier(mat)
+        if not isclass(_pf) and _pf == self.prefix or _pf.__class__ == self.prefix:
+            return (_pf, command), (_pf, command), True, self.gd_supplier(mat)
 
 
 class Double:
     """用于匹配前缀和命令的组合"""
-    __slots__ = ("elements", "patterns", "prefix", "command")
+    command: TPattern | BasePattern | str
 
-    def __init__(self, es: list, pats: UnionPattern | None, prefix: TPattern | None, command: BasePattern | TPattern):
-        self.elements = es
-        self.patterns = pats
-        self.prefix = prefix
-        self.command = command
+    def __init__(
+        self,
+        prefixes: TPrefixes,
+        command: str | BasePattern,
+    ):
+        patterns = []
+        texts = []
+        for h in prefixes:
+            if isinstance(h, str):
+                texts.append(h)
+            elif isinstance(h, BasePattern):
+                patterns.append(h)
+            else:
+                patterns.append(type_parser(h))
+        self.patterns = UnionPattern(patterns)
+        if isinstance(command, BasePattern):
+            self.command = command
+            self.prefix = set(texts) if texts else None
+            self.comp_pattern = command.prefixed()
+            self.cmd_type = 0
+        elif not texts:
+            self.prefix = None
+            self.command = re.compile(command)
+            self.comp_pattern = re.compile(f"^{command}")
+            self.cmd_type = 1
+        else:
+            prf = "|".join(re.escape(h) for h in texts)
+            self.prefix = re.compile(f"(?:{prf}){command}")
+            self.command = re.compile(command)
+            self.cmd_type = 2
+            self.comp_pattern = re.compile(f"^(?:{prf}){command}")
+
+    def match0(self, pf: Any, cmd: Any, p_str: bool, c_str: bool, pbfn: Callable[..., ...], comp: bool):
+        if self.prefix and p_str and pf in self.prefix:
+            if (val := self.command.exec(cmd, Empty)).success:
+                return (pf, cmd), (pf, val.value), True, None
+            if comp and (val := self.comp_pattern.exec(cmd, Empty)).success:
+                if c_str:
+                    pbfn(cmd[len(str(val.value)):], replace=True)
+                return (pf, cmd), (pf, cmd[:len(str(val.value))]), True, None
+            return
+        if (val := self.patterns.exec(pf, Empty)).success:
+            if (val2 := self.command.exec(cmd, Empty)).success:
+                return (pf, cmd), (val.value, val2.value), True, None
+            if comp and (val2 := self.comp_pattern.exec(cmd, Empty)).success:
+                if c_str:
+                    pbfn(cmd[len(str(val2.value)):], replace=True)
+                return (pf, cmd), (val.value, cmd[:len(str(val2.value))]), True, None
+            return
+
+    def match1(self, pf: Any, cmd: Any, p_str: bool, c_str: bool, pbfn: Callable[..., ...], comp: bool):
+        if p_str or not c_str:
+            return
+        if (val := self.patterns.exec(pf, Empty)).success and (mat := self.command.fullmatch(cmd)):
+            return (pf, cmd), (val.value, cmd), True, mat.groupdict()
+        if comp and (mat := self.comp_pattern.match(cmd)):
+            pbfn(cmd[len(mat[0]):], replace=True)
+            return (pf, cmd), (pf, mat[0]), True, mat.groupdict()
 
     def match(self, pf: Any, cmd: Any, p_str: bool, c_str: bool, pbfn: Callable[..., ...], comp: bool):
-        if self.prefix and p_str:
-            if c_str:
-                pat = re.compile(self.prefix.pattern + self.command.pattern)
-                if mat := pat.fullmatch(pf):
-                    pbfn(cmd)
-                    return pf, pf, True, mat.groupdict()
-                elif mat := pat.fullmatch(name := (pf + cmd)):
-                    return name, name, True, mat.groupdict()
-                elif comp and (mat := pat.match(pf)):
-                    pbfn(cmd)
-                    pbfn(pf[len(mat[0]):], replace=True)
-                    return mat[0], mat[0], True, mat.groupdict()
-                elif comp and (mat := pat.match(name)):
-                    pbfn(name[len(mat[0]):], replace=True)
-                    return mat[0], mat[0], True, mat.groupdict()
-            if (mat := self.prefix.fullmatch(pf)) and (_val := self.command.exec(cmd, Empty)).success:
-                return (pf, cmd), (pf, _val.value), True, mat.groupdict()
-            elif comp and (mat := self.prefix.fullmatch(pf)) and (
-                _val := self.command.prefixed().exec(cmd, Empty)
-            ).success:
-                if c_str:
-                    pbfn(cmd[len(str(_val.value)):], replace=True)
-                return (pf, _val.value), (pf, _val.value), True, mat.groupdict()
-        if self.patterns and (val := self.patterns.validate(pf, Empty)).success:
-            _po, _pr = pf, val.value
-        elif (
-            self.elements
-            and not isclass(pf)
-            and (pf in self.elements or type(pf) in self.elements)
-        ):
-            _po, _pr = pf, pf
-        else:
+        if not self.cmd_type:
+            return self.match0(pf, cmd, p_str, c_str, pbfn, comp)
+        if self.cmd_type == 1:
+            return self.match1(pf, cmd, p_str, c_str, pbfn, comp)
+        if not p_str and not c_str:
+            return
+        if p_str:
+            if mat := self.prefix.fullmatch(pf):
+                pbfn(cmd)
+                return pf, pf, True, mat.groupdict()
+            if comp and (mat := self.comp_pattern.match(pf)):
+                pbfn(cmd)
+                pbfn(pf[len(mat[0]):], replace=True)
+                return mat[0], mat[0], True, mat.groupdict()
+            if not c_str:
+                return
+            if mat := self.prefix.fullmatch((name := pf + cmd)):
+                return name, name, True, mat.groupdict()
+            if comp and (mat := self.comp_pattern.match(name)):
+                pbfn(name[len(mat[0]):], replace=True)
+                return mat[0], mat[0], True, mat.groupdict()
             return
-        if self.command.__class__ is TPattern and c_str:
+        if (val := self.patterns.exec(pf, Empty)).success:
             if mat := self.command.fullmatch(cmd):
-                return (_po, cmd), (_pr, cmd), True, mat.groupdict()
+                return (pf, cmd), (val.value, cmd), True, mat.groupdict()
             if comp and (mat := self.command.match(cmd)):
                 pbfn(cmd[len(mat[0]):], replace=True)
-                return (_po, mat[0]), (_pr, mat[0]), True, mat.groupdict()
-        elif isinstance(self.command, BasePattern):
-            if (_val := self.command.exec(cmd, Empty)).success:
-                return (_po, cmd), (_pr, _val.value), True
-            if comp and (val := self.command.prefixed().exec(cmd, Empty)).success:
-                if c_str:
-                    pbfn(cmd[len(str(val.value)):], replace=True)
-                return (_po, _val.value), (_pr, _val.value), True
+                return (pf, cmd), (val.value, mat[0]), True, mat.groupdict()
 
 
 class Header:
     """命令头部的匹配表达式"""
-    __slots__ = ("origin", "content", "mapping", "compact")
+    __slots__ = ("origin", "content", "mapping", "compact", "compact_pattern")
 
     def __init__(
         self,
         origin: tuple[str | type | BasePattern, TPrefixes],
-        content: TPattern | BasePattern | list[Pair] | Double,
+        content: set[str] | TPattern | BasePattern | list[Pair] | Double,
         mapping: dict[str, BasePattern] | None = None,
-        compact: bool = False
+        compact: bool = False,
+        compact_pattern: TPattern | BasePattern | None = None,
     ):
         self.origin = origin
         self.content = content
         self.mapping = mapping or {}
         self.compact = compact
+        self.compact_pattern = compact_pattern
 
     @classmethod
     def generate(
         cls,
         command: str | type | BasePattern,
         prefixes: TPrefixes,
         compact: bool,
     ):
-        mapping = {}
         if isinstance(command, str):
-            command, mapping = handle_bracket(command)
-        _cmd_name: TPattern | BasePattern
-        _cmd_str: str
-        _cmd_name, _cmd_str = (
-            (re.compile(command), command)
-            if isinstance(command, str)
-            else (deepcopy(type_parser(command)), str(command))
-        )
-        if not prefixes:
-            return cls((command, prefixes), _cmd_name, mapping, compact)
-        if isinstance(prefixes[0], tuple):
-            return cls(
-                (command, prefixes),
-                [Pair(h[0], re.compile(re.escape(h[1]) + _cmd_str)) for h in prefixes],
-                mapping,
-                compact
-            )
-        elements = []
-        patterns = []
-        ch_text = ""
-        for h in prefixes:
-            if isinstance(h, str):
-                ch_text += f"{re.escape(h)}|"
-            elif isinstance(h, BasePattern):
-                patterns.append(h)
+            mapping = {}
+            if command.startswith("re:"):
+                _cmd = command[3:]
+                to_regex = True
             else:
-                elements.append(h)
-        if not elements and not patterns:
-            if isinstance(_cmd_name, TPattern):
-                return cls((command, prefixes), re.compile(f"(?:{ch_text[:-1]}){_cmd_str}"), mapping, compact)
-            _cmd_name.pattern = f"(?:{ch_text[:-1]}){_cmd_name.pattern}"  # type: ignore
-            _cmd_name.regex_pattern = re.compile(_cmd_name.pattern)  # type: ignore
-            return cls((command, prefixes), _cmd_name, compact=compact)
-        return cls(
-            (command, prefixes),
-            Double(
-                elements,
-                UnionPattern(patterns) if patterns else None,
-                re.compile(f"(?:{ch_text[:-1]})") if ch_text else None,
-                _cmd_name,
-            ),
-            mapping,
-            compact
-        )
+                _cmd, to_regex = handle_bracket(command, mapping)
+            if not prefixes:
+                cmd = re.compile(_cmd) if to_regex else {_cmd}
+                return cls((command, prefixes), cmd, mapping, compact, re.compile(f"^{_cmd}"))
+            if isinstance(prefixes[0], tuple):
+                return cls(
+                    (command, prefixes), [
+                        Pair(h[0], re.compile(re.escape(h[1]) + _cmd) if to_regex else h[1] + _cmd)
+                        for h in prefixes
+                    ], mapping, compact
+                )
+            if all(isinstance(h, str) for h in prefixes):
+                prf = "|".join(re.escape(h) for h in prefixes)
+                compp = re.compile(f"^(?:{prf}){_cmd}")
+                if to_regex:
+                    return cls((command, prefixes), re.compile(f"(?:{prf}){_cmd}"), mapping, compact, compp)
+                return cls((command, prefixes), {f"{h}{_cmd}" for h in prefixes}, mapping, compact, compp)
+            return cls((command, prefixes), Double(prefixes, _cmd), mapping, compact)
+        else:
+            _cmd = deepcopy(type_parser(command))
+            if not prefixes:
+                return cls((command, prefixes), _cmd, {}, compact, _cmd.prefixed())
+            if isinstance(prefixes[0], tuple):
+                raise TypeError(lang.require("header", "prefix_error"))
+            return cls((command, prefixes), Double(prefixes, _cmd), {}, compact)
```

### Comparing `arclet-alconna-1.7.4/src/arclet/alconna/_internal/_util.py` & `arclet-alconna-1.7.5/src/arclet/alconna/_internal/_util.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.4/src/arclet/alconna/action.py` & `arclet-alconna-1.7.5/src/arclet/alconna/action.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.4/src/arclet/alconna/args.py` & `arclet-alconna-1.7.5/src/arclet/alconna/args.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.4/src/arclet/alconna/argv.py` & `arclet-alconna-1.7.5/src/arclet/alconna/argv.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.4/src/arclet/alconna/arparma.py` & `arclet-alconna-1.7.5/src/arclet/alconna/arparma.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.4/src/arclet/alconna/base.py` & `arclet-alconna-1.7.5/src/arclet/alconna/base.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.4/src/arclet/alconna/builtin.py` & `arclet-alconna-1.7.5/src/arclet/alconna/builtin.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.4/src/arclet/alconna/completion.py` & `arclet-alconna-1.7.5/src/arclet/alconna/completion.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.4/src/arclet/alconna/config.py` & `arclet-alconna-1.7.5/src/arclet/alconna/config.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.4/src/arclet/alconna/core.py` & `arclet-alconna-1.7.5/src/arclet/alconna/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,15 @@
         name = f"{self.command or self.prefixes[0]}"  # type: ignore
         self.path = f"{self.namespace}::{name}"
         _args = Args()
         for i in filter(lambda x: isinstance(x, (Args, Arg)), args):
             _args << i
         super().__init__(
             "ALCONNA::",
-            _args, *options, dest=name, separators=separators or ns_config.separators,
+            _args, *options, dest=name, separators=separators or ns_config.separators, help_text=self.meta.description
         )
         self.name = name
         self.behaviors = []
         for behavior in behaviors or []:
             self.behaviors.extend(requirement_handler(behavior))
         command_manager.register(self)
         self._executors: list[ArparmaExecutor] = []
```

### Comparing `arclet-alconna-1.7.4/src/arclet/alconna/duplication.py` & `arclet-alconna-1.7.5/src/arclet/alconna/duplication.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.4/src/arclet/alconna/exceptions.py` & `arclet-alconna-1.7.5/src/arclet/alconna/exceptions.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.4/src/arclet/alconna/formatter.py` & `arclet-alconna-1.7.5/src/arclet/alconna/formatter.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.4/src/arclet/alconna/i18n/en-US.json` & `arclet-alconna-1.7.5/src/arclet/alconna/i18n/en-US.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9861111111111112%*

 * *Differences: {"'header'": "{'prefix_error': 'Prefixes cannot be tuple when command is not str'}"}*

```diff
@@ -54,15 +54,16 @@
         "subcommands.subs": "Commands in above command",
         "usage": "Usage"
     },
     "fuzzy": {
         "matched": "{target} is not matched. Do you mean \"{source}\"?"
     },
     "header": {
-        "error": "{target} dose not matched"
+        "error": "{target} dose not matched",
+        "prefix_error": "Prefixes cannot be tuple when command is not str"
     },
     "manager": {
         "help_footer": "# Invoke '$command {help}' to see syntax",
         "help_header": "# Following commands are available:",
         "help_pages": "Page {current} of {total}",
         "incorrect_shortcut": "Shortcut {target} cannot be used",
         "target_command_error": "The target command of {shortcut} is not {target}",
```

### Comparing `arclet-alconna-1.7.4/src/arclet/alconna/i18n/zh-CN.json` & `arclet-alconna-1.7.5/src/arclet/alconna/i18n/zh-CN.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9861111111111112%*

 * *Differences: {"'header'": "{'prefix_error': '当命令名不是字符串时，命令前缀不能是元组'}"}*

```diff
@@ -54,15 +54,16 @@
         "subcommands.subs": "\u8be5\u5b50\u547d\u4ee4\u5185\u53ef\u7528\u7684\u5b50\u547d\u4ee4\u6709",
         "usage": "\u7528\u6cd5"
     },
     "fuzzy": {
         "matched": "\u65e0\u6cd5\u89e3\u6790 {target}\u3002\u60a8\u60f3\u8981\u8f93\u5165\u7684\u662f\u4e0d\u662f \"{source}\" ?"
     },
     "header": {
-        "error": "\u547d\u4ee4\u5934\u90e8 {target} \u5339\u914d\u5931\u8d25"
+        "error": "\u547d\u4ee4\u5934\u90e8 {target} \u5339\u914d\u5931\u8d25",
+        "prefix_error": "\u5f53\u547d\u4ee4\u540d\u4e0d\u662f\u5b57\u7b26\u4e32\u65f6\uff0c\u547d\u4ee4\u524d\u7f00\u4e0d\u80fd\u662f\u5143\u7ec4"
     },
     "manager": {
         "help_footer": "# \u8f93\u5165'\u547d\u4ee4\u540d {help}' \u67e5\u770b\u7279\u5b9a\u547d\u4ee4\u7684\u8bed\u6cd5",
         "help_header": "# \u5f53\u524d\u53ef\u7528\u7684\u547d\u4ee4\u6709:",
         "help_pages": "\u7b2c {current}/{total} \u9875",
         "incorrect_shortcut": "\u5feb\u6377\u547d\u4ee4 {target} \u65e0\u6cd5\u4f7f\u7528",
         "target_command_error": "{shortcut} \u7684\u76ee\u6807\u547d\u4ee4 {target} \u9519\u8bef",
```

### Comparing `arclet-alconna-1.7.4/src/arclet/alconna/manager.py` & `arclet-alconna-1.7.5/src/arclet/alconna/manager.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.4/src/arclet/alconna/model.py` & `arclet-alconna-1.7.5/src/arclet/alconna/model.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.4/src/arclet/alconna/model.pyi` & `arclet-alconna-1.7.5/src/arclet/alconna/model.pyi`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.4/src/arclet/alconna/output.py` & `arclet-alconna-1.7.5/src/arclet/alconna/output.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.4/src/arclet/alconna/stub.py` & `arclet-alconna-1.7.5/src/arclet/alconna/stub.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.4/src/arclet/alconna/typing.py` & `arclet-alconna-1.7.5/src/arclet/alconna/typing.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.4/tests/analyser_test.py` & `arclet-alconna-1.7.5/tests/analyser_test.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.4/tests/args_test.py` & `arclet-alconna-1.7.5/tests/args_test.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.4/tests/base_test.py` & `arclet-alconna-1.7.5/tests/base_test.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.4/tests/components_test.py` & `arclet-alconna-1.7.5/tests/components_test.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.4/tests/config_test.py` & `arclet-alconna-1.7.5/tests/config_test.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.4/tests/core_test.py` & `arclet-alconna-1.7.5/tests/core_test.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.4/PKG-INFO` & `arclet-alconna-1.7.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arclet-alconna
-Version: 1.7.4
+Version: 1.7.5
 Summary: A High-performance, Generality, Humane Command Line Arguments Parser Library.
 License: MIT
 Keywords: command,argparse,fast,alconna,cli,command-line,parsing,optparse
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 Requires-Python: >=3.8
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

