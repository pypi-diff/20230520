# Comparing `tmp/satori_playbook_validator-1.0.3.tar.gz` & `tmp/satori_playbook_validator-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satori_playbook_validator-1.0.3.tar", last modified: Sat May 20 00:15:29 2023, max compression
+gzip compressed data, was "satori_playbook_validator-1.0.4.tar", last modified: Sat May 20 05:48:16 2023, max compression
```

## Comparing `satori_playbook_validator-1.0.3.tar` & `satori_playbook_validator-1.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       30 2023-05-19 04:01:53.443821 satori_playbook_validator-1.0.3/README.md
--rw-r--r--   0        0        0      433 2023-05-20 00:15:29.321934 satori_playbook_validator-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      163 2023-05-19 23:03:01.874905 satori_playbook_validator-1.0.3/src/satorici/validator/__init__.py
--rw-r--r--   0        0        0     3085 2023-05-20 00:12:28.043887 satori_playbook_validator-1.0.3/src/satorici/validator/_validator.py
--rw-r--r--   0        0        0       51 2023-05-19 23:02:04.723720 satori_playbook_validator-1.0.3/src/satorici/validator/exceptions.py
--rw-r--r--   0        0        0      267 2023-05-19 01:00:58.588993 satori_playbook_validator-1.0.3/src/satorici/validator/schemas/command.json
--rw-r--r--   0        0        0      251 2023-05-19 01:00:58.588993 satori_playbook_validator-1.0.3/src/satorici/validator/schemas/import.json
--rw-r--r--   0        0        0     2197 2023-05-19 01:00:58.588993 satori_playbook_validator-1.0.3/src/satorici/validator/schemas/input.json
--rw-r--r--   0        0        0     1025 2023-05-19 01:00:58.588993 satori_playbook_validator-1.0.3/src/satorici/validator/schemas/settings.json
--rw-r--r--   0        0        0     1743 2023-05-19 01:00:58.588993 satori_playbook_validator-1.0.3/src/satorici/validator/schemas/test.json
--rw-r--r--   0        0        0      286 1970-01-01 00:00:00.000000 satori_playbook_validator-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0       30 2023-05-20 05:47:58.876425 satori_playbook_validator-1.0.4/README.md
+-rw-r--r--   0        0        0      433 2023-05-20 05:48:16.012914 satori_playbook_validator-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      163 2023-05-20 05:47:58.876425 satori_playbook_validator-1.0.4/src/satorici/validator/__init__.py
+-rw-r--r--   0        0        0     3114 2023-05-20 05:47:58.876425 satori_playbook_validator-1.0.4/src/satorici/validator/_validator.py
+-rw-r--r--   0        0        0       51 2023-05-20 05:47:58.876425 satori_playbook_validator-1.0.4/src/satorici/validator/exceptions.py
+-rw-r--r--   0        0        0      267 2023-05-20 05:47:58.876425 satori_playbook_validator-1.0.4/src/satorici/validator/schemas/command.json
+-rw-r--r--   0        0        0      251 2023-05-20 05:47:58.876425 satori_playbook_validator-1.0.4/src/satorici/validator/schemas/import.json
+-rw-r--r--   0        0        0     2197 2023-05-20 05:47:58.876425 satori_playbook_validator-1.0.4/src/satorici/validator/schemas/input.json
+-rw-r--r--   0        0        0     1025 2023-05-20 05:47:58.876425 satori_playbook_validator-1.0.4/src/satorici/validator/schemas/settings.json
+-rw-r--r--   0        0        0     1743 2023-05-20 05:47:58.876425 satori_playbook_validator-1.0.4/src/satorici/validator/schemas/test.json
+-rw-r--r--   0        0        0      286 1970-01-01 00:00:00.000000 satori_playbook_validator-1.0.4/PKG-INFO
```

### Comparing `satori_playbook_validator-1.0.3/src/satorici/validator/_validator.py` & `satori_playbook_validator-1.0.4/src/satorici/validator/_validator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import re
+from copy import deepcopy
 from pathlib import Path
 
 from flatdict import FlatDict
 from jsonschema import Draft7Validator, FormatChecker
 from jsonschema.exceptions import ValidationError
 from jsonschema.validators import RefResolver
 
@@ -78,15 +79,15 @@
 
     Raises `PlaybookValidationError` on invalid playbook
     """
 
     if not isinstance(config, dict):
         raise TypeError("config must be a dict")
 
-    config_copy = config.copy()
+    config_copy = deepcopy(config)
 
     try:
         if config_copy.get("settings"):
             settings_schema.validate(config_copy["settings"])
             del config_copy["settings"]
 
         test_schema.validate(config_copy)
```

### Comparing `satori_playbook_validator-1.0.3/src/satorici/validator/schemas/input.json` & `satori_playbook_validator-1.0.4/src/satorici/validator/schemas/input.json`

 * *Files identical despite different names*

### Comparing `satori_playbook_validator-1.0.3/src/satorici/validator/schemas/settings.json` & `satori_playbook_validator-1.0.4/src/satorici/validator/schemas/settings.json`

 * *Files identical despite different names*

### Comparing `satori_playbook_validator-1.0.3/src/satorici/validator/schemas/test.json` & `satori_playbook_validator-1.0.4/src/satorici/validator/schemas/test.json`

 * *Files identical despite different names*

