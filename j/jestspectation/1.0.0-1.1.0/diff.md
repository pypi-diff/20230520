# Comparing `tmp/jestspectation-1.0.0.tar.gz` & `tmp/jestspectation-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jestspectation-1.0.0.tar", max compression
+gzip compressed data, was "jestspectation-1.1.0.tar", max compression
```

## Comparing `jestspectation-1.0.0.tar` & `jestspectation-1.1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1073 2023-04-22 18:13:30.788580 jestspectation-1.0.0/LICENSE
--rw-r--r--   0        0        0     1421 2023-04-22 18:13:30.788580 jestspectation-1.0.0/README.md
--rw-r--r--   0        0        0     1455 2023-04-22 18:13:30.788580 jestspectation-1.0.0/jestspectation/__any.py
--rw-r--r--   0        0        0      609 2023-04-22 18:13:30.788580 jestspectation-1.0.0/jestspectation/__config/__config.py
--rw-r--r--   0        0        0      105 2023-04-22 18:13:30.788580 jestspectation-1.0.0/jestspectation/__config/__init__.py
--rw-r--r--   0        0        0    10767 2023-04-22 18:13:30.788580 jestspectation-1.0.0/jestspectation/__containers.py
--rw-r--r--   0        0        0     2451 2023-04-22 18:13:30.788580 jestspectation-1.0.0/jestspectation/__equals.py
--rw-r--r--   0        0        0     3613 2023-04-22 18:13:30.788580 jestspectation-1.0.0/jestspectation/__float_approx.py
--rw-r--r--   0        0        0      993 2023-04-22 18:13:30.788580 jestspectation-1.0.0/jestspectation/__init__.py
--rw-r--r--   0        0        0     2610 2023-04-22 18:13:30.788580 jestspectation-1.0.0/jestspectation/__jestspectation_base.py
--rw-r--r--   0        0        0     2861 2023-04-22 18:13:30.788580 jestspectation-1.0.0/jestspectation/__py_diffs.py
--rw-r--r--   0        0        0     1304 2023-04-22 18:13:30.788580 jestspectation-1.0.0/jestspectation/__strings/__containing.py
--rw-r--r--   0        0        0      292 2023-04-22 18:13:30.788580 jestspectation-1.0.0/jestspectation/__strings/__init__.py
--rw-r--r--   0        0        0     4741 2023-04-22 18:13:30.788580 jestspectation-1.0.0/jestspectation/__strings/__lines_like.py
--rw-r--r--   0        0        0     1360 2023-04-22 18:13:30.788580 jestspectation-1.0.0/jestspectation/__strings/__matching_regex.py
--rw-r--r--   0        0        0     2547 2023-04-22 18:13:30.788580 jestspectation-1.0.0/jestspectation/__strings/__text_like.py
--rw-r--r--   0        0        0     3699 2023-04-22 18:13:30.788580 jestspectation-1.0.0/jestspectation/__util.py
--rw-r--r--   0        0        0     1670 2023-04-22 18:13:30.788580 jestspectation-1.0.0/jestspectation/logicals/__and.py
--rw-r--r--   0        0        0      242 2023-04-22 18:13:30.788580 jestspectation-1.0.0/jestspectation/logicals/__init__.py
--rw-r--r--   0        0        0     1279 2023-04-22 18:13:30.788580 jestspectation-1.0.0/jestspectation/logicals/__not.py
--rw-r--r--   0        0        0     1612 2023-04-22 18:13:30.788580 jestspectation-1.0.0/jestspectation/logicals/__or.py
--rw-r--r--   0        0        0     2162 2023-04-22 18:13:30.788580 jestspectation-1.0.0/jestspectation/logicals/__xor.py
--rw-r--r--   0        0        0        0 2023-04-22 18:13:30.788580 jestspectation-1.0.0/jestspectation/py.typed
--rw-r--r--   0        0        0      719 2023-04-22 18:13:30.788580 jestspectation-1.0.0/jestspectation/pytest.py
--rw-r--r--   0        0        0     1408 2023-04-22 18:13:30.788580 jestspectation-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2741 1970-01-01 00:00:00.000000 jestspectation-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-20 15:47:56.860653 jestspectation-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1421 2023-05-20 15:47:56.860653 jestspectation-1.1.0/README.md
+-rw-r--r--   0        0        0     1455 2023-05-20 15:47:56.860653 jestspectation-1.1.0/jestspectation/__any.py
+-rw-r--r--   0        0        0      609 2023-05-20 15:47:56.860653 jestspectation-1.1.0/jestspectation/__config/__config.py
+-rw-r--r--   0        0        0      105 2023-05-20 15:47:56.860653 jestspectation-1.1.0/jestspectation/__config/__init__.py
+-rw-r--r--   0        0        0    14203 2023-05-20 15:47:56.860653 jestspectation-1.1.0/jestspectation/__containers.py
+-rw-r--r--   0        0        0     2451 2023-05-20 15:47:56.860653 jestspectation-1.1.0/jestspectation/__equals.py
+-rw-r--r--   0        0        0     3613 2023-05-20 15:47:56.860653 jestspectation-1.1.0/jestspectation/__float_approx.py
+-rw-r--r--   0        0        0     1115 2023-05-20 15:47:56.860653 jestspectation-1.1.0/jestspectation/__init__.py
+-rw-r--r--   0        0        0     2610 2023-05-20 15:47:56.860653 jestspectation-1.1.0/jestspectation/__jestspectation_base.py
+-rw-r--r--   0        0        0     2861 2023-05-20 15:47:56.860653 jestspectation-1.1.0/jestspectation/__py_diffs.py
+-rw-r--r--   0        0        0     1304 2023-05-20 15:47:56.860653 jestspectation-1.1.0/jestspectation/__strings/__containing.py
+-rw-r--r--   0        0        0      292 2023-05-20 15:47:56.860653 jestspectation-1.1.0/jestspectation/__strings/__init__.py
+-rw-r--r--   0        0        0     4741 2023-05-20 15:47:56.860653 jestspectation-1.1.0/jestspectation/__strings/__lines_like.py
+-rw-r--r--   0        0        0     1360 2023-05-20 15:47:56.860653 jestspectation-1.1.0/jestspectation/__strings/__matching_regex.py
+-rw-r--r--   0        0        0     2547 2023-05-20 15:47:56.860653 jestspectation-1.1.0/jestspectation/__strings/__text_like.py
+-rw-r--r--   0        0        0     3699 2023-05-20 15:47:56.860653 jestspectation-1.1.0/jestspectation/__util.py
+-rw-r--r--   0        0        0     1670 2023-05-20 15:47:56.860653 jestspectation-1.1.0/jestspectation/logicals/__and.py
+-rw-r--r--   0        0        0      242 2023-05-20 15:47:56.860653 jestspectation-1.1.0/jestspectation/logicals/__init__.py
+-rw-r--r--   0        0        0     1279 2023-05-20 15:47:56.864653 jestspectation-1.1.0/jestspectation/logicals/__not.py
+-rw-r--r--   0        0        0     1612 2023-05-20 15:47:56.864653 jestspectation-1.1.0/jestspectation/logicals/__or.py
+-rw-r--r--   0        0        0     2162 2023-05-20 15:47:56.864653 jestspectation-1.1.0/jestspectation/logicals/__xor.py
+-rw-r--r--   0        0        0        0 2023-05-20 15:47:56.864653 jestspectation-1.1.0/jestspectation/py.typed
+-rw-r--r--   0        0        0      719 2023-05-20 15:47:56.864653 jestspectation-1.1.0/jestspectation/pytest.py
+-rw-r--r--   0        0        0     1479 2023-05-20 15:47:56.864653 jestspectation-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2774 1970-01-01 00:00:00.000000 jestspectation-1.1.0/PKG-INFO
```

### Comparing `jestspectation-1.0.0/LICENSE` & `jestspectation-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jestspectation-1.0.0/README.md` & `jestspectation-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `jestspectation-1.0.0/jestspectation/__any.py` & `jestspectation-1.1.0/jestspectation/__any.py`

 * *Files identical despite different names*

### Comparing `jestspectation-1.0.0/jestspectation/__config/__config.py` & `jestspectation-1.1.0/jestspectation/__config/__config.py`

 * *Files identical despite different names*

### Comparing `jestspectation-1.0.0/jestspectation/__containers.py` & `jestspectation-1.1.0/jestspectation/__containers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Matchers for specific container types
 """
 
 from abc import abstractmethod
 from collections.abc import Iterable, ItemsView
-from typing import TypeVar, Generic
+from typing import Any, TypeVar, Generic, cast
 from typing_extensions import TypeGuard
 from .__jestspectation_base import JestspectationBase
 from .__util import get_object_type_name, safe_diff_wrapper, sub_diff_delegate
 
 
 T = TypeVar('T', bound=Iterable)
 
@@ -242,14 +242,50 @@
     def _get_items(self) -> set:
         return self.__keys
 
     def _is_present(self, item: object, other: set) -> bool:
         return item in other
 
 
+class ObjectContainingProperties(JestspectationContainer):
+    """
+    Matches any object containing all the given properties. Note that this does
+    not check property values - just the presence of those properties.
+    """
+
+    def __init__(self, properties: set[str]) -> None:
+        """
+        Matches any object containing all the given properties. Note that this
+        does not check property values - just the presence of those properties.
+
+        Args:
+            properties (set): set of properties to match
+        """
+        self.__properties = properties
+
+    def get_contents_repr(self) -> list[str]:
+        return sorted(self.__properties)
+
+    def get_contents_repr_edges(self) -> tuple[str, str]:
+        return '', ''
+
+    @staticmethod
+    def _get_allowed_types() -> tuple[type, ...]:
+        return (object,)
+
+    def _get_items(self) -> list[str]:
+        return sorted(self.__properties)
+
+    def _is_present(self, item: object, other: set) -> bool:
+        return item in dir(other)
+
+    def _format_missing_item(self, item: object) -> str:
+        return cast(str, item)
+
+
 class DictContainingValues(JestspectationContainer):
     """
     Matches any dictionary containing all the given values
     """
 
     def __init__(self, values: list) -> None:
         """
@@ -338,14 +374,86 @@
         return [eq_expr] + diff
 
     def _format_missing_item(self, item: object) -> str:
         # Format like dict keys
         return f"{repr(item[0])}: {repr(item[1])}"  # type: ignore
 
 
+class ObjectContainingItems(JestspectationContainer):
+    """
+    Matches any object containing all the given items, where an item is a
+    property-value pair.
+    """
+
+    def __init__(self, items: dict[str, Any]) -> None:
+        """
+        Matches any object containing all the given items, where an item is a
+        property-value pair.
+
+        Args:
+            items (dict): dict of items to match
+        """
+        self.__items = items
+
+    def __repr__(self) -> str:
+        inners = []
+        for property, value in self.__items.items():
+            inners.append(f"{property} = {value}")
+
+        return f"ObjectContainingItems({', '.join(inners)})"
+
+    def get_contents_repr(self) -> list[str]:
+        return [f"{repr(i[0])} == {repr(i[1])}" for i in self.__items.items()]
+
+    def get_contents_repr_edges(self) -> tuple[str, str]:
+        return '', ''
+
+    @staticmethod
+    def _get_allowed_types() -> tuple[type, ...]:
+        return (object,)
+
+    def _get_items(self) -> ItemsView:
+        return self.__items.items()
+
+    def _is_present(self, item: object, other: object) -> bool:
+        # TODO: Use generics to make this type-safe
+        return item[0] in dir(other)  # type: ignore
+
+    def _is_correct(self, item: object, other: object) -> bool:
+        return getattr(other, item[0]) == item[1]  # type: ignore
+
+    def _format_sub_diff(
+        self,
+        item: object,
+        other: ItemsView,
+        other_is_lhs: bool,
+    ) -> list[str]:
+        # Lots of type: ignores here because I can't figure out how to make
+        # this type-safe :(
+        # Just need to get good test coverage
+        other_value = getattr(other, item[0])  # type: ignore
+        diff = sub_diff_delegate(
+            item[1],  # type: ignore
+            other_value,
+            other_is_lhs,
+        )
+        assert diff is not None
+        self_repr = self._format_missing_item(item)
+        other_repr = f"{item[0]} = {repr(other_value)}"  # type: ignore
+        if other_is_lhs:
+            eq_expr = f"   {other_repr} == {self_repr}"
+        else:
+            eq_expr = f"   {self_repr} == {other_repr}"
+        return [eq_expr] + diff
+
+    def _format_missing_item(self, item: object) -> str:
+        # Format like dict keys
+        return f"{item[0]} = {repr(item[1])}"  # type: ignore
+
+
 class ListOfLength(JestspectationBase):
     """
     Matches any list of the given length
     """
 
     def __init__(self, length: int) -> None:
         if length < 0:
```

### Comparing `jestspectation-1.0.0/jestspectation/__equals.py` & `jestspectation-1.1.0/jestspectation/__equals.py`

 * *Files identical despite different names*

### Comparing `jestspectation-1.0.0/jestspectation/__float_approx.py` & `jestspectation-1.1.0/jestspectation/__float_approx.py`

 * *Files identical despite different names*

### Comparing `jestspectation-1.0.0/jestspectation/__init__.py` & `jestspectation-1.1.0/jestspectation/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,16 +8,18 @@
 
 from .__any import Any, Anything
 from .__containers import (
     DictContainingKeys,
     DictContainingValues,
     DictContainingItems,
     ListContaining,
-    SetContaining,
     ListOfLength,
+    SetContaining,
+    ObjectContainingProperties,
+    ObjectContainingItems,
 )
 from .__float_approx import FloatApprox
 from .__equals import Equals, Is
 from .logicals import And, Not, Or, Xor
 from .__strings import (
     StringMatchingRegex,
     StringContaining,
@@ -38,14 +40,16 @@
     'Equals',
     'FloatApprox',
     'Is',
     'LinesLike',
     'ListContaining',
     'ListOfLength',
     'Not',
+    'ObjectContainingProperties',
+    'ObjectContainingItems',
     'Or',
     'SetContaining',
     'StringContaining',
     'StringMatchingRegex',
     'TextLike',
     'Xor',
 ]
```

### Comparing `jestspectation-1.0.0/jestspectation/__jestspectation_base.py` & `jestspectation-1.1.0/jestspectation/__jestspectation_base.py`

 * *Files identical despite different names*

### Comparing `jestspectation-1.0.0/jestspectation/__py_diffs.py` & `jestspectation-1.1.0/jestspectation/__py_diffs.py`

 * *Files identical despite different names*

### Comparing `jestspectation-1.0.0/jestspectation/__strings/__containing.py` & `jestspectation-1.1.0/jestspectation/__strings/__containing.py`

 * *Files identical despite different names*

### Comparing `jestspectation-1.0.0/jestspectation/__strings/__lines_like.py` & `jestspectation-1.1.0/jestspectation/__strings/__lines_like.py`

 * *Files identical despite different names*

### Comparing `jestspectation-1.0.0/jestspectation/__strings/__matching_regex.py` & `jestspectation-1.1.0/jestspectation/__strings/__matching_regex.py`

 * *Files identical despite different names*

### Comparing `jestspectation-1.0.0/jestspectation/__strings/__text_like.py` & `jestspectation-1.1.0/jestspectation/__strings/__text_like.py`

 * *Files identical despite different names*

### Comparing `jestspectation-1.0.0/jestspectation/__util.py` & `jestspectation-1.1.0/jestspectation/__util.py`

 * *Files identical despite different names*

### Comparing `jestspectation-1.0.0/jestspectation/logicals/__and.py` & `jestspectation-1.1.0/jestspectation/logicals/__and.py`

 * *Files identical despite different names*

### Comparing `jestspectation-1.0.0/jestspectation/logicals/__not.py` & `jestspectation-1.1.0/jestspectation/logicals/__not.py`

 * *Files identical despite different names*

### Comparing `jestspectation-1.0.0/jestspectation/logicals/__or.py` & `jestspectation-1.1.0/jestspectation/logicals/__or.py`

 * *Files identical despite different names*

### Comparing `jestspectation-1.0.0/jestspectation/logicals/__xor.py` & `jestspectation-1.1.0/jestspectation/logicals/__xor.py`

 * *Files identical despite different names*

### Comparing `jestspectation-1.0.0/jestspectation/pytest.py` & `jestspectation-1.1.0/jestspectation/pytest.py`

 * *Files 17% similar despite different names*

```diff
@@ -21,10 +21,10 @@
     """
     if op == "==":
         if isinstance(right, JestspectationBase):
             return right.get_diff(left, True)
         elif isinstance(left, JestspectationBase):
             return left.get_diff(right, False)
         elif configure().pytest_all_diffs:
-            return Equals(left).get_diff(right, False)
+            return Equals(right).get_diff(left, False)
 
     return None
```

### Comparing `jestspectation-1.0.0/pyproject.toml` & `jestspectation-1.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Jestspectation"
-version = "1.0.0"
+version = "1.1.0"
 description = "Pattern matching helper classes designed to allow for testing of complex data structures in a readable and logical format"
 readme = "README.md"
 
 authors = ["Miguel Guthridge <hdsq@outlook.com.au>"]
 license = "MIT"
 
 repository = "https://github.com/MiguelGuthridge/Jestspectation"
@@ -21,14 +21,16 @@
     "Programming Language :: Python :: 3",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Development Status :: 4 - Beta",
     "Environment :: Other Environment",
     "Framework :: Pytest",
+    "Topic :: Software Development :: Testing",
+    "Typing :: Typed",
 ]
 include = ["py.typed"]
 
 packages = [
     { include = "jestspectation" }
 ]
 
@@ -40,16 +42,16 @@
 "Bug Tracker" = "https://github.com/MiguelGuthridge/Jestspectation/issues"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 typing-extensions = "^4.5.0"
 
 [tool.poetry.dev-dependencies]
-mypy = "^1.2.0"
+mypy = "^1.3.0"
 flake8 = "^6.0.0"
 pytest = "^7.3.1"
 autopep8 = "^2.0.2"
-coverage = "^7.2.3"
+coverage = "^7.2.5"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `jestspectation-1.0.0/PKG-INFO` & `jestspectation-1.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jestspectation
-Version: 1.0.0
+Version: 1.1.0
 Summary: Pattern matching helper classes designed to allow for testing of complex data structures in a readable and logical format
 Home-page: https://github.com/MiguelGuthridge/Jestspectation
 License: MIT
 Keywords: jest,pattern,matching,pytest,equality
 Author: Miguel Guthridge
 Author-email: hdsq@outlook.com.au
 Requires-Python: >=3.9,<4.0
@@ -14,15 +14,16 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development :: Testing
+Classifier: Typing :: Typed
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
 Project-URL: Bug Tracker, https://github.com/MiguelGuthridge/Jestspectation/issues
 Project-URL: Documentation, https://miguelguthridge.github.io/Jestspectation
 Project-URL: Online Documentation, https://github.com/MiguelGuthridge/Jestspectation
 Project-URL: Repository, https://github.com/MiguelGuthridge/Jestspectation
 Description-Content-Type: text/markdown
```

