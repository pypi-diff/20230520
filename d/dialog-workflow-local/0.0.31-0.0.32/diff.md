# Comparing `tmp/dialog-workflow-local-0.0.31.tar.gz` & `tmp/dialog-workflow-local-0.0.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dialog-workflow-local-0.0.31.tar", last modified: Sat May 20 08:57:25 2023, max compression
+gzip compressed data, was "dialog-workflow-local-0.0.32.tar", last modified: Sat May 20 09:01:31 2023, max compression
```

## Comparing `dialog-workflow-local-0.0.31.tar` & `dialog-workflow-local-0.0.32.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:57:25.840354 dialog-workflow-local-0.0.31/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-20 08:57:25.840354 dialog-workflow-local-0.0.31/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-20 08:57:08.000000 dialog-workflow-local-0.0.31/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:57:25.840354 dialog-workflow-local-0.0.31/dialog_workflow/
--rw-r--r--   0 runner    (1001) docker     (123)    20876 2023-05-20 08:57:08.000000 dialog-workflow-local-0.0.31/dialog_workflow/Act.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-20 08:57:08.000000 dialog-workflow-local-0.0.31/dialog_workflow/Constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-20 08:57:08.000000 dialog-workflow-local-0.0.31/dialog_workflow/DialogWorkflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-05-20 08:57:08.000000 dialog-workflow-local-0.0.31/dialog_workflow/TablesAsObjects.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 08:57:08.000000 dialog-workflow-local-0.0.31/dialog_workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-05-20 08:57:08.000000 dialog-workflow-local-0.0.31/dialog_workflow/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11827 2023-05-20 08:57:08.000000 dialog-workflow-local-0.0.31/dialog_workflow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:57:25.840354 dialog-workflow-local-0.0.31/dialog_workflow_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-20 08:57:25.000000 dialog-workflow-local-0.0.31/dialog_workflow_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-20 08:57:25.000000 dialog-workflow-local-0.0.31/dialog_workflow_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 08:57:25.000000 dialog-workflow-local-0.0.31/dialog_workflow_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-20 08:57:25.000000 dialog-workflow-local-0.0.31/dialog_workflow_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-20 08:57:08.000000 dialog-workflow-local-0.0.31/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 08:57:25.840354 dialog-workflow-local-0.0.31/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-20 08:57:08.000000 dialog-workflow-local-0.0.31/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:01:31.906504 dialog-workflow-local-0.0.32/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-20 09:01:31.906504 dialog-workflow-local-0.0.32/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-20 09:01:19.000000 dialog-workflow-local-0.0.32/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:01:31.902504 dialog-workflow-local-0.0.32/dialog_workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)    20876 2023-05-20 09:01:19.000000 dialog-workflow-local-0.0.32/dialog_workflow/Act.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-20 09:01:19.000000 dialog-workflow-local-0.0.32/dialog_workflow/Constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-20 09:01:19.000000 dialog-workflow-local-0.0.32/dialog_workflow/DialogWorkflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-05-20 09:01:19.000000 dialog-workflow-local-0.0.32/dialog_workflow/TablesAsObjects.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 09:01:19.000000 dialog-workflow-local-0.0.32/dialog_workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-05-20 09:01:19.000000 dialog-workflow-local-0.0.32/dialog_workflow/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11827 2023-05-20 09:01:19.000000 dialog-workflow-local-0.0.32/dialog_workflow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:01:31.906504 dialog-workflow-local-0.0.32/dialog_workflow_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-20 09:01:31.000000 dialog-workflow-local-0.0.32/dialog_workflow_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-20 09:01:31.000000 dialog-workflow-local-0.0.32/dialog_workflow_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 09:01:31.000000 dialog-workflow-local-0.0.32/dialog_workflow_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-20 09:01:31.000000 dialog-workflow-local-0.0.32/dialog_workflow_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-20 09:01:19.000000 dialog-workflow-local-0.0.32/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 09:01:31.906504 dialog-workflow-local-0.0.32/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-20 09:01:19.000000 dialog-workflow-local-0.0.32/setup.py
```

### Comparing `dialog-workflow-local-0.0.31/dialog_workflow/Act.py` & `dialog-workflow-local-0.0.32/dialog_workflow/Act.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.31/dialog_workflow/Constants.py` & `dialog-workflow-local-0.0.32/dialog_workflow/Constants.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.31/dialog_workflow/DialogWorkflow.py` & `dialog-workflow-local-0.0.32/dialog_workflow/DialogWorkflow.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.31/dialog_workflow/TablesAsObjects.py` & `dialog-workflow-local-0.0.32/dialog_workflow/TablesAsObjects.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.31/dialog_workflow/test.py` & `dialog-workflow-local-0.0.32/dialog_workflow/test.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.31/dialog_workflow/utils.py` & `dialog-workflow-local-0.0.32/dialog_workflow/utils.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.31/setup.py` & `dialog-workflow-local-0.0.32/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
      name='dialog-workflow-local',  
-     version='0.0.31',
+     version='0.0.32',
      author="Circles",
      author_email="info@circle.life",
      description="PyPI Package for dialog workflow",
      long_description="This is a package for running the dialog workflow",
      long_description_content_type="text/markdown",
      url="https://github.com/javatechy/dokr",
      packages=setuptools.find_packages(),
```

