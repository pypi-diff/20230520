# Comparing `tmp/molecule_multipass-0.3.5.tar.gz` & `tmp/molecule_multipass-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molecule_multipass-0.3.5.tar", last modified: Sat May 20 14:00:13 2023, max compression
+gzip compressed data, was "molecule_multipass-0.4.0.tar", last modified: Sat May 20 14:11:19 2023, max compression
```

## Comparing `molecule_multipass-0.3.5.tar` & `molecule_multipass-0.4.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:00:13.754064 molecule_multipass-0.3.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:00:13.750064 molecule_multipass-0.3.5/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-20 14:00:03.000000 molecule_multipass-0.3.5/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:00:13.750064 molecule_multipass-0.3.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-20 14:00:03.000000 molecule_multipass-0.3.5/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-20 14:00:03.000000 molecule_multipass-0.3.5/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-20 14:00:03.000000 molecule_multipass-0.3.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-20 14:00:03.000000 molecule_multipass-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-20 14:00:13.754064 molecule_multipass-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 14:00:03.000000 molecule_multipass-0.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:00:13.750064 molecule_multipass-0.3.5/molecule_multipass/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 14:00:03.000000 molecule_multipass-0.3.5/molecule_multipass/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:00:13.754064 molecule_multipass-0.3.5/molecule_multipass/cookiecutter/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-20 14:00:03.000000 molecule_multipass-0.3.5/molecule_multipass/cookiecutter/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:00:13.750064 molecule_multipass-0.3.5/molecule_multipass/cookiecutter/{{cookiecutter.molecule_directory}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:00:13.754064 molecule_multipass-0.3.5/molecule_multipass/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 14:00:03.000000 molecule_multipass-0.3.5/molecule_multipass/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-20 14:00:03.000000 molecule_multipass-0.3.5/molecule_multipass/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:00:13.754064 molecule_multipass-0.3.5/molecule_multipass/playbooks/
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-20 14:00:03.000000 molecule_multipass-0.3.5/molecule_multipass/playbooks/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-05-20 14:00:03.000000 molecule_multipass-0.3.5/molecule_multipass/playbooks/destroy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:00:13.754064 molecule_multipass-0.3.5/molecule_multipass/playbooks/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-20 14:00:03.000000 molecule_multipass-0.3.5/molecule_multipass/playbooks/templates/cloud-init.yml.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:00:13.750064 molecule_multipass-0.3.5/molecule_multipass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-20 14:00:13.000000 molecule_multipass-0.3.5/molecule_multipass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-20 14:00:13.000000 molecule_multipass-0.3.5/molecule_multipass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 14:00:13.000000 molecule_multipass-0.3.5/molecule_multipass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-20 14:00:13.000000 molecule_multipass-0.3.5/molecule_multipass.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-20 14:00:13.000000 molecule_multipass-0.3.5/molecule_multipass.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-20 14:00:13.000000 molecule_multipass-0.3.5/molecule_multipass.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-20 14:00:03.000000 molecule_multipass-0.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 14:00:13.754064 molecule_multipass-0.3.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:11:19.143421 molecule_multipass-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:11:19.135421 molecule_multipass-0.4.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-20 14:11:07.000000 molecule_multipass-0.4.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:11:19.135421 molecule_multipass-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-20 14:11:07.000000 molecule_multipass-0.4.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-20 14:11:07.000000 molecule_multipass-0.4.0/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-20 14:11:07.000000 molecule_multipass-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-20 14:11:07.000000 molecule_multipass-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-20 14:11:19.143421 molecule_multipass-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 14:11:07.000000 molecule_multipass-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:11:19.135421 molecule_multipass-0.4.0/molecule_multipass/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 14:11:07.000000 molecule_multipass-0.4.0/molecule_multipass/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:11:19.139421 molecule_multipass-0.4.0/molecule_multipass/cookiecutter/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-20 14:11:07.000000 molecule_multipass-0.4.0/molecule_multipass/cookiecutter/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:11:19.131420 molecule_multipass-0.4.0/molecule_multipass/cookiecutter/{{cookiecutter.molecule_directory}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:11:19.139421 molecule_multipass-0.4.0/molecule_multipass/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 14:11:07.000000 molecule_multipass-0.4.0/molecule_multipass/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-20 14:11:07.000000 molecule_multipass-0.4.0/molecule_multipass/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/prepare.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-20 14:11:07.000000 molecule_multipass-0.4.0/molecule_multipass/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:11:19.139421 molecule_multipass-0.4.0/molecule_multipass/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-20 14:11:07.000000 molecule_multipass-0.4.0/molecule_multipass/playbooks/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-05-20 14:11:07.000000 molecule_multipass-0.4.0/molecule_multipass/playbooks/destroy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:11:19.139421 molecule_multipass-0.4.0/molecule_multipass/playbooks/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-20 14:11:07.000000 molecule_multipass-0.4.0/molecule_multipass/playbooks/templates/cloud-init.yml.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:11:19.139421 molecule_multipass-0.4.0/molecule_multipass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-20 14:11:19.000000 molecule_multipass-0.4.0/molecule_multipass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-20 14:11:19.000000 molecule_multipass-0.4.0/molecule_multipass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 14:11:19.000000 molecule_multipass-0.4.0/molecule_multipass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-20 14:11:19.000000 molecule_multipass-0.4.0/molecule_multipass.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-20 14:11:19.000000 molecule_multipass-0.4.0/molecule_multipass.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-20 14:11:19.000000 molecule_multipass-0.4.0/molecule_multipass.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-20 14:11:07.000000 molecule_multipass-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 14:11:19.143421 molecule_multipass-0.4.0/setup.cfg
```

### Comparing `molecule_multipass-0.3.5/.github/workflows/python-publish.yml` & `molecule_multipass-0.4.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `molecule_multipass-0.3.5/.gitignore` & `molecule_multipass-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `molecule_multipass-0.3.5/LICENSE` & `molecule_multipass-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `molecule_multipass-0.3.5/molecule_multipass/driver.py` & `molecule_multipass-0.4.0/molecule_multipass/driver.py`

 * *Files identical despite different names*

### Comparing `molecule_multipass-0.3.5/molecule_multipass/playbooks/create.yml` & `molecule_multipass-0.4.0/molecule_multipass/playbooks/create.yml`

 * *Files identical despite different names*

### Comparing `molecule_multipass-0.3.5/molecule_multipass/playbooks/destroy.yml` & `molecule_multipass-0.4.0/molecule_multipass/playbooks/destroy.yml`

 * *Files identical despite different names*

### Comparing `molecule_multipass-0.3.5/molecule_multipass.egg-info/SOURCES.txt` & `molecule_multipass-0.4.0/molecule_multipass.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -11,10 +11,11 @@
 molecule_multipass.egg-info/SOURCES.txt
 molecule_multipass.egg-info/dependency_links.txt
 molecule_multipass.egg-info/entry_points.txt
 molecule_multipass.egg-info/requires.txt
 molecule_multipass.egg-info/top_level.txt
 molecule_multipass/cookiecutter/cookiecutter.json
 molecule_multipass/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
+molecule_multipass/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/prepare.yml
 molecule_multipass/playbooks/create.yml
 molecule_multipass/playbooks/destroy.yml
 molecule_multipass/playbooks/templates/cloud-init.yml.j2
```

### Comparing `molecule_multipass-0.3.5/pyproject.toml` & `molecule_multipass-0.4.0/pyproject.toml`

 * *Files identical despite different names*

