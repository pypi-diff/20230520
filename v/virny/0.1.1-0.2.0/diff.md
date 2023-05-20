# Comparing `tmp/virny-0.1.1.tar.gz` & `tmp/virny-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "virny-0.1.1.tar", last modified: Sun Feb  5 23:52:42 2023, max compression
+gzip compressed data, was "virny-0.2.0.tar", last modified: Sat May 20 11:35:24 2023, max compression
```

## Comparing `virny-0.1.1.tar` & `virny-0.2.0.tar`

### file list

```diff
@@ -1,67 +1,77 @@
-drwxrwxr-x   0 denys_herasymuk  (1000) denys_herasymuk  (1000)        0 2023-02-05 23:52:42.809013 virny-0.1.1/
--rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     5489 2023-02-05 23:52:42.809013 virny-0.1.1/PKG-INFO
--rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     4042 2023-02-05 23:43:57.000000 virny-0.1.1/README.md
--rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)       38 2023-02-05 23:52:42.813012 virny-0.1.1/setup.cfg
--rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     2475 2023-02-05 23:43:57.000000 virny-0.1.1/setup.py
-drwxrwxr-x   0 denys_herasymuk  (1000) denys_herasymuk  (1000)        0 2023-02-05 23:52:42.805013 virny-0.1.1/tests/
-drwxrwxr-x   0 denys_herasymuk  (1000) denys_herasymuk  (1000)        0 2023-02-05 23:52:42.805013 virny-0.1.1/tests/custom_classes/
--rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)        0 2023-02-05 23:43:57.000000 virny-0.1.1/tests/custom_classes/__init__.py
--rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     2894 2023-02-05 23:43:57.000000 virny-0.1.1/tests/custom_classes/test_metrics_composer.py
-drwxrwxr-x   0 denys_herasymuk  (1000) denys_herasymuk  (1000)        0 2023-02-05 23:52:42.805013 virny-0.1.1/tests/metrics/
--rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)        0 2023-02-05 23:43:57.000000 virny-0.1.1/tests/metrics/__init__.py
--rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     2403 2023-02-05 23:43:57.000000 virny-0.1.1/tests/metrics/test_stability_metrics.py
-drwxrwxr-x   0 denys_herasymuk  (1000) denys_herasymuk  (1000)        0 2023-02-05 23:52:42.805013 virny-0.1.1/tests/preprocessing/
--rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)        0 2023-02-05 23:43:57.000000 virny-0.1.1/tests/preprocessing/__init__.py
--rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     2096 2023-02-05 23:43:57.000000 virny-0.1.1/tests/preprocessing/test_basic_preprocessing.py
-drwxrwxr-x   0 denys_herasymuk  (1000) denys_herasymuk  (1000)        0 2023-02-05 23:52:42.805013 virny-0.1.1/tests/utils/
--rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)        0 2023-02-05 23:43:57.000000 virny-0.1.1/tests/utils/__init__.py
--rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     7237 2023-02-05 23:43:57.000000 virny-0.1.1/tests/utils/test_common_helpers.py
--rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     1768 2023-02-05 23:43:57.000000 virny-0.1.1/tests/utils/test_custom_initializers.py
--rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     2660 2023-02-05 23:43:57.000000 virny-0.1.1/tests/utils/test_stability_utils.py
-drwxrwxr-x   0 denys_herasymuk  (1000) denys_herasymuk  (1000)        0 2023-02-05 23:52:42.805013 virny-0.1.1/virny/
--rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)       37 2023-02-05 23:43:57.000000 virny-0.1.1/virny/__init__.py
--rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)       63 2023-02-05 23:51:06.000000 virny-0.1.1/virny/__version__.py
-drwxrwxr-x   0 denys_herasymuk  (1000) denys_herasymuk  (1000)        0 2023-02-05 23:52:42.809013 virny-0.1.1/virny/analyzers/
--rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)      884 2023-02-05 23:43:57.000000 virny-0.1.1/virny/analyzers/__init__.py
--rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     9057 2023-02-05 23:43:57.000000 virny-0.1.1/virny/analyzers/abstract_overall_variance_analyzer.py
--rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     3087 2023-02-05 23:43:57.000000 virny-0.1.1/virny/analyzers/abstract_subgroup_analyzer.py
--rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     2116 2023-02-05 23:43:57.000000 virny-0.1.1/virny/analyzers/batch_overall_variance_analyzer.py
--rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     1249 2023-02-05 23:43:57.000000 virny-0.1.1/virny/analyzers/subgroup_statistical_bias_analyzer.py
--rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     3941 2023-02-05 23:43:57.000000 virny-0.1.1/virny/analyzers/subgroup_variance_analyzer.py
--rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     3741 2023-02-05 23:43:57.000000 virny-0.1.1/virny/analyzers/subgroup_variance_calculator.py
--rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)      292 2023-02-05 23:43:57.000000 virny-0.1.1/virny/api.py
-drwxrwxr-x   0 denys_herasymuk  (1000) denys_herasymuk  (1000)        0 2023-02-05 23:52:42.809013 virny-0.1.1/virny/configs/
--rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)       71 2023-02-05 23:43:57.000000 virny-0.1.1/virny/configs/__init__.py
--rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)      628 2023-02-05 23:43:57.000000 virny-0.1.1/virny/configs/constants.py
-drwxrwxr-x   0 denys_herasymuk  (1000) denys_herasymuk  (1000)        0 2023-02-05 23:52:42.809013 virny-0.1.1/virny/custom_classes/
--rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)      510 2023-02-05 23:43:57.000000 virny-0.1.1/virny/custom_classes/__init__.py
--rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     1483 2023-02-05 23:43:57.000000 virny-0.1.1/virny/custom_classes/base_dataset.py
--rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)      574 2023-02-05 23:43:57.000000 virny-0.1.1/virny/custom_classes/custom_logger.py
--rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     5538 2023-02-05 23:43:57.000000 virny-0.1.1/virny/custom_classes/generic_pipeline.py
--rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     3599 2023-02-05 23:43:57.000000 virny-0.1.1/virny/custom_classes/metrics_composer.py
--rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)    27276 2023-02-05 23:43:57.000000 virny-0.1.1/virny/custom_classes/metrics_visualizer.py
-drwxrwxr-x   0 denys_herasymuk  (1000) denys_herasymuk  (1000)        0 2023-02-05 23:52:42.809013 virny-0.1.1/virny/datasets/
--rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)      343 2023-02-05 23:43:57.000000 virny-0.1.1/virny/datasets/__init__.py
--rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)    14315 2023-02-05 23:43:57.000000 virny-0.1.1/virny/datasets/data_loaders.py
-drwxrwxr-x   0 denys_herasymuk  (1000) denys_herasymuk  (1000)        0 2023-02-05 23:52:42.809013 virny-0.1.1/virny/metrics/
--rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)      523 2023-02-05 23:43:57.000000 virny-0.1.1/virny/metrics/__init__.py
--rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     3806 2023-02-05 23:43:57.000000 virny-0.1.1/virny/metrics/stability_metrics.py
-drwxrwxr-x   0 denys_herasymuk  (1000) denys_herasymuk  (1000)        0 2023-02-05 23:52:42.809013 virny-0.1.1/virny/preprocessing/
--rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)      222 2023-02-05 23:43:57.000000 virny-0.1.1/virny/preprocessing/__init__.py
--rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     1773 2023-02-05 23:43:57.000000 virny-0.1.1/virny/preprocessing/basic_preprocessing.py
-drwxrwxr-x   0 denys_herasymuk  (1000) denys_herasymuk  (1000)        0 2023-02-05 23:52:42.809013 virny-0.1.1/virny/user_interfaces/
--rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)      505 2023-02-05 23:43:57.000000 virny-0.1.1/virny/user_interfaces/__init__.py
--rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)    14262 2023-02-05 23:43:57.000000 virny-0.1.1/virny/user_interfaces/metrics_computation_interfaces.py
-drwxrwxr-x   0 denys_herasymuk  (1000) denys_herasymuk  (1000)        0 2023-02-05 23:52:42.809013 virny-0.1.1/virny/utils/
--rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)      278 2023-02-05 23:43:57.000000 virny-0.1.1/virny/utils/__init__.py
--rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     7550 2023-02-05 23:43:57.000000 virny-0.1.1/virny/utils/common_helpers.py
--rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     2165 2023-02-05 23:43:57.000000 virny-0.1.1/virny/utils/custom_initializers.py
--rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     4268 2023-02-05 23:43:57.000000 virny-0.1.1/virny/utils/data_viz_utils.py
--rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     8489 2023-02-05 23:43:57.000000 virny-0.1.1/virny/utils/model_tuning_utils.py
--rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     3945 2023-02-05 23:43:57.000000 virny-0.1.1/virny/utils/stability_utils.py
-drwxrwxr-x   0 denys_herasymuk  (1000) denys_herasymuk  (1000)        0 2023-02-05 23:52:42.809013 virny-0.1.1/virny.egg-info/
--rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     5489 2023-02-05 23:52:42.000000 virny-0.1.1/virny.egg-info/PKG-INFO
--rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     1655 2023-02-05 23:52:42.000000 virny-0.1.1/virny.egg-info/SOURCES.txt
--rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)        1 2023-02-05 23:52:42.000000 virny-0.1.1/virny.egg-info/dependency_links.txt
--rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)      665 2023-02-05 23:52:42.000000 virny-0.1.1/virny.egg-info/requires.txt
--rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)       12 2023-02-05 23:52:42.000000 virny-0.1.1/virny.egg-info/top_level.txt
+drwxrwxr-x   0 denys_herasymuk  (1000) denys_herasymuk  (1000)        0 2023-05-20 11:35:24.032506 virny-0.2.0/
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)       85 2023-05-20 10:38:33.000000 virny-0.2.0/MANIFEST.in
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     5494 2023-05-20 11:35:24.032506 virny-0.2.0/PKG-INFO
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     4055 2023-05-20 11:34:35.000000 virny-0.2.0/README.md
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)       38 2023-05-20 11:35:24.036506 virny-0.2.0/setup.cfg
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     2482 2023-05-20 10:38:33.000000 virny-0.2.0/setup.py
+drwxrwxr-x   0 denys_herasymuk  (1000) denys_herasymuk  (1000)        0 2023-05-20 11:35:24.020506 virny-0.2.0/tests/
+drwxrwxr-x   0 denys_herasymuk  (1000) denys_herasymuk  (1000)        0 2023-05-20 11:35:24.024506 virny-0.2.0/tests/custom_classes/
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)        0 2023-02-05 23:43:57.000000 virny-0.2.0/tests/custom_classes/__init__.py
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     3108 2023-05-20 10:38:33.000000 virny-0.2.0/tests/custom_classes/test_metrics_composer.py
+drwxrwxr-x   0 denys_herasymuk  (1000) denys_herasymuk  (1000)        0 2023-05-20 11:35:24.024506 virny-0.2.0/tests/metrics/
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)        0 2023-02-05 23:43:57.000000 virny-0.2.0/tests/metrics/__init__.py
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     2403 2023-02-05 23:43:57.000000 virny-0.2.0/tests/metrics/test_stability_metrics.py
+drwxrwxr-x   0 denys_herasymuk  (1000) denys_herasymuk  (1000)        0 2023-05-20 11:35:24.024506 virny-0.2.0/tests/preprocessing/
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)        0 2023-02-05 23:43:57.000000 virny-0.2.0/tests/preprocessing/__init__.py
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     2096 2023-02-05 23:43:57.000000 virny-0.2.0/tests/preprocessing/test_basic_preprocessing.py
+drwxrwxr-x   0 denys_herasymuk  (1000) denys_herasymuk  (1000)        0 2023-05-20 11:35:24.024506 virny-0.2.0/tests/utils/
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)        0 2023-02-05 23:43:57.000000 virny-0.2.0/tests/utils/__init__.py
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     2369 2023-05-20 10:38:33.000000 virny-0.2.0/tests/utils/test_common_helpers.py
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     4941 2023-05-20 10:38:33.000000 virny-0.2.0/tests/utils/test_protected_groups_partitioning.py
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     3060 2023-05-20 10:38:33.000000 virny-0.2.0/tests/utils/test_stability_utils.py
+drwxrwxr-x   0 denys_herasymuk  (1000) denys_herasymuk  (1000)        0 2023-05-20 11:35:24.024506 virny-0.2.0/virny/
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)       37 2023-02-05 23:43:57.000000 virny-0.2.0/virny/__init__.py
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)       63 2023-05-20 11:09:39.000000 virny-0.2.0/virny/__version__.py
+drwxrwxr-x   0 denys_herasymuk  (1000) denys_herasymuk  (1000)        0 2023-05-20 11:35:24.024506 virny-0.2.0/virny/analyzers/
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)      842 2023-05-20 10:38:33.000000 virny-0.2.0/virny/analyzers/__init__.py
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     9874 2023-05-20 10:38:33.000000 virny-0.2.0/virny/analyzers/abstract_overall_variance_analyzer.py
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     3087 2023-02-05 23:43:57.000000 virny-0.2.0/virny/analyzers/abstract_subgroup_analyzer.py
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     2611 2023-05-20 10:38:33.000000 virny-0.2.0/virny/analyzers/batch_overall_variance_analyzer.py
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     4617 2023-05-20 10:38:33.000000 virny-0.2.0/virny/analyzers/incremental_overall_variance_analyzer.py
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     1230 2023-05-20 10:38:33.000000 virny-0.2.0/virny/analyzers/subgroup_error_analyzer.py
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     6929 2023-05-20 10:38:33.000000 virny-0.2.0/virny/analyzers/subgroup_variance_analyzer.py
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     3741 2023-02-05 23:43:57.000000 virny-0.2.0/virny/analyzers/subgroup_variance_calculator.py
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)      292 2023-02-05 23:43:57.000000 virny-0.2.0/virny/api.py
+drwxrwxr-x   0 denys_herasymuk  (1000) denys_herasymuk  (1000)        0 2023-05-20 11:35:24.024506 virny-0.2.0/virny/configs/
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)       71 2023-02-05 23:43:57.000000 virny-0.2.0/virny/configs/__init__.py
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)      628 2023-04-20 18:16:05.000000 virny-0.2.0/virny/configs/constants.py
+drwxrwxr-x   0 denys_herasymuk  (1000) denys_herasymuk  (1000)        0 2023-05-20 11:35:24.028506 virny-0.2.0/virny/custom_classes/
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)      449 2023-05-20 10:38:33.000000 virny-0.2.0/virny/custom_classes/__init__.py
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     1880 2023-05-20 10:38:33.000000 virny-0.2.0/virny/custom_classes/base_dataset.py
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)      633 2023-05-20 10:38:33.000000 virny-0.2.0/virny/custom_classes/custom_logger.py
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)      535 2023-05-20 10:38:33.000000 virny-0.2.0/virny/custom_classes/incremental_pandas_dataset.py
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     3700 2023-05-20 10:38:33.000000 virny-0.2.0/virny/custom_classes/metrics_composer.py
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)    27392 2023-05-20 10:38:33.000000 virny-0.2.0/virny/custom_classes/metrics_visualizer.py
+drwxrwxr-x   0 denys_herasymuk  (1000) denys_herasymuk  (1000)        0 2023-05-20 11:35:24.028506 virny-0.2.0/virny/datasets/
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)   391642 2023-02-05 23:43:57.000000 virny-0.2.0/virny/datasets/COMPAS.csv
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)      595 2023-05-20 10:38:33.000000 virny-0.2.0/virny/datasets/__init__.py
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     1399 2023-05-20 10:38:33.000000 virny-0.2.0/virny/datasets/base.py
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)    21540 2023-05-20 10:38:33.000000 virny-0.2.0/virny/datasets/data_loaders.py
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)  7564965 2023-05-20 10:38:33.000000 virny-0.2.0/virny/datasets/givemesomecredit.csv
+drwxrwxr-x   0 denys_herasymuk  (1000) denys_herasymuk  (1000)        0 2023-05-20 11:35:24.032506 virny-0.2.0/virny/incremental_ml/
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)       13 2023-05-20 10:38:33.000000 virny-0.2.0/virny/incremental_ml/__init__.py
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     1904 2023-05-20 10:38:33.000000 virny-0.2.0/virny/incremental_ml/river_utils.py
+drwxrwxr-x   0 denys_herasymuk  (1000) denys_herasymuk  (1000)        0 2023-05-20 11:35:24.032506 virny-0.2.0/virny/metrics/
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)      531 2023-05-20 10:38:33.000000 virny-0.2.0/virny/metrics/__init__.py
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     3806 2023-02-05 23:43:57.000000 virny-0.2.0/virny/metrics/stability_metrics.py
+drwxrwxr-x   0 denys_herasymuk  (1000) denys_herasymuk  (1000)        0 2023-05-20 11:35:24.032506 virny-0.2.0/virny/preprocessing/
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)      268 2023-05-20 10:38:33.000000 virny-0.2.0/virny/preprocessing/__init__.py
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     4053 2023-05-20 10:38:33.000000 virny-0.2.0/virny/preprocessing/basic_preprocessing.py
+drwxrwxr-x   0 denys_herasymuk  (1000) denys_herasymuk  (1000)        0 2023-05-20 11:35:24.032506 virny-0.2.0/virny/user_interfaces/
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)      726 2023-05-20 10:38:33.000000 virny-0.2.0/virny/user_interfaces/__init__.py
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)    36895 2023-05-20 10:38:33.000000 virny-0.2.0/virny/user_interfaces/metrics_computation_interfaces.py
+drwxrwxr-x   0 denys_herasymuk  (1000) denys_herasymuk  (1000)        0 2023-05-20 11:35:24.032506 virny-0.2.0/virny/utils/
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)      307 2023-05-20 10:38:33.000000 virny-0.2.0/virny/utils/__init__.py
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     4458 2023-05-20 10:38:33.000000 virny-0.2.0/virny/utils/common_helpers.py
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     3455 2023-05-20 10:38:33.000000 virny-0.2.0/virny/utils/custom_initializers.py
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     4268 2023-02-05 23:43:57.000000 virny-0.2.0/virny/utils/data_viz_utils.py
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     8347 2023-05-20 10:38:33.000000 virny-0.2.0/virny/utils/model_tuning_utils.py
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     3903 2023-05-20 10:38:33.000000 virny-0.2.0/virny/utils/protected_groups_partitioning.py
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     3945 2023-02-05 23:43:57.000000 virny-0.2.0/virny/utils/stability_utils.py
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     1982 2023-05-20 10:38:33.000000 virny-0.2.0/virny/utils/validation.py
+drwxrwxr-x   0 denys_herasymuk  (1000) denys_herasymuk  (1000)        0 2023-05-20 11:35:24.024506 virny-0.2.0/virny.egg-info/
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     5494 2023-05-20 11:35:23.000000 virny-0.2.0/virny.egg-info/PKG-INFO
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)     1958 2023-05-20 11:35:24.000000 virny-0.2.0/virny.egg-info/SOURCES.txt
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)        1 2023-05-20 11:35:23.000000 virny-0.2.0/virny.egg-info/dependency_links.txt
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)      601 2023-05-20 11:35:23.000000 virny-0.2.0/virny.egg-info/requires.txt
+-rw-rw-r--   0 denys_herasymuk  (1000) denys_herasymuk  (1000)       12 2023-05-20 11:35:23.000000 virny-0.2.0/virny.egg-info/top_level.txt
```

### Comparing `virny-0.1.1/PKG-INFO` & `virny-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: virny
-Version: 0.1.1
+Version: 0.2.0
 Summary: Python library for auditing model stability and fairness
 Home-page: https://github.com/DataResponsibly/Virny
 Author: Denys Herasymuk
 Author-email: denis.gerasymuk799@gmail.com
 License: BSD-3
 Description: # Virny Software Library
         
@@ -32,15 +32,15 @@
           <!-- Last Commit -->
           <a href="">
             <img src="https://img.shields.io/github/last-commit/DataResponsibly/Virny.svg" alt="last_commit">
           </a>
         </p>
         
         
-        ## Description 📜
+        ## 📜 Description
         
         **Virny** is a Python library for auditing model stability and fairness. The Virny library was
         developed based on three fundamental principles: 
         
         1) easy extensibility of model analysis capabilities;
         2) compatibility to user-defined/custom datasets and model types;
         3) simple composition of parity metrics based on context of use.
@@ -48,63 +48,62 @@
         Virny decouples model auditing into several stages, including: **subgroup metrics computation**, **group metrics composition**,
         and **metrics visualization and reporting**. This gives data scientists and practitioners more control and flexibility 
         to use the library for model development and monitoring post-deployment.
         
         For quickstart, look at our [Use Case Examples](https://dataresponsibly.github.io/Virny/examples/Multiple_Runs_Interface_Use_Case/).
         
         
-        ## Documentation 📒
+        ## 📒 Documentation
         
         * [Introduction](https://dataresponsibly.github.io/Virny/)
         * [API Reference](https://dataresponsibly.github.io/Virny/api/overview/)
         * [Use Case Examples](https://dataresponsibly.github.io/Virny/examples/Multiple_Runs_Interface_Use_Case/)
         
         
-        ## Features 💡
+        ## 💡 Features
         
         * Entire pipeline for auditing model stability and fairness
         * Metrics reports and visualizations
         * Ability to analyze intersections of sensitive attributes
         * Blind classifiers audit
         * Interface for multiple runs and multiple models
         * User-friendly parameters input via config yaml files
         * Built-in preprocessing techniques for raw classification datasets
         * Check out [our documentation](https://dataresponsibly.github.io/Virny/) for a comprehensive overview
         
         
-        ## Library Terminology 📖
+        ## 📖 Library Terminology
         
         This section briefly explains the main terminology used in our library.
         
         * A **sensitive attribute** is an attribute that partitions the population into groups with unequal benefits received.
         * A **protected group** (or simply _group_) is created by partitioning the population by one or many sensitive attributes.
         * A **privileged value** of a sensitive attribute is a value that gives more benefit to a protected group, which includes it, than to protected groups, which do not include it.
         * A **subgroup** is created by splitting a protected group by privileges and disprivileged values.
         * A **group metric** is a metric that shows the relation between privileged and disprivileged subgroups created based on one or many sensitive attributes.
         
         
-        ## Installation 🛠
+        ## 🛠 Installation
         
-        Virny supports **Python 3.8, 3.9** and can be installed with `pip`:
+        Virny supports **Python 3.8 (recommended), 3.9** and can be installed with `pip`:
         
         ```bash
         pip install virny
         ```
         
         
-        ## Affiliations 🤗
+        ## 🤗 Affiliations
         
         ![NYU-UCU-Logos](https://user-images.githubusercontent.com/42843889/216840888-071bf184-f0e3-4a3e-94dc-c0d1c7784143.png)
         
         
-        ## License 📝
+        ## 📝 License
         
         **Virny** is free and open-source software licensed under the [3-clause BSD license](https://github.com/DataResponsibly/Virny/blob/main/LICENSE).
         
-        
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,50 +1,50 @@
-Metadata-Version: 2.1 Name: virny Version: 0.1.1 Summary: Python library for
+Metadata-Version: 2.1 Name: virny Version: 0.2.0 Summary: Python library for
 auditing model stability and fairness Home-page: https://github.com/
 DataResponsibly/Virny Author: Denys Herasymuk Author-email:
 denis.gerasymuk799@gmail.com License: BSD-3 Description: # Virny Software
 Library
  [CI_Pipeline]  [documentation]  [pypi]  [bsd_3_license]  [code_size]
 [last_commit]
-## Description ð **Virny** is a Python library for auditing model stability
+## ð Description **Virny** is a Python library for auditing model stability
 and fairness. The Virny library was developed based on three fundamental
 principles: 1) easy extensibility of model analysis capabilities; 2)
 compatibility to user-defined/custom datasets and model types; 3) simple
 composition of parity metrics based on context of use. Virny decouples model
 auditing into several stages, including: **subgroup metrics computation**,
 **group metrics composition**, and **metrics visualization and reporting**.
 This gives data scientists and practitioners more control and flexibility to
 use the library for model development and monitoring post-deployment. For
 quickstart, look at our [Use Case Examples](https://dataresponsibly.github.io/
-Virny/examples/Multiple_Runs_Interface_Use_Case/). ## Documentation ð *
+Virny/examples/Multiple_Runs_Interface_Use_Case/). ## ð Documentation *
 [Introduction](https://dataresponsibly.github.io/Virny/) * [API Reference]
 (https://dataresponsibly.github.io/Virny/api/overview/) * [Use Case Examples]
 (https://dataresponsibly.github.io/Virny/examples/
-Multiple_Runs_Interface_Use_Case/) ## Features ð¡ * Entire pipeline for
+Multiple_Runs_Interface_Use_Case/) ## ð¡ Features * Entire pipeline for
 auditing model stability and fairness * Metrics reports and visualizations *
 Ability to analyze intersections of sensitive attributes * Blind classifiers
 audit * Interface for multiple runs and multiple models * User-friendly
 parameters input via config yaml files * Built-in preprocessing techniques for
 raw classification datasets * Check out [our documentation](https://
-dataresponsibly.github.io/Virny/) for a comprehensive overview ## Library
-Terminology ð This section briefly explains the main terminology used in our
+dataresponsibly.github.io/Virny/) for a comprehensive overview ## ð Library
+Terminology This section briefly explains the main terminology used in our
 library. * A **sensitive attribute** is an attribute that partitions the
 population into groups with unequal benefits received. * A **protected group**
 (or simply _group_) is created by partitioning the population by one or many
 sensitive attributes. * A **privileged value** of a sensitive attribute is a
 value that gives more benefit to a protected group, which includes it, than to
 protected groups, which do not include it. * A **subgroup** is created by
 splitting a protected group by privileges and disprivileged values. * A **group
 metric** is a metric that shows the relation between privileged and
 disprivileged subgroups created based on one or many sensitive attributes. ##
-Installation ð  Virny supports **Python 3.8, 3.9** and can be installed with
-`pip`: ```bash pip install virny ``` ## Affiliations ð¤ ![NYU-UCU-Logos]
-(https://user-images.githubusercontent.com/42843889/216840888-071bf184-f0e3-
-4a3e-94dc-c0d1c7784143.png) ## License ð **Virny** is free and open-source
-software licensed under the [3-clause BSD license](https://github.com/
-DataResponsibly/Virny/blob/main/LICENSE). Platform: UNKNOWN Classifier:
-Intended Audience :: Developers Classifier: License :: OSI Approved :: BSD
-License Classifier: Programming Language :: Python Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Operating System
-:: OS Independent Description-Content-Type: text/markdown Provides-Extra: dev
-Provides-Extra: docs
+ð  Installation Virny supports **Python 3.8 (recommended), 3.9** and can be
+installed with `pip`: ```bash pip install virny ``` ## ð¤ Affiliations ![NYU-
+UCU-Logos](https://user-images.githubusercontent.com/42843889/216840888-
+071bf184-f0e3-4a3e-94dc-c0d1c7784143.png) ## ð License **Virny** is free and
+open-source software licensed under the [3-clause BSD license](https://
+github.com/DataResponsibly/Virny/blob/main/LICENSE). Platform: UNKNOWN
+Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
+:: BSD License Classifier: Programming Language :: Python Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Operating
+System :: OS Independent Description-Content-Type: text/markdown Provides-
+Extra: dev Provides-Extra: docs
```

### Comparing `virny-0.1.1/README.md` & `virny-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
   <!-- Last Commit -->
   <a href="">
     <img src="https://img.shields.io/github/last-commit/DataResponsibly/Virny.svg" alt="last_commit">
   </a>
 </p>
 
 
-## Description 📜
+## 📜 Description
 
 **Virny** is a Python library for auditing model stability and fairness. The Virny library was
 developed based on three fundamental principles: 
 
 1) easy extensibility of model analysis capabilities;
 2) compatibility to user-defined/custom datasets and model types;
 3) simple composition of parity metrics based on context of use.
@@ -40,55 +40,54 @@
 Virny decouples model auditing into several stages, including: **subgroup metrics computation**, **group metrics composition**,
 and **metrics visualization and reporting**. This gives data scientists and practitioners more control and flexibility 
 to use the library for model development and monitoring post-deployment.
 
 For quickstart, look at our [Use Case Examples](https://dataresponsibly.github.io/Virny/examples/Multiple_Runs_Interface_Use_Case/).
 
 
-## Documentation 📒
+## 📒 Documentation
 
 * [Introduction](https://dataresponsibly.github.io/Virny/)
 * [API Reference](https://dataresponsibly.github.io/Virny/api/overview/)
 * [Use Case Examples](https://dataresponsibly.github.io/Virny/examples/Multiple_Runs_Interface_Use_Case/)
 
 
-## Features 💡
+## 💡 Features
 
 * Entire pipeline for auditing model stability and fairness
 * Metrics reports and visualizations
 * Ability to analyze intersections of sensitive attributes
 * Blind classifiers audit
 * Interface for multiple runs and multiple models
 * User-friendly parameters input via config yaml files
 * Built-in preprocessing techniques for raw classification datasets
 * Check out [our documentation](https://dataresponsibly.github.io/Virny/) for a comprehensive overview
 
 
-## Library Terminology 📖
+## 📖 Library Terminology
 
 This section briefly explains the main terminology used in our library.
 
 * A **sensitive attribute** is an attribute that partitions the population into groups with unequal benefits received.
 * A **protected group** (or simply _group_) is created by partitioning the population by one or many sensitive attributes.
 * A **privileged value** of a sensitive attribute is a value that gives more benefit to a protected group, which includes it, than to protected groups, which do not include it.
 * A **subgroup** is created by splitting a protected group by privileges and disprivileged values.
 * A **group metric** is a metric that shows the relation between privileged and disprivileged subgroups created based on one or many sensitive attributes.
 
 
-## Installation 🛠
+## 🛠 Installation
 
-Virny supports **Python 3.8, 3.9** and can be installed with `pip`:
+Virny supports **Python 3.8 (recommended), 3.9** and can be installed with `pip`:
 
 ```bash
 pip install virny
 ```
 
 
-## Affiliations 🤗
+## 🤗 Affiliations
 
 ![NYU-UCU-Logos](https://user-images.githubusercontent.com/42843889/216840888-071bf184-f0e3-4a3e-94dc-c0d1c7784143.png)
 
 
-## License 📝
+## 📝 License
 
 **Virny** is free and open-source software licensed under the [3-clause BSD license](https://github.com/DataResponsibly/Virny/blob/main/LICENSE).
-
```

#### html2text {}

```diff
@@ -1,40 +1,40 @@
 # Virny Software Library
  [CI_Pipeline]  [documentation]  [pypi]  [bsd_3_license]  [code_size]
 [last_commit]
-## Description ð **Virny** is a Python library for auditing model stability
+## ð Description **Virny** is a Python library for auditing model stability
 and fairness. The Virny library was developed based on three fundamental
 principles: 1) easy extensibility of model analysis capabilities; 2)
 compatibility to user-defined/custom datasets and model types; 3) simple
 composition of parity metrics based on context of use. Virny decouples model
 auditing into several stages, including: **subgroup metrics computation**,
 **group metrics composition**, and **metrics visualization and reporting**.
 This gives data scientists and practitioners more control and flexibility to
 use the library for model development and monitoring post-deployment. For
 quickstart, look at our [Use Case Examples](https://dataresponsibly.github.io/
-Virny/examples/Multiple_Runs_Interface_Use_Case/). ## Documentation ð *
+Virny/examples/Multiple_Runs_Interface_Use_Case/). ## ð Documentation *
 [Introduction](https://dataresponsibly.github.io/Virny/) * [API Reference]
 (https://dataresponsibly.github.io/Virny/api/overview/) * [Use Case Examples]
 (https://dataresponsibly.github.io/Virny/examples/
-Multiple_Runs_Interface_Use_Case/) ## Features ð¡ * Entire pipeline for
+Multiple_Runs_Interface_Use_Case/) ## ð¡ Features * Entire pipeline for
 auditing model stability and fairness * Metrics reports and visualizations *
 Ability to analyze intersections of sensitive attributes * Blind classifiers
 audit * Interface for multiple runs and multiple models * User-friendly
 parameters input via config yaml files * Built-in preprocessing techniques for
 raw classification datasets * Check out [our documentation](https://
-dataresponsibly.github.io/Virny/) for a comprehensive overview ## Library
-Terminology ð This section briefly explains the main terminology used in our
+dataresponsibly.github.io/Virny/) for a comprehensive overview ## ð Library
+Terminology This section briefly explains the main terminology used in our
 library. * A **sensitive attribute** is an attribute that partitions the
 population into groups with unequal benefits received. * A **protected group**
 (or simply _group_) is created by partitioning the population by one or many
 sensitive attributes. * A **privileged value** of a sensitive attribute is a
 value that gives more benefit to a protected group, which includes it, than to
 protected groups, which do not include it. * A **subgroup** is created by
 splitting a protected group by privileges and disprivileged values. * A **group
 metric** is a metric that shows the relation between privileged and
 disprivileged subgroups created based on one or many sensitive attributes. ##
-Installation ð  Virny supports **Python 3.8, 3.9** and can be installed with
-`pip`: ```bash pip install virny ``` ## Affiliations ð¤ ![NYU-UCU-Logos]
-(https://user-images.githubusercontent.com/42843889/216840888-071bf184-f0e3-
-4a3e-94dc-c0d1c7784143.png) ## License ð **Virny** is free and open-source
-software licensed under the [3-clause BSD license](https://github.com/
-DataResponsibly/Virny/blob/main/LICENSE).
+ð  Installation Virny supports **Python 3.8 (recommended), 3.9** and can be
+installed with `pip`: ```bash pip install virny ``` ## ð¤ Affiliations ![NYU-
+UCU-Logos](https://user-images.githubusercontent.com/42843889/216840888-
+071bf184-f0e3-4a3e-94dc-c0d1c7784143.png) ## ð License **Virny** is free and
+open-source software licensed under the [3-clause BSD license](https://
+github.com/DataResponsibly/Virny/blob/main/LICENSE).
```

### Comparing `virny-0.1.1/setup.py` & `virny-0.2.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -24,19 +24,19 @@
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 about: dict = {}
 with open(os.path.join(HERE, NAME, "__version__.py")) as f:
     exec(f.read(), about)
 
-with pathlib.Path('requirements.txt').open() as requirements_txt:
+with pathlib.Path('lib_base_packages.txt').open() as lib_base_packages_txt:
     base_packages = [
         str(requirement)
         for requirement
-        in pkg_resources.parse_requirements(requirements_txt)
+        in pkg_resources.parse_requirements(lib_base_packages_txt)
     ]
 
 # This call to setup() does all the work
 setup(
     name=NAME,
     version=about["__version__"],
     description=DESCRIPTION,
@@ -60,26 +60,26 @@
     install_requires=base_packages,
     extras_require={
         "dev": base_packages
                 + [
                     "pytest~=7.2.1",
                 ],
         "docs": [
-                    "numpy>=1.23",
+                    "scikit-learn",
+                    "numpy",
                     "scipy",
-                    "pandas>=1.5",
+                    "pandas",
                     "dominate",
                     "flask",
                     "ipykernel",
                     "jupyter-client",
                     "mike",
                     "mkdocs",
                     "mkdocs-awesome-pages-plugin",
                     "mkdocs-material",
                     "mkdocs-redirects",
                     "nbconvert",
                     "python-slugify",
                     "spacy",
-                    "watermark",
                 ],
     },
 )
```

### Comparing `virny-0.1.1/tests/custom_classes/test_metrics_composer.py` & `virny-0.2.0/tests/custom_classes/test_metrics_composer.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,38 +16,40 @@
 
 # ========================== Test compose_metrics ==========================
 def test_compose_metrics_true1(models_metrics_dct, config_params):
     metrics_composer = MetricsComposer(models_metrics_dct, config_params.sensitive_attributes_dct)
     models_composed_metrics_df = metrics_composer.compose_metrics()
 
     # Check shape
-    assert models_composed_metrics_df.shape == (20, 5)
+    assert models_composed_metrics_df.shape == (22, 5)
 
     # Check column names
     assert sorted(models_composed_metrics_df.columns.tolist()) == sorted(['Metric', 'Model_Name', 'sex', 'race', 'sex&race'])
 
     # Check unique Model_Name
     assert sorted(models_composed_metrics_df['Model_Name'].unique().tolist()) == sorted(['DecisionTreeClassifier', 'LogisticRegression'])
 
     # Check all metrics presence
-    assert sorted(models_composed_metrics_df['Metric'].unique().tolist()) == sorted(['Equalized_Odds_TPR', 'Equalized_Odds_FPR', 'Disparate_Impact',
-                                                                                     'Statistical_Parity_Difference', 'Accuracy_Parity', 'Label_Stability_Ratio',
-                                                                                     'IQR_Parity', 'Std_Parity', 'Std_Ratio', 'Jitter_Parity'])
+    assert sorted(models_composed_metrics_df['Metric'].unique().tolist()) == sorted(['Equalized_Odds_TPR', 'Equalized_Odds_FPR', 'Equalized_Odds_FNR',
+                                                                                     'Disparate_Impact', 'Statistical_Parity_Difference', 'Accuracy_Parity',
+                                                                                     'Label_Stability_Ratio', 'IQR_Parity', 'Std_Parity',
+                                                                                     'Std_Ratio', 'Jitter_Parity'])
 
 
 def test_compose_metrics_true2(models_metrics_dct, config_params):
     metrics_composer = MetricsComposer(models_metrics_dct, {'sex': 0, 'race': 'Caucasian'})
     models_composed_metrics_df = metrics_composer.compose_metrics()
 
     # Check shape
-    assert models_composed_metrics_df.shape == (20, 4)
+    assert models_composed_metrics_df.shape == (22, 4)
 
     # Check column names
     assert sorted(models_composed_metrics_df.columns.tolist()) == sorted(['Metric', 'Model_Name', 'sex', 'race'])
 
     # Check unique Model_Name
     assert sorted(models_composed_metrics_df['Model_Name'].unique().tolist()) == sorted(['DecisionTreeClassifier', 'LogisticRegression'])
 
     # Check all metrics presence
-    assert sorted(models_composed_metrics_df['Metric'].unique().tolist()) == sorted(['Equalized_Odds_TPR', 'Equalized_Odds_FPR', 'Disparate_Impact',
-                                                                                     'Statistical_Parity_Difference', 'Accuracy_Parity', 'Label_Stability_Ratio',
-                                                                                     'IQR_Parity', 'Std_Parity', 'Std_Ratio', 'Jitter_Parity'])
+    assert sorted(models_composed_metrics_df['Metric'].unique().tolist()) == sorted(['Equalized_Odds_TPR', 'Equalized_Odds_FPR', 'Equalized_Odds_FNR',
+                                                                                     'Disparate_Impact', 'Statistical_Parity_Difference', 'Accuracy_Parity',
+                                                                                     'Label_Stability_Ratio', 'IQR_Parity', 'Std_Parity', 'Std_Ratio',
+                                                                                     'Jitter_Parity'])
```

### Comparing `virny-0.1.1/tests/metrics/test_stability_metrics.py` & `virny-0.2.0/tests/metrics/test_stability_metrics.py`

 * *Files identical despite different names*

### Comparing `virny-0.1.1/tests/preprocessing/test_basic_preprocessing.py` & `virny-0.2.0/tests/preprocessing/test_basic_preprocessing.py`

 * *Files identical despite different names*

### Comparing `virny-0.1.1/virny/analyzers/__init__.py` & `virny-0.2.0/virny/analyzers/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """
-Subgroup Statistical Bias and Variance Analyzers.
+Subgroup Error and Variance Analyzers.
 
 This module contains fairness and stability analysing methods for defined subgroups.
 The purpose of an analyzer is to analyse defined metrics for defined subgroups.
 """
 from .abstract_overall_variance_analyzer import AbstractOverallVarianceAnalyzer
 from .abstract_subgroup_analyzer import AbstractSubgroupAnalyzer
 from .batch_overall_variance_analyzer import BatchOverallVarianceAnalyzer
-from .subgroup_statistical_bias_analyzer import SubgroupStatisticalBiasAnalyzer
+from .subgroup_error_analyzer import SubgroupErrorAnalyzer
 from .subgroup_variance_analyzer import SubgroupVarianceAnalyzer
 from .subgroup_variance_calculator import SubgroupVarianceCalculator
 
 __all__ = [
     "AbstractOverallVarianceAnalyzer",
     "AbstractSubgroupAnalyzer",
     "BatchOverallVarianceAnalyzer",
-    "SubgroupStatisticalBiasAnalyzer",
+    "SubgroupErrorAnalyzer",
     "SubgroupVarianceAnalyzer",
     "SubgroupVarianceCalculator",
 ]
```

### Comparing `virny-0.1.1/virny/analyzers/abstract_overall_variance_analyzer.py` & `virny-0.2.0/virny/analyzers/abstract_overall_variance_analyzer.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,28 +32,33 @@
         Processed features test set
     y_test
         Targets test set
     dataset_name
         Name of dataset, used for correct results naming
     n_estimators
         Number of estimators in ensemble to measure base_model stability
+    verbose
+        [Optional] Level of logs printing. The greater level provides more logs.
+         As for now, 0, 1, 2 levels are supported.
 
     """
+
     def __init__(self, base_model, base_model_name: str, bootstrap_fraction: float,
                  X_train: pd.DataFrame, y_train: pd.DataFrame, X_test: pd.DataFrame, y_test: pd.DataFrame,
-                 dataset_name: str, n_estimators: int):
+                 dataset_name: str, n_estimators: int, verbose: int = 0):
         self.base_model = base_model
         self.base_model_name = base_model_name
         self.bootstrap_fraction = bootstrap_fraction
         self.dataset_name = dataset_name
         self.n_estimators = n_estimators
         self.models_lst = [deepcopy(base_model) for _ in range(n_estimators)]
         self.models_predictions = None
 
-        self.__logger = get_logger()
+        self._verbose = verbose
+        self.__logger = get_logger(verbose)
 
         self.X_train = X_train
         self.y_train = y_train
         self.X_test = X_test
         self.y_test = y_test
 
         # Metrics
@@ -73,29 +78,31 @@
     def _batch_predict(self, classifier, X_test):
         pass
 
     @abstractmethod
     def _batch_predict_proba(self, classifier, X_test):
         pass
 
-    def compute_metrics(self, make_plots: bool = False, save_results: bool = True):
+    def compute_metrics(self, make_plots: bool = False, save_results: bool = True, with_fit: bool = True):
         """
         Measure metrics for the base model. Display plots for analysis if needed. Save results to a .pkl file
 
         Parameters
         ----------
         make_plots
             bool, if to display plots for analysis
         save_results
             If to save result metrics in a file
+        with_fit
+            If to fit estimators in bootstrap
 
         """
         # Quantify uncertainty for the base model
         boostrap_size = int(self.bootstrap_fraction * self.X_train.shape[0])
-        self.models_predictions = self.UQ_by_boostrap(boostrap_size, with_replacement=True)
+        self.models_predictions = self.UQ_by_boostrap(boostrap_size, with_replacement=True, with_fit=with_fit)
 
         # Count metrics based on prediction proba results
         y_preds, uq_labels, prediction_stats = count_prediction_stats(self.y_test.values, self.models_predictions)
         self.__logger.info(f'Successfully computed predict proba metrics')
 
         self.__update_metrics(prediction_stats.means_lst,
                               prediction_stats.stds_lst,
@@ -111,54 +118,68 @@
 
             # Count metrics based on label predictions to visualize plots
             labels_means_lst, labels_stds_lst, labels_iqr_lst = compute_std_mean_iqr_metrics(uq_labels)
             self.__logger.info(f'Successfully computed predict labels metrics')
             per_sample_accuracy_lst = prediction_stats.per_sample_accuracy_lst
             label_stability_lst = prediction_stats.label_stability_lst
 
-            plot_generic(labels_means_lst, labels_stds_lst, "Mean of probability", "Standard deviation", x_lim=1.01, y_lim=0.5, plot_title="Probability mean vs Standard deviation")
-            plot_generic(labels_stds_lst, label_stability_lst, "Standard deviation", "Label stability", x_lim=0.5, y_lim=1.01, plot_title="Standard deviation vs Label stability")
-            plot_generic(labels_means_lst, label_stability_lst, "Mean", "Label stability", x_lim=1.01, y_lim=1.01, plot_title="Mean vs Label stability")
-            plot_generic(per_sample_accuracy_lst, labels_stds_lst, "Accuracy", "Standard deviation", x_lim=1.01, y_lim=0.5, plot_title="Accuracy vs Standard deviation")
-            plot_generic(per_sample_accuracy_lst, labels_iqr_lst, "Accuracy", "Inter quantile range", x_lim=1.01, y_lim=1.01, plot_title="Accuracy vs Inter quantile range")
+            plot_generic(labels_means_lst, labels_stds_lst, "Mean of probability", "Standard deviation", x_lim=1.01,
+                         y_lim=0.5, plot_title="Probability mean vs Standard deviation")
+            plot_generic(labels_stds_lst, label_stability_lst, "Standard deviation", "Label stability", x_lim=0.5,
+                         y_lim=1.01, plot_title="Standard deviation vs Label stability")
+            plot_generic(labels_means_lst, label_stability_lst, "Mean", "Label stability", x_lim=1.01, y_lim=1.01,
+                         plot_title="Mean vs Label stability")
+            plot_generic(per_sample_accuracy_lst, labels_stds_lst, "Accuracy", "Standard deviation", x_lim=1.01,
+                         y_lim=0.5, plot_title="Accuracy vs Standard deviation")
+            plot_generic(per_sample_accuracy_lst, labels_iqr_lst, "Accuracy", "Inter quantile range", x_lim=1.01,
+                         y_lim=1.01, plot_title="Accuracy vs Inter quantile range")
 
         if save_results:
             self.save_metrics_to_file()
         else:
             return y_preds, self.y_test
 
-    def UQ_by_boostrap(self, boostrap_size: int, with_replacement: bool) -> dict:
+    def UQ_by_boostrap(self, boostrap_size: int, with_replacement: bool, with_fit: bool = True) -> dict:
         """
         Quantifying uncertainty of the base model by constructing an ensemble from bootstrapped samples.
 
         Return a dictionary where keys are models indexes, and values are lists of
          correspondent model predictions for X_test set.
 
         Parameters
         ----------
         boostrap_size
             Number of records in bootstrap splits
         with_replacement
             Enable replacement or not
+        with_fit
+            Whether to fit estimators in bootstrap
 
         """
         models_predictions = {idx: [] for idx in range(self.n_estimators)}
-        print('\n', flush=True)
+        if self._verbose >= 1:
+            print('\n', flush=True)
         self.__logger.info('Start classifiers testing by bootstrap')
+        # Remove a progress bar for UQ without estimators fitting
+        cycle_range = range(self.n_estimators) if with_fit is False else \
+            tqdm(range(self.n_estimators),
+                 desc="Classifiers testing by bootstrap",
+                 colour="blue",
+                 mininterval=10)
         # Train and test each estimator in models_predictions
-        for idx in tqdm(range(self.n_estimators),
-                        desc="Classifiers testing by bootstrap",
-                        colour="blue",
-                        mininterval=10):
+        for idx in cycle_range:
             classifier = self.models_lst[idx]
-            X_sample, y_sample = generate_bootstrap(self.X_train, self.y_train, boostrap_size, with_replacement)
-            classifier = self._fit_model(classifier, X_sample, y_sample)
+            if with_fit:
+                X_sample, y_sample = generate_bootstrap(self.X_train, self.y_train, boostrap_size, with_replacement)
+                classifier = self._fit_model(classifier, X_sample, y_sample)
             models_predictions[idx] = self._batch_predict_proba(classifier, self.X_test)
+            self.models_lst[idx] = classifier
 
-        print('\n', flush=True)
+        if self._verbose >= 1:
+            print('\n', flush=True)
         self.__logger.info('Successfully tested classifiers by bootstrap')
 
         return models_predictions
 
     def __update_metrics(self, means_lst, stds_lst, iqr_lst, entropy_lst, jitter_lst,
                          per_sample_accuracy, label_stability):
         self.mean = np.mean(means_lst)
@@ -201,14 +222,15 @@
         metrics_to_report['Mean'] = [self.mean]
         metrics_to_report['Std'] = [self.std]
         metrics_to_report['IQR'] = [self.iqr]
         metrics_to_report['Entropy'] = [self.entropy]
         metrics_to_report['Jitter'] = [self.jitter]
         metrics_to_report['Per_Sample_Accuracy'] = [self.per_sample_accuracy]
         metrics_to_report['Label_Stability'] = [self.label_stability]
+
         metrics_df = pd.DataFrame(metrics_to_report)
 
         dir_path = os.path.join('..', '..', 'results', 'models_stability_metrics')
         os.makedirs(dir_path, exist_ok=True)
 
         filename = f"{self.dataset_name}_{self.n_estimators}_estimators_{self.base_model_name}_base_model_stability_metrics.csv"
         metrics_df.to_csv(f'{dir_path}/{filename}', index=False)
```

### Comparing `virny-0.1.1/virny/analyzers/abstract_subgroup_analyzer.py` & `virny-0.2.0/virny/analyzers/abstract_subgroup_analyzer.py`

 * *Files identical despite different names*

### Comparing `virny-0.1.1/virny/analyzers/batch_overall_variance_analyzer.py` & `virny-0.2.0/virny/analyzers/batch_overall_variance_analyzer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import numpy as np
 import pandas as pd
 
 from virny.analyzers.abstract_overall_variance_analyzer import AbstractOverallVarianceAnalyzer
 
 
 class BatchOverallVarianceAnalyzer(AbstractOverallVarianceAnalyzer):
     """
@@ -25,26 +26,37 @@
         Targets test set
     target_column
         Name of the target column
     dataset_name
         Name of dataset, used for correct results naming
     n_estimators
         Number of estimators in ensemble to measure base_model stability
+    verbose
+        [Optional] Level of logs printing. The greater level provides more logs.
+         As for now, 0, 1, 2 levels are supported.
 
     """
     def __init__(self, base_model, base_model_name: str, bootstrap_fraction: float,
                  X_train: pd.DataFrame, y_train: pd.DataFrame, X_test: pd.DataFrame, y_test: pd.DataFrame,
-                 target_column: str, dataset_name: str, n_estimators: int):
-        super().__init__(base_model, base_model_name, bootstrap_fraction,
-                         X_train, y_train, X_test, y_test, dataset_name, n_estimators)
+                 target_column: str, dataset_name: str, n_estimators: int, verbose: int = 0):
+        super().__init__(base_model=base_model,
+                         base_model_name=base_model_name,
+                         bootstrap_fraction=bootstrap_fraction,
+                         X_train=X_train,
+                         y_train=y_train,
+                         X_test=X_test,
+                         y_test=y_test,
+                         dataset_name=dataset_name,
+                         n_estimators=n_estimators,
+                         verbose=verbose)
         self.target_column = target_column
 
-    def _fit_model(self, classifier, X_train: pd.DataFrame, y_train: pd.DataFrame):
+    def _fit_model(self, classifier, X_train: np.ndarray, y_train: np.ndarray):
         """
-        Fit a classifier that is an instance of self.base_model.
+        Fit a classifier that is an instance of self.base_model
         """
         return classifier.fit(X_train, y_train)
 
     def _batch_predict(self, classifier, X_test: pd.DataFrame):
         """
         Predict with the classifier for X_test set and return predictions
         """
```

### Comparing `virny-0.1.1/virny/analyzers/subgroup_statistical_bias_analyzer.py` & `virny-0.2.0/virny/analyzers/subgroup_error_analyzer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import pandas as pd
 
 from virny.analyzers.abstract_subgroup_analyzer import AbstractSubgroupAnalyzer
 from virny.utils.common_helpers import confusion_matrix_metrics
 
 
-class SubgroupStatisticalBiasAnalyzer(AbstractSubgroupAnalyzer):
+class SubgroupErrorAnalyzer(AbstractSubgroupAnalyzer):
     """
-    Analyzer to compute statistical bias metrics for subgroups.
+    Analyzer to compute error metrics for subgroups.
 
     Parameters
     ----------
     X_test
         Processed features test set
     y_test
         Targets test set
@@ -19,15 +19,15 @@
          and values are privilege values for these subgroups
     test_protected_groups
         A dictionary where keys are sensitive attributes, and values input dataset rows
          that are correspondent to these sensitive attributes
 
     """
     def __init__(self, X_test: pd.DataFrame, y_test: pd.DataFrame,
-                 sensitive_attributes_dct: dict, test_protected_groups: dict=None):
+                 sensitive_attributes_dct: dict, test_protected_groups: dict = None):
         super().__init__(X_test, y_test, sensitive_attributes_dct, test_protected_groups)
 
     def _compute_metrics(self, y_test: pd.DataFrame, y_preds: list):
         """
         Compute metrics for subgroups using a confusion matrix
         """
         return confusion_matrix_metrics(y_test, y_preds)
```

### Comparing `virny-0.1.1/virny/analyzers/subgroup_variance_calculator.py` & `virny-0.2.0/virny/analyzers/subgroup_variance_calculator.py`

 * *Files identical despite different names*

### Comparing `virny-0.1.1/virny/configs/constants.py` & `virny-0.2.0/virny/configs/constants.py`

 * *Files identical despite different names*

### Comparing `virny-0.1.1/virny/custom_classes/custom_logger.py` & `virny-0.2.0/virny/custom_classes/custom_logger.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,17 +6,17 @@
         logging.StreamHandler.__init__(self)
         fmt = '%(asctime)s %(filename)-18s %(levelname)-8s: %(message)s'
         fmt_date = '%Y-%m-%d %H:%M:%S'
         formatter = logging.Formatter(fmt, fmt_date)
         self.setFormatter(formatter)
 
 
-def get_logger():
+def get_logger(verbose: int = 0):
     logger = logging.getLogger('root')
-    logger.setLevel('INFO')
+    logger.setLevel(logging.INFO if verbose >= 1 else logging.WARNING)
     logging.disable(logging.DEBUG)
 
     if logger.hasHandlers():
         logger.handlers.clear()
     logger.addHandler(CustomHandler())
 
     return logger
```

### Comparing `virny-0.1.1/virny/custom_classes/metrics_composer.py` & `virny-0.2.0/virny/custom_classes/metrics_composer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import pandas as pd
 
 
 class MetricsComposer:
     """
-    Composer class that combines different metrics to create new ones such as 'Disparate_Impact' or 'Accuracy_Parity'
+    Composer class that combines different subgroup metrics to create group metrics
+     such as 'Disparate_Impact' or 'Accuracy_Parity'
 
     Parameters
     ----------
     models_metrics_dct
         Dictionary where keys are model names and values are dataframes of subgroups metrics for each model
     sensitive_attributes_dct
         A dictionary where keys are sensitive attribute names (including attributes intersections),
@@ -41,17 +42,18 @@
             cfm = cfm.set_index('Metric')
 
             for sensitive_attr in self.sensitive_attributes_dct.keys():
                 dis_group = sensitive_attr + '_dis'
                 priv_group = sensitive_attr + '_priv'
 
                 groups_metrics_dct[sensitive_attr] = {
-                    # Group statistical bias metrics
+                    # Group fairness metrics
                     'Equalized_Odds_TPR': cfm[dis_group]['TPR'] - cfm[priv_group]['TPR'],
                     'Equalized_Odds_FPR': cfm[dis_group]['FPR'] - cfm[priv_group]['FPR'],
+                    'Equalized_Odds_FNR': cfm[dis_group]['FNR'] - cfm[priv_group]['FNR'],
                     'Disparate_Impact': cfm[dis_group]['Positive-Rate'] / cfm[priv_group]['Positive-Rate'],
                     'Statistical_Parity_Difference': cfm[dis_group]['Positive-Rate'] - cfm[priv_group]['Positive-Rate'],
                     'Accuracy_Parity': cfm[dis_group]['Accuracy'] - cfm[priv_group]['Accuracy'],
                     # Group variance metrics
                     'Label_Stability_Ratio': cfm[dis_group]['Label_Stability'] / cfm[priv_group]['Label_Stability'],
                     'IQR_Parity': cfm[dis_group]['IQR'] - cfm[priv_group]['IQR'],
                     'Std_Parity': cfm[dis_group]['Std'] - cfm[priv_group]['Std'],
```

### Comparing `virny-0.1.1/virny/custom_classes/metrics_visualizer.py` & `virny-0.2.0/virny/custom_classes/metrics_visualizer.py`

 * *Files 17% similar despite different names*

```diff
@@ -33,15 +33,15 @@
                  dataset_name: str, model_names: list, sensitive_attributes_dct: dict):
         sns.set_theme(style="whitegrid")
 
         self.dataset_name = dataset_name
         self.model_names = model_names
         self.sensitive_attributes_dct = sensitive_attributes_dct
         self.__create_report = False
-        self.bias_metrics_lst = [
+        self.fairness_metrics_lst = [
             'Accuracy_Parity',
             'Equalized_Odds_TPR',
             'Equalized_Odds_FPR',
             'Disparate_Impact',
             'Statistical_Parity_Difference',
         ]
         self.variance_metrics_lst = [
@@ -84,16 +84,16 @@
                                                                                       var_name="Subgroup",
                                                                                       value_name="Value")
         self.sorted_models_composed_metrics_df = self.melted_models_composed_metrics_df.sort_values(by=['Value'])
 
     def create_overall_metrics_bar_char(self, metrics_names: list, reversed_metrics_names: list = None,
                                         metrics_title: str = "Overall Metrics"):
         """
-        This bar chart includes all defined models and all overall subgroup bias and variance metrics,
-        which are averaged across multiple runs. Using it, you can compare all models for each subgroup bias or variance metric.
+        This bar chart includes all defined models and all overall subgroup error and stability metrics,
+        which are averaged across multiple runs. Using it, you can compare all models for each subgroup error or stability metric.
         This comparison also includes reversed metrics, in which values closer to zero are better
         since straight and reversed metrics in this plot are converted to the same format -- values closer to one are better.
 
         Parameters
         ----------
         metrics_names
             List of subgroup metric names to visualize that have a scale from 0 to 1 where closer to 1 is better
@@ -145,15 +145,15 @@
             labelFontSize=14, titleFontSize=18
         )
 
         return models_metrics_chart
 
     def create_boxes_and_whiskers_for_models_multiple_runs(self, metrics_lst: list):
         """
-        This boxes and whiskers plot is based on overall subgroup bias and variance metrics for all defined models
+        This boxes and whiskers plot is based on overall subgroup error and stability metrics for all defined models
         and results after all runs. Using it, you can see combined information on one plot that includes different models,
          subgroup metrics, and results after multiple runs.
 
         Parameters
         ----------
         metrics_lst
             List of subgroup metric names to visualize
@@ -223,35 +223,35 @@
                 y=alt.Y("Model_Name:N", axis=alt.Axis(title="Model Name", titleFontSize=15)),
                 color=alt.Color("Model_Name:N", scale=alt.Scale(scheme="tableau20")),
             )
         )
 
         return models_metrics_chart, select_metric_legend, color_legend
 
-    def create_bias_variance_interactive_bar_chart(self):
+    def create_fairness_variance_interactive_bar_chart(self):
         """
-        This interactive bar chart includes all groups, all composed group bias and variance metrics,
-         and all defined models. Using it, you can select any pair of group bias and variance metrics and
+        This interactive bar chart includes all groups, all composed group fairness and stability metrics,
+         and all defined models. Using it, you can select any pair of group fairness and stability metrics and
           compare them across all groups and models. Since this plot is interactive, it saves a lot of space for other plots.
-           Also, it could be more convenient to compare individual group bias and variance metrics using the interactive mode.
+           Also, it could be more convenient to compare each group fairness and stability metric using the interactive mode.
         """
-        models_bias_metrics_chart, select_bias_metric_legend, bias_color_legend = \
-            self.create_models_metrics_bar_chart(self.bias_metrics_lst, metrics_group_name="Bias")
+        models_fairness_metrics_chart, select_fairness_metric_legend, fairness_color_legend = \
+            self.create_models_metrics_bar_chart(self.fairness_metrics_lst, metrics_group_name="Fairness")
 
         models_variance_metrics_chart, select_variance_metric_legend, variance_color_legend = \
             self.create_models_metrics_bar_chart(self.variance_metrics_lst, metrics_group_name="Variance")
 
         return (
                 alt.hconcat(
                     alt.vconcat(
-                        select_bias_metric_legend.properties(height=200, width=50),
+                        select_fairness_metric_legend.properties(height=200, width=50),
                         select_variance_metric_legend.properties(height=200, width=50),
-                        bias_color_legend.properties(height=200, width=50),
+                        fairness_color_legend.properties(height=200, width=50),
                     ),
-                    models_bias_metrics_chart.properties(height=200, width=300, title="Bias Metric Plot"),
+                    models_fairness_metrics_chart.properties(height=200, width=300, title="Fairness Metric Plot"),
                     models_variance_metrics_chart.properties(height=200, width=300, title="Variance Metric Plot"),
                 )
         )
 
     @staticmethod
     def _create_sorted_matrix_by_rank(model_metrics_matrix) -> np.array:
         models_distances_matrix = model_metrics_matrix.copy(deep=True).T
@@ -263,15 +263,15 @@
 
         models_distances_matrix = models_distances_matrix.T
         sorted_matrix_by_rank = np.argsort(np.argsort(models_distances_matrix, axis=1), axis=1)
         return sorted_matrix_by_rank
 
     def create_model_rank_heatmap(self, model_metrics_matrix, sorted_matrix_by_rank, num_models: int):
         """
-        This heatmap includes all group bias and variance metrics and all defined models.
+        This heatmap includes all group fairness and stability metrics and all defined models.
         Using it, you can visually compare all models across all group metrics. On this plot,
         colors display ranks where 1 is the best model for the metric. These ranks are conditioned
         on difference or ratio operations used to create these group metrics:
 
         1) if the metric is created based on the difference operation, closer values to zero have ranks that are closer to the first rank
 
         2) if the metric is created based on the ratio operation, closer values to one have ranks that are closer to the first rank
@@ -304,40 +304,40 @@
         cbar.set_ticklabels(tick_labels)
         cbar.set_label('Model Ranks')
 
         if self.__create_report:
             plt.close()
             return ax
 
-        ax.set_title('Model Ranks Based On Group Statistical Bias and Variance Metrics', fontsize=20)
+        ax.set_title('Model Ranks Based On Group Fairness and Stability Metrics', fontsize=20)
 
     def create_total_model_rank_heatmap(self, sorted_matrix_by_rank, num_models):
         """
-        This heatmap includes all defined models and sums of their bias and variance ranks.
+        This heatmap includes all defined models and sums of their fairness and stability ranks.
         On this plot, colors display sums of ranks for one model. If the sum is smaller,
-        the model has better bias or variance characteristics than other models.
-        Using this plot, you can visually compare all models for bias and variance characteristics.
+        the model has better fairness or stability characteristics than other models.
+        Using this plot, you can visually compare all models for fairness and stability characteristics.
 
         Parameters
         ----------
         sorted_matrix_by_rank
             Matrix of model ranks per metric where indexes are group metric names and columns are model names
         num_models
             Number of models to visualize
 
         """
         total_model_ranks = dict()
-        matrix_bias_metrics = [metric_name for metric_name in sorted_matrix_by_rank[self.model_names[0]].index
-                               if metric_name[:metric_name.rfind('_')] in self.bias_metrics_lst]
+        matrix_fairness_metrics = [metric_name for metric_name in sorted_matrix_by_rank[self.model_names[0]].index
+                               if metric_name[:metric_name.rfind('_')] in self.fairness_metrics_lst]
         matrix_variance_metrics = [metric_name for metric_name in sorted_matrix_by_rank[self.model_names[0]].index
                                    if metric_name[:metric_name.rfind('_')] in self.variance_metrics_lst]
 
         for model_name in self.model_names:
             model_ranks = dict()
-            model_ranks['Bias_Ranks_Sum'] = np.sum(sorted_matrix_by_rank[model_name][matrix_bias_metrics] + 1)
+            model_ranks['Fairness_Ranks_Sum'] = np.sum(sorted_matrix_by_rank[model_name][matrix_fairness_metrics] + 1)
             model_ranks['Variance_Ranks_Sum'] = np.sum(sorted_matrix_by_rank[model_name][matrix_variance_metrics] + 1)
             total_model_ranks[model_name] = model_ranks
 
         total_model_ranks_df = pd.DataFrame(total_model_ranks).T
 
         matrix_width = 6
         matrix_height = num_models // 2
@@ -346,15 +346,15 @@
         ax.set(xlabel="", ylabel="")
         ax.xaxis.tick_top()
 
         if self.__create_report:
             plt.close()
             return ax
 
-        ax.set_title('Total Ranks Sum For Group Statistical Bias and Variance Metrics', fontsize=15)
+        ax.set_title('Total Ranks Sum For Group Fairness and Stability Metrics', fontsize=15)
 
     def create_model_rank_heatmaps(self, metrics_lst: list, groups_lst):
         """
         Create model rank and total model rank heatmaps.
 
         Parameters
         ----------
@@ -389,146 +389,146 @@
         model_rank_heatmap = self.create_model_rank_heatmap(model_metrics_matrix, sorted_matrix_by_rank, num_models)
         total_model_rank_heatmap = self.create_total_model_rank_heatmap(sorted_matrix_by_rank, num_models)
         if self.__create_report:
             return model_rank_heatmap, total_model_rank_heatmap
 
     def create_html_report(self, report_type: ReportType, report_save_path: str):
         """
-        Create Statistical Bias and Variance Report depending on report type.
+        Create Fairness and Stability Report depending on report type.
         It includes visualizations and helpful details to them.
         """
         # Create a directory if it does not exist
         if not os.path.exists(report_save_path):
             os.makedirs(report_save_path, exist_ok=True)
 
         self.__create_report = True
 
         # Create plots
-        bias_overall_metrics_bar_chart = self.create_overall_metrics_bar_char(
+        fairness_overall_metrics_bar_chart = self.create_overall_metrics_bar_char(
             metrics_names=['TPR', 'PPV', 'Accuracy', 'F1', 'Selection-Rate', 'Positive-Rate'],
-            metrics_title="Bias Metrics"
+            metrics_title="Fairness Metrics"
         )
         variance_overall_metrics_bar_chart = self.create_overall_metrics_bar_char(
             metrics_names=['Label_Stability'],
             reversed_metrics_names=['Std', 'IQR', 'Jitter'],
-            metrics_title="Variance Metrics"
+            metrics_title="Stability Metrics"
         )
-        interactive_bar_chart = self.create_bias_variance_interactive_bar_chart()
+        interactive_bar_chart = self.create_fairness_variance_interactive_bar_chart()
         model_rank_heatmap, total_model_rank_heatmap = \
-            self.create_model_rank_heatmaps(metrics_lst=self.bias_metrics_lst + self.variance_metrics_lst,
+            self.create_model_rank_heatmaps(metrics_lst=self.fairness_metrics_lst + self.variance_metrics_lst,
                                             groups_lst=self.sensitive_attributes_dct.keys())
 
         # Set descriptions for the report
         general_desc = dp.Text(
             f"**Date of creation**: {datetime.now().strftime('%m/%d/%Y, %H:%M:%S')}\n\n\n"
             "This report was created based on the following input arguments:\n"
             f"* __Dataset name__: {self.dataset_name}\n"
             f"* __Model names__: {self.model_names}\n"
             f"* __Sensitive attributes__: {list(self.sensitive_attributes_dct.keys())}\n"
         )
         composed_metrics_desc = dp.Text(
             "Below you can find a dataframe of composed group metrics for all defined models and sensitive attributes.\n"
         )
         boxes_and_whiskers_plot_desc = dp.Text(
-            "The below boxes and whiskers plot is based on _overall_ subgroup bias and variance metrics for all defined models and results after all runs.\n"
+            "The below boxes and whiskers plot is based on _overall_ subgroup error and stability metrics for all defined models and results after all runs.\n"
             "This plot can give you the following benefits:\n"
             "* You can see combined information on one plot that includes different models, subgroup metrics, and results after multiple runs\n"
             "* You can see all quartiles for each model metric based on multiple runs\n"
             "* You can compare different models for each metric\n"
-            "* You can see the variance of each model metric\n"
+            "* You can see the stability of each model metric\n"
         )
         overall_metrics_desc = dp.Text(
-            "The below bar chart includes all defined models and all _overall_ subgroup bias and variance metrics, which are averaged across multiple runs.\n"
+            "The below bar chart includes all defined models and all _overall_ subgroup error and stability metrics, which are averaged across multiple runs.\n"
             "This plot can give you the following benefits:\n"
-            "* You can compare all models for each subgroup bias or variance metric\n"
+            "* You can compare all models for each subgroup error or stability metric\n"
             "* This comparison also includes reversed metrics, in which values closer to zero are better "
             "since straight and reversed metrics in this plot are converted to the same format -- values closer to one are better\n"
         )
         individual_metrics_interactive_bar_chart_desc = dp.Text(
-            "The below interactive bar chart includes all groups, all composed group bias and variance metrics, "
+            "The below interactive bar chart includes all groups, all composed group fairness and stability metrics, "
             "and all defined models.\n"
             "This plot can give you the following benefits:\n"
-            "* You can select any pair of group bias and variance metrics and compare them across all groups and models\n"
+            "* You can select any pair of group fairness and stability metrics and compare them across all groups and models\n"
             "* Since this plot is interactive, it saves a lot of space for other plots. "
-            "Also, it could be more convenient to compare individual group bias and variance metrics using the interactive mode\n"
+            "Also, it could be more convenient to compare each group fairness and stability metric using the interactive mode\n"
         )
         model_ranked_heatmap_desc = dp.Text(
-            "The below heatmap includes all group bias and variance metrics and all defined models.\n"
+            "The below heatmap includes all group fairness and stability metrics and all defined models.\n"
             "On this plot, colors display ranks where 1 is the best model for the metric. "
             "These ranks are conditioned on difference or ratio operations used to create these group metrics:\n"
             "* If the metric is created based on the difference operation, **closer values to zero** have ranks that are closer to the first rank\n"
             "* If the metric is created based on the ratio operation, **closer values to one** have ranks that are closer to the first rank\n\n"
             "This plot can give you the following benefits:\n"
             "* You can visually compare all models across all group metrics\n"
             "* You can visually understand where one model is better or worse than other models\n"
             "* You can find the best and worst models for each group metric\n"
         )
         overall_model_ranked_heatmap_desc = dp.Text(
-            "The below heatmap includes all defined models and sums of their bias and variance ranks.\n"
-            "On this plot, colors display sums of ranks for one model. If the sum is smaller, the model has better bias or variance characteristics than other models.\n"
+            "The below heatmap includes all defined models and sums of their fairness and stability ranks.\n"
+            "On this plot, colors display sums of ranks for one model. If the sum is smaller, the model has better fairness or stability characteristics than other models.\n"
             "This plot can give you the following benefits:\n"
-            "* You can visually compare all models for bias and variance characteristics\n"
+            "* You can visually compare all models for fairness and stability characteristics\n"
             "* You can visually understand where one model is better or worse than other models\n"
-            "* You can find the best or most balanced model based on bias or variance metrics\n"
+            "* You can find the best or most balanced model based on fairness or stability metrics\n"
         )
 
         report_filename = f'{self.dataset_name}_Metrics_Report_{datetime.now(timezone.utc).strftime("%Y%m%d__%H%M%S")}.html'
         if report_type == ReportType.MULTIPLE_RUNS_MULTIPLE_MODELS:
             boxes_and_whiskers_plot = self.create_boxes_and_whiskers_for_models_multiple_runs(
                 metrics_lst=['Std', 'IQR', 'Jitter', 'Label_Stability', 'Accuracy', 'TPR', 'TNR', 'FPR', 'FNR']
             )
 
-            dp.Report("# Statistical Bias and Variance Report",
+            dp.Report("# Fairness and Stability Report",
                       general_desc,
 
                       "## Model Composed Metrics",
                       composed_metrics_desc,
                       dp.DataTable(self.models_composed_metrics_df),
 
                       "## Boxes and Whiskers Plot Based On Multiple Models Runs",
                       boxes_and_whiskers_plot_desc,
                       dp.Plot(boxes_and_whiskers_plot),
 
-                      "## Overall Bias and Variance Model Metrics Comparison",
+                      "## Overall Fairness and Stability Model Metrics Comparison",
                       overall_metrics_desc,
-                      dp.Plot(bias_overall_metrics_bar_chart, responsive=False),
+                      dp.Plot(fairness_overall_metrics_bar_chart, responsive=False),
                       dp.Plot(variance_overall_metrics_bar_chart, responsive=False),
 
-                      "## Bias and Variance Interactive Bar Chart",
+                      "## Fairness and Stability Interactive Bar Chart",
                       individual_metrics_interactive_bar_chart_desc,
                       dp.Plot(interactive_bar_chart),
 
-                      "## Model Ranks Based On Group Statistical Bias and Variance Metrics",
+                      "## Model Ranks Based On Group Fairness and Stability Metrics",
                       model_ranked_heatmap_desc,
                       dp.Plot(model_rank_heatmap, responsive=False),
 
-                      "## Total Ranks Sum For Group Statistical Bias and Variance Metrics",
+                      "## Total Ranks Sum For Group Fairness and Stability Metrics",
                       overall_model_ranked_heatmap_desc,
                       dp.Plot(total_model_rank_heatmap, responsive=False),
                       ).save(path=os.path.join(report_save_path, report_filename))
         else:
-            dp.Report("# Statistical Bias and Variance Report",
+            dp.Report("# Fairness and Stability Report",
                       general_desc,
 
                       "## Model Composed Metrics",
                       composed_metrics_desc,
                       dp.DataTable(self.models_composed_metrics_df),
 
-                      "## Overall Bias and Variance Model Metrics Comparison",
+                      "## Overall Fairness and Stability Model Metrics Comparison",
                       overall_metrics_desc,
-                      dp.Plot(bias_overall_metrics_bar_chart, responsive=False),
+                      dp.Plot(fairness_overall_metrics_bar_chart, responsive=False),
                       dp.Plot(variance_overall_metrics_bar_chart, responsive=False),
 
-                      "## Bias and Variance Interactive Bar Chart",
+                      "## Fairness and Stability Interactive Bar Chart",
                       individual_metrics_interactive_bar_chart_desc,
                       dp.Plot(interactive_bar_chart),
 
-                      "## Model Ranks Based On Group Statistical Bias and Variance Metrics",
+                      "## Model Ranks Based On Group Fairness and Stability Metrics",
                       model_ranked_heatmap_desc,
                       dp.Plot(model_rank_heatmap, responsive=False),
 
-                      "## Total Ranks Sum For Group Statistical Bias and Variance Metrics",
+                      "## Total Ranks Sum For Group Fairness and Stability Metrics",
                       overall_model_ranked_heatmap_desc,
                       dp.Plot(total_model_rank_heatmap, responsive=False),
                       ).save(path=os.path.join(report_save_path, report_filename))
 
         self.__create_report = False
```

### Comparing `virny-0.1.1/virny/metrics/__init__.py` & `virny-0.2.0/virny/metrics/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-This module contains functions for variance and statistical bias metrics.
+This module contains functions for computing subgroup variance and error metrics.
 """
 from .stability_metrics import (
     compute_std_mean_iqr_metrics,
     compute_churn,
     compute_jitter,
     compute_entropy,
     compute_conf_interval,
```

### Comparing `virny-0.1.1/virny/metrics/stability_metrics.py` & `virny-0.2.0/virny/metrics/stability_metrics.py`

 * *Files identical despite different names*

### Comparing `virny-0.1.1/virny/utils/custom_initializers.py` & `virny-0.2.0/virny/utils/custom_initializers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import yaml
 import pandas as pd
 from munch import DefaultMunch
 
-from virny.custom_classes.generic_pipeline import GenericPipeline
 from virny.utils.common_helpers import validate_config
+from virny.configs.constants import INTERSECTION_SIGN
 
 
 def create_config_obj(config_yaml_path: str):
     """
     Return a config object created based on a config yaml file.
 
     Parameters
@@ -19,14 +19,23 @@
     """
     with open(config_yaml_path) as f:
         config_dct = yaml.load(f, Loader=yaml.FullLoader)
 
     config_obj = DefaultMunch.fromDict(config_dct)
     validate_config(config_obj)
 
+    # Fix formatting
+    sensitive_attributes_dct_keys = list(config_obj.sensitive_attributes_dct.keys())
+    for attr in sensitive_attributes_dct_keys:
+        if INTERSECTION_SIGN in attr:
+            attrs = attr.strip().split(INTERSECTION_SIGN)
+            cleaned_attr = INTERSECTION_SIGN.join(attr.strip() for attr in attrs)
+            if cleaned_attr != attr:
+                config_obj.sensitive_attributes_dct[cleaned_attr] = config_obj.sensitive_attributes_dct.pop(attr)
+
     return config_obj
 
 
 def read_model_metric_dfs(metrics_path, model_names):
     # Read models metrics dfs
     metrics_filenames = [filename for filename in os.listdir(metrics_path)]
     models_metrics_dct = dict()
@@ -35,28 +44,46 @@
             if model_name in filename:
                 models_metrics_dct[model_name] = pd.read_csv(f'{metrics_path}/{filename}')
                 break
 
     return models_metrics_dct
 
 
-def create_models_config_from_tuned_params_df(models_config_for_tuning, models_tuned_params_df):
-    experiment_models_config = dict()
-    for model_idx in range(len(models_config_for_tuning)):
-        model_name = models_config_for_tuning[model_idx]["model_name"]
-        base_model = create_tuned_base_model(models_config_for_tuning[model_idx]['model'], model_name, models_tuned_params_df)
-        experiment_models_config[model_name] = base_model
+def create_models_metrics_dct_from_database_df(model_metric_dfs):
+    """
+    Create a models_metrics_dct from a metrics dataframe written to a database.
+    Return the models_metrics_dct where a key is a model name and a value is a metrics dataframe for the model.
 
-    return experiment_models_config
+    Parameters
+    ----------
+    model_metric_dfs
+        Path to a config yaml file
 
+    """
+    # Create columns based on values in the Subgroup column
+    pivoted_model_metric_dfs = model_metric_dfs.pivot(columns='Subgroup', values='Metric_Value',
+                                                      index=[col for col in model_metric_dfs.columns
+                                                             if col not in ('Subgroup', 'Metric_Value')]).reset_index()
+    pivoted_model_metric_dfs = pivoted_model_metric_dfs.rename_axis(None, axis=1)
+
+    # Create a dict of metrics for each model
+    models_metrics_dct = dict()
+    for model_name in pivoted_model_metric_dfs['Model_Name'].unique():
+        models_metrics_dct[model_name] = pivoted_model_metric_dfs[pivoted_model_metric_dfs['Model_Name'] == model_name]
+
+    return models_metrics_dct
 
-def create_base_pipeline(dataset, sensitive_attributes_dct, model_seed, test_set_fraction):
-    base_pipeline = GenericPipeline(dataset, sensitive_attributes_dct)
-    _ = base_pipeline.create_preprocessed_train_test_split(dataset, test_set_fraction, seed=model_seed)
 
-    return base_pipeline
+def create_models_config_from_tuned_params_df(models_config_for_tuning: dict, tuned_params_df_path: str):
+    models_tuned_params_df = pd.read_csv(tuned_params_df_path)
+    experiment_models_config = dict()
+    for model_name, model_params in models_config_for_tuning.items():
+        base_model = create_tuned_base_model(model_params['model'], model_name, models_tuned_params_df)
+        experiment_models_config[model_name] = base_model
+
+    return experiment_models_config
 
 
 def create_tuned_base_model(init_model, model_name, models_tuned_params_df):
     model_params = eval(models_tuned_params_df.loc[models_tuned_params_df['Model_Name'] == model_name,
                                                    'Model_Best_Params'].iloc[0])
     return init_model.set_params(**model_params)
```

### Comparing `virny-0.1.1/virny/utils/data_viz_utils.py` & `virny-0.2.0/virny/utils/data_viz_utils.py`

 * *Files identical despite different names*

### Comparing `virny-0.1.1/virny/utils/model_tuning_utils.py` & `virny-0.2.0/virny/utils/model_tuning_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,79 +3,36 @@
 import seaborn as sns
 import matplotlib.pyplot as plt
 
 from pprint import pprint
 from copy import deepcopy
 from datetime import datetime
 
-from sklearn.model_selection import train_test_split
 from sklearn.model_selection import GridSearchCV
 from sklearn.metrics import make_scorer, accuracy_score, f1_score
 from sklearn.metrics import confusion_matrix, ConfusionMatrixDisplay, classification_report
 
-from virny.configs.constants import MODELS_TUNING_TEST_SET_FRACTION, MODELS_TUNING_SEED
-from virny.preprocessing.basic_preprocessing import make_features_dfs
+from virny.custom_classes.base_dataset import BaseFlowDataset
 
 
 def folds_iterator(n_folds, samples_per_fold, size):
     """
     Iterator for GridSearch based on Cross-Validation
 
     :param n_folds: number of folds for Cross-Validation
     :param samples_per_fold: number of samples per fold
     """
     for i in range(n_folds):
         yield np.arange(0, size - samples_per_fold * (i + 1)), \
               np.arange(size - samples_per_fold * (i + 1), size - samples_per_fold * i)
 
 
-def test_baseline_models(models_config, dataset, dataset_name, n_folds = 3):
-    """
-    Prepare datasets and find the best model for an original baseline dataset without nulls.
-
-    :return: a dataframe of metrics, measured for each model and its best parameters
-    """
-    X_train, X_test, y_train, y_test = train_test_split(dataset.X_data, dataset.y_data,
-                                                        test_size=MODELS_TUNING_TEST_SET_FRACTION,
-                                                        random_state=MODELS_TUNING_SEED)
-    print("Baseline X_train shape: ", X_train.shape)
-    print("Baseline X_test shape: ", X_test.shape)
-
-    X_train_features, X_test_features = make_features_dfs(X_train, X_test, dataset)
-    print('X_train_features.columns: ', X_train_features.columns)
-
-    samples_per_fold = len(y_test)
-    best_results_df = pd.DataFrame(columns=('Dataset_Name', 'Model_Name', 'F1_Score',
-                                            'Accuracy_Score',
-                                            'Model_Best_Params', 'Model_Pred'))
-    ML_results_df = test_ML_models(best_results_df, models_config, n_folds, samples_per_fold,
-                                   X_train_features, y_train, X_test_features, y_test, dataset_name,
-                                   show_plots=True, debug_mode=True)
-    return ML_results_df
-
-
-def test_models(models_config, X_train_features, y_train, X_test_features, y_test, n_folds = 3):
-    """
-    Find the best model for a non-baseline dataset without nulls.
-
-    :return: a dataframe of metrics, measured for each model and its best parameters
-    """
-    samples_per_fold = len(y_test)
-    best_results_df = pd.DataFrame(columns=('Dataset_Name', 'Model_Name', 'F1_Score',
-                                            'Accuracy_Score',
-                                            'Model_Best_Params', 'Model_Pred'))
-    ML_results_df = test_ML_models(best_results_df, models_config, n_folds, samples_per_fold,
-                                   X_train_features, y_train, X_test_features, y_test, "Folktables [NY 2018]",
-                                   show_plots=True, debug_mode=True)
-    return ML_results_df
-
-
 def validate_model(model, x, y, params, n_folds, samples_per_fold):
     """
-    Use GridSearchCV for a special model to find the best hyper-parameters based on validation set
+    Use GridSearchCV for a special model to find the best hyperparameters based on validation set
     """
     grid_search = GridSearchCV(estimator=model,
                                param_grid=params,
                                scoring={
                                    "F1_Score": make_scorer(f1_score, average='macro'),
                                    "Accuracy_Score": make_scorer(accuracy_score),
                                },
@@ -118,28 +75,66 @@
     if show_plots:
         # plot the confusion matrix
         sns.set_style("white")
         cm = confusion_matrix(cur_y_test, cur_model_pred, labels=cur_best_model.classes_)
         disp = ConfusionMatrixDisplay(confusion_matrix=cm, display_labels=["Employed", "Not Employed"])
         disp.plot()
         plt.show()
+
     return test_f1_score, test_accuracy, cur_model_pred
 
 
-def test_ML_models(best_results_df, models_config, n_folds, samples_per_fold,
-                   X_train, y_train, X_test, y_test, dataset_title, show_plots, debug_mode):
+def tune_ML_models(models_params_for_tuning: dict, base_flow_dataset: BaseFlowDataset,
+                   dataset_name: str, n_folds: int = 3, samples_per_fold: int = None):
+    """
+    Tune each model on a validation set with GridSearchCV.
+
+    Return each model with its best hyperparameters that have the highest F1 score and Accuracy.
+     results_df is a dataframe with metrics and tuned parameters;
+     models_config is a dict with model tuned params for the metrics computation stage
+    """
+    if samples_per_fold is None:
+        samples_per_fold = len(base_flow_dataset.y_test)
+
+    models_config = dict()
+    tuned_params_df = pd.DataFrame(columns=('Dataset_Name', 'Model_Name', 'F1_Score', 'Accuracy_Score', 'Model_Best_Params'))
+    # Find the most optimal hyperparameters based on accuracy and F1-score for each model in models_config
+    for model_idx, (model_name, model_params) in enumerate(models_params_for_tuning.items()):
+        try:
+            print(f"{datetime.now().strftime('%Y/%m/%d, %H:%M:%S')}: Tuning {model_name}...")
+            cur_model, cur_f1_score, cur_accuracy, cur_params = validate_model(deepcopy(model_params['model']),
+                                                                               base_flow_dataset.X_train_val,
+                                                                               base_flow_dataset.y_train_val,
+                                                                               model_params['params'],
+                                                                               n_folds, samples_per_fold)
+            print(f'{datetime.now().strftime("%Y/%m/%d, %H:%M:%S")}: Tuning for {model_name} is finished '
+                  f'[F1 score = {cur_f1_score}, Accuracy = {cur_accuracy}]\n')
+
+        except Exception as err:
+            print(f"ERROR with {model_name}: ", err)
+            continue
+
+        # Save test results of each model in dataframe
+        tuned_params_df.loc[model_idx] = [dataset_name, model_name, cur_f1_score, cur_accuracy, cur_params]
+        models_config[model_name] = model_params['model'].set_params(**cur_params)
+
+    return tuned_params_df, models_config
+
+
+def test_ML_models(best_results_df, models_config, n_folds, X_train, y_train, X_test, y_test,
+                   dataset_title, show_plots, debug_mode):
     """
     Find the best model from defined list.
     Tune each model on a validation set with GridSearchCV and
-    return best_model with its hyper-parameters, which has the highest F1 score
+    return best_model with its hyperparameters, which has the highest F1 score
     """
     results_df = pd.DataFrame(columns=('Dataset_Name', 'Model_Name', 'F1_Score',
                                        'Accuracy_Score',
                                        'Model_Best_Params'))
-
+    samples_per_fold = len(y_test)
     best_f1_score = -np.Inf
     best_accuracy = -np.Inf
     best_model_pred = []
     best_model_name = 'No model'
     best_params = None
     idx = 0
     # find the best model among defined in models_config
```

### Comparing `virny-0.1.1/virny/utils/stability_utils.py` & `virny-0.2.0/virny/utils/stability_utils.py`

 * *Files identical despite different names*

### Comparing `virny-0.1.1/virny.egg-info/PKG-INFO` & `virny-0.2.0/virny.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: virny
-Version: 0.1.1
+Version: 0.2.0
 Summary: Python library for auditing model stability and fairness
 Home-page: https://github.com/DataResponsibly/Virny
 Author: Denys Herasymuk
 Author-email: denis.gerasymuk799@gmail.com
 License: BSD-3
 Description: # Virny Software Library
         
@@ -32,15 +32,15 @@
           <!-- Last Commit -->
           <a href="">
             <img src="https://img.shields.io/github/last-commit/DataResponsibly/Virny.svg" alt="last_commit">
           </a>
         </p>
         
         
-        ## Description 📜
+        ## 📜 Description
         
         **Virny** is a Python library for auditing model stability and fairness. The Virny library was
         developed based on three fundamental principles: 
         
         1) easy extensibility of model analysis capabilities;
         2) compatibility to user-defined/custom datasets and model types;
         3) simple composition of parity metrics based on context of use.
@@ -48,63 +48,62 @@
         Virny decouples model auditing into several stages, including: **subgroup metrics computation**, **group metrics composition**,
         and **metrics visualization and reporting**. This gives data scientists and practitioners more control and flexibility 
         to use the library for model development and monitoring post-deployment.
         
         For quickstart, look at our [Use Case Examples](https://dataresponsibly.github.io/Virny/examples/Multiple_Runs_Interface_Use_Case/).
         
         
-        ## Documentation 📒
+        ## 📒 Documentation
         
         * [Introduction](https://dataresponsibly.github.io/Virny/)
         * [API Reference](https://dataresponsibly.github.io/Virny/api/overview/)
         * [Use Case Examples](https://dataresponsibly.github.io/Virny/examples/Multiple_Runs_Interface_Use_Case/)
         
         
-        ## Features 💡
+        ## 💡 Features
         
         * Entire pipeline for auditing model stability and fairness
         * Metrics reports and visualizations
         * Ability to analyze intersections of sensitive attributes
         * Blind classifiers audit
         * Interface for multiple runs and multiple models
         * User-friendly parameters input via config yaml files
         * Built-in preprocessing techniques for raw classification datasets
         * Check out [our documentation](https://dataresponsibly.github.io/Virny/) for a comprehensive overview
         
         
-        ## Library Terminology 📖
+        ## 📖 Library Terminology
         
         This section briefly explains the main terminology used in our library.
         
         * A **sensitive attribute** is an attribute that partitions the population into groups with unequal benefits received.
         * A **protected group** (or simply _group_) is created by partitioning the population by one or many sensitive attributes.
         * A **privileged value** of a sensitive attribute is a value that gives more benefit to a protected group, which includes it, than to protected groups, which do not include it.
         * A **subgroup** is created by splitting a protected group by privileges and disprivileged values.
         * A **group metric** is a metric that shows the relation between privileged and disprivileged subgroups created based on one or many sensitive attributes.
         
         
-        ## Installation 🛠
+        ## 🛠 Installation
         
-        Virny supports **Python 3.8, 3.9** and can be installed with `pip`:
+        Virny supports **Python 3.8 (recommended), 3.9** and can be installed with `pip`:
         
         ```bash
         pip install virny
         ```
         
         
-        ## Affiliations 🤗
+        ## 🤗 Affiliations
         
         ![NYU-UCU-Logos](https://user-images.githubusercontent.com/42843889/216840888-071bf184-f0e3-4a3e-94dc-c0d1c7784143.png)
         
         
-        ## License 📝
+        ## 📝 License
         
         **Virny** is free and open-source software licensed under the [3-clause BSD license](https://github.com/DataResponsibly/Virny/blob/main/LICENSE).
         
-        
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,50 +1,50 @@
-Metadata-Version: 2.1 Name: virny Version: 0.1.1 Summary: Python library for
+Metadata-Version: 2.1 Name: virny Version: 0.2.0 Summary: Python library for
 auditing model stability and fairness Home-page: https://github.com/
 DataResponsibly/Virny Author: Denys Herasymuk Author-email:
 denis.gerasymuk799@gmail.com License: BSD-3 Description: # Virny Software
 Library
  [CI_Pipeline]  [documentation]  [pypi]  [bsd_3_license]  [code_size]
 [last_commit]
-## Description ð **Virny** is a Python library for auditing model stability
+## ð Description **Virny** is a Python library for auditing model stability
 and fairness. The Virny library was developed based on three fundamental
 principles: 1) easy extensibility of model analysis capabilities; 2)
 compatibility to user-defined/custom datasets and model types; 3) simple
 composition of parity metrics based on context of use. Virny decouples model
 auditing into several stages, including: **subgroup metrics computation**,
 **group metrics composition**, and **metrics visualization and reporting**.
 This gives data scientists and practitioners more control and flexibility to
 use the library for model development and monitoring post-deployment. For
 quickstart, look at our [Use Case Examples](https://dataresponsibly.github.io/
-Virny/examples/Multiple_Runs_Interface_Use_Case/). ## Documentation ð *
+Virny/examples/Multiple_Runs_Interface_Use_Case/). ## ð Documentation *
 [Introduction](https://dataresponsibly.github.io/Virny/) * [API Reference]
 (https://dataresponsibly.github.io/Virny/api/overview/) * [Use Case Examples]
 (https://dataresponsibly.github.io/Virny/examples/
-Multiple_Runs_Interface_Use_Case/) ## Features ð¡ * Entire pipeline for
+Multiple_Runs_Interface_Use_Case/) ## ð¡ Features * Entire pipeline for
 auditing model stability and fairness * Metrics reports and visualizations *
 Ability to analyze intersections of sensitive attributes * Blind classifiers
 audit * Interface for multiple runs and multiple models * User-friendly
 parameters input via config yaml files * Built-in preprocessing techniques for
 raw classification datasets * Check out [our documentation](https://
-dataresponsibly.github.io/Virny/) for a comprehensive overview ## Library
-Terminology ð This section briefly explains the main terminology used in our
+dataresponsibly.github.io/Virny/) for a comprehensive overview ## ð Library
+Terminology This section briefly explains the main terminology used in our
 library. * A **sensitive attribute** is an attribute that partitions the
 population into groups with unequal benefits received. * A **protected group**
 (or simply _group_) is created by partitioning the population by one or many
 sensitive attributes. * A **privileged value** of a sensitive attribute is a
 value that gives more benefit to a protected group, which includes it, than to
 protected groups, which do not include it. * A **subgroup** is created by
 splitting a protected group by privileges and disprivileged values. * A **group
 metric** is a metric that shows the relation between privileged and
 disprivileged subgroups created based on one or many sensitive attributes. ##
-Installation ð  Virny supports **Python 3.8, 3.9** and can be installed with
-`pip`: ```bash pip install virny ``` ## Affiliations ð¤ ![NYU-UCU-Logos]
-(https://user-images.githubusercontent.com/42843889/216840888-071bf184-f0e3-
-4a3e-94dc-c0d1c7784143.png) ## License ð **Virny** is free and open-source
-software licensed under the [3-clause BSD license](https://github.com/
-DataResponsibly/Virny/blob/main/LICENSE). Platform: UNKNOWN Classifier:
-Intended Audience :: Developers Classifier: License :: OSI Approved :: BSD
-License Classifier: Programming Language :: Python Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Operating System
-:: OS Independent Description-Content-Type: text/markdown Provides-Extra: dev
-Provides-Extra: docs
+ð  Installation Virny supports **Python 3.8 (recommended), 3.9** and can be
+installed with `pip`: ```bash pip install virny ``` ## ð¤ Affiliations ![NYU-
+UCU-Logos](https://user-images.githubusercontent.com/42843889/216840888-
+071bf184-f0e3-4a3e-94dc-c0d1c7784143.png) ## ð License **Virny** is free and
+open-source software licensed under the [3-clause BSD license](https://
+github.com/DataResponsibly/Virny/blob/main/LICENSE). Platform: UNKNOWN
+Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
+:: BSD License Classifier: Programming Language :: Python Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Operating
+System :: OS Independent Description-Content-Type: text/markdown Provides-
+Extra: dev Provides-Extra: docs
```

### Comparing `virny-0.1.1/virny.egg-info/SOURCES.txt` & `virny-0.2.0/virny.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,49 +1,58 @@
+MANIFEST.in
 README.md
 setup.py
 tests/custom_classes/__init__.py
 tests/custom_classes/test_metrics_composer.py
 tests/metrics/__init__.py
 tests/metrics/test_stability_metrics.py
 tests/preprocessing/__init__.py
 tests/preprocessing/test_basic_preprocessing.py
 tests/utils/__init__.py
 tests/utils/test_common_helpers.py
-tests/utils/test_custom_initializers.py
+tests/utils/test_protected_groups_partitioning.py
 tests/utils/test_stability_utils.py
 virny/__init__.py
 virny/__version__.py
 virny/api.py
 virny.egg-info/PKG-INFO
 virny.egg-info/SOURCES.txt
 virny.egg-info/dependency_links.txt
 virny.egg-info/requires.txt
 virny.egg-info/top_level.txt
 virny/analyzers/__init__.py
 virny/analyzers/abstract_overall_variance_analyzer.py
 virny/analyzers/abstract_subgroup_analyzer.py
 virny/analyzers/batch_overall_variance_analyzer.py
-virny/analyzers/subgroup_statistical_bias_analyzer.py
+virny/analyzers/incremental_overall_variance_analyzer.py
+virny/analyzers/subgroup_error_analyzer.py
 virny/analyzers/subgroup_variance_analyzer.py
 virny/analyzers/subgroup_variance_calculator.py
 virny/configs/__init__.py
 virny/configs/constants.py
 virny/custom_classes/__init__.py
 virny/custom_classes/base_dataset.py
 virny/custom_classes/custom_logger.py
-virny/custom_classes/generic_pipeline.py
+virny/custom_classes/incremental_pandas_dataset.py
 virny/custom_classes/metrics_composer.py
 virny/custom_classes/metrics_visualizer.py
+virny/datasets/COMPAS.csv
 virny/datasets/__init__.py
+virny/datasets/base.py
 virny/datasets/data_loaders.py
+virny/datasets/givemesomecredit.csv
+virny/incremental_ml/__init__.py
+virny/incremental_ml/river_utils.py
 virny/metrics/__init__.py
 virny/metrics/stability_metrics.py
 virny/preprocessing/__init__.py
 virny/preprocessing/basic_preprocessing.py
 virny/user_interfaces/__init__.py
 virny/user_interfaces/metrics_computation_interfaces.py
 virny/utils/__init__.py
 virny/utils/common_helpers.py
 virny/utils/custom_initializers.py
 virny/utils/data_viz_utils.py
 virny/utils/model_tuning_utils.py
-virny/utils/stability_utils.py
+virny/utils/protected_groups_partitioning.py
+virny/utils/stability_utils.py
+virny/utils/validation.py
```

