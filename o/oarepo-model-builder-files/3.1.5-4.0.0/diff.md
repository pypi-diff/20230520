# Comparing `tmp/oarepo-model-builder-files-3.1.5.tar.gz` & `tmp/oarepo-model-builder-files-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-model-builder-files-3.1.5.tar", last modified: Tue Apr 25 08:23:00 2023, max compression
+gzip compressed data, was "oarepo-model-builder-files-4.0.0.tar", last modified: Sat May 20 14:03:16 2023, max compression
```

## Comparing `oarepo-model-builder-files-3.1.5.tar` & `oarepo-model-builder-files-4.0.0.tar`

### file list

```diff
@@ -1,63 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:23:00.925293 oarepo-model-builder-files-3.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-25 08:23:00.925293 oarepo-model-builder-files-3.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:23:00.909293 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:23:00.913293 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/builtin_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/builtin_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/builtin_models/invenio_files.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:23:00.913293 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio/invenio_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio/invenio_files_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio/invenio_files_record_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio/invenio_files_record_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio/invenio_files_record_service_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio/invenio_files_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:23:00.917292 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio/templates/invenio_files_record.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio/templates/invenio_files_record_metadata.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio/templates/invenio_files_record_permissions.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio/templates/invenio_files_record_service_config.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio/templates/invenio_files_schema.py.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:23:00.917292 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio_parent/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio_parent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio_parent/invenio_files_parent_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio_parent/invenio_files_parent_record_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio_parent/invenio_files_parent_record_service_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio_parent/invenio_files_parent_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:23:00.921293 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio_parent/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio_parent/templates/invenio_files_record.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio_parent/templates/invenio_files_record_metadata.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio_parent/templates/invenio_files_record_service_config.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio_parent/templates/invenio_files_schema.py.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:23:00.921293 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/model_preprocessors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/model_preprocessors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/model_preprocessors/invenio_files_after.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/model_preprocessors/invenio_files_base_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/model_preprocessors/invenio_files_before.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:23:00.921293 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/profiles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/profiles/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:23:00.925293 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/tests/invenio_conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/tests/invenio_files_conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/tests/invenio_files_test_file_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:23:00.925293 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/tests/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/tests/templates/invenio_conftest.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/tests/templates/invenio_files_conftest.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)    10473 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/tests/templates/invenio_files_test_file_resources.py.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:23:00.925293 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/validation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:23:00.913293 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-25 08:23:00.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-04-25 08:23:00.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 08:23:00.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-04-25 08:23:00.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-25 08:23:00.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-25 08:23:00.000000 oarepo-model-builder-files-3.1.5/oarepo_model_builder_files.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-04-25 08:23:00.925293 oarepo-model-builder-files-3.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 08:18:13.000000 oarepo-model-builder-files-3.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:03:16.599688 oarepo-model-builder-files-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-05-20 14:03:16.599688 oarepo-model-builder-files-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:03:16.595688 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:03:16.595688 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:03:16.595688 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/invenio/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/invenio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/invenio/invenio_files_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/invenio/invenio_files_record_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/invenio/invenio_files_record_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/invenio/invenio_files_record_service_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:03:16.595688 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/invenio/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/invenio/templates/invenio_files_record.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/invenio/templates/invenio_files_record_metadata.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/invenio/templates/invenio_files_record_permissions.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/invenio/templates/invenio_files_record_service_config.py.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:03:16.599688 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/invenio_parent/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/invenio_parent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/invenio_parent/invenio_files_parent_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/invenio_parent/invenio_files_parent_record_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/invenio_parent/invenio_files_parent_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:03:16.599688 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/invenio_parent/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/invenio_parent/templates/invenio_files_record.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/invenio_parent/templates/invenio_files_record_metadata.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/invenio_parent/templates/invenio_files_schema.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/parent_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:03:16.599688 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/tests/invenio_files_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/tests/invenio_files_conftest_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/tests/invenio_files_test_file_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:03:16.599688 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/tests/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/tests/templates/invenio_files_conftest.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/tests/templates/invenio_files_conftest_files.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)    11067 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/tests/templates/invenio_files_test_file_resources.py.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:03:16.599688 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builtin_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builtin_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builtin_models/invenio_files.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:03:16.599688 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/datatypes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:03:16.599688 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/datatypes/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/datatypes/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/datatypes/components/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/datatypes/components/parent_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/datatypes/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:03:16.599688 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/profiles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/profiles/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:03:16.595688 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-05-20 14:03:16.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-20 14:03:16.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 14:03:16.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-05-20 14:03:16.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-20 14:03:16.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-20 14:03:16.000000 oarepo-model-builder-files-4.0.0/oarepo_model_builder_files.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-20 14:03:16.603688 oarepo-model-builder-files-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 13:59:40.000000 oarepo-model-builder-files-4.0.0/setup.py
```

### Comparing `oarepo-model-builder-files-3.1.5/PKG-INFO` & `oarepo-model-builder-files-4.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-Metadata-Version: 2.1
-Name: oarepo-model-builder-files
-Version: 3.1.5
-Description-Content-Type: text/markdown
-
 # OARepo model builder files
 
 Plugin adding support for working with files based on the invenio model. <br>
 Files are represented as another ("file") record connected with the original parent one.
 The plugin generates the file record and modifies the parent record to create connection with new file one.
 The file record is specified under "files" attribute in the model yaml file, see example 
 in tests.
@@ -22,36 +17,38 @@
 The api is by default accessible at {original model url}/{base record id}/files.
 The api is taken from InvenioRDM, the docs are [here](https://inveniordm.docs.cern.ch/reference/rest_api_drafts_records/#record-files)
 
 ## Example
 
 A simple record with associated files can be defined as this:
 ```yaml
-model:
+record:
   properties:
     metadata:
       properties:
         title:
           type: fulltext
         status:
           type: keyword
-  package: thesis
-  schema-server: 'local://'
+  module:
+    name: thesis
   use:
     - invenio
 
 files:
   properties:
     metadata:
       properties:
         title:
           type: fulltext
-  package: thesis
-  schema-server: 'local://'
+  module:
+    name: thesis
   use:
     - invenio_files
+settings:
+  schema-server: 'local://'
 ```
 Using the api, first an
 instance of the model has to be created. Then an instance of the
 associated file record. The file content is then uploaded in separate step and
 finally the upload must be commited.
- 
+
```

### Comparing `oarepo-model-builder-files-3.1.5/README.md` & `oarepo-model-builder-files-4.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+Metadata-Version: 2.1
+Name: oarepo-model-builder-files
+Version: 4.0.0
+Description-Content-Type: text/markdown
+
 # OARepo model builder files
 
 Plugin adding support for working with files based on the invenio model. <br>
 Files are represented as another ("file") record connected with the original parent one.
 The plugin generates the file record and modifies the parent record to create connection with new file one.
 The file record is specified under "files" attribute in the model yaml file, see example 
 in tests.
@@ -17,36 +22,38 @@
 The api is by default accessible at {original model url}/{base record id}/files.
 The api is taken from InvenioRDM, the docs are [here](https://inveniordm.docs.cern.ch/reference/rest_api_drafts_records/#record-files)
 
 ## Example
 
 A simple record with associated files can be defined as this:
 ```yaml
-model:
+record:
   properties:
     metadata:
       properties:
         title:
           type: fulltext
         status:
           type: keyword
-  package: thesis
-  schema-server: 'local://'
+  module:
+    name: thesis
   use:
     - invenio
 
 files:
   properties:
     metadata:
       properties:
         title:
           type: fulltext
-  package: thesis
-  schema-server: 'local://'
+  module:
+    name: thesis
   use:
     - invenio_files
+settings:
+  schema-server: 'local://'
 ```
 Using the api, first an
 instance of the model has to be created. Then an instance of the
 associated file record. The file content is then uploaded in separate step and
 finally the upload must be commited.
- 
+
```

### Comparing `oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/invenio/__init__.py` & `oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/invenio/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 TEMPLATES = {
     "files-record": "templates/invenio_files_record.py.jinja2",
     "files-record-parent-extension": "templates/invenio_files_record_parent_extension.py.jinja2",
     "files-record-metadata": "templates/invenio_files_record_metadata.py.jinja2",
     "files-permissions": "templates/invenio_files_record_permissions.py.jinja2",
     "files-service-config": "templates/invenio_files_record_service_config.py.jinja2",
     "files-schema": "templates/invenio_files_schema.py.jinja2",
-    "files-original-schema-extension": "templates/invenio_files_schema_parent_extension.py.jinja2"
-}
+    "files-original-schema-extension": "templates/invenio_files_schema_parent_extension.py.jinja2",
+}
```

### Comparing `oarepo-model-builder-files-3.1.5/oarepo_model_builder_files/tests/templates/invenio_files_conftest.py.jinja2` & `oarepo-model-builder-files-4.0.0/oarepo_model_builder_files/builders/tests/templates/invenio_files_conftest_files.py.jinja2`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import os
 
-from {{ files.record_service_config_class|package_name }} import {{ files.record_service_config_class|base_name }}
-from {{ files.record_service_class|package_name }} import {{ files.record_service_class|base_name }}
-from {{ files.record_resource_config_class|package_name }} import {{ files.record_resource_config_class|base_name }}
+{{ vars.service_config.class|generate_import }}
+{{ vars.service.class|generate_import }}
+{{ vars.resource_config.class|generate_import }}
 from invenio_records_resources.resources import FileResource
 from invenio_app.factory import create_api as _create_api
 import pytest
 
 @pytest.fixture(scope="module")
 def file_service():
     """File service shared fixture."""
-    service = {{ files.record_service_class|base_name }}({{ files.record_service_config_class|base_name }}())
+    service = {{ vars.service.class|base_name }}({{ vars.service_config.class|base_name }}())
     return service
 
 @pytest.fixture(scope="module")
 def file_resource(file_service):
     """File Resources."""
-    return FileResource({{ files.record_resource_config_class|base_name }}(), file_service)
+    return FileResource({{ vars.resource_config.class|base_name }}(), file_service)
 
 
 @pytest.fixture(scope="module")
 def headers():
     """Default headers for making requests."""
     return {
         "content-type": "application/json",
@@ -32,8 +32,8 @@
     app_config["FILES_REST_STORAGE_CLASS_LIST"] = {
         "L": "Local",
         "F": "Fetch",
         "R": "Remote",
     }
     app_config["FILES_REST_DEFAULT_STORAGE_CLASS"] = "L"
 
-    return app_config
+    return app_config
```

### Comparing `oarepo-model-builder-files-3.1.5/oarepo_model_builder_files.egg-info/PKG-INFO` & `oarepo-model-builder-files-4.0.0/oarepo_model_builder_files.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-files
-Version: 3.1.5
+Version: 4.0.0
 Description-Content-Type: text/markdown
 
 # OARepo model builder files
 
 Plugin adding support for working with files based on the invenio model. <br>
 Files are represented as another ("file") record connected with the original parent one.
 The plugin generates the file record and modifies the parent record to create connection with new file one.
@@ -22,36 +22,38 @@
 The api is by default accessible at {original model url}/{base record id}/files.
 The api is taken from InvenioRDM, the docs are [here](https://inveniordm.docs.cern.ch/reference/rest_api_drafts_records/#record-files)
 
 ## Example
 
 A simple record with associated files can be defined as this:
 ```yaml
-model:
+record:
   properties:
     metadata:
       properties:
         title:
           type: fulltext
         status:
           type: keyword
-  package: thesis
-  schema-server: 'local://'
+  module:
+    name: thesis
   use:
     - invenio
 
 files:
   properties:
     metadata:
       properties:
         title:
           type: fulltext
-  package: thesis
-  schema-server: 'local://'
+  module:
+    name: thesis
   use:
     - invenio_files
+settings:
+  schema-server: 'local://'
 ```
 Using the api, first an
 instance of the model has to be created. Then an instance of the
 associated file record. The file content is then uploaded in separate step and
 finally the upload must be commited.
```

### Comparing `oarepo-model-builder-files-3.1.5/oarepo_model_builder_files.egg-info/SOURCES.txt` & `oarepo-model-builder-files-4.0.0/oarepo_model_builder_files.egg-info/entry_points.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,49 +1,31 @@
-MANIFEST.in
-README.md
-pyproject.toml
-setup.cfg
-setup.py
-oarepo_model_builder_files/__init__.py
-oarepo_model_builder_files.egg-info/PKG-INFO
-oarepo_model_builder_files.egg-info/SOURCES.txt
-oarepo_model_builder_files.egg-info/dependency_links.txt
-oarepo_model_builder_files.egg-info/entry_points.txt
-oarepo_model_builder_files.egg-info/requires.txt
-oarepo_model_builder_files.egg-info/top_level.txt
-oarepo_model_builder_files/builtin_models/__init__.py
-oarepo_model_builder_files/builtin_models/invenio_files.json
-oarepo_model_builder_files/invenio/__init__.py
-oarepo_model_builder_files/invenio/invenio_files.py
-oarepo_model_builder_files/invenio/invenio_files_record.py
-oarepo_model_builder_files/invenio/invenio_files_record_metadata.py
-oarepo_model_builder_files/invenio/invenio_files_record_permissions.py
-oarepo_model_builder_files/invenio/invenio_files_record_service_config.py
-oarepo_model_builder_files/invenio/invenio_files_schema.py
-oarepo_model_builder_files/invenio/templates/invenio_files_record.py.jinja2
-oarepo_model_builder_files/invenio/templates/invenio_files_record_metadata.py.jinja2
-oarepo_model_builder_files/invenio/templates/invenio_files_record_permissions.py.jinja2
-oarepo_model_builder_files/invenio/templates/invenio_files_record_service_config.py.jinja2
-oarepo_model_builder_files/invenio/templates/invenio_files_schema.py.jinja2
-oarepo_model_builder_files/invenio_parent/__init__.py
-oarepo_model_builder_files/invenio_parent/invenio_files_parent_record.py
-oarepo_model_builder_files/invenio_parent/invenio_files_parent_record_metadata.py
-oarepo_model_builder_files/invenio_parent/invenio_files_parent_record_service_config.py
-oarepo_model_builder_files/invenio_parent/invenio_files_parent_schema.py
-oarepo_model_builder_files/invenio_parent/templates/invenio_files_record.py.jinja2
-oarepo_model_builder_files/invenio_parent/templates/invenio_files_record_metadata.py.jinja2
-oarepo_model_builder_files/invenio_parent/templates/invenio_files_record_service_config.py.jinja2
-oarepo_model_builder_files/invenio_parent/templates/invenio_files_schema.py.jinja2
-oarepo_model_builder_files/model_preprocessors/__init__.py
-oarepo_model_builder_files/model_preprocessors/invenio_files_after.py
-oarepo_model_builder_files/model_preprocessors/invenio_files_base_classes.py
-oarepo_model_builder_files/model_preprocessors/invenio_files_before.py
-oarepo_model_builder_files/profiles/__init__.py
-oarepo_model_builder_files/profiles/file.py
-oarepo_model_builder_files/tests/__init__.py
-oarepo_model_builder_files/tests/invenio_conftest.py
-oarepo_model_builder_files/tests/invenio_files_conftest.py
-oarepo_model_builder_files/tests/invenio_files_test_file_resources.py
-oarepo_model_builder_files/tests/templates/invenio_conftest.py.jinja2
-oarepo_model_builder_files/tests/templates/invenio_files_conftest.py.jinja2
-oarepo_model_builder_files/tests/templates/invenio_files_test_file_resources.py.jinja2
-oarepo_model_builder_files/validation/__init__.py
+[oarepo.models]
+invenio_files = oarepo_model_builder_files.builtin_models:invenio_files.json
+
+[oarepo_model_builder.builders.files]
+2010-invenio_files_record = oarepo_model_builder_files.builders.invenio.invenio_files_record:InvenioFilesRecordBuilder
+2010-invenio_files_record_metadata = oarepo_model_builder_files.builders.invenio.invenio_files_record_metadata:InvenioFilesRecordMetadataBuilder
+2020-invenio_files_permissions = oarepo_model_builder_files.builders.invenio.invenio_files_record_permissions:InvenioFilesRecordPermissionsBuilder
+2030-invenio_files_parent_record = oarepo_model_builder_files.builders.invenio_parent.invenio_files_parent_record:InvenioFilesParentRecordBuilder
+2030-invenio_files_parent_record_metadata = oarepo_model_builder_files.builders.invenio_parent.invenio_files_parent_record_metadata:InvenioFilesParentRecordMetadataBuilder
+2030-invenio_files_parent_schema = oarepo_model_builder_files.builders.invenio_parent.invenio_files_parent_schema:InvenioFilesParentSchemaBuilder
+2030-invenio_files_record_service_config = oarepo_model_builder_files.builders.invenio.invenio_files_record_service_config:InvenioRecordServiceConfigBuilder
+2040-invenio_files_conftest = oarepo_model_builder_files.builders.tests.invenio_files_conftest:InvenioFilesConftestBuilder
+2040-invenio_files_conftest_files = oarepo_model_builder_files.builders.tests.invenio_files_conftest_files:InvenioFilesConftestFilesBuilder
+2040-invenio_files_test_files_resources = oarepo_model_builder_files.builders.tests.invenio_files_test_file_resources:InvenioFilesTestFileResourcesBuilder
+
+[oarepo_model_builder.builders.files.inherit]
+0100-model = oarepo_model_builder.builders.record
+
+[oarepo_model_builder.datatypes]
+invenio_files = oarepo_model_builder_files.datatypes:file_datatypes
+
+[oarepo_model_builder.datatypes.components]
+invenio_files = oarepo_model_builder_files.datatypes.components:file_components
+
+[oarepo_model_builder.profiles]
+files = oarepo_model_builder_files.profiles.file:FileProfile
+
+[oarepo_model_builder.templates]
+99-files_parent_templates = oarepo_model_builder_files.builders.invenio_parent
+99-files_templates = oarepo_model_builder_files.builders.invenio
+99-files_test_templates = oarepo_model_builder_files.builders.tests
```

