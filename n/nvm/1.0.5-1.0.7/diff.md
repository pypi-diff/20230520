# Comparing `tmp/nvm-1.0.5.tar.gz` & `tmp/nvm-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvm-1.0.5.tar", last modified: Sat May 20 00:51:22 2023, max compression
+gzip compressed data, was "nvm-1.0.7.tar", last modified: Sat May 20 01:24:29 2023, max compression
```

## Comparing `nvm-1.0.5.tar` & `nvm-1.0.7.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.019164 nvm-1.0.5/
--rw-------   0 jiko      (1000) jiko      (1000)      292 2023-05-03 18:32:02.000000 nvm-1.0.5/.editorconfig
--rw-------   0 jiko      (1000) jiko      (1000)       29 2023-05-03 18:32:02.000000 nvm-1.0.5/.gitattributes
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.011164 nvm-1.0.5/.github/
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.011164 nvm-1.0.5/.github/ISSUE_TEMPLATE/
--rw-------   0 jiko      (1000) jiko      (1000)      348 2023-05-01 20:22:08.000000 nvm-1.0.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-------   0 jiko      (1000) jiko      (1000)      360 2023-05-01 20:22:08.000000 nvm-1.0.5/.github/ISSUE_TEMPLATE/feature_request.md
--rw-------   0 jiko      (1000) jiko      (1000)      446 2023-05-01 20:22:08.000000 nvm-1.0.5/.github/PULL_REQUEST_TEMPLATE.md
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.011164 nvm-1.0.5/.github/workflows/
--rw-------   0 jiko      (1000) jiko      (1000)      961 2023-05-05 21:24:14.000000 nvm-1.0.5/.github/workflows/build-main.yml
--rw-------   0 jiko      (1000) jiko      (1000)     1249 2023-05-04 01:10:13.000000 nvm-1.0.5/.gitignore
--rw-rw-r--   0 jiko      (1000) jiko      (1000)      716 2023-05-05 19:23:38.000000 nvm-1.0.5/.readthedocs.yaml
--rw-------   0 jiko      (1000) jiko      (1000)      151 2023-05-03 18:32:02.000000 nvm-1.0.5/AUTHORS.rst
--rw-------   0 jiko      (1000) jiko      (1000)     3466 2023-05-03 18:32:02.000000 nvm-1.0.5/CONTRIBUTING.rst
--rw-------   0 jiko      (1000) jiko      (1000)       69 2023-05-05 23:01:31.000000 nvm-1.0.5/HISTORY.rst
--rw-------   0 jiko      (1000) jiko      (1000)     1534 2023-05-03 18:32:02.000000 nvm-1.0.5/LICENSE
--rw-------   0 jiko      (1000) jiko      (1000)      460 2023-05-20 00:40:26.000000 nvm-1.0.5/MANIFEST.in
--rw-rw-r--   0 jiko      (1000) jiko      (1000)     3140 2023-05-20 00:43:36.000000 nvm-1.0.5/Makefile
--rw-------   0 jiko      (1000) jiko      (1000)     2000 2023-05-20 00:51:22.019164 nvm-1.0.5/PKG-INFO
--rw-------   0 jiko      (1000) jiko      (1000)     1205 2023-05-05 23:20:54.000000 nvm-1.0.5/README.rst
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.011164 nvm-1.0.5/docs/
--rw-------   0 jiko      (1000) jiko      (1000)      612 2023-05-14 21:15:09.000000 nvm-1.0.5/docs/Makefile
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.011164 nvm-1.0.5/docs/build/
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.011164 nvm-1.0.5/docs/build/html/
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.015164 nvm-1.0.5/docs/build/html/_static/
--rw-------   0 jiko      (1000) jiko      (1000)      313 2023-05-04 17:45:22.000000 nvm-1.0.5/docs/build/html/_static/check-solid.svg
--rw-------   0 jiko      (1000) jiko      (1000)      411 2023-05-04 17:45:22.000000 nvm-1.0.5/docs/build/html/_static/copy-button.svg
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.011164 nvm-1.0.5/docs/build/html/_static/css/
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.015164 nvm-1.0.5/docs/build/html/_static/css/fonts/
--rw-------   0 jiko      (1000) jiko      (1000)   444379 2023-05-04 17:45:23.000000 nvm-1.0.5/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-------   0 jiko      (1000) jiko      (1000)      286 2023-05-04 17:45:09.000000 nvm-1.0.5/docs/build/html/_static/file.png
--rw-------   0 jiko      (1000) jiko      (1000)       90 2023-05-04 17:45:09.000000 nvm-1.0.5/docs/build/html/_static/minus.png
--rw-------   0 jiko      (1000) jiko      (1000)       90 2023-05-04 17:45:09.000000 nvm-1.0.5/docs/build/html/_static/plus.png
--rw-------   0 jiko      (1000) jiko      (1000)      588 2023-05-05 19:42:21.000000 nvm-1.0.5/docs/requirements.txt
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.015164 nvm-1.0.5/docs/source/
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.015164 nvm-1.0.5/docs/source/_static/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-03 18:32:02.000000 nvm-1.0.5/docs/source/_static/.gitkeep
--rw-------   0 jiko      (1000) jiko      (1000)       31 2023-05-03 18:32:02.000000 nvm-1.0.5/docs/source/authors.rst
--rwx------   0 jiko      (1000) jiko      (1000)     5572 2023-05-14 23:09:27.000000 nvm-1.0.5/docs/source/conf.py
--rw-------   0 jiko      (1000) jiko      (1000)       36 2023-05-03 18:32:02.000000 nvm-1.0.5/docs/source/contributing.rst
--rw-------   0 jiko      (1000) jiko      (1000)       31 2023-05-03 18:32:02.000000 nvm-1.0.5/docs/source/history.rst
--rw-------   0 jiko      (1000) jiko      (1000)      319 2023-05-14 22:54:59.000000 nvm-1.0.5/docs/source/index.rst
--rw-------   0 jiko      (1000) jiko      (1000)     1086 2023-05-03 18:32:02.000000 nvm-1.0.5/docs/source/installation.rst
--rw-------   0 jiko      (1000) jiko      (1000)       46 2023-05-20 00:50:52.000000 nvm-1.0.5/docs/source/modules.rst
--rw-------   0 jiko      (1000) jiko      (1000)      331 2023-05-20 00:50:51.000000 nvm-1.0.5/docs/source/nvm.aux_log.rst
--rw-------   0 jiko      (1000) jiko      (1000)      358 2023-05-20 00:50:51.000000 nvm-1.0.5/docs/source/nvm.aux_pandas.rst
--rw-------   0 jiko      (1000) jiko      (1000)      230 2023-05-20 00:50:52.000000 nvm-1.0.5/docs/source/nvm.aux_spacy.data.NicolasEtAl2019a.rst
--rw-------   0 jiko      (1000) jiko      (1000)      239 2023-05-20 00:50:52.000000 nvm-1.0.5/docs/source/nvm.aux_spacy.data.PennebakerEtAl2015a.rst
--rw-------   0 jiko      (1000) jiko      (1000)      254 2023-05-20 00:50:52.000000 nvm-1.0.5/docs/source/nvm.aux_spacy.data.PietraszkiewiczEtAl2019a.rst
--rw-------   0 jiko      (1000) jiko      (1000)      363 2023-05-20 00:50:51.000000 nvm-1.0.5/docs/source/nvm.aux_spacy.data.rst
--rw-------   0 jiko      (1000) jiko      (1000)     1373 2023-05-20 00:50:52.000000 nvm-1.0.5/docs/source/nvm.aux_spacy.factories.rst
--rw-------   0 jiko      (1000) jiko      (1000)      663 2023-05-20 00:50:51.000000 nvm-1.0.5/docs/source/nvm.aux_spacy.rst
--rw-------   0 jiko      (1000) jiko      (1000)      349 2023-05-20 00:50:52.000000 nvm-1.0.5/docs/source/nvm.aux_srsly.rst
--rw-------   0 jiko      (1000) jiko      (1000)      658 2023-05-20 00:50:52.000000 nvm-1.0.5/docs/source/nvm.aux_str.rst
--rw-------   0 jiko      (1000) jiko      (1000)      331 2023-05-20 00:50:52.000000 nvm-1.0.5/docs/source/nvm.aux_sys.rst
--rw-------   0 jiko      (1000) jiko      (1000)      289 2023-05-20 00:50:52.000000 nvm-1.0.5/docs/source/nvm.cli.rst
--rw-------   0 jiko      (1000) jiko      (1000)      442 2023-05-20 00:50:51.000000 nvm-1.0.5/docs/source/nvm.rst
--rw-------   0 jiko      (1000) jiko      (1000)      642 2023-05-20 00:50:52.000000 nvm-1.0.5/docs/source/nvm.tests.rst
--rw-------   0 jiko      (1000) jiko      (1000)       30 2023-05-03 18:32:02.000000 nvm-1.0.5/docs/source/readme.rst
--rw-------   0 jiko      (1000) jiko      (1000)       61 2023-05-03 18:32:02.000000 nvm-1.0.5/docs/source/usage.rst
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.019164 nvm-1.0.5/nvm/
--rw-------   0 jiko      (1000) jiko      (1000)      885 2023-05-19 23:56:36.000000 nvm-1.0.5/nvm/__init__.py
--rw-------   0 jiko      (1000) jiko      (1000)      497 2023-05-20 00:51:22.019164 nvm-1.0.5/nvm/_version.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.015164 nvm-1.0.5/nvm/aux_log/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)       51 2023-05-04 00:33:55.000000 nvm-1.0.5/nvm/aux_log/__init__.py
--rw-rw-r--   0 jiko      (1000) jiko      (1000)     5073 2023-05-04 01:17:45.000000 nvm-1.0.5/nvm/aux_log/aux_log.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.015164 nvm-1.0.5/nvm/aux_pandas/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)      137 2023-05-09 09:25:31.000000 nvm-1.0.5/nvm/aux_pandas/__init__.py
--rw-rw-r--   0 jiko      (1000) jiko      (1000)     1993 2023-05-09 09:31:34.000000 nvm-1.0.5/nvm/aux_pandas/aux_pandas.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.015164 nvm-1.0.5/nvm/aux_spacy/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)      489 2023-05-19 23:05:08.000000 nvm-1.0.5/nvm/aux_spacy/__init__.py
--rw-rw-r--   0 jiko      (1000) jiko      (1000)       23 2023-05-19 23:02:54.000000 nvm-1.0.5/nvm/aux_spacy/aux_spacy.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.015164 nvm-1.0.5/nvm/aux_spacy/data/
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.015164 nvm-1.0.5/nvm/aux_spacy/data/NicolasEtAl2019a/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)      396 2023-05-19 22:51:19.000000 nvm-1.0.5/nvm/aux_spacy/data/NicolasEtAl2019a/__init__.py
--rw-------   0 jiko      (1000) jiko      (1000)    47658 2022-03-18 04:48:30.000000 nvm-1.0.5/nvm/aux_spacy/data/NicolasEtAl2019a/data.json
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.015164 nvm-1.0.5/nvm/aux_spacy/data/PennebakerEtAl2015a/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)       43 2023-05-19 21:19:19.000000 nvm-1.0.5/nvm/aux_spacy/data/PennebakerEtAl2015a/.gitignore
--rw-rw-r--   0 jiko      (1000) jiko      (1000)      944 2023-05-20 00:32:47.000000 nvm-1.0.5/nvm/aux_spacy/data/PennebakerEtAl2015a/__init__.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.015164 nvm-1.0.5/nvm/aux_spacy/data/PietraszkiewiczEtAl2019a/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)      553 2023-05-19 22:52:48.000000 nvm-1.0.5/nvm/aux_spacy/data/PietraszkiewiczEtAl2019a/__init__.py
--rw-rw-r--   0 jiko      (1000) jiko      (1000)    13614 2023-05-13 01:10:01.000000 nvm-1.0.5/nvm/aux_spacy/data/PietraszkiewiczEtAl2019a/data.json
--rw-------   0 jiko      (1000) jiko      (1000)    32392 2022-03-18 05:27:49.000000 nvm-1.0.5/nvm/aux_spacy/data/PietraszkiewiczEtAl2019a/data_liwc.json
--rw-rw-r--   0 jiko      (1000) jiko      (1000)       23 2023-05-14 19:16:37.000000 nvm-1.0.5/nvm/aux_spacy/data/__init__.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.015164 nvm-1.0.5/nvm/aux_spacy/factories/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)       23 2023-05-15 01:52:05.000000 nvm-1.0.5/nvm/aux_spacy/factories/__init__.py
--rw-rw-r--   0 jiko      (1000) jiko      (1000)     6033 2023-05-20 00:18:54.000000 nvm-1.0.5/nvm/aux_spacy/factories/get_doc_basic_metrics.py
--rw-rw-r--   0 jiko      (1000) jiko      (1000)     8091 2023-05-20 00:18:16.000000 nvm-1.0.5/nvm/aux_spacy/factories/get_doc_count_of_dict_items.py
--rw-------   0 jiko      (1000) jiko      (1000)     1786 2023-05-14 22:44:24.000000 nvm-1.0.5/nvm/aux_spacy/factories/get_doc_sentences.py
--rw-rw-r--   0 jiko      (1000) jiko      (1000)     2462 2023-05-20 00:30:58.000000 nvm-1.0.5/nvm/aux_spacy/factories/get_doc_summary_dict.py
--rw-rw-r--   0 jiko      (1000) jiko      (1000)     1564 2023-05-14 23:53:03.000000 nvm-1.0.5/nvm/aux_spacy/factories/get_doc_word_count.py
--rw-rw-r--   0 jiko      (1000) jiko      (1000)     3736 2023-05-20 00:13:47.000000 nvm-1.0.5/nvm/aux_spacy/set_container_extensions.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.015164 nvm-1.0.5/nvm/aux_srsly/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)       73 2023-05-19 23:56:47.000000 nvm-1.0.5/nvm/aux_srsly/__init__.py
--rw-rw-r--   0 jiko      (1000) jiko      (1000)     1691 2023-05-20 00:21:53.000000 nvm-1.0.5/nvm/aux_srsly/aux_srsly.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.015164 nvm-1.0.5/nvm/aux_str/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)      370 2023-05-16 08:02:31.000000 nvm-1.0.5/nvm/aux_str/__init__.py
--rw-rw-r--   0 jiko      (1000) jiko      (1000)     6834 2023-05-19 23:26:41.000000 nvm-1.0.5/nvm/aux_str/aux_str.py
--rw-rw-r--   0 jiko      (1000) jiko      (1000)     2083 2023-05-16 07:59:44.000000 nvm-1.0.5/nvm/aux_str/clean_str_mappings.py
--rw-rw-r--   0 jiko      (1000) jiko      (1000)      140 2023-05-07 02:51:21.000000 nvm-1.0.5/nvm/aux_str/regex.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.015164 nvm-1.0.5/nvm/aux_sys/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)       80 2023-05-12 14:03:28.000000 nvm-1.0.5/nvm/aux_sys/__init__.py
--rw-rw-r--   0 jiko      (1000) jiko      (1000)     2054 2023-05-12 14:08:28.000000 nvm-1.0.5/nvm/aux_sys/aux_sys.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.015164 nvm-1.0.5/nvm/cli/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-03 18:32:02.000000 nvm-1.0.5/nvm/cli/.gitkeep
--rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-06 09:19:24.000000 nvm-1.0.5/nvm/cli/__init__.py
--rw-------   0 jiko      (1000) jiko      (1000)      429 2023-05-12 04:26:04.000000 nvm-1.0.5/nvm/cli/nvm.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.015164 nvm-1.0.5/nvm/data/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-03 18:32:02.000000 nvm-1.0.5/nvm/data/.gitkeep
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.019164 nvm-1.0.5/nvm/data/emacs-logo/
--rw-------   0 jiko      (1000) jiko      (1000)     9818 2023-05-03 18:32:02.000000 nvm-1.0.5/nvm/data/emacs-logo/emacs-128x128.png
--rw-rw-r--   0 jiko      (1000) jiko      (1000)    13358 2023-05-03 18:32:02.000000 nvm-1.0.5/nvm/data/emacs-logo/emacs.svg
--rw-------   0 jiko      (1000) jiko      (1000)       66 2023-05-03 18:32:02.000000 nvm-1.0.5/nvm/nvm.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.019164 nvm-1.0.5/nvm/tests/
--rw-------   0 jiko      (1000) jiko      (1000)       28 2023-05-06 10:03:21.000000 nvm-1.0.5/nvm/tests/__init__.py
--rw-rw-r--   0 jiko      (1000) jiko      (1000)     6136 2023-05-20 00:11:39.000000 nvm-1.0.5/nvm/tests/test_aux_spacy.py
--rw-rw-r--   0 jiko      (1000) jiko      (1000)     2538 2023-05-14 19:32:09.000000 nvm-1.0.5/nvm/tests/test_aux_str.py
--rw-------   0 jiko      (1000) jiko      (1000)      554 2023-05-05 13:11:09.000000 nvm-1.0.5/nvm/tests/test_nvm.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.015164 nvm-1.0.5/nvm.egg-info/
--rw-------   0 jiko      (1000) jiko      (1000)     2000 2023-05-20 00:51:21.000000 nvm-1.0.5/nvm.egg-info/PKG-INFO
--rw-------   0 jiko      (1000) jiko      (1000)     2910 2023-05-20 00:51:22.000000 nvm-1.0.5/nvm.egg-info/SOURCES.txt
--rw-------   0 jiko      (1000) jiko      (1000)        1 2023-05-20 00:51:21.000000 nvm-1.0.5/nvm.egg-info/dependency_links.txt
--rw-------   0 jiko      (1000) jiko      (1000)       41 2023-05-20 00:51:21.000000 nvm-1.0.5/nvm.egg-info/entry_points.txt
--rw-------   0 jiko      (1000) jiko      (1000)        1 2023-05-20 00:51:21.000000 nvm-1.0.5/nvm.egg-info/not-zip-safe
--rw-------   0 jiko      (1000) jiko      (1000)     1013 2023-05-20 00:51:21.000000 nvm-1.0.5/nvm.egg-info/requires.txt
--rw-------   0 jiko      (1000) jiko      (1000)        4 2023-05-20 00:51:21.000000 nvm-1.0.5/nvm.egg-info/top_level.txt
--rw-rw-r--   0 jiko      (1000) jiko      (1000)      755 2023-05-03 18:32:02.000000 nvm-1.0.5/pyproject.toml
--rw-------   0 jiko      (1000) jiko      (1000)      494 2023-05-05 21:20:43.000000 nvm-1.0.5/requirements_dev.txt
--rw-------   0 jiko      (1000) jiko      (1000)      739 2023-05-20 00:51:22.019164 nvm-1.0.5/setup.cfg
--rw-------   0 jiko      (1000) jiko      (1000)     2592 2023-05-06 10:12:14.000000 nvm-1.0.5/setup.py
--rw-------   0 jiko      (1000) jiko      (1000)      493 2023-05-05 23:16:08.000000 nvm-1.0.5/tox.ini
--rw-------   0 jiko      (1000) jiko      (1000)    83607 2023-05-03 18:32:02.000000 nvm-1.0.5/versioneer.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 01:24:29.268806 nvm-1.0.7/
+-rw-------   0 jiko      (1000) jiko      (1000)      292 2023-05-03 18:32:02.000000 nvm-1.0.7/.editorconfig
+-rw-------   0 jiko      (1000) jiko      (1000)       29 2023-05-03 18:32:02.000000 nvm-1.0.7/.gitattributes
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 01:24:29.264806 nvm-1.0.7/.github/
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 01:24:29.264806 nvm-1.0.7/.github/ISSUE_TEMPLATE/
+-rw-------   0 jiko      (1000) jiko      (1000)      348 2023-05-01 20:22:08.000000 nvm-1.0.7/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-------   0 jiko      (1000) jiko      (1000)      360 2023-05-01 20:22:08.000000 nvm-1.0.7/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-------   0 jiko      (1000) jiko      (1000)      446 2023-05-01 20:22:08.000000 nvm-1.0.7/.github/PULL_REQUEST_TEMPLATE.md
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 01:24:29.264806 nvm-1.0.7/.github/workflows/
+-rw-------   0 jiko      (1000) jiko      (1000)      961 2023-05-05 21:24:14.000000 nvm-1.0.7/.github/workflows/build-main.yml
+-rw-------   0 jiko      (1000) jiko      (1000)     1249 2023-05-04 01:10:13.000000 nvm-1.0.7/.gitignore
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)      716 2023-05-05 19:23:38.000000 nvm-1.0.7/.readthedocs.yaml
+-rw-------   0 jiko      (1000) jiko      (1000)      151 2023-05-03 18:32:02.000000 nvm-1.0.7/AUTHORS.rst
+-rw-------   0 jiko      (1000) jiko      (1000)     3466 2023-05-03 18:32:02.000000 nvm-1.0.7/CONTRIBUTING.rst
+-rw-------   0 jiko      (1000) jiko      (1000)       69 2023-05-05 23:01:31.000000 nvm-1.0.7/HISTORY.rst
+-rw-------   0 jiko      (1000) jiko      (1000)     1534 2023-05-03 18:32:02.000000 nvm-1.0.7/LICENSE
+-rw-------   0 jiko      (1000) jiko      (1000)      460 2023-05-20 00:40:26.000000 nvm-1.0.7/MANIFEST.in
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)     3140 2023-05-20 00:43:36.000000 nvm-1.0.7/Makefile
+-rw-------   0 jiko      (1000) jiko      (1000)     2000 2023-05-20 01:24:29.268806 nvm-1.0.7/PKG-INFO
+-rw-------   0 jiko      (1000) jiko      (1000)     1205 2023-05-05 23:20:54.000000 nvm-1.0.7/README.rst
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 01:24:29.264806 nvm-1.0.7/docs/
+-rw-------   0 jiko      (1000) jiko      (1000)      612 2023-05-14 21:15:09.000000 nvm-1.0.7/docs/Makefile
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 01:24:29.260806 nvm-1.0.7/docs/build/
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 01:24:29.260806 nvm-1.0.7/docs/build/html/
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 01:24:29.264806 nvm-1.0.7/docs/build/html/_static/
+-rw-------   0 jiko      (1000) jiko      (1000)      313 2023-05-04 17:45:22.000000 nvm-1.0.7/docs/build/html/_static/check-solid.svg
+-rw-------   0 jiko      (1000) jiko      (1000)      411 2023-05-04 17:45:22.000000 nvm-1.0.7/docs/build/html/_static/copy-button.svg
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 01:24:29.260806 nvm-1.0.7/docs/build/html/_static/css/
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 01:24:29.264806 nvm-1.0.7/docs/build/html/_static/css/fonts/
+-rw-------   0 jiko      (1000) jiko      (1000)   444379 2023-05-04 17:45:23.000000 nvm-1.0.7/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-------   0 jiko      (1000) jiko      (1000)      286 2023-05-04 17:45:09.000000 nvm-1.0.7/docs/build/html/_static/file.png
+-rw-------   0 jiko      (1000) jiko      (1000)       90 2023-05-04 17:45:09.000000 nvm-1.0.7/docs/build/html/_static/minus.png
+-rw-------   0 jiko      (1000) jiko      (1000)       90 2023-05-04 17:45:09.000000 nvm-1.0.7/docs/build/html/_static/plus.png
+-rw-------   0 jiko      (1000) jiko      (1000)      610 2023-05-20 01:16:35.000000 nvm-1.0.7/docs/requirements.txt
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 01:24:29.264806 nvm-1.0.7/docs/source/
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 01:24:29.264806 nvm-1.0.7/docs/source/_static/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-03 18:32:02.000000 nvm-1.0.7/docs/source/_static/.gitkeep
+-rw-------   0 jiko      (1000) jiko      (1000)       31 2023-05-03 18:32:02.000000 nvm-1.0.7/docs/source/authors.rst
+-rwx------   0 jiko      (1000) jiko      (1000)     5572 2023-05-14 23:09:27.000000 nvm-1.0.7/docs/source/conf.py
+-rw-------   0 jiko      (1000) jiko      (1000)       36 2023-05-03 18:32:02.000000 nvm-1.0.7/docs/source/contributing.rst
+-rw-------   0 jiko      (1000) jiko      (1000)       31 2023-05-03 18:32:02.000000 nvm-1.0.7/docs/source/history.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      319 2023-05-14 22:54:59.000000 nvm-1.0.7/docs/source/index.rst
+-rw-------   0 jiko      (1000) jiko      (1000)     1086 2023-05-03 18:32:02.000000 nvm-1.0.7/docs/source/installation.rst
+-rw-------   0 jiko      (1000) jiko      (1000)       46 2023-05-20 00:50:52.000000 nvm-1.0.7/docs/source/modules.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      331 2023-05-20 00:50:51.000000 nvm-1.0.7/docs/source/nvm.aux_log.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      358 2023-05-20 00:50:51.000000 nvm-1.0.7/docs/source/nvm.aux_pandas.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      230 2023-05-20 00:50:52.000000 nvm-1.0.7/docs/source/nvm.aux_spacy.data.NicolasEtAl2019a.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      239 2023-05-20 00:50:52.000000 nvm-1.0.7/docs/source/nvm.aux_spacy.data.PennebakerEtAl2015a.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      254 2023-05-20 00:50:52.000000 nvm-1.0.7/docs/source/nvm.aux_spacy.data.PietraszkiewiczEtAl2019a.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      363 2023-05-20 00:50:51.000000 nvm-1.0.7/docs/source/nvm.aux_spacy.data.rst
+-rw-------   0 jiko      (1000) jiko      (1000)     1373 2023-05-20 00:50:52.000000 nvm-1.0.7/docs/source/nvm.aux_spacy.factories.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      663 2023-05-20 00:50:51.000000 nvm-1.0.7/docs/source/nvm.aux_spacy.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      349 2023-05-20 00:50:52.000000 nvm-1.0.7/docs/source/nvm.aux_srsly.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      658 2023-05-20 00:50:52.000000 nvm-1.0.7/docs/source/nvm.aux_str.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      331 2023-05-20 00:50:52.000000 nvm-1.0.7/docs/source/nvm.aux_sys.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      289 2023-05-20 00:50:52.000000 nvm-1.0.7/docs/source/nvm.cli.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      442 2023-05-20 00:50:51.000000 nvm-1.0.7/docs/source/nvm.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      642 2023-05-20 00:50:52.000000 nvm-1.0.7/docs/source/nvm.tests.rst
+-rw-------   0 jiko      (1000) jiko      (1000)       30 2023-05-03 18:32:02.000000 nvm-1.0.7/docs/source/readme.rst
+-rw-------   0 jiko      (1000) jiko      (1000)       61 2023-05-03 18:32:02.000000 nvm-1.0.7/docs/source/usage.rst
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 01:24:29.268806 nvm-1.0.7/nvm/
+-rw-------   0 jiko      (1000) jiko      (1000)      885 2023-05-19 23:56:36.000000 nvm-1.0.7/nvm/__init__.py
+-rw-------   0 jiko      (1000) jiko      (1000)      497 2023-05-20 01:24:29.268806 nvm-1.0.7/nvm/_version.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 01:24:29.264806 nvm-1.0.7/nvm/aux_log/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)       51 2023-05-04 00:33:55.000000 nvm-1.0.7/nvm/aux_log/__init__.py
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)     5073 2023-05-04 01:17:45.000000 nvm-1.0.7/nvm/aux_log/aux_log.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 01:24:29.264806 nvm-1.0.7/nvm/aux_pandas/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)      137 2023-05-09 09:25:31.000000 nvm-1.0.7/nvm/aux_pandas/__init__.py
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)     1993 2023-05-09 09:31:34.000000 nvm-1.0.7/nvm/aux_pandas/aux_pandas.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 01:24:29.264806 nvm-1.0.7/nvm/aux_spacy/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)      489 2023-05-19 23:05:08.000000 nvm-1.0.7/nvm/aux_spacy/__init__.py
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)       23 2023-05-19 23:02:54.000000 nvm-1.0.7/nvm/aux_spacy/aux_spacy.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 01:24:29.264806 nvm-1.0.7/nvm/aux_spacy/data/
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 01:24:29.268806 nvm-1.0.7/nvm/aux_spacy/data/NicolasEtAl2019a/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)      396 2023-05-19 22:51:19.000000 nvm-1.0.7/nvm/aux_spacy/data/NicolasEtAl2019a/__init__.py
+-rw-------   0 jiko      (1000) jiko      (1000)    47658 2022-03-18 04:48:30.000000 nvm-1.0.7/nvm/aux_spacy/data/NicolasEtAl2019a/data.json
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 01:24:29.268806 nvm-1.0.7/nvm/aux_spacy/data/PennebakerEtAl2015a/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)       43 2023-05-19 21:19:19.000000 nvm-1.0.7/nvm/aux_spacy/data/PennebakerEtAl2015a/.gitignore
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)      944 2023-05-20 00:32:47.000000 nvm-1.0.7/nvm/aux_spacy/data/PennebakerEtAl2015a/__init__.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 01:24:29.268806 nvm-1.0.7/nvm/aux_spacy/data/PietraszkiewiczEtAl2019a/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)      553 2023-05-19 22:52:48.000000 nvm-1.0.7/nvm/aux_spacy/data/PietraszkiewiczEtAl2019a/__init__.py
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)    13614 2023-05-13 01:10:01.000000 nvm-1.0.7/nvm/aux_spacy/data/PietraszkiewiczEtAl2019a/data.json
+-rw-------   0 jiko      (1000) jiko      (1000)    32392 2022-03-18 05:27:49.000000 nvm-1.0.7/nvm/aux_spacy/data/PietraszkiewiczEtAl2019a/data_liwc.json
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)       23 2023-05-14 19:16:37.000000 nvm-1.0.7/nvm/aux_spacy/data/__init__.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 01:24:29.268806 nvm-1.0.7/nvm/aux_spacy/factories/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)       23 2023-05-15 01:52:05.000000 nvm-1.0.7/nvm/aux_spacy/factories/__init__.py
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)     6033 2023-05-20 00:18:54.000000 nvm-1.0.7/nvm/aux_spacy/factories/get_doc_basic_metrics.py
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)     8091 2023-05-20 00:18:16.000000 nvm-1.0.7/nvm/aux_spacy/factories/get_doc_count_of_dict_items.py
+-rw-------   0 jiko      (1000) jiko      (1000)     1786 2023-05-14 22:44:24.000000 nvm-1.0.7/nvm/aux_spacy/factories/get_doc_sentences.py
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)     2462 2023-05-20 00:30:58.000000 nvm-1.0.7/nvm/aux_spacy/factories/get_doc_summary_dict.py
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)     1564 2023-05-14 23:53:03.000000 nvm-1.0.7/nvm/aux_spacy/factories/get_doc_word_count.py
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)     3736 2023-05-20 00:13:47.000000 nvm-1.0.7/nvm/aux_spacy/set_container_extensions.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 01:24:29.268806 nvm-1.0.7/nvm/aux_srsly/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)       73 2023-05-19 23:56:47.000000 nvm-1.0.7/nvm/aux_srsly/__init__.py
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)     1691 2023-05-20 00:21:53.000000 nvm-1.0.7/nvm/aux_srsly/aux_srsly.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 01:24:29.268806 nvm-1.0.7/nvm/aux_str/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)      370 2023-05-16 08:02:31.000000 nvm-1.0.7/nvm/aux_str/__init__.py
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)     6834 2023-05-19 23:26:41.000000 nvm-1.0.7/nvm/aux_str/aux_str.py
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)     2083 2023-05-16 07:59:44.000000 nvm-1.0.7/nvm/aux_str/clean_str_mappings.py
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)      140 2023-05-07 02:51:21.000000 nvm-1.0.7/nvm/aux_str/regex.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 01:24:29.268806 nvm-1.0.7/nvm/aux_sys/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)       80 2023-05-12 14:03:28.000000 nvm-1.0.7/nvm/aux_sys/__init__.py
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)     2054 2023-05-12 14:08:28.000000 nvm-1.0.7/nvm/aux_sys/aux_sys.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 01:24:29.268806 nvm-1.0.7/nvm/cli/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-03 18:32:02.000000 nvm-1.0.7/nvm/cli/.gitkeep
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-06 09:19:24.000000 nvm-1.0.7/nvm/cli/__init__.py
+-rw-------   0 jiko      (1000) jiko      (1000)      429 2023-05-12 04:26:04.000000 nvm-1.0.7/nvm/cli/nvm.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 01:24:29.268806 nvm-1.0.7/nvm/data/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-03 18:32:02.000000 nvm-1.0.7/nvm/data/.gitkeep
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 01:24:29.268806 nvm-1.0.7/nvm/data/emacs-logo/
+-rw-------   0 jiko      (1000) jiko      (1000)     9818 2023-05-03 18:32:02.000000 nvm-1.0.7/nvm/data/emacs-logo/emacs-128x128.png
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)    13358 2023-05-03 18:32:02.000000 nvm-1.0.7/nvm/data/emacs-logo/emacs.svg
+-rw-------   0 jiko      (1000) jiko      (1000)       66 2023-05-03 18:32:02.000000 nvm-1.0.7/nvm/nvm.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 01:24:29.268806 nvm-1.0.7/nvm/tests/
+-rw-------   0 jiko      (1000) jiko      (1000)       28 2023-05-06 10:03:21.000000 nvm-1.0.7/nvm/tests/__init__.py
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)     6136 2023-05-20 00:11:39.000000 nvm-1.0.7/nvm/tests/test_aux_spacy.py
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)     2538 2023-05-14 19:32:09.000000 nvm-1.0.7/nvm/tests/test_aux_str.py
+-rw-------   0 jiko      (1000) jiko      (1000)      554 2023-05-05 13:11:09.000000 nvm-1.0.7/nvm/tests/test_nvm.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 01:24:29.264806 nvm-1.0.7/nvm.egg-info/
+-rw-------   0 jiko      (1000) jiko      (1000)     2000 2023-05-20 01:24:29.000000 nvm-1.0.7/nvm.egg-info/PKG-INFO
+-rw-------   0 jiko      (1000) jiko      (1000)     2910 2023-05-20 01:24:29.000000 nvm-1.0.7/nvm.egg-info/SOURCES.txt
+-rw-------   0 jiko      (1000) jiko      (1000)        1 2023-05-20 01:24:29.000000 nvm-1.0.7/nvm.egg-info/dependency_links.txt
+-rw-------   0 jiko      (1000) jiko      (1000)       41 2023-05-20 01:24:29.000000 nvm-1.0.7/nvm.egg-info/entry_points.txt
+-rw-------   0 jiko      (1000) jiko      (1000)        1 2023-05-20 01:24:29.000000 nvm-1.0.7/nvm.egg-info/not-zip-safe
+-rw-------   0 jiko      (1000) jiko      (1000)     1013 2023-05-20 01:24:29.000000 nvm-1.0.7/nvm.egg-info/requires.txt
+-rw-------   0 jiko      (1000) jiko      (1000)        4 2023-05-20 01:24:29.000000 nvm-1.0.7/nvm.egg-info/top_level.txt
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)      755 2023-05-03 18:32:02.000000 nvm-1.0.7/pyproject.toml
+-rw-------   0 jiko      (1000) jiko      (1000)      507 2023-05-20 00:54:31.000000 nvm-1.0.7/requirements_dev.txt
+-rw-------   0 jiko      (1000) jiko      (1000)      739 2023-05-20 01:24:29.268806 nvm-1.0.7/setup.cfg
+-rw-------   0 jiko      (1000) jiko      (1000)     2592 2023-05-06 10:12:14.000000 nvm-1.0.7/setup.py
+-rw-------   0 jiko      (1000) jiko      (1000)      493 2023-05-05 23:16:08.000000 nvm-1.0.7/tox.ini
+-rw-------   0 jiko      (1000) jiko      (1000)    83607 2023-05-03 18:32:02.000000 nvm-1.0.7/versioneer.py
```

### Comparing `nvm-1.0.5/.github/workflows/build-main.yml` & `nvm-1.0.7/.github/workflows/build-main.yml`

 * *Files identical despite different names*

### Comparing `nvm-1.0.5/.gitignore` & `nvm-1.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `nvm-1.0.5/.readthedocs.yaml` & `nvm-1.0.7/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `nvm-1.0.5/CONTRIBUTING.rst` & `nvm-1.0.7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nvm-1.0.5/LICENSE` & `nvm-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nvm-1.0.5/Makefile` & `nvm-1.0.7/Makefile`

 * *Files identical despite different names*

### Comparing `nvm-1.0.5/PKG-INFO` & `nvm-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvm
-Version: 1.0.5
+Version: 1.0.7
 Summary: Plenty little helpers.
 Home-page: https://github.com/cogsys-io/nvm
 Author: cogsys.io
 Author-email: cogsys@cogsys.io
 License: GNU General Public License v3
 Keywords: nvm
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nvm-1.0.5/README.rst` & `nvm-1.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `nvm-1.0.5/docs/Makefile` & `nvm-1.0.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nvm-1.0.5/docs/build/html/_static/css/fonts/fontawesome-webfont.svg` & `nvm-1.0.7/docs/build/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `nvm-1.0.5/docs/requirements.txt` & `nvm-1.0.7/docs/requirements.txt`

 * *Files 19% similar despite different names*

```diff
@@ -22,7 +22,11 @@
 tqdm>=4
 sphinx_copybutton>=0.5.2
 numpy>=1.24.3
 pandas>=2.0.1
 pytz>=2023.3
 scikit-learn
 ipython
+
+pytest
+
+spacy>=3.2.4
```

### Comparing `nvm-1.0.5/docs/source/conf.py` & `nvm-1.0.7/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nvm-1.0.5/docs/source/installation.rst` & `nvm-1.0.7/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `nvm-1.0.5/docs/source/nvm.aux_spacy.factories.rst` & `nvm-1.0.7/docs/source/nvm.aux_spacy.factories.rst`

 * *Files identical despite different names*

### Comparing `nvm-1.0.5/docs/source/nvm.aux_spacy.rst` & `nvm-1.0.7/docs/source/nvm.aux_spacy.rst`

 * *Files identical despite different names*

### Comparing `nvm-1.0.5/docs/source/nvm.aux_str.rst` & `nvm-1.0.7/docs/source/nvm.aux_str.rst`

 * *Files identical despite different names*

### Comparing `nvm-1.0.5/docs/source/nvm.tests.rst` & `nvm-1.0.7/docs/source/nvm.tests.rst`

 * *Files identical despite different names*

### Comparing `nvm-1.0.5/nvm/__init__.py` & `nvm-1.0.7/nvm/__init__.py`

 * *Files identical despite different names*

### Comparing `nvm-1.0.5/nvm/aux_log/aux_log.py` & `nvm-1.0.7/nvm/aux_log/aux_log.py`

 * *Files identical despite different names*

### Comparing `nvm-1.0.5/nvm/aux_pandas/aux_pandas.py` & `nvm-1.0.7/nvm/aux_pandas/aux_pandas.py`

 * *Files identical despite different names*

### Comparing `nvm-1.0.5/nvm/aux_spacy/data/NicolasEtAl2019a/data.json` & `nvm-1.0.7/nvm/aux_spacy/data/NicolasEtAl2019a/data.json`

 * *Files identical despite different names*

### Comparing `nvm-1.0.5/nvm/aux_spacy/data/PennebakerEtAl2015a/__init__.py` & `nvm-1.0.7/nvm/aux_spacy/data/PennebakerEtAl2015a/__init__.py`

 * *Files identical despite different names*

### Comparing `nvm-1.0.5/nvm/aux_spacy/data/PietraszkiewiczEtAl2019a/__init__.py` & `nvm-1.0.7/nvm/aux_spacy/data/PietraszkiewiczEtAl2019a/__init__.py`

 * *Files identical despite different names*

### Comparing `nvm-1.0.5/nvm/aux_spacy/data/PietraszkiewiczEtAl2019a/data.json` & `nvm-1.0.7/nvm/aux_spacy/data/PietraszkiewiczEtAl2019a/data.json`

 * *Files identical despite different names*

### Comparing `nvm-1.0.5/nvm/aux_spacy/data/PietraszkiewiczEtAl2019a/data_liwc.json` & `nvm-1.0.7/nvm/aux_spacy/data/PietraszkiewiczEtAl2019a/data_liwc.json`

 * *Files identical despite different names*

### Comparing `nvm-1.0.5/nvm/aux_spacy/factories/get_doc_basic_metrics.py` & `nvm-1.0.7/nvm/aux_spacy/factories/get_doc_basic_metrics.py`

 * *Files identical despite different names*

### Comparing `nvm-1.0.5/nvm/aux_spacy/factories/get_doc_count_of_dict_items.py` & `nvm-1.0.7/nvm/aux_spacy/factories/get_doc_count_of_dict_items.py`

 * *Files identical despite different names*

### Comparing `nvm-1.0.5/nvm/aux_spacy/factories/get_doc_sentences.py` & `nvm-1.0.7/nvm/aux_spacy/factories/get_doc_sentences.py`

 * *Files identical despite different names*

### Comparing `nvm-1.0.5/nvm/aux_spacy/factories/get_doc_summary_dict.py` & `nvm-1.0.7/nvm/aux_spacy/factories/get_doc_summary_dict.py`

 * *Files identical despite different names*

### Comparing `nvm-1.0.5/nvm/aux_spacy/factories/get_doc_word_count.py` & `nvm-1.0.7/nvm/aux_spacy/factories/get_doc_word_count.py`

 * *Files identical despite different names*

### Comparing `nvm-1.0.5/nvm/aux_spacy/set_container_extensions.py` & `nvm-1.0.7/nvm/aux_spacy/set_container_extensions.py`

 * *Files identical despite different names*

### Comparing `nvm-1.0.5/nvm/aux_srsly/aux_srsly.py` & `nvm-1.0.7/nvm/aux_srsly/aux_srsly.py`

 * *Files identical despite different names*

### Comparing `nvm-1.0.5/nvm/aux_str/aux_str.py` & `nvm-1.0.7/nvm/aux_str/aux_str.py`

 * *Files identical despite different names*

### Comparing `nvm-1.0.5/nvm/aux_str/clean_str_mappings.py` & `nvm-1.0.7/nvm/aux_str/clean_str_mappings.py`

 * *Files identical despite different names*

### Comparing `nvm-1.0.5/nvm/aux_sys/aux_sys.py` & `nvm-1.0.7/nvm/aux_sys/aux_sys.py`

 * *Files identical despite different names*

### Comparing `nvm-1.0.5/nvm/data/emacs-logo/emacs-128x128.png` & `nvm-1.0.7/nvm/data/emacs-logo/emacs-128x128.png`

 * *Files identical despite different names*

### Comparing `nvm-1.0.5/nvm/data/emacs-logo/emacs.svg` & `nvm-1.0.7/nvm/data/emacs-logo/emacs.svg`

 * *Files identical despite different names*

### Comparing `nvm-1.0.5/nvm/tests/test_aux_spacy.py` & `nvm-1.0.7/nvm/tests/test_aux_spacy.py`

 * *Files identical despite different names*

### Comparing `nvm-1.0.5/nvm/tests/test_aux_str.py` & `nvm-1.0.7/nvm/tests/test_aux_str.py`

 * *Files identical despite different names*

### Comparing `nvm-1.0.5/nvm/tests/test_nvm.py` & `nvm-1.0.7/nvm/tests/test_nvm.py`

 * *Files identical despite different names*

### Comparing `nvm-1.0.5/nvm.egg-info/PKG-INFO` & `nvm-1.0.7/nvm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvm
-Version: 1.0.5
+Version: 1.0.7
 Summary: Plenty little helpers.
 Home-page: https://github.com/cogsys-io/nvm
 Author: cogsys.io
 Author-email: cogsys@cogsys.io
 License: GNU General Public License v3
 Keywords: nvm
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nvm-1.0.5/nvm.egg-info/SOURCES.txt` & `nvm-1.0.7/nvm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nvm-1.0.5/nvm.egg-info/requires.txt` & `nvm-1.0.7/nvm.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `nvm-1.0.5/pyproject.toml` & `nvm-1.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nvm-1.0.5/setup.cfg` & `nvm-1.0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `nvm-1.0.5/setup.py` & `nvm-1.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `nvm-1.0.5/versioneer.py` & `nvm-1.0.7/versioneer.py`

 * *Files identical despite different names*

