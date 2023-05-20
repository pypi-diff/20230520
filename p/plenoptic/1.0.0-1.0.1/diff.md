# Comparing `tmp/plenoptic-1.0.0.tar.gz` & `tmp/plenoptic-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plenoptic-1.0.0.tar", last modified: Fri May 19 17:45:07 2023, max compression
+gzip compressed data, was "plenoptic-1.0.1.tar", last modified: Sat May 20 16:36:09 2023, max compression
```

## Comparing `plenoptic-1.0.0.tar` & `plenoptic-1.0.1.tar`

### file list

```diff
@@ -1,67 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:45:07.820342 plenoptic-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-19 17:44:56.000000 plenoptic-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7681 2023-05-19 17:45:07.820342 plenoptic-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-05-19 17:44:56.000000 plenoptic-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:45:07.816342 plenoptic-1.0.0/plenoptic/
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-19 17:44:56.000000 plenoptic-1.0.0/plenoptic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:45:07.816342 plenoptic-1.0.0/plenoptic/metric/
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-19 17:44:56.000000 plenoptic-1.0.0/plenoptic/metric/DN_filts.npy
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-19 17:44:56.000000 plenoptic-1.0.0/plenoptic/metric/DN_sigmas.npy
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-19 17:44:56.000000 plenoptic-1.0.0/plenoptic/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-19 17:44:56.000000 plenoptic-1.0.0/plenoptic/metric/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-19 17:44:56.000000 plenoptic-1.0.0/plenoptic/metric/model_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-19 17:44:56.000000 plenoptic-1.0.0/plenoptic/metric/naive.py
--rw-r--r--   0 runner    (1001) docker     (123)    21252 2023-05-19 17:44:56.000000 plenoptic-1.0.0/plenoptic/metric/perceptual_distance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:45:07.816342 plenoptic-1.0.0/plenoptic/simulate/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-19 17:44:56.000000 plenoptic-1.0.0/plenoptic/simulate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:45:07.816342 plenoptic-1.0.0/plenoptic/simulate/canonical_computations/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 17:44:56.000000 plenoptic-1.0.0/plenoptic/simulate/canonical_computations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-19 17:44:56.000000 plenoptic-1.0.0/plenoptic/simulate/canonical_computations/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-05-19 17:44:56.000000 plenoptic-1.0.0/plenoptic/simulate/canonical_computations/laplacian_pyramid.py
--rw-r--r--   0 runner    (1001) docker     (123)     7902 2023-05-19 17:44:56.000000 plenoptic-1.0.0/plenoptic/simulate/canonical_computations/non_linearities.py
--rw-r--r--   0 runner    (1001) docker     (123)    39902 2023-05-19 17:44:56.000000 plenoptic-1.0.0/plenoptic/simulate/canonical_computations/steerable_pyramid_freq.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:45:07.816342 plenoptic-1.0.0/plenoptic/simulate/models/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-19 17:44:56.000000 plenoptic-1.0.0/plenoptic/simulate/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16483 2023-05-19 17:44:56.000000 plenoptic-1.0.0/plenoptic/simulate/models/frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)     9433 2023-05-19 17:44:56.000000 plenoptic-1.0.0/plenoptic/simulate/models/naive.py
--rw-r--r--   0 runner    (1001) docker     (123)    46368 2023-05-19 17:44:56.000000 plenoptic-1.0.0/plenoptic/simulate/models/portilla_simoncelli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:45:07.816342 plenoptic-1.0.0/plenoptic/synthesize/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-19 17:44:56.000000 plenoptic-1.0.0/plenoptic/synthesize/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5129 2023-05-19 17:44:56.000000 plenoptic-1.0.0/plenoptic/synthesize/autodiff.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25090 2023-05-19 17:44:56.000000 plenoptic-1.0.0/plenoptic/synthesize/eigendistortion.py
--rw-r--r--   0 runner    (1001) docker     (123)    25147 2023-05-19 17:44:56.000000 plenoptic-1.0.0/plenoptic/synthesize/geodesic.py
--rw-r--r--   0 runner    (1001) docker     (123)    56546 2023-05-19 17:44:56.000000 plenoptic-1.0.0/plenoptic/synthesize/mad_competition.py
--rw-r--r--   0 runner    (1001) docker     (123)    72830 2023-05-19 17:44:56.000000 plenoptic-1.0.0/plenoptic/synthesize/metamer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-05-19 17:44:56.000000 plenoptic-1.0.0/plenoptic/synthesize/simple_metamer.py
--rw-r--r--   0 runner    (1001) docker     (123)    17289 2023-05-19 17:44:56.000000 plenoptic-1.0.0/plenoptic/synthesize/synthesis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:45:07.820342 plenoptic-1.0.0/plenoptic/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-19 17:44:56.000000 plenoptic-1.0.0/plenoptic/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-05-19 17:44:56.000000 plenoptic-1.0.0/plenoptic/tools/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-05-19 17:44:56.000000 plenoptic-1.0.0/plenoptic/tools/convergence.py
--rw-r--r--   0 runner    (1001) docker     (123)    13440 2023-05-19 17:44:56.000000 plenoptic-1.0.0/plenoptic/tools/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    46389 2023-05-19 17:44:56.000000 plenoptic-1.0.0/plenoptic/tools/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-05-19 17:44:56.000000 plenoptic-1.0.0/plenoptic/tools/external.py
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-05-19 17:44:56.000000 plenoptic-1.0.0/plenoptic/tools/optim.py
--rw-r--r--   0 runner    (1001) docker     (123)    12541 2023-05-19 17:44:56.000000 plenoptic-1.0.0/plenoptic/tools/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-19 17:44:56.000000 plenoptic-1.0.0/plenoptic/tools/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-05-19 17:44:56.000000 plenoptic-1.0.0/plenoptic/tools/straightness.py
--rw-r--r--   0 runner    (1001) docker     (123)    11791 2023-05-19 17:44:56.000000 plenoptic-1.0.0/plenoptic/tools/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-19 17:44:56.000000 plenoptic-1.0.0/plenoptic/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:45:07.816342 plenoptic-1.0.0/plenoptic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7681 2023-05-19 17:45:07.000000 plenoptic-1.0.0/plenoptic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-05-19 17:45:07.000000 plenoptic-1.0.0/plenoptic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 17:45:07.000000 plenoptic-1.0.0/plenoptic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-19 17:45:07.000000 plenoptic-1.0.0/plenoptic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-19 17:45:07.000000 plenoptic-1.0.0/plenoptic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 17:45:07.820342 plenoptic-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-19 17:44:56.000000 plenoptic-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:45:07.820342 plenoptic-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    36133 2023-05-19 17:44:56.000000 plenoptic-1.0.0/tests/test_display.py
--rw-r--r--   0 runner    (1001) docker     (123)    13244 2023-05-19 17:44:56.000000 plenoptic-1.0.0/tests/test_eigendistortion.py
--rw-r--r--   0 runner    (1001) docker     (123)    17176 2023-05-19 17:44:56.000000 plenoptic-1.0.0/tests/test_geodesic.py
--rw-r--r--   0 runner    (1001) docker     (123)    10940 2023-05-19 17:44:56.000000 plenoptic-1.0.0/tests/test_mad.py
--rw-r--r--   0 runner    (1001) docker     (123)    12804 2023-05-19 17:44:56.000000 plenoptic-1.0.0/tests/test_metamers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10930 2023-05-19 17:44:56.000000 plenoptic-1.0.0/tests/test_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    19730 2023-05-19 17:44:56.000000 plenoptic-1.0.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    14857 2023-05-19 17:44:56.000000 plenoptic-1.0.0/tests/test_steerable_pyr.py
--rw-r--r--   0 runner    (1001) docker     (123)    13300 2023-05-19 17:44:56.000000 plenoptic-1.0.0/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 16:36:09.418532 plenoptic-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-20 16:35:58.000000 plenoptic-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-20 16:35:58.000000 plenoptic-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7681 2023-05-20 16:36:09.418532 plenoptic-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-05-20 16:35:58.000000 plenoptic-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 16:36:09.410532 plenoptic-1.0.1/jenkins/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-20 16:35:58.000000 plenoptic-1.0.1/jenkins/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 16:36:09.410532 plenoptic-1.0.1/plenoptic/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-20 16:35:58.000000 plenoptic-1.0.1/plenoptic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 16:36:09.414532 plenoptic-1.0.1/plenoptic/metric/
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-20 16:35:58.000000 plenoptic-1.0.1/plenoptic/metric/DN_filts.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-20 16:35:58.000000 plenoptic-1.0.1/plenoptic/metric/DN_sigmas.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-20 16:35:58.000000 plenoptic-1.0.1/plenoptic/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-20 16:35:58.000000 plenoptic-1.0.1/plenoptic/metric/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-20 16:35:58.000000 plenoptic-1.0.1/plenoptic/metric/model_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-20 16:35:58.000000 plenoptic-1.0.1/plenoptic/metric/naive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21252 2023-05-20 16:35:58.000000 plenoptic-1.0.1/plenoptic/metric/perceptual_distance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 16:36:09.414532 plenoptic-1.0.1/plenoptic/simulate/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-20 16:35:58.000000 plenoptic-1.0.1/plenoptic/simulate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 16:36:09.414532 plenoptic-1.0.1/plenoptic/simulate/canonical_computations/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 16:35:58.000000 plenoptic-1.0.1/plenoptic/simulate/canonical_computations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-20 16:35:58.000000 plenoptic-1.0.1/plenoptic/simulate/canonical_computations/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-05-20 16:35:58.000000 plenoptic-1.0.1/plenoptic/simulate/canonical_computations/laplacian_pyramid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7902 2023-05-20 16:35:58.000000 plenoptic-1.0.1/plenoptic/simulate/canonical_computations/non_linearities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39902 2023-05-20 16:35:58.000000 plenoptic-1.0.1/plenoptic/simulate/canonical_computations/steerable_pyramid_freq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 16:36:09.414532 plenoptic-1.0.1/plenoptic/simulate/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-20 16:35:58.000000 plenoptic-1.0.1/plenoptic/simulate/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16483 2023-05-20 16:35:58.000000 plenoptic-1.0.1/plenoptic/simulate/models/frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9433 2023-05-20 16:35:58.000000 plenoptic-1.0.1/plenoptic/simulate/models/naive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46368 2023-05-20 16:35:58.000000 plenoptic-1.0.1/plenoptic/simulate/models/portilla_simoncelli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 16:36:09.414532 plenoptic-1.0.1/plenoptic/synthesize/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-20 16:35:58.000000 plenoptic-1.0.1/plenoptic/synthesize/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5129 2023-05-20 16:35:58.000000 plenoptic-1.0.1/plenoptic/synthesize/autodiff.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25090 2023-05-20 16:35:58.000000 plenoptic-1.0.1/plenoptic/synthesize/eigendistortion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25147 2023-05-20 16:35:58.000000 plenoptic-1.0.1/plenoptic/synthesize/geodesic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56546 2023-05-20 16:35:58.000000 plenoptic-1.0.1/plenoptic/synthesize/mad_competition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72830 2023-05-20 16:35:58.000000 plenoptic-1.0.1/plenoptic/synthesize/metamer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-05-20 16:35:58.000000 plenoptic-1.0.1/plenoptic/synthesize/simple_metamer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17289 2023-05-20 16:35:58.000000 plenoptic-1.0.1/plenoptic/synthesize/synthesis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 16:36:09.418532 plenoptic-1.0.1/plenoptic/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-20 16:35:58.000000 plenoptic-1.0.1/plenoptic/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-05-20 16:35:58.000000 plenoptic-1.0.1/plenoptic/tools/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-05-20 16:35:58.000000 plenoptic-1.0.1/plenoptic/tools/convergence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13440 2023-05-20 16:35:58.000000 plenoptic-1.0.1/plenoptic/tools/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46389 2023-05-20 16:35:58.000000 plenoptic-1.0.1/plenoptic/tools/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-05-20 16:35:58.000000 plenoptic-1.0.1/plenoptic/tools/external.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-05-20 16:35:58.000000 plenoptic-1.0.1/plenoptic/tools/optim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12541 2023-05-20 16:35:58.000000 plenoptic-1.0.1/plenoptic/tools/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-20 16:35:58.000000 plenoptic-1.0.1/plenoptic/tools/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-05-20 16:35:58.000000 plenoptic-1.0.1/plenoptic/tools/straightness.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11791 2023-05-20 16:35:58.000000 plenoptic-1.0.1/plenoptic/tools/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-20 16:35:58.000000 plenoptic-1.0.1/plenoptic/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 16:36:09.410532 plenoptic-1.0.1/plenoptic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7681 2023-05-20 16:36:09.000000 plenoptic-1.0.1/plenoptic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-20 16:36:09.000000 plenoptic-1.0.1/plenoptic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 16:36:09.000000 plenoptic-1.0.1/plenoptic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-20 16:36:09.000000 plenoptic-1.0.1/plenoptic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-20 16:36:09.000000 plenoptic-1.0.1/plenoptic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 16:36:09.418532 plenoptic-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-20 16:35:58.000000 plenoptic-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 16:36:09.418532 plenoptic-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    36133 2023-05-20 16:35:58.000000 plenoptic-1.0.1/tests/test_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13244 2023-05-20 16:35:58.000000 plenoptic-1.0.1/tests/test_eigendistortion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17176 2023-05-20 16:35:58.000000 plenoptic-1.0.1/tests/test_geodesic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10940 2023-05-20 16:35:58.000000 plenoptic-1.0.1/tests/test_mad.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12804 2023-05-20 16:35:58.000000 plenoptic-1.0.1/tests/test_metamers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10930 2023-05-20 16:35:58.000000 plenoptic-1.0.1/tests/test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19730 2023-05-20 16:35:58.000000 plenoptic-1.0.1/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14857 2023-05-20 16:35:58.000000 plenoptic-1.0.1/tests/test_steerable_pyr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13300 2023-05-20 16:35:58.000000 plenoptic-1.0.1/tests/test_tools.py
```

### Comparing `plenoptic-1.0.0/LICENSE` & `plenoptic-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `plenoptic-1.0.0/PKG-INFO` & `plenoptic-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plenoptic
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python library for model-based stimulus synthesis.
 Home-page: https://github.com/LabForComputationalVision/plenoptic
 Author: LabForComputationalVision
 License: MIT
 Keywords: Visual Information Processing,PyTorch
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.7
@@ -20,15 +20,15 @@
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/LabForComputationalVision/plenoptic/blob/main/LICENSE)
 ![Python version](https://img.shields.io/badge/python-3.7|3.8|3.9|3.10-blue.svg)
 [![Build Status](https://github.com/LabForComputationalVision/plenoptic/workflows/build/badge.svg)](https://github.com/LabForComputationalVision/plenoptic/actions?query=workflow%3Abuild)
 [![Documentation Status](https://readthedocs.org/projects/plenoptic/badge/?version=latest)](https://plenoptic.readthedocs.io/en/latest/?badge=latest)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3995057.svg)](https://doi.org/10.5281/zenodo.3995057)
 [![codecov](https://codecov.io/gh/LabForComputationalVision/plenoptic/branch/main/graph/badge.svg?token=EDtl5kqXKA)](https://codecov.io/gh/LabForComputationalVision/plenoptic)
 [![Tutorials Status](https://github.com/LabForComputationalVision/plenoptic/workflows/tutorials/badge.svg)](https://github.com/LabForComputationalVision/plenoptic/actions?query=workflow%3Atutorials)
-[![Binder](http://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/LabForComputationalVision/plenoptic/1.0.0?filepath=examples)
+[![Binder](http://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/LabForComputationalVision/plenoptic/1.0.1?filepath=examples)
 
 ![](docs/images/plenoptic_logo_wide.svg)
 
 `plenoptic` is a python library for model-based stimulus synthesis. It
 provides tools to help researchers understand their model by
 synthesizing novel informative stimuli, which help build intuition for
 what features the model ignores and what it is sensitive to. These
```

### Comparing `plenoptic-1.0.0/README.md` & `plenoptic-1.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/LabForComputationalVision/plenoptic/blob/main/LICENSE)
 ![Python version](https://img.shields.io/badge/python-3.7|3.8|3.9|3.10-blue.svg)
 [![Build Status](https://github.com/LabForComputationalVision/plenoptic/workflows/build/badge.svg)](https://github.com/LabForComputationalVision/plenoptic/actions?query=workflow%3Abuild)
 [![Documentation Status](https://readthedocs.org/projects/plenoptic/badge/?version=latest)](https://plenoptic.readthedocs.io/en/latest/?badge=latest)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3995057.svg)](https://doi.org/10.5281/zenodo.3995057)
 [![codecov](https://codecov.io/gh/LabForComputationalVision/plenoptic/branch/main/graph/badge.svg?token=EDtl5kqXKA)](https://codecov.io/gh/LabForComputationalVision/plenoptic)
 [![Tutorials Status](https://github.com/LabForComputationalVision/plenoptic/workflows/tutorials/badge.svg)](https://github.com/LabForComputationalVision/plenoptic/actions?query=workflow%3Atutorials)
-[![Binder](http://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/LabForComputationalVision/plenoptic/1.0.0?filepath=examples)
+[![Binder](http://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/LabForComputationalVision/plenoptic/1.0.1?filepath=examples)
 
 ![](docs/images/plenoptic_logo_wide.svg)
 
 `plenoptic` is a python library for model-based stimulus synthesis. It
 provides tools to help researchers understand their model by
 synthesizing novel informative stimuli, which help build intuition for
 what features the model ignores and what it is sensitive to. These
```

### Comparing `plenoptic-1.0.0/plenoptic/metric/DN_filts.npy` & `plenoptic-1.0.1/plenoptic/metric/DN_filts.npy`

 * *Files identical despite different names*

### Comparing `plenoptic-1.0.0/plenoptic/metric/classes.py` & `plenoptic-1.0.1/plenoptic/metric/classes.py`

 * *Files identical despite different names*

### Comparing `plenoptic-1.0.0/plenoptic/metric/model_metric.py` & `plenoptic-1.0.1/plenoptic/metric/model_metric.py`

 * *Files identical despite different names*

### Comparing `plenoptic-1.0.0/plenoptic/metric/naive.py` & `plenoptic-1.0.1/plenoptic/metric/naive.py`

 * *Files identical despite different names*

### Comparing `plenoptic-1.0.0/plenoptic/metric/perceptual_distance.py` & `plenoptic-1.0.1/plenoptic/metric/perceptual_distance.py`

 * *Files identical despite different names*

### Comparing `plenoptic-1.0.0/plenoptic/simulate/canonical_computations/filters.py` & `plenoptic-1.0.1/plenoptic/simulate/canonical_computations/filters.py`

 * *Files identical despite different names*

### Comparing `plenoptic-1.0.0/plenoptic/simulate/canonical_computations/laplacian_pyramid.py` & `plenoptic-1.0.1/plenoptic/simulate/canonical_computations/laplacian_pyramid.py`

 * *Files identical despite different names*

### Comparing `plenoptic-1.0.0/plenoptic/simulate/canonical_computations/non_linearities.py` & `plenoptic-1.0.1/plenoptic/simulate/canonical_computations/non_linearities.py`

 * *Files identical despite different names*

### Comparing `plenoptic-1.0.0/plenoptic/simulate/canonical_computations/steerable_pyramid_freq.py` & `plenoptic-1.0.1/plenoptic/simulate/canonical_computations/steerable_pyramid_freq.py`

 * *Files identical despite different names*

### Comparing `plenoptic-1.0.0/plenoptic/simulate/models/frontend.py` & `plenoptic-1.0.1/plenoptic/simulate/models/frontend.py`

 * *Files identical despite different names*

### Comparing `plenoptic-1.0.0/plenoptic/simulate/models/naive.py` & `plenoptic-1.0.1/plenoptic/simulate/models/naive.py`

 * *Files identical despite different names*

### Comparing `plenoptic-1.0.0/plenoptic/simulate/models/portilla_simoncelli.py` & `plenoptic-1.0.1/plenoptic/simulate/models/portilla_simoncelli.py`

 * *Files identical despite different names*

### Comparing `plenoptic-1.0.0/plenoptic/synthesize/autodiff.py` & `plenoptic-1.0.1/plenoptic/synthesize/autodiff.py`

 * *Files identical despite different names*

### Comparing `plenoptic-1.0.0/plenoptic/synthesize/eigendistortion.py` & `plenoptic-1.0.1/plenoptic/synthesize/eigendistortion.py`

 * *Files identical despite different names*

### Comparing `plenoptic-1.0.0/plenoptic/synthesize/geodesic.py` & `plenoptic-1.0.1/plenoptic/synthesize/geodesic.py`

 * *Files identical despite different names*

### Comparing `plenoptic-1.0.0/plenoptic/synthesize/mad_competition.py` & `plenoptic-1.0.1/plenoptic/synthesize/mad_competition.py`

 * *Files identical despite different names*

### Comparing `plenoptic-1.0.0/plenoptic/synthesize/metamer.py` & `plenoptic-1.0.1/plenoptic/synthesize/metamer.py`

 * *Files identical despite different names*

### Comparing `plenoptic-1.0.0/plenoptic/synthesize/simple_metamer.py` & `plenoptic-1.0.1/plenoptic/synthesize/simple_metamer.py`

 * *Files identical despite different names*

### Comparing `plenoptic-1.0.0/plenoptic/synthesize/synthesis.py` & `plenoptic-1.0.1/plenoptic/synthesize/synthesis.py`

 * *Files identical despite different names*

### Comparing `plenoptic-1.0.0/plenoptic/tools/conv.py` & `plenoptic-1.0.1/plenoptic/tools/conv.py`

 * *Files identical despite different names*

### Comparing `plenoptic-1.0.0/plenoptic/tools/convergence.py` & `plenoptic-1.0.1/plenoptic/tools/convergence.py`

 * *Files identical despite different names*

### Comparing `plenoptic-1.0.0/plenoptic/tools/data.py` & `plenoptic-1.0.1/plenoptic/tools/data.py`

 * *Files identical despite different names*

### Comparing `plenoptic-1.0.0/plenoptic/tools/display.py` & `plenoptic-1.0.1/plenoptic/tools/display.py`

 * *Files identical despite different names*

### Comparing `plenoptic-1.0.0/plenoptic/tools/external.py` & `plenoptic-1.0.1/plenoptic/tools/external.py`

 * *Files identical despite different names*

### Comparing `plenoptic-1.0.0/plenoptic/tools/optim.py` & `plenoptic-1.0.1/plenoptic/tools/optim.py`

 * *Files identical despite different names*

### Comparing `plenoptic-1.0.0/plenoptic/tools/signal.py` & `plenoptic-1.0.1/plenoptic/tools/signal.py`

 * *Files identical despite different names*

### Comparing `plenoptic-1.0.0/plenoptic/tools/stats.py` & `plenoptic-1.0.1/plenoptic/tools/stats.py`

 * *Files identical despite different names*

### Comparing `plenoptic-1.0.0/plenoptic/tools/straightness.py` & `plenoptic-1.0.1/plenoptic/tools/straightness.py`

 * *Files identical despite different names*

### Comparing `plenoptic-1.0.0/plenoptic/tools/validate.py` & `plenoptic-1.0.1/plenoptic/tools/validate.py`

 * *Files identical despite different names*

### Comparing `plenoptic-1.0.0/plenoptic.egg-info/PKG-INFO` & `plenoptic-1.0.1/plenoptic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plenoptic
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python library for model-based stimulus synthesis.
 Home-page: https://github.com/LabForComputationalVision/plenoptic
 Author: LabForComputationalVision
 License: MIT
 Keywords: Visual Information Processing,PyTorch
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.7
@@ -20,15 +20,15 @@
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/LabForComputationalVision/plenoptic/blob/main/LICENSE)
 ![Python version](https://img.shields.io/badge/python-3.7|3.8|3.9|3.10-blue.svg)
 [![Build Status](https://github.com/LabForComputationalVision/plenoptic/workflows/build/badge.svg)](https://github.com/LabForComputationalVision/plenoptic/actions?query=workflow%3Abuild)
 [![Documentation Status](https://readthedocs.org/projects/plenoptic/badge/?version=latest)](https://plenoptic.readthedocs.io/en/latest/?badge=latest)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3995057.svg)](https://doi.org/10.5281/zenodo.3995057)
 [![codecov](https://codecov.io/gh/LabForComputationalVision/plenoptic/branch/main/graph/badge.svg?token=EDtl5kqXKA)](https://codecov.io/gh/LabForComputationalVision/plenoptic)
 [![Tutorials Status](https://github.com/LabForComputationalVision/plenoptic/workflows/tutorials/badge.svg)](https://github.com/LabForComputationalVision/plenoptic/actions?query=workflow%3Atutorials)
-[![Binder](http://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/LabForComputationalVision/plenoptic/1.0.0?filepath=examples)
+[![Binder](http://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/LabForComputationalVision/plenoptic/1.0.1?filepath=examples)
 
 ![](docs/images/plenoptic_logo_wide.svg)
 
 `plenoptic` is a python library for model-based stimulus synthesis. It
 provides tools to help researchers understand their model by
 synthesizing novel informative stimuli, which help build intuition for
 what features the model ignores and what it is sensitive to. These
```

### Comparing `plenoptic-1.0.0/plenoptic.egg-info/SOURCES.txt` & `plenoptic-1.0.1/plenoptic.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 LICENSE
+MANIFEST.in
 README.md
 setup.py
+jenkins/requirements.txt
 plenoptic/__init__.py
 plenoptic/version.py
 plenoptic.egg-info/PKG-INFO
 plenoptic.egg-info/SOURCES.txt
 plenoptic.egg-info/dependency_links.txt
 plenoptic.egg-info/requires.txt
 plenoptic.egg-info/top_level.txt
```

### Comparing `plenoptic-1.0.0/setup.py` & `plenoptic-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `plenoptic-1.0.0/tests/test_display.py` & `plenoptic-1.0.1/tests/test_display.py`

 * *Files identical despite different names*

### Comparing `plenoptic-1.0.0/tests/test_eigendistortion.py` & `plenoptic-1.0.1/tests/test_eigendistortion.py`

 * *Files identical despite different names*

### Comparing `plenoptic-1.0.0/tests/test_geodesic.py` & `plenoptic-1.0.1/tests/test_geodesic.py`

 * *Files identical despite different names*

### Comparing `plenoptic-1.0.0/tests/test_mad.py` & `plenoptic-1.0.1/tests/test_mad.py`

 * *Files identical despite different names*

### Comparing `plenoptic-1.0.0/tests/test_metamers.py` & `plenoptic-1.0.1/tests/test_metamers.py`

 * *Files identical despite different names*

### Comparing `plenoptic-1.0.0/tests/test_metric.py` & `plenoptic-1.0.1/tests/test_metric.py`

 * *Files identical despite different names*

### Comparing `plenoptic-1.0.0/tests/test_models.py` & `plenoptic-1.0.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `plenoptic-1.0.0/tests/test_steerable_pyr.py` & `plenoptic-1.0.1/tests/test_steerable_pyr.py`

 * *Files identical despite different names*

### Comparing `plenoptic-1.0.0/tests/test_tools.py` & `plenoptic-1.0.1/tests/test_tools.py`

 * *Files identical despite different names*

