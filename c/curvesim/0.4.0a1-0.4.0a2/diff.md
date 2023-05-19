# Comparing `tmp/curvesim-0.4.0a1.tar.gz` & `tmp/curvesim-0.4.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curvesim-0.4.0a1.tar", last modified: Fri May 19 21:56:54 2023, max compression
+gzip compressed data, was "curvesim-0.4.0a2.tar", last modified: Fri May 19 22:24:41 2023, max compression
```

## Comparing `curvesim-0.4.0a1.tar` & `curvesim-0.4.0a2.tar`

### file list

```diff
@@ -1,120 +1,127 @@
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.793441 curvesim-0.4.0a1/
--rw-r--r--   0 suh        (501) staff       (20)     1071 2022-11-09 15:51:57.000000 curvesim-0.4.0a1/LICENSE.md
--rw-r--r--   0 suh        (501) staff       (20)     9758 2023-05-19 21:56:54.793651 curvesim-0.4.0a1/PKG-INFO
--rw-r--r--   0 suh        (501) staff       (20)     8738 2023-05-19 21:10:12.000000 curvesim-0.4.0a1/README.md
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.736475 curvesim-0.4.0a1/curvesim/
--rw-r--r--   0 suh        (501) staff       (20)      281 2023-03-06 16:00:39.000000 curvesim-0.4.0a1/curvesim/__init__.py
--rw-r--r--   0 suh        (501) staff       (20)      427 2023-04-07 15:09:59.000000 curvesim-0.4.0a1/curvesim/__main__.py
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.740067 curvesim-0.4.0a1/curvesim/_bonding_curve/
--rw-r--r--   0 suh        (501) staff       (20)     2391 2023-05-17 21:31:12.000000 curvesim-0.4.0a1/curvesim/_bonding_curve/__init__.py
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.740622 curvesim-0.4.0a1/curvesim/_order_book/
--rw-r--r--   0 suh        (501) staff       (20)     3600 2023-01-20 15:19:10.000000 curvesim-0.4.0a1/curvesim/_order_book/__init__.py
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.741107 curvesim-0.4.0a1/curvesim/exceptions/
--rw-r--r--   0 suh        (501) staff       (20)     1466 2023-05-19 14:49:10.000000 curvesim-0.4.0a1/curvesim/exceptions/__init__.py
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.741559 curvesim-0.4.0a1/curvesim/iterators/
--rw-r--r--   0 suh        (501) staff       (20)      408 2022-11-12 00:31:20.000000 curvesim-0.4.0a1/curvesim/iterators/__init__.py
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.742500 curvesim-0.4.0a1/curvesim/iterators/param_samplers/
--rw-r--r--   0 suh        (501) staff       (20)      116 2022-11-09 14:28:48.000000 curvesim-0.4.0a1/curvesim/iterators/param_samplers/__init__.py
--rw-r--r--   0 suh        (501) staff       (20)     3358 2023-05-17 18:59:58.000000 curvesim-0.4.0a1/curvesim/iterators/param_samplers/grid.py
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.744058 curvesim-0.4.0a1/curvesim/iterators/price_samplers/
--rw-r--r--   0 suh        (501) staff       (20)      153 2022-11-09 14:28:48.000000 curvesim-0.4.0a1/curvesim/iterators/price_samplers/__init__.py
--rw-r--r--   0 suh        (501) staff       (20)     2620 2023-05-19 14:49:10.000000 curvesim-0.4.0a1/curvesim/iterators/price_samplers/price_volume.py
--rw-r--r--   0 suh        (501) staff       (20)     3394 2023-05-19 14:49:10.000000 curvesim-0.4.0a1/curvesim/logging.py
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.746388 curvesim-0.4.0a1/curvesim/metrics/
--rw-r--r--   0 suh        (501) staff       (20)     1542 2023-05-17 18:59:58.000000 curvesim-0.4.0a1/curvesim/metrics/__init__.py
--rw-r--r--   0 suh        (501) staff       (20)    13007 2023-05-19 21:10:12.000000 curvesim-0.4.0a1/curvesim/metrics/base.py
--rw-r--r--   0 suh        (501) staff       (20)    16984 2023-05-19 21:10:12.000000 curvesim-0.4.0a1/curvesim/metrics/metrics.py
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.748311 curvesim-0.4.0a1/curvesim/metrics/results/
--rw-r--r--   0 suh        (501) staff       (20)      215 2023-05-19 21:10:12.000000 curvesim-0.4.0a1/curvesim/metrics/results/__init__.py
--rw-r--r--   0 suh        (501) staff       (20)     1469 2023-05-19 21:10:12.000000 curvesim-0.4.0a1/curvesim/metrics/results/make_results.py
--rw-r--r--   0 suh        (501) staff       (20)     3805 2023-05-19 21:10:12.000000 curvesim-0.4.0a1/curvesim/metrics/results/sim_results.py
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.751945 curvesim-0.4.0a1/curvesim/metrics/state_log/
--rw-r--r--   0 suh        (501) staff       (20)      186 2023-05-19 21:10:12.000000 curvesim-0.4.0a1/curvesim/metrics/state_log/__init__.py
--rw-r--r--   0 suh        (501) staff       (20)     1861 2023-05-19 21:10:12.000000 curvesim-0.4.0a1/curvesim/metrics/state_log/log.py
--rw-r--r--   0 suh        (501) staff       (20)     1268 2023-05-19 21:10:12.000000 curvesim-0.4.0a1/curvesim/metrics/state_log/pool_parameters.py
--rw-r--r--   0 suh        (501) staff       (20)     1034 2023-05-19 21:10:12.000000 curvesim-0.4.0a1/curvesim/metrics/state_log/pool_state.py
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.758339 curvesim-0.4.0a1/curvesim/network/
--rw-r--r--   0 suh        (501) staff       (20)      459 2022-11-09 14:28:48.000000 curvesim-0.4.0a1/curvesim/network/__init__.py
--rw-r--r--   0 suh        (501) staff       (20)     6157 2022-11-12 00:31:19.000000 curvesim-0.4.0a1/curvesim/network/coingecko.py
--rw-r--r--   0 suh        (501) staff       (20)     1704 2023-04-26 15:33:34.000000 curvesim-0.4.0a1/curvesim/network/http.py
--rw-r--r--   0 suh        (501) staff       (20)     2680 2022-11-13 23:49:59.000000 curvesim-0.4.0a1/curvesim/network/llamaAPI.py
--rw-r--r--   0 suh        (501) staff       (20)    14800 2023-04-27 21:23:34.000000 curvesim-0.4.0a1/curvesim/network/nomics.py
--rw-r--r--   0 suh        (501) staff       (20)    13108 2023-05-19 19:57:52.000000 curvesim-0.4.0a1/curvesim/network/subgraph.py
--rw-r--r--   0 suh        (501) staff       (20)     1921 2023-01-20 15:19:10.000000 curvesim-0.4.0a1/curvesim/network/utils.py
--rw-r--r--   0 suh        (501) staff       (20)     4302 2023-04-25 20:54:10.000000 curvesim-0.4.0a1/curvesim/network/web3.py
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.758942 curvesim-0.4.0a1/curvesim/overrides/
--rw-r--r--   0 suh        (501) staff       (20)     1024 2022-11-12 00:31:19.000000 curvesim-0.4.0a1/curvesim/overrides/__init__.py
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.761248 curvesim-0.4.0a1/curvesim/pipelines/
--rw-r--r--   0 suh        (501) staff       (20)      501 2022-11-09 14:28:48.000000 curvesim-0.4.0a1/curvesim/pipelines/__init__.py
--rw-r--r--   0 suh        (501) staff       (20)    14384 2023-05-19 21:10:12.000000 curvesim-0.4.0a1/curvesim/pipelines/arbitrage.py
--rw-r--r--   0 suh        (501) staff       (20)     5277 2023-05-18 18:36:37.000000 curvesim-0.4.0a1/curvesim/pipelines/templates.py
--rw-r--r--   0 suh        (501) staff       (20)     2646 2023-05-17 21:31:12.000000 curvesim-0.4.0a1/curvesim/pipelines/utils.py
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.763148 curvesim-0.4.0a1/curvesim/plot/
--rw-r--r--   0 suh        (501) staff       (20)      122 2023-05-19 21:10:12.000000 curvesim-0.4.0a1/curvesim/plot/__init__.py
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.766626 curvesim-0.4.0a1/curvesim/plot/altair/
--rw-r--r--   0 suh        (501) staff       (20)      169 2023-05-19 21:10:12.000000 curvesim-0.4.0a1/curvesim/plot/altair/__init__.py
--rw-r--r--   0 suh        (501) staff       (20)     1749 2023-05-17 18:59:58.000000 curvesim-0.4.0a1/curvesim/plot/altair/chart_properties.py
--rw-r--r--   0 suh        (501) staff       (20)     1474 2023-05-17 18:59:58.000000 curvesim-0.4.0a1/curvesim/plot/altair/make_chart.py
--rw-r--r--   0 suh        (501) staff       (20)     1948 2023-05-17 18:59:58.000000 curvesim-0.4.0a1/curvesim/plot/altair/selectors.py
--rw-r--r--   0 suh        (501) staff       (20)     1001 2023-05-17 18:59:58.000000 curvesim-0.4.0a1/curvesim/plot/altair/styles.py
--rw-r--r--   0 suh        (501) staff       (20)     2132 2023-05-19 21:10:12.000000 curvesim-0.4.0a1/curvesim/plot/result_plotter.py
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.769106 curvesim-0.4.0a1/curvesim/pool/
--rw-r--r--   0 suh        (501) staff       (20)     6772 2023-05-19 14:49:10.000000 curvesim-0.4.0a1/curvesim/pool/__init__.py
--rw-r--r--   0 suh        (501) staff       (20)     2552 2023-05-17 21:31:12.000000 curvesim-0.4.0a1/curvesim/pool/base.py
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.770205 curvesim-0.4.0a1/curvesim/pool/cryptoswap/
--rw-r--r--   0 suh        (501) staff       (20)      112 2023-02-13 20:22:55.000000 curvesim-0.4.0a1/curvesim/pool/cryptoswap/__init__.py
--rw-r--r--   0 suh        (501) staff       (20)    36552 2023-05-18 17:46:09.000000 curvesim-0.4.0a1/curvesim/pool/cryptoswap/pool.py
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.773331 curvesim-0.4.0a1/curvesim/pool/sim_interface/
--rw-r--r--   0 suh        (501) staff       (20)      174 2023-01-20 15:19:10.000000 curvesim-0.4.0a1/curvesim/pool/sim_interface/__init__.py
--rw-r--r--   0 suh        (501) staff       (20)     5327 2023-05-17 21:31:12.000000 curvesim-0.4.0a1/curvesim/pool/sim_interface/metapool.py
--rw-r--r--   0 suh        (501) staff       (20)     2967 2023-05-17 21:31:12.000000 curvesim-0.4.0a1/curvesim/pool/sim_interface/pool.py
--rw-r--r--   0 suh        (501) staff       (20)     1098 2023-01-20 15:19:10.000000 curvesim-0.4.0a1/curvesim/pool/sim_interface/raipool.py
--rw-r--r--   0 suh        (501) staff       (20)     1787 2023-05-17 21:31:12.000000 curvesim-0.4.0a1/curvesim/pool/sim_interface/simpool.py
--rw-r--r--   0 suh        (501) staff       (20)     4154 2023-01-20 15:19:10.000000 curvesim-0.4.0a1/curvesim/pool/snapshot.py
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.775858 curvesim-0.4.0a1/curvesim/pool/stableswap/
--rw-r--r--   0 suh        (501) staff       (20)      267 2023-01-20 15:19:10.000000 curvesim-0.4.0a1/curvesim/pool/stableswap/__init__.py
--rw-r--r--   0 suh        (501) staff       (20)    24771 2023-05-19 21:10:12.000000 curvesim-0.4.0a1/curvesim/pool/stableswap/metapool.py
--rw-r--r--   0 suh        (501) staff       (20)    17204 2023-05-17 21:31:12.000000 curvesim-0.4.0a1/curvesim/pool/stableswap/pool.py
--rw-r--r--   0 suh        (501) staff       (20)     1502 2023-01-20 15:19:10.000000 curvesim-0.4.0a1/curvesim/pool/stableswap/raipool.py
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.777854 curvesim-0.4.0a1/curvesim/pool_data/
--rw-r--r--   0 suh        (501) staff       (20)     1574 2023-05-19 21:10:12.000000 curvesim-0.4.0a1/curvesim/pool_data/__init__.py
--rw-r--r--   0 suh        (501) staff       (20)     4790 2023-05-19 21:10:12.000000 curvesim-0.4.0a1/curvesim/pool_data/cache.py
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.780926 curvesim-0.4.0a1/curvesim/pool_data/metadata/
--rw-r--r--   0 suh        (501) staff       (20)     2376 2023-05-19 21:10:12.000000 curvesim-0.4.0a1/curvesim/pool_data/metadata/__init__.py
--rw-r--r--   0 suh        (501) staff       (20)     2618 2023-05-17 21:31:12.000000 curvesim-0.4.0a1/curvesim/pool_data/metadata/base.py
--rw-r--r--   0 suh        (501) staff       (20)     2007 2023-05-17 21:31:12.000000 curvesim-0.4.0a1/curvesim/pool_data/metadata/cryptoswap.py
--rw-r--r--   0 suh        (501) staff       (20)     2515 2023-05-17 21:31:12.000000 curvesim-0.4.0a1/curvesim/pool_data/metadata/stableswap.py
--rw-r--r--   0 suh        (501) staff       (20)     1287 2023-05-19 21:10:12.000000 curvesim-0.4.0a1/curvesim/pool_data/queries.py
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.782758 curvesim-0.4.0a1/curvesim/price_data/
--rw-r--r--   0 suh        (501) staff       (20)     1382 2023-05-19 14:49:10.000000 curvesim-0.4.0a1/curvesim/price_data/__init__.py
--rw-r--r--   0 suh        (501) staff       (20)     1586 2023-04-27 21:23:34.000000 curvesim-0.4.0a1/curvesim/price_data/sources.py
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.784405 curvesim-0.4.0a1/curvesim/sim/
--rw-r--r--   0 suh        (501) staff       (20)     6025 2023-05-19 21:10:12.000000 curvesim-0.4.0a1/curvesim/sim/__init__.py
--rw-r--r--   0 suh        (501) staff       (20)     3676 2023-05-19 14:49:10.000000 curvesim-0.4.0a1/curvesim/utils.py
--rw-r--r--   0 suh        (501) staff       (20)      361 2023-05-19 21:52:52.000000 curvesim-0.4.0a1/curvesim/version.py
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.739584 curvesim-0.4.0a1/curvesim.egg-info/
--rw-r--r--   0 suh        (501) staff       (20)     9758 2023-05-19 21:56:54.000000 curvesim-0.4.0a1/curvesim.egg-info/PKG-INFO
--rw-r--r--   0 suh        (501) staff       (20)     2764 2023-05-19 21:56:54.000000 curvesim-0.4.0a1/curvesim.egg-info/SOURCES.txt
--rw-r--r--   0 suh        (501) staff       (20)        1 2023-05-19 21:56:54.000000 curvesim-0.4.0a1/curvesim.egg-info/dependency_links.txt
--rw-r--r--   0 suh        (501) staff       (20)      155 2023-05-19 21:56:54.000000 curvesim-0.4.0a1/curvesim.egg-info/requires.txt
--rw-r--r--   0 suh        (501) staff       (20)       14 2023-05-19 21:56:54.000000 curvesim-0.4.0a1/curvesim.egg-info/top_level.txt
--rw-r--r--   0 suh        (501) staff       (20)      170 2022-11-08 18:43:56.000000 curvesim-0.4.0a1/pyproject.toml
--rw-r--r--   0 suh        (501) staff       (20)     1960 2023-05-19 21:56:54.796434 curvesim-0.4.0a1/setup.cfg
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.727281 curvesim-0.4.0a1/test/
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.785967 curvesim-0.4.0a1/test/fixtures/
--rw-r--r--   0 suh        (501) staff       (20)        0 2022-10-14 18:34:20.000000 curvesim-0.4.0a1/test/fixtures/__init__.py
--rw-r--r--   0 suh        (501) staff       (20)     5506 2023-02-13 20:22:55.000000 curvesim-0.4.0a1/test/fixtures/pool.py
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.787330 curvesim-0.4.0a1/test/integration/
--rw-r--r--   0 suh        (501) staff       (20)        0 2023-04-27 21:23:34.000000 curvesim-0.4.0a1/test/integration/__init__.py
--rw-r--r--   0 suh        (501) staff       (20)     1581 2023-05-17 21:31:12.000000 curvesim-0.4.0a1/test/integration/test_subgraph.py
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.788796 curvesim-0.4.0a1/test/scripts/
--rw-r--r--   0 suh        (501) staff       (20)        0 2023-01-20 15:19:11.000000 curvesim-0.4.0a1/test/scripts/__init__.py
--rw-r--r--   0 suh        (501) staff       (20)     4078 2023-05-17 22:06:08.000000 curvesim-0.4.0a1/test/scripts/make_test_data.py
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 21:56:54.793028 curvesim-0.4.0a1/test/unit/
--rw-r--r--   0 suh        (501) staff       (20)        0 2022-10-14 18:34:20.000000 curvesim-0.4.0a1/test/unit/__init__.py
--rw-r--r--   0 suh        (501) staff       (20)    22383 2023-05-17 21:31:12.000000 curvesim-0.4.0a1/test/unit/test_cryptopool.py
--rw-r--r--   0 suh        (501) staff       (20)    13246 2023-02-13 20:22:55.000000 curvesim-0.4.0a1/test/unit/test_metapool.py
--rw-r--r--   0 suh        (501) staff       (20)     8717 2023-03-02 16:07:35.000000 curvesim-0.4.0a1/test/unit/test_pool.py
--rw-r--r--   0 suh        (501) staff       (20)    11214 2023-05-17 21:31:12.000000 curvesim-0.4.0a1/test/unit/test_pool_metadata.py
--rw-r--r--   0 suh        (501) staff       (20)     4168 2023-05-17 18:59:58.000000 curvesim-0.4.0a1/test/unit/test_sim_stableswap.py
--rw-r--r--   0 suh        (501) staff       (20)     3531 2023-01-20 15:19:11.000000 curvesim-0.4.0a1/test/unit/test_snapshot.py
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.995117 curvesim-0.4.0a2/
+-rw-r--r--   0 suh        (501) staff       (20)     1071 2022-11-09 15:51:57.000000 curvesim-0.4.0a2/LICENSE.md
+-rw-r--r--   0 suh        (501) staff       (20)     9758 2023-05-19 22:24:41.995473 curvesim-0.4.0a2/PKG-INFO
+-rw-r--r--   0 suh        (501) staff       (20)     8738 2023-05-19 21:10:12.000000 curvesim-0.4.0a2/README.md
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.807599 curvesim-0.4.0a2/curvesim/
+-rw-r--r--   0 suh        (501) staff       (20)      281 2023-03-06 16:00:39.000000 curvesim-0.4.0a2/curvesim/__init__.py
+-rw-r--r--   0 suh        (501) staff       (20)      427 2023-04-07 15:09:59.000000 curvesim-0.4.0a2/curvesim/__main__.py
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.811215 curvesim-0.4.0a2/curvesim/_bonding_curve/
+-rw-r--r--   0 suh        (501) staff       (20)     2391 2023-05-17 21:31:12.000000 curvesim-0.4.0a2/curvesim/_bonding_curve/__init__.py
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.812066 curvesim-0.4.0a2/curvesim/_order_book/
+-rw-r--r--   0 suh        (501) staff       (20)     3600 2023-01-20 15:19:10.000000 curvesim-0.4.0a2/curvesim/_order_book/__init__.py
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.814781 curvesim-0.4.0a2/curvesim/exceptions/
+-rw-r--r--   0 suh        (501) staff       (20)     1466 2023-05-19 14:49:10.000000 curvesim-0.4.0a2/curvesim/exceptions/__init__.py
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.817026 curvesim-0.4.0a2/curvesim/iterators/
+-rw-r--r--   0 suh        (501) staff       (20)      408 2022-11-12 00:31:20.000000 curvesim-0.4.0a2/curvesim/iterators/__init__.py
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.821111 curvesim-0.4.0a2/curvesim/iterators/param_samplers/
+-rw-r--r--   0 suh        (501) staff       (20)      116 2022-11-09 14:28:48.000000 curvesim-0.4.0a2/curvesim/iterators/param_samplers/__init__.py
+-rw-r--r--   0 suh        (501) staff       (20)     3358 2023-05-17 18:59:58.000000 curvesim-0.4.0a2/curvesim/iterators/param_samplers/grid.py
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.826278 curvesim-0.4.0a2/curvesim/iterators/price_samplers/
+-rw-r--r--   0 suh        (501) staff       (20)      153 2022-11-09 14:28:48.000000 curvesim-0.4.0a2/curvesim/iterators/price_samplers/__init__.py
+-rw-r--r--   0 suh        (501) staff       (20)     2620 2023-05-19 14:49:10.000000 curvesim-0.4.0a2/curvesim/iterators/price_samplers/price_volume.py
+-rw-r--r--   0 suh        (501) staff       (20)     3394 2023-05-19 14:49:10.000000 curvesim-0.4.0a2/curvesim/logging.py
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.832631 curvesim-0.4.0a2/curvesim/metrics/
+-rw-r--r--   0 suh        (501) staff       (20)     1542 2023-05-17 18:59:58.000000 curvesim-0.4.0a2/curvesim/metrics/__init__.py
+-rw-r--r--   0 suh        (501) staff       (20)    13007 2023-05-19 21:10:12.000000 curvesim-0.4.0a2/curvesim/metrics/base.py
+-rw-r--r--   0 suh        (501) staff       (20)    16984 2023-05-19 21:10:12.000000 curvesim-0.4.0a2/curvesim/metrics/metrics.py
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.839191 curvesim-0.4.0a2/curvesim/metrics/results/
+-rw-r--r--   0 suh        (501) staff       (20)      215 2023-05-19 21:10:12.000000 curvesim-0.4.0a2/curvesim/metrics/results/__init__.py
+-rw-r--r--   0 suh        (501) staff       (20)     1469 2023-05-19 21:10:12.000000 curvesim-0.4.0a2/curvesim/metrics/results/make_results.py
+-rw-r--r--   0 suh        (501) staff       (20)     3805 2023-05-19 21:10:12.000000 curvesim-0.4.0a2/curvesim/metrics/results/sim_results.py
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.848754 curvesim-0.4.0a2/curvesim/metrics/state_log/
+-rw-r--r--   0 suh        (501) staff       (20)      186 2023-05-19 21:10:12.000000 curvesim-0.4.0a2/curvesim/metrics/state_log/__init__.py
+-rw-r--r--   0 suh        (501) staff       (20)     1861 2023-05-19 21:10:12.000000 curvesim-0.4.0a2/curvesim/metrics/state_log/log.py
+-rw-r--r--   0 suh        (501) staff       (20)     1268 2023-05-19 21:10:12.000000 curvesim-0.4.0a2/curvesim/metrics/state_log/pool_parameters.py
+-rw-r--r--   0 suh        (501) staff       (20)     1034 2023-05-19 21:10:12.000000 curvesim-0.4.0a2/curvesim/metrics/state_log/pool_state.py
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.864543 curvesim-0.4.0a2/curvesim/network/
+-rw-r--r--   0 suh        (501) staff       (20)      459 2022-11-09 14:28:48.000000 curvesim-0.4.0a2/curvesim/network/__init__.py
+-rw-r--r--   0 suh        (501) staff       (20)     6157 2022-11-12 00:31:19.000000 curvesim-0.4.0a2/curvesim/network/coingecko.py
+-rw-r--r--   0 suh        (501) staff       (20)     1704 2023-04-26 15:33:34.000000 curvesim-0.4.0a2/curvesim/network/http.py
+-rw-r--r--   0 suh        (501) staff       (20)     2680 2022-11-13 23:49:59.000000 curvesim-0.4.0a2/curvesim/network/llamaAPI.py
+-rw-r--r--   0 suh        (501) staff       (20)    14800 2023-04-27 21:23:34.000000 curvesim-0.4.0a2/curvesim/network/nomics.py
+-rw-r--r--   0 suh        (501) staff       (20)    13108 2023-05-19 19:57:52.000000 curvesim-0.4.0a2/curvesim/network/subgraph.py
+-rw-r--r--   0 suh        (501) staff       (20)     1921 2023-01-20 15:19:10.000000 curvesim-0.4.0a2/curvesim/network/utils.py
+-rw-r--r--   0 suh        (501) staff       (20)     4302 2023-04-25 20:54:10.000000 curvesim-0.4.0a2/curvesim/network/web3.py
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.866428 curvesim-0.4.0a2/curvesim/overrides/
+-rw-r--r--   0 suh        (501) staff       (20)     1024 2022-11-12 00:31:19.000000 curvesim-0.4.0a2/curvesim/overrides/__init__.py
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.873692 curvesim-0.4.0a2/curvesim/pipelines/
+-rw-r--r--   0 suh        (501) staff       (20)      501 2022-11-09 14:28:48.000000 curvesim-0.4.0a2/curvesim/pipelines/__init__.py
+-rw-r--r--   0 suh        (501) staff       (20)    14384 2023-05-19 21:10:12.000000 curvesim-0.4.0a2/curvesim/pipelines/arbitrage.py
+-rw-r--r--   0 suh        (501) staff       (20)     5277 2023-05-18 18:36:37.000000 curvesim-0.4.0a2/curvesim/pipelines/templates.py
+-rw-r--r--   0 suh        (501) staff       (20)     2646 2023-05-17 21:31:12.000000 curvesim-0.4.0a2/curvesim/pipelines/utils.py
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.881693 curvesim-0.4.0a2/curvesim/plot/
+-rw-r--r--   0 suh        (501) staff       (20)      122 2023-05-19 21:10:12.000000 curvesim-0.4.0a2/curvesim/plot/__init__.py
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.907373 curvesim-0.4.0a2/curvesim/plot/altair/
+-rw-r--r--   0 suh        (501) staff       (20)      169 2023-05-19 21:10:12.000000 curvesim-0.4.0a2/curvesim/plot/altair/__init__.py
+-rw-r--r--   0 suh        (501) staff       (20)     1749 2023-05-17 18:59:58.000000 curvesim-0.4.0a2/curvesim/plot/altair/chart_properties.py
+-rw-r--r--   0 suh        (501) staff       (20)     1474 2023-05-17 18:59:58.000000 curvesim-0.4.0a2/curvesim/plot/altair/make_chart.py
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.920390 curvesim-0.4.0a2/curvesim/plot/altair/results/
+-rw-r--r--   0 suh        (501) staff       (20)        0 2023-05-19 22:22:27.000000 curvesim-0.4.0a2/curvesim/plot/altair/results/__init__.py
+-rw-r--r--   0 suh        (501) staff       (20)     3083 2023-05-17 18:59:58.000000 curvesim-0.4.0a2/curvesim/plot/altair/results/make_page.py
+-rw-r--r--   0 suh        (501) staff       (20)     1558 2023-05-17 18:59:58.000000 curvesim-0.4.0a2/curvesim/plot/altair/results/preprocessing.py
+-rw-r--r--   0 suh        (501) staff       (20)     1618 2023-05-19 21:10:12.000000 curvesim-0.4.0a2/curvesim/plot/altair/results/result_plotter.py
+-rw-r--r--   0 suh        (501) staff       (20)     2597 2023-05-19 21:47:18.000000 curvesim-0.4.0a2/curvesim/plot/altair/results/result_selectors.py
+-rw-r--r--   0 suh        (501) staff       (20)      436 2023-05-17 18:59:58.000000 curvesim-0.4.0a2/curvesim/plot/altair/results/tooltip.py
+-rw-r--r--   0 suh        (501) staff       (20)     1948 2023-05-17 18:59:58.000000 curvesim-0.4.0a2/curvesim/plot/altair/selectors.py
+-rw-r--r--   0 suh        (501) staff       (20)     1001 2023-05-17 18:59:58.000000 curvesim-0.4.0a2/curvesim/plot/altair/styles.py
+-rw-r--r--   0 suh        (501) staff       (20)     2132 2023-05-19 21:10:12.000000 curvesim-0.4.0a2/curvesim/plot/result_plotter.py
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.926321 curvesim-0.4.0a2/curvesim/pool/
+-rw-r--r--   0 suh        (501) staff       (20)     6772 2023-05-19 14:49:10.000000 curvesim-0.4.0a2/curvesim/pool/__init__.py
+-rw-r--r--   0 suh        (501) staff       (20)     2552 2023-05-17 21:31:12.000000 curvesim-0.4.0a2/curvesim/pool/base.py
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.930644 curvesim-0.4.0a2/curvesim/pool/cryptoswap/
+-rw-r--r--   0 suh        (501) staff       (20)      112 2023-02-13 20:22:55.000000 curvesim-0.4.0a2/curvesim/pool/cryptoswap/__init__.py
+-rw-r--r--   0 suh        (501) staff       (20)    36552 2023-05-18 17:46:09.000000 curvesim-0.4.0a2/curvesim/pool/cryptoswap/pool.py
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.943349 curvesim-0.4.0a2/curvesim/pool/sim_interface/
+-rw-r--r--   0 suh        (501) staff       (20)      174 2023-01-20 15:19:10.000000 curvesim-0.4.0a2/curvesim/pool/sim_interface/__init__.py
+-rw-r--r--   0 suh        (501) staff       (20)     5327 2023-05-17 21:31:12.000000 curvesim-0.4.0a2/curvesim/pool/sim_interface/metapool.py
+-rw-r--r--   0 suh        (501) staff       (20)     2967 2023-05-17 21:31:12.000000 curvesim-0.4.0a2/curvesim/pool/sim_interface/pool.py
+-rw-r--r--   0 suh        (501) staff       (20)     1098 2023-01-20 15:19:10.000000 curvesim-0.4.0a2/curvesim/pool/sim_interface/raipool.py
+-rw-r--r--   0 suh        (501) staff       (20)     1787 2023-05-17 21:31:12.000000 curvesim-0.4.0a2/curvesim/pool/sim_interface/simpool.py
+-rw-r--r--   0 suh        (501) staff       (20)     4154 2023-01-20 15:19:10.000000 curvesim-0.4.0a2/curvesim/pool/snapshot.py
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.954135 curvesim-0.4.0a2/curvesim/pool/stableswap/
+-rw-r--r--   0 suh        (501) staff       (20)      267 2023-01-20 15:19:10.000000 curvesim-0.4.0a2/curvesim/pool/stableswap/__init__.py
+-rw-r--r--   0 suh        (501) staff       (20)    24771 2023-05-19 21:10:12.000000 curvesim-0.4.0a2/curvesim/pool/stableswap/metapool.py
+-rw-r--r--   0 suh        (501) staff       (20)    17204 2023-05-17 21:31:12.000000 curvesim-0.4.0a2/curvesim/pool/stableswap/pool.py
+-rw-r--r--   0 suh        (501) staff       (20)     1502 2023-01-20 15:19:10.000000 curvesim-0.4.0a2/curvesim/pool/stableswap/raipool.py
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.959305 curvesim-0.4.0a2/curvesim/pool_data/
+-rw-r--r--   0 suh        (501) staff       (20)     1574 2023-05-19 21:10:12.000000 curvesim-0.4.0a2/curvesim/pool_data/__init__.py
+-rw-r--r--   0 suh        (501) staff       (20)     4790 2023-05-19 21:10:12.000000 curvesim-0.4.0a2/curvesim/pool_data/cache.py
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.968252 curvesim-0.4.0a2/curvesim/pool_data/metadata/
+-rw-r--r--   0 suh        (501) staff       (20)     2376 2023-05-19 21:10:12.000000 curvesim-0.4.0a2/curvesim/pool_data/metadata/__init__.py
+-rw-r--r--   0 suh        (501) staff       (20)     2618 2023-05-17 21:31:12.000000 curvesim-0.4.0a2/curvesim/pool_data/metadata/base.py
+-rw-r--r--   0 suh        (501) staff       (20)     2007 2023-05-17 21:31:12.000000 curvesim-0.4.0a2/curvesim/pool_data/metadata/cryptoswap.py
+-rw-r--r--   0 suh        (501) staff       (20)     2515 2023-05-17 21:31:12.000000 curvesim-0.4.0a2/curvesim/pool_data/metadata/stableswap.py
+-rw-r--r--   0 suh        (501) staff       (20)     1287 2023-05-19 21:10:12.000000 curvesim-0.4.0a2/curvesim/pool_data/queries.py
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.972477 curvesim-0.4.0a2/curvesim/price_data/
+-rw-r--r--   0 suh        (501) staff       (20)     1382 2023-05-19 14:49:10.000000 curvesim-0.4.0a2/curvesim/price_data/__init__.py
+-rw-r--r--   0 suh        (501) staff       (20)     1586 2023-04-27 21:23:34.000000 curvesim-0.4.0a2/curvesim/price_data/sources.py
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.974202 curvesim-0.4.0a2/curvesim/sim/
+-rw-r--r--   0 suh        (501) staff       (20)     6025 2023-05-19 21:10:12.000000 curvesim-0.4.0a2/curvesim/sim/__init__.py
+-rw-r--r--   0 suh        (501) staff       (20)     3676 2023-05-19 14:49:10.000000 curvesim-0.4.0a2/curvesim/utils.py
+-rw-r--r--   0 suh        (501) staff       (20)      361 2023-05-19 22:23:56.000000 curvesim-0.4.0a2/curvesim/version.py
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.810710 curvesim-0.4.0a2/curvesim.egg-info/
+-rw-r--r--   0 suh        (501) staff       (20)     9758 2023-05-19 22:24:41.000000 curvesim-0.4.0a2/curvesim.egg-info/PKG-INFO
+-rw-r--r--   0 suh        (501) staff       (20)     3029 2023-05-19 22:24:41.000000 curvesim-0.4.0a2/curvesim.egg-info/SOURCES.txt
+-rw-r--r--   0 suh        (501) staff       (20)        1 2023-05-19 22:24:41.000000 curvesim-0.4.0a2/curvesim.egg-info/dependency_links.txt
+-rw-r--r--   0 suh        (501) staff       (20)      155 2023-05-19 22:24:41.000000 curvesim-0.4.0a2/curvesim.egg-info/requires.txt
+-rw-r--r--   0 suh        (501) staff       (20)       14 2023-05-19 22:24:41.000000 curvesim-0.4.0a2/curvesim.egg-info/top_level.txt
+-rw-r--r--   0 suh        (501) staff       (20)      170 2022-11-08 18:43:56.000000 curvesim-0.4.0a2/pyproject.toml
+-rw-r--r--   0 suh        (501) staff       (20)     1960 2023-05-19 22:24:41.996864 curvesim-0.4.0a2/setup.cfg
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.786510 curvesim-0.4.0a2/test/
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.976685 curvesim-0.4.0a2/test/fixtures/
+-rw-r--r--   0 suh        (501) staff       (20)        0 2022-10-14 18:34:20.000000 curvesim-0.4.0a2/test/fixtures/__init__.py
+-rw-r--r--   0 suh        (501) staff       (20)     5506 2023-02-13 20:22:55.000000 curvesim-0.4.0a2/test/fixtures/pool.py
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.978964 curvesim-0.4.0a2/test/integration/
+-rw-r--r--   0 suh        (501) staff       (20)        0 2023-04-27 21:23:34.000000 curvesim-0.4.0a2/test/integration/__init__.py
+-rw-r--r--   0 suh        (501) staff       (20)     1581 2023-05-17 21:31:12.000000 curvesim-0.4.0a2/test/integration/test_subgraph.py
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.981117 curvesim-0.4.0a2/test/scripts/
+-rw-r--r--   0 suh        (501) staff       (20)        0 2023-01-20 15:19:11.000000 curvesim-0.4.0a2/test/scripts/__init__.py
+-rw-r--r--   0 suh        (501) staff       (20)     4078 2023-05-17 22:06:08.000000 curvesim-0.4.0a2/test/scripts/make_test_data.py
+drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.993640 curvesim-0.4.0a2/test/unit/
+-rw-r--r--   0 suh        (501) staff       (20)        0 2022-10-14 18:34:20.000000 curvesim-0.4.0a2/test/unit/__init__.py
+-rw-r--r--   0 suh        (501) staff       (20)    22383 2023-05-17 21:31:12.000000 curvesim-0.4.0a2/test/unit/test_cryptopool.py
+-rw-r--r--   0 suh        (501) staff       (20)    13246 2023-02-13 20:22:55.000000 curvesim-0.4.0a2/test/unit/test_metapool.py
+-rw-r--r--   0 suh        (501) staff       (20)     8717 2023-03-02 16:07:35.000000 curvesim-0.4.0a2/test/unit/test_pool.py
+-rw-r--r--   0 suh        (501) staff       (20)    11214 2023-05-17 21:31:12.000000 curvesim-0.4.0a2/test/unit/test_pool_metadata.py
+-rw-r--r--   0 suh        (501) staff       (20)     4168 2023-05-17 18:59:58.000000 curvesim-0.4.0a2/test/unit/test_sim_stableswap.py
+-rw-r--r--   0 suh        (501) staff       (20)     3531 2023-01-20 15:19:11.000000 curvesim-0.4.0a2/test/unit/test_snapshot.py
```

### Comparing `curvesim-0.4.0a1/LICENSE.md` & `curvesim-0.4.0a2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/PKG-INFO` & `curvesim-0.4.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curvesim
-Version: 0.4.0a1
+Version: 0.4.0a2
 Summary: Simulate Curve pools
 Home-page: https://github.com/curveresearch/curvesim
 Author: Curve Research
 Author-email: help@curveresearch.org
 License: MIT
 Project-URL: Documentation, https://curvesim.readthedocs.io
 Project-URL: Source, https://github.com/curveresearch/curvesim
```

### Comparing `curvesim-0.4.0a1/README.md` & `curvesim-0.4.0a2/README.md`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/curvesim/_bonding_curve/__init__.py` & `curvesim-0.4.0a2/curvesim/_bonding_curve/__init__.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/curvesim/_order_book/__init__.py` & `curvesim-0.4.0a2/curvesim/_order_book/__init__.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/curvesim/exceptions/__init__.py` & `curvesim-0.4.0a2/curvesim/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/curvesim/iterators/param_samplers/grid.py` & `curvesim-0.4.0a2/curvesim/iterators/param_samplers/grid.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/curvesim/iterators/price_samplers/price_volume.py` & `curvesim-0.4.0a2/curvesim/iterators/price_samplers/price_volume.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/curvesim/logging.py` & `curvesim-0.4.0a2/curvesim/logging.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/curvesim/metrics/__init__.py` & `curvesim-0.4.0a2/curvesim/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/curvesim/metrics/base.py` & `curvesim-0.4.0a2/curvesim/metrics/base.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/curvesim/metrics/metrics.py` & `curvesim-0.4.0a2/curvesim/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/curvesim/metrics/results/make_results.py` & `curvesim-0.4.0a2/curvesim/metrics/results/make_results.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/curvesim/metrics/results/sim_results.py` & `curvesim-0.4.0a2/curvesim/metrics/results/sim_results.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/curvesim/metrics/state_log/log.py` & `curvesim-0.4.0a2/curvesim/metrics/state_log/log.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/curvesim/metrics/state_log/pool_parameters.py` & `curvesim-0.4.0a2/curvesim/metrics/state_log/pool_parameters.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/curvesim/metrics/state_log/pool_state.py` & `curvesim-0.4.0a2/curvesim/metrics/state_log/pool_state.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/curvesim/network/coingecko.py` & `curvesim-0.4.0a2/curvesim/network/coingecko.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/curvesim/network/http.py` & `curvesim-0.4.0a2/curvesim/network/http.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/curvesim/network/llamaAPI.py` & `curvesim-0.4.0a2/curvesim/network/llamaAPI.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/curvesim/network/nomics.py` & `curvesim-0.4.0a2/curvesim/network/nomics.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/curvesim/network/subgraph.py` & `curvesim-0.4.0a2/curvesim/network/subgraph.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/curvesim/network/utils.py` & `curvesim-0.4.0a2/curvesim/network/utils.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/curvesim/network/web3.py` & `curvesim-0.4.0a2/curvesim/network/web3.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/curvesim/overrides/__init__.py` & `curvesim-0.4.0a2/curvesim/overrides/__init__.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/curvesim/pipelines/arbitrage.py` & `curvesim-0.4.0a2/curvesim/pipelines/arbitrage.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/curvesim/pipelines/templates.py` & `curvesim-0.4.0a2/curvesim/pipelines/templates.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/curvesim/pipelines/utils.py` & `curvesim-0.4.0a2/curvesim/pipelines/utils.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/curvesim/plot/altair/chart_properties.py` & `curvesim-0.4.0a2/curvesim/plot/altair/chart_properties.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/curvesim/plot/altair/make_chart.py` & `curvesim-0.4.0a2/curvesim/plot/altair/make_chart.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/curvesim/plot/altair/selectors.py` & `curvesim-0.4.0a2/curvesim/plot/altair/selectors.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/curvesim/plot/altair/styles.py` & `curvesim-0.4.0a2/curvesim/plot/altair/styles.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/curvesim/plot/result_plotter.py` & `curvesim-0.4.0a2/curvesim/plot/result_plotter.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/curvesim/pool/__init__.py` & `curvesim-0.4.0a2/curvesim/pool/__init__.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/curvesim/pool/base.py` & `curvesim-0.4.0a2/curvesim/pool/base.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/curvesim/pool/cryptoswap/pool.py` & `curvesim-0.4.0a2/curvesim/pool/cryptoswap/pool.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/curvesim/pool/sim_interface/metapool.py` & `curvesim-0.4.0a2/curvesim/pool/sim_interface/metapool.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/curvesim/pool/sim_interface/pool.py` & `curvesim-0.4.0a2/curvesim/pool/sim_interface/pool.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/curvesim/pool/sim_interface/raipool.py` & `curvesim-0.4.0a2/curvesim/pool/sim_interface/raipool.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/curvesim/pool/sim_interface/simpool.py` & `curvesim-0.4.0a2/curvesim/pool/sim_interface/simpool.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/curvesim/pool/snapshot.py` & `curvesim-0.4.0a2/curvesim/pool/snapshot.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/curvesim/pool/stableswap/metapool.py` & `curvesim-0.4.0a2/curvesim/pool/stableswap/metapool.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/curvesim/pool/stableswap/pool.py` & `curvesim-0.4.0a2/curvesim/pool/stableswap/pool.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/curvesim/pool/stableswap/raipool.py` & `curvesim-0.4.0a2/curvesim/pool/stableswap/raipool.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/curvesim/pool_data/__init__.py` & `curvesim-0.4.0a2/curvesim/pool_data/__init__.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/curvesim/pool_data/cache.py` & `curvesim-0.4.0a2/curvesim/pool_data/cache.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/curvesim/pool_data/metadata/__init__.py` & `curvesim-0.4.0a2/curvesim/pool_data/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/curvesim/pool_data/metadata/base.py` & `curvesim-0.4.0a2/curvesim/pool_data/metadata/base.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/curvesim/pool_data/metadata/cryptoswap.py` & `curvesim-0.4.0a2/curvesim/pool_data/metadata/cryptoswap.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/curvesim/pool_data/metadata/stableswap.py` & `curvesim-0.4.0a2/curvesim/pool_data/metadata/stableswap.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/curvesim/pool_data/queries.py` & `curvesim-0.4.0a2/curvesim/pool_data/queries.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/curvesim/price_data/__init__.py` & `curvesim-0.4.0a2/curvesim/price_data/__init__.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/curvesim/price_data/sources.py` & `curvesim-0.4.0a2/curvesim/price_data/sources.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/curvesim/sim/__init__.py` & `curvesim-0.4.0a2/curvesim/sim/__init__.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/curvesim/utils.py` & `curvesim-0.4.0a2/curvesim/utils.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/curvesim.egg-info/PKG-INFO` & `curvesim-0.4.0a2/curvesim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curvesim
-Version: 0.4.0a1
+Version: 0.4.0a2
 Summary: Simulate Curve pools
 Home-page: https://github.com/curveresearch/curvesim
 Author: Curve Research
 Author-email: help@curveresearch.org
 License: MIT
 Project-URL: Documentation, https://curvesim.readthedocs.io
 Project-URL: Source, https://github.com/curveresearch/curvesim
```

### Comparing `curvesim-0.4.0a1/curvesim.egg-info/SOURCES.txt` & `curvesim-0.4.0a2/curvesim.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,20 @@
 curvesim/plot/__init__.py
 curvesim/plot/result_plotter.py
 curvesim/plot/altair/__init__.py
 curvesim/plot/altair/chart_properties.py
 curvesim/plot/altair/make_chart.py
 curvesim/plot/altair/selectors.py
 curvesim/plot/altair/styles.py
+curvesim/plot/altair/results/__init__.py
+curvesim/plot/altair/results/make_page.py
+curvesim/plot/altair/results/preprocessing.py
+curvesim/plot/altair/results/result_plotter.py
+curvesim/plot/altair/results/result_selectors.py
+curvesim/plot/altair/results/tooltip.py
 curvesim/pool/__init__.py
 curvesim/pool/base.py
 curvesim/pool/snapshot.py
 curvesim/pool/cryptoswap/__init__.py
 curvesim/pool/cryptoswap/pool.py
 curvesim/pool/sim_interface/__init__.py
 curvesim/pool/sim_interface/metapool.py
```

### Comparing `curvesim-0.4.0a1/setup.cfg` & `curvesim-0.4.0a2/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.4.0.a1
+current_version = 0.4.0.a2
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\.(?P<release>.*)(?P<build>\d+))?
 serialize = 
 	{major}.{minor}.{patch}.{release}{build}
 	{major}.{minor}.{patch}
 commit = True
 tag = True
```

### Comparing `curvesim-0.4.0a1/test/fixtures/pool.py` & `curvesim-0.4.0a2/test/fixtures/pool.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/test/integration/test_subgraph.py` & `curvesim-0.4.0a2/test/integration/test_subgraph.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/test/scripts/make_test_data.py` & `curvesim-0.4.0a2/test/scripts/make_test_data.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/test/unit/test_cryptopool.py` & `curvesim-0.4.0a2/test/unit/test_cryptopool.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/test/unit/test_metapool.py` & `curvesim-0.4.0a2/test/unit/test_metapool.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/test/unit/test_pool.py` & `curvesim-0.4.0a2/test/unit/test_pool.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/test/unit/test_pool_metadata.py` & `curvesim-0.4.0a2/test/unit/test_pool_metadata.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/test/unit/test_sim_stableswap.py` & `curvesim-0.4.0a2/test/unit/test_sim_stableswap.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a1/test/unit/test_snapshot.py` & `curvesim-0.4.0a2/test/unit/test_snapshot.py`

 * *Files identical despite different names*

