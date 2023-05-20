# Comparing `tmp/openai_pygenerator-0.1.0.tar.gz` & `tmp/openai-pygenerator-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_pygenerator-0.1.0.tar", last modified: Fri May 19 15:54:07 2023, max compression
+gzip compressed data, was "openai-pygenerator-0.1.1.tar", last modified: Sat May 20 08:07:55 2023, max compression
```

## Comparing `openai_pygenerator-0.1.0.tar` & `openai-pygenerator-0.1.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:54:07.641098 openai_pygenerator-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:54:07.637098 openai_pygenerator-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:54:07.641098 openai_pygenerator-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-19 15:53:56.000000 openai_pygenerator-0.1.0/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-19 15:53:56.000000 openai_pygenerator-0.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-19 15:53:56.000000 openai_pygenerator-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-19 15:53:56.000000 openai_pygenerator-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    21334 2023-05-19 15:53:56.000000 openai_pygenerator-0.1.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-19 15:53:56.000000 openai_pygenerator-0.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-19 15:54:07.641098 openai_pygenerator-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-19 15:53:56.000000 openai_pygenerator-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:53:56.000000 openai_pygenerator-0.1.0/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-19 15:53:56.000000 openai_pygenerator-0.1.0/mypy-tests.ini
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-19 15:53:56.000000 openai_pygenerator-0.1.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-19 15:53:56.000000 openai_pygenerator-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-19 15:54:07.641098 openai_pygenerator-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-19 15:53:56.000000 openai_pygenerator-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:54:07.641098 openai_pygenerator-0.1.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-19 15:53:56.000000 openai_pygenerator-0.1.0/src/example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:54:07.641098 openai_pygenerator-0.1.0/src/openai_pygenerator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-19 15:54:07.000000 openai_pygenerator-0.1.0/src/openai_pygenerator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-19 15:54:07.000000 openai_pygenerator-0.1.0/src/openai_pygenerator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 15:54:07.000000 openai_pygenerator-0.1.0/src/openai_pygenerator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-19 15:54:07.000000 openai_pygenerator-0.1.0/src/openai_pygenerator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-19 15:54:07.000000 openai_pygenerator-0.1.0/src/openai_pygenerator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 15:54:07.000000 openai_pygenerator-0.1.0/src/openai_pygenerator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-19 15:53:56.000000 openai_pygenerator-0.1.0/src/openai_pygenerator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:54:07.641098 openai_pygenerator-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-19 15:53:56.000000 openai_pygenerator-0.1.0/tests/test_gpt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:07:55.347290 openai-pygenerator-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:07:55.343290 openai-pygenerator-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:07:55.343290 openai-pygenerator-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-20 08:07:40.000000 openai-pygenerator-0.1.1/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-20 08:07:40.000000 openai-pygenerator-0.1.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-20 08:07:40.000000 openai-pygenerator-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-20 08:07:40.000000 openai-pygenerator-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    21334 2023-05-20 08:07:40.000000 openai-pygenerator-0.1.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-20 08:07:40.000000 openai-pygenerator-0.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-20 08:07:55.347290 openai-pygenerator-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-20 08:07:40.000000 openai-pygenerator-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 08:07:40.000000 openai-pygenerator-0.1.1/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-20 08:07:40.000000 openai-pygenerator-0.1.1/mypy-tests.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-20 08:07:40.000000 openai-pygenerator-0.1.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-20 08:07:40.000000 openai-pygenerator-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-20 08:07:55.347290 openai-pygenerator-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-20 08:07:40.000000 openai-pygenerator-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:07:55.343290 openai-pygenerator-0.1.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-20 08:07:40.000000 openai-pygenerator-0.1.1/src/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:07:55.347290 openai-pygenerator-0.1.1/src/openai_pygenerator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-20 08:07:55.000000 openai-pygenerator-0.1.1/src/openai_pygenerator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-20 08:07:55.000000 openai-pygenerator-0.1.1/src/openai_pygenerator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 08:07:55.000000 openai-pygenerator-0.1.1/src/openai_pygenerator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-20 08:07:55.000000 openai-pygenerator-0.1.1/src/openai_pygenerator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-20 08:07:55.000000 openai-pygenerator-0.1.1/src/openai_pygenerator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 08:07:55.000000 openai-pygenerator-0.1.1/src/openai_pygenerator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-20 08:07:40.000000 openai-pygenerator-0.1.1/src/openai_pygenerator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:07:55.347290 openai-pygenerator-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-20 08:07:40.000000 openai-pygenerator-0.1.1/tests/test_gpt.py
```

### Comparing `openai_pygenerator-0.1.0/.github/workflows/python-package.yml` & `openai-pygenerator-0.1.1/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `openai_pygenerator-0.1.0/.github/workflows/python-publish.yml` & `openai-pygenerator-0.1.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `openai_pygenerator-0.1.0/.pre-commit-config.yaml` & `openai-pygenerator-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `openai_pygenerator-0.1.0/.pylintrc` & `openai-pygenerator-0.1.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `openai_pygenerator-0.1.0/LICENSE.txt` & `openai-pygenerator-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openai_pygenerator-0.1.0/PKG-INFO` & `openai-pygenerator-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
-Name: openai_pygenerator
-Version: 0.1.0
+Name: openai-pygenerator
+Version: 0.1.1
 Summary: Simple generator wrapper for OpenAI Python API with retry
 Author-email: Steve Phelps <sphelps@sphelps.net>
 Project-URL: Homepage, https://github.com/phelps-sg/openai-pygenerator
 Project-URL: Bug Tracker, https://github.com/phelps-sg/openai-pygenerator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 # openai-pygenerator
 
+[![GitHub Workflow Status](https://github.com/phelps-sg/openai-pygenerator/actions/workflows/python-package.yml/badge.svg)](https://github.com/phelps-sg/openai-generator/actions/workflows/continouos-integration.yml)
+![GitHub release (latest by date)](https://img.shields.io/github/v/release/phelps-sg/openai-pygenerator)
+![GitHub](https://img.shields.io/github/license/phelps-sg/openai-pygenerator?color=blue)
+
 This is a simple wrapper around the OpenAI Python API which provides
 type annotations, retry functionality and a generator over completions.
 
 
 ## Installation
 
 ~~~bash
```

### Comparing `openai_pygenerator-0.1.0/pyproject.toml` & `openai-pygenerator-0.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.setuptools_scm]
 write_to = "src/version.py"
 
 [tool.pytest.ini_options]
 pythonpath = "src"
 
 [project]
-name = "openai_pygenerator"
+name = "openai-pygenerator"
 dynamic = ["version"]
 
 authors = [
   { name="Steve Phelps", email="sphelps@sphelps.net" },
 ]
 description = "Simple generator wrapper for OpenAI Python API with retry"
 readme = "README.md"
```

### Comparing `openai_pygenerator-0.1.0/src/example.py` & `openai-pygenerator-0.1.1/src/example.py`

 * *Files identical despite different names*

### Comparing `openai_pygenerator-0.1.0/src/openai_pygenerator.egg-info/PKG-INFO` & `openai-pygenerator-0.1.1/src/openai_pygenerator.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: openai-pygenerator
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simple generator wrapper for OpenAI Python API with retry
 Author-email: Steve Phelps <sphelps@sphelps.net>
 Project-URL: Homepage, https://github.com/phelps-sg/openai-pygenerator
 Project-URL: Bug Tracker, https://github.com/phelps-sg/openai-pygenerator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 # openai-pygenerator
 
+[![GitHub Workflow Status](https://github.com/phelps-sg/openai-pygenerator/actions/workflows/python-package.yml/badge.svg)](https://github.com/phelps-sg/openai-generator/actions/workflows/continouos-integration.yml)
+![GitHub release (latest by date)](https://img.shields.io/github/v/release/phelps-sg/openai-pygenerator)
+![GitHub](https://img.shields.io/github/license/phelps-sg/openai-pygenerator?color=blue)
+
 This is a simple wrapper around the OpenAI Python API which provides
 type annotations, retry functionality and a generator over completions.
 
 
 ## Installation
 
 ~~~bash
```

### Comparing `openai_pygenerator-0.1.0/src/openai_pygenerator.egg-info/SOURCES.txt` & `openai-pygenerator-0.1.1/src/openai_pygenerator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openai_pygenerator-0.1.0/src/openai_pygenerator.py` & `openai-pygenerator-0.1.1/src/openai_pygenerator.py`

 * *Files identical despite different names*

### Comparing `openai_pygenerator-0.1.0/tests/test_gpt.py` & `openai-pygenerator-0.1.1/tests/test_gpt.py`

 * *Files identical despite different names*

