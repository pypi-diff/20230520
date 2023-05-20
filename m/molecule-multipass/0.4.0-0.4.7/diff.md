# Comparing `tmp/molecule_multipass-0.4.0.tar.gz` & `tmp/molecule_multipass-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molecule_multipass-0.4.0.tar", last modified: Sat May 20 14:11:19 2023, max compression
+gzip compressed data, was "molecule_multipass-0.4.7.tar", last modified: Sat May 20 19:56:42 2023, max compression
```

## Comparing `molecule_multipass-0.4.0.tar` & `molecule_multipass-0.4.7.tar`

### file list

```diff
@@ -1,33 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:11:19.143421 molecule_multipass-0.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:11:19.135421 molecule_multipass-0.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-20 14:11:07.000000 molecule_multipass-0.4.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:11:19.135421 molecule_multipass-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-20 14:11:07.000000 molecule_multipass-0.4.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-20 14:11:07.000000 molecule_multipass-0.4.0/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-20 14:11:07.000000 molecule_multipass-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-20 14:11:07.000000 molecule_multipass-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-20 14:11:19.143421 molecule_multipass-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 14:11:07.000000 molecule_multipass-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:11:19.135421 molecule_multipass-0.4.0/molecule_multipass/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 14:11:07.000000 molecule_multipass-0.4.0/molecule_multipass/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:11:19.139421 molecule_multipass-0.4.0/molecule_multipass/cookiecutter/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-20 14:11:07.000000 molecule_multipass-0.4.0/molecule_multipass/cookiecutter/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:11:19.131420 molecule_multipass-0.4.0/molecule_multipass/cookiecutter/{{cookiecutter.molecule_directory}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:11:19.139421 molecule_multipass-0.4.0/molecule_multipass/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 14:11:07.000000 molecule_multipass-0.4.0/molecule_multipass/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-20 14:11:07.000000 molecule_multipass-0.4.0/molecule_multipass/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/prepare.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-20 14:11:07.000000 molecule_multipass-0.4.0/molecule_multipass/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:11:19.139421 molecule_multipass-0.4.0/molecule_multipass/playbooks/
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-20 14:11:07.000000 molecule_multipass-0.4.0/molecule_multipass/playbooks/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-05-20 14:11:07.000000 molecule_multipass-0.4.0/molecule_multipass/playbooks/destroy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:11:19.139421 molecule_multipass-0.4.0/molecule_multipass/playbooks/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-20 14:11:07.000000 molecule_multipass-0.4.0/molecule_multipass/playbooks/templates/cloud-init.yml.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:11:19.139421 molecule_multipass-0.4.0/molecule_multipass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-20 14:11:19.000000 molecule_multipass-0.4.0/molecule_multipass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-20 14:11:19.000000 molecule_multipass-0.4.0/molecule_multipass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 14:11:19.000000 molecule_multipass-0.4.0/molecule_multipass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-20 14:11:19.000000 molecule_multipass-0.4.0/molecule_multipass.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-20 14:11:19.000000 molecule_multipass-0.4.0/molecule_multipass.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-20 14:11:19.000000 molecule_multipass-0.4.0/molecule_multipass.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-20 14:11:07.000000 molecule_multipass-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 14:11:19.143421 molecule_multipass-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:56:42.133785 molecule_multipass-0.4.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:56:42.129785 molecule_multipass-0.4.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:56:42.129785 molecule_multipass-0.4.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-20 19:56:32.000000 molecule_multipass-0.4.7/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-20 19:56:32.000000 molecule_multipass-0.4.7/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-20 19:56:32.000000 molecule_multipass-0.4.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-20 19:56:32.000000 molecule_multipass-0.4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-20 19:56:42.133785 molecule_multipass-0.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 19:56:32.000000 molecule_multipass-0.4.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:56:42.129785 molecule_multipass-0.4.7/molecule_multipass/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 19:56:32.000000 molecule_multipass-0.4.7/molecule_multipass/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:56:42.129785 molecule_multipass-0.4.7/molecule_multipass/cookiecutter/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-20 19:56:32.000000 molecule_multipass-0.4.7/molecule_multipass/cookiecutter/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:56:42.129785 molecule_multipass-0.4.7/molecule_multipass/cookiecutter/{{cookiecutter.molecule_directory}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:56:42.133785 molecule_multipass-0.4.7/molecule_multipass/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 19:56:32.000000 molecule_multipass-0.4.7/molecule_multipass/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-20 19:56:32.000000 molecule_multipass-0.4.7/molecule_multipass/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/prepare.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-20 19:56:32.000000 molecule_multipass-0.4.7/molecule_multipass/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:56:42.133785 molecule_multipass-0.4.7/molecule_multipass/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-20 19:56:32.000000 molecule_multipass-0.4.7/molecule_multipass/playbooks/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-20 19:56:32.000000 molecule_multipass-0.4.7/molecule_multipass/playbooks/destroy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:56:42.133785 molecule_multipass-0.4.7/molecule_multipass/playbooks/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-20 19:56:32.000000 molecule_multipass-0.4.7/molecule_multipass/playbooks/templates/cloud-init.yml.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:56:42.129785 molecule_multipass-0.4.7/molecule_multipass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-20 19:56:42.000000 molecule_multipass-0.4.7/molecule_multipass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-20 19:56:42.000000 molecule_multipass-0.4.7/molecule_multipass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 19:56:42.000000 molecule_multipass-0.4.7/molecule_multipass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-20 19:56:42.000000 molecule_multipass-0.4.7/molecule_multipass.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-20 19:56:42.000000 molecule_multipass-0.4.7/molecule_multipass.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-20 19:56:42.000000 molecule_multipass-0.4.7/molecule_multipass.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-20 19:56:32.000000 molecule_multipass-0.4.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 19:56:42.133785 molecule_multipass-0.4.7/setup.cfg
```

### Comparing `molecule_multipass-0.4.0/.github/workflows/python-publish.yml` & `molecule_multipass-0.4.7/.github/workflows/python-publish.yml`

 * *Files 2% similar despite different names*

```diff
@@ -9,35 +9,31 @@
 
 jobs:
   deploy:
     runs-on: ubuntu-latest
 
     steps:
     - uses: actions/checkout@v3
-
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
         python-version: '3.x'
-
     - name: Install dependencies
       run: >-
         python -m
         pip install
         build
         --user
-
     - name: Build a binary wheel and a source tarball
       run: >-
         python -m
         build
         --sdist
         --wheel
         --outdir dist/
         .
-
     - name: Publish package
       if: startsWith(github.ref, 'refs/tags')
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
         user: __token__
         password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `molecule_multipass-0.4.0/.gitignore` & `molecule_multipass-0.4.7/.gitignore`

 * *Files identical despite different names*

### Comparing `molecule_multipass-0.4.0/LICENSE` & `molecule_multipass-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `molecule_multipass-0.4.0/molecule_multipass/driver.py` & `molecule_multipass-0.4.7/molecule_multipass/driver.py`

 * *Files identical despite different names*

### Comparing `molecule_multipass-0.4.0/molecule_multipass/playbooks/create.yml` & `molecule_multipass-0.4.7/molecule_multipass/playbooks/create.yml`

 * *Files identical despite different names*

### Comparing `molecule_multipass-0.4.0/molecule_multipass/playbooks/destroy.yml` & `molecule_multipass-0.4.7/molecule_multipass/playbooks/destroy.yml`

 * *Files 23% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
   tasks:
     - name: Get multipass executable path
       ansible.builtin.shell: "command -v {{ multipass_executable }}"
       register: multipass_path
       changed_when: false
 
-    - name: Register multipass executable path
+    - name: Set multipass executable path
       ansible.builtin.set_fact:
         multipass_cmd: "{{ multipass_path.stdout }}"
 
     - block:
         - name: Prepare VMs config
           set_fact:
             instance_conf: "{{ lookup('file', molecule_instance_config) | from_yaml }}"
@@ -43,7 +43,15 @@
       loop_control:
         label: "{{ item.item.instance }}"
       register: multipass_destroy_status
       until: multipass_destroy_status.finished
       retries: 30
       delay: 5
 
+    - name: Prepare VMs config list
+      set_fact:
+        instance_conf: {}
+
+    - name: Dump VMs config
+      copy:
+        content: "{{ instance_conf | to_json | from_json | to_yaml }}"
+        dest: "{{ molecule_instance_config }}"
```

### Comparing `molecule_multipass-0.4.0/molecule_multipass.egg-info/SOURCES.txt` & `molecule_multipass-0.4.7/molecule_multipass.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 .gitignore
 LICENSE
 README.md
 pyproject.toml
-.github/release-drafter.yml
 .github/workflows/python-publish.yml
-.github/workflows/release-drafter.yml
+.github/workflows/release.yml
 molecule_multipass/__init__.py
 molecule_multipass/driver.py
 molecule_multipass.egg-info/PKG-INFO
 molecule_multipass.egg-info/SOURCES.txt
 molecule_multipass.egg-info/dependency_links.txt
 molecule_multipass.egg-info/entry_points.txt
 molecule_multipass.egg-info/requires.txt
```

### Comparing `molecule_multipass-0.4.0/pyproject.toml` & `molecule_multipass-0.4.7/pyproject.toml`

 * *Files identical despite different names*

