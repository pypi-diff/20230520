# Comparing `tmp/configzen-0.1.23.tar.gz` & `tmp/configzen-0.1.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configzen-0.1.23.tar", max compression
+gzip compressed data, was "configzen-0.1.24.tar", max compression
```

## Comparing `configzen-0.1.23.tar` & `configzen-0.1.24.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      216 2023-05-17 21:14:40.122071 configzen-0.1.23/configzen/__init__.py
--rw-r--r--   0        0        0      904 2023-05-19 14:41:10.408896 configzen-0.1.23/configzen/__main__.py
--rw-r--r--   0        0        0    52979 2023-05-19 22:51:22.835958 configzen-0.1.23/configzen/config.py
--rw-r--r--   0        0        0     2470 2023-05-19 16:49:24.141768 configzen-0.1.23/configzen/errors.py
--rw-r--r--   0        0        0    18864 2023-05-19 23:20:26.793709 configzen-0.1.23/configzen/processor.py
--rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.1.23/configzen/py.typed
--rw-r--r--   0        0        0      777 2023-05-19 17:03:50.493938 configzen-0.1.23/configzen/typedefs.py
--rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.1.23/LICENSE
--rw-r--r--   0        0        0     1687 2023-05-19 23:21:12.811782 configzen-0.1.23/pyproject.toml
--rw-r--r--   0        0        0     7150 2023-05-19 22:44:45.534902 configzen-0.1.23/README.md
--rw-r--r--   0        0        0     7841 1970-01-01 00:00:00.000000 configzen-0.1.23/PKG-INFO
+-rw-r--r--   0        0        0      216 2023-05-17 21:14:40.122071 configzen-0.1.24/configzen/__init__.py
+-rw-r--r--   0        0        0      904 2023-05-19 14:41:10.408896 configzen-0.1.24/configzen/__main__.py
+-rw-r--r--   0        0        0    53152 2023-05-20 00:12:29.622344 configzen-0.1.24/configzen/config.py
+-rw-r--r--   0        0        0     2470 2023-05-19 16:49:24.141768 configzen-0.1.24/configzen/errors.py
+-rw-r--r--   0        0        0    19828 2023-05-20 00:04:43.942145 configzen-0.1.24/configzen/processor.py
+-rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.1.24/configzen/py.typed
+-rw-r--r--   0        0        0      777 2023-05-19 17:03:50.493938 configzen-0.1.24/configzen/typedefs.py
+-rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.1.24/LICENSE
+-rw-r--r--   0        0        0     1687 2023-05-20 00:14:57.999530 configzen-0.1.24/pyproject.toml
+-rw-r--r--   0        0        0     7150 2023-05-19 22:44:45.534902 configzen-0.1.24/README.md
+-rw-r--r--   0        0        0     7841 1970-01-01 00:00:00.000000 configzen-0.1.24/PKG-INFO
```

### Comparing `configzen-0.1.23/configzen/__main__.py` & `configzen-0.1.24/configzen/__main__.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.23/configzen/config.py` & `configzen-0.1.24/configzen/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1541,15 +1541,15 @@
         if kwargs.get("to_dict", False):
             state = {}
             for key, value in super()._iter(**kwargs):
                 state[key] = value
             metadata = getattr(self, SUBST_METADATA, None)
             if metadata:
                 context = get_context(self)
-                context.loader.processor_class.export(state, metadata)
+                context.loader.processor_class.export(state, metadata=metadata)
             yield from state.items()
         else:
             yield from super()._iter(**kwargs)
 
     @classmethod
     def _resolve_loader(
         cls,
@@ -1620,14 +1620,20 @@
             # pydantic.BaseModel.__instancecheck__() and __subclasscheck__()...
             and ConfigModel in type(value).mro()
             and not hasattr(value, CONTEXT)
         ):
             context.enter(name).bind_to(value)
         return value
 
+    def __deepcopy__(
+        self: ConfigModelT,
+        memodict: dict[Any, Any] | None = None
+    ) -> ConfigModelT:
+        return self.parse_obj(self.dict())
+
     def __getattribute__(self, attr: str) -> Any:
         value = super().__getattribute__(attr)
         if isinstance(value, ConfigModel):
             return self._ensure_settings_with_context(attr, value)
         return value
 
     @classmethod
```

### Comparing `configzen-0.1.23/configzen/errors.py` & `configzen-0.1.24/configzen/errors.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.23/configzen/processor.py` & `configzen-0.1.24/configzen/processor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import dataclasses
 import enum
 from collections.abc import Callable
-from typing import TYPE_CHECKING, Any, ClassVar, Generic, TypedDict, TypeVar
+from typing import TYPE_CHECKING, Any, ClassVar, Generic, TypedDict, TypeVar, cast
 
 from anyconfig.utils import is_dict_like, is_list_like
 
 from configzen.errors import (
     InternalConfigError,
     format_syntax_error,
     ConfigPreprocessingError,
@@ -274,49 +274,83 @@
     ) -> None:
         self.loader = resource
         self.dict_config = dict_config
 
     @classmethod
     def export(
         cls,
-        state: dict[str, Any],
+        state: Any,
+        *,
+        metadata: SubstitutionMetadata[ConfigModelT] | None = None,
+    ) -> None:
+        """
+        Export the state.
+
+        Parameters
+        ----------
+        state
+            The state to export.
+        metadata
+            The metadata of the substitution.
+        """
+        if is_dict_like(state):
+            if metadata is None:
+                from configzen.config import CONTEXT
+                state.pop(CONTEXT, None)
+                metadata = state.pop(SUBST_METADATA, None)
+            if metadata:
+                cls._export(state, metadata)
+            else:
+                cls.export(list(state.values()), metadata=None)
+        elif is_list_like(state):
+            for item in state:
+                cls.export(item, metadata=None)
+
+    @classmethod
+    def _export(
+        cls,
+        state: Any,
         metadata: SubstitutionMetadata[ConfigModelT],
     ) -> None:
-        pass
+        raise NotImplementedError
 
     def preprocess(self) -> dict[str, Any]:
         """
         Parse the dictionary config and return the parsed config,
         ready for instantiating the model.
 
         Returns
         -------
         The parsed config.
         """
-        return self._preprocess(self.dict_config)
+        return cast(dict[str, Any], self._preprocess(self.dict_config))
+
+    def _preprocess(self, container: Any) -> Any:
+        if not is_dict_like(container):
+            if is_list_like(container):
+                return [self._preprocess(v) for v in container]
+            return container
 
-    def _preprocess(self, container: dict[str, Any]) -> dict[str, Any]:
         result: dict[str, Any] = {}
 
         for key, value in sorted(
-            container.items(),
+            cast(dict[str, Any], container).items(),
             key=lambda item: item[0] == self.directive_prefix,
         ):
             if key.startswith(self.extension_prefix):
                 actual_key = key.lstrip(self.extension_prefix)
                 overridden = result.get(actual_key, {})
                 if not is_dict_like(overridden):
                     raise ConfigPreprocessingError(
                         f"{self.extension_prefix} can be used only for overriding "
                         f"dictionary sections but item at {actual_key!r} "
                         f"is not a dictionary"
                     )
                 replacement = overridden | value
-                self._preprocess(replacement)
-                result[actual_key] = replacement
+                result[actual_key] = self._preprocess(replacement)
             elif key.startswith(self.directive_prefix):
                 directive_name, arguments = parse_directive_call(
                     self.directive_prefix, key
                 )
                 context_container = container.copy()
                 del context_container[key]
                 context = DirectiveContext(
@@ -326,22 +360,16 @@
                     arguments=arguments,
                     snippet=value,
                     container=context_container,
                 )
                 self._call_directive(context)
                 new_container = self._preprocess(context.container)
                 result |= new_container
-            elif is_dict_like(value):
-                result[key] = self._preprocess(value)
-            elif is_list_like(value):
-                result[key] = [
-                    self._preprocess(v) if isinstance(v, dict) else v for v in value
-                ]
             else:
-                result[key] = value
+                result[key] = self._preprocess(value)
         return result
 
     def _call_directive(self, context: DirectiveContext) -> None:
         handler = self._directive_handlers.get(context.directive)
         if handler is None:
             raise ConfigPreprocessingError(
                 f"unknown preprocessing directive: {context.directive!r}"
@@ -570,15 +598,15 @@
                 CONTEXT: context,
                 SUBST_METADATA: SubstitutionMetadata(
                     route=substitution_route, context=context, preprocess=preprocess
                 ),
             }
 
     @classmethod
-    def export(
+    def _export(
         cls,
         state: dict[str, Any],
         metadata: SubstitutionMetadata[ConfigModelT],
     ) -> None:
         """
         Exports model state preserving substition directive calls in the model state.
 
@@ -607,33 +635,41 @@
         missing = object()
 
         for key, value in loaded.items():
             counterpart_value = state.pop(key, missing)
             if counterpart_value is missing:
                 continue
             counterpart_value = convert(counterpart_value)
+
             if is_dict_like(value):
                 if SUBST_METADATA in value:
                     value.pop(CONTEXT, None)
-                    cls.export(value, value.pop(SUBST_METADATA))
+                    cls.export(value, metadata=value.pop(SUBST_METADATA))
                 overrides_for_key = {
                     sub_key: comp
                     for sub_key, orig in value.items()
                     if (
                         (comp := counterpart_value.get(sub_key, missing)) is not missing
                         and orig != comp
                     )
                 }
                 if overrides_for_key:
                     export_key = loader.processor_class.extension_prefix + key
                     overrides[export_key] = overrides_for_key
+
+            elif is_list_like(value):
+                cls.export(value, metadata=None)
+
             elif counterpart_value != value:
                 overrides[key] = counterpart_value
                 del substituted_values[key]
 
+        for value in state.values():
+            cls.export(value, metadata=None)
+
         if substituted_values:
             arguments = [] if route is None else [route]
             substitution_directive = cls.directive(Directives.EXTEND, arguments)
             # Put the substitution directive at the beginning of the state in-place.
             state |= {substitution_directive: context.loader.resource} | {
                 key: state.pop(key) for key in set(state)
             }
```

### Comparing `configzen-0.1.23/configzen/typedefs.py` & `configzen-0.1.24/configzen/typedefs.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.23/LICENSE` & `configzen-0.1.24/LICENSE`

 * *Files identical despite different names*

### Comparing `configzen-0.1.23/pyproject.toml` & `configzen-0.1.24/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "configzen"
-version = "0.1.23"
+version = "0.1.24"
 description = "The easiest way to manage configuration files in Python"
 authors = ["bswck <bswck.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `configzen-0.1.23/README.md` & `configzen-0.1.24/README.md`

 * *Files identical despite different names*

### Comparing `configzen-0.1.23/PKG-INFO` & `configzen-0.1.24/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configzen
-Version: 0.1.23
+Version: 0.1.24
 Summary: The easiest way to manage configuration files in Python
 License: MIT
 Author: bswck
 Author-email: bswck.dev@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

