# Comparing `tmp/utype-0.3.1.tar.gz` & `tmp/utype-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utype-0.3.1.tar", last modified: Thu Apr 27 03:12:23 2023, max compression
+gzip compressed data, was "utype-0.3.2.tar", last modified: Sat May 20 13:30:10 2023, max compression
```

## Comparing `utype-0.3.1.tar` & `utype-0.3.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 03:12:23.618145 utype-0.3.1/
--rw-rw-rw-   0        0        0      588 2022-11-30 10:26:26.000000 utype-0.3.1/LICENSE
--rw-rw-rw-   0        0        0     9845 2023-04-27 03:12:23.618145 utype-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     8413 2023-04-27 03:11:22.000000 utype-0.3.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-27 03:12:23.618145 utype-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1824 2022-12-16 10:42:48.000000 utype-0.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-27 03:12:23.544938 utype-0.3.1/utype/
--rw-rw-rw-   0        0        0     1231 2023-04-27 03:11:22.000000 utype-0.3.1/utype/__init__.py
--rw-rw-rw-   0        0        0     6219 2023-02-18 08:54:07.000000 utype-0.3.1/utype/decorator.py
-drwxrwxrwx   0        0        0        0 2023-04-27 03:12:23.576854 utype-0.3.1/utype/parser/
--rw-rw-rw-   0        0        0        0 2022-12-02 05:43:17.000000 utype-0.3.1/utype/parser/__init__.py
--rw-rw-rw-   0        0        0    22638 2023-03-14 16:30:18.000000 utype-0.3.1/utype/parser/base.py
--rw-rw-rw-   0        0        0    20646 2023-03-21 10:41:05.000000 utype-0.3.1/utype/parser/cls.py
--rw-rw-rw-   0        0        0    47187 2023-03-07 11:36:34.000000 utype-0.3.1/utype/parser/field.py
--rw-rw-rw-   0        0        0    36288 2023-03-11 14:32:10.000000 utype-0.3.1/utype/parser/func.py
--rw-rw-rw-   0        0        0    16412 2023-04-08 06:18:37.000000 utype-0.3.1/utype/parser/options.py
--rw-rw-rw-   0        0        0    66625 2023-03-07 08:37:00.000000 utype-0.3.1/utype/parser/rule.py
--rw-rw-rw-   0        0        0    18006 2023-03-07 13:07:37.000000 utype-0.3.1/utype/schema.py
-drwxrwxrwx   0        0        0        0 2023-04-27 03:12:23.583233 utype-0.3.1/utype/specs/
--rw-rw-rw-   0        0        0        0 2022-11-30 10:26:26.000000 utype-0.3.1/utype/specs/__init__.py
--rw-rw-rw-   0        0        0    12612 2023-03-06 10:25:57.000000 utype-0.3.1/utype/specs/json_schema.py
--rw-rw-rw-   0        0        0     5515 2023-03-19 14:44:00.000000 utype-0.3.1/utype/types.py
-drwxrwxrwx   0        0        0        0 2023-04-27 03:12:23.617143 utype-0.3.1/utype/utils/
--rw-rw-rw-   0        0        0        0 2022-11-30 10:26:26.000000 utype-0.3.1/utype/utils/__init__.py
--rw-rw-rw-   0        0        0     3676 2023-03-04 11:33:54.000000 utype-0.3.1/utype/utils/base.py
--rw-rw-rw-   0        0        0     3260 2023-02-18 09:22:30.000000 utype-0.3.1/utype/utils/compat.py
--rw-rw-rw-   0        0        0     2017 2022-12-16 09:30:29.000000 utype-0.3.1/utype/utils/datastructures.py
--rw-rw-rw-   0        0        0     2957 2023-04-17 07:53:54.000000 utype-0.3.1/utype/utils/encode.py
--rw-rw-rw-   0        0        0     7155 2022-12-16 09:43:52.000000 utype-0.3.1/utype/utils/exceptions.py
--rw-rw-rw-   0        0        0     1184 2022-12-16 05:01:12.000000 utype-0.3.1/utype/utils/functional.py
--rw-rw-rw-   0        0        0     6219 2022-12-16 09:43:52.000000 utype-0.3.1/utype/utils/style.py
--rw-rw-rw-   0        0        0    23130 2023-03-10 09:41:24.000000 utype-0.3.1/utype/utils/transform.py
-drwxrwxrwx   0        0        0        0 2023-04-27 03:12:23.560895 utype-0.3.1/utype.egg-info/
--rw-rw-rw-   0        0        0     9845 2023-04-27 03:12:23.000000 utype-0.3.1/utype.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      659 2023-04-27 03:12:23.000000 utype-0.3.1/utype.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 03:12:23.000000 utype-0.3.1/utype.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-04-27 03:12:23.000000 utype-0.3.1/utype.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-27 03:12:23.000000 utype-0.3.1/utype.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-20 13:30:10.281525 utype-0.3.2/
+-rw-rw-rw-   0        0        0      588 2022-11-30 10:26:26.000000 utype-0.3.2/LICENSE
+-rw-rw-rw-   0        0        0     9845 2023-05-20 13:30:10.281525 utype-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     8413 2023-05-20 13:28:46.000000 utype-0.3.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-20 13:30:10.282523 utype-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1824 2022-12-16 10:42:48.000000 utype-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 13:30:10.194502 utype-0.3.2/utype/
+-rw-rw-rw-   0        0        0     1231 2023-05-20 13:28:46.000000 utype-0.3.2/utype/__init__.py
+-rw-rw-rw-   0        0        0     6219 2023-02-18 08:54:07.000000 utype-0.3.2/utype/decorator.py
+drwxrwxrwx   0        0        0        0 2023-05-20 13:30:10.236646 utype-0.3.2/utype/parser/
+-rw-rw-rw-   0        0        0        0 2022-12-02 05:43:17.000000 utype-0.3.2/utype/parser/__init__.py
+-rw-rw-rw-   0        0        0    22638 2023-03-14 16:30:18.000000 utype-0.3.2/utype/parser/base.py
+-rw-rw-rw-   0        0        0    20646 2023-03-21 10:41:05.000000 utype-0.3.2/utype/parser/cls.py
+-rw-rw-rw-   0        0        0    47619 2023-05-13 09:42:03.000000 utype-0.3.2/utype/parser/field.py
+-rw-rw-rw-   0        0        0    36288 2023-03-11 14:32:10.000000 utype-0.3.2/utype/parser/func.py
+-rw-rw-rw-   0        0        0    16412 2023-04-08 06:18:37.000000 utype-0.3.2/utype/parser/options.py
+-rw-rw-rw-   0        0        0    66752 2023-05-16 11:05:22.000000 utype-0.3.2/utype/parser/rule.py
+-rw-rw-rw-   0        0        0    18029 2023-05-13 09:44:39.000000 utype-0.3.2/utype/schema.py
+drwxrwxrwx   0        0        0        0 2023-05-20 13:30:10.243631 utype-0.3.2/utype/specs/
+-rw-rw-rw-   0        0        0        0 2022-11-30 10:26:26.000000 utype-0.3.2/utype/specs/__init__.py
+-rw-rw-rw-   0        0        0    12612 2023-03-06 10:25:57.000000 utype-0.3.2/utype/specs/json_schema.py
+-rw-rw-rw-   0        0        0     5515 2023-03-19 14:44:00.000000 utype-0.3.2/utype/types.py
+drwxrwxrwx   0        0        0        0 2023-05-20 13:30:10.280532 utype-0.3.2/utype/utils/
+-rw-rw-rw-   0        0        0        0 2022-11-30 10:26:26.000000 utype-0.3.2/utype/utils/__init__.py
+-rw-rw-rw-   0        0        0     3676 2023-03-04 11:33:54.000000 utype-0.3.2/utype/utils/base.py
+-rw-rw-rw-   0        0        0     3260 2023-02-18 09:22:30.000000 utype-0.3.2/utype/utils/compat.py
+-rw-rw-rw-   0        0        0     2017 2022-12-16 09:30:29.000000 utype-0.3.2/utype/utils/datastructures.py
+-rw-rw-rw-   0        0        0     2957 2023-04-17 07:53:54.000000 utype-0.3.2/utype/utils/encode.py
+-rw-rw-rw-   0        0        0     7155 2022-12-16 09:43:52.000000 utype-0.3.2/utype/utils/exceptions.py
+-rw-rw-rw-   0        0        0     1184 2022-12-16 05:01:12.000000 utype-0.3.2/utype/utils/functional.py
+-rw-rw-rw-   0        0        0     6219 2022-12-16 09:43:52.000000 utype-0.3.2/utype/utils/style.py
+-rw-rw-rw-   0        0        0    23466 2023-05-07 09:05:24.000000 utype-0.3.2/utype/utils/transform.py
+drwxrwxrwx   0        0        0        0 2023-05-20 13:30:10.209564 utype-0.3.2/utype.egg-info/
+-rw-rw-rw-   0        0        0     9845 2023-05-20 13:30:10.000000 utype-0.3.2/utype.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      659 2023-05-20 13:30:10.000000 utype-0.3.2/utype.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 13:30:10.000000 utype-0.3.2/utype.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-05-20 13:30:10.000000 utype-0.3.2/utype.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-20 13:30:10.000000 utype-0.3.2/utype.egg-info/top_level.txt
```

### Comparing `utype-0.3.1/LICENSE` & `utype-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `utype-0.3.1/PKG-INFO` & `utype-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utype
-Version: 0.3.1
+Version: 0.3.2
 Summary: Declare & parse types / dataclasses / functions based on Python type annotations
 Home-page: https://utype.io
 Author: XuLin Zhou
 Author-email: zxl@utilmeta.com
 License: Apache 2.0
 Project-URL: Project Home, https://utype.io
 Project-URL: Documentation, https://utype.io
@@ -39,15 +39,15 @@
 [![Test Coverage](https://img.shields.io/codecov/c/github/utilmeta/utype?color=green)](https://app.codecov.io/github/utilmeta/utype)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Downloads](https://pepy.tech/badge/utype/month)](https://pepy.tech/project/utype)
 
 utype is a data types declaration & parsing library based on Python type annotations, 
 enforce types and constraints for classes and functions at runtime
 
-* Version: `0.3.1` [test]
+* Version: `0.3.2` [test]
 * Author: [@voidZXL](https://github.com/voidZXL)
 * License: Apache 2.0
 * Source Code: [https://github.com/utilmeta/utype](https://github.com/utilmeta/utype)
 * Documentation: [https://utype.io](https://utype.io)
 * 中文文档: [https://utype.io/zh](https://utype.io/zh)
```

### Comparing `utype-0.3.1/README.md` & `utype-0.3.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![Test Coverage](https://img.shields.io/codecov/c/github/utilmeta/utype?color=green)](https://app.codecov.io/github/utilmeta/utype)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Downloads](https://pepy.tech/badge/utype/month)](https://pepy.tech/project/utype)
 
 utype is a data types declaration & parsing library based on Python type annotations, 
 enforce types and constraints for classes and functions at runtime
 
-* Version: `0.3.1` [test]
+* Version: `0.3.2` [test]
 * Author: [@voidZXL](https://github.com/voidZXL)
 * License: Apache 2.0
 * Source Code: [https://github.com/utilmeta/utype](https://github.com/utilmeta/utype)
 * Documentation: [https://utype.io](https://utype.io)
 * 中文文档: [https://utype.io/zh](https://utype.io/zh)
```

### Comparing `utype-0.3.1/setup.py` & `utype-0.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `utype-0.3.1/utype/__init__.py` & `utype-0.3.2/utype/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from .utils.transform import (TypeTransformer, type_transform)
 from .utils.datastructures import unprovided
 from .specs.json_schema import JsonSchemaGenerator
 
 register_transformer = TypeTransformer.registry.register
 
 
-VERSION = (0, 3, 1, None)
+VERSION = (0, 3, 2, None)
 
 
 def _get_version():
     pre_release = VERSION[3] if len(VERSION) > 3 else ""
     version = ".".join([str(v) for v in VERSION[:3]])
     if pre_release:
         version += f"-{pre_release}"
```

### Comparing `utype-0.3.1/utype/decorator.py` & `utype-0.3.2/utype/decorator.py`

 * *Files identical despite different names*

### Comparing `utype-0.3.1/utype/parser/base.py` & `utype-0.3.2/utype/parser/base.py`

 * *Files identical despite different names*

### Comparing `utype-0.3.1/utype/parser/cls.py` & `utype-0.3.2/utype/parser/cls.py`

 * *Files identical despite different names*

### Comparing `utype-0.3.1/utype/parser/field.py` & `utype-0.3.2/utype/parser/field.py`

 * *Files 2% similar despite different names*

```diff
@@ -784,14 +784,17 @@
         if not options.mode:
             # no mode
             return no_input if isinstance(no_input, bool) else False
 
         if isinstance(no_input, (str, list, set, tuple)):
             return options.mode in no_input
 
+        if no_input is True:
+            return True
+
         if self.mode:
             return options.mode not in self.mode
 
         return bool(no_input)
 
     def always_no_input(self, options: Options):
         # calculate before get the value
@@ -836,14 +839,17 @@
         if not options.mode:
             # no mode
             return no_output if isinstance(no_output, bool) else False
 
         if isinstance(no_output, (str, list, set, tuple)):
             return options.mode in no_output
 
+        if no_output is True:
+            return True
+
         if self.mode:
             return options.mode not in self.mode
 
         return bool(no_output)
 
     def check_function(self, func):
         if not self.always_provided:
@@ -1125,15 +1131,20 @@
                 required = False
 
             if prop.fget:
                 return_annotation = getattr(prop.fget, "__annotations__", {}).get(
                     "return"
                 )
 
-                dependencies = inspect.getclosurevars(prop.fget).unbound
+                # dependencies = inspect.getclosurevars(prop.fget).unbound
+                # !!
+                # UNBOUND MAY GET THE WRONG DEPENDENCY AND THUS THE WRONG RESULT (without explicit error)
+                # [SUCH AS self.a.b will make "b" an unbound, which is not the desired dependency]
+                # SO WE SHOULD LET DEVELOPER SPECIFY DEPENDENCIES OR [LET IT FAIL]
+
                 # use the unbound properties as default dependencies of property
                 # you can use @Field(dependencies=[...]) to specify yourself
 
                 output_field = getattr(prop.fget, "__field__", None)
                 if isinstance(output_field, Field):
 
                     if output_field.dependencies:
```

### Comparing `utype-0.3.1/utype/parser/func.py` & `utype-0.3.2/utype/parser/func.py`

 * *Files identical despite different names*

### Comparing `utype-0.3.1/utype/parser/options.py` & `utype-0.3.2/utype/parser/options.py`

 * *Files identical despite different names*

### Comparing `utype-0.3.1/utype/parser/rule.py` & `utype-0.3.2/utype/parser/rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -1423,25 +1423,28 @@
             return t
         if cls.combinator:
             return t & cls
         if cls.__origin__ and issubclass(cls.__origin__, t):
             return cls
         constraints = {}
         for name, val, func in cls.__validators__:
-            constraints[name] = val
+            constraints[name] = getattr(cls, name, val)
+            # do not lose the mode info
+            # so we get value from cls first
+
         # try to find a strong constraint
         if 'const' in constraints or 'enum' in constraints:
             return cls
 
         if isinstance(t, LogicalType):
             if t.combinator:
                 return t & cls
             elif issubclass(t, Rule):
                 for name, val, func in t.__validators__:
-                    constraints[name] = val
+                    constraints[name] = getattr(t, name, val)
                 if 'const' in constraints or 'enum' in constraints:
                     return t
                 return Rule.annotate(
                     t.__origin__ or cls.__origin__,
                     *(t.__args__ or cls.__args__ or []),
                     constraints=constraints
                 )
```

### Comparing `utype-0.3.1/utype/schema.py` & `utype-0.3.2/utype/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,15 +219,15 @@
     # coerce_properties need to separate from set_attributes and execute by order
     # because the dependencies that the property need may not be set during one-time loop
     # (which is guarantee by the field orders, and consider not reliable)
     def __coerce_property__(self, field: ParserField, context: RuntimeContext):
         if field.always_no_output(context.options):
             return
 
-        if not field.dependencies.issubset(self):
+        if field.dependencies and not field.dependencies.issubset(self):
             # maybe some of the dependencies is no_output=True, but still accessible through attribute
             # check if any of those dependencies is not in __dict__, and directly return if found one
             for dep in field.dependencies:
                 dep_field = self.__parser__.get_field(dep)
                 if not dep_field or dep_field.attname not in self.__dict__:
                     return
```

### Comparing `utype-0.3.1/utype/specs/json_schema.py` & `utype-0.3.2/utype/specs/json_schema.py`

 * *Files identical despite different names*

### Comparing `utype-0.3.1/utype/types.py` & `utype-0.3.2/utype/types.py`

 * *Files identical despite different names*

### Comparing `utype-0.3.1/utype/utils/base.py` & `utype-0.3.2/utype/utils/base.py`

 * *Files identical despite different names*

### Comparing `utype-0.3.1/utype/utils/compat.py` & `utype-0.3.2/utype/utils/compat.py`

 * *Files identical despite different names*

### Comparing `utype-0.3.1/utype/utils/datastructures.py` & `utype-0.3.2/utype/utils/datastructures.py`

 * *Files identical despite different names*

### Comparing `utype-0.3.1/utype/utils/encode.py` & `utype-0.3.2/utype/utils/encode.py`

 * *Files identical despite different names*

### Comparing `utype-0.3.1/utype/utils/exceptions.py` & `utype-0.3.2/utype/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `utype-0.3.1/utype/utils/functional.py` & `utype-0.3.2/utype/utils/functional.py`

 * *Files identical despite different names*

### Comparing `utype-0.3.1/utype/utils/style.py` & `utype-0.3.2/utype/utils/style.py`

 * *Files identical despite different names*

### Comparing `utype-0.3.1/utype/utils/transform.py` & `utype-0.3.2/utype/utils/transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import io
 import json
 import re
 from collections import deque
 from collections.abc import Iterable, Iterator, Mapping, Sequence
 from datetime import date, datetime, time, timedelta, timezone
 from decimal import Decimal
 from enum import Enum
@@ -610,14 +611,24 @@
                 return t.__members__[data]  # noqa
         member_type = getattr(t, "_member_type_", None)
         if member_type and member_type != object:
             if type(data) != member_type:
                 data = self(data, member_type)
         return t(data)  # noqa
 
+    @registry.register(io.BytesIO)
+    def to_filelike(self, data, t):
+        if isinstance(data, t):
+            return data
+        if isinstance(data, (bytes, bytearray, memoryview)):
+            return t(data)
+        if self.no_explicit_cast:
+            raise TypeError
+        return t(str(data).encode())
+
     @registry.register(type, allow_subclasses=False)
     def to_type(self, data, t=type) -> type:
         if not isinstance(data, type):
             raise TypeError('data is not a type')
         return data
 
     def handle_unresolved(self, data, t):
```

### Comparing `utype-0.3.1/utype.egg-info/PKG-INFO` & `utype-0.3.2/utype.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utype
-Version: 0.3.1
+Version: 0.3.2
 Summary: Declare & parse types / dataclasses / functions based on Python type annotations
 Home-page: https://utype.io
 Author: XuLin Zhou
 Author-email: zxl@utilmeta.com
 License: Apache 2.0
 Project-URL: Project Home, https://utype.io
 Project-URL: Documentation, https://utype.io
@@ -39,15 +39,15 @@
 [![Test Coverage](https://img.shields.io/codecov/c/github/utilmeta/utype?color=green)](https://app.codecov.io/github/utilmeta/utype)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Downloads](https://pepy.tech/badge/utype/month)](https://pepy.tech/project/utype)
 
 utype is a data types declaration & parsing library based on Python type annotations, 
 enforce types and constraints for classes and functions at runtime
 
-* Version: `0.3.1` [test]
+* Version: `0.3.2` [test]
 * Author: [@voidZXL](https://github.com/voidZXL)
 * License: Apache 2.0
 * Source Code: [https://github.com/utilmeta/utype](https://github.com/utilmeta/utype)
 * Documentation: [https://utype.io](https://utype.io)
 * 中文文档: [https://utype.io/zh](https://utype.io/zh)
```

### Comparing `utype-0.3.1/utype.egg-info/SOURCES.txt` & `utype-0.3.2/utype.egg-info/SOURCES.txt`

 * *Files identical despite different names*

