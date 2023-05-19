# Comparing `tmp/cappr-0.2.5.tar.gz` & `tmp/cappr-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cappr-0.2.5.tar", last modified: Fri May  5 10:33:42 2023, max compression
+gzip compressed data, was "cappr-0.2.6.tar", last modified: Fri May 19 22:17:46 2023, max compression
```

## Comparing `cappr-0.2.5.tar` & `cappr-0.2.6.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:33:41.997619 cappr-0.2.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:33:41.985619 cappr-0.2.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:33:41.985619 cappr-0.2.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-05 10:33:31.000000 cappr-0.2.5/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-05 10:33:31.000000 cappr-0.2.5/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-05 10:33:31.000000 cappr-0.2.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-05 10:33:31.000000 cappr-0.2.5/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-05 10:33:31.000000 cappr-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15204 2023-05-05 10:33:41.997619 cappr-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14820 2023-05-05 10:33:31.000000 cappr-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:33:41.989619 cappr-0.2.5/demos/
--rw-r--r--   0 runner    (1001) docker     (123)  2760040 2023-05-05 10:33:31.000000 cappr-0.2.5/demos/computational_analysis.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    19512 2023-05-05 10:33:31.000000 cappr-0.2.5/demos/politeness.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:33:41.989619 cappr-0.2.5/demos/raft/
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-05 10:33:31.000000 cappr-0.2.5/demos/raft/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-05-05 10:33:31.000000 cappr-0.2.5/demos/raft/ade.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    13328 2023-05-05 10:33:31.000000 cappr-0.2.5/demos/raft/b77.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    15238 2023-05-05 10:33:31.000000 cappr-0.2.5/demos/raft/nis.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11465 2023-05-05 10:33:31.000000 cappr-0.2.5/demos/raft/ose.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8789 2023-05-05 10:33:31.000000 cappr-0.2.5/demos/raft/over.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11177 2023-05-05 10:33:31.000000 cappr-0.2.5/demos/raft/sot.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12914 2023-05-05 10:33:31.000000 cappr-0.2.5/demos/raft/sri.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    15611 2023-05-05 10:33:31.000000 cappr-0.2.5/demos/raft/tai.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11933 2023-05-05 10:33:31.000000 cappr-0.2.5/demos/raft/tc.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-05-05 10:33:31.000000 cappr-0.2.5/demos/raft/teh.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-05-05 10:33:31.000000 cappr-0.2.5/demos/raft/tos.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:33:41.989619 cappr-0.2.5/demos/superglue/
--rw-r--r--   0 runner    (1001) docker     (123)    64027 2023-05-05 10:33:31.000000 cappr-0.2.5/demos/superglue/copa.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    42865 2023-05-05 10:33:31.000000 cappr-0.2.5/demos/superglue/wsc.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-05 10:33:31.000000 cappr-0.2.5/demos/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:33:41.989619 cappr-0.2.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-05 10:33:31.000000 cappr-0.2.5/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-05 10:33:31.000000 cappr-0.2.5/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:33:41.993619 cappr-0.2.5/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-05 10:33:31.000000 cappr-0.2.5/docs/source/1_is_for_me.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-05-05 10:33:31.000000 cappr-0.2.5/docs/source/2_motivation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-05 10:33:31.000000 cappr-0.2.5/docs/source/3_installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-05-05 10:33:31.000000 cappr-0.2.5/docs/source/4_user_guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-05 10:33:31.000000 cappr-0.2.5/docs/source/5_examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-05 10:33:31.000000 cappr-0.2.5/docs/source/6_computational_performance.rst
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-05 10:33:31.000000 cappr-0.2.5/docs/source/7_future_research.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:33:41.993619 cappr-0.2.5/docs/source/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:33:41.993619 cappr-0.2.5/docs/source/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-05 10:33:31.000000 cappr-0.2.5/docs/source/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-05-05 10:33:31.000000 cappr-0.2.5/docs/source/_static/github-mark.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:33:41.993619 cappr-0.2.5/docs/source/_static/scaling_classes/
--rw-r--r--   0 runner    (1001) docker     (123)    53692 2023-05-05 10:33:31.000000 cappr-0.2.5/docs/source/_static/scaling_classes/batch_size_32.png
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-05 10:33:31.000000 cappr-0.2.5/docs/source/cappr.huggingface.classify.rst
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-05 10:33:31.000000 cappr-0.2.5/docs/source/cappr.huggingface.classify_no_cache.rst
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-05 10:33:31.000000 cappr-0.2.5/docs/source/cappr.huggingface.rst
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-05 10:33:31.000000 cappr-0.2.5/docs/source/cappr.openai.api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-05 10:33:31.000000 cappr-0.2.5/docs/source/cappr.openai.classify.rst
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-05 10:33:31.000000 cappr-0.2.5/docs/source/cappr.openai.rst
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-05 10:33:31.000000 cappr-0.2.5/docs/source/cappr.rst
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-05 10:33:31.000000 cappr-0.2.5/docs/source/cappr.utils.classify.rst
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-05 10:33:31.000000 cappr-0.2.5/docs/source/cappr.utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-05-05 10:33:31.000000 cappr-0.2.5/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-05 10:33:31.000000 cappr-0.2.5/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-05 10:33:31.000000 cappr-0.2.5/docs/source/related_work.rst
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-05 10:33:31.000000 cappr-0.2.5/docs/source/research.rst
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-05 10:33:31.000000 cappr-0.2.5/docs/source/walkthrough.rst
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-05 10:33:31.000000 cappr-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 10:33:41.997619 cappr-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-05-05 10:33:31.000000 cappr-0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:33:41.985619 cappr-0.2.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:33:41.993619 cappr-0.2.5/src/cappr/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-05 10:33:31.000000 cappr-0.2.5/src/cappr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-05 10:33:31.000000 cappr-0.2.5/src/cappr/_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:33:41.993619 cappr-0.2.5/src/cappr/huggingface/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-05 10:33:31.000000 cappr-0.2.5/src/cappr/huggingface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-05-05 10:33:31.000000 cappr-0.2.5/src/cappr/huggingface/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    34123 2023-05-05 10:33:31.000000 cappr-0.2.5/src/cappr/huggingface/classify.py
--rw-r--r--   0 runner    (1001) docker     (123)    27982 2023-05-05 10:33:31.000000 cappr-0.2.5/src/cappr/huggingface/classify_no_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:33:41.993619 cappr-0.2.5/src/cappr/openai/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-05 10:33:31.000000 cappr-0.2.5/src/cappr/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-05-05 10:33:31.000000 cappr-0.2.5/src/cappr/openai/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25351 2023-05-05 10:33:31.000000 cappr-0.2.5/src/cappr/openai/classify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:33:41.997619 cappr-0.2.5/src/cappr/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-05 10:33:31.000000 cappr-0.2.5/src/cappr/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-05 10:33:31.000000 cappr-0.2.5/src/cappr/utils/_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-05 10:33:31.000000 cappr-0.2.5/src/cappr/utils/_check.py
--rw-r--r--   0 runner    (1001) docker     (123)    11531 2023-05-05 10:33:31.000000 cappr-0.2.5/src/cappr/utils/classify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:33:41.993619 cappr-0.2.5/src/cappr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15204 2023-05-05 10:33:41.000000 cappr-0.2.5/src/cappr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-05 10:33:41.000000 cappr-0.2.5/src/cappr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 10:33:41.000000 cappr-0.2.5/src/cappr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-05 10:33:41.000000 cappr-0.2.5/src/cappr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-05 10:33:41.000000 cappr-0.2.5/src/cappr.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:33:41.997619 cappr-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-05-05 10:33:31.000000 cappr-0.2.5/tests/_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:33:41.997619 cappr-0.2.5/tests/huggingface/
--rw-r--r--   0 runner    (1001) docker     (123)    14616 2023-05-05 10:33:31.000000 cappr-0.2.5/tests/huggingface/test_huggingface_classify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:33:41.997619 cappr-0.2.5/tests/openai/
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-05-05 10:33:31.000000 cappr-0.2.5/tests/openai/test_openai_classify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:33:41.997619 cappr-0.2.5/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-05 10:33:31.000000 cappr-0.2.5/tests/utils/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-05 10:33:31.000000 cappr-0.2.5/tests/utils/test_utils_classify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:17:46.150595 cappr-0.2.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:17:46.126595 cappr-0.2.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:17:46.130595 cappr-0.2.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-19 22:17:32.000000 cappr-0.2.6/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-19 22:17:32.000000 cappr-0.2.6/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-19 22:17:32.000000 cappr-0.2.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-19 22:17:32.000000 cappr-0.2.6/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-19 22:17:32.000000 cappr-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14554 2023-05-19 22:17:46.150595 cappr-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14170 2023-05-19 22:17:32.000000 cappr-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:17:46.134595 cappr-0.2.6/demos/
+-rw-r--r--   0 runner    (1001) docker     (123)  2760040 2023-05-19 22:17:32.000000 cappr-0.2.6/demos/computational_analysis.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    19512 2023-05-19 22:17:32.000000 cappr-0.2.6/demos/politeness.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:17:46.138595 cappr-0.2.6/demos/raft/
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-19 22:17:32.000000 cappr-0.2.6/demos/raft/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-05-19 22:17:32.000000 cappr-0.2.6/demos/raft/ade.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    13328 2023-05-19 22:17:32.000000 cappr-0.2.6/demos/raft/b77.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    15238 2023-05-19 22:17:32.000000 cappr-0.2.6/demos/raft/nis.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11465 2023-05-19 22:17:32.000000 cappr-0.2.6/demos/raft/ose.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8789 2023-05-19 22:17:32.000000 cappr-0.2.6/demos/raft/over.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11177 2023-05-19 22:17:32.000000 cappr-0.2.6/demos/raft/sot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12914 2023-05-19 22:17:32.000000 cappr-0.2.6/demos/raft/sri.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    15611 2023-05-19 22:17:32.000000 cappr-0.2.6/demos/raft/tai.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11933 2023-05-19 22:17:32.000000 cappr-0.2.6/demos/raft/tc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-05-19 22:17:32.000000 cappr-0.2.6/demos/raft/teh.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-05-19 22:17:32.000000 cappr-0.2.6/demos/raft/tos.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:17:46.138595 cappr-0.2.6/demos/superglue/
+-rw-r--r--   0 runner    (1001) docker     (123)    64027 2023-05-19 22:17:32.000000 cappr-0.2.6/demos/superglue/copa.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    42865 2023-05-19 22:17:32.000000 cappr-0.2.6/demos/superglue/wsc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-19 22:17:32.000000 cappr-0.2.6/demos/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:17:46.138595 cappr-0.2.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-19 22:17:32.000000 cappr-0.2.6/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-19 22:17:32.000000 cappr-0.2.6/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:17:46.142595 cappr-0.2.6/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-19 22:17:32.000000 cappr-0.2.6/docs/source/1_is_for_me.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-05-19 22:17:32.000000 cappr-0.2.6/docs/source/2_motivation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-19 22:17:32.000000 cappr-0.2.6/docs/source/3_installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-05-19 22:17:32.000000 cappr-0.2.6/docs/source/4_user_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-19 22:17:32.000000 cappr-0.2.6/docs/source/5_examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-19 22:17:32.000000 cappr-0.2.6/docs/source/6_computational_performance.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-19 22:17:32.000000 cappr-0.2.6/docs/source/7_future_research.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:17:46.146595 cappr-0.2.6/docs/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:17:46.146595 cappr-0.2.6/docs/source/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-19 22:17:32.000000 cappr-0.2.6/docs/source/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-05-19 22:17:32.000000 cappr-0.2.6/docs/source/_static/github-mark.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:17:46.146595 cappr-0.2.6/docs/source/_static/scaling_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)    53692 2023-05-19 22:17:32.000000 cappr-0.2.6/docs/source/_static/scaling_classes/batch_size_32.png
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-19 22:17:32.000000 cappr-0.2.6/docs/source/cappr.huggingface.classify.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-19 22:17:32.000000 cappr-0.2.6/docs/source/cappr.huggingface.classify_no_cache.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-19 22:17:32.000000 cappr-0.2.6/docs/source/cappr.huggingface.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-19 22:17:32.000000 cappr-0.2.6/docs/source/cappr.openai.api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-19 22:17:32.000000 cappr-0.2.6/docs/source/cappr.openai.classify.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-19 22:17:32.000000 cappr-0.2.6/docs/source/cappr.openai.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-19 22:17:32.000000 cappr-0.2.6/docs/source/cappr.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-19 22:17:32.000000 cappr-0.2.6/docs/source/cappr.utils.classify.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-19 22:17:32.000000 cappr-0.2.6/docs/source/cappr.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-05-19 22:17:32.000000 cappr-0.2.6/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-19 22:17:32.000000 cappr-0.2.6/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-19 22:17:32.000000 cappr-0.2.6/docs/source/related_work.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-19 22:17:32.000000 cappr-0.2.6/docs/source/research.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-19 22:17:32.000000 cappr-0.2.6/docs/source/walkthrough.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-19 22:17:32.000000 cappr-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 22:17:46.150595 cappr-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-05-19 22:17:32.000000 cappr-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:17:46.130595 cappr-0.2.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:17:46.146595 cappr-0.2.6/src/cappr/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-19 22:17:32.000000 cappr-0.2.6/src/cappr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-19 22:17:32.000000 cappr-0.2.6/src/cappr/_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:17:46.146595 cappr-0.2.6/src/cappr/huggingface/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-19 22:17:32.000000 cappr-0.2.6/src/cappr/huggingface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-19 22:17:32.000000 cappr-0.2.6/src/cappr/huggingface/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31664 2023-05-19 22:17:32.000000 cappr-0.2.6/src/cappr/huggingface/classify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25608 2023-05-19 22:17:32.000000 cappr-0.2.6/src/cappr/huggingface/classify_no_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:17:46.146595 cappr-0.2.6/src/cappr/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-19 22:17:32.000000 cappr-0.2.6/src/cappr/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-05-19 22:17:32.000000 cappr-0.2.6/src/cappr/openai/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25383 2023-05-19 22:17:32.000000 cappr-0.2.6/src/cappr/openai/classify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:17:46.150595 cappr-0.2.6/src/cappr/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-19 22:17:32.000000 cappr-0.2.6/src/cappr/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-19 22:17:32.000000 cappr-0.2.6/src/cappr/utils/_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-19 22:17:32.000000 cappr-0.2.6/src/cappr/utils/_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11541 2023-05-19 22:17:32.000000 cappr-0.2.6/src/cappr/utils/classify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:17:46.146595 cappr-0.2.6/src/cappr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14554 2023-05-19 22:17:46.000000 cappr-0.2.6/src/cappr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-19 22:17:46.000000 cappr-0.2.6/src/cappr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 22:17:46.000000 cappr-0.2.6/src/cappr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-19 22:17:46.000000 cappr-0.2.6/src/cappr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-19 22:17:46.000000 cappr-0.2.6/src/cappr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:17:46.150595 cappr-0.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-05-19 22:17:32.000000 cappr-0.2.6/tests/_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:17:46.150595 cappr-0.2.6/tests/huggingface/
+-rw-r--r--   0 runner    (1001) docker     (123)    14616 2023-05-19 22:17:32.000000 cappr-0.2.6/tests/huggingface/test_huggingface_classify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:17:46.150595 cappr-0.2.6/tests/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-05-19 22:17:32.000000 cappr-0.2.6/tests/openai/test_openai_classify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:17:46.150595 cappr-0.2.6/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-19 22:17:32.000000 cappr-0.2.6/tests/utils/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-19 22:17:32.000000 cappr-0.2.6/tests/utils/test_utils_classify.py
```

### Comparing `cappr-0.2.5/.github/workflows/python-publish.yml` & `cappr-0.2.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `cappr-0.2.5/.github/workflows/test.yml` & `cappr-0.2.6/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `cappr-0.2.5/LICENSE` & `cappr-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cappr-0.2.5/PKG-INFO` & `cappr-0.2.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: cappr
-Version: 0.2.5
-Summary: Zero-shot text classification using autoregressive language models.
-Home-page: https://github.com/kddubey/cappr/
-Author-email: kushdubey63@gmail.com
-License: Apache License 2.0
-Requires-Python: >=3.8.0
-Description-Content-Type: text/markdown
-Provides-Extra: hf
-Provides-Extra: demos
-Provides-Extra: dev
-License-File: LICENSE
-
 # CAPPr: zero-shot text classification using autoregressive language models
 
 [![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-380/)
 [![Documentation Status](https://readthedocs.org/projects/cappr/badge/?version=latest)](https://cappr.readthedocs.io/en/latest/?badge=latest)
 [![tests](https://github.com/kddubey/cappr/actions/workflows/test.yml/badge.svg)](https://github.com/kddubey/cappr/actions/workflows/test.yml)
 [![codecov](https://codecov.io/gh/kddubey/cappr/branch/main/graph/badge.svg?token=NYIL076PSM)](https://codecov.io/gh/kddubey/cappr)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
@@ -26,15 +12,15 @@
 completion comes after an inputted prompt. Hence the name:
 
 > **C**ompletion<br>
   **A**fter<br>
   **P**rompt<br>
   **Pr**obability<br>
 
-The method is fleshed out in my [question on CrossValidated](https://stats.stackexchange.com/q/601159/337906).
+The method is fleshed out in my [question on Cross Validated](https://stats.stackexchange.com/q/601159/337906).
 
 
 ## Usage
 
 <details>
 <summary>Use a model from the OpenAI API</summary>
 
@@ -65,42 +51,47 @@
 ```
 </details>
 
 <details>
 <summary>Use a model from the HuggingFace model hub</summary>
 
 Specifically, this model must be able to be loaded using
-`transformers.AutoModelForCausalLM.from_pretrained(model)`.
-
-Smaller LMs may not work well. But there will likely be better ones in the hub soon.
+`transformers.AutoModelForCausalLM.from_pretrained`.
 
 ```python
+from transformers import AutoModelForCausalLM, AutoTokenizer
 from cappr.huggingface.classify import predict
 
 prompt = 'Which planet is closer to the Sun: Mercury or Earth?'
 
 class_names = ('Mercury', 'Earth')
 prior = None  # uniform prior
 
+# load model and tokenizer
+model_name = 'gpt2'
+model = AutoModelForCausalLM.from_pretrained(model_name)
+tokenizer = AutoTokenizer.from_pretrained(model_name)
+
 preds = predict(prompts=[prompt],
                 completions=class_names,
-                model='gpt2',
+                model_and_tokenizer=(model, tokenizer),
                 prior=prior)
 preds
 # ['Mercury']
 ```
 </details>
 
 <details>
 <summary>Run in batches</summary>
 
 Let's use `huggingface` for this example cuz it's free. And let's predict probabilities
 instead of the class.
 
 ```python
+from transformers import AutoModelForCausalLM, AutoTokenizer
 from cappr.huggingface.classify import predict_proba
 
 prompts = [
     'Stephen Curry is a',
     'Martina Navratilova was a',
     "Dexter, from the TV Series Dexter's Laboratory, is a",
     'LeBron James is a',    
@@ -115,17 +106,23 @@
 
 prior = (
     1/6,  # few
     1/6,  # few
     2/3   # there are more
 )
 
+
+# load model and tokenizer
+model_name = 'gpt2'
+model = AutoModelForCausalLM.from_pretrained(model_name)
+tokenizer = AutoTokenizer.from_pretrained(model_name)
+
 pred_probs = predict_proba(prompts=prompts,
                            completions=class_names,
-                           model='gpt2',
+                           model_and_tokenizer=(model, tokenizer),
                            batch_size=32,  # whatever fits on your CPU/GPU
                            prior=prior)
 
 # pred_probs[i,j] = probability that prompts[i] is classified as class_names[j]
 print(pred_probs.round(1))
 # [[0.5 0.3 0.2]
 #  [0.3 0.6 0.2]
@@ -142,17 +139,15 @@
 ```
 </details>
 
 <details>
 <summary>Run in batches, where each prompt has a different set of possible completions
 </summary>
 
-Again, let's use `huggingface` to predict probabilities. And this time, let's pass in an 
-instantiated model and tokenizer instead of its name. That way, the model isn't
-re-loaded every time you wanna use it.
+Again, let's use `huggingface` to predict probabilities.
 
 ```python
 import numpy as np
 from transformers import AutoModelForCausalLM, AutoTokenizer
 
 from cappr import Example
 from cappr.huggingface.classify import predict_proba_examples
@@ -194,18 +189,15 @@
 See
 [`demos/superglue/copa.ipynb`](https://github.com/kddubey/cappr/blob/main/demos/superglue/copa.ipynb)
 for a demonstration of a slightly harder classification task.
 
 
 ## Documentation
 
-https://cappr.readthedocs.io/en/latest/
-
-Please let me know if you find the writing too dense. The main motivation behind this
-project is simplicity :-)
+https://cappr.readthedocs.io
 
 
 ## Setup
 
 If you intend on using OpenAI models, [sign up for the OpenAI API
 here](https://platform.openai.com/signup), and then set the environment variable
 `OPENAI_API_KEY`. For zero-shot classification, OpenAI models are currently far ahead of
@@ -213,43 +205,39 @@
 
 Install with `pip`:
 
 ```
 python -m pip install cappr
 ```
 
-<details>
-<summary>(Optional) Install requirements for HuggingFace models</summary>
+(Optional) Install requirements for HuggingFace models
 
 ```
 python -m pip install cappr[hf]
 ```
-</details>
 
-<details>
-<summary>(Optional) Install requirements for running demos</summary>
+(Optional) Install requirements for running demos
 
 ```
 python -m pip install cappr[demos]
 ```
-</details>
 
 
 ## Motivation
 
 Create a more usable zero-shot text classification interface than
 [classification via sampling (CVS)](https://platform.openai.com/docs/guides/completion/classification).
 
 <details>
 <summary>Short</summary>
 
-In CVS, your job is to write up your classification task in a `prompt` string, and then
-write custom code to post-process arbitrary `completion`/output strings.
+With CVS, your job is to write up your classification task in a `prompt` string, and
+then write custom code to post-process arbitrary `completion`/output strings.
 
-In CAPPr, your job starts and stops at writing up your classification task as a
+With CAPPr, your job starts and stops at writing up your classification task as a
 `{prompt}{end_of_prompt}{completion}` string.
 </details>
 
 <details>
 <summary>Long</summary>
 
 Please see [this page of the
@@ -305,20 +293,20 @@
 you'll be on the *cappr (slow)* line** :-(
 
 ![](/docs/source/_static/scaling_classes/batch_size_32.png)
 
 *Figure 1: [COPA](https://people.ict.usc.edu/~gordon/copa.html) dataset, repeating the
 choices to simulate multi-class classification tasks. [GPT-2
 (small)](https://huggingface.co/gpt2) was run on a Tesla K80 GPU (whatever was free in
-Google Colab in March 2023, I'm not hardware savvy). 96 classification inputs were
-processed in batches of size 32. Each point in the graph is a median of 5 runs. For
-classification via sampling (CVS), exactly 4 tokens were generated for each prompt,
-which is the number of tokens in `'\n\nAnswer A'`. 1-token times are also shown. But for
-COPA (and other multiple-choice style prompts), that may result in lower zero-shot
-accuracy, as most of the sampled choices come after the first token.*
+Google Colab in March 2023). 96 classification inputs were processed in batches of size
+32. Each point in the graph is a median of 5 runs. For classification via sampling
+(CVS), exactly 4 tokens were generated for each prompt, which is the number of tokens in
+`'\n\nAnswer A'`. 1-token times are also shown. But for COPA (and other multiple-choice
+style prompts), that may result in lower zero-shot accuracy, as most of the sampled
+choices come after the first token.*
 
 See the [`demos/computational_analysis.ipynb`
 notebook](https://github.com/kddubey/cappr/blob/main/demos/computational_analysis.ipynb).
 
 </details>
 
 
@@ -384,74 +372,64 @@
 (**) = I'm currently working on this or will work on it really soon
 
 <details>
 <summary>Code</summary>
 
 - [ ] Testing
   - [ ] Increase test cases
-  - [ ] Some more standardization b/t openai and huggingface tests
-  - [x] Add code coverage badge to look cool
   - [ ] Test input checks
+  - [ ] Test `cappr.openai.api`
+- [ ] Factor out the discount feature in `cappr.openai.classify.predict_proba` into
+`cappr.utils.classify._predict_proba`
 - [x] Small CPU speed-ups
   - [x] For constant-completions input, vectorize `agg_log_probs`
   - [x] For `examples` input, if # completions per prompt is constant, vectorize
   `posterior_prob`
 - [ ] Make progress bars optional, since inference often isn't batched
 - [ ] Factor out input checks (on prompts and completions)
 - [x] De-automate overzealous auto-docstring stuff :-(
 - [ ] HuggingFace `transformers.AutoModelForCausalLM`
+  - [ ] Support as many of them as possible, regardless of way positions are encoded
   - [x] Optimize backend to enable greater scaling wrt # completions/classes
-  - [x] Get it working on single-GPU, check that it's faster than sampling assuming
-  batching
+  - [x] Get it working on GPU, check that it's faster than sampling
     - [ ] Get to the bottom of why it's slower w/o batching
   - [ ] Allow non-`' '` `end_of_prompt`! I'll have to go back to the drawing board I
   think
-  - [ ] Consider batchifying the completions again, since they technically don't go in
-  batches of `batch_size`; the actual batch size is the sum of the number of completions
-  corresponding to the batch of prompts! Not a huge memory issue I think b/c completions
-  are usually half as long. But it should be configurable at the very least.
   - [ ] Factor out repeated code b/t `classify` and `classify_no_cache`
   - [ ] Support [Inference
     Endpoints](https://huggingface.co/docs/inference-endpoints/index)?
-  - [ ] Support TensorFlow models if it's easy
+  - [ ] Support TensorFlow models
   - [ ] Support priming, as in: cache it
 - [x] (for me) Auto-enforced code formatting b/c it's getting time-consuming
 - [ ] Allow for multi-label classification
   - [ ] Pass `normalize` as an argument to predict_proba functions
   - [ ] For `huggingface`, add note that you'll get faster results by passing all
   labels at once (assuming prompt is identical for each label)
-- [ ] Create a notebook template
 - [ ] Fill in missing or non-numpy docstrings
 </details>
 
 <details>
 <summary>Research</summary>
 
 Evaluate on more datasets, and understand its relative advantages and disadvantages vs
 other classification methods.
 
-- [ ] RAFT benchmark (**)
+- [ ] RAFT benchmark
   - [x] Zero-shot training scores
   - [ ] Submit zero-shot test predictions
   - [ ] Few-shot (priming) training scores
   - [ ] Submit few-shot test predictions
 - [ ] Create a user guide, build a table of results comparing competing approaches on
 statistical performance, cost, and computation
-- [ ] Make a computational comparison to sampling (**)
-  - [x] Assume I have full freedom to decide how inference works. Demo w/
-  GPT-2. Process inputs in batches.
+- [ ] Make a computational comparison to sampling
+  - [x] Assume I have full freedom to decide how inference works. Demo w/ GPT-2. Process
+  inputs in batches.
   - [ ] Process inputs 1-by-1
 - [ ] More SuperGLUE tasks?
-  - [ ] Re-run COPA demo w/ left-stripped completions (there are a few which aren't)
 - [ ] Calibration
   - [ ] Is the prior actually effective? Downsample and see
   - [ ] curves
-- [ ] Compare against few-shot embeddings
 - [ ] Finetune smaller, cheaper model and compare against zero-shot w/ davinci
   - [ ] e.g., GPT-2 from huggingface, `text-ada-001`
   - [ ] Again, compare against sampling
 - [ ] Evaluate a bigger model like GPT-J
-- [ ] Evaluate different aggregation functions. Currently taking mean, but
-there was no good theory for that
-- [ ] A bit ambitious: support insertion and backwards-completion. Quite ambitious b/c
-manipulating position IDs isn't sufficient (I think).
 </details>
```

### Comparing `cappr-0.2.5/README.md` & `cappr-0.2.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: cappr
+Version: 0.2.6
+Summary: Zero-shot text classification using autoregressive language models.
+Home-page: https://github.com/kddubey/cappr/
+Author-email: kushdubey63@gmail.com
+License: Apache License 2.0
+Requires-Python: >=3.8.0
+Description-Content-Type: text/markdown
+Provides-Extra: hf
+Provides-Extra: demos
+Provides-Extra: dev
+License-File: LICENSE
+
 # CAPPr: zero-shot text classification using autoregressive language models
 
 [![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-380/)
 [![Documentation Status](https://readthedocs.org/projects/cappr/badge/?version=latest)](https://cappr.readthedocs.io/en/latest/?badge=latest)
 [![tests](https://github.com/kddubey/cappr/actions/workflows/test.yml/badge.svg)](https://github.com/kddubey/cappr/actions/workflows/test.yml)
 [![codecov](https://codecov.io/gh/kddubey/cappr/branch/main/graph/badge.svg?token=NYIL076PSM)](https://codecov.io/gh/kddubey/cappr)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
@@ -12,15 +26,15 @@
 completion comes after an inputted prompt. Hence the name:
 
 > **C**ompletion<br>
   **A**fter<br>
   **P**rompt<br>
   **Pr**obability<br>
 
-The method is fleshed out in my [question on CrossValidated](https://stats.stackexchange.com/q/601159/337906).
+The method is fleshed out in my [question on Cross Validated](https://stats.stackexchange.com/q/601159/337906).
 
 
 ## Usage
 
 <details>
 <summary>Use a model from the OpenAI API</summary>
 
@@ -51,42 +65,47 @@
 ```
 </details>
 
 <details>
 <summary>Use a model from the HuggingFace model hub</summary>
 
 Specifically, this model must be able to be loaded using
-`transformers.AutoModelForCausalLM.from_pretrained(model)`.
-
-Smaller LMs may not work well. But there will likely be better ones in the hub soon.
+`transformers.AutoModelForCausalLM.from_pretrained`.
 
 ```python
+from transformers import AutoModelForCausalLM, AutoTokenizer
 from cappr.huggingface.classify import predict
 
 prompt = 'Which planet is closer to the Sun: Mercury or Earth?'
 
 class_names = ('Mercury', 'Earth')
 prior = None  # uniform prior
 
+# load model and tokenizer
+model_name = 'gpt2'
+model = AutoModelForCausalLM.from_pretrained(model_name)
+tokenizer = AutoTokenizer.from_pretrained(model_name)
+
 preds = predict(prompts=[prompt],
                 completions=class_names,
-                model='gpt2',
+                model_and_tokenizer=(model, tokenizer),
                 prior=prior)
 preds
 # ['Mercury']
 ```
 </details>
 
 <details>
 <summary>Run in batches</summary>
 
 Let's use `huggingface` for this example cuz it's free. And let's predict probabilities
 instead of the class.
 
 ```python
+from transformers import AutoModelForCausalLM, AutoTokenizer
 from cappr.huggingface.classify import predict_proba
 
 prompts = [
     'Stephen Curry is a',
     'Martina Navratilova was a',
     "Dexter, from the TV Series Dexter's Laboratory, is a",
     'LeBron James is a',    
@@ -101,17 +120,23 @@
 
 prior = (
     1/6,  # few
     1/6,  # few
     2/3   # there are more
 )
 
+
+# load model and tokenizer
+model_name = 'gpt2'
+model = AutoModelForCausalLM.from_pretrained(model_name)
+tokenizer = AutoTokenizer.from_pretrained(model_name)
+
 pred_probs = predict_proba(prompts=prompts,
                            completions=class_names,
-                           model='gpt2',
+                           model_and_tokenizer=(model, tokenizer),
                            batch_size=32,  # whatever fits on your CPU/GPU
                            prior=prior)
 
 # pred_probs[i,j] = probability that prompts[i] is classified as class_names[j]
 print(pred_probs.round(1))
 # [[0.5 0.3 0.2]
 #  [0.3 0.6 0.2]
@@ -128,17 +153,15 @@
 ```
 </details>
 
 <details>
 <summary>Run in batches, where each prompt has a different set of possible completions
 </summary>
 
-Again, let's use `huggingface` to predict probabilities. And this time, let's pass in an 
-instantiated model and tokenizer instead of its name. That way, the model isn't
-re-loaded every time you wanna use it.
+Again, let's use `huggingface` to predict probabilities.
 
 ```python
 import numpy as np
 from transformers import AutoModelForCausalLM, AutoTokenizer
 
 from cappr import Example
 from cappr.huggingface.classify import predict_proba_examples
@@ -180,18 +203,15 @@
 See
 [`demos/superglue/copa.ipynb`](https://github.com/kddubey/cappr/blob/main/demos/superglue/copa.ipynb)
 for a demonstration of a slightly harder classification task.
 
 
 ## Documentation
 
-https://cappr.readthedocs.io/en/latest/
-
-Please let me know if you find the writing too dense. The main motivation behind this
-project is simplicity :-)
+https://cappr.readthedocs.io
 
 
 ## Setup
 
 If you intend on using OpenAI models, [sign up for the OpenAI API
 here](https://platform.openai.com/signup), and then set the environment variable
 `OPENAI_API_KEY`. For zero-shot classification, OpenAI models are currently far ahead of
@@ -199,43 +219,39 @@
 
 Install with `pip`:
 
 ```
 python -m pip install cappr
 ```
 
-<details>
-<summary>(Optional) Install requirements for HuggingFace models</summary>
+(Optional) Install requirements for HuggingFace models
 
 ```
 python -m pip install cappr[hf]
 ```
-</details>
 
-<details>
-<summary>(Optional) Install requirements for running demos</summary>
+(Optional) Install requirements for running demos
 
 ```
 python -m pip install cappr[demos]
 ```
-</details>
 
 
 ## Motivation
 
 Create a more usable zero-shot text classification interface than
 [classification via sampling (CVS)](https://platform.openai.com/docs/guides/completion/classification).
 
 <details>
 <summary>Short</summary>
 
-In CVS, your job is to write up your classification task in a `prompt` string, and then
-write custom code to post-process arbitrary `completion`/output strings.
+With CVS, your job is to write up your classification task in a `prompt` string, and
+then write custom code to post-process arbitrary `completion`/output strings.
 
-In CAPPr, your job starts and stops at writing up your classification task as a
+With CAPPr, your job starts and stops at writing up your classification task as a
 `{prompt}{end_of_prompt}{completion}` string.
 </details>
 
 <details>
 <summary>Long</summary>
 
 Please see [this page of the
@@ -291,20 +307,20 @@
 you'll be on the *cappr (slow)* line** :-(
 
 ![](/docs/source/_static/scaling_classes/batch_size_32.png)
 
 *Figure 1: [COPA](https://people.ict.usc.edu/~gordon/copa.html) dataset, repeating the
 choices to simulate multi-class classification tasks. [GPT-2
 (small)](https://huggingface.co/gpt2) was run on a Tesla K80 GPU (whatever was free in
-Google Colab in March 2023, I'm not hardware savvy). 96 classification inputs were
-processed in batches of size 32. Each point in the graph is a median of 5 runs. For
-classification via sampling (CVS), exactly 4 tokens were generated for each prompt,
-which is the number of tokens in `'\n\nAnswer A'`. 1-token times are also shown. But for
-COPA (and other multiple-choice style prompts), that may result in lower zero-shot
-accuracy, as most of the sampled choices come after the first token.*
+Google Colab in March 2023). 96 classification inputs were processed in batches of size
+32. Each point in the graph is a median of 5 runs. For classification via sampling
+(CVS), exactly 4 tokens were generated for each prompt, which is the number of tokens in
+`'\n\nAnswer A'`. 1-token times are also shown. But for COPA (and other multiple-choice
+style prompts), that may result in lower zero-shot accuracy, as most of the sampled
+choices come after the first token.*
 
 See the [`demos/computational_analysis.ipynb`
 notebook](https://github.com/kddubey/cappr/blob/main/demos/computational_analysis.ipynb).
 
 </details>
 
 
@@ -370,74 +386,64 @@
 (**) = I'm currently working on this or will work on it really soon
 
 <details>
 <summary>Code</summary>
 
 - [ ] Testing
   - [ ] Increase test cases
-  - [ ] Some more standardization b/t openai and huggingface tests
-  - [x] Add code coverage badge to look cool
   - [ ] Test input checks
+  - [ ] Test `cappr.openai.api`
+- [ ] Factor out the discount feature in `cappr.openai.classify.predict_proba` into
+`cappr.utils.classify._predict_proba`
 - [x] Small CPU speed-ups
   - [x] For constant-completions input, vectorize `agg_log_probs`
   - [x] For `examples` input, if # completions per prompt is constant, vectorize
   `posterior_prob`
 - [ ] Make progress bars optional, since inference often isn't batched
 - [ ] Factor out input checks (on prompts and completions)
 - [x] De-automate overzealous auto-docstring stuff :-(
 - [ ] HuggingFace `transformers.AutoModelForCausalLM`
+  - [ ] Support as many of them as possible, regardless of way positions are encoded
   - [x] Optimize backend to enable greater scaling wrt # completions/classes
-  - [x] Get it working on single-GPU, check that it's faster than sampling assuming
-  batching
+  - [x] Get it working on GPU, check that it's faster than sampling
     - [ ] Get to the bottom of why it's slower w/o batching
   - [ ] Allow non-`' '` `end_of_prompt`! I'll have to go back to the drawing board I
   think
-  - [ ] Consider batchifying the completions again, since they technically don't go in
-  batches of `batch_size`; the actual batch size is the sum of the number of completions
-  corresponding to the batch of prompts! Not a huge memory issue I think b/c completions
-  are usually half as long. But it should be configurable at the very least.
   - [ ] Factor out repeated code b/t `classify` and `classify_no_cache`
   - [ ] Support [Inference
     Endpoints](https://huggingface.co/docs/inference-endpoints/index)?
-  - [ ] Support TensorFlow models if it's easy
+  - [ ] Support TensorFlow models
   - [ ] Support priming, as in: cache it
 - [x] (for me) Auto-enforced code formatting b/c it's getting time-consuming
 - [ ] Allow for multi-label classification
   - [ ] Pass `normalize` as an argument to predict_proba functions
   - [ ] For `huggingface`, add note that you'll get faster results by passing all
   labels at once (assuming prompt is identical for each label)
-- [ ] Create a notebook template
 - [ ] Fill in missing or non-numpy docstrings
 </details>
 
 <details>
 <summary>Research</summary>
 
 Evaluate on more datasets, and understand its relative advantages and disadvantages vs
 other classification methods.
 
-- [ ] RAFT benchmark (**)
+- [ ] RAFT benchmark
   - [x] Zero-shot training scores
   - [ ] Submit zero-shot test predictions
   - [ ] Few-shot (priming) training scores
   - [ ] Submit few-shot test predictions
 - [ ] Create a user guide, build a table of results comparing competing approaches on
 statistical performance, cost, and computation
-- [ ] Make a computational comparison to sampling (**)
-  - [x] Assume I have full freedom to decide how inference works. Demo w/
-  GPT-2. Process inputs in batches.
+- [ ] Make a computational comparison to sampling
+  - [x] Assume I have full freedom to decide how inference works. Demo w/ GPT-2. Process
+  inputs in batches.
   - [ ] Process inputs 1-by-1
 - [ ] More SuperGLUE tasks?
-  - [ ] Re-run COPA demo w/ left-stripped completions (there are a few which aren't)
 - [ ] Calibration
   - [ ] Is the prior actually effective? Downsample and see
   - [ ] curves
-- [ ] Compare against few-shot embeddings
 - [ ] Finetune smaller, cheaper model and compare against zero-shot w/ davinci
   - [ ] e.g., GPT-2 from huggingface, `text-ada-001`
   - [ ] Again, compare against sampling
 - [ ] Evaluate a bigger model like GPT-J
-- [ ] Evaluate different aggregation functions. Currently taking mean, but
-there was no good theory for that
-- [ ] A bit ambitious: support insertion and backwards-completion. Quite ambitious b/c
-manipulating position IDs isn't sufficient (I think).
 </details>
```

### Comparing `cappr-0.2.5/demos/computational_analysis.ipynb` & `cappr-0.2.6/demos/computational_analysis.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.5/demos/politeness.ipynb` & `cappr-0.2.6/demos/politeness.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.5/demos/raft/README.md` & `cappr-0.2.6/demos/raft/README.md`

 * *Files identical despite different names*

### Comparing `cappr-0.2.5/demos/raft/ade.ipynb` & `cappr-0.2.6/demos/raft/ade.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.5/demos/raft/b77.ipynb` & `cappr-0.2.6/demos/raft/b77.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.5/demos/raft/nis.ipynb` & `cappr-0.2.6/demos/raft/nis.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.5/demos/raft/ose.ipynb` & `cappr-0.2.6/demos/raft/ose.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.5/demos/raft/over.ipynb` & `cappr-0.2.6/demos/raft/over.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.5/demos/raft/sot.ipynb` & `cappr-0.2.6/demos/raft/sot.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.5/demos/raft/sri.ipynb` & `cappr-0.2.6/demos/raft/sri.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.5/demos/raft/tai.ipynb` & `cappr-0.2.6/demos/raft/tai.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.5/demos/raft/tc.ipynb` & `cappr-0.2.6/demos/raft/tc.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.5/demos/raft/teh.ipynb` & `cappr-0.2.6/demos/raft/teh.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.5/demos/raft/tos.ipynb` & `cappr-0.2.6/demos/raft/tos.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.5/demos/superglue/copa.ipynb` & `cappr-0.2.6/demos/superglue/copa.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.5/demos/superglue/wsc.ipynb` & `cappr-0.2.6/demos/superglue/wsc.ipynb`

 * *Files identical despite different names*

### Comparing `cappr-0.2.5/demos/utils.py` & `cappr-0.2.6/demos/utils.py`

 * *Files identical despite different names*

### Comparing `cappr-0.2.5/docs/Makefile` & `cappr-0.2.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cappr-0.2.5/docs/make.bat` & `cappr-0.2.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cappr-0.2.5/docs/source/1_is_for_me.rst` & `cappr-0.2.6/docs/source/1_is_for_me.rst`

 * *Files identical despite different names*

### Comparing `cappr-0.2.5/docs/source/2_motivation.rst` & `cappr-0.2.6/docs/source/2_motivation.rst`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ==========
 
 Why does this package exist? The short answer is to create a more usable zero-shot text
 classification interface than `classification via sampling`_.
 
 .. _classification via sampling: https://platform.openai.com/docs/guides/completion/classification
 
-Now for a longer answer, which takes a deep dive into what's meant by *usable*.
+Now for a longer answer, which expands on what's meant by *usable*.
 
 
 Problem
 -------
 
 There are many ways to do zero-shot text classification. The one that this package is
 competing against is what I'll call **classification via sampling (CVS)**. This method
@@ -52,27 +52,26 @@
                                       max_tokens=10,
                                       temperature=0)
    completion = api_resp[0]['text']
    completion
    # '\nThe product is difficult to use'
    # correct!
 
-This usually works well. But if you've ever run CVS on a slightly larger scale, then
-you'll know that there are a considerable fraction of cases where the ``completion`` is
-not actually in ``class_names``. To address these cases, you add:
+This usually works well. But if you've ever run CVS on a slightly larger scale, then you
+know that there may be a considerable fraction of cases where the ``completion`` is not
+actually in ``class_names``. To address these cases, you add:
 
 .. code:: python
 
    if completion not in class_names:
        completion = post_process(completion)
 
    assert completion in class_names
 
-Herein lies the problem. Because if you've made it this far, then I'm sure you know that
-implementing ``post_process`` can be challenging, as the ``completion`` is sampled from
+Implementing ``post_process`` can be challenging, as the ``completion`` is sampled from
 the space of all possible sequences of tokens. This means you'll likely have to deal
 with the cases where:
 
 - The ``completion`` includes multiple plausible classes from ``class_names``
 
 - The ``completion`` includes a bit of fluff
 
@@ -104,16 +103,15 @@
 
 Solution
 --------
 
 With CAPPr's ``predict`` interface, your job starts and stops at writing up your
 classification task as a ``{prompt}{end_of_prompt}{completion}`` string.
 
-That being said, let's now run CAPPr on that product review classification task. Also,
-let's:
+Let's now run CAPPr on that product review classification task. Also, let's:
 
 - trivially incorporate a prior (optional)
 
 - predict a probability distribution over classes (optional)
 
 - replace the expensive ``text-davinci-003`` model call with a ``text-curie-001`` one
```

### Comparing `cappr-0.2.5/docs/source/3_installation.rst` & `cappr-0.2.6/docs/source/3_installation.rst`

 * *Files identical despite different names*

### Comparing `cappr-0.2.5/docs/source/4_user_guide.rst` & `cappr-0.2.6/docs/source/4_user_guide.rst`

 * *Files identical despite different names*

### Comparing `cappr-0.2.5/docs/source/6_computational_performance.rst` & `cappr-0.2.6/docs/source/6_computational_performance.rst`

 * *Files 10% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 .. _this code: https://github.com/kddubey/cappr/blob/main/src/cappr/huggingface/classify.py
 
 .. figure:: _static/scaling_classes/batch_size_32.png
    :align: center
 
    `COPA`_ dataset, repeating the choices to simulate multi-class classification tasks.
    `GPT-2 (small)`_ was run on a Tesla K80 GPU (whatever was free in Google Colab in
-   March 2023, I'm not hardware savvy). 96 classification inputs were processed in
-   batches of size 32. Each point in the graph is a median of 5 runs. For classification
-   via sampling (CVS), exactly 4 tokens were generated for each prompt, which is the
-   number of tokens in ``'\n\nAnswer A'``. 1-token times are also shown. But for COPA
-   (and other multiple-choice style prompts), that may result in lower zero-shot
-   accuracy, as most of the sampled choices come after the first token.
+   March 2023). 96 classification inputs were processed in batches of size 32. Each
+   point in the graph is a median of 5 runs. For classification via sampling (CVS),
+   exactly 4 tokens were generated for each prompt, which is the number of tokens in
+   ``'\n\nAnswer A'``. 1-token times are also shown. But for COPA (and other
+   multiple-choice style prompts), that may result in lower zero-shot accuracy, as most
+   of the sampled choices come after the first token.
 
 .. _COPA: https://people.ict.usc.edu/~gordon/copa.html
 
 .. _GPT-2 (small): https://huggingface.co/gpt2
 
 See the `this notebook`_ for the experiment code which produced the figure above.
```

### Comparing `cappr-0.2.5/docs/source/7_future_research.rst` & `cappr-0.2.6/docs/source/7_future_research.rst`

 * *Files identical despite different names*

### Comparing `cappr-0.2.5/docs/source/_static/github-mark.png` & `cappr-0.2.6/docs/source/_static/github-mark.png`

 * *Files identical despite different names*

### Comparing `cappr-0.2.5/docs/source/_static/scaling_classes/batch_size_32.png` & `cappr-0.2.6/docs/source/_static/scaling_classes/batch_size_32.png`

 * *Files identical despite different names*

### Comparing `cappr-0.2.5/docs/source/conf.py` & `cappr-0.2.6/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `cappr-0.2.5/docs/source/index.rst` & `cappr-0.2.6/docs/source/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Welcome to CAPPr's documentation
+CAPPr Docs
 ================================
 
 |gittycat| `GitHub <https://github.com/kddubey/cappr>`_
 
 .. |gittycat| image:: _static/github-mark.png
               :scale: 10%
```

### Comparing `cappr-0.2.5/docs/source/related_work.rst` & `cappr-0.2.6/docs/source/related_work.rst`

 * *Files identical despite different names*

### Comparing `cappr-0.2.5/setup.py` & `cappr-0.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `cappr-0.2.5/src/cappr/_example.py` & `cappr-0.2.6/src/cappr/_example.py`

 * *Files identical despite different names*

### Comparing `cappr-0.2.5/src/cappr/huggingface/classify.py` & `cappr-0.2.6/src/cappr/huggingface/classify.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 In the implementation, attention block keys and values for prompts are cached and shared
 across completions. See the computational performance `here`_.
 
 .. _here: https://cappr.readthedocs.io/en/latest/6_computational_performance.html
 
 You probably just want the :func:`predict` or :func:`predict_examples` functions :-)
 
-.. warning:: This module currently requires that ``end_of_prompt`` is a whitespace.
-
 .. warning:: This module doesn't work with ``transformers.BartForCausalLM``, among
              others probably.
 """
 from __future__ import annotations
 from typing import Mapping, Optional, Sequence, Union
 
 import numpy as np
@@ -379,40 +377,31 @@
         )
     ]
 
 
 def log_probs_conditional(
     prompts: Sequence[str],
     completions: Sequence[str],
-    model: str = None,
-    model_and_tokenizer: tuple[AutoModelForCausalLM, PreTrainedTokenizer] = None,
+    model_and_tokenizer: tuple[AutoModelForCausalLM, PreTrainedTokenizer],
     end_of_prompt: str = " ",
     batch_size: int = 32,
 ) -> list[list[list[float]]]:
     """
     Log-probabilities of each completion token conditional on each prompt and previous
     completion tokens.
 
-    Note
-    ----
-    Either `model` or `model_and_tokenizer` must be inputted. It's usually better to
-    instantiate/pre-load a model and tokenizer and pass them to `model_and_tokenizer`.
-    See the Example.
-
     Parameters
     ----------
     prompts : Sequence[str]
         strings, where, e.g., each contains the text you want to classify
     completions : Sequence[str]
         strings, where, e.g., each one is the name of a class which could come after a
         prompt
-    model : str, optional
-        the name of an `AutoModelForCausalLM`, by default None
-    model_and_tokenizer : tuple[AutoModelForCausalLM, PreTrainedTokenizer], optional
-        an instantiated model and its corresponding tokenizer, by default None
+    model_and_tokenizer : tuple[AutoModelForCausalLM, PreTrainedTokenizer]
+        an instantiated model and its corresponding tokenizer
     end_of_prompt : str, optional
         the string to tack on at the end of every prompt, by default " "
     batch_size : int, optional
         the maximum number of inputs that the model will process in parallel, by default
         32
 
     Returns
@@ -455,19 +444,17 @@
 
         log_probs_completions[0]
         # [[-4.5],        [[log Pr(z | x, y)],
         #  [-5.6, -3.2]]   [log Pr(d | x, y),    log Pr(e | x, y, d)]]
 
         log_probs_completions[1]
         # [[-9.7],        [[log Pr(z | a, b, c)],
-        #  [-0.2, -0.03]]  [log Pr(d | a, b, c), log Pr(e | a, b, c)]]
+        #  [-0.2, -0.03]]  [log Pr(d | a, b, c), log Pr(e | a, b, c, d)]]
     """
-    model, tokenizer = hf._utils.load_model_and_tokenizer(
-        model=model, model_and_tokenizer=model_and_tokenizer
-    )
+    model, tokenizer = hf._utils.load_model_and_tokenizer(model_and_tokenizer)
 
     @_batch.flatten
     @_batch.batchify(batchable_arg="prompts", progress_bar_desc="log-probs")
     def log_probs_completions_batch(prompts, batch_size=batch_size):
         logits, encodings = _logits_completions_given_prompts(
             model, tokenizer, prompts, completions, end_of_prompt=end_of_prompt
         )
@@ -475,37 +462,28 @@
 
     log_probs_completions = log_probs_completions_batch(prompts)
     return list(_batch.constant(log_probs_completions, size=len(completions)))
 
 
 def log_probs_conditional_examples(
     examples: Sequence[Example],
-    model: str = None,
-    model_and_tokenizer: tuple[AutoModelForCausalLM, PreTrainedTokenizer] = None,
+    model_and_tokenizer: tuple[AutoModelForCausalLM, PreTrainedTokenizer],
     batch_size: int = 32,
 ) -> list[list[list[float]]]:
     """
     Log-probabilities of each completion token conditional on each prompt and previous
     completion tokens.
 
-    Note
-    ----
-    Either `model` or `model_and_tokenizer` must be inputted. It's usually better to
-    instantiate/pre-load a model and tokenizer and pass them to `model_and_tokenizer`.
-    See the Example.
-
     Parameters
     ----------
     examples : Sequence[Example]
         `Example` objects, where each contains a prompt and its set of possible
         completions
-    model : str, optional
-        the name of an `AutoModelForCausalLM`, by default None
-    model_and_tokenizer : tuple[AutoModelForCausalLM, PreTrainedTokenizer], optional
-        an instantiated model and its corresponding tokenizer, by default None
+    model_and_tokenizer : tuple[AutoModelForCausalLM, PreTrainedTokenizer]
+        an instantiated model and its corresponding tokenizer
     batch_size : int, optional
         the maximum number of inputs that the model will process in parallel, by default
         32
 
     Returns
     -------
     log_probs_completions : list[list[list[float]]]
@@ -552,17 +530,15 @@
         log_probs_completions[0] # corresponds to examples[0]
         # [[-4.5],        [[log Pr(z | x, y)],
         #  [-5.6, -3.2]]   [log Pr(d | x, y),    log Pr(e | x, y, d)]]
 
         log_probs_completions[1] # corresponds to examples[1]
         # [[-5.0, -1.7]]  [[log Pr(1 | a, b, c)], log Pr(2 | a, b, c, 1)]]
     """
-    model, tokenizer = hf._utils.load_model_and_tokenizer(
-        model=model, model_and_tokenizer=model_and_tokenizer
-    )
+    model, tokenizer = hf._utils.load_model_and_tokenizer(model_and_tokenizer)
 
     @_batch.flatten
     @_batch.batchify(batchable_arg="examples", progress_bar_desc="log-probs")
     def log_probs_completions_batch(examples, batch_size=batch_size):
         logits, encodings = _logits_completions_given_prompts_examples(
             model, tokenizer, examples
         )
@@ -575,40 +551,31 @@
     )
 
 
 @classify._predict_proba
 def predict_proba(
     prompts: Sequence[str],
     completions: Sequence[str],
-    model: str = None,
-    model_and_tokenizer: tuple[AutoModelForCausalLM, PreTrainedTokenizer] = None,
+    model_and_tokenizer: tuple[AutoModelForCausalLM, PreTrainedTokenizer],
     prior: Optional[Sequence[float]] = None,
     end_of_prompt: str = " ",
     batch_size: int = 32,
 ) -> npt.NDArray[np.floating]:
     """
     Predict probabilities of each completion coming after each prompt.
 
-    Note
-    ----
-    Either `model` or `model_and_tokenizer` must be inputted. It's usually better to
-    instantiate/pre-load a model and tokenizer and pass them to `model_and_tokenizer`.
-    See the Example.
-
     Parameters
     ----------
     prompts : Sequence[str]
         strings, where, e.g., each contains the text you want to classify
     completions : Sequence[str]
         strings, where, e.g., each one is the name of a class which could come after a
         prompt
-    model : str, optional
-        the name of an `AutoModelForCausalLM`, by default None
-    model_and_tokenizer : tuple[AutoModelForCausalLM, PreTrainedTokenizer], optional
-        an instantiated model and its corresponding tokenizer, by default None
+    model_and_tokenizer : tuple[AutoModelForCausalLM, PreTrainedTokenizer]
+        an instantiated model and its corresponding tokenizer
     prior : Sequence[float], optional
         a probability distribution over `completions`, representing a belief about their
         likelihoods regardless of the prompt. By default, each completion in
         `completions` is assumed to be equally likely
     end_of_prompt : str, optional
         the string to tack on at the end of every prompt, by default " "
     batch_size : int, optional
@@ -666,59 +633,49 @@
         # predicted probability that ice cream is in the fridge
         pred_probs[1,2]
         # 0.4
     """
     return log_probs_conditional(
         prompts,
         completions,
-        model=model,
-        model_and_tokenizer=model_and_tokenizer,
+        model_and_tokenizer,
         end_of_prompt=end_of_prompt,
         batch_size=batch_size,
     )
 
 
 @classify._predict_proba_examples
 def predict_proba_examples(
     examples: Sequence[Example],
-    model: str = None,
-    model_and_tokenizer: tuple[AutoModelForCausalLM, PreTrainedTokenizer] = None,
+    model_and_tokenizer: tuple[AutoModelForCausalLM, PreTrainedTokenizer],
     batch_size: int = 32,
-) -> Union[list[list[float]], npt.NDArray[np.floating]]:
+) -> Union[list[npt.NDArray[np.floating]], npt.NDArray[np.floating]]:
     """
     Predict probabilities of each completion coming after each prompt.
 
-    Note
-    ----
-    Either `model` or `model_and_tokenizer` must be inputted. It's usually better to
-    instantiate/pre-load a model and tokenizer and pass them to `model_and_tokenizer`.
-    See the Example.
-
     Parameters
     ----------
     examples : Sequence[Example]
         `Example` objects, where each contains a prompt and its set of possible
         completions
-    model : str, optional
-        the name of an `AutoModelForCausalLM`, by default None
-    model_and_tokenizer : tuple[AutoModelForCausalLM, PreTrainedTokenizer], optional
-        an instantiated model and its corresponding tokenizer, by default None
+    model_and_tokenizer : tuple[AutoModelForCausalLM, PreTrainedTokenizer]
+        an instantiated model and its corresponding tokenizer
     batch_size : int, optional
         the maximum number of inputs that the model will process in parallel, by default
         32
 
     Returns
     -------
-    pred_probs : list[list[float]] | npt.NDArray[np.floating]
+    pred_probs : list[npt.NDArray[np.floating]] | npt.NDArray[np.floating]
         `pred_probs[example_idx][completion_idx]` is the model's estimate of the
         probability that `examples[example_idx].completions[completion_idx]` comes after
         `examples[example_idx].prompt + examples[example_idx].end_of_prompt`.
 
         If the number of completions per example is a constant `k`, then an array with
-        shape `(len(examples), k)` is returned instead of a nested/2-D list.
+        shape `(len(examples), k)` is returned instead of a list of 1-D arrays.
 
     Example
     -------
     GPT-2 (small) doing media trivia::
 
         from transformers import AutoModelForCausalLM, AutoTokenizer
         from cappr import Example
@@ -746,50 +703,40 @@
 
         # predicted probability that Batman was played by Kevin Conroy
         pred_probs[0][1]
         # 0.97
     """
     return log_probs_conditional_examples(
         examples,
-        model=model,
-        model_and_tokenizer=model_and_tokenizer,
+        model_and_tokenizer,
         batch_size=batch_size,
     )
 
 
 @classify._predict
 def predict(
     prompts: Sequence[str],
     completions: Sequence[str],
-    model: str = None,
-    model_and_tokenizer: tuple[AutoModelForCausalLM, PreTrainedTokenizer] = None,
+    model_and_tokenizer: tuple[AutoModelForCausalLM, PreTrainedTokenizer],
     prior: Optional[Sequence[float]] = None,
     end_of_prompt: str = " ",
     batch_size: int = 32,
 ) -> list[str]:
     """
     Predict which completion is most likely to follow each prompt.
 
-    Note
-    ----
-    Either `model` or `model_and_tokenizer` must be inputted. It's usually better to
-    instantiate/pre-load a model and tokenizer and pass them to `model_and_tokenizer`.
-    See the Example.
-
     Parameters
     ----------
     prompts : Sequence[str]
         strings, where, e.g., each contains the text you want to classify
     completions : Sequence[str]
         strings, where, e.g., each one is the name of a class which could come after a
         prompt
-    model : str, optional
-        the name of an `AutoModelForCausalLM`, by default None
-    model_and_tokenizer : tuple[AutoModelForCausalLM, PreTrainedTokenizer], optional
-        an instantiated model and its corresponding tokenizer, by default None
+    model_and_tokenizer : tuple[AutoModelForCausalLM, PreTrainedTokenizer]
+        an instantiated model and its corresponding tokenizer
     prior : Sequence[float], optional
         a probability distribution over `completions`, representing a belief about their
         likelihoods regardless of the prompt. By default, each completion in
         `completions` is assumed to be equally likely
     end_of_prompt : str, optional
         the string to tack on at the end of every prompt, by default " "
     batch_size : int, optional
@@ -833,47 +780,37 @@
         preds
         # ['on the stove',
         #  'in the freezer']
     """
     return predict_proba(
         prompts,
         completions,
-        model=model,
-        model_and_tokenizer=model_and_tokenizer,
+        model_and_tokenizer,
         prior=prior,
         end_of_prompt=end_of_prompt,
         batch_size=batch_size,
     )
 
 
 @classify._predict_examples
 def predict_examples(
     examples: Sequence[Example],
-    model: str = None,
-    model_and_tokenizer: tuple[AutoModelForCausalLM, PreTrainedTokenizer] = None,
+    model_and_tokenizer: tuple[AutoModelForCausalLM, PreTrainedTokenizer],
     batch_size: int = 32,
 ) -> list[str]:
     """
     Predict which completion is most likely to follow each prompt.
 
-    Note
-    ----
-    Either `model` or `model_and_tokenizer` must be inputted. It's usually better to
-    instantiate/pre-load a model and tokenizer and pass them to `model_and_tokenizer`.
-    See the Example.
-
     Parameters
     ----------
     examples : Sequence[Example]
         `Example` objects, where each contains a prompt and its set of possible
         completions
-    model : str, optional
-        the name of an `AutoModelForCausalLM`, by default None
-    model_and_tokenizer : tuple[AutoModelForCausalLM, PreTrainedTokenizer], optional
-        an instantiated model and its corresponding tokenizer, by default None
+    model_and_tokenizer : tuple[AutoModelForCausalLM, PreTrainedTokenizer]
+        an instantiated model and its corresponding tokenizer
     batch_size : int, optional
         the maximum number of inputs that the model will process in parallel, by default
         32
 
     Returns
     -------
     preds : list[str]
@@ -906,11 +843,10 @@
         preds = predict_examples(examples, model_and_tokenizer=(model, tokenizer))
         preds
         # ['Clarice Starling',
         #  'Kevin Conroy']
     """
     return predict_proba_examples(
         examples,
-        model=model,
-        model_and_tokenizer=model_and_tokenizer,
+        model_and_tokenizer,
         batch_size=batch_size,
     )
```

### Comparing `cappr-0.2.5/src/cappr/huggingface/classify_no_cache.py` & `cappr-0.2.6/src/cappr/huggingface/classify_no_cache.py`

 * *Files 8% similar despite different names*

```diff
@@ -214,40 +214,31 @@
         )
     ]
 
 
 def log_probs_conditional(
     prompts: Sequence[str],
     completions: Sequence[str],
-    model: str = None,
-    model_and_tokenizer: tuple[AutoModelForCausalLM, PreTrainedTokenizer] = None,
+    model_and_tokenizer: tuple[AutoModelForCausalLM, PreTrainedTokenizer],
     end_of_prompt: str = " ",
     batch_size: int = 32,
 ) -> list[list[list[float]]]:
     """
     Log-probabilities of each completion token conditional on each prompt and previous
     completion tokens.
 
-    Note
-    ----
-    Either `model` or `model_and_tokenizer` must be inputted. It's usually better to
-    instantiate/pre-load a model and tokenizer and pass them to `model_and_tokenizer`.
-    See the Example.
-
     Parameters
     ----------
     prompts : Sequence[str]
         strings, where, e.g., each contains the text you want to classify
     completions : Sequence[str]
         strings, where, e.g., each one is the name of a class which could come after a
         prompt
-    model : str, optional
-        the name of an `AutoModelForCausalLM`, by default None
-    model_and_tokenizer : tuple[AutoModelForCausalLM, PreTrainedTokenizer], optional
-        an instantiated model and its corresponding tokenizer, by default None
+    model_and_tokenizer : tuple[AutoModelForCausalLM, PreTrainedTokenizer]
+        an instantiated model and its corresponding tokenizer
     end_of_prompt : str, optional
         the string to tack on at the end of every prompt, by default " "
     batch_size : int, optional
         the maximum number of inputs that the model will process in parallel, by default
         32
 
     Returns
@@ -290,19 +281,17 @@
 
         log_probs_completions[0]
         # [[-4.5],        [[log Pr(z | x, y)],
         #  [-5.6, -3.2]]   [log Pr(d | x, y),    log Pr(e | x, y, d)]]
 
         log_probs_completions[1]
         # [[-9.7],        [[log Pr(z | a, b, c)],
-        #  [-0.2, -0.03]]  [log Pr(d | a, b, c), log Pr(e | a, b, c)]]
+        #  [-0.2, -0.03]]  [log Pr(d | a, b, c), log Pr(e | a, b, c, d)]]
     """
-    model, tokenizer = hf._utils.load_model_and_tokenizer(
-        model=model, model_and_tokenizer=model_and_tokenizer
-    )
+    model, tokenizer = hf._utils.load_model_and_tokenizer(model_and_tokenizer)
 
     @_batch.flatten
     @_batch.batchify(batchable_arg="prompts", progress_bar_desc="log-probs (no cache)")
     def log_probs_completions_batch(prompts, batch_size=batch_size):
         logits, encodings = _logits_completions_given_prompts(
             model, tokenizer, prompts, completions, end_of_prompt=end_of_prompt
         )
@@ -310,37 +299,28 @@
 
     log_probs_completions = log_probs_completions_batch(prompts)
     return list(_batch.constant(log_probs_completions, size=len(completions)))
 
 
 def log_probs_conditional_examples(
     examples: Sequence[Example],
-    model: str = None,
-    model_and_tokenizer: tuple[AutoModelForCausalLM, PreTrainedTokenizer] = None,
+    model_and_tokenizer: tuple[AutoModelForCausalLM, PreTrainedTokenizer],
     batch_size: int = 32,
 ) -> list[list[list[float]]]:
     """
     Log-probabilities of each completion token conditional on each prompt and previous
     completion tokens.
 
-    Note
-    ----
-    Either `model` or `model_and_tokenizer` must be inputted. It's usually better to
-    instantiate/pre-load a model and tokenizer and pass them to `model_and_tokenizer`.
-    See the Example.
-
     Parameters
     ----------
     examples : Sequence[Example]
         `Example` objects, where each contains a prompt and its set of possible
         completions
-    model : str, optional
-        the name of an `AutoModelForCausalLM`, by default None
-    model_and_tokenizer : tuple[AutoModelForCausalLM, PreTrainedTokenizer], optional
-        an instantiated model and its corresponding tokenizer, by default None
+    model_and_tokenizer : tuple[AutoModelForCausalLM, PreTrainedTokenizer]
+        an instantiated model and its corresponding tokenizer
     batch_size : int, optional
         the maximum number of inputs that the model will process in parallel, by default
         32
 
     Returns
     -------
     log_probs_completions : list[list[list[float]]]
@@ -387,17 +367,15 @@
         log_probs_completions[0] # corresponds to examples[0]
         # [[-4.5],        [[log Pr(z | x, y)],
         #  [-5.6, -3.2]]   [log Pr(d | x, y),    log Pr(e | x, y, d)]]
 
         log_probs_completions[1] # corresponds to examples[1]
         # [[-5.0, -1.7]]  [[log Pr(1 | a, b, c)], log Pr(2 | a, b, c, 1)]]
     """
-    model, tokenizer = hf._utils.load_model_and_tokenizer(
-        model=model, model_and_tokenizer=model_and_tokenizer
-    )
+    model, tokenizer = hf._utils.load_model_and_tokenizer(model_and_tokenizer)
 
     @_batch.flatten
     @_batch.batchify(batchable_arg="examples", progress_bar_desc="log-probs (no cache)")
     def log_probs_completions_batch(examples, batch_size=batch_size):
         logits, encodings = _logits_completions_given_prompts_examples(
             model, tokenizer, examples
         )
@@ -410,40 +388,31 @@
     )
 
 
 @classify._predict_proba
 def predict_proba(
     prompts: Sequence[str],
     completions: Sequence[str],
-    model: str = None,
-    model_and_tokenizer: tuple[AutoModelForCausalLM, PreTrainedTokenizer] = None,
+    model_and_tokenizer: tuple[AutoModelForCausalLM, PreTrainedTokenizer],
     prior: Optional[Sequence[float]] = None,
     end_of_prompt: str = " ",
     batch_size: int = 32,
 ) -> npt.NDArray[np.floating]:
     """
     Predict probabilities of each completion coming after each prompt.
 
-    Note
-    ----
-    Either `model` or `model_and_tokenizer` must be inputted. It's usually better to
-    instantiate/pre-load a model and tokenizer and pass them to `model_and_tokenizer`.
-    See the Example.
-
     Parameters
     ----------
     prompts : Sequence[str]
         strings, where, e.g., each contains the text you want to classify
     completions : Sequence[str]
         strings, where, e.g., each one is the name of a class which could come after a
         prompt
-    model : str, optional
-        the name of an `AutoModelForCausalLM`, by default None
-    model_and_tokenizer : tuple[AutoModelForCausalLM, PreTrainedTokenizer], optional
-        an instantiated model and its corresponding tokenizer, by default None
+    model_and_tokenizer : tuple[AutoModelForCausalLM, PreTrainedTokenizer]
+        an instantiated model and its corresponding tokenizer
     prior : Sequence[float], optional
         a probability distribution over `completions`, representing a belief about their
         likelihoods regardless of the prompt. By default, each completion in
         `completions` is assumed to be equally likely
     end_of_prompt : str, optional
         the string to tack on at the end of every prompt, by default " "
     batch_size : int, optional
@@ -501,59 +470,49 @@
         # predicted probability that ice cream is in the fridge
         pred_probs[1,2]
         # 0.4
     """
     return log_probs_conditional(
         prompts,
         completions,
-        model=model,
-        model_and_tokenizer=model_and_tokenizer,
+        model_and_tokenizer,
         end_of_prompt=end_of_prompt,
         batch_size=batch_size,
     )
 
 
 @classify._predict_proba_examples
 def predict_proba_examples(
     examples: Sequence[Example],
-    model: str = None,
-    model_and_tokenizer: tuple[AutoModelForCausalLM, PreTrainedTokenizer] = None,
+    model_and_tokenizer: tuple[AutoModelForCausalLM, PreTrainedTokenizer],
     batch_size: int = 32,
-) -> Union[list[list[float]], npt.NDArray[np.floating]]:
+) -> Union[list[npt.NDArray[np.floating]], npt.NDArray[np.floating]]:
     """
     Predict probabilities of each completion coming after each prompt.
 
-    Note
-    ----
-    Either `model` or `model_and_tokenizer` must be inputted. It's usually better to
-    instantiate/pre-load a model and tokenizer and pass them to `model_and_tokenizer`.
-    See the Example.
-
     Parameters
     ----------
     examples : Sequence[Example]
         `Example` objects, where each contains a prompt and its set of possible
         completions
-    model : str, optional
-        the name of an `AutoModelForCausalLM`, by default None
-    model_and_tokenizer : tuple[AutoModelForCausalLM, PreTrainedTokenizer], optional
-        an instantiated model and its corresponding tokenizer, by default None
+    model_and_tokenizer : tuple[AutoModelForCausalLM, PreTrainedTokenizer]
+        an instantiated model and its corresponding tokenizer
     batch_size : int, optional
         the maximum number of inputs that the model will process in parallel, by default
         32
 
     Returns
     -------
-    pred_probs : list[list[float]] | npt.NDArray[np.floating]
+    pred_probs : list[npt.NDArray[np.floating]] | npt.NDArray[np.floating]
         `pred_probs[example_idx][completion_idx]` is the model's estimate of the
         probability that `examples[example_idx].completions[completion_idx]` comes after
         `examples[example_idx].prompt + examples[example_idx].end_of_prompt`.
 
         If the number of completions per example is a constant `k`, then an array with
-        shape `(len(examples), k)` is returned instead of a nested/2-D list.
+        shape `(len(examples), k)` is returned instead of a list of 1-D arrays.
 
     Example
     -------
     GPT-2 (small) doing media trivia::
 
         from transformers import AutoModelForCausalLM, AutoTokenizer
         from cappr import Example
@@ -581,50 +540,40 @@
 
         # predicted probability that Batman was played by Kevin Conroy
         pred_probs[0][1]
         # 0.97
     """
     return log_probs_conditional_examples(
         examples,
-        model=model,
-        model_and_tokenizer=model_and_tokenizer,
+        model_and_tokenizer,
         batch_size=batch_size,
     )
 
 
 @classify._predict
 def predict(
     prompts: Sequence[str],
     completions: Sequence[str],
-    model: str = None,
-    model_and_tokenizer: tuple[AutoModelForCausalLM, PreTrainedTokenizer] = None,
+    model_and_tokenizer: tuple[AutoModelForCausalLM, PreTrainedTokenizer],
     prior: Optional[Sequence[float]] = None,
     end_of_prompt: str = " ",
     batch_size: int = 32,
 ) -> list[str]:
     """
     Predict which completion is most likely to follow each prompt.
 
-    Note
-    ----
-    Either `model` or `model_and_tokenizer` must be inputted. It's usually better to
-    instantiate/pre-load a model and tokenizer and pass them to `model_and_tokenizer`.
-    See the Example.
-
     Parameters
     ----------
     prompts : Sequence[str]
         strings, where, e.g., each contains the text you want to classify
     completions : Sequence[str]
         strings, where, e.g., each one is the name of a class which could come after a
         prompt
-    model : str, optional
-        the name of an `AutoModelForCausalLM`, by default None
-    model_and_tokenizer : tuple[AutoModelForCausalLM, PreTrainedTokenizer], optional
-        an instantiated model and its corresponding tokenizer, by default None
+    model_and_tokenizer : tuple[AutoModelForCausalLM, PreTrainedTokenizer]
+        an instantiated model and its corresponding tokenizer
     prior : Sequence[float], optional
         a probability distribution over `completions`, representing a belief about their
         likelihoods regardless of the prompt. By default, each completion in
         `completions` is assumed to be equally likely
     end_of_prompt : str, optional
         the string to tack on at the end of every prompt, by default " "
     batch_size : int, optional
@@ -668,47 +617,37 @@
         preds
         # ['on the stove',
         #  'in the freezer']
     """
     return predict_proba(
         prompts,
         completions,
-        model=model,
-        model_and_tokenizer=model_and_tokenizer,
+        model_and_tokenizer,
         prior=prior,
         end_of_prompt=end_of_prompt,
         batch_size=batch_size,
     )
 
 
 @classify._predict_examples
 def predict_examples(
     examples: Sequence[Example],
-    model: str = None,
-    model_and_tokenizer: tuple[AutoModelForCausalLM, PreTrainedTokenizer] = None,
+    model_and_tokenizer: tuple[AutoModelForCausalLM, PreTrainedTokenizer],
     batch_size: int = 32,
 ) -> list[str]:
     """
     Predict which completion is most likely to follow each prompt.
 
-    Note
-    ----
-    Either `model` or `model_and_tokenizer` must be inputted. It's usually better to
-    instantiate/pre-load a model and tokenizer and pass them to `model_and_tokenizer`.
-    See the Example.
-
     Parameters
     ----------
     examples : Sequence[Example]
         `Example` objects, where each contains a prompt and its set of possible
         completions
-    model : str, optional
-        the name of an `AutoModelForCausalLM`, by default None
-    model_and_tokenizer : tuple[AutoModelForCausalLM, PreTrainedTokenizer], optional
-        an instantiated model and its corresponding tokenizer, by default None
+    model_and_tokenizer : tuple[AutoModelForCausalLM, PreTrainedTokenizer]
+        an instantiated model and its corresponding tokenizer
     batch_size : int, optional
         the maximum number of inputs that the model will process in parallel, by default
         32
 
     Returns
     -------
     preds : list[str]
@@ -741,11 +680,10 @@
         preds = predict_examples(examples, model_and_tokenizer=(model, tokenizer))
         preds
         # ['Clarice Starling',
         #  'Kevin Conroy']
     """
     return predict_proba_examples(
         examples,
-        model=model,
-        model_and_tokenizer=model_and_tokenizer,
+        model_and_tokenizer,
         batch_size=batch_size,
     )
```

### Comparing `cappr-0.2.5/src/cappr/openai/api.py` & `cappr-0.2.6/src/cappr/openai/api.py`

 * *Files identical despite different names*

### Comparing `cappr-0.2.5/src/cappr/openai/classify.py` & `cappr-0.2.6/src/cappr/openai/classify.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,15 +156,15 @@
 
         log_probs_completions[0]
         # [[-5.5],        [[log Pr(z | x, y)],
         #  [-8.2, -2.1]]   [log Pr(d | x, y),    log Pr(e | x, y, d)]]
 
         log_probs_completions[1]
         # [[-11.6],       [[log Pr(z | a, b, c)],
-        #  [-0.3, -1.2]]   [log Pr(d | a, b, c), log Pr(e | a, b, c)]]
+        #  [-0.3, -1.2]]   [log Pr(d | a, b, c), log Pr(e | a, b, c, d)]]
     """
     ## str / non-Sequence[str] inputs silently, wastefully, and irreparably fail
     if isinstance(prompts, str) or not isinstance(prompts, Sequence):
         raise TypeError("prompts must be a Sequence of strings.")
     if isinstance(completions, str) or not isinstance(completions, Sequence):
         raise TypeError("completions must be a Sequence of strings.")
     ## Flat list of prompts and their completions. Will post-process
@@ -413,15 +413,15 @@
         for log_probs_prompt_completions in log_probs_completions
     ]
 
 
 @classify._predict_proba_examples
 def predict_proba_examples(
     examples: Sequence[Example], model: openai.api.Model, ask_if_ok: bool = False
-) -> Union[list[list[float]], npt.NDArray[np.floating]]:
+) -> Union[list[npt.NDArray[np.floating]], npt.NDArray[np.floating]]:
     """
     Predict probabilities of each completion coming after each prompt.
 
     Parameters
     ----------
     examples : Sequence[Example]
         `Example` objects, where each contains a prompt and its set of possible
@@ -433,21 +433,21 @@
     ask_if_ok : bool, optional
         whether or not to prompt you to manually give the go-ahead to run this function,
         after notifying you of the approximate cost of the OpenAI API calls. By default
         False
 
     Returns
     -------
-    pred_probs : list[list[float]] | npt.NDArray[np.floating]
+    pred_probs : list[npt.NDArray[np.floating]] | npt.NDArray[np.floating]
         `pred_probs[example_idx][completion_idx]` is the model's estimate of the
         probability that `examples[example_idx].completions[completion_idx]` comes after
         `examples[example_idx].prompt + examples[example_idx].end_of_prompt`.
 
         If the number of completions per example is a constant `k`, then an array with
-        shape `(len(examples), k)` is returned instead of a nested/2-D list.
+        shape `(len(examples), k)` is returned instead of a list of 1-D arrays.
 
     Example
     -------
     Let's demo COPA https://people.ict.usc.edu/~gordon/copa.html::
 
         from cappr import Example
         from cappr.openai.classify import predict_proba_examples
```

### Comparing `cappr-0.2.5/src/cappr/utils/_batch.py` & `cappr-0.2.6/src/cappr/utils/_batch.py`

 * *Files identical despite different names*

### Comparing `cappr-0.2.5/src/cappr/utils/_check.py` & `cappr-0.2.6/src/cappr/utils/_check.py`

 * *Files identical despite different names*

### Comparing `cappr-0.2.5/src/cappr/utils/classify.py` & `cappr-0.2.6/src/cappr/utils/classify.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,15 +213,15 @@
     Decorator which converts a `log_probs_conditional_examples` function call into a
     `predict_proba_examples` call.
     """
 
     @wraps(log_probs_conditional_examples)
     def wrapper(
         examples, *args, **kwargs
-    ) -> Union[list[list[float]], npt.NDArray[np.floating]]:
+    ) -> Union[list[npt.NDArray[np.floating]], npt.NDArray[np.floating]]:
         log_probs_completions = log_probs_conditional_examples(
             examples, *args, **kwargs
         )
         likelihoods = agg_log_probs(log_probs_completions)
         ## If an example has just 1 completion, normalizing will cause the probability
         ## to trivially be 1! So let's not normalize in that case, and hope the user
         ## knows what they're doing
@@ -257,15 +257,15 @@
             )
         ## prior cannot be jagged b/c every example has the same # of completions
         return posterior_prob(
             likelihoods,
             axis=1,
             prior=prior,
             normalize=normalize,
-            check_prior=False,  ## ## already checked during example construction
+            check_prior=False,  ## already checked during example construction
         )
 
     return wrapper
 
 
 def _predict(predict_proba_func):
     """
```

### Comparing `cappr-0.2.5/src/cappr.egg-info/PKG-INFO` & `cappr-0.2.6/src/cappr.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cappr
-Version: 0.2.5
+Version: 0.2.6
 Summary: Zero-shot text classification using autoregressive language models.
 Home-page: https://github.com/kddubey/cappr/
 Author-email: kushdubey63@gmail.com
 License: Apache License 2.0
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: hf
@@ -26,15 +26,15 @@
 completion comes after an inputted prompt. Hence the name:
 
 > **C**ompletion<br>
   **A**fter<br>
   **P**rompt<br>
   **Pr**obability<br>
 
-The method is fleshed out in my [question on CrossValidated](https://stats.stackexchange.com/q/601159/337906).
+The method is fleshed out in my [question on Cross Validated](https://stats.stackexchange.com/q/601159/337906).
 
 
 ## Usage
 
 <details>
 <summary>Use a model from the OpenAI API</summary>
 
@@ -65,42 +65,47 @@
 ```
 </details>
 
 <details>
 <summary>Use a model from the HuggingFace model hub</summary>
 
 Specifically, this model must be able to be loaded using
-`transformers.AutoModelForCausalLM.from_pretrained(model)`.
-
-Smaller LMs may not work well. But there will likely be better ones in the hub soon.
+`transformers.AutoModelForCausalLM.from_pretrained`.
 
 ```python
+from transformers import AutoModelForCausalLM, AutoTokenizer
 from cappr.huggingface.classify import predict
 
 prompt = 'Which planet is closer to the Sun: Mercury or Earth?'
 
 class_names = ('Mercury', 'Earth')
 prior = None  # uniform prior
 
+# load model and tokenizer
+model_name = 'gpt2'
+model = AutoModelForCausalLM.from_pretrained(model_name)
+tokenizer = AutoTokenizer.from_pretrained(model_name)
+
 preds = predict(prompts=[prompt],
                 completions=class_names,
-                model='gpt2',
+                model_and_tokenizer=(model, tokenizer),
                 prior=prior)
 preds
 # ['Mercury']
 ```
 </details>
 
 <details>
 <summary>Run in batches</summary>
 
 Let's use `huggingface` for this example cuz it's free. And let's predict probabilities
 instead of the class.
 
 ```python
+from transformers import AutoModelForCausalLM, AutoTokenizer
 from cappr.huggingface.classify import predict_proba
 
 prompts = [
     'Stephen Curry is a',
     'Martina Navratilova was a',
     "Dexter, from the TV Series Dexter's Laboratory, is a",
     'LeBron James is a',    
@@ -115,17 +120,23 @@
 
 prior = (
     1/6,  # few
     1/6,  # few
     2/3   # there are more
 )
 
+
+# load model and tokenizer
+model_name = 'gpt2'
+model = AutoModelForCausalLM.from_pretrained(model_name)
+tokenizer = AutoTokenizer.from_pretrained(model_name)
+
 pred_probs = predict_proba(prompts=prompts,
                            completions=class_names,
-                           model='gpt2',
+                           model_and_tokenizer=(model, tokenizer),
                            batch_size=32,  # whatever fits on your CPU/GPU
                            prior=prior)
 
 # pred_probs[i,j] = probability that prompts[i] is classified as class_names[j]
 print(pred_probs.round(1))
 # [[0.5 0.3 0.2]
 #  [0.3 0.6 0.2]
@@ -142,17 +153,15 @@
 ```
 </details>
 
 <details>
 <summary>Run in batches, where each prompt has a different set of possible completions
 </summary>
 
-Again, let's use `huggingface` to predict probabilities. And this time, let's pass in an 
-instantiated model and tokenizer instead of its name. That way, the model isn't
-re-loaded every time you wanna use it.
+Again, let's use `huggingface` to predict probabilities.
 
 ```python
 import numpy as np
 from transformers import AutoModelForCausalLM, AutoTokenizer
 
 from cappr import Example
 from cappr.huggingface.classify import predict_proba_examples
@@ -194,18 +203,15 @@
 See
 [`demos/superglue/copa.ipynb`](https://github.com/kddubey/cappr/blob/main/demos/superglue/copa.ipynb)
 for a demonstration of a slightly harder classification task.
 
 
 ## Documentation
 
-https://cappr.readthedocs.io/en/latest/
-
-Please let me know if you find the writing too dense. The main motivation behind this
-project is simplicity :-)
+https://cappr.readthedocs.io
 
 
 ## Setup
 
 If you intend on using OpenAI models, [sign up for the OpenAI API
 here](https://platform.openai.com/signup), and then set the environment variable
 `OPENAI_API_KEY`. For zero-shot classification, OpenAI models are currently far ahead of
@@ -213,43 +219,39 @@
 
 Install with `pip`:
 
 ```
 python -m pip install cappr
 ```
 
-<details>
-<summary>(Optional) Install requirements for HuggingFace models</summary>
+(Optional) Install requirements for HuggingFace models
 
 ```
 python -m pip install cappr[hf]
 ```
-</details>
 
-<details>
-<summary>(Optional) Install requirements for running demos</summary>
+(Optional) Install requirements for running demos
 
 ```
 python -m pip install cappr[demos]
 ```
-</details>
 
 
 ## Motivation
 
 Create a more usable zero-shot text classification interface than
 [classification via sampling (CVS)](https://platform.openai.com/docs/guides/completion/classification).
 
 <details>
 <summary>Short</summary>
 
-In CVS, your job is to write up your classification task in a `prompt` string, and then
-write custom code to post-process arbitrary `completion`/output strings.
+With CVS, your job is to write up your classification task in a `prompt` string, and
+then write custom code to post-process arbitrary `completion`/output strings.
 
-In CAPPr, your job starts and stops at writing up your classification task as a
+With CAPPr, your job starts and stops at writing up your classification task as a
 `{prompt}{end_of_prompt}{completion}` string.
 </details>
 
 <details>
 <summary>Long</summary>
 
 Please see [this page of the
@@ -305,20 +307,20 @@
 you'll be on the *cappr (slow)* line** :-(
 
 ![](/docs/source/_static/scaling_classes/batch_size_32.png)
 
 *Figure 1: [COPA](https://people.ict.usc.edu/~gordon/copa.html) dataset, repeating the
 choices to simulate multi-class classification tasks. [GPT-2
 (small)](https://huggingface.co/gpt2) was run on a Tesla K80 GPU (whatever was free in
-Google Colab in March 2023, I'm not hardware savvy). 96 classification inputs were
-processed in batches of size 32. Each point in the graph is a median of 5 runs. For
-classification via sampling (CVS), exactly 4 tokens were generated for each prompt,
-which is the number of tokens in `'\n\nAnswer A'`. 1-token times are also shown. But for
-COPA (and other multiple-choice style prompts), that may result in lower zero-shot
-accuracy, as most of the sampled choices come after the first token.*
+Google Colab in March 2023). 96 classification inputs were processed in batches of size
+32. Each point in the graph is a median of 5 runs. For classification via sampling
+(CVS), exactly 4 tokens were generated for each prompt, which is the number of tokens in
+`'\n\nAnswer A'`. 1-token times are also shown. But for COPA (and other multiple-choice
+style prompts), that may result in lower zero-shot accuracy, as most of the sampled
+choices come after the first token.*
 
 See the [`demos/computational_analysis.ipynb`
 notebook](https://github.com/kddubey/cappr/blob/main/demos/computational_analysis.ipynb).
 
 </details>
 
 
@@ -384,74 +386,64 @@
 (**) = I'm currently working on this or will work on it really soon
 
 <details>
 <summary>Code</summary>
 
 - [ ] Testing
   - [ ] Increase test cases
-  - [ ] Some more standardization b/t openai and huggingface tests
-  - [x] Add code coverage badge to look cool
   - [ ] Test input checks
+  - [ ] Test `cappr.openai.api`
+- [ ] Factor out the discount feature in `cappr.openai.classify.predict_proba` into
+`cappr.utils.classify._predict_proba`
 - [x] Small CPU speed-ups
   - [x] For constant-completions input, vectorize `agg_log_probs`
   - [x] For `examples` input, if # completions per prompt is constant, vectorize
   `posterior_prob`
 - [ ] Make progress bars optional, since inference often isn't batched
 - [ ] Factor out input checks (on prompts and completions)
 - [x] De-automate overzealous auto-docstring stuff :-(
 - [ ] HuggingFace `transformers.AutoModelForCausalLM`
+  - [ ] Support as many of them as possible, regardless of way positions are encoded
   - [x] Optimize backend to enable greater scaling wrt # completions/classes
-  - [x] Get it working on single-GPU, check that it's faster than sampling assuming
-  batching
+  - [x] Get it working on GPU, check that it's faster than sampling
     - [ ] Get to the bottom of why it's slower w/o batching
   - [ ] Allow non-`' '` `end_of_prompt`! I'll have to go back to the drawing board I
   think
-  - [ ] Consider batchifying the completions again, since they technically don't go in
-  batches of `batch_size`; the actual batch size is the sum of the number of completions
-  corresponding to the batch of prompts! Not a huge memory issue I think b/c completions
-  are usually half as long. But it should be configurable at the very least.
   - [ ] Factor out repeated code b/t `classify` and `classify_no_cache`
   - [ ] Support [Inference
     Endpoints](https://huggingface.co/docs/inference-endpoints/index)?
-  - [ ] Support TensorFlow models if it's easy
+  - [ ] Support TensorFlow models
   - [ ] Support priming, as in: cache it
 - [x] (for me) Auto-enforced code formatting b/c it's getting time-consuming
 - [ ] Allow for multi-label classification
   - [ ] Pass `normalize` as an argument to predict_proba functions
   - [ ] For `huggingface`, add note that you'll get faster results by passing all
   labels at once (assuming prompt is identical for each label)
-- [ ] Create a notebook template
 - [ ] Fill in missing or non-numpy docstrings
 </details>
 
 <details>
 <summary>Research</summary>
 
 Evaluate on more datasets, and understand its relative advantages and disadvantages vs
 other classification methods.
 
-- [ ] RAFT benchmark (**)
+- [ ] RAFT benchmark
   - [x] Zero-shot training scores
   - [ ] Submit zero-shot test predictions
   - [ ] Few-shot (priming) training scores
   - [ ] Submit few-shot test predictions
 - [ ] Create a user guide, build a table of results comparing competing approaches on
 statistical performance, cost, and computation
-- [ ] Make a computational comparison to sampling (**)
-  - [x] Assume I have full freedom to decide how inference works. Demo w/
-  GPT-2. Process inputs in batches.
+- [ ] Make a computational comparison to sampling
+  - [x] Assume I have full freedom to decide how inference works. Demo w/ GPT-2. Process
+  inputs in batches.
   - [ ] Process inputs 1-by-1
 - [ ] More SuperGLUE tasks?
-  - [ ] Re-run COPA demo w/ left-stripped completions (there are a few which aren't)
 - [ ] Calibration
   - [ ] Is the prior actually effective? Downsample and see
   - [ ] curves
-- [ ] Compare against few-shot embeddings
 - [ ] Finetune smaller, cheaper model and compare against zero-shot w/ davinci
   - [ ] e.g., GPT-2 from huggingface, `text-ada-001`
   - [ ] Again, compare against sampling
 - [ ] Evaluate a bigger model like GPT-J
-- [ ] Evaluate different aggregation functions. Currently taking mean, but
-there was no good theory for that
-- [ ] A bit ambitious: support insertion and backwards-completion. Quite ambitious b/c
-manipulating position IDs isn't sufficient (I think).
 </details>
```

### Comparing `cappr-0.2.5/src/cappr.egg-info/SOURCES.txt` & `cappr-0.2.6/src/cappr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cappr-0.2.5/tests/_test.py` & `cappr-0.2.6/tests/_test.py`

 * *Files identical despite different names*

### Comparing `cappr-0.2.5/tests/huggingface/test_huggingface_classify.py` & `cappr-0.2.6/tests/huggingface/test_huggingface_classify.py`

 * *Files identical despite different names*

### Comparing `cappr-0.2.5/tests/openai/test_openai_classify.py` & `cappr-0.2.6/tests/openai/test_openai_classify.py`

 * *Files identical despite different names*

### Comparing `cappr-0.2.5/tests/utils/test_batch.py` & `cappr-0.2.6/tests/utils/test_batch.py`

 * *Files identical despite different names*

### Comparing `cappr-0.2.5/tests/utils/test_utils_classify.py` & `cappr-0.2.6/tests/utils/test_utils_classify.py`

 * *Files identical despite different names*

