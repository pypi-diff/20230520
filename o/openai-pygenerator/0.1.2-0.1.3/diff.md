# Comparing `tmp/openai-pygenerator-0.1.2.tar.gz` & `tmp/openai-pygenerator-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai-pygenerator-0.1.2.tar", last modified: Sat May 20 08:34:54 2023, max compression
+gzip compressed data, was "openai-pygenerator-0.1.3.tar", last modified: Sat May 20 09:04:07 2023, max compression
```

## Comparing `openai-pygenerator-0.1.2.tar` & `openai-pygenerator-0.1.3.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:34:54.973235 openai-pygenerator-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:34:54.969236 openai-pygenerator-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:34:54.973235 openai-pygenerator-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-20 08:34:43.000000 openai-pygenerator-0.1.2/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-20 08:34:43.000000 openai-pygenerator-0.1.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-20 08:34:43.000000 openai-pygenerator-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-20 08:34:43.000000 openai-pygenerator-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    21334 2023-05-20 08:34:43.000000 openai-pygenerator-0.1.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-20 08:34:43.000000 openai-pygenerator-0.1.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-20 08:34:54.977235 openai-pygenerator-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-20 08:34:43.000000 openai-pygenerator-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 08:34:43.000000 openai-pygenerator-0.1.2/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-20 08:34:43.000000 openai-pygenerator-0.1.2/mypy-tests.ini
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-20 08:34:43.000000 openai-pygenerator-0.1.2/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-20 08:34:43.000000 openai-pygenerator-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-20 08:34:54.977235 openai-pygenerator-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-20 08:34:43.000000 openai-pygenerator-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:34:54.973235 openai-pygenerator-0.1.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-20 08:34:43.000000 openai-pygenerator-0.1.2/src/example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:34:54.973235 openai-pygenerator-0.1.2/src/openai_pygenerator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-20 08:34:54.000000 openai-pygenerator-0.1.2/src/openai_pygenerator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-20 08:34:54.000000 openai-pygenerator-0.1.2/src/openai_pygenerator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 08:34:54.000000 openai-pygenerator-0.1.2/src/openai_pygenerator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-20 08:34:54.000000 openai-pygenerator-0.1.2/src/openai_pygenerator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-20 08:34:54.000000 openai-pygenerator-0.1.2/src/openai_pygenerator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 08:34:54.000000 openai-pygenerator-0.1.2/src/openai_pygenerator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-20 08:34:43.000000 openai-pygenerator-0.1.2/src/openai_pygenerator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:34:54.973235 openai-pygenerator-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-20 08:34:43.000000 openai-pygenerator-0.1.2/tests/test_gpt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:04:07.812879 openai-pygenerator-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:04:07.808879 openai-pygenerator-0.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:04:07.812879 openai-pygenerator-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-20 09:03:57.000000 openai-pygenerator-0.1.3/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-20 09:03:57.000000 openai-pygenerator-0.1.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-20 09:03:57.000000 openai-pygenerator-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-20 09:03:57.000000 openai-pygenerator-0.1.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    21334 2023-05-20 09:03:57.000000 openai-pygenerator-0.1.3/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-20 09:03:57.000000 openai-pygenerator-0.1.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-20 09:04:07.812879 openai-pygenerator-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-20 09:03:57.000000 openai-pygenerator-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 09:03:57.000000 openai-pygenerator-0.1.3/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-20 09:03:57.000000 openai-pygenerator-0.1.3/mypy-tests.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-20 09:03:57.000000 openai-pygenerator-0.1.3/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-20 09:03:57.000000 openai-pygenerator-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-20 09:04:07.812879 openai-pygenerator-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-20 09:03:57.000000 openai-pygenerator-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:04:07.808879 openai-pygenerator-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:04:07.812879 openai-pygenerator-0.1.3/src/openai_pygenerator/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-20 09:03:57.000000 openai-pygenerator-0.1.3/src/openai_pygenerator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-20 09:03:57.000000 openai-pygenerator-0.1.3/src/openai_pygenerator/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-20 09:03:57.000000 openai-pygenerator-0.1.3/src/openai_pygenerator/openai_pygenerator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:04:07.812879 openai-pygenerator-0.1.3/src/openai_pygenerator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-20 09:04:07.000000 openai-pygenerator-0.1.3/src/openai_pygenerator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-20 09:04:07.000000 openai-pygenerator-0.1.3/src/openai_pygenerator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 09:04:07.000000 openai-pygenerator-0.1.3/src/openai_pygenerator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-20 09:04:07.000000 openai-pygenerator-0.1.3/src/openai_pygenerator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-20 09:04:07.000000 openai-pygenerator-0.1.3/src/openai_pygenerator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-20 09:04:07.000000 openai-pygenerator-0.1.3/src/openai_pygenerator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:04:07.812879 openai-pygenerator-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-20 09:03:57.000000 openai-pygenerator-0.1.3/tests/test_gpt.py
```

### Comparing `openai-pygenerator-0.1.2/.github/workflows/python-package.yml` & `openai-pygenerator-0.1.3/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.1.2/.github/workflows/python-publish.yml` & `openai-pygenerator-0.1.3/.github/workflows/python-publish.yml`

 * *Files 8% similar despite different names*

```diff
@@ -40,12 +40,13 @@
         setuptools_scm
         --user
     - name: Build a binary wheel and a source tarball
       run: >-
         python -m
         build
         --sdist
+        --wheel
         --outdir dist/
         .
     - name: Publish package distributions to PyPI
       if: startsWith(github.ref, 'refs/tags')
       uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `openai-pygenerator-0.1.2/.pre-commit-config.yaml` & `openai-pygenerator-0.1.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.1.2/.pylintrc` & `openai-pygenerator-0.1.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.1.2/LICENSE.txt` & `openai-pygenerator-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.1.2/PKG-INFO` & `openai-pygenerator-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-pygenerator
-Version: 0.1.2
+Version: 0.1.3
 Summary: Simple generator wrapper for OpenAI Python API with retry
 Author-email: Steve Phelps <sphelps@sphelps.net>
 Project-URL: Homepage, https://github.com/phelps-sg/openai-pygenerator
 Project-URL: Bug Tracker, https://github.com/phelps-sg/openai-pygenerator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -39,15 +39,15 @@
 print(solution)
 working = session.ask("Show your working")
 print(working)
 print("Transcript:")
 print(session.transcript)
 ~~~
 
-For an example of overriding parameters see [src/example.py](src/example.py).
+For an example of overriding parameters see [src/example.py](src/openai_pygenerator/example.py).
 
 ## Running 
 
 ~~~bash
 export OPENAI_API_KEY=<key>
 python src/example.py
 ~~~
```

### Comparing `openai-pygenerator-0.1.2/README.md` & `openai-pygenerator-0.1.3/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 print(solution)
 working = session.ask("Show your working")
 print(working)
 print("Transcript:")
 print(session.transcript)
 ~~~
 
-For an example of overriding parameters see [src/example.py](src/example.py).
+For an example of overriding parameters see [src/example.py](src/openai_pygenerator/example.py).
 
 ## Running 
 
 ~~~bash
 export OPENAI_API_KEY=<key>
 python src/example.py
 ~~~
```

### Comparing `openai-pygenerator-0.1.2/pyproject.toml` & `openai-pygenerator-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.1.2/src/example.py` & `openai-pygenerator-0.1.3/src/openai_pygenerator/example.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from openai_pygenerator import ChatSession, completer
+from openai_pygenerator.openai_pygenerator import ChatSession, completer
 
 
 def heading(message: str, margin: int = 80) -> None:
     print()
     print("-" * margin)
     print(message)
     print("-" * margin)
```

### Comparing `openai-pygenerator-0.1.2/src/openai_pygenerator.egg-info/PKG-INFO` & `openai-pygenerator-0.1.3/src/openai_pygenerator.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-pygenerator
-Version: 0.1.2
+Version: 0.1.3
 Summary: Simple generator wrapper for OpenAI Python API with retry
 Author-email: Steve Phelps <sphelps@sphelps.net>
 Project-URL: Homepage, https://github.com/phelps-sg/openai-pygenerator
 Project-URL: Bug Tracker, https://github.com/phelps-sg/openai-pygenerator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -39,15 +39,15 @@
 print(solution)
 working = session.ask("Show your working")
 print(working)
 print("Transcript:")
 print(session.transcript)
 ~~~
 
-For an example of overriding parameters see [src/example.py](src/example.py).
+For an example of overriding parameters see [src/example.py](src/openai_pygenerator/example.py).
 
 ## Running 
 
 ~~~bash
 export OPENAI_API_KEY=<key>
 python src/example.py
 ~~~
```

### Comparing `openai-pygenerator-0.1.2/src/openai_pygenerator.egg-info/SOURCES.txt` & `openai-pygenerator-0.1.3/src/openai_pygenerator.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 mypy-tests.ini
 mypy.ini
 pyproject.toml
 setup.cfg
 setup.py
 .github/workflows/python-package.yml
 .github/workflows/python-publish.yml
-src/example.py
-src/openai_pygenerator.py
+src/openai_pygenerator/__init__.py
+src/openai_pygenerator/example.py
+src/openai_pygenerator/openai_pygenerator.py
 src/openai_pygenerator.egg-info/PKG-INFO
 src/openai_pygenerator.egg-info/SOURCES.txt
 src/openai_pygenerator.egg-info/dependency_links.txt
 src/openai_pygenerator.egg-info/entry_points.txt
 src/openai_pygenerator.egg-info/requires.txt
 src/openai_pygenerator.egg-info/top_level.txt
 tests/test_gpt.py
```

### Comparing `openai-pygenerator-0.1.2/src/openai_pygenerator.py` & `openai-pygenerator-0.1.3/src/openai_pygenerator/openai_pygenerator.py`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.1.2/tests/test_gpt.py` & `openai-pygenerator-0.1.3/tests/test_gpt.py`

 * *Files identical despite different names*

