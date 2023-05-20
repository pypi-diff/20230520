# Comparing `tmp/home_assistant_streamdeck_yaml-2023.4.9.tar.gz` & `tmp/home_assistant_streamdeck_yaml-2023.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "home_assistant_streamdeck_yaml-2023.4.9.tar", last modified: Sat Apr  8 19:22:57 2023, max compression
+gzip compressed data, was "home_assistant_streamdeck_yaml-2023.5.0.tar", last modified: Sat May 20 20:35:06 2023, max compression
```

## Comparing `home_assistant_streamdeck_yaml-2023.4.9.tar` & `home_assistant_streamdeck_yaml-2023.5.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 19:22:57.372556 home_assistant_streamdeck_yaml-2023.4.9/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/.env.example
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 19:22:57.368556 home_assistant_streamdeck_yaml-2023.4.9/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/.github/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 19:22:57.368556 home_assistant_streamdeck_yaml-2023.4.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/.github/workflows/docker-build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/.github/workflows/pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/.github/workflows/toc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/.github/workflows/update-readme.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    34673 2023-04-08 19:22:57.372556 home_assistant_streamdeck_yaml-2023.4.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    34199 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 19:22:57.368556 home_assistant_streamdeck_yaml-2023.4.9/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   158604 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/assets/Roboto-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/assets/fireplace.png
--rw-r--r--   0 runner    (1001) docker     (123)    14446 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/assets/hogwarts.png
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/assets/netflix.png
--rw-r--r--   0 runner    (1001) docker     (123)    13386 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/assets/night_sky.png
--rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/assets/space-heater.png
--rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/assets/spotify.png
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/assets/xbox.png
--rw-r--r--   0 runner    (1001) docker     (123)     9763 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/configuration.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/docker-compose.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 19:22:57.372556 home_assistant_streamdeck_yaml-2023.4.9/home_assistant_streamdeck_yaml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    34673 2023-04-08 19:22:57.000000 home_assistant_streamdeck_yaml-2023.4.9/home_assistant_streamdeck_yaml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-08 19:22:57.000000 home_assistant_streamdeck_yaml-2023.4.9/home_assistant_streamdeck_yaml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 19:22:57.000000 home_assistant_streamdeck_yaml-2023.4.9/home_assistant_streamdeck_yaml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-08 19:22:57.000000 home_assistant_streamdeck_yaml-2023.4.9/home_assistant_streamdeck_yaml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-08 19:22:57.000000 home_assistant_streamdeck_yaml-2023.4.9/home_assistant_streamdeck_yaml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-08 19:22:57.000000 home_assistant_streamdeck_yaml-2023.4.9/home_assistant_streamdeck_yaml.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    45796 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/home_assistant_streamdeck_yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 19:22:57.372556 home_assistant_streamdeck_yaml-2023.4.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 19:22:57.372556 home_assistant_streamdeck_yaml-2023.4.9/systemd/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/systemd/home-assistant-streamdeck-yaml.service
--rwxr-xr-x   0 runner    (1001) docker     (123)       74 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/systemd/restart
--rwxr-xr-x   0 runner    (1001) docker     (123)      278 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/systemd/run.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)       73 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/systemd/status
--rwxr-xr-x   0 runner    (1001) docker     (123)       83 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/systemd/update
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 19:22:57.372556 home_assistant_streamdeck_yaml-2023.4.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/tests/state.json
--rw-r--r--   0 runner    (1001) docker     (123)    32493 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (123)    35837 2023-04-08 19:22:39.000000 home_assistant_streamdeck_yaml-2023.4.9/tests/test_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:35:06.728837 home_assistant_streamdeck_yaml-2023.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-20 20:34:41.000000 home_assistant_streamdeck_yaml-2023.5.0/.env.example
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:35:06.720837 home_assistant_streamdeck_yaml-2023.5.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-05-20 20:34:41.000000 home_assistant_streamdeck_yaml-2023.5.0/.github/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:35:06.720837 home_assistant_streamdeck_yaml-2023.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-20 20:34:41.000000 home_assistant_streamdeck_yaml-2023.5.0/.github/workflows/docker-build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-20 20:34:41.000000 home_assistant_streamdeck_yaml-2023.5.0/.github/workflows/pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-20 20:34:41.000000 home_assistant_streamdeck_yaml-2023.5.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-20 20:34:41.000000 home_assistant_streamdeck_yaml-2023.5.0/.github/workflows/toc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-20 20:34:41.000000 home_assistant_streamdeck_yaml-2023.5.0/.github/workflows/update-readme.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-05-20 20:34:41.000000 home_assistant_streamdeck_yaml-2023.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-20 20:34:41.000000 home_assistant_streamdeck_yaml-2023.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-20 20:34:41.000000 home_assistant_streamdeck_yaml-2023.5.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-20 20:34:41.000000 home_assistant_streamdeck_yaml-2023.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    42758 2023-05-20 20:35:06.728837 home_assistant_streamdeck_yaml-2023.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    42284 2023-05-20 20:34:41.000000 home_assistant_streamdeck_yaml-2023.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:35:06.724837 home_assistant_streamdeck_yaml-2023.5.0/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   158604 2023-05-20 20:34:41.000000 home_assistant_streamdeck_yaml-2023.5.0/assets/Roboto-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-05-20 20:34:41.000000 home_assistant_streamdeck_yaml-2023.5.0/assets/fireplace.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14446 2023-05-20 20:34:41.000000 home_assistant_streamdeck_yaml-2023.5.0/assets/hogwarts.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-05-20 20:34:41.000000 home_assistant_streamdeck_yaml-2023.5.0/assets/netflix.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13386 2023-05-20 20:34:41.000000 home_assistant_streamdeck_yaml-2023.5.0/assets/night_sky.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-05-20 20:34:41.000000 home_assistant_streamdeck_yaml-2023.5.0/assets/space-heater.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-05-20 20:34:41.000000 home_assistant_streamdeck_yaml-2023.5.0/assets/spotify.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-05-20 20:34:41.000000 home_assistant_streamdeck_yaml-2023.5.0/assets/xbox.png
+-rw-r--r--   0 runner    (1001) docker     (123)    22558 2023-05-20 20:34:41.000000 home_assistant_streamdeck_yaml-2023.5.0/configuration.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-20 20:34:41.000000 home_assistant_streamdeck_yaml-2023.5.0/docker-compose.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:35:06.724837 home_assistant_streamdeck_yaml-2023.5.0/home_assistant_streamdeck_yaml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    42758 2023-05-20 20:35:06.000000 home_assistant_streamdeck_yaml-2023.5.0/home_assistant_streamdeck_yaml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-20 20:35:06.000000 home_assistant_streamdeck_yaml-2023.5.0/home_assistant_streamdeck_yaml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 20:35:06.000000 home_assistant_streamdeck_yaml-2023.5.0/home_assistant_streamdeck_yaml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-20 20:35:06.000000 home_assistant_streamdeck_yaml-2023.5.0/home_assistant_streamdeck_yaml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-20 20:35:06.000000 home_assistant_streamdeck_yaml-2023.5.0/home_assistant_streamdeck_yaml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-20 20:35:06.000000 home_assistant_streamdeck_yaml-2023.5.0/home_assistant_streamdeck_yaml.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    59997 2023-05-20 20:34:41.000000 home_assistant_streamdeck_yaml-2023.5.0/home_assistant_streamdeck_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-20 20:34:41.000000 home_assistant_streamdeck_yaml-2023.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 20:35:06.728837 home_assistant_streamdeck_yaml-2023.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:35:06.724837 home_assistant_streamdeck_yaml-2023.5.0/systemd/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-20 20:34:41.000000 home_assistant_streamdeck_yaml-2023.5.0/systemd/home-assistant-streamdeck-yaml.service
+-rwxr-xr-x   0 runner    (1001) docker     (123)       74 2023-05-20 20:34:41.000000 home_assistant_streamdeck_yaml-2023.5.0/systemd/restart
+-rwxr-xr-x   0 runner    (1001) docker     (123)      278 2023-05-20 20:34:41.000000 home_assistant_streamdeck_yaml-2023.5.0/systemd/run.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)       73 2023-05-20 20:34:41.000000 home_assistant_streamdeck_yaml-2023.5.0/systemd/status
+-rwxr-xr-x   0 runner    (1001) docker     (123)      107 2023-05-20 20:34:41.000000 home_assistant_streamdeck_yaml-2023.5.0/systemd/update
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:35:06.724837 home_assistant_streamdeck_yaml-2023.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-20 20:34:41.000000 home_assistant_streamdeck_yaml-2023.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-05-20 20:34:41.000000 home_assistant_streamdeck_yaml-2023.5.0/tests/state.json
+-rw-r--r--   0 runner    (1001) docker     (123)    35391 2023-05-20 20:34:41.000000 home_assistant_streamdeck_yaml-2023.5.0/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39246 2023-05-20 20:34:41.000000 home_assistant_streamdeck_yaml-2023.5.0/tests/test_examples.py
```

### Comparing `home_assistant_streamdeck_yaml-2023.4.9/.github/release.py` & `home_assistant_streamdeck_yaml-2023.5.0/.github/release.py`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.4.9/.github/workflows/docker-build.yml` & `home_assistant_streamdeck_yaml-2023.5.0/.github/workflows/docker-build.yml`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,18 @@
     branches:
       - "main"
   # Test the image on PRs
   pull_request:
     branches:
       - '*'
 
+concurrency:
+  group: ${{ github.workflow }}-${{ github.event_name }}
+  cancel-in-progress: true
+
 jobs:
   docker:
     runs-on: ubuntu-latest
     steps:
       - name: Checkout
         uses: actions/checkout@v2
         with:
```

### Comparing `home_assistant_streamdeck_yaml-2023.4.9/.github/workflows/pytest.yml` & `home_assistant_streamdeck_yaml-2023.5.0/.github/workflows/pytest.yml`

 * *Files 4% similar despite different names*

```diff
@@ -15,11 +15,10 @@
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          pip install -e ".[test,colormap]"
-          pip install pytest
+          pip install -e ".[test,colormap,docs]"
       - name: Run pytest
         run: pytest
```

### Comparing `home_assistant_streamdeck_yaml-2023.4.9/.github/workflows/release.yml` & `home_assistant_streamdeck_yaml-2023.5.0/.github/workflows/release.yml`

 * *Files 13% similar despite different names*

```diff
@@ -39,15 +39,14 @@
       run: python .github/release.py
 
     - name: Create GitHub Release
       uses: softprops/action-gh-release@v1
       if: steps.generate_version.outputs.version != ''
       with:
         tag_name: ${{ steps.generate_version.outputs.version }}
-        release_name: version ${{ steps.generate_version.outputs.version }}
         generate_release_notes: true
 
     - name: Build and publish
       if: steps.generate_version.outputs.version != ''
       env:
         TWINE_USERNAME: __token__
         TWINE_PASSWORD: ${{ secrets.PYPI_TOKEN }}
```

### Comparing `home_assistant_streamdeck_yaml-2023.4.9/.github/workflows/update-readme.yml` & `home_assistant_streamdeck_yaml-2023.5.0/.github/workflows/update-readme.yml`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.4.9/.gitignore` & `home_assistant_streamdeck_yaml-2023.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.4.9/.pre-commit-config.yaml` & `home_assistant_streamdeck_yaml-2023.5.0/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -3,21 +3,21 @@
     rev: v4.4.0
     hooks:
       - id: check-added-large-files
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: mixed-line-ending
   - repo: "https://github.com/ambv/black"
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
       - id: black-jupyter
         language_version: python3
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: "v0.0.259"
+    rev: "v0.0.261"
     hooks:
       - id: ruff
         args: ["--fix"]
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: "v1.1.1"
+    rev: "v1.2.0"
     hooks:
       - id: mypy
         additional_dependencies: ["types-PyYAML", "types-requests", "types-setuptools"]
```

### Comparing `home_assistant_streamdeck_yaml-2023.4.9/Dockerfile` & `home_assistant_streamdeck_yaml-2023.5.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.4.9/LICENSE` & `home_assistant_streamdeck_yaml-2023.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.4.9/PKG-INFO` & `home_assistant_streamdeck_yaml-2023.5.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: home_assistant_streamdeck_yaml
-Version: 2023.4.9
-Summary: Home Assistant on Stream Deck: configured via YAML (with templates) and running on Linux, MacOS, and Windows
-Author-email: Bas Nijholt <bas@nijho.lt>
-Project-URL: Homepage, https://github.com/basnijholt/home-assistant-streamdeck-yaml
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: docs
-Provides-Extra: colormap
-License-File: LICENSE
-
 <img src="https://user-images.githubusercontent.com/6897215/225175629-28f80bfb-3b0a-44ac-8b52-b719953958d7.png" align="right" style="width: 300px;" />
 
 <h1 align="center">Home Assistant on Stream Deck</h1>
 <h3 align="center">Configured via YAML (with templates) and running on Linux, MacOS, and Windows</h3>
 
 Introducing: Home Assistant on Stream Deck!
 
@@ -35,15 +22,15 @@
 [[ToC](#books-table-of-contents)]
 
 **Why choose our solution over others?**
 
 You might have seen a similar project ([`cgiesche/streamdeck-homeassistant`](https://github.com/cgiesche/streamdeck-homeassistant)) on Github before [[†](https://github.com/cgiesche/streamdeck-homeassistant)].
 However, our solution is more versatile and allows you to connect a Stream Deck to the same Linux machine where Home Assistant is running.
 The native Stream Deck software doesn't support Linux, but we've got you covered with the help of the [`python-elgato-streamdeck`](https://github.com/abcminiuser/python-elgato-streamdeck) library.
-If you are looking for some inspiration, check out the [>20 Button Configurations ideas](#bulb-more-than-20-button-configurations-ideas) section below.
+If you are looking for some inspiration, check out the [>20 Button Configurations ideas](#bulb-more-than-30-button-configurations-ideas) section below.
 
 **Check out the video below to see it in action!**
 
 https://user-images.githubusercontent.com/6897215/226788119-6c198ea6-2950-4f95-95dc-346c9e5b5cee.mp4
 
 ## :books: Table of Contents
 
@@ -56,16 +43,18 @@
     - [:whale: Installation with Docker](#whale-installation-with-docker)
     - [:computer: Installation without Docker](#computer-installation-without-docker)
       - [:penguin: Linux](#penguin-linux)
       - [:apple: MacOS](#apple-macos)
       - [:desktop_computer: Windows](#desktop_computer-windows)
   - [:gear: Configuration](#gear-configuration)
     - [:page_facing_up: `configuration.yaml`](#page_facing_up-configurationyaml)
+    - [:clipboard: Config YAML configuration](#clipboard-config-yaml-configuration)
+    - [:bookmark_tabs: Page YAML configuration](#bookmark_tabs-page-yaml-configuration)
     - [:white_square_button: Button YAML configuration](#white_square_button-button-yaml-configuration)
-- [:bulb: More than 20 Button Configurations ideas](#bulb-more-than-20-button-configurations-ideas)
+- [:bulb: More than 30 Button Configurations ideas](#bulb-more-than-30-button-configurations-ideas)
 
 <!-- END doctoc generated TOC please keep comment here to allow auto update -->
 
 ## 🌟 Share Your Success
 
 I love hearing from users!
 If you're using Home Assistant StreamDeck YAML in your projects, please consider opening an issue on the [GitHub repository](https://github.com/basnijholt/home-assistant-streamdeck-yaml/issues/new) to let me know.
@@ -186,14 +175,15 @@
 ### :page_facing_up: `configuration.yaml`
 
 Here's an example `configuration.yaml` file to help
 
 ```yaml
 brightness: 100  # Default brightness of the Stream Deck (0-100)
 state_entity_id: binary_sensor.anyone_home  # Entity to sync display state with
+auto_reload: true  # Automatically reload the configuration file when it changes
 pages:
   - name: Home
     buttons:
       - entity_id: light.bedroom_lights
         service: light.toggle
         text: |
           Bedroom
@@ -247,46 +237,85 @@
         text: '{{ (100 * state_attr("media_player.kef_ls50", "volume_level")) | int }}%'
         text_size: 16
         icon_mdi: "volume-minus"
       - special_type: go-to-page
         special_type_data: 0
 ```
 
+### :clipboard: Config YAML configuration
+
+Each YAML config can take the following configuration
+
+<!-- CODE:START -->
+<!-- from home_assistant_streamdeck_yaml import Config -->
+<!-- print(Config.to_markdown_table()) -->
+<!-- CODE:END -->
+<!-- OUTPUT:START -->
+<!-- ⚠️ This content is auto-generated by `markdown-code-runner`. -->
+| Variable name     | Description                                                                                                                                                                                                                                                                               | Default   | Type            |
+|:------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:----------|:----------------|
+| `pages`           | A list of `Page`s in the configuration.                                                                                                                                                                                                                                                   |           | `List[Page]`    |
+| `anonymous_pages` | A list of anonymous Pages in the configuration. These pages are hidden and not displayed when cycling through the pages. They can only be reached using the `special_type: 'go-to-page'` button. Designed for single use, these pages return to the previous page upon clicking a button. |           | `List[Page]`    |
+| `state_entity_id` | The entity ID to sync display state with. For example `input_boolean.streamdeck` or `binary_sensor.anyone_home`.                                                                                                                                                                          | `None`    | `Optional[str]` |
+| `brightness`      | The default brightness of the Stream Deck (0-100).                                                                                                                                                                                                                                        | `100`     | `int`           |
+| `auto_reload`     | If True, the configuration YAML file will automatically be reloaded when it is modified.                                                                                                                                                                                                  | `False`   | `bool`          |
+
+<!-- OUTPUT:END -->
+
+### :bookmark_tabs: Page YAML configuration
+
+Each button can take the following configuration
+
+<!-- CODE:START -->
+<!-- from home_assistant_streamdeck_yaml import Page -->
+<!-- print(Page.to_markdown_table()) -->
+<!-- CODE:END -->
+<!-- OUTPUT:START -->
+<!-- ⚠️ This content is auto-generated by `markdown-code-runner`. -->
+| Variable name   | Description                    | Default   | Type           |
+|:----------------|:-------------------------------|:----------|:---------------|
+| `name`          | The name of the page.          |           | `str`          |
+| `buttons`       | A list of buttons on the page. |           | `List[Button]` |
+
+<!-- OUTPUT:END -->
+
 ### :white_square_button: Button YAML configuration
 
 Each button can take the following configuration
 
 <!-- CODE:START -->
 <!-- from home_assistant_streamdeck_yaml import Button -->
 <!-- print(Button.to_markdown_table()) -->
 <!-- CODE:END -->
 <!-- OUTPUT:START -->
 <!-- ⚠️ This content is auto-generated by `markdown-code-runner`. -->
-| Variable name           | Allow template   | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            | Default   | Type                                                                                                  |
-|:------------------------|:-----------------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:----------|:------------------------------------------------------------------------------------------------------|
-| `entity_id`             | ✅                | The `entity_id` that this button controls. This entitity will be passed to the `service` when the button is pressed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |           | `Optional[str]`                                                                                       |
-| `service`               | ✅                | The `service` that will be called when the button is pressed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |           | `Optional[str]`                                                                                       |
-| `service_data`          | ✅                | The `service_data` that will be passed to the `service` when the button is pressed. If empty, the `entity_id` will be passed.                                                                                                                                                                                                                                                                                                                                                                                                                                                          |           | `Optional[Mapping[str, Any]]`                                                                         |
-| `target`                | ✅                | The `target` that will be passed to the `service` when the button is pressed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |           | `Optional[Mapping[str, Any]]`                                                                         |
-| `text`                  | ✅                | The text to display on the button. If empty, no text is displayed. You might want to add `\n` characters to spread the text over several lines, or use the `\|` character in YAML to create a multi-line string.                                                                                                                                                                                                                                                                                                                                                                       |           | `str`                                                                                                 |
-| `text_color`            | ✅                | Color of the text. If empty, the color is `white`, unless an `entity_id` is specified, in which case the color is `amber` when the state is `on`, and `white` when it is `off`.                                                                                                                                                                                                                                                                                                                                                                                                        |           | `Optional[str]`                                                                                       |
-| `text_size`             | ❌                | Integer size of the text.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              | `12`      | `int`                                                                                                 |
-| `icon`                  | ✅                | The icon filename to display on the button. Make the path absolute (e.g., `/config/streamdeck/my_icon.png`) or relative to the `assets` directory (e.g., `my_icon.png`). If empty, a icon with `icon_background_color` and `text` is displayed. The icon can be a URL to an image, like `'url:https://www.nijho.lt/authors/admin/avatar.jpg'`, or a `spotify:` icon, like `'spotify:album/6gnYcXVaffdG0vwVM34cr8'`. If the icon is a `spotify:` icon, the icon will be downloaded and cached.                                                                                          |           | `Optional[str]`                                                                                       |
-| `icon_mdi`              | ✅                | The Material Design Icon to display on the button. If empty, no icon is displayed. See https://mdi.bessarabov.com/ for a list of icons. The SVG icon will be downloaded and cached.                                                                                                                                                                                                                                                                                                                                                                                                    |           | `Optional[str]`                                                                                       |
-| `icon_background_color` | ✅                | A color (in hex format, e.g., '#FF0000') for the background of the icon (if no `icon` is specified).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   | `#000000` | `str`                                                                                                 |
-| `icon_mdi_color`        | ✅                | The color of the Material Design Icon (in hex format, e.g., '#FF0000'). If empty, the color is derived from `text_color` but is less saturated (gray is mixed in).                                                                                                                                                                                                                                                                                                                                                                                                                     |           | `Optional[str]`                                                                                       |
-| `icon_gray_when_off`    | ❌                | When specifying `icon` and `entity_id`, if the state is `off`, the icon will be converted to grayscale.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |           | `bool`                                                                                                |
-| `special_type`          | ❌                | Special type of button. If no specified, the button is a normal button. If `next-page`, the button will go to the next page. If `previous-page`, the button will go to the previous page. If `turn-off`, the button will turn off the SteamDeck until any button is pressed. If `empty`, the button will be empty. If `go-to-page`, the button will go to the page specified by `special_type_data` (either an `int` or `str` (name of the page)). If `light-control`, the button will control a light, and the `special_type_data` can be a dictionary, see its description.          |           | `Optional[Literal['next-page', 'previous-page', 'empty', 'go-to-page', 'turn-off', 'light-control']]` |
-| `special_type_data`     | ✅                | Data for the special type of button. If `go-to-page`, the data should be an `int` or `str` (name of the page). If `light-control`, the data should optionally be a dictionary. The dictionary can contain the following keys: The `colors` key and a value a list of max (`n_keys_on_streamdeck - 5`) hex colors. The `colormap` key and a value a colormap (https://matplotlib.org/stable/tutorials/colors/colormaps.html) can be used. This requires the `matplotlib` package to be installed. If no list of `colors` or `colormap` is specified, 10 equally spaced colors are used. |           | `Optional[Any]`                                                                                       |
+| Variable name           | Allow template   | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            | Default   | Type                                                                                                            |
+|:------------------------|:-----------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:----------|:----------------------------------------------------------------------------------------------------------------|
+| `entity_id`             | ✅                | The `entity_id` that this button controls. This entitity will be passed to the `service` when the button is pressed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |           | `Optional[str]`                                                                                                 |
+| `service`               | ✅                | The `service` that will be called when the button is pressed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |           | `Optional[str]`                                                                                                 |
+| `service_data`          | ✅                | The `service_data` that will be passed to the `service` when the button is pressed. If empty, the `entity_id` will be passed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |           | `Optional[Mapping[str, Any]]`                                                                                   |
+| `target`                | ✅                | The `target` that will be passed to the `service` when the button is pressed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |           | `Optional[Mapping[str, Any]]`                                                                                   |
+| `text`                  | ✅                | The text to display on the button. If empty, no text is displayed. You might want to add `\n` characters to spread the text over several lines, or use the `\|` character in YAML to create a multi-line string.                                                                                                                                                                                                                                                                                                                                                                                                                                       |           | `str`                                                                                                           |
+| `text_color`            | ✅                | Color of the text. If empty, the color is `white`, unless an `entity_id` is specified, in which case the color is `amber` when the state is `on`, and `white` when it is `off`.                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |           | `Optional[str]`                                                                                                 |
+| `text_size`             | ❌                | Integer size of the text.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              | `12`      | `int`                                                                                                           |
+| `text_offset`           | ❌                | The text's position can be moved up or down from the center of the button, and this movement is measured in pixels. The value can be positive (for upward movement) or negative (for downward movement).                                                                                                                                                                                                                                                                                                                                                                                                                                               |           | `int`                                                                                                           |
+| `icon`                  | ✅                | The icon filename to display on the button. Make the path absolute (e.g., `/config/streamdeck/my_icon.png`) or relative to the `assets` directory (e.g., `my_icon.png`). If empty, a icon with `icon_background_color` and `text` is displayed. The icon can be a URL to an image, like `'url:https://www.nijho.lt/authors/admin/avatar.jpg'`, or a `spotify:` icon, like `'spotify:album/6gnYcXVaffdG0vwVM34cr8'`. If the icon is a `spotify:` icon, the icon will be downloaded and cached. The icon can also display a partially complete ring, like a progress bar, or sensor value, like `ring:25` for a 25% complete ring.                       |           | `Optional[str]`                                                                                                 |
+| `icon_mdi`              | ✅                | The Material Design Icon to display on the button. If empty, no icon is displayed. See https://mdi.bessarabov.com/ for a list of icons. The SVG icon will be downloaded and cached.                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |           | `Optional[str]`                                                                                                 |
+| `icon_background_color` | ✅                | A color (in hex format, e.g., '#FF0000') for the background of the icon (if no `icon` is specified).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   | `#000000` | `str`                                                                                                           |
+| `icon_mdi_color`        | ✅                | The color of the Material Design Icon (in hex format, e.g., '#FF0000'). If empty, the color is derived from `text_color` but is less saturated (gray is mixed in).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |           | `Optional[str]`                                                                                                 |
+| `icon_gray_when_off`    | ❌                | When specifying `icon` and `entity_id`, if the state is `off`, the icon will be converted to grayscale.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |           | `bool`                                                                                                          |
+| `delay`                 | ✅                | The delay (in seconds) before the `service` is called. This is useful if you want to wait before calling the `service`. Counts down from the time the button is pressed. If while counting the button is pressed again, the timer is cancelled. Should be a float or template string that evaluates to a float.                                                                                                                                                                                                                                                                                                                                        |           | `Union[float, str]`                                                                                             |
+| `special_type`          | ❌                | Special type of button. If no specified, the button is a normal button. If `next-page`, the button will go to the next page. If `previous-page`, the button will go to the previous page. If `turn-off`, the button will turn off the SteamDeck until any button is pressed. If `empty`, the button will be empty. If `go-to-page`, the button will go to the page specified by `special_type_data` (either an `int` or `str` (name of the page)). If `light-control`, the button will control a light, and the `special_type_data` can be a dictionary, see its description. If `reload`, the button will reload the configuration file when pressed. |           | `Optional[Literal['next-page', 'previous-page', 'empty', 'go-to-page', 'turn-off', 'light-control', 'reload']]` |
+| `special_type_data`     | ✅                | Data for the special type of button. If `go-to-page`, the data should be an `int` or `str` (name of the page). If `light-control`, the data should optionally be a dictionary. The dictionary can contain the following keys: The `colors` key and a value a list of max (`n_keys_on_streamdeck - 5`) hex colors. The `colormap` key and a value a colormap (https://matplotlib.org/stable/tutorials/colors/colormaps.html) can be used. This requires the `matplotlib` package to be installed. If no list of `colors` or `colormap` is specified, 10 equally spaced colors are used.                                                                 |           | `Optional[Any]`                                                                                                 |
 
 <!-- OUTPUT:END -->
 
-# :bulb: More than 20 Button Configurations ideas
+# :bulb: More than 30 Button Configurations ideas
 
-Here are >20 interesting uses for the Stream Deck with Home Assistant:
+Here are >30 interesting uses for the Stream Deck with Home Assistant (click on text to expand):
 
 <!-- CODE:START -->
 <!-- import os, sys -->
 <!-- sys.path.append(os.path.abspath(".")) -->
 <!-- from tests.test_examples import generate_readme_entry -->
 <!-- print(generate_readme_entry()) -->
 <!-- CODE:END -->
@@ -402,40 +431,46 @@
     Bedroom
     {{ 'On' if is_state('fan.bedroom_fan', 'on') else 'Off' }}
 ```
 
 </details>
 
 <details>
-<summary>7. 🔒 Lock/unlock a door:</summary>
+<summary>7. 🔒 Lock/unlock a door after 30 seconds:</summary>
 
 ```yaml
 - entity_id: lock.front_door
   service: lock.toggle
+  delay: "{{ 30 if is_state('lock.front_door', 'unlocked') else 0 }}"
   icon_mdi: "{{ 'door-open' if is_state('lock.front_door', 'unlocked') else 'door-closed' }}"
   text: |
     Front Door
     {{ 'Unlocked' if is_state('lock.front_door', 'unlocked') else 'Locked' }}
   text_size: 10
+  text_color: "{{ 'green' if is_state('lock.front_door', 'unlocked') else 'red' }}"
 ```
 
 </details>
 
 <details>
-<summary>8. ⚠️ Arm/disarm an alarm system:</summary>
+<summary>8. ⚠️ Arm/disarm an alarm system after 30 seconds:</summary>
 
 ```yaml
 - entity_id: alarm_control_panel.home_alarm
+  delay: "{{ 0 if is_state('alarm_control_panel.home_alarm', 'armed_away') else 30 }}"
   service: "{{ 'alarm_control_panel.alarm_disarm' if is_state('alarm_control_panel.home_alarm', 'armed_away') else 'alarm_control_panel.alarm_arm_away' }}"
   icon_mdi: "{{ 'shield-check' if is_state('alarm_control_panel.home_alarm', 'armed_away') else 'shield-off' }}"
   text: |
     {{ 'Disarm' if is_state('alarm_control_panel.home_alarm', 'armed_away') else 'Arm' }}
     Alarm
+  text_color: "{{ 'red' if is_state('alarm_control_panel.home_alarm', 'armed_away') else 'green' }}"
 ```
 
+Arm the alarm system in 30 seconds if it's disarmed, disarm it immediately if it's armed.
+
 </details>
 
 <details>
 <summary>9. ⏰ Set an alarm time for the next day:</summary>
 
 ```yaml
 - service: input_datetime.set_datetime
@@ -700,21 +735,23 @@
         filename: "/config/www/recordings/camera_{{ now().strftime('%Y%m%d_%H%M%S') }}.mp4"
 ```
 
 
 </details>
 
 <details>
-<summary>25. 🌙 Enable/disable a nightlight:</summary>
+<summary>25. 🌙 Enable/disable a nightlight after 30 min:</summary>
 
 ```yaml
 - entity_id: light.nightlight
   service: light.toggle
+  delay: 1800
   icon_mdi: "{{ 'lightbulb-on' if is_state('light.nightlight', 'on') else 'lightbulb-off' }}"
   text: "{{ 'Disable' if is_state('light.nightlight', 'on') else 'Enable' }} Nightlight"
+  text_color: "{{ 'red' if is_state('light.nightlight', 'on') else 'green' }}"
 ```
 
 </details>
 
 <details>
 <summary>26. 🔥 Control a smart fireplace:</summary>
 
@@ -781,13 +818,61 @@
   service: media_player.toggle
   icon: >
     {% if is_state('media_player.tv', 'on') %}
     url:https://raw.githubusercontent.com/basnijholt/home-assistant-streamdeck-yaml/main/assets/fireplace.png
     {% else %}
     url:https://raw.githubusercontent.com/basnijholt/home-assistant-streamdeck-yaml/main/assets/hogwarts.png
     {% endif %}
+  text: >
+    Turn {{ 'Off' if is_state('media_player.tv', 'on') else 'On' }}
 ```
 
 </details>
 
+<details>
+<summary>31. ⏰ Turn off all lights in 60s:</summary>
+
+```yaml
+- entity_id: light.all_lights
+  service: light.turn_off
+  text: |
+    Turn off
+    in 60s
+  delay: 60
+```
+
+</details>
+
+<details>
+<summary>32. 🌡️ Display outside temperature with a ring indicator:</summary>
+
+```yaml
+- entity_id: sensor.temperature_sensor_outside_temperature
+  icon: >
+    {%- set temp = states('sensor.temperature_sensor_outside_temperature') -%}
+    {%- set min_temp = -10 -%}
+    {%- set max_temp = 40 -%}
+    {%- set pct = ((temp - min_temp) / (max_temp - min_temp)) * 100 -%}
+    ring:{{ pct | round }}
+  text: |
+    {%- set temp = states('sensor.temperature_sensor_outside_temperature') -%}
+    Outside
+    {{ temp | round(1) }}°C
+```
+
+This sets 0% to -10°C and 100% to 40°C.
+
+</details>
+
+<details>
+<summary>33. 🔄 Reload the `configuration.yaml` file:</summary>
+
+```yaml
+- special_type: reload
+```
+
+When pressed, the `configuration.yaml` is reloaded.
+
+</details>
+
 
 <!-- OUTPUT:END -->
```

### Comparing `home_assistant_streamdeck_yaml-2023.4.9/README.md` & `home_assistant_streamdeck_yaml-2023.5.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: home_assistant_streamdeck_yaml
+Version: 2023.5.0
+Summary: Home Assistant on Stream Deck: configured via YAML (with templates) and running on Linux, MacOS, and Windows
+Author-email: Bas Nijholt <bas@nijho.lt>
+Project-URL: Homepage, https://github.com/basnijholt/home-assistant-streamdeck-yaml
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: test
+Provides-Extra: docs
+Provides-Extra: colormap
+License-File: LICENSE
+
 <img src="https://user-images.githubusercontent.com/6897215/225175629-28f80bfb-3b0a-44ac-8b52-b719953958d7.png" align="right" style="width: 300px;" />
 
 <h1 align="center">Home Assistant on Stream Deck</h1>
 <h3 align="center">Configured via YAML (with templates) and running on Linux, MacOS, and Windows</h3>
 
 Introducing: Home Assistant on Stream Deck!
 
@@ -22,15 +35,15 @@
 [[ToC](#books-table-of-contents)]
 
 **Why choose our solution over others?**
 
 You might have seen a similar project ([`cgiesche/streamdeck-homeassistant`](https://github.com/cgiesche/streamdeck-homeassistant)) on Github before [[†](https://github.com/cgiesche/streamdeck-homeassistant)].
 However, our solution is more versatile and allows you to connect a Stream Deck to the same Linux machine where Home Assistant is running.
 The native Stream Deck software doesn't support Linux, but we've got you covered with the help of the [`python-elgato-streamdeck`](https://github.com/abcminiuser/python-elgato-streamdeck) library.
-If you are looking for some inspiration, check out the [>20 Button Configurations ideas](#bulb-more-than-20-button-configurations-ideas) section below.
+If you are looking for some inspiration, check out the [>20 Button Configurations ideas](#bulb-more-than-30-button-configurations-ideas) section below.
 
 **Check out the video below to see it in action!**
 
 https://user-images.githubusercontent.com/6897215/226788119-6c198ea6-2950-4f95-95dc-346c9e5b5cee.mp4
 
 ## :books: Table of Contents
 
@@ -43,16 +56,18 @@
     - [:whale: Installation with Docker](#whale-installation-with-docker)
     - [:computer: Installation without Docker](#computer-installation-without-docker)
       - [:penguin: Linux](#penguin-linux)
       - [:apple: MacOS](#apple-macos)
       - [:desktop_computer: Windows](#desktop_computer-windows)
   - [:gear: Configuration](#gear-configuration)
     - [:page_facing_up: `configuration.yaml`](#page_facing_up-configurationyaml)
+    - [:clipboard: Config YAML configuration](#clipboard-config-yaml-configuration)
+    - [:bookmark_tabs: Page YAML configuration](#bookmark_tabs-page-yaml-configuration)
     - [:white_square_button: Button YAML configuration](#white_square_button-button-yaml-configuration)
-- [:bulb: More than 20 Button Configurations ideas](#bulb-more-than-20-button-configurations-ideas)
+- [:bulb: More than 30 Button Configurations ideas](#bulb-more-than-30-button-configurations-ideas)
 
 <!-- END doctoc generated TOC please keep comment here to allow auto update -->
 
 ## 🌟 Share Your Success
 
 I love hearing from users!
 If you're using Home Assistant StreamDeck YAML in your projects, please consider opening an issue on the [GitHub repository](https://github.com/basnijholt/home-assistant-streamdeck-yaml/issues/new) to let me know.
@@ -173,14 +188,15 @@
 ### :page_facing_up: `configuration.yaml`
 
 Here's an example `configuration.yaml` file to help
 
 ```yaml
 brightness: 100  # Default brightness of the Stream Deck (0-100)
 state_entity_id: binary_sensor.anyone_home  # Entity to sync display state with
+auto_reload: true  # Automatically reload the configuration file when it changes
 pages:
   - name: Home
     buttons:
       - entity_id: light.bedroom_lights
         service: light.toggle
         text: |
           Bedroom
@@ -234,46 +250,85 @@
         text: '{{ (100 * state_attr("media_player.kef_ls50", "volume_level")) | int }}%'
         text_size: 16
         icon_mdi: "volume-minus"
       - special_type: go-to-page
         special_type_data: 0
 ```
 
+### :clipboard: Config YAML configuration
+
+Each YAML config can take the following configuration
+
+<!-- CODE:START -->
+<!-- from home_assistant_streamdeck_yaml import Config -->
+<!-- print(Config.to_markdown_table()) -->
+<!-- CODE:END -->
+<!-- OUTPUT:START -->
+<!-- ⚠️ This content is auto-generated by `markdown-code-runner`. -->
+| Variable name     | Description                                                                                                                                                                                                                                                                               | Default   | Type            |
+|:------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:----------|:----------------|
+| `pages`           | A list of `Page`s in the configuration.                                                                                                                                                                                                                                                   |           | `List[Page]`    |
+| `anonymous_pages` | A list of anonymous Pages in the configuration. These pages are hidden and not displayed when cycling through the pages. They can only be reached using the `special_type: 'go-to-page'` button. Designed for single use, these pages return to the previous page upon clicking a button. |           | `List[Page]`    |
+| `state_entity_id` | The entity ID to sync display state with. For example `input_boolean.streamdeck` or `binary_sensor.anyone_home`.                                                                                                                                                                          | `None`    | `Optional[str]` |
+| `brightness`      | The default brightness of the Stream Deck (0-100).                                                                                                                                                                                                                                        | `100`     | `int`           |
+| `auto_reload`     | If True, the configuration YAML file will automatically be reloaded when it is modified.                                                                                                                                                                                                  | `False`   | `bool`          |
+
+<!-- OUTPUT:END -->
+
+### :bookmark_tabs: Page YAML configuration
+
+Each button can take the following configuration
+
+<!-- CODE:START -->
+<!-- from home_assistant_streamdeck_yaml import Page -->
+<!-- print(Page.to_markdown_table()) -->
+<!-- CODE:END -->
+<!-- OUTPUT:START -->
+<!-- ⚠️ This content is auto-generated by `markdown-code-runner`. -->
+| Variable name   | Description                    | Default   | Type           |
+|:----------------|:-------------------------------|:----------|:---------------|
+| `name`          | The name of the page.          |           | `str`          |
+| `buttons`       | A list of buttons on the page. |           | `List[Button]` |
+
+<!-- OUTPUT:END -->
+
 ### :white_square_button: Button YAML configuration
 
 Each button can take the following configuration
 
 <!-- CODE:START -->
 <!-- from home_assistant_streamdeck_yaml import Button -->
 <!-- print(Button.to_markdown_table()) -->
 <!-- CODE:END -->
 <!-- OUTPUT:START -->
 <!-- ⚠️ This content is auto-generated by `markdown-code-runner`. -->
-| Variable name           | Allow template   | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            | Default   | Type                                                                                                  |
-|:------------------------|:-----------------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:----------|:------------------------------------------------------------------------------------------------------|
-| `entity_id`             | ✅                | The `entity_id` that this button controls. This entitity will be passed to the `service` when the button is pressed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |           | `Optional[str]`                                                                                       |
-| `service`               | ✅                | The `service` that will be called when the button is pressed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |           | `Optional[str]`                                                                                       |
-| `service_data`          | ✅                | The `service_data` that will be passed to the `service` when the button is pressed. If empty, the `entity_id` will be passed.                                                                                                                                                                                                                                                                                                                                                                                                                                                          |           | `Optional[Mapping[str, Any]]`                                                                         |
-| `target`                | ✅                | The `target` that will be passed to the `service` when the button is pressed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |           | `Optional[Mapping[str, Any]]`                                                                         |
-| `text`                  | ✅                | The text to display on the button. If empty, no text is displayed. You might want to add `\n` characters to spread the text over several lines, or use the `\|` character in YAML to create a multi-line string.                                                                                                                                                                                                                                                                                                                                                                       |           | `str`                                                                                                 |
-| `text_color`            | ✅                | Color of the text. If empty, the color is `white`, unless an `entity_id` is specified, in which case the color is `amber` when the state is `on`, and `white` when it is `off`.                                                                                                                                                                                                                                                                                                                                                                                                        |           | `Optional[str]`                                                                                       |
-| `text_size`             | ❌                | Integer size of the text.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              | `12`      | `int`                                                                                                 |
-| `icon`                  | ✅                | The icon filename to display on the button. Make the path absolute (e.g., `/config/streamdeck/my_icon.png`) or relative to the `assets` directory (e.g., `my_icon.png`). If empty, a icon with `icon_background_color` and `text` is displayed. The icon can be a URL to an image, like `'url:https://www.nijho.lt/authors/admin/avatar.jpg'`, or a `spotify:` icon, like `'spotify:album/6gnYcXVaffdG0vwVM34cr8'`. If the icon is a `spotify:` icon, the icon will be downloaded and cached.                                                                                          |           | `Optional[str]`                                                                                       |
-| `icon_mdi`              | ✅                | The Material Design Icon to display on the button. If empty, no icon is displayed. See https://mdi.bessarabov.com/ for a list of icons. The SVG icon will be downloaded and cached.                                                                                                                                                                                                                                                                                                                                                                                                    |           | `Optional[str]`                                                                                       |
-| `icon_background_color` | ✅                | A color (in hex format, e.g., '#FF0000') for the background of the icon (if no `icon` is specified).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   | `#000000` | `str`                                                                                                 |
-| `icon_mdi_color`        | ✅                | The color of the Material Design Icon (in hex format, e.g., '#FF0000'). If empty, the color is derived from `text_color` but is less saturated (gray is mixed in).                                                                                                                                                                                                                                                                                                                                                                                                                     |           | `Optional[str]`                                                                                       |
-| `icon_gray_when_off`    | ❌                | When specifying `icon` and `entity_id`, if the state is `off`, the icon will be converted to grayscale.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |           | `bool`                                                                                                |
-| `special_type`          | ❌                | Special type of button. If no specified, the button is a normal button. If `next-page`, the button will go to the next page. If `previous-page`, the button will go to the previous page. If `turn-off`, the button will turn off the SteamDeck until any button is pressed. If `empty`, the button will be empty. If `go-to-page`, the button will go to the page specified by `special_type_data` (either an `int` or `str` (name of the page)). If `light-control`, the button will control a light, and the `special_type_data` can be a dictionary, see its description.          |           | `Optional[Literal['next-page', 'previous-page', 'empty', 'go-to-page', 'turn-off', 'light-control']]` |
-| `special_type_data`     | ✅                | Data for the special type of button. If `go-to-page`, the data should be an `int` or `str` (name of the page). If `light-control`, the data should optionally be a dictionary. The dictionary can contain the following keys: The `colors` key and a value a list of max (`n_keys_on_streamdeck - 5`) hex colors. The `colormap` key and a value a colormap (https://matplotlib.org/stable/tutorials/colors/colormaps.html) can be used. This requires the `matplotlib` package to be installed. If no list of `colors` or `colormap` is specified, 10 equally spaced colors are used. |           | `Optional[Any]`                                                                                       |
+| Variable name           | Allow template   | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            | Default   | Type                                                                                                            |
+|:------------------------|:-----------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:----------|:----------------------------------------------------------------------------------------------------------------|
+| `entity_id`             | ✅                | The `entity_id` that this button controls. This entitity will be passed to the `service` when the button is pressed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |           | `Optional[str]`                                                                                                 |
+| `service`               | ✅                | The `service` that will be called when the button is pressed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |           | `Optional[str]`                                                                                                 |
+| `service_data`          | ✅                | The `service_data` that will be passed to the `service` when the button is pressed. If empty, the `entity_id` will be passed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |           | `Optional[Mapping[str, Any]]`                                                                                   |
+| `target`                | ✅                | The `target` that will be passed to the `service` when the button is pressed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |           | `Optional[Mapping[str, Any]]`                                                                                   |
+| `text`                  | ✅                | The text to display on the button. If empty, no text is displayed. You might want to add `\n` characters to spread the text over several lines, or use the `\|` character in YAML to create a multi-line string.                                                                                                                                                                                                                                                                                                                                                                                                                                       |           | `str`                                                                                                           |
+| `text_color`            | ✅                | Color of the text. If empty, the color is `white`, unless an `entity_id` is specified, in which case the color is `amber` when the state is `on`, and `white` when it is `off`.                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |           | `Optional[str]`                                                                                                 |
+| `text_size`             | ❌                | Integer size of the text.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              | `12`      | `int`                                                                                                           |
+| `text_offset`           | ❌                | The text's position can be moved up or down from the center of the button, and this movement is measured in pixels. The value can be positive (for upward movement) or negative (for downward movement).                                                                                                                                                                                                                                                                                                                                                                                                                                               |           | `int`                                                                                                           |
+| `icon`                  | ✅                | The icon filename to display on the button. Make the path absolute (e.g., `/config/streamdeck/my_icon.png`) or relative to the `assets` directory (e.g., `my_icon.png`). If empty, a icon with `icon_background_color` and `text` is displayed. The icon can be a URL to an image, like `'url:https://www.nijho.lt/authors/admin/avatar.jpg'`, or a `spotify:` icon, like `'spotify:album/6gnYcXVaffdG0vwVM34cr8'`. If the icon is a `spotify:` icon, the icon will be downloaded and cached. The icon can also display a partially complete ring, like a progress bar, or sensor value, like `ring:25` for a 25% complete ring.                       |           | `Optional[str]`                                                                                                 |
+| `icon_mdi`              | ✅                | The Material Design Icon to display on the button. If empty, no icon is displayed. See https://mdi.bessarabov.com/ for a list of icons. The SVG icon will be downloaded and cached.                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |           | `Optional[str]`                                                                                                 |
+| `icon_background_color` | ✅                | A color (in hex format, e.g., '#FF0000') for the background of the icon (if no `icon` is specified).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   | `#000000` | `str`                                                                                                           |
+| `icon_mdi_color`        | ✅                | The color of the Material Design Icon (in hex format, e.g., '#FF0000'). If empty, the color is derived from `text_color` but is less saturated (gray is mixed in).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |           | `Optional[str]`                                                                                                 |
+| `icon_gray_when_off`    | ❌                | When specifying `icon` and `entity_id`, if the state is `off`, the icon will be converted to grayscale.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |           | `bool`                                                                                                          |
+| `delay`                 | ✅                | The delay (in seconds) before the `service` is called. This is useful if you want to wait before calling the `service`. Counts down from the time the button is pressed. If while counting the button is pressed again, the timer is cancelled. Should be a float or template string that evaluates to a float.                                                                                                                                                                                                                                                                                                                                        |           | `Union[float, str]`                                                                                             |
+| `special_type`          | ❌                | Special type of button. If no specified, the button is a normal button. If `next-page`, the button will go to the next page. If `previous-page`, the button will go to the previous page. If `turn-off`, the button will turn off the SteamDeck until any button is pressed. If `empty`, the button will be empty. If `go-to-page`, the button will go to the page specified by `special_type_data` (either an `int` or `str` (name of the page)). If `light-control`, the button will control a light, and the `special_type_data` can be a dictionary, see its description. If `reload`, the button will reload the configuration file when pressed. |           | `Optional[Literal['next-page', 'previous-page', 'empty', 'go-to-page', 'turn-off', 'light-control', 'reload']]` |
+| `special_type_data`     | ✅                | Data for the special type of button. If `go-to-page`, the data should be an `int` or `str` (name of the page). If `light-control`, the data should optionally be a dictionary. The dictionary can contain the following keys: The `colors` key and a value a list of max (`n_keys_on_streamdeck - 5`) hex colors. The `colormap` key and a value a colormap (https://matplotlib.org/stable/tutorials/colors/colormaps.html) can be used. This requires the `matplotlib` package to be installed. If no list of `colors` or `colormap` is specified, 10 equally spaced colors are used.                                                                 |           | `Optional[Any]`                                                                                                 |
 
 <!-- OUTPUT:END -->
 
-# :bulb: More than 20 Button Configurations ideas
+# :bulb: More than 30 Button Configurations ideas
 
-Here are >20 interesting uses for the Stream Deck with Home Assistant:
+Here are >30 interesting uses for the Stream Deck with Home Assistant (click on text to expand):
 
 <!-- CODE:START -->
 <!-- import os, sys -->
 <!-- sys.path.append(os.path.abspath(".")) -->
 <!-- from tests.test_examples import generate_readme_entry -->
 <!-- print(generate_readme_entry()) -->
 <!-- CODE:END -->
@@ -389,40 +444,46 @@
     Bedroom
     {{ 'On' if is_state('fan.bedroom_fan', 'on') else 'Off' }}
 ```
 
 </details>
 
 <details>
-<summary>7. 🔒 Lock/unlock a door:</summary>
+<summary>7. 🔒 Lock/unlock a door after 30 seconds:</summary>
 
 ```yaml
 - entity_id: lock.front_door
   service: lock.toggle
+  delay: "{{ 30 if is_state('lock.front_door', 'unlocked') else 0 }}"
   icon_mdi: "{{ 'door-open' if is_state('lock.front_door', 'unlocked') else 'door-closed' }}"
   text: |
     Front Door
     {{ 'Unlocked' if is_state('lock.front_door', 'unlocked') else 'Locked' }}
   text_size: 10
+  text_color: "{{ 'green' if is_state('lock.front_door', 'unlocked') else 'red' }}"
 ```
 
 </details>
 
 <details>
-<summary>8. ⚠️ Arm/disarm an alarm system:</summary>
+<summary>8. ⚠️ Arm/disarm an alarm system after 30 seconds:</summary>
 
 ```yaml
 - entity_id: alarm_control_panel.home_alarm
+  delay: "{{ 0 if is_state('alarm_control_panel.home_alarm', 'armed_away') else 30 }}"
   service: "{{ 'alarm_control_panel.alarm_disarm' if is_state('alarm_control_panel.home_alarm', 'armed_away') else 'alarm_control_panel.alarm_arm_away' }}"
   icon_mdi: "{{ 'shield-check' if is_state('alarm_control_panel.home_alarm', 'armed_away') else 'shield-off' }}"
   text: |
     {{ 'Disarm' if is_state('alarm_control_panel.home_alarm', 'armed_away') else 'Arm' }}
     Alarm
+  text_color: "{{ 'red' if is_state('alarm_control_panel.home_alarm', 'armed_away') else 'green' }}"
 ```
 
+Arm the alarm system in 30 seconds if it's disarmed, disarm it immediately if it's armed.
+
 </details>
 
 <details>
 <summary>9. ⏰ Set an alarm time for the next day:</summary>
 
 ```yaml
 - service: input_datetime.set_datetime
@@ -687,21 +748,23 @@
         filename: "/config/www/recordings/camera_{{ now().strftime('%Y%m%d_%H%M%S') }}.mp4"
 ```
 
 
 </details>
 
 <details>
-<summary>25. 🌙 Enable/disable a nightlight:</summary>
+<summary>25. 🌙 Enable/disable a nightlight after 30 min:</summary>
 
 ```yaml
 - entity_id: light.nightlight
   service: light.toggle
+  delay: 1800
   icon_mdi: "{{ 'lightbulb-on' if is_state('light.nightlight', 'on') else 'lightbulb-off' }}"
   text: "{{ 'Disable' if is_state('light.nightlight', 'on') else 'Enable' }} Nightlight"
+  text_color: "{{ 'red' if is_state('light.nightlight', 'on') else 'green' }}"
 ```
 
 </details>
 
 <details>
 <summary>26. 🔥 Control a smart fireplace:</summary>
 
@@ -768,13 +831,61 @@
   service: media_player.toggle
   icon: >
     {% if is_state('media_player.tv', 'on') %}
     url:https://raw.githubusercontent.com/basnijholt/home-assistant-streamdeck-yaml/main/assets/fireplace.png
     {% else %}
     url:https://raw.githubusercontent.com/basnijholt/home-assistant-streamdeck-yaml/main/assets/hogwarts.png
     {% endif %}
+  text: >
+    Turn {{ 'Off' if is_state('media_player.tv', 'on') else 'On' }}
 ```
 
 </details>
 
+<details>
+<summary>31. ⏰ Turn off all lights in 60s:</summary>
+
+```yaml
+- entity_id: light.all_lights
+  service: light.turn_off
+  text: |
+    Turn off
+    in 60s
+  delay: 60
+```
+
+</details>
+
+<details>
+<summary>32. 🌡️ Display outside temperature with a ring indicator:</summary>
+
+```yaml
+- entity_id: sensor.temperature_sensor_outside_temperature
+  icon: >
+    {%- set temp = states('sensor.temperature_sensor_outside_temperature') -%}
+    {%- set min_temp = -10 -%}
+    {%- set max_temp = 40 -%}
+    {%- set pct = ((temp - min_temp) / (max_temp - min_temp)) * 100 -%}
+    ring:{{ pct | round }}
+  text: |
+    {%- set temp = states('sensor.temperature_sensor_outside_temperature') -%}
+    Outside
+    {{ temp | round(1) }}°C
+```
+
+This sets 0% to -10°C and 100% to 40°C.
+
+</details>
+
+<details>
+<summary>33. 🔄 Reload the `configuration.yaml` file:</summary>
+
+```yaml
+- special_type: reload
+```
+
+When pressed, the `configuration.yaml` is reloaded.
+
+</details>
+
 
 <!-- OUTPUT:END -->
```

### Comparing `home_assistant_streamdeck_yaml-2023.4.9/assets/Roboto-Regular.ttf` & `home_assistant_streamdeck_yaml-2023.5.0/assets/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.4.9/assets/fireplace.png` & `home_assistant_streamdeck_yaml-2023.5.0/assets/fireplace.png`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.4.9/assets/hogwarts.png` & `home_assistant_streamdeck_yaml-2023.5.0/assets/hogwarts.png`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.4.9/assets/netflix.png` & `home_assistant_streamdeck_yaml-2023.5.0/assets/netflix.png`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.4.9/assets/night_sky.png` & `home_assistant_streamdeck_yaml-2023.5.0/assets/night_sky.png`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.4.9/assets/space-heater.png` & `home_assistant_streamdeck_yaml-2023.5.0/assets/space-heater.png`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.4.9/assets/spotify.png` & `home_assistant_streamdeck_yaml-2023.5.0/assets/spotify.png`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.4.9/assets/xbox.png` & `home_assistant_streamdeck_yaml-2023.5.0/assets/xbox.png`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.4.9/home_assistant_streamdeck_yaml.egg-info/PKG-INFO` & `home_assistant_streamdeck_yaml-2023.5.0/home_assistant_streamdeck_yaml.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: home-assistant-streamdeck-yaml
-Version: 2023.4.9
+Version: 2023.5.0
 Summary: Home Assistant on Stream Deck: configured via YAML (with templates) and running on Linux, MacOS, and Windows
 Author-email: Bas Nijholt <bas@nijho.lt>
 Project-URL: Homepage, https://github.com/basnijholt/home-assistant-streamdeck-yaml
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: docs
@@ -35,15 +35,15 @@
 [[ToC](#books-table-of-contents)]
 
 **Why choose our solution over others?**
 
 You might have seen a similar project ([`cgiesche/streamdeck-homeassistant`](https://github.com/cgiesche/streamdeck-homeassistant)) on Github before [[†](https://github.com/cgiesche/streamdeck-homeassistant)].
 However, our solution is more versatile and allows you to connect a Stream Deck to the same Linux machine where Home Assistant is running.
 The native Stream Deck software doesn't support Linux, but we've got you covered with the help of the [`python-elgato-streamdeck`](https://github.com/abcminiuser/python-elgato-streamdeck) library.
-If you are looking for some inspiration, check out the [>20 Button Configurations ideas](#bulb-more-than-20-button-configurations-ideas) section below.
+If you are looking for some inspiration, check out the [>20 Button Configurations ideas](#bulb-more-than-30-button-configurations-ideas) section below.
 
 **Check out the video below to see it in action!**
 
 https://user-images.githubusercontent.com/6897215/226788119-6c198ea6-2950-4f95-95dc-346c9e5b5cee.mp4
 
 ## :books: Table of Contents
 
@@ -56,16 +56,18 @@
     - [:whale: Installation with Docker](#whale-installation-with-docker)
     - [:computer: Installation without Docker](#computer-installation-without-docker)
       - [:penguin: Linux](#penguin-linux)
       - [:apple: MacOS](#apple-macos)
       - [:desktop_computer: Windows](#desktop_computer-windows)
   - [:gear: Configuration](#gear-configuration)
     - [:page_facing_up: `configuration.yaml`](#page_facing_up-configurationyaml)
+    - [:clipboard: Config YAML configuration](#clipboard-config-yaml-configuration)
+    - [:bookmark_tabs: Page YAML configuration](#bookmark_tabs-page-yaml-configuration)
     - [:white_square_button: Button YAML configuration](#white_square_button-button-yaml-configuration)
-- [:bulb: More than 20 Button Configurations ideas](#bulb-more-than-20-button-configurations-ideas)
+- [:bulb: More than 30 Button Configurations ideas](#bulb-more-than-30-button-configurations-ideas)
 
 <!-- END doctoc generated TOC please keep comment here to allow auto update -->
 
 ## 🌟 Share Your Success
 
 I love hearing from users!
 If you're using Home Assistant StreamDeck YAML in your projects, please consider opening an issue on the [GitHub repository](https://github.com/basnijholt/home-assistant-streamdeck-yaml/issues/new) to let me know.
@@ -186,14 +188,15 @@
 ### :page_facing_up: `configuration.yaml`
 
 Here's an example `configuration.yaml` file to help
 
 ```yaml
 brightness: 100  # Default brightness of the Stream Deck (0-100)
 state_entity_id: binary_sensor.anyone_home  # Entity to sync display state with
+auto_reload: true  # Automatically reload the configuration file when it changes
 pages:
   - name: Home
     buttons:
       - entity_id: light.bedroom_lights
         service: light.toggle
         text: |
           Bedroom
@@ -247,46 +250,85 @@
         text: '{{ (100 * state_attr("media_player.kef_ls50", "volume_level")) | int }}%'
         text_size: 16
         icon_mdi: "volume-minus"
       - special_type: go-to-page
         special_type_data: 0
 ```
 
+### :clipboard: Config YAML configuration
+
+Each YAML config can take the following configuration
+
+<!-- CODE:START -->
+<!-- from home_assistant_streamdeck_yaml import Config -->
+<!-- print(Config.to_markdown_table()) -->
+<!-- CODE:END -->
+<!-- OUTPUT:START -->
+<!-- ⚠️ This content is auto-generated by `markdown-code-runner`. -->
+| Variable name     | Description                                                                                                                                                                                                                                                                               | Default   | Type            |
+|:------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:----------|:----------------|
+| `pages`           | A list of `Page`s in the configuration.                                                                                                                                                                                                                                                   |           | `List[Page]`    |
+| `anonymous_pages` | A list of anonymous Pages in the configuration. These pages are hidden and not displayed when cycling through the pages. They can only be reached using the `special_type: 'go-to-page'` button. Designed for single use, these pages return to the previous page upon clicking a button. |           | `List[Page]`    |
+| `state_entity_id` | The entity ID to sync display state with. For example `input_boolean.streamdeck` or `binary_sensor.anyone_home`.                                                                                                                                                                          | `None`    | `Optional[str]` |
+| `brightness`      | The default brightness of the Stream Deck (0-100).                                                                                                                                                                                                                                        | `100`     | `int`           |
+| `auto_reload`     | If True, the configuration YAML file will automatically be reloaded when it is modified.                                                                                                                                                                                                  | `False`   | `bool`          |
+
+<!-- OUTPUT:END -->
+
+### :bookmark_tabs: Page YAML configuration
+
+Each button can take the following configuration
+
+<!-- CODE:START -->
+<!-- from home_assistant_streamdeck_yaml import Page -->
+<!-- print(Page.to_markdown_table()) -->
+<!-- CODE:END -->
+<!-- OUTPUT:START -->
+<!-- ⚠️ This content is auto-generated by `markdown-code-runner`. -->
+| Variable name   | Description                    | Default   | Type           |
+|:----------------|:-------------------------------|:----------|:---------------|
+| `name`          | The name of the page.          |           | `str`          |
+| `buttons`       | A list of buttons on the page. |           | `List[Button]` |
+
+<!-- OUTPUT:END -->
+
 ### :white_square_button: Button YAML configuration
 
 Each button can take the following configuration
 
 <!-- CODE:START -->
 <!-- from home_assistant_streamdeck_yaml import Button -->
 <!-- print(Button.to_markdown_table()) -->
 <!-- CODE:END -->
 <!-- OUTPUT:START -->
 <!-- ⚠️ This content is auto-generated by `markdown-code-runner`. -->
-| Variable name           | Allow template   | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            | Default   | Type                                                                                                  |
-|:------------------------|:-----------------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:----------|:------------------------------------------------------------------------------------------------------|
-| `entity_id`             | ✅                | The `entity_id` that this button controls. This entitity will be passed to the `service` when the button is pressed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |           | `Optional[str]`                                                                                       |
-| `service`               | ✅                | The `service` that will be called when the button is pressed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |           | `Optional[str]`                                                                                       |
-| `service_data`          | ✅                | The `service_data` that will be passed to the `service` when the button is pressed. If empty, the `entity_id` will be passed.                                                                                                                                                                                                                                                                                                                                                                                                                                                          |           | `Optional[Mapping[str, Any]]`                                                                         |
-| `target`                | ✅                | The `target` that will be passed to the `service` when the button is pressed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |           | `Optional[Mapping[str, Any]]`                                                                         |
-| `text`                  | ✅                | The text to display on the button. If empty, no text is displayed. You might want to add `\n` characters to spread the text over several lines, or use the `\|` character in YAML to create a multi-line string.                                                                                                                                                                                                                                                                                                                                                                       |           | `str`                                                                                                 |
-| `text_color`            | ✅                | Color of the text. If empty, the color is `white`, unless an `entity_id` is specified, in which case the color is `amber` when the state is `on`, and `white` when it is `off`.                                                                                                                                                                                                                                                                                                                                                                                                        |           | `Optional[str]`                                                                                       |
-| `text_size`             | ❌                | Integer size of the text.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              | `12`      | `int`                                                                                                 |
-| `icon`                  | ✅                | The icon filename to display on the button. Make the path absolute (e.g., `/config/streamdeck/my_icon.png`) or relative to the `assets` directory (e.g., `my_icon.png`). If empty, a icon with `icon_background_color` and `text` is displayed. The icon can be a URL to an image, like `'url:https://www.nijho.lt/authors/admin/avatar.jpg'`, or a `spotify:` icon, like `'spotify:album/6gnYcXVaffdG0vwVM34cr8'`. If the icon is a `spotify:` icon, the icon will be downloaded and cached.                                                                                          |           | `Optional[str]`                                                                                       |
-| `icon_mdi`              | ✅                | The Material Design Icon to display on the button. If empty, no icon is displayed. See https://mdi.bessarabov.com/ for a list of icons. The SVG icon will be downloaded and cached.                                                                                                                                                                                                                                                                                                                                                                                                    |           | `Optional[str]`                                                                                       |
-| `icon_background_color` | ✅                | A color (in hex format, e.g., '#FF0000') for the background of the icon (if no `icon` is specified).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   | `#000000` | `str`                                                                                                 |
-| `icon_mdi_color`        | ✅                | The color of the Material Design Icon (in hex format, e.g., '#FF0000'). If empty, the color is derived from `text_color` but is less saturated (gray is mixed in).                                                                                                                                                                                                                                                                                                                                                                                                                     |           | `Optional[str]`                                                                                       |
-| `icon_gray_when_off`    | ❌                | When specifying `icon` and `entity_id`, if the state is `off`, the icon will be converted to grayscale.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |           | `bool`                                                                                                |
-| `special_type`          | ❌                | Special type of button. If no specified, the button is a normal button. If `next-page`, the button will go to the next page. If `previous-page`, the button will go to the previous page. If `turn-off`, the button will turn off the SteamDeck until any button is pressed. If `empty`, the button will be empty. If `go-to-page`, the button will go to the page specified by `special_type_data` (either an `int` or `str` (name of the page)). If `light-control`, the button will control a light, and the `special_type_data` can be a dictionary, see its description.          |           | `Optional[Literal['next-page', 'previous-page', 'empty', 'go-to-page', 'turn-off', 'light-control']]` |
-| `special_type_data`     | ✅                | Data for the special type of button. If `go-to-page`, the data should be an `int` or `str` (name of the page). If `light-control`, the data should optionally be a dictionary. The dictionary can contain the following keys: The `colors` key and a value a list of max (`n_keys_on_streamdeck - 5`) hex colors. The `colormap` key and a value a colormap (https://matplotlib.org/stable/tutorials/colors/colormaps.html) can be used. This requires the `matplotlib` package to be installed. If no list of `colors` or `colormap` is specified, 10 equally spaced colors are used. |           | `Optional[Any]`                                                                                       |
+| Variable name           | Allow template   | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            | Default   | Type                                                                                                            |
+|:------------------------|:-----------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:----------|:----------------------------------------------------------------------------------------------------------------|
+| `entity_id`             | ✅                | The `entity_id` that this button controls. This entitity will be passed to the `service` when the button is pressed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |           | `Optional[str]`                                                                                                 |
+| `service`               | ✅                | The `service` that will be called when the button is pressed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |           | `Optional[str]`                                                                                                 |
+| `service_data`          | ✅                | The `service_data` that will be passed to the `service` when the button is pressed. If empty, the `entity_id` will be passed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |           | `Optional[Mapping[str, Any]]`                                                                                   |
+| `target`                | ✅                | The `target` that will be passed to the `service` when the button is pressed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |           | `Optional[Mapping[str, Any]]`                                                                                   |
+| `text`                  | ✅                | The text to display on the button. If empty, no text is displayed. You might want to add `\n` characters to spread the text over several lines, or use the `\|` character in YAML to create a multi-line string.                                                                                                                                                                                                                                                                                                                                                                                                                                       |           | `str`                                                                                                           |
+| `text_color`            | ✅                | Color of the text. If empty, the color is `white`, unless an `entity_id` is specified, in which case the color is `amber` when the state is `on`, and `white` when it is `off`.                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |           | `Optional[str]`                                                                                                 |
+| `text_size`             | ❌                | Integer size of the text.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              | `12`      | `int`                                                                                                           |
+| `text_offset`           | ❌                | The text's position can be moved up or down from the center of the button, and this movement is measured in pixels. The value can be positive (for upward movement) or negative (for downward movement).                                                                                                                                                                                                                                                                                                                                                                                                                                               |           | `int`                                                                                                           |
+| `icon`                  | ✅                | The icon filename to display on the button. Make the path absolute (e.g., `/config/streamdeck/my_icon.png`) or relative to the `assets` directory (e.g., `my_icon.png`). If empty, a icon with `icon_background_color` and `text` is displayed. The icon can be a URL to an image, like `'url:https://www.nijho.lt/authors/admin/avatar.jpg'`, or a `spotify:` icon, like `'spotify:album/6gnYcXVaffdG0vwVM34cr8'`. If the icon is a `spotify:` icon, the icon will be downloaded and cached. The icon can also display a partially complete ring, like a progress bar, or sensor value, like `ring:25` for a 25% complete ring.                       |           | `Optional[str]`                                                                                                 |
+| `icon_mdi`              | ✅                | The Material Design Icon to display on the button. If empty, no icon is displayed. See https://mdi.bessarabov.com/ for a list of icons. The SVG icon will be downloaded and cached.                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |           | `Optional[str]`                                                                                                 |
+| `icon_background_color` | ✅                | A color (in hex format, e.g., '#FF0000') for the background of the icon (if no `icon` is specified).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   | `#000000` | `str`                                                                                                           |
+| `icon_mdi_color`        | ✅                | The color of the Material Design Icon (in hex format, e.g., '#FF0000'). If empty, the color is derived from `text_color` but is less saturated (gray is mixed in).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |           | `Optional[str]`                                                                                                 |
+| `icon_gray_when_off`    | ❌                | When specifying `icon` and `entity_id`, if the state is `off`, the icon will be converted to grayscale.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |           | `bool`                                                                                                          |
+| `delay`                 | ✅                | The delay (in seconds) before the `service` is called. This is useful if you want to wait before calling the `service`. Counts down from the time the button is pressed. If while counting the button is pressed again, the timer is cancelled. Should be a float or template string that evaluates to a float.                                                                                                                                                                                                                                                                                                                                        |           | `Union[float, str]`                                                                                             |
+| `special_type`          | ❌                | Special type of button. If no specified, the button is a normal button. If `next-page`, the button will go to the next page. If `previous-page`, the button will go to the previous page. If `turn-off`, the button will turn off the SteamDeck until any button is pressed. If `empty`, the button will be empty. If `go-to-page`, the button will go to the page specified by `special_type_data` (either an `int` or `str` (name of the page)). If `light-control`, the button will control a light, and the `special_type_data` can be a dictionary, see its description. If `reload`, the button will reload the configuration file when pressed. |           | `Optional[Literal['next-page', 'previous-page', 'empty', 'go-to-page', 'turn-off', 'light-control', 'reload']]` |
+| `special_type_data`     | ✅                | Data for the special type of button. If `go-to-page`, the data should be an `int` or `str` (name of the page). If `light-control`, the data should optionally be a dictionary. The dictionary can contain the following keys: The `colors` key and a value a list of max (`n_keys_on_streamdeck - 5`) hex colors. The `colormap` key and a value a colormap (https://matplotlib.org/stable/tutorials/colors/colormaps.html) can be used. This requires the `matplotlib` package to be installed. If no list of `colors` or `colormap` is specified, 10 equally spaced colors are used.                                                                 |           | `Optional[Any]`                                                                                                 |
 
 <!-- OUTPUT:END -->
 
-# :bulb: More than 20 Button Configurations ideas
+# :bulb: More than 30 Button Configurations ideas
 
-Here are >20 interesting uses for the Stream Deck with Home Assistant:
+Here are >30 interesting uses for the Stream Deck with Home Assistant (click on text to expand):
 
 <!-- CODE:START -->
 <!-- import os, sys -->
 <!-- sys.path.append(os.path.abspath(".")) -->
 <!-- from tests.test_examples import generate_readme_entry -->
 <!-- print(generate_readme_entry()) -->
 <!-- CODE:END -->
@@ -402,40 +444,46 @@
     Bedroom
     {{ 'On' if is_state('fan.bedroom_fan', 'on') else 'Off' }}
 ```
 
 </details>
 
 <details>
-<summary>7. 🔒 Lock/unlock a door:</summary>
+<summary>7. 🔒 Lock/unlock a door after 30 seconds:</summary>
 
 ```yaml
 - entity_id: lock.front_door
   service: lock.toggle
+  delay: "{{ 30 if is_state('lock.front_door', 'unlocked') else 0 }}"
   icon_mdi: "{{ 'door-open' if is_state('lock.front_door', 'unlocked') else 'door-closed' }}"
   text: |
     Front Door
     {{ 'Unlocked' if is_state('lock.front_door', 'unlocked') else 'Locked' }}
   text_size: 10
+  text_color: "{{ 'green' if is_state('lock.front_door', 'unlocked') else 'red' }}"
 ```
 
 </details>
 
 <details>
-<summary>8. ⚠️ Arm/disarm an alarm system:</summary>
+<summary>8. ⚠️ Arm/disarm an alarm system after 30 seconds:</summary>
 
 ```yaml
 - entity_id: alarm_control_panel.home_alarm
+  delay: "{{ 0 if is_state('alarm_control_panel.home_alarm', 'armed_away') else 30 }}"
   service: "{{ 'alarm_control_panel.alarm_disarm' if is_state('alarm_control_panel.home_alarm', 'armed_away') else 'alarm_control_panel.alarm_arm_away' }}"
   icon_mdi: "{{ 'shield-check' if is_state('alarm_control_panel.home_alarm', 'armed_away') else 'shield-off' }}"
   text: |
     {{ 'Disarm' if is_state('alarm_control_panel.home_alarm', 'armed_away') else 'Arm' }}
     Alarm
+  text_color: "{{ 'red' if is_state('alarm_control_panel.home_alarm', 'armed_away') else 'green' }}"
 ```
 
+Arm the alarm system in 30 seconds if it's disarmed, disarm it immediately if it's armed.
+
 </details>
 
 <details>
 <summary>9. ⏰ Set an alarm time for the next day:</summary>
 
 ```yaml
 - service: input_datetime.set_datetime
@@ -700,21 +748,23 @@
         filename: "/config/www/recordings/camera_{{ now().strftime('%Y%m%d_%H%M%S') }}.mp4"
 ```
 
 
 </details>
 
 <details>
-<summary>25. 🌙 Enable/disable a nightlight:</summary>
+<summary>25. 🌙 Enable/disable a nightlight after 30 min:</summary>
 
 ```yaml
 - entity_id: light.nightlight
   service: light.toggle
+  delay: 1800
   icon_mdi: "{{ 'lightbulb-on' if is_state('light.nightlight', 'on') else 'lightbulb-off' }}"
   text: "{{ 'Disable' if is_state('light.nightlight', 'on') else 'Enable' }} Nightlight"
+  text_color: "{{ 'red' if is_state('light.nightlight', 'on') else 'green' }}"
 ```
 
 </details>
 
 <details>
 <summary>26. 🔥 Control a smart fireplace:</summary>
 
@@ -781,13 +831,61 @@
   service: media_player.toggle
   icon: >
     {% if is_state('media_player.tv', 'on') %}
     url:https://raw.githubusercontent.com/basnijholt/home-assistant-streamdeck-yaml/main/assets/fireplace.png
     {% else %}
     url:https://raw.githubusercontent.com/basnijholt/home-assistant-streamdeck-yaml/main/assets/hogwarts.png
     {% endif %}
+  text: >
+    Turn {{ 'Off' if is_state('media_player.tv', 'on') else 'On' }}
+```
+
+</details>
+
+<details>
+<summary>31. ⏰ Turn off all lights in 60s:</summary>
+
+```yaml
+- entity_id: light.all_lights
+  service: light.turn_off
+  text: |
+    Turn off
+    in 60s
+  delay: 60
 ```
 
 </details>
 
+<details>
+<summary>32. 🌡️ Display outside temperature with a ring indicator:</summary>
+
+```yaml
+- entity_id: sensor.temperature_sensor_outside_temperature
+  icon: >
+    {%- set temp = states('sensor.temperature_sensor_outside_temperature') -%}
+    {%- set min_temp = -10 -%}
+    {%- set max_temp = 40 -%}
+    {%- set pct = ((temp - min_temp) / (max_temp - min_temp)) * 100 -%}
+    ring:{{ pct | round }}
+  text: |
+    {%- set temp = states('sensor.temperature_sensor_outside_temperature') -%}
+    Outside
+    {{ temp | round(1) }}°C
+```
+
+This sets 0% to -10°C and 100% to 40°C.
+
+</details>
+
+<details>
+<summary>33. 🔄 Reload the `configuration.yaml` file:</summary>
+
+```yaml
+- special_type: reload
+```
+
+When pressed, the `configuration.yaml` is reloaded.
+
+</details>
+
 
 <!-- OUTPUT:END -->
```

### Comparing `home_assistant_streamdeck_yaml-2023.4.9/home_assistant_streamdeck_yaml.egg-info/SOURCES.txt` & `home_assistant_streamdeck_yaml-2023.5.0/home_assistant_streamdeck_yaml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.4.9/home_assistant_streamdeck_yaml.py` & `home_assistant_streamdeck_yaml-2023.5.0/home_assistant_streamdeck_yaml.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,44 +5,52 @@
 import asyncio
 import colorsys
 import functools as ft
 import hashlib
 import io
 import json
 import re
+import time
 import warnings
 from contextlib import asynccontextmanager
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Callable, Literal, TypeAlias
 
 import jinja2
 import pkg_resources
 import requests
 import websockets
 import yaml
 from lxml import etree
 from PIL import Image, ImageColor, ImageDraw, ImageFont, ImageOps
-from pydantic import BaseModel, Field, validator
+from pydantic import BaseModel, Field, PrivateAttr, validator
+from pydantic.fields import Undefined
 from rich.console import Console
+from rich.table import Table
 from StreamDeck.DeviceManager import DeviceManager
 from StreamDeck.ImageHelpers import PILHelper
 
 if TYPE_CHECKING:
     from collections.abc import Coroutine
 
+    import pandas as pd
     from StreamDeck.Devices import StreamDeck
 
 __version__ = pkg_resources.get_distribution("home_assistant_streamdeck_yaml").version
 
 
 SCRIPT_DIR = Path(__file__).parent
 ASSETS_PATH = SCRIPT_DIR / "assets"
 DEFAULT_CONFIG = SCRIPT_DIR / "configuration.yaml"
 DEFAULT_FONT: str = "Roboto-Regular.ttf"
-DEFAULT_MDI_ICONS = {"light": "lightbulb", "switch": "power-socket-eu"}
+DEFAULT_MDI_ICONS = {
+    "light": "lightbulb",
+    "switch": "power-socket-eu",
+    "script": "script",
+}
 ICON_PIXELS = 72
 _ID_COUNTER = 0
 
 console = Console()
 StateDict: TypeAlias = dict[str, dict[str, Any]]
 
 
@@ -87,25 +95,34 @@
         " which case the color is `amber` when the state is `on`, and `white` when it is `off`.",
     )
     text_size: int = Field(
         default=12,
         allow_template=False,
         description="Integer size of the text.",
     )
+    text_offset: int = Field(
+        default=0,
+        allow_template=False,
+        description="The text's position can be moved up or down from the center of"
+        " the button, and this movement is measured in pixels. The value can be"
+        " positive (for upward movement) or negative (for downward movement).",
+    )
     icon: str | None = Field(
         default=None,
         allow_template=True,
         description="The icon filename to display on the button."
         " Make the path absolute (e.g., `/config/streamdeck/my_icon.png`) or relative to the"
         " `assets` directory (e.g., `my_icon.png`)."
         " If empty, a icon with `icon_background_color` and `text` is displayed."
         " The icon can be a URL to an image,"
         " like `'url:https://www.nijho.lt/authors/admin/avatar.jpg'`, or a `spotify:`"
         " icon, like `'spotify:album/6gnYcXVaffdG0vwVM34cr8'`."
-        " If the icon is a `spotify:` icon, the icon will be downloaded and cached.",
+        " If the icon is a `spotify:` icon, the icon will be downloaded and cached."
+        " The icon can also display a partially complete ring, like a progress bar,"
+        " or sensor value, like `ring:25` for a 25% complete ring.",
     )
     icon_mdi: str | None = Field(
         default=None,
         allow_template=True,
         description="The Material Design Icon to display on the button."
         " If empty, no icon is displayed."
         " See https://mdi.bessarabov.com/ for a list of icons."
@@ -123,57 +140,70 @@
         " If empty, the color is derived from `text_color` but is less saturated (gray is mixed in).",
     )
     icon_gray_when_off: bool = Field(
         default=False,
         allow_template=False,
         description="When specifying `icon` and `entity_id`, if the state is `off`, the icon will be converted to grayscale.",
     )
+    delay: float | str = Field(
+        default=0.0,
+        allow_template=True,
+        description="The delay (in seconds) before the `service` is called."
+        " This is useful if you want to wait before calling the `service`."
+        " Counts down from the time the button is pressed."
+        " If while counting the button is pressed again, the timer is cancelled."
+        " Should be a float or template string that evaluates to a float.",
+    )
     special_type: Literal[
         "next-page",
         "previous-page",
         "empty",
         "go-to-page",
         "turn-off",
         "light-control",
+        "reload",
     ] | None = Field(
         default=None,
         allow_template=False,
         description="Special type of button."
         " If no specified, the button is a normal button."
         " If `next-page`, the button will go to the next page."
         " If `previous-page`, the button will go to the previous page."
         " If `turn-off`, the button will turn off the SteamDeck until any button is pressed."
         " If `empty`, the button will be empty."
         " If `go-to-page`, the button will go to the page specified by `special_type_data`"
         " (either an `int` or `str` (name of the page))."
         " If `light-control`, the button will control a light, and the `special_type_data`"
-        " can be a dictionary, see its description.",
+        " can be a dictionary, see its description."
+        " If `reload`, the button will reload the configuration file when pressed.",
     )
     special_type_data: Any | None = Field(
         default=None,
         allow_template=True,
         description="Data for the special type of button."
         " If `go-to-page`, the data should be an `int` or `str` (name of the page)."
         " If `light-control`, the data should optionally be a dictionary."
         " The dictionary can contain the following keys:"
         " The `colors` key and a value a list of max (`n_keys_on_streamdeck - 5`) hex colors."
         " The `colormap` key and a value a colormap (https://matplotlib.org/stable/tutorials/colors/colormaps.html)"
         " can be used. This requires the `matplotlib` package to be installed. If no"
         " list of `colors` or `colormap` is specified, 10 equally spaced colors are used.",
     )
 
+    _timer: AsyncDelayedCallback | None = PrivateAttr(None)
+
     @classmethod
     def from_yaml(cls: type[Button], yaml_str: str) -> Button:
         """Set the attributes from a YAML string."""
         data = yaml.safe_load(yaml_str)
         return cls(**data[0])
 
     @classmethod
-    def to_markdown_table(cls: type[Button]) -> str:
-        """Return a markdown table with the schema."""
+    def to_pandas_table(cls: type[Button]) -> pd.DataFrame:
+        """Return a pandas table with the schema."""
         import pandas as pd
 
         rows = []
         for k, field in cls.__fields__.items():
             info = field.field_info
             if info.description is None:
                 continue
@@ -182,18 +212,23 @@
                 return f"`{text}`"
 
             row = {
                 "Variable name": code(k),
                 "Allow template": "✅" if info.extra["allow_template"] else "❌",
                 "Description": info.description,
                 "Default": code(info.default) if info.default else "",
-                "Type": code(field._type_display()),  # noqa: SLF001
+                "Type": code(field._type_display()),
             }
             rows.append(row)
-        return pd.DataFrame(rows).to_markdown(index=False)
+        return pd.DataFrame(rows)
+
+    @classmethod
+    def to_markdown_table(cls: type[Button]) -> str:
+        """Return a markdown table with the schema."""
+        return cls.to_pandas_table().to_markdown(index=False)
 
     @property
     def domain(self) -> str | None:
         """Return the domain of the entity."""
         if self.service is None:
             return None
         return self.service.split(".", 1)[0]
@@ -245,34 +280,44 @@
             warnings.warn(
                 f"Failed to render icon for {self}: {exc}",
                 IconWarning,
                 stacklevel=2,
             )
             return _generate_failed_icon(size)
 
-    def render_icon(
+    def render_icon(  # noqa: PLR0912 PLR0915
         self,
         complete_state: StateDict,
         *,
         key_pressed: bool = False,
         size: tuple[int, int] = (ICON_PIXELS, ICON_PIXELS),
         icon_mdi_margin: int = 0,
         font_filename: str = DEFAULT_FONT,
     ) -> Image.Image:
         """Render the icon."""
-        button = self.rendered_template_button(complete_state)
+        if self.is_sleeping():
+            button, image = self.sleep_button_and_image(size)
+        else:
+            button = self.rendered_template_button(complete_state)
+            image = None
 
         if isinstance(button.icon, str) and ":" in button.icon:
             which, id_ = button.icon.split(":", 1)
             if which == "spotify":
                 filename = _to_filename(button.icon, ".jpeg")
-                return _download_spotify_image(id_, filename)
+                # copy to avoid modifying the cached image
+                image = _download_spotify_image(id_, filename).copy()
             if which == "url":
                 filename = _url_to_filename(id_)
-                return _download_image(id_, filename, size)
+                # copy to avoid modifying the cached image
+                image = _download_image(id_, filename, size).copy()
+            if which == "ring":
+                pct = _maybe_number(id_)
+                assert isinstance(pct, (int, float)), f"Invalid ring percentage: {id_}"
+                image = _draw_percentage_ring(pct, size)
 
         icon_convert_to_grayscale = False
         text = button.text
         text_color = button.text_color or "white"
         icon_mdi = button.icon_mdi
 
         if button.special_type == "next-page":
@@ -284,14 +329,17 @@
         elif button.special_type == "go-to-page":
             page = button.special_type_data
             text = button.text or f"Go to\nPage\n{page}"
             icon_mdi = button.icon_mdi or "book-open-page-variant"
         elif button.special_type == "turn-off":
             text = button.text or "Turn off"
             icon_mdi = button.icon_mdi or "power"
+        elif button.special_type == "reload":
+            text = button.text or "Reload\nconfig"
+            icon_mdi = button.icon_mdi or "reload"
         elif button.entity_id in complete_state:
             # Has entity_id
             state = complete_state[button.entity_id]
 
             if button.text_color is not None:
                 text_color = button.text_color
             elif state["state"] == "on":
@@ -303,29 +351,34 @@
                 and button.domain in DEFAULT_MDI_ICONS
             ):
                 icon_mdi = DEFAULT_MDI_ICONS[button.domain]
 
             if state["state"] == "off":
                 icon_convert_to_grayscale = button.icon_gray_when_off
 
-        image = _init_icon(
-            icon_background_color=button.icon_background_color,
-            icon_filename=button.icon,
-            icon_mdi=icon_mdi,
-            icon_mdi_margin=icon_mdi_margin,
-            icon_mdi_color=_named_to_hex(button.icon_mdi_color or text_color),
-            icon_convert_to_grayscale=icon_convert_to_grayscale,
-            size=size,
-        ).copy()  # copy to avoid modifying the cached image
+        if image is None:
+            image = _init_icon(
+                icon_background_color=button.icon_background_color,
+                icon_filename=button.icon,
+                icon_mdi=icon_mdi,
+                icon_mdi_margin=icon_mdi_margin,
+                icon_mdi_color=_named_to_hex(button.icon_mdi_color or text_color),
+                size=size,
+            ).copy()  # copy to avoid modifying the cached image
+
+        if icon_convert_to_grayscale:
+            image = _convert_to_grayscale(image)
+
         _add_text(
-            image,
-            font_filename,
-            self.text_size,
-            text,
+            image=image,
+            font_filename=font_filename,
+            text_size=self.text_size,
+            text=text,
             text_color=text_color if not key_pressed else "green",
+            text_offset=self.text_offset,
         )
         return image
 
     @validator("special_type_data")
     def _validate_special_type(
         cls: type[Button],
         v: Any,
@@ -370,89 +423,365 @@
                     if not isinstance(color, str):
                         msg = "All colors must be strings"
                         raise AssertionError(msg)  # noqa: TRY004
                 # Cast colors to tuple (to make it hashable)
                 v["colors"] = tuple(v["colors"])
         return v
 
+    def maybe_start_or_cancel_timer(
+        self,
+        callback: Callable[[], None | Coroutine] | None = None,
+    ) -> bool:
+        """Start or cancel the timer."""
+        if self.delay:
+            if self._timer is None:
+                assert isinstance(
+                    self.delay,
+                    (int, float),
+                ), f"Invalid delay: {self.delay}"
+                self._timer = AsyncDelayedCallback(delay=self.delay, callback=callback)
+            if self._timer.is_running():
+                self._timer.cancel()
+            else:
+                self._timer.start()
+            return True
+        return False
+
+    def is_sleeping(self) -> bool:
+        """Return True if the timer is sleeping."""
+        return self._timer is not None and self._timer.is_sleeping
+
+    def sleep_button_and_image(
+        self,
+        size: tuple[int, int],
+    ) -> tuple[Button, Image.Image]:
+        """Return the button and image for the sleep button."""
+        assert self._timer is not None
+        assert isinstance(self.delay, (int, float)), f"Invalid delay: {self.delay}"
+        remaining = self._timer.remaining_time()
+        pct = round(remaining / self.delay * 100)
+        image = _draw_percentage_ring(pct, size)
+        button = Button(
+            text=f"{remaining:.0f}s\n{pct}%",
+            text_color="white",
+        )
+        return button, image
+
 
 def _to_filename(id_: str, suffix: str = "") -> Path:
     """Converts an id with ":" and "_" to a filename with optional suffix."""
     filename = ASSETS_PATH / id_.replace("/", "_").replace(":", "_")
     return filename.with_suffix(suffix)
 
 
+def to_pandas_table(cls: type[BaseModel]) -> pd.DataFrame:
+    """Return a markdown table with the schema."""
+    import pandas as pd
+
+    rows = []
+    for k, field in cls.__fields__.items():
+        info = field.field_info
+        if info.description is None:
+            continue
+
+        def code(text: str) -> str:
+            return f"`{text}`"
+
+        row = {
+            "Variable name": code(k),
+            "Description": info.description,
+            "Default": code(info.default) if info.default is not Undefined else "",
+            "Type": code(field._type_display()),
+        }
+        rows.append(row)
+    return pd.DataFrame(rows)
+
+
+def _pandas_to_rich_table(df: pd.DataFrame) -> Table:
+    """Return a rich table from a pandas DataFrame."""
+    table = Table()
+
+    # Add the columns
+    for column in df.columns:
+        table.add_column(column)
+
+    # Add the rows
+    for _, row in df.iterrows():
+        table.add_row(*row.astype(str).tolist())
+
+    return table
+
+
 class Page(BaseModel):
     """A page of buttons."""
 
-    name: str
-    buttons: list[Button] = Field(default_factory=list)
+    name: str = Field(description="The name of the page.")
+    buttons: list[Button] = Field(
+        default_factory=list,
+        description="A list of buttons on the page.",
+    )
+
+    @classmethod
+    def to_pandas_table(cls: type[Page]) -> pd.DataFrame:
+        """Return a pandas DataFrame with the schema."""
+        return to_pandas_table(cls)
+
+    @classmethod
+    def to_markdown_table(cls: type[Page]) -> str:
+        """Return a markdown table with the schema."""
+        return cls.to_pandas_table().to_markdown(index=False)
 
 
 class Config(BaseModel):
     """Configuration file."""
 
-    pages: list[Page] = Field(default_factory=list)
-    current_page_index: int = 0
-    special_page: Page | None = None
-    state_entity_id: str | None = None
-    is_on: bool = True
-    brightness: int = 100
+    pages: list[Page] = Field(
+        default_factory=list,
+        description="A list of `Page`s in the configuration.",
+    )
+    anonymous_pages: list[Page] = Field(
+        default_factory=list,
+        description="A list of anonymous Pages in the configuration."
+        " These pages are hidden and not displayed when cycling through the pages."
+        " They can only be reached using the `special_type: 'go-to-page'` button."
+        " Designed for single use, these pages return to the previous page"
+        " upon clicking a button.",
+    )
+    state_entity_id: str | None = Field(
+        default=None,
+        description="The entity ID to sync display state with. For"
+        " example `input_boolean.streamdeck` or `binary_sensor.anyone_home`.",
+    )
+    brightness: int = Field(
+        default=100,
+        description="The default brightness of the Stream Deck (0-100).",
+    )
+    auto_reload: bool = Field(
+        default=False,
+        description="If True, the configuration YAML file will automatically"
+        " be reloaded when it is modified.",
+    )
+    _current_page_index: int = PrivateAttr(default=0)
+    _is_on: bool = PrivateAttr(default=True)
+    _detached_page: Page | None = PrivateAttr(default=None)
+    _configuration_file: Path | None = PrivateAttr(default=None)
+
+    @classmethod
+    def load(cls: type[Config], fname: Path) -> Config:
+        """Read the configuration file."""
+        with fname.open() as f:
+            data = yaml.safe_load(f)
+            config = cls(**data)
+            config._configuration_file = fname
+            return config
+
+    def reload(self) -> None:
+        """Reload the configuration file."""
+        assert self._configuration_file is not None
+        # Updates all public attributes
+        new = self.load(self._configuration_file).__dict__
+        self.__dict__.update(new)
+        # Set the private attributes we want to preserve
+        if self._detached_page is not None:
+            self._detached_page = self.to_page(self._detached_page.name)
+        if self._current_page_index >= len(self.pages):
+            # In case pages were removed, reset to the first page
+            self._current_page_index = 0
+
+    @classmethod
+    def to_pandas_table(cls: type[Config]) -> pd.DataFrame:
+        """Return a pandas DataFrame with the schema."""
+        return to_pandas_table(cls)
+
+    @classmethod
+    def to_markdown_table(cls: type[Config]) -> str:
+        """Return a markdown table with the schema."""
+        return cls.to_pandas_table().to_markdown(index=False)
+
+    def update_timers(
+        self,
+        deck: StreamDeck,
+        complete_state: dict[str, dict[str, Any]],
+    ) -> None:
+        """Update all timers."""
+        for key in range(deck.key_count()):
+            button = self.button(key)
+            if button is not None and button.is_sleeping():
+                console.log(f"Updating timer for key {key}")
+                update_key_image(
+                    deck,
+                    key=key,
+                    config=self,
+                    complete_state=complete_state,
+                    key_pressed=False,
+                )
 
     def next_page(self) -> Page:
         """Go to the next page."""
-        self.current_page_index = self.next_page_index
-        return self.pages[self.current_page_index]
+        self._current_page_index = self.next_page_index
+        return self.pages[self._current_page_index]
 
     @property
     def next_page_index(self) -> int:
         """Return the next page index."""
-        return (self.current_page_index + 1) % len(self.pages)
+        return (self._current_page_index + 1) % len(self.pages)
 
     @property
     def previous_page_index(self) -> int:
         """Return the previous page index."""
-        return (self.current_page_index - 1) % len(self.pages)
+        return (self._current_page_index - 1) % len(self.pages)
 
     def previous_page(self) -> Page:
         """Go to the previous page."""
-        self.current_page_index = self.previous_page_index
-        return self.pages[self.current_page_index]
+        self._current_page_index = self.previous_page_index
+        return self.pages[self._current_page_index]
 
     def current_page(self) -> Page:
         """Return the current page."""
-        if self.special_page is not None:
-            return self.special_page
-        return self.pages[self.current_page_index]
+        if self._detached_page is not None:
+            return self._detached_page
+        return self.pages[self._current_page_index]
 
     def button(self, key: int) -> Button | None:
         """Return the button for a key."""
         buttons = self.current_page().buttons
         if key < len(buttons):
             return buttons[key]
         return None
 
     def to_page(self, page: int | str) -> Page:
         """Go to a page based on the page name or index."""
         if isinstance(page, int):
-            self.current_page_index = page
-        else:
-            for i, p in enumerate(self.pages):
-                if p.name == page:
-                    self.current_page_index = i
-                    break
+            self._current_page_index = page
+            return self.current_page()
+
+        for i, p in enumerate(self.pages):
+            if p.name == page:
+                self._current_page_index = i
+                return self.current_page()
+
+        for p in self.anonymous_pages:
+            if p.name == page:
+                self._detached_page = p
+                return p
+        console.log(f"Could find page {page}, staying on current page")
         return self.current_page()
 
 
 def _next_id() -> int:
     global _ID_COUNTER
     _ID_COUNTER += 1
     return _ID_COUNTER
 
 
+class AsyncDelayedCallback:
+    """A callback that is called after a delay.
+
+    Parameters
+    ----------
+    delay
+        The delay in seconds after which the callback will be called.
+    callback
+        The function or coroutine to be called after the delay.
+    """
+
+    def __init__(
+        self,
+        delay: float,
+        callback: Callable[[], None | Coroutine] | None = None,
+    ) -> None:
+        """Initialize."""
+        self.delay = delay
+        self.callback = callback
+        self.task: asyncio.Task | None = None
+        self.start_time: float | None = None
+        self.is_sleeping: bool = False
+
+    async def _run(self) -> None:
+        """Run the timer. Don't call this directly, use start() instead."""
+        self.is_sleeping = True
+        self.start_time = time.time()
+        await asyncio.sleep(self.delay)
+        self.is_sleeping = False
+        if self.callback is not None:
+            if asyncio.iscoroutinefunction(self.callback):
+                await self.callback()
+            else:
+                self.callback()
+
+    def is_running(self) -> bool:
+        """Return whether the timer is running."""
+        return self.task is not None and not self.task.done()
+
+    def start(self) -> None:
+        """Start the timer."""
+        if self.task is not None and not self.task.done():
+            self.cancel()
+        self.task = asyncio.ensure_future(self._run())
+
+    def cancel(self) -> None:
+        """Cancel the timer."""
+        console.log("Cancel timer")
+        if self.task:
+            self.task.cancel()
+            self.is_sleeping = False
+            self.task = None
+
+    def remaining_time(self) -> float:
+        """Return the remaining time before the timer expires."""
+        if self.task is None:
+            return 0
+        if self.start_time is not None:
+            elapsed_time = time.time() - self.start_time
+            return max(0, self.delay - elapsed_time)
+        return 0
+
+
+def _draw_percentage_ring(
+    percentage: int | float,
+    size: tuple[int, int],
+    *,
+    radius: int | None = None,
+    thickness: int = 4,
+    ring_color: tuple[int, int, int] = (255, 0, 0),
+    full_ring_backgroud_color: tuple[int, int, int] = (100, 100, 100),
+) -> Image.Image:
+    """Draw a ring with a percentage."""
+    img = Image.new("RGB", size, (0, 0, 0))
+
+    if radius is None:
+        radius = size[0] // 2 - thickness // 2
+
+    # Draw the full ring for the background
+    draw = ImageDraw.Draw(img)
+    draw.ellipse(
+        [
+            (size[0] // 2 - radius, size[1] // 2 - radius),
+            (size[0] // 2 + radius, size[1] // 2 + radius),
+        ],
+        outline=full_ring_backgroud_color,
+        width=thickness,
+    )
+
+    # Draw the percentage of the ring with a bright color
+    start_angle = -90
+    end_angle = start_angle + (360 * percentage / 100)
+    draw.arc(
+        [
+            (size[0] // 2 - radius, size[1] // 2 - radius),
+            (size[0] // 2 + radius, size[1] // 2 + radius),
+        ],
+        start_angle,
+        end_angle,
+        fill=ring_color,
+        width=thickness,
+    )
+    return img
+
+
 def _linspace(start: float, stop: float, num: int) -> list[float]:
     """Return evenly spaced numbers over a specified interval."""
     if num == 1:
         return [start]
     step = (stop - start) / (num - 1)
     return [start + i * step for i in range(num)]
 
@@ -607,25 +936,62 @@
         "type": "subscribe_events",
         "event_type": "state_changed",
         "id": _next_id(),
     }
     await websocket.send(json.dumps(subscribe_payload))
 
 
-async def handle_state_changes(
+async def handle_changes(
     websocket: websockets.WebSocketClientProtocol,
     complete_state: StateDict,
     deck: StreamDeck,
     config: Config,
 ) -> None:
     """Handle state changes."""
-    # Wait for the state change events
-    while True:
-        data = json.loads(await websocket.recv())
-        _update_state(complete_state, data, config, deck)
+
+    async def process_websocket_messages() -> None:
+        """Process websocket messages."""
+        while True:
+            data = json.loads(await websocket.recv())
+            _update_state(complete_state, data, config, deck)
+
+    async def call_update_timers() -> None:
+        """Call config.update_timers every second."""
+        while True:
+            await asyncio.sleep(1)
+            config.update_timers(deck, complete_state)
+
+    async def watch_configuration_file() -> None:
+        """Watch for changes to the configuration file and reload config when it changes."""
+        if config._configuration_file is None:
+            console.log("[red bold] No configuration file to watch[/]")
+            return
+        last_modified_time = config._configuration_file.stat().st_mtime
+        while True:
+            if (
+                config.auto_reload
+                and config._configuration_file.stat().st_mtime != last_modified_time
+            ):
+                console.log("Configuration file has been modified, reloading")
+                last_modified_time = config._configuration_file.stat().st_mtime
+                try:
+                    config.reload()
+                    deck.reset()
+                    update_all_key_images(deck, config, complete_state)
+                except Exception as e:  # noqa: BLE001
+                    console.log(f"Error reloading configuration: {e}")
+
+            await asyncio.sleep(1)
+
+    # Run the websocket message processing and timer update tasks concurrently
+    await asyncio.gather(
+        process_websocket_messages(),
+        call_update_timers(),
+        watch_configuration_file(),
+    )
 
 
 def _keys(entity_id: str, buttons: list[Button]) -> list[int]:
     """Get the key indices for an entity_id."""
     return [i for i, button in enumerate(buttons) if button.entity_id == entity_id]
 
 
@@ -667,25 +1033,63 @@
 
 def _state_attr(
     entity_id: str,
     attr: str,
     complete_state: StateDict,
 ) -> Any:
     """Get the state attribute for an entity."""
-    return complete_state.get(entity_id, {}).get("attributes", {}).get(attr)
+    attrs = complete_state.get(entity_id, {}).get("attributes", {})
+    state_attr = attrs.get(attr)
+    return _maybe_number(state_attr)
 
 
 def _is_state_attr(
     entity_id: str,
     attr: str,
     value: Any,
     complete_state: StateDict,
 ) -> bool:
     """Check if the state attribute for an entity is a value."""
-    return _state_attr(entity_id, attr, complete_state) == value
+    return _state_attr(entity_id, attr, complete_state) == _maybe_number(value)
+
+
+def _is_float(s: str) -> bool:
+    try:
+        float(s)
+    except ValueError:
+        return False
+    else:
+        return True
+
+
+def _maybe_number(s: str, *, rounded: bool = False) -> int | str | float:
+    """Convert a string to a number if possible."""
+    if not isinstance(s, str):  # already a number or other type
+        return s
+
+    if _is_integer(s):
+        num = int(s)
+    elif _is_float(s):
+        num = float(s)  # type: ignore[assignment]
+    else:
+        return s
+
+    if rounded:
+        return round(num)
+
+    return num
+
+
+def _is_integer(s: str) -> bool:
+    try:
+        int(s)
+    except ValueError:
+        return False
+    else:
+        return True
 
 
 def _states(
     entity_id: str,
     *,
     with_unit: bool = False,
     rounded: bool = False,
@@ -693,30 +1097,29 @@
 ) -> Any:
     """Get the state for an entity."""
     assert complete_state is not None
     entity_state = complete_state.get(entity_id, {})
     if not entity_state:
         return None
     state = entity_state["state"]
+    state = _maybe_number(state, rounded=rounded)
     if with_unit:
         unit = entity_state.get("attributes", {}).get("unit_of_measurement")
         if unit:
             state += f" {unit}"
-    if rounded:
-        state = round(float(state))
     return state
 
 
 def _is_state(
     entity_id: str,
     state: str,
     complete_state: StateDict,
 ) -> bool:
     """Check if the state for an entity is a value."""
-    return _states(entity_id, complete_state=complete_state) == state
+    return _states(entity_id, complete_state=complete_state) == _maybe_number(state)
 
 
 def _min_filter(value: float, other_value: float) -> float:
     """Return the minimum of two values.
 
     Can be used in Jinja templates like
     >>> {{ 1 | min(2) }}
@@ -745,15 +1148,15 @@
         env = jinja2.Environment(
             loader=jinja2.BaseLoader(),
             autoescape=False,  # noqa: S701
         )
         env.filters["min"] = _min_filter
         env.filters["max"] = _max_filter
         template = env.from_string(text)
-        return template.render(  # noqa: TRY300
+        return template.render(
             min=min,
             max=max,
             is_state_attr=ft.partial(_is_state_attr, complete_state=complete_state),
             state_attr=ft.partial(_state_attr, complete_state=complete_state),
             states=ft.partial(_states, complete_state=complete_state),
             is_state=ft.partial(_is_state, complete_state=complete_state),
         ).strip()
@@ -862,24 +1265,21 @@
 def _init_icon(
     *,
     icon_filename: str | None = None,
     icon_mdi: str | None = None,
     icon_mdi_margin: int | None = None,
     icon_mdi_color: str | None = None,  # hex color
     icon_background_color: str | None = None,  # hex color
-    icon_convert_to_grayscale: bool = False,
     size: tuple[int, int] = (ICON_PIXELS, ICON_PIXELS),
 ) -> Image.Image:
     """Initialize the icon."""
     if icon_filename is not None:
         icon_path = Path(icon_filename)
         path = icon_path if icon_path.is_absolute() else ASSETS_PATH / icon_path
         icon = Image.open(path)
-        if icon_convert_to_grayscale:
-            icon = _convert_to_grayscale(icon)
         # Convert to RGB if needed
         if icon.mode != "RGB":
             icon = icon.convert("RGB")
         return icon
     if icon_mdi is not None:
         assert icon_mdi_margin is not None
         filename_svg = _download_and_save_mdi(icon_mdi)
@@ -895,24 +1295,26 @@
         icon_background_color = "white"
     color = _named_to_hex(icon_background_color)
     rgb_color = _hex_to_rgb(color)
     return Image.new("RGB", size, rgb_color)
 
 
 def _add_text(
+    *,
     image: Image.Image,
     font_filename: str,
     text_size: int,
     text: str,
     text_color: str,
+    text_offset: int = 0,
 ) -> None:
     draw = ImageDraw.Draw(image)
     font = ImageFont.truetype(str(ASSETS_PATH / font_filename), text_size)
     draw.text(
-        (image.width / 2, image.height / 2),
+        (image.width / 2, image.height / 2 + text_offset),
         text=text,
         font=font,
         anchor="ms",
         fill=text_color,
         align="center",
     )
 
@@ -976,128 +1378,131 @@
     if not found:
         msg = "No Stream Deck found"
         raise RuntimeError(msg)
     console.log(f"Found {deck.key_count()} keys, {deck=}")
     return deck
 
 
-def read_config(fname: Path) -> Config:
-    """Read the configuration file."""
-    with fname.open() as f:
-        data = yaml.safe_load(f)
-        return Config(
-            pages=data["pages"],
-            state_entity_id=data.get("state_entity_id"),
-            brightness=data.get("brightness", 100),
-        )
-
-
 def turn_on(config: Config, deck: StreamDeck, complete_state: StateDict) -> None:
     """Turn on the Stream Deck and update all key images."""
-    console.log(f"Calling turn_on, with {config.is_on=}")
-    if config.is_on:
+    console.log(f"Calling turn_on, with {config._is_on=}")
+    if config._is_on:
         return
-    config.is_on = True
+    config._is_on = True
     update_all_key_images(deck, config, complete_state)
     deck.set_brightness(config.brightness)
 
 
 def turn_off(config: Config, deck: StreamDeck) -> None:
     """Turn off the Stream Deck."""
-    console.log(f"Calling turn_off, with {config.is_on=}")
-    if not config.is_on:
+    console.log(f"Calling turn_off, with {config._is_on=}")
+    if not config._is_on:
         return
-    config.is_on = False
+    config._is_on = False
     # This resets all buttons except the turn-off button that
     # was just pressed, however, this doesn't matter with the
     # 0 brightness. Unless no button was pressed.
     deck.reset()
     deck.set_brightness(0)
 
 
 async def _handle_key_press(
     websocket: websockets.WebSocketClientProtocol,
     complete_state: StateDict,
     config: Config,
-    key: int,
+    button: Button,
     deck: StreamDeck,
 ) -> None:
-    if not config.is_on:
+    if not config._is_on:
         turn_on(config, deck, complete_state)
         return
-    button = config.button(key)
-    if button is None:
-        return
-    if button.special_type == "next-page":
-        config.next_page()
+
+    def update_all() -> None:
         deck.reset()
         update_all_key_images(deck, config, complete_state)
+
+    if button.special_type == "next-page":
+        config.next_page()
+        update_all()
     elif button.special_type == "previous-page":
         config.previous_page()
-        deck.reset()
-        update_all_key_images(deck, config, complete_state)
+        update_all()
     elif button.special_type == "go-to-page":
         assert isinstance(button.special_type_data, (str, int))
         config.to_page(button.special_type_data)  # type: ignore[arg-type]
-        deck.reset()
-        update_all_key_images(deck, config, complete_state)
+        update_all()
+        return  # to skip the _detached_page reset below
     elif button.special_type == "turn-off":
         turn_off(config, deck)
     elif button.special_type == "light-control":
         assert isinstance(button.special_type_data, dict)
         page = _light_page(
             entity_id=button.entity_id,
             n_colors=10,
             colormap=button.special_type_data.get("colormap", None),
             colors=button.special_type_data.get("colors", None),
         )
-        assert config.special_page is None
-        config.special_page = page
-        deck.reset()
-        update_all_key_images(deck, config, complete_state)
+        config._detached_page = page
+        update_all()
+        return  # to skip the _detached_page reset below
+    elif button.special_type == "reload":
+        config.reload()
+        update_all()
+        return
     elif button.service is not None:
         button = button.rendered_template_button(complete_state)
         if button.service_data is None:
             service_data = {}
             if button.entity_id is not None:
                 service_data["entity_id"] = button.entity_id
         else:
             service_data = button.service_data
         console.log(f"Calling service {button.service} with data {service_data}")
         assert button.service is not None  # for mypy
         await call_service(websocket, button.service, service_data, button.target)
 
+    if config._detached_page:
+        config._detached_page = None
+        update_all()
+
 
 def _on_press_callback(
     websocket: websockets.WebSocketClientProtocol,
     complete_state: StateDict,
     config: Config,
 ) -> Callable[[StreamDeck, int, bool], Coroutine[StreamDeck, int, None]]:
     async def key_change_callback(
         deck: StreamDeck,
         key: int,
         key_pressed: bool,  # noqa: FBT001
     ) -> None:
         console.log(f"Key {key} {'pressed' if key_pressed else 'released'}")
+
+        button = config.button(key)
+        assert button is not None
+        if button is not None and key_pressed:
+
+            async def cb() -> None:
+                """Update the deck once more after the timer is over."""
+                assert button is not None  # for mypy
+                await _handle_key_press(websocket, complete_state, config, button, deck)
+
+            if button.maybe_start_or_cancel_timer(cb):
+                key_pressed = False  # do not click now
+
         try:
             update_key_image(
                 deck,
                 key=key,
                 config=config,
                 complete_state=complete_state,
                 key_pressed=key_pressed,
             )
             if key_pressed:
-                has_special_page = config.special_page is not None
-                await _handle_key_press(websocket, complete_state, config, key, deck)
-                if has_special_page:
-                    # Reset after a keypress
-                    config.special_page = None
-                    deck.reset()
-                    update_all_key_images(deck, config, complete_state)
+                await _handle_key_press(websocket, complete_state, config, button, deck)
         except Exception as e:  # noqa: BLE001
             console.print_exception(show_locals=True)
             console.log(f"key_change_callback failed with a {type(e)}: {e}")
 
     return key_change_callback
 
 
@@ -1324,27 +1729,49 @@
         complete_state = await get_states(websocket)
         update_all_key_images(deck, config, complete_state)
         deck.set_key_callback_async(
             _on_press_callback(websocket, complete_state, config),
         )
         deck.set_brightness(config.brightness)
         await subscribe_state_changes(websocket)
-        await handle_state_changes(websocket, complete_state, deck, config)
+        await handle_changes(websocket, complete_state, deck, config)
+
+
+def _rich_table_str(df: pd.DataFrame) -> str:
+    table = _pandas_to_rich_table(df)
+    console = Console(file=io.StringIO(), width=120)
+    console.print(table)
+    return console.file.getvalue()
+
+
+def _help() -> str:
+    try:
+        return (
+            f"See the configuration options below:\n\n"
+            f"Config YAML options:\n{_rich_table_str(Config.to_pandas_table())}\n\n"
+            f"Page YAML options:\n{_rich_table_str(Page.to_pandas_table())}\n\n"
+            f"Button YAML options:\n{_rich_table_str(Button.to_pandas_table())}\n\n"
+        )
+    except ModuleNotFoundError:
+        return ""
 
 
 def main() -> None:
     """Start the Stream Deck integration."""
     import argparse
     import os
 
     from dotenv import load_dotenv
 
     load_dotenv()
 
-    parser = argparse.ArgumentParser()
+    parser = argparse.ArgumentParser(
+        epilog=_help(),
+        formatter_class=argparse.RawDescriptionHelpFormatter,
+    )
     parser.add_argument("--host", default=os.environ.get("HASS_HOST", "localhost"))
     parser.add_argument("--token", default=os.environ.get("HASS_TOKEN"))
     parser.add_argument(
         "--config",
         default=os.environ.get("STREAMDECK_CONFIG", DEFAULT_CONFIG),
         type=Path,
     )
@@ -1354,15 +1781,15 @@
         choices=["wss", "ws"],
     )
     args = parser.parse_args()
     console.log(f"Using version {__version__} of the Home Assistant Stream Deck.")
     console.log(
         f"Starting Stream Deck integration with {args.host=}, {args.config=}, {args.protocol=}",
     )
-    config = read_config(args.config)
+    config = Config.load(args.config)
     asyncio.run(
         run(
             host=args.host,
             token=args.token,
             protocol=args.protocol,
             config=config,
         ),
```

### Comparing `home_assistant_streamdeck_yaml-2023.4.9/pyproject.toml` & `home_assistant_streamdeck_yaml-2023.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 py-modules = ["home_assistant_streamdeck_yaml"]
 
 [tool.pytest.ini_options]
 addopts = """
     --cov=home_assistant_streamdeck_yaml
     --cov-report term
     --cov-report html
-    --cov-fail-under=64
+    --cov-fail-under=70
     --asyncio-mode=auto
 """
 
 [tool.coverage.report]
 exclude_lines = [
     "pragma: no cover",
     "raise NotImplementedError",
@@ -69,14 +69,15 @@
     "ANN101",  # Missing type annotation for {name} in method
     "S101",    # Use of assert detected
     "PD901",   # df is a bad variable name. Be kinder to your future self.
     "ANN401",  # Dynamically typed expressions (typing.Any) are disallowed in {name}
     "D402",    # First line should not be the function's signature
     "PLW0603", # Using the global statement to update `X` is discouraged
     "D401",    # First line of docstring should be in imperative mood
+    "SLF001",  # Private member accessed
 ]
 
 [tool.ruff.per-file-ignores]
 "tests/*" = ["SLF001"]
 "tests/test_examples.py" = ["E501"]
 ".github/*" = ["INP001"]
```

### Comparing `home_assistant_streamdeck_yaml-2023.4.9/systemd/home-assistant-streamdeck-yaml.service` & `home_assistant_streamdeck_yaml-2023.5.0/systemd/home-assistant-streamdeck-yaml.service`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.4.9/tests/state.json` & `home_assistant_streamdeck_yaml-2023.5.0/tests/state.json`

 * *Files identical despite different names*

### Comparing `home_assistant_streamdeck_yaml-2023.4.9/tests/test_app.py` & `home_assistant_streamdeck_yaml-2023.5.0/tests/test_app.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Test Home Assistant Stream Deck YAML."""
 from __future__ import annotations
 
+import asyncio
 import json
 import sys
 import textwrap
 from pathlib import Path
 from typing import Any
-from unittest.mock import Mock
+from unittest.mock import Mock, patch
 
 import pytest
 import websockets
 from dotenv import dotenv_values
 from PIL import Image
 from pydantic import ValidationError
 from StreamDeck.Devices.StreamDeckOriginal import StreamDeckOriginal
@@ -28,34 +29,43 @@
     _handle_key_press,
     _init_icon,
     _is_state,
     _is_state_attr,
     _keys,
     _light_page,
     _named_to_hex,
+    _on_press_callback,
     _render_jinja,
     _states,
     _to_filename,
     _url_to_filename,
     get_states,
-    read_config,
     setup_ws,
     update_key_image,
 )
 
 ROOT = Path(__file__).parent.parent
 sys.path.append(str(ROOT))
 TEST_STATE_FILENAME = ROOT / "tests" / "state.json"
 IS_CONNECTED_TO_HOMEASSISTANT = False
 BUTTONS_PER_PAGE = 15
 
 
-def test_read_config() -> None:
-    """Test read_config."""
-    read_config(DEFAULT_CONFIG)
+def test_load_config() -> None:
+    """Test Config.load."""
+    Config.load(DEFAULT_CONFIG)
+
+
+def test_reload_config() -> None:
+    """Test Config.load."""
+    c = Config.load(DEFAULT_CONFIG)
+    c.pages = []
+    assert c.pages == []
+    c.reload()
+    assert c.pages != []
 
 
 @pytest.fixture()
 def state() -> dict[str, dict[str, Any]]:
     """State fixture."""
     with TEST_STATE_FILENAME.open("r") as f:
         return json.load(f)
@@ -107,14 +117,15 @@
         "script_with_text": {
             "service": "script.reset_adaptive_lighting",
             "text": "Reset\nadaptive\nlighting\n",
         },
         "script_with_text_and_icon": {
             "service": "script.turn_off_everything",
             "text": "ALL OFF",
+            "text_offset": 4,
             "icon": "night_sky.png",
         },
         "input_select_with_template": {
             "entity_id": "input_select.sleep_mode",
             "service": "input_select.select_previous",
             "text": 'Sleep {{ states("input_select.sleep_mode") }}',
             "icon_mdi": "power-sleep",
@@ -127,14 +138,19 @@
             "service": "script.start_spotify",
             "service_data": {
                 "playlist": "37i9dQZF1DXaRycgyh6kXP",
                 "source": "KEF LS50",
             },
             "icon": "spotify:playlist/37i9dQZF1DXaRycgyh6kXP",
         },
+        "grayscale_button": {
+            "entity_id": "input_select.sleep_mode",
+            "icon": "spotify:playlist/37i9dQZF1DXaRycgyh6kXP",
+            "icon_gray_when_off": True,
+        },
         "special_empty": {"special_type": "empty"},
         "special_goto_0": {"special_type": "go-to-page", "special_type_data": 0},
         "special_goto_home": {
             "special_type": "go-to-page",
             "special_type_data": "Home",
         },
         "special_prev_page": {"special_type": "previous-page"},
@@ -158,51 +174,51 @@
         "light-control",
         "special_empty",
         "turn_off",
         "special_goto_0",
         "special_goto_home",
         "special_prev_page",
         "special_next_page",
+        "grayscale_button",
     ]
 
-    assert len(button_order) == BUTTONS_PER_PAGE
     return [Button(**button_dict[key]) for key in button_order]
 
 
 @pytest.fixture()
 def config(buttons: list[Button]) -> Config:
     """Config fixture."""
-    page_1 = Page(buttons=buttons, name="Home")
-    page_2 = Page(buttons=buttons[::-1], name="Second")
+    page_1 = Page(buttons=buttons[:BUTTONS_PER_PAGE], name="Home")
+    page_2 = Page(buttons=buttons[BUTTONS_PER_PAGE:], name="Second")
     return Config(pages=[page_1, page_2])
 
 
 def test_named_to_hex() -> None:
     """Test named to hex conversion."""
     assert _named_to_hex("red") == "#ff0000"
     assert _named_to_hex("#ff0000") == "#ff0000"
 
 
 def test_example_config_browsing_pages(config: Config) -> None:
     """Test example config browsing pages."""
     assert isinstance(config, Config)
-    assert config.current_page_index == 0
+    assert config._current_page_index == 0
     second_page = config.next_page()
     assert isinstance(second_page, Page)
-    assert config.current_page_index == 1
+    assert config._current_page_index == 1
     first_page = config.previous_page()
     assert isinstance(first_page, Page)
-    assert config.current_page_index == 0
+    assert config._current_page_index == 0
     assert len(first_page.buttons) == BUTTONS_PER_PAGE
-    assert len(second_page.buttons) == BUTTONS_PER_PAGE
+    assert len(second_page.buttons) == 1  # update when adding more buttons
     second_page = config.to_page(1)
     assert isinstance(second_page, Page)
-    assert config.current_page_index == 1
+    assert config._current_page_index == 1
     first_page = config.to_page(first_page.name)
-    assert config.current_page_index == 0
+    assert config._current_page_index == 0
     assert config.button(0) == first_page.buttons[0]
 
 
 @pytest.mark.skipif(
     not IS_CONNECTED_TO_HOMEASSISTANT,
     reason="Not connected to Home Assistant",
 )
@@ -301,15 +317,14 @@
     assert filename.exists()
     filename.unlink()
 
 
 def test_init_icon() -> None:
     """Test init icon."""
     _init_icon(icon_filename="xbox.png")
-    _init_icon(icon_filename="xbox.png", icon_convert_to_grayscale=True)
     _init_icon(
         icon_mdi="phone",
         icon_mdi_margin=1,
         icon_mdi_color="#ffbb00",
         size=(100, 100),
     )
     _init_icon(size=(100, 100))
@@ -346,15 +361,15 @@
     mock_deck: Mock,
     config: Config,
     state: dict[str, dict[str, Any]],
 ) -> None:
     """Test update_key_image with MockDeck."""
     update_key_image(mock_deck, key=0, config=config, complete_state=state)
     page = config.current_page()
-    assert config.current_page_index == 0
+    assert config._current_page_index == 0
     for key, _ in enumerate(page.buttons):
         update_key_image(mock_deck, key=key, config=config, complete_state=state)
 
     key_empty = next(
         (i for i, b in enumerate(page.buttons) if b.special_type == "empty"),
     )
     assert key_empty is not None
@@ -489,16 +504,17 @@
 async def test_handle_key_press_toggle_light(
     mock_deck: Mock,
     websocket_mock: Mock,
     state: dict[str, dict[str, Any]],
     config: Config,
 ) -> None:
     """Test handle_key_press toggle light."""
-    key = 0
-    await _handle_key_press(websocket_mock, state, config, key, mock_deck)
+    button = config.button(0)
+    assert button is not None
+    await _handle_key_press(websocket_mock, state, config, button, mock_deck)
 
     websocket_mock.send.assert_called_once()
     send_call_args = websocket_mock.send.call_args.args[0]
     payload = json.loads(send_call_args)
 
     assert payload["type"] == "call_service"
     assert payload["domain"] == "light"
@@ -509,22 +525,23 @@
 async def test_handle_key_press_next_page(
     websocket_mock: Mock,
     mock_deck: Mock,
     state: dict[str, dict[str, Any]],
     config: Config,
 ) -> None:
     """Test handle_key_press next page."""
-    key = 14
-    await _handle_key_press(websocket_mock, state, config, key, mock_deck)
+    button = config.button(14)
+    assert button is not None
+    await _handle_key_press(websocket_mock, state, config, button, mock_deck)
 
     # No service should be called
     websocket_mock.send.assert_not_called()
 
     # Ensure that the next_page method is called
-    assert config.current_page_index == 1
+    assert config._current_page_index == 1
 
 
 async def test_button_with_target(
     websocket_mock: Mock,
     mock_deck: Mock,
 ) -> None:
     """Test button with target."""
@@ -535,15 +552,15 @@
         },
         target={"entity_id": "media_player.1"},
     )
     config = Config(pages=[Page(buttons=[button], name="test")])
     _button = config.button(0)
     assert _button is not None
     assert _button.service == "media_player.join"
-    await _handle_key_press(websocket_mock, {}, config, 0, mock_deck)
+    await _handle_key_press(websocket_mock, {}, config, _button, mock_deck)
     # Check that the send method was called with the correct payload
     called_payload = json.loads(websocket_mock.send.call_args.args[0])
     expected_payload = {
         "id": called_payload["id"],  # Use the called id to match it
         "type": "call_service",
         "domain": "media_player",
         "service": "join",
@@ -1032,7 +1049,75 @@
     with pytest.warns(IconWarning):
         button.try_render_icon({})
 
     icon = button.try_render_icon({}, size=(100, 100))
     assert icon is not None
     assert isinstance(icon, Image.Image)
     assert icon.size == (100, 100)
+
+
+async def test_delay() -> None:
+    """Test the delay."""
+    button = Button(delay=0.1)
+    assert not button.is_sleeping()
+    assert button.maybe_start_or_cancel_timer()
+    await asyncio.sleep(0)  # TODO: figure out why this is needed
+    assert button._timer is not None
+    assert button._timer.is_sleeping
+    assert button.is_sleeping()
+    _ = button.render_icon({})
+    await asyncio.sleep(0.1)
+    assert not button.is_sleeping()
+
+
+def test_to_markdown_table() -> None:
+    """Test to_markdown_table for docs."""
+    table = Button.to_markdown_table()
+    assert isinstance(table, str)
+
+
+async def test_anonymous_page(
+    mock_deck: Mock,
+    websocket_mock: Mock,
+    state: dict[str, dict[str, Any]],
+) -> None:
+    """Test that the anonymous page works."""
+    home = Page(
+        name="home",
+        buttons=[Button(special_type="go-to-page", special_type_data="anon")],
+    )
+    anon = Page(
+        name="anon",
+        buttons=[Button(text="yolo"), Button(text="foo", delay=0.1)],
+    )
+    config = Config(pages=[home], anonymous_pages=[anon])
+    assert config._current_page_index == 0
+    assert config._detached_page is None
+    assert config.to_page("anon") == anon
+    assert config._detached_page is not None
+    assert config.current_page() == anon
+    button = config.button(0)
+    assert button.text == "yolo"
+    press = _on_press_callback(websocket_mock, state, config)
+    # Click the button
+    await press(mock_deck, 0, key_pressed=True)
+    # Should now be the button on the first page
+    button = config.button(0)
+    assert button.special_type == "go-to-page"
+    # Back to anon page
+    assert config.to_page("anon") == anon
+    # Click the delay button
+    button = config.button(1)
+    assert button.text == "foo"
+    await press(mock_deck, 1, key_pressed=True)
+    # Should now still be the button because of the delay
+    assert button.text == "foo"
+    assert config._detached_page is not None
+    assert config.current_page() == anon
+    with patch("home_assistant_streamdeck_yaml.update_all_key_images") as mock:
+        await asyncio.sleep(0.15)  # longer than delay should then switch to home
+        mock.assert_called_once()
+    assert config._detached_page is None
+    assert config.current_page() == home
+    # Should now be the button on the first page
+    button = config.button(0)
+    assert button.special_type == "go-to-page"
```

### Comparing `home_assistant_streamdeck_yaml-2023.4.9/tests/test_examples.py` & `home_assistant_streamdeck_yaml-2023.5.0/tests/test_examples.py`

 * *Files 3% similar despite different names*

```diff
@@ -250,81 +250,94 @@
             icon_mdi="fan-off",
             text="Bedroom\nOff",
         ),
     ],
 }
 
 lock_unlock_door = {
-    "description": "🔒 Lock/unlock a door",
+    "description": "🔒 Lock/unlock a door after 30 seconds",
     "yaml": textwrap.dedent(
         """
         - entity_id: lock.front_door
           service: lock.toggle
+          delay: "{{ 30 if is_state('lock.front_door', 'unlocked') else 0 }}"
           icon_mdi: "{{ 'door-open' if is_state('lock.front_door', 'unlocked') else 'door-closed' }}"
           text: |
             Front Door
             {{ 'Unlocked' if is_state('lock.front_door', 'unlocked') else 'Locked' }}
           text_size: 10
+          text_color: "{{ 'green' if is_state('lock.front_door', 'unlocked') else 'red' }}"
         """,
     ),
     "state": [
         {"lock.front_door": {"state": "unlocked"}},
         {"lock.front_door": {"state": "locked"}},
     ],
     "result": [
         Button(
             entity_id="lock.front_door",
             service="lock.toggle",
             icon_mdi="door-open",
             text="Front Door\nUnlocked",
             text_size=10,
+            delay=30.0,
+            text_color="green",
         ),
         Button(
             entity_id="lock.front_door",
             service="lock.toggle",
             icon_mdi="door-closed",
             text="Front Door\nLocked",
             text_size=10,
+            delay=0.0,
+            text_color="red",
         ),
     ],
 }
 
-
 arm_disarm_alarm_system = {
-    "description": "⚠️ Arm/disarm an alarm system",
+    "description": "⚠️ Arm/disarm an alarm system after 30 seconds",
+    "extra": "Arm the alarm system in 30 seconds if it's disarmed, disarm it immediately if it's armed.",
     "yaml": textwrap.dedent(
         """
         - entity_id: alarm_control_panel.home_alarm
+          delay: "{{ 0 if is_state('alarm_control_panel.home_alarm', 'armed_away') else 30 }}"
           service: "{{ 'alarm_control_panel.alarm_disarm' if is_state('alarm_control_panel.home_alarm', 'armed_away') else 'alarm_control_panel.alarm_arm_away' }}"
           icon_mdi: "{{ 'shield-check' if is_state('alarm_control_panel.home_alarm', 'armed_away') else 'shield-off' }}"
           text: |
             {{ 'Disarm' if is_state('alarm_control_panel.home_alarm', 'armed_away') else 'Arm' }}
             Alarm
+          text_color: "{{ 'red' if is_state('alarm_control_panel.home_alarm', 'armed_away') else 'green' }}"
         """,
     ),
     "state": [
         {"alarm_control_panel.home_alarm": {"state": "armed_away"}},
         {"alarm_control_panel.home_alarm": {"state": "disarmed"}},
     ],
     "result": [
         Button(
             entity_id="alarm_control_panel.home_alarm",
             service="alarm_control_panel.alarm_disarm",
             icon_mdi="shield-check",
             text="Disarm\nAlarm",
+            text_color="red",
+            delay=0.0,
         ),
         Button(
             entity_id="alarm_control_panel.home_alarm",
             service="alarm_control_panel.alarm_arm_away",
             icon_mdi="shield-off",
             text="Arm\nAlarm",
+            text_color="green",
+            delay=30.0,
         ),
     ],
 }
 
+
 set_alarm_time_for_next_day = {
     "description": "⏰ Set an alarm time for the next day",
     "yaml": textwrap.dedent(
         """
         - service: input_datetime.set_datetime
           service_data:
             entity_id: input_datetime.alarm_time
@@ -902,39 +915,45 @@
                 filename: "/config/www/recordings/camera_{{ now().strftime('%Y%m%d_%H%M%S') }}.mp4"
         ```
         """,
     ),
 }
 
 enable_disable_nightlight = {
-    "description": "🌙 Enable/disable a nightlight",
+    "description": "🌙 Enable/disable a nightlight after 30 min",
     "yaml": textwrap.dedent(
         """
         - entity_id: light.nightlight
           service: light.toggle
+          delay: 1800
           icon_mdi: "{{ 'lightbulb-on' if is_state('light.nightlight', 'on') else 'lightbulb-off' }}"
           text: "{{ 'Disable' if is_state('light.nightlight', 'on') else 'Enable' }} Nightlight"
+          text_color: "{{ 'red' if is_state('light.nightlight', 'on') else 'green' }}"
         """,
     ),
     "state": [
         {"light.nightlight": {"state": "on"}},
         {"light.nightlight": {"state": "off"}},
     ],
     "result": [
         Button(
             entity_id="light.nightlight",
             service="light.toggle",
             icon_mdi="lightbulb-on",
             text="Disable Nightlight",
+            text_color="red",
+            delay=1800.0,
         ),
         Button(
             entity_id="light.nightlight",
             service="light.toggle",
             icon_mdi="lightbulb-off",
             text="Enable Nightlight",
+            text_color="green",
+            delay=1800.0,
         ),
     ],
 }
 
 control_smart_fireplace = {
     "description": "🔥 Control a smart fireplace",
     "yaml": textwrap.dedent(
@@ -1086,34 +1105,117 @@
           service: media_player.toggle
           icon: >
             {% if is_state('media_player.tv', 'on') %}
             url:https://raw.githubusercontent.com/basnijholt/home-assistant-streamdeck-yaml/main/assets/fireplace.png
             {% else %}
             url:https://raw.githubusercontent.com/basnijholt/home-assistant-streamdeck-yaml/main/assets/hogwarts.png
             {% endif %}
+          text: >
+            Turn {{ 'Off' if is_state('media_player.tv', 'on') else 'On' }}
         """,
     ),
     "state": [
         {"media_player.tv": {"state": "on"}},
         {"media_player.tv": {"state": "off"}},
     ],
     "result": [
         Button(
             entity_id="media_player.tv",
             service="media_player.toggle",
             icon="url:https://raw.githubusercontent.com/basnijholt/home-assistant-streamdeck-yaml/main/assets/fireplace.png",
+            text="Turn Off",
         ),
         Button(
             entity_id="media_player.tv",
             service="media_player.toggle",
             icon="url:https://raw.githubusercontent.com/basnijholt/home-assistant-streamdeck-yaml/main/assets/hogwarts.png",
+            text="Turn On",
+        ),
+    ],
+}
+
+start_timer = {
+    "description": "⏰ Turn off all lights in 60s",
+    "yaml": textwrap.dedent(
+        """
+        - entity_id: light.all_lights
+          service: light.turn_off
+          text: |
+            Turn off
+            in 60s
+          delay: 60
+        """,
+    ),
+    "state": [{}],
+    "result": [
+        Button(
+            entity_id="light.all_lights",
+            service="light.turn_off",
+            text="Turn off\nin 60s\n",
+            delay=60.0,
+        ),
+    ],
+}
+
+
+outside_temperature_display = {
+    "description": "🌡️ Display outside temperature with a ring indicator",
+    "extra": "This sets 0% to -10°C and 100% to 40°C.",
+    "yaml": textwrap.dedent(
+        """
+        - entity_id: sensor.temperature_sensor_outside_temperature
+          icon: >
+            {%- set temp = states('sensor.temperature_sensor_outside_temperature') -%}
+            {%- set min_temp = -10 -%}
+            {%- set max_temp = 40 -%}
+            {%- set pct = ((temp - min_temp) / (max_temp - min_temp)) * 100 -%}
+            ring:{{ pct | round }}
+          text: |
+            {%- set temp = states('sensor.temperature_sensor_outside_temperature') -%}
+            Outside
+            {{ temp | round(1) }}°C
+        """,
+    ),
+    "state": [
+        {
+            "sensor.temperature_sensor_outside_temperature": {
+                "state": "20",
+            },
+        },
+        {
+            "sensor.temperature_sensor_outside_temperature": {
+                "state": "10",
+            },
+        },
+    ],
+    "result": [
+        Button(
+            entity_id="sensor.temperature_sensor_outside_temperature",
+            icon="ring:60.0",
+            text="Outside\n20°C",
+        ),
+        Button(
+            entity_id="sensor.temperature_sensor_outside_temperature",
+            icon="ring:40.0",
+            text="Outside\n10°C",
         ),
     ],
 }
 
+reload_configuration_yaml = {
+    "description": "🔄 Reload the `configuration.yaml` file",
+    "extra": "When pressed, the `configuration.yaml` is reloaded.",
+    "yaml": textwrap.dedent(
+        """
+        - special_type: reload
+        """,
+    ),
+    "state": [{}],
+    "result": [Button(special_type="reload")],
+}
 
 BUTTONS = [
     activate_a_scene,
     toggle_a_cover,
     start_or_stop_vacuum,
     mute_unmute_media_player,
     control_brightness_of_light,
@@ -1138,14 +1240,17 @@
     start_stop_security_camera_recording,
     enable_disable_nightlight,
     control_smart_fireplace,
     toggle_smart_plug,
     irrigation_toggle,
     change_cover_position,
     control_media_player_tv,
+    start_timer,
+    outside_temperature_display,
+    reload_configuration_yaml,
 ]
 
 
 @pytest.mark.parametrize("button_dct", BUTTONS)
 def test_button(button_dct: dict[str, Any]) -> None:
     """Test all buttons."""
     button = Button.from_yaml(button_dct["yaml"])  # type: ignore[arg-type]
```

