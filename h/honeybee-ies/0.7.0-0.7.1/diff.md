# Comparing `tmp/honeybee-ies-0.7.0.tar.gz` & `tmp/honeybee-ies-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/honeybee-ies-0.7.0.tar", last modified: Fri May 12 22:37:07 2023, max compression
+gzip compressed data, was "dist/honeybee-ies-0.7.1.tar", last modified: Sat May 20 20:36:59 2023, max compression
```

## Comparing `honeybee-ies-0.7.0.tar` & `honeybee-ies-0.7.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:37:07.000000 honeybee-ies-0.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:37:07.000000 honeybee-ies-0.7.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:37:07.000000 honeybee-ies-0.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-05-12 22:35:48.000000 honeybee-ies-0.7.0/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-12 22:35:48.000000 honeybee-ies-0.7.0/.github/workflows/dependency-release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-12 22:35:48.000000 honeybee-ies-0.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-12 22:35:48.000000 honeybee-ies-0.7.0/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-12 22:35:48.000000 honeybee-ies-0.7.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-12 22:35:48.000000 honeybee-ies-0.7.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-12 22:35:48.000000 honeybee-ies-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-12 22:37:07.000000 honeybee-ies-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-12 22:35:48.000000 honeybee-ies-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-12 22:35:48.000000 honeybee-ies-0.7.0/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-12 22:35:48.000000 honeybee-ies-0.7.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:37:07.000000 honeybee-ies-0.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-12 22:35:48.000000 honeybee-ies-0.7.0/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:37:07.000000 honeybee-ies-0.7.0/docs/_build/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 22:35:48.000000 honeybee-ies-0.7.0/docs/_build/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-12 22:35:48.000000 honeybee-ies-0.7.0/docs/_build/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:37:07.000000 honeybee-ies-0.7.0/docs/_build/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-12 22:35:48.000000 honeybee-ies-0.7.0/docs/_build/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:37:07.000000 honeybee-ies-0.7.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-12 22:35:48.000000 honeybee-ies-0.7.0/docs/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:37:07.000000 honeybee-ies-0.7.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-05-12 22:35:48.000000 honeybee-ies-0.7.0/docs/_templates/layout.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:37:07.000000 honeybee-ies-0.7.0/docs/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-12 22:35:48.000000 honeybee-ies-0.7.0/docs/cli/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    21471 2023-05-12 22:35:48.000000 honeybee-ies-0.7.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-12 22:35:48.000000 honeybee-ies-0.7.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-12 22:35:48.000000 honeybee-ies-0.7.0/docs/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:37:07.000000 honeybee-ies-0.7.0/honeybee_ies/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-12 22:35:48.000000 honeybee-ies-0.7.0/honeybee_ies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-12 22:35:48.000000 honeybee-ies-0.7.0/honeybee_ies/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-12 22:35:48.000000 honeybee-ies-0.7.0/honeybee_ies/_extend_honeybee.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:37:07.000000 honeybee-ies-0.7.0/honeybee_ies/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-12 22:35:48.000000 honeybee-ies-0.7.0/honeybee_ies/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-05-12 22:35:48.000000 honeybee-ies-0.7.0/honeybee_ies/cli/translate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8201 2023-05-12 22:35:48.000000 honeybee-ies-0.7.0/honeybee_ies/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-12 22:35:48.000000 honeybee-ies-0.7.0/honeybee_ies/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)    12240 2023-05-12 22:35:48.000000 honeybee-ies-0.7.0/honeybee_ies/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:37:07.000000 honeybee-ies-0.7.0/honeybee_ies.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-12 22:37:06.000000 honeybee-ies-0.7.0/honeybee_ies.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-12 22:37:07.000000 honeybee-ies-0.7.0/honeybee_ies.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 22:37:06.000000 honeybee-ies-0.7.0/honeybee_ies.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-12 22:37:06.000000 honeybee-ies-0.7.0/honeybee_ies.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-12 22:37:06.000000 honeybee-ies-0.7.0/honeybee_ies.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-12 22:37:06.000000 honeybee-ies-0.7.0/honeybee_ies.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-12 22:35:48.000000 honeybee-ies-0.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-12 22:37:07.000000 honeybee-ies-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-12 22:35:48.000000 honeybee-ies-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:37:07.000000 honeybee-ies-0.7.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:37:07.000000 honeybee-ies-0.7.0/tests/assets/
--rw-r--r--   0 runner    (1001) docker     (123)  2630219 2023-05-12 22:35:48.000000 honeybee-ies-0.7.0/tests/assets/lab_building.hbjson
--rw-r--r--   0 runner    (1001) docker     (123)    55839 2023-05-12 22:35:48.000000 honeybee-ies-0.7.0/tests/assets/model_with_holes.hbjson
--rw-r--r--   0 runner    (1001) docker     (123)   134559 2023-05-12 22:35:48.000000 honeybee-ies-0.7.0/tests/assets/multiline_name_test.hbjson
--rw-r--r--   0 runner    (1001) docker     (123)   274009 2023-05-12 22:35:48.000000 honeybee-ies-0.7.0/tests/assets/revit_sample_model.hbjson
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-12 22:35:48.000000 honeybee-ies-0.7.0/tests/assets/room_underground.gem
--rw-r--r--   0 runner    (1001) docker     (123)    47646 2023-05-12 22:35:48.000000 honeybee-ies-0.7.0/tests/assets/room_with_air_boundary.hbjson
--rw-r--r--   0 runner    (1001) docker     (123)    46729 2023-05-12 22:35:48.000000 honeybee-ies-0.7.0/tests/assets/sample_model_45.hbjson
--rw-r--r--   0 runner    (1001) docker     (123)    42885 2023-05-12 22:35:48.000000 honeybee-ies-0.7.0/tests/assets/shade_with_holes.hbjson
--rw-r--r--   0 runner    (1001) docker     (123)    46189 2023-05-12 22:35:48.000000 honeybee-ies-0.7.0/tests/assets/single_face_shade.hbjson
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:37:07.000000 honeybee-ies-0.7.0/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 22:35:48.000000 honeybee-ies-0.7.0/tests/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-12 22:35:48.000000 honeybee-ies-0.7.0/tests/cli/translate_cli_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-12 22:35:48.000000 honeybee-ies-0.7.0/tests/extend_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-12 22:35:48.000000 honeybee-ies-0.7.0/tests/reader_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-05-12 22:35:48.000000 honeybee-ies-0.7.0/tests/writer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:36:59.000000 honeybee-ies-0.7.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:36:59.000000 honeybee-ies-0.7.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:36:59.000000 honeybee-ies-0.7.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-05-20 20:35:41.000000 honeybee-ies-0.7.1/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-20 20:35:41.000000 honeybee-ies-0.7.1/.github/workflows/dependency-release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-20 20:35:41.000000 honeybee-ies-0.7.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-20 20:35:41.000000 honeybee-ies-0.7.1/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-20 20:35:41.000000 honeybee-ies-0.7.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-20 20:35:41.000000 honeybee-ies-0.7.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-20 20:35:41.000000 honeybee-ies-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-20 20:36:59.000000 honeybee-ies-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-20 20:35:41.000000 honeybee-ies-0.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-20 20:35:41.000000 honeybee-ies-0.7.1/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-20 20:35:41.000000 honeybee-ies-0.7.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:36:59.000000 honeybee-ies-0.7.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-20 20:35:41.000000 honeybee-ies-0.7.1/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:36:59.000000 honeybee-ies-0.7.1/docs/_build/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 20:35:41.000000 honeybee-ies-0.7.1/docs/_build/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-20 20:35:41.000000 honeybee-ies-0.7.1/docs/_build/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:36:59.000000 honeybee-ies-0.7.1/docs/_build/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-20 20:35:41.000000 honeybee-ies-0.7.1/docs/_build/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:36:59.000000 honeybee-ies-0.7.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-20 20:35:41.000000 honeybee-ies-0.7.1/docs/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:36:59.000000 honeybee-ies-0.7.1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-05-20 20:35:41.000000 honeybee-ies-0.7.1/docs/_templates/layout.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:36:59.000000 honeybee-ies-0.7.1/docs/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-20 20:35:41.000000 honeybee-ies-0.7.1/docs/cli/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    21471 2023-05-20 20:35:41.000000 honeybee-ies-0.7.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-20 20:35:41.000000 honeybee-ies-0.7.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-20 20:35:41.000000 honeybee-ies-0.7.1/docs/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:36:59.000000 honeybee-ies-0.7.1/honeybee_ies/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-20 20:35:41.000000 honeybee-ies-0.7.1/honeybee_ies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-20 20:35:41.000000 honeybee-ies-0.7.1/honeybee_ies/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-20 20:35:41.000000 honeybee-ies-0.7.1/honeybee_ies/_extend_honeybee.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:36:59.000000 honeybee-ies-0.7.1/honeybee_ies/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-20 20:35:41.000000 honeybee-ies-0.7.1/honeybee_ies/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-05-20 20:35:41.000000 honeybee-ies-0.7.1/honeybee_ies/cli/translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8203 2023-05-20 20:35:41.000000 honeybee-ies-0.7.1/honeybee_ies/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-20 20:35:41.000000 honeybee-ies-0.7.1/honeybee_ies/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12240 2023-05-20 20:35:41.000000 honeybee-ies-0.7.1/honeybee_ies/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:36:59.000000 honeybee-ies-0.7.1/honeybee_ies.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-20 20:36:59.000000 honeybee-ies-0.7.1/honeybee_ies.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-20 20:36:59.000000 honeybee-ies-0.7.1/honeybee_ies.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 20:36:59.000000 honeybee-ies-0.7.1/honeybee_ies.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-20 20:36:59.000000 honeybee-ies-0.7.1/honeybee_ies.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-20 20:36:59.000000 honeybee-ies-0.7.1/honeybee_ies.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-20 20:36:59.000000 honeybee-ies-0.7.1/honeybee_ies.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-20 20:35:41.000000 honeybee-ies-0.7.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-20 20:36:59.000000 honeybee-ies-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-20 20:35:41.000000 honeybee-ies-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:36:59.000000 honeybee-ies-0.7.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:36:59.000000 honeybee-ies-0.7.1/tests/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)  2630219 2023-05-20 20:35:41.000000 honeybee-ies-0.7.1/tests/assets/lab_building.hbjson
+-rw-r--r--   0 runner    (1001) docker     (123)    55839 2023-05-20 20:35:41.000000 honeybee-ies-0.7.1/tests/assets/model_with_holes.hbjson
+-rw-r--r--   0 runner    (1001) docker     (123)   134559 2023-05-20 20:35:41.000000 honeybee-ies-0.7.1/tests/assets/multiline_name_test.hbjson
+-rw-r--r--   0 runner    (1001) docker     (123)   274009 2023-05-20 20:35:41.000000 honeybee-ies-0.7.1/tests/assets/revit_sample_model.hbjson
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-20 20:35:41.000000 honeybee-ies-0.7.1/tests/assets/room_underground.gem
+-rw-r--r--   0 runner    (1001) docker     (123)    47646 2023-05-20 20:35:41.000000 honeybee-ies-0.7.1/tests/assets/room_with_air_boundary.hbjson
+-rw-r--r--   0 runner    (1001) docker     (123)    46729 2023-05-20 20:35:41.000000 honeybee-ies-0.7.1/tests/assets/sample_model_45.hbjson
+-rw-r--r--   0 runner    (1001) docker     (123)    42885 2023-05-20 20:35:41.000000 honeybee-ies-0.7.1/tests/assets/shade_with_holes.hbjson
+-rw-r--r--   0 runner    (1001) docker     (123)    46189 2023-05-20 20:35:41.000000 honeybee-ies-0.7.1/tests/assets/single_face_shade.hbjson
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:36:59.000000 honeybee-ies-0.7.1/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 20:35:41.000000 honeybee-ies-0.7.1/tests/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-20 20:35:41.000000 honeybee-ies-0.7.1/tests/cli/translate_cli_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-20 20:35:41.000000 honeybee-ies-0.7.1/tests/extend_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-20 20:35:41.000000 honeybee-ies-0.7.1/tests/reader_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-05-20 20:35:41.000000 honeybee-ies-0.7.1/tests/writer_test.py
```

### Comparing `honeybee-ies-0.7.0/.github/workflows/ci.yaml` & `honeybee-ies-0.7.1/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `honeybee-ies-0.7.0/.github/workflows/dependency-release.yaml` & `honeybee-ies-0.7.1/.github/workflows/dependency-release.yaml`

 * *Files identical despite different names*

### Comparing `honeybee-ies-0.7.0/LICENSE` & `honeybee-ies-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `honeybee-ies-0.7.0/PKG-INFO` & `honeybee-ies-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-ies
-Version: 0.7.0
+Version: 0.7.1
 Summary: Honeybee extension for import and export to/from IES-VE
 Home-page: https://github.com/ladybug-tools/honeybee-ies
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `honeybee-ies-0.7.0/README.md` & `honeybee-ies-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `honeybee-ies-0.7.0/docs/_static/custom.css` & `honeybee-ies-0.7.1/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `honeybee-ies-0.7.0/docs/_templates/layout.html` & `honeybee-ies-0.7.1/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `honeybee-ies-0.7.0/docs/conf.py` & `honeybee-ies-0.7.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `honeybee-ies-0.7.0/honeybee_ies/cli/translate.py` & `honeybee-ies-0.7.1/honeybee_ies/cli/translate.py`

 * *Files identical despite different names*

### Comparing `honeybee-ies-0.7.0/honeybee_ies/reader.py` & `honeybee-ies-0.7.1/honeybee_ies/reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,11 +200,11 @@
         if isinstance(r, Room):
             rooms.append(r)
         else:
             shades.extend(r)
 
     model = Model(
         clean_string(gem_file.stem), rooms=rooms, units='Meters', orphaned_shades=shades,
-        tolerance=0.01
+        tolerance=0.0001
     )
     model.display_name = gem_file.stem
     return model
```

### Comparing `honeybee-ies-0.7.0/honeybee_ies/templates.py` & `honeybee-ies-0.7.1/honeybee_ies/templates.py`

 * *Files identical despite different names*

### Comparing `honeybee-ies-0.7.0/honeybee_ies/writer.py` & `honeybee-ies-0.7.1/honeybee_ies/writer.py`

 * *Files identical despite different names*

### Comparing `honeybee-ies-0.7.0/honeybee_ies.egg-info/PKG-INFO` & `honeybee-ies-0.7.1/honeybee_ies.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-ies
-Version: 0.7.0
+Version: 0.7.1
 Summary: Honeybee extension for import and export to/from IES-VE
 Home-page: https://github.com/ladybug-tools/honeybee-ies
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `honeybee-ies-0.7.0/honeybee_ies.egg-info/SOURCES.txt` & `honeybee-ies-0.7.1/honeybee_ies.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `honeybee-ies-0.7.0/setup.py` & `honeybee-ies-0.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `honeybee-ies-0.7.0/tests/assets/lab_building.hbjson` & `honeybee-ies-0.7.1/tests/assets/lab_building.hbjson`

 * *Files identical despite different names*

### Comparing `honeybee-ies-0.7.0/tests/assets/model_with_holes.hbjson` & `honeybee-ies-0.7.1/tests/assets/model_with_holes.hbjson`

 * *Files identical despite different names*

### Comparing `honeybee-ies-0.7.0/tests/assets/multiline_name_test.hbjson` & `honeybee-ies-0.7.1/tests/assets/multiline_name_test.hbjson`

 * *Files identical despite different names*

### Comparing `honeybee-ies-0.7.0/tests/assets/revit_sample_model.hbjson` & `honeybee-ies-0.7.1/tests/assets/revit_sample_model.hbjson`

 * *Files identical despite different names*

### Comparing `honeybee-ies-0.7.0/tests/assets/room_underground.gem` & `honeybee-ies-0.7.1/tests/assets/room_underground.gem`

 * *Files identical despite different names*

### Comparing `honeybee-ies-0.7.0/tests/assets/room_with_air_boundary.hbjson` & `honeybee-ies-0.7.1/tests/assets/room_with_air_boundary.hbjson`

 * *Files identical despite different names*

### Comparing `honeybee-ies-0.7.0/tests/assets/sample_model_45.hbjson` & `honeybee-ies-0.7.1/tests/assets/sample_model_45.hbjson`

 * *Files identical despite different names*

### Comparing `honeybee-ies-0.7.0/tests/assets/shade_with_holes.hbjson` & `honeybee-ies-0.7.1/tests/assets/shade_with_holes.hbjson`

 * *Files identical despite different names*

### Comparing `honeybee-ies-0.7.0/tests/assets/single_face_shade.hbjson` & `honeybee-ies-0.7.1/tests/assets/single_face_shade.hbjson`

 * *Files identical despite different names*

### Comparing `honeybee-ies-0.7.0/tests/cli/translate_cli_test.py` & `honeybee-ies-0.7.1/tests/cli/translate_cli_test.py`

 * *Files identical despite different names*

### Comparing `honeybee-ies-0.7.0/tests/writer_test.py` & `honeybee-ies-0.7.1/tests/writer_test.py`

 * *Files identical despite different names*

