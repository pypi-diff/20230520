# Comparing `tmp/arclet-alconna-1.7.5.tar.gz` & `tmp/arclet-alconna-1.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arclet-alconna-1.7.5.tar", last modified: Sat May 20 10:54:11 2023, max compression
+gzip compressed data, was "arclet-alconna-1.7.6.tar", last modified: Sat May 20 12:06:18 2023, max compression
```

## Comparing `arclet-alconna-1.7.5.tar` & `arclet-alconna-1.7.6.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524011 arclet-alconna-1.7.5/LICENSE
--rw-r--r--   0        0        0     2810 2023-05-11 05:55:21.918053 arclet-alconna-1.7.5/pyproject.toml
--rw-r--r--   0        0        0     6702 2023-05-11 05:55:23.383958 arclet-alconna-1.7.5/README-EN.md
--rw-r--r--   0        0        0     1084 2023-05-19 14:58:51.597031 arclet-alconna-1.7.5/src/arclet/alconna/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 05:53:44.746150 arclet-alconna-1.7.5/src/arclet/alconna/_internal/__init__.py
--rw-r--r--   0        0        0    17863 2023-05-19 14:58:51.598030 arclet-alconna-1.7.5/src/arclet/alconna/_internal/_analyser.py
--rw-r--r--   0        0        0     8476 2023-05-11 05:53:44.748144 arclet-alconna-1.7.5/src/arclet/alconna/_internal/_argv.py
--rw-r--r--   0        0        0    23361 2023-05-19 14:58:51.599030 arclet-alconna-1.7.5/src/arclet/alconna/_internal/_handlers.py
--rw-r--r--   0        0        0     9971 2023-05-19 14:58:51.600030 arclet-alconna-1.7.5/src/arclet/alconna/_internal/_header.py
--rw-r--r--   0        0        0      837 2023-05-11 05:53:44.749146 arclet-alconna-1.7.5/src/arclet/alconna/_internal/_util.py
--rw-r--r--   0        0        0     1543 2023-05-11 05:54:34.441719 arclet-alconna-1.7.5/src/arclet/alconna/action.py
--rw-r--r--   0        0        0    14429 2023-05-11 05:55:00.317381 arclet-alconna-1.7.5/src/arclet/alconna/args.py
--rw-r--r--   0        0        0     1499 2023-05-11 05:53:44.752371 arclet-alconna-1.7.5/src/arclet/alconna/argv.py
--rw-r--r--   0        0        0    15660 2023-05-11 05:55:01.638197 arclet-alconna-1.7.5/src/arclet/alconna/arparma.py
--rw-r--r--   0        0        0    13248 2023-05-11 05:55:02.886909 arclet-alconna-1.7.5/src/arclet/alconna/base.py
--rw-r--r--   0        0        0     1889 2023-05-11 05:55:04.954858 arclet-alconna-1.7.5/src/arclet/alconna/builtin.py
--rw-r--r--   0        0        0     4867 2023-05-11 05:53:44.757144 arclet-alconna-1.7.5/src/arclet/alconna/completion.py
--rw-r--r--   0        0        0     4465 2023-05-11 05:55:07.597153 arclet-alconna-1.7.5/src/arclet/alconna/config.py
--rw-r--r--   0        0        0    14061 2023-05-19 14:58:51.601035 arclet-alconna-1.7.5/src/arclet/alconna/core.py
--rw-r--r--   0        0        0     2617 2023-05-11 05:55:14.716787 arclet-alconna-1.7.5/src/arclet/alconna/duplication.py
--rw-r--r--   0        0        0     1009 2023-05-11 05:55:16.833416 arclet-alconna-1.7.5/src/arclet/alconna/exceptions.py
--rw-r--r--   0        0        0    11287 2023-05-11 05:55:17.442184 arclet-alconna-1.7.5/src/arclet/alconna/formatter.py
--rw-r--r--   0        0        0       99 2023-05-11 05:53:44.763145 arclet-alconna-1.7.5/src/arclet/alconna/i18n/.config.json
--rw-r--r--   0        0        0     3638 2023-05-19 14:58:51.602031 arclet-alconna-1.7.5/src/arclet/alconna/i18n/en-US.json
--rw-r--r--   0        0        0     3687 2023-05-19 14:58:51.603034 arclet-alconna-1.7.5/src/arclet/alconna/i18n/zh-CN.json
--rw-r--r--   0        0        0    16956 2023-05-11 05:55:18.044404 arclet-alconna-1.7.5/src/arclet/alconna/manager.py
--rw-r--r--   0        0        0     1484 2023-05-11 05:55:18.667097 arclet-alconna-1.7.5/src/arclet/alconna/model.py
--rw-r--r--   0        0        0     1943 2023-05-11 05:55:19.651541 arclet-alconna-1.7.5/src/arclet/alconna/model.pyi
--rw-r--r--   0        0        0     3940 2023-05-11 05:55:20.308191 arclet-alconna-1.7.5/src/arclet/alconna/output.py
--rw-r--r--   0        0        0        0 2023-05-11 05:53:44.769149 arclet-alconna-1.7.5/src/arclet/alconna/py.typed
--rw-r--r--   0        0        0     5815 2023-05-11 05:55:25.933152 arclet-alconna-1.7.5/src/arclet/alconna/stub.py
--rw-r--r--   0        0        0     3586 2023-05-11 05:55:26.563876 arclet-alconna-1.7.5/src/arclet/alconna/typing.py
--rw-r--r--   0        0        0     3246 2023-05-11 05:53:44.772143 arclet-alconna-1.7.5/tests/analyser_test.py
--rw-r--r--   0        0        0     7583 2023-05-11 05:53:44.773143 arclet-alconna-1.7.5/tests/args_test.py
--rw-r--r--   0        0        0     2167 2023-05-11 05:55:03.459296 arclet-alconna-1.7.5/tests/base_test.py
--rw-r--r--   0        0        0     3113 2023-05-11 05:53:44.774144 arclet-alconna-1.7.5/tests/components_test.py
--rw-r--r--   0        0        0     1199 2023-05-11 05:53:44.774144 arclet-alconna-1.7.5/tests/config_test.py
--rw-r--r--   0        0        0    23995 2023-05-19 14:58:51.604030 arclet-alconna-1.7.5/tests/core_test.py
--rw-r--r--   0        0        0      505 2023-05-11 05:53:44.775105 arclet-alconna-1.7.5/tests/util_test.py
--rw-r--r--   0        0        0     7363 1970-01-01 00:00:00.000000 arclet-alconna-1.7.5/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524011 arclet-alconna-1.7.6/LICENSE
+-rw-r--r--   0        0        0     2810 2023-05-11 05:55:21.918053 arclet-alconna-1.7.6/pyproject.toml
+-rw-r--r--   0        0        0     6702 2023-05-11 05:55:23.383958 arclet-alconna-1.7.6/README-EN.md
+-rw-r--r--   0        0        0     1084 2023-05-20 11:27:26.756981 arclet-alconna-1.7.6/src/arclet/alconna/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 05:53:44.746150 arclet-alconna-1.7.6/src/arclet/alconna/_internal/__init__.py
+-rw-r--r--   0        0        0    17897 2023-05-20 11:20:33.572115 arclet-alconna-1.7.6/src/arclet/alconna/_internal/_analyser.py
+-rw-r--r--   0        0        0     8476 2023-05-11 05:53:44.748144 arclet-alconna-1.7.6/src/arclet/alconna/_internal/_argv.py
+-rw-r--r--   0        0        0    23361 2023-05-19 14:58:51.599030 arclet-alconna-1.7.6/src/arclet/alconna/_internal/_handlers.py
+-rw-r--r--   0        0        0     9971 2023-05-19 14:58:51.600030 arclet-alconna-1.7.6/src/arclet/alconna/_internal/_header.py
+-rw-r--r--   0        0        0      837 2023-05-11 05:53:44.749146 arclet-alconna-1.7.6/src/arclet/alconna/_internal/_util.py
+-rw-r--r--   0        0        0     1543 2023-05-11 05:54:34.441719 arclet-alconna-1.7.6/src/arclet/alconna/action.py
+-rw-r--r--   0        0        0    14429 2023-05-11 05:55:00.317381 arclet-alconna-1.7.6/src/arclet/alconna/args.py
+-rw-r--r--   0        0        0     1499 2023-05-11 05:53:44.752371 arclet-alconna-1.7.6/src/arclet/alconna/argv.py
+-rw-r--r--   0        0        0    15660 2023-05-11 05:55:01.638197 arclet-alconna-1.7.6/src/arclet/alconna/arparma.py
+-rw-r--r--   0        0        0    13248 2023-05-11 05:55:02.886909 arclet-alconna-1.7.6/src/arclet/alconna/base.py
+-rw-r--r--   0        0        0     1889 2023-05-11 05:55:04.954858 arclet-alconna-1.7.6/src/arclet/alconna/builtin.py
+-rw-r--r--   0        0        0     4867 2023-05-11 05:53:44.757144 arclet-alconna-1.7.6/src/arclet/alconna/completion.py
+-rw-r--r--   0        0        0     4465 2023-05-11 05:55:07.597153 arclet-alconna-1.7.6/src/arclet/alconna/config.py
+-rw-r--r--   0        0        0    14061 2023-05-19 14:58:51.601035 arclet-alconna-1.7.6/src/arclet/alconna/core.py
+-rw-r--r--   0        0        0     2617 2023-05-11 05:55:14.716787 arclet-alconna-1.7.6/src/arclet/alconna/duplication.py
+-rw-r--r--   0        0        0     1009 2023-05-11 05:55:16.833416 arclet-alconna-1.7.6/src/arclet/alconna/exceptions.py
+-rw-r--r--   0        0        0    11287 2023-05-11 05:55:17.442184 arclet-alconna-1.7.6/src/arclet/alconna/formatter.py
+-rw-r--r--   0        0        0       99 2023-05-11 05:53:44.763145 arclet-alconna-1.7.6/src/arclet/alconna/i18n/.config.json
+-rw-r--r--   0        0        0     3638 2023-05-19 14:58:51.602031 arclet-alconna-1.7.6/src/arclet/alconna/i18n/en-US.json
+-rw-r--r--   0        0        0     3687 2023-05-19 14:58:51.603034 arclet-alconna-1.7.6/src/arclet/alconna/i18n/zh-CN.json
+-rw-r--r--   0        0        0    17034 2023-05-20 11:18:12.523446 arclet-alconna-1.7.6/src/arclet/alconna/manager.py
+-rw-r--r--   0        0        0     1484 2023-05-11 05:55:18.667097 arclet-alconna-1.7.6/src/arclet/alconna/model.py
+-rw-r--r--   0        0        0     1943 2023-05-11 05:55:19.651541 arclet-alconna-1.7.6/src/arclet/alconna/model.pyi
+-rw-r--r--   0        0        0     3940 2023-05-11 05:55:20.308191 arclet-alconna-1.7.6/src/arclet/alconna/output.py
+-rw-r--r--   0        0        0        0 2023-05-11 05:53:44.769149 arclet-alconna-1.7.6/src/arclet/alconna/py.typed
+-rw-r--r--   0        0        0     5815 2023-05-11 05:55:25.933152 arclet-alconna-1.7.6/src/arclet/alconna/stub.py
+-rw-r--r--   0        0        0     3586 2023-05-11 05:55:26.563876 arclet-alconna-1.7.6/src/arclet/alconna/typing.py
+-rw-r--r--   0        0        0     3246 2023-05-11 05:53:44.772143 arclet-alconna-1.7.6/tests/analyser_test.py
+-rw-r--r--   0        0        0     7583 2023-05-11 05:53:44.773143 arclet-alconna-1.7.6/tests/args_test.py
+-rw-r--r--   0        0        0     2167 2023-05-11 05:55:03.459296 arclet-alconna-1.7.6/tests/base_test.py
+-rw-r--r--   0        0        0     3113 2023-05-11 05:53:44.774144 arclet-alconna-1.7.6/tests/components_test.py
+-rw-r--r--   0        0        0     1199 2023-05-11 05:53:44.774144 arclet-alconna-1.7.6/tests/config_test.py
+-rw-r--r--   0        0        0    23993 2023-05-20 11:16:57.405551 arclet-alconna-1.7.6/tests/core_test.py
+-rw-r--r--   0        0        0      505 2023-05-11 05:53:44.775105 arclet-alconna-1.7.6/tests/util_test.py
+-rw-r--r--   0        0        0     7363 1970-01-01 00:00:00.000000 arclet-alconna-1.7.6/PKG-INFO
```

### Comparing `arclet-alconna-1.7.5/LICENSE` & `arclet-alconna-1.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.5/pyproject.toml` & `arclet-alconna-1.7.6/pyproject.toml`

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
-version = "1.7.5"
+version = "1.7.6"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 documentation = "https://arcletproject.github.io/docs/alconna/tutorial"
 repository = "https://github.com/ArcletProject/Alconna"
```

### Comparing `arclet-alconna-1.7.5/README-EN.md` & `arclet-alconna-1.7.6/README-EN.md`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.5/src/arclet/alconna/__init__.py` & `arclet-alconna-1.7.6/src/arclet/alconna/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,12 +17,12 @@
 from .builtin import set_default
 from .model import OptionResult, SubcommandResult, HeadResult
 from .output import output_manager
 from .formatter import TextFormatter
 from .duplication import Duplication
 from .stub import ArgsStub, OptionStub, SubcommandStub
 
-__version__ = "1.7.5"
+__version__ = "1.7.6"
 
 # backward compatibility
 Arpamar = Arparma
 DataCollectionContainer = Argv
```

### Comparing `arclet-alconna-1.7.5/src/arclet/alconna/_internal/_analyser.py` & `arclet-alconna-1.7.6/src/arclet/alconna/_internal/_analyser.py`

 * *Files 1% similar despite different names*

```diff
@@ -281,15 +281,16 @@
             Arparma[TDC]: Arparma 解析结果
 
         Raises:
             ParamsUnmatched: 若不允许快捷命令后随其他参数，则抛出此异常
         """
         if isinstance(short, Arparma):
             return short
-        argv.build(short.get('command', self.command.command or self.command.name))
+
+        argv.build(short.get('command', argv.converter(self.command.command) or argv.converter(self.command.name)))
         if not short.get('fuzzy') and data:
             exc = ParamsUnmatched(lang.require("analyser", "param_unmatched").format(target=data[0]))
             if self.command.meta.raise_exception:
                 raise exc
             return self.export(argv, True, exc)
         data_index = 0
         for i, unit in enumerate(argv.raw_data):
```

### Comparing `arclet-alconna-1.7.5/src/arclet/alconna/_internal/_argv.py` & `arclet-alconna-1.7.6/src/arclet/alconna/_internal/_argv.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.5/src/arclet/alconna/_internal/_handlers.py` & `arclet-alconna-1.7.6/src/arclet/alconna/_internal/_handlers.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.5/src/arclet/alconna/_internal/_header.py` & `arclet-alconna-1.7.6/src/arclet/alconna/_internal/_header.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.5/src/arclet/alconna/_internal/_util.py` & `arclet-alconna-1.7.6/src/arclet/alconna/_internal/_util.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.5/src/arclet/alconna/action.py` & `arclet-alconna-1.7.6/src/arclet/alconna/action.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.5/src/arclet/alconna/args.py` & `arclet-alconna-1.7.6/src/arclet/alconna/args.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.5/src/arclet/alconna/argv.py` & `arclet-alconna-1.7.6/src/arclet/alconna/argv.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.5/src/arclet/alconna/arparma.py` & `arclet-alconna-1.7.6/src/arclet/alconna/arparma.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.5/src/arclet/alconna/base.py` & `arclet-alconna-1.7.6/src/arclet/alconna/base.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.5/src/arclet/alconna/builtin.py` & `arclet-alconna-1.7.6/src/arclet/alconna/builtin.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.5/src/arclet/alconna/completion.py` & `arclet-alconna-1.7.6/src/arclet/alconna/completion.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.5/src/arclet/alconna/config.py` & `arclet-alconna-1.7.6/src/arclet/alconna/config.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.5/src/arclet/alconna/core.py` & `arclet-alconna-1.7.6/src/arclet/alconna/core.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.5/src/arclet/alconna/duplication.py` & `arclet-alconna-1.7.6/src/arclet/alconna/duplication.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.5/src/arclet/alconna/exceptions.py` & `arclet-alconna-1.7.6/src/arclet/alconna/exceptions.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.5/src/arclet/alconna/formatter.py` & `arclet-alconna-1.7.6/src/arclet/alconna/formatter.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.5/src/arclet/alconna/i18n/en-US.json` & `arclet-alconna-1.7.6/src/arclet/alconna/i18n/en-US.json`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.5/src/arclet/alconna/i18n/zh-CN.json` & `arclet-alconna-1.7.6/src/arclet/alconna/i18n/zh-CN.json`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.5/src/arclet/alconna/manager.py` & `arclet-alconna-1.7.6/src/arclet/alconna/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,15 +244,16 @@
         """
         namespace, name = self._command_part(target.path)
         if query:
             try:
                 return self.__shortcuts[f"{namespace}.{name}::{query}"], None
             except KeyError as e:
                 for k in self.__shortcuts:
-                    if mat := re.match(k.split("::")[1], query):
+                    prefix, key = k.rsplit("::", 1)
+                    if f"{namespace}.{name}" == prefix and (mat := re.match(key, query)):
                         return self.__shortcuts[k], mat
                 raise ValueError(
                     lang.require("manager", "target_command_error").format(target=f"{namespace}.{name}", shortcut=query)
                 ) from e
         return [self.__shortcuts[k] for k in self.__shortcuts if f"{namespace}.{name}" in k]
 
     def delete_shortcut(self, target: Alconna, key: str | None = None):
```

### Comparing `arclet-alconna-1.7.5/src/arclet/alconna/model.py` & `arclet-alconna-1.7.6/src/arclet/alconna/model.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.5/src/arclet/alconna/model.pyi` & `arclet-alconna-1.7.6/src/arclet/alconna/model.pyi`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.5/src/arclet/alconna/output.py` & `arclet-alconna-1.7.6/src/arclet/alconna/output.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.5/src/arclet/alconna/stub.py` & `arclet-alconna-1.7.6/src/arclet/alconna/stub.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.5/src/arclet/alconna/typing.py` & `arclet-alconna-1.7.6/src/arclet/alconna/typing.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.5/tests/analyser_test.py` & `arclet-alconna-1.7.6/tests/analyser_test.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.5/tests/args_test.py` & `arclet-alconna-1.7.6/tests/args_test.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.5/tests/base_test.py` & `arclet-alconna-1.7.6/tests/base_test.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.5/tests/components_test.py` & `arclet-alconna-1.7.6/tests/components_test.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.5/tests/config_test.py` & `arclet-alconna-1.7.6/tests/config_test.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-1.7.5/tests/core_test.py` & `arclet-alconna-1.7.6/tests/core_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -419,15 +419,14 @@
     res8 = alc16_2.parse("test")
     assert res8.foo is True
     res9 = alc16_2.parse([2, "test"])
     assert res9.foo is True
     assert not alc16_2.parse("3test").matched
 
 
-
 def test_help():
     from arclet.alconna.exceptions import SpecialOptionTriggered
 
     alc17 = Alconna("core17") + Option("foo", Args["bar", str])
     res = alc17.parse("core17 --help")
     assert isinstance(res.error_info, SpecialOptionTriggered)
     alc17.parse("core17 --help foo")
```

### Comparing `arclet-alconna-1.7.5/PKG-INFO` & `arclet-alconna-1.7.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arclet-alconna
-Version: 1.7.5
+Version: 1.7.6
 Summary: A High-performance, Generality, Humane Command Line Arguments Parser Library.
 License: MIT
 Keywords: command,argparse,fast,alconna,cli,command-line,parsing,optparse
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 Requires-Python: >=3.8
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

