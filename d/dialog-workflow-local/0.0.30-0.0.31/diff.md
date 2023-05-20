# Comparing `tmp/dialog-workflow-local-0.0.30.tar.gz` & `tmp/dialog-workflow-local-0.0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dialog-workflow-local-0.0.30.tar", last modified: Fri May 19 12:49:07 2023, max compression
+gzip compressed data, was "dialog-workflow-local-0.0.31.tar", last modified: Sat May 20 08:57:25 2023, max compression
```

## Comparing `dialog-workflow-local-0.0.30.tar` & `dialog-workflow-local-0.0.31.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:49:07.582520 dialog-workflow-local-0.0.30/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-19 12:49:07.582520 dialog-workflow-local-0.0.30/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-19 12:48:52.000000 dialog-workflow-local-0.0.30/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:49:07.578520 dialog-workflow-local-0.0.30/dialog_workflow/
--rw-r--r--   0 runner    (1001) docker     (123)    20867 2023-05-19 12:48:52.000000 dialog-workflow-local-0.0.30/dialog_workflow/Act.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-19 12:48:52.000000 dialog-workflow-local-0.0.30/dialog_workflow/Constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-19 12:48:52.000000 dialog-workflow-local-0.0.30/dialog_workflow/DialogWorkflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-05-19 12:48:52.000000 dialog-workflow-local-0.0.30/dialog_workflow/TablesAsObjects.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 12:48:52.000000 dialog-workflow-local-0.0.30/dialog_workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-05-19 12:48:52.000000 dialog-workflow-local-0.0.30/dialog_workflow/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11827 2023-05-19 12:48:52.000000 dialog-workflow-local-0.0.30/dialog_workflow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:49:07.582520 dialog-workflow-local-0.0.30/dialog_workflow_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-19 12:49:07.000000 dialog-workflow-local-0.0.30/dialog_workflow_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-19 12:49:07.000000 dialog-workflow-local-0.0.30/dialog_workflow_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 12:49:07.000000 dialog-workflow-local-0.0.30/dialog_workflow_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-19 12:49:07.000000 dialog-workflow-local-0.0.30/dialog_workflow_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-19 12:48:52.000000 dialog-workflow-local-0.0.30/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 12:49:07.582520 dialog-workflow-local-0.0.30/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-19 12:48:52.000000 dialog-workflow-local-0.0.30/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:57:25.840354 dialog-workflow-local-0.0.31/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-20 08:57:25.840354 dialog-workflow-local-0.0.31/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-20 08:57:08.000000 dialog-workflow-local-0.0.31/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:57:25.840354 dialog-workflow-local-0.0.31/dialog_workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)    20876 2023-05-20 08:57:08.000000 dialog-workflow-local-0.0.31/dialog_workflow/Act.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-20 08:57:08.000000 dialog-workflow-local-0.0.31/dialog_workflow/Constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-20 08:57:08.000000 dialog-workflow-local-0.0.31/dialog_workflow/DialogWorkflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-05-20 08:57:08.000000 dialog-workflow-local-0.0.31/dialog_workflow/TablesAsObjects.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 08:57:08.000000 dialog-workflow-local-0.0.31/dialog_workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-05-20 08:57:08.000000 dialog-workflow-local-0.0.31/dialog_workflow/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11827 2023-05-20 08:57:08.000000 dialog-workflow-local-0.0.31/dialog_workflow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:57:25.840354 dialog-workflow-local-0.0.31/dialog_workflow_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-20 08:57:25.000000 dialog-workflow-local-0.0.31/dialog_workflow_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-20 08:57:25.000000 dialog-workflow-local-0.0.31/dialog_workflow_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 08:57:25.000000 dialog-workflow-local-0.0.31/dialog_workflow_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-20 08:57:25.000000 dialog-workflow-local-0.0.31/dialog_workflow_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-20 08:57:08.000000 dialog-workflow-local-0.0.31/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 08:57:25.840354 dialog-workflow-local-0.0.31/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-20 08:57:08.000000 dialog-workflow-local-0.0.31/setup.py
```

### Comparing `dialog-workflow-local-0.0.30/dialog_workflow/Act.py` & `dialog-workflow-local-0.0.31/dialog_workflow/Act.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from dialog_workflow.utils import *
 from dialog_workflow.TablesAsObjects import DialogWorkflowRecord, Variable, ProfileContext
 import time
 # import msvcrt
 # import requests
-from src import DetectAge
+from AgeDetection import DetectAge
 
 class action(object):
     def __init__(self, incoming_message: str, profile_id: int, language: str, profile_curr_state: int, variables: Variable):
         self.incoming_message = incoming_message
         self.profile_id = profile_id
         self.language = language
         self.variables = variables
```

### Comparing `dialog-workflow-local-0.0.30/dialog_workflow/Constants.py` & `dialog-workflow-local-0.0.31/dialog_workflow/Constants.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.30/dialog_workflow/DialogWorkflow.py` & `dialog-workflow-local-0.0.31/dialog_workflow/DialogWorkflow.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.30/dialog_workflow/TablesAsObjects.py` & `dialog-workflow-local-0.0.31/dialog_workflow/TablesAsObjects.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.30/dialog_workflow/test.py` & `dialog-workflow-local-0.0.31/dialog_workflow/test.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.30/dialog_workflow/utils.py` & `dialog-workflow-local-0.0.31/dialog_workflow/utils.py`

 * *Files identical despite different names*

