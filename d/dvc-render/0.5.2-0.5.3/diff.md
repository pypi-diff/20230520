# Comparing `tmp/dvc-render-0.5.2.tar.gz` & `tmp/dvc-render-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvc-render-0.5.2.tar", last modified: Wed May 17 08:30:14 2023, max compression
+gzip compressed data, was "dvc-render-0.5.3.tar", last modified: Sat May 20 07:59:16 2023, max compression
```

## Comparing `dvc-render-0.5.2.tar` & `dvc-render-0.5.3.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:30:14.672426 dvc-render-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-17 08:29:46.000000 dvc-render-0.5.2/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-17 08:29:46.000000 dvc-render-0.5.2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:30:14.664426 dvc-render-0.5.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-17 08:29:46.000000 dvc-render-0.5.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:30:14.664426 dvc-render-0.5.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-17 08:29:46.000000 dvc-render-0.5.2/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-17 08:29:46.000000 dvc-render-0.5.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-17 08:29:46.000000 dvc-render-0.5.2/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-17 08:29:46.000000 dvc-render-0.5.2/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-17 08:29:46.000000 dvc-render-0.5.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-05-17 08:29:46.000000 dvc-render-0.5.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-05-17 08:29:46.000000 dvc-render-0.5.2/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-17 08:29:46.000000 dvc-render-0.5.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-05-17 08:29:46.000000 dvc-render-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-05-17 08:30:14.672426 dvc-render-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-05-17 08:29:46.000000 dvc-render-0.5.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:30:14.664426 dvc-render-0.5.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:30:14.664426 dvc-render-0.5.2/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-05-17 08:29:46.000000 dvc-render-0.5.2/docs/assets/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-17 08:29:46.000000 dvc-render-0.5.2/docs/gen_ref_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-17 08:29:46.000000 dvc-render-0.5.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-17 08:29:46.000000 dvc-render-0.5.2/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-17 08:29:46.000000 dvc-render-0.5.2/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-17 08:29:46.000000 dvc-render-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-17 08:30:14.672426 dvc-render-0.5.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:30:14.660426 dvc-render-0.5.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:30:14.668426 dvc-render-0.5.2/src/dvc_render/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-17 08:29:46.000000 dvc-render-0.5.2/src/dvc_render/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-17 08:29:46.000000 dvc-render-0.5.2/src/dvc_render/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-17 08:29:46.000000 dvc-render-0.5.2/src/dvc_render/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-17 08:29:46.000000 dvc-render-0.5.2/src/dvc_render/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-17 08:29:46.000000 dvc-render-0.5.2/src/dvc_render/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-17 08:29:46.000000 dvc-render-0.5.2/src/dvc_render/markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-05-17 08:29:46.000000 dvc-render-0.5.2/src/dvc_render/plotly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-17 08:29:46.000000 dvc-render-0.5.2/src/dvc_render/table.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-17 08:29:46.000000 dvc-render-0.5.2/src/dvc_render/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-05-17 08:29:46.000000 dvc-render-0.5.2/src/dvc_render/vega.py
--rw-r--r--   0 runner    (1001) docker     (123)    24018 2023-05-17 08:29:46.000000 dvc-render-0.5.2/src/dvc_render/vega_templates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:30:14.668426 dvc-render-0.5.2/src/dvc_render.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-05-17 08:30:14.000000 dvc-render-0.5.2/src/dvc_render.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-17 08:30:14.000000 dvc-render-0.5.2/src/dvc_render.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 08:30:14.000000 dvc-render-0.5.2/src/dvc_render.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 08:30:14.000000 dvc-render-0.5.2/src/dvc_render.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-17 08:30:14.000000 dvc-render-0.5.2/src/dvc_render.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-17 08:30:14.000000 dvc-render-0.5.2/src/dvc_render.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:30:14.672426 dvc-render-0.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 08:29:46.000000 dvc-render-0.5.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-05-17 08:29:46.000000 dvc-render-0.5.2/tests/test_html.py
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-05-17 08:29:46.000000 dvc-render-0.5.2/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-17 08:29:46.000000 dvc-render-0.5.2/tests/test_markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-17 08:29:46.000000 dvc-render-0.5.2/tests/test_parallel_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-17 08:29:46.000000 dvc-render-0.5.2/tests/test_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-17 08:29:46.000000 dvc-render-0.5.2/tests/test_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-05-17 08:29:46.000000 dvc-render-0.5.2/tests/test_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-05-17 08:29:46.000000 dvc-render-0.5.2/tests/test_vega.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:59:16.171728 dvc-render-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-20 07:58:44.000000 dvc-render-0.5.3/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-20 07:58:44.000000 dvc-render-0.5.3/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:59:16.167729 dvc-render-0.5.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-20 07:58:44.000000 dvc-render-0.5.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:59:16.167729 dvc-render-0.5.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-20 07:58:44.000000 dvc-render-0.5.3/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-20 07:58:44.000000 dvc-render-0.5.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-20 07:58:44.000000 dvc-render-0.5.3/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-20 07:58:44.000000 dvc-render-0.5.3/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-20 07:58:44.000000 dvc-render-0.5.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-05-20 07:58:44.000000 dvc-render-0.5.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-05-20 07:58:44.000000 dvc-render-0.5.3/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-20 07:58:44.000000 dvc-render-0.5.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-05-20 07:58:44.000000 dvc-render-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-05-20 07:59:16.175729 dvc-render-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-05-20 07:58:44.000000 dvc-render-0.5.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:59:16.167729 dvc-render-0.5.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:59:16.167729 dvc-render-0.5.3/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-05-20 07:58:44.000000 dvc-render-0.5.3/docs/assets/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-20 07:58:44.000000 dvc-render-0.5.3/docs/gen_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-20 07:58:44.000000 dvc-render-0.5.3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-20 07:58:44.000000 dvc-render-0.5.3/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-20 07:58:44.000000 dvc-render-0.5.3/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-20 07:58:44.000000 dvc-render-0.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-20 07:59:16.175729 dvc-render-0.5.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:59:16.163728 dvc-render-0.5.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:59:16.171728 dvc-render-0.5.3/src/dvc_render/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-20 07:58:44.000000 dvc-render-0.5.3/src/dvc_render/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-20 07:58:44.000000 dvc-render-0.5.3/src/dvc_render/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-20 07:58:44.000000 dvc-render-0.5.3/src/dvc_render/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-20 07:58:44.000000 dvc-render-0.5.3/src/dvc_render/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-20 07:58:44.000000 dvc-render-0.5.3/src/dvc_render/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-20 07:58:44.000000 dvc-render-0.5.3/src/dvc_render/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-05-20 07:58:44.000000 dvc-render-0.5.3/src/dvc_render/plotly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-20 07:58:44.000000 dvc-render-0.5.3/src/dvc_render/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-20 07:58:44.000000 dvc-render-0.5.3/src/dvc_render/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-05-20 07:58:44.000000 dvc-render-0.5.3/src/dvc_render/vega.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24185 2023-05-20 07:58:44.000000 dvc-render-0.5.3/src/dvc_render/vega_templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:59:16.171728 dvc-render-0.5.3/src/dvc_render.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-05-20 07:59:16.000000 dvc-render-0.5.3/src/dvc_render.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-20 07:59:16.000000 dvc-render-0.5.3/src/dvc_render.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 07:59:16.000000 dvc-render-0.5.3/src/dvc_render.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 07:59:15.000000 dvc-render-0.5.3/src/dvc_render.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-20 07:59:16.000000 dvc-render-0.5.3/src/dvc_render.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-20 07:59:16.000000 dvc-render-0.5.3/src/dvc_render.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:59:16.171728 dvc-render-0.5.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:58:44.000000 dvc-render-0.5.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-05-20 07:58:44.000000 dvc-render-0.5.3/tests/test_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-05-20 07:58:44.000000 dvc-render-0.5.3/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-20 07:58:44.000000 dvc-render-0.5.3/tests/test_markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-20 07:58:44.000000 dvc-render-0.5.3/tests/test_parallel_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-20 07:58:44.000000 dvc-render-0.5.3/tests/test_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-20 07:58:44.000000 dvc-render-0.5.3/tests/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-05-20 07:58:44.000000 dvc-render-0.5.3/tests/test_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-05-20 07:58:44.000000 dvc-render-0.5.3/tests/test_vega.py
```

### Comparing `dvc-render-0.5.2/.cruft.json` & `dvc-render-0.5.3/.cruft.json`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.2/.github/dependabot.yml` & `dvc-render-0.5.3/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.2/.github/workflows/docs.yml` & `dvc-render-0.5.3/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.2/.github/workflows/release.yml` & `dvc-render-0.5.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.2/.github/workflows/tests.yml` & `dvc-render-0.5.3/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.2/.gitignore` & `dvc-render-0.5.3/.gitignore`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.2/.pre-commit-config.yaml` & `dvc-render-0.5.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.2/CODE_OF_CONDUCT.rst` & `dvc-render-0.5.3/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.2/CONTRIBUTING.rst` & `dvc-render-0.5.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.2/LICENSE` & `dvc-render-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.2/PKG-INFO` & `dvc-render-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc-render
-Version: 0.5.2
+Version: 0.5.3
 Summary: DVC render
 Home-page: https://github.com/iterative/dvc-render
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dvc-render-0.5.2/README.rst` & `dvc-render-0.5.3/README.rst`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.2/docs/assets/logo.svg` & `dvc-render-0.5.3/docs/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.2/docs/gen_ref_pages.py` & `dvc-render-0.5.3/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.2/mkdocs.yml` & `dvc-render-0.5.3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.2/noxfile.py` & `dvc-render-0.5.3/noxfile.py`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.2/pyproject.toml` & `dvc-render-0.5.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.2/setup.cfg` & `dvc-render-0.5.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.2/src/dvc_render/base.py` & `dvc-render-0.5.3/src/dvc_render/base.py`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.2/src/dvc_render/html.py` & `dvc-render-0.5.3/src/dvc_render/html.py`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.2/src/dvc_render/image.py` & `dvc-render-0.5.3/src/dvc_render/image.py`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.2/src/dvc_render/markdown.py` & `dvc-render-0.5.3/src/dvc_render/markdown.py`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.2/src/dvc_render/plotly.py` & `dvc-render-0.5.3/src/dvc_render/plotly.py`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.2/src/dvc_render/table.py` & `dvc-render-0.5.3/src/dvc_render/table.py`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.2/src/dvc_render/vega.py` & `dvc-render-0.5.3/src/dvc_render/vega.py`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.2/src/dvc_render/vega_templates.py` & `dvc-render-0.5.3/src/dvc_render/vega_templates.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,24 +57,29 @@
         elif isinstance(e, str):
             if e == name:
                 e = value
         x.append(e)
     return x
 
 
-def dict_find_value(d: dict, value: str) -> bool:
-    for v in d.values():
-        if isinstance(v, dict):
-            if dict_find_value(v, value):
-                return True
-        if isinstance(v, str):
-            if v == value:
-                return True
-        if isinstance(v, list):
-            return any(dict_find_value(e, value) for e in v)
+def find_value(d: Union[dict, list, str], value: str) -> bool:
+    if isinstance(d, dict):
+        for v in d.values():
+            if isinstance(v, dict):
+                if find_value(v, value):
+                    return True
+            if isinstance(v, str):
+                if v == value:
+                    return True
+            if isinstance(v, list):
+                if any(find_value(e, value) for e in v):
+                    return True
+    elif isinstance(d, str):
+        if d == value:
+            return True
     return False
 
 
 class Template:
     EXTENSION = ".json"
     ANCHOR = "<DVC_METRIC_{}>"
 
@@ -116,15 +121,15 @@
 
     def reset(self):
         """Reset self.content to its original state."""
         self.content = self._original_content
 
     def has_anchor(self, name) -> bool:
         "Check if ANCHOR formatted with name is in content."
-        found = dict_find_value(self.content, self.anchor(name))
+        found = find_value(self.content, self.anchor(name))
         return found
 
     def fill_anchor(self, name, value) -> None:
         "Replace anchor `name` with `value` in content."
         self.content = dict_replace_value(self.content, self.anchor(name), value)
```

### Comparing `dvc-render-0.5.2/src/dvc_render.egg-info/PKG-INFO` & `dvc-render-0.5.3/src/dvc_render.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc-render
-Version: 0.5.2
+Version: 0.5.3
 Summary: DVC render
 Home-page: https://github.com/iterative/dvc-render
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dvc-render-0.5.2/src/dvc_render.egg-info/SOURCES.txt` & `dvc-render-0.5.3/src/dvc_render.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.2/src/dvc_render.egg-info/requires.txt` & `dvc-render-0.5.3/src/dvc_render.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.2/tests/test_html.py` & `dvc-render-0.5.3/tests/test_html.py`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.2/tests/test_image.py` & `dvc-render-0.5.3/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.2/tests/test_markdown.py` & `dvc-render-0.5.3/tests/test_markdown.py`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.2/tests/test_parallel_coordinates.py` & `dvc-render-0.5.3/tests/test_parallel_coordinates.py`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.2/tests/test_table.py` & `dvc-render-0.5.3/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `dvc-render-0.5.2/tests/test_templates.py` & `dvc-render-0.5.3/tests/test_templates.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from dvc_render.vega_templates import (
     TEMPLATES,
     LinearTemplate,
     ScatterTemplate,
     Template,
     TemplateContentDoesNotMatch,
     TemplateNotFoundError,
-    dict_find_value,
     dump_templates,
+    find_value,
     get_template,
 )
 
 # pylint: disable=missing-function-docstring, unused-argument
 
 
 def test_raise_on_no_template():
@@ -106,11 +106,12 @@
 
 @pytest.mark.parametrize(
     "content_dict, value_name",
     [
         ({"key": "value"}, "value"),
         ({"key": {"subkey": "value"}}, "value"),
         ({"key": [{"subkey": "value"}]}, "value"),
+        ({"key1": [{"subkey": "foo"}], "key2": {"subkey2": "value"}}, "value"),
     ],
 )
-def test_dict_find_value(content_dict, value_name):
-    assert dict_find_value(content_dict, value_name)
+def test_find_value(content_dict, value_name):
+    assert find_value(content_dict, value_name)
```

### Comparing `dvc-render-0.5.2/tests/test_vega.py` & `dvc-render-0.5.3/tests/test_vega.py`

 * *Files 6% similar despite different names*

```diff
@@ -106,28 +106,43 @@
 
 
 def test_bad_template_on_init():
     with pytest.raises(BadTemplateError):
         Template("name", "content")
 
 
-def test_bad_template_on_missing_data(tmp_dir):
-    template_content = {"data": {"values": "BAD_ANCHOR"}}
-    tmp_dir.gen("bar.json", json.dumps(template_content))
+@pytest.mark.parametrize(
+    "bad_content,good_content",
+    (
+        (
+            {"data": {"values": "BAD_ANCHOR"}},
+            {"data": {"values": Template.anchor("data")}},
+        ),
+        (
+            {"mark": {"type": "bar"}, "data": {"values": "BAD_ANCHOR"}},
+            {"mark": {"type": "bar"}, "data": {"values": Template.anchor("data")}},
+        ),
+        (
+            {"repeat": ["quintile"], "spec": {"data": {"values": "BAD_ANCHOR"}}},
+            {
+                "repeat": ["quintile"],
+                "spec": {"data": {"values": Template.anchor("data")}},
+            },
+        ),
+    ),
+)
+def test_bad_template_on_missing_data(tmp_dir, bad_content, good_content):
+    tmp_dir.gen("bar.json", json.dumps(bad_content))
     datapoints = [{"val": 2}, {"val": 3}]
     renderer = VegaRenderer(datapoints, "foo", template="bar.json")
 
     with pytest.raises(BadTemplateError):
         renderer.get_filled_template()
 
-    template_content = {
-        "mark": {"type": "bar"},
-        "data": {"values": Template.anchor("data")},
-    }
-    tmp_dir.gen("bar.json", json.dumps(template_content))
+    tmp_dir.gen("bar.json", json.dumps(good_content))
     renderer = VegaRenderer(datapoints, "foo", template="bar.json")
     assert renderer.get_filled_template()
 
 
 def test_raise_on_wrong_field():
     datapoints = [{"val": 2}, {"val": 3}]
     props = {"x": "no_val"}
```

