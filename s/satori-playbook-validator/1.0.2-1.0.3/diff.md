# Comparing `tmp/satori_playbook_validator-1.0.2.tar.gz` & `tmp/satori_playbook_validator-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satori_playbook_validator-1.0.2.tar", last modified: Fri May 19 15:30:40 2023, max compression
+gzip compressed data, was "satori_playbook_validator-1.0.3.tar", last modified: Sat May 20 00:15:29 2023, max compression
```

## Comparing `satori_playbook_validator-1.0.2.tar` & `satori_playbook_validator-1.0.3.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0       30 2023-05-19 04:01:53.443821 satori_playbook_validator-1.0.2/README.md
--rw-r--r--   0        0        0      433 2023-05-19 15:30:40.944797 satori_playbook_validator-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      163 2023-05-19 04:31:06.265674 satori_playbook_validator-1.0.2/src/satorici/validator/__init__.py
--rw-r--r--   0        0        0     2772 2023-05-19 04:29:51.667588 satori_playbook_validator-1.0.2/src/satorici/validator/_validator.py
--rw-r--r--   0        0        0      267 2023-05-19 01:00:58.588993 satori_playbook_validator-1.0.2/src/satorici/validator/schemas/command.json
--rw-r--r--   0        0        0      251 2023-05-19 01:00:58.588993 satori_playbook_validator-1.0.2/src/satorici/validator/schemas/import.json
--rw-r--r--   0        0        0     2197 2023-05-19 01:00:58.588993 satori_playbook_validator-1.0.2/src/satorici/validator/schemas/input.json
--rw-r--r--   0        0        0     1025 2023-05-19 01:00:58.588993 satori_playbook_validator-1.0.2/src/satorici/validator/schemas/settings.json
--rw-r--r--   0        0        0     1743 2023-05-19 01:00:58.588993 satori_playbook_validator-1.0.2/src/satorici/validator/schemas/test.json
--rw-r--r--   0        0        0      286 1970-01-01 00:00:00.000000 satori_playbook_validator-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0       30 2023-05-19 04:01:53.443821 satori_playbook_validator-1.0.3/README.md
+-rw-r--r--   0        0        0      433 2023-05-20 00:15:29.321934 satori_playbook_validator-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      163 2023-05-19 23:03:01.874905 satori_playbook_validator-1.0.3/src/satorici/validator/__init__.py
+-rw-r--r--   0        0        0     3085 2023-05-20 00:12:28.043887 satori_playbook_validator-1.0.3/src/satorici/validator/_validator.py
+-rw-r--r--   0        0        0       51 2023-05-19 23:02:04.723720 satori_playbook_validator-1.0.3/src/satorici/validator/exceptions.py
+-rw-r--r--   0        0        0      267 2023-05-19 01:00:58.588993 satori_playbook_validator-1.0.3/src/satorici/validator/schemas/command.json
+-rw-r--r--   0        0        0      251 2023-05-19 01:00:58.588993 satori_playbook_validator-1.0.3/src/satorici/validator/schemas/import.json
+-rw-r--r--   0        0        0     2197 2023-05-19 01:00:58.588993 satori_playbook_validator-1.0.3/src/satorici/validator/schemas/input.json
+-rw-r--r--   0        0        0     1025 2023-05-19 01:00:58.588993 satori_playbook_validator-1.0.3/src/satorici/validator/schemas/settings.json
+-rw-r--r--   0        0        0     1743 2023-05-19 01:00:58.588993 satori_playbook_validator-1.0.3/src/satorici/validator/schemas/test.json
+-rw-r--r--   0        0        0      286 1970-01-01 00:00:00.000000 satori_playbook_validator-1.0.3/PKG-INFO
```

### Comparing `satori_playbook_validator-1.0.2/src/satorici/validator/_validator.py` & `satori_playbook_validator-1.0.3/src/satorici/validator/_validator.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import json
 import re
 from pathlib import Path
 
 from flatdict import FlatDict
 from jsonschema import Draft7Validator, FormatChecker
+from jsonschema.exceptions import ValidationError
 from jsonschema.validators import RefResolver
 
+from .exceptions import PlaybookValidationError
+
 INPUT_REGEX = re.compile(r"\$\(([\w-]+)\)")
 
 SCHEMAS = Path(__file__).parent / "schemas"
 
 with (
     open(SCHEMAS / "command.json") as commands,
     open(SCHEMAS / "input.json") as inputs,
@@ -57,37 +60,42 @@
 
             found_prefix = prefix
 
             for key, value in flat_config.items():
                 if key.startswith(prefix) and input_schema.is_valid(value):
                     break
             else:
-                raise Exception(f"No valid inputs for variable: {variable}")
+                raise PlaybookValidationError(
+                    f"No valid inputs for variable: {variable}"
+                )
 
         if not found_prefix:
-            raise Exception(f"Can't resolve variable: {variable}")
+            raise PlaybookValidationError(f"Can't resolve variable: {variable}")
 
 
-def validate_playbook(config):
+def validate_playbook(config: dict):
     """
-    Validate yaml loaded playbook and return corresponding dict
+    Validate yaml loaded playbook config and return corresponding dict
 
-    Raises exception on errors
+    Raises `PlaybookValidationError` on invalid playbook
     """
 
     if not isinstance(config, dict):
-        raise Exception("No identifier found")
+        raise TypeError("config must be a dict")
 
     config_copy = config.copy()
 
-    if config_copy.get("settings"):
-        settings_schema.validate(config_copy["settings"])
-        del config_copy["settings"]
-
-    test_schema.validate(config_copy)
+    try:
+        if config_copy.get("settings"):
+            settings_schema.validate(config_copy["settings"])
+            del config_copy["settings"]
+
+        test_schema.validate(config_copy)
+    except ValidationError as e:
+        raise PlaybookValidationError(e.message)
 
     flat_config = FlatDict(config_copy)
 
     for key, value in flat_config.items():
         if command_schema.is_valid(value):
             validate_command_block(value, key, flat_config)
```

### Comparing `satori_playbook_validator-1.0.2/src/satorici/validator/schemas/input.json` & `satori_playbook_validator-1.0.3/src/satorici/validator/schemas/input.json`

 * *Files identical despite different names*

### Comparing `satori_playbook_validator-1.0.2/src/satorici/validator/schemas/settings.json` & `satori_playbook_validator-1.0.3/src/satorici/validator/schemas/settings.json`

 * *Files identical despite different names*

### Comparing `satori_playbook_validator-1.0.2/src/satorici/validator/schemas/test.json` & `satori_playbook_validator-1.0.3/src/satorici/validator/schemas/test.json`

 * *Files identical despite different names*

