# Comparing `tmp/katalytic-data-0.9.0.tar.gz` & `tmp/katalytic-data-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katalytic-data-0.9.0.tar", last modified: Sat May  6 03:48:10 2023, max compression
+gzip compressed data, was "katalytic-data-0.9.1.tar", last modified: Sat May 20 16:31:58 2023, max compression
```

## Comparing `katalytic-data-0.9.0.tar` & `katalytic-data-0.9.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       87 2023-04-16 12:25:23.268033 katalytic-data-0.9.0/.coveragerc
--rw-r--r--   0        0        0      651 2023-04-26 18:43:19.705157 katalytic-data-0.9.0/.gitignore
--rw-r--r--   0        0        0     3242 2023-05-05 03:59:46.034609 katalytic-data-0.9.0/.gitlab-ci.yml
--rw-r--r--   0        0        0    13305 2023-05-06 03:48:04.491993 katalytic-data-0.9.0/CHANGELOG.md
--rw-r--r--   0        0        0     1066 2023-04-16 12:25:23.268033 katalytic-data-0.9.0/LICENSE.txt
--rw-r--r--   0        0        0     1836 2023-04-30 14:20:58.779511 katalytic-data-0.9.0/README.md
--rw-r--r--   0        0        0     1236 2023-05-06 03:48:04.467993 katalytic-data-0.9.0/pyproject.toml
--rw-r--r--   0        0        0    27212 2023-05-06 03:37:32.028261 katalytic-data-0.9.0/src/katalytic/data/__init__.py
--rw-r--r--   0        0        0     6192 2023-05-05 10:53:33.309343 katalytic-data-0.9.0/src/katalytic/data/checks.py
--rw-r--r--   0        0        0    17113 2023-05-05 11:04:41.773899 katalytic-data-0.9.0/tests/test_checks.py
--rw-r--r--   0        0        0    49962 2023-05-06 03:38:53.016355 katalytic-data-0.9.0/tests/test_data.py
--rw-r--r--   0        0        0     2928 1970-01-01 00:00:00.000000 katalytic-data-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0       87 2023-04-16 12:25:23.268033 katalytic-data-0.9.1/.coveragerc
+-rw-r--r--   0        0        0      651 2023-04-26 18:43:19.705157 katalytic-data-0.9.1/.gitignore
+-rw-r--r--   0        0        0     3242 2023-05-05 03:59:46.034609 katalytic-data-0.9.1/.gitlab-ci.yml
+-rw-r--r--   0        0        0    13511 2023-05-20 16:31:54.839563 katalytic-data-0.9.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1066 2023-04-16 12:25:23.268033 katalytic-data-0.9.1/LICENSE.txt
+-rw-r--r--   0        0        0     1866 2023-05-14 08:37:30.818379 katalytic-data-0.9.1/README.md
+-rw-r--r--   0        0        0     1236 2023-05-20 16:31:54.839563 katalytic-data-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0    27246 2023-05-20 16:27:22.878218 katalytic-data-0.9.1/src/katalytic/data/__init__.py
+-rw-r--r--   0        0        0     6192 2023-05-05 10:53:33.309343 katalytic-data-0.9.1/src/katalytic/data/checks.py
+-rw-r--r--   0        0        0    17113 2023-05-05 11:04:41.773899 katalytic-data-0.9.1/tests/test_checks.py
+-rw-r--r--   0        0        0    49962 2023-05-20 16:28:10.046455 katalytic-data-0.9.1/tests/test_data.py
+-rw-r--r--   0        0        0     2958 1970-01-01 00:00:00.000000 katalytic-data-0.9.1/PKG-INFO
```

### Comparing `katalytic-data-0.9.0/.gitignore` & `katalytic-data-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.9.0/.gitlab-ci.yml` & `katalytic-data-0.9.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.9.0/CHANGELOG.md` & `katalytic-data-0.9.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+## 0.9.1 (2023-05-20)
+### fix
+- [[`131e3ad`](https://gitlab.com/katalytic/katalytic-data/commit/131e3ad13db07a9e23e33e8d9c66df73a65a95f0)] use `[True, False]` instead of just `False` in the `_types` dict
+
+
 ## 0.9.0 (2023-05-06)
 ### feat
 - [[`1fddfe3`](https://gitlab.com/katalytic/katalytic-data/commit/1fddfe3b1910d55350c004003c808536f4999548)] pop_{min, max}, pop_{min, max}_by_dict_{keys,values}, swap_keys_and_values
 ### fix
 - [[`75403ec`](https://gitlab.com/katalytic/katalytic-data/commit/75403ecb6d65ee217788438530d2ff666dc573cf)] exclude map from all_types_besides('iterables') and correct all_types('dict')
```

### Comparing `katalytic-data-0.9.0/LICENSE.txt` & `katalytic-data-0.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.9.0/README.md` & `katalytic-data-0.9.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# Not fit for public use yet
+
 ## Description
 TODO: Let people know what your project can do specifically. Provide context and add a link to any reference visitors might be unfamiliar with. A list of Features or a Background subsection can also be added here. If there are alternatives to your project, this is a good place to list differentiating factors.
 
 [![version](https://img.shields.io/pypi/v/katalytic-data)](https://pypi.org/project/katalytic-data/)
 [![tests](https://gitlab.com/katalytic/katalytic-data/badges/main/pipeline.svg?key_text=tests&key_width=38)](https://gitlab.com/katalytic/katalytic-data/-/commits/main)
 [![coverage](https://gitlab.com/katalytic/katalytic-data/badges/main/coverage.svg)](https://gitlab.com/katalytic/katalytic-data/-/commits/main)
 [![docs](https://img.shields.io/readthedocs/katalytic-data.svg)](https://katalytic-data.readthedocs.io/en/latest/)
```

### Comparing `katalytic-data-0.9.0/pyproject.toml` & `katalytic-data-0.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "katalytic-data"
-version = "0.9.0"
+version = "0.9.1"
 description = "This plugin adds utilities for working with data to the katalytic namespace"
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
```

### Comparing `katalytic-data-0.9.0/src/katalytic/data/__init__.py` & `katalytic-data-0.9.1/src/katalytic/data/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,25 +29,26 @@
 _lambda = lambda x: x
 _generator_expr = (x for x in [])
 _sequences = [[], (), range(0)]
 _dict_views = [{}.keys(), {}.values(), {}.items()]
 _iterators = [_generator, _generator_expr, iter([]), _map, enumerate([]), zip([], [])]
 _iterables = [*_dict_views, *_iterators, *_sequences, set(), {}]
 _collections = [(), set(), frozenset([]), {}, []]
+_booleans = [True, False]
 _singletons = [None, True, False]
 _primitives = [*_singletons, 0, 0.0, '', b'', bytearray(b'')]
 _callables = [_generator, _function, _lambda, _C_obj, _C]
 _numbers = [0, 0.0, 0j, Decimal('0'), Fraction(0, 1)]
 _objects = [_obj, _C_obj]
 _generators = [_generator, _generator_expr]
 _functions = [_generator, _function, _lambda]
 _strings = ['', b'', bytearray(b'')]
 
 _types = {
-    'bool': False,
+    'booleans': _booleans,
     'bytearray': bytearray(b''),
     'bytes': b'',
     'callables': _callables,
     'callable_obj': _C_obj,
     'class': _C,
     'collections': _collections,
     'complex': 0 + 0j,
```

### Comparing `katalytic-data-0.9.0/src/katalytic/data/checks.py` & `katalytic-data-0.9.1/src/katalytic/data/checks.py`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.9.0/tests/test_checks.py` & `katalytic-data-0.9.1/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.9.0/tests/test_data.py` & `katalytic-data-0.9.1/tests/test_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,23 +78,23 @@
     def test_unexpected(self, unexpected):
         with pytest.raises(ValueError):
             all_types_besides(unexpected)
 
     @pytest.mark.parametrize('blacklist, expected', [
         (
             ['iterables'],
-            [False, bytearray(b''), b'', _function, _lambda, _C_obj, _C, 0j, Decimal('0'), 0.0, Fraction(0, 1), 0, None, _obj, PosixPath('.'), True, '']
+            [True, False, bytearray(b''), b'', _function, _lambda, _C_obj, _C, 0j, Decimal('0'), 0.0, Fraction(0, 1), 0, None, _obj, PosixPath('.'), '']
         ),
         (
             'iterables',
-            [False, bytearray(b''), b'', _function, _lambda, _C_obj, _C, 0j, Decimal('0'), 0.0, Fraction(0, 1), 0, None, _obj, PosixPath('.'), True, '']
+            [True, False, bytearray(b''), b'', _function, _lambda, _C_obj, _C, 0j, Decimal('0'), 0.0, Fraction(0, 1), 0, None, _obj, PosixPath('.'), '']
         ),
         (
             ['iterables', 'generators', 'functions', 'objects', 'path'],
-            [False, bytearray(b''), b'', _C, 0j, Decimal('0'), 0.0, Fraction(0, 1), 0, None, True, '']
+            [True, False, bytearray(b''), b'', _C, 0j, Decimal('0'), 0.0, Fraction(0, 1), 0, None, '']
         ),
     ])
     def test_all_types_besides(self, blacklist, expected):
         assert all_types_besides(blacklist) == expected
 
 
 class Test_as_dict_of_lists:
```

### Comparing `katalytic-data-0.9.0/PKG-INFO` & `katalytic-data-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katalytic-data
-Version: 0.9.0
+Version: 0.9.1
 Summary: This plugin adds utilities for working with data to the katalytic namespace
 Keywords: high-level,data conversion
 Author-email: Valentin Neagu <vali19th@protonmail.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -20,14 +20,16 @@
 Requires-Dist: pytest-cov ; extra == "dev"
 Requires-Dist: pytest-clarity ; extra == "dev"
 Requires-Dist: pytest-randomly ; extra == "dev"
 Project-URL: homepage, https://gitlab.com/katalytic/katalytic-data.git
 Project-URL: repository, https://gitlab.com/katalytic/katalytic-data.git
 Provides-Extra: dev
 
+# Not fit for public use yet
+
 ## Description
 TODO: Let people know what your project can do specifically. Provide context and add a link to any reference visitors might be unfamiliar with. A list of Features or a Background subsection can also be added here. If there are alternatives to your project, this is a good place to list differentiating factors.
 
 [![version](https://img.shields.io/pypi/v/katalytic-data)](https://pypi.org/project/katalytic-data/)
 [![tests](https://gitlab.com/katalytic/katalytic-data/badges/main/pipeline.svg?key_text=tests&key_width=38)](https://gitlab.com/katalytic/katalytic-data/-/commits/main)
 [![coverage](https://gitlab.com/katalytic/katalytic-data/badges/main/coverage.svg)](https://gitlab.com/katalytic/katalytic-data/-/commits/main)
 [![docs](https://img.shields.io/readthedocs/katalytic-data.svg)](https://katalytic-data.readthedocs.io/en/latest/)
```

