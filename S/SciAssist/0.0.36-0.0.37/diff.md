# Comparing `tmp/SciAssist-0.0.36.tar.gz` & `tmp/SciAssist-0.0.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SciAssist-0.0.36.tar", last modified: Sat Apr 29 16:26:43 2023, max compression
+gzip compressed data, was "SciAssist-0.0.37.tar", last modified: Sat May 20 13:58:25 2023, max compression
```

## Comparing `SciAssist-0.0.36.tar` & `SciAssist-0.0.37.tar`

### file list

```diff
@@ -1,125 +1,119 @@
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 16:26:43.164286 SciAssist-0.0.36/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    21150 2022-09-28 02:29:12.000000 SciAssist-0.0.36/LICENSE
--rw-rw-r--   0 yixi      (1025) yixi      (1027)       38 2022-09-28 02:29:12.000000 SciAssist-0.0.36/MANIFEST.in
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    30858 2023-04-29 16:26:43.164286 SciAssist-0.0.36/PKG-INFO
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     6208 2022-11-05 13:55:02.000000 SciAssist-0.0.36/README.md
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1451 2023-04-29 16:26:23.000000 SciAssist-0.0.36/pyproject.toml
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      635 2023-04-29 16:26:43.164286 SciAssist-0.0.36/setup.cfg
--rw-rw-r--   0 yixi      (1025) yixi      (1027)       96 2022-09-28 02:29:12.000000 SciAssist-0.0.36/setup.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 16:26:43.156285 SciAssist-0.0.36/src/
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 16:26:43.156285 SciAssist-0.0.36/src/SciAssist/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      818 2023-04-14 07:10:04.000000 SciAssist-0.0.36/src/SciAssist/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 16:26:43.156285 SciAssist-0.0.36/src/SciAssist/bin/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      668 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/bin/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 16:26:43.156285 SciAssist-0.0.36/src/SciAssist/bin/__pycache__/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      916 2023-03-15 13:25:23.000000 SciAssist-0.0.36/src/SciAssist/bin/__pycache__/__init__.cpython-38.pyc
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 16:26:43.156285 SciAssist-0.0.36/src/SciAssist/bin/doc2json/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    11558 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/LICENSE
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 16:26:43.156285 SciAssist-0.0.36/src/SciAssist/bin/doc2json/__pycache__/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      158 2023-03-15 13:25:23.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/__pycache__/__init__.cpython-38.pyc
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 16:26:43.156285 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 16:26:43.160285 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/__pycache__/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      167 2023-03-15 13:25:23.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      227 2023-03-15 13:25:23.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/__pycache__/config.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    15546 2023-03-15 13:25:23.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/__pycache__/s2orc.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)       59 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/config.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 16:26:43.160285 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 16:26:43.160285 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      179 2023-03-15 13:25:23.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2874 2023-03-15 13:25:23.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/process_pdf.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    15434 2023-03-15 13:25:23.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/tei_to_json.cpython-38.pyc
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 16:26:43.160285 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4449 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/Readme.md
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 16:26:43.160285 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      186 2023-03-15 13:25:23.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     6183 2023-03-15 13:25:23.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/client.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     5972 2023-03-15 13:25:23.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/grobid_client.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     6614 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/client.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1019 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/config.yaml
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2736 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/grobid.properties
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     9058 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/grobid_client.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        8 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/pdf_to_tei.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     3622 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/process_pdf.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    27209 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/tei_to_json.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    16382 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/s2orc.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 16:26:43.160285 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/utils/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/utils/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 16:26:43.160285 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      173 2023-03-15 13:25:23.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2743 2023-03-15 13:25:23.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/citation_util.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     8839 2023-03-15 13:25:23.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/grobid_util.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     3531 2023-03-15 13:25:23.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/refspan_util.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     3144 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/utils/citation_util.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    11737 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/utils/grobid_util.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     6935 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/utils/latex_util.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4235 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/utils/refspan_util.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      585 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/utils/soup_utils.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 16:26:43.160285 SciAssist-0.0.36/src/SciAssist/bin/doc2json/scripts/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)       73 2022-10-04 11:07:26.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/scripts/run_grobid_linux.sh
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      751 2022-10-04 11:09:22.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/scripts/setup_grobid_linux.sh
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      275 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/bin/doc2json/setup.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 16:26:43.160285 SciAssist-0.0.36/src/SciAssist/datamodules/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/datamodules/__init__.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4113 2023-03-26 03:08:44.000000 SciAssist-0.0.36/src/SciAssist/datamodules/acl_datamodule.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 16:26:43.160285 SciAssist-0.0.36/src/SciAssist/datamodules/components/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/datamodules/components/__init__.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      370 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/datamodules/components/cora_label.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     3112 2022-11-05 13:55:02.000000 SciAssist-0.0.36/src/SciAssist/datamodules/cora_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     3357 2023-04-14 07:10:04.000000 SciAssist-0.0.36/src/SciAssist/datamodules/dataset_extraction_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     3198 2022-11-10 14:45:14.000000 SciAssist-0.0.36/src/SciAssist/datamodules/fid_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2948 2022-11-27 14:04:32.000000 SciAssist-0.0.36/src/SciAssist/datamodules/general_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4331 2022-12-14 08:45:15.000000 SciAssist-0.0.36/src/SciAssist/datamodules/longsumm_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     3179 2023-04-02 03:32:15.000000 SciAssist-0.0.36/src/SciAssist/datamodules/mup_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     7753 2023-03-18 16:34:11.000000 SciAssist-0.0.36/src/SciAssist/datamodules/mup_mup_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     6862 2023-04-29 14:42:50.000000 SciAssist-0.0.36/src/SciAssist/datamodules/mup_scisumm_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     5991 2023-04-25 15:59:38.000000 SciAssist-0.0.36/src/SciAssist/datamodules/mup_scisumm_noctrl_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     5865 2023-04-14 07:09:42.000000 SciAssist-0.0.36/src/SciAssist/datamodules/scisumm_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4850 2023-02-23 16:55:34.000000 SciAssist-0.0.36/src/SciAssist/datamodules/test_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4211 2022-12-18 15:08:30.000000 SciAssist-0.0.36/src/SciAssist/datamodules/xsum_datamodule.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 16:26:43.164286 SciAssist-0.0.36/src/SciAssist/models/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/models/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 16:26:43.164286 SciAssist-0.0.36/src/SciAssist/models/components/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/models/components/__init__.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1554 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/models/components/bart_summarization.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2845 2023-04-14 07:10:04.000000 SciAssist-0.0.36/src/SciAssist/models/components/bert_dataset_extraction.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1547 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/models/components/bert_token_classifier.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1728 2023-04-17 15:52:16.000000 SciAssist-0.0.36/src/SciAssist/models/components/flant5_summarization.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     6869 2022-11-19 15:12:24.000000 SciAssist-0.0.36/src/SciAssist/models/cora_module.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     8632 2023-04-14 07:10:04.000000 SciAssist-0.0.36/src/SciAssist/models/dataset_extraction_module.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    13319 2023-04-02 03:32:15.000000 SciAssist-0.0.36/src/SciAssist/models/mup_bart_module.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 16:26:43.164286 SciAssist-0.0.36/src/SciAssist/pipelines/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     3876 2023-04-26 07:13:45.000000 SciAssist-0.0.36/src/SciAssist/pipelines/__init__.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    12872 2023-04-14 07:10:04.000000 SciAssist-0.0.36/src/SciAssist/pipelines/dataset_extraction.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2056 2022-11-05 13:55:02.000000 SciAssist-0.0.36/src/SciAssist/pipelines/pipeline.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    13826 2022-11-05 13:55:02.000000 SciAssist-0.0.36/src/SciAssist/pipelines/reference_string_parsing.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    14045 2023-04-29 14:44:31.000000 SciAssist-0.0.36/src/SciAssist/pipelines/summarization.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1950 2023-02-20 05:27:12.000000 SciAssist-0.0.36/src/SciAssist/pipelines/testing_pipeline.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4003 2022-11-05 13:55:02.000000 SciAssist-0.0.36/src/SciAssist/pipelines/training_pipeline.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      786 2022-09-28 02:29:12.000000 SciAssist-0.0.36/src/SciAssist/test.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      787 2022-10-02 15:49:40.000000 SciAssist-0.0.36/src/SciAssist/train.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2852 2022-11-27 16:49:31.000000 SciAssist-0.0.36/src/SciAssist/training_args.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 16:26:43.164286 SciAssist-0.0.36/src/SciAssist/utils/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4733 2023-02-03 14:21:07.000000 SciAssist-0.0.36/src/SciAssist/utils/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 16:26:43.164286 SciAssist-0.0.36/src/SciAssist/utils/collators/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2323 2022-11-10 14:30:40.000000 SciAssist-0.0.36/src/SciAssist/utils/collators/CollatorForFid.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-11-06 14:22:00.000000 SciAssist-0.0.36/src/SciAssist/utils/collators/__init__.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1232 2023-01-11 16:34:32.000000 SciAssist-0.0.36/src/SciAssist/utils/data_reader.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    53624 2023-04-29 14:37:32.000000 SciAssist-0.0.36/src/SciAssist/utils/data_utils.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2899 2023-04-22 06:46:59.000000 SciAssist-0.0.36/src/SciAssist/utils/extract_keywords_flant5.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     5722 2023-04-22 06:20:33.000000 SciAssist-0.0.36/src/SciAssist/utils/pdf2text.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2432 2023-04-29 16:24:14.000000 SciAssist-0.0.36/src/SciAssist/utils/windows_pdf2text.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 16:26:43.156285 SciAssist-0.0.36/src/SciAssist.egg-info/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    30858 2023-04-29 16:26:43.000000 SciAssist-0.0.36/src/SciAssist.egg-info/PKG-INFO
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4822 2023-04-29 16:26:43.000000 SciAssist-0.0.36/src/SciAssist.egg-info/SOURCES.txt
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        1 2023-04-29 16:26:43.000000 SciAssist-0.0.36/src/SciAssist.egg-info/dependency_links.txt
--rw-rw-r--   0 yixi      (1025) yixi      (1027)       98 2023-04-29 16:26:43.000000 SciAssist-0.0.36/src/SciAssist.egg-info/entry_points.txt
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      396 2023-04-29 16:26:43.000000 SciAssist-0.0.36/src/SciAssist.egg-info/requires.txt
--rw-rw-r--   0 yixi      (1025) yixi      (1027)       34 2023-04-29 16:26:43.000000 SciAssist-0.0.36/src/SciAssist.egg-info/top_level.txt
--rwxrwxr-x   0 yixi      (1025) yixi      (1027)      690 2022-12-10 17:44:58.000000 SciAssist-0.0.36/src/process.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-29 16:26:43.164286 SciAssist-0.0.36/tests/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1095 2022-12-11 12:29:46.000000 SciAssist-0.0.36/tests/test_rsp.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1129 2022-12-11 12:29:46.000000 SciAssist-0.0.36/tests/test_summ.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-05-20 13:58:25.914371 SciAssist-0.0.37/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    21150 2022-09-28 02:29:12.000000 SciAssist-0.0.37/LICENSE
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)       38 2022-09-28 02:29:12.000000 SciAssist-0.0.37/MANIFEST.in
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    32200 2023-05-20 13:58:25.914371 SciAssist-0.0.37/PKG-INFO
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     7572 2023-05-20 13:47:34.000000 SciAssist-0.0.37/README.md
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1451 2023-05-20 13:50:42.000000 SciAssist-0.0.37/pyproject.toml
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      635 2023-05-20 13:58:25.914371 SciAssist-0.0.37/setup.cfg
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)       96 2022-09-28 02:29:12.000000 SciAssist-0.0.37/setup.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-05-20 13:58:25.902370 SciAssist-0.0.37/src/
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-05-20 13:58:25.906370 SciAssist-0.0.37/src/SciAssist/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      818 2023-04-14 07:10:04.000000 SciAssist-0.0.37/src/SciAssist/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-05-20 13:58:25.906370 SciAssist-0.0.37/src/SciAssist/bin/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      668 2022-09-28 02:29:12.000000 SciAssist-0.0.37/src/SciAssist/bin/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-05-20 13:58:25.906370 SciAssist-0.0.37/src/SciAssist/bin/__pycache__/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      916 2023-03-15 13:25:23.000000 SciAssist-0.0.37/src/SciAssist/bin/__pycache__/__init__.cpython-38.pyc
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-05-20 13:58:25.906370 SciAssist-0.0.37/src/SciAssist/bin/doc2json/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    11558 2022-09-28 02:29:12.000000 SciAssist-0.0.37/src/SciAssist/bin/doc2json/LICENSE
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.37/src/SciAssist/bin/doc2json/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-05-20 13:58:25.906370 SciAssist-0.0.37/src/SciAssist/bin/doc2json/__pycache__/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      158 2023-03-15 13:25:23.000000 SciAssist-0.0.37/src/SciAssist/bin/doc2json/__pycache__/__init__.cpython-38.pyc
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-05-20 13:58:25.906370 SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-05-20 13:58:25.906370 SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/__pycache__/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      167 2023-03-15 13:25:23.000000 SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      227 2023-03-15 13:25:23.000000 SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/__pycache__/config.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    15546 2023-03-15 13:25:23.000000 SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/__pycache__/s2orc.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)       59 2022-09-28 02:29:12.000000 SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/config.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-05-20 13:58:25.906370 SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/grobid2json/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/grobid2json/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-05-20 13:58:25.906370 SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      179 2023-03-15 13:25:23.000000 SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2874 2023-03-15 13:25:23.000000 SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/process_pdf.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    15434 2023-03-15 13:25:23.000000 SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/tei_to_json.cpython-38.pyc
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-05-20 13:58:25.906370 SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4449 2022-09-28 02:29:12.000000 SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/Readme.md
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-05-20 13:58:25.910370 SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      186 2023-03-15 13:25:23.000000 SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     6183 2023-03-15 13:25:23.000000 SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/client.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     5972 2023-03-15 13:25:23.000000 SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/grobid_client.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     6614 2022-09-28 02:29:12.000000 SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/client.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1019 2022-09-28 02:29:12.000000 SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/config.yaml
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2736 2022-09-28 02:29:12.000000 SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/grobid.properties
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     9058 2022-09-28 02:29:12.000000 SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/grobid_client.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        8 2022-09-28 02:29:12.000000 SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/grobid2json/pdf_to_tei.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     3622 2022-09-28 02:29:12.000000 SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/grobid2json/process_pdf.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    27209 2022-09-28 02:29:12.000000 SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/grobid2json/tei_to_json.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    16382 2022-09-28 02:29:12.000000 SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/s2orc.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-05-20 13:58:25.910370 SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/utils/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/utils/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-05-20 13:58:25.910370 SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      173 2023-03-15 13:25:23.000000 SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2743 2023-03-15 13:25:23.000000 SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/citation_util.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     8839 2023-03-15 13:25:23.000000 SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/grobid_util.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     3531 2023-03-15 13:25:23.000000 SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/refspan_util.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     3144 2022-09-28 02:29:12.000000 SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/utils/citation_util.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    11737 2022-09-28 02:29:12.000000 SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/utils/grobid_util.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     6935 2022-09-28 02:29:12.000000 SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/utils/latex_util.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4235 2022-09-28 02:29:12.000000 SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/utils/refspan_util.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      585 2022-09-28 02:29:12.000000 SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/utils/soup_utils.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-05-20 13:58:25.910370 SciAssist-0.0.37/src/SciAssist/bin/doc2json/scripts/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)       73 2022-10-04 11:07:26.000000 SciAssist-0.0.37/src/SciAssist/bin/doc2json/scripts/run_grobid_linux.sh
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      751 2022-10-04 11:09:22.000000 SciAssist-0.0.37/src/SciAssist/bin/doc2json/scripts/setup_grobid_linux.sh
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      275 2022-09-28 02:29:12.000000 SciAssist-0.0.37/src/SciAssist/bin/doc2json/setup.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-05-20 13:58:25.910370 SciAssist-0.0.37/src/SciAssist/datamodules/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.37/src/SciAssist/datamodules/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-05-20 13:58:25.910370 SciAssist-0.0.37/src/SciAssist/datamodules/components/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.37/src/SciAssist/datamodules/components/__init__.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      370 2022-09-28 02:29:12.000000 SciAssist-0.0.37/src/SciAssist/datamodules/components/cora_label.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     3112 2022-11-05 13:55:02.000000 SciAssist-0.0.37/src/SciAssist/datamodules/cora_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     3357 2023-04-14 07:10:04.000000 SciAssist-0.0.37/src/SciAssist/datamodules/dataset_extraction_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2948 2022-11-27 14:04:32.000000 SciAssist-0.0.37/src/SciAssist/datamodules/general_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     3179 2023-04-02 03:32:15.000000 SciAssist-0.0.37/src/SciAssist/datamodules/mup_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     6862 2023-04-29 14:42:50.000000 SciAssist-0.0.37/src/SciAssist/datamodules/mup_scisumm_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     5991 2023-04-25 15:59:38.000000 SciAssist-0.0.37/src/SciAssist/datamodules/mup_scisumm_noctrl_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4850 2023-02-23 16:55:34.000000 SciAssist-0.0.37/src/SciAssist/datamodules/test_datamodule.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-05-20 13:58:25.910370 SciAssist-0.0.37/src/SciAssist/models/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.37/src/SciAssist/models/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-05-20 13:58:25.910370 SciAssist-0.0.37/src/SciAssist/models/components/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.37/src/SciAssist/models/components/__init__.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1554 2022-09-28 02:29:12.000000 SciAssist-0.0.37/src/SciAssist/models/components/bart_summarization.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2489 2023-05-20 13:47:34.000000 SciAssist-0.0.37/src/SciAssist/models/components/bert_dataset_extraction.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1547 2022-09-28 02:29:12.000000 SciAssist-0.0.37/src/SciAssist/models/components/bert_token_classifier.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1728 2023-04-17 15:52:16.000000 SciAssist-0.0.37/src/SciAssist/models/components/flant5_summarization.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     6869 2022-11-19 15:12:24.000000 SciAssist-0.0.37/src/SciAssist/models/cora_module.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     8632 2023-04-14 07:10:04.000000 SciAssist-0.0.37/src/SciAssist/models/dataset_extraction_module.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    13319 2023-04-02 03:32:15.000000 SciAssist-0.0.37/src/SciAssist/models/mup_bart_module.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-05-20 13:58:25.910370 SciAssist-0.0.37/src/SciAssist/pipelines/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     3690 2023-05-20 13:50:35.000000 SciAssist-0.0.37/src/SciAssist/pipelines/__init__.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    12872 2023-04-14 07:10:04.000000 SciAssist-0.0.37/src/SciAssist/pipelines/dataset_extraction.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2056 2022-11-05 13:55:02.000000 SciAssist-0.0.37/src/SciAssist/pipelines/pipeline.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    13826 2022-11-05 13:55:02.000000 SciAssist-0.0.37/src/SciAssist/pipelines/reference_string_parsing.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    14045 2023-05-20 13:51:17.000000 SciAssist-0.0.37/src/SciAssist/pipelines/summarization.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    12861 2023-04-14 07:08:00.000000 SciAssist-0.0.37/src/SciAssist/pipelines/summarization_origin.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1950 2023-02-20 05:27:12.000000 SciAssist-0.0.37/src/SciAssist/pipelines/testing_pipeline.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4003 2022-11-05 13:55:02.000000 SciAssist-0.0.37/src/SciAssist/pipelines/training_pipeline.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      786 2022-09-28 02:29:12.000000 SciAssist-0.0.37/src/SciAssist/test.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      787 2022-10-02 15:49:40.000000 SciAssist-0.0.37/src/SciAssist/train.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2852 2022-11-27 16:49:31.000000 SciAssist-0.0.37/src/SciAssist/training_args.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-05-20 13:58:25.914371 SciAssist-0.0.37/src/SciAssist/utils/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4733 2023-02-03 14:21:07.000000 SciAssist-0.0.37/src/SciAssist/utils/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-05-20 13:58:25.914371 SciAssist-0.0.37/src/SciAssist/utils/collators/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2323 2022-11-10 14:30:40.000000 SciAssist-0.0.37/src/SciAssist/utils/collators/CollatorForFid.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-11-06 14:22:00.000000 SciAssist-0.0.37/src/SciAssist/utils/collators/__init__.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1232 2023-01-11 16:34:32.000000 SciAssist-0.0.37/src/SciAssist/utils/data_reader.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    53624 2023-05-03 16:41:19.000000 SciAssist-0.0.37/src/SciAssist/utils/data_utils.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     5722 2023-04-22 06:20:33.000000 SciAssist-0.0.37/src/SciAssist/utils/pdf2text.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2432 2023-05-20 13:51:36.000000 SciAssist-0.0.37/src/SciAssist/utils/windows_pdf2text.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1499 2023-03-22 11:40:06.000000 SciAssist-0.0.37/src/SciAssist/utils/xml2txt.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-05-20 13:58:25.906370 SciAssist-0.0.37/src/SciAssist.egg-info/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    32200 2023-05-20 13:58:25.000000 SciAssist-0.0.37/src/SciAssist.egg-info/PKG-INFO
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4561 2023-05-20 13:58:25.000000 SciAssist-0.0.37/src/SciAssist.egg-info/SOURCES.txt
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        1 2023-05-20 13:58:25.000000 SciAssist-0.0.37/src/SciAssist.egg-info/dependency_links.txt
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)       98 2023-05-20 13:58:25.000000 SciAssist-0.0.37/src/SciAssist.egg-info/entry_points.txt
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      396 2023-05-20 13:58:25.000000 SciAssist-0.0.37/src/SciAssist.egg-info/requires.txt
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)       26 2023-05-20 13:58:25.000000 SciAssist-0.0.37/src/SciAssist.egg-info/top_level.txt
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-05-20 13:58:25.914371 SciAssist-0.0.37/tests/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1095 2022-12-11 12:29:46.000000 SciAssist-0.0.37/tests/test_rsp.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1129 2022-12-11 12:29:46.000000 SciAssist-0.0.37/tests/test_summ.py
```

### Comparing `SciAssist-0.0.36/LICENSE` & `SciAssist-0.0.37/LICENSE`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.36/PKG-INFO` & `SciAssist-0.0.37/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SciAssist
-Version: 0.0.36
+Version: 0.0.37
 Summary: A toolkit for Scientific Document Processing
 Author-email: WING-NUS <dingyixi@hotmail.com>
 Maintainer-email: Yixi Ding <dingyixi@hotmail.com>
 License: Attribution-NonCommercial-ShareAlike 4.0 International
         
         =======================================================================
         
@@ -457,15 +457,15 @@
 
 **Documentation**
 - Move the definition of `Pipeline` class from `Usage` to `Contribution Guide`.
 - Add catalog for Contribution Guide.
 - Add examples for choosing devices in `Usage`.
 
 <div align="center">
-   
+
 # SciAssist
 [![PyPI Status](https://badge.fury.io/py/sciassist.svg)](https://badge.fury.io/py/sciassist)
 <a href="https://pytorch.org/get-started/locally/"><img alt="PyTorch" src="https://img.shields.io/badge/PyTorch-ee4c2c?logo=pytorch&logoColor=white"></a>
 <a href="https://pytorchlightning.ai/"><img alt="Lightning" src="https://img.shields.io/badge/-Lightning-792ee5?logo=pytorchlightning&logoColor=white"></a>
 <a href="https://hydra.cc/"><img alt="Config: Hydra" src="https://img.shields.io/badge/Config-Hydra-89b8cd"></a>
 <a href="https://github.com/ashleve/lightning-hydra-template"><img alt="Template" src="https://img.shields.io/badge/-Lightning--Hydra--Template-017F2F?style=flat&logo=github&labelColor=gray"></a><br>
 [![ReadTheDocs](https://readthedocs.org/projects/wing-sciassist/badge/)](https://wing-sciassist.readthedocs.io/en/latest/)
@@ -500,14 +500,15 @@
 
 
 ## Usage
 
 Here are some example usages.
 
 **Reference string parsing:**
+
 ```python
 from SciAssist import ReferenceStringParsing
 
 # Set device="cpu" if you want to use only CPU. The default device is "gpu".
 # ref_parser = ReferenceStringParsing(device="cpu")
 ref_parser = ReferenceStringParsing(device="gpu")
 
@@ -519,14 +520,15 @@
 # For text
 res  = ref_parser.predict("test.txt", type="txt")
 # For pdf
 res = ref_parser.predict("test.pdf")
 ```
 
 **Summarizarion for single document:**
+
 ```python
 from SciAssist import Summarization
 
 # Set device="cpu" if you want to use only CPU. The default device is "gpu".
 # pipleine = Summarization(device="cpu")
 summerizer = Summarization(device="gpu")
 
@@ -548,22 +550,42 @@
 # For text
 res = summerizer.predict("bodytext.txt", type="txt")
 # For pdf
 res = summerizer.predict("raw.pdf")
 
 ```
 
+**Dataset mention extraction:**
+
+```python
+from SciAssist import DatasetExtraction
+
+# Set device="cpu" if you want to use only CPU. The default device is "gpu".
+# ref_parser = DatasetExtraction(device="cpu")
+extractor = DatasetExtraction(device="gpu")
+
+# For string
+res = extractor.extract("The impact of gender identity on emotions was examined by researchers using a subsample from the National Longitudinal Study of Adolescent Health. The study aimed to investigate the direct effects of gender identity on emotional experiences and expression. By focusing on a subsample of the larger study, the researchers were able to hone in on the specific relationship between gender identity and emotions. Through their analysis, the researchers sought to determine whether gender identity could have a significant and direct impact on emotional well-being. The findings of the study have important implications for our understanding of the complex interplay between gender identity and emotional experiences, and may help to inform future interventions and support for individuals who experience gender-related emotional distress.", type="str")
+# For text: please input the path of your .txt file
+res = extractor.extract("test.txt", type="txt")
+# For pdf: please input the path of your .pdf file
+res = extractor.predict("test.pdf", type="pdf")
+```
+
+
+
 ## Contribution
+
 Here's a simple introduction about how to incorporate a new task into SciAssist. 
 Generally, to add a new task, you will need to:
 
     1. Git clone this repo and prepare the virtual environment.
     2. Install Grobid Server.
     3. Create a LightningModule and a DataLightningModule.
     4. Train a model.
     5. Provide a pipeline for users.
-    
+
 We provide a step-by-step contribution guide, see [SciAssist’s documentation](https://wing-sciassist.readthedocs.io/en/latest/Contribution.html#).
 
 ## LICENSE
 This toolkit is licensed under the `Attribution-NonCommercial-ShareAlike 4.0 International`.
 Read [LICENSE](https://github.com/WING-NUS/SciAssist/blob/main/LICENSE) for more information.
```

### Comparing `SciAssist-0.0.36/README.md` & `SciAssist-0.0.37/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 **Documentation**
 - Move the definition of `Pipeline` class from `Usage` to `Contribution Guide`.
 - Add catalog for Contribution Guide.
 - Add examples for choosing devices in `Usage`.
 
 <div align="center">
-   
+
 # SciAssist
 [![PyPI Status](https://badge.fury.io/py/sciassist.svg)](https://badge.fury.io/py/sciassist)
 <a href="https://pytorch.org/get-started/locally/"><img alt="PyTorch" src="https://img.shields.io/badge/PyTorch-ee4c2c?logo=pytorch&logoColor=white"></a>
 <a href="https://pytorchlightning.ai/"><img alt="Lightning" src="https://img.shields.io/badge/-Lightning-792ee5?logo=pytorchlightning&logoColor=white"></a>
 <a href="https://hydra.cc/"><img alt="Config: Hydra" src="https://img.shields.io/badge/Config-Hydra-89b8cd"></a>
 <a href="https://github.com/ashleve/lightning-hydra-template"><img alt="Template" src="https://img.shields.io/badge/-Lightning--Hydra--Template-017F2F?style=flat&logo=github&labelColor=gray"></a><br>
 [![ReadTheDocs](https://readthedocs.org/projects/wing-sciassist/badge/)](https://wing-sciassist.readthedocs.io/en/latest/)
@@ -50,14 +50,15 @@
 
 
 ## Usage
 
 Here are some example usages.
 
 **Reference string parsing:**
+
 ```python
 from SciAssist import ReferenceStringParsing
 
 # Set device="cpu" if you want to use only CPU. The default device is "gpu".
 # ref_parser = ReferenceStringParsing(device="cpu")
 ref_parser = ReferenceStringParsing(device="gpu")
 
@@ -69,14 +70,15 @@
 # For text
 res  = ref_parser.predict("test.txt", type="txt")
 # For pdf
 res = ref_parser.predict("test.pdf")
 ```
 
 **Summarizarion for single document:**
+
 ```python
 from SciAssist import Summarization
 
 # Set device="cpu" if you want to use only CPU. The default device is "gpu".
 # pipleine = Summarization(device="cpu")
 summerizer = Summarization(device="gpu")
 
@@ -98,22 +100,42 @@
 # For text
 res = summerizer.predict("bodytext.txt", type="txt")
 # For pdf
 res = summerizer.predict("raw.pdf")
 
 ```
 
+**Dataset mention extraction:**
+
+```python
+from SciAssist import DatasetExtraction
+
+# Set device="cpu" if you want to use only CPU. The default device is "gpu".
+# ref_parser = DatasetExtraction(device="cpu")
+extractor = DatasetExtraction(device="gpu")
+
+# For string
+res = extractor.extract("The impact of gender identity on emotions was examined by researchers using a subsample from the National Longitudinal Study of Adolescent Health. The study aimed to investigate the direct effects of gender identity on emotional experiences and expression. By focusing on a subsample of the larger study, the researchers were able to hone in on the specific relationship between gender identity and emotions. Through their analysis, the researchers sought to determine whether gender identity could have a significant and direct impact on emotional well-being. The findings of the study have important implications for our understanding of the complex interplay between gender identity and emotional experiences, and may help to inform future interventions and support for individuals who experience gender-related emotional distress.", type="str")
+# For text: please input the path of your .txt file
+res = extractor.extract("test.txt", type="txt")
+# For pdf: please input the path of your .pdf file
+res = extractor.predict("test.pdf", type="pdf")
+```
+
+
+
 ## Contribution
+
 Here's a simple introduction about how to incorporate a new task into SciAssist. 
 Generally, to add a new task, you will need to:
 
     1. Git clone this repo and prepare the virtual environment.
     2. Install Grobid Server.
     3. Create a LightningModule and a DataLightningModule.
     4. Train a model.
     5. Provide a pipeline for users.
-    
+
 We provide a step-by-step contribution guide, see [SciAssist’s documentation](https://wing-sciassist.readthedocs.io/en/latest/Contribution.html#).
 
 ## LICENSE
 This toolkit is licensed under the `Attribution-NonCommercial-ShareAlike 4.0 International`.
 Read [LICENSE](https://github.com/WING-NUS/SciAssist/blob/main/LICENSE) for more information.
```

#### html2text {}

```diff
@@ -57,17 +57,35 @@
 perfectly fitting/interpolating the data . Much recent work in statistical
 learning theory has tried to find theoretical ground for this empirical finding
 . Since learning using models that interpolate is not exclusive to deep neural
 networks , we study generalization in the presence of interpolation in the case
 of kernel methods . We study both linear and kernel least squares problems in
 this paper . """ # For string res = summerizer.predict(text, type="str") # For
 text res = summerizer.predict("bodytext.txt", type="txt") # For pdf res =
-summerizer.predict("raw.pdf") ``` ## Contribution Here's a simple introduction
-about how to incorporate a new task into SciAssist. Generally, to add a new
-task, you will need to: 1. Git clone this repo and prepare the virtual
-environment. 2. Install Grobid Server. 3. Create a LightningModule and a
-DataLightningModule. 4. Train a model. 5. Provide a pipeline for users. We
-provide a step-by-step contribution guide, see [SciAssistâs documentation]
-(https://wing-sciassist.readthedocs.io/en/latest/Contribution.html#). ##
-LICENSE This toolkit is licensed under the `Attribution-NonCommercial-
-ShareAlike 4.0 International`. Read [LICENSE](https://github.com/WING-NUS/
-SciAssist/blob/main/LICENSE) for more information.
+summerizer.predict("raw.pdf") ``` **Dataset mention extraction:** ```python
+from SciAssist import DatasetExtraction # Set device="cpu" if you want to use
+only CPU. The default device is "gpu". # ref_parser = DatasetExtraction
+(device="cpu") extractor = DatasetExtraction(device="gpu") # For string res =
+extractor.extract("The impact of gender identity on emotions was examined by
+researchers using a subsample from the National Longitudinal Study of
+Adolescent Health. The study aimed to investigate the direct effects of gender
+identity on emotional experiences and expression. By focusing on a subsample of
+the larger study, the researchers were able to hone in on the specific
+relationship between gender identity and emotions. Through their analysis, the
+researchers sought to determine whether gender identity could have a
+significant and direct impact on emotional well-being. The findings of the
+study have important implications for our understanding of the complex
+interplay between gender identity and emotional experiences, and may help to
+inform future interventions and support for individuals who experience gender-
+related emotional distress.", type="str") # For text: please input the path of
+your .txt file res = extractor.extract("test.txt", type="txt") # For pdf:
+please input the path of your .pdf file res = extractor.predict("test.pdf",
+type="pdf") ``` ## Contribution Here's a simple introduction about how to
+incorporate a new task into SciAssist. Generally, to add a new task, you will
+need to: 1. Git clone this repo and prepare the virtual environment. 2. Install
+Grobid Server. 3. Create a LightningModule and a DataLightningModule. 4. Train
+a model. 5. Provide a pipeline for users. We provide a step-by-step
+contribution guide, see [SciAssistâs documentation](https://wing-
+sciassist.readthedocs.io/en/latest/Contribution.html#). ## LICENSE This toolkit
+is licensed under the `Attribution-NonCommercial-ShareAlike 4.0 International`.
+Read [LICENSE](https://github.com/WING-NUS/SciAssist/blob/main/LICENSE) for
+more information.
```

### Comparing `SciAssist-0.0.36/pyproject.toml` & `SciAssist-0.0.37/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "SciAssist"
-version = "0.0.36"
+version = "0.0.37"
 authors = [
   { name="WING-NUS", email="dingyixi@hotmail.com" },
 ]
 maintainers = [
   { name="Yixi Ding", email="dingyixi@hotmail.com" },
 ]
 description = "A toolkit for Scientific Document Processing"
```

### Comparing `SciAssist-0.0.36/setup.cfg` & `SciAssist-0.0.37/setup.cfg`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.36/src/SciAssist/__init__.py` & `SciAssist-0.0.37/src/SciAssist/__init__.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.36/src/SciAssist/bin/__init__.py` & `SciAssist-0.0.37/src/SciAssist/bin/__init__.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.36/src/SciAssist/bin/__pycache__/__init__.cpython-38.pyc` & `SciAssist-0.0.37/src/SciAssist/bin/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.36/src/SciAssist/bin/doc2json/LICENSE` & `SciAssist-0.0.37/src/SciAssist/bin/doc2json/LICENSE`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/__pycache__/s2orc.cpython-38.pyc` & `SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/__pycache__/s2orc.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/process_pdf.cpython-38.pyc` & `SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/process_pdf.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/tei_to_json.cpython-38.pyc` & `SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/tei_to_json.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/Readme.md` & `SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/Readme.md`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/client.cpython-38.pyc` & `SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/client.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/grobid_client.cpython-38.pyc` & `SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/grobid_client.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/client.py` & `SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/client.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/config.yaml` & `SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/config.yaml`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/grobid.properties` & `SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/grobid.properties`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/grobid_client.py` & `SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/grobid_client.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/process_pdf.py` & `SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/grobid2json/process_pdf.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/grobid2json/tei_to_json.py` & `SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/grobid2json/tei_to_json.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/s2orc.py` & `SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/s2orc.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/citation_util.cpython-38.pyc` & `SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/citation_util.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/grobid_util.cpython-38.pyc` & `SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/grobid_util.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/refspan_util.cpython-38.pyc` & `SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/refspan_util.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/utils/citation_util.py` & `SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/utils/citation_util.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/utils/grobid_util.py` & `SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/utils/grobid_util.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/utils/latex_util.py` & `SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/utils/latex_util.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/utils/refspan_util.py` & `SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/utils/refspan_util.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.36/src/SciAssist/bin/doc2json/doc2json/utils/soup_utils.py` & `SciAssist-0.0.37/src/SciAssist/bin/doc2json/doc2json/utils/soup_utils.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.36/src/SciAssist/bin/doc2json/scripts/setup_grobid_linux.sh` & `SciAssist-0.0.37/src/SciAssist/bin/doc2json/scripts/setup_grobid_linux.sh`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.36/src/SciAssist/datamodules/acl_datamodule.py` & `SciAssist-0.0.37/src/SciAssist/datamodules/test_datamodule.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from SciAssist.utils.data_utils import DataUtilsForSeq2Seq
 import nltk
 from nltk.corpus import stopwords
 from nltk.tokenize import word_tokenize
 
 
 
-class ACLDataModule(LightningDataModule):
+class TestDataModule(LightningDataModule):
     def __init__(
         self,
         data_repo: str,
         train_batch_size: int = 8,
         num_workers: int = 0,
         pin_memory: bool = False,
         data_cache_dir: str = ".cache",
@@ -35,52 +35,68 @@
         self.data_utils = self.hparams.data_utils
         self.data_collator = self.data_utils.collator()
 
         self.data_test: Optional[Dataset] = None
 
     def prepare_data(self) -> DatasetDict:
 
+        stop_words = set(stopwords.words('english'))
         # Prepare keywords
         text = []
         summ = []
         kw = []
         id = []
         lengths = []
-        with open("/home/yixi/project/sciassist/data/pdfs/text/test.csv", 'r', newline='', encoding='ISO-8859-1') as f:
+        with open("/home/dingyx/project/SciAssist/data/MUP/mup_flant5_target_Entities_sci2.csv", 'r', newline='', encoding='ISO-8859-1') as f:
             rows = csv.reader(f)
             # Get Column names
             keys = next(rows)
             # Add values by column
             for row in rows:
+                # keywords = list(set(row[4].split(",")))
+                # kws = []
+                # for k in keywords:
+                #     word_tokens = word_tokenize(k)
+                #     for w in word_tokens:
+                #         if w not in stop_words:
+                #             kws.append(w)
 
-                kws = row[2].split(",")
 
-                kws = [kws[0]]
+                kws = row[4].split(",")
 
-                with open("/home/yixi/project/sciassist/data/pdfs/summary_ours/" + row[0] + ".txt" , "w") as f:
-                    f.write(" ".join(kws) + " => ")
-                # for i in range(5):
-                    with open("/home/yixi/project/sciassist/data/pdfs/text/" + row[1], "r") as t:
-                        txt = t.readlines()
-                        txt = " ".join(txt)
-                        text.append(txt)
-                    summ.append("a")
+                kws = [kws[0]]
+                # if int(row[0]) <= 300 and int(row[0]) % 10 == 0:
+                #     with open("/home/dingyx/project/SciAssist/data/Flan-T5/" + row[0] +".txt","w") as f:
+                #         f.write(row[3])
+                #         f.write("\n\n")
+                #         f.write(" ".join(kws))
+                #         f.write(" => ")
+                #     text.append(row[3])
+                #     summ.append(row[2])
+                #     kw.append(kws)
+                #     id.append(int(row[0]))
+
+                # with open("/home/dingyx/project/SciAssist/data/MUP_all2/" + row[0] + ".txt", "w") as f:
+                #     f.write(" ".join(kws) + " => ")
+                for i in range(5):
+                    text.append(row[3])
+                    summ.append(row[2])
                     kw.append(kws)
                     id.append(int(row[0]))
-                    lengths.append(100)
+                    lengths.append((i+1)*50)
 
 
         # lengths = [len(s.split(" ")) for s in summ]
         # lengths = [50*math.ceil(s/50) for s in lengths]
         # lengths = [50 for s in lengths]
         mup_datasets = {
             "text": text,
             "summary": summ,
-            "keywords": kw,
-            # "length": lengths,
+            # "keywords": kw,
+            "length": lengths,
             "id": id,
             # "length": [None for i in text]
         }
         # raw_datasets["validation"] = {
 
 
         raw_datasets = DatasetDict()
```

### Comparing `SciAssist-0.0.36/src/SciAssist/datamodules/cora_datamodule.py` & `SciAssist-0.0.37/src/SciAssist/datamodules/cora_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.36/src/SciAssist/datamodules/dataset_extraction_datamodule.py` & `SciAssist-0.0.37/src/SciAssist/datamodules/dataset_extraction_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.36/src/SciAssist/datamodules/fid_datamodule.py` & `SciAssist-0.0.37/src/SciAssist/datamodules/mup_datamodule.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,28 +3,27 @@
 from typing import Optional
 
 import datasets
 from datasets import Dataset, DatasetDict
 from pytorch_lightning import LightningDataModule
 from torch.utils.data import DataLoader
 
-from SciAssist.utils.data_reader import csv_reader
-from SciAssist.utils.data_utils import DataUtilsForFiD
+from SciAssist.utils.data_utils import DataUtilsForSeq2Seq
 
 
-class FiDDataModule(LightningDataModule):
+class MupDataModule(LightningDataModule):
     def __init__(
         self,
         data_repo: str,
         train_batch_size: int = 8,
         num_workers: int = 0,
         pin_memory: bool = False,
         data_cache_dir: str = ".cache",
         seed: int = 777,
-        data_utils = DataUtilsForFiD
+        data_utils = DataUtilsForSeq2Seq
     ):
         super().__init__()
         self.save_hyperparameters(logger=False)
         self.data_cache_dir = Path(self.hparams.data_cache_dir)
         self.data_utils = self.hparams.data_utils
         self.data_collator = self.data_utils.collator()
 
@@ -35,31 +34,30 @@
     def prepare_data(self) -> DatasetDict:
         raw_datasets = datasets.load_dataset(
             self.hparams.data_repo,
             cache_dir=self.data_cache_dir
         )
 
         # Get test from csv
-        raw_datasets["test"] = csv_reader("data/mup/test-release.csv")
+        # raw_datasets["test"] = csv_reader("data/mup/test-release.csv")
         return raw_datasets
 
     def setup(self, stage: Optional[str] = None):
         if not self.data_train and not self.data_val and not self.data_test:
             processed_datasets = self.prepare_data()
             tokenized_datasets = processed_datasets.map(
                 lambda x: self.data_utils.tokenize_and_align_labels(x, inputs_column="text", labels_column="summary"),
                 batched=True,
                 remove_columns=processed_datasets["train"].column_names,
                 load_from_cache_file=True
             )
             self.data_train = tokenized_datasets["train"]
             self.data_val = tokenized_datasets["validation"]
-            # If labels are not provided, delete the column "target"
-            self.data_test = tokenized_datasets["test"]
-
+            # If labels are not provided, delete the column "labels"
+            self.data_test = tokenized_datasets["test"].remove_columns("labels")
 
     def train_dataloader(self):
         return DataLoader(
             dataset=self.data_train,
             batch_size=self.hparams.train_batch_size,
             num_workers=self.hparams.num_workers,
             pin_memory=self.hparams.pin_memory,
```

### Comparing `SciAssist-0.0.36/src/SciAssist/datamodules/general_datamodule.py` & `SciAssist-0.0.37/src/SciAssist/datamodules/general_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.36/src/SciAssist/datamodules/mup_mup_datamodule.py` & `SciAssist-0.0.37/src/SciAssist/datamodules/mup_scisumm_noctrl_datamodule.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,163 +1,98 @@
 # main developer: Yixi Ding <dingyixi@hotmail.com>
 import csv
 import math
 import os
-import random
 from pathlib import Path
 from typing import Optional
 
 import datasets
 from datasets import Dataset, DatasetDict
 from pytorch_lightning import LightningDataModule
 from torch.utils.data import DataLoader, random_split
 
-from SciAssist.utils.data_reader import csv_reader
 from SciAssist.utils.data_utils import DataUtilsForSeq2Seq
 
 
-class MupSciSummDataModule(LightningDataModule):
+class MupSciSummNoCtrlDataModule(LightningDataModule):
     def __init__(
-        self,
-        data_repo: str,
-        train_batch_size: int = 8,
-        num_workers: int = 0,
-        pin_memory: bool = False,
-        data_cache_dir: str = ".cache",
-        seed: int = 777,
-        data_utils = DataUtilsForSeq2Seq
+            self,
+            data_repo: str,
+            train_batch_size: int = 8,
+            num_workers: int = 0,
+            pin_memory: bool = False,
+            data_cache_dir: str = ".cache",
+            seed: int = 777,
+            data_utils=DataUtilsForSeq2Seq
     ):
         super().__init__()
         self.save_hyperparameters(logger=False)
         self.data_cache_dir = Path(self.hparams.data_cache_dir)
         self.data_utils = self.hparams.data_utils
         self.data_collator = self.data_utils.collator()
 
         self.data_train: Optional[Dataset] = None
         self.data_val: Optional[Dataset] = None
         self.data_test: Optional[Dataset] = None
 
-    # def prepare_data(self) -> DatasetDict:
-    #     mup_datasets  = datasets.load_dataset(
-    #         self.hparams.data_repo,
-    #         cache_dir=self.data_cache_dir
-    #     )
-    #     # Prepare keywords
-    #     id2kw = {}
-    #     with open("/home/dingyx/project/SciAssist/data/Task2/From-ScisummNet-2019/scisumm_flant5_target_Entities_sci2.csv", 'r', newline='', encoding='ISO-8859-1') as f:
-    #         rows = csv.reader(f)
-    #         # Get Column names
-    #         keys = next(rows)
-    #         # Add values by column
-    #         for row in rows:
-    #             id2kw[row[0]] = row[1]
-    #
-    #
-    #     file_list = []
-    #     root_dir = "/home/dingyx/project/SciAssist/data/Task2/From-ScisummNet-2019/"
-    #     for dirpath, dirnames, files in os.walk(root_dir):
-    #         file_list = dirnames
-    #         break
-    #
-    #     texts = []
-    #     summaries = []
-    #     keywords = []
-    #     for file in file_list:
-    #         with open(os.path.join(root_dir, file, "summary", file + ".scisummnet_human.txt"), "r") as f:
-    #             summary = f.readlines()
-    #             summary = " ".join(summary[1:])
-    #             summaries.append(summary)
-    #         with open(os.path.join(root_dir, file, file + ".txt"), "r") as f:
-    #             text = f.readlines()
-    #             text = " ".join(text)
-    #             texts.append(text)
-    #         keywords.append(id2kw[file].split(","))
-    #     scisumm_datasets = {
-    #         "text": texts,
-    #         "summary": summaries,
-    #         "keywords": keywords,
-    #         "length": [None for i in texts]
-    #     }
-    #
-    #     lengths = [len(s.split(" ")) for s in mup_datasets["train"]["summary"]]
-    #     lengths = [50*math.ceil(s/50) for s in lengths]
-    #
-    #     raw_datasets = DatasetDict()
-    #     raw_datasets["train"] = {
-    #         "text": scisumm_datasets["text"] + mup_datasets["train"]["text"],
-    #         "summary": scisumm_datasets["summary"] + mup_datasets["train"]["summary"],
-    #         "keywords": keywords + [None for i in mup_datasets["train"]["text"]],
-    #         "length": scisumm_datasets["length"] + lengths
-    #     }
-    #
-    #
-    #
-    #     raw_datasets["train"] = Dataset.from_dict(raw_datasets["train"])
-    #     # raw_datasets["test"] = Dataset.from_dict(mup_datasets)
-    #     # raw_datasets["validation"] = Dataset.from_dict(raw_datasets["validation"])
-    #     # raw_datasets = Dataset.from_dict(raw_datasets)
-    #     return raw_datasets
-
-
     def prepare_data(self) -> DatasetDict:
-
+        mup_datasets = datasets.load_dataset(
+            self.hparams.data_repo,
+            cache_dir=self.data_cache_dir
+        )
         # Prepare keywords
-        summ = []
-        kw = []
-        text = []
-        with open("/home/yixi/project/sciassist/data/train2.csv", 'r', newline='', encoding='ISO-8859-1') as f:
-            rows = csv.reader(f)
-            # Get Column names
-            keys = next(rows)
-            # Add values by column
-            for row in rows:
-                if row[0].isnumeric():
-                    kws = row[4].split(",")
-                    kws = list(set(kws))
-                    summ.append(row[2])
-                    kw.append(kws)
-                    text.append(row[3])
-                # lengths.append(100)
-
-        lengths = [len(s.split(" ")) for s in summ]
-        lengths = [50*math.ceil(s/50) for s in lengths]
-
-        mask1=[]
-        mask2=[]
-        mask1 = random.sample(range(0, int(len(text))), int(len(text) / 3))
-        mask2 = random.sample(range(0, int(len(text))), int(len(text) / 5))
-
-        # for i in range(int(len(text)/3)):
-        #     mask2.append(random.randint(0, len(text)-1))
-
-        for i in mask1:
-            if len(kw[i])<=1:
-                kw[i] = None
-        for i in mask2:
-            if lengths[i] <= 100:
-                lengths[i] = None
+        id2kw = {}
+        filter_files = ['C04-1046', 'J93-2004', 'C00-1072', 'J94-4004', 'C04-1100', 'C88-1016', 'M95-1005', 'J05-1004',
+                        'H94-1046', 'C86-1016', 'P90-1010', 'C96-1079', 'P89-1009', 'C92-3150', 'C00-2136', 'C92-1025',
+                        'H94-1048', 'M95-1012', 'H92-1026', 'P85-1011', 'C96-2183', 'C94-1042', 'C92-2082', 'C02-2025',
+                        'H05-2018', 'W08-2123', 'C96-1058', 'H91-1060', 'C88-2128', 'C02-1139', 'C00-1007', 'C92-3126',
+                        'I05-3025', 'J06-1003', 'J08-2005', 'H91-1026', 'C94-1032', 'C94-1027', 'H93-1051', 'C88-2147',
+                        'H92-1045', 'C90-3063', 'C90-3044', 'C94-2174', 'D07-1074', 'H93-1052', 'N03-2021', 'C88-2121',
+                        'C92-2070', 'C00-2137', 'W97-0703', 'H94-1020', 'C90-3030', 'H01-1035', 'C96-1055', 'H93-1061',
+                        'C96-1005', 'C00-1044', 'C92-1038', 'C00-2163', 'C90-3052', 'J94-2003', 'C04-1073']
+        texts = []
+        summaries = []
+
+
+        file_list = []
+        root_dir = "/home/yixi/project/scisumm-corpus/data/Training-Set-2019/Task2/From-ScisummNet-2019"
+        for dirpath, dirnames, files in os.walk(root_dir):
+            file_list = dirnames
+            break
+
+        for file in file_list:
+            if file in filter_files:
+                continue
+            with open(os.path.join(root_dir, file, "summary", file + ".scisummnet_human.txt"), "r") as f:
+                summary = f.readlines()
+                summary = " ".join(summary[1:])
+                summaries.append(summary)
+            with open(os.path.join(root_dir, file, file + ".txt"), "r") as f:
+                text = f.readlines()
+                text = " ".join(text)
+                texts.append(text)
+        scisumm_datasets = {
+            "text": texts,
+            "summary": summaries,
+        }
+
+
 
         raw_datasets = DatasetDict()
         raw_datasets["train"] = {
-            "text": text,
-            "summary": summ,
-            "keywords": kw,
-            "length": lengths
+            "text": scisumm_datasets["text"] + mup_datasets["train"]["text"],
+            "summary": scisumm_datasets["summary"] + mup_datasets["train"]["summary"],
         }
 
-
-
         raw_datasets["train"] = Dataset.from_dict(raw_datasets["train"])
         # raw_datasets["test"] = Dataset.from_dict(mup_datasets)
         # raw_datasets["validation"] = Dataset.from_dict(raw_datasets["validation"])
         # raw_datasets = Dataset.from_dict(raw_datasets)
         return raw_datasets
 
-
-
     def setup(self, stage: Optional[str] = None):
         if not self.data_train and not self.data_val and not self.data_test:
             processed_datasets = self.prepare_data()
             tokenized_datasets = processed_datasets.map(
                 lambda x: self.data_utils.tokenize_and_align_labels(x, inputs_column="text", labels_column="summary"),
                 batched=True,
                 remove_columns=processed_datasets["train"].column_names,
```

### Comparing `SciAssist-0.0.36/src/SciAssist/datamodules/mup_scisumm_datamodule.py` & `SciAssist-0.0.37/src/SciAssist/datamodules/mup_scisumm_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.36/src/SciAssist/models/components/bart_summarization.py` & `SciAssist-0.0.37/src/SciAssist/models/components/bart_summarization.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.36/src/SciAssist/models/components/bert_dataset_extraction.py` & `SciAssist-0.0.37/src/SciAssist/models/components/bert_dataset_extraction.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,15 +21,14 @@
         self.bert = AutoModel.from_pretrained(model_checkpoint, cache_dir=cache_dir)
 
         self.dropout = nn.Dropout(self.bert.config.hidden_dropout_prob)
         self.crf = CRF(self.num_ner_tags, batch_first=True)
         self.cel = CrossEntropyLoss()
         self.ner_classifier = nn.Linear(self.bert.config.hidden_size, self.num_ner_tags)
         self.cls_classifier = nn.Linear(self.bert.config.hidden_size, self.num_cls_labels)
-        # self.init_weights()
 
     def forward(self, input_subwords, input_token_start_indexs, attention_mask=None, ner_tags=None, cls_labels=None):
         outputs = self.bert(input_subwords,
                             attention_mask=attention_mask,
                             token_type_ids=None,
                             position_ids=None,
                             head_mask=None,
@@ -39,25 +38,23 @@
         # obtain original token representations from subwords representations (by selecting the first subword)
         origin_sequence_output = [layer[starts.nonzero().squeeze(1)] for layer, starts in zip(sequence_output, input_token_start_indexs)]
         padded_sequence_output = pad_sequence(origin_sequence_output, batch_first=True)
         padded_sequence_output = self.dropout(padded_sequence_output)
 
         ner_logits = self.ner_classifier(padded_sequence_output)
 
-        cls_logits = self.cls_classifier(sequence_output[:, 0, :]) # 分类任务
-        # cls_logits = self.cls_classifier(outputs[1]) # 分类任务
+        cls_logits = self.cls_classifier(sequence_output[:, 0, :])
 
         outputs = (ner_logits, cls_logits,)
 
         if ner_tags is not None:
-            alpha, beta = 1, 0 # alpha(0~1)控制两个任务的损失权重， beta控制额外引入的正则项
+            alpha = 0.3
             mask = ner_tags.gt(-1)
 
             loss_ner = self.crf(ner_logits, ner_tags, mask) * (-1)
             loss_cls = self.cel(cls_logits.view(-1, 2), cls_labels.view(-1))
-            loss_penalty = torch.mean((2 * torch.argmax(cls_logits, dim=-1) - 1.0) * torch.mean(ner_logits[:,:,-1], dim=-1))
-            loss = alpha * loss_ner + (1- alpha) * loss_cls + beta * loss_penalty
+            loss = alpha * loss_ner + (1- alpha) * loss_cls
 
             outputs = (loss,) + outputs
 
         return outputs
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `SciAssist-0.0.36/src/SciAssist/models/components/bert_token_classifier.py` & `SciAssist-0.0.37/src/SciAssist/models/components/bert_token_classifier.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.36/src/SciAssist/models/components/flant5_summarization.py` & `SciAssist-0.0.37/src/SciAssist/models/components/flant5_summarization.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.36/src/SciAssist/models/cora_module.py` & `SciAssist-0.0.37/src/SciAssist/models/cora_module.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.36/src/SciAssist/models/dataset_extraction_module.py` & `SciAssist-0.0.37/src/SciAssist/models/dataset_extraction_module.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.36/src/SciAssist/models/mup_bart_module.py` & `SciAssist-0.0.37/src/SciAssist/models/mup_bart_module.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.36/src/SciAssist/pipelines/__init__.py` & `SciAssist-0.0.37/src/SciAssist/pipelines/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,16 +6,15 @@
 
 from SciAssist import BASE_CACHE_DIR
 from SciAssist.models.components.bert_dataset_extraction import BertForDatasetExtraction
 from SciAssist.models.components.bert_token_classifier import BertForTokenClassifier
 from SciAssist.models.components.flant5_summarization import FlanT5ForSummarization
 from SciAssist.utils.data_utils import (
     DataUtilsForTokenClassification,
-    DataUtilsForFlanT5, DataUtilsForT5,
-    DataUtilsForSeq2Seq,
+    DataUtilsForFlanT5, DataUtilsForSeq2Seq,
     DataUtilsForDatasetExtraction
 )
 
 # Provided models for each task
 TASKS = {
     "reference-string-parsing": {
         "scibert-on-cora":  {
@@ -32,19 +31,14 @@
 
     "single-doc-summarization": {
         "default": {
             "model": FlanT5ForSummarization,
             "model_dict_url": "https://huggingface.co/spaces/dyxohjl666/Controlled-summarization/resolve/main/flant5-base-mup-scisumm-noctrl.pt",
             "data_utils": DataUtilsForSeq2Seq,
         },
-        # "t5": {
-        #     "model": FlanT5ForSummarization,
-        #     "model_dict_url": None,
-        #     "data_utils": DataUtilsForT5,
-        # },
         "flan-t5": {
             "model": FlanT5ForSummarization,
             "model_dict_url": "https://huggingface.co/spaces/dyxohjl666/Controlled-summarization/resolve/main/flant5-base-mup-scisumm-noctrl.pt",
             "data_utils": DataUtilsForFlanT5,
         }
     },
```

### Comparing `SciAssist-0.0.36/src/SciAssist/pipelines/dataset_extraction.py` & `SciAssist-0.0.37/src/SciAssist/pipelines/dataset_extraction.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.36/src/SciAssist/pipelines/pipeline.py` & `SciAssist-0.0.37/src/SciAssist/pipelines/pipeline.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.36/src/SciAssist/pipelines/reference_string_parsing.py` & `SciAssist-0.0.37/src/SciAssist/pipelines/reference_string_parsing.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.36/src/SciAssist/pipelines/summarization.py` & `SciAssist-0.0.37/src/SciAssist/pipelines/summarization.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
             cache_dir=None,
             output_dir=None,
             temp_dir=None,
             tokenizer=None,
             checkpoint="google/flan-t5-base",
             model_max_length=1024,
             max_source_length=1024,
-            max_target_length=500,
+            max_target_length=300,
             os_name=None,
     ):
         super().__init__(task_name=task_name, model_name=model_name, device=device,
                          cache_dir=cache_dir, output_dir=output_dir, temp_dir=temp_dir)
 
         self.data_utils = self.data_utils(
             tokenizer=tokenizer,
```

### Comparing `SciAssist-0.0.36/src/SciAssist/pipelines/testing_pipeline.py` & `SciAssist-0.0.37/src/SciAssist/pipelines/testing_pipeline.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.36/src/SciAssist/pipelines/training_pipeline.py` & `SciAssist-0.0.37/src/SciAssist/pipelines/training_pipeline.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.36/src/SciAssist/test.py` & `SciAssist-0.0.37/src/SciAssist/test.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.36/src/SciAssist/train.py` & `SciAssist-0.0.37/src/SciAssist/train.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.36/src/SciAssist/training_args.py` & `SciAssist-0.0.37/src/SciAssist/training_args.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.36/src/SciAssist/utils/__init__.py` & `SciAssist-0.0.37/src/SciAssist/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.36/src/SciAssist/utils/collators/CollatorForFid.py` & `SciAssist-0.0.37/src/SciAssist/utils/collators/CollatorForFid.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.36/src/SciAssist/utils/data_reader.py` & `SciAssist-0.0.37/src/SciAssist/utils/data_reader.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.36/src/SciAssist/utils/data_utils.py` & `SciAssist-0.0.37/src/SciAssist/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.36/src/SciAssist/utils/pdf2text.py` & `SciAssist-0.0.37/src/SciAssist/utils/pdf2text.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.36/src/SciAssist/utils/windows_pdf2text.py` & `SciAssist-0.0.37/src/SciAssist/utils/windows_pdf2text.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.36/src/SciAssist.egg-info/PKG-INFO` & `SciAssist-0.0.37/src/SciAssist.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SciAssist
-Version: 0.0.36
+Version: 0.0.37
 Summary: A toolkit for Scientific Document Processing
 Author-email: WING-NUS <dingyixi@hotmail.com>
 Maintainer-email: Yixi Ding <dingyixi@hotmail.com>
 License: Attribution-NonCommercial-ShareAlike 4.0 International
         
         =======================================================================
         
@@ -457,15 +457,15 @@
 
 **Documentation**
 - Move the definition of `Pipeline` class from `Usage` to `Contribution Guide`.
 - Add catalog for Contribution Guide.
 - Add examples for choosing devices in `Usage`.
 
 <div align="center">
-   
+
 # SciAssist
 [![PyPI Status](https://badge.fury.io/py/sciassist.svg)](https://badge.fury.io/py/sciassist)
 <a href="https://pytorch.org/get-started/locally/"><img alt="PyTorch" src="https://img.shields.io/badge/PyTorch-ee4c2c?logo=pytorch&logoColor=white"></a>
 <a href="https://pytorchlightning.ai/"><img alt="Lightning" src="https://img.shields.io/badge/-Lightning-792ee5?logo=pytorchlightning&logoColor=white"></a>
 <a href="https://hydra.cc/"><img alt="Config: Hydra" src="https://img.shields.io/badge/Config-Hydra-89b8cd"></a>
 <a href="https://github.com/ashleve/lightning-hydra-template"><img alt="Template" src="https://img.shields.io/badge/-Lightning--Hydra--Template-017F2F?style=flat&logo=github&labelColor=gray"></a><br>
 [![ReadTheDocs](https://readthedocs.org/projects/wing-sciassist/badge/)](https://wing-sciassist.readthedocs.io/en/latest/)
@@ -500,14 +500,15 @@
 
 
 ## Usage
 
 Here are some example usages.
 
 **Reference string parsing:**
+
 ```python
 from SciAssist import ReferenceStringParsing
 
 # Set device="cpu" if you want to use only CPU. The default device is "gpu".
 # ref_parser = ReferenceStringParsing(device="cpu")
 ref_parser = ReferenceStringParsing(device="gpu")
 
@@ -519,14 +520,15 @@
 # For text
 res  = ref_parser.predict("test.txt", type="txt")
 # For pdf
 res = ref_parser.predict("test.pdf")
 ```
 
 **Summarizarion for single document:**
+
 ```python
 from SciAssist import Summarization
 
 # Set device="cpu" if you want to use only CPU. The default device is "gpu".
 # pipleine = Summarization(device="cpu")
 summerizer = Summarization(device="gpu")
 
@@ -548,22 +550,42 @@
 # For text
 res = summerizer.predict("bodytext.txt", type="txt")
 # For pdf
 res = summerizer.predict("raw.pdf")
 
 ```
 
+**Dataset mention extraction:**
+
+```python
+from SciAssist import DatasetExtraction
+
+# Set device="cpu" if you want to use only CPU. The default device is "gpu".
+# ref_parser = DatasetExtraction(device="cpu")
+extractor = DatasetExtraction(device="gpu")
+
+# For string
+res = extractor.extract("The impact of gender identity on emotions was examined by researchers using a subsample from the National Longitudinal Study of Adolescent Health. The study aimed to investigate the direct effects of gender identity on emotional experiences and expression. By focusing on a subsample of the larger study, the researchers were able to hone in on the specific relationship between gender identity and emotions. Through their analysis, the researchers sought to determine whether gender identity could have a significant and direct impact on emotional well-being. The findings of the study have important implications for our understanding of the complex interplay between gender identity and emotional experiences, and may help to inform future interventions and support for individuals who experience gender-related emotional distress.", type="str")
+# For text: please input the path of your .txt file
+res = extractor.extract("test.txt", type="txt")
+# For pdf: please input the path of your .pdf file
+res = extractor.predict("test.pdf", type="pdf")
+```
+
+
+
 ## Contribution
+
 Here's a simple introduction about how to incorporate a new task into SciAssist. 
 Generally, to add a new task, you will need to:
 
     1. Git clone this repo and prepare the virtual environment.
     2. Install Grobid Server.
     3. Create a LightningModule and a DataLightningModule.
     4. Train a model.
     5. Provide a pipeline for users.
-    
+
 We provide a step-by-step contribution guide, see [SciAssist’s documentation](https://wing-sciassist.readthedocs.io/en/latest/Contribution.html#).
 
 ## LICENSE
 This toolkit is licensed under the `Attribution-NonCommercial-ShareAlike 4.0 International`.
 Read [LICENSE](https://github.com/WING-NUS/SciAssist/blob/main/LICENSE) for more information.
```

### Comparing `SciAssist-0.0.36/src/SciAssist.egg-info/SOURCES.txt` & `SciAssist-0.0.37/src/SciAssist.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
-src/process.py
 src/SciAssist/__init__.py
 src/SciAssist/test.py
 src/SciAssist/train.py
 src/SciAssist/training_args.py
 src/SciAssist.egg-info/PKG-INFO
 src/SciAssist.egg-info/SOURCES.txt
 src/SciAssist.egg-info/dependency_links.txt
@@ -52,27 +51,21 @@
 src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/__init__.cpython-38.pyc
 src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/citation_util.cpython-38.pyc
 src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/grobid_util.cpython-38.pyc
 src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/refspan_util.cpython-38.pyc
 src/SciAssist/bin/doc2json/scripts/run_grobid_linux.sh
 src/SciAssist/bin/doc2json/scripts/setup_grobid_linux.sh
 src/SciAssist/datamodules/__init__.py
-src/SciAssist/datamodules/acl_datamodule.py
 src/SciAssist/datamodules/cora_datamodule.py
 src/SciAssist/datamodules/dataset_extraction_datamodule.py
-src/SciAssist/datamodules/fid_datamodule.py
 src/SciAssist/datamodules/general_datamodule.py
-src/SciAssist/datamodules/longsumm_datamodule.py
 src/SciAssist/datamodules/mup_datamodule.py
-src/SciAssist/datamodules/mup_mup_datamodule.py
 src/SciAssist/datamodules/mup_scisumm_datamodule.py
 src/SciAssist/datamodules/mup_scisumm_noctrl_datamodule.py
-src/SciAssist/datamodules/scisumm_datamodule.py
 src/SciAssist/datamodules/test_datamodule.py
-src/SciAssist/datamodules/xsum_datamodule.py
 src/SciAssist/datamodules/components/__init__.py
 src/SciAssist/datamodules/components/cora_label.py
 src/SciAssist/models/__init__.py
 src/SciAssist/models/cora_module.py
 src/SciAssist/models/dataset_extraction_module.py
 src/SciAssist/models/mup_bart_module.py
 src/SciAssist/models/components/__init__.py
@@ -81,19 +74,20 @@
 src/SciAssist/models/components/bert_token_classifier.py
 src/SciAssist/models/components/flant5_summarization.py
 src/SciAssist/pipelines/__init__.py
 src/SciAssist/pipelines/dataset_extraction.py
 src/SciAssist/pipelines/pipeline.py
 src/SciAssist/pipelines/reference_string_parsing.py
 src/SciAssist/pipelines/summarization.py
+src/SciAssist/pipelines/summarization_origin.py
 src/SciAssist/pipelines/testing_pipeline.py
 src/SciAssist/pipelines/training_pipeline.py
 src/SciAssist/utils/__init__.py
 src/SciAssist/utils/data_reader.py
 src/SciAssist/utils/data_utils.py
-src/SciAssist/utils/extract_keywords_flant5.py
 src/SciAssist/utils/pdf2text.py
 src/SciAssist/utils/windows_pdf2text.py
+src/SciAssist/utils/xml2txt.py
 src/SciAssist/utils/collators/CollatorForFid.py
 src/SciAssist/utils/collators/__init__.py
 tests/test_rsp.py
 tests/test_summ.py
```

### Comparing `SciAssist-0.0.36/tests/test_rsp.py` & `SciAssist-0.0.37/tests/test_rsp.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.36/tests/test_summ.py` & `SciAssist-0.0.37/tests/test_summ.py`

 * *Files identical despite different names*

