# Comparing `tmp/lark_dynamic-1.1.3.tar.gz` & `tmp/lark_dynamic-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lark_dynamic-1.1.3.tar", max compression
+gzip compressed data, was "lark_dynamic-1.1.4.tar", max compression
```

## Comparing `lark_dynamic-1.1.3.tar` & `lark_dynamic-1.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1068 2023-05-16 16:54:07.903637 lark_dynamic-1.1.3/LICENSE
--rw-r--r--   0        0        0    12179 2023-05-16 16:54:07.903637 lark_dynamic-1.1.3/README.md
--rw-r--r--   0        0        0      808 2023-05-16 16:54:07.903637 lark_dynamic-1.1.3/lark_dynamic/__init__.py
--rw-r--r--   0        0        0     3471 2023-05-16 16:54:07.903637 lark_dynamic-1.1.3/lark_dynamic/atoms.py
--rw-r--r--   0        0        0     3340 2023-05-16 16:54:07.903637 lark_dynamic-1.1.3/lark_dynamic/combinators.py
--rw-r--r--   0        0        0       60 2023-05-16 16:54:07.903637 lark_dynamic-1.1.3/lark_dynamic/constants.py
--rw-r--r--   0        0        0     3085 2023-05-16 16:54:07.903637 lark_dynamic-1.1.3/lark_dynamic/definitions.py
--rw-r--r--   0        0        0     6217 2023-05-16 16:54:07.903637 lark_dynamic-1.1.3/lark_dynamic/grammar.py
--rw-r--r--   0        0        0      578 2023-05-16 16:54:07.903637 lark_dynamic-1.1.3/lark_dynamic/modifier.py
--rw-r--r--   0        0        0        0 2023-05-16 16:54:07.903637 lark_dynamic-1.1.3/lark_dynamic/py.typed
--rw-r--r--   0        0        0     1382 2023-05-16 16:54:07.903637 lark_dynamic-1.1.3/lark_dynamic/token.py
--rw-r--r--   0        0        0     1226 2023-05-16 16:54:07.903637 lark_dynamic-1.1.3/lark_dynamic/utils.py
--rw-r--r--   0        0        0      913 2023-05-16 16:54:07.903637 lark_dynamic-1.1.3/lark_dynamic/variable.py
--rw-r--r--   0        0        0      425 2023-05-16 16:54:07.903637 lark_dynamic-1.1.3/pyproject.toml
--rw-r--r--   0        0        0    12776 1970-01-01 00:00:00.000000 lark_dynamic-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-05-20 02:24:30.055374 lark_dynamic-1.1.4/LICENSE
+-rw-r--r--   0        0        0    12179 2023-05-20 02:24:30.055374 lark_dynamic-1.1.4/README.md
+-rw-r--r--   0        0        0      808 2023-05-20 02:24:30.055374 lark_dynamic-1.1.4/lark_dynamic/__init__.py
+-rw-r--r--   0        0        0     3471 2023-05-20 02:24:30.055374 lark_dynamic-1.1.4/lark_dynamic/atoms.py
+-rw-r--r--   0        0        0     3340 2023-05-20 02:24:30.055374 lark_dynamic-1.1.4/lark_dynamic/combinators.py
+-rw-r--r--   0        0        0       60 2023-05-20 02:24:30.055374 lark_dynamic-1.1.4/lark_dynamic/constants.py
+-rw-r--r--   0        0        0     3085 2023-05-20 02:24:30.055374 lark_dynamic-1.1.4/lark_dynamic/definitions.py
+-rw-r--r--   0        0        0     6217 2023-05-20 02:24:30.055374 lark_dynamic-1.1.4/lark_dynamic/grammar.py
+-rw-r--r--   0        0        0      578 2023-05-20 02:24:30.055374 lark_dynamic-1.1.4/lark_dynamic/modifier.py
+-rw-r--r--   0        0        0        0 2023-05-20 02:24:30.055374 lark_dynamic-1.1.4/lark_dynamic/py.typed
+-rw-r--r--   0        0        0     1362 2023-05-20 02:24:30.055374 lark_dynamic-1.1.4/lark_dynamic/token.py
+-rw-r--r--   0        0        0     1226 2023-05-20 02:24:30.055374 lark_dynamic-1.1.4/lark_dynamic/utils.py
+-rw-r--r--   0        0        0      913 2023-05-20 02:24:30.055374 lark_dynamic-1.1.4/lark_dynamic/variable.py
+-rw-r--r--   0        0        0      425 2023-05-20 02:24:30.055374 lark_dynamic-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0    12776 1970-01-01 00:00:00.000000 lark_dynamic-1.1.4/PKG-INFO
```

### Comparing `lark_dynamic-1.1.3/LICENSE` & `lark_dynamic-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lark_dynamic-1.1.3/README.md` & `lark_dynamic-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `lark_dynamic-1.1.3/lark_dynamic/__init__.py` & `lark_dynamic-1.1.4/lark_dynamic/__init__.py`

 * *Files identical despite different names*

### Comparing `lark_dynamic-1.1.3/lark_dynamic/atoms.py` & `lark_dynamic-1.1.4/lark_dynamic/atoms.py`

 * *Files identical despite different names*

### Comparing `lark_dynamic-1.1.3/lark_dynamic/combinators.py` & `lark_dynamic-1.1.4/lark_dynamic/combinators.py`

 * *Files identical despite different names*

### Comparing `lark_dynamic-1.1.3/lark_dynamic/definitions.py` & `lark_dynamic-1.1.4/lark_dynamic/definitions.py`

 * *Files identical despite different names*

### Comparing `lark_dynamic-1.1.3/lark_dynamic/grammar.py` & `lark_dynamic-1.1.4/lark_dynamic/grammar.py`

 * *Files identical despite different names*

### Comparing `lark_dynamic-1.1.3/lark_dynamic/modifier.py` & `lark_dynamic-1.1.4/lark_dynamic/modifier.py`

 * *Files identical despite different names*

### Comparing `lark_dynamic-1.1.3/lark_dynamic/token.py` & `lark_dynamic-1.1.4/lark_dynamic/token.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     @staticmethod
     def render_str(token: Renderable, context: ContextType) -> Iterable[str]:
         if isinstance(token, tuple):
             yield from Group(*token).render(context)
         elif isinstance(token, list):
             yield from Optional(*token).render(context)
         elif isinstance(token, str):
-            str_escaped = str_encoder(token.replace('"', '\\"'))[0].decode("utf-8")
+            str_escaped = str_encoder(token)[0].decode("utf-8")
 
             yield '"'
             yield str_escaped
             yield '"'
         else:
             yield from token.render(context)
```

### Comparing `lark_dynamic-1.1.3/lark_dynamic/utils.py` & `lark_dynamic-1.1.4/lark_dynamic/utils.py`

 * *Files identical despite different names*

### Comparing `lark_dynamic-1.1.3/lark_dynamic/variable.py` & `lark_dynamic-1.1.4/lark_dynamic/variable.py`

 * *Files identical despite different names*

### Comparing `lark_dynamic-1.1.3/PKG-INFO` & `lark_dynamic-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lark-dynamic
-Version: 1.1.3
+Version: 1.1.4
 Summary: Grammar generator for Lark parsing toolkit
 License: MIT
 Author: Dmitry Gritsenko
 Author-email: k01419q45@ya.ru
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

