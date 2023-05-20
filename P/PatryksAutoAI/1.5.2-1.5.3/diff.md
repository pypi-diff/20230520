# Comparing `tmp/PatryksAutoAI-1.5.2.tar.gz` & `tmp/PatryksAutoAI-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PatryksAutoAI-1.5.2.tar", last modified: Fri May 19 18:50:58 2023, max compression
+gzip compressed data, was "PatryksAutoAI-1.5.3.tar", last modified: Sat May 20 06:12:28 2023, max compression
```

## Comparing `PatryksAutoAI-1.5.2.tar` & `PatryksAutoAI-1.5.3.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-19 18:50:58.061220 PatryksAutoAI-1.5.2/
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-19 18:50:58.053220 PatryksAutoAI-1.5.2/KaggleAutoAI/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      271 2023-05-13 17:48:42.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/__init__.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-19 18:50:58.053220 PatryksAutoAI-1.5.2/KaggleAutoAI/automated_ai/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      101 2023-05-12 20:27:46.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/automated_ai/__init__.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-19 18:50:58.053220 PatryksAutoAI-1.5.2/KaggleAutoAI/automated_ai/algorithms/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       97 2023-05-12 19:31:03.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/automated_ai/algorithms/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     1893 2023-05-12 21:11:33.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/automated_ai/algorithms/complexity_level0.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2230 2023-05-19 09:19:31.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/automated_ai/algorithms/complexity_level1.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-19 18:50:58.053220 PatryksAutoAI-1.5.2/KaggleAutoAI/automated_ai/classification_automated/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      534 2023-05-12 19:33:34.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/automated_ai/classification_automated/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      849 2023-05-12 19:35:36.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/automated_ai/classification_automated/cat_automated.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      880 2023-05-12 19:35:47.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/automated_ai/classification_automated/extra_trees.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      910 2023-05-12 19:35:56.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/automated_ai/classification_automated/gradient_boosting_automated.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      882 2023-05-12 19:36:07.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/automated_ai/classification_automated/hist_gradient_automated.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      860 2023-05-12 19:36:17.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/automated_ai/classification_automated/lgb_automated.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      920 2023-05-12 19:36:29.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/automated_ai/classification_automated/logistic_regression_automated.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      890 2023-05-12 19:36:40.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/automated_ai/classification_automated/random_forest_automated.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      844 2023-05-12 19:36:55.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/automated_ai/classification_automated/xgb_automated.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-19 18:50:58.053220 PatryksAutoAI-1.5.2/KaggleAutoAI/automated_ai/regression_automated/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      308 2023-05-12 19:57:48.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/automated_ai/regression_automated/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      840 2023-05-12 21:49:08.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/automated_ai/regression_automated/cat_automated.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      905 2023-05-12 19:55:05.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/automated_ai/regression_automated/gradient_boosting_automated.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      840 2023-05-12 19:55:24.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/automated_ai/regression_automated/lgb_automated.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      840 2023-05-12 19:56:32.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/automated_ai/regression_automated/xgb_automated.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-19 18:50:58.053220 PatryksAutoAI-1.5.2/KaggleAutoAI/classification/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       72 2023-05-10 18:02:22.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/classification/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      648 2023-04-17 06:33:02.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/classification/metrics.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-19 18:50:58.057220 PatryksAutoAI-1.5.2/KaggleAutoAI/classification/models/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      317 2023-05-10 18:02:39.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/classification/models/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     9064 2023-05-18 09:26:27.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/classification/models/cat.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     7070 2023-05-18 13:47:34.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/classification/models/extra_trees.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6724 2023-05-18 13:47:54.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/classification/models/gradient_boosting.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6921 2023-05-18 13:48:13.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/classification/models/hist_gradient.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2400 2023-05-16 13:32:16.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/classification/models/kneighbours.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     8274 2023-05-18 14:23:56.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/classification/models/light_lgb.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2493 2023-05-16 13:32:12.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/classification/models/linear_svc.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     5866 2023-05-18 13:48:54.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/classification/models/logistic_regression.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     7080 2023-05-17 16:29:50.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/classification/models/random_forest.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2512 2023-05-16 13:31:56.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/classification/models/sgd_classifier.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2732 2023-05-17 18:02:36.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/classification/models/svc.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6875 2023-05-18 13:48:34.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/classification/models/xgb.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      920 2023-03-10 12:07:04.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/helper_function.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-19 18:50:58.057220 PatryksAutoAI-1.5.2/KaggleAutoAI/language_processing/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      192 2023-05-14 19:03:52.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/language_processing/__init__.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-19 18:50:58.057220 PatryksAutoAI-1.5.2/KaggleAutoAI/language_processing/data_manipulation/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      115 2023-05-13 17:40:53.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/language_processing/data_manipulation/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      654 2023-05-12 21:36:49.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/language_processing/data_manipulation/metrics.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6153 2023-05-19 18:50:47.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/language_processing/data_manipulation/text2number.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     4078 2023-05-17 16:36:27.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/language_processing/data_manipulation/text_preprocessing.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-19 18:50:58.057220 PatryksAutoAI-1.5.2/KaggleAutoAI/language_processing/models/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       78 2023-05-16 09:57:09.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/language_processing/models/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     1975 2023-05-16 09:57:20.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/language_processing/models/baseline.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     1759 2023-05-19 09:50:59.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/language_processing/models/transformer_model.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-19 18:50:58.057220 PatryksAutoAI-1.5.2/KaggleAutoAI/model_data/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      110 2023-05-10 18:02:54.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/model_data/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      646 2023-05-16 07:40:06.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/model_data/animated.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6075 2023-04-18 06:00:32.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/model_data/model_data.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-19 18:50:58.057220 PatryksAutoAI-1.5.2/KaggleAutoAI/regression/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       89 2023-05-12 20:27:28.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/regression/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      607 2023-05-09 13:49:56.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/regression/metrics_regression.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-19 18:50:58.061220 PatryksAutoAI-1.5.2/KaggleAutoAI/regression/models/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      216 2023-05-12 20:11:18.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/regression/models/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     7013 2023-05-16 17:25:47.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/regression/models/cat.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2885 2023-05-16 13:17:22.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/regression/models/elastic_net.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6865 2023-05-16 13:17:21.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/regression/models/gradient_boosting.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2807 2023-05-16 13:17:18.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/regression/models/lasso.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6240 2023-05-16 17:26:05.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/regression/models/lgb.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     3095 2023-05-16 13:17:18.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/regression/models/sgd.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2883 2023-05-16 13:17:16.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/regression/models/svr.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     8274 2023-05-16 17:26:31.000000 PatryksAutoAI-1.5.2/KaggleAutoAI/regression/models/xgb.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      538 2023-05-19 18:50:58.061220 PatryksAutoAI-1.5.2/PKG-INFO
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-19 18:50:58.061220 PatryksAutoAI-1.5.2/PatryksAutoAI.egg-info/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      538 2023-05-19 18:50:57.000000 PatryksAutoAI-1.5.2/PatryksAutoAI.egg-info/PKG-INFO
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     3193 2023-05-19 18:50:58.000000 PatryksAutoAI-1.5.2/PatryksAutoAI.egg-info/SOURCES.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)        1 2023-05-19 18:50:57.000000 PatryksAutoAI-1.5.2/PatryksAutoAI.egg-info/dependency_links.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      253 2023-05-19 18:50:57.000000 PatryksAutoAI-1.5.2/PatryksAutoAI.egg-info/requires.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       13 2023-05-19 18:50:57.000000 PatryksAutoAI-1.5.2/PatryksAutoAI.egg-info/top_level.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       38 2023-05-19 18:50:58.061220 PatryksAutoAI-1.5.2/setup.cfg
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     1050 2023-05-19 18:50:51.000000 PatryksAutoAI-1.5.2/setup.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-20 06:12:28.496300 PatryksAutoAI-1.5.3/
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-20 06:12:28.484300 PatryksAutoAI-1.5.3/KaggleAutoAI/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      271 2023-05-13 17:48:42.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/__init__.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-20 06:12:28.484300 PatryksAutoAI-1.5.3/KaggleAutoAI/automated_ai/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      101 2023-05-12 20:27:46.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/automated_ai/__init__.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-20 06:12:28.484300 PatryksAutoAI-1.5.3/KaggleAutoAI/automated_ai/algorithms/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       97 2023-05-12 19:31:03.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/automated_ai/algorithms/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     1893 2023-05-12 21:11:33.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/automated_ai/algorithms/complexity_level0.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2230 2023-05-19 09:19:31.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/automated_ai/algorithms/complexity_level1.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-20 06:12:28.488300 PatryksAutoAI-1.5.3/KaggleAutoAI/automated_ai/classification_automated/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      534 2023-05-12 19:33:34.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/automated_ai/classification_automated/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      849 2023-05-12 19:35:36.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/automated_ai/classification_automated/cat_automated.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      880 2023-05-12 19:35:47.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/automated_ai/classification_automated/extra_trees.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      910 2023-05-12 19:35:56.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/automated_ai/classification_automated/gradient_boosting_automated.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      882 2023-05-12 19:36:07.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/automated_ai/classification_automated/hist_gradient_automated.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      860 2023-05-12 19:36:17.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/automated_ai/classification_automated/lgb_automated.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      920 2023-05-12 19:36:29.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/automated_ai/classification_automated/logistic_regression_automated.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      890 2023-05-12 19:36:40.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/automated_ai/classification_automated/random_forest_automated.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      844 2023-05-12 19:36:55.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/automated_ai/classification_automated/xgb_automated.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-20 06:12:28.488300 PatryksAutoAI-1.5.3/KaggleAutoAI/automated_ai/regression_automated/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      308 2023-05-12 19:57:48.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/automated_ai/regression_automated/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      840 2023-05-12 21:49:08.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/automated_ai/regression_automated/cat_automated.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      905 2023-05-12 19:55:05.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/automated_ai/regression_automated/gradient_boosting_automated.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      840 2023-05-12 19:55:24.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/automated_ai/regression_automated/lgb_automated.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      840 2023-05-12 19:56:32.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/automated_ai/regression_automated/xgb_automated.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-20 06:12:28.488300 PatryksAutoAI-1.5.3/KaggleAutoAI/classification/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       72 2023-05-10 18:02:22.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/classification/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      648 2023-04-17 06:33:02.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/classification/metrics.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-20 06:12:28.492300 PatryksAutoAI-1.5.3/KaggleAutoAI/classification/models/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      317 2023-05-10 18:02:39.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/classification/models/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     9064 2023-05-18 09:26:27.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/classification/models/cat.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     7070 2023-05-18 13:47:34.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/classification/models/extra_trees.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6724 2023-05-18 13:47:54.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/classification/models/gradient_boosting.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6921 2023-05-18 13:48:13.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/classification/models/hist_gradient.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2400 2023-05-16 13:32:16.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/classification/models/kneighbours.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     8274 2023-05-18 14:23:56.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/classification/models/light_lgb.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2493 2023-05-16 13:32:12.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/classification/models/linear_svc.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     5866 2023-05-18 13:48:54.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/classification/models/logistic_regression.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     7080 2023-05-17 16:29:50.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/classification/models/random_forest.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2512 2023-05-16 13:31:56.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/classification/models/sgd_classifier.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2732 2023-05-17 18:02:36.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/classification/models/svc.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6875 2023-05-18 13:48:34.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/classification/models/xgb.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      920 2023-03-10 12:07:04.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/helper_function.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-20 06:12:28.492300 PatryksAutoAI-1.5.3/KaggleAutoAI/language_processing/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      192 2023-05-14 19:03:52.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/language_processing/__init__.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-20 06:12:28.492300 PatryksAutoAI-1.5.3/KaggleAutoAI/language_processing/data_manipulation/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      115 2023-05-13 17:40:53.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/language_processing/data_manipulation/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      654 2023-05-12 21:36:49.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/language_processing/data_manipulation/metrics.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     5024 2023-05-20 06:12:00.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/language_processing/data_manipulation/text2number.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     4078 2023-05-17 16:36:27.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/language_processing/data_manipulation/text_preprocessing.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-20 06:12:28.492300 PatryksAutoAI-1.5.3/KaggleAutoAI/language_processing/models/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       78 2023-05-16 09:57:09.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/language_processing/models/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     1975 2023-05-16 09:57:20.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/language_processing/models/baseline.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     1759 2023-05-19 09:50:59.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/language_processing/models/transformer_model.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-20 06:12:28.492300 PatryksAutoAI-1.5.3/KaggleAutoAI/model_data/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      110 2023-05-10 18:02:54.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/model_data/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      646 2023-05-16 07:40:06.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/model_data/animated.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6075 2023-04-18 06:00:32.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/model_data/model_data.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-20 06:12:28.492300 PatryksAutoAI-1.5.3/KaggleAutoAI/regression/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       89 2023-05-12 20:27:28.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/regression/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      607 2023-05-09 13:49:56.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/regression/metrics_regression.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-20 06:12:28.492300 PatryksAutoAI-1.5.3/KaggleAutoAI/regression/models/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      216 2023-05-12 20:11:18.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/regression/models/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     7013 2023-05-16 17:25:47.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/regression/models/cat.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2885 2023-05-16 13:17:22.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/regression/models/elastic_net.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6865 2023-05-16 13:17:21.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/regression/models/gradient_boosting.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2807 2023-05-16 13:17:18.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/regression/models/lasso.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6240 2023-05-16 17:26:05.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/regression/models/lgb.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     3095 2023-05-16 13:17:18.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/regression/models/sgd.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2883 2023-05-16 13:17:16.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/regression/models/svr.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     8274 2023-05-16 17:26:31.000000 PatryksAutoAI-1.5.3/KaggleAutoAI/regression/models/xgb.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      538 2023-05-20 06:12:28.496300 PatryksAutoAI-1.5.3/PKG-INFO
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-20 06:12:28.492300 PatryksAutoAI-1.5.3/PatryksAutoAI.egg-info/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      538 2023-05-20 06:12:28.000000 PatryksAutoAI-1.5.3/PatryksAutoAI.egg-info/PKG-INFO
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     3193 2023-05-20 06:12:28.000000 PatryksAutoAI-1.5.3/PatryksAutoAI.egg-info/SOURCES.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)        1 2023-05-20 06:12:28.000000 PatryksAutoAI-1.5.3/PatryksAutoAI.egg-info/dependency_links.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      253 2023-05-20 06:12:28.000000 PatryksAutoAI-1.5.3/PatryksAutoAI.egg-info/requires.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       13 2023-05-20 06:12:28.000000 PatryksAutoAI-1.5.3/PatryksAutoAI.egg-info/top_level.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       38 2023-05-20 06:12:28.496300 PatryksAutoAI-1.5.3/setup.cfg
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     1050 2023-05-20 06:12:22.000000 PatryksAutoAI-1.5.3/setup.py
```

### Comparing `PatryksAutoAI-1.5.2/KaggleAutoAI/automated_ai/algorithms/complexity_level0.py` & `PatryksAutoAI-1.5.3/KaggleAutoAI/automated_ai/algorithms/complexity_level0.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.5.2/KaggleAutoAI/automated_ai/algorithms/complexity_level1.py` & `PatryksAutoAI-1.5.3/KaggleAutoAI/automated_ai/algorithms/complexity_level1.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.5.2/KaggleAutoAI/automated_ai/classification_automated/__init__.py` & `PatryksAutoAI-1.5.3/KaggleAutoAI/automated_ai/classification_automated/__init__.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.5.2/KaggleAutoAI/automated_ai/classification_automated/cat_automated.py` & `PatryksAutoAI-1.5.3/KaggleAutoAI/automated_ai/classification_automated/cat_automated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.5.2/KaggleAutoAI/automated_ai/classification_automated/extra_trees.py` & `PatryksAutoAI-1.5.3/KaggleAutoAI/automated_ai/classification_automated/extra_trees.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.5.2/KaggleAutoAI/automated_ai/classification_automated/gradient_boosting_automated.py` & `PatryksAutoAI-1.5.3/KaggleAutoAI/automated_ai/classification_automated/gradient_boosting_automated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.5.2/KaggleAutoAI/automated_ai/classification_automated/hist_gradient_automated.py` & `PatryksAutoAI-1.5.3/KaggleAutoAI/automated_ai/classification_automated/hist_gradient_automated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.5.2/KaggleAutoAI/automated_ai/classification_automated/lgb_automated.py` & `PatryksAutoAI-1.5.3/KaggleAutoAI/automated_ai/classification_automated/lgb_automated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.5.2/KaggleAutoAI/automated_ai/classification_automated/logistic_regression_automated.py` & `PatryksAutoAI-1.5.3/KaggleAutoAI/automated_ai/classification_automated/logistic_regression_automated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.5.2/KaggleAutoAI/automated_ai/classification_automated/random_forest_automated.py` & `PatryksAutoAI-1.5.3/KaggleAutoAI/automated_ai/classification_automated/random_forest_automated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.5.2/KaggleAutoAI/automated_ai/classification_automated/xgb_automated.py` & `PatryksAutoAI-1.5.3/KaggleAutoAI/automated_ai/classification_automated/xgb_automated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.5.2/KaggleAutoAI/automated_ai/regression_automated/cat_automated.py` & `PatryksAutoAI-1.5.3/KaggleAutoAI/automated_ai/regression_automated/cat_automated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.5.2/KaggleAutoAI/automated_ai/regression_automated/gradient_boosting_automated.py` & `PatryksAutoAI-1.5.3/KaggleAutoAI/automated_ai/regression_automated/gradient_boosting_automated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.5.2/KaggleAutoAI/automated_ai/regression_automated/lgb_automated.py` & `PatryksAutoAI-1.5.3/KaggleAutoAI/automated_ai/regression_automated/lgb_automated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.5.2/KaggleAutoAI/automated_ai/regression_automated/xgb_automated.py` & `PatryksAutoAI-1.5.3/KaggleAutoAI/automated_ai/regression_automated/xgb_automated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.5.2/KaggleAutoAI/classification/metrics.py` & `PatryksAutoAI-1.5.3/KaggleAutoAI/classification/metrics.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.5.2/KaggleAutoAI/classification/models/cat.py` & `PatryksAutoAI-1.5.3/KaggleAutoAI/classification/models/cat.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.5.2/KaggleAutoAI/classification/models/extra_trees.py` & `PatryksAutoAI-1.5.3/KaggleAutoAI/classification/models/extra_trees.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.5.2/KaggleAutoAI/classification/models/gradient_boosting.py` & `PatryksAutoAI-1.5.3/KaggleAutoAI/classification/models/gradient_boosting.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.5.2/KaggleAutoAI/classification/models/hist_gradient.py` & `PatryksAutoAI-1.5.3/KaggleAutoAI/classification/models/hist_gradient.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.5.2/KaggleAutoAI/classification/models/kneighbours.py` & `PatryksAutoAI-1.5.3/KaggleAutoAI/classification/models/kneighbours.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.5.2/KaggleAutoAI/classification/models/light_lgb.py` & `PatryksAutoAI-1.5.3/KaggleAutoAI/classification/models/light_lgb.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.5.2/KaggleAutoAI/classification/models/linear_svc.py` & `PatryksAutoAI-1.5.3/KaggleAutoAI/classification/models/linear_svc.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.5.2/KaggleAutoAI/classification/models/logistic_regression.py` & `PatryksAutoAI-1.5.3/KaggleAutoAI/classification/models/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.5.2/KaggleAutoAI/classification/models/random_forest.py` & `PatryksAutoAI-1.5.3/KaggleAutoAI/classification/models/random_forest.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.5.2/KaggleAutoAI/classification/models/sgd_classifier.py` & `PatryksAutoAI-1.5.3/KaggleAutoAI/classification/models/sgd_classifier.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.5.2/KaggleAutoAI/classification/models/svc.py` & `PatryksAutoAI-1.5.3/KaggleAutoAI/classification/models/svc.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.5.2/KaggleAutoAI/classification/models/xgb.py` & `PatryksAutoAI-1.5.3/KaggleAutoAI/classification/models/xgb.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.5.2/KaggleAutoAI/helper_function.py` & `PatryksAutoAI-1.5.3/KaggleAutoAI/helper_function.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.5.2/KaggleAutoAI/language_processing/data_manipulation/metrics.py` & `PatryksAutoAI-1.5.3/KaggleAutoAI/language_processing/data_manipulation/metrics.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.5.2/KaggleAutoAI/language_processing/data_manipulation/text2number.py` & `PatryksAutoAI-1.5.3/KaggleAutoAI/language_processing/data_manipulation/text2number.py`

 * *Files 25% similar despite different names*

```diff
@@ -81,72 +81,42 @@
                           max_length=seq_len,
                           truncation=True,
                           padding='max_length',
                           add_special_tokens=True,
                           return_attention_mask=True,)
         self.token = token
 
-    def train_val_test(self, data, labels, seq_len=128, train_size=0.8, val_size=0.1):
+    def train_val_test(self, data, labels, seq_len=128):
         '''
             Creates the train and validation datasets
         '''
         train_ds_ids = []
         train_ds_mask = []
         train_label = []
-        val_ds = []
-        val_label = []
-        test_ds = []
-        test_label = []
         labels = np.array(labels.tolist()).reshape(-1,1)
 
-        train_size = int(len(data) * train_size)
-        val_size = int(len(data) * val_size) + train_size
         tokenizer = BertTokenizer.from_pretrained("bert-base-cased")
-
         for i, val in enumerate(data.tolist()):
             val = tokenizer.encode_plus(val,
                           max_length=seq_len,
                           truncation=True,
                           padding='max_length',
                           add_special_tokens=True,
                           return_attention_mask=True,)
-            if i < train_size:
-                train_ds_ids.append(val['input_ids'])
-                train_ds_mask.append(val['attention_mask'])
-                train_label.append(labels[i])
-                continue
-            if i < val_size:
-                val_ds.append([val['input_ids'], val['attention_mask']])
-                val_label.append(labels[i])
-                continue
-            else:
-                test_ds.append([val['input_ids'], val['attention_mask']])
-                test_label.append(labels[i])
+
+            train_ds_ids.append(val['input_ids'])
+            train_ds_mask.append(val['attention_mask'])
+            train_label.append(labels[i])
 
         train_ds_ids = tf.convert_to_tensor(train_ds_ids)
         train_ds_mask = tf.convert_to_tensor(train_ds_mask)
         train_label = tf.convert_to_tensor(train_label)
-        val_ds = tf.convert_to_tensor(val_ds)
-        val_label = tf.convert_to_tensor(val_label)
-        test_ds = tf.convert_to_tensor(test_ds)
-        test_label = tf.convert_to_tensor(test_label)
 
         return train_ds_ids,train_ds_mask, train_label
     
-    def test(self, labels):
-        test_ds = []
-        test_label = []
-        labels = np.array(labels.tolist()).reshape(-1,1)
-
-        for i, val in enumerate(self.token):
-            test_ds.append([val['input_ids'], val['attention_mask']])
-            test_label.append(labels[i])
-
-        return test_ds, test_label
-    
     def map_func_test(self, input_ids, masks):
         return {'input_ids':input_ids,
                 'attention_mask':masks}
     
     def map_func(self, input_ids, masks, labels):
         return {'input_ids':input_ids,
                 'attention_mask':masks}, labels
```

### Comparing `PatryksAutoAI-1.5.2/KaggleAutoAI/language_processing/data_manipulation/text_preprocessing.py` & `PatryksAutoAI-1.5.3/KaggleAutoAI/language_processing/data_manipulation/text_preprocessing.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.5.2/KaggleAutoAI/language_processing/models/baseline.py` & `PatryksAutoAI-1.5.3/KaggleAutoAI/language_processing/models/baseline.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.5.2/KaggleAutoAI/language_processing/models/transformer_model.py` & `PatryksAutoAI-1.5.3/KaggleAutoAI/language_processing/models/transformer_model.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.5.2/KaggleAutoAI/model_data/animated.py` & `PatryksAutoAI-1.5.3/KaggleAutoAI/model_data/animated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.5.2/KaggleAutoAI/model_data/model_data.py` & `PatryksAutoAI-1.5.3/KaggleAutoAI/model_data/model_data.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.5.2/KaggleAutoAI/regression/metrics_regression.py` & `PatryksAutoAI-1.5.3/KaggleAutoAI/regression/metrics_regression.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.5.2/KaggleAutoAI/regression/models/cat.py` & `PatryksAutoAI-1.5.3/KaggleAutoAI/regression/models/cat.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.5.2/KaggleAutoAI/regression/models/elastic_net.py` & `PatryksAutoAI-1.5.3/KaggleAutoAI/regression/models/elastic_net.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.5.2/KaggleAutoAI/regression/models/gradient_boosting.py` & `PatryksAutoAI-1.5.3/KaggleAutoAI/regression/models/gradient_boosting.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.5.2/KaggleAutoAI/regression/models/lasso.py` & `PatryksAutoAI-1.5.3/KaggleAutoAI/regression/models/lasso.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.5.2/KaggleAutoAI/regression/models/lgb.py` & `PatryksAutoAI-1.5.3/KaggleAutoAI/regression/models/lgb.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.5.2/KaggleAutoAI/regression/models/sgd.py` & `PatryksAutoAI-1.5.3/KaggleAutoAI/regression/models/sgd.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.5.2/KaggleAutoAI/regression/models/svr.py` & `PatryksAutoAI-1.5.3/KaggleAutoAI/regression/models/svr.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.5.2/KaggleAutoAI/regression/models/xgb.py` & `PatryksAutoAI-1.5.3/KaggleAutoAI/regression/models/xgb.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.5.2/PKG-INFO` & `PatryksAutoAI-1.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PatryksAutoAI
-Version: 1.5.2
+Version: 1.5.3
 Summary: Auto_AI_patryk
 Author: patryk
 Author-email: lyczkopatryk1@gmail.com
 Keywords: python,machine_learning,auto
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PatryksAutoAI-1.5.2/PatryksAutoAI.egg-info/PKG-INFO` & `PatryksAutoAI-1.5.3/PatryksAutoAI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PatryksAutoAI
-Version: 1.5.2
+Version: 1.5.3
 Summary: Auto_AI_patryk
 Author: patryk
 Author-email: lyczkopatryk1@gmail.com
 Keywords: python,machine_learning,auto
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PatryksAutoAI-1.5.2/PatryksAutoAI.egg-info/SOURCES.txt` & `PatryksAutoAI-1.5.3/PatryksAutoAI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-1.5.2/setup.py` & `PatryksAutoAI-1.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
-VERSION = '1.5.2'
+VERSION = '1.5.3'
 DESCRIPTION = 'Auto_AI_patryk'
 LONG_DESCRIPTION = 'Package contains helping functions for creating ML models'
 
 # Read the requirements from requirements.txt
 with open('./KaggleAutoAI/requirements.txt') as f:
     requirements = f.read().splitlines()
```

