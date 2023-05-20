# Comparing `tmp/psyke-0.3.3.dev9.tar.gz` & `tmp/psyke-0.3.4.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psyke-0.3.3.dev9.tar", last modified: Tue Dec 13 14:44:24 2022, max compression
+gzip compressed data, was "psyke-0.3.4.dev1.tar", last modified: Sat May 20 00:30:36 2023, max compression
```

## Comparing `psyke-0.3.3.dev9.tar` & `psyke-0.3.4.dev1.tar`

### file list

```diff
@@ -1,135 +1,133 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:44:24.231766 psyke-0.3.3.dev9/
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      140 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7926 2022-12-13 14:44:24.231766 psyke-0.3.3.dev9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6843 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       10 2022-12-13 14:44:24.000000 psyke-0.3.3.dev9/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:44:24.219766 psyke-0.3.3.dev9/psyke/
--rw-r--r--   0 runner    (1001) docker     (123)    11862 2022-12-13 14:44:16.000000 psyke-0.3.3.dev9/psyke/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:44:24.219766 psyke-0.3.3.dev9/psyke/clustering/
--rw-r--r--   0 runner    (1001) docker     (123)      969 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/psyke/clustering/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:44:24.219766 psyke-0.3.3.dev9/psyke/clustering/cream/
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/psyke/clustering/cream/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:44:24.219766 psyke-0.3.3.dev9/psyke/clustering/exact/
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/psyke/clustering/exact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/psyke/clustering/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:44:24.219766 psyke-0.3.3.dev9/psyke/extraction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/psyke/extraction/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:44:24.219766 psyke-0.3.3.dev9/psyke/extraction/cart/
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/psyke/extraction/cart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/psyke/extraction/cart/predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:44:24.219766 psyke-0.3.3.dev9/psyke/extraction/hypercubic/
--rw-r--r--   0 runner    (1001) docker     (123)     5712 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/psyke/extraction/hypercubic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:44:24.219766 psyke-0.3.3.dev9/psyke/extraction/hypercubic/creepy/
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/psyke/extraction/hypercubic/creepy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:44:24.219766 psyke-0.3.3.dev9/psyke/extraction/hypercubic/gridex/
--rw-r--r--   0 runner    (1001) docker     (123)     5608 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/psyke/extraction/hypercubic/gridex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:44:24.219766 psyke-0.3.3.dev9/psyke/extraction/hypercubic/gridrex/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/psyke/extraction/hypercubic/gridrex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15111 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/psyke/extraction/hypercubic/hypercube.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:44:24.219766 psyke-0.3.3.dev9/psyke/extraction/hypercubic/iter/
--rw-r--r--   0 runner    (1001) docker     (123)    10106 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/psyke/extraction/hypercubic/iter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:44:24.219766 psyke-0.3.3.dev9/psyke/extraction/hypercubic/orchid/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/psyke/extraction/hypercubic/orchid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/psyke/extraction/hypercubic/strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/psyke/extraction/hypercubic/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:44:24.219766 psyke-0.3.3.dev9/psyke/extraction/real/
--rw-r--r--   0 runner    (1001) docker     (123)     6406 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/psyke/extraction/real/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/psyke/extraction/real/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:44:24.219766 psyke-0.3.3.dev9/psyke/extraction/trepan/
--rw-r--r--   0 runner    (1001) docker     (123)     6663 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/psyke/extraction/trepan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/psyke/extraction/trepan/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:44:24.219766 psyke-0.3.3.dev9/psyke/gui/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/psyke/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/psyke/gui/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:44:24.223766 psyke-0.3.3.dev9/psyke/gui/controller/
--rw-r--r--   0 runner    (1001) docker     (123)     5294 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/psyke/gui/controller/Controller.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/psyke/gui/controller/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:44:24.215765 psyke-0.3.3.dev9/psyke/gui/libs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:44:24.215765 psyke-0.3.3.dev9/psyke/gui/libs/garden/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:44:24.223766 psyke-0.3.3.dev9/psyke/gui/libs/garden/garden.matplotlib/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2022-12-13 14:44:16.000000 psyke-0.3.3.dev9/psyke/gui/libs/garden/garden.matplotlib/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       20 2022-12-13 14:44:16.000000 psyke-0.3.3.dev9/psyke/gui/libs/garden/garden.matplotlib/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      562 2022-12-13 14:44:16.000000 psyke-0.3.3.dev9/psyke/gui/libs/garden/garden.matplotlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50930 2022-12-13 14:44:16.000000 psyke-0.3.3.dev9/psyke/gui/libs/garden/garden.matplotlib/backend_kivy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7628 2022-12-13 14:44:16.000000 psyke-0.3.3.dev9/psyke/gui/libs/garden/garden.matplotlib/backend_kivyagg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:44:24.223766 psyke-0.3.3.dev9/psyke/gui/model/
--rw-r--r--   0 runner    (1001) docker     (123)    13743 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/psyke/gui/model/Model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/psyke/gui/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/psyke/gui/model/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:44:24.223766 psyke-0.3.3.dev9/psyke/gui/view/
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/psyke/gui/view/DataPanel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/psyke/gui/view/ExtractorPanel.py
--rw-r--r--   0 runner    (1001) docker     (123)     7478 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/psyke/gui/view/FeaturePanel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/psyke/gui/view/PlotPanel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/psyke/gui/view/PredictorPanel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/psyke/gui/view/TheoryPanel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/psyke/gui/view/View.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/psyke/gui/view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5967 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/psyke/gui/view/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)      191 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/psyke/gui/view/style.kv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:44:24.223766 psyke-0.3.3.dev9/psyke/schema/
--rw-r--r--   0 runner    (1001) docker     (123)    15760 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/psyke/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:44:24.223766 psyke-0.3.3.dev9/psyke/tuning/
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/psyke/tuning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:44:24.223766 psyke-0.3.3.dev9/psyke/tuning/crash/
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/psyke/tuning/crash/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:44:24.223766 psyke-0.3.3.dev9/psyke/tuning/pedro/
--rw-r--r--   0 runner    (1001) docker     (123)     5396 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/psyke/tuning/pedro/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:44:24.227766 psyke-0.3.3.dev9/psyke/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/psyke/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6841 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/psyke/utils/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    12284 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/psyke/utils/logic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/psyke/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/psyke/utils/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/psyke/utils/sorted.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:44:24.219766 psyke-0.3.3.dev9/psyke.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7926 2022-12-13 14:44:24.000000 psyke-0.3.3.dev9/psyke.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2022-12-13 14:44:24.000000 psyke-0.3.3.dev9/psyke.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-13 14:44:24.000000 psyke-0.3.3.dev9/psyke.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-13 14:44:23.000000 psyke-0.3.3.dev9/psyke.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      150 2022-12-13 14:44:24.000000 psyke-0.3.3.dev9/psyke.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2022-12-13 14:44:24.000000 psyke-0.3.3.dev9/psyke.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-13 14:44:24.231766 psyke-0.3.3.dev9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     9486 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:44:24.215765 psyke-0.3.3.dev9/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:44:24.227766 psyke-0.3.3.dev9/test/psyke/
--rw-r--r--   0 runner    (1001) docker     (123)     7590 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/test/psyke/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:44:24.227766 psyke-0.3.3.dev9/test/psyke/extraction/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/test/psyke/extraction/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:44:24.227766 psyke-0.3.3.dev9/test/psyke/extraction/cart/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/test/psyke/extraction/cart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/test/psyke/extraction/cart/test_cart.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/test/psyke/extraction/cart/test_simplified_cart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:44:24.227766 psyke-0.3.3.dev9/test/psyke/extraction/hypercubic/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/test/psyke/extraction/hypercubic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:44:24.227766 psyke-0.3.3.dev9/test/psyke/extraction/hypercubic/gridex/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/test/psyke/extraction/hypercubic/gridex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/test/psyke/extraction/hypercubic/gridex/test_gridex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:44:24.227766 psyke-0.3.3.dev9/test/psyke/extraction/hypercubic/iter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/test/psyke/extraction/hypercubic/iter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/test/psyke/extraction/hypercubic/iter/test_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8764 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/test/psyke/extraction/hypercubic/test_hypercube.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:44:24.227766 psyke-0.3.3.dev9/test/psyke/extraction/real/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/test/psyke/extraction/real/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/test/psyke/extraction/real/test_real.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/test/psyke/extraction/real/test_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:44:24.227766 psyke-0.3.3.dev9/test/psyke/extraction/trepan/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/test/psyke/extraction/trepan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/test/psyke/extraction/trepan/test_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/test/psyke/extraction/trepan/test_split.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/test/psyke/extraction/trepan/test_trepan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:44:24.227766 psyke-0.3.3.dev9/test/psyke/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/test/psyke/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/test/psyke/utils/test_prune.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/test/psyke/utils/test_simplify.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2022-12-13 14:42:42.000000 psyke-0.3.3.dev9/test/psyke/utils/test_simplify_formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:44:24.231766 psyke-0.3.3.dev9/test/resources/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2022-12-13 14:42:46.000000 psyke-0.3.3.dev9/test/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:44:24.231766 psyke-0.3.3.dev9/test/resources/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2022-12-13 14:42:46.000000 psyke-0.3.3.dev9/test/resources/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:44:24.231766 psyke-0.3.3.dev9/test/resources/predictors/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2022-12-13 14:42:46.000000 psyke-0.3.3.dev9/test/resources/predictors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 14:44:24.231766 psyke-0.3.3.dev9/test/resources/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2022-12-13 14:42:47.000000 psyke-0.3.3.dev9/test/resources/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:30:36.236739 psyke-0.3.4.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-05-20 00:30:36.236739 psyke-0.3.4.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-20 00:30:36.000000 psyke-0.3.4.dev1/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:30:36.224739 psyke-0.3.4.dev1/psyke/
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-20 00:30:28.000000 psyke-0.3.4.dev1/psyke/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:30:36.228740 psyke-0.3.4.dev1/psyke/clustering/
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/psyke/clustering/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:30:36.228740 psyke-0.3.4.dev1/psyke/clustering/cream/
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/psyke/clustering/cream/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:30:36.228740 psyke-0.3.4.dev1/psyke/clustering/exact/
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/psyke/clustering/exact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/psyke/clustering/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:30:36.228740 psyke-0.3.4.dev1/psyke/extraction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/psyke/extraction/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:30:36.228740 psyke-0.3.4.dev1/psyke/extraction/cart/
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/psyke/extraction/cart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/psyke/extraction/cart/predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:30:36.228740 psyke-0.3.4.dev1/psyke/extraction/hypercubic/
+-rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/psyke/extraction/hypercubic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:30:36.228740 psyke-0.3.4.dev1/psyke/extraction/hypercubic/creepy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/psyke/extraction/hypercubic/creepy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:30:36.228740 psyke-0.3.4.dev1/psyke/extraction/hypercubic/gridex/
+-rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/psyke/extraction/hypercubic/gridex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:30:36.228740 psyke-0.3.4.dev1/psyke/extraction/hypercubic/gridrex/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/psyke/extraction/hypercubic/gridrex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15111 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/psyke/extraction/hypercubic/hypercube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:30:36.228740 psyke-0.3.4.dev1/psyke/extraction/hypercubic/iter/
+-rw-r--r--   0 runner    (1001) docker     (123)    10106 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/psyke/extraction/hypercubic/iter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/psyke/extraction/hypercubic/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/psyke/extraction/hypercubic/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:30:36.228740 psyke-0.3.4.dev1/psyke/extraction/real/
+-rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/psyke/extraction/real/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/psyke/extraction/real/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:30:36.228740 psyke-0.3.4.dev1/psyke/extraction/trepan/
+-rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/psyke/extraction/trepan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/psyke/extraction/trepan/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:30:36.228740 psyke-0.3.4.dev1/psyke/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/psyke/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/psyke/gui/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:30:36.228740 psyke-0.3.4.dev1/psyke/gui/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/psyke/gui/controller/Controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/psyke/gui/controller/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:30:36.224739 psyke-0.3.4.dev1/psyke/gui/libs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:30:36.224739 psyke-0.3.4.dev1/psyke/gui/libs/garden/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:30:36.228740 psyke-0.3.4.dev1/psyke/gui/libs/garden/garden.matplotlib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-20 00:30:28.000000 psyke-0.3.4.dev1/psyke/gui/libs/garden/garden.matplotlib/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-20 00:30:28.000000 psyke-0.3.4.dev1/psyke/gui/libs/garden/garden.matplotlib/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-20 00:30:28.000000 psyke-0.3.4.dev1/psyke/gui/libs/garden/garden.matplotlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50930 2023-05-20 00:30:28.000000 psyke-0.3.4.dev1/psyke/gui/libs/garden/garden.matplotlib/backend_kivy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7628 2023-05-20 00:30:28.000000 psyke-0.3.4.dev1/psyke/gui/libs/garden/garden.matplotlib/backend_kivyagg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:30:36.232740 psyke-0.3.4.dev1/psyke/gui/model/
+-rw-r--r--   0 runner    (1001) docker     (123)    15233 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/psyke/gui/model/Model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/psyke/gui/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:30:36.232740 psyke-0.3.4.dev1/psyke/gui/view/
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/psyke/gui/view/DataPanel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/psyke/gui/view/ExtractorPanel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9408 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/psyke/gui/view/FeaturePanel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/psyke/gui/view/PlotPanel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/psyke/gui/view/PredictorPanel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/psyke/gui/view/TheoryPanel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/psyke/gui/view/View.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/psyke/gui/view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/psyke/gui/view/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/psyke/gui/view/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/psyke/gui/view/style.kv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:30:36.232740 psyke-0.3.4.dev1/psyke/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)    15760 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/psyke/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:30:36.232740 psyke-0.3.4.dev1/psyke/tuning/
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/psyke/tuning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:30:36.232740 psyke-0.3.4.dev1/psyke/tuning/crash/
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/psyke/tuning/crash/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:30:36.232740 psyke-0.3.4.dev1/psyke/tuning/pedro/
+-rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/psyke/tuning/pedro/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:30:36.232740 psyke-0.3.4.dev1/psyke/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/psyke/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/psyke/utils/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12284 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/psyke/utils/logic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/psyke/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/psyke/utils/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/psyke/utils/sorted.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:30:36.228740 psyke-0.3.4.dev1/psyke.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-05-20 00:30:36.000000 psyke-0.3.4.dev1/psyke.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-05-20 00:30:36.000000 psyke-0.3.4.dev1/psyke.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 00:30:36.000000 psyke-0.3.4.dev1/psyke.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 00:30:36.000000 psyke-0.3.4.dev1/psyke.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-20 00:30:36.000000 psyke-0.3.4.dev1/psyke.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-20 00:30:36.000000 psyke-0.3.4.dev1/psyke.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 00:30:36.236739 psyke-0.3.4.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     9486 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:30:36.224739 psyke-0.3.4.dev1/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:30:36.232740 psyke-0.3.4.dev1/test/psyke/
+-rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/test/psyke/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:30:36.232740 psyke-0.3.4.dev1/test/psyke/extraction/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/test/psyke/extraction/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:30:36.232740 psyke-0.3.4.dev1/test/psyke/extraction/cart/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/test/psyke/extraction/cart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/test/psyke/extraction/cart/test_cart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/test/psyke/extraction/cart/test_simplified_cart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:30:36.232740 psyke-0.3.4.dev1/test/psyke/extraction/hypercubic/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/test/psyke/extraction/hypercubic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:30:36.232740 psyke-0.3.4.dev1/test/psyke/extraction/hypercubic/gridex/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/test/psyke/extraction/hypercubic/gridex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/test/psyke/extraction/hypercubic/gridex/test_gridex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:30:36.236739 psyke-0.3.4.dev1/test/psyke/extraction/hypercubic/iter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/test/psyke/extraction/hypercubic/iter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/test/psyke/extraction/hypercubic/iter/test_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/test/psyke/extraction/hypercubic/test_hypercube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:30:36.236739 psyke-0.3.4.dev1/test/psyke/extraction/real/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/test/psyke/extraction/real/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/test/psyke/extraction/real/test_real.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/test/psyke/extraction/real/test_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:30:36.236739 psyke-0.3.4.dev1/test/psyke/extraction/trepan/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/test/psyke/extraction/trepan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/test/psyke/extraction/trepan/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/test/psyke/extraction/trepan/test_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/test/psyke/extraction/trepan/test_trepan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:30:36.236739 psyke-0.3.4.dev1/test/psyke/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/test/psyke/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/test/psyke/utils/test_prune.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/test/psyke/utils/test_simplify.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-20 00:29:02.000000 psyke-0.3.4.dev1/test/psyke/utils/test_simplify_formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:30:36.236739 psyke-0.3.4.dev1/test/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-20 00:29:06.000000 psyke-0.3.4.dev1/test/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:30:36.236739 psyke-0.3.4.dev1/test/resources/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-20 00:29:06.000000 psyke-0.3.4.dev1/test/resources/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:30:36.236739 psyke-0.3.4.dev1/test/resources/predictors/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-20 00:29:06.000000 psyke-0.3.4.dev1/test/resources/predictors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:30:36.236739 psyke-0.3.4.dev1/test/resources/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-20 00:29:06.000000 psyke-0.3.4.dev1/test/resources/tests/__init__.py
```

### Comparing `psyke-0.3.3.dev9/LICENSE` & `psyke-0.3.4.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `psyke-0.3.3.dev9/PKG-INFO` & `psyke-0.3.4.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psyke
-Version: 0.3.3.dev9
+Version: 0.3.4.dev1
 Summary: Python-based implementation of PSyKE, i.e. a Platform for Symbolic Knowledge Extraction
 Home-page: https://github.com/psykei/psyke-python
 Author: Matteo Magnini
 Author-email: matteo.magnini@unibo.it
 License: Apache 2.0 License
 Project-URL: Bug Reports, https://github.com/psykei/psyke-python/issues
 Project-URL: Source, https://github.com/psykei/psyke-python
```

### Comparing `psyke-0.3.3.dev9/README.md` & `psyke-0.3.4.dev1/README.md`

 * *Files identical despite different names*

### Comparing `psyke-0.3.3.dev9/psyke/__init__.py` & `psyke-0.3.4.dev1/psyke/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -189,34 +189,23 @@
         """
         Creates a new GridREx extractor.
         """
         from psyke.extraction.hypercubic.gridrex import GridREx
         return GridREx(predictor, grid, min_examples, threshold, normalization, seed)
 
     @staticmethod
-    def creepy(predictor, depth: int, error_threshold: float, output, gauss_components: int = 2,
+    def creepy(predictor, clustering, depth: int, error_threshold: float, output, gauss_components: int = 2,
                ranks: [(str, float)] = [], ignore_threshold: float = 0.0,
                normalization: dict[str, tuple[float, float]] = None) -> Extractor:
         """
         Creates a new CReEPy extractor.
         """
         from psyke.extraction.hypercubic.creepy import CReEPy
         return CReEPy(predictor, depth, error_threshold, output, gauss_components, ranks, ignore_threshold,
-                      normalization)
-
-    @staticmethod
-    def orchid(predictor, depth: int, error_threshold: float, output, gauss_components: int = 2,
-               ranks: [(str, float)] = [], ignore_threshold: float = 0.0,
-               normalization: dict[str, tuple[float, float]] = None) -> Extractor:
-        """
-        Creates a new ORCHiD extractor.
-        """
-        from psyke.extraction.hypercubic.orchid import ORCHiD
-        return ORCHiD(predictor, depth, error_threshold, output, gauss_components, ranks, ignore_threshold,
-                      normalization)
+                      normalization, clustering)
 
     @staticmethod
     def real(predictor, discretization=None) -> Extractor:
         """
         Creates a new REAL extractor.
         """
         from psyke.extraction.real import REAL
```

### Comparing `psyke-0.3.3.dev9/psyke/clustering/__init__.py` & `psyke-0.3.4.dev1/psyke/clustering/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.3.dev9/psyke/clustering/cream/__init__.py` & `psyke-0.3.4.dev1/psyke/clustering/cream/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.3.dev9/psyke/clustering/exact/__init__.py` & `psyke-0.3.4.dev1/psyke/clustering/exact/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.3.dev9/psyke/clustering/utils.py` & `psyke-0.3.4.dev1/psyke/clustering/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 def select_dbscan_epsilon(data: pd.DataFrame, clusters: int) -> float:
     neighbors = NearestNeighbors(n_neighbors=min(len(data.columns) * 2, len(data))).fit(data)
     distances = sorted(np.mean(neighbors.kneighbors(data)[1], axis=1), reverse=True)
     try:
         kn = KneeLocator([d for d in range(len(distances))], distances,
                          curve='convex', direction='decreasing', online=True)
-        if kn.knee is None:
+        if kn.knee_y is None:
             epsilon = max(distances[-1], 1e-3)
         else:
             epsilon = kn.knee_y
     except (RuntimeWarning, UserWarning, ValueError):
         epsilon = max(distances[-1], 1e-3)
     k = 1.
     dbscan_pred = DBSCAN(eps=epsilon * k).fit_predict(data.iloc[:, :-1])
```

### Comparing `psyke-0.3.3.dev9/psyke/extraction/cart/__init__.py` & `psyke-0.3.4.dev1/psyke/extraction/cart/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.3.dev9/psyke/extraction/cart/predictor.py` & `psyke-0.3.4.dev1/psyke/extraction/cart/predictor.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.3.dev9/psyke/extraction/hypercubic/__init__.py` & `psyke-0.3.4.dev1/psyke/extraction/hypercubic/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 from abc import ABC
 from typing import Iterable
 import numpy as np
 import pandas as pd
+from sklearn.base import ClassifierMixin, RegressorMixin
 from sklearn.feature_selection import SelectKBest, f_regression, f_classif
 from sklearn.linear_model import LinearRegression
 from tuprolog.core import Var, Struct, clause
 from tuprolog.theory import Theory, mutable_theory
 from psyke import Extractor, logger
 from psyke.extraction.hypercubic.hypercube import HyperCube, RegressionCube, ClassificationCube, ClosedCube
 from psyke.utils.logic import create_variable_list, create_head, to_var, Simplifier
@@ -89,19 +90,25 @@
 class FeatureRanker:
     def __init__(self, feat):
         self.scores = None
         self.feat = feat
 
     def fit(self, model, samples):
         predictions = np.array(model.predict(samples)).flatten()
-        function = f_classif if isinstance(predictions[0], str) else f_regression
+        function = f_classif if isinstance(model, ClassifierMixin) else f_regression
         best = SelectKBest(score_func=function, k="all").fit(samples, predictions)
         self.scores = np.array(best.scores_) / max(best.scores_)
         return self
 
+    def fit_on_data(self, samples):
+        function = f_classif if isinstance(samples.iloc[0, -1], str) else f_regression
+        best = SelectKBest(score_func=function, k="all").fit(samples.iloc[:, :-1], samples.iloc[:, -1])
+        self.scores = np.array(best.scores_) / max(best.scores_)
+        return self
+
     def rankings(self):
         return list(zip(self.feat, self.scores))
 
 
 class Grid:
     def __init__(self, iterations: int = 1, strategy: Strategy | list[Strategy] = FixedStrategy()):
         self.iterations = iterations
```

### Comparing `psyke-0.3.3.dev9/psyke/extraction/hypercubic/creepy/__init__.py` & `psyke-0.3.4.dev1/psyke/extraction/hypercubic/creepy/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
                  normalization=None, clustering=Extractor.exact):
         super().__init__(predictor, normalization)
         self._output = Target.CLASSIFICATION if isinstance(predictor, ClassifierMixin) else output
         self.clustering = clustering(depth, error_threshold, self._output, gauss_components)
         self.ranks = ranks
         self.ignore_threshold = ignore_threshold
 
-    def _extract(self, dataframe: pd.DataFrame, mapping: dict[str: int] = None) -> Theory:
+    def _extract(self, dataframe: pd.DataFrame, mapping: dict[str: int] = None, sort: bool = True) -> Theory:
         self._hypercubes = self.clustering.extract(dataframe)
         for cube in self._hypercubes:
             for dimension in self._ignore_dimensions():
                 cube[dimension] = [-np.inf, np.inf]
         theory = self._create_theory(dataframe)
         last_clause = list(theory.clauses)[-1]
         theory.retract(last_clause)
```

### Comparing `psyke-0.3.3.dev9/psyke/extraction/hypercubic/gridex/__init__.py` & `psyke-0.3.4.dev1/psyke/extraction/hypercubic/gridex/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.3.dev9/psyke/extraction/hypercubic/gridrex/__init__.py` & `psyke-0.3.4.dev1/psyke/extraction/hypercubic/gridrex/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.3.dev9/psyke/extraction/hypercubic/hypercube.py` & `psyke-0.3.4.dev1/psyke/extraction/hypercubic/hypercube.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.3.dev9/psyke/extraction/hypercubic/iter/__init__.py` & `psyke-0.3.4.dev1/psyke/extraction/hypercubic/iter/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.3.dev9/psyke/extraction/hypercubic/strategy.py` & `psyke-0.3.4.dev1/psyke/extraction/hypercubic/strategy.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.3.dev9/psyke/extraction/hypercubic/utils.py` & `psyke-0.3.4.dev1/psyke/extraction/hypercubic/utils.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.3.dev9/psyke/extraction/real/__init__.py` & `psyke-0.3.4.dev1/psyke/extraction/real/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.3.dev9/psyke/extraction/real/utils.py` & `psyke-0.3.4.dev1/psyke/extraction/real/utils.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.3.dev9/psyke/extraction/trepan/__init__.py` & `psyke-0.3.4.dev1/psyke/extraction/trepan/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.3.dev9/psyke/extraction/trepan/utils.py` & `psyke-0.3.4.dev1/psyke/extraction/trepan/utils.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.3.dev9/psyke/gui/__init__.py` & `psyke-0.3.4.dev1/psyke/gui/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,17 +8,18 @@
     Config.set('graphics', 'height', height)
     Config.set('graphics', 'minimum_width', '1800')
     Config.set('graphics', 'minimum_height', '950')
 
     Builder.load_file('view/style.kv')
 
     class PSyKEApp(App):
+        import os
         from psyke.gui.controller.Controller import Controller
         from psyke.gui.model.Model import Model
 
-        model = Model()
+        model = Model(os.getcwd())
         controller = Controller(model)
 
         def build(self):
             return self.controller.screen
 
     PSyKEApp().run()
```

### Comparing `psyke-0.3.3.dev9/psyke/gui/controller/Controller.py` & `psyke-0.3.4.dev1/psyke/gui/controller/Controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,17 @@
 
     def get_dataset_from_model(self):
         return self.model.dataset
 
     def get_data_from_model(self):
         return self.model.data, self.model.pruned_data, self.model.preprocessing_action, self.model.preprocessing
 
+    def get_data_rankings_from_model(self):
+        return self.model.ranked_data
+
     def get_predictor_from_model(self):
         return self.model.predictor_name, self.model.predictor, self.model.predictor_params
 
     def get_extractor_from_model(self):
         return self.model.extractor_name, self.model.extractor, self.model.extractor_params
 
     def get_test_set_from_model(self):
@@ -50,14 +53,17 @@
     def select_preprocessing(self, action, value):
         if value:
             self.model.select_preprocessing(action)
         else:
             self.model.reset_preprocessing()
         self.load_dataset()
 
+    def select_colormap(self, cmap):
+        self.model.select_colormap(cmap)
+
     def select_dataset(self, dataset):
         self.model.reset_dataset()
         self.model.select_dataset(dataset)
         self.reset_predictor()
         self.view.data_panel.disable()
         self.view.data_panel.set_info()
         self.view.feature_panel.set_info()
@@ -74,24 +80,30 @@
         self.model.reset_extractor()
         self.model.select_extractor(extractor)
         self.view.extractor_panel.set_info()
         self.view.theory_panel.set_info()
         self.view.plot_panel.clear_extractor()
 
     def reload_dataset(self, features):
-        self.model.select_features(features)
+        ret = True
+        try:
+            self.model.select_features(features)
+        except ValueError as e:
+            self.view.feature_panel.set_alert('Cannot calculate ranking for these features')
+            ret = False
         self.reset_predictor()
         self.view.data_panel.set_info()
         self.view.predictor_panel.enable()
         self.view.plot_panel.clear_data()
+        return ret
 
-    def plot(self, features, plot_features):
+    def plot(self, features, plot_features, save=False):
         inputs = [k for k, v in features.items() if v == 'I' and k in plot_features]
         output = [k for k, v in features.items() if v == 'O' and k in plot_features][0]
-        self.model.plot(inputs, output)
+        self.model.plot(inputs, output, save)
         self.view.plot_panel.set_info()
 
     def get_plots_from_model(self):
         return self.model.data_plot, self.model.predictor_plot, self.model.extractor_plot
 
     def reset_dataset(self):
         self.model.reset_dataset()
```

### Comparing `psyke-0.3.3.dev9/psyke/gui/libs/garden/garden.matplotlib/LICENSE` & `psyke-0.3.4.dev1/psyke/gui/libs/garden/garden.matplotlib/LICENSE`

 * *Files identical despite different names*

### Comparing `psyke-0.3.3.dev9/psyke/gui/libs/garden/garden.matplotlib/__init__.py` & `psyke-0.3.4.dev1/psyke/gui/libs/garden/garden.matplotlib/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.3.dev9/psyke/gui/libs/garden/garden.matplotlib/backend_kivy.py` & `psyke-0.3.4.dev1/psyke/gui/libs/garden/garden.matplotlib/backend_kivy.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.3.dev9/psyke/gui/libs/garden/garden.matplotlib/backend_kivyagg.py` & `psyke-0.3.4.dev1/psyke/gui/libs/garden/garden.matplotlib/backend_kivyagg.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.3.dev9/psyke/gui/model/Model.py` & `psyke-0.3.4.dev1/psyke/gui/model/Model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,42 @@
+import random
+
 import pandas as pd
 from matplotlib import pyplot as plt
 from sklearn.datasets import load_iris, load_wine, fetch_california_housing
 from sklearn.ensemble import RandomForestClassifier, RandomForestRegressor
 from sklearn.linear_model import LinearRegression
 from sklearn.model_selection import train_test_split
 from sklearn.neighbors import KNeighborsClassifier, KNeighborsRegressor
 from sklearn.svm import SVC, SVR
 from sklearn.tree import DecisionTreeClassifier, DecisionTreeRegressor
 
 from psyke import Extractor
 from psyke.extraction.hypercubic import Grid, FixedStrategy, FeatureRanker
-from psyke.gui.model import PREDICTORS, FIXED_PREDICTOR_PARAMS, EXTRACTORS, cast_param, DatasetError, SVMError, \
-    PredictorError
-from psyke.gui.model.plot import init_plot, plotSamples, create_grid, plot_regions
+from psyke.extraction.hypercubic.strategy import AdaptiveStrategy
+from psyke.gui.model import PREDICTORS, FIXED_PREDICTOR_PARAMS, EXTRACTORS, cast_param, DatasetError, PredictorError
+from psyke.gui.view import COLOR_MAPS
+from psyke.gui.view.plot import init_plot, plotSamples, create_grid, plot_regions
 from psyke.utils import Target
 from psyke.utils.dataframe import get_discrete_features_supervised, get_discrete_dataset, get_scaled_dataset, \
     scale_dataset
 
 
 class Model:
 
-    def __init__(self):
+    def __init__(self, path):
+        self.path = f'{path}/plots'
         self.task = 'Classification'
         self.preprocessing_action = None
         self.preprocessing = None
         self.dataset = None
         self.data = None
         self.pruned_data = None
+        self.ranked_data = None
+        self.colormap = None
         self.train = None
         self.test = None
         self.predictor_name = None
         self.predictor = None
         self.predictor_params = {}
         self.extractor_name = None
         self.extractor = None
@@ -38,18 +44,22 @@
         self.theory = None
         self.data_plot = None
         self.predictor_plot = None
         self.extractor_plot = None
 
     def select_task(self, task):
         self.task = task
+        self.colormap = None
 
     def select_preprocessing(self, action):
         self.preprocessing_action = action
 
+    def select_colormap(self, cmap):
+        self.colormap = cmap
+
     def select_dataset(self, dataset):
         self.dataset = dataset
 
     def select_predictor(self, predictor):
         self.predictor_name = predictor
 
     def select_extractor(self, extractor):
@@ -61,14 +71,15 @@
 
     def reset_dataset(self, soft=False):
         if not soft:
             self.data = None
         self.pruned_data = None
         self.train = None
         self.test = None
+        self.ranked_data = None
         self.data_plot = None
 
     def reset_predictor(self):
         self.predictor_name = None
         self.predictor = None
         self.predictor_params = {}
         self.predictor_plot = None
@@ -80,14 +91,17 @@
         self.theory = None
         self.extractor_plot = None
 
     def load_dataset(self, ret=False):
         print(f'Loading {self.dataset}... ', end='')
         if self.dataset == 'Arti':
             data = pd.read_csv('test/resources/datasets/arti.csv')
+        elif self.dataset == 'Bank marketing':
+            data = pd.read_csv('test/resources/datasets/akbilgic.csv')
+            data = data.iloc[:, [i for i in range(len(data.columns) - 7, len(data.columns))] + [1]]
         else:
             if self.dataset == 'Iris':
                 x, y = load_iris(return_X_y=True, as_frame=True)
                 x.columns = ['SepalLength', 'SepalWidth', 'PetalLength', 'PetalWidth']
                 y.name = 'iris'
                 data = (x, y.replace({0: 'setosa', 1: 'versicolor', 2: 'virginica'}))
             elif self.dataset == 'Wine':
@@ -97,14 +111,15 @@
                 data = fetch_california_housing(return_X_y=True, as_frame=True)
             else:
                 raise DatasetError
             data = data[0].join(data[1])
         print('Done')
         if ret:
             return data
+        self.ranked_data = FeatureRanker(data.columns[:-1]).fit_on_data(data).rankings()
         if self.preprocessing_action == 'Discretize':
             self.preprocessing = get_discrete_features_supervised(data)
             self.data = get_discrete_dataset(data.iloc[:, :-1], self.preprocessing, False).join(data.iloc[:, -1])
         elif self.preprocessing_action == 'Scale':
             self.data, self.preprocessing = get_scaled_dataset(data)
         else:
             self.data = data
@@ -113,14 +128,20 @@
         inputs = [k for k, v in features.items() if v == 'I']
         output = [k for k, v in features.items() if v == 'O'][0]
         if self.preprocessing_action == 'Discretize':
             inputs = [[list(discretization.admissible_values.keys()) for discretization in self.preprocessing
                        if discretization.name == variable] for variable in inputs]
             inputs = [item for sublist in inputs for item in sublist[0]]
         self.pruned_data = self.data[inputs].join(self.data[output])
+        data = self.load_dataset(True)
+        try:
+            self.ranked_data = FeatureRanker(data[inputs]).fit_on_data(data[inputs].join(data[output])).rankings()
+        except ValueError:
+            self.ranked_data = None
+            raise ValueError
 
     def train_predictor(self):
         self.read_predictor_param()
 
         print(f'Training {self.predictor_name}... ', end='')
         if self.predictor_name == 'K-NN':
             self.predictor = KNeighborsClassifier() if self.task == 'Classification' else KNeighborsRegressor()
@@ -149,15 +170,20 @@
 
     def train_extractor(self):
         def get_output():
             return Target.CONSTANT if self.extractor_params['Constant output'] else Target.REGRESSION
 
         def get_rankings():
             data = (self.data if self.pruned_data is None else self.pruned_data)
-            return FeatureRanker(data.columns[:-1]).fit(self.predictor, data.iloc[:, :-1]).rankings()
+            return FeatureRanker(data.columns[:-1]).fit_on_data(data).rankings()
+
+        def get_strategy():
+            return FixedStrategy(self.extractor_params['Splits']) if not self.extractor_params['Adaptive'] else \
+                AdaptiveStrategy(get_rankings(), [(self.extractor_params['Adaptive threshold'],
+                                                   self.extractor_params['Splits'])])
 
         # GRIDEX, GRIDREX -> strategy
         self.read_extractor_param()
 
         print(f'Training {self.extractor_name}... ', end='')
         if self.extractor_name == 'REAL':
             self.extractor = Extractor.real(self.predictor, discretization=self.preprocessing)
@@ -179,46 +205,50 @@
                                             n_points=self.extractor_params['N points'],
                                             max_iterations=self.extractor_params['Max iterations'],
                                             fill_gaps=self.extractor_params['Fill gaps'],
                                             normalization=self.preprocessing)
         elif self.extractor_name == 'GridEx':
             self.extractor = Extractor.gridex(self.predictor, threshold=self.extractor_params['Threshold'],
                                               min_examples=self.extractor_params['Min examples'],
-                                              grid=Grid(self.extractor_params['Max depth'],
-                                                        FixedStrategy(self.extractor_params['Splits'])),
+                                              grid=Grid(self.extractor_params['Max depth'], get_strategy()),
                                               normalization=self.preprocessing)
         elif self.extractor_name == 'GridREx':
             self.extractor = Extractor.gridrex(self.predictor, threshold=self.extractor_params['Threshold'],
                                                min_examples=self.extractor_params['Min examples'],
-                                               grid=Grid(self.extractor_params['Max depth'],
-                                                         FixedStrategy(self.extractor_params['Splits'])),
+                                               grid=Grid(self.extractor_params['Max depth'], get_strategy()),
                                                normalization=self.preprocessing)
         elif self.extractor_name in ['CReEPy', 'ORCHiD']:
             extractor = Extractor.creepy if self.extractor_name == 'CReEPy' else Extractor.orchid
             self.extractor = extractor(self.predictor, depth=self.extractor_params['Max depth'],
                                        error_threshold=self.extractor_params['Threshold'],
                                        ignore_threshold=self.extractor_params['Feat threshold'],
                                        gauss_components=self.extractor_params['Max components'],
-                                       output=get_output(), ranks=get_rankings(), normalization=self.preprocessing)
+                                       output=Target.CLASSIFICATION if self.task == 'Classification' else get_output(),
+                                       ranks=get_rankings(), normalization=self.preprocessing)
         else:
             raise NotImplementedError
 
         self.theory = self.extractor.extract(self.train)
         print('Done')
 
-    def plot(self, inputs, output):
+    def plot(self, inputs, output, save=False):
         x = inputs[0]
         y = inputs[1] if len(inputs) > 1 else output
         z = output if len(inputs) > 1 else None
 
+        index = 0 if self.colormap is None else \
+            [i for i, (n, _) in enumerate(COLOR_MAPS[self.task]) if n == self.colormap][0]
+        cmap = COLOR_MAPS[self.task][index][1]
+
         data = self.load_dataset(True)
         actual_data = self.data if self.pruned_data is None else self.pruned_data
 
         init_plot(data[x], data[y], 'Data set')
-        plotSamples(data[x], data[y], data[z if z is not None else y])
+        plotSamples(data[x], data[y], data[z if z is not None else y], cmap, index,
+                    f'{self.path}/data.pdf' if save else None)
         self.data_plot = plt.gcf()
         plt.close()
 
         if self.predictor is None:
             return
 
         grid = create_grid(x, y, data)
@@ -239,16 +269,17 @@
                 [grid, pd.DataFrame(predictions, columns=[actual_data.columns[-1]])], axis=1
             )
             grid_data = grid_data[grid_data.iloc[:, -1].notna()]
             grouped = grid_data.groupby([x, y])[grid_data.columns[-1]]
             outputs = grouped.agg(pd.Series.mode) if isinstance(grid_data.iloc[0, -1], str) else grouped.mean()
             grid_data = grid_data.groupby([x, y])[grid_data.columns[:-1]].mean().join(outputs)
             if z is not None:
-                plot_regions(grid_data[x].values, grid_data[y].values, grid_data[z].values)
-            plotSamples(data[x], data[y], data[z if z is not None else y])
+                plot_regions(grid_data[x].values, grid_data[y].values, grid_data[z].values, cmap)
+            plotSamples(data[x], data[y], data[z if z is not None else y], cmap, index,
+                        f'{self.path}/{name}.pdf' if save else None)
             if isinstance(model, Extractor):
                 self.extractor_plot = plt.gcf()
             else:
                 self.predictor_plot = plt.gcf()
             plt.close()
 
     def set_predictor_param(self, key, value):
```

### Comparing `psyke-0.3.3.dev9/psyke/gui/model/__init__.py` & `psyke-0.3.4.dev1/psyke/gui/model/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 TASKS = ['Classification', 'Regression']
 
 DATASETS = [
     ['Iris', [TASKS[0]]],
     ['Wine', [TASKS[0]]],
     ['Arti', [TASKS[1]]],
     ['House', [TASKS[1]]],
+    ['Bank marketing', [TASKS[1]]],
     ['Custom', TASKS]
 ]
 
 FIXED_PREDICTOR_PARAMS = {
     'Test set': (0.5, 'float', None),
     'Split seed': (0, 'int', None)
 }
@@ -54,18 +55,20 @@
 EXTRACTORS = {
     'REAL': [[TASKS[0]], {}],
     'Trepan': [[TASKS[0]], {'Max depth': MAX_DEPTH, 'Min examples': (0, 'int', None)}],
     'CART': [TASKS, {'Max depth': MAX_DEPTH, 'Max leaves': (3, 'int', None), 'Simplify': (True, 'bool', None)}],
     'Iter': [TASKS, {'Min examples': MIN_EXAMPLES, 'Threshold': THRESHOLD, 'Max iterations': (600, 'int', None),
                      'N points': (1, 'int', None), 'Min update': (0.05, 'float', None),
                      'Fill gaps': (True, 'bool', None)}],
-    'GridEx': [TASKS, {'Max depth': MAX_DEPTH, 'Splits': (1, 'int', None),
-                       'Min examples': MIN_EXAMPLES, 'Threshold': THRESHOLD}],
-    'GridREx': [[TASKS[1]], {'Max depth': MAX_DEPTH, 'Splits': (1, 'int', None),
-                             'Min examples': MIN_EXAMPLES, 'Threshold': THRESHOLD}],
+    'GridEx': [TASKS, {'Max depth': MAX_DEPTH, 'Splits': (2, 'int', None), 'Adaptive': (True, 'bool', None),
+                       'Adaptive threshold': (0.8, 'float', None), 'Min examples': MIN_EXAMPLES,
+                       'Threshold': THRESHOLD}],
+    'GridREx': [[TASKS[1]], {'Max depth': MAX_DEPTH, 'Splits': (2, 'int', None), 'Adaptive': (True, 'bool', None),
+                             'Adaptive threshold': (0.8, 'float', None), 'Min examples': MIN_EXAMPLES,
+                             'Threshold': THRESHOLD}],
     'CReEPy': [TASKS, {'Max depth': MAX_DEPTH, 'Threshold': THRESHOLD, 'Max components': (10, 'int', None),
                        'Feat threshold': (0.8, 'float', None), 'Constant output': (True, 'bool', TASKS[1])}],
     'ORCHiD': [TASKS, {'Max depth': MAX_DEPTH, 'Threshold': THRESHOLD, 'Max components': (10, 'int', None),
                        'Feat threshold': (0.8, 'float', None), 'Constant output': (True, 'bool', TASKS[1])}]
 }
```

### Comparing `psyke-0.3.3.dev9/psyke/gui/view/DataPanel.py` & `psyke-0.3.4.dev1/psyke/gui/view/DataPanel.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.3.dev9/psyke/gui/view/ExtractorPanel.py` & `psyke-0.3.4.dev1/psyke/gui/view/ExtractorPanel.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.3.dev9/psyke/gui/view/PlotPanel.py` & `psyke-0.3.4.dev1/psyke/gui/view/PlotPanel.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.3.dev9/psyke/gui/view/PredictorPanel.py` & `psyke-0.3.4.dev1/psyke/gui/view/PredictorPanel.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.3.dev9/psyke/gui/view/TheoryPanel.py` & `psyke-0.3.4.dev1/psyke/gui/view/TheoryPanel.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         self.theory_label.pos_hint = {'x': -.2, 'y': 0.}
 
     def set_info(self):
         theory = self.controller.get_theory_from_model()
         if theory is not None:
             n_rules = len(list(theory.clauses))
             theory = pretty_theory(theory)
+            print(theory)
             if n_rules > 6:
                 self.theory_label.text = THEORY_ERROR_MESSAGE['amount']
             else:
                 length = len(max(theory.split('\n'), key=len))
                 if length > 150:
                     self.theory_label.text = THEORY_ERROR_MESSAGE['length']
                 else:
```

### Comparing `psyke-0.3.3.dev9/psyke/gui/view/View.py` & `psyke-0.3.4.dev1/psyke/gui/view/View.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,16 @@
             RoundedRectangle(pos=[self.pad, self.height * self.b + self.pad],
                              size=[self.width * self.l - self.pad, self.height * self.m - self.pad])
             RoundedRectangle(pos=[self.width * self.l + self.pad, self.height * self.b + self.pad],
                              size=[self.width * self.r - self.pad * 2, self.height * self.m - self.pad])
             RoundedRectangle(pos=[self.pad, self.height * (self.b + self.m) + self.pad],
                              size=[self.width - self.pad * 2, self.height * self.t - self.pad])
             Color(1, 1, 1)
+            RoundedRectangle(pos=[self.width * (self.l + self.r / 2) - self.pad * 5, self.height * .95 - self.pad * 4],
+                             size=[self.width * self.r / 2, self.height * .05])
             for i in range(3):
                 RoundedRectangle(pos=[self.width * (self.l + self.r * i / 3) + self.pad * (2 - i),
                                       self.height * self.b + self.pad * 2],
                                  size=[(self.width * self.r - self.pad * 6) / 3, self.height * self.m - self.pad * 3])
             Line(points=[self.width * self.l * .575, 0, self.width * self.l * .575, self.height])
             Line(points=[self.width * self.l + self.pad / 2, 0, self.width * self.l + self.pad / 2, self.height])
```

### Comparing `psyke-0.3.3.dev9/psyke/gui/view/layout.py` & `psyke-0.3.4.dev1/psyke/gui/view/layout.py`

 * *Files 5% similar despite different names*

```diff
@@ -119,30 +119,38 @@
 
     def set_info(self):
         pass
 
 
 class FeatureSelectionBoxLayout(RelativeLayout):
 
-    def __init__(self, feature, role, action, plot_action, **kwargs):
+    def __init__(self, feature, role, ranking, action, plot_action, **kwargs):
         super().__init__(size_hint=(.24, 1. / 7.), **kwargs)
         self.buttons = {}
-        text = feature if len(feature) < 18 else feature[:15] + '...'
-        self.add_widget(Label(text=text, size_hint=(.7, 1.), pos_hint={'x': 0, 'y': 0}))
+        self.label = Label(size_hint=(.7, 1.), pos_hint={'x': 0, 'y': 0},
+                           halign='right', text_size=(self.width * 2, self.height * .2))
+        self.set_text(feature, ranking)
+        self.add_widget(self.label)
         for i, text in enumerate(['I', 'O']):
             button = ToggleButton(text=text, size_hint=(.1, .8), pos_hint={'x': .7 + .1 * i, 'y': .1},
                                   state='down' if role == text else 'normal', group=f'feature_{feature}')
             button.bind(on_press=action)
             self.add_widget(button)
             self.buttons[text] = button
         self.plot_button = ToggleButton(text='P', size_hint=(.1, .8), pos_hint={'x': .9, 'y': .1},
                                         state='down' if role == 'O' else 'normal')
         self.plot_button.bind(on_press=plot_action)
         self.add_widget(self.plot_button)
 
+    def set_text(self, feature, ranking):
+        text = feature if len(feature) < 16 else feature[:12] + '...'
+        if ranking is not None:
+            text += f' [{ranking:.2f}]'
+        self.label.text = text
+
 
 def create_param_layout(name: str, default: Union[str, bool, int, float], type, action, index: int, ratio: float):
     if isinstance(type, list):
         widget = SpinnerLabelCoupledRelativeLayout(name, default, type, action, index, ratio)
     elif type == 'bool':
         widget = RadioLabelCoupledRelativeLayout(f'{name}', default, action, index, ratio)
     else:
```

### Comparing `psyke-0.3.3.dev9/psyke/schema/__init__.py` & `psyke-0.3.4.dev1/psyke/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.3.dev9/psyke/tuning/__init__.py` & `psyke-0.3.4.dev1/psyke/tuning/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.3.dev9/psyke/tuning/crash/__init__.py` & `psyke-0.3.4.dev1/psyke/tuning/crash/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 from psyke import Extractor
 from psyke.tuning import Objective, Optimizer
 from psyke.utils import Target
 
 
 class CRASH(Optimizer):
     class Algorithm(Enum):
-        CReEPy = 1,
-        ORCHiD = 2
+        ExACT = 1,
+        CREAM = 2
 
     def __init__(self, predictor, dataframe: pd.DataFrame, max_mae_increase: float = 1.2,
                  min_rule_decrease: float = 0.9, readability_tradeoff: float = 0.1, max_depth: int = 10,
-                 patience: int = 5, algorithm: Algorithm = Algorithm.ORCHiD, output: Target = Target.CONSTANT,
+                 patience: int = 5, algorithm: Algorithm = Algorithm.CREAM, output: Target = Target.CONSTANT,
                  objective: Objective = Objective.MODEL, normalization=None):
         super().__init__(predictor, algorithm, dataframe, max_mae_increase, min_rule_decrease, readability_tradeoff,
                          max_depth, patience, objective, normalization)
         self.output = output
 
     def search(self):
         self.params = self.__search_depth()
@@ -46,18 +46,18 @@
     def __search_threshold(self, depth):
         step = self.model_mae / 2.0
         threshold = self.model_mae * 0.9
         params = []
         patience = self.patience
         while patience > 0:
             print(f"{self.algorithm}. Depth: {depth}. Threshold = {threshold:.2f}. ", end="")
-            extractor = Extractor.creepy(self.predictor, depth, threshold, self.output, 10,
-                                         normalization=self.normalization) if self.algorithm == CRASH.Algorithm.CReEPy \
-                else Extractor.orchid(self.predictor, depth, threshold, self.output, 10,
-                                      normalization=self.normalization)
+            extractor = Extractor.creepy(
+                self.predictor, depth, threshold, self.output, 10, normalization=self.normalization,
+                clustering=Extractor.cream if self.algorithm == CRASH.Algorithm.CREAM else Extractor.exact
+            )
             _ = extractor.extract(self.dataframe)
             mae, n = (extractor.mae(self.dataframe, self.predictor) if self.objective == Objective.MODEL else
                       extractor.mae(self.dataframe)), extractor.n_rules
             print(f"MAE = {mae:.2f}, {n} rules")
 
             if len(params) == 0:
                 params.append((mae, n, depth, threshold))
```

### Comparing `psyke-0.3.3.dev9/psyke/tuning/pedro/__init__.py` & `psyke-0.3.4.dev1/psyke/tuning/pedro/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.3.dev9/psyke/utils/__init__.py` & `psyke-0.3.4.dev1/psyke/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.3.dev9/psyke/utils/dataframe.py` & `psyke-0.3.4.dev1/psyke/utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.3.dev9/psyke/utils/logic.py` & `psyke-0.3.4.dev1/psyke/utils/logic.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.3.dev9/psyke/utils/metrics.py` & `psyke-0.3.4.dev1/psyke/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.3.dev9/psyke/utils/plot.py` & `psyke-0.3.4.dev1/psyke/utils/plot.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.3.dev9/psyke/utils/sorted.py` & `psyke-0.3.4.dev1/psyke/utils/sorted.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.3.dev9/psyke.egg-info/PKG-INFO` & `psyke-0.3.4.dev1/psyke.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psyke
-Version: 0.3.3.dev9
+Version: 0.3.4.dev1
 Summary: Python-based implementation of PSyKE, i.e. a Platform for Symbolic Knowledge Extraction
 Home-page: https://github.com/psykei/psyke-python
 Author: Matteo Magnini
 Author-email: matteo.magnini@unibo.it
 License: Apache 2.0 License
 Project-URL: Bug Reports, https://github.com/psykei/psyke-python/issues
 Project-URL: Source, https://github.com/psykei/psyke-python
```

### Comparing `psyke-0.3.3.dev9/psyke.egg-info/SOURCES.txt` & `psyke-0.3.4.dev1/psyke.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 psyke/extraction/hypercubic/hypercube.py
 psyke/extraction/hypercubic/strategy.py
 psyke/extraction/hypercubic/utils.py
 psyke/extraction/hypercubic/creepy/__init__.py
 psyke/extraction/hypercubic/gridex/__init__.py
 psyke/extraction/hypercubic/gridrex/__init__.py
 psyke/extraction/hypercubic/iter/__init__.py
-psyke/extraction/hypercubic/orchid/__init__.py
 psyke/extraction/real/__init__.py
 psyke/extraction/real/utils.py
 psyke/extraction/trepan/__init__.py
 psyke/extraction/trepan/utils.py
 psyke/gui/__init__.py
 psyke/gui/__main__.py
 psyke/gui/controller/Controller.py
@@ -38,24 +37,24 @@
 psyke/gui/libs/garden/garden.matplotlib/LICENSE
 psyke/gui/libs/garden/garden.matplotlib/README.md
 psyke/gui/libs/garden/garden.matplotlib/__init__.py
 psyke/gui/libs/garden/garden.matplotlib/backend_kivy.py
 psyke/gui/libs/garden/garden.matplotlib/backend_kivyagg.py
 psyke/gui/model/Model.py
 psyke/gui/model/__init__.py
-psyke/gui/model/plot.py
 psyke/gui/view/DataPanel.py
 psyke/gui/view/ExtractorPanel.py
 psyke/gui/view/FeaturePanel.py
 psyke/gui/view/PlotPanel.py
 psyke/gui/view/PredictorPanel.py
 psyke/gui/view/TheoryPanel.py
 psyke/gui/view/View.py
 psyke/gui/view/__init__.py
 psyke/gui/view/layout.py
+psyke/gui/view/plot.py
 psyke/gui/view/style.kv
 psyke/schema/__init__.py
 psyke/tuning/__init__.py
 psyke/tuning/crash/__init__.py
 psyke/tuning/pedro/__init__.py
 psyke/utils/__init__.py
 psyke/utils/dataframe.py
```

### Comparing `psyke-0.3.3.dev9/setup.py` & `psyke-0.3.4.dev1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,21 +15,21 @@
 # Get the long description from the README file
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 
 EPOCHS: int = 50
 BATCH_SIZE: int = 16
 REQUIREMENTS = [
-    'numpy~=1.23.2',
+    'numpy~=1.24.0',
     'pandas~=1.5.0',
     'scikit-learn~=1.2.0',
     '2ppy~=0.4.0',
     'kneed~=0.8.1',
     'kivy~=2.1.0',
-    'matplotlib~=3.6.0',
+    'matplotlib~=3.7.0',
     'kivy-garden~=0.1.5',
     'screeninfo~=0.8',
     'sympy~=1.11'
 ]  # Optional
 
 
 def format_git_describe_version(version):
```

### Comparing `psyke-0.3.3.dev9/test/psyke/__init__.py` & `psyke-0.3.4.dev1/test/psyke/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.3.dev9/test/psyke/extraction/cart/test_cart.py` & `psyke-0.3.4.dev1/test/psyke/extraction/cart/test_cart.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.3.dev9/test/psyke/extraction/cart/test_simplified_cart.py` & `psyke-0.3.4.dev1/test/psyke/extraction/cart/test_simplified_cart.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.3.dev9/test/psyke/extraction/hypercubic/gridex/test_gridex.py` & `psyke-0.3.4.dev1/test/psyke/extraction/hypercubic/gridex/test_gridex.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.3.dev9/test/psyke/extraction/hypercubic/iter/test_iter.py` & `psyke-0.3.4.dev1/test/psyke/extraction/hypercubic/iter/test_iter.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.3.dev9/test/psyke/extraction/hypercubic/test_hypercube.py` & `psyke-0.3.4.dev1/test/psyke/extraction/hypercubic/test_hypercube.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.3.dev9/test/psyke/extraction/real/test_real.py` & `psyke-0.3.4.dev1/test/psyke/extraction/real/test_real.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.3.dev9/test/psyke/extraction/real/test_rule.py` & `psyke-0.3.4.dev1/test/psyke/extraction/real/test_rule.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.3.dev9/test/psyke/extraction/trepan/test_node.py` & `psyke-0.3.4.dev1/test/psyke/extraction/trepan/test_node.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.3.dev9/test/psyke/extraction/trepan/test_split.py` & `psyke-0.3.4.dev1/test/psyke/extraction/trepan/test_split.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.3.dev9/test/psyke/extraction/trepan/test_trepan.py` & `psyke-0.3.4.dev1/test/psyke/extraction/trepan/test_trepan.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.3.dev9/test/psyke/utils/test_prune.py` & `psyke-0.3.4.dev1/test/psyke/utils/test_prune.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.3.dev9/test/psyke/utils/test_simplify.py` & `psyke-0.3.4.dev1/test/psyke/utils/test_simplify.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.3.dev9/test/psyke/utils/test_simplify_formatter.py` & `psyke-0.3.4.dev1/test/psyke/utils/test_simplify_formatter.py`

 * *Files identical despite different names*

### Comparing `psyke-0.3.3.dev9/test/resources/tests/__init__.py` & `psyke-0.3.4.dev1/test/resources/tests/__init__.py`

 * *Files identical despite different names*

