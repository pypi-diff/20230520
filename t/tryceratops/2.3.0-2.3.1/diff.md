# Comparing `tmp/tryceratops-2.3.0.tar.gz` & `tmp/tryceratops-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tryceratops-2.3.0.tar", max compression
+gzip compressed data, was "tryceratops-2.3.1.tar", max compression
```

## Comparing `tryceratops-2.3.0.tar` & `tryceratops-2.3.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1084 2023-05-20 11:15:32.105742 tryceratops-2.3.0/LICENSE
--rw-r--r--   0        0        0     6243 2023-05-20 11:16:05.812017 tryceratops-2.3.0/README.md
--rw-r--r--   0        0        0     2243 2023-05-20 11:16:05.868020 tryceratops-2.3.0/pyproject.toml
--rw-r--r--   0        0        0       69 2023-05-20 11:16:05.812017 tryceratops-2.3.0/src/tryceratops/__init__.py
--rw-r--r--   0        0        0     2227 2023-05-20 11:15:32.109743 tryceratops-2.3.0/src/tryceratops/__main__.py
--rw-r--r--   0        0        0     1185 2023-05-20 11:15:32.109743 tryceratops-2.3.0/src/tryceratops/analyzers/__init__.py
--rw-r--r--   0        0        0     1865 2023-05-20 11:15:32.109743 tryceratops-2.3.0/src/tryceratops/analyzers/base.py
--rw-r--r--   0        0        0     5624 2023-05-20 11:15:32.109743 tryceratops-2.3.0/src/tryceratops/analyzers/call.py
--rw-r--r--   0        0        0     2398 2023-05-20 11:15:32.109743 tryceratops-2.3.0/src/tryceratops/analyzers/classdefs.py
--rw-r--r--   0        0        0     2154 2023-05-20 11:15:32.109743 tryceratops-2.3.0/src/tryceratops/analyzers/conditional.py
--rw-r--r--   0        0        0     6385 2023-05-20 11:15:32.109743 tryceratops-2.3.0/src/tryceratops/analyzers/exception_block.py
--rw-r--r--   0        0        0      350 2023-05-20 11:15:32.109743 tryceratops-2.3.0/src/tryceratops/analyzers/exceptions.py
--rw-r--r--   0        0        0     1192 2023-05-20 11:15:32.109743 tryceratops-2.3.0/src/tryceratops/analyzers/try_block.py
--rw-r--r--   0        0        0       50 2023-05-20 11:15:32.109743 tryceratops-2.3.0/src/tryceratops/files/__init__.py
--rw-r--r--   0        0        0     3618 2023-05-20 11:15:32.109743 tryceratops-2.3.0/src/tryceratops/files/discovery.py
--rw-r--r--   0        0        0     1455 2023-05-20 11:15:32.109743 tryceratops-2.3.0/src/tryceratops/files/parser.py
--rw-r--r--   0        0        0      602 2023-05-20 11:15:32.109743 tryceratops-2.3.0/src/tryceratops/fixers/__init__.py
--rw-r--r--   0        0        0     2713 2023-05-20 11:15:32.113743 tryceratops-2.3.0/src/tryceratops/fixers/base.py
--rw-r--r--   0        0        0     2772 2023-05-20 11:15:32.113743 tryceratops-2.3.0/src/tryceratops/fixers/exception_block.py
--rw-r--r--   0        0        0      361 2023-05-20 11:15:32.113743 tryceratops-2.3.0/src/tryceratops/fixers/exceptions.py
--rw-r--r--   0        0        0     2130 2023-05-20 11:15:32.113743 tryceratops-2.3.0/src/tryceratops/flake_plugin.py
--rw-r--r--   0        0        0     2729 2023-05-20 11:15:32.113743 tryceratops-2.3.0/src/tryceratops/interfaces.py
--rw-r--r--   0        0        0     1065 2023-05-20 11:15:32.113743 tryceratops-2.3.0/src/tryceratops/logging_config.py
--rw-r--r--   0        0        0      165 2023-05-20 11:15:32.113743 tryceratops-2.3.0/src/tryceratops/processors.py
--rw-r--r--   0        0        0     3039 2023-05-20 11:15:32.113743 tryceratops-2.3.0/src/tryceratops/runners.py
--rw-r--r--   0        0        0     3629 2023-05-20 11:15:32.113743 tryceratops-2.3.0/src/tryceratops/settings.py
--rw-r--r--   0        0        0      791 2023-05-20 11:15:32.113743 tryceratops-2.3.0/src/tryceratops/types.py
--rw-r--r--   0        0        0      108 2023-05-20 11:15:32.113743 tryceratops-2.3.0/src/tryceratops/violations/__init__.py
--rw-r--r--   0        0        0     1745 2023-05-20 11:15:32.113743 tryceratops-2.3.0/src/tryceratops/violations/codes.py
--rw-r--r--   0        0        0     2403 2023-05-20 11:15:32.113743 tryceratops-2.3.0/src/tryceratops/violations/violations.py
--rw-r--r--   0        0        0     7443 1970-01-01 00:00:00.000000 tryceratops-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-05-20 14:58:46.889732 tryceratops-2.3.1/LICENSE
+-rw-r--r--   0        0        0     6243 2023-05-20 14:59:24.646022 tryceratops-2.3.1/README.md
+-rw-r--r--   0        0        0     2243 2023-05-20 14:59:24.714022 tryceratops-2.3.1/pyproject.toml
+-rw-r--r--   0        0        0       69 2023-05-20 14:59:24.642022 tryceratops-2.3.1/src/tryceratops/__init__.py
+-rw-r--r--   0        0        0     2227 2023-05-20 14:58:46.893733 tryceratops-2.3.1/src/tryceratops/__main__.py
+-rw-r--r--   0        0        0     1185 2023-05-20 14:58:46.893733 tryceratops-2.3.1/src/tryceratops/analyzers/__init__.py
+-rw-r--r--   0        0        0     1865 2023-05-20 14:58:46.893733 tryceratops-2.3.1/src/tryceratops/analyzers/base.py
+-rw-r--r--   0        0        0     5624 2023-05-20 14:58:46.893733 tryceratops-2.3.1/src/tryceratops/analyzers/call.py
+-rw-r--r--   0        0        0     2492 2023-05-20 14:58:46.893733 tryceratops-2.3.1/src/tryceratops/analyzers/classdefs.py
+-rw-r--r--   0        0        0     2154 2023-05-20 14:58:46.893733 tryceratops-2.3.1/src/tryceratops/analyzers/conditional.py
+-rw-r--r--   0        0        0     6385 2023-05-20 14:58:46.893733 tryceratops-2.3.1/src/tryceratops/analyzers/exception_block.py
+-rw-r--r--   0        0        0      350 2023-05-20 14:58:46.893733 tryceratops-2.3.1/src/tryceratops/analyzers/exceptions.py
+-rw-r--r--   0        0        0     1192 2023-05-20 14:58:46.893733 tryceratops-2.3.1/src/tryceratops/analyzers/try_block.py
+-rw-r--r--   0        0        0       50 2023-05-20 14:58:46.893733 tryceratops-2.3.1/src/tryceratops/files/__init__.py
+-rw-r--r--   0        0        0     3618 2023-05-20 14:58:46.893733 tryceratops-2.3.1/src/tryceratops/files/discovery.py
+-rw-r--r--   0        0        0     1455 2023-05-20 14:58:46.893733 tryceratops-2.3.1/src/tryceratops/files/parser.py
+-rw-r--r--   0        0        0      602 2023-05-20 14:58:46.893733 tryceratops-2.3.1/src/tryceratops/fixers/__init__.py
+-rw-r--r--   0        0        0     2713 2023-05-20 14:58:46.893733 tryceratops-2.3.1/src/tryceratops/fixers/base.py
+-rw-r--r--   0        0        0     2772 2023-05-20 14:58:46.893733 tryceratops-2.3.1/src/tryceratops/fixers/exception_block.py
+-rw-r--r--   0        0        0      361 2023-05-20 14:58:46.893733 tryceratops-2.3.1/src/tryceratops/fixers/exceptions.py
+-rw-r--r--   0        0        0     2130 2023-05-20 14:58:46.893733 tryceratops-2.3.1/src/tryceratops/flake_plugin.py
+-rw-r--r--   0        0        0     2729 2023-05-20 14:58:46.897733 tryceratops-2.3.1/src/tryceratops/interfaces.py
+-rw-r--r--   0        0        0     1065 2023-05-20 14:58:46.897733 tryceratops-2.3.1/src/tryceratops/logging_config.py
+-rw-r--r--   0        0        0      165 2023-05-20 14:58:46.897733 tryceratops-2.3.1/src/tryceratops/processors.py
+-rw-r--r--   0        0        0     3039 2023-05-20 14:58:46.897733 tryceratops-2.3.1/src/tryceratops/runners.py
+-rw-r--r--   0        0        0     3629 2023-05-20 14:58:46.897733 tryceratops-2.3.1/src/tryceratops/settings.py
+-rw-r--r--   0        0        0      791 2023-05-20 14:58:46.897733 tryceratops-2.3.1/src/tryceratops/types.py
+-rw-r--r--   0        0        0      108 2023-05-20 14:58:46.897733 tryceratops-2.3.1/src/tryceratops/violations/__init__.py
+-rw-r--r--   0        0        0     1745 2023-05-20 14:58:46.897733 tryceratops-2.3.1/src/tryceratops/violations/codes.py
+-rw-r--r--   0        0        0     2403 2023-05-20 14:58:46.897733 tryceratops-2.3.1/src/tryceratops/violations/violations.py
+-rw-r--r--   0        0        0     7443 1970-01-01 00:00:00.000000 tryceratops-2.3.1/PKG-INFO
```

### Comparing `tryceratops-2.3.0/LICENSE` & `tryceratops-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tryceratops-2.3.0/README.md` & `tryceratops-2.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -142,15 +142,15 @@
 
 ## Pre-commit
 
 If you wish to use pre-commit, add this:
 
 ```yaml
   - repo: https://github.com/guilatrova/tryceratops
-    rev: v2.3.0
+    rev: v2.3.1
     hooks:
       - id: tryceratops
 ```
 
 ## Show your style
 
 [![try/except style: tryceratops](https://img.shields.io/badge/try%2Fexcept%20style-tryceratops%20%F0%9F%A6%96%E2%9C%A8-black)](https://github.com/guilatrova/tryceratops)
```

### Comparing `tryceratops-2.3.0/pyproject.toml` & `tryceratops-2.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tryceratops"
-version = "2.3.0"
+version = "2.3.1"
 description = "Prevent Exception Handling AntiPatterns"
 authors = ["Guilherme Latrova <hello@guilatrova.dev>"]
 license = "MIT"
 keywords = ["lint", "try", "except"]
 readme = "README.md"
 homepage = "https://github.com/guilatrova/tryceratops"
 repository = "https://github.com/guilatrova/tryceratops"
```

### Comparing `tryceratops-2.3.0/src/tryceratops/__main__.py` & `tryceratops-2.3.1/src/tryceratops/__main__.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.3.0/src/tryceratops/analyzers/__init__.py` & `tryceratops-2.3.1/src/tryceratops/analyzers/__init__.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.3.0/src/tryceratops/analyzers/base.py` & `tryceratops-2.3.1/src/tryceratops/analyzers/base.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.3.0/src/tryceratops/analyzers/call.py` & `tryceratops-2.3.1/src/tryceratops/analyzers/call.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.3.0/src/tryceratops/analyzers/classdefs.py` & `tryceratops-2.3.1/src/tryceratops/analyzers/classdefs.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,18 +50,21 @@
 
 class InheritFromBaseAnalyzer(BaseAnalyzer):
     violation_code = codes.ALLOWED_BASE_EXCEPTION
     violation_type = InheritFromNonBaseViolation
 
     @visit_error_handler
     def visit_ClassDef(self, node: ast.ClassDef) -> t.Any:
+        settings = t.cast(GlobalSettings, self._settings)
+        if not settings.allowed_base_exceptions:
+            return self.generic_visit(node)
+
         is_exc = any([base for base in node.bases if getattr(base, "id", None) == "Exception"])
         if is_exc is False:
             return self.generic_visit(node)
 
-        settings = t.cast(GlobalSettings, self._settings)
         if node.name not in settings.allowed_base_exceptions:
             self._mark_violation(
                 node,
                 class_name=node.name,
                 allowed_bases=settings.allowed_base_exceptions,
             )
```

### Comparing `tryceratops-2.3.0/src/tryceratops/analyzers/conditional.py` & `tryceratops-2.3.1/src/tryceratops/analyzers/conditional.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.3.0/src/tryceratops/analyzers/exception_block.py` & `tryceratops-2.3.1/src/tryceratops/analyzers/exception_block.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.3.0/src/tryceratops/analyzers/try_block.py` & `tryceratops-2.3.1/src/tryceratops/analyzers/try_block.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.3.0/src/tryceratops/files/discovery.py` & `tryceratops-2.3.1/src/tryceratops/files/discovery.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.3.0/src/tryceratops/files/parser.py` & `tryceratops-2.3.1/src/tryceratops/files/parser.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.3.0/src/tryceratops/fixers/__init__.py` & `tryceratops-2.3.1/src/tryceratops/fixers/__init__.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.3.0/src/tryceratops/fixers/base.py` & `tryceratops-2.3.1/src/tryceratops/fixers/base.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.3.0/src/tryceratops/fixers/exception_block.py` & `tryceratops-2.3.1/src/tryceratops/fixers/exception_block.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.3.0/src/tryceratops/flake_plugin.py` & `tryceratops-2.3.1/src/tryceratops/flake_plugin.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.3.0/src/tryceratops/interfaces.py` & `tryceratops-2.3.1/src/tryceratops/interfaces.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.3.0/src/tryceratops/logging_config.py` & `tryceratops-2.3.1/src/tryceratops/logging_config.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.3.0/src/tryceratops/runners.py` & `tryceratops-2.3.1/src/tryceratops/runners.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.3.0/src/tryceratops/settings.py` & `tryceratops-2.3.1/src/tryceratops/settings.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.3.0/src/tryceratops/types.py` & `tryceratops-2.3.1/src/tryceratops/types.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.3.0/src/tryceratops/violations/codes.py` & `tryceratops-2.3.1/src/tryceratops/violations/codes.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.3.0/src/tryceratops/violations/violations.py` & `tryceratops-2.3.1/src/tryceratops/violations/violations.py`

 * *Files identical despite different names*

### Comparing `tryceratops-2.3.0/PKG-INFO` & `tryceratops-2.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tryceratops
-Version: 2.3.0
+Version: 2.3.1
 Summary: Prevent Exception Handling AntiPatterns
 Home-page: https://github.com/guilatrova/tryceratops
 License: MIT
 Keywords: lint,try,except
 Author: Guilherme Latrova
 Author-email: hello@guilatrova.dev
 Requires-Python: >=3.8.1,<4.0
@@ -171,15 +171,15 @@
 
 ## Pre-commit
 
 If you wish to use pre-commit, add this:
 
 ```yaml
   - repo: https://github.com/guilatrova/tryceratops
-    rev: v2.3.0
+    rev: v2.3.1
     hooks:
       - id: tryceratops
 ```
 
 ## Show your style
 
 [![try/except style: tryceratops](https://img.shields.io/badge/try%2Fexcept%20style-tryceratops%20%F0%9F%A6%96%E2%9C%A8-black)](https://github.com/guilatrova/tryceratops)
```

