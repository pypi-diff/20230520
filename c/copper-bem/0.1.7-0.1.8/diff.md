# Comparing `tmp/copper-bem-0.1.7.tar.gz` & `tmp/copper-bem-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copper-bem-0.1.7.tar", last modified: Wed Feb 15 18:31:08 2023, max compression
+gzip compressed data, was "copper-bem-0.1.8.tar", last modified: Sat May 20 06:20:21 2023, max compression
```

## Comparing `copper-bem-0.1.7.tar` & `copper-bem-0.1.8.tar`

### file list

```diff
@@ -1,67 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 18:31:08.931490 copper-bem-0.1.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 18:31:08.923490 copper-bem-0.1.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 18:31:08.927490 copper-bem-0.1.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-02-15 18:31:01.000000 copper-bem-0.1.7/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-02-15 18:31:01.000000 copper-bem-0.1.7/.github/workflows/draft-pdf.yml
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-02-15 18:31:01.000000 copper-bem-0.1.7/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-02-15 18:31:01.000000 copper-bem-0.1.7/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-02-15 18:31:01.000000 copper-bem-0.1.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-02-15 18:31:01.000000 copper-bem-0.1.7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-02-15 18:31:08.931490 copper-bem-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-02-15 18:31:01.000000 copper-bem-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 18:31:08.927490 copper-bem-0.1.7/copper/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-02-15 18:31:01.000000 copper-bem-0.1.7/copper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29682 2023-02-15 18:31:01.000000 copper-bem-0.1.7/copper/chiller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-02-15 18:31:01.000000 copper-bem-0.1.7/copper/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-02-15 18:31:01.000000 copper-bem-0.1.7/copper/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    36034 2023-02-15 18:31:01.000000 copper-bem-0.1.7/copper/curves.py
--rw-r--r--   0 runner    (1001) docker     (123)    26045 2023-02-15 18:31:01.000000 copper-bem-0.1.7/copper/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-02-15 18:31:01.000000 copper-bem-0.1.7/copper/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 18:31:08.927490 copper-bem-0.1.7/copper/lib/
--rw-r--r--   0 runner    (1001) docker     (123)  1021792 2023-02-15 18:31:01.000000 copper-bem-0.1.7/copper/lib/chiller_curves.json
--rw-r--r--   0 runner    (1001) docker     (123)    13952 2023-02-15 18:31:01.000000 copper-bem-0.1.7/copper/library.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-02-15 18:31:01.000000 copper-bem-0.1.7/copper/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 18:31:08.931490 copper-bem-0.1.7/copper_bem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-02-15 18:31:08.000000 copper-bem-0.1.7/copper_bem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-02-15 18:31:08.000000 copper-bem-0.1.7/copper_bem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 18:31:08.000000 copper-bem-0.1.7/copper_bem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-02-15 18:31:08.000000 copper-bem-0.1.7/copper_bem.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-02-15 18:31:08.000000 copper-bem-0.1.7/copper_bem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-15 18:31:08.000000 copper-bem-0.1.7/copper_bem.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 18:31:08.931490 copper-bem-0.1.7/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-02-15 18:31:01.000000 copper-bem-0.1.7/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-02-15 18:31:01.000000 copper-bem-0.1.7/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-02-15 18:31:01.000000 copper-bem-0.1.7/docs/paper.bib
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-02-15 18:31:01.000000 copper-bem-0.1.7/docs/paper.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 18:31:08.931490 copper-bem-0.1.7/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-02-15 18:31:01.000000 copper-bem-0.1.7/docs/source/Acknowledgement.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-02-15 18:31:01.000000 copper-bem-0.1.7/docs/source/Additional Examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-02-15 18:31:01.000000 copper-bem-0.1.7/docs/source/Applications.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-02-15 18:31:01.000000 copper-bem-0.1.7/docs/source/Chillers.rst
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-02-15 18:31:01.000000 copper-bem-0.1.7/docs/source/Code Documentation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-02-15 18:31:01.000000 copper-bem-0.1.7/docs/source/Contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-02-15 18:31:01.000000 copper-bem-0.1.7/docs/source/Equipment.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-02-15 18:31:01.000000 copper-bem-0.1.7/docs/source/Introduction.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-02-15 18:31:01.000000 copper-bem-0.1.7/docs/source/License.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-02-15 18:31:01.000000 copper-bem-0.1.7/docs/source/Methodology.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-02-15 18:31:01.000000 copper-bem-0.1.7/docs/source/Quickstart Guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)    35912 2023-02-15 18:31:01.000000 copper-bem-0.1.7/docs/source/chiller_curves.png
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-02-15 18:31:01.000000 copper-bem-0.1.7/docs/source/chiller_lib_summary.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-02-15 18:31:01.000000 copper-bem-0.1.7/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-02-15 18:31:01.000000 copper-bem-0.1.7/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    42295 2023-02-15 18:31:01.000000 copper-bem-0.1.7/docs/source/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-02-15 18:31:01.000000 copper-bem-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-02-15 18:31:01.000000 copper-bem-0.1.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-15 18:31:08.931490 copper-bem-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-02-15 18:31:01.000000 copper-bem-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 18:31:08.931490 copper-bem-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 18:31:01.000000 copper-bem-0.1.7/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 18:31:08.931490 copper-bem-0.1.7/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-02-15 18:31:01.000000 copper-bem-0.1.7/tests/data/agg_curves.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-02-15 18:31:01.000000 copper-bem-0.1.7/tests/test_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     9649 2023-02-15 18:31:01.000000 copper-bem-0.1.7/tests/test_chiller.py
--rw-r--r--   0 runner    (1001) docker     (123)    11035 2023-02-15 18:31:01.000000 copper-bem-0.1.7/tests/test_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)    11591 2023-02-15 18:31:01.000000 copper-bem-0.1.7/tests/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-02-15 18:31:01.000000 copper-bem-0.1.7/tests/test_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-02-15 18:31:01.000000 copper-bem-0.1.7/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-02-15 18:31:01.000000 copper-bem-0.1.7/tests/test_units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:20:21.928361 copper-bem-0.1.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:20:21.916361 copper-bem-0.1.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:20:21.920361 copper-bem-0.1.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-20 06:20:10.000000 copper-bem-0.1.8/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-20 06:20:10.000000 copper-bem-0.1.8/.github/workflows/draft-pdf.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-20 06:20:10.000000 copper-bem-0.1.8/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-20 06:20:10.000000 copper-bem-0.1.8/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-20 06:20:10.000000 copper-bem-0.1.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-20 06:20:10.000000 copper-bem-0.1.8/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-05-20 06:20:21.928361 copper-bem-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-05-20 06:20:10.000000 copper-bem-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:20:21.920361 copper-bem-0.1.8/copper/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-20 06:20:10.000000 copper-bem-0.1.8/copper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29682 2023-05-20 06:20:10.000000 copper-bem-0.1.8/copper/chiller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-05-20 06:20:10.000000 copper-bem-0.1.8/copper/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-20 06:20:10.000000 copper-bem-0.1.8/copper/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36034 2023-05-20 06:20:10.000000 copper-bem-0.1.8/copper/curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26045 2023-05-20 06:20:10.000000 copper-bem-0.1.8/copper/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-20 06:20:10.000000 copper-bem-0.1.8/copper/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:20:21.920361 copper-bem-0.1.8/copper/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)  1021792 2023-05-20 06:20:10.000000 copper-bem-0.1.8/copper/lib/chiller_curves.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13952 2023-05-20 06:20:10.000000 copper-bem-0.1.8/copper/library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-05-20 06:20:10.000000 copper-bem-0.1.8/copper/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:20:21.924361 copper-bem-0.1.8/copper_bem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-05-20 06:20:21.000000 copper-bem-0.1.8/copper_bem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-20 06:20:21.000000 copper-bem-0.1.8/copper_bem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 06:20:21.000000 copper-bem-0.1.8/copper_bem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-20 06:20:21.000000 copper-bem-0.1.8/copper_bem.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-20 06:20:21.000000 copper-bem-0.1.8/copper_bem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-20 06:20:21.000000 copper-bem-0.1.8/copper_bem.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:20:21.924361 copper-bem-0.1.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-20 06:20:10.000000 copper-bem-0.1.8/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-20 06:20:10.000000 copper-bem-0.1.8/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-05-20 06:20:10.000000 copper-bem-0.1.8/docs/paper.bib
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-05-20 06:20:10.000000 copper-bem-0.1.8/docs/paper.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:20:21.924361 copper-bem-0.1.8/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-20 06:20:10.000000 copper-bem-0.1.8/docs/source/Acknowledgement.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-20 06:20:10.000000 copper-bem-0.1.8/docs/source/Additional Examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-20 06:20:10.000000 copper-bem-0.1.8/docs/source/Applications.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-20 06:20:10.000000 copper-bem-0.1.8/docs/source/Chillers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-20 06:20:10.000000 copper-bem-0.1.8/docs/source/Code Documentation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-20 06:20:10.000000 copper-bem-0.1.8/docs/source/Contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-20 06:20:10.000000 copper-bem-0.1.8/docs/source/Equipment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-05-20 06:20:10.000000 copper-bem-0.1.8/docs/source/Introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-20 06:20:10.000000 copper-bem-0.1.8/docs/source/License.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-20 06:20:10.000000 copper-bem-0.1.8/docs/source/Methodology.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-05-20 06:20:10.000000 copper-bem-0.1.8/docs/source/Quickstart Guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    35912 2023-05-20 06:20:10.000000 copper-bem-0.1.8/docs/source/chiller_curves.png
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-20 06:20:10.000000 copper-bem-0.1.8/docs/source/chiller_lib_summary.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-05-20 06:20:10.000000 copper-bem-0.1.8/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-20 06:20:10.000000 copper-bem-0.1.8/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    42295 2023-05-20 06:20:10.000000 copper-bem-0.1.8/docs/source/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-20 06:20:10.000000 copper-bem-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-20 06:20:10.000000 copper-bem-0.1.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 06:20:21.928361 copper-bem-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-20 06:20:10.000000 copper-bem-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:20:21.924361 copper-bem-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 06:20:10.000000 copper-bem-0.1.8/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:20:21.928361 copper-bem-0.1.8/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-20 06:20:10.000000 copper-bem-0.1.8/tests/data/agg_curves.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-20 06:20:10.000000 copper-bem-0.1.8/tests/data/cli_input_file.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-20 06:20:10.000000 copper-bem-0.1.8/tests/test_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9649 2023-05-20 06:20:10.000000 copper-bem-0.1.8/tests/test_chiller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-20 06:20:10.000000 copper-bem-0.1.8/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11035 2023-05-20 06:20:10.000000 copper-bem-0.1.8/tests/test_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11591 2023-05-20 06:20:10.000000 copper-bem-0.1.8/tests/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-05-20 06:20:10.000000 copper-bem-0.1.8/tests/test_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-05-20 06:20:10.000000 copper-bem-0.1.8/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-05-20 06:20:10.000000 copper-bem-0.1.8/tests/test_units.py
```

### Comparing `copper-bem-0.1.7/.github/workflows/docs.yml` & `copper-bem-0.1.8/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `copper-bem-0.1.7/.github/workflows/draft-pdf.yml` & `copper-bem-0.1.8/.github/workflows/draft-pdf.yml`

 * *Files identical despite different names*

### Comparing `copper-bem-0.1.7/.github/workflows/tests.yml` & `copper-bem-0.1.8/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `copper-bem-0.1.7/LICENSE.md` & `copper-bem-0.1.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `copper-bem-0.1.7/PKG-INFO` & `copper-bem-0.1.8/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: copper-bem
-Version: 0.1.7
+Version: 0.1.8
 Summary: Performance curve generator for building energy simulation
 Home-page: https://github.com/pnnl/copper
 Author: Jérémy Lerond
 Author-email: jeremy.lerond@pnnl.gov
 Keywords: building energy simulation performance curves
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Copper
 Copper is a building energy simulation performance curve generator for heating, ventilation, and air-conditioning equipment. It uses a genetic algorithm to modify existing or a set of aggregated existing performance curves to match specific design characteristics including full and part load energy performance metric values.
 
 Copper generates performance curves that can be used in most common building energy software such as [EnergyPlus](https://energyplus.net/) or [DOE-2](https://doe2.com/).
 
 ![Tests](https://github.com/lymereJ/copper/actions/workflows/tests.yml/badge.svg)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7644215.svg)](https://doi.org/10.5281/zenodo.7644215)
+[![status](https://joss.theoj.org/papers/9509076e1ef0a0c05f141fde6810c313/status.svg)](https://joss.theoj.org/papers/9509076e1ef0a0c05f141fde6810c313)
 
 # Purpose
 Results from building energy simulations largely depend on how heating and cooling equipment are modeled. As they rarely operate at their full load and rated performance it is important that reasonable data is used to model an heating or cooling equipment's part load performance. Copper was created to allow building energy modelers, engineers, and researchers to generate simulation-ready performance curves of heating and cooling equipment that not only capture their typical behavior at part load but are also generated to match a set of design characteristics such as full load and part load efficiencies.
 
 While chillers, which are rated at both full load and part load through an integrated part load value (IPLV), are currently the main application of Copper, other heating and cooling equipment will be handled in the near future.
 
 # Documentation
```

### Comparing `copper-bem-0.1.7/README.md` & `copper-bem-0.1.8/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Copper
 Copper is a building energy simulation performance curve generator for heating, ventilation, and air-conditioning equipment. It uses a genetic algorithm to modify existing or a set of aggregated existing performance curves to match specific design characteristics including full and part load energy performance metric values.
 
 Copper generates performance curves that can be used in most common building energy software such as [EnergyPlus](https://energyplus.net/) or [DOE-2](https://doe2.com/).
 
 ![Tests](https://github.com/lymereJ/copper/actions/workflows/tests.yml/badge.svg)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7644215.svg)](https://doi.org/10.5281/zenodo.7644215)
+[![status](https://joss.theoj.org/papers/9509076e1ef0a0c05f141fde6810c313/status.svg)](https://joss.theoj.org/papers/9509076e1ef0a0c05f141fde6810c313)
 
 # Purpose
 Results from building energy simulations largely depend on how heating and cooling equipment are modeled. As they rarely operate at their full load and rated performance it is important that reasonable data is used to model an heating or cooling equipment's part load performance. Copper was created to allow building energy modelers, engineers, and researchers to generate simulation-ready performance curves of heating and cooling equipment that not only capture their typical behavior at part load but are also generated to match a set of design characteristics such as full load and part load efficiencies.
 
 While chillers, which are rated at both full load and part load through an integrated part load value (IPLV), are currently the main application of Copper, other heating and cooling equipment will be handled in the near future.
 
 # Documentation
```

### Comparing `copper-bem-0.1.7/copper/chiller.py` & `copper-bem-0.1.8/copper/chiller.py`

 * *Files identical despite different names*

### Comparing `copper-bem-0.1.7/copper/cli.py` & `copper-bem-0.1.8/copper/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 """
 cli.py
 ====================================
 This the command line interface module of Copper. It faciliate the integration of Copper into different workflow by being about to run some of Copper's functionality through command line.
 """
 
 import click, json, inspect
-import copper.chiller as chiller
+
+# import copper.Chiller as chiller
+from copper.chiller import Chiller
 
 
 @click.group()
 def cli():
     """
-    Command Line Interface for Copper
+    Copper
+
+    A performance curve generator for building energy simulation
     """
 
 
 @cli.command()
 @click.argument("input_file", type=click.File("rb"), required=True)
 def run(input_file):
+    """Run a set of Copper instructions through a JSON input file. See 'Using Copper's command line interface in the Quickstart Guide section of the documenation for more information."""
     try:
         f = json.load(input_file)
     except:
         raise ValueError("Could not read the input file. A JSON file is expected.")
     for eqp, eqp_props in f.items():
         # Make sure that the equipment is supported by Copper
-        assert eqp_props["eqp_type"].lower() in ["chiller"]
+        assert eqp_props["eqp_type"].lower() in [
+            "chiller"
+        ], "Equipment type not currently supported by Copper."
 
         # Get properties for equipment type
         eqp_type_props = inspect.getfullargspec(eval(eqp_props["eqp_type"]).__init__)[0]
 
         # Set the equipment properties from input file
         obj_args = {}
         for p in eqp_type_props:
```

### Comparing `copper-bem-0.1.7/copper/curves.py` & `copper-bem-0.1.8/copper/curves.py`

 * *Files identical despite different names*

### Comparing `copper-bem-0.1.7/copper/generator.py` & `copper-bem-0.1.8/copper/generator.py`

 * *Files identical despite different names*

### Comparing `copper-bem-0.1.7/copper/helpers.py` & `copper-bem-0.1.8/copper/helpers.py`

 * *Files identical despite different names*

### Comparing `copper-bem-0.1.7/copper/lib/chiller_curves.json` & `copper-bem-0.1.8/copper/lib/chiller_curves.json`

 * *Files identical despite different names*

### Comparing `copper-bem-0.1.7/copper/library.py` & `copper-bem-0.1.8/copper/library.py`

 * *Files identical despite different names*

### Comparing `copper-bem-0.1.7/copper/units.py` & `copper-bem-0.1.8/copper/units.py`

 * *Files identical despite different names*

### Comparing `copper-bem-0.1.7/copper_bem.egg-info/PKG-INFO` & `copper-bem-0.1.8/copper_bem.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: copper-bem
-Version: 0.1.7
+Version: 0.1.8
 Summary: Performance curve generator for building energy simulation
 Home-page: https://github.com/pnnl/copper
 Author: Jérémy Lerond
 Author-email: jeremy.lerond@pnnl.gov
 Keywords: building energy simulation performance curves
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Copper
 Copper is a building energy simulation performance curve generator for heating, ventilation, and air-conditioning equipment. It uses a genetic algorithm to modify existing or a set of aggregated existing performance curves to match specific design characteristics including full and part load energy performance metric values.
 
 Copper generates performance curves that can be used in most common building energy software such as [EnergyPlus](https://energyplus.net/) or [DOE-2](https://doe2.com/).
 
 ![Tests](https://github.com/lymereJ/copper/actions/workflows/tests.yml/badge.svg)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7644215.svg)](https://doi.org/10.5281/zenodo.7644215)
+[![status](https://joss.theoj.org/papers/9509076e1ef0a0c05f141fde6810c313/status.svg)](https://joss.theoj.org/papers/9509076e1ef0a0c05f141fde6810c313)
 
 # Purpose
 Results from building energy simulations largely depend on how heating and cooling equipment are modeled. As they rarely operate at their full load and rated performance it is important that reasonable data is used to model an heating or cooling equipment's part load performance. Copper was created to allow building energy modelers, engineers, and researchers to generate simulation-ready performance curves of heating and cooling equipment that not only capture their typical behavior at part load but are also generated to match a set of design characteristics such as full load and part load efficiencies.
 
 While chillers, which are rated at both full load and part load through an integrated part load value (IPLV), are currently the main application of Copper, other heating and cooling equipment will be handled in the near future.
 
 # Documentation
```

### Comparing `copper-bem-0.1.7/copper_bem.egg-info/SOURCES.txt` & `copper-bem-0.1.8/copper_bem.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -43,13 +43,15 @@
 docs/source/chiller_lib_summary.csv
 docs/source/conf.py
 docs/source/index.rst
 docs/source/logo.png
 tests/__init__.py
 tests/test_benchmark.py
 tests/test_chiller.py
+tests/test_cli.py
 tests/test_curves.py
 tests/test_generator.py
 tests/test_library.py
 tests/test_logging.py
 tests/test_units.py
-tests/data/agg_curves.pkl
+tests/data/agg_curves.pkl
+tests/data/cli_input_file.json
```

### Comparing `copper-bem-0.1.7/docs/Makefile` & `copper-bem-0.1.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `copper-bem-0.1.7/docs/make.bat` & `copper-bem-0.1.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `copper-bem-0.1.7/docs/paper.bib` & `copper-bem-0.1.8/docs/paper.bib`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 @misc {ahri_550590,
     title={550/590 Performance Rating of Water-chilling and Heat Pump Water-heating Packages Using the Vapor Compression Cycle},
-    author={AHRI},
+    author={{AHRI}},
     organization={AHRI},
     institution ={AHRI},
     address={Arlington, VA},
     year={2020}
 }
 
 @misc {ahri_551591,
     title={551/591 Performance Rating of Water-chilling and Heat Pump Water-heating Packages Using the Vapor Compression Cycle},
-    author={AHRI},
+    author={{AHRI}},
     organization={AHRI},
     institution ={AHRI},
     address={Arlington, VA},
     year={2020}
 }
 
 @misc {90.1,
     title={ANSI/ASHRAE/IES 90.1-2019, Energy Standard for Buildings Except Low-Rise Residential Buildings},
-    author={ASHRAE},
+    author={{ASHRAE}},
     organization={ASHRAE},
     institution={ASHRAE},
     address={Atlanta, GA},
     year={2019}
 }
 
 @article{ashrae_conf_paper,
@@ -33,40 +33,40 @@
     volume={125},
     number={2},
     pages={93}
 }
 
 @misc{comnet,
     title={COMNET, Appendix H - Equipment Performance Curves},
-    author={COMNET},
+    author={{COMNET}},
     howpublished={\url{https://comnet.org/}},
     note={Accessed: 2022-09-22}
 }
 
 @misc{osti_1395882,
     title={EnergyPlus™},
     author={},
     abstractNote={Originally developed in 1999. EnergyPlus™ is a whole building energy simulation program that engineers, architects, and researchers use to model both energy consumption—for heating, cooling, ventilation, lighting and plug and process loads—and water use in buildings. EnergyPlus is a console-based program that reads input and writes output to text files. It ships with a number of utilities including IDF-Editor for creating input files using a simple spreadsheet-like interface, EP-Launch for managing input and output files and performing batch simulations, and EP-Compare for graphically comparing the results of two or more simulations. Several comprehensive graphical interfaces for EnergyPlus are also available. DOE does most of its work with EnergyPlus using the OpenStudio® software development kit and suite of applications. DOE releases major updates to EnergyPlus twice annually.},
     url={https://www.osti.gov//servlets/purl/1395882},
     doi={},
     url={https://www.osti.gov/biblio/1395882}
 }
 
 @software{doe2,
-  author={James J. Hirsch & Associates (JJH)},
+  author={{James J. Hirsch & Associates (JJH)}},
   title={DOE-2.2},
   url={https://www.doe2.com/}
 }
 
 @misc{addendumbd,
-    author={ASHRAE},
+    author={{ASHRAE}},
     title={Addendum bd to Standard 90.1-2019, Energy Standard for Buildings Except Low-Rise Residential Buildings},
     institution={ASHRAE},
     year={2022}
 }
 
 @misc{tspr,
     title={TSPR Washington State Analysis Tool},
-    author={PNNL},
+    author={{Pacific Northwest National Laboratory}},
     howpublished={\url{https://energycode.pnl.gov/HVACSystemPerformance/}},
     note={Accessed: 2022-09-22}
 }
```

### Comparing `copper-bem-0.1.7/docs/paper.md` & `copper-bem-0.1.8/docs/paper.md`

 * *Files identical despite different names*

### Comparing `copper-bem-0.1.7/docs/source/Additional Examples.rst` & `copper-bem-0.1.8/docs/source/Additional Examples.rst`

 * *Files identical despite different names*

### Comparing `copper-bem-0.1.7/docs/source/Applications.rst` & `copper-bem-0.1.8/docs/source/Applications.rst`

 * *Files identical despite different names*

### Comparing `copper-bem-0.1.7/docs/source/Chillers.rst` & `copper-bem-0.1.8/docs/source/Chillers.rst`

 * *Files identical despite different names*

### Comparing `copper-bem-0.1.7/docs/source/Code Documentation.rst` & `copper-bem-0.1.8/docs/source/Code Documentation.rst`

 * *Files identical despite different names*

### Comparing `copper-bem-0.1.7/docs/source/Contributing.rst` & `copper-bem-0.1.8/docs/source/Contributing.rst`

 * *Files identical despite different names*

### Comparing `copper-bem-0.1.7/docs/source/Introduction.rst` & `copper-bem-0.1.8/docs/source/Introduction.rst`

 * *Files identical despite different names*

### Comparing `copper-bem-0.1.7/docs/source/License.rst` & `copper-bem-0.1.8/docs/source/License.rst`

 * *Files identical despite different names*

### Comparing `copper-bem-0.1.7/docs/source/Methodology.rst` & `copper-bem-0.1.8/docs/source/Methodology.rst`

 * *Files identical despite different names*

### Comparing `copper-bem-0.1.7/docs/source/Quickstart Guide.rst` & `copper-bem-0.1.8/docs/source/Quickstart Guide.rst`

 * *Files identical despite different names*

### Comparing `copper-bem-0.1.7/docs/source/chiller_curves.png` & `copper-bem-0.1.8/docs/source/chiller_curves.png`

 * *Files identical despite different names*

### Comparing `copper-bem-0.1.7/docs/source/chiller_lib_summary.csv` & `copper-bem-0.1.8/docs/source/chiller_lib_summary.csv`

 * *Files identical despite different names*

### Comparing `copper-bem-0.1.7/docs/source/conf.py` & `copper-bem-0.1.8/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `copper-bem-0.1.7/docs/source/index.rst` & `copper-bem-0.1.8/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `copper-bem-0.1.7/docs/source/logo.png` & `copper-bem-0.1.8/docs/source/logo.png`

 * *Files identical despite different names*

### Comparing `copper-bem-0.1.7/setup.py` & `copper-bem-0.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `copper-bem-0.1.7/tests/data/agg_curves.pkl` & `copper-bem-0.1.8/tests/data/agg_curves.pkl`

 * *Files identical despite different names*

### Comparing `copper-bem-0.1.7/tests/test_benchmark.py` & `copper-bem-0.1.8/tests/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `copper-bem-0.1.7/tests/test_chiller.py` & `copper-bem-0.1.8/tests/test_chiller.py`

 * *Files identical despite different names*

### Comparing `copper-bem-0.1.7/tests/test_curves.py` & `copper-bem-0.1.8/tests/test_curves.py`

 * *Files identical despite different names*

### Comparing `copper-bem-0.1.7/tests/test_generator.py` & `copper-bem-0.1.8/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `copper-bem-0.1.7/tests/test_library.py` & `copper-bem-0.1.8/tests/test_library.py`

 * *Files identical despite different names*

### Comparing `copper-bem-0.1.7/tests/test_logging.py` & `copper-bem-0.1.8/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `copper-bem-0.1.7/tests/test_units.py` & `copper-bem-0.1.8/tests/test_units.py`

 * *Files identical despite different names*

