# Comparing `tmp/tranquilo-0.0.2.tar.gz` & `tmp/tranquilo-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tranquilo-0.0.2.tar", last modified: Mon Apr 10 09:14:49 2023, max compression
+gzip compressed data, was "tranquilo-0.0.3.tar", last modified: Sat May 20 10:06:50 2023, max compression
```

## Comparing `tranquilo-0.0.2.tar` & `tranquilo-0.0.3.tar`

### file list

```diff
@@ -1,74 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:14:49.650888 tranquilo-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:14:49.638887 tranquilo-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:14:49.642887 tranquilo-0.0.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-10 09:14:35.000000 tranquilo-0.0.2/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-10 09:14:35.000000 tranquilo-0.0.2/.github/ISSUE_TEMPLATE/enhancement.md
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-10 09:14:35.000000 tranquilo-0.0.2/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:14:49.642887 tranquilo-0.0.2/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-10 09:14:35.000000 tranquilo-0.0.2/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:14:49.642887 tranquilo-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-10 09:14:35.000000 tranquilo-0.0.2/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-10 09:14:35.000000 tranquilo-0.0.2/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-10 09:14:35.000000 tranquilo-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-10 09:14:35.000000 tranquilo-0.0.2/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-04-10 09:14:35.000000 tranquilo-0.0.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-10 09:14:35.000000 tranquilo-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-10 09:14:35.000000 tranquilo-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-04-10 09:14:49.650888 tranquilo-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-10 09:14:35.000000 tranquilo-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-10 09:14:35.000000 tranquilo-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-10 09:14:49.650888 tranquilo-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-10 09:14:35.000000 tranquilo-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:14:49.638887 tranquilo-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:14:49.646888 tranquilo-0.0.2/src/tranquilo/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-10 09:14:49.000000 tranquilo-0.0.2/src/tranquilo/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/acceptance_decision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/acceptance_sample_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/adjust_radius.py
--rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/aggregate_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/bounds.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/estimate_variance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/exploration_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/filter_points.py
--rw-r--r--   0 runner    (1001) docker     (123)    15697 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/fit_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/get_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/handle_infinity.py
--rw-r--r--   0 runner    (1001) docker     (123)     7773 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     8496 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/poisedness.py
--rw-r--r--   0 runner    (1001) docker     (123)     9549 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/process_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/region.py
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/rho_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)    17087 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/sample_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/solve_subproblem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:14:49.646888 tranquilo-0.0.2/src/tranquilo/subsolvers/
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/subsolvers/_conjugate_gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/subsolvers/_conjugate_gradient_fast.py
--rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/subsolvers/_steihaug_toint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/subsolvers/_steihaug_toint_fast.py
--rw-r--r--   0 runner    (1001) docker     (123)    20191 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/subsolvers/_trsbox.py
--rw-r--r--   0 runner    (1001) docker     (123)    20818 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/subsolvers/_trsbox_fast.py
--rw-r--r--   0 runner    (1001) docker     (123)    30890 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/subsolvers/bntr.py
--rw-r--r--   0 runner    (1001) docker     (123)    39169 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/subsolvers/bntr_fast.py
--rw-r--r--   0 runner    (1001) docker     (123)    20403 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/subsolvers/gqtpar.py
--rw-r--r--   0 runner    (1001) docker     (123)    21641 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/subsolvers/gqtpar_fast.py
--rw-r--r--   0 runner    (1001) docker     (123)    11824 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/subsolvers/linear_subsolvers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/subsolvers/wrapped_subsolvers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14962 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/tranquilo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    19526 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/visualize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/volume.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/weighting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-04-10 09:14:35.000000 tranquilo-0.0.2/src/tranquilo/wrap_criterion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 09:14:49.646888 tranquilo-0.0.2/src/tranquilo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-04-10 09:14:49.000000 tranquilo-0.0.2/src/tranquilo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-04-10 09:14:49.000000 tranquilo-0.0.2/src/tranquilo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 09:14:49.000000 tranquilo-0.0.2/src/tranquilo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 09:14:49.000000 tranquilo-0.0.2/src/tranquilo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-10 09:14:49.000000 tranquilo-0.0.2/src/tranquilo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-10 09:14:49.000000 tranquilo-0.0.2/src/tranquilo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:06:50.515989 tranquilo-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:06:50.503990 tranquilo-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:06:50.503990 tranquilo-0.0.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-20 10:06:37.000000 tranquilo-0.0.3/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-20 10:06:37.000000 tranquilo-0.0.3/.github/ISSUE_TEMPLATE/enhancement.md
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-20 10:06:37.000000 tranquilo-0.0.3/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:06:50.507990 tranquilo-0.0.3/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-20 10:06:37.000000 tranquilo-0.0.3/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:06:50.507990 tranquilo-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-20 10:06:37.000000 tranquilo-0.0.3/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-20 10:06:37.000000 tranquilo-0.0.3/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-20 10:06:37.000000 tranquilo-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-20 10:06:37.000000 tranquilo-0.0.3/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-05-20 10:06:37.000000 tranquilo-0.0.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-20 10:06:37.000000 tranquilo-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-20 10:06:37.000000 tranquilo-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-05-20 10:06:50.515989 tranquilo-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-20 10:06:37.000000 tranquilo-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-20 10:06:37.000000 tranquilo-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-20 10:06:50.515989 tranquilo-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-20 10:06:37.000000 tranquilo-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:06:50.503990 tranquilo-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:06:50.511989 tranquilo-0.0.3/src/tranquilo/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-20 10:06:50.000000 tranquilo-0.0.3/src/tranquilo/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14272 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/acceptance_decision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/acceptance_sample_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/adjust_n_evals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/adjust_radius.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/aggregate_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/bounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/estimate_variance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/exploration_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/filter_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15697 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/fit_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/get_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/handle_infinity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7933 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8496 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/poisedness.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10502 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/process_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/rho_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17087 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/sample_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/solve_subproblem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:06:50.511989 tranquilo-0.0.3/src/tranquilo/subsolvers/
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/subsolvers/_conjugate_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/subsolvers/_conjugate_gradient_fast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/subsolvers/_steihaug_toint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/subsolvers/_steihaug_toint_fast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20191 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/subsolvers/_trsbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20818 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/subsolvers/_trsbox_fast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30890 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/subsolvers/bntr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39169 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/subsolvers/bntr_fast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20403 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/subsolvers/gqtpar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21641 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/subsolvers/gqtpar_fast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11824 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/subsolvers/linear_subsolvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/subsolvers/wrapped_subsolvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18522 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/tranquilo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19526 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/visualize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/weighting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-20 10:06:37.000000 tranquilo-0.0.3/src/tranquilo/wrap_criterion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:06:50.511989 tranquilo-0.0.3/src/tranquilo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-05-20 10:06:50.000000 tranquilo-0.0.3/src/tranquilo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-20 10:06:50.000000 tranquilo-0.0.3/src/tranquilo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 10:06:50.000000 tranquilo-0.0.3/src/tranquilo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 10:06:50.000000 tranquilo-0.0.3/src/tranquilo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-20 10:06:50.000000 tranquilo-0.0.3/src/tranquilo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-20 10:06:50.000000 tranquilo-0.0.3/src/tranquilo.egg-info/top_level.txt
```

### Comparing `tranquilo-0.0.2/.github/ISSUE_TEMPLATE/bug-report.md` & `tranquilo-0.0.3/.github/ISSUE_TEMPLATE/bug-report.md`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.2/.github/ISSUE_TEMPLATE/enhancement.md` & `tranquilo-0.0.3/.github/ISSUE_TEMPLATE/enhancement.md`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.2/.github/ISSUE_TEMPLATE/feature_request.md` & `tranquilo-0.0.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.2/.github/workflows/main.yml` & `tranquilo-0.0.3/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.2/.github/workflows/publish-to-pypi.yml` & `tranquilo-0.0.3/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.2/.gitignore` & `tranquilo-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.2/CODE_OF_CONDUCT.md` & `tranquilo-0.0.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.2/LICENSE` & `tranquilo-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.2/MANIFEST.in` & `tranquilo-0.0.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.2/PKG-INFO` & `tranquilo-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tranquilo
-Version: 0.0.2
+Version: 0.0.3
 Summary: Trust-region optimizer for scalar, least-square and noisy problems
 Home-page: https://github.com/OpenSourceEconomics/tranquilo
 Author: Janos Gabler
 Author-email: janos.gabler@gmail.com
 License: MIT
 Keywords: optimization,dfo,derivative free optimization,noisy optimization,parallel optimization,numerical optimization
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tranquilo-0.0.2/README.md` & `tranquilo-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.2/pyproject.toml` & `tranquilo-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.2/setup.cfg` & `tranquilo-0.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.2/src/tranquilo/acceptance_sample_size.py` & `tranquilo-0.0.3/src/tranquilo/acceptance_sample_size.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.2/src/tranquilo/adjust_radius.py` & `tranquilo-0.0.3/src/tranquilo/adjust_radius.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 import numpy as np
 
 
-def adjust_radius(radius, rho, step_length, options):
+def adjust_radius(radius, rho, step_length, options, n_evals_is_increased):
     """Adjust the trustregion radius based on relative improvement and stepsize.
 
     This is just a slight generalization of the pounders radius adjustment. With default
     options it yields the same result.
 
     Noise handling is not built-in here. It will be achieved by calling the
     function with a noise-adjusted rho.
 
     Args:
         radius (float): The current trust-region radius.
         rho (float): Actual over expected improvement between the last two accepted
             parameter vectors.
         step (np.ndarray): The step between the last two accepted parameter vectors.
         options (NamedTuple): Options for radius management.
+        n_evals_is_increased (bool): Whether the number of evaluations was increased.
 
     Returns:
         float: The updated radius.
 
     """
     is_large_step = step_length / radius >= options.large_step
 
     if rho >= options.rho_increase and is_large_step:
         new_radius = radius * options.expansion_factor
-    elif rho >= options.rho_decrease:
+    elif rho >= options.rho_decrease or n_evals_is_increased:
         new_radius = radius
     else:
         new_radius = radius * options.shrinking_factor
 
     if np.isfinite(options.max_radius_to_step_ratio):
         max_radius = np.min(
             [options.max_radius, step_length * options.max_radius_to_step_ratio]
```

### Comparing `tranquilo-0.0.2/src/tranquilo/aggregate_models.py` & `tranquilo-0.0.3/src/tranquilo/aggregate_models.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.2/src/tranquilo/bounds.py` & `tranquilo-0.0.3/src/tranquilo/bounds.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.2/src/tranquilo/clustering.py` & `tranquilo-0.0.3/src/tranquilo/clustering.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.2/src/tranquilo/config.py` & `tranquilo-0.0.3/src/tranquilo/config.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.2/src/tranquilo/estimate_variance.py` & `tranquilo-0.0.3/src/tranquilo/estimate_variance.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.2/src/tranquilo/exploration_sample.py` & `tranquilo-0.0.3/src/tranquilo/exploration_sample.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.2/src/tranquilo/filter_points.py` & `tranquilo-0.0.3/src/tranquilo/filter_points.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.2/src/tranquilo/fit_models.py` & `tranquilo-0.0.3/src/tranquilo/fit_models.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.2/src/tranquilo/geometry.py` & `tranquilo-0.0.3/src/tranquilo/geometry.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.2/src/tranquilo/get_component.py` & `tranquilo-0.0.3/src/tranquilo/get_component.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.2/src/tranquilo/handle_infinity.py` & `tranquilo-0.0.3/src/tranquilo/handle_infinity.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.2/src/tranquilo/history.py` & `tranquilo-0.0.3/src/tranquilo/history.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,14 +169,19 @@
             arr=self.fvals[: self.n_fun],
             mapper=self.index_mapper,
             x_indices=x_indices,
             n_xs=self.n_xs,
         )
         return out
 
+    def get_n_evals(self, x_indices):
+        fvals = self.get_fvals(x_indices)
+        n_evals = {k: len(v) for k, v in fvals.items()}
+        return n_evals
+
     def get_model_data(self, x_indices, average=True):
         if np.isscalar(x_indices):
             x_indices = [x_indices]
 
         raw_xs = self.get_xs(x_indices)
         raw_fvecs = self.get_fvecs(x_indices)
```

### Comparing `tranquilo-0.0.2/src/tranquilo/models.py` & `tranquilo-0.0.3/src/tranquilo/models.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.2/src/tranquilo/options.py` & `tranquilo-0.0.3/src/tranquilo/options.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,32 @@
 from typing import NamedTuple
 from tranquilo.models import n_free_params
 
 import numpy as np
 
 
+def get_default_stagnation_options(noisy, batch_size):
+    if noisy:
+        out = StagnationOptions(
+            min_relative_step_keep=0.0,
+            drop=False,
+        )
+    elif batch_size > 1:
+        out = StagnationOptions(
+            min_relative_step_keep=0.0,
+            drop=True,
+        )
+    else:
+        out = StagnationOptions(
+            min_relative_step_keep=0.125,
+            drop=True,
+        )
+    return out
+
+
 def get_default_radius_options(x):
     return RadiusOptions(initial_radius=0.1 * np.max(np.abs(x)))
 
 
 def get_default_batch_size(n_cores):
     return n_cores
 
@@ -71,14 +90,18 @@
     return aggregator
 
 
 def get_default_n_evals_at_start(noisy):
     return 5 if noisy else 1
 
 
+def get_default_n_evals_per_point(noisy, noise_adaptation_options):
+    return noise_adaptation_options.min_n_evals if noisy else 1
+
+
 class StopOptions(NamedTuple):
     """Criteria for stopping without successful convergence."""
 
     max_iter: int
     max_eval: int
     max_time: float
 
@@ -107,28 +130,28 @@
     shrinking_factor: float = 0.5
     expansion_factor: float = 2.0
     large_step: float = 0.5
     max_radius_to_step_ratio: float = np.inf
 
 
 class AcceptanceOptions(NamedTuple):
-    confidence_level: float = 0.8
-    power_level: float = 0.8
+    confidence_level: float = 0.95
+    power_level: float = 0.95
     n_initial: int = 5
-    n_min: int = 5
-    n_max: int = 100
+    n_min: int = 4
+    n_max: int = 50
     min_improvement: float = 0.0
 
 
 class StagnationOptions(NamedTuple):
-    min_relative_step_keep: float = 0.125
+    min_relative_step_keep: float
+    drop: bool
     min_relative_step: float = 0.05
     sample_increment: int = 1
     max_trials: int = 1
-    drop: bool = True
 
 
 class SubsolverOptions(NamedTuple):
     maxiter: int = 20
     maxiter_gradient_descent: int = 5
     conjugate_gradient_method: str = "cg"
     gtol_abs: float = 1e-8
@@ -164,14 +187,26 @@
     algorithm: str = "scipy_lbfgsb"
     algo_options: dict = None
     criterion: str = None
     n_points_randomsearch: int = 1
     return_info: bool = False
 
 
+class NoiseAdaptationOptions(NamedTuple):
+    rho_noise_n_draws: int = 100
+    high_rho: float = 0.6
+    low_rho: float = 0.1
+    ignore_corelation: bool = True
+    min_share_high_rho: float = 0.7
+    min_share_low_rho: float = 0.9
+    min_n_evals: int = 1
+    max_n_evals: int = 30
+    good_rho_threshold: float = 0.1
+
+
 def update_option_bundle(default_options, user_options=None):
     """Update default options with user options.
 
     The user option is converted to the type of the default option if possible.
 
     Args:
         default_options (NamedTuple): Options that behave like a `typing.NamedTuple`,
```

### Comparing `tranquilo-0.0.2/src/tranquilo/poisedness.py` & `tranquilo-0.0.3/src/tranquilo/poisedness.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.2/src/tranquilo/process_arguments.py` & `tranquilo-0.0.3/src/tranquilo/process_arguments.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,27 +9,29 @@
 from tranquilo.bounds import Bounds
 from tranquilo.estimate_variance import get_variance_estimator
 from tranquilo.filter_points import get_sample_filter
 from tranquilo.fit_models import get_fitter
 from tranquilo.history import History
 from tranquilo.options import (
     ConvOptions,
-    StagnationOptions,
     StopOptions,
     get_default_acceptance_decider,
     get_default_aggregator,
     get_default_batch_size,
     get_default_model_fitter,
     get_default_residualize,
     get_default_model_type,
     get_default_n_evals_at_start,
+    get_default_n_evals_per_point,
     get_default_radius_options,
     get_default_sample_size,
     get_default_search_radius_factor,
+    get_default_stagnation_options,
     update_option_bundle,
+    NoiseAdaptationOptions,
 )
 from tranquilo.region import Region
 from tranquilo.sample_points import get_sampler
 from tranquilo.solve_subproblem import get_subsolver
 from tranquilo.wrap_criterion import get_wrapped_criterion
 
 
@@ -60,20 +62,21 @@
     # single advanced options
     batch_evaluator="joblib",
     n_cores=1,
     batch_size=None,
     sample_size=None,
     model_type=None,
     search_radius_factor=None,
-    n_evals_per_point=1,
+    n_evals_per_point=None,
     n_evals_at_start=None,
     seed=925408,
     # bundled advanced options
     radius_options=None,
     stagnation_options=None,
+    noise_adaptation_options=None,
     # component names and related options
     sampler="optimal_hull",
     sampler_options=None,
     sample_filter="keep_all",
     sample_filter_options=None,
     model_fitter=None,
     model_fitter_options=None,
@@ -106,30 +109,42 @@
         max_time=float(stopping_max_time),
     )
 
     # process simple options with static defaults
     x = _process_x(x)
     noisy = _process_noisy(noisy)
     n_cores = _process_n_cores(n_cores)
-    stagnation_options = update_option_bundle(StagnationOptions(), stagnation_options)
-    n_evals_per_point = int(n_evals_per_point)
     sampling_rng = _process_seed(seed)
+    simulation_rng = _process_seed(seed + 1000)
+
     n_evals_at_start = _process_n_evals_at_start(
         n_evals_at_start,
         noisy,
     )
+    noise_adaptation_options = update_option_bundle(
+        NoiseAdaptationOptions(), noise_adaptation_options
+    )
+
+    n_evals_per_point = _process_n_evals_per_point(
+        n_evals=n_evals_per_point,
+        noisy=noisy,
+        noise_adaptation_options=noise_adaptation_options,
+    )
 
     # process options that depend on arguments with static defaults
     search_radius_factor = _process_search_radius_factor(search_radius_factor, functype)
     batch_size = _process_batch_size(batch_size, n_cores)
     radius_options = update_option_bundle(get_default_radius_options(x), radius_options)
     model_type = _process_model_type(model_type, functype)
     acceptance_decider = _process_acceptance_decider(acceptance_decider, noisy)
 
     # process options that depend on arguments with dependent defaults
+    stagnation_options = update_option_bundle(
+        get_default_stagnation_options(noisy, batch_size=batch_size), stagnation_options
+    )
     target_sample_size = _process_sample_size(
         sample_size=sample_size,
         model_type=model_type,
         x=x,
     )
     model_fitter = _process_model_fitter(
         model_fitter, model_type=model_type, sample_size=target_sample_size, x=x
@@ -194,19 +209,21 @@
         "noisy": noisy,
         "conv_options": conv_options,
         "stop_options": stop_options,
         "radius_options": radius_options,
         "batch_size": batch_size,
         "target_sample_size": target_sample_size,
         "stagnation_options": stagnation_options,
+        "noise_adaptation_options": noise_adaptation_options,
         "search_radius_factor": search_radius_factor,
         "n_evals_per_point": n_evals_per_point,
         "n_evals_at_start": n_evals_at_start,
         "trustregion": trustregion,
         "sampling_rng": sampling_rng,
+        "simulation_rng": simulation_rng,
         "history": history,
         "sample_points": sample_points,
         "solve_subproblem": solve_subproblem,
         "filter_points": filter_points,
         "fit_model": fit_model,
         "aggregate_model": aggregate_model,
         "estimate_variance": estimate_variance,
@@ -308,7 +325,23 @@
     else:
         out = int(n_evals)
 
     if out < 1:
         raise ValueError("n_initial_acceptance_evals must be non-negative.")
 
     return out
+
+
+def next_multiple(n, base):
+    return int(np.ceil(n / base) * base)
+
+
+def _process_n_evals_per_point(n_evals, noisy, noise_adaptation_options):
+    if n_evals is None:
+        out = get_default_n_evals_per_point(noisy, noise_adaptation_options)
+    else:
+        out = int(n_evals)
+
+    if out < 1:
+        raise ValueError("n_evals_per_point must be non-negative.")
+
+    return out
```

### Comparing `tranquilo-0.0.2/src/tranquilo/region.py` & `tranquilo-0.0.3/src/tranquilo/region.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.2/src/tranquilo/rho_noise.py` & `tranquilo-0.0.3/src/tranquilo/rho_noise.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 
 from tranquilo.acceptance_decision import calculate_rho
 
 
 def simulate_rho_noise(
     xs,
     vector_model,
+    old_vector_model,
     trustregion,
     noise_cov,
     model_fitter,
     model_aggregator,
     subsolver,
     rng,
-    n_draws=100,
-    ignore_corelation=True,
+    options,
 ):
     """Simulate a rho that would obtain on average if there is no approximation error.
 
     This can be used to adjust the sample size in the presence of noise.
 
     Throughout this function the prefix true refers to what is considered as ground
     truth for the purpose of the simulation. The prefix sim refers to the simulated
@@ -25,38 +25,43 @@
 
     Args:
         xs (np.ndarray): Sample of points on which surrogate models will be
             fitted during the simulation. This sample is not scaled to the trustregion.
         vector_model (VectorModel): A vector surrogate model that is taken as true model
             for the simulation. In many cases this model was fitted on xs but this is
             not a requirement.
+        old_vector_model (VectorModel): A vector surrogate model that is potentially
+            used to fit the new model (if residualize=True).
         trustregion (Region): The trustregion in which the optimization is performed.
         noise_cov(np.ndarray): Covariance matrix of the noise. The noise is assumed to
             be drawn from a multivariate normal distribution with mean zero and this
             covariance matrix.
         model_fitter (callable): A function that fits a model.
         model_aggregator (callable): A function that aggregates a vector model to a
             scalar model.
         subsolver (callable): A function that solves the subproblem.
         rng (np.random.Generator): Random number generator.
-        n_draws (int): Number of draws used to estimate the rho noise.
-        ignore_corelation (bool): If True, the noise is assumed to be uncorrelated and
-            only the diagonal entries of the covariance matrix are used.
+        options (NoiseAdaptationOptions): Options for the noise adaptation.
 
     """
+    n_draws = options.rho_noise_n_draws
+    ignore_corelation = options.ignore_corelation
+
     n_samples, n_params = xs.shape
     n_residuals = len(noise_cov)
 
     x_unit = trustregion.map_to_unit(xs)
 
     true_fvecs = vector_model.predict(x_unit)
 
     true_scalar_model = model_aggregator(vector_model=vector_model)
 
-    true_current_fval = true_scalar_model.predict(np.zeros(n_params))
+    true_current_fval = true_scalar_model.predict(
+        trustregion.map_to_unit(trustregion.center)
+    )
 
     if ignore_corelation:
         noise_cov = np.diag(np.diag(noise_cov))
 
     noise = rng.multivariate_normal(
         mean=np.zeros(n_residuals), cov=noise_cov, size=n_draws * n_samples
     ).reshape(n_draws, n_samples, n_residuals)
@@ -65,15 +70,15 @@
     for draw in noise:
         sim_fvecs = true_fvecs + draw
         sim_vector_model = model_fitter(
             xs,
             sim_fvecs,
             weights=None,
             region=trustregion,
-            old_model=None,
+            old_model=old_vector_model,
         )
         sim_scalar_model = model_aggregator(vector_model=sim_vector_model)
         sim_sub_sol = subsolver(sim_scalar_model, trustregion)
 
         sim_candidate_fval = true_scalar_model.predict(sim_sub_sol.x_unit)
         sim_actual_improvement = -(sim_candidate_fval - true_current_fval)
```

### Comparing `tranquilo-0.0.2/src/tranquilo/sample_points.py` & `tranquilo-0.0.3/src/tranquilo/sample_points.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.2/src/tranquilo/solve_subproblem.py` & `tranquilo-0.0.3/src/tranquilo/solve_subproblem.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.2/src/tranquilo/subsolvers/_conjugate_gradient.py` & `tranquilo-0.0.3/src/tranquilo/subsolvers/_conjugate_gradient.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.2/src/tranquilo/subsolvers/_conjugate_gradient_fast.py` & `tranquilo-0.0.3/src/tranquilo/subsolvers/_conjugate_gradient_fast.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.2/src/tranquilo/subsolvers/_steihaug_toint.py` & `tranquilo-0.0.3/src/tranquilo/subsolvers/_steihaug_toint.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.2/src/tranquilo/subsolvers/_steihaug_toint_fast.py` & `tranquilo-0.0.3/src/tranquilo/subsolvers/_steihaug_toint_fast.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.2/src/tranquilo/subsolvers/_trsbox.py` & `tranquilo-0.0.3/src/tranquilo/subsolvers/_trsbox.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.2/src/tranquilo/subsolvers/_trsbox_fast.py` & `tranquilo-0.0.3/src/tranquilo/subsolvers/_trsbox_fast.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.2/src/tranquilo/subsolvers/bntr.py` & `tranquilo-0.0.3/src/tranquilo/subsolvers/bntr.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.2/src/tranquilo/subsolvers/bntr_fast.py` & `tranquilo-0.0.3/src/tranquilo/subsolvers/bntr_fast.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.2/src/tranquilo/subsolvers/gqtpar.py` & `tranquilo-0.0.3/src/tranquilo/subsolvers/gqtpar.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.2/src/tranquilo/subsolvers/gqtpar_fast.py` & `tranquilo-0.0.3/src/tranquilo/subsolvers/gqtpar_fast.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.2/src/tranquilo/subsolvers/linear_subsolvers.py` & `tranquilo-0.0.3/src/tranquilo/subsolvers/linear_subsolvers.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.2/src/tranquilo/subsolvers/wrapped_subsolvers.py` & `tranquilo-0.0.3/src/tranquilo/subsolvers/wrapped_subsolvers.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.2/src/tranquilo/tranquilo.py` & `tranquilo-0.0.3/src/tranquilo/tranquilo.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,16 +9,18 @@
 from tranquilo.filter_points import (
     drop_worst_points,
 )
 from tranquilo.models import (
     ScalarModel,
     VectorModel,
 )
-from tranquilo.process_arguments import process_arguments
+from tranquilo.process_arguments import process_arguments, next_multiple
 from tranquilo.region import Region
+from tranquilo.rho_noise import simulate_rho_noise
+from tranquilo.adjust_n_evals import adjust_n_evals
 
 
 # wrapping gives us the signature and docstring of process arguments
 @functools.wraps(process_arguments)
 def _tranquilo(*args, **kwargs):
     internal_kwargs = process_arguments(*args, **kwargs)
     return _internal_tranquilo(**internal_kwargs)
@@ -27,32 +29,37 @@
 def _internal_tranquilo(
     evaluate_criterion,
     x,
     noisy,
     conv_options,
     stop_options,
     radius_options,
+    noise_adaptation_options,
     batch_size,
     target_sample_size,
     stagnation_options,
     search_radius_factor,
     n_evals_per_point,
     n_evals_at_start,
     trustregion,
     sampling_rng,
+    simulation_rng,
     history,
     sample_points,
     solve_subproblem,
     filter_points,
     fit_model,
     aggregate_model,
     estimate_variance,
     accept_candidate,
 ):
-    eval_info = {0: n_evals_at_start}
+    if n_evals_at_start > 1:
+        eval_info = {0: next_multiple(n_evals_at_start, base=batch_size)}
+    else:
+        eval_info = {0: 1}
 
     evaluate_criterion(eval_info)
 
     _init_fvec = history.get_fvecs(0).mean(axis=0)
 
     _init_vector_model = VectorModel(
         intercepts=_init_fvec,
@@ -101,29 +108,45 @@
         old_xs = history.get_xs(old_indices)
 
         model_xs, model_indices = filter_points(
             xs=old_xs,
             indices=old_indices,
             state=state,
             target_size=target_sample_size,
+            history=history,
+            n_evals_per_point=n_evals_per_point,
+        )
+        # ==============================================================================
+        # determine number of evaluations needed at existing xs
+        # ==============================================================================
+
+        additional_eval_info = _get_additional_eval_info(
+            model_indices=model_indices,
+            history=history,
+            n_evals_per_point=n_evals_per_point,
         )
 
         # ==========================================================================
         # sample points if necessary and do simple iteration
         # ==========================================================================
+
+        n_new_points = max(0, target_sample_size - len(model_xs))
+        n_new_points = next_multiple(n_new_points, base=batch_size)
+
         new_xs = sample_points(
             trustregion=state.trustregion,
-            n_points=max(0, target_sample_size - len(model_xs)),
+            n_points=n_new_points,
             existing_xs=model_xs,
             rng=sampling_rng,
         )
 
         new_indices = history.add_xs(new_xs)
 
         eval_info = {i: n_evals_per_point for i in new_indices}
+        eval_info.update(additional_eval_info)
 
         evaluate_criterion(eval_info)
 
         model_indices = _concatenate_indices(model_indices, new_indices)
 
         model_xs = history.get_xs(model_indices)
         model_data = history.get_model_data(
@@ -191,25 +214,27 @@
 
         # ==========================================================================
         # If step length is still too small, replace the worst point with a new one
         # ==========================================================================
 
         sample_counter = 0
         while _relative_step_length < stagnation_options.min_relative_step:
-            if stagnation_options.drop:
+            n_to_drop = stagnation_options.sample_increment
+
+            if stagnation_options.drop and len(model_xs) > n_to_drop:
                 model_xs, model_indices = drop_worst_points(
                     xs=model_xs,
                     indices=model_indices,
                     state=state,
-                    n_to_drop=stagnation_options.sample_increment,
+                    n_to_drop=n_to_drop,
                 )
 
             new_xs = sample_points(
                 trustregion=state.trustregion,
-                n_points=stagnation_options.sample_increment,
+                n_points=n_to_drop,
                 existing_xs=model_xs,
                 rng=sampling_rng,
             )
 
             new_indices = history.add_xs(new_xs)
 
             eval_info = {i: n_evals_per_point for i in new_indices}
@@ -243,64 +268,105 @@
             )
 
             sample_counter += 1
             if sample_counter >= stagnation_options.max_trials:
                 break
 
         # ==============================================================================
-        # fit noise model based on previous acceptance samples
+        # fit noise models
         # ==============================================================================
 
         if noisy:
-            scalar_noise_variance = estimate_variance(
+            noise_variance = estimate_variance(
                 trustregion=state.trustregion,
                 history=history,
                 model_type="scalar",
             )
+            noise_cov = estimate_variance(
+                trustregion=state.trustregion,
+                history=history,
+                model_type="vector",
+            )
         else:
-            scalar_noise_variance = None
+            noise_variance = None
+            noise_cov = None
 
         # ==============================================================================
         # acceptance decision
         # ==============================================================================
 
         acceptance_result = accept_candidate(
             subproblem_solution=sub_sol,
             state=state,
             wrapped_criterion=evaluate_criterion,
-            noise_variance=scalar_noise_variance,
+            noise_variance=noise_variance,
             history=history,
+            search_radius_factor=search_radius_factor,
+            batch_size=batch_size,
+            sample_points=sample_points,
+            rng=sampling_rng,
         )
 
         # ==============================================================================
         # update state with information on this iteration
         # ==============================================================================
 
         state = state._replace(
             model_indices=model_indices,
             model=scalar_model,
             new_indices=np.setdiff1d(model_indices, old_indices),
             old_indices_used=np.intersect1d(model_indices, old_indices),
             old_indices_discarded=np.setdiff1d(old_indices, model_indices),
             **acceptance_result._asdict(),
+            n_evals_per_point=n_evals_per_point,
         )
 
         states.append(state)
 
         # ==============================================================================
-        # update state for beginning of next iteration
+        # estimate rho noise and adjust n_evals_per_point
+        # ==============================================================================
+
+        if noisy:
+            rho_noise_vec = simulate_rho_noise(
+                xs=model_xs,
+                vector_model=vector_model,
+                old_vector_model=state.vector_model,
+                trustregion=state.trustregion,
+                noise_cov=noise_cov,
+                model_fitter=fit_model,
+                model_aggregator=aggregate_model,
+                subsolver=solve_subproblem,
+                rng=simulation_rng,
+                options=noise_adaptation_options,
+            )
+
+            n_evals_per_point, n_evals_is_increased = adjust_n_evals(
+                n_evals=n_evals_per_point,
+                rho=acceptance_result.rho,
+                rho_noise=rho_noise_vec,
+                options=noise_adaptation_options,
+            )
+        else:
+            n_evals_is_increased = False
+        # ==============================================================================
+        # update trust region radius
         # ==============================================================================
 
         new_radius = adjust_radius(
             radius=state.trustregion.radius,
             rho=acceptance_result.rho,
             step_length=acceptance_result.step_length,
             options=radius_options,
+            n_evals_is_increased=n_evals_is_increased,
         )
 
+        # ==============================================================================
+        # update state for beginning of next iteration
+        # ==============================================================================
         new_trustregion = state.trustregion._replace(
             center=acceptance_result.x, radius=new_radius
         )
 
         state = state._replace(trustregion=new_trustregion)
 
         # ==============================================================================
@@ -408,14 +474,18 @@
     # information on step length
     step_length: float = None
     """The euclidian distance between `State.x` and `State.trustregion.center`."""
 
     relative_step_length: float = None
     """The step_length divided by the radius of the trustregion."""
 
+    n_evals_per_point: int = None
+
+    n_evals_acceptance: int = None
+
 
 def _is_converged(states, options):
     old, new = states[-2:]
 
     f_change_abs = np.abs(old.fval - new.fval)
     f_change_rel = f_change_abs / max(np.abs(old.fval), 1)
     x_change_abs = np.linalg.norm(old.x - new.x)
@@ -462,7 +532,28 @@
 )
 
 
 def _concatenate_indices(first, second):
     first = np.atleast_1d(first).astype(int)
     second = np.atleast_1d(second).astype(int)
     return np.hstack((first, second))
+
+
+def _get_additional_eval_info(model_indices, history, n_evals_per_point):
+    """Determine the evaluations needed at existing xs.
+
+    We need additional evaluations at existing xs if `n_evals_per_point` has increased
+    since we last evaluated the criterion function at those xs.
+
+    Args:
+        model_indices (np.ndarray): The indices of the points used to build the model.
+        history (History): The history object.
+        n_evals_per_point (int): The number of evaluations per point.
+
+    Returns:
+        dict: Dict that maps x_indices to the number of additional evaluations needed.
+
+    """
+    existing_n_evals = history.get_n_evals(model_indices)
+    eval_info = {k: n_evals_per_point - v for k, v in existing_n_evals.items()}
+    eval_info = {k: v for k, v in eval_info.items() if v > 0}
+    return eval_info
```

### Comparing `tranquilo-0.0.2/src/tranquilo/utilities.py` & `tranquilo-0.0.3/src/tranquilo/utilities.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.2/src/tranquilo/visualize.py` & `tranquilo-0.0.3/src/tranquilo/visualize.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.2/src/tranquilo/volume.py` & `tranquilo-0.0.3/src/tranquilo/volume.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.2/src/tranquilo/weighting.py` & `tranquilo-0.0.3/src/tranquilo/weighting.py`

 * *Files identical despite different names*

### Comparing `tranquilo-0.0.2/src/tranquilo/wrap_criterion.py` & `tranquilo-0.0.3/src/tranquilo/wrap_criterion.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,20 +4,32 @@
 
 from estimagic.batch_evaluators import process_batch_evaluator
 
 
 def get_wrapped_criterion(criterion, batch_evaluator, n_cores, history):
     """Wrap the criterion function to do get parallelization and history handling.
 
+    Notes
+    -----
+
     The wrapped criterion function takes a dict mapping x_indices to required numbers of
     evaluations as only argument. It evaluates the criterion function in parallel and
     saves the resulting function evaluations in the history.
 
     The wrapped criterion function does not return anything.
 
+    Args:
+        criterion (function): The criterion function to wrap.
+        batch_evaluator (function): The batch evaluator to use.
+        n_cores (int): The number of cores to use.
+        history (History): The tranquilo history.
+
+    Returns:
+        callable: The wrapped criterion function.
+
     """
     batch_evaluator = process_batch_evaluator(batch_evaluator)
 
     @functools.wraps(criterion)
     def wrapper_criterion(eval_info):
         if not isinstance(eval_info, dict):
             raise ValueError("eval_info must be a dict.")
```

### Comparing `tranquilo-0.0.2/src/tranquilo.egg-info/PKG-INFO` & `tranquilo-0.0.3/src/tranquilo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tranquilo
-Version: 0.0.2
+Version: 0.0.3
 Summary: Trust-region optimizer for scalar, least-square and noisy problems
 Home-page: https://github.com/OpenSourceEconomics/tranquilo
 Author: Janos Gabler
 Author-email: janos.gabler@gmail.com
 License: MIT
 Keywords: optimization,dfo,derivative free optimization,noisy optimization,parallel optimization,numerical optimization
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tranquilo-0.0.2/src/tranquilo.egg-info/SOURCES.txt` & `tranquilo-0.0.3/src/tranquilo.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 .github/PULL_REQUEST_TEMPLATE/pull_request_template.md
 .github/workflows/main.yml
 .github/workflows/publish-to-pypi.yml
 src/tranquilo/__init__.py
 src/tranquilo/_version.py
 src/tranquilo/acceptance_decision.py
 src/tranquilo/acceptance_sample_size.py
+src/tranquilo/adjust_n_evals.py
 src/tranquilo/adjust_radius.py
 src/tranquilo/aggregate_models.py
 src/tranquilo/bounds.py
 src/tranquilo/clustering.py
 src/tranquilo/config.py
 src/tranquilo/estimate_variance.py
 src/tranquilo/exploration_sample.py
```

