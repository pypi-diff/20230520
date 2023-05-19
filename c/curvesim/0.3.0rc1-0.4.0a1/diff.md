# Comparing `tmp/curvesim-0.3.0rc1.tar.gz` & `tmp/curvesim-0.4.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curvesim-0.3.0rc1.tar", last modified: Tue Nov 15 02:40:35 2022, max compression
+gzip compressed data, was "curvesim-0.4.0a1.tar", last modified: Fri May 19 21:56:54 2023, max compression
```

## Comparing `curvesim-0.3.0rc1.tar` & `curvesim-0.4.0a1.tar`

### file list

```diff
@@ -1,76 +1,120 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 02:40:35.797635 curvesim-0.3.0rc1/
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-11-15 02:40:20.000000 curvesim-0.3.0rc1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)     9594 2022-11-15 02:40:35.797635 curvesim-0.3.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8573 2022-11-15 02:40:20.000000 curvesim-0.3.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 02:40:35.789635 curvesim-0.3.0rc1/curvesim/
--rw-r--r--   0 runner    (1001) docker     (121)      281 2022-11-15 02:40:20.000000 curvesim-0.3.0rc1/curvesim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      427 2022-11-15 02:40:20.000000 curvesim-0.3.0rc1/curvesim/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 02:40:35.793635 curvesim-0.3.0rc1/curvesim/_bonding_curve/
--rw-r--r--   0 runner    (1001) docker     (121)     2355 2022-11-15 02:40:20.000000 curvesim-0.3.0rc1/curvesim/_bonding_curve/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 02:40:35.793635 curvesim-0.3.0rc1/curvesim/_order_book/
--rw-r--r--   0 runner    (1001) docker     (121)     4208 2022-11-15 02:40:20.000000 curvesim-0.3.0rc1/curvesim/_order_book/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 02:40:35.793635 curvesim-0.3.0rc1/curvesim/exceptions/
--rw-r--r--   0 runner    (1001) docker     (121)      361 2022-11-15 02:40:20.000000 curvesim-0.3.0rc1/curvesim/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 02:40:35.793635 curvesim-0.3.0rc1/curvesim/iterators/
--rw-r--r--   0 runner    (1001) docker     (121)      408 2022-11-15 02:40:20.000000 curvesim-0.3.0rc1/curvesim/iterators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 02:40:35.793635 curvesim-0.3.0rc1/curvesim/iterators/param_samplers/
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-11-15 02:40:20.000000 curvesim-0.3.0rc1/curvesim/iterators/param_samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3906 2022-11-15 02:40:20.000000 curvesim-0.3.0rc1/curvesim/iterators/param_samplers/grid.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 02:40:35.793635 curvesim-0.3.0rc1/curvesim/iterators/price_samplers/
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-11-15 02:40:20.000000 curvesim-0.3.0rc1/curvesim/iterators/price_samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2080 2022-11-15 02:40:20.000000 curvesim-0.3.0rc1/curvesim/iterators/price_samplers/price_volume.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 02:40:35.793635 curvesim-0.3.0rc1/curvesim/network/
--rw-r--r--   0 runner    (1001) docker     (121)      459 2022-11-15 02:40:20.000000 curvesim-0.3.0rc1/curvesim/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6157 2022-11-15 02:40:20.000000 curvesim-0.3.0rc1/curvesim/network/coingecko.py
--rw-r--r--   0 runner    (1001) docker     (121)     1032 2022-11-15 02:40:20.000000 curvesim-0.3.0rc1/curvesim/network/http.py
--rw-r--r--   0 runner    (1001) docker     (121)     2680 2022-11-15 02:40:20.000000 curvesim-0.3.0rc1/curvesim/network/llamaAPI.py
--rw-r--r--   0 runner    (1001) docker     (121)    14541 2022-11-15 02:40:20.000000 curvesim-0.3.0rc1/curvesim/network/nomics.py
--rw-r--r--   0 runner    (1001) docker     (121)     9894 2022-11-15 02:40:20.000000 curvesim-0.3.0rc1/curvesim/network/subgraph.py
--rw-r--r--   0 runner    (1001) docker     (121)     1811 2022-11-15 02:40:20.000000 curvesim-0.3.0rc1/curvesim/network/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     4046 2022-11-15 02:40:20.000000 curvesim-0.3.0rc1/curvesim/network/web3.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 02:40:35.793635 curvesim-0.3.0rc1/curvesim/overrides/
--rw-r--r--   0 runner    (1001) docker     (121)     1024 2022-11-15 02:40:20.000000 curvesim-0.3.0rc1/curvesim/overrides/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 02:40:35.793635 curvesim-0.3.0rc1/curvesim/pipelines/
--rw-r--r--   0 runner    (1001) docker     (121)      501 2022-11-15 02:40:20.000000 curvesim-0.3.0rc1/curvesim/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19783 2022-11-15 02:40:20.000000 curvesim-0.3.0rc1/curvesim/pipelines/arbitrage.py
--rw-r--r--   0 runner    (1001) docker     (121)     4051 2022-11-15 02:40:20.000000 curvesim-0.3.0rc1/curvesim/pipelines/templates.py
--rw-r--r--   0 runner    (1001) docker     (121)     2554 2022-11-15 02:40:20.000000 curvesim-0.3.0rc1/curvesim/pipelines/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 02:40:35.793635 curvesim-0.3.0rc1/curvesim/plot/
--rw-r--r--   0 runner    (1001) docker     (121)     1883 2022-11-15 02:40:20.000000 curvesim-0.3.0rc1/curvesim/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7037 2022-11-15 02:40:20.000000 curvesim-0.3.0rc1/curvesim/plot/legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 02:40:35.793635 curvesim-0.3.0rc1/curvesim/pool/
--rw-r--r--   0 runner    (1001) docker     (121)     4295 2022-11-15 02:40:20.000000 curvesim-0.3.0rc1/curvesim/pool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1370 2022-11-15 02:40:20.000000 curvesim-0.3.0rc1/curvesim/pool/base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 02:40:35.793635 curvesim-0.3.0rc1/curvesim/pool/stableswap/
--rw-r--r--   0 runner    (1001) docker     (121)      344 2022-11-15 02:40:20.000000 curvesim-0.3.0rc1/curvesim/pool/stableswap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12678 2022-11-15 02:40:20.000000 curvesim-0.3.0rc1/curvesim/pool/stableswap/functions.py
--rw-r--r--   0 runner    (1001) docker     (121)    14564 2022-11-15 02:40:20.000000 curvesim-0.3.0rc1/curvesim/pool/stableswap/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (121)    24666 2022-11-15 02:40:20.000000 curvesim-0.3.0rc1/curvesim/pool/stableswap/metapool.py
--rw-r--r--   0 runner    (1001) docker     (121)    16741 2022-11-15 02:40:20.000000 curvesim-0.3.0rc1/curvesim/pool/stableswap/pool.py
--rw-r--r--   0 runner    (1001) docker     (121)     1999 2022-11-15 02:40:20.000000 curvesim-0.3.0rc1/curvesim/pool/stableswap/raipool.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 02:40:35.793635 curvesim-0.3.0rc1/curvesim/pool_data/
--rw-r--r--   0 runner    (1001) docker     (121)     7962 2022-11-15 02:40:20.000000 curvesim-0.3.0rc1/curvesim/pool_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1009 2022-11-15 02:40:20.000000 curvesim-0.3.0rc1/curvesim/pool_data/queries.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 02:40:35.793635 curvesim-0.3.0rc1/curvesim/price_data/
--rw-r--r--   0 runner    (1001) docker     (121)     1336 2022-11-15 02:40:20.000000 curvesim-0.3.0rc1/curvesim/price_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      957 2022-11-15 02:40:20.000000 curvesim-0.3.0rc1/curvesim/price_data/sources.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 02:40:35.793635 curvesim-0.3.0rc1/curvesim/sim/
--rw-r--r--   0 runner    (1001) docker     (121)     6121 2022-11-15 02:40:20.000000 curvesim-0.3.0rc1/curvesim/sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      932 2022-11-15 02:40:20.000000 curvesim-0.3.0rc1/curvesim/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      362 2022-11-15 02:40:20.000000 curvesim-0.3.0rc1/curvesim/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 02:40:35.793635 curvesim-0.3.0rc1/curvesim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9594 2022-11-15 02:40:35.000000 curvesim-0.3.0rc1/curvesim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1561 2022-11-15 02:40:35.000000 curvesim-0.3.0rc1/curvesim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-15 02:40:35.000000 curvesim-0.3.0rc1/curvesim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      141 2022-11-15 02:40:35.000000 curvesim-0.3.0rc1/curvesim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-11-15 02:40:35.000000 curvesim-0.3.0rc1/curvesim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      170 2022-11-15 02:40:20.000000 curvesim-0.3.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1946 2022-11-15 02:40:35.797635 curvesim-0.3.0rc1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 02:40:35.789635 curvesim-0.3.0rc1/test/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 02:40:35.793635 curvesim-0.3.0rc1/test/fixtures/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-15 02:40:20.000000 curvesim-0.3.0rc1/test/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2643 2022-11-15 02:40:20.000000 curvesim-0.3.0rc1/test/fixtures/pool.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 02:40:35.797635 curvesim-0.3.0rc1/test/unit/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-15 02:40:20.000000 curvesim-0.3.0rc1/test/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12953 2022-11-15 02:40:20.000000 curvesim-0.3.0rc1/test/unit/test_metapool.py
--rw-r--r--   0 runner    (1001) docker     (121)     8628 2022-11-15 02:40:20.000000 curvesim-0.3.0rc1/test/unit/test_pool.py
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.793441 curvesim-0.4.0a1/
+-rw-r--r--   0 suh        (501) staff       (20)     1071 2022-11-09 15:51:57.000000 curvesim-0.4.0a1/LICENSE.md
+-rw-r--r--   0 suh        (501) staff       (20)     9758 2023-05-19 21:56:54.793651 curvesim-0.4.0a1/PKG-INFO
+-rw-r--r--   0 suh        (501) staff       (20)     8738 2023-05-19 21:10:12.000000 curvesim-0.4.0a1/README.md
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.736475 curvesim-0.4.0a1/curvesim/
+-rw-r--r--   0 suh        (501) staff       (20)      281 2023-03-06 16:00:39.000000 curvesim-0.4.0a1/curvesim/__init__.py
+-rw-r--r--   0 suh        (501) staff       (20)      427 2023-04-07 15:09:59.000000 curvesim-0.4.0a1/curvesim/__main__.py
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.740067 curvesim-0.4.0a1/curvesim/_bonding_curve/
+-rw-r--r--   0 suh        (501) staff       (20)     2391 2023-05-17 21:31:12.000000 curvesim-0.4.0a1/curvesim/_bonding_curve/__init__.py
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.740622 curvesim-0.4.0a1/curvesim/_order_book/
+-rw-r--r--   0 suh        (501) staff       (20)     3600 2023-01-20 15:19:10.000000 curvesim-0.4.0a1/curvesim/_order_book/__init__.py
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.741107 curvesim-0.4.0a1/curvesim/exceptions/
+-rw-r--r--   0 suh        (501) staff       (20)     1466 2023-05-19 14:49:10.000000 curvesim-0.4.0a1/curvesim/exceptions/__init__.py
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.741559 curvesim-0.4.0a1/curvesim/iterators/
+-rw-r--r--   0 suh        (501) staff       (20)      408 2022-11-12 00:31:20.000000 curvesim-0.4.0a1/curvesim/iterators/__init__.py
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.742500 curvesim-0.4.0a1/curvesim/iterators/param_samplers/
+-rw-r--r--   0 suh        (501) staff       (20)      116 2022-11-09 14:28:48.000000 curvesim-0.4.0a1/curvesim/iterators/param_samplers/__init__.py
+-rw-r--r--   0 suh        (501) staff       (20)     3358 2023-05-17 18:59:58.000000 curvesim-0.4.0a1/curvesim/iterators/param_samplers/grid.py
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.744058 curvesim-0.4.0a1/curvesim/iterators/price_samplers/
+-rw-r--r--   0 suh        (501) staff       (20)      153 2022-11-09 14:28:48.000000 curvesim-0.4.0a1/curvesim/iterators/price_samplers/__init__.py
+-rw-r--r--   0 suh        (501) staff       (20)     2620 2023-05-19 14:49:10.000000 curvesim-0.4.0a1/curvesim/iterators/price_samplers/price_volume.py
+-rw-r--r--   0 suh        (501) staff       (20)     3394 2023-05-19 14:49:10.000000 curvesim-0.4.0a1/curvesim/logging.py
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.746388 curvesim-0.4.0a1/curvesim/metrics/
+-rw-r--r--   0 suh        (501) staff       (20)     1542 2023-05-17 18:59:58.000000 curvesim-0.4.0a1/curvesim/metrics/__init__.py
+-rw-r--r--   0 suh        (501) staff       (20)    13007 2023-05-19 21:10:12.000000 curvesim-0.4.0a1/curvesim/metrics/base.py
+-rw-r--r--   0 suh        (501) staff       (20)    16984 2023-05-19 21:10:12.000000 curvesim-0.4.0a1/curvesim/metrics/metrics.py
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.748311 curvesim-0.4.0a1/curvesim/metrics/results/
+-rw-r--r--   0 suh        (501) staff       (20)      215 2023-05-19 21:10:12.000000 curvesim-0.4.0a1/curvesim/metrics/results/__init__.py
+-rw-r--r--   0 suh        (501) staff       (20)     1469 2023-05-19 21:10:12.000000 curvesim-0.4.0a1/curvesim/metrics/results/make_results.py
+-rw-r--r--   0 suh        (501) staff       (20)     3805 2023-05-19 21:10:12.000000 curvesim-0.4.0a1/curvesim/metrics/results/sim_results.py
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.751945 curvesim-0.4.0a1/curvesim/metrics/state_log/
+-rw-r--r--   0 suh        (501) staff       (20)      186 2023-05-19 21:10:12.000000 curvesim-0.4.0a1/curvesim/metrics/state_log/__init__.py
+-rw-r--r--   0 suh        (501) staff       (20)     1861 2023-05-19 21:10:12.000000 curvesim-0.4.0a1/curvesim/metrics/state_log/log.py
+-rw-r--r--   0 suh        (501) staff       (20)     1268 2023-05-19 21:10:12.000000 curvesim-0.4.0a1/curvesim/metrics/state_log/pool_parameters.py
+-rw-r--r--   0 suh        (501) staff       (20)     1034 2023-05-19 21:10:12.000000 curvesim-0.4.0a1/curvesim/metrics/state_log/pool_state.py
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.758339 curvesim-0.4.0a1/curvesim/network/
+-rw-r--r--   0 suh        (501) staff       (20)      459 2022-11-09 14:28:48.000000 curvesim-0.4.0a1/curvesim/network/__init__.py
+-rw-r--r--   0 suh        (501) staff       (20)     6157 2022-11-12 00:31:19.000000 curvesim-0.4.0a1/curvesim/network/coingecko.py
+-rw-r--r--   0 suh        (501) staff       (20)     1704 2023-04-26 15:33:34.000000 curvesim-0.4.0a1/curvesim/network/http.py
+-rw-r--r--   0 suh        (501) staff       (20)     2680 2022-11-13 23:49:59.000000 curvesim-0.4.0a1/curvesim/network/llamaAPI.py
+-rw-r--r--   0 suh        (501) staff       (20)    14800 2023-04-27 21:23:34.000000 curvesim-0.4.0a1/curvesim/network/nomics.py
+-rw-r--r--   0 suh        (501) staff       (20)    13108 2023-05-19 19:57:52.000000 curvesim-0.4.0a1/curvesim/network/subgraph.py
+-rw-r--r--   0 suh        (501) staff       (20)     1921 2023-01-20 15:19:10.000000 curvesim-0.4.0a1/curvesim/network/utils.py
+-rw-r--r--   0 suh        (501) staff       (20)     4302 2023-04-25 20:54:10.000000 curvesim-0.4.0a1/curvesim/network/web3.py
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.758942 curvesim-0.4.0a1/curvesim/overrides/
+-rw-r--r--   0 suh        (501) staff       (20)     1024 2022-11-12 00:31:19.000000 curvesim-0.4.0a1/curvesim/overrides/__init__.py
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.761248 curvesim-0.4.0a1/curvesim/pipelines/
+-rw-r--r--   0 suh        (501) staff       (20)      501 2022-11-09 14:28:48.000000 curvesim-0.4.0a1/curvesim/pipelines/__init__.py
+-rw-r--r--   0 suh        (501) staff       (20)    14384 2023-05-19 21:10:12.000000 curvesim-0.4.0a1/curvesim/pipelines/arbitrage.py
+-rw-r--r--   0 suh        (501) staff       (20)     5277 2023-05-18 18:36:37.000000 curvesim-0.4.0a1/curvesim/pipelines/templates.py
+-rw-r--r--   0 suh        (501) staff       (20)     2646 2023-05-17 21:31:12.000000 curvesim-0.4.0a1/curvesim/pipelines/utils.py
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.763148 curvesim-0.4.0a1/curvesim/plot/
+-rw-r--r--   0 suh        (501) staff       (20)      122 2023-05-19 21:10:12.000000 curvesim-0.4.0a1/curvesim/plot/__init__.py
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.766626 curvesim-0.4.0a1/curvesim/plot/altair/
+-rw-r--r--   0 suh        (501) staff       (20)      169 2023-05-19 21:10:12.000000 curvesim-0.4.0a1/curvesim/plot/altair/__init__.py
+-rw-r--r--   0 suh        (501) staff       (20)     1749 2023-05-17 18:59:58.000000 curvesim-0.4.0a1/curvesim/plot/altair/chart_properties.py
+-rw-r--r--   0 suh        (501) staff       (20)     1474 2023-05-17 18:59:58.000000 curvesim-0.4.0a1/curvesim/plot/altair/make_chart.py
+-rw-r--r--   0 suh        (501) staff       (20)     1948 2023-05-17 18:59:58.000000 curvesim-0.4.0a1/curvesim/plot/altair/selectors.py
+-rw-r--r--   0 suh        (501) staff       (20)     1001 2023-05-17 18:59:58.000000 curvesim-0.4.0a1/curvesim/plot/altair/styles.py
+-rw-r--r--   0 suh        (501) staff       (20)     2132 2023-05-19 21:10:12.000000 curvesim-0.4.0a1/curvesim/plot/result_plotter.py
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.769106 curvesim-0.4.0a1/curvesim/pool/
+-rw-r--r--   0 suh        (501) staff       (20)     6772 2023-05-19 14:49:10.000000 curvesim-0.4.0a1/curvesim/pool/__init__.py
+-rw-r--r--   0 suh        (501) staff       (20)     2552 2023-05-17 21:31:12.000000 curvesim-0.4.0a1/curvesim/pool/base.py
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.770205 curvesim-0.4.0a1/curvesim/pool/cryptoswap/
+-rw-r--r--   0 suh        (501) staff       (20)      112 2023-02-13 20:22:55.000000 curvesim-0.4.0a1/curvesim/pool/cryptoswap/__init__.py
+-rw-r--r--   0 suh        (501) staff       (20)    36552 2023-05-18 17:46:09.000000 curvesim-0.4.0a1/curvesim/pool/cryptoswap/pool.py
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.773331 curvesim-0.4.0a1/curvesim/pool/sim_interface/
+-rw-r--r--   0 suh        (501) staff       (20)      174 2023-01-20 15:19:10.000000 curvesim-0.4.0a1/curvesim/pool/sim_interface/__init__.py
+-rw-r--r--   0 suh        (501) staff       (20)     5327 2023-05-17 21:31:12.000000 curvesim-0.4.0a1/curvesim/pool/sim_interface/metapool.py
+-rw-r--r--   0 suh        (501) staff       (20)     2967 2023-05-17 21:31:12.000000 curvesim-0.4.0a1/curvesim/pool/sim_interface/pool.py
+-rw-r--r--   0 suh        (501) staff       (20)     1098 2023-01-20 15:19:10.000000 curvesim-0.4.0a1/curvesim/pool/sim_interface/raipool.py
+-rw-r--r--   0 suh        (501) staff       (20)     1787 2023-05-17 21:31:12.000000 curvesim-0.4.0a1/curvesim/pool/sim_interface/simpool.py
+-rw-r--r--   0 suh        (501) staff       (20)     4154 2023-01-20 15:19:10.000000 curvesim-0.4.0a1/curvesim/pool/snapshot.py
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.775858 curvesim-0.4.0a1/curvesim/pool/stableswap/
+-rw-r--r--   0 suh        (501) staff       (20)      267 2023-01-20 15:19:10.000000 curvesim-0.4.0a1/curvesim/pool/stableswap/__init__.py
+-rw-r--r--   0 suh        (501) staff       (20)    24771 2023-05-19 21:10:12.000000 curvesim-0.4.0a1/curvesim/pool/stableswap/metapool.py
+-rw-r--r--   0 suh        (501) staff       (20)    17204 2023-05-17 21:31:12.000000 curvesim-0.4.0a1/curvesim/pool/stableswap/pool.py
+-rw-r--r--   0 suh        (501) staff       (20)     1502 2023-01-20 15:19:10.000000 curvesim-0.4.0a1/curvesim/pool/stableswap/raipool.py
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.777854 curvesim-0.4.0a1/curvesim/pool_data/
+-rw-r--r--   0 suh        (501) staff       (20)     1574 2023-05-19 21:10:12.000000 curvesim-0.4.0a1/curvesim/pool_data/__init__.py
+-rw-r--r--   0 suh        (501) staff       (20)     4790 2023-05-19 21:10:12.000000 curvesim-0.4.0a1/curvesim/pool_data/cache.py
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.780926 curvesim-0.4.0a1/curvesim/pool_data/metadata/
+-rw-r--r--   0 suh        (501) staff       (20)     2376 2023-05-19 21:10:12.000000 curvesim-0.4.0a1/curvesim/pool_data/metadata/__init__.py
+-rw-r--r--   0 suh        (501) staff       (20)     2618 2023-05-17 21:31:12.000000 curvesim-0.4.0a1/curvesim/pool_data/metadata/base.py
+-rw-r--r--   0 suh        (501) staff       (20)     2007 2023-05-17 21:31:12.000000 curvesim-0.4.0a1/curvesim/pool_data/metadata/cryptoswap.py
+-rw-r--r--   0 suh        (501) staff       (20)     2515 2023-05-17 21:31:12.000000 curvesim-0.4.0a1/curvesim/pool_data/metadata/stableswap.py
+-rw-r--r--   0 suh        (501) staff       (20)     1287 2023-05-19 21:10:12.000000 curvesim-0.4.0a1/curvesim/pool_data/queries.py
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.782758 curvesim-0.4.0a1/curvesim/price_data/
+-rw-r--r--   0 suh        (501) staff       (20)     1382 2023-05-19 14:49:10.000000 curvesim-0.4.0a1/curvesim/price_data/__init__.py
+-rw-r--r--   0 suh        (501) staff       (20)     1586 2023-04-27 21:23:34.000000 curvesim-0.4.0a1/curvesim/price_data/sources.py
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.784405 curvesim-0.4.0a1/curvesim/sim/
+-rw-r--r--   0 suh        (501) staff       (20)     6025 2023-05-19 21:10:12.000000 curvesim-0.4.0a1/curvesim/sim/__init__.py
+-rw-r--r--   0 suh        (501) staff       (20)     3676 2023-05-19 14:49:10.000000 curvesim-0.4.0a1/curvesim/utils.py
+-rw-r--r--   0 suh        (501) staff       (20)      361 2023-05-19 21:52:52.000000 curvesim-0.4.0a1/curvesim/version.py
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.739584 curvesim-0.4.0a1/curvesim.egg-info/
+-rw-r--r--   0 suh        (501) staff       (20)     9758 2023-05-19 21:56:54.000000 curvesim-0.4.0a1/curvesim.egg-info/PKG-INFO
+-rw-r--r--   0 suh        (501) staff       (20)     2764 2023-05-19 21:56:54.000000 curvesim-0.4.0a1/curvesim.egg-info/SOURCES.txt
+-rw-r--r--   0 suh        (501) staff       (20)        1 2023-05-19 21:56:54.000000 curvesim-0.4.0a1/curvesim.egg-info/dependency_links.txt
+-rw-r--r--   0 suh        (501) staff       (20)      155 2023-05-19 21:56:54.000000 curvesim-0.4.0a1/curvesim.egg-info/requires.txt
+-rw-r--r--   0 suh        (501) staff       (20)       14 2023-05-19 21:56:54.000000 curvesim-0.4.0a1/curvesim.egg-info/top_level.txt
+-rw-r--r--   0 suh        (501) staff       (20)      170 2022-11-08 18:43:56.000000 curvesim-0.4.0a1/pyproject.toml
+-rw-r--r--   0 suh        (501) staff       (20)     1960 2023-05-19 21:56:54.796434 curvesim-0.4.0a1/setup.cfg
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.727281 curvesim-0.4.0a1/test/
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.785967 curvesim-0.4.0a1/test/fixtures/
+-rw-r--r--   0 suh        (501) staff       (20)        0 2022-10-14 18:34:20.000000 curvesim-0.4.0a1/test/fixtures/__init__.py
+-rw-r--r--   0 suh        (501) staff       (20)     5506 2023-02-13 20:22:55.000000 curvesim-0.4.0a1/test/fixtures/pool.py
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.787330 curvesim-0.4.0a1/test/integration/
+-rw-r--r--   0 suh        (501) staff       (20)        0 2023-04-27 21:23:34.000000 curvesim-0.4.0a1/test/integration/__init__.py
+-rw-r--r--   0 suh        (501) staff       (20)     1581 2023-05-17 21:31:12.000000 curvesim-0.4.0a1/test/integration/test_subgraph.py
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.788796 curvesim-0.4.0a1/test/scripts/
+-rw-r--r--   0 suh        (501) staff       (20)        0 2023-01-20 15:19:11.000000 curvesim-0.4.0a1/test/scripts/__init__.py
+-rw-r--r--   0 suh        (501) staff       (20)     4078 2023-05-17 22:06:08.000000 curvesim-0.4.0a1/test/scripts/make_test_data.py
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.793028 curvesim-0.4.0a1/test/unit/
+-rw-r--r--   0 suh        (501) staff       (20)        0 2022-10-14 18:34:20.000000 curvesim-0.4.0a1/test/unit/__init__.py
+-rw-r--r--   0 suh        (501) staff       (20)    22383 2023-05-17 21:31:12.000000 curvesim-0.4.0a1/test/unit/test_cryptopool.py
+-rw-r--r--   0 suh        (501) staff       (20)    13246 2023-02-13 20:22:55.000000 curvesim-0.4.0a1/test/unit/test_metapool.py
+-rw-r--r--   0 suh        (501) staff       (20)     8717 2023-03-02 16:07:35.000000 curvesim-0.4.0a1/test/unit/test_pool.py
+-rw-r--r--   0 suh        (501) staff       (20)    11214 2023-05-17 21:31:12.000000 curvesim-0.4.0a1/test/unit/test_pool_metadata.py
+-rw-r--r--   0 suh        (501) staff       (20)     4168 2023-05-17 18:59:58.000000 curvesim-0.4.0a1/test/unit/test_sim_stableswap.py
+-rw-r--r--   0 suh        (501) staff       (20)     3531 2023-01-20 15:19:11.000000 curvesim-0.4.0a1/test/unit/test_snapshot.py
```

### Comparing `curvesim-0.3.0rc1/LICENSE.md` & `curvesim-0.4.0a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `curvesim-0.3.0rc1/PKG-INFO` & `curvesim-0.4.0a1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,76 +1,52 @@
-Metadata-Version: 2.1
-Name: curvesim
-Version: 0.3.0rc1
-Summary: Simulate Curve pools
-Home-page: https://github.com/curveresearch/curvesim
-Author: Curve Research
-Author-email: help@curveresearch.org
-License: MIT
-Project-URL: Documentation, https://curvesim.readthedocs.io
-Project-URL: Source, https://github.com/curveresearch/curvesim
-Project-URL: Tracker, https://github.com/curveresearch/curvesim/issues
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Financial and Insurance Industry
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 [![image](https://img.shields.io/pypi/v/curvesim.svg)](https://pypi.org/project/curvesim/)
 [![image](https://img.shields.io/pypi/l/curvesim.svg)](https://pypi.org/project/curvesim/)
 [![image](https://img.shields.io/pypi/pyversions/curvesim.svg)](https://pypi.org/project/curvesim/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![CI](https://github.com/curveresearch/curvesim/actions/workflows/CI.yml/badge.svg)](https://github.com/curveresearch/curvesim/actions/workflows/CI.yml)
 [![Docs](https://readthedocs.org/projects/curvesim/badge/?version=latest)](https://curvesim.readthedocs.io/en/latest)
+![badge](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/chanhosuh/3da3c072e081f4509ebdd09c63e6ede5/raw/curvesim_coverage_badge.json)
 
 
 # Curvesim
 Curvesim simulates Curve finance pools with optimal arbitrageurs trading against them. It's primary use is to determine optimal amplitude (A) and fee parameters given historical price and volume feeds.
 
 #### Dependencies:
 The maintainers use Python 3.8 or above, but 3.11 is not yet supported.  The code is likely fine for 3.6 and 3.7 but not officially supported.
 
-Primary package dependencies: scipy, numpy, pandas, Web3, matplotlib, requests, gmpy2
+Primary package dependencies: scipy, numpy, pandas, altair, matplotlib, requests, web3, gmpy2
 
-When working on the codebase, to avoid dependency issues it is recommended to use the included `requirements.txt` file in a Python virtual environment (`venv`).
+When working on the codebase, to avoid dependency issues it is recommended to use the included `requirements.txt` file in a Python virtual environment (`venv`).  Python 3.10 is required for this.
 
 
 ## Documentation
 Check out the full documentation at https://curvesim.readthedocs.io/
 
 ## Licensing
-Portions of the codebase are authorized derivatives of code owned by Curve.fi (Swiss Stake GbmH).  These are the vyper snippets used for testing (`test/fixtures/curve`) and the python code derived from them (`curvesim/pool/stableswap`); there are copyright notices placed appropriately.  The rest of the codebase has an MIT license.
+Portions of the codebase are authorized derivatives of code owned by Curve.fi (Swiss Stake GmbH).  These are the vyper snippets used for testing (`test/fixtures/curve`) and the python code derived from them (`curvesim/pool/stableswap` and `curvesim/pool/cryptoswap`); there are copyright notices placed appropriately.  The rest of the codebase has an MIT license.
 
 ## Basic Use: Autosim
-The autosim() function simulates existing Curve pools with a range of A and/or fee parameters. The function fetches pool properties (e.g., current pool size) and 2 months of price/volume data, runs multiple simulations in parallel, and saves results plots to the "results" directory. 
+The autosim() function simulates existing Curve pools with a range of A and/or fee parameters. The function fetches pool properties (e.g., current pool size) and 2 months of price/volume data, runs multiple simulations in parallel, and returns a results object that can be introspected or generate charts.
 
 Curve pools from any chain supported by the [Convex Community Subgraphs](https://thegraph.com/hosted-service/subgraph/convex-community/volume-mainnet) can be simulated directly by inputting the pool's address or symbol. For factory pools, the pool and LP token use the same symbol. For earlier pools, we use the LP token symbol.
 
 ### Example:
-For example, to simulate 3pool with the default configuration, you could use either its address or the '3crv' LP token symbol (both are case-insensitive):
+To simulate 3pool with the default configuration:
 
 ```python
 import curvesim
 res = curvesim.autosim("0xbEbc44782C7dB0a1A60Cb6fe97d0b483032FF1C7")
-res = curvesim.autosim("3crv")
 ```
 
 To simulate pools on chains other than Ethereum, use the "chain" argument:
+
 ```python
 import curvesim
-res = curvesim.autosim("2crv", chain="arbitrum")
+# run sim on Arbitrum 2Crv
+res = curvesim.autosim("0x7f90122BF0700F9E7e1F688fe926940E8839F353", chain="arbitrum")
 ```
 
 
 ### Results:
 Plots of the results will be saved to the "results/poolname" (e.g., pools/3crv) directory. The output dictionary, "res", contains pandas dataframes for all of the data plotted in the figures:
 
 * **ar**: annualized returns
@@ -96,51 +72,50 @@
 Custom A and fee ranges can be specified using the "A" and "fee" arguments. Inputs must be lists or numpy arrays containing lists:
 
 ```python
 import curvesim
 import numpy as np
 
 #Specify A values:
-res = curvesim.autosim('3crv', A=range(1000,2001,100))
+res = curvesim.autosim('0xbEbc44782C7dB0a1A60Cb6fe97d0b483032FF1C7', A=range(1000,2001,100))
 
 #Specify fees (0.03% and 0.04% with 10 decimal precision):
-res = curvesim.autosim('3crv', fee=[3000000, 4000000])
+res = curvesim.autosim('0xbEbc44782C7dB0a1A60Cb6fe97d0b483032FF1C7', fee=[3000000, 4000000])
 
 #Specify custom A range and 0.03% fee
-#Note that single fee must still be a list
-res = curvesim.autosim('3crv', A=range(1000,2001,100), fee=3000000)
+res = curvesim.autosim('0xbEbc44782C7dB0a1A60Cb6fe97d0b483032FF1C7', A=range(1000,2001,100), fee=3000000)
 ```
 Additionally, a small number of A/fee values (2 each) can be set for testing purposes: 
 ```python
-res = curvesim.autosim('3crv', test=True)
+res = curvesim.autosim('0xbEbc44782C7dB0a1A60Cb6fe97d0b483032FF1C7', test=True)
 ```
 
 
 ### Overriding Simulation Parameters
 The following parameters are automatically specified by autosim(), but can be overridden with keyword arguments:
 * **D**: total deposit size; default: fetched from on-chain data
 * **vol_mult**: multiplied by market volume to produce trade size limits; default: computed from Curve Subraph data (see Volume Limits for details)
 * **feemul**: fee multiplier used in dynamic fee pools; default: specified in poolDF_\*.csv
 
 ```python
 import curvesim
 
 #Simulate 3pool assuming total deposit of $10B, fee = 0.03%
-res = curvesim.autosim('3crv', D=10000000000, fee=3000000)
+res = curvesim.autosim('0xbEbc44782C7dB0a1A60Cb6fe97d0b483032FF1C7', D=10000000000, fee=3000000)
 
 #For metapools, specifying D effects the deposit in the metapool, but not the basepool
 #Simulate USDN metapool assuming total deposit of $1B, fee = 0.03%
-res = curvesim.autosim('usdn3crv', D=1000000000, fee=3000000)
+res = curvesim.autosim('0x0f9cb53Ebe405d49A0bbdBD291A65Ff571bC83e1', D=1000000000, fee=3000000)
 
 #Simulate 3pool, limiting volume to 75% of market volume, fee = 0.03% 
 #Note: it is not reccomended to adjust this parameter, try vol_mode instead (see below)
-res = curvesim.autosim('3crv', vol_mult=.75, fee=3000000)
+res = curvesim.autosim('0xbEbc44782C7dB0a1A60Cb6fe97d0b483032FF1C7', vol_mult=.75, fee=3000000)
 
 #Simulate hypothetical 3pool with dynamic fee like AAVE pool, fee = 0.03% 
-res = curvesim.autosim('3crv', feemul=2*10**10, fee=3000000)
+res = curvesim.autosim('0xbEbc44782C7dB0a1A60Cb6fe97d0b483032FF1C7', feemul=2*10**10, fee=3000000)
 ```
 
 ### Volume Limits
 To approximate realistic market conditions, the "vol_mult" argument is used to limit trade volume at each timepoint in the simulation. By default (vol_mode=1), vol_mult is simply the expected proportion of market volume that goes through the Curve pool (e.g., monthly pool volume / monthly price feed volume). At each timepoint, vol_mult is multiplied by the each coin-pair's market volume to produce a volume limit for each pair, thereby appropriately scaling trade volume while retaining natural volume dynamics. For metapools, vol_mult is computed seperately for the base pool and meta-pool.
 
 In some cases, it may be helpful to limit trade volume differently. In particular, for new coins with little volume for some (but not all) pairs included in the pool, more robust simulations can be achieved by assuming equal volumes across trading pairs. We therefore provide three volume-limiting modes (vol_mode):
 
@@ -149,19 +124,18 @@
 * **vol_mode = 3**: mode 2 for trades with meta-pool asset, mode 1 for basepool-only trades
 
 We reccomend using the default vol_mode 1 in most cases. However, if that returns noisy/uninterpretable results, it may be worth trying mode 2 (for normal pools) or mode 3 (for meta-pools).
 
 ### Data Sources
 The "src" argument can be used to choose between 3 different data sources:
 * **src = "coingecko"**: CoinGecko API (free); default
-* **src = "nomics"**: Nomics API (paid); set `NOMICS_API_KEY` as env variable or in `.env` file.
 * **src = "local"**: local data stored in the "data" folder
 
-#### Note on CoinGecko vs. Nomics Data
-While Nomics provides 30-minute-interval data for each specific coin-pair, CoinGecko provides prices *per coin* in 1-hour intervals. Each coin's price is computed relative to all its trading pairs and converted to a quote currency (e.g., USD), with volume summed across all trading pairs. Therefore, market volume taken from CoinGecko is often much higher than one can expect for a specific coin-pair. This issue is largely ameloriated by our volume limiting approach, with CoinGecko results typically mirroring Nomics results qualitatively, but it should be noted that CoinGecko data may be less reliable than Nomics data for certain simulations.
+Note that Nomics data is no longer supported since they went out of service.
 
-For comparison, compare 3pool_cg and 3pool_nomics results in the pools/demo direectory.
+#### Note on CoinGecko Data
+Coingecko price/volume data is computed using all trading pairs for each coin, with volume summed across all pairs. Therefore, market volume taken from CoinGecko can be much higher than that of any specific trading pair used in a simulation. This issue is largely ameloriated by our volume limiting approach, with CoinGecko results typically mirroring results from pairwise data, but it should be noted that CoinGecko data may be less reliable than more granular data for certain simulations.
 
 ### Technical Parameters
 Additionally, one can specify:
 * **ncpu**: number of CPUs to use for parallel processing (default: all cores); for use with profilers, e.g. `cProfile`, use `ncpu=1`.
 * **days**: the number of days worth of data to use in the simulation (default: 60)
```

### Comparing `curvesim-0.3.0rc1/README.md` & `curvesim-0.4.0a1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,50 +1,78 @@
+Metadata-Version: 2.1
+Name: curvesim
+Version: 0.4.0a1
+Summary: Simulate Curve pools
+Home-page: https://github.com/curveresearch/curvesim
+Author: Curve Research
+Author-email: help@curveresearch.org
+License: MIT
+Project-URL: Documentation, https://curvesim.readthedocs.io
+Project-URL: Source, https://github.com/curveresearch/curvesim
+Project-URL: Tracker, https://github.com/curveresearch/curvesim/issues
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Financial and Insurance Industry
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
 [![image](https://img.shields.io/pypi/v/curvesim.svg)](https://pypi.org/project/curvesim/)
 [![image](https://img.shields.io/pypi/l/curvesim.svg)](https://pypi.org/project/curvesim/)
 [![image](https://img.shields.io/pypi/pyversions/curvesim.svg)](https://pypi.org/project/curvesim/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![CI](https://github.com/curveresearch/curvesim/actions/workflows/CI.yml/badge.svg)](https://github.com/curveresearch/curvesim/actions/workflows/CI.yml)
 [![Docs](https://readthedocs.org/projects/curvesim/badge/?version=latest)](https://curvesim.readthedocs.io/en/latest)
+![badge](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/chanhosuh/3da3c072e081f4509ebdd09c63e6ede5/raw/curvesim_coverage_badge.json)
 
 
 # Curvesim
 Curvesim simulates Curve finance pools with optimal arbitrageurs trading against them. It's primary use is to determine optimal amplitude (A) and fee parameters given historical price and volume feeds.
 
 #### Dependencies:
 The maintainers use Python 3.8 or above, but 3.11 is not yet supported.  The code is likely fine for 3.6 and 3.7 but not officially supported.
 
-Primary package dependencies: scipy, numpy, pandas, Web3, matplotlib, requests, gmpy2
+Primary package dependencies: scipy, numpy, pandas, altair, matplotlib, requests, web3, gmpy2
 
-When working on the codebase, to avoid dependency issues it is recommended to use the included `requirements.txt` file in a Python virtual environment (`venv`).
+When working on the codebase, to avoid dependency issues it is recommended to use the included `requirements.txt` file in a Python virtual environment (`venv`).  Python 3.10 is required for this.
 
 
 ## Documentation
 Check out the full documentation at https://curvesim.readthedocs.io/
 
 ## Licensing
-Portions of the codebase are authorized derivatives of code owned by Curve.fi (Swiss Stake GbmH).  These are the vyper snippets used for testing (`test/fixtures/curve`) and the python code derived from them (`curvesim/pool/stableswap`); there are copyright notices placed appropriately.  The rest of the codebase has an MIT license.
+Portions of the codebase are authorized derivatives of code owned by Curve.fi (Swiss Stake GmbH).  These are the vyper snippets used for testing (`test/fixtures/curve`) and the python code derived from them (`curvesim/pool/stableswap` and `curvesim/pool/cryptoswap`); there are copyright notices placed appropriately.  The rest of the codebase has an MIT license.
 
 ## Basic Use: Autosim
-The autosim() function simulates existing Curve pools with a range of A and/or fee parameters. The function fetches pool properties (e.g., current pool size) and 2 months of price/volume data, runs multiple simulations in parallel, and saves results plots to the "results" directory. 
+The autosim() function simulates existing Curve pools with a range of A and/or fee parameters. The function fetches pool properties (e.g., current pool size) and 2 months of price/volume data, runs multiple simulations in parallel, and returns a results object that can be introspected or generate charts.
 
 Curve pools from any chain supported by the [Convex Community Subgraphs](https://thegraph.com/hosted-service/subgraph/convex-community/volume-mainnet) can be simulated directly by inputting the pool's address or symbol. For factory pools, the pool and LP token use the same symbol. For earlier pools, we use the LP token symbol.
 
 ### Example:
-For example, to simulate 3pool with the default configuration, you could use either its address or the '3crv' LP token symbol (both are case-insensitive):
+To simulate 3pool with the default configuration:
 
 ```python
 import curvesim
 res = curvesim.autosim("0xbEbc44782C7dB0a1A60Cb6fe97d0b483032FF1C7")
-res = curvesim.autosim("3crv")
 ```
 
 To simulate pools on chains other than Ethereum, use the "chain" argument:
+
 ```python
 import curvesim
-res = curvesim.autosim("2crv", chain="arbitrum")
+# run sim on Arbitrum 2Crv
+res = curvesim.autosim("0x7f90122BF0700F9E7e1F688fe926940E8839F353", chain="arbitrum")
 ```
 
 
 ### Results:
 Plots of the results will be saved to the "results/poolname" (e.g., pools/3crv) directory. The output dictionary, "res", contains pandas dataframes for all of the data plotted in the figures:
 
 * **ar**: annualized returns
@@ -70,51 +98,50 @@
 Custom A and fee ranges can be specified using the "A" and "fee" arguments. Inputs must be lists or numpy arrays containing lists:
 
 ```python
 import curvesim
 import numpy as np
 
 #Specify A values:
-res = curvesim.autosim('3crv', A=range(1000,2001,100))
+res = curvesim.autosim('0xbEbc44782C7dB0a1A60Cb6fe97d0b483032FF1C7', A=range(1000,2001,100))
 
 #Specify fees (0.03% and 0.04% with 10 decimal precision):
-res = curvesim.autosim('3crv', fee=[3000000, 4000000])
+res = curvesim.autosim('0xbEbc44782C7dB0a1A60Cb6fe97d0b483032FF1C7', fee=[3000000, 4000000])
 
 #Specify custom A range and 0.03% fee
-#Note that single fee must still be a list
-res = curvesim.autosim('3crv', A=range(1000,2001,100), fee=3000000)
+res = curvesim.autosim('0xbEbc44782C7dB0a1A60Cb6fe97d0b483032FF1C7', A=range(1000,2001,100), fee=3000000)
 ```
 Additionally, a small number of A/fee values (2 each) can be set for testing purposes: 
 ```python
-res = curvesim.autosim('3crv', test=True)
+res = curvesim.autosim('0xbEbc44782C7dB0a1A60Cb6fe97d0b483032FF1C7', test=True)
 ```
 
 
 ### Overriding Simulation Parameters
 The following parameters are automatically specified by autosim(), but can be overridden with keyword arguments:
 * **D**: total deposit size; default: fetched from on-chain data
 * **vol_mult**: multiplied by market volume to produce trade size limits; default: computed from Curve Subraph data (see Volume Limits for details)
 * **feemul**: fee multiplier used in dynamic fee pools; default: specified in poolDF_\*.csv
 
 ```python
 import curvesim
 
 #Simulate 3pool assuming total deposit of $10B, fee = 0.03%
-res = curvesim.autosim('3crv', D=10000000000, fee=3000000)
+res = curvesim.autosim('0xbEbc44782C7dB0a1A60Cb6fe97d0b483032FF1C7', D=10000000000, fee=3000000)
 
 #For metapools, specifying D effects the deposit in the metapool, but not the basepool
 #Simulate USDN metapool assuming total deposit of $1B, fee = 0.03%
-res = curvesim.autosim('usdn3crv', D=1000000000, fee=3000000)
+res = curvesim.autosim('0x0f9cb53Ebe405d49A0bbdBD291A65Ff571bC83e1', D=1000000000, fee=3000000)
 
 #Simulate 3pool, limiting volume to 75% of market volume, fee = 0.03% 
 #Note: it is not reccomended to adjust this parameter, try vol_mode instead (see below)
-res = curvesim.autosim('3crv', vol_mult=.75, fee=3000000)
+res = curvesim.autosim('0xbEbc44782C7dB0a1A60Cb6fe97d0b483032FF1C7', vol_mult=.75, fee=3000000)
 
 #Simulate hypothetical 3pool with dynamic fee like AAVE pool, fee = 0.03% 
-res = curvesim.autosim('3crv', feemul=2*10**10, fee=3000000)
+res = curvesim.autosim('0xbEbc44782C7dB0a1A60Cb6fe97d0b483032FF1C7', feemul=2*10**10, fee=3000000)
 ```
 
 ### Volume Limits
 To approximate realistic market conditions, the "vol_mult" argument is used to limit trade volume at each timepoint in the simulation. By default (vol_mode=1), vol_mult is simply the expected proportion of market volume that goes through the Curve pool (e.g., monthly pool volume / monthly price feed volume). At each timepoint, vol_mult is multiplied by the each coin-pair's market volume to produce a volume limit for each pair, thereby appropriately scaling trade volume while retaining natural volume dynamics. For metapools, vol_mult is computed seperately for the base pool and meta-pool.
 
 In some cases, it may be helpful to limit trade volume differently. In particular, for new coins with little volume for some (but not all) pairs included in the pool, more robust simulations can be achieved by assuming equal volumes across trading pairs. We therefore provide three volume-limiting modes (vol_mode):
 
@@ -123,19 +150,18 @@
 * **vol_mode = 3**: mode 2 for trades with meta-pool asset, mode 1 for basepool-only trades
 
 We reccomend using the default vol_mode 1 in most cases. However, if that returns noisy/uninterpretable results, it may be worth trying mode 2 (for normal pools) or mode 3 (for meta-pools).
 
 ### Data Sources
 The "src" argument can be used to choose between 3 different data sources:
 * **src = "coingecko"**: CoinGecko API (free); default
-* **src = "nomics"**: Nomics API (paid); set `NOMICS_API_KEY` as env variable or in `.env` file.
 * **src = "local"**: local data stored in the "data" folder
 
-#### Note on CoinGecko vs. Nomics Data
-While Nomics provides 30-minute-interval data for each specific coin-pair, CoinGecko provides prices *per coin* in 1-hour intervals. Each coin's price is computed relative to all its trading pairs and converted to a quote currency (e.g., USD), with volume summed across all trading pairs. Therefore, market volume taken from CoinGecko is often much higher than one can expect for a specific coin-pair. This issue is largely ameloriated by our volume limiting approach, with CoinGecko results typically mirroring Nomics results qualitatively, but it should be noted that CoinGecko data may be less reliable than Nomics data for certain simulations.
+Note that Nomics data is no longer supported since they went out of service.
 
-For comparison, compare 3pool_cg and 3pool_nomics results in the pools/demo direectory.
+#### Note on CoinGecko Data
+Coingecko price/volume data is computed using all trading pairs for each coin, with volume summed across all pairs. Therefore, market volume taken from CoinGecko can be much higher than that of any specific trading pair used in a simulation. This issue is largely ameloriated by our volume limiting approach, with CoinGecko results typically mirroring results from pairwise data, but it should be noted that CoinGecko data may be less reliable than more granular data for certain simulations.
 
 ### Technical Parameters
 Additionally, one can specify:
 * **ncpu**: number of CPUs to use for parallel processing (default: all cores); for use with profilers, e.g. `cProfile`, use `ncpu=1`.
 * **days**: the number of days worth of data to use in the simulation (default: 60)
```

### Comparing `curvesim-0.3.0rc1/curvesim/_bonding_curve/__init__.py` & `curvesim-0.4.0a1/curvesim/_bonding_curve/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 bonding curve and current reserves.
 """
 from itertools import combinations
 
 import matplotlib.pyplot as plt
 from numpy import linspace
 
-from ..pool import CurveMetaPool
+from curvesim.pool import CurveMetaPool
 
 
-def bonding_curve(pool_obj, *, truncate=0.0005, resolution=1000, show=True):
+def bonding_curve(pool, *, truncate=0.0005, resolution=1000, show=True):
     """
     Computes and optionally plots a pool's bonding curve and current reserves.
 
     Parameters
     ----------
-    pool_obj : CurvePool or CurveMetaPool
+    pool : CurvePool or CurveMetaPool
         A pool object to compute the bonding curve for.
 
     truncate : float, default=0.0001
         Determines where to truncate the bonding curve (i.e., D*truncate).
 
     resolution : int, default=1000
         Number of points along the bonding curve to compute.
@@ -34,42 +34,43 @@
         Lists of reserves for the first coin in each combination of token pairs
 
     ys : list of lists
         Lists of reserves for the second coin in each combination of token pairs
 
     """
 
-    if isinstance(pool_obj, CurveMetaPool):
+    if isinstance(pool, CurveMetaPool):
         combos = [(0, 1)]
     else:
-        combos = list(combinations(range(pool_obj.n), 2))
+        combos = list(combinations(range(pool.n), 2))
 
     try:
-        labels = pool_obj.metadata["coins"]["names"]
+        labels = pool.metadata["coins"]["names"]
     except (AttributeError, KeyError):
-        labels = [f"Coin {str(label)}" for label in range(pool_obj.n)]
+        labels = [f"Coin {str(label)}" for label in range(pool.n)]
 
     if show:
         _, axs = plt.subplots(1, len(combos), constrained_layout=True)
 
-    D = pool_obj.D()
-    xp = pool_obj._xp()
+    D = pool.D()
+    xp = pool._xp()  # pylint: disable=protected-access
 
     xs_out = []
     ys_out = []
     for n, combo in enumerate(combos):
         i, j = combo
 
+        truncated_D = int(D * truncate)
         xs_n = linspace(
-            int(D * truncate), pool_obj.get_y(j, i, D * truncate, xp), resolution
+            truncated_D, pool.get_y(j, i, truncated_D, xp), resolution
         ).round()
 
         ys_n = []
         for x in xs_n:
-            ys_n.append(pool_obj.get_y(i, j, int(x), xp))
+            ys_n.append(pool.get_y(i, j, int(x), xp))
 
         xs_n = [x / 10**18 for x in xs_n]
         ys_n = [y / 10**18 for y in ys_n]
         xs_out.append(xs_n)
         ys_out.append(ys_n)
 
         if show:
```

### Comparing `curvesim-0.3.0rc1/curvesim/_order_book/__init__.py` & `curvesim-0.4.0a1/curvesim/_order_book/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,27 +2,25 @@
 Contains order_book function for computing and optionally plotting orderbook
 representations of exchange rates between two tokens.
 """
 
 import matplotlib.pyplot as plt
 from pandas import DataFrame
 
-from ..pool import CurveMetaPool
+from curvesim.pool import CurveMetaPool
 
 
-def order_book(
-    pool_obj, i, j, *, width=0.1, resolution=10**23, use_fee=True, show=True
-):
+def order_book(pool, i, j, *, width=0.1, resolution=10**23, use_fee=True, show=True):
     """
     Computes and optionally plots an orderbook representation of exchange rates
     between two tokens.
 
     Parameters
     ----------
-    pool_obj : CurvePool or CurveMetaPool
+    pool : CurvePool or CurveMetaPool
         A pool object to compute the bonding curve for.
 
     i : int
         The index of the "base" token to compute exchange rates for.
         To index the basepool token, use "bp_token"
 
     j : int
@@ -47,18 +45,16 @@
     bids : pandas.DataFrame
         DataFrame of prices and depths for each point on the "bid" side of the orderbook
 
     asks : pandas.DataFrame
         DataFrame of prices and depths for each point on the "ask" side of the orderbook
 
     """
-
-    is_meta = isinstance(pool_obj, CurveMetaPool)
-
-    i, j, functions, pre_trade_state = _orderbook_args(pool_obj, is_meta, i, j)
+    snapshot = pool.get_snapshot()
+    i, j, functions = _orderbook_args(pool, i, j)
     get_price, exchange = functions
 
     # Bids
     depth = 0
     price = get_price(i, j, use_fee=use_fee)
 
     bids = [(price, depth)]
@@ -68,18 +64,15 @@
 
         dy, _ = exchange(i, j, depth)
         price = get_price(i, j, use_fee=use_fee)
 
         bids.append((price, depth / 10**18))
 
         # Return to initial state
-        pool_obj.x = pre_trade_state["x0"][:]
-        if is_meta:
-            pool_obj.basepool.x = pre_trade_state["x0_base"][:]
-            pool_obj.basepool.tokens = pre_trade_state["t0_base"]
+        pool.revert_to_snapshot(snapshot)
 
     # Asks
     depth = 0
     price = get_price(j, i, use_fee=use_fee)
 
     asks = [(1 / price, depth)]
 
@@ -87,18 +80,15 @@
         depth += resolution
         dy, _ = exchange(j, i, depth)
         price = get_price(j, i, use_fee=use_fee)
 
         asks.append((1 / price, dy / 10**18))
 
         # Return to initial state
-        pool_obj.x = pre_trade_state["x0"][:]
-        if is_meta:
-            pool_obj.basepool.x = pre_trade_state["x0_base"][:]
-            pool_obj.basepool.tokens = pre_trade_state["t0_base"]
+        pool.revert_to_snapshot(snapshot)
 
     # Format DataFrames
     bids = DataFrame(bids, columns=["price", "depth"]).set_index("price")
     asks = DataFrame(asks, columns=["price", "depth"]).set_index("price")
 
     if show:
         plt.plot(bids, color="red")
@@ -106,43 +96,35 @@
         plt.xlabel("Price")
         plt.ylabel("Depth")
         plt.show()
 
     return bids, asks
 
 
-def _orderbook_args(pool_obj, is_meta, i, j):
-    if is_meta:
-
-        # Store initial state
-        pre_trade_state = {
-            "x0": pool_obj.x[:],
-            "x0_base": pool_obj.basepool.x[:],
-            "t0_base": pool_obj.basepool.tokens,
-        }
-
+def _orderbook_args(pool, i, j):
+    if isinstance(pool, CurveMetaPool):
         # Set functions/parameters
-        get_price = pool_obj.dydx
-        exchange = pool_obj.exchange_underlying
+        get_price = pool.dydx
+        exchange = pool.exchange_underlying
 
         # Price function closure if bp_token used
         def get_meta_price(i, j, use_fee):
-            xp = pool_obj._xp()
-            price = pool_obj._dydx(i, j, xp, use_fee=use_fee)
+            # pylint: disable=protected-access
+            xp = pool._xp()
+            price = pool._dydx(i, j, xp, use_fee=use_fee)
             return price
 
         if i == "bp_token":
-            i = pool_obj.max_coin
+            i = pool.max_coin
             get_price = get_meta_price
-            exchange = pool_obj.exchange
+            exchange = pool.exchange
 
         if j == "bp_token":
-            j = pool_obj.max_coin
+            j = pool.max_coin
             get_price = get_meta_price
-            exchange = pool_obj.exchange
+            exchange = pool.exchange
 
     else:
-        pre_trade_state = {"x0": pool_obj.x[:]}
-        get_price = pool_obj.dydx
-        exchange = pool_obj.exchange
+        get_price = pool.dydx
+        exchange = pool.exchange
 
-    return i, j, (get_price, exchange), pre_trade_state
+    return i, j, (get_price, exchange)
```

### Comparing `curvesim-0.3.0rc1/curvesim/iterators/param_samplers/grid.py` & `curvesim-0.4.0a1/curvesim/iterators/param_samplers/grid.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
             Basepool parameters can be included with a "basepool" key.
 
             Example
             -------
             .. code-block ::
 
-                variable_params = {"A": [100, 1000], "basepool": {fee: [10**6, 4*10**6]}}
+                {"A": [100, 1000], "basepool": {fee: [10**6, 4*10**6]}}
 
         fixed_params : dict, optional
             Pool parameters set before all simulations.
             keys: pool parameters, values: ints
 
         """
         self.pool_template = pool
@@ -52,32 +52,14 @@
 
         """
         params = next(self.param_generator)
         pool = deepcopy(self.pool_template)
         self.set_attributes(pool, params)
         return pool, params
 
-    def flat_grid(self):
-        """
-        Returns
-        -------
-        list of dicts
-            A list of the parameters used in each iteration, flattened such
-            that basepool parameters are named, e.g., A_base, fee_base, etc.
-
-        """
-        flat = self.param_grid.copy()
-        for params in flat:
-            basepool = params.pop("basepool", None)
-            if basepool:
-                for key, val in basepool.items():
-                    params.update({key + "_base": val})
-
-        return flat
-
     @staticmethod
     def param_product(p_dict):
         p_dict = p_dict.copy()
         basepool = p_dict.pop("basepool", None)
 
         keys = p_dict.keys()
         vals = p_dict.values()
@@ -106,26 +88,26 @@
             return
 
         for key, value in attribute_dict.items():
             if key == "basepool":
                 items = attribute_dict["basepool"].items()
                 for base_key, base_value in items:
                     if base_key == "D":
-                        p = pool.basepool.p[:]
+                        p = pool.basepool.rates[:]
                         n = pool.basepool.n
                         D = base_value
                         x = [D // n * 10**18 // _p for _p in p]
-                        pool.basepool.x = x
+                        pool.basepool.balances = x
 
                     else:
                         setattr(pool.basepool, base_key, base_value)
 
             else:
                 if key == "D":
-                    p = getattr(pool, "rates", pool.p[:])
+                    p = pool.rates[:]
                     n = pool.n
                     D = value
                     x = [D // n * 10**18 // _p for _p in p]
-                    pool.x = x
+                    pool.balances = x
 
                 else:
                     setattr(pool, key, value)
```

### Comparing `curvesim-0.3.0rc1/curvesim/network/coingecko.py` & `curvesim-0.4.0a1/curvesim/network/coingecko.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.3.0rc1/curvesim/network/llamaAPI.py` & `curvesim-0.4.0a1/curvesim/network/llamaAPI.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.3.0rc1/curvesim/network/nomics.py` & `curvesim-0.4.0a1/curvesim/network/nomics.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,24 +5,27 @@
 import os
 from datetime import timedelta, timezone
 from itertools import combinations
 
 import pandas as pd
 from numpy import NaN
 
+from curvesim.logging import get_logger
 from curvesim.utils import get_env_var
 
 from .http import HTTP
 from .utils import sync
 
 URL = "https://api.nomics.com/v1/"
 
 FORMAT = "%Y-%m-%dT%H:%M:%SZ"
 ETH_addr = "0xEeeeeEeeeEeEeeEeEeEeeEEEeeeeEeeeeeeeEEeE"
 
+logger = get_logger(__name__)
+
 
 def get_nomics_api_key():
     return get_env_var("NOMICS_API_KEY")
 
 
 async def get_data(url, params, t_start, t_end, exp=1):
     # Chunk times by days
@@ -164,15 +167,17 @@
     data = data.reindex(t_samples)
     data["volume"].fillna(0, inplace=True)
     data["price"].fillna(method="ffill", inplace=True)
 
     return data
 
 
-def update(coins, quote, t_start, t_end, pairs=False, data_dir="data"):  # noqa: C901
+def update(
+    coins, quote, t_start, t_end, pairs=False, data_dir="data", custom_suffix=""
+):  # noqa: C901
     t_start = t_start.replace(tzinfo=timezone.utc)
     t_start_orig = t_start
     t_end = t_end.replace(tzinfo=timezone.utc)
 
     loop = asyncio.get_event_loop()
     coins = coin_ids_from_addresses_sync(coins, event_loop=loop)
 
@@ -189,19 +194,20 @@
     # Coins prices against single quote currency
     else:
         quote = coin_ids_from_addresses_sync(quote, event_loop=loop)
         combos = [(coin, quote) for coin in coins]
 
     # Get data for each pair
     for pair in combos:
-        f_name = os.path.join(data_dir, f"{pair[0]}-{pair[1]}.csv")
+        filename = f"{pair[0]}-{pair[1]}{custom_suffix}.csv"
+        filepath = os.path.join(data_dir, filename)
         vwap_args = None
 
         try:
-            curr_file = pd.read_csv(f_name, index_col=0)
+            curr_file = pd.read_csv(filepath, index_col=0)
             curr_file.index = pd.to_datetime(curr_file.index)
 
             if t_start_orig < curr_file.index[-1]:
                 t_start = pd.to_datetime(curr_file.index[-1]) + timedelta(minutes=30)
                 t_start = t_start.replace(tzinfo=timezone.utc)
             else:
                 t_start = t_start_orig
@@ -211,32 +217,33 @@
 
         except Exception:
             curr_file = None
             vwap_args = (pair, t_start_orig, t_end)
 
         # Save if any new data
         if vwap_args is not None:
-            print(f"Downloading {pair[0]}-{pair[1]}")
+            logger.info(f"Downloading {pair[0]}-{pair[1]}")
             data = vwap_agg_sync(*vwap_args)
             if curr_file is not None:
                 data = pd.concat([curr_file, data])
             data = data[data.index >= t_start_orig]
             os.makedirs(data_dir, exist_ok=True)
-            data.to_csv(f_name)
+            data.to_csv(filepath)
 
 
 def pool_prices(  # noqa: C901
     coins=None,
     quote=None,
     quotediv=False,
     t_start=None,
     t_end=None,
     resample=None,
     pairs=None,
     data_dir="data",
+    custom_suffix="",
 ):
     """
     Loads and formats price/volume data from CSVs.
 
     Parameters
     ----------
     coins: list of str
@@ -287,25 +294,25 @@
             quote = coin_ids_from_addresses_sync(quote, event_loop=loop)
             symbol_pairs = zip(coins, [quote] * len(coins))
 
         else:
             symbol_pairs = list(combinations(coins, 2))
 
     elif pairs:
-        pairs = coin_ids_from_addresses_sync(pairs, event_loop=loop)
-        symbol_pairs = pairs
+        symbol_pairs = coin_ids_from_addresses_sync(pairs, event_loop=loop)
 
     else:
         raise ValueError("Must use one of 'coins' or 'pairs'.")
 
     prices = []
     volumes = []
     for (sym_1, sym_2) in symbol_pairs:
-        filename = os.path.join(data_dir, f"{sym_1}-{sym_2}.csv")
-        data_df = pd.read_csv(filename, index_col=0)
+        filename = f"{sym_1}-{sym_2}{custom_suffix}.csv"
+        filepath = os.path.join(data_dir, filename)
+        data_df = pd.read_csv(filepath, index_col=0)
         prices.append(data_df["price"])
         volumes.append(data_df["volume"])
 
     prices = pd.concat(prices, axis=1)
     volumes = pd.concat(volumes, axis=1)
 
     pzero = (volumes == 0).mean()
@@ -363,14 +370,15 @@
     quote=None,
     quotediv=False,
     t_start=None,
     t_end=None,
     resample=None,
     pairs=None,
     data_dir="data",
+    custom_suffix="",
 ):
     """
     Loads and formats price/volume data from CSVs.
 
     Parameters
     ----------
     coins: list of str
@@ -421,16 +429,17 @@
         symbol_pairs = pairs
     else:
         raise ValueError("Must use one of 'coins' or 'pairs'.")
 
     prices = []
     volumes = []
     for (sym_1, sym_2) in symbol_pairs:
-        filename = os.path.join(data_dir, f"{sym_1}-{sym_2}.csv")
-        data_df = pd.read_csv(filename, index_col=0)
+        filename = f"{sym_1}-{sym_2}{custom_suffix}.csv"
+        filepath = os.path.join(data_dir, filename)
+        data_df = pd.read_csv(filepath, index_col=0)
         prices.append(data_df["price"])
         volumes.append(data_df["volume"])
 
     prices = pd.concat(prices, axis=1)
     volumes = pd.concat(volumes, axis=1)
 
     pzero = (prices == 0).mean()
@@ -466,15 +475,15 @@
     # Trim to t_start and/or t_end
     if t_start is not None:
         prices = prices.loc[t_start:]
         volumes = volumes.loc[t_start:]
 
     if t_end is not None:
         prices = prices.loc[:t_end]
-        volumes = prices.loc[:t_end]
+        volumes = volumes.loc[:t_end]
 
     # Resample times
     if resample is not None:
         prices = prices.resample(resample).first()
         volumes = volumes.resample(resample).sum()
     else:
         prices.index.freq = pd.infer_freq(prices.index)
```

### Comparing `curvesim-0.3.0rc1/curvesim/network/subgraph.py` & `curvesim-0.4.0a1/curvesim/network/subgraph.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,19 +4,25 @@
 
 from asyncio import gather
 from datetime import datetime, timedelta, timezone
 
 import pandas as pd
 from eth_utils import to_checksum_address
 
+from curvesim.logging import get_logger
+
 from ..exceptions import SubgraphResultError
 from ..overrides import override_subgraph_data
 from .http import HTTP
 from .utils import compute_D, sync
 
+# pylint: disable=redefined-outer-name
+
+logger = get_logger(__name__)
+
 
 async def query(url, q):
     """
     Core async function to query subgraphs.
 
     Parameters
     ----------
@@ -63,15 +69,19 @@
     -------
     str
         The returned results.
 
     """
     url = CONVEX_COMMUNITY_URL % chain
     r = await query(url, q)
-    return r
+    if "data" not in r:
+        raise SubgraphResultError(
+            f"No data returned from Convex: chain: {chain}, query: {q}"
+        )
+    return r["data"]
 
 
 async def symbol_address(symbol, chain):
     """
     Async function to get a pool's address from it's (LP token) symbol.
 
     Parameters
@@ -110,69 +120,77 @@
             address
           }
         }
     """
         % symbol
     )
 
-    r = await convex(chain, q)
+    data = await convex(chain, q)
 
-    if len(r["data"]["pools"]) > 1:
+    if len(data["pools"]) > 1:
         pool_list = "\n\n"
-        for pool in r["data"]["pools"]:
+        for pool in data["pools"]:
             pool_list += f"\"{pool['symbol']}\": {pool['address']}\n"
 
         raise SubgraphResultError(
             "Multiple pools returned for symbol query:" + pool_list
         )
+    if len(data["pools"]) < 1:
+        raise SubgraphResultError("No pools found for symbol query.")
 
-    addr = to_checksum_address(r["data"]["pools"][0]["address"])
+    addr = to_checksum_address(data["pools"][0]["address"])
 
     return addr
 
 
-async def _volume(address, chain, days=60):
-    t_end = datetime.utcnow().replace(hour=0, minute=0, second=0, microsecond=0)
+async def _volume(address, chain, days=60, end=None):
+    if end is None:
+        t_end = datetime.now(timezone.utc).replace(
+            hour=0, minute=0, second=0, microsecond=0
+        )
+    else:
+        t_end = datetime.fromtimestamp(end, tz=timezone.utc)
+    logger.info(f"Volume end date: {t_end}")
     t_start = t_end - timedelta(days=days)
 
     q = """
         {
           swapVolumeSnapshots(
             orderBy: timestamp,
             orderDirection: desc,
             where:
               {
                 pool: "%s"
                 period: "86400"
                 timestamp_gte: %d
-                timestamp_lte: %d
+                timestamp_lt: %d
               }
           )
           {
             volume
             timestamp
           }
         }
     """ % (
         address.lower(),
         int(t_start.timestamp()),
         int(t_end.timestamp()),
     )
 
-    r = await convex(chain, q)
-    r = r["data"]["swapVolumeSnapshots"]
-    r_length = len(r)
+    data = await convex(chain, q)
+    snapshots = data["swapVolumeSnapshots"]
+    num_snapshots = len(snapshots)
 
-    if r_length < days:
-        print(f"Warning: only {r_length}/{days} days of pool volume returned")
+    if num_snapshots < days:
+        logger.warning(f"Only {num_snapshots}/{days} days of pool volume returned.")
 
-    return r
+    return snapshots
 
 
-async def volume(addresses, chain, days=60):
+async def volume(addresses, chain, days=60, end=None):
     """
     Retrieves historical volume for a pool or multiple pools.
 
     Parameters
     ----------
     addresses : str or iterable of str
         The pool address(es).
@@ -186,21 +204,21 @@
     Returns
     -------
     list of float
         A list of total volumes for each day.
 
     """
     if isinstance(addresses, str):
-        r = await _volume(addresses, chain, days=days)
+        r = await _volume(addresses, chain, days=days, end=end)
         vol = [float(e["volume"]) for e in r]
 
     else:
         tasks = []
         for addr in addresses:
-            tasks.append(_volume(addr, chain, days=days))
+            tasks.append(_volume(addr, chain, days=days, end=end))
 
         r = await gather(*tasks)
 
         vol = []
         for _r in r:
             _vol = [float(e["volume"]) for e in _r]
             vol.append(_vol)
@@ -226,32 +244,54 @@
               name
               address
               symbol
               metapool
               basePool
               coins
               coinNames
+              coinDecimals
               poolType
               isV2
             }
 
             A
             fee
+            adminFee
             offPegFeeMultiplier
+            reserves
             normalizedReserves
             virtualPrice
             timestamp
+
+            gamma
+            midFee
+            outFee
+            feeGamma
+            allowedExtraProfit
+            adjustmentStep
+            maHalfTime
+            priceScale
+            priceOracle
+            lastPrices
+            lastPricesTimestamp
+            xcpProfit
+            xcpProfitA
           }
         }
     """
         % address.lower()
     )
 
     r = await convex(chain, q)
-    r = r["data"]["dailyPoolSnapshots"][0]
+    try:
+        r = r["dailyPoolSnapshots"][0]
+    except IndexError:
+        raise SubgraphResultError(
+            f"No daily snapshot for this pool: {address}, {chain}"
+        )
 
     return r
 
 
 async def pool_snapshot(address, chain):
     """
     Async function to pull pool state and metadata from daily snapshots.
@@ -288,79 +328,112 @@
     # Fee_mul
     if r["offPegFeeMultiplier"] == "0":
         fee_mul = None
     else:
         fee_mul = int(r["offPegFeeMultiplier"]) * 10**10
 
     # Coins
+    names = r["coinNames"]
     addrs = [to_checksum_address(c) for c in r["coins"]]
+    decimals = [int(d) for d in r["coinDecimals"]]
 
-    coins = {"names": r["coinNames"], "addresses": addrs}
+    coins = {"names": names, "addresses": addrs, "decimals": decimals}
 
     # Reserves
-    reserves = [int(nr) for nr in r["normalizedReserves"]]
+    normalized_reserves = [int(r) for r in r["normalizedReserves"]]
+    unnormalized_reserves = [int(r) for r in r["reserves"]]
 
     # Basepool
     if r["metapool"]:
         basepool = await pool_snapshot(r["basePool"], chain)
     else:
         basepool = None
 
     # Output
-    data = {
-        "name": r["name"],
-        "address": to_checksum_address(r["address"]),
-        "chain": chain,
-        "symbol": r["symbol"].strip(),
-        "version": version,
-        "pool_type": r["poolType"],
-        "params": {
-            "A": int(r["A"]),
-            "fee": int(float(r["fee"]) * 10**10),
-            "fee_mul": fee_mul,
-        },
-        "coins": coins,
-        "reserves": {
-            "D": D,
-            "by_coin": reserves,
-            "virtual_price": int(r["virtualPrice"]),
-            "tokens": D * 10**18 // int(r["virtualPrice"]),
-        },
-        "basepool": basepool,
-        "timestamp": int(r["timestamp"]),
-    }
-
-    # Kwargs for Pool Init
-    init_kwargs = {
-        "A": data["params"]["A"],
-        "D": D,
-        "reserves": reserves,
-        "n": len(data["coins"]["names"]),
-        "fee": data["params"]["fee"],
-        "fee_mul": data["params"]["fee_mul"],
-        "tokens": data["reserves"]["tokens"],
-    }
-
-    data.update({"init_kwargs": init_kwargs})
+    if version == 1:
+        data = {
+            "name": r["name"],
+            "address": to_checksum_address(r["address"]),
+            "chain": chain,
+            "symbol": r["symbol"].strip(),
+            "version": version,
+            "pool_type": r["poolType"],
+            "params": {
+                "A": int(r["A"]),
+                "fee": int(float(r["fee"]) * 10**10),
+                "fee_mul": fee_mul,
+                "admin_fee": int(r["adminFee"]),
+            },
+            "coins": coins,
+            "reserves": {
+                "D": D,
+                "by_coin": normalized_reserves,
+                "unnormalized_by_coin": unnormalized_reserves,
+                "virtual_price": int(r["virtualPrice"]),
+                "tokens": D * 10**18 // int(r["virtualPrice"]),
+            },
+            "basepool": basepool,
+            "timestamp": int(r["timestamp"]),
+        }
+    else:
+        data = {
+            "name": r["name"],
+            "address": to_checksum_address(r["address"]),
+            "chain": chain,
+            "symbol": r["symbol"].strip(),
+            "version": version,
+            "pool_type": r["poolType"],
+            "params": {
+                "A": int(r["A"]),
+                "gamma": int(r["gamma"]),
+                "fee_gamma": int(r["feeGamma"]),
+                "mid_fee": int(r["midFee"]),
+                "out_fee": int(r["outFee"]),
+                "allowed_extra_profit": int(r["allowedExtraProfit"]),
+                "adjustment_step": int(r["adjustmentStep"]),
+                "ma_half_time": int(r["adjustmentStep"]),
+                "price_scale": int(r["priceScale"]),
+                "price_oracle": int(r["priceOracle"]),
+                "last_prices": int(r["lastPrices"]),
+                "last_prices_timestamp": int(r["lastPricesTimestamp"]),
+                "admin_fee": int(r["adminFee"]),
+                "xcp_profit": int(r["xcpProfit"]),
+                "xcp_profit_a": int(r["xcpProfitA"]),
+            },
+            "coins": coins,
+            "reserves": {
+                "D": D,
+                "by_coin": normalized_reserves,
+                "unnormalized_by_coin": unnormalized_reserves,
+                "virtual_price": int(r["virtualPrice"]),
+                "tokens": D * 10**18 // int(r["virtualPrice"]),
+            },
+            "basepool": basepool,
+            "timestamp": int(r["timestamp"]),
+        }
 
     return override_subgraph_data(data, "pool_snapshot", (address, chain))
 
 
 convex_sync = sync(convex)
 symbol_address_sync = sync(symbol_address)
 volume_sync = sync(volume)
 pool_snapshot_sync = sync(pool_snapshot)
 
 
 # Reflexer Subgraph
 RAI_ADDR = ("0x618788357D0EBd8A37e763ADab3bc575D54c2C7d", "mainnet")
 
 
+def has_redemption_prices(address, chain):
+    return (address, chain) == RAI_ADDR
+
+
 async def _redemption_prices(address, chain, t_start, t_end, n):
-    if (address, chain) != RAI_ADDR:
+    if not has_redemption_prices(address, chain):
         return None
 
     t_end = int(t_end.timestamp())
     t_start = int(t_start.timestamp())
 
     url = "https://api.thegraph.com/subgraphs/name/reflexer-labs/rai-mainnet"
     q = """{
@@ -381,15 +454,17 @@
     while t_earliest >= t_start:
         r = await query(url, q % (n, t_earliest))
         data += r["data"]["redemptionPrices"]
         t_earliest = int(data[-1]["timestamp"])
     return data
 
 
-async def redemption_prices(address=RAI_ADDR[0], chain=RAI_ADDR[1], days=60, n=1000):
+async def redemption_prices(
+    address=RAI_ADDR[0], chain=RAI_ADDR[1], days=60, n=1000, end=None
+):
     """
     Async function to pull RAI redemption prices.
     Returns None if input pool is not RAI3CRV.
 
     Parameters
     ----------
     address : str
@@ -409,16 +484,20 @@
 
     Returns
     -------
     dict
         A formatted dict of pool state/metadata information.
 
     """
-
-    t_end = datetime.utcnow().replace(hour=0, minute=0, second=0, microsecond=0)
+    if end is None:
+        t_end = datetime.now(timezone.utc).replace(
+            hour=0, minute=0, second=0, microsecond=0
+        )
+    else:
+        t_end = datetime.fromtimestamp(end, tz=timezone.utc)
     t_end = t_end.replace(tzinfo=timezone.utc)
     t_start = t_end - timedelta(days=days)
 
     r = await _redemption_prices(address, chain, t_start, t_end, n)
 
     if r is None:
         return None
@@ -433,7 +512,18 @@
 
     t0 = data.index.asof(t_start)
 
     return data[data.index >= t0]
 
 
 redemption_prices_sync = sync(redemption_prices)
+
+if __name__ == "__main__":
+    chain = "mainnet"
+    symbol = "3Crv"
+    print("Chain:", chain)
+    print("Symbol:", symbol)
+    address = symbol_address_sync(symbol, chain)
+    print("Address:", address)
+    _volume_sync = sync(_volume)
+    volumes = _volume_sync(address, chain, days=2)
+    print("Volumes:", volumes)
```

### Comparing `curvesim-0.3.0rc1/curvesim/network/utils.py` & `curvesim-0.4.0a1/curvesim/network/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+"""Common or miscellaneous utility functions"""
 import asyncio
 import functools
 from concurrent.futures import ThreadPoolExecutor
 
 from gmpy2 import mpz
 
 
 def compute_D(xp, A):
+    """Standalone `D` calc neede for some data processing."""
     xp = list(map(int, xp))
     n = len(xp)
     S = sum(xp)
     Dprev = 0
     D = S
     Ann = A * n
     D = mpz(D)
```

### Comparing `curvesim-0.3.0rc1/curvesim/network/web3.py` & `curvesim-0.4.0a1/curvesim/network/web3.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,20 +12,28 @@
 from .http import HTTP
 from .utils import sync
 
 ETHERSCAN_URL = "https://api.etherscan.io/api"
 
 
 def get_etherscan_api_key():
+    """
+    Get the Etherscan API key from the environment.
+    Default to key provided by `curvesim` (not recommended).
+    """
     default_key = "PT1D9IGAPPPRFMD312V9GARWW93BS9ZV6V"
     key = get_env_var("ETHERSCAN_API_KEY", default=default_key)
     return key
 
 
 def get_alchemy_api_key():
+    """
+    Get the Alchemy API key from the environment.
+    Default to key provided by `curvesim` (not recommended).
+    """
     default_key = "WLcYLj9I1w7wEOgKmzidN1z62sbFILUz"
     key = get_env_var("ALCHEMY_API_KEY", default=default_key)
     return key
 
 
 async def explorer(params):
     """
```

### Comparing `curvesim-0.3.0rc1/curvesim/overrides/__init__.py` & `curvesim-0.4.0a1/curvesim/overrides/__init__.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.3.0rc1/curvesim/pipelines/arbitrage.py` & `curvesim-0.4.0a1/curvesim/pipelines/arbitrage.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,60 +1,59 @@
 """
 Implements the volume-limited arbitrage pipeline.
 """
 
 import os
-import traceback
-from datetime import timedelta
 from functools import partial
 
-from numpy import array, exp, isnan, log
-from pandas import DataFrame, MultiIndex
+from numpy import array, isnan
 from scipy.optimize import least_squares, root_scalar
 
-from ..iterators.param_samplers import Grid
-from ..iterators.price_samplers import PriceVolume
-from ..plot import saveplots
-from ..pool.stableswap import StableSwapSimInterface
-from ..pool.stableswap.functions import get_D, get_xp
-from .templates import run_pipeline
-from .utils import compute_volume_multipliers
+from curvesim.iterators.param_samplers import Grid
+from curvesim.iterators.price_samplers import PriceVolume
+from curvesim.logging import get_logger
+from curvesim.metrics import StateLog, init_metrics, make_results
+from curvesim.metrics import metrics as Metrics
+from curvesim.pool import get_sim_pool
+from curvesim.pool_data.cache import PoolDataCache
 
-DEFAULT_PARAMS = {
-    "A": [int(2 ** (a / 2)) for a in range(12, 28)],
-    "fee": list(range(1000000, 5000000, 1000000)),
-}
+from .templates import TradeData, run_pipeline
+from .utils import compute_volume_multipliers
 
-TEST_PARAMS = {"A": [100, 1000], "fee": [3000000, 4000000]}
+logger = get_logger(__name__)
 
 
+# pylint: disable-next=too-many-arguments
 def volume_limited_arbitrage(
-    pool_data,
+    pool_metadata,
+    pool_data_cache=None,
     variable_params=None,
     fixed_params=None,
+    metrics=None,
     test=False,
     days=60,
     src="coingecko",
     data_dir="data",
     vol_mult=None,
     vol_mode=1,
     ncpu=None,
+    end=None,
 ):
     """
     Implements the volume-limited arbitrage pipeline.
 
     At each timestep, the pool is arbitraged as close to the prevailing market price
     as possible without surpassing a volume constraint. By default, volume is limited
     to the total market volume at each timestep, scaled by the proportion of
     volume attributable to the pool over the whole simulation period (vol_mult).
 
     Parameters
     ----------
-    pool_data : :class:`.PoolData`
-        Pool data object for the pool of interest.
+    pool_metadata : :class:`~curvesim.pool_data.metadata.PoolMetaDataInterface`
+        Pool metadata object for the pool of interest.
 
     variable_params : dict, defaults to broad range of A/fee values
         Pool parameters to vary across simulations.
         keys: pool parameters, values: iterables of ints
 
         Example
         --------
@@ -75,15 +74,15 @@
 
             {"A": [100, 1000], "fee": [3000000, 4000000]}
 
     days : int, default=60
         Number of days to pull pool and price data for.
 
     src : str, default="coingecko"
-        Source for price/volume data: "coingecko", "nomics", or "local".
+        Source for price/volume data: "coingecko" or "local".
 
     data_dir : str, default="data"
         relative path to saved price data folder
 
     vol_mult : float or numpy.ndarray, default computed from data
         Value(s) multiplied by market volume to specify volume limits
         (overrides vol_mode).
@@ -103,73 +102,64 @@
         Number of cores to use.
 
     Returns
     -------
     dict
 
     """
-    if variable_params is None:
-        variable_params = DEFAULT_PARAMS
     if test:
         variable_params = TEST_PARAMS
 
     if ncpu is None:
-        ncpu = os.cpu_count() if os.cpu_count() is not None else 1
-
-    pool = pool_data.pool()
-    coins = pool_data.coins()
+        cpu_count = os.cpu_count()
+        ncpu = cpu_count if cpu_count is not None else 1
 
-    param_sampler = Grid(pool, variable_params, fixed_params=fixed_params)
-    price_sampler = PriceVolume(coins, days=days, data_dir=data_dir, src=src)
+    variable_params = variable_params or DEFAULT_PARAMS
+    metrics = metrics or DEFAULT_METRICS
 
-    vol_args = (
-        pool_data.volume(days=days),
-        price_sampler.total_volumes(),
-        pool_data.n(),
-        pool_data.type(),
-    )
+    if pool_data_cache is None:
+        pool_data_cache = PoolDataCache(pool_metadata, days=days, end=end)
 
-    vol_mult = vol_mult or compute_volume_multipliers(*vol_args, mode=vol_mode)
-    strat = partial(strategy, vol_mult=vol_mult)
+    pool = get_sim_pool(pool_metadata, pool_data_cache=pool_data_cache)
+    coins = pool_metadata.coins
 
-    results = run_pipeline(param_sampler, price_sampler, strat, ncpu=ncpu)
-    results = format_results(
-        results, param_sampler.flat_grid(), price_sampler.prices.index
-    )
+    param_sampler = Grid(pool, variable_params, fixed_params=fixed_params)
+    price_sampler = PriceVolume(coins, days=days, data_dir=data_dir, src=src, end=end)
 
-    p_keys = sorted(variable_params.keys())
-    if p_keys == ["A", "fee"]:
-        symbol = pool.symbol
-        address = pool.address
-        folder_name = _plot_folder_name(symbol, address)
-        saveplots(
-            folder_name,
-            variable_params["A"],
-            variable_params["fee"],
-            results,
+    if vol_mult is None:
+        total_pool_volume = pool_data_cache.volume
+        total_market_volume = price_sampler.total_volumes()
+        vol_mult = compute_volume_multipliers(
+            total_pool_volume,
+            total_market_volume,
+            pool_metadata.n,
+            pool_metadata.pool_type,
+            mode=vol_mode,
         )
 
-    return results
+    metrics = init_metrics(metrics, pool=pool, freq=price_sampler.freq)
+    strat = partial(strategy, metrics=metrics, vol_mult=vol_mult)
 
+    output = run_pipeline(param_sampler, price_sampler, strat, ncpu=ncpu)
+    results = make_results(*output, metrics)
 
-def _plot_folder_name(symbol, address):
-    return symbol.lower() + "_" + address[:7].lower()
+    return results
 
 
 # Strategy
-def strategy(pool, params, price_sampler, vol_mult):
+def strategy(pool, parameters, price_sampler, metrics, vol_mult):
     """
     Computes and executes volume-limited arbitrage trades at each timestep.
 
     Parameters
     ----------
     pool : Pool, MetaPool, or RaiPool
         The pool to be arbitraged.
 
-    params : dict
+    parameters : dict
         Current pool parameters from the param_sampler (only used for logging/display).
 
     price_sampler : iterator
         Iterator that returns prices and volumes at each timestep.
 
     vol_mult : float or numpy.ndarray
         Value(s) multiplied by market volume to specify volume limits.
@@ -177,49 +167,43 @@
         Can be a scalar or vector with values for each pairwise coin combination.
 
     Returns
     -------
     metrics : tuple of lists
 
     """
+    trader = Arbitrageur(pool)
+    state_log = StateLog(pool, metrics)
 
-    pool_interface = StableSwapSimInterface(pool)
-    trader = Arbitrageur(pool_interface)
-    metrics = Metrics()
-
-    symbol = pool_interface.pool.metadata["symbol"]
-    print(f"[{symbol}] Simulating with {params}")
-
-    for prices, volumes, timestamp in price_sampler:
-        limits = volumes * vol_mult
-        pool_interface.next_timestamp(timestamp)
-        trades, errors, _ = trader.compute_trades(prices, limits)
-        _, volume = trader.do_trades(trades)
+    symbol = pool.symbol
+    logger.info(f"[{symbol}] Simulating with {parameters}")
 
-        metrics.update(trader.pool_interface, errors, volume)
+    for price_sample in price_sampler:
+        volume_limits = price_sample.volumes * vol_mult
+        pool.prepare_for_trades(price_sample.timestamp)
+        trade_data = trader.arb_pool(price_sample.prices, volume_limits)
+        state_log.update(price_sample=price_sample, trade_data=trade_data)
 
-    return metrics()
+    return state_log.compute_metrics()
 
 
 class Arbitrageur:
     """
     Computes, executes, and reports out arbitrage trades.
     """
 
-    def __init__(self, pool_interface):
+    def __init__(self, pool):
         """
         Parameters
         ----------
-        pool_interface :
+        pool :
             Simulation interface to a subclass of :class:`.Pool`.
 
         """
-        self.pool_interface = pool_interface
-        self.pool_precisions = pool_interface.precisions()
-        self.max_coin = pool_interface.max_coin
+        self.pool = pool
 
     def compute_trades(self, prices, volume_limits):
         """
         Computes trades to optimally arbitrage the pool, constrained by volume limits.
 
         Parameters
         ----------
@@ -238,15 +222,15 @@
         errors : numpy.ndarray
             Post-trade price error between pool price and market price.
 
         res : scipy.optimize.OptimizeResult
             Results object from the numerical optimizer.
 
         """
-        trades, errors, res = opt_arb_multi(self.pool_interface, prices, volume_limits)
+        trades, errors, res = opt_arb_multi(self.pool, prices, volume_limits)
         return trades, errors, res
 
     def do_trades(self, trades):
         """
         Executes a series of trades.
 
         Parameters
@@ -262,201 +246,29 @@
         volume : int
             Total volume of trades in 18 decimal precision.
 
         """
         if len(trades) == 0:
             return [], 0
 
-        p = self.pool_precisions
-        max_coin = self.max_coin
-
-        volume = 0
+        total_volume = 0
         trades_done = []
         for trade in trades:
             i, j, dx = trade
-            dy, _ = self.pool_interface.trade(i, j, dx)
-            trades_done.append(trade + (dy,))
-
-            if max_coin:
-                if i < max_coin or j < max_coin:
-                    volume += dx * p[i] // 10**18  # in D units
-            else:
-                volume += dx * p[i] // 10**18  # in D units
-
-        return trades_done, volume
-
+            dy, fee, volume = self.pool.trade(i, j, dx)
+            trades_done.append((i, j, dx, dy, fee))
 
-# Metrics
-class Metrics:
-    """
-    Computes and stores metrics at each timestep.
-    Calling the instance returns the accumulated data.
-
-    """
+            total_volume += volume
 
-    def __init__(self):
-        self.xs = []
-        self.ps = []
-        self.pool_balance = []
-        self.pool_value = []
-        self.price_depth = []
-        self.price_error = []
-        self.volume = []
+        return trades_done, total_volume
 
-    def __call__(self):
-        """
-        Returns the data accumulated through updates.
-
-        Returns
-        -------
-        records : tuple of lists
-            The accumulated data.
-
-        """
-        records = (
-            self.xs,
-            self.ps,
-            self.pool_balance,
-            self.pool_value,
-            self.price_depth,
-            self.price_error,
-            self.volume,
-        )
-
-        return records
-
-    def update(self, pool_interface, errors, trade_volume):
-        """
-        Computes and stores pool metrics for each timestep.
-
-        Parameters
-        ----------
-        pool_interface :
-            Simulation interface to a subclass of :class:`.Pool`.
-
-        errors : numpy.ndarray
-            Post-trade price error between pool price and market price for each token
-            pair (returned from :meth:`Arbitrageur.compute_trades`).
-
-        trade_volume: int
-            Total volume of trades in 18 decimal precision
-            (returned from :meth:`Arbitrageur.do_trades`).
-
-        """
-        pool_state = pool_interface.get_pool_state()
-        p = getattr(pool_state, "rates", pool_state.p)
-
-        xp = get_xp(pool_state.x, p)
-        bal = self.compute_balance(xp)
-        price_depth = self.compute_price_depth(pool_interface)
-        value = get_D(xp, pool_state.A) / 10**18
-
-        self.xs.append(pool_state.x)
-        self.ps.append(p)
-        self.pool_balance.append(bal)
-        self.pool_value.append(value)
-        self.price_depth.append(sum(price_depth) / len(price_depth))
-        self.price_error.append(sum(abs(errors)))
-        self.volume.append(trade_volume / 10**18)
-
-    @staticmethod
-    def compute_balance(xp):
-        """Compute imbalance factor."""
-        n = len(xp)
-        xp = array(xp)
-        bal = 1 - sum(abs(xp / sum(xp) - 1 / n)) / (2 * (n - 1) / n)
-        return bal
-
-    @staticmethod
-    def compute_price_depth(pool_interface):
-        """Compute price depth."""
-        combos = pool_interface.base_index_combos
-
-        LD = []
-        for i, j in combos:
-            ld = pool_interface.get_liquidity_density(i, j)
-            LD.append(ld)
-        return LD
-
-
-def format_results(results, parameters, timestamps):
-    """
-    Format metrics and compute additional statistics after simulation.
-
-    Parameters
-    ----------
-    results : iterable of iterables
-        Results returned by metrics.
-
-    parameters : iterable of dicts
-        Series of dicts listing the parameters used in each simulation run.
-
-    timestamps : iterable of datetime.datetime
-        Timestamps that were stepped through in the simulation.
-
-    Returns
-    -------
-    results : dict of pandas.DataFrame
-
-        ar: annualized returns
-        bal: pool balance
-        pool_value: pool value
-        depth: liquidity density
-        volume: pool trade volume
-        log_returns: log returns
-        err: post-trade price error
-        x: pool balances
-        p: pool precisions (including basepool virtual price and/or redemption price)
-
-    """
-    (
-        xs,
-        ps,
-        pool_balance,
-        pool_value,
-        price_depth,
-        price_error,
-        volume,
-    ) = results
-
-    param_tuples = [tuple(p.values()) for p in parameters]
-    names = list(parameters[0].keys())
-    p_list = MultiIndex.from_tuples(param_tuples, names=names)
-
-    x = DataFrame(xs, index=p_list, columns=timestamps)
-    p = DataFrame(ps, index=p_list, columns=timestamps)
-    err = DataFrame(price_error, index=p_list, columns=timestamps)
-    bal = DataFrame(pool_balance, index=p_list, columns=timestamps)
-    pool_value = DataFrame(pool_value, index=p_list, columns=timestamps)
-    depth = DataFrame(price_depth, index=p_list, columns=timestamps)
-    volume = DataFrame(volume, index=p_list, columns=timestamps)
-    # pylint: disable-next=no-member
-    log_returns = DataFrame(log(pool_value).diff(axis=1).iloc[:, 1:])
-
-    try:
-        freq = timestamps.freq / timedelta(minutes=1)
-    except Exception:
-        print("Warning: assuming 30 minute sampling for annualizing returns")
-        freq = 30
-    yearmult = 60 / freq * 24 * 365
-    ar = DataFrame(exp(log_returns.mean(axis=1) * yearmult) - 1)
-
-    res = {
-        "ar": ar,
-        "bal": bal,
-        "pool_value": pool_value,
-        "depth": depth,
-        "volume": volume,
-        "log_returns": log_returns,
-        "err": err,
-        "x": x,
-        "p": p,
-    }
-
-    return res
+    def arb_pool(self, prices, volume_limits):
+        trades, price_errors, _ = self.compute_trades(prices, volume_limits)
+        trades_done, volume = self.do_trades(trades)
+        return TradeData(trades_done, volume, volume_limits, price_errors)
 
 
 # Optimizers
 def opt_arb(get_bounds, error_function, i, j, p):
     """
     Estimates a single trade to optimally arbitrage coin[i] for coin[j] given
     external price p (base: i, quote: j).
@@ -499,21 +311,21 @@
 
     trade = (i, j, int(res.root))
     error = error_function(int(res.root), i, j, p)
 
     return trade, error, res
 
 
-def opt_arb_multi(pool_interface, prices, limits):  # noqa: C901
+def opt_arb_multi(pool, prices, limits):  # noqa: C901
     """
     Computes trades to optimally arbitrage the pool, constrained by volume limits.
 
     Parameters
     ----------
-    pool_interface :
+    pool :
         Simulation interface to a subclass of :class:`Pool`.
 
     prices : pandas.Series
         Current market prices from the price_sampler
 
     volume_limits : pandas.Series
         Current volume limits
@@ -527,24 +339,37 @@
     errors : numpy.ndarray
         Post-trade price error between pool price and market price for each token pair.
 
     res : scipy.optimize.OptimizeResult
         Results object from the numerical optimizer.
 
     """
-    get_bounds, error_function, error_function_multi = pool_interface.make_error_fns()
+    (
+        get_bounds,
+        error_function,
+        error_function_multi,
+        index_combos,
+    ) = pool.make_error_fns()
     x0, lo, hi, coins, price_targets = get_trade_args(
-        pool_interface.price,
+        pool.price,
         get_bounds,
         error_function,
         prices,
         limits,
-        pool_interface.index_combos,
+        index_combos,
     )
 
+    # Order trades in terms of expected size
+    order = sorted(range(len(x0)), reverse=True, key=x0.__getitem__)
+    x0 = [x0[i] for i in order]
+    lo = [lo[i] for i in order]
+    hi = [hi[i] for i in order]
+    coins = [coins[i] for i in order]
+    price_targets = [price_targets[i] for i in order]
+
     # Find trades that minimize difference between
     # pool price and external market price
     trades = []
     try:
         res = least_squares(
             error_function_multi,
             x0=x0,
@@ -566,28 +391,18 @@
                 i = coins[k][0]
                 j = coins[k][1]
                 trades.append((i, j, dx))
 
         errors = res.fun
 
     except Exception:
-        print(traceback.format_exc())
-        print(
-            "Optarbs args:\n",
-            "x0: ",
-            str(x0),
-            "lo: ",
-            str(lo),
-            "hi: ",
-            str(hi),
-            "prices: ",
-            str(price_targets),
-            end="\n" * 2,
+        logger.error(
+            f"Optarbs args: x0: {x0}, lo: {lo}, hi: {hi}, prices: {price_targets}",
+            exc_info=True,
         )
-
         errors = array(error_function_multi([0] * len(x0), price_targets, coins))
         res = []
 
     return trades, errors, res
 
 
 def get_trade_args(get_pool_price, get_bounds, error_function, prices, limits, combos):
@@ -624,78 +439,72 @@
 
     hi: list
         Upper bounds on trade sizes for each token pair
 
     coins : list of tuples
         Ordered list of token pairs
 
-    price_targs : list of floats
+    price_targets : list of floats
         Ordered list of price targets for each token pair
 
     """
     x0 = []
     lo = []
     hi = []
     coins = []
-    price_targs = []
+    price_targets = []
 
     for k, pair in enumerate(combos):
         i, j = pair
+        limit = int(limits[k] * 10**18)
         lo.append(0)
-        hi.append(int(limits[k] * 10**18) + 1)
+        hi.append(limit + 1)
 
         if get_pool_price(i, j) - prices[k] > 0:
-            try:
-                trade, _, _ = opt_arb(get_bounds, error_function, i, j, prices[k])
-                x0.append(min(trade[2], int(limits[k] * 10**18)))
-            except ValueError:
-                print(
-                    "Warning: Opt_arb error,",
-                    "Pair:",
-                    (i, j),
-                    "Pool price:",
-                    get_pool_price(i, j),
-                    "Target Price:",
-                    prices[k],
-                    "Diff:",
-                    get_pool_price(i, j) - prices[k],
-                )
-                x0.append(0)
-
-            coins.append((i, j))
-            price_targs.append(prices[k])
-
+            price = prices[k]
+            in_index = i
+            out_index = j
         elif get_pool_price(j, i) - 1 / prices[k] > 0:
-            try:
-                trade, _, _ = opt_arb(get_bounds, error_function, j, i, 1 / prices[k])
-                x0.append(min(trade[2], int(limits[k] * 10**18)))
-            except ValueError:
-                print(
-                    "Warning: Opt_arb error,",
-                    "Pair:",
-                    (j, i),
-                    "Pool price:",
-                    get_pool_price(j, i),
-                    "Target Price:",
-                    1 / prices[k],
-                    "Diff:",
-                    get_pool_price(j, i) - 1 / prices[k],
-                )
-                x0.append(0)
-
-            coins.append((j, i))
-            price_targs.append(1 / prices[k])
-
+            price = 1 / prices[k]
+            in_index = j
+            out_index = i
         else:
             x0.append(0)
             coins.append((i, j))
-            price_targs.append(prices[k])
+            price_targets.append(prices[k])
+            continue
 
-    # Order trades in terms of expected size
-    order = sorted(range(len(x0)), reverse=True, key=x0.__getitem__)
-    x0 = [x0[i] for i in order]
-    lo = [lo[i] for i in order]
-    hi = [hi[i] for i in order]
-    coins = [coins[i] for i in order]
-    price_targs = [price_targs[i] for i in order]
+        try:
+            trade, _, _ = opt_arb(
+                get_bounds, error_function, in_index, out_index, price
+            )
+            size = min(trade[2], limit)
+            x0.append(size)
+        except ValueError:
+            pool_price = get_pool_price(in_index, out_index)
+            logger.error(
+                f"Opt_arb error: Pair: {(in_index, out_index)}, Pool price: {pool_price},"
+                f"Target Price: {price}, Diff: {pool_price - price}"
+            )
+            x0.append(0)
+
+        coins.append((in_index, out_index))
+        price_targets.append(price)
+
+    return x0, lo, hi, coins, price_targets
 
-    return x0, lo, hi, coins, price_targs
+
+# Defaults
+DEFAULT_METRICS = [
+    Metrics.Timestamp,
+    Metrics.PoolValue,
+    Metrics.PoolBalance,
+    Metrics.PriceDepth,
+    Metrics.ArbMetrics,
+]
+
+DEFAULT_PARAMS = {
+    "A": [int(2 ** (a / 2)) for a in range(12, 28)],
+    "fee": list(range(1000000, 5000000, 1000000)),
+}
+
+TEST_PARAMS = {"A": [100, 1000], "fee": [3000000, 4000000]}
```

### Comparing `curvesim-0.3.0rc1/curvesim/pipelines/utils.py` & `curvesim-0.4.0a1/curvesim/pipelines/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+"""Miscellaneous utility functions."""
 from math import factorial
 
 from numpy import append
 
+from curvesim.logging import get_logger
 from curvesim.pool import CurveMetaPool, CurvePool
 
+logger = get_logger(__name__)
+
 
-# Volume Multipliers
 def compute_volume_multipliers(pool_vol, market_vol, n, pool_type, mode=1):
     """
     Computes volume multipliers (vol_mult) used for volume limiting.
 
     Parameters
     ----------
     pool_vol : numpy.ndarray
@@ -30,38 +33,36 @@
         1: limits trade volumes proportionally to market volume for each pair
 
         2: limits trade volumes equally across pairs
 
         3: mode 2 for trades with meta-pool asset, mode 1 for basepool-only trades
 
     """
-    if pool_type == CurvePool:
+    if pool_type is CurvePool:
         vol_mult = pool_vol_mult(pool_vol, market_vol, n, mode)
 
-    elif pool_type == CurveMetaPool:
+    elif pool_type is CurveMetaPool:
         vol_mult = metapool_vol_mult(pool_vol, market_vol, n, mode)
 
     else:
         raise TypeError(f"Pool type {pool_type} not supported by this pipeline")
 
-    print("Volume Multipliers:")
-    print(vol_mult)
-
+    logger.info(f"Volume Multipliers: {vol_mult}")
     return vol_mult
 
 
 def pool_vol_mult(pool_vol, market_vol, n, mode):
     if mode == 1:
         vol_mult = pool_vol / market_vol.sum()
 
     if mode == 2:
         vol_mult = pool_vol.repeat(n) / n / market_vol
 
     if mode == 3:
-        print("Vol_mode=3 only available for meta-pools. Reverting to vol_mode=1")
+        logger.info("Vol_mode=3 only available for meta-pools. Reverting to vol_mode=1")
         vol_mult = pool_vol / market_vol.sum()
 
     return vol_mult
 
 
 def metapool_vol_mult(pool_vol, market_vol, n, mode):
     pool_vol_meta = pool_vol[0]
```

### Comparing `curvesim-0.3.0rc1/curvesim/pool/base.py` & `curvesim-0.4.0a1/curvesim/pool/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,32 @@
 """
 Module housing the required implementation for any pool entity
 in the Curvesim Framework.
 """
 
 
-class Pool:
+from curvesim.pool.snapshot import SnapshotMixin
+
+
+class Pool(SnapshotMixin):
     """
-    The `Pool` base class has the explicitly required properties for any pool-like
-    object used in Curvesim.
+    The `Pool` base class has the explicitly required properties for any
+    pool-like object used in Curvesim.
+
+    The `SnapshotMixin` gives the ability to snapshot balances and revert
+    balance changes.
 
     Currently the base attributes are not informative for pools
     constructed manually rather than from chain data.
     """
 
+    # need to configure in derived class otherwise the
+    # snapshotting will not work
+    snapshot_class = None
+
     @property
     def name(self):
         """Descriptive name for this pool"""
         if hasattr(self, "metadata"):
             return self.metadata["name"]
         return "Custom pool"
 
@@ -24,14 +34,35 @@
     def address(self):
         """Address on chain"""
         if hasattr(self, "metadata"):
             return self.metadata["address"]
         return "0x" + "0" * 40
 
     @property
+    def coin_names(self):
+        """Symbols for the pool coins."""
+        if hasattr(self, "metadata"):
+            return self.metadata["coins"]["names"]
+        return []
+
+    @property
+    def coin_addresses(self):
+        """Addresses for the pool coins."""
+        if hasattr(self, "metadata"):
+            return self.metadata["coins"]["addresses"]
+        return []
+
+    @property
+    def coin_decimals(self):
+        """Addresses for the pool coins."""
+        if hasattr(self, "metadata"):
+            return self.metadata["coins"]["decimals"]
+        return []
+
+    @property
     def chain(self):
         """Chain for this pool"""
         if hasattr(self, "metadata"):
             return self.metadata["chain"]
         return "No chain"
 
     @property
@@ -44,9 +75,18 @@
     @property
     def symbol(self):
         """LP token symbol"""
         if hasattr(self, "metadata"):
             return self.metadata["symbol"]
         return "Custom"
 
+    @property
+    def folder_name(self):
+        """Name of folder containing saved sim results."""
+        if hasattr(self, "metadata"):
+            symbol = self.symbol
+            address = self.address
+            return symbol.lower() + "_" + address[:7].lower()
+        return "custom_pool_" + str(hash(self))
+
     def __repr__(self):
         return f"<{self.__class__.__name__} address={self.address} chain={self.chain}>"
```

### Comparing `curvesim-0.3.0rc1/curvesim/pool/stableswap/metapool.py` & `curvesim-0.4.0a1/curvesim/pool/stableswap/metapool.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,47 +1,67 @@
 """
 Mainly a module to house the `MetaPool`, a metapool stableswap implementation in Python.
 """
 from math import prod
 
 from gmpy2 import mpz
 
+from curvesim.pool.snapshot import CurveMetaPoolBalanceSnapshot
+
 from ..base import Pool
 
 
-class CurveMetaPool(Pool):
+class CurveMetaPool(Pool):  # pylint: disable=too-many-instance-attributes
     """
     Basic stableswap metapool implementation in Python.
     """
 
+    snapshot_class = CurveMetaPoolBalanceSnapshot
+
+    __slots__ = (
+        "A",
+        "n",
+        "max_coin",
+        "fee",
+        "admin_fee",
+        "basepool",
+        "rate_multiplier",
+        "balances",
+        "n_total",
+        "tokens",
+        "fee_mul",
+        "admin_balances",
+    )
+
+    # pylint: disable=too-many-arguments
     def __init__(
         self,
         A,
         D,
         n,
         basepool,
-        p=None,
+        rate_multiplier=10**18,
         tokens=None,
         fee=4 * 10**6,
         fee_mul=None,
         admin_fee=0 * 10**9,
     ):
         """
         Parameters
         ----------
         A : int
             Amplification coefficient; this is :math:`A n^{n-1}` in the whitepaper.
         D : int or list of int
-            coin balances or virtual total balance
+            virtual total balance or coin balances in native token units
         n: int
             number of coins
         basepool: :class:`curvesim.pool.Pool`
             basepool for the metapool
-        p: list of int, optional
-            precision and rate adjustments, defaults to 10**18 each coin
+        rate_multiplier: int, optional
+            precision and rate adjustment, defaults to 10**18
         tokens: int
             LP token supply
         fee: int, optional
             fee with 10**10 precision (default = .004%)
         fee_mul: optional
             fee multiplier for dynamic fee pools
         admin_fee: int, optional
@@ -55,49 +75,30 @@
         self.max_coin = self.n - 1
         self.fee = fee
         self.admin_fee = admin_fee
 
         # If basepool coins have too few decimals, it can wreak havoc
         # on a certain codepath of our `dydx` function, where we use
         # a difference quotient to estimate the derivative.
-        for _p in basepool.p:
+        for _p in basepool.rates:
             if _p > 10**30:
                 raise ValueError(f"{_p} too high: decimals must be >= 6.")
         self.basepool = basepool
 
-        if p:
-            self.p = p
-        else:
-            self.p = [10**18] * n
+        self.rate_multiplier = rate_multiplier
 
         if isinstance(D, list):
-            self.x = D
+            self.balances = D
         else:
-            rates = self.rates()
-            self.x = [D // n * 10**18 // _p for _p in rates]
+            self.balances = [D // n * 10**18 // _p for _p in self.rates]
 
         self.n_total = n + basepool.n - 1
         self.tokens = tokens
         self.fee_mul = fee_mul
-        self.collected_admin_fees = [0] * n
-
-    @property
-    def balances(self):
-        """
-        Alias to adhere closer to vyper interface.
-
-        Returns
-        -------
-        list of int
-            pool coin balances in native token units
-        """
-        return self.x
-
-    def next_timestamp(self, *args, **kwargs):
-        pass
+        self.admin_balances = [0] * n
 
     def D(self, xp=None):
         """
         `D` is the stableswap invariant; this can be thought of as the value of
         all coin balances if the pool were to become balanced.
 
         Convenience wrapper for `get_D` which uses the set `A` and makes `xp`
@@ -115,16 +116,16 @@
 
         Note
         ----
         This is a "view" function; it doesn't change the state of the pool.
         """
         A = self.A
         if not xp:
-            rates = self.rates()
-            xp = [x * p // 10**18 for x, p in zip(self.x, rates)]
+            rates = self.rates
+            xp = [x * p // 10**18 for x, p in zip(self.balances, rates)]
         return self.get_D(xp, A)
 
     def get_D(self, xp, A):
         r"""
         Calculate D invariant iteratively using non-overflowing integer operations.
 
         Stableswap equation:
@@ -170,16 +171,16 @@
             Dprev = D
             D = (Ann * S + D_P * self.n) * D // ((Ann - 1) * D + (self.n + 1) * D_P)
 
         D = int(D)
         return D
 
     def _xp(self):
-        rates = self.rates()
-        balances = self.x
+        rates = self.rates
+        balances = self.balances
         return self._xp_mem(rates, balances)
 
     def _xp_mem(self, rates, balances):
         return [x * p // 10**18 for x, p in zip(balances, rates)]
 
     def get_D_mem(self, rates, balances, A):
         """
@@ -332,36 +333,37 @@
         Examples
         --------
 
         >>> pool = MetaPool(A=250, D=1000000 * 10**18, n=2, p=[10**30, 10**30])
         >>> pool.exchange(0, 1, 150 * 10**6)
         (149939820, 59999)
         """
-        xp = self._xp()
-        x = xp[i] + dx * self.p[i] // 10**18
+        rates = self.rates
+        xp = self._xp_mem(rates, self.balances)
+        x = xp[i] + dx * rates[i] // 10**18
         y = self.get_y(i, j, x, xp)
         dy = xp[j] - y - 1
 
         if self.fee_mul is None:
             fee = dy * self.fee // 10**10
         else:
             fee = dy * self.dynamic_fee((xp[i] + x) // 2, (xp[j] + y) // 2) // 10**10
 
         admin_fee = fee * self.admin_fee // 10**10
 
         # Convert all to real units
-        rate = self.p[j]
+        rate = rates[j]
         dy = (dy - fee) * 10**18 // rate
         fee = fee * 10**18 // rate
         admin_fee = admin_fee * 10**18 // rate
         assert dy >= 0
 
-        self.x[i] += dx
-        self.x[j] -= dy + admin_fee
-        self.collected_admin_fees[j] += admin_fee
+        self.balances[i] += dx
+        self.balances[j] -= dy + admin_fee
+        self.admin_balances[j] += admin_fee
         return dy, fee
 
     def exchange_underlying(self, i, j, dx):
         """
         Perform an exchange between two coins.
 
         Index values include underlyer indices.  The zero index
@@ -379,28 +381,28 @@
             Amount of coin `i` being exchanged.
 
         Returns
         -------
         (int, int)
             (amount of coin `j` received, trading fee)
         """
-        rates = self.rates()
+        rates = self.rates
 
         # Use base_i or base_j if they are >= 0
         base_i = i - self.max_coin
         base_j = j - self.max_coin
         meta_i = self.max_coin
         meta_j = self.max_coin
         if base_i < 0:
             meta_i = i
         if base_j < 0:
             meta_j = j
 
         if base_i < 0 or base_j < 0:  # if i or j not in basepool
-            xp = [x * p // 10**18 for x, p in zip(self.x, rates)]
+            xp = [x * p // 10**18 for x, p in zip(self.balances, rates)]
 
             if base_i < 0:
                 x = xp[i] + dx * rates[i] // 10**18
             else:
                 # i is from BasePool
                 # At first, get the amount of pool tokens
                 base_inputs = [0] * self.basepool.n
@@ -424,18 +426,18 @@
 
             dy_admin_fee = dy_fee * self.admin_fee // 10**10
             dy_admin_fee = dy_admin_fee * 10**18 // rates[meta_j]
 
             dy_fee = dy_fee * 10**18 // rates[meta_j]
 
             # Change balances exactly in same way as we change actual ERC20 coin amounts
-            self.x[meta_i] += dx
+            self.balances[meta_i] += dx
             # When rounding errors happen, we undercharge admin fee in favor of LP
-            self.x[meta_j] -= dy + dy_admin_fee
-            self.collected_admin_fees[meta_j] += dy_admin_fee
+            self.balances[meta_j] -= dy + dy_admin_fee
+            self.admin_balances[meta_j] += dy_admin_fee
 
             # Withdraw from the base pool if needed
             if base_j >= 0:
                 dy, dy_fee = self.basepool.remove_liquidity_one_coin(dy, base_j)
 
         else:
             # If both are from the base pool
@@ -465,20 +467,21 @@
             Redemption amount in i-th coin
 
         Note
         ----
         This is a "view" function; it doesn't change the state of the pool.
         """
         A = self.A
-        xp = self._xp()
+        rates = self.rates
+        xp = self._xp_mem(rates, self.balances)
         D0 = self.D()
         D1 = D0 - token_amount * D0 // self.tokens
 
         new_y = self.get_y_D(A, i, xp, D1)
-        dy_before_fee = (xp[i] - new_y) * 10**18 // self.p[i]
+        dy_before_fee = (xp[i] - new_y) * 10**18 // rates[i]
 
         xp_reduced = xp
         if self.fee and use_fee:
             n_coins = self.n
             _fee = self.fee * n_coins // (4 * (n_coins - 1))
 
             for j in range(n_coins):
@@ -486,20 +489,21 @@
                 if j == i:
                     dx_expected = xp[j] * D1 // D0 - new_y
                 else:
                     dx_expected = xp[j] - xp[j] * D1 // D0
                 xp_reduced[j] -= _fee * dx_expected // 10**10
 
         dy = xp[i] - self.get_y_D(A, i, xp_reduced, D1)
-        dy = (dy - 1) * 10**18 // self.p[i]
+        dy = (dy - 1) * 10**18 // rates[i]
+
         if use_fee:
             dy_fee = dy_before_fee - dy
             return dy, dy_fee
-        else:
-            return dy
+
+        return dy
 
     def add_liquidity(self, amounts):
         """
         Deposit coin amounts for LP token.
 
         Parameters
         ----------
@@ -510,24 +514,22 @@
         -------
         int
             LP token amount received for the deposit amounts.
         """
         mint_amount, fees = self.calc_token_amount(amounts, use_fee=True)
         self.tokens += mint_amount
 
-        balances = self.x
+        balances = self.balances
         afee = self.admin_fee
         admin_fees = [f * afee // 10**10 for f in fees]
         new_balances = [
             bal + amt - fee for bal, amt, fee in zip(balances, amounts, admin_fees)
         ]
-        self.x = new_balances
-        self.collected_admin_fees = [
-            t + a for t, a in zip(self.collected_admin_fees, admin_fees)
-        ]
+        self.balances = new_balances
+        self.admin_balances = [t + a for t, a in zip(self.admin_balances, admin_fees)]
 
         return mint_amount
 
     def remove_liquidity_one_coin(self, token_amount, i):
         """
         Redeem given LP token amount for the i-th coin.
 
@@ -541,23 +543,23 @@
         Returns
         -------
         int
             Redemption amount in i-th coin
         """
         dy, dy_fee = self.calc_withdraw_one_coin(token_amount, i, use_fee=True)
         admin_fee = dy_fee * self.admin_fee // 10**10
-        self.x[i] -= dy + admin_fee
-        self.collected_admin_fees[i] += admin_fee
+        self.balances[i] -= dy + admin_fee
+        self.admin_balances[i] += admin_fee
         self.tokens -= token_amount
         return dy, dy_fee
 
+    @property
     def rates(self):
-        rates = self.p[:]
-        rates[self.max_coin] = self.basepool.get_virtual_price()
-        return rates
+        base_virtual_price = self.basepool.get_virtual_price()
+        return [self.rate_multiplier, base_virtual_price]
 
     def calc_token_amount(self, amounts, use_fee=False):
         """
         Calculate the amount of LP tokens received for the given coin
         deposit amounts.
 
         Fee logic is based on add_liquidity, which makes this more accurate than
@@ -579,19 +581,19 @@
             LP token amount received for the deposit amounts.
 
         Note
         ----
         This is a "view" function; it doesn't change the state of the pool.
         """
         A = self.A
-        old_balances = self.x
-        rates = self.rates()
+        old_balances = self.balances
+        rates = self.rates
         D0 = self.get_D_mem(rates, old_balances, A)
 
-        new_balances = self.x[:]
+        new_balances = self.balances[:]
         for i in range(self.n):
             new_balances[i] += amounts[i]
         D1 = self.get_D_mem(rates, new_balances, A)
 
         mint_balances = new_balances[:]
 
         if use_fee:
@@ -603,18 +605,19 @@
                 difference = abs(ideal_balance - new_balances[i])
                 fees[i] = _fee * difference // 10**10
                 mint_balances[i] -= fees[i]
 
         D2 = self.get_D_mem(rates, mint_balances, A)
 
         mint_amount = self.tokens * (D2 - D0) // D0
+
         if use_fee:
             return mint_amount, fees
-        else:
-            return mint_amount
+
+        return mint_amount
 
     def get_virtual_price(self):
         """
         Returns the expected value of one LP token if the pool were
         to become perfectly balanced (all coins revert to peg).
 
         Returns
@@ -693,24 +696,24 @@
         Note
         ----
         This is a "view" function; it doesn't change the state of the pool.
 
         The following formulae are useful when swapping the primary stablecoin
         for one of the basepool underlyers:
 
-            $z$: primary coin virtual balance\n
-            $w$: basepool virtual balance in the metapool \n
-            $x_i$: basepool coin virtual balances\n
-            $D$: basepool invariant\n
+            |  $z$: primary coin virtual balance
+            |  $w$: basepool virtual balance in the metapool
+            |  $x_i$: basepool coin virtual balances
+            |  $D$: basepool invariant
 
             The chain rule gives:
 
             .. math::
-                \\frac{dz}{dx_i} = \\frac{dz}{dw} \\frac{dw}{dx_i}
-                    = \\frac{dz}{dw} \\frac{dD}{dx_i} = \\frac{dz}{dw} D'
+                \frac{dz}{dx_i} = \frac{dz}{dw} \frac{dw}{dx_i}
+                    = \frac{dz}{dw} \frac{dD}{dx_i} = \frac{dz}{dw} D'
 
             where
 
             .. math::
                 D' = -1 ( A n^{n+1} \prod{x_k} + D^{n+1} / x_i)
                         / ( n^n \prod{x_k} - A n^{n+1} \prod{x_k} - (n + 1) D^n
         """  # noqa
@@ -718,20 +721,19 @@
         base_j = j - self.max_coin
 
         # both in and out tokens are in basepool
         if base_i >= 0 and base_j >= 0:
             _dydx = self.basepool.dydx(base_i, base_j, use_fee=use_fee)
             return float(_dydx)
 
-        rates = self.p[:]
-        rates[self.max_coin] = self.basepool.get_virtual_price()
-        xp = [mpz(x) * p // 10**18 for x, p in zip(self.x, rates)]
+        rates = self.rates
+        xp = [mpz(x) * p // 10**18 for x, p in zip(self.balances, rates)]
 
         bp = self.basepool
-        base_xp = [mpz(x) * p // 10**18 for x, p in zip(bp.x, bp.p)]
+        base_xp = [mpz(x) * p // 10**18 for x, p in zip(bp.balances, bp.rates)]
         x_prod = prod(base_xp)
         n = bp.n
         A = bp.A
         D = mpz(bp.D())
         D_pow = D ** (n + 1)
         A_pow = A * n ** (n + 1)
 
@@ -752,15 +754,15 @@
             else:
                 fee = 0
             _dydx *= 1 - fee / 10**10
 
         else:  # i is from basepool
             dx = 10**12
             base_inputs = [0] * self.basepool.n
-            base_inputs[base_i] = dx * 10**18 // self.basepool.p[base_i]
+            base_inputs[base_i] = dx * 10**18 // self.basepool.rates[base_i]
 
             dw, _ = self.basepool.calc_token_amount(base_inputs, use_fee=True)
             # Convert lp token amount to virtual units
             dw = dw * rates[self.max_coin] // 10**18
             x = xp[self.max_coin] + dw
 
             meta_i = self.max_coin
@@ -824,17 +826,14 @@
             xi * (xj * A_pow * x_prod + D_pow)
         )
 
         if use_fee:
             if self.fee_mul is None:
                 fee_factor = self.fee / 10**10
             else:
-                dx = 10**12
-                fee_factor = (
-                    self.dynamic_fee(xi + dx // 2, xj - int(dydx * dx) // 2) / 10**10
-                )
+                fee_factor = self.dynamic_fee(xi, xj) / 10**10
         else:
             fee_factor = 0
 
         dydx *= 1 - fee_factor
 
         return float(dydx)
```

### Comparing `curvesim-0.3.0rc1/curvesim/pool/stableswap/pool.py` & `curvesim-0.4.0a1/curvesim/pool/stableswap/pool.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,92 +1,100 @@
 """
 Mainly a module to house the `Pool`, a basic stableswap implementation in Python.
 """
 from math import prod
 
 from gmpy2 import mpz
 
+from curvesim.pool.snapshot import CurvePoolBalanceSnapshot
+
 from ..base import Pool
 
 
-class CurvePool(Pool):
+class CurvePool(Pool):  # pylint: disable=too-many-instance-attributes
     """
     Basic stableswap implementation in Python.
     """
 
-    def __init__(
+    snapshot_class = CurvePoolBalanceSnapshot
+
+    __slots__ = (
+        "A",
+        "n",
+        "fee",
+        "rates",
+        "balances",
+        "tokens",
+        "fee_mul",
+        "admin_fee",
+        "r",
+        "n_total",
+        "admin_balances",
+    )
+
+    def __init__(  # pylint: disable=too-many-arguments
         self,
         A,
         D,
         n,
-        p=None,
+        rates=None,
         tokens=None,
         fee=4 * 10**6,
         fee_mul=None,
         admin_fee=0 * 10**9,
     ):
         """
         Parameters
         ----------
         A : int
             Amplification coefficient; this is :math:`A n^{n-1}` in the whitepaper.
         D : int or list of int
-            coin balances or virtual total balance
+            virtual total balance or pool coin balances in native token units
         n: int
             number of coins
-        p: list of int
+        rates: list of int
             precision and rate adjustments
         tokens: int
             LP token supply
         fee: int, optional
             fee with 10**10 precision (default = .004%)
         fee_mul: optional
             fee multiplier for dynamic fee pools
         admin_fee: int, optional
             percentage of `fee` with 10**10 precision (default = 50%)
         """
         # FIXME: set admin_fee default back to 5 * 10**9
         # once sim code is updated.  Right now we use 0
         # to pass the CI tests.
-        p = p or [10**18] * n
+        rates = rates or [10**18] * n
 
         if isinstance(D, list):
-            x = D
+            balances = D
         else:
-            x = [D // n * 10**18 // _p for _p in p]
+            balances = [D // n * 10**18 // _p for _p in rates]
 
         self.A = A
         self.n = n
         self.fee = fee
-        self.p = p
-        self.x = x
+        self.rates = rates
+        self.balances = balances
         self.tokens = tokens or self.D()
         self.fee_mul = fee_mul
         self.admin_fee = admin_fee
         self.r = False
         self.n_total = n
         self.admin_balances = [0] * n
 
-    @property
-    def balances(self):
-        """
-        Alias to adhere closer to vyper interface.
-
-        Returns
-        -------
-        list of int
-            pool coin balances in native token units
-        """
-        return self.x
-
-    def next_timestamp(self, *args, **kwargs):
-        pass
-
     def _xp(self):
-        return [x * p // 10**18 for x, p in zip(self.x, self.p)]
+        rates = self.rates
+        balances = self.balances
+        return self._xp_mem(rates, balances)
+
+    def _xp_mem(self, rates, balances):
+        return [x * p // 10**18 for x, p in zip(balances, rates)]
 
     def D(self, xp=None):
         """
         `D` is the stableswap invariant; this can be thought of as the value of
         all coin balances if the pool were to become balanced.
 
         Convenience wrapper for `get_D` which uses the set `A` and makes `xp`
@@ -178,15 +186,15 @@
         int
             The stableswap invariant, `D`.
 
         Note
         ----
         This is a "view" function; it doesn't change the state of the pool.
         """
-        xp = [x * p // 10**18 for x, p in zip(balances, self.p)]
+        xp = [x * p // 10**18 for x, p in zip(balances, self.rates)]
         return self.get_D(xp, A)
 
     def get_y(self, i, j, x, xp):
         r"""
         Calculate x[j] if one makes x[i] = x.
 
         The stableswap equation gives the following:
@@ -316,34 +324,34 @@
         --------
 
         >>> pool = Pool(A=250, D=1000000 * 10**18, n=2, p=[10**30, 10**30])
         >>> pool.exchange(0, 1, 150 * 10**6)
         (149939820, 59999)
         """
         xp = self._xp()
-        x = xp[i] + dx * self.p[i] // 10**18
+        x = xp[i] + dx * self.rates[i] // 10**18
         y = self.get_y(i, j, x, xp)
         dy = xp[j] - y - 1
 
         if self.fee_mul is None:
             fee = dy * self.fee // 10**10
         else:
             fee = dy * self.dynamic_fee((xp[i] + x) // 2, (xp[j] + y) // 2) // 10**10
 
         admin_fee = fee * self.admin_fee // 10**10
 
         # Convert all to real units
-        rate = self.p[j]
+        rate = self.rates[j]
         dy = (dy - fee) * 10**18 // rate
         fee = fee * 10**18 // rate
         admin_fee = admin_fee * 10**18 // rate
         assert dy >= 0
 
-        self.x[i] += dx
-        self.x[j] -= dy + admin_fee
+        self.balances[i] += dx
+        self.balances[j] -= dy + admin_fee
         self.admin_balances[j] += admin_fee
         return dy, fee
 
     def calc_withdraw_one_coin(self, token_amount, i, use_fee=True):
         """
         Calculate the amount in the i-th coin received from
         redeeming the given amount of LP tokens.
@@ -370,15 +378,15 @@
         """
         A = self.A
         xp = self._xp()
         D0 = self.D()
         D1 = D0 - token_amount * D0 // self.tokens
 
         new_y = self.get_y_D(A, i, xp, D1)
-        dy_before_fee = (xp[i] - new_y) * 10**18 // self.p[i]
+        dy_before_fee = (xp[i] - new_y) * 10**18 // self.rates[i]
 
         xp_reduced = xp
         if self.fee and use_fee:
             n_coins = self.n
             _fee = self.fee * n_coins // (4 * (n_coins - 1))
 
             for j in range(n_coins):
@@ -386,20 +394,21 @@
                 if j == i:
                     dx_expected = xp[j] * D1 // D0 - new_y
                 else:
                     dx_expected = xp[j] - xp[j] * D1 // D0
                 xp_reduced[j] -= _fee * dx_expected // 10**10
 
         dy = xp[i] - self.get_y_D(A, i, xp_reduced, D1)
-        dy = (dy - 1) * 10**18 // self.p[i]
+        dy = (dy - 1) * 10**18 // self.rates[i]
+
         if use_fee:
             dy_fee = dy_before_fee - dy
             return dy, dy_fee
-        else:
-            return dy
+
+        return dy
 
     def add_liquidity(self, amounts):
         """
         Deposit coin amounts for LP token.
 
         Parameters
         ----------
@@ -410,21 +419,21 @@
         -------
         int
             LP token amount received for the deposit amounts.
         """
         mint_amount, fees = self.calc_token_amount(amounts, use_fee=True)
         self.tokens += mint_amount
 
-        balances = self.x
+        balances = self.balances
         afee = self.admin_fee
         admin_fees = [f * afee // 10**10 for f in fees]
         new_balances = [
             bal + amt - fee for bal, amt, fee in zip(balances, amounts, admin_fees)
         ]
-        self.x = new_balances
+        self.balances = new_balances
         self.admin_balances = [t + a for t, a in zip(self.admin_balances, admin_fees)]
 
         return mint_amount
 
     def remove_liquidity_one_coin(self, token_amount, i):
         """
         Redeem given LP token amount for the i-th coin.
@@ -439,15 +448,15 @@
         Returns
         -------
         int
             Redemption amount in i-th coin
         """
         dy, dy_fee = self.calc_withdraw_one_coin(token_amount, i, use_fee=True)
         admin_fee = dy_fee * self.admin_fee // 10**10
-        self.x[i] -= dy + admin_fee
+        self.balances[i] -= dy + admin_fee
         self.admin_balances[i] += admin_fee
         self.tokens -= token_amount
         return dy, dy_fee
 
     def calc_token_amount(self, amounts, use_fee=False):
         """
         Calculate the amount of LP tokens received for the given coin
@@ -472,18 +481,18 @@
             LP token amount received for the deposit amounts.
 
         Note
         ----
         This is a "view" function; it doesn't change the state of the pool.
         """
         A = self.A
-        old_balances = self.x
+        old_balances = self.balances
         D0 = self.get_D_mem(old_balances, A)
 
-        new_balances = self.x[:]
+        new_balances = self.balances[:]
         for i in range(self.n):
             new_balances[i] += amounts[i]
         D1 = self.get_D_mem(new_balances, A)
 
         mint_balances = new_balances[:]
 
         if use_fee:
@@ -495,18 +504,19 @@
                 difference = abs(ideal_balance - new_balances[i])
                 fees[i] = _fee * difference // 10**10
                 mint_balances[i] -= fees[i]
 
         D2 = self.get_D_mem(mint_balances, A)
 
         mint_amount = self.tokens * (D2 - D0) // D0
+
         if use_fee:
             return mint_amount, fees
-        else:
-            return mint_amount
+
+        return mint_amount
 
     def get_virtual_price(self):
         """
         Returns the expected value of one LP token if the pool were
         to become perfectly balanced (all coins revert to peg).
 
         Returns
@@ -579,14 +589,17 @@
             Price of i-th coin quoted in j-th coin
 
         Note
         ----
         This is a "view" function; it doesn't change the state of the pool.
         """
         xp = self._xp()
+        return self._dydx(i, j, xp, use_fee)
+
+    def _dydx(self, i, j, xp, use_fee):
         xi = xp[i]
         xj = xp[j]
         n = self.n
         A = self.A
         D = self.D(xp)
         D_pow = mpz(D) ** (n + 1)
         x_prod = prod(xp)
```

### Comparing `curvesim-0.3.0rc1/curvesim/price_data/__init__.py` & `curvesim-0.4.0a1/curvesim/price_data/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 Tools for retrieving price data.
 Currently supports Coingecko, Nomics, and locally stored data.
 
 To use nomics, set the OS environment variable NOMICS_API_KEY.
 
 """
 
-from .sources import coingecko, local, nomics
+from curvesim.exceptions import NetworkError
 
+from .sources import coingecko, local
 
-def get(coins, days=60, data_dir="data", src="coingecko"):
+
+def get(coins, days=60, data_dir="data", src="coingecko", end=None):
     """
     Pull price and volume data for given coins.
 
     Data is returned for all pairwise combinations of the input coins.
 
     Parameters
     ----------
@@ -42,13 +44,13 @@
         Proportion of timestamps with zero volume.
 
     """
     if src == "coingecko":
         prices, volumes, pzero = coingecko(coins, days=days)
 
     elif src == "nomics":
-        prices, volumes, pzero = nomics(coins, days=days, data_dir=data_dir)
+        raise NetworkError("Nomics data is no longer supported.")
 
     elif src == "local":
-        prices, volumes, pzero = local(coins, data_dir=data_dir)
+        prices, volumes, pzero = local(coins, data_dir=data_dir, end=end)
 
     return prices, volumes, pzero
```

### Comparing `curvesim-0.3.0rc1/curvesim/sim/__init__.py` & `curvesim-0.4.0a1/curvesim/sim/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,56 +2,56 @@
 A simulation runs trades against Curve pools, possibly a variety of
 informed and noisy trades, although currently only "optimal" arbitrages
 are supported.
 
 The primary use-case is to determine optimal amplitude (A) and
 fee parameters given historical price and volume feeds.
 """
+from curvesim.logging import get_logger
 from curvesim.pipelines.arbitrage import DEFAULT_PARAMS, volume_limited_arbitrage
-from curvesim.pool_data import get as get_pool_data
+from curvesim.pool_data import get_metadata
 
+logger = get_logger(__name__)
 
-def autosim(pool=None, chain="mainnet", pool_data=None, **kwargs):
+
+def autosim(
+    pool=None, chain="mainnet", pool_metadata=None, pool_data_cache=None, **kwargs
+):
     """
     The autosim() function simulates existing Curve pools with a range of
     parameters (e.g., the amplitude parameter, A, and/or the exchange fee).
 
     The function fetches pool properties (e.g., current pool size) and 2
-    months of price/volume data, runs multiple simulations in parallel, and
-    saves results plots to the "results" directory.
+    months of price/volume data and runs multiple simulations in parallel.
 
     Curve pools from any chain supported by the Convex Community Subgraphs
-    can be simulated directly by inputting the pool's address or its LP
-    token symbol.
+    can be simulated directly by inputting the pool's address.
 
     Parameters
     ----------
     pool: str, optional
-        This string identifies the pool by address or LP token symbol.
+        This 0x-prefixed string identifies the pool by address.
 
         .. note::
-            Either `pool` or `pool_data` must be provided.
-
-        .. warning::
-            An LP token symbol need not be unique.  In particular, factory
-            pools are deployed permissionlessly and no checks are done to
-            ensure unique LP token symbol.  Currently the first pool
-            retrieved from the subgraph is used, which can be effectively
-            random if token symbols clash.
+            Either `pool` or `pool_metadata` must be provided.
 
     chain: str, default='mainnet'
         Identifier for blockchain or layer2.  Supported values are:
             "mainnet", "arbitrum", "optimism", "fantom", "avalanche"
             "matic", "xdai"
 
-    pool_data: PoolData, optional
-        Pool data necessary to instantiate a pool object.
+    pool_metadata: PoolMetaDataInterface, optional
+        Pool state and metadata necessary to instantiate a pool object.
 
         .. note::
-            Either `pool` or `pool_data` must be provided.
+            Either `pool` or `pool_metadata` must be provided.
+
+    pool_data_cache: PoolDataCache, optional
+        Cached data used in sims.  Useful for replication of results and
+        avoiding re-fetches of data.
 
     A: int or iterable of int, optional
         Amplification coefficient.  This controls the curvature of the
         stableswap bonding curve.  Increased values makes the curve
         flatter in a greater neighborhood of equal balances.
 
         Defaults to ``[int(2 ** (a / 2)) for a in range(12, 28)]``.
@@ -99,15 +99,15 @@
 
             {"A": [100, 1000], "fee": [3000000, 4000000]}
 
     days: int, default=60
         Number of days to fetch data for.
 
     src: str, default='coingecko'
-        Valid values for data source are 'coingecko', 'nomics', or 'local'
+        Valid values for data source are 'coingecko' or 'local'
 
     data_dir: str, default='data'
         Relative path to saved data folder.
 
     vol_mult : float or numpy.ndarray, default computed from data
         Value(s) multiplied by market volume to specify volume limits
         (overrides vol_mode).
@@ -125,21 +125,25 @@
         Number of cores to use.
 
     Returns
     -------
     dict
         Dictionary of results, each value being a pandas.Series.
     """
-    assert any([pool, pool_data]), "Must input 'pool' or 'pool_data'"
+    assert any([pool, pool_metadata]), "Must input 'pool' or 'pool_metadata'"
 
-    pool_data = pool_data or get_pool_data(pool, chain)
+    pool_metadata = pool_metadata or get_metadata(pool, chain)
     p_var, p_fixed, kwargs = _parse_arguments(**kwargs)
 
     results = volume_limited_arbitrage(
-        pool_data, variable_params=p_var, fixed_params=p_fixed, **kwargs
+        pool_metadata,
+        pool_data_cache,
+        variable_params=p_var,
+        fixed_params=p_fixed,
+        **kwargs,
     )
 
     return results
 
 
 def _parse_arguments(**kwargs):
     pool_args = ["A", "D", "x", "p", "fee", "fee_mul", "tokens", "admin_fee"]
```

### Comparing `curvesim-0.3.0rc1/curvesim.egg-info/PKG-INFO` & `curvesim-0.4.0a1/curvesim.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curvesim
-Version: 0.3.0rc1
+Version: 0.4.0a1
 Summary: Simulate Curve pools
 Home-page: https://github.com/curveresearch/curvesim
 Author: Curve Research
 Author-email: help@curveresearch.org
 License: MIT
 Project-URL: Documentation, https://curvesim.readthedocs.io
 Project-URL: Source, https://github.com/curveresearch/curvesim
@@ -26,51 +26,53 @@
 
 [![image](https://img.shields.io/pypi/v/curvesim.svg)](https://pypi.org/project/curvesim/)
 [![image](https://img.shields.io/pypi/l/curvesim.svg)](https://pypi.org/project/curvesim/)
 [![image](https://img.shields.io/pypi/pyversions/curvesim.svg)](https://pypi.org/project/curvesim/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![CI](https://github.com/curveresearch/curvesim/actions/workflows/CI.yml/badge.svg)](https://github.com/curveresearch/curvesim/actions/workflows/CI.yml)
 [![Docs](https://readthedocs.org/projects/curvesim/badge/?version=latest)](https://curvesim.readthedocs.io/en/latest)
+![badge](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/chanhosuh/3da3c072e081f4509ebdd09c63e6ede5/raw/curvesim_coverage_badge.json)
 
 
 # Curvesim
 Curvesim simulates Curve finance pools with optimal arbitrageurs trading against them. It's primary use is to determine optimal amplitude (A) and fee parameters given historical price and volume feeds.
 
 #### Dependencies:
 The maintainers use Python 3.8 or above, but 3.11 is not yet supported.  The code is likely fine for 3.6 and 3.7 but not officially supported.
 
-Primary package dependencies: scipy, numpy, pandas, Web3, matplotlib, requests, gmpy2
+Primary package dependencies: scipy, numpy, pandas, altair, matplotlib, requests, web3, gmpy2
 
-When working on the codebase, to avoid dependency issues it is recommended to use the included `requirements.txt` file in a Python virtual environment (`venv`).
+When working on the codebase, to avoid dependency issues it is recommended to use the included `requirements.txt` file in a Python virtual environment (`venv`).  Python 3.10 is required for this.
 
 
 ## Documentation
 Check out the full documentation at https://curvesim.readthedocs.io/
 
 ## Licensing
-Portions of the codebase are authorized derivatives of code owned by Curve.fi (Swiss Stake GbmH).  These are the vyper snippets used for testing (`test/fixtures/curve`) and the python code derived from them (`curvesim/pool/stableswap`); there are copyright notices placed appropriately.  The rest of the codebase has an MIT license.
+Portions of the codebase are authorized derivatives of code owned by Curve.fi (Swiss Stake GmbH).  These are the vyper snippets used for testing (`test/fixtures/curve`) and the python code derived from them (`curvesim/pool/stableswap` and `curvesim/pool/cryptoswap`); there are copyright notices placed appropriately.  The rest of the codebase has an MIT license.
 
 ## Basic Use: Autosim
-The autosim() function simulates existing Curve pools with a range of A and/or fee parameters. The function fetches pool properties (e.g., current pool size) and 2 months of price/volume data, runs multiple simulations in parallel, and saves results plots to the "results" directory. 
+The autosim() function simulates existing Curve pools with a range of A and/or fee parameters. The function fetches pool properties (e.g., current pool size) and 2 months of price/volume data, runs multiple simulations in parallel, and returns a results object that can be introspected or generate charts.
 
 Curve pools from any chain supported by the [Convex Community Subgraphs](https://thegraph.com/hosted-service/subgraph/convex-community/volume-mainnet) can be simulated directly by inputting the pool's address or symbol. For factory pools, the pool and LP token use the same symbol. For earlier pools, we use the LP token symbol.
 
 ### Example:
-For example, to simulate 3pool with the default configuration, you could use either its address or the '3crv' LP token symbol (both are case-insensitive):
+To simulate 3pool with the default configuration:
 
 ```python
 import curvesim
 res = curvesim.autosim("0xbEbc44782C7dB0a1A60Cb6fe97d0b483032FF1C7")
-res = curvesim.autosim("3crv")
 ```
 
 To simulate pools on chains other than Ethereum, use the "chain" argument:
+
 ```python
 import curvesim
-res = curvesim.autosim("2crv", chain="arbitrum")
+# run sim on Arbitrum 2Crv
+res = curvesim.autosim("0x7f90122BF0700F9E7e1F688fe926940E8839F353", chain="arbitrum")
 ```
 
 
 ### Results:
 Plots of the results will be saved to the "results/poolname" (e.g., pools/3crv) directory. The output dictionary, "res", contains pandas dataframes for all of the data plotted in the figures:
 
 * **ar**: annualized returns
@@ -96,51 +98,50 @@
 Custom A and fee ranges can be specified using the "A" and "fee" arguments. Inputs must be lists or numpy arrays containing lists:
 
 ```python
 import curvesim
 import numpy as np
 
 #Specify A values:
-res = curvesim.autosim('3crv', A=range(1000,2001,100))
+res = curvesim.autosim('0xbEbc44782C7dB0a1A60Cb6fe97d0b483032FF1C7', A=range(1000,2001,100))
 
 #Specify fees (0.03% and 0.04% with 10 decimal precision):
-res = curvesim.autosim('3crv', fee=[3000000, 4000000])
+res = curvesim.autosim('0xbEbc44782C7dB0a1A60Cb6fe97d0b483032FF1C7', fee=[3000000, 4000000])
 
 #Specify custom A range and 0.03% fee
-#Note that single fee must still be a list
-res = curvesim.autosim('3crv', A=range(1000,2001,100), fee=3000000)
+res = curvesim.autosim('0xbEbc44782C7dB0a1A60Cb6fe97d0b483032FF1C7', A=range(1000,2001,100), fee=3000000)
 ```
 Additionally, a small number of A/fee values (2 each) can be set for testing purposes: 
 ```python
-res = curvesim.autosim('3crv', test=True)
+res = curvesim.autosim('0xbEbc44782C7dB0a1A60Cb6fe97d0b483032FF1C7', test=True)
 ```
 
 
 ### Overriding Simulation Parameters
 The following parameters are automatically specified by autosim(), but can be overridden with keyword arguments:
 * **D**: total deposit size; default: fetched from on-chain data
 * **vol_mult**: multiplied by market volume to produce trade size limits; default: computed from Curve Subraph data (see Volume Limits for details)
 * **feemul**: fee multiplier used in dynamic fee pools; default: specified in poolDF_\*.csv
 
 ```python
 import curvesim
 
 #Simulate 3pool assuming total deposit of $10B, fee = 0.03%
-res = curvesim.autosim('3crv', D=10000000000, fee=3000000)
+res = curvesim.autosim('0xbEbc44782C7dB0a1A60Cb6fe97d0b483032FF1C7', D=10000000000, fee=3000000)
 
 #For metapools, specifying D effects the deposit in the metapool, but not the basepool
 #Simulate USDN metapool assuming total deposit of $1B, fee = 0.03%
-res = curvesim.autosim('usdn3crv', D=1000000000, fee=3000000)
+res = curvesim.autosim('0x0f9cb53Ebe405d49A0bbdBD291A65Ff571bC83e1', D=1000000000, fee=3000000)
 
 #Simulate 3pool, limiting volume to 75% of market volume, fee = 0.03% 
 #Note: it is not reccomended to adjust this parameter, try vol_mode instead (see below)
-res = curvesim.autosim('3crv', vol_mult=.75, fee=3000000)
+res = curvesim.autosim('0xbEbc44782C7dB0a1A60Cb6fe97d0b483032FF1C7', vol_mult=.75, fee=3000000)
 
 #Simulate hypothetical 3pool with dynamic fee like AAVE pool, fee = 0.03% 
-res = curvesim.autosim('3crv', feemul=2*10**10, fee=3000000)
+res = curvesim.autosim('0xbEbc44782C7dB0a1A60Cb6fe97d0b483032FF1C7', feemul=2*10**10, fee=3000000)
 ```
 
 ### Volume Limits
 To approximate realistic market conditions, the "vol_mult" argument is used to limit trade volume at each timepoint in the simulation. By default (vol_mode=1), vol_mult is simply the expected proportion of market volume that goes through the Curve pool (e.g., monthly pool volume / monthly price feed volume). At each timepoint, vol_mult is multiplied by the each coin-pair's market volume to produce a volume limit for each pair, thereby appropriately scaling trade volume while retaining natural volume dynamics. For metapools, vol_mult is computed seperately for the base pool and meta-pool.
 
 In some cases, it may be helpful to limit trade volume differently. In particular, for new coins with little volume for some (but not all) pairs included in the pool, more robust simulations can be achieved by assuming equal volumes across trading pairs. We therefore provide three volume-limiting modes (vol_mode):
 
@@ -149,19 +150,18 @@
 * **vol_mode = 3**: mode 2 for trades with meta-pool asset, mode 1 for basepool-only trades
 
 We reccomend using the default vol_mode 1 in most cases. However, if that returns noisy/uninterpretable results, it may be worth trying mode 2 (for normal pools) or mode 3 (for meta-pools).
 
 ### Data Sources
 The "src" argument can be used to choose between 3 different data sources:
 * **src = "coingecko"**: CoinGecko API (free); default
-* **src = "nomics"**: Nomics API (paid); set `NOMICS_API_KEY` as env variable or in `.env` file.
 * **src = "local"**: local data stored in the "data" folder
 
-#### Note on CoinGecko vs. Nomics Data
-While Nomics provides 30-minute-interval data for each specific coin-pair, CoinGecko provides prices *per coin* in 1-hour intervals. Each coin's price is computed relative to all its trading pairs and converted to a quote currency (e.g., USD), with volume summed across all trading pairs. Therefore, market volume taken from CoinGecko is often much higher than one can expect for a specific coin-pair. This issue is largely ameloriated by our volume limiting approach, with CoinGecko results typically mirroring Nomics results qualitatively, but it should be noted that CoinGecko data may be less reliable than Nomics data for certain simulations.
+Note that Nomics data is no longer supported since they went out of service.
 
-For comparison, compare 3pool_cg and 3pool_nomics results in the pools/demo direectory.
+#### Note on CoinGecko Data
+Coingecko price/volume data is computed using all trading pairs for each coin, with volume summed across all pairs. Therefore, market volume taken from CoinGecko can be much higher than that of any specific trading pair used in a simulation. This issue is largely ameloriated by our volume limiting approach, with CoinGecko results typically mirroring results from pairwise data, but it should be noted that CoinGecko data may be less reliable than more granular data for certain simulations.
 
 ### Technical Parameters
 Additionally, one can specify:
 * **ncpu**: number of CPUs to use for parallel processing (default: all cores); for use with profilers, e.g. `cProfile`, use `ncpu=1`.
 * **days**: the number of days worth of data to use in the simulation (default: 60)
```

### Comparing `curvesim-0.3.0rc1/curvesim.egg-info/SOURCES.txt` & `curvesim-0.4.0a1/curvesim.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE.md
 README.md
 pyproject.toml
 setup.cfg
 curvesim/__init__.py
 curvesim/__main__.py
+curvesim/logging.py
 curvesim/utils.py
 curvesim/version.py
 curvesim.egg-info/PKG-INFO
 curvesim.egg-info/SOURCES.txt
 curvesim.egg-info/dependency_links.txt
 curvesim.egg-info/requires.txt
 curvesim.egg-info/top_level.txt
@@ -15,40 +16,74 @@
 curvesim/_order_book/__init__.py
 curvesim/exceptions/__init__.py
 curvesim/iterators/__init__.py
 curvesim/iterators/param_samplers/__init__.py
 curvesim/iterators/param_samplers/grid.py
 curvesim/iterators/price_samplers/__init__.py
 curvesim/iterators/price_samplers/price_volume.py
+curvesim/metrics/__init__.py
+curvesim/metrics/base.py
+curvesim/metrics/metrics.py
+curvesim/metrics/results/__init__.py
+curvesim/metrics/results/make_results.py
+curvesim/metrics/results/sim_results.py
+curvesim/metrics/state_log/__init__.py
+curvesim/metrics/state_log/log.py
+curvesim/metrics/state_log/pool_parameters.py
+curvesim/metrics/state_log/pool_state.py
 curvesim/network/__init__.py
 curvesim/network/coingecko.py
 curvesim/network/http.py
 curvesim/network/llamaAPI.py
 curvesim/network/nomics.py
 curvesim/network/subgraph.py
 curvesim/network/utils.py
 curvesim/network/web3.py
 curvesim/overrides/__init__.py
 curvesim/pipelines/__init__.py
 curvesim/pipelines/arbitrage.py
 curvesim/pipelines/templates.py
 curvesim/pipelines/utils.py
 curvesim/plot/__init__.py
-curvesim/plot/legacy.py
+curvesim/plot/result_plotter.py
+curvesim/plot/altair/__init__.py
+curvesim/plot/altair/chart_properties.py
+curvesim/plot/altair/make_chart.py
+curvesim/plot/altair/selectors.py
+curvesim/plot/altair/styles.py
 curvesim/pool/__init__.py
 curvesim/pool/base.py
+curvesim/pool/snapshot.py
+curvesim/pool/cryptoswap/__init__.py
+curvesim/pool/cryptoswap/pool.py
+curvesim/pool/sim_interface/__init__.py
+curvesim/pool/sim_interface/metapool.py
+curvesim/pool/sim_interface/pool.py
+curvesim/pool/sim_interface/raipool.py
+curvesim/pool/sim_interface/simpool.py
 curvesim/pool/stableswap/__init__.py
-curvesim/pool/stableswap/functions.py
-curvesim/pool/stableswap/interfaces.py
 curvesim/pool/stableswap/metapool.py
 curvesim/pool/stableswap/pool.py
 curvesim/pool/stableswap/raipool.py
 curvesim/pool_data/__init__.py
+curvesim/pool_data/cache.py
 curvesim/pool_data/queries.py
+curvesim/pool_data/metadata/__init__.py
+curvesim/pool_data/metadata/base.py
+curvesim/pool_data/metadata/cryptoswap.py
+curvesim/pool_data/metadata/stableswap.py
 curvesim/price_data/__init__.py
 curvesim/price_data/sources.py
 curvesim/sim/__init__.py
 test/fixtures/__init__.py
 test/fixtures/pool.py
+test/integration/__init__.py
+test/integration/test_subgraph.py
+test/scripts/__init__.py
+test/scripts/make_test_data.py
 test/unit/__init__.py
+test/unit/test_cryptopool.py
 test/unit/test_metapool.py
-test/unit/test_pool.py
+test/unit/test_pool.py
+test/unit/test_pool_metadata.py
+test/unit/test_sim_stableswap.py
+test/unit/test_snapshot.py
```

### Comparing `curvesim-0.3.0rc1/setup.cfg` & `curvesim-0.4.0a1/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.3.0.rc1
+current_version = 0.4.0.a1
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\.(?P<release>.*)(?P<build>\d+))?
 serialize = 
 	{major}.{minor}.{patch}.{release}{build}
 	{major}.{minor}.{patch}
 commit = True
 tag = True
 
@@ -77,14 +77,15 @@
 	scipy >= 1.9.3
 	gmpy2 >= 2.1.2
 	matplotlib >= 3.5.3
 	web3 >= 6.0.0b4
 	requests >= 2.28.1
 	tenacity >= 8.1.0
 	python-dotenv>=0.21.0
+	altair>=5.0.0
 
 [options.packages.find]
 exclude = 
 	.github
 	data
 	git_hooks
 	results
```

### Comparing `curvesim-0.3.0rc1/test/unit/test_metapool.py` & `curvesim-0.4.0a1/test/unit/test_metapool.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,46 @@
+"""Unit tests for CurveMetaPool"""
 import pytest
 from hypothesis import HealthCheck, assume, given, settings
 from hypothesis import strategies as st
 
 from curvesim.pool import CurveMetaPool, CurvePool
 
 from .test_pool import initialize_pool
 
 
 def convert_to_virtual_balances(rates, balances):
+    """Convert from native token units to D units."""
     return [b * p // 10**18 for b, p in zip(balances, rates)]
 
 
 def convert_to_real_balances(rates, balances):
+    """Convert from D units to native token units."""
     return [b * 10**18 // p for b, p in zip(balances, rates)]
 
 
 def initialize_metapool(vyper_metapool, vyper_3pool):
     """
     Initialize python-based pool from the state variables of the
     vyper-based implementation.
     """
     A = vyper_metapool.A()
     n_coins = vyper_metapool.N_COINS()
     balances = [vyper_metapool.balances(i) for i in range(n_coins)]
-    p = [vyper_metapool.rates(i) for i in range(n_coins)]
     lp_total_supply = vyper_metapool.totalSupply()
     fee = vyper_metapool.fee()
     admin_fee = vyper_metapool.admin_fee()
+    rate_multiplier = vyper_metapool.rate_multiplier()
     basepool = initialize_pool(vyper_3pool)
     metapool = CurveMetaPool(
         A,
         D=balances,
         n=n_coins,
         basepool=basepool,
-        p=p,
+        rate_multiplier=rate_multiplier,
         tokens=lp_total_supply,
         fee=fee,
         admin_fee=admin_fee,
     )
     return metapool
 
 
@@ -119,16 +122,16 @@
 def test_get_y_D(vyper_metapool, vyper_3pool, dx, i, j):
     """Test y calculation against vyper implementation"""
     assume(i != j)
 
     python_metapool = initialize_metapool(vyper_metapool, vyper_3pool)
     A = python_metapool.A
     D = python_metapool.D()
-    rates = python_metapool.rates()
-    balances = python_metapool.x
+    rates = python_metapool.rates
+    balances = python_metapool.balances
     vyper_balances = [vyper_metapool.balances(i) for i in range(2)]
     assert balances == vyper_balances
     virtual_balances = convert_to_virtual_balances(rates, balances)
 
     virtual_balances[j] += dx
 
     # Need `eval` since this function is internal.
@@ -173,27 +176,25 @@
     python_metapool = initialize_metapool(vyper_metapool, vyper_3pool)
 
     _balances = [x0, x1]
     rates = [vyper_metapool.rates(i) for i in range(len(_balances))]
     amounts = convert_to_real_balances(rates, _balances)
 
     old_vyper_balances = [vyper_metapool.balances(i) for i in range(len(_balances))]
-    balances = python_metapool.x
-    assert balances == old_vyper_balances
+    assert python_metapool.balances == old_vyper_balances
 
-    lp_total_supply = vyper_metapool.totalSupply()
-    vyper_metapool.add_liquidity(amounts, 0)
-    expected_lp_amount = vyper_metapool.totalSupply() - lp_total_supply
+    expected_lp_amount = vyper_metapool.add_liquidity(amounts, 0)
+    expected_balances = [vyper_metapool.balances(i) for i in range(len(_balances))]
+    expected_lp_supply = vyper_metapool.totalSupply()
 
     lp_amount = python_metapool.add_liquidity(amounts)
-    assert lp_amount == expected_lp_amount
 
-    expected_balances = [vyper_metapool.balances(i) for i in range(len(_balances))]
-    new_balances = python_metapool.x
-    assert new_balances == expected_balances
+    assert lp_amount == expected_lp_amount
+    assert python_metapool.tokens == expected_lp_supply
+    assert python_metapool.balances == expected_balances
 
 
 @given(
     positive_balance,
     st.integers(min_value=0, max_value=1),
     st.integers(min_value=0, max_value=1),
 )
@@ -205,27 +206,27 @@
 def test_exchange(vyper_metapool, vyper_3pool, dx, i, j):
     """Test `exchange` against vyper implementation."""
     assume(i != j)
 
     python_metapool = initialize_metapool(vyper_metapool, vyper_3pool)
 
     old_vyper_balances = [vyper_metapool.balances(i) for i in range(2)]
-    balances = python_metapool.x
+    balances = python_metapool.balances
     assert balances == old_vyper_balances
 
     # convert to real units
     dx = dx * 10**18 // vyper_metapool.rates(i)
 
     expected_dy = vyper_metapool.exchange(i, j, dx, 0)
     dy, _ = python_metapool.exchange(i, j, dx)
 
     assert dy == expected_dy
 
     expected_balances = [vyper_metapool.balances(i) for i in range(2)]
-    new_balances = python_metapool.x
+    new_balances = python_metapool.balances
     assert new_balances == expected_balances
 
 
 @given(
     positive_balance,
     st.integers(min_value=0, max_value=3),
     st.integers(min_value=0, max_value=3),
@@ -240,19 +241,19 @@
     assume(i != j)
 
     python_metapool = initialize_metapool(vyper_metapool, vyper_3pool)
     python_basepool = python_metapool.basepool
 
     # check metapool balances
     old_vyper_balances = [vyper_metapool.balances(i) for i in range(2)]
-    balances = python_metapool.x
+    balances = python_metapool.balances
     assert balances == old_vyper_balances
     # check basepool balances
     old_vyper_balances = [vyper_3pool.balances(i) for i in range(3)]
-    balances = python_basepool.x
+    balances = python_basepool.balances
     assert balances == old_vyper_balances
 
     # convert to real units
     if i == 0:
         dx = dx * 10**18 // vyper_metapool.rates(0)
     else:
         base_i = i - 1
@@ -261,19 +262,19 @@
     expected_dy = vyper_metapool.exchange_underlying(i, j, dx, 0)
     dy, _ = python_metapool.exchange_underlying(i, j, dx)
 
     assert dy == expected_dy
 
     # check metapool balances
     expected_balances = [vyper_metapool.balances(i) for i in range(2)]
-    new_balances = python_metapool.x
+    new_balances = python_metapool.balances
     assert new_balances == expected_balances
     # check basepool balances
     expected_balances = [vyper_3pool.balances(i) for i in range(3)]
-    new_balances = python_basepool.x
+    new_balances = python_basepool.balances
     assert new_balances == expected_balances
 
 
 @given(positive_balance, st.integers(min_value=0, max_value=1))
 @settings(
     suppress_health_check=[HealthCheck.function_scoped_fixture],
     max_examples=5,
@@ -299,27 +300,27 @@
 def test_remove_liquidity_one_coin(vyper_metapool, vyper_3pool, amount, i):
     """Test `remove_liquidity_one_coin` against vyper implementation."""
     assume(amount < vyper_metapool.totalSupply())
 
     python_metapool = initialize_metapool(vyper_metapool, vyper_3pool)
 
     old_vyper_balances = [vyper_metapool.balances(i) for i in range(2)]
-    balances = python_metapool.x
+    balances = python_metapool.balances
     assert balances == old_vyper_balances
 
     old_vyper_supply = vyper_metapool.totalSupply()
     lp_supply = python_metapool.tokens
     assert lp_supply == old_vyper_supply
 
     vyper_metapool.remove_liquidity_one_coin(amount, i, 0)
     expected_coin_balance = vyper_metapool.balances(i)
     expected_lp_supply = vyper_metapool.totalSupply()
 
     python_metapool.remove_liquidity_one_coin(amount, i)
-    coin_balance = python_metapool.x[i]
+    coin_balance = python_metapool.balances[i]
     lp_supply = python_metapool.tokens
 
     assert coin_balance == expected_coin_balance
     assert lp_supply == expected_lp_supply
 
 
 @pytest.mark.skip(reason="WIP: various issues affecting reliabililty of test")
@@ -341,53 +342,54 @@
     """Test `dydxfee` against discrete pricing using `exchange`"""
     # don't test between base underlyers here; will be done in regular pool tests
     assume(i != j and (i == 0 or j == 0))
 
     admin_fee = 5 * 10**9
 
     base_A = 3000
-    base_p = [10**18, 10**30, 10**30]
+    base_rates = [10**18, 10**30, 10**30]
     base_balances = [b0, b1, b2]
-    base_balances = convert_to_real_balances(base_p, base_balances)
+    base_balances = convert_to_real_balances(base_rates, base_balances)
     base_n = len(base_balances)
     base_tokens = sum(base_balances)
     base_fee = 1 * 10**6
     base_fee = 0
     basepool = CurvePool(
         base_A,
         D=base_balances,
         n=base_n,
-        p=base_p,
+        rates=base_rates,
         tokens=base_tokens,
         fee=base_fee,
         admin_fee=admin_fee,
     )
 
     A = 1365
-    p = [10**18, 10**18]
+    rate_multiplier = 10**18
+    p = [rate_multiplier, 10**18]
     balances = [x0, x1]
     balances = convert_to_real_balances(p, balances)
     n = len(balances)
     tokens = sum(balances)
     fee = 4 * 10**6
     fee = 0
     metapool = CurveMetaPool(
         A,
         D=balances,
         n=n,
         basepool=basepool,
-        p=p,
+        rate_multiplier=rate_multiplier,
         tokens=tokens,
         fee=fee,
         admin_fee=admin_fee,
     )
 
     _dydx = metapool.dydxfee(i, j)
 
-    rates = p[:1] + base_p
+    rates = [rate_multiplier] + base_rates
     _dx = 10**12
     dx = _dx * 10**18 // rates[i]
     dy, _ = metapool.exchange_underlying(i, j, dx)
     _dy = dy * rates[j] // 10**18
 
     price = _dy / _dx
     # print("\n")
```

### Comparing `curvesim-0.3.0rc1/test/unit/test_pool.py` & `curvesim-0.4.0a1/test/unit/test_pool.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,31 @@
+"""Unit tests for CurvePool"""
 from hypothesis import HealthCheck, assume, given, settings
 from hypothesis import strategies as st
 
 from curvesim.pool import CurvePool
 
 
 def initialize_pool(vyper_pool):
     """
     Initialize python-based pool from the state variables of the
     vyper-based implementation.
     """
     A = vyper_pool.A()
     n_coins = vyper_pool.N_COINS()
     balances = [vyper_pool.balances(i) for i in range(n_coins)]
-    p = [vyper_pool.rates(i) for i in range(n_coins)]
+    rates = [vyper_pool.rates(i) for i in range(n_coins)]
     lp_total_supply = vyper_pool.totalSupply()
     fee = vyper_pool.fee()
     admin_fee = vyper_pool.admin_fee()
     pool = CurvePool(
         A,
         D=balances,
         n=n_coins,
-        p=p,
+        rates=rates,
         tokens=lp_total_supply,
         fee=fee,
         admin_fee=admin_fee,
     )
     return pool
 
 
@@ -94,22 +95,22 @@
 
     # create balanced pool
     balances = [
         295949605740077000000000000,
         295949605740077,
         295949605740077,
     ]
-    p = [10**18, 10**30, 10**30]
+    rates = [10**18, 10**30, 10**30]
     n_coins = 3
     A = 5858
 
-    pool = CurvePool(A, D=balances, n=n_coins, p=p)
+    pool = CurvePool(A, D=balances, n=n_coins, rates=rates)
     D = pool.D()
 
-    virtualized_balances = [b * p // 10**18 for b, p in zip(balances, p)]
+    virtualized_balances = [b * p // 10**18 for b, p in zip(balances, rates)]
     expected_D = sum(virtualized_balances)
 
     assert D == expected_D
 
 
 def test_get_virtual_price(vyper_3pool):
     """Test `get_virtual_price` against vyper implementation."""
@@ -137,15 +138,15 @@
 
 
 def test_get_y_D(vyper_3pool):
     """Test y calculation against vyper implementation"""
 
     python_3pool = initialize_pool(vyper_3pool)
     A = python_3pool.A
-    virtual_balances = python_3pool._xp()
+    virtual_balances = python_3pool._xp()  # pylint: disable=protected-access
     D = python_3pool.D()
 
     i = 0
     j = 1
     dx = 516 * 10**18
     virtual_balances[j] += dx
     expected_y = vyper_3pool.eval(f"self.get_y_D({A}, {i}, {virtual_balances}, {D})")
@@ -185,27 +186,25 @@
     python_3pool = initialize_pool(vyper_3pool)
 
     _balances = [x0, x1, x2]
     rates = [vyper_3pool.rates(i) for i in range(len(_balances))]
     amounts = [b * 10**18 // r for b, r in zip(_balances, rates)]
 
     old_vyper_balances = [vyper_3pool.balances(i) for i in range(len(_balances))]
-    balances = python_3pool.x
-    assert balances == old_vyper_balances
+    assert python_3pool.balances == old_vyper_balances
 
-    lp_total_supply = vyper_3pool.totalSupply()
-    vyper_3pool.add_liquidity(amounts, 0)
-    expected_lp_amount = vyper_3pool.totalSupply() - lp_total_supply
+    expected_lp_amount = vyper_3pool.add_liquidity(amounts, 0)
+    expected_balances = [vyper_3pool.balances(i) for i in range(len(_balances))]
+    expected_lp_supply = vyper_3pool.totalSupply()
 
     lp_amount = python_3pool.add_liquidity(amounts)
-    assert lp_amount == expected_lp_amount
 
-    expected_balances = [vyper_3pool.balances(i) for i in range(len(_balances))]
-    new_balances = python_3pool.x
-    assert new_balances == expected_balances
+    assert lp_amount == expected_lp_amount
+    assert python_3pool.tokens == expected_lp_supply
+    assert python_3pool.balances == expected_balances
 
 
 @given(
     positive_balance,
     st.integers(min_value=0, max_value=2),
     st.integers(min_value=0, max_value=2),
 )
@@ -217,27 +216,27 @@
 def test_exchange(vyper_3pool, dx, i, j):
     """Test `exchange` against vyper implementation."""
     assume(i != j)
 
     python_3pool = initialize_pool(vyper_3pool)
 
     old_vyper_balances = [vyper_3pool.balances(i) for i in range(3)]
-    balances = python_3pool.x
+    balances = python_3pool.balances
     assert balances == old_vyper_balances
 
     # convert to real units
     dx = dx * 10**18 // vyper_3pool.rates(i)
 
     expected_dy = vyper_3pool.exchange(i, j, dx, 0)
     dy, _ = python_3pool.exchange(i, j, dx)
 
     assert dy == expected_dy
 
     expected_balances = [vyper_3pool.balances(i) for i in range(3)]
-    new_balances = python_3pool.x
+    new_balances = python_3pool.balances
     assert new_balances == expected_balances
 
 
 @given(positive_balance, st.integers(min_value=0, max_value=2))
 @settings(
     suppress_health_check=[HealthCheck.function_scoped_fixture],
     max_examples=5,
@@ -263,24 +262,24 @@
 def test_remove_liquidity_one_coin(vyper_3pool, amount, i):
     """Test `remove_liquidity_one_coin` against vyper implementation."""
     assume(amount < vyper_3pool.totalSupply())
 
     python_3pool = initialize_pool(vyper_3pool)
 
     old_vyper_balances = [vyper_3pool.balances(i) for i in range(3)]
-    balances = python_3pool.x
+    balances = python_3pool.balances
     assert balances == old_vyper_balances
 
     old_vyper_supply = vyper_3pool.totalSupply()
     lp_supply = python_3pool.tokens
     assert lp_supply == old_vyper_supply
 
     vyper_3pool.remove_liquidity_one_coin(amount, i, 0)
     expected_coin_balance = vyper_3pool.balances(i)
     expected_lp_supply = vyper_3pool.totalSupply()
 
     python_3pool.remove_liquidity_one_coin(amount, i)
-    coin_balance = python_3pool.x[i]
+    coin_balance = python_3pool.balances[i]
     lp_supply = python_3pool.tokens
 
     assert coin_balance == expected_coin_balance
     assert lp_supply == expected_lp_supply
```

