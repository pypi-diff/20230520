# Comparing `tmp/passagerole-0.0.1.tar.gz` & `tmp/passagerole-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "passagerole-0.0.1.tar", last modified: Fri May 19 22:09:49 2023, max compression
+gzip compressed data, was "passagerole-0.0.2.tar", last modified: Sat May 20 20:35:35 2023, max compression
```

## Comparing `passagerole-0.0.1.tar` & `passagerole-0.0.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-19 22:09:49.974933 passagerole-0.0.1/
--rw-r--r--   0 mtm        (501) staff       (20)      594 2023-05-19 16:23:15.000000 passagerole-0.0.1/.coveragerc
--rw-r--r--   0 mtm        (501) staff       (20)      582 2023-05-19 17:14:53.000000 passagerole-0.0.1/.gitignore
--rw-r--r--   0 mtm        (501) staff       (20)       59 2023-05-19 16:23:15.000000 passagerole-0.0.1/.isort.cfg
--rw-r--r--   0 mtm        (501) staff       (20)     1670 2023-05-19 16:32:45.000000 passagerole-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0 mtm        (501) staff       (20)      530 2023-05-19 16:23:15.000000 passagerole-0.0.1/.readthedocs.yml
--rw-r--r--   0 mtm        (501) staff       (20)       87 2023-05-19 16:23:15.000000 passagerole-0.0.1/AUTHORS.rst
--rw-r--r--   0 mtm        (501) staff       (20)      128 2023-05-19 16:23:15.000000 passagerole-0.0.1/CHANGELOG.rst
--rw-r--r--   0 mtm        (501) staff       (20)    13866 2023-05-19 16:23:15.000000 passagerole-0.0.1/CONTRIBUTING.rst
--rw-r--r--   0 mtm        (501) staff       (20)     1083 2023-05-19 16:23:15.000000 passagerole-0.0.1/LICENSE.txt
--rw-r--r--   0 mtm        (501) staff       (20)     2598 2023-05-19 22:09:49.975195 passagerole-0.0.1/PKG-INFO
--rw-r--r--   0 mtm        (501) staff       (20)     2118 2023-05-19 16:23:15.000000 passagerole-0.0.1/README.rst
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-19 22:09:49.964332 passagerole-0.0.1/docs/
--rw-r--r--   0 mtm        (501) staff       (20)     1154 2023-05-19 16:23:15.000000 passagerole-0.0.1/docs/Makefile
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-19 22:09:49.965736 passagerole-0.0.1/docs/_static/
--rw-r--r--   0 mtm        (501) staff       (20)       18 2023-05-19 16:23:15.000000 passagerole-0.0.1/docs/_static/.gitignore
--rw-r--r--   0 mtm        (501) staff       (20)       41 2023-05-19 16:23:15.000000 passagerole-0.0.1/docs/authors.rst
--rw-r--r--   0 mtm        (501) staff       (20)       43 2023-05-19 16:23:15.000000 passagerole-0.0.1/docs/changelog.rst
--rw-r--r--   0 mtm        (501) staff       (20)     9799 2023-05-19 19:52:15.000000 passagerole-0.0.1/docs/conf.py
--rw-r--r--   0 mtm        (501) staff       (20)       33 2023-05-19 16:23:15.000000 passagerole-0.0.1/docs/contributing.rst
--rw-r--r--   0 mtm        (501) staff       (20)     2329 2023-05-19 16:23:15.000000 passagerole-0.0.1/docs/index.rst
--rw-r--r--   0 mtm        (501) staff       (20)       67 2023-05-19 16:23:15.000000 passagerole-0.0.1/docs/license.rst
--rw-r--r--   0 mtm        (501) staff       (20)       39 2023-05-19 16:23:15.000000 passagerole-0.0.1/docs/readme.rst
--rw-r--r--   0 mtm        (501) staff       (20)      233 2023-05-19 16:23:15.000000 passagerole-0.0.1/docs/requirements.txt
--rw-r--r--   0 mtm        (501) staff       (20)      346 2023-05-19 16:23:15.000000 passagerole-0.0.1/pyproject.toml
--rw-r--r--   0 mtm        (501) staff       (20)     1263 2023-05-19 22:09:49.976722 passagerole-0.0.1/setup.cfg
--rw-r--r--   0 mtm        (501) staff       (20)      706 2023-05-19 16:23:15.000000 passagerole-0.0.1/setup.py
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-19 22:09:49.941875 passagerole-0.0.1/src/
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-19 22:09:49.967832 passagerole-0.0.1/src/passagerole/
--rw-r--r--   0 mtm        (501) staff       (20)      577 2023-05-19 16:23:15.000000 passagerole-0.0.1/src/passagerole/__init__.py
--rw-r--r--   0 mtm        (501) staff       (20)     1801 2023-05-19 19:53:20.000000 passagerole-0.0.1/src/passagerole/lib.py
--rw-r--r--   0 mtm        (501) staff       (20)     4570 2023-05-19 19:45:08.000000 passagerole-0.0.1/src/passagerole/main.py
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-19 22:09:49.972627 passagerole-0.0.1/src/passagerole/templates/
--rw-r--r--   0 mtm        (501) staff       (20)      508 2023-05-19 17:36:10.000000 passagerole-0.0.1/src/passagerole/templates/authorized_keys_dummy_data
--rw-r--r--   0 mtm        (501) staff       (20)     1300 2023-05-19 18:52:15.000000 passagerole-0.0.1/src/passagerole/templates/userdata_bash_ssh_keys.sh.j2
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-19 22:09:49.971423 passagerole-0.0.1/src/passagerole.egg-info/
--rw-r--r--   0 mtm        (501) staff       (20)     2598 2023-05-19 22:09:49.000000 passagerole-0.0.1/src/passagerole.egg-info/PKG-INFO
--rw-r--r--   0 mtm        (501) staff       (20)      859 2023-05-19 22:09:49.000000 passagerole-0.0.1/src/passagerole.egg-info/SOURCES.txt
--rw-r--r--   0 mtm        (501) staff       (20)        1 2023-05-19 22:09:49.000000 passagerole-0.0.1/src/passagerole.egg-info/dependency_links.txt
--rw-r--r--   0 mtm        (501) staff       (20)       53 2023-05-19 22:09:49.000000 passagerole-0.0.1/src/passagerole.egg-info/entry_points.txt
--rw-r--r--   0 mtm        (501) staff       (20)        1 2023-05-19 22:09:49.000000 passagerole-0.0.1/src/passagerole.egg-info/not-zip-safe
--rw-r--r--   0 mtm        (501) staff       (20)       93 2023-05-19 22:09:49.000000 passagerole-0.0.1/src/passagerole.egg-info/requires.txt
--rw-r--r--   0 mtm        (501) staff       (20)       12 2023-05-19 22:09:49.000000 passagerole-0.0.1/src/passagerole.egg-info/top_level.txt
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-19 22:09:49.974388 passagerole-0.0.1/tests/
--rw-r--r--   0 mtm        (501) staff       (20)      279 2023-05-19 16:23:15.000000 passagerole-0.0.1/tests/conftest.py
--rw-r--r--   0 mtm        (501) staff       (20)      596 2023-05-19 16:23:15.000000 passagerole-0.0.1/tests/test_skeleton.py
--rw-r--r--   0 mtm        (501) staff       (20)     2851 2023-05-19 16:23:15.000000 passagerole-0.0.1/tox.ini
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-20 20:35:35.290926 passagerole-0.0.2/
+-rw-r--r--   0 mtm        (501) staff       (20)      594 2023-05-19 16:23:15.000000 passagerole-0.0.2/.coveragerc
+-rw-r--r--   0 mtm        (501) staff       (20)      582 2023-05-19 17:14:53.000000 passagerole-0.0.2/.gitignore
+-rw-r--r--   0 mtm        (501) staff       (20)       59 2023-05-19 16:23:15.000000 passagerole-0.0.2/.isort.cfg
+-rw-r--r--   0 mtm        (501) staff       (20)     1670 2023-05-19 16:32:45.000000 passagerole-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 mtm        (501) staff       (20)      530 2023-05-19 16:23:15.000000 passagerole-0.0.2/.readthedocs.yml
+-rw-r--r--   0 mtm        (501) staff       (20)       87 2023-05-19 16:23:15.000000 passagerole-0.0.2/AUTHORS.rst
+-rw-r--r--   0 mtm        (501) staff       (20)      128 2023-05-19 16:23:15.000000 passagerole-0.0.2/CHANGELOG.rst
+-rw-r--r--   0 mtm        (501) staff       (20)    13866 2023-05-19 16:23:15.000000 passagerole-0.0.2/CONTRIBUTING.rst
+-rw-r--r--   0 mtm        (501) staff       (20)     1083 2023-05-19 16:23:15.000000 passagerole-0.0.2/LICENSE.txt
+-rw-r--r--   0 mtm        (501) staff       (20)     2598 2023-05-20 20:35:35.291288 passagerole-0.0.2/PKG-INFO
+-rw-r--r--   0 mtm        (501) staff       (20)     2118 2023-05-19 16:23:15.000000 passagerole-0.0.2/README.rst
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-20 20:35:35.267713 passagerole-0.0.2/docs/
+-rw-r--r--   0 mtm        (501) staff       (20)     1154 2023-05-19 16:23:15.000000 passagerole-0.0.2/docs/Makefile
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-20 20:35:35.278761 passagerole-0.0.2/docs/_static/
+-rw-r--r--   0 mtm        (501) staff       (20)       18 2023-05-19 16:23:15.000000 passagerole-0.0.2/docs/_static/.gitignore
+-rw-r--r--   0 mtm        (501) staff       (20)       41 2023-05-19 16:23:15.000000 passagerole-0.0.2/docs/authors.rst
+-rw-r--r--   0 mtm        (501) staff       (20)       43 2023-05-19 16:23:15.000000 passagerole-0.0.2/docs/changelog.rst
+-rw-r--r--   0 mtm        (501) staff       (20)     9799 2023-05-19 19:52:15.000000 passagerole-0.0.2/docs/conf.py
+-rw-r--r--   0 mtm        (501) staff       (20)       33 2023-05-19 16:23:15.000000 passagerole-0.0.2/docs/contributing.rst
+-rw-r--r--   0 mtm        (501) staff       (20)     2329 2023-05-19 16:23:15.000000 passagerole-0.0.2/docs/index.rst
+-rw-r--r--   0 mtm        (501) staff       (20)       67 2023-05-19 16:23:15.000000 passagerole-0.0.2/docs/license.rst
+-rw-r--r--   0 mtm        (501) staff       (20)       39 2023-05-19 16:23:15.000000 passagerole-0.0.2/docs/readme.rst
+-rw-r--r--   0 mtm        (501) staff       (20)      233 2023-05-19 16:23:15.000000 passagerole-0.0.2/docs/requirements.txt
+-rw-r--r--   0 mtm        (501) staff       (20)      346 2023-05-19 16:23:15.000000 passagerole-0.0.2/pyproject.toml
+-rw-r--r--   0 mtm        (501) staff       (20)     1263 2023-05-20 20:35:35.293558 passagerole-0.0.2/setup.cfg
+-rw-r--r--   0 mtm        (501) staff       (20)      706 2023-05-19 16:23:15.000000 passagerole-0.0.2/setup.py
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-20 20:35:35.228257 passagerole-0.0.2/src/
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-20 20:35:35.281285 passagerole-0.0.2/src/passagerole/
+-rw-r--r--   0 mtm        (501) staff       (20)      577 2023-05-19 16:23:15.000000 passagerole-0.0.2/src/passagerole/__init__.py
+-rw-r--r--   0 mtm        (501) staff       (20)     1856 2023-05-20 20:35:07.000000 passagerole-0.0.2/src/passagerole/lib.py
+-rw-r--r--   0 mtm        (501) staff       (20)     4570 2023-05-19 19:45:08.000000 passagerole-0.0.2/src/passagerole/main.py
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-20 20:35:35.288978 passagerole-0.0.2/src/passagerole/templates/
+-rw-r--r--   0 mtm        (501) staff       (20)      508 2023-05-19 17:36:10.000000 passagerole-0.0.2/src/passagerole/templates/authorized_keys_dummy_data
+-rw-r--r--   0 mtm        (501) staff       (20)     1300 2023-05-19 18:52:15.000000 passagerole-0.0.2/src/passagerole/templates/userdata_bash_ssh_keys.sh.j2
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-20 20:35:35.286577 passagerole-0.0.2/src/passagerole.egg-info/
+-rw-r--r--   0 mtm        (501) staff       (20)     2598 2023-05-20 20:35:35.000000 passagerole-0.0.2/src/passagerole.egg-info/PKG-INFO
+-rw-r--r--   0 mtm        (501) staff       (20)      859 2023-05-20 20:35:35.000000 passagerole-0.0.2/src/passagerole.egg-info/SOURCES.txt
+-rw-r--r--   0 mtm        (501) staff       (20)        1 2023-05-20 20:35:35.000000 passagerole-0.0.2/src/passagerole.egg-info/dependency_links.txt
+-rw-r--r--   0 mtm        (501) staff       (20)       53 2023-05-20 20:35:35.000000 passagerole-0.0.2/src/passagerole.egg-info/entry_points.txt
+-rw-r--r--   0 mtm        (501) staff       (20)        1 2023-05-20 20:35:34.000000 passagerole-0.0.2/src/passagerole.egg-info/not-zip-safe
+-rw-r--r--   0 mtm        (501) staff       (20)       93 2023-05-20 20:35:35.000000 passagerole-0.0.2/src/passagerole.egg-info/requires.txt
+-rw-r--r--   0 mtm        (501) staff       (20)       12 2023-05-20 20:35:35.000000 passagerole-0.0.2/src/passagerole.egg-info/top_level.txt
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-20 20:35:35.290440 passagerole-0.0.2/tests/
+-rw-r--r--   0 mtm        (501) staff       (20)      279 2023-05-19 16:23:15.000000 passagerole-0.0.2/tests/conftest.py
+-rw-r--r--   0 mtm        (501) staff       (20)      596 2023-05-19 16:23:15.000000 passagerole-0.0.2/tests/test_skeleton.py
+-rw-r--r--   0 mtm        (501) staff       (20)     2851 2023-05-19 16:23:15.000000 passagerole-0.0.2/tox.ini
```

### Comparing `passagerole-0.0.1/.coveragerc` & `passagerole-0.0.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `passagerole-0.0.1/.gitignore` & `passagerole-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `passagerole-0.0.1/.pre-commit-config.yaml` & `passagerole-0.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `passagerole-0.0.1/.readthedocs.yml` & `passagerole-0.0.2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `passagerole-0.0.1/CONTRIBUTING.rst` & `passagerole-0.0.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `passagerole-0.0.1/LICENSE.txt` & `passagerole-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `passagerole-0.0.1/PKG-INFO` & `passagerole-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: passagerole
-Version: 0.0.1
+Version: 0.0.2
 Summary: Add a short description here!
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Taylor Monacelli
 Author-email: taylormonacelli@gmail.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `passagerole-0.0.1/README.rst` & `passagerole-0.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `passagerole-0.0.1/docs/Makefile` & `passagerole-0.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `passagerole-0.0.1/docs/conf.py` & `passagerole-0.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `passagerole-0.0.1/docs/index.rst` & `passagerole-0.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `passagerole-0.0.1/setup.cfg` & `passagerole-0.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `passagerole-0.0.1/setup.py` & `passagerole-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `passagerole-0.0.1/src/passagerole/__init__.py` & `passagerole-0.0.2/src/passagerole/__init__.py`

 * *Files identical despite different names*

### Comparing `passagerole-0.0.1/src/passagerole/main.py` & `passagerole-0.0.2/src/passagerole/main.py`

 * *Files identical despite different names*

### Comparing `passagerole-0.0.1/src/passagerole/templates/userdata_bash_ssh_keys.sh.j2` & `passagerole-0.0.2/src/passagerole/templates/userdata_bash_ssh_keys.sh.j2`

 * *Files identical despite different names*

### Comparing `passagerole-0.0.1/src/passagerole.egg-info/PKG-INFO` & `passagerole-0.0.2/src/passagerole.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: passagerole
-Version: 0.0.1
+Version: 0.0.2
 Summary: Add a short description here!
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Taylor Monacelli
 Author-email: taylormonacelli@gmail.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `passagerole-0.0.1/src/passagerole.egg-info/SOURCES.txt` & `passagerole-0.0.2/src/passagerole.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `passagerole-0.0.1/tests/test_skeleton.py` & `passagerole-0.0.2/tests/test_skeleton.py`

 * *Files identical despite different names*

### Comparing `passagerole-0.0.1/tox.ini` & `passagerole-0.0.2/tox.ini`

 * *Files identical despite different names*

