# Comparing `tmp/probability-0.0.8.tar.gz` & `tmp/probability-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/probability-0.0.8.tar", last modified: Sat Feb  8 19:58:08 2020, max compression
+gzip compressed data, was "dist/probability-0.0.9.tar", last modified: Mon May 18 19:09:26 2020, max compression
```

## Comparing `probability-0.0.8.tar` & `probability-0.0.9.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 vahndi.minah (1618459704) 1841347858        0 2020-02-08 19:58:08.000000 probability-0.0.8/
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858      450 2020-02-08 19:58:08.000000 probability-0.0.8/PKG-INFO
-drwxr-xr-x   0 vahndi.minah (1618459704) 1841347858        0 2020-02-08 19:58:06.000000 probability-0.0.8/probability/
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858        0 2020-01-01 17:32:02.000000 probability-0.0.8/probability/__init__.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858     1293 2019-12-28 20:57:50.000000 probability-0.0.8/probability/plots.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858      824 2020-01-17 19:12:37.000000 probability-0.0.8/probability/utils.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858      664 2020-01-08 03:14:33.000000 probability-0.0.8/probability/custom_types.py
-drwxr-xr-x   0 vahndi.minah (1618459704) 1841347858        0 2020-02-08 19:58:07.000000 probability-0.0.8/probability/distributions/
-drwxr-xr-x   0 vahndi.minah (1618459704) 1841347858        0 2020-02-08 19:58:08.000000 probability-0.0.8/probability/distributions/multivariate/
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858      912 2020-01-10 19:59:41.000000 probability-0.0.8/probability/distributions/multivariate/dirichlet.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858     2002 2020-01-11 18:20:52.000000 probability-0.0.8/probability/distributions/multivariate/mv_normal.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858      216 2020-01-10 13:12:28.000000 probability-0.0.8/probability/distributions/multivariate/__init__.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858     1335 2020-01-11 18:54:36.000000 probability-0.0.8/probability/distributions/multivariate/multinomial.py
-drwxr-xr-x   0 vahndi.minah (1618459704) 1841347858        0 2020-02-08 19:58:08.000000 probability-0.0.8/probability/distributions/mixins/
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858        0 2020-01-02 22:21:33.000000 probability-0.0.8/probability/distributions/mixins/likelihood_mixin.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858     1389 2020-01-16 16:39:23.000000 probability-0.0.8/probability/distributions/mixins/rv_continuous_1d_mixin.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858        0 2019-12-18 21:38:55.000000 probability-0.0.8/probability/distributions/mixins/__init__.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858      640 2020-01-16 20:04:50.000000 probability-0.0.8/probability/distributions/mixins/plottable_mixin.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858      954 2020-01-03 15:24:47.000000 probability-0.0.8/probability/distributions/mixins/prior_mixin.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858        0 2020-01-02 22:21:44.000000 probability-0.0.8/probability/distributions/mixins/posterior_mixin.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858     1304 2020-01-16 16:49:27.000000 probability-0.0.8/probability/distributions/mixins/rv_discrete_1d_mixin.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858    12035 2020-01-10 13:09:09.000000 probability-0.0.8/probability/distributions/mixins/rv_mixins.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858      974 2020-01-16 00:34:42.000000 probability-0.0.8/probability/distributions/mixins/conjugate_mixin.py
-drwxr-xr-x   0 vahndi.minah (1618459704) 1841347858        0 2020-02-08 19:58:07.000000 probability-0.0.8/probability/distributions/discrete/
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858      717 2020-01-08 02:22:11.000000 probability-0.0.8/probability/distributions/discrete/poisson.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858      128 2020-01-10 13:10:52.000000 probability-0.0.8/probability/distributions/discrete/__init__.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858     1110 2020-01-17 16:12:47.000000 probability-0.0.8/probability/distributions/discrete/negative_binomial.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858      894 2020-01-07 20:45:25.000000 probability-0.0.8/probability/distributions/discrete/binomial.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858      203 2020-01-20 16:57:15.000000 probability-0.0.8/probability/distributions/__init__.py
-drwxr-xr-x   0 vahndi.minah (1618459704) 1841347858        0 2020-02-08 19:58:08.000000 probability-0.0.8/probability/distributions/special/
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858      690 2019-12-19 14:35:25.000000 probability-0.0.8/probability/distributions/special/_no_numba.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858      266 2020-01-04 18:00:52.000000 probability-0.0.8/probability/distributions/special/__init__.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858      732 2019-12-19 14:35:25.000000 probability-0.0.8/probability/distributions/special/_with_numba.py
-drwxr-xr-x   0 vahndi.minah (1618459704) 1841347858        0 2020-02-08 19:58:08.000000 probability-0.0.8/probability/distributions/functions/
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858      423 2020-02-03 20:48:26.000000 probability-0.0.8/probability/distributions/functions/function_of_two.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858     2324 2020-01-16 17:48:40.000000 probability-0.0.8/probability/distributions/functions/discrete_function_1d.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858        0 2019-12-31 22:28:34.000000 probability-0.0.8/probability/distributions/functions/__init__.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858     1928 2020-01-16 17:41:12.000000 probability-0.0.8/probability/distributions/functions/continuous_function_1d.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858     2593 2020-01-11 18:20:52.000000 probability-0.0.8/probability/distributions/functions/discrete_function_nd.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858     4559 2020-01-11 18:20:52.000000 probability-0.0.8/probability/distributions/functions/continuous_function_nd.py
-drwxr-xr-x   0 vahndi.minah (1618459704) 1841347858        0 2020-02-08 19:58:07.000000 probability-0.0.8/probability/distributions/conjugate/
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858     3530 2020-02-03 20:48:26.000000 probability-0.0.8/probability/distributions/conjugate/gamma_exponential.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858     3380 2020-01-20 22:43:45.000000 probability-0.0.8/probability/distributions/conjugate/beta_binomial.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858      386 2020-01-20 16:56:12.000000 probability-0.0.8/probability/distributions/conjugate/__init__.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858      798 2020-02-06 13:23:22.000000 probability-0.0.8/probability/distributions/conjugate/beta_geometric.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858     2591 2020-01-20 17:07:10.000000 probability-0.0.8/probability/distributions/conjugate/inv_gamma_normal.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858     4281 2020-01-20 22:44:05.000000 probability-0.0.8/probability/distributions/conjugate/normal_normal.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858      493 2020-02-06 13:24:40.000000 probability-0.0.8/probability/distributions/conjugate/dirichlet_multinomial.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858     2626 2020-01-20 22:43:45.000000 probability-0.0.8/probability/distributions/conjugate/gamma_normal.py
-drwxr-xr-x   0 vahndi.minah (1618459704) 1841347858        0 2020-02-08 19:58:07.000000 probability-0.0.8/probability/distributions/continuous/
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858      918 2020-01-08 02:20:49.000000 probability-0.0.8/probability/distributions/continuous/laplace.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858      842 2020-01-16 01:39:24.000000 probability-0.0.8/probability/distributions/continuous/lomax.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858     2133 2020-01-17 19:13:28.000000 probability-0.0.8/probability/distributions/continuous/normal.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858      997 2020-01-07 02:25:54.000000 probability-0.0.8/probability/distributions/continuous/beta.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858      520 2020-01-20 16:56:12.000000 probability-0.0.8/probability/distributions/continuous/__init__.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858      725 2020-01-16 01:39:24.000000 probability-0.0.8/probability/distributions/continuous/exponential.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858     1016 2020-01-16 16:33:40.000000 probability-0.0.8/probability/distributions/continuous/inv_gamma.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858     2147 2020-01-15 22:07:43.000000 probability-0.0.8/probability/distributions/continuous/gamma.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858     2193 2020-01-16 17:18:56.000000 probability-0.0.8/probability/distributions/continuous/students_t.py
-drwxr-xr-x   0 vahndi.minah (1618459704) 1841347858        0 2020-02-08 19:58:08.000000 probability-0.0.8/probability/pandas/
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858     8724 2020-02-08 19:50:26.000000 probability-0.0.8/probability/pandas/prob_utils.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858       74 2020-01-27 22:54:09.000000 probability-0.0.8/probability/pandas/__init__.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858     2971 2020-02-06 03:02:20.000000 probability-0.0.8/probability/pandas/variable_filter.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858     3883 2020-02-06 02:19:18.000000 probability-0.0.8/probability/pandas/conditional_table.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858     9859 2020-02-08 19:51:29.000000 probability-0.0.8/probability/pandas/discrete_distribution.py
-drwxr-xr-x   0 vahndi.minah (1618459704) 1841347858        0 2020-02-08 19:58:08.000000 probability-0.0.8/tests/
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858      223 2020-02-05 01:48:03.000000 probability-0.0.8/tests/paths.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858        0 2020-01-22 16:41:03.000000 probability-0.0.8/tests/__init__.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858     1450 2020-01-27 21:27:14.000000 probability-0.0.8/tests/shared.py
-drwxr-xr-x   0 vahndi.minah (1618459704) 1841347858        0 2020-02-08 19:58:08.000000 probability-0.0.8/tests/test_pandas/
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858     3372 2020-02-08 19:53:01.000000 probability-0.0.8/tests/test_pandas/test_discrete_distribution.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858      893 2020-02-05 16:26:31.000000 probability-0.0.8/tests/test_pandas/test_conditional_table.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858        0 2020-02-04 01:34:45.000000 probability-0.0.8/tests/test_pandas/__init__.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858     1997 2020-02-06 02:30:36.000000 probability-0.0.8/tests/test_pandas/test_examples.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858     5608 2020-02-05 16:58:32.000000 probability-0.0.8/tests/test_pandas/test_prob_utils.py
-drwxr-xr-x   0 vahndi.minah (1618459704) 1841347858        0 2020-02-08 19:58:06.000000 probability-0.0.8/probability.egg-info/
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858      450 2020-02-08 19:58:01.000000 probability-0.0.8/probability.egg-info/PKG-INFO
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858     4257 2020-02-08 19:58:02.000000 probability-0.0.8/probability.egg-info/SOURCES.txt
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858       30 2020-02-08 19:58:01.000000 probability-0.0.8/probability.egg-info/requires.txt
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858       27 2020-02-08 19:58:02.000000 probability-0.0.8/probability.egg-info/top_level.txt
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858        1 2020-02-08 19:58:01.000000 probability-0.0.8/probability.egg-info/dependency_links.txt
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858      610 2020-02-08 19:56:50.000000 probability-0.0.8/setup.py
-drwxr-xr-x   0 vahndi.minah (1618459704) 1841347858        0 2020-02-08 19:58:05.000000 probability-0.0.8/examples/
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858        0 2019-12-28 20:55:00.000000 probability-0.0.8/examples/__init__.py
-drwxr-xr-x   0 vahndi.minah (1618459704) 1841347858        0 2020-02-08 19:58:05.000000 probability-0.0.8/examples/distributions/
-drwxr-xr-x   0 vahndi.minah (1618459704) 1841347858        0 2020-02-08 19:58:06.000000 probability-0.0.8/examples/distributions/multivariate/
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858      214 2020-01-10 20:24:50.000000 probability-0.0.8/examples/distributions/multivariate/dirichlet.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858      377 2020-01-10 19:31:04.000000 probability-0.0.8/examples/distributions/multivariate/mv_normal.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858        0 2020-01-08 03:03:39.000000 probability-0.0.8/examples/distributions/multivariate/__init__.py
-drwxr-xr-x   0 vahndi.minah (1618459704) 1841347858        0 2020-02-08 19:58:06.000000 probability-0.0.8/examples/distributions/discrete/
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858     1893 2020-01-11 19:07:25.000000 probability-0.0.8/examples/distributions/discrete/poisson.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858        0 2020-01-05 22:13:45.000000 probability-0.0.8/examples/distributions/discrete/__init__.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858      545 2020-01-11 18:56:07.000000 probability-0.0.8/examples/distributions/discrete/multinomial.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858      784 2020-01-16 20:06:37.000000 probability-0.0.8/examples/distributions/discrete/negative_binomial.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858     2160 2020-01-11 19:07:25.000000 probability-0.0.8/examples/distributions/discrete/binomial.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858        0 2020-01-05 22:12:59.000000 probability-0.0.8/examples/distributions/__init__.py
-drwxr-xr-x   0 vahndi.minah (1618459704) 1841347858        0 2020-02-08 19:58:06.000000 probability-0.0.8/examples/distributions/conjugate/
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858      647 2020-01-16 00:44:02.000000 probability-0.0.8/examples/distributions/conjugate/gamma_exponential.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858     2162 2020-01-11 18:20:52.000000 probability-0.0.8/examples/distributions/conjugate/beta_binomial.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858        0 2020-01-05 22:14:19.000000 probability-0.0.8/examples/distributions/conjugate/__init__.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858      955 2020-01-16 18:00:37.000000 probability-0.0.8/examples/distributions/conjugate/inv_gamma_normal.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858     1120 2020-01-17 20:14:23.000000 probability-0.0.8/examples/distributions/conjugate/normal_normal.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858      945 2020-01-17 20:30:38.000000 probability-0.0.8/examples/distributions/conjugate/gamma_normal.py
-drwxr-xr-x   0 vahndi.minah (1618459704) 1841347858        0 2020-02-08 19:58:06.000000 probability-0.0.8/examples/distributions/continuous/
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858     1135 2020-01-15 15:58:02.000000 probability-0.0.8/examples/distributions/continuous/laplace.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858     1100 2020-01-15 15:58:03.000000 probability-0.0.8/examples/distributions/continuous/lomax.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858     1214 2020-01-16 17:19:09.000000 probability-0.0.8/examples/distributions/continuous/comparisons.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858     1212 2020-01-15 15:58:02.000000 probability-0.0.8/examples/distributions/continuous/normal.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858     1408 2020-01-15 15:56:08.000000 probability-0.0.8/examples/distributions/continuous/beta.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858        0 2020-01-05 22:13:09.000000 probability-0.0.8/examples/distributions/continuous/__init__.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858     1078 2020-01-15 15:58:02.000000 probability-0.0.8/examples/distributions/continuous/exponential.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858      974 2020-01-16 01:37:07.000000 probability-0.0.8/examples/distributions/continuous/inv_gamma.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858     1799 2020-01-15 15:58:03.000000 probability-0.0.8/examples/distributions/continuous/gamma.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858     2587 2020-01-16 17:18:35.000000 probability-0.0.8/examples/distributions/continuous/students_t.py
-drwxr-xr-x   0 vahndi.minah (1618459704) 1841347858        0 2020-02-08 19:58:06.000000 probability-0.0.8/examples/pandas/
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858        0 2020-01-22 20:27:43.000000 probability-0.0.8/examples/pandas/__init__.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858     2343 2020-02-06 02:30:36.000000 probability-0.0.8/examples/pandas/discrete_distribution.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858       29 2020-01-11 18:42:31.000000 probability-0.0.8/examples/colors.py
--rw-r--r--   0 vahndi.minah (1618459704) 1841347858       79 2020-02-08 19:58:08.000000 probability-0.0.8/setup.cfg
+drwxr-xr-x   0 vahndi.minah (1618459704) 1841347858        0 2020-05-18 19:09:26.000000 probability-0.0.9/
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858      450 2020-05-18 19:09:26.000000 probability-0.0.9/PKG-INFO
+drwxr-xr-x   0 vahndi.minah (1618459704) 1841347858        0 2020-05-18 19:09:26.000000 probability-0.0.9/examples/
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858        0 2019-12-28 20:55:00.000000 probability-0.0.9/examples/__init__.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858       29 2020-01-11 18:42:31.000000 probability-0.0.9/examples/colors.py
+drwxr-xr-x   0 vahndi.minah (1618459704) 1841347858        0 2020-05-18 19:09:26.000000 probability-0.0.9/examples/discrete/
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858        0 2020-01-22 20:27:43.000000 probability-0.0.9/examples/discrete/__init__.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858     2345 2020-02-17 15:26:57.000000 probability-0.0.9/examples/discrete/discrete_distribution.py
+drwxr-xr-x   0 vahndi.minah (1618459704) 1841347858        0 2020-05-18 19:09:26.000000 probability-0.0.9/examples/distributions/
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858        0 2020-01-05 22:12:59.000000 probability-0.0.9/examples/distributions/__init__.py
+drwxr-xr-x   0 vahndi.minah (1618459704) 1841347858        0 2020-05-18 19:09:26.000000 probability-0.0.9/examples/distributions/conjugate/
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858        0 2020-01-05 22:14:19.000000 probability-0.0.9/examples/distributions/conjugate/__init__.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858     2162 2020-01-11 18:20:52.000000 probability-0.0.9/examples/distributions/conjugate/beta_binomial.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858      647 2020-01-16 00:44:02.000000 probability-0.0.9/examples/distributions/conjugate/gamma_exponential.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858      945 2020-01-17 20:30:38.000000 probability-0.0.9/examples/distributions/conjugate/gamma_normal.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858      955 2020-01-16 18:00:37.000000 probability-0.0.9/examples/distributions/conjugate/inv_gamma_normal.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858     1120 2020-01-17 20:14:23.000000 probability-0.0.9/examples/distributions/conjugate/normal_normal.py
+drwxr-xr-x   0 vahndi.minah (1618459704) 1841347858        0 2020-05-18 19:09:26.000000 probability-0.0.9/examples/distributions/continuous/
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858        0 2020-01-05 22:13:09.000000 probability-0.0.9/examples/distributions/continuous/__init__.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858     1408 2020-01-15 15:56:08.000000 probability-0.0.9/examples/distributions/continuous/beta.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858     1214 2020-01-16 17:19:09.000000 probability-0.0.9/examples/distributions/continuous/comparisons.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858     1078 2020-01-15 15:58:02.000000 probability-0.0.9/examples/distributions/continuous/exponential.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858     1799 2020-01-15 15:58:03.000000 probability-0.0.9/examples/distributions/continuous/gamma.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858      974 2020-01-16 01:37:07.000000 probability-0.0.9/examples/distributions/continuous/inv_gamma.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858     1135 2020-01-15 15:58:02.000000 probability-0.0.9/examples/distributions/continuous/laplace.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858     1100 2020-01-15 15:58:03.000000 probability-0.0.9/examples/distributions/continuous/lomax.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858     1212 2020-01-15 15:58:02.000000 probability-0.0.9/examples/distributions/continuous/normal.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858     2587 2020-01-16 17:18:35.000000 probability-0.0.9/examples/distributions/continuous/students_t.py
+drwxr-xr-x   0 vahndi.minah (1618459704) 1841347858        0 2020-05-18 19:09:26.000000 probability-0.0.9/examples/distributions/discrete/
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858        0 2020-01-05 22:13:45.000000 probability-0.0.9/examples/distributions/discrete/__init__.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858     2160 2020-01-11 19:07:25.000000 probability-0.0.9/examples/distributions/discrete/binomial.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858      545 2020-01-11 18:56:07.000000 probability-0.0.9/examples/distributions/discrete/multinomial.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858      784 2020-01-16 20:06:37.000000 probability-0.0.9/examples/distributions/discrete/negative_binomial.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858     1893 2020-01-11 19:07:25.000000 probability-0.0.9/examples/distributions/discrete/poisson.py
+drwxr-xr-x   0 vahndi.minah (1618459704) 1841347858        0 2020-05-18 19:09:26.000000 probability-0.0.9/examples/distributions/multivariate/
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858        0 2020-01-08 03:03:39.000000 probability-0.0.9/examples/distributions/multivariate/__init__.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858      214 2020-01-10 20:24:50.000000 probability-0.0.9/examples/distributions/multivariate/dirichlet.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858      377 2020-01-10 19:31:04.000000 probability-0.0.9/examples/distributions/multivariate/mv_normal.py
+drwxr-xr-x   0 vahndi.minah (1618459704) 1841347858        0 2020-05-18 19:09:26.000000 probability-0.0.9/probability/
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858        0 2020-01-01 17:32:02.000000 probability-0.0.9/probability/__init__.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858      664 2020-01-08 03:14:33.000000 probability-0.0.9/probability/custom_types.py
+drwxr-xr-x   0 vahndi.minah (1618459704) 1841347858        0 2020-05-18 19:09:26.000000 probability-0.0.9/probability/discrete/
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858      144 2020-02-17 15:26:57.000000 probability-0.0.9/probability/discrete/__init__.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858     5231 2020-02-17 19:48:21.000000 probability-0.0.9/probability/discrete/conditional_table.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858    12319 2020-02-18 00:14:12.000000 probability-0.0.9/probability/discrete/discrete_distribution.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858     9854 2020-02-17 19:47:55.000000 probability-0.0.9/probability/discrete/prob_utils.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858     2973 2020-02-17 15:26:57.000000 probability-0.0.9/probability/discrete/variable_filter.py
+drwxr-xr-x   0 vahndi.minah (1618459704) 1841347858        0 2020-05-18 19:09:26.000000 probability-0.0.9/probability/distributions/
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858      203 2020-01-20 16:57:15.000000 probability-0.0.9/probability/distributions/__init__.py
+drwxr-xr-x   0 vahndi.minah (1618459704) 1841347858        0 2020-05-18 19:09:26.000000 probability-0.0.9/probability/distributions/conjugate/
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858      386 2020-01-20 16:56:12.000000 probability-0.0.9/probability/distributions/conjugate/__init__.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858     3380 2020-01-20 22:43:45.000000 probability-0.0.9/probability/distributions/conjugate/beta_binomial.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858      798 2020-02-06 13:23:22.000000 probability-0.0.9/probability/distributions/conjugate/beta_geometric.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858      493 2020-02-06 13:24:40.000000 probability-0.0.9/probability/distributions/conjugate/dirichlet_multinomial.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858     3530 2020-02-03 20:48:26.000000 probability-0.0.9/probability/distributions/conjugate/gamma_exponential.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858     2626 2020-01-20 22:43:45.000000 probability-0.0.9/probability/distributions/conjugate/gamma_normal.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858     2591 2020-01-20 17:07:10.000000 probability-0.0.9/probability/distributions/conjugate/inv_gamma_normal.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858     4281 2020-01-20 22:44:05.000000 probability-0.0.9/probability/distributions/conjugate/normal_normal.py
+drwxr-xr-x   0 vahndi.minah (1618459704) 1841347858        0 2020-05-18 19:09:26.000000 probability-0.0.9/probability/distributions/continuous/
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858      520 2020-01-20 16:56:12.000000 probability-0.0.9/probability/distributions/continuous/__init__.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858      997 2020-01-07 02:25:54.000000 probability-0.0.9/probability/distributions/continuous/beta.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858      725 2020-01-16 01:39:24.000000 probability-0.0.9/probability/distributions/continuous/exponential.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858     2147 2020-01-15 22:07:43.000000 probability-0.0.9/probability/distributions/continuous/gamma.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858     1016 2020-01-16 16:33:40.000000 probability-0.0.9/probability/distributions/continuous/inv_gamma.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858      918 2020-01-08 02:20:49.000000 probability-0.0.9/probability/distributions/continuous/laplace.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858      842 2020-01-16 01:39:24.000000 probability-0.0.9/probability/distributions/continuous/lomax.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858     2133 2020-01-17 19:13:28.000000 probability-0.0.9/probability/distributions/continuous/normal.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858     2193 2020-01-16 17:18:56.000000 probability-0.0.9/probability/distributions/continuous/students_t.py
+drwxr-xr-x   0 vahndi.minah (1618459704) 1841347858        0 2020-05-18 19:09:26.000000 probability-0.0.9/probability/distributions/discrete/
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858      128 2020-01-10 13:10:52.000000 probability-0.0.9/probability/distributions/discrete/__init__.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858      894 2020-01-07 20:45:25.000000 probability-0.0.9/probability/distributions/discrete/binomial.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858     1110 2020-01-17 16:12:47.000000 probability-0.0.9/probability/distributions/discrete/negative_binomial.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858      717 2020-01-08 02:22:11.000000 probability-0.0.9/probability/distributions/discrete/poisson.py
+drwxr-xr-x   0 vahndi.minah (1618459704) 1841347858        0 2020-05-18 19:09:26.000000 probability-0.0.9/probability/distributions/functions/
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858        0 2019-12-31 22:28:34.000000 probability-0.0.9/probability/distributions/functions/__init__.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858     2000 2020-05-18 19:05:46.000000 probability-0.0.9/probability/distributions/functions/continuous_function_1d.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858     4559 2020-01-11 18:20:52.000000 probability-0.0.9/probability/distributions/functions/continuous_function_nd.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858     2318 2020-05-18 19:07:31.000000 probability-0.0.9/probability/distributions/functions/discrete_function_1d.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858     2593 2020-01-11 18:20:52.000000 probability-0.0.9/probability/distributions/functions/discrete_function_nd.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858      423 2020-02-03 20:48:26.000000 probability-0.0.9/probability/distributions/functions/function_of_two.py
+drwxr-xr-x   0 vahndi.minah (1618459704) 1841347858        0 2020-05-18 19:09:26.000000 probability-0.0.9/probability/distributions/mixins/
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858        0 2019-12-18 21:38:55.000000 probability-0.0.9/probability/distributions/mixins/__init__.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858      974 2020-01-16 00:34:42.000000 probability-0.0.9/probability/distributions/mixins/conjugate_mixin.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858        0 2020-01-02 22:21:33.000000 probability-0.0.9/probability/distributions/mixins/likelihood_mixin.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858      640 2020-01-16 20:04:50.000000 probability-0.0.9/probability/distributions/mixins/plottable_mixin.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858        0 2020-01-02 22:21:44.000000 probability-0.0.9/probability/distributions/mixins/posterior_mixin.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858      954 2020-01-03 15:24:47.000000 probability-0.0.9/probability/distributions/mixins/prior_mixin.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858     1389 2020-01-16 16:39:23.000000 probability-0.0.9/probability/distributions/mixins/rv_continuous_1d_mixin.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858     1304 2020-01-16 16:49:27.000000 probability-0.0.9/probability/distributions/mixins/rv_discrete_1d_mixin.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858    12035 2020-01-10 13:09:09.000000 probability-0.0.9/probability/distributions/mixins/rv_mixins.py
+drwxr-xr-x   0 vahndi.minah (1618459704) 1841347858        0 2020-05-18 19:09:26.000000 probability-0.0.9/probability/distributions/multivariate/
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858      216 2020-01-10 13:12:28.000000 probability-0.0.9/probability/distributions/multivariate/__init__.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858      912 2020-01-10 19:59:41.000000 probability-0.0.9/probability/distributions/multivariate/dirichlet.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858     1335 2020-01-11 18:54:36.000000 probability-0.0.9/probability/distributions/multivariate/multinomial.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858     2002 2020-01-11 18:20:52.000000 probability-0.0.9/probability/distributions/multivariate/mv_normal.py
+drwxr-xr-x   0 vahndi.minah (1618459704) 1841347858        0 2020-05-18 19:09:26.000000 probability-0.0.9/probability/distributions/special/
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858      266 2020-01-04 18:00:52.000000 probability-0.0.9/probability/distributions/special/__init__.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858      690 2019-12-19 14:35:25.000000 probability-0.0.9/probability/distributions/special/_no_numba.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858      732 2019-12-19 14:35:25.000000 probability-0.0.9/probability/distributions/special/_with_numba.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858     1293 2019-12-28 20:57:50.000000 probability-0.0.9/probability/plots.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858      824 2020-01-17 19:12:37.000000 probability-0.0.9/probability/utils.py
+drwxr-xr-x   0 vahndi.minah (1618459704) 1841347858        0 2020-05-18 19:09:26.000000 probability-0.0.9/probability.egg-info/
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858      450 2020-05-18 19:09:26.000000 probability-0.0.9/probability.egg-info/PKG-INFO
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858     4281 2020-05-18 19:09:26.000000 probability-0.0.9/probability.egg-info/SOURCES.txt
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858        1 2020-05-18 19:09:26.000000 probability-0.0.9/probability.egg-info/dependency_links.txt
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858       30 2020-05-18 19:09:26.000000 probability-0.0.9/probability.egg-info/requires.txt
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858       27 2020-05-18 19:09:26.000000 probability-0.0.9/probability.egg-info/top_level.txt
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858       79 2020-05-18 19:09:26.000000 probability-0.0.9/setup.cfg
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858      610 2020-05-18 19:08:57.000000 probability-0.0.9/setup.py
+drwxr-xr-x   0 vahndi.minah (1618459704) 1841347858        0 2020-05-18 19:09:26.000000 probability-0.0.9/tests/
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858        0 2020-01-22 16:41:03.000000 probability-0.0.9/tests/__init__.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858      223 2020-02-05 01:48:03.000000 probability-0.0.9/tests/paths.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858     1450 2020-01-27 21:27:14.000000 probability-0.0.9/tests/shared.py
+drwxr-xr-x   0 vahndi.minah (1618459704) 1841347858        0 2020-05-18 19:09:26.000000 probability-0.0.9/tests/test_discrete/
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858        0 2020-02-04 01:34:45.000000 probability-0.0.9/tests/test_discrete/__init__.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858      895 2020-02-17 15:26:57.000000 probability-0.0.9/tests/test_discrete/test_conditional_table.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858     5210 2020-02-18 00:26:39.000000 probability-0.0.9/tests/test_discrete/test_discrete_distribution.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858     1999 2020-02-17 15:26:57.000000 probability-0.0.9/tests/test_discrete/test_examples.py
+-rw-r--r--   0 vahndi.minah (1618459704) 1841347858     6257 2020-02-17 15:26:57.000000 probability-0.0.9/tests/test_discrete/test_prob_utils.py
```

### Comparing `probability-0.0.8/probability/plots.py` & `probability-0.0.9/probability/plots.py`

 * *Files identical despite different names*

### Comparing `probability-0.0.8/probability/utils.py` & `probability-0.0.9/probability/utils.py`

 * *Files identical despite different names*

### Comparing `probability-0.0.8/probability/custom_types.py` & `probability-0.0.9/probability/custom_types.py`

 * *Files identical despite different names*

### Comparing `probability-0.0.8/probability/distributions/multivariate/dirichlet.py` & `probability-0.0.9/probability/distributions/multivariate/dirichlet.py`

 * *Files identical despite different names*

### Comparing `probability-0.0.8/probability/distributions/multivariate/mv_normal.py` & `probability-0.0.9/probability/distributions/multivariate/mv_normal.py`

 * *Files identical despite different names*

### Comparing `probability-0.0.8/probability/distributions/multivariate/multinomial.py` & `probability-0.0.9/probability/distributions/multivariate/multinomial.py`

 * *Files identical despite different names*

### Comparing `probability-0.0.8/probability/distributions/mixins/rv_continuous_1d_mixin.py` & `probability-0.0.9/probability/distributions/mixins/rv_continuous_1d_mixin.py`

 * *Files identical despite different names*

### Comparing `probability-0.0.8/probability/distributions/mixins/plottable_mixin.py` & `probability-0.0.9/probability/distributions/mixins/plottable_mixin.py`

 * *Files identical despite different names*

### Comparing `probability-0.0.8/probability/distributions/mixins/prior_mixin.py` & `probability-0.0.9/probability/distributions/mixins/prior_mixin.py`

 * *Files identical despite different names*

### Comparing `probability-0.0.8/probability/distributions/mixins/rv_discrete_1d_mixin.py` & `probability-0.0.9/probability/distributions/mixins/rv_discrete_1d_mixin.py`

 * *Files identical despite different names*

### Comparing `probability-0.0.8/probability/distributions/mixins/rv_mixins.py` & `probability-0.0.9/probability/distributions/mixins/rv_mixins.py`

 * *Files identical despite different names*

### Comparing `probability-0.0.8/probability/distributions/mixins/conjugate_mixin.py` & `probability-0.0.9/probability/distributions/mixins/conjugate_mixin.py`

 * *Files identical despite different names*

### Comparing `probability-0.0.8/probability/distributions/discrete/poisson.py` & `probability-0.0.9/probability/distributions/discrete/poisson.py`

 * *Files identical despite different names*

### Comparing `probability-0.0.8/probability/distributions/discrete/negative_binomial.py` & `probability-0.0.9/probability/distributions/discrete/negative_binomial.py`

 * *Files identical despite different names*

### Comparing `probability-0.0.8/probability/distributions/discrete/binomial.py` & `probability-0.0.9/probability/distributions/discrete/binomial.py`

 * *Files identical despite different names*

### Comparing `probability-0.0.8/probability/distributions/special/_no_numba.py` & `probability-0.0.9/probability/distributions/special/_no_numba.py`

 * *Files identical despite different names*

### Comparing `probability-0.0.8/probability/distributions/special/_with_numba.py` & `probability-0.0.9/probability/distributions/special/_with_numba.py`

 * *Files identical despite different names*

### Comparing `probability-0.0.8/probability/distributions/functions/discrete_function_1d.py` & `probability-0.0.9/probability/distributions/functions/continuous_function_1d.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,70 +1,59 @@
 from matplotlib.axes import Axes
 from pandas import Series
-from scipy.stats import rv_discrete
+from scipy.stats import rv_continuous
 from typing import Iterable, overload
 
 from probability.distributions.mixins.plottable_mixin import PlottableMixin
 from probability.plots import new_axes
 
 
-class DiscreteFunction1d(object):
+class ContinuousFunction1d(object):
 
-    def __init__(self, distribution: rv_discrete, method_name: str, name: str,
+    def __init__(self, distribution: rv_continuous, method_name: str, name: str,
                  parent: PlottableMixin):
 
         self._distribution = distribution
         self._method_name: str = method_name
         self._name: str = name
         self._method = getattr(distribution, method_name)
         self._parent: PlottableMixin = parent
 
     @overload
-    def at(self, k: int) -> int:
+    def at(self, x: float) -> float:
         pass
 
     @overload
-    def at(self, k: Iterable[int]) -> Series:
+    def at(self, x: Iterable) -> Series:
         pass
 
-    def at(self, k):
+    def at(self, x):
         """
-        Evaluation of the function for each value of k.
+        Log of the probability density function of the given RV.
         """
-        if isinstance(k, int):
-            return self._method(k)
-        elif isinstance(k, Iterable):
-            return Series(index=k, data=self._method(k), name=self._name)
+        if isinstance(x, float):
+            return self._method(x)
+        elif isinstance(x, Iterable):
+            return Series(index=x, data=self._method(x), name=self._name)
 
-    def plot(self, k: Iterable[int], color: str = 'C0', kind: str = 'bar', ax: Axes = None,
+    def plot(self, x: Iterable, kind: str = 'line', color: str = 'C0', ax: Axes = None,
              **kwargs) -> Axes:
         """
         Plot the function.
 
-        :param k: Range of values of k to plot p(k) over.
-        :param color: Optional color for the series.
+        :param x: Range of values of x to plot p(x) over.
         :param kind: Kind of plot e.g. 'bar', 'line'.
+        :param color: Optional color for the series.
         :param ax: Optional matplotlib axes to plot on.
         :param kwargs: Additional arguments for the matplotlib plot function.
         """
-        data: Series = self.at(k)
+        data: Series = self.at(x)
         ax = ax or new_axes()
-
-        # special kwargs
-        vlines = None
-        if 'vlines' in kwargs.keys():
-            vlines = kwargs.pop('vlines')
-
-        if self._name == 'PMF':
-            data.plot(kind=kind, label=self._parent.label, color=color,
-                      ax=ax, **kwargs)
-        elif self._name == 'CDF':
-            data.plot(kind='line', label=self._parent.label, color=color,
-                      drawstyle='steps-post', ax=ax,
-                      **kwargs)
+        if self._name in ('PDF', 'CDF', 'log(PDF)'):
+            if 'label' not in kwargs.keys():
+                kwargs['label'] = self._parent.label
+            data.plot(kind=kind, color=color, ax=ax, **kwargs)
         else:
             raise ValueError('plot not implemented for {}'.format(self._name))
-        if vlines:
-            ax.vlines(x=k, ymin=0, ymax=data.values, color=color)
         ax.set_xlabel(self._parent.x_label)
         ax.set_ylabel(self._name)
         return ax
```

### Comparing `probability-0.0.8/probability/distributions/functions/continuous_function_1d.py` & `probability-0.0.9/probability/distributions/functions/discrete_function_1d.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,57 +1,70 @@
 from matplotlib.axes import Axes
 from pandas import Series
-from scipy.stats import rv_continuous
+from scipy.stats import rv_discrete
 from typing import Iterable, overload
 
 from probability.distributions.mixins.plottable_mixin import PlottableMixin
 from probability.plots import new_axes
 
 
-class ContinuousFunction1d(object):
+class DiscreteFunction1d(object):
 
-    def __init__(self, distribution: rv_continuous, method_name: str, name: str,
+    def __init__(self, distribution: rv_discrete, method_name: str, name: str,
                  parent: PlottableMixin):
 
         self._distribution = distribution
         self._method_name: str = method_name
         self._name: str = name
         self._method = getattr(distribution, method_name)
         self._parent: PlottableMixin = parent
 
     @overload
-    def at(self, x: float) -> float:
+    def at(self, k: int) -> int:
         pass
 
     @overload
-    def at(self, x: Iterable) -> Series:
+    def at(self, k: Iterable[int]) -> Series:
         pass
 
-    def at(self, x):
+    def at(self, k):
         """
-        Log of the probability density function of the given RV.
+        Evaluation of the function for each value of k.
         """
-        if isinstance(x, float):
-            return self._method(x)
-        elif isinstance(x, Iterable):
-            return Series(index=x, data=self._method(x), name=self._name)
+        if isinstance(k, int):
+            return self._method(k)
+        elif isinstance(k, Iterable):
+            return Series(index=k, data=self._method(k), name=self._name)
 
-    def plot(self, x: Iterable, kind: str = 'line', color: str = 'C0', ax: Axes = None,
+    def plot(self, k: Iterable[int], color: str = 'C0', kind: str = 'bar', ax: Axes = None,
              **kwargs) -> Axes:
         """
         Plot the function.
 
-        :param x: Range of values of x to plot p(x) over.
-        :param kind: Kind of plot e.g. 'bar', 'line'.
+        :param k: Range of values of k to plot p(k) over.
         :param color: Optional color for the series.
+        :param kind: Kind of plot e.g. 'bar', 'line'.
         :param ax: Optional matplotlib axes to plot on.
         :param kwargs: Additional arguments for the matplotlib plot function.
         """
-        data: Series = self.at(x)
+        data: Series = self.at(k)
         ax = ax or new_axes()
-        if self._name in ('PDF', 'CDF', 'log(PDF)'):
-            data.plot(kind=kind, label=self._parent.label, color=color, ax=ax, **kwargs)
+
+        # special kwargs
+        vlines = None
+        if 'vlines' in kwargs.keys():
+            vlines = kwargs.pop('vlines')
+        if 'label' not in kwargs.keys():
+            kwargs['label'] = self._parent.label
+
+        if self._name == 'PMF':
+            data.plot(kind=kind, color=color, ax=ax, **kwargs)
+        elif self._name == 'CDF':
+            data.plot(kind='line', color=color, drawstyle='steps-post', ax=ax,
+                      **kwargs)
         else:
             raise ValueError('plot not implemented for {}'.format(self._name))
+        if vlines:
+            ax.vlines(x=k, ymin=0, ymax=data.values, color=color)
         ax.set_xlabel(self._parent.x_label)
         ax.set_ylabel(self._name)
         return ax
```

### Comparing `probability-0.0.8/probability/distributions/functions/discrete_function_nd.py` & `probability-0.0.9/probability/distributions/functions/discrete_function_nd.py`

 * *Files identical despite different names*

### Comparing `probability-0.0.8/probability/distributions/functions/continuous_function_nd.py` & `probability-0.0.9/probability/distributions/functions/continuous_function_nd.py`

 * *Files identical despite different names*

### Comparing `probability-0.0.8/probability/distributions/conjugate/gamma_exponential.py` & `probability-0.0.9/probability/distributions/conjugate/gamma_exponential.py`

 * *Files identical despite different names*

### Comparing `probability-0.0.8/probability/distributions/conjugate/beta_binomial.py` & `probability-0.0.9/probability/distributions/conjugate/beta_binomial.py`

 * *Files identical despite different names*

### Comparing `probability-0.0.8/probability/distributions/conjugate/beta_geometric.py` & `probability-0.0.9/probability/distributions/conjugate/beta_geometric.py`

 * *Files identical despite different names*

### Comparing `probability-0.0.8/probability/distributions/conjugate/inv_gamma_normal.py` & `probability-0.0.9/probability/distributions/conjugate/inv_gamma_normal.py`

 * *Files identical despite different names*

### Comparing `probability-0.0.8/probability/distributions/conjugate/normal_normal.py` & `probability-0.0.9/probability/distributions/conjugate/normal_normal.py`

 * *Files identical despite different names*

### Comparing `probability-0.0.8/probability/distributions/conjugate/gamma_normal.py` & `probability-0.0.9/probability/distributions/conjugate/gamma_normal.py`

 * *Files identical despite different names*

### Comparing `probability-0.0.8/probability/distributions/continuous/laplace.py` & `probability-0.0.9/probability/distributions/continuous/laplace.py`

 * *Files identical despite different names*

### Comparing `probability-0.0.8/probability/distributions/continuous/lomax.py` & `probability-0.0.9/probability/distributions/continuous/lomax.py`

 * *Files identical despite different names*

### Comparing `probability-0.0.8/probability/distributions/continuous/normal.py` & `probability-0.0.9/probability/distributions/continuous/normal.py`

 * *Files identical despite different names*

### Comparing `probability-0.0.8/probability/distributions/continuous/beta.py` & `probability-0.0.9/probability/distributions/continuous/beta.py`

 * *Files identical despite different names*

### Comparing `probability-0.0.8/probability/distributions/continuous/__init__.py` & `probability-0.0.9/probability/distributions/continuous/__init__.py`

 * *Files identical despite different names*

### Comparing `probability-0.0.8/probability/distributions/continuous/exponential.py` & `probability-0.0.9/probability/distributions/continuous/exponential.py`

 * *Files identical despite different names*

### Comparing `probability-0.0.8/probability/distributions/continuous/inv_gamma.py` & `probability-0.0.9/probability/distributions/continuous/inv_gamma.py`

 * *Files identical despite different names*

### Comparing `probability-0.0.8/probability/distributions/continuous/gamma.py` & `probability-0.0.9/probability/distributions/continuous/gamma.py`

 * *Files identical despite different names*

### Comparing `probability-0.0.8/probability/distributions/continuous/students_t.py` & `probability-0.0.9/probability/distributions/continuous/students_t.py`

 * *Files identical despite different names*

### Comparing `probability-0.0.8/probability/pandas/prob_utils.py` & `probability-0.0.9/probability/discrete/prob_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from collections import OrderedDict
+
 from pandas import merge, Series, DataFrame
 from typing import Any, Tuple, List
 
 """
 The following methods assume that the distribution is represented as follows.
 - The distribution is a pandas Series.
 - The columns of the index are named after the variables in the distribution.
@@ -13,15 +15,15 @@
 
 def margin(distribution: Series, *margins) -> Series:
     """
     Marginalize the distribution over the variables not in args, leaving the marginal probability of args.
 
     :param distribution: The probability distribution to marginalize e.g. P(A,B,C,D).
     :param margins: Names of variables to put in the margin e.g. 'C', 'D'.
-    :return: P(C,D)
+    :return: Marginalized distribution e.g. P(C,D).
     """
     return distribution.to_frame().groupby(list(margins))['p'].sum()
 
 
 _match_codes: List[str] = ['eq', 'ne', 'lt', 'gt', 'le', 'ge', 'in', 'not_in']
 comparator_symbols = {
     'eq': lambda arg, val: f'{arg}={val}',
@@ -86,27 +88,28 @@
         return distribution.loc[distribution[name_comparator[: -4]] >= value], name_comparator[: -4]
     elif match_var('in'):
         return distribution.loc[distribution[name_comparator[: -4]].isin(value)], name_comparator[: -4]
     elif match_var('not_in'):
         return distribution.loc[~distribution[name_comparator[: -8]].isin(value)], name_comparator[: -8]
 
 
-def cond_name(name_comparator: str, var_names: List[str]) -> str:
+def cond_name(name_comparator: str, var_names: List[str] = None) -> str:
     """
     Return the conditioning variable name from the name and comparator code.
 
     :param name_comparator: Amalgamation of variable name and filtering comparator in the form '{name}__{comparator}'.
     :param var_names: List of valid variables names to look for in `name_comparator`.
     """
-    if name_comparator in var_names:
-        return name_comparator
-    for var_name in var_names:
-        for code in _match_codes:
-            if var_name + '__' + code == name_comparator:
-                return var_name
+    if var_names is not None:
+        if name_comparator in var_names:
+            return name_comparator
+    for code in _match_codes:
+        if name_comparator.endswith('__' + code):
+            return name_comparator[:-len('__' + code)]
+    return name_comparator
 
 
 def cond_name_and_symbol(name_comparator: str, value, var_names: List[str]) -> str:
     """
     Return the conditioning variable name and mathematical symbol from the name and comparator code.
 
     :param name_comparator: Amalgamation of variable name and filtering comparator in the form '{name}__{comparator}'.
@@ -124,31 +127,31 @@
 def condition(distribution: Series, *cond_vars) -> Series:
     """
     Condition the distribution on given and/or not-given values of the variables.
 
     :param distribution: The probability distribution to condition e.g. P(A,B,C,D).
     :param cond_vars: Names of variables to condition over every value of e.g. 'C'.
     :return: Conditioned distribution. Filtered to only given values of the cond_values.
-             Contains a stacked Series of probabily distributions for each combination of conditioning variable values.
+             Contains a stacked Series of probability distributions for each combination of conditioning variable values.
              e.g. P(A,B|C,D=d1), P(A,B|C,D=d2) etc.
     """
     col_names = distribution.index.names
     var_names = ([
         n for n in col_names
         if n not in cond_vars
     ])
     var_names.extend([n for n in col_names if n in cond_vars])
     data = distribution.copy().reset_index()
-    not_given_vars = list(cond_vars)
-    if not_given_vars:
+    cond_vars = list(cond_vars)
+    if cond_vars:
         # find total probabilities for each combination of unique values in the conditional variables e.g. P(C)
-        sums = data.groupby(not_given_vars).sum().reset_index()
+        sums = data.groupby(cond_vars).sum().reset_index()
         # normalize each individual probability e.g. p(Ai,Bj,Ck,Dl) to probability of its conditional values p(Ck)
-        sums = sums[not_given_vars + ['p']].rename(columns={'p': 'p_sum'})
-        merged = merge(left=data, right=sums, on=not_given_vars)
+        sums = sums[cond_vars + ['p']].rename(columns={'p': 'p_sum'})
+        merged = merge(left=data, right=sums, on=cond_vars)
         merged['p'] = merged['p'] / merged['p_sum']
         data = merged[var_names + ['p']]
     return data.set_index(var_names)['p']
 
 
 def given(distribution: Series, **givens) -> Series:
     """
@@ -156,34 +159,58 @@
 
     :param distribution: The probability distribution to condition e.g. P(A,B,C,D).
     :param givens: Names and values of variables to condition on a given value e.g. D=1.
     :return: Conditioned distribution. Filtered to only given values of the cond_values.
              Contains a single probability distribution summing to 1.
     """
     col_names = distribution.index.names
-    var_names = ([
+    joint_names = ([
         n for n in col_names
-        if n not in givens.keys()
-        and not set([f'{n}__{code}' for code in _match_codes]).intersection(givens.keys())
+        if n not in givens.keys()  # not a given variable name without comparator
+        and not set(
+            [f'{n}__{code}' for code in _match_codes]
+        ).intersection(givens.keys())  # not a given variable name with comparator
     ])
+    var_names = joint_names.copy()
     data = distribution.copy().reset_index()
     for given_var, given_val in givens.items():
         # filter individual probabilities to given values e.g. P(A,B,C,D=d1)
         data, var_name = _filter_distribution(data, given_var, given_val)
         var_names.append(var_name)
     # normalize each individual remaining probability P(Ai,Bj,Ck,d1)
     # to the sum of remaining probabilities P(A,B,C,d1)
     data['p'] = data['p'] / data['p'].sum()
-    return data.set_index([var_name for var_name in var_names if var_name not in givens.keys()])['p']
+    return data.set_index([
+        var_name for var_name in var_names if var_name not in givens.keys()
+    ])['p']
+
+
+def p(distribution: Series, **joint_vars_vals) -> float:
+    """
+    Calculate the probability of the values of the joint values given.
+
+    :param distribution: Probability distribution data to calculate probability from.
+    :param joint_vars_vals: Names and values of variables to find probability of e.g. `C=1`, `D__le=1`.
+    """
+    data = distribution.copy().reset_index()
+    for joint_var, joint_val in joint_vars_vals.items():
+        # filter individual probabilities to specified values e.g. P(A,B,C,D=d1)
+        data, var_name = _filter_distribution(data, joint_var, joint_val)
+    # calculate probability
+    return data['p'].sum()
 
 
 def multiply(conditional: Series, marginal: Series) -> Series:
+    """
+    Multiply a conditional distribution by a marginal distribution to give a joint distribution.
 
-    # P(a,b) = P(a|b) * P(b)
-    # joint = conditional * marginal
+    :param conditional: The conditional distribution e.g. P(a|b)
+    :param marginal: The marginal distribution e.g. P(b)
+    :return: The joint distribution e.g. P(a,b)
+    """
     marginal_vars = marginal.index.names
     non_marginal_vars = [v for v in conditional.index.names if v not in marginal_vars]
     cond_data = conditional.copy().rename('p_cond').to_frame().reset_index()
     joint_data = marginal.copy().rename('p_joint').to_frame().reset_index()
     merged = merge(left=cond_data, right=joint_data, on=marginal_vars)
     merged['p'] = merged['p_cond'] * merged['p_joint']
     results = merged.groupby(non_marginal_vars + marginal_vars)['p'].sum()
```

### Comparing `probability-0.0.8/probability/pandas/variable_filter.py` & `probability-0.0.9/probability/discrete/variable_filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pandas import DataFrame, Series
 import re
 from typing import Any, List, Optional
 
-from probability.pandas.prob_utils import comparator_symbols
+from probability.discrete.prob_utils import comparator_symbols
 
 
 class VariableFilter(object):
 
     re_var_comparator = re.compile(
         r'(\w+)__((?:eq)|(?:ne)|(?:lt)|(?:gt)|(?:le)|(?:ge)|(?:in)|(?:not_in))'
     )
```

### Comparing `probability-0.0.8/probability/pandas/conditional_table.py` & `probability-0.0.9/probability/discrete/conditional_table.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,43 +1,64 @@
 from pandas import Series
-from typing import List, Optional
+from typing import Dict, List, Union
 
-from probability.pandas import DiscreteDistribution
-from probability.pandas.prob_utils import margin, given
+from probability.discrete.discrete_distribution import DiscreteDistribution
+from probability.discrete.prob_utils import margin, given
 
 
 class ConditionalTable(object):
 
-    def __init__(self, data: Series,
-                 cond_variables: Optional[List[str]] = None):
+    def __init__(self, data: Series, cond_var_names: Union[str, List[str]]):
+        """
+        Create a new Conditional Table from a Series of probabilities.
 
-        self._data: Series = data.copy()
+        :param data: Series mapping values of random variables to their probabilities.
+        :param cond_var_names: Names of conditional variables.
+        """
+        # self._data: Series = data.copy()
         self._var_names: List[str] = list(data.index.names)
-        self._cond_vars: List[str] = cond_variables or []
-        self._joints: List[str] = [n for n in self._var_names if n not in self._cond_vars]
+        self._cond_var_names: List[str] = [cond_var_names] if isinstance(cond_var_names, str) else cond_var_names
+        self._joints: List[str] = [n for n in self._var_names if n not in self._cond_var_names]
+        var_order = self._joints + self._cond_var_names
+        self._data = data.copy().reset_index()[var_order + ['p']].set_index(var_order)['p']
 
     # region attributes
 
+    @staticmethod
+    def from_dict(data: Dict[Union[str, int, tuple], float],
+                  var_names: Union[str, List[str]],
+                  cond_var_names: Union[str, List[str]] = None):
+        """
+        Create a new Conditional Table from a dictionary of probabilities.
+
+        :param data: Dictionary mapping values of random variables to their probabilities.
+        :param var_names: List of variable names for the elements of the
+        :param cond_var_names: Names of conditional variables.
+        """
+        s_data = Series(data=data, name='p')
+        s_data.index.names = [var_names] if isinstance(var_names, str) else var_names
+        return ConditionalTable(data=s_data, cond_var_names=cond_var_names)
+
     @property
     def name(self) -> str:
 
         str_joints = ','.join(self._joints)
         strs_conditions = []
-        for cond_var in self._cond_vars:
+        for cond_var in self._cond_var_names:
             strs_conditions.append(cond_var)
         str_conditions = '|' + ','.join(strs_conditions) if strs_conditions else ''
         return f'P({str_joints}{str_conditions})'
 
     @property
     def data(self) -> Series:
         return self._data
 
     @property
     def cond_vars(self) -> List[str]:
-        return self._cond_vars
+        return self._cond_var_names
 
     # endregion
 
     # region methods
 
     def margin(self, *margins) -> 'ConditionalTable':
         """
@@ -47,48 +68,49 @@
         """
         # check input arguments
         if not len(margins) > 0:
             raise ValueError('Must pass at least one margin variable.')
         if not set(margins).issubset(self._joints):
             raise ValueError('All margins must be joint variables.')
         # calculate marginal distributions
-        data = margin(self._data, *margins, *self._cond_vars)
-        return ConditionalTable(data=data, cond_variables=self._cond_vars)
+        data = margin(self._data, *margins, *self._cond_var_names)
+        return ConditionalTable(data=data, cond_var_names=self._cond_var_names)
 
     def p(self, **var_vals) -> float:
         """
         Return the probability of the the specified values of the joint and conditional variables.
 
         N.B. need to supply all values for conditional and joint variables.
 
         :param var_vals: Values for each conditional and joint variable.
         """
         # check input arguments
         var_val_keys = set(var_vals.keys())
-        has_all_conds = set(self._cond_vars).intersection(var_val_keys) == set(self._cond_vars)
+        has_all_conds = set(self._cond_var_names).intersection(var_val_keys) == set(self._cond_var_names)
         has_all_joints = set(self._joints).intersection(var_val_keys) == set(self._joints)
         if not has_all_conds and has_all_joints:
             raise ValueError('Must specify a value for each conditional and joint variable.')
-        if not len(self._cond_vars) + len(self._joints) == len(var_vals):
+        if not len(self._cond_var_names) + len(self._joints) == len(var_vals):
             raise ValueError('Too many variable values passed.')
         # calculate probability
         joint_cond_vals = [var_vals[name] for name in self._data.index.names]
         if len(joint_cond_vals) == 1:
             joint_cond_vals = joint_cond_vals[0]
         return self._data.xs(joint_cond_vals)
 
     def given(self, **given_vals) -> DiscreteDistribution:
         """
         Return the Discrete Distribution at the given values of the conditional variables.
+        N.B. will give incorrect results if the conditional table was created from incomplete distributions.
 
         :param given_vals: Values of conditional variables to create probability distribution from.
         """
         # check input arguments
         given_val_keys = set(given_vals.keys())
-        has_all_conds = set(self._cond_vars).intersection(given_val_keys) == set(self._cond_vars)
+        has_all_conds = set(self._cond_var_names).intersection(given_val_keys) == set(self._cond_var_names)
         if not has_all_conds:
             raise ValueError('Must supply values for all conditioned variables to get to joint distribution.')
         # calculate probability
         data = given(self._data, **given_vals)
         return DiscreteDistribution(data, given_conditions=given_vals)
 
     # endregion
```

### Comparing `probability-0.0.8/probability/pandas/discrete_distribution.py` & `probability-0.0.9/probability/discrete/discrete_distribution.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,40 @@
+from collections import OrderedDict
+
 from pandas import Index, MultiIndex, Series, DataFrame
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Dict, List, Optional, Union, overload, TYPE_CHECKING
+
+from probability.discrete.prob_utils import margin, condition, multiply, cond_name_and_symbol, given, valid_name_comparator, \
+    cond_name, p
 
-from probability.pandas.prob_utils import margin, condition, multiply, cond_name_and_symbol, given, valid_name_comparator, \
-    cond_name
+if TYPE_CHECKING:
+    from probability.discrete import ConditionalTable
 
 
 class DiscreteDistribution(object):
 
     def __init__(self, data: Series,
-                 given_var_names: List[str] = None,
+                 cond_var_names: List[str] = None,
                  given_conditions: Optional[Dict[str, Any]] = None):
         """
         Create a new DiscreteDistribution e.g. `P(A,B,C,D)`.
 
         :param data: Series with an index column for each variable, and values of probability of each index row.
-        :param given_var_names: List of names of conditioned variables with given values.
+        :param cond_var_names: List of names of conditioned variables without given values.
         :param given_conditions: Dict[{name}__{comparator}, value] for each conditioned variable.
         """
         self._data: Series = data.copy()
-        self._joints: List[str] = list(data.index.names)
-        self._given_vars = given_var_names or []
+        self._cond_var_names = cond_var_names or []
+        self._joints: List[str] = [name for name in list(data.index.names) if name not in self._cond_var_names]
         self._given_conditions: Dict[str, Any] = given_conditions or {}
-        self._var_names: List[str] = self._joints + self._given_vars
+        self._var_names: List[str] = (
+            self._joints +
+            self._cond_var_names +
+            [cond_name(k) for k in self._given_conditions.keys()]
+        )
 
     # region constructors
 
     @staticmethod
     def from_dict(data: Dict[Union[str, int, tuple], float],
                   var_names: Union[str, List[str]],
                   **given_conditions) -> 'DiscreteDistribution':
@@ -43,15 +52,15 @@
         elif type(first_key) in (str, int):
             index = Index(list(data.keys()),
                           name=var_names[0] if isinstance(var_names, list) else var_names)
         else:
             raise TypeError('probs must be Dict[[Union[str, int, tuple], float]')
         data = Series(data=list(data.values()), index=index, name='p')
         return DiscreteDistribution(data,
-                                    given_var_names=list(given_conditions.keys()),
+                                    cond_var_names=list(given_conditions.keys()),
                                     given_conditions=given_conditions)
 
     @staticmethod
     def from_counts(counts: Dict[Union[str, int], int],
                     names: Union[str, List[str]]) -> 'DiscreteDistribution':
         """
         Return a new joint distribution from counts of random variable values.
@@ -89,14 +98,21 @@
     def joints(self) -> List[str]:
         """
         Return a list of the names of all joint variables.
         """
         return self._joints
 
     @property
+    def cond_var_names(self) -> List[str]:
+        """
+        Return a list of the names of all conditional variables.
+        """
+        return self._cond_var_names
+
+    @property
     def given_conditions(self) -> Dict[str, Any]:
         """
         Return the names and given values of conditioned variables.
         """
         return self._given_conditions
 
     @property
@@ -110,14 +126,16 @@
     def name(self) -> str:
         """
         Return a name for the distribution based on the names of the joint variables and the names,
         conditional comparators and values of the given variables.
         """
         str_joints = ','.join(self._joints)
         strs_conditions = []
+        for cond_var in self._cond_var_names:
+            strs_conditions.append(cond_var)
         for cond_var, cond_val in self.given_conditions.items():
             strs_conditions.append(cond_name_and_symbol(cond_var, cond_val, self.var_names))
         str_conditions = '|' + ','.join(strs_conditions) if strs_conditions else ''
         return f'P({str_joints}{str_conditions})'
 
     # endregion
 
@@ -149,16 +167,16 @@
         # check input variables
         if not set(cond_var_names).issubset(self._joints):
             raise ValueError('All conditioning variables must be joint variables.')
         if not len(cond_var_names) < len(self._joints):
             raise ValueError('Cannot condition on all joint variables simultaneously.')
         # calculate conditional table
         data = condition(self._data, *cond_var_names)
-        from probability.pandas.conditional_table import ConditionalTable
-        return ConditionalTable(data, cond_variables=[cv for cv in cond_var_names])
+        from probability.discrete.conditional_table import ConditionalTable
+        return ConditionalTable(data, cond_var_names=[cv for cv in cond_var_names])
 
     def given(self, **given_conditions) -> 'DiscreteDistribution':
         """
         Condition on values of variables.
 
         :param given_conditions: Dict[{name}__{comparator}, value] for each conditioned variable.
         """
@@ -167,67 +185,103 @@
         if not all([valid_name_comparator(name_comp, self._joints) for name_comp in names_comps]):
             raise ValueError('Given variables must be members of joint distribution.')
         # calculate conditional distribution
         data = given(self._data, **given_conditions)
         cond_values = {**self._given_conditions, **given_conditions}
         return DiscreteDistribution(
             data=data,
-            given_var_names=self._given_vars + [cond_name(k, self.var_names) for k in names_comps],
+            cond_var_names=self._cond_var_names,
             given_conditions=cond_values
         )
 
     def p(self, **joint_vals) -> float:
         """
         Return the value of the probability distribution at the values of the joint variables.
 
         :param joint_vals: Dict[name, value] for each joint variable to find probability at.
         """
         # check input variables
-        if not set(joint_vals.keys()) == set(self._joints):
-            raise ValueError('Must specify a value for each conditioned variable.')
+        joint_arg_names = set([cond_name(joint_var, self._joints)
+                               for joint_var in joint_vals.keys()])
+        if not joint_arg_names == set(self._joints):
+            raise ValueError('Must specify a value (+condition) for each joint variable.')
         # find probability of joint variable values
-        var_vals = [joint_vals[name] for name in self._data.index.names]
-        if len(var_vals) == 1:
-            var_vals = var_vals[0]
-        try:
-            return self._data.xs(var_vals)
-        except KeyError:
-            # not all values are in distribution variable values
-            return 0.0
+        return p(self._data, **joint_vals)
 
     # endregion
 
     # region operators
 
+    @overload
+    def __mul__(self, other: 'DiscreteDistribution') -> 'DiscreteDistribution':
+        """
+        Multiply the joint distribution e.g. `P(A)` by another DiscreteDistribution e.g. P(B) and return a new
+        joint distribution i.e. `P(A,B)`. Assumes that P(A) and P(B) are independent such that P(A) = P(A)  P(B)
+
+        :param other: DiscreteDistribution to multiply by.
+        """
+        pass
+
+    @overload
     def __mul__(self, other: 'ConditionalTable') -> 'DiscreteDistribution':
         """
-        Multiply the joint distribution e.g. `P(B)` by another ConditionalTable conditioned over this distribution's
+        Multiply the joint distribution e.g. `P(B)` by a ConditionalTable conditioned over this distribution's
         joint variables e.g. `P(A|B)` and return a new joint distribution i.e. `P(A)` over the ConditionalTable's
         joint variables i.e. `A`.
 
-        :param other: Conditional Table with conditional variables matching this distributions joint variables.
+        :param other: ConditionalTable with conditional variables matching this distributions joint variables.
         """
-        if self.joints == other.cond_vars and not self.given_conditions:
+        pass
+
+    def __mul__(self, other):
+
+        from probability.discrete import ConditionalTable
+        if isinstance(other, ConditionalTable):
+            if self.given_conditions:
+                raise ValueError('DiscreteDistribution cannot have any conditional variables.')
+            if set(self.joints) != set(other.cond_vars):
+                raise ValueError('Joint variables of DiscreteDistribution must be same as'
+                                 ' conditional variables of ConditionalTable.')
             data = multiply(conditional=other.data, marginal=self.data)
             return DiscreteDistribution(data=data)
-        else:
-            raise ValueError('Cannot multiply these distributions.')
+        elif isinstance(other, DiscreteDistribution):
+            if self.given_conditions or other.given_conditions or self.cond_var_names or other.cond_var_names:
+                raise ValueError('Neither DiscreteDistribution should have conditional variables or values.')
+            if set(self.var_names).intersection(other.var_names):
+                raise ValueError('DiscreteDistributions have shared variables.')
+            keys = []
+            values = []
+            for ix_1, p_1 in self._data.iteritems():
+                for ix_2, p_2 in other._data.iteritems():
+                    if not isinstance(ix_1, tuple):
+                        ix_1 = (ix_1,)
+                    if not isinstance(ix_2, tuple):
+                        ix_2 = (ix_2,)
+                    keys.append((*ix_1, *ix_2))
+                    values.append(p_1 * p_2)
+            data = Series(data=values,
+                          index=MultiIndex.from_tuples(
+                              tuples=keys,
+                              names=self._data.index.names + other._data.index.names
+                          ))
+            return DiscreteDistribution(data=data)
 
     def __rmul__(self, other: 'ConditionalTable') -> 'DiscreteDistribution':
         return self * other
 
     def __truediv__(self, other: 'DiscreteDistribution') -> 'ConditionalTable':
 
         if not set(other.joints).issubset(self.joints):
             raise ValueError(
                 'All joint variables in denominator distribution must be present in numerator distribution to divide.'
             )
         if not len(other.joints) < len(self.joints):
             raise ValueError('Denominator distribution must contain fewer joint variables than numerator distribution.')
-        return self.condition(*other.joints)
+        from probability.discrete.conditional_table import ConditionalTable
+        return ConditionalTable(data=self._data / other._data, cond_var_names=other.joints)
 
     # endregion
 
     def __repr__(self):
 
         return self.name
```

### Comparing `probability-0.0.8/tests/shared.py` & `probability-0.0.9/tests/shared.py`

 * *Files identical despite different names*

### Comparing `probability-0.0.8/tests/test_pandas/test_conditional_table.py` & `probability-0.0.9/tests/test_discrete/test_conditional_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from unittest import TestCase
 
-from probability.pandas import DiscreteDistribution
+from probability.discrete import DiscreteDistribution
 from tests.shared import read_distribution_data, series_are_equivalent
 
 
 class TestConditionalTable(TestCase):
 
     def setUp(self) -> None:
```

### Comparing `probability-0.0.8/tests/test_pandas/test_examples.py` & `probability-0.0.9/tests/test_discrete/test_examples.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from itertools import product
 from unittest import TestCase
 
 from pandas import DataFrame, Series
 
-from probability.pandas import DiscreteDistribution
+from probability.discrete import DiscreteDistribution
 
 
 class TestExamples(TestCase):
 
     def test_fruit_box(self):
         fruit_box_data = DataFrame({
             'box': ['red'] * 8 + ['blue'] * 4,
```

### Comparing `probability-0.0.8/tests/test_pandas/test_prob_utils.py` & `probability-0.0.9/tests/test_discrete/test_prob_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from itertools import product, permutations
 from pandas import ExcelFile
 import unittest
 from unittest import TestCase
 
-from probability.pandas.prob_utils import margin, condition, multiply, given
+from probability.discrete.prob_utils import margin, condition, multiply, given, p
 
 from tests.paths import FN_PANDAS_TESTS
 from tests.shared import read_distribution_data, series_are_equivalent
 
 
 class TestProbUtils(TestCase):
 
@@ -121,11 +121,24 @@
         p_A__B = condition(p_AB, 'B')
         p_B__A = condition(p_AB, 'A')
         p_A__B_p_B = multiply(p_A__B, p_B)
         p_B__A_p_A = multiply(p_B__A, p_A)
         self.assertTrue(series_are_equivalent(p_A__B_p_B, p_AB))
         self.assertTrue(series_are_equivalent(p_B__A_p_A, p_AB))
 
+    def test_p(self):
+
+        self.assertAlmostEqual(0.33, p(self.p_A, A=1))
+        self.assertAlmostEqual(0.36, p(self.p_A, A=2))
+        self.assertAlmostEqual(0.31, p(self.p_A, A=3))
+        self.assertAlmostEqual(0.33, p(self.p_A, A__lt=2))
+        self.assertAlmostEqual(0.31, p(self.p_A, A__gt=2))
+        self.assertAlmostEqual(0.33 + 0.31, p(self.p_A, A__ne=2))
+        self.assertAlmostEqual(0.33 + 0.36, p(self.p_A, A__le=2))
+        self.assertAlmostEqual(0.36 + 0.31, p(self.p_A, A__ge=2))
+        self.assertAlmostEqual(0.33 + 0.31, p(self.p_A, A__in=[1, 3]))
+        self.assertAlmostEqual(0.36, p(self.p_A, A__not_in=[1, 3]))
+
 
 if __name__ == '__main__':
 
     unittest.main()
```

### Comparing `probability-0.0.8/probability.egg-info/SOURCES.txt` & `probability-0.0.9/probability.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 setup.cfg
 setup.py
 examples/__init__.py
 examples/colors.py
+examples/discrete/__init__.py
+examples/discrete/discrete_distribution.py
 examples/distributions/__init__.py
 examples/distributions/conjugate/__init__.py
 examples/distributions/conjugate/beta_binomial.py
 examples/distributions/conjugate/gamma_exponential.py
 examples/distributions/conjugate/gamma_normal.py
 examples/distributions/conjugate/inv_gamma_normal.py
 examples/distributions/conjugate/normal_normal.py
@@ -23,25 +25,28 @@
 examples/distributions/discrete/binomial.py
 examples/distributions/discrete/multinomial.py
 examples/distributions/discrete/negative_binomial.py
 examples/distributions/discrete/poisson.py
 examples/distributions/multivariate/__init__.py
 examples/distributions/multivariate/dirichlet.py
 examples/distributions/multivariate/mv_normal.py
-examples/pandas/__init__.py
-examples/pandas/discrete_distribution.py
 probability/__init__.py
 probability/custom_types.py
 probability/plots.py
 probability/utils.py
 probability.egg-info/PKG-INFO
 probability.egg-info/SOURCES.txt
 probability.egg-info/dependency_links.txt
 probability.egg-info/requires.txt
 probability.egg-info/top_level.txt
+probability/discrete/__init__.py
+probability/discrete/conditional_table.py
+probability/discrete/discrete_distribution.py
+probability/discrete/prob_utils.py
+probability/discrete/variable_filter.py
 probability/distributions/__init__.py
 probability/distributions/conjugate/__init__.py
 probability/distributions/conjugate/beta_binomial.py
 probability/distributions/conjugate/beta_geometric.py
 probability/distributions/conjugate/dirichlet_multinomial.py
 probability/distributions/conjugate/gamma_exponential.py
 probability/distributions/conjugate/gamma_normal.py
@@ -78,20 +83,15 @@
 probability/distributions/multivariate/__init__.py
 probability/distributions/multivariate/dirichlet.py
 probability/distributions/multivariate/multinomial.py
 probability/distributions/multivariate/mv_normal.py
 probability/distributions/special/__init__.py
 probability/distributions/special/_no_numba.py
 probability/distributions/special/_with_numba.py
-probability/pandas/__init__.py
-probability/pandas/conditional_table.py
-probability/pandas/discrete_distribution.py
-probability/pandas/prob_utils.py
-probability/pandas/variable_filter.py
 tests/__init__.py
 tests/paths.py
 tests/shared.py
-tests/test_pandas/__init__.py
-tests/test_pandas/test_conditional_table.py
-tests/test_pandas/test_discrete_distribution.py
-tests/test_pandas/test_examples.py
-tests/test_pandas/test_prob_utils.py
+tests/test_discrete/__init__.py
+tests/test_discrete/test_conditional_table.py
+tests/test_discrete/test_discrete_distribution.py
+tests/test_discrete/test_examples.py
+tests/test_discrete/test_prob_utils.py
```

### Comparing `probability-0.0.8/setup.py` & `probability-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 setup(
   name='probability',
   packages=find_packages(),
-  version='0.0.8',
+  version='0.0.9',
   license='MIT',
   description='Probability in Python 3',
   author='Vahndi Minah',
   url='https://github.com/vahndi/probability',
   keywords=['python', 'probability'],
   install_requires=[
         'matplotlib',
```

### Comparing `probability-0.0.8/examples/distributions/discrete/poisson.py` & `probability-0.0.9/examples/distributions/discrete/poisson.py`

 * *Files identical despite different names*

### Comparing `probability-0.0.8/examples/distributions/discrete/multinomial.py` & `probability-0.0.9/examples/distributions/discrete/multinomial.py`

 * *Files identical despite different names*

### Comparing `probability-0.0.8/examples/distributions/discrete/negative_binomial.py` & `probability-0.0.9/examples/distributions/discrete/negative_binomial.py`

 * *Files identical despite different names*

### Comparing `probability-0.0.8/examples/distributions/discrete/binomial.py` & `probability-0.0.9/examples/distributions/discrete/binomial.py`

 * *Files identical despite different names*

### Comparing `probability-0.0.8/examples/distributions/conjugate/gamma_exponential.py` & `probability-0.0.9/examples/distributions/conjugate/gamma_exponential.py`

 * *Files identical despite different names*

### Comparing `probability-0.0.8/examples/distributions/conjugate/beta_binomial.py` & `probability-0.0.9/examples/distributions/conjugate/beta_binomial.py`

 * *Files identical despite different names*

### Comparing `probability-0.0.8/examples/distributions/conjugate/inv_gamma_normal.py` & `probability-0.0.9/examples/distributions/conjugate/inv_gamma_normal.py`

 * *Files identical despite different names*

### Comparing `probability-0.0.8/examples/distributions/conjugate/normal_normal.py` & `probability-0.0.9/examples/distributions/conjugate/normal_normal.py`

 * *Files identical despite different names*

### Comparing `probability-0.0.8/examples/distributions/conjugate/gamma_normal.py` & `probability-0.0.9/examples/distributions/conjugate/gamma_normal.py`

 * *Files identical despite different names*

### Comparing `probability-0.0.8/examples/distributions/continuous/laplace.py` & `probability-0.0.9/examples/distributions/continuous/laplace.py`

 * *Files identical despite different names*

### Comparing `probability-0.0.8/examples/distributions/continuous/lomax.py` & `probability-0.0.9/examples/distributions/continuous/lomax.py`

 * *Files identical despite different names*

### Comparing `probability-0.0.8/examples/distributions/continuous/comparisons.py` & `probability-0.0.9/examples/distributions/continuous/comparisons.py`

 * *Files identical despite different names*

### Comparing `probability-0.0.8/examples/distributions/continuous/normal.py` & `probability-0.0.9/examples/distributions/continuous/normal.py`

 * *Files identical despite different names*

### Comparing `probability-0.0.8/examples/distributions/continuous/beta.py` & `probability-0.0.9/examples/distributions/continuous/beta.py`

 * *Files identical despite different names*

### Comparing `probability-0.0.8/examples/distributions/continuous/exponential.py` & `probability-0.0.9/examples/distributions/continuous/exponential.py`

 * *Files identical despite different names*

### Comparing `probability-0.0.8/examples/distributions/continuous/inv_gamma.py` & `probability-0.0.9/examples/distributions/continuous/inv_gamma.py`

 * *Files identical despite different names*

### Comparing `probability-0.0.8/examples/distributions/continuous/gamma.py` & `probability-0.0.9/examples/distributions/continuous/gamma.py`

 * *Files identical despite different names*

### Comparing `probability-0.0.8/examples/distributions/continuous/students_t.py` & `probability-0.0.9/examples/distributions/continuous/students_t.py`

 * *Files identical despite different names*

### Comparing `probability-0.0.8/examples/pandas/discrete_distribution.py` & `probability-0.0.9/examples/discrete/discrete_distribution.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pandas import DataFrame
 
-from probability.pandas.discrete_distribution import DiscreteDistribution
+from probability.discrete.discrete_distribution import DiscreteDistribution
 
 
 def fruit_boxes():
     """
     Example from Section 1.2 of "Pattern Recognition and Machine Learning"
     """
     fruit_box_data = DataFrame({
```

