# Comparing `tmp/zeroshot-classifier-0.1.2.tar.gz` & `tmp/zeroshot-classifier-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeroshot-classifier-0.1.2.tar", last modified: Fri May 19 16:38:54 2023, max compression
+gzip compressed data, was "zeroshot-classifier-0.2.0.tar", last modified: Sat May 20 15:05:43 2023, max compression
```

## Comparing `zeroshot-classifier-0.1.2.tar` & `zeroshot-classifier-0.2.0.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2023-05-19 16:38:54.718367 zeroshot-classifier-0.1.2/
--rw-r--r--   0 stefanhg   (501) staff       (20)     1351 2023-05-19 16:38:54.718089 zeroshot-classifier-0.1.2/PKG-INFO
--rw-r--r--   0 stefanhg   (501) staff       (20)    11394 2023-05-18 16:52:25.000000 zeroshot-classifier-0.1.2/README.md
--rw-r--r--   0 stefanhg   (501) staff       (20)       38 2023-05-19 16:38:54.718484 zeroshot-classifier-0.1.2/setup.cfg
--rw-r--r--   0 stefanhg   (501) staff       (20)     1804 2023-05-19 16:38:24.000000 zeroshot-classifier-0.1.2/setup.py
-drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2023-05-19 16:38:54.683194 zeroshot-classifier-0.1.2/zeroshot_classifier/
--rw-r--r--   0 stefanhg   (501) staff       (20)       64 2022-06-08 21:00:21.000000 zeroshot-classifier-0.1.2/zeroshot_classifier/__init__.py
-drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2023-05-19 16:38:54.694438 zeroshot-classifier-0.1.2/zeroshot_classifier/models/
--rw-r--r--   0 stefanhg   (501) staff       (20)      120 2023-05-15 21:19:13.000000 zeroshot-classifier-0.1.2/zeroshot_classifier/models/__init__.py
--rw-r--r--   0 stefanhg   (501) staff       (20)     1648 2023-05-11 21:27:47.000000 zeroshot-classifier-0.1.2/zeroshot_classifier/models/_bert_based_models.py
-drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2023-05-19 16:38:54.697390 zeroshot-classifier-0.1.2/zeroshot_classifier/models/architecture/
--rw-r--r--   0 stefanhg   (501) staff       (20)       21 2023-05-15 21:19:13.000000 zeroshot-classifier-0.1.2/zeroshot_classifier/models/architecture/__init__.py
--rw-r--r--   0 stefanhg   (501) staff       (20)     2037 2023-05-11 21:06:00.000000 zeroshot-classifier-0.1.2/zeroshot_classifier/models/architecture/binary_bert.py
--rw-r--r--   0 stefanhg   (501) staff       (20)    20988 2023-05-15 21:19:13.000000 zeroshot-classifier-0.1.2/zeroshot_classifier/models/architecture/sbert.py
--rw-r--r--   0 stefanhg   (501) staff       (20)     7617 2023-05-11 21:11:58.000000 zeroshot-classifier-0.1.2/zeroshot_classifier/models/bart.py
--rw-r--r--   0 stefanhg   (501) staff       (20)     9481 2023-05-18 16:57:42.000000 zeroshot-classifier-0.1.2/zeroshot_classifier/models/bert.py
--rw-r--r--   0 stefanhg   (501) staff       (20)     6623 2022-10-09 05:20:14.000000 zeroshot-classifier-0.1.2/zeroshot_classifier/models/bert_nli.py
--rw-r--r--   0 stefanhg   (501) staff       (20)     8224 2023-05-15 16:29:41.000000 zeroshot-classifier-0.1.2/zeroshot_classifier/models/bi-encoder.py
--rw-r--r--   0 stefanhg   (501) staff       (20)     9586 2023-05-11 21:33:02.000000 zeroshot-classifier-0.1.2/zeroshot_classifier/models/binary_bert.py
-drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2023-05-19 16:38:54.698847 zeroshot-classifier-0.1.2/zeroshot_classifier/models/dual_bi_encoder/
--rw-r--r--   0 stefanhg   (501) staff       (20)      113 2022-05-17 00:55:33.000000 zeroshot-classifier-0.1.2/zeroshot_classifier/models/dual_bi_encoder/__init__.py
--rw-r--r--   0 stefanhg   (501) staff       (20)    13733 2022-10-11 06:06:43.000000 zeroshot-classifier-0.1.2/zeroshot_classifier/models/dual_bi_encoder/dual_bi_encoder.py
-drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2023-05-19 16:38:54.699447 zeroshot-classifier-0.1.2/zeroshot_classifier/models/dual_bi_encoder/jskit/
--rw-r--r--   0 stefanhg   (501) staff       (20)       23 2022-05-17 00:55:33.000000 zeroshot-classifier-0.1.2/zeroshot_classifier/models/dual_bi_encoder/jskit/__init__.py
-drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2023-05-19 16:38:54.701965 zeroshot-classifier-0.1.2/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/
--rw-r--r--   0 stefanhg   (501) staff       (20)       37 2022-05-17 00:55:33.000000 zeroshot-classifier-0.1.2/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/__init__.py
--rw-r--r--   0 stefanhg   (501) staff       (20)    12593 2022-06-08 19:09:36.000000 zeroshot-classifier-0.1.2/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/bi.py
--rw-r--r--   0 stefanhg   (501) staff       (20)     6981 2022-05-17 00:55:33.000000 zeroshot-classifier-0.1.2/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/poly.py
--rw-r--r--   0 stefanhg   (501) staff       (20)     4920 2022-05-17 00:55:33.000000 zeroshot-classifier-0.1.2/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/sent_enc.py
-drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2023-05-19 16:38:54.704242 zeroshot-classifier-0.1.2/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/tests/
--rw-r--r--   0 stefanhg   (501) staff       (20)        0 2022-06-08 19:09:09.000000 zeroshot-classifier-0.1.2/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/tests/__init__.py
--rw-r--r--   0 stefanhg   (501) staff       (20)     2168 2022-05-17 00:55:33.000000 zeroshot-classifier-0.1.2/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/tests/test_biencoder.py
--rw-r--r--   0 stefanhg   (501) staff       (20)    10637 2022-05-17 00:55:33.000000 zeroshot-classifier-0.1.2/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/tests/test_data.py
-drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2023-05-19 16:38:54.706398 zeroshot-classifier-0.1.2/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/utils/
--rw-r--r--   0 stefanhg   (501) staff       (20)      595 2022-06-08 21:00:21.000000 zeroshot-classifier-0.1.2/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/utils/__init__.py
--rw-r--r--   0 stefanhg   (501) staff       (20)     4392 2022-06-08 19:09:36.000000 zeroshot-classifier-0.1.2/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/utils/evaluate.py
--rw-r--r--   0 stefanhg   (501) staff       (20)    11707 2022-05-17 00:55:33.000000 zeroshot-classifier-0.1.2/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/utils/models.py
--rw-r--r--   0 stefanhg   (501) staff       (20)     8478 2022-06-10 19:38:06.000000 zeroshot-classifier-0.1.2/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/utils/tokenizer.py
--rw-r--r--   0 stefanhg   (501) staff       (20)    10795 2022-10-08 11:44:22.000000 zeroshot-classifier-0.1.2/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/utils/train.py
-drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2023-05-19 16:38:54.708763 zeroshot-classifier-0.1.2/zeroshot_classifier/models/explicit/
--rw-r--r--   0 stefanhg   (501) staff       (20)       27 2022-06-10 19:40:02.000000 zeroshot-classifier-0.1.2/zeroshot_classifier/models/explicit/__init__.py
--rw-r--r--   0 stefanhg   (501) staff       (20)    18865 2023-05-11 21:11:58.000000 zeroshot-classifier-0.1.2/zeroshot_classifier/models/explicit/binary_bert.py
--rw-r--r--   0 stefanhg   (501) staff       (20)     5958 2023-05-11 21:11:58.000000 zeroshot-classifier-0.1.2/zeroshot_classifier/models/explicit/binary_bert_pretrain.py
--rw-r--r--   0 stefanhg   (501) staff       (20)     2467 2023-05-11 21:11:58.000000 zeroshot-classifier-0.1.2/zeroshot_classifier/models/explicit/explicit_v2.py
--rw-r--r--   0 stefanhg   (501) staff       (20)     4529 2023-05-11 21:11:58.000000 zeroshot-classifier-0.1.2/zeroshot_classifier/models/explicit/gpt2_pretrain.py
--rw-r--r--   0 stefanhg   (501) staff       (20)    56056 2023-05-17 16:47:57.000000 zeroshot-classifier-0.1.2/zeroshot_classifier/models/gpt2.py
--rw-r--r--   0 stefanhg   (501) staff       (20)    18487 2023-05-11 21:11:58.000000 zeroshot-classifier-0.1.2/zeroshot_classifier/models/gpt3.py
--rw-r--r--   0 stefanhg   (501) staff       (20)    11200 2022-10-21 11:22:04.000000 zeroshot-classifier-0.1.2/zeroshot_classifier/models/gpt_neo.py
-drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2023-05-19 16:38:54.709856 zeroshot-classifier-0.1.2/zeroshot_classifier/preprocess/
--rw-r--r--   0 stefanhg   (501) staff       (20)       23 2022-06-10 19:40:02.000000 zeroshot-classifier-0.1.2/zeroshot_classifier/preprocess/__init__.py
--rw-r--r--   0 stefanhg   (501) staff       (20)     6510 2023-05-11 21:18:59.000000 zeroshot-classifier-0.1.2/zeroshot_classifier/preprocess/dataset.py
-drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2023-05-19 16:38:54.716213 zeroshot-classifier-0.1.2/zeroshot_classifier/util/
--rw-r--r--   0 stefanhg   (501) staff       (20)      198 2023-05-19 16:28:24.000000 zeroshot-classifier-0.1.2/zeroshot_classifier/util/__init__.py
--rw-r--r--   0 stefanhg   (501) staff       (20)    20678 2023-05-19 16:35:50.000000 zeroshot-classifier-0.1.2/zeroshot_classifier/util/config.py
--rw-r--r--   0 stefanhg   (501) staff       (20)      684 2022-10-08 11:42:19.000000 zeroshot-classifier-0.1.2/zeroshot_classifier/util/data_path.py
--rw-r--r--   0 stefanhg   (501) staff       (20)     6424 2022-11-21 23:48:12.000000 zeroshot-classifier-0.1.2/zeroshot_classifier/util/explicit_v2_pretrain.py
--rw-r--r--   0 stefanhg   (501) staff       (20)    35035 2023-05-11 21:22:23.000000 zeroshot-classifier-0.1.2/zeroshot_classifier/util/gpt2_train.py
--rw-r--r--   0 stefanhg   (501) staff       (20)    27648 2023-05-11 21:22:23.000000 zeroshot-classifier-0.1.2/zeroshot_classifier/util/load_data.py
--rw-r--r--   0 stefanhg   (501) staff       (20)      614 2023-05-11 21:22:32.000000 zeroshot-classifier-0.1.2/zeroshot_classifier/util/training.py
--rw-r--r--   0 stefanhg   (501) staff       (20)    32754 2023-05-11 21:25:05.000000 zeroshot-classifier-0.1.2/zeroshot_classifier/util/utcd.py
--rw-r--r--   0 stefanhg   (501) staff       (20)     6970 2023-05-19 16:31:12.000000 zeroshot-classifier-0.1.2/zeroshot_classifier/util/util.py
-drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2023-05-19 16:38:54.717341 zeroshot-classifier-0.1.2/zeroshot_classifier/visualize/
--rw-r--r--   0 stefanhg   (501) staff       (20)       60 2022-05-17 00:55:33.000000 zeroshot-classifier-0.1.2/zeroshot_classifier/visualize/__init__.py
--rw-r--r--   0 stefanhg   (501) staff       (20)     6868 2022-10-09 11:59:47.000000 zeroshot-classifier-0.1.2/zeroshot_classifier/visualize/visualize_text_sample_loss.py
-drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2023-05-19 16:38:54.685627 zeroshot-classifier-0.1.2/zeroshot_classifier.egg-info/
--rw-r--r--   0 stefanhg   (501) staff       (20)     1351 2023-05-19 16:38:54.000000 zeroshot-classifier-0.1.2/zeroshot_classifier.egg-info/PKG-INFO
--rw-r--r--   0 stefanhg   (501) staff       (20)     2656 2023-05-19 16:38:54.000000 zeroshot-classifier-0.1.2/zeroshot_classifier.egg-info/SOURCES.txt
--rw-r--r--   0 stefanhg   (501) staff       (20)        1 2023-05-19 16:38:54.000000 zeroshot-classifier-0.1.2/zeroshot_classifier.egg-info/dependency_links.txt
--rw-r--r--   0 stefanhg   (501) staff       (20)      203 2023-05-19 16:38:54.000000 zeroshot-classifier-0.1.2/zeroshot_classifier.egg-info/requires.txt
--rw-r--r--   0 stefanhg   (501) staff       (20)       20 2023-05-19 16:38:54.000000 zeroshot-classifier-0.1.2/zeroshot_classifier.egg-info/top_level.txt
+drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2023-05-20 15:05:43.583736 zeroshot-classifier-0.2.0/
+-rw-r--r--   0 stefanhg   (501) staff       (20)     1351 2023-05-20 15:05:43.583473 zeroshot-classifier-0.2.0/PKG-INFO
+-rw-r--r--   0 stefanhg   (501) staff       (20)    11394 2023-05-18 16:52:25.000000 zeroshot-classifier-0.2.0/README.md
+-rw-r--r--   0 stefanhg   (501) staff       (20)       38 2023-05-20 15:05:43.583862 zeroshot-classifier-0.2.0/setup.cfg
+-rw-r--r--   0 stefanhg   (501) staff       (20)     1804 2023-05-20 15:04:54.000000 zeroshot-classifier-0.2.0/setup.py
+drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2023-05-20 15:05:43.553138 zeroshot-classifier-0.2.0/zeroshot_classifier/
+-rw-r--r--   0 stefanhg   (501) staff       (20)       64 2022-06-08 21:00:21.000000 zeroshot-classifier-0.2.0/zeroshot_classifier/__init__.py
+drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2023-05-20 15:05:43.563447 zeroshot-classifier-0.2.0/zeroshot_classifier/models/
+-rw-r--r--   0 stefanhg   (501) staff       (20)       68 2023-05-19 21:40:37.000000 zeroshot-classifier-0.2.0/zeroshot_classifier/models/__init__.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)     1648 2023-05-11 21:27:47.000000 zeroshot-classifier-0.2.0/zeroshot_classifier/models/_bert_based_models.py
+drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2023-05-20 15:05:43.565434 zeroshot-classifier-0.2.0/zeroshot_classifier/models/architecture/
+-rw-r--r--   0 stefanhg   (501) staff       (20)       21 2023-05-15 21:19:13.000000 zeroshot-classifier-0.2.0/zeroshot_classifier/models/architecture/__init__.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)     2037 2023-05-11 21:06:00.000000 zeroshot-classifier-0.2.0/zeroshot_classifier/models/architecture/binary_bert.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)    20988 2023-05-15 21:19:13.000000 zeroshot-classifier-0.2.0/zeroshot_classifier/models/architecture/sbert.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)     7617 2023-05-11 21:11:58.000000 zeroshot-classifier-0.2.0/zeroshot_classifier/models/bart.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)     9481 2023-05-18 16:57:42.000000 zeroshot-classifier-0.2.0/zeroshot_classifier/models/bert.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)     6623 2022-10-09 05:20:14.000000 zeroshot-classifier-0.2.0/zeroshot_classifier/models/bert_nli.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)     8224 2023-05-15 16:29:41.000000 zeroshot-classifier-0.2.0/zeroshot_classifier/models/bi-encoder.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)     9586 2023-05-11 21:33:02.000000 zeroshot-classifier-0.2.0/zeroshot_classifier/models/binary_bert.py
+drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2023-05-20 15:05:43.566639 zeroshot-classifier-0.2.0/zeroshot_classifier/models/dual_bi_encoder/
+-rw-r--r--   0 stefanhg   (501) staff       (20)      113 2022-05-17 00:55:33.000000 zeroshot-classifier-0.2.0/zeroshot_classifier/models/dual_bi_encoder/__init__.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)    13733 2022-10-11 06:06:43.000000 zeroshot-classifier-0.2.0/zeroshot_classifier/models/dual_bi_encoder/dual_bi_encoder.py
+drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2023-05-20 15:05:43.567215 zeroshot-classifier-0.2.0/zeroshot_classifier/models/dual_bi_encoder/jskit/
+-rw-r--r--   0 stefanhg   (501) staff       (20)       23 2022-05-17 00:55:33.000000 zeroshot-classifier-0.2.0/zeroshot_classifier/models/dual_bi_encoder/jskit/__init__.py
+drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2023-05-20 15:05:43.569030 zeroshot-classifier-0.2.0/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/
+-rw-r--r--   0 stefanhg   (501) staff       (20)       37 2022-05-17 00:55:33.000000 zeroshot-classifier-0.2.0/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/__init__.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)    12593 2022-06-08 19:09:36.000000 zeroshot-classifier-0.2.0/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/bi.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)     6981 2022-05-17 00:55:33.000000 zeroshot-classifier-0.2.0/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/poly.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)     4920 2022-05-17 00:55:33.000000 zeroshot-classifier-0.2.0/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/sent_enc.py
+drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2023-05-20 15:05:43.570169 zeroshot-classifier-0.2.0/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/tests/
+-rw-r--r--   0 stefanhg   (501) staff       (20)        0 2022-06-08 19:09:09.000000 zeroshot-classifier-0.2.0/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/tests/__init__.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)     2168 2022-05-17 00:55:33.000000 zeroshot-classifier-0.2.0/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/tests/test_biencoder.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)    10637 2022-05-17 00:55:33.000000 zeroshot-classifier-0.2.0/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/tests/test_data.py
+drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2023-05-20 15:05:43.572115 zeroshot-classifier-0.2.0/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/utils/
+-rw-r--r--   0 stefanhg   (501) staff       (20)      595 2022-06-08 21:00:21.000000 zeroshot-classifier-0.2.0/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/utils/__init__.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)     4392 2022-06-08 19:09:36.000000 zeroshot-classifier-0.2.0/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/utils/evaluate.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)    11707 2022-05-17 00:55:33.000000 zeroshot-classifier-0.2.0/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/utils/models.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)     8478 2022-06-10 19:38:06.000000 zeroshot-classifier-0.2.0/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/utils/tokenizer.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)    10795 2022-10-08 11:44:22.000000 zeroshot-classifier-0.2.0/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/utils/train.py
+drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2023-05-20 15:05:43.574434 zeroshot-classifier-0.2.0/zeroshot_classifier/models/explicit/
+-rw-r--r--   0 stefanhg   (501) staff       (20)       27 2022-06-10 19:40:02.000000 zeroshot-classifier-0.2.0/zeroshot_classifier/models/explicit/__init__.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)    18865 2023-05-11 21:11:58.000000 zeroshot-classifier-0.2.0/zeroshot_classifier/models/explicit/binary_bert.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)     5958 2023-05-11 21:11:58.000000 zeroshot-classifier-0.2.0/zeroshot_classifier/models/explicit/binary_bert_pretrain.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)     2467 2023-05-11 21:11:58.000000 zeroshot-classifier-0.2.0/zeroshot_classifier/models/explicit/explicit_v2.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)     4529 2023-05-11 21:11:58.000000 zeroshot-classifier-0.2.0/zeroshot_classifier/models/explicit/gpt2_pretrain.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)    56056 2023-05-17 16:47:57.000000 zeroshot-classifier-0.2.0/zeroshot_classifier/models/gpt2.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)    18487 2023-05-11 21:11:58.000000 zeroshot-classifier-0.2.0/zeroshot_classifier/models/gpt3.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)    11200 2022-10-21 11:22:04.000000 zeroshot-classifier-0.2.0/zeroshot_classifier/models/gpt_neo.py
+drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2023-05-20 15:05:43.575361 zeroshot-classifier-0.2.0/zeroshot_classifier/preprocess/
+-rw-r--r--   0 stefanhg   (501) staff       (20)       23 2022-06-10 19:40:02.000000 zeroshot-classifier-0.2.0/zeroshot_classifier/preprocess/__init__.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)     6510 2023-05-11 21:18:59.000000 zeroshot-classifier-0.2.0/zeroshot_classifier/preprocess/dataset.py
+drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2023-05-20 15:05:43.581764 zeroshot-classifier-0.2.0/zeroshot_classifier/util/
+-rw-r--r--   0 stefanhg   (501) staff       (20)      198 2023-05-19 16:28:24.000000 zeroshot-classifier-0.2.0/zeroshot_classifier/util/__init__.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)    21893 2023-05-20 04:32:54.000000 zeroshot-classifier-0.2.0/zeroshot_classifier/util/config.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)      684 2022-10-08 11:42:19.000000 zeroshot-classifier-0.2.0/zeroshot_classifier/util/data_path.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)     6424 2022-11-21 23:48:12.000000 zeroshot-classifier-0.2.0/zeroshot_classifier/util/explicit_v2_pretrain.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)    35035 2023-05-11 21:22:23.000000 zeroshot-classifier-0.2.0/zeroshot_classifier/util/gpt2_train.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)    26419 2023-05-20 04:30:33.000000 zeroshot-classifier-0.2.0/zeroshot_classifier/util/load_data.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)      614 2023-05-11 21:22:32.000000 zeroshot-classifier-0.2.0/zeroshot_classifier/util/training.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)    32754 2023-05-11 21:25:05.000000 zeroshot-classifier-0.2.0/zeroshot_classifier/util/utcd.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)     8501 2023-05-20 04:32:57.000000 zeroshot-classifier-0.2.0/zeroshot_classifier/util/util.py
+drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2023-05-20 15:05:43.582770 zeroshot-classifier-0.2.0/zeroshot_classifier/visualize/
+-rw-r--r--   0 stefanhg   (501) staff       (20)       60 2022-05-17 00:55:33.000000 zeroshot-classifier-0.2.0/zeroshot_classifier/visualize/__init__.py
+-rw-r--r--   0 stefanhg   (501) staff       (20)     6868 2022-10-09 11:59:47.000000 zeroshot-classifier-0.2.0/zeroshot_classifier/visualize/visualize_text_sample_loss.py
+drwxr-xr-x   0 stefanhg   (501) staff       (20)        0 2023-05-20 15:05:43.555960 zeroshot-classifier-0.2.0/zeroshot_classifier.egg-info/
+-rw-r--r--   0 stefanhg   (501) staff       (20)     1351 2023-05-20 15:05:43.000000 zeroshot-classifier-0.2.0/zeroshot_classifier.egg-info/PKG-INFO
+-rw-r--r--   0 stefanhg   (501) staff       (20)     2656 2023-05-20 15:05:43.000000 zeroshot-classifier-0.2.0/zeroshot_classifier.egg-info/SOURCES.txt
+-rw-r--r--   0 stefanhg   (501) staff       (20)        1 2023-05-20 15:05:43.000000 zeroshot-classifier-0.2.0/zeroshot_classifier.egg-info/dependency_links.txt
+-rw-r--r--   0 stefanhg   (501) staff       (20)      203 2023-05-20 15:05:43.000000 zeroshot-classifier-0.2.0/zeroshot_classifier.egg-info/requires.txt
+-rw-r--r--   0 stefanhg   (501) staff       (20)       20 2023-05-20 15:05:43.000000 zeroshot-classifier-0.2.0/zeroshot_classifier.egg-info/top_level.txt
```

### Comparing `zeroshot-classifier-0.1.2/PKG-INFO` & `zeroshot-classifier-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: zeroshot-classifier
-Version: 0.1.2
+Version: 0.2.0
 Summary: code and data for the Findings of ACL'23 paper Label Agnostic Pre-training for Zero-shot Text Classification 
 Home-page: https://github.com/ChrisIsKing/zero-shot-text-classification
-Download-URL: https://github.com/ChrisIsKing/zero-shot-text-classification/archive/refs/tags/v0.1.2.tar.gz
+Download-URL: https://github.com/ChrisIsKing/zero-shot-text-classification/archive/refs/tags/v0.2.0.tar.gz
 Author: Christopher Clarke & Yuzhao Heng
 Author-email: csclarke@umich.edu
 License: MIT
 Keywords: python,nlp,machine-learning,deep-learning,text-classification,zero-shot-classification
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: GPU :: NVIDIA CUDA
 Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.6
```

### Comparing `zeroshot-classifier-0.1.2/README.md` & `zeroshot-classifier-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.2/setup.py` & `zeroshot-classifier-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.2'
+VERSION = '0.2.0'
 DESCRIPTION = """
 code and data for the Findings of ACL'23 paper Label Agnostic Pre-training for Zero-shot Text Classification 
 by Christopher Clarke, Yuzhao Heng, Yiping Kang, Krisztian Flautner, Lingjia Tang and Jason Mars
  """
 
 setup(
     name='zeroshot-classifier',
     version=VERSION,
     license='MIT',
     author='Christopher Clarke & Yuzhao Heng',
     author_email='csclarke@umich.edu',
     description=DESCRIPTION,
     long_description=DESCRIPTION,
     url='https://github.com/ChrisIsKing/zero-shot-text-classification',
-    download_url='https://github.com/ChrisIsKing/zero-shot-text-classification/archive/refs/tags/v0.1.2.tar.gz',
+    download_url='https://github.com/ChrisIsKing/zero-shot-text-classification/archive/refs/tags/v0.2.0.tar.gz',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'gdown==4.5.4', 'openai==0.25.0', 'requests==2.28.1', 'tenacity==8.1.0',
         'spacy==3.2.2', 'nltk==3.7', 'scikit-learn==1.1.3',
         'torch==1.12.0', 'sentence-transformers==2.2.0', 'transformers==4.16.2',
         'datasets==1.18.3',
```

### Comparing `zeroshot-classifier-0.1.2/zeroshot_classifier/models/_bert_based_models.py` & `zeroshot-classifier-0.2.0/zeroshot_classifier/models/_bert_based_models.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.2/zeroshot_classifier/models/architecture/binary_bert.py` & `zeroshot-classifier-0.2.0/zeroshot_classifier/models/architecture/binary_bert.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.2/zeroshot_classifier/models/architecture/sbert.py` & `zeroshot-classifier-0.2.0/zeroshot_classifier/models/architecture/sbert.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.2/zeroshot_classifier/models/bart.py` & `zeroshot-classifier-0.2.0/zeroshot_classifier/models/bart.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.2/zeroshot_classifier/models/bert.py` & `zeroshot-classifier-0.2.0/zeroshot_classifier/models/bert.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.2/zeroshot_classifier/models/bert_nli.py` & `zeroshot-classifier-0.2.0/zeroshot_classifier/models/bert_nli.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.2/zeroshot_classifier/models/bi-encoder.py` & `zeroshot-classifier-0.2.0/zeroshot_classifier/models/bi-encoder.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.2/zeroshot_classifier/models/binary_bert.py` & `zeroshot-classifier-0.2.0/zeroshot_classifier/models/binary_bert.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.2/zeroshot_classifier/models/dual_bi_encoder/dual_bi_encoder.py` & `zeroshot-classifier-0.2.0/zeroshot_classifier/models/dual_bi_encoder/dual_bi_encoder.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.2/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/bi.py` & `zeroshot-classifier-0.2.0/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/bi.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.2/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/poly.py` & `zeroshot-classifier-0.2.0/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/poly.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.2/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/sent_enc.py` & `zeroshot-classifier-0.2.0/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/sent_enc.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.2/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/tests/test_biencoder.py` & `zeroshot-classifier-0.2.0/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/tests/test_biencoder.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.2/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/tests/test_data.py` & `zeroshot-classifier-0.2.0/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.2/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/utils/__init__.py` & `zeroshot-classifier-0.2.0/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.2/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/utils/evaluate.py` & `zeroshot-classifier-0.2.0/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/utils/evaluate.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.2/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/utils/models.py` & `zeroshot-classifier-0.2.0/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/utils/models.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.2/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/utils/tokenizer.py` & `zeroshot-classifier-0.2.0/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/utils/tokenizer.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.2/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/utils/train.py` & `zeroshot-classifier-0.2.0/zeroshot_classifier/models/dual_bi_encoder/jskit/encoders/utils/train.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.2/zeroshot_classifier/models/explicit/binary_bert.py` & `zeroshot-classifier-0.2.0/zeroshot_classifier/models/explicit/binary_bert.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.2/zeroshot_classifier/models/explicit/binary_bert_pretrain.py` & `zeroshot-classifier-0.2.0/zeroshot_classifier/models/explicit/binary_bert_pretrain.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.2/zeroshot_classifier/models/explicit/explicit_v2.py` & `zeroshot-classifier-0.2.0/zeroshot_classifier/models/explicit/explicit_v2.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.2/zeroshot_classifier/models/explicit/gpt2_pretrain.py` & `zeroshot-classifier-0.2.0/zeroshot_classifier/models/explicit/gpt2_pretrain.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.2/zeroshot_classifier/models/gpt2.py` & `zeroshot-classifier-0.2.0/zeroshot_classifier/models/gpt2.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.2/zeroshot_classifier/models/gpt3.py` & `zeroshot-classifier-0.2.0/zeroshot_classifier/models/gpt3.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.2/zeroshot_classifier/models/gpt_neo.py` & `zeroshot-classifier-0.2.0/zeroshot_classifier/models/gpt_neo.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.2/zeroshot_classifier/preprocess/dataset.py` & `zeroshot-classifier-0.2.0/zeroshot_classifier/preprocess/dataset.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.2/zeroshot_classifier/util/config.py` & `zeroshot-classifier-0.2.0/zeroshot_classifier/util/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,242 +1,32 @@
+import os.path
 import re
 import math
 import json
 import itertools
 from os.path import join as os_join
-from typing import List, Tuple, Dict, Callable, Union
+from typing import List, Tuple, Dict, Callable, Union, Optional, Any
 from collections import Counter
 
 import numpy as np
 import pandas as pd
 from scipy.stats import norm
 from transformers import AutoTokenizer
 import matplotlib.pyplot as plt
 import seaborn as sns
 from tqdm import tqdm
 
 from stefutil import *
-from zeroshot_classifier.util.util import save_fig
-from zeroshot_classifier.util.data_path import BASE_PATH, PROJ_DIR, DSET_DIR
+from zeroshot_classifier.util.data_path import *
 
 
-STSb = 'stsb_multi_mt'  # Per Hugging Face
-config_dict = {
-    'fine-tune': dict(
-        eg_sbert=dict(  # Per *Sentence-BERT: Sentence Embeddings using Siamese BERT-Networks*, section 4.2
-            dataset_name=STSb,
-            embedding_model_name='bert-base-uncased',
-            max_seq_length=256,
-            batch_size=16,
-            n_epochs=4,
-            n_eval=100,  # Total number of evaluations during training
-            warmup_frac=0.1,
-            pooling_model_kwargs=dict(pooling_mode_mean_tokens=True)
-        )
-    ),
-    'datasets': {
-        STSb: dict(
-            n_sample=dict(
-                train=5749,
-                dev=1500,
-                test=1379
-            ),
-            label_range=dict(
-                min=0,
-                max=5
-            )
-        )
-    },
-    'baselines': {
-        'gpt2-nvidia': {
-            'templates': [
-                'To which category does the following document belong? : {}',
-                'To which category does the following text belong? : {}',
-                'To which category does the text belong? : {}',
-                'To which category does the article belong? : {}',
-                'How would you describe the following document? : as {}',
-                'How would you describe the text? : as {}',
-                'How would you describe the following text? : as {}',
-                'Which best describes the text? : {}',
-                'Which best describes the document? : {}',
-                'Which best describes the following document? : {}',
-                'Which best describes the following text? : {}',
-                'The following document is _ ? : {}',
-                'The following text is _ ? : {}',
-                'The text is _ ? : {}',
-                'The document is _ ? : {}',
-                'How is the text best described? : {}',
-                'How is the document best described? : {}',
-                'How is the following text best described? : {}',
-                'How is the following document best described? : {}',
-                'Which of these choices best describes the text? : {}',
-                'Which of these options best describes the text? : {}',
-                'Which of these choices best describes the document? : {}',
-                'Which of these options best describes the document? : {}',
-                'Which of these categories best describes the following document? : {}',
-                'Which of these choices best describes the following document? : {}',
-                'Which of these options best describes the following text? : {}'
-            ],
-            'label-descriptors': dict(  # string label to natural language descriptor, as in paper
-                ag_news={
-                    'World': 'World News',
-                    'Sports': 'Sports',
-                    'Business': 'Business',
-                    'Sci/Tech': 'Science & Technology'
-                }
-            )
-        },
-        'bert-mnli': dict(
-            templates=dict(
-                sentiment='This text expresses a {} sentiment',
-                intent='This text expresses the intent of {}',
-                topic='This text belongs to the topic of {}'
-            )
-        ),
-    },
-    'UTCD': dict(
-        datasets=dict(
-            # in-domain evaluation has the same labels as training
-            go_emotion=dict(
-                path='UTCD/in-domain/go_emotion', aspect='sentiment', eval_labels_same=True, domain='in',
-                name='GoEmotions', name_compact='GoEmotions'
-            ),
-            sentiment_tweets_2020=dict(
-                path='UTCD/in-domain/sentiment_tweets_2020', aspect='sentiment', eval_labels_same=True, domain='in',
-                name='TweetEval', name_compact='TweetEval'
-            ),
-            emotion=dict(
-                path='UTCD/in-domain/emotion', aspect='sentiment', eval_labels_same=True, domain='in',
-                name='Emotion', name_compact='Emotion'
-            ),
-            # not `eval_labels_same` := has some unique test labels
-            sgd=dict(
-                path='UTCD/in-domain/sgd', aspect='intent', eval_labels_same=False, domain='in',
-                name='Schema-Guided Dialogue', name_compact='SGD'
-            ),
-            clinc_150=dict(
-                path='UTCD/in-domain/clinc_150', aspect='intent', eval_labels_same=True, domain='in',
-                name='Clinc-150', name_compact='Clinc-150'
-            ),
-            slurp=dict(
-                path='UTCD/in-domain/slurp', aspect='intent', eval_labels_same=False, domain='in',
-                name='SLURP', name_compact='SLURP'
-            ),
-            ag_news=dict(
-                path='UTCD/in-domain/ag_news', aspect='topic', eval_labels_same=True, domain='in',
-                name='AG News', name_compact='AG News'
-            ),
-            dbpedia=dict(
-                path='UTCD/in-domain/dbpedia', aspect='topic', eval_labels_same=True, domain='in',
-                name='DBpedia', name_compact='DBpedia'
-            ),
-            yahoo=dict(
-                path='UTCD/in-domain/yahoo', aspect='topic', eval_labels_same=True, domain='in',
-                name='Yahoo Answer Topics', name_compact='Yahoo'
-            ),
-            # Out-of-domain datasets: only test split used & intended for evaluation
-            amazon_polarity=dict(
-                path='UTCD/out-of-domain/amazon_polarity', aspect='sentiment', eval_labels_same=True, domain='out',
-                name='Amazon Review Polarity', name_compact='Amazon Polarity'
-            ),
-            finance_sentiment=dict(
-                path='UTCD/out-of-domain/finance_sentiment', aspect='sentiment', eval_labels_same=True, domain='out',
-                name='Financial Phrase Bank', name_compact='Fin. Phrase Bank'
-            ),
-            yelp=dict(
-                path='UTCD/out-of-domain/yelp', aspect='sentiment', eval_labels_same=True, domain='out',
-                name='Yelp Review', name_compact='Yelp'
-            ),
-            banking77=dict(
-                path='UTCD/out-of-domain/banking77', aspect='intent', eval_labels_same=True, domain='out',
-                name='Banking77', name_compact='Banking77'
-            ),
-            snips=dict(
-                path='UTCD/out-of-domain/snips', aspect='intent', eval_labels_same=True, domain='out',
-                name='SNIPS', name_compact='SNIPS'
-            ),
-            nlu_evaluation=dict(
-                path='UTCD/out-of-domain/nlu_evaluation', aspect='intent', eval_labels_same=True, domain='out',
-                name='NLU Evaluation', name_compact='NLU Eval'
-            ),
-            # Removed for too many options, blowing up GPT2's 1024 token length
-            # arxiv=dict(path='UTCD/out-of-domain/arxiv', aspect='topic', eval_labels_same=True, domain='out'),
-            multi_eurlex=dict(
-                path='UTCD/out-of-domain/multi_eurlex', aspect='topic', eval_labels_same=True, domain='out',
-                name='MultiEURLEX', name_compact='MultiEURLEX'
-            ),
-            patent=dict(
-                path='UTCD/out-of-domain/patent', aspect='topic', eval_labels_same=True, domain='out',
-                name='Big Patent', name_compact='Patent'
-            ),
-            consumer_finance=dict(
-                path='UTCD/out-of-domain/consumer_finance', aspect='topic', eval_labels_same=True, domain='out',
-                name='Consumer Finance Complaints', name_compact='Consumer Finance'
-            )
-        ),
-        aspects=['sentiment', 'intent', 'topic'],
-        domains=['in', 'out'],
-        num_aspect=3,
-        num_dataset_per_aspect=6,
-        num_dataset_per_domain_per_aspect=3,
-        num_domain=2,
-        num_dataset_per_domain=9,
-        dataset_ext='json'  # all in json
-    ),
-    'training': {
-        'implicit-on-text': {
-            'encode-aspect': {
-                'aspect2aspect-token': dict(sentiment='<|sentiment|>', intent='<|intent|>', topic='<|topic|>')
-            },
-            'encode-sep': {'aspect-sep-token': '<|ASPECT-SEP|>'}
-        },
-        'strategies': [
-            'vanilla',
-            'implicit',  # prepend aspect text before each label
-            'implicit-on-text-encode-aspect',  # encode each of the 3 aspects as 3 special tokens, followed by text
-            'implicit-on-text-encode-sep',  # encode aspects normally, but add special token between aspect and text
-            'explicit'  # see `zeroshot_classifier.explicit.binary_bert.py` for explicit training
-        ]
-    },
-    'random-seed': 77,
-    'check-arg': [
-        dict(
-            display_name='Model Name', attr_name='model_name',
-            accepted_values=[
-                'bert-seq-cls',  # not a Zeroshot framework, a supervised learning upperbound
-                'binary-bert', 'bert-nli', 'bi-encoder', 'dual-bi-encoder', 'gpt2-nvidia'
-            ]
-        ),
-        dict(
-            display_name='Dataset Domain', attr_name='dataset_domain',
-            accepted_values=['in', 'out']
-        ),
-        dict(
-            display_name='Sampling Strategy', attr_name='sampling_strategy',
-            accepted_values=['rand', 'vect', 'none', 'NA']
-        ),
-        dict(
-            display_name='Training strategy', attr_name='training_strategy',
-            accepted_values=[
-                'vanilla',
-                'implicit',
-                'implicit-on-text-encode-aspect',
-                'implicit-on-text-encode-sep',
-                'explicit'
-            ]
-        ),
-        dict(
-            display_name='GPT2 Training Strategy', attr_name='gpt2_training_strategy',
-            accepted_values=['vanilla', 'implicit', 'explicit']
-        )
-    ]
-}
+__all__ = ['ConfigDict']
 
-path_dset = os_join(BASE_PATH, PROJ_DIR, DSET_DIR)
-ext = config_dict['UTCD']['dataset_ext']
+
+tokenize_modes = ['re', 'bert', 'gpt2']
 
 
 def _re_call() -> Callable[[str], int]:
     if not hasattr(_re_call, 'token_pattern'):
         # taken from sklearn.CountVectorizer
         _re_call.token_pattern = re.compile(r'(?u)\b\w+\b')
     return lambda x: len(_re_call.token_pattern.findall(x))
@@ -265,117 +55,326 @@
             re=_re_call(),
             bert=_hf_call('bert-base-cased'),
             gpt2=_hf_call('gpt2')
         )
     return get_tokenizer_len.d_f[mode](s)
 
 
-tokenize_modes = ['re', 'bert', 'gpt2']
+class ConfigDict:
+    d = {
+        'baselines': {
+            'gpt2-nvidia': {
+                'templates': [
+                    'To which category does the following document belong? : {}',
+                    'To which category does the following text belong? : {}',
+                    'To which category does the text belong? : {}',
+                    'To which category does the article belong? : {}',
+                    'How would you describe the following document? : as {}',
+                    'How would you describe the text? : as {}',
+                    'How would you describe the following text? : as {}',
+                    'Which best describes the text? : {}',
+                    'Which best describes the document? : {}',
+                    'Which best describes the following document? : {}',
+                    'Which best describes the following text? : {}',
+                    'The following document is _ ? : {}',
+                    'The following text is _ ? : {}',
+                    'The text is _ ? : {}',
+                    'The document is _ ? : {}',
+                    'How is the text best described? : {}',
+                    'How is the document best described? : {}',
+                    'How is the following text best described? : {}',
+                    'How is the following document best described? : {}',
+                    'Which of these choices best describes the text? : {}',
+                    'Which of these options best describes the text? : {}',
+                    'Which of these choices best describes the document? : {}',
+                    'Which of these options best describes the document? : {}',
+                    'Which of these categories best describes the following document? : {}',
+                    'Which of these choices best describes the following document? : {}',
+                    'Which of these options best describes the following text? : {}'
+                ],
+                'label-descriptors': dict(  # string label to natural language descriptor, as in paper
+                    ag_news={
+                        'World': 'World News',
+                        'Sports': 'Sports',
+                        'Business': 'Business',
+                        'Sci/Tech': 'Science & Technology'
+                    }
+                )
+            },
+            'bert-mnli': dict(
+                templates=dict(
+                    sentiment='This text expresses a {} sentiment',
+                    intent='This text expresses the intent of {}',
+                    topic='This text belongs to the topic of {}'
+                )
+            ),
+        },
+        'UTCD': dict(
+            datasets=dict(
+                # in-domain evaluation has the same labels as training
+                go_emotion=dict(
+                    path='in-domain/go_emotion', aspect='sentiment', eval_labels_same=True, domain='in',
+                    name='GoEmotions', name_compact='GoEmotions'
+                ),
+                sentiment_tweets_2020=dict(
+                    path='in-domain/sentiment_tweets_2020', aspect='sentiment', eval_labels_same=True, domain='in',
+                    name='TweetEval', name_compact='TweetEval'
+                ),
+                emotion=dict(
+                    path='in-domain/emotion', aspect='sentiment', eval_labels_same=True, domain='in',
+                    name='Emotion', name_compact='Emotion'
+                ),
+                # not `eval_labels_same` := has some unique test labels
+                sgd=dict(
+                    path='in-domain/sgd', aspect='intent', eval_labels_same=False, domain='in',
+                    name='Schema-Guided Dialogue', name_compact='SGD'
+                ),
+                clinc_150=dict(
+                    path='in-domain/clinc_150', aspect='intent', eval_labels_same=True, domain='in',
+                    name='Clinc-150', name_compact='Clinc-150'
+                ),
+                slurp=dict(
+                    path='in-domain/slurp', aspect='intent', eval_labels_same=False, domain='in',
+                    name='SLURP', name_compact='SLURP'
+                ),
+                ag_news=dict(
+                    path='in-domain/ag_news', aspect='topic', eval_labels_same=True, domain='in',
+                    name='AG News', name_compact='AG News'
+                ),
+                dbpedia=dict(
+                    path='in-domain/dbpedia', aspect='topic', eval_labels_same=True, domain='in',
+                    name='DBpedia', name_compact='DBpedia'
+                ),
+                yahoo=dict(
+                    path='in-domain/yahoo', aspect='topic', eval_labels_same=True, domain='in',
+                    name='Yahoo Answer Topics', name_compact='Yahoo'
+                ),
+                # Out-of-domain datasets: only test split used & intended for evaluation
+                amazon_polarity=dict(
+                    path='out-of-domain/amazon_polarity', aspect='sentiment', eval_labels_same=True, domain='out',
+                    name='Amazon Review Polarity', name_compact='Amazon Polarity'
+                ),
+                finance_sentiment=dict(
+                    path='out-of-domain/finance_sentiment', aspect='sentiment', eval_labels_same=True,
+                    domain='out',
+                    name='Financial Phrase Bank', name_compact='Fin. Phrase Bank'
+                ),
+                yelp=dict(
+                    path='out-of-domain/yelp', aspect='sentiment', eval_labels_same=True, domain='out',
+                    name='Yelp Review', name_compact='Yelp'
+                ),
+                banking77=dict(
+                    path='out-of-domain/banking77', aspect='intent', eval_labels_same=True, domain='out',
+                    name='Banking77', name_compact='Banking77'
+                ),
+                snips=dict(
+                    path='out-of-domain/snips', aspect='intent', eval_labels_same=True, domain='out',
+                    name='SNIPS', name_compact='SNIPS'
+                ),
+                nlu_evaluation=dict(
+                    path='out-of-domain/nlu_evaluation', aspect='intent', eval_labels_same=True, domain='out',
+                    name='NLU Evaluation', name_compact='NLU Eval'
+                ),
+                multi_eurlex=dict(
+                    path='out-of-domain/multi_eurlex', aspect='topic', eval_labels_same=True, domain='out',
+                    name='MultiEURLEX', name_compact='MultiEURLEX'
+                ),
+                patent=dict(
+                    path='out-of-domain/patent', aspect='topic', eval_labels_same=True, domain='out',
+                    name='Big Patent', name_compact='Patent'
+                ),
+                consumer_finance=dict(
+                    path='out-of-domain/consumer_finance', aspect='topic', eval_labels_same=True, domain='out',
+                    name='Consumer Finance Complaints', name_compact='Consumer Finance'
+                )
+            ),
+            aspects=['sentiment', 'intent', 'topic'],
+            domains=['in', 'out'],
+            num_aspect=3,
+            num_dataset_per_aspect=6,
+            num_dataset_per_domain_per_aspect=3,
+            num_domain=2,
+            num_dataset_per_domain=9,
+            dataset_ext='json'  # all in json
+        ),
+        'training': {
+            'implicit-on-text': {
+                'encode-aspect': {
+                    'aspect2aspect-token': dict(sentiment='<|sentiment|>', intent='<|intent|>', topic='<|topic|>')
+                },
+                'encode-sep': {'aspect-sep-token': '<|ASPECT-SEP|>'}
+            },
+            'strategies': [
+                'vanilla',
+                'implicit',  # prepend aspect text before each label
+                'implicit-on-text-encode-aspect',  # encode each of the 3 aspects as 3 special tokens, followed by text
+                'implicit-on-text-encode-sep',  # encode aspects normally, but add special token between aspect and text
+                'explicit'  # see `zeroshot_classifier.explicit.binary_bert.py` for explicit training
+            ]
+        },
+        'random-seed': 77,
+        'check-arg': [
+            dict(
+                display_name='Model Name', attr_name='model_name',
+                accepted_values=[
+                    'bert-seq-cls',  # not a Zeroshot framework, a supervised learning upperbound
+                    'binary-bert', 'bert-nli', 'bi-encoder', 'dual-bi-encoder', 'gpt2-nvidia'
+                ]
+            ),
+            dict(
+                display_name='Dataset Domain', attr_name='dataset_domain',
+                accepted_values=['in', 'out']
+            ),
+            dict(
+                display_name='Sampling Strategy', attr_name='sampling_strategy',
+                accepted_values=['rand', 'vect', 'none', 'NA']
+            ),
+            dict(
+                display_name='Training strategy', attr_name='training_strategy',
+                accepted_values=[
+                    'vanilla',
+                    'implicit',
+                    'implicit-on-text-encode-aspect',
+                    'implicit-on-text-encode-sep',
+                    'explicit'
+                ]
+            ),
+            dict(
+                display_name='GPT2 Training Strategy', attr_name='gpt2_training_strategy',
+                accepted_values=['vanilla', 'implicit', 'explicit']
+            )
+        ]
+    }
 
+    def __init__(self, fast: bool = False):
+        """
+        :param fast: If true, token length statistics on all datasets will not be computed
+            Intended for fast loading
+        """
+        self.fast = fast
+        self.d = ConfigDict.d  # TODO: just use the same dict
 
-def path2dataset_info(d: Dict) -> Tuple[Dict, Dict, Dict]:
-    """
-    :return: 3-tuple of (
-        dataset label information per split for `config`,
-        dataset token information per dataset for `config`,
-        number of tokens for plot
-    )
-    """
-    path = os_join(path_dset, f'{d["path"]}.{ext}')
-    with open(path) as fl:
-        dsets: Dict = json.load(fl)
-
-    def split2info(split, dset: Dict[str, List[str]], count_token_length: bool = True) -> Dict:
-        # Based on heuristics on how the `json` are stored
-        # creating a list of all the strings consume memory for prohibitively large datasets
-        n_text_, n_pair_ = len(dset.keys()), sum([len(lbs) for lbs in dset.values()])
-        lbs_uniq = set().union(*dset.values())
-        n_multi_label = sum([len(lbs_) > 1 for lbs_ in dset.values()])
-        txt_n_toks, lb_n_toks = None, None
-        if count_token_length:
-            txt_n_toks, lb_n_toks = dict(), dict()
-            for mode in tokenize_modes:
-                n, desc_t, desc_l = 16, f'{split}-{mode}-text', f'{split}-{mode}-label'
-                lb2tokenize_len = {lb: get_tokenizer_len(lb, mode) for lb in lbs_uniq}
-
-                counter_txt, counter_lb = Counter(), Counter()
-                if mode == 're':
-                    for t in tqdm(dset.keys(), total=len(dset), desc=f'{desc_t:>{n}}'):
-                        counter_txt[get_tokenizer_len(t, mode)] += 1
-                else:
-                    batch_size = 2048*2
-                    for grp in tqdm(
-                            group_n(dset.keys(), batch_size),
-                            total=math.ceil(len(dset) / batch_size), desc=f'{desc_t:>{n}}'
-                    ):
-                        lens: List[int] = get_tokenizer_len(list(grp), mode)
-                        counter_txt.update(lens)
-                for t in tqdm(dset.values(), desc=f'{desc_l:>{n}}'):
-                    for lb in t:
-                        counter_lb[lb2tokenize_len[lb]] += 1
-                txt_n_toks[mode], lb_n_toks[mode] = counter_txt, counter_lb
-        return dict(
-            labels=sorted(lbs_uniq),
-            n_label=len(lbs_uniq),
-            n_text=n_text_,
-            n_pair=n_pair_,
-            multi_label=n_text_ < n_pair_,
-            n_multi_label=n_multi_label,
-            txt_n_toks=txt_n_toks,
-            lb_n_toks=lb_n_toks
+        self.d_n_toks = self.extract_utcd_meta()  # Mutates config_dict
+
+    def _path2dataset_info(self, d: Dict) -> Optional[Tuple[Dict, Dict, Dict]]:
+        """
+        :return: 3-tuple of (
+            dataset label information per split for `config`,
+            dataset token information per dataset for `config`,
+            number of tokens for plot
         )
-    labels, aspect = dsets.pop('labels'), dsets.pop('aspect')
-    assert aspect == d['aspect']
-    d_out = {  # ignore out of domain train split for potentially too large
-        split: split2info(split, dset, count_token_length=not (split == 'train' and d['domain'] == 'out'))
-        for split, dset in dsets.items()
-    }  # Labels for each split
-    assert all(split in ['train', 'test'] for split in d_out.keys())
-    # sum over all splits of the dataset for token length computation
-    txt_n_toks_all = [d_out.pop('txt_n_toks') for d_out in d_out.values()]
-    lb_n_toks_all = [d_out.pop('lb_n_toks') for d_out in d_out.values()]
-    txt_n_toks_all = [e for e in txt_n_toks_all if e]  # pop from the dict, then remove them for stats
-    lb_n_toks_all = [e for e in lb_n_toks_all if e]
-    txt_n_toks_all = {mode: sum([c[mode] for c in txt_n_toks_all], start=Counter()) for mode in tokenize_modes}
-    lb_n_toks_all = {mode: sum([c[mode] for c in lb_n_toks_all], start=Counter()) for mode in tokenize_modes}
-
-    def counter2mean(c: Counter) -> float:
-        lens, counts = zip(*c.items())
-        return np.average(lens, weights=counts)
-    avg_toks = {
-        **{f'{mode}-txt_avg_tokens': counter2mean(txt_n_toks_all[mode]) for mode in tokenize_modes},
-        **{f'{mode}-lb_avg_tokens': counter2mean(lb_n_toks_all[mode]) for mode in tokenize_modes}
-    }
-    assert set(labels) == set().union(*[set(d['labels']) for d in d_out.values()])
-    if d['eval_labels_same']:
-        assert d_out['train']['labels'] == d_out['test']['labels']
-    return d_out, avg_toks, dict(text=txt_n_toks_all, label=lb_n_toks_all)
-
-
-def extract_utcd_meta() -> Dict:
-    d_dsets: Dict = config_dict['UTCD']['datasets']
-    logger = get_logger('Process UTCD')
-    d_n_toks = dict()
-    for dnm, d_dset in d_dsets.items():
-        logger.info(f'Processing {pl.i(dnm)}... ')
-        d_meta, d_avg_tok, d_n_toks[dnm] = path2dataset_info(d_dset)
-        d_dset['splits'] = d_meta
-        d_dset.update(d_avg_tok)
-    dnms = sorted(d_dsets)  # All datasets, in- and out-of-domain, share the same dataset <=> id mapping
-    config_dict['UTCD']['dataset_id2name'] = dnms
-    config_dict['UTCD']['dataset_name2id'] = {dnm: i for i, dnm in enumerate(dnms)}
-    return d_n_toks
+        """
+        path = os_join(BASE_PATH, PROJ_DIR, DSET_DIR, f'{d["path"]}.json')
+        assert os.path.exists(path)  # datasets must be present to extract config metadata
+        with open(path) as fl:
+            dsets: Dict = json.load(fl)
+
+        def split2info(split, dset: Dict[str, List[str]], count_token_length: bool = True) -> Dict:
+            # Based on heuristics on how the `json` are stored
+            # creating a list of all the strings consume memory for prohibitively large datasets
+            n_text_, n_pair_ = len(dset.keys()), sum([len(lbs) for lbs in dset.values()])
+            lbs_uniq = set().union(*dset.values())
+            n_multi_label = sum([len(lbs_) > 1 for lbs_ in dset.values()])
+            txt_n_toks, lb_n_toks = None, None
+            count_len = not self.fast and count_token_length
+            if count_len:
+                txt_n_toks, lb_n_toks = dict(), dict()
+                for mode in tokenize_modes:
+                    n, desc_t, desc_l = 16, f'{split}-{mode}-text', f'{split}-{mode}-label'
+                    lb2tokenize_len = {lb: get_tokenizer_len(lb, mode) for lb in lbs_uniq}
+
+                    counter_txt, counter_lb = Counter(), Counter()
+                    if mode == 're':
+                        for t in tqdm(dset.keys(), total=len(dset), desc=f'{desc_t:>{n}}'):
+                            counter_txt[get_tokenizer_len(t, mode)] += 1
+                    else:
+                        batch_size = 2048*2
+                        for grp in tqdm(
+                                group_n(dset.keys(), batch_size),
+                                total=math.ceil(len(dset) / batch_size), desc=f'{desc_t:>{n}}'
+                        ):
+                            lens: List[int] = get_tokenizer_len(list(grp), mode)
+                            counter_txt.update(lens)
+                    for t in tqdm(dset.values(), desc=f'{desc_l:>{n}}'):
+                        for lb in t:
+                            counter_lb[lb2tokenize_len[lb]] += 1
+                    txt_n_toks[mode], lb_n_toks[mode] = counter_txt, counter_lb
+            ret: Dict[str, Any] = dict(
+                labels=sorted(lbs_uniq),
+                n_label=len(lbs_uniq),
+                n_text=n_text_,
+                n_pair=n_pair_,
+                multi_label=n_text_ < n_pair_,
+                n_multi_label=n_multi_label
+            )
+            if count_len:
+                ret.update(dict(txt_n_toks=txt_n_toks, lb_n_toks=lb_n_toks))
+            return ret
+        labels, aspect = dsets.pop('labels'), dsets.pop('aspect')
+        assert aspect == d['aspect']
+        d_out = {  # ignore out of domain train split for potentially too large
+            split: split2info(split, dset, count_token_length=not (split == 'train' and d['domain'] == 'out'))
+            for split, dset in dsets.items()
+        }  # Labels for each split
+        assert all(split in ['train', 'test'] for split in d_out.keys())
+        assert set(labels) == set().union(*[set(d['labels']) for d in d_out.values()])
+
+        if not self.fast:
+            # sum over all splits of the dataset for token length computation
+            txt_n_toks_all = [d_out.pop('txt_n_toks') for d_out in d_out.values()]
+            lb_n_toks_all = [d_out.pop('lb_n_toks') for d_out in d_out.values()]
+            txt_n_toks_all = [e for e in txt_n_toks_all if e]  # pop from the dict, then remove them for stats
+            lb_n_toks_all = [e for e in lb_n_toks_all if e]
+            txt_n_toks_all = {mode: sum([c[mode] for c in txt_n_toks_all], start=Counter()) for mode in tokenize_modes}
+            lb_n_toks_all = {mode: sum([c[mode] for c in lb_n_toks_all], start=Counter()) for mode in tokenize_modes}
+
+            def counter2mean(c: Counter) -> float:
+                lens, counts = zip(*c.items())
+                return np.average(lens, weights=counts)
+            avg_toks = {
+                **{f'{mode}-txt_avg_tokens': counter2mean(txt_n_toks_all[mode]) for mode in tokenize_modes},
+                **{f'{mode}-lb_avg_tokens': counter2mean(lb_n_toks_all[mode]) for mode in tokenize_modes}
+            }
+            d_n_tok = dict(text=txt_n_toks_all, label=lb_n_toks_all)
+        else:
+            avg_toks, d_n_tok = None, None
+
+        if d['eval_labels_same']:
+            assert d_out['train']['labels'] == d_out['test']['labels']
+        return d_out, avg_toks, d_n_tok
+
+    def extract_utcd_meta(self) -> Dict:
+        d_utcd = self.d['UTCD']
+        d_dsets: Dict = d_utcd['datasets']
+        logger = get_logger('Extracting UTCD metadata')
+        d_n_toks = dict()
+
+        it = d_dsets.items()
+        if self.fast:
+            it = tqdm(it, desc='Extracting UTCD metadata', total=len(d_dsets))
+        for dnm, d_dset in it:
+            if self.fast:
+                it.set_postfix(dnm=pl.i(dnm))
+            else:
+                logger.info(f'Processing {pl.i(dnm)}... ')
+            d_dset['splits'], d_avg_tok, d_n_toks[dnm] = self._path2dataset_info(d_dset)
+            if d_avg_tok is not None:
+                d_dset.update(d_avg_tok)
+        dnms = sorted(d_dsets)  # All datasets, in- and out-of-domain, share the same dataset <=> id mapping
+        d_utcd['dataset_id2name'] = dnms
+        d_utcd['dataset_name2id'] = {dnm: i for i, dnm in enumerate(dnms)}
+        return d_n_toks
 
 
 def plot_utcd_n_toks(d_n_toks: Dict, domain: str, save=True):
     def weighted_quantile(values, quantiles, sample_weight=None, values_sorted=False, old_style=False):
         # Credit: https://stackoverflow.com/a/29677616/10732321
-        """ Very close to numpy.percentile, but supports weights.
+        """ Very close to numpy::percentile, but supports weights.
         NOTE: quantiles should be in [0, 1]!
-        :param values: numpy.array with data
+        :param values: numpy array with data
         :param quantiles: array-like with many quantiles needed
         :param sample_weight: array-like of the same length as `array`
         :param values_sorted: bool, if True, then will avoid sorting of
             initial array
         :param old_style: if True, will correct output to be consistent
             with numpy.percentile.
         :return: numpy.array with computed quantiles.
@@ -440,27 +439,31 @@
             ax.set_xticks(list(range(math.floor(xticks.min()), math.ceil(xticks.max()) + 1)))
     domain = 'in-domain' if domain == 'in' else 'out-of-domain eval'
     title = f'Tokenization length distribution across {domain} datasets'
     plt.suptitle(title)
     fig.supxlabel('#token')
     fig.supylabel('Density')
     if save:
+        # this function is for standalone execution, importing here prevents circular import
+        from zeroshot_classifier.util.util import save_fig
         save_fig(title)
     else:
         plt.show()
 
 
-d_n_tok = extract_utcd_meta()
-for dom in ['in']:
-    # plot only in-domain data as out-of-domain tokens lengths are too long,
-    # resulting in prohibitively large # of patches for bar-plot to terminate soon
-    d_n_tok_ = {dnm: v for dnm, v in d_n_tok.items() if get(config_dict, f'UTCD.datasets.{dnm}.domain') == dom}
-    plot_utcd_n_toks(d_n_tok_, domain=dom, save=True)
-
-
 if __name__ == '__main__':
-    from zeroshot_classifier.util.data_path import PKG_NM
+    config_d = ConfigDict(fast=False)  # If run standalone, compute #token stats
 
-    fl_nm = 'config.json'
-    mic(config_dict)
-    with open(os_join(BASE_PATH, PROJ_DIR, PKG_NM, 'util', 'config.json'), 'w') as f:
-        json.dump(config_dict, f, indent=4)
+    def plot_toks():
+        d_n_tok = config_d.d_n_toks
+        for dom in ['in']:
+            # plot only in-domain data as out-of-domain tokens lengths are too long,
+            # resulting in prohibitively large # of patches for bar-plot to terminate soon
+            d_n_tok_ = {dnm: v for dnm, v in d_n_tok.items() if get(config_d.d, f'UTCD.datasets.{dnm}.domain') == dom}
+            plot_utcd_n_toks(d_n_tok_, domain=dom, save=True)
+    # plot_toks()
+
+    def write_config():
+        mic(config_d.d)
+        with open(os_join(BASE_PATH, PROJ_DIR, PKG_NM, 'util', 'config.json'), 'w') as f:
+            json.dump(config_d.d, f, indent=4)
+    write_config()
```

### Comparing `zeroshot-classifier-0.1.2/zeroshot_classifier/util/data_path.py` & `zeroshot-classifier-0.2.0/zeroshot_classifier/util/data_path.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.2/zeroshot_classifier/util/explicit_v2_pretrain.py` & `zeroshot-classifier-0.2.0/zeroshot_classifier/util/explicit_v2_pretrain.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.2/zeroshot_classifier/util/gpt2_train.py` & `zeroshot-classifier-0.2.0/zeroshot_classifier/util/gpt2_train.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.2/zeroshot_classifier/util/load_data.py` & `zeroshot-classifier-0.2.0/zeroshot_classifier/util/load_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,47 +3,39 @@
 import json
 import time
 import gzip
 import random
 import itertools
 from os import listdir
 from os.path import isfile, join as os_join, basename
-from zipfile import ZipFile
 from collections import Counter, defaultdict
 from typing import List, Tuple, Set, Dict, Union
 
 import numpy as np
 from numpy import argmax, argmin
 import spacy
 from sentence_transformers.readers import InputExample
 from sentence_transformers import util
-import gdown
 from tqdm import tqdm
 
 from stefutil import *
 from zeroshot_classifier.util import *
 
 
 __all__ = [
-    'in_domain_url', 'out_of_domain_url', 'in_domain_data_path', 'out_of_domain_data_path',
     'Dataset', 'SplitDataset',
     'get_datasets', 'to_aspect_normalized_datasets',
     'nli_template', 'get_nli_data', 'binary_cls_format', 'nli_cls_format', 'encoder_cls_format', 'seq_cls_format',
     'binary_explicit_format'
 ]
 
 
 logger = get_logger('Load Data')
 
 
-in_domain_url = 'https://drive.google.com/uc?id=1V7IzdZ9HQbFUQz9NzBDjmqYBdPd9Yfe3'
-out_of_domain_url = 'https://drive.google.com/uc?id=1nd32_UrFbgoCgH4bDtFFD_YFZhzcts3x'
-dataset_path = './dataset'
-in_domain_data_path = './dataset/in-domain'
-out_of_domain_data_path = './dataset/out-of-domain'
 ASPECT_NORM_DIRNM = 'aspect-normalized'
 
 
 def _get_nlp():
     if not hasattr(_get_nlp, 'nlp'):
         _get_nlp.nlp = spacy.load("en_core_web_md")
         _get_nlp.nlp.disable_pipes(['tagger', 'parser', 'attribute_ruler', 'lemmatizer', 'ner'])
@@ -86,20 +78,18 @@
     :param normalize_aspect: If true, # of training samples for each aspect is normalized
         via subsampling datasets in the larger aspect
         If int given, used as seed for sampling
     :param domain: Needed for aspect normalization
         Intended for training directly on out-of-domain data, see `zeroshot_classifier/models/bert.py`
     :param dataset_names: If given, only load the specified datasets
     """
-    domain_paths = in_domain_data_path if domain == 'in' else out_of_domain_data_path
-    domain_paths = [d for d in domain_paths.split(os.sep) if d != '.']
-    path = os_join(u.proj_path, *domain_paths)
+    domain_dir_nm = in_domain_dir_nm if domain == 'in' else out_of_domain_dir_nm
+    path = os_join(u.proj_path, u.dset_dir, domain_dir_nm)
     if not os.path.exists(path):
-        logger.info(f'Downloading {pl.i(domain)} domain data from GDrive to {pl.i(path)}...')
-        download_data(path)
+        download_data(domain=domain)
     datasets = None
     _keys = {'train', 'test', 'aspect', 'labels'}
     if normalize_aspect:
         if isinstance(normalize_aspect, int):
             assert normalize_aspect == sconfig('random-seed')
         path = os_join(path, ASPECT_NORM_DIRNM)
         if not os.path.exists(path):
@@ -247,15 +237,17 @@
     logger.info(f'Training set after split: {pl.i(dset2meta(tr))}')
     logger.info(f'Eval set after split: {pl.i(dset2meta(vl))}')
     return dict(train=tr, eval=vl)
 
 
 def save_aspect_normalized_datasets(domain: str = 'in'):
     seed = sconfig('random-seed')
-    path = in_domain_data_path if domain == 'in' else out_of_domain_data_path
+
+    domain_dir_nm = in_domain_dir_nm if domain == 'in' else out_of_domain_dir_nm
+    path = os_join(u.proj_path, u.dset_dir, domain_dir_nm)
     dsets = get_datasets(domain=domain)
     dsets = to_aspect_normalized_datasets(dsets, seed=seed, domain=domain)
 
     out_path = os.path.join(path, ASPECT_NORM_DIRNM)
     os.makedirs(out_path, exist_ok=True)
 
     ret = dict()
@@ -267,35 +259,14 @@
         logger.info(f'Saving normalized {pl.i(dnm)} dataset to {pl.i(path_out)}... ')
         with open(path, 'w') as f:
             json.dump(dsets__, f)
         ret[dnm] = dsets__
     return ret
 
 
-def download_data(path):
-    if 'in-domain' in path:
-        file = './dataset/in-domain.zip'
-        url = in_domain_url
-    else:
-        assert 'out-of-domain' in path
-        file = './dataset/out-domain.zip'
-        url = out_of_domain_url
-    fl_paths = [d for d in file.split(os.sep) if d != '.']
-    fl_path = os.path.join(u.proj_path, *fl_paths)
-    os.makedirs(os.path.dirname(fl_path), exist_ok=True)
-    gdown.download(url, fl_path, quiet=False)
-
-    with ZipFile(file, "r") as zfl:
-        dset_paths = [d for d in dataset_path.split(os.sep) if d != '.']
-        path = os_join(u.proj_path, *dset_paths)
-        os.makedirs(path, exist_ok=True)
-        zfl.extractall(path)
-        zfl.close()
-
-
 def get_nli_data():
     nli_dataset_path = 'dataset/AllNLI.tsv.gz'
 
     if not os.path.exists(nli_dataset_path):
         util.http_get('https://sbert.net/datasets/AllNLI.tsv.gz', nli_dataset_path)
 
     label2int = {"contradiction": 0, "entailment": 1, "neutral": 2}
@@ -627,15 +598,15 @@
 
 if __name__ == '__main__':
     mic.output_width = 512
 
     random.seed(sconfig('random-seed'))
 
     def check_sampling():
-        data = get_datasets(in_domain_data_path)
+        data = get_datasets(domain='in')
         data = to_aspect_normalized_datasets(data)
         for dnm, d_dset in data.items():
             mic(dnm, len(d_dset['train']))
             c = Counter()
             for txt, lbs in d_dset['train'].items():
                 c.update(lbs)
             mic(c, len(c))
```

### Comparing `zeroshot-classifier-0.1.2/zeroshot_classifier/util/training.py` & `zeroshot-classifier-0.2.0/zeroshot_classifier/util/training.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.2/zeroshot_classifier/util/utcd.py` & `zeroshot-classifier-0.2.0/zeroshot_classifier/util/utcd.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.2/zeroshot_classifier/util/util.py` & `zeroshot-classifier-0.2.0/zeroshot_classifier/util/util.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,81 @@
 import os
 import math
 import json
 import configparser
 from os.path import join as os_join
 from typing import List, Tuple, Dict, Iterable, Optional
+from zipfile import ZipFile
 
 import numpy as np
 import pandas as pd
 import sklearn
 from datasets import load_metric
 import matplotlib.pyplot as plt
+import gdown
 
 from stefutil import *
 from zeroshot_classifier.util.data_path import BASE_PATH, PROJ_DIR, DSET_DIR, PKG_NM, MODEL_DIR
 
 
 __all__ = [
+    'in_domain_url', 'out_of_domain_url', 'in_domain_dir_nm', 'out_of_domain_dir_nm', 'download_data',
     'sconfig', 'u', 'save_fig', 'plot_points',
     'on_great_lakes', 'get_base_path',
     'map_model_dir_nm', 'map_model_output_path', 'domain2eval_dir_nm', 'TrainStrategy2PairMap',
     'eval_res2df', 'compute_metrics'
 ]
 
 
 logger = get_logger('Util')
 
 
+in_domain_url = 'https://drive.google.com/uc?id=1V7IzdZ9HQbFUQz9NzBDjmqYBdPd9Yfe3'
+out_of_domain_url = 'https://drive.google.com/uc?id=1nd32_UrFbgoCgH4bDtFFD_YFZhzcts3x'
+in_domain_dir_nm = 'in-domain'
+out_of_domain_dir_nm = 'out-of-domain'
+
+
+def download_data(domain: str = 'in'):  # Needed for writing config
+    assert domain in ['in', 'out']
+    if domain == 'in':
+        fnm, url = f'{in_domain_dir_nm}.zip', in_domain_url
+    else:  # `out`
+        fnm, url = f'{out_of_domain_dir_nm}.zip', out_of_domain_url
+    base_path = os.path.join(BASE_PATH, PROJ_DIR, DSET_DIR)
+    os.makedirs(base_path, exist_ok=True)
+    fl_path = os_join(base_path, fnm)
+
+    domain_str = 'in-domain' if domain == 'in' else 'out-of-domain'
+    logger.info(f'Downloading {pl.i(domain_str)} data from GDrive to {pl.i(fl_path)}...')
+    gdown.download(url, fl_path, quiet=False)
+
+    with ZipFile(fl_path, 'r') as zfl:
+        zfl.extractall(base_path)
+        zfl.close()
+
+
+def _download_all_data():
+    dset_path = os_join(BASE_PATH, PROJ_DIR, DSET_DIR)
+    path_in = os_join(dset_path, in_domain_dir_nm)
+    if not os.path.exists(path_in):
+        download_data(domain='in')
+    path_out = os_join(dset_path, out_of_domain_dir_nm)
+    if not os.path.exists(path_out):
+        download_data(domain='out')
+
+
+_download_all_data()  # Needed for writing config
+
+
 config_path = os_join(BASE_PATH, PROJ_DIR, PKG_NM, 'util', 'config.json')
 if not os.path.exists(config_path):
-    from zeroshot_classifier.util.config import config_dict
-    logger.info(f'Writing config file at {pl.i(config_path)}')
+    from zeroshot_classifier.util.config import ConfigDict
+    logger.info(f'Writing config file to {pl.i(config_path)}... ')
+    config_dict = ConfigDict(fast=True).d
     with open(config_path, 'w') as f:
         json.dump(config_dict, f, indent=4)
 
 sconfig = StefConfig(config_file=config_path).__call__
 u = StefUtil(
     base_path=BASE_PATH, project_dir=PROJ_DIR, package_name=PKG_NM, dataset_dir=DSET_DIR, model_dir=MODEL_DIR
 )
```

### Comparing `zeroshot-classifier-0.1.2/zeroshot_classifier/visualize/visualize_text_sample_loss.py` & `zeroshot-classifier-0.2.0/zeroshot_classifier/visualize/visualize_text_sample_loss.py`

 * *Files identical despite different names*

### Comparing `zeroshot-classifier-0.1.2/zeroshot_classifier.egg-info/PKG-INFO` & `zeroshot-classifier-0.2.0/zeroshot_classifier.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: zeroshot-classifier
-Version: 0.1.2
+Version: 0.2.0
 Summary: code and data for the Findings of ACL'23 paper Label Agnostic Pre-training for Zero-shot Text Classification 
 Home-page: https://github.com/ChrisIsKing/zero-shot-text-classification
-Download-URL: https://github.com/ChrisIsKing/zero-shot-text-classification/archive/refs/tags/v0.1.2.tar.gz
+Download-URL: https://github.com/ChrisIsKing/zero-shot-text-classification/archive/refs/tags/v0.2.0.tar.gz
 Author: Christopher Clarke & Yuzhao Heng
 Author-email: csclarke@umich.edu
 License: MIT
 Keywords: python,nlp,machine-learning,deep-learning,text-classification,zero-shot-classification
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: GPU :: NVIDIA CUDA
 Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.6
```

### Comparing `zeroshot-classifier-0.1.2/zeroshot_classifier.egg-info/SOURCES.txt` & `zeroshot-classifier-0.2.0/zeroshot_classifier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

