# Comparing `tmp/molecule_multipass-0.0.0.tar.gz` & `tmp/molecule_multipass-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molecule_multipass-0.0.0.tar", last modified: Sat May 20 13:26:47 2023, max compression
+gzip compressed data, was "molecule_multipass-0.1.0.tar", last modified: Sat May 20 13:22:58 2023, max compression
```

## Comparing `molecule_multipass-0.0.0.tar` & `molecule_multipass-0.1.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:26:47.451094 molecule_multipass-0.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:26:47.447094 molecule_multipass-0.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:26:47.451094 molecule_multipass-0.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-20 13:26:37.000000 molecule_multipass-0.0.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-20 13:26:37.000000 molecule_multipass-0.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-20 13:26:37.000000 molecule_multipass-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-20 13:26:47.451094 molecule_multipass-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 13:26:37.000000 molecule_multipass-0.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:26:47.451094 molecule_multipass-0.0.0/molecule_multipass/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 13:26:37.000000 molecule_multipass-0.0.0/molecule_multipass/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:26:47.451094 molecule_multipass-0.0.0/molecule_multipass/cookiecutter/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-20 13:26:37.000000 molecule_multipass-0.0.0/molecule_multipass/cookiecutter/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:26:47.447094 molecule_multipass-0.0.0/molecule_multipass/cookiecutter/{{cookiecutter.molecule_directory}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:26:47.451094 molecule_multipass-0.0.0/molecule_multipass/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 13:26:37.000000 molecule_multipass-0.0.0/molecule_multipass/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-20 13:26:37.000000 molecule_multipass-0.0.0/molecule_multipass/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:26:47.451094 molecule_multipass-0.0.0/molecule_multipass/playbooks/
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-20 13:26:37.000000 molecule_multipass-0.0.0/molecule_multipass/playbooks/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-05-20 13:26:37.000000 molecule_multipass-0.0.0/molecule_multipass/playbooks/destroy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:26:47.451094 molecule_multipass-0.0.0/molecule_multipass/playbooks/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-20 13:26:37.000000 molecule_multipass-0.0.0/molecule_multipass/playbooks/templates/cloud-init.yml.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:26:47.451094 molecule_multipass-0.0.0/molecule_multipass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-20 13:26:47.000000 molecule_multipass-0.0.0/molecule_multipass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-20 13:26:47.000000 molecule_multipass-0.0.0/molecule_multipass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 13:26:47.000000 molecule_multipass-0.0.0/molecule_multipass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-20 13:26:47.000000 molecule_multipass-0.0.0/molecule_multipass.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-20 13:26:47.000000 molecule_multipass-0.0.0/molecule_multipass.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-20 13:26:47.000000 molecule_multipass-0.0.0/molecule_multipass.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-20 13:26:37.000000 molecule_multipass-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 13:26:47.451094 molecule_multipass-0.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:22:58.260431 molecule_multipass-0.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:22:58.256431 molecule_multipass-0.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:22:58.256431 molecule_multipass-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-20 13:22:47.000000 molecule_multipass-0.1.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-20 13:22:47.000000 molecule_multipass-0.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-20 13:22:47.000000 molecule_multipass-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-20 13:22:58.260431 molecule_multipass-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 13:22:47.000000 molecule_multipass-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:22:58.256431 molecule_multipass-0.1.0/molecule_multipass/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 13:22:47.000000 molecule_multipass-0.1.0/molecule_multipass/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:22:58.260431 molecule_multipass-0.1.0/molecule_multipass/cookiecutter/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-20 13:22:47.000000 molecule_multipass-0.1.0/molecule_multipass/cookiecutter/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:22:58.256431 molecule_multipass-0.1.0/molecule_multipass/cookiecutter/{{cookiecutter.molecule_directory}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:22:58.260431 molecule_multipass-0.1.0/molecule_multipass/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 13:22:47.000000 molecule_multipass-0.1.0/molecule_multipass/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-20 13:22:47.000000 molecule_multipass-0.1.0/molecule_multipass/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:22:58.260431 molecule_multipass-0.1.0/molecule_multipass/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-20 13:22:47.000000 molecule_multipass-0.1.0/molecule_multipass/playbooks/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-05-20 13:22:47.000000 molecule_multipass-0.1.0/molecule_multipass/playbooks/destroy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:22:58.260431 molecule_multipass-0.1.0/molecule_multipass/playbooks/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-20 13:22:47.000000 molecule_multipass-0.1.0/molecule_multipass/playbooks/templates/cloud-init.yml.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:22:58.260431 molecule_multipass-0.1.0/molecule_multipass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-20 13:22:58.000000 molecule_multipass-0.1.0/molecule_multipass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-20 13:22:58.000000 molecule_multipass-0.1.0/molecule_multipass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 13:22:58.000000 molecule_multipass-0.1.0/molecule_multipass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-20 13:22:58.000000 molecule_multipass-0.1.0/molecule_multipass.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-20 13:22:58.000000 molecule_multipass-0.1.0/molecule_multipass.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-20 13:22:58.000000 molecule_multipass-0.1.0/molecule_multipass.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-20 13:22:47.000000 molecule_multipass-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 13:22:58.260431 molecule_multipass-0.1.0/setup.cfg
```

### Comparing `molecule_multipass-0.0.0/.github/workflows/python-publish.yml` & `molecule_multipass-0.1.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `molecule_multipass-0.0.0/.gitignore` & `molecule_multipass-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `molecule_multipass-0.0.0/LICENSE` & `molecule_multipass-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `molecule_multipass-0.0.0/molecule_multipass/driver.py` & `molecule_multipass-0.1.0/molecule_multipass/driver.py`

 * *Files identical despite different names*

### Comparing `molecule_multipass-0.0.0/molecule_multipass/playbooks/create.yml` & `molecule_multipass-0.1.0/molecule_multipass/playbooks/create.yml`

 * *Files identical despite different names*

### Comparing `molecule_multipass-0.0.0/molecule_multipass/playbooks/destroy.yml` & `molecule_multipass-0.1.0/molecule_multipass/playbooks/destroy.yml`

 * *Files identical despite different names*

### Comparing `molecule_multipass-0.0.0/molecule_multipass.egg-info/SOURCES.txt` & `molecule_multipass-0.1.0/molecule_multipass.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `molecule_multipass-0.0.0/pyproject.toml` & `molecule_multipass-0.1.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   "setuptools_scm[toml] >= 7.0.5",
   "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "molecule_multipass"
-dynamic = ["version"]
+version = "0.1.0"
 description = "Molecule Multipass"
 authors = [{ "name" = "Andrey Gubarev", "email" = "andrey@andreygubarev.com" }]
 
 readme = "README.md"
 license = { text = "MIT" }
 
 dependencies = ["molecule >= 5.0"]
```

