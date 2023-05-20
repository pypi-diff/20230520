# Comparing `tmp/oarepo-model-builder-cf-1.0.0.tar.gz` & `tmp/oarepo-model-builder-cf-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-model-builder-cf-1.0.0.tar", last modified: Mon Feb 13 08:36:23 2023, max compression
+gzip compressed data, was "oarepo-model-builder-cf-1.0.1.tar", last modified: Mon Feb 13 18:30:57 2023, max compression
```

## Comparing `oarepo-model-builder-cf-1.0.0.tar` & `oarepo-model-builder-cf-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 08:36:23.718065 oarepo-model-builder-cf-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-13 08:33:51.000000 oarepo-model-builder-cf-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-02-13 08:36:23.718065 oarepo-model-builder-cf-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-02-13 08:33:51.000000 oarepo-model-builder-cf-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 08:36:23.714065 oarepo-model-builder-cf-1.0.0/oarepo_model_builder_cf/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-02-13 08:33:51.000000 oarepo-model-builder-cf-1.0.0/oarepo_model_builder_cf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-02-13 08:33:51.000000 oarepo-model-builder-cf-1.0.0/oarepo_model_builder_cf/builders.py
--rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-02-13 08:33:51.000000 oarepo-model-builder-cf-1.0.0/oarepo_model_builder_cf/model_preprocessors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 08:36:23.718065 oarepo-model-builder-cf-1.0.0/oarepo_model_builder_cf/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 08:33:51.000000 oarepo-model-builder-cf-1.0.0/oarepo_model_builder_cf/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-02-13 08:33:51.000000 oarepo-model-builder-cf-1.0.0/oarepo_model_builder_cf/templates/record.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-02-13 08:33:51.000000 oarepo-model-builder-cf-1.0.0/oarepo_model_builder_cf/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 08:36:23.718065 oarepo-model-builder-cf-1.0.0/oarepo_model_builder_cf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-02-13 08:36:23.000000 oarepo-model-builder-cf-1.0.0/oarepo_model_builder_cf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-02-13 08:36:23.000000 oarepo-model-builder-cf-1.0.0/oarepo_model_builder_cf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 08:36:23.000000 oarepo-model-builder-cf-1.0.0/oarepo_model_builder_cf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-02-13 08:36:23.000000 oarepo-model-builder-cf-1.0.0/oarepo_model_builder_cf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 08:34:46.000000 oarepo-model-builder-cf-1.0.0/oarepo_model_builder_cf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-02-13 08:36:23.000000 oarepo-model-builder-cf-1.0.0/oarepo_model_builder_cf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-13 08:36:23.000000 oarepo-model-builder-cf-1.0.0/oarepo_model_builder_cf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-02-13 08:33:51.000000 oarepo-model-builder-cf-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-02-13 08:36:23.718065 oarepo-model-builder-cf-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-02-13 08:33:51.000000 oarepo-model-builder-cf-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 18:30:57.603500 oarepo-model-builder-cf-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-13 18:28:26.000000 oarepo-model-builder-cf-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-02-13 18:30:57.603500 oarepo-model-builder-cf-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-02-13 18:28:26.000000 oarepo-model-builder-cf-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 18:30:57.599499 oarepo-model-builder-cf-1.0.1/oarepo_model_builder_cf/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-02-13 18:28:26.000000 oarepo-model-builder-cf-1.0.1/oarepo_model_builder_cf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-02-13 18:28:26.000000 oarepo-model-builder-cf-1.0.1/oarepo_model_builder_cf/builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-02-13 18:28:26.000000 oarepo-model-builder-cf-1.0.1/oarepo_model_builder_cf/model_preprocessors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 18:30:57.599499 oarepo-model-builder-cf-1.0.1/oarepo_model_builder_cf/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 18:28:26.000000 oarepo-model-builder-cf-1.0.1/oarepo_model_builder_cf/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-02-13 18:28:26.000000 oarepo-model-builder-cf-1.0.1/oarepo_model_builder_cf/templates/record.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-02-13 18:28:26.000000 oarepo-model-builder-cf-1.0.1/oarepo_model_builder_cf/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 18:30:57.599499 oarepo-model-builder-cf-1.0.1/oarepo_model_builder_cf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-02-13 18:30:57.000000 oarepo-model-builder-cf-1.0.1/oarepo_model_builder_cf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-02-13 18:30:57.000000 oarepo-model-builder-cf-1.0.1/oarepo_model_builder_cf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 18:30:57.000000 oarepo-model-builder-cf-1.0.1/oarepo_model_builder_cf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-02-13 18:30:57.000000 oarepo-model-builder-cf-1.0.1/oarepo_model_builder_cf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 18:29:18.000000 oarepo-model-builder-cf-1.0.1/oarepo_model_builder_cf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-02-13 18:30:57.000000 oarepo-model-builder-cf-1.0.1/oarepo_model_builder_cf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-13 18:30:57.000000 oarepo-model-builder-cf-1.0.1/oarepo_model_builder_cf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-02-13 18:28:26.000000 oarepo-model-builder-cf-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-02-13 18:30:57.603500 oarepo-model-builder-cf-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-02-13 18:28:26.000000 oarepo-model-builder-cf-1.0.1/setup.py
```

### Comparing `oarepo-model-builder-cf-1.0.0/PKG-INFO` & `oarepo-model-builder-cf-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-cf
-Version: 1.0.0
+Version: 1.0.1
 Summary: "A model builder plugin for custom fields support"
 Home-page: https://github.com/oarepo/oarepo-model-builder-cf
 Author: Miroslav Simek
 Author-email: simek.miroslav@techlib.cz
 License: MIT
 Keywords: invenio cf model builder
 Platform: any
```

### Comparing `oarepo-model-builder-cf-1.0.0/README.md` & `oarepo-model-builder-cf-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-cf-1.0.0/oarepo_model_builder_cf/builders.py` & `oarepo-model-builder-cf-1.0.1/oarepo_model_builder_cf/builders.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-cf-1.0.0/oarepo_model_builder_cf/model_preprocessors.py` & `oarepo-model-builder-cf-1.0.1/oarepo_model_builder_cf/model_preprocessors.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-cf-1.0.0/oarepo_model_builder_cf/templates/record.py.jinja2` & `oarepo-model-builder-cf-1.0.1/oarepo_model_builder_cf/templates/record.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-cf-1.0.0/oarepo_model_builder_cf/validation.py` & `oarepo-model-builder-cf-1.0.1/oarepo_model_builder_cf/validation.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-cf-1.0.0/oarepo_model_builder_cf.egg-info/PKG-INFO` & `oarepo-model-builder-cf-1.0.1/oarepo_model_builder_cf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-cf
-Version: 1.0.0
+Version: 1.0.1
 Summary: "A model builder plugin for custom fields support"
 Home-page: https://github.com/oarepo/oarepo-model-builder-cf
 Author: Miroslav Simek
 Author-email: simek.miroslav@techlib.cz
 License: MIT
 Keywords: invenio cf model builder
 Platform: any
```

### Comparing `oarepo-model-builder-cf-1.0.0/oarepo_model_builder_cf.egg-info/SOURCES.txt` & `oarepo-model-builder-cf-1.0.1/oarepo_model_builder_cf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-cf-1.0.0/setup.cfg` & `oarepo-model-builder-cf-1.0.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-model-builder-cf
-version = 1.0.0
+version = 1.0.1
 description = "A model builder plugin for custom fields support"
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = invenio cf model builder
 license = MIT
 author = Miroslav Simek
 author_email = simek.miroslav@techlib.cz
@@ -29,15 +29,15 @@
 
 [options.entry_points]
 oarepo_model_builder.validation = 
 	cf = oarepo_model_builder_cf.validation:VALIDATION
 oarepo_model_builder.templates = 
 	99-cf-templates  = oarepo_model_builder_cf
 oarepo_model_builder.builders.model = 
-	1000-relation-field = oarepo_model_builder_cf.builders:InvenioRecordCFBuilder
+	1000-cf-field = oarepo_model_builder_cf.builders:InvenioRecordCFBuilder
 oarepo_model_builder.model_preprocessors.model = 
 	1000-cf = oarepo_model_builder_cf.model_preprocessors:CFModelPreprocessor
 
 [build_sphinx]
 source-dir = docs/
 build-dir = docs/_build
 all_files = 1
```

