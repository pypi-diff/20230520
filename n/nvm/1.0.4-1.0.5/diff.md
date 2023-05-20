# Comparing `tmp/nvm-1.0.4.tar.gz` & `tmp/nvm-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvm-1.0.4.tar", last modified: Fri May  5 23:21:39 2023, max compression
+gzip compressed data, was "nvm-1.0.5.tar", last modified: Sat May 20 00:51:22 2023, max compression
```

## Comparing `nvm-1.0.4.tar` & `nvm-1.0.5.tar`

### file list

```diff
@@ -1,94 +1,132 @@
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 23:21:39.198428 nvm-1.0.4/
--rw-------   0 jiko      (1000) jiko      (1000)      292 2023-05-03 18:32:02.000000 nvm-1.0.4/.editorconfig
--rw-------   0 jiko      (1000) jiko      (1000)       29 2023-05-03 18:32:02.000000 nvm-1.0.4/.gitattributes
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 23:21:39.190428 nvm-1.0.4/.github/
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 23:21:39.190428 nvm-1.0.4/.github/ISSUE_TEMPLATE/
--rw-------   0 jiko      (1000) jiko      (1000)      348 2023-05-01 20:22:08.000000 nvm-1.0.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-------   0 jiko      (1000) jiko      (1000)      360 2023-05-01 20:22:08.000000 nvm-1.0.4/.github/ISSUE_TEMPLATE/feature_request.md
--rw-------   0 jiko      (1000) jiko      (1000)      446 2023-05-01 20:22:08.000000 nvm-1.0.4/.github/PULL_REQUEST_TEMPLATE.md
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 23:21:39.190428 nvm-1.0.4/.github/workflows/
--rw-------   0 jiko      (1000) jiko      (1000)      961 2023-05-05 21:24:14.000000 nvm-1.0.4/.github/workflows/build-main.yml
--rw-------   0 jiko      (1000) jiko      (1000)     1249 2023-05-04 01:10:13.000000 nvm-1.0.4/.gitignore
--rw-rw-r--   0 jiko      (1000) jiko      (1000)      716 2023-05-05 19:23:38.000000 nvm-1.0.4/.readthedocs.yaml
--rw-------   0 jiko      (1000) jiko      (1000)      151 2023-05-03 18:32:02.000000 nvm-1.0.4/AUTHORS.rst
--rw-------   0 jiko      (1000) jiko      (1000)     3466 2023-05-03 18:32:02.000000 nvm-1.0.4/CONTRIBUTING.rst
--rw-------   0 jiko      (1000) jiko      (1000)       69 2023-05-05 23:01:31.000000 nvm-1.0.4/HISTORY.rst
--rw-------   0 jiko      (1000) jiko      (1000)     1534 2023-05-03 18:32:02.000000 nvm-1.0.4/LICENSE
--rw-------   0 jiko      (1000) jiko      (1000)      316 2023-05-03 18:32:02.000000 nvm-1.0.4/MANIFEST.in
--rw-------   0 jiko      (1000) jiko      (1000)     3032 2023-05-03 20:09:42.000000 nvm-1.0.4/Makefile
--rw-------   0 jiko      (1000) jiko      (1000)     2000 2023-05-05 23:21:39.198428 nvm-1.0.4/PKG-INFO
--rw-------   0 jiko      (1000) jiko      (1000)     1205 2023-05-05 23:20:54.000000 nvm-1.0.4/README.rst
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 23:21:39.190428 nvm-1.0.4/bin/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-03 18:32:02.000000 nvm-1.0.4/bin/.gitkeep
--rw-------   0 jiko      (1000) jiko      (1000)      425 2023-05-03 18:32:02.000000 nvm-1.0.4/bin/nvm.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 23:21:39.190428 nvm-1.0.4/data/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-03 18:32:02.000000 nvm-1.0.4/data/.gitkeep
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 23:21:39.190428 nvm-1.0.4/data/emacs-logo/
--rw-------   0 jiko      (1000) jiko      (1000)     9818 2023-05-03 18:32:02.000000 nvm-1.0.4/data/emacs-logo/emacs-128x128.png
--rw-rw-r--   0 jiko      (1000) jiko      (1000)    13358 2023-05-03 18:32:02.000000 nvm-1.0.4/data/emacs-logo/emacs.svg
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 23:21:39.190428 nvm-1.0.4/docs/
--rw-------   0 jiko      (1000) jiko      (1000)      606 2023-05-03 18:32:02.000000 nvm-1.0.4/docs/Makefile
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 23:21:39.186428 nvm-1.0.4/docs/build/
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 23:21:39.186428 nvm-1.0.4/docs/build/html/
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 23:21:39.190428 nvm-1.0.4/docs/build/html/_static/
--rw-------   0 jiko      (1000) jiko      (1000)      313 2023-05-04 17:45:22.000000 nvm-1.0.4/docs/build/html/_static/check-solid.svg
--rw-------   0 jiko      (1000) jiko      (1000)      411 2023-05-04 17:45:22.000000 nvm-1.0.4/docs/build/html/_static/copy-button.svg
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 23:21:39.186428 nvm-1.0.4/docs/build/html/_static/css/
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 23:21:39.194428 nvm-1.0.4/docs/build/html/_static/css/fonts/
--rw-------   0 jiko      (1000) jiko      (1000)   444379 2023-05-04 17:45:23.000000 nvm-1.0.4/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-------   0 jiko      (1000) jiko      (1000)      286 2023-05-04 17:45:09.000000 nvm-1.0.4/docs/build/html/_static/file.png
--rw-------   0 jiko      (1000) jiko      (1000)       90 2023-05-04 17:45:09.000000 nvm-1.0.4/docs/build/html/_static/minus.png
--rw-------   0 jiko      (1000) jiko      (1000)       90 2023-05-04 17:45:09.000000 nvm-1.0.4/docs/build/html/_static/plus.png
--rw-------   0 jiko      (1000) jiko      (1000)      588 2023-05-05 19:42:21.000000 nvm-1.0.4/docs/requirements.txt
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 23:21:39.194428 nvm-1.0.4/docs/source/
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 23:21:39.194428 nvm-1.0.4/docs/source/_static/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-03 18:32:02.000000 nvm-1.0.4/docs/source/_static/.gitkeep
--rw-------   0 jiko      (1000) jiko      (1000)       31 2023-05-03 18:32:02.000000 nvm-1.0.4/docs/source/authors.rst
--rwx------   0 jiko      (1000) jiko      (1000)     5541 2023-05-04 00:55:18.000000 nvm-1.0.4/docs/source/conf.py
--rw-------   0 jiko      (1000) jiko      (1000)       36 2023-05-03 18:32:02.000000 nvm-1.0.4/docs/source/contributing.rst
--rw-------   0 jiko      (1000) jiko      (1000)       31 2023-05-03 18:32:02.000000 nvm-1.0.4/docs/source/history.rst
--rw-------   0 jiko      (1000) jiko      (1000)      319 2023-05-03 18:32:02.000000 nvm-1.0.4/docs/source/index.rst
--rw-------   0 jiko      (1000) jiko      (1000)     1086 2023-05-03 18:32:02.000000 nvm-1.0.4/docs/source/installation.rst
--rw-------   0 jiko      (1000) jiko      (1000)       46 2023-05-05 23:21:13.000000 nvm-1.0.4/docs/source/modules.rst
--rw-------   0 jiko      (1000) jiko      (1000)      331 2023-05-04 00:48:09.000000 nvm-1.0.4/docs/source/nvm.aux_log.rst
--rw-------   0 jiko      (1000) jiko      (1000)      358 2023-05-05 13:07:38.000000 nvm-1.0.4/docs/source/nvm.aux_pandas.rst
--rw-------   0 jiko      (1000) jiko      (1000)      331 2023-05-03 20:38:41.000000 nvm-1.0.4/docs/source/nvm.aux_str.rst
--rw-------   0 jiko      (1000) jiko      (1000)      331 2023-05-03 23:04:50.000000 nvm-1.0.4/docs/source/nvm.aux_sys.rst
--rw-------   0 jiko      (1000) jiko      (1000)      384 2023-05-05 23:21:13.000000 nvm-1.0.4/docs/source/nvm.rst
--rw-------   0 jiko      (1000) jiko      (1000)       30 2023-05-03 18:32:02.000000 nvm-1.0.4/docs/source/readme.rst
--rw-------   0 jiko      (1000) jiko      (1000)       61 2023-05-03 18:32:02.000000 nvm-1.0.4/docs/source/usage.rst
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 23:21:39.198428 nvm-1.0.4/nvm/
--rw-------   0 jiko      (1000) jiko      (1000)      494 2023-05-05 19:45:20.000000 nvm-1.0.4/nvm/__init__.py
--rw-------   0 jiko      (1000) jiko      (1000)      497 2023-05-05 23:21:39.198428 nvm-1.0.4/nvm/_version.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 23:21:39.198428 nvm-1.0.4/nvm/aux_log/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)       51 2023-05-04 00:33:55.000000 nvm-1.0.4/nvm/aux_log/__init__.py
--rw-rw-r--   0 jiko      (1000) jiko      (1000)     5073 2023-05-04 01:17:45.000000 nvm-1.0.4/nvm/aux_log/aux_log.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 23:21:39.198428 nvm-1.0.4/nvm/aux_pandas/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)      105 2023-05-04 02:17:41.000000 nvm-1.0.4/nvm/aux_pandas/__init__.py
--rw-rw-r--   0 jiko      (1000) jiko      (1000)     1590 2023-05-05 18:55:20.000000 nvm-1.0.4/nvm/aux_pandas/aux_pandas.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 23:21:39.198428 nvm-1.0.4/nvm/aux_str/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)      179 2023-05-05 15:19:07.000000 nvm-1.0.4/nvm/aux_str/__init__.py
--rw-rw-r--   0 jiko      (1000) jiko      (1000)     5209 2023-05-05 22:58:41.000000 nvm-1.0.4/nvm/aux_str/aux_str.py
--rw-rw-r--   0 jiko      (1000) jiko      (1000)     1789 2023-05-05 22:20:16.000000 nvm-1.0.4/nvm/aux_str/clean_str_mappings.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 23:21:39.198428 nvm-1.0.4/nvm/aux_sys/
--rw-rw-r--   0 jiko      (1000) jiko      (1000)       51 2023-05-03 23:08:53.000000 nvm-1.0.4/nvm/aux_sys/__init__.py
--rw-rw-r--   0 jiko      (1000) jiko      (1000)     1342 2023-05-05 19:03:51.000000 nvm-1.0.4/nvm/aux_sys/aux_sys.py
--rw-------   0 jiko      (1000) jiko      (1000)       66 2023-05-03 18:32:02.000000 nvm-1.0.4/nvm/nvm.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 23:21:39.194428 nvm-1.0.4/nvm.egg-info/
--rw-------   0 jiko      (1000) jiko      (1000)     2000 2023-05-05 23:21:39.000000 nvm-1.0.4/nvm.egg-info/PKG-INFO
--rw-------   0 jiko      (1000) jiko      (1000)     1635 2023-05-05 23:21:39.000000 nvm-1.0.4/nvm.egg-info/SOURCES.txt
--rw-------   0 jiko      (1000) jiko      (1000)        1 2023-05-05 23:21:39.000000 nvm-1.0.4/nvm.egg-info/dependency_links.txt
--rw-------   0 jiko      (1000) jiko      (1000)       37 2023-05-05 23:21:39.000000 nvm-1.0.4/nvm.egg-info/entry_points.txt
--rw-------   0 jiko      (1000) jiko      (1000)        1 2023-05-05 23:21:39.000000 nvm-1.0.4/nvm.egg-info/not-zip-safe
--rw-------   0 jiko      (1000) jiko      (1000)     1013 2023-05-05 23:21:39.000000 nvm-1.0.4/nvm.egg-info/requires.txt
--rw-------   0 jiko      (1000) jiko      (1000)        4 2023-05-05 23:21:39.000000 nvm-1.0.4/nvm.egg-info/top_level.txt
--rw-rw-r--   0 jiko      (1000) jiko      (1000)      755 2023-05-03 18:32:02.000000 nvm-1.0.4/pyproject.toml
--rw-------   0 jiko      (1000) jiko      (1000)      494 2023-05-05 21:20:43.000000 nvm-1.0.4/requirements_dev.txt
--rw-------   0 jiko      (1000) jiko      (1000)      673 2023-05-05 23:21:39.198428 nvm-1.0.4/setup.cfg
--rw-------   0 jiko      (1000) jiko      (1000)     2584 2023-05-05 23:14:48.000000 nvm-1.0.4/setup.py
-drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-05 23:21:39.198428 nvm-1.0.4/tests/
--rw-------   0 jiko      (1000) jiko      (1000)       33 2023-05-03 18:32:02.000000 nvm-1.0.4/tests/__init__.py
--rw-rw-r--   0 jiko      (1000) jiko      (1000)     1563 2023-05-05 15:01:56.000000 nvm-1.0.4/tests/test_aux_str.py
--rw-------   0 jiko      (1000) jiko      (1000)      554 2023-05-05 13:11:09.000000 nvm-1.0.4/tests/test_nvm.py
--rw-------   0 jiko      (1000) jiko      (1000)      493 2023-05-05 23:16:08.000000 nvm-1.0.4/tox.ini
--rw-------   0 jiko      (1000) jiko      (1000)    83607 2023-05-03 18:32:02.000000 nvm-1.0.4/versioneer.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.019164 nvm-1.0.5/
+-rw-------   0 jiko      (1000) jiko      (1000)      292 2023-05-03 18:32:02.000000 nvm-1.0.5/.editorconfig
+-rw-------   0 jiko      (1000) jiko      (1000)       29 2023-05-03 18:32:02.000000 nvm-1.0.5/.gitattributes
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.011164 nvm-1.0.5/.github/
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.011164 nvm-1.0.5/.github/ISSUE_TEMPLATE/
+-rw-------   0 jiko      (1000) jiko      (1000)      348 2023-05-01 20:22:08.000000 nvm-1.0.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-------   0 jiko      (1000) jiko      (1000)      360 2023-05-01 20:22:08.000000 nvm-1.0.5/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-------   0 jiko      (1000) jiko      (1000)      446 2023-05-01 20:22:08.000000 nvm-1.0.5/.github/PULL_REQUEST_TEMPLATE.md
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.011164 nvm-1.0.5/.github/workflows/
+-rw-------   0 jiko      (1000) jiko      (1000)      961 2023-05-05 21:24:14.000000 nvm-1.0.5/.github/workflows/build-main.yml
+-rw-------   0 jiko      (1000) jiko      (1000)     1249 2023-05-04 01:10:13.000000 nvm-1.0.5/.gitignore
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)      716 2023-05-05 19:23:38.000000 nvm-1.0.5/.readthedocs.yaml
+-rw-------   0 jiko      (1000) jiko      (1000)      151 2023-05-03 18:32:02.000000 nvm-1.0.5/AUTHORS.rst
+-rw-------   0 jiko      (1000) jiko      (1000)     3466 2023-05-03 18:32:02.000000 nvm-1.0.5/CONTRIBUTING.rst
+-rw-------   0 jiko      (1000) jiko      (1000)       69 2023-05-05 23:01:31.000000 nvm-1.0.5/HISTORY.rst
+-rw-------   0 jiko      (1000) jiko      (1000)     1534 2023-05-03 18:32:02.000000 nvm-1.0.5/LICENSE
+-rw-------   0 jiko      (1000) jiko      (1000)      460 2023-05-20 00:40:26.000000 nvm-1.0.5/MANIFEST.in
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)     3140 2023-05-20 00:43:36.000000 nvm-1.0.5/Makefile
+-rw-------   0 jiko      (1000) jiko      (1000)     2000 2023-05-20 00:51:22.019164 nvm-1.0.5/PKG-INFO
+-rw-------   0 jiko      (1000) jiko      (1000)     1205 2023-05-05 23:20:54.000000 nvm-1.0.5/README.rst
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.011164 nvm-1.0.5/docs/
+-rw-------   0 jiko      (1000) jiko      (1000)      612 2023-05-14 21:15:09.000000 nvm-1.0.5/docs/Makefile
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.011164 nvm-1.0.5/docs/build/
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.011164 nvm-1.0.5/docs/build/html/
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.015164 nvm-1.0.5/docs/build/html/_static/
+-rw-------   0 jiko      (1000) jiko      (1000)      313 2023-05-04 17:45:22.000000 nvm-1.0.5/docs/build/html/_static/check-solid.svg
+-rw-------   0 jiko      (1000) jiko      (1000)      411 2023-05-04 17:45:22.000000 nvm-1.0.5/docs/build/html/_static/copy-button.svg
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.011164 nvm-1.0.5/docs/build/html/_static/css/
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.015164 nvm-1.0.5/docs/build/html/_static/css/fonts/
+-rw-------   0 jiko      (1000) jiko      (1000)   444379 2023-05-04 17:45:23.000000 nvm-1.0.5/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-------   0 jiko      (1000) jiko      (1000)      286 2023-05-04 17:45:09.000000 nvm-1.0.5/docs/build/html/_static/file.png
+-rw-------   0 jiko      (1000) jiko      (1000)       90 2023-05-04 17:45:09.000000 nvm-1.0.5/docs/build/html/_static/minus.png
+-rw-------   0 jiko      (1000) jiko      (1000)       90 2023-05-04 17:45:09.000000 nvm-1.0.5/docs/build/html/_static/plus.png
+-rw-------   0 jiko      (1000) jiko      (1000)      588 2023-05-05 19:42:21.000000 nvm-1.0.5/docs/requirements.txt
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.015164 nvm-1.0.5/docs/source/
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.015164 nvm-1.0.5/docs/source/_static/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-03 18:32:02.000000 nvm-1.0.5/docs/source/_static/.gitkeep
+-rw-------   0 jiko      (1000) jiko      (1000)       31 2023-05-03 18:32:02.000000 nvm-1.0.5/docs/source/authors.rst
+-rwx------   0 jiko      (1000) jiko      (1000)     5572 2023-05-14 23:09:27.000000 nvm-1.0.5/docs/source/conf.py
+-rw-------   0 jiko      (1000) jiko      (1000)       36 2023-05-03 18:32:02.000000 nvm-1.0.5/docs/source/contributing.rst
+-rw-------   0 jiko      (1000) jiko      (1000)       31 2023-05-03 18:32:02.000000 nvm-1.0.5/docs/source/history.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      319 2023-05-14 22:54:59.000000 nvm-1.0.5/docs/source/index.rst
+-rw-------   0 jiko      (1000) jiko      (1000)     1086 2023-05-03 18:32:02.000000 nvm-1.0.5/docs/source/installation.rst
+-rw-------   0 jiko      (1000) jiko      (1000)       46 2023-05-20 00:50:52.000000 nvm-1.0.5/docs/source/modules.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      331 2023-05-20 00:50:51.000000 nvm-1.0.5/docs/source/nvm.aux_log.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      358 2023-05-20 00:50:51.000000 nvm-1.0.5/docs/source/nvm.aux_pandas.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      230 2023-05-20 00:50:52.000000 nvm-1.0.5/docs/source/nvm.aux_spacy.data.NicolasEtAl2019a.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      239 2023-05-20 00:50:52.000000 nvm-1.0.5/docs/source/nvm.aux_spacy.data.PennebakerEtAl2015a.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      254 2023-05-20 00:50:52.000000 nvm-1.0.5/docs/source/nvm.aux_spacy.data.PietraszkiewiczEtAl2019a.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      363 2023-05-20 00:50:51.000000 nvm-1.0.5/docs/source/nvm.aux_spacy.data.rst
+-rw-------   0 jiko      (1000) jiko      (1000)     1373 2023-05-20 00:50:52.000000 nvm-1.0.5/docs/source/nvm.aux_spacy.factories.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      663 2023-05-20 00:50:51.000000 nvm-1.0.5/docs/source/nvm.aux_spacy.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      349 2023-05-20 00:50:52.000000 nvm-1.0.5/docs/source/nvm.aux_srsly.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      658 2023-05-20 00:50:52.000000 nvm-1.0.5/docs/source/nvm.aux_str.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      331 2023-05-20 00:50:52.000000 nvm-1.0.5/docs/source/nvm.aux_sys.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      289 2023-05-20 00:50:52.000000 nvm-1.0.5/docs/source/nvm.cli.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      442 2023-05-20 00:50:51.000000 nvm-1.0.5/docs/source/nvm.rst
+-rw-------   0 jiko      (1000) jiko      (1000)      642 2023-05-20 00:50:52.000000 nvm-1.0.5/docs/source/nvm.tests.rst
+-rw-------   0 jiko      (1000) jiko      (1000)       30 2023-05-03 18:32:02.000000 nvm-1.0.5/docs/source/readme.rst
+-rw-------   0 jiko      (1000) jiko      (1000)       61 2023-05-03 18:32:02.000000 nvm-1.0.5/docs/source/usage.rst
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.019164 nvm-1.0.5/nvm/
+-rw-------   0 jiko      (1000) jiko      (1000)      885 2023-05-19 23:56:36.000000 nvm-1.0.5/nvm/__init__.py
+-rw-------   0 jiko      (1000) jiko      (1000)      497 2023-05-20 00:51:22.019164 nvm-1.0.5/nvm/_version.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.015164 nvm-1.0.5/nvm/aux_log/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)       51 2023-05-04 00:33:55.000000 nvm-1.0.5/nvm/aux_log/__init__.py
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)     5073 2023-05-04 01:17:45.000000 nvm-1.0.5/nvm/aux_log/aux_log.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.015164 nvm-1.0.5/nvm/aux_pandas/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)      137 2023-05-09 09:25:31.000000 nvm-1.0.5/nvm/aux_pandas/__init__.py
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)     1993 2023-05-09 09:31:34.000000 nvm-1.0.5/nvm/aux_pandas/aux_pandas.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.015164 nvm-1.0.5/nvm/aux_spacy/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)      489 2023-05-19 23:05:08.000000 nvm-1.0.5/nvm/aux_spacy/__init__.py
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)       23 2023-05-19 23:02:54.000000 nvm-1.0.5/nvm/aux_spacy/aux_spacy.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.015164 nvm-1.0.5/nvm/aux_spacy/data/
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.015164 nvm-1.0.5/nvm/aux_spacy/data/NicolasEtAl2019a/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)      396 2023-05-19 22:51:19.000000 nvm-1.0.5/nvm/aux_spacy/data/NicolasEtAl2019a/__init__.py
+-rw-------   0 jiko      (1000) jiko      (1000)    47658 2022-03-18 04:48:30.000000 nvm-1.0.5/nvm/aux_spacy/data/NicolasEtAl2019a/data.json
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.015164 nvm-1.0.5/nvm/aux_spacy/data/PennebakerEtAl2015a/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)       43 2023-05-19 21:19:19.000000 nvm-1.0.5/nvm/aux_spacy/data/PennebakerEtAl2015a/.gitignore
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)      944 2023-05-20 00:32:47.000000 nvm-1.0.5/nvm/aux_spacy/data/PennebakerEtAl2015a/__init__.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.015164 nvm-1.0.5/nvm/aux_spacy/data/PietraszkiewiczEtAl2019a/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)      553 2023-05-19 22:52:48.000000 nvm-1.0.5/nvm/aux_spacy/data/PietraszkiewiczEtAl2019a/__init__.py
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)    13614 2023-05-13 01:10:01.000000 nvm-1.0.5/nvm/aux_spacy/data/PietraszkiewiczEtAl2019a/data.json
+-rw-------   0 jiko      (1000) jiko      (1000)    32392 2022-03-18 05:27:49.000000 nvm-1.0.5/nvm/aux_spacy/data/PietraszkiewiczEtAl2019a/data_liwc.json
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)       23 2023-05-14 19:16:37.000000 nvm-1.0.5/nvm/aux_spacy/data/__init__.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.015164 nvm-1.0.5/nvm/aux_spacy/factories/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)       23 2023-05-15 01:52:05.000000 nvm-1.0.5/nvm/aux_spacy/factories/__init__.py
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)     6033 2023-05-20 00:18:54.000000 nvm-1.0.5/nvm/aux_spacy/factories/get_doc_basic_metrics.py
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)     8091 2023-05-20 00:18:16.000000 nvm-1.0.5/nvm/aux_spacy/factories/get_doc_count_of_dict_items.py
+-rw-------   0 jiko      (1000) jiko      (1000)     1786 2023-05-14 22:44:24.000000 nvm-1.0.5/nvm/aux_spacy/factories/get_doc_sentences.py
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)     2462 2023-05-20 00:30:58.000000 nvm-1.0.5/nvm/aux_spacy/factories/get_doc_summary_dict.py
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)     1564 2023-05-14 23:53:03.000000 nvm-1.0.5/nvm/aux_spacy/factories/get_doc_word_count.py
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)     3736 2023-05-20 00:13:47.000000 nvm-1.0.5/nvm/aux_spacy/set_container_extensions.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.015164 nvm-1.0.5/nvm/aux_srsly/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)       73 2023-05-19 23:56:47.000000 nvm-1.0.5/nvm/aux_srsly/__init__.py
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)     1691 2023-05-20 00:21:53.000000 nvm-1.0.5/nvm/aux_srsly/aux_srsly.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.015164 nvm-1.0.5/nvm/aux_str/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)      370 2023-05-16 08:02:31.000000 nvm-1.0.5/nvm/aux_str/__init__.py
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)     6834 2023-05-19 23:26:41.000000 nvm-1.0.5/nvm/aux_str/aux_str.py
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)     2083 2023-05-16 07:59:44.000000 nvm-1.0.5/nvm/aux_str/clean_str_mappings.py
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)      140 2023-05-07 02:51:21.000000 nvm-1.0.5/nvm/aux_str/regex.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.015164 nvm-1.0.5/nvm/aux_sys/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)       80 2023-05-12 14:03:28.000000 nvm-1.0.5/nvm/aux_sys/__init__.py
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)     2054 2023-05-12 14:08:28.000000 nvm-1.0.5/nvm/aux_sys/aux_sys.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.015164 nvm-1.0.5/nvm/cli/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-03 18:32:02.000000 nvm-1.0.5/nvm/cli/.gitkeep
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-06 09:19:24.000000 nvm-1.0.5/nvm/cli/__init__.py
+-rw-------   0 jiko      (1000) jiko      (1000)      429 2023-05-12 04:26:04.000000 nvm-1.0.5/nvm/cli/nvm.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.015164 nvm-1.0.5/nvm/data/
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)        0 2023-05-03 18:32:02.000000 nvm-1.0.5/nvm/data/.gitkeep
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.019164 nvm-1.0.5/nvm/data/emacs-logo/
+-rw-------   0 jiko      (1000) jiko      (1000)     9818 2023-05-03 18:32:02.000000 nvm-1.0.5/nvm/data/emacs-logo/emacs-128x128.png
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)    13358 2023-05-03 18:32:02.000000 nvm-1.0.5/nvm/data/emacs-logo/emacs.svg
+-rw-------   0 jiko      (1000) jiko      (1000)       66 2023-05-03 18:32:02.000000 nvm-1.0.5/nvm/nvm.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.019164 nvm-1.0.5/nvm/tests/
+-rw-------   0 jiko      (1000) jiko      (1000)       28 2023-05-06 10:03:21.000000 nvm-1.0.5/nvm/tests/__init__.py
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)     6136 2023-05-20 00:11:39.000000 nvm-1.0.5/nvm/tests/test_aux_spacy.py
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)     2538 2023-05-14 19:32:09.000000 nvm-1.0.5/nvm/tests/test_aux_str.py
+-rw-------   0 jiko      (1000) jiko      (1000)      554 2023-05-05 13:11:09.000000 nvm-1.0.5/nvm/tests/test_nvm.py
+drwx------   0 jiko      (1000) jiko      (1000)        0 2023-05-20 00:51:22.015164 nvm-1.0.5/nvm.egg-info/
+-rw-------   0 jiko      (1000) jiko      (1000)     2000 2023-05-20 00:51:21.000000 nvm-1.0.5/nvm.egg-info/PKG-INFO
+-rw-------   0 jiko      (1000) jiko      (1000)     2910 2023-05-20 00:51:22.000000 nvm-1.0.5/nvm.egg-info/SOURCES.txt
+-rw-------   0 jiko      (1000) jiko      (1000)        1 2023-05-20 00:51:21.000000 nvm-1.0.5/nvm.egg-info/dependency_links.txt
+-rw-------   0 jiko      (1000) jiko      (1000)       41 2023-05-20 00:51:21.000000 nvm-1.0.5/nvm.egg-info/entry_points.txt
+-rw-------   0 jiko      (1000) jiko      (1000)        1 2023-05-20 00:51:21.000000 nvm-1.0.5/nvm.egg-info/not-zip-safe
+-rw-------   0 jiko      (1000) jiko      (1000)     1013 2023-05-20 00:51:21.000000 nvm-1.0.5/nvm.egg-info/requires.txt
+-rw-------   0 jiko      (1000) jiko      (1000)        4 2023-05-20 00:51:21.000000 nvm-1.0.5/nvm.egg-info/top_level.txt
+-rw-rw-r--   0 jiko      (1000) jiko      (1000)      755 2023-05-03 18:32:02.000000 nvm-1.0.5/pyproject.toml
+-rw-------   0 jiko      (1000) jiko      (1000)      494 2023-05-05 21:20:43.000000 nvm-1.0.5/requirements_dev.txt
+-rw-------   0 jiko      (1000) jiko      (1000)      739 2023-05-20 00:51:22.019164 nvm-1.0.5/setup.cfg
+-rw-------   0 jiko      (1000) jiko      (1000)     2592 2023-05-06 10:12:14.000000 nvm-1.0.5/setup.py
+-rw-------   0 jiko      (1000) jiko      (1000)      493 2023-05-05 23:16:08.000000 nvm-1.0.5/tox.ini
+-rw-------   0 jiko      (1000) jiko      (1000)    83607 2023-05-03 18:32:02.000000 nvm-1.0.5/versioneer.py
```

### Comparing `nvm-1.0.4/.github/workflows/build-main.yml` & `nvm-1.0.5/.github/workflows/build-main.yml`

 * *Files identical despite different names*

### Comparing `nvm-1.0.4/.gitignore` & `nvm-1.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `nvm-1.0.4/.readthedocs.yaml` & `nvm-1.0.5/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `nvm-1.0.4/CONTRIBUTING.rst` & `nvm-1.0.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nvm-1.0.4/LICENSE` & `nvm-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nvm-1.0.4/Makefile` & `nvm-1.0.5/Makefile`

 * *Files 4% similar despite different names*

```diff
@@ -45,19 +45,24 @@
 
 clean-test: ## remove test and coverage artifacts
 	rm -fr .tox/
 	rm -f .coverage
 	rm -fr htmlcov/
 	rm -fr .pytest_cache
 
+clean-docs: ## clean docs
+	rm -fv docs/source/nvm.rst
+	rm -fv docs/source/nvm*.rst
+	rm -fv docs/source/modules.rst
+
 lint-flake8: ## check style with flake8
-	flake8 nvm tests --exit-zero --count --statistics
+	flake8 nvm nvm/tests --exit-zero --count --statistics
 
 lint-black: ## check style with black
-	black --check nvm tests || true
+	black --check nvm nvm/tests || true
 
 lint: lint-flake8 lint-black ## check style
 
 test: ## run tests quickly with the default Python
 	pytest -W "ignore::DeprecationWarning" -v
 
 test-all: ## run tests on every Python version with tox
@@ -65,44 +70,43 @@
 
 coverage: ## check code coverage quickly with the default Python
 	coverage run --source nvm -m pytest
 	coverage report -m
 	coverage html
 	$(BROWSER) htmlcov/index.html
 
-docs: ## generate Sphinx HTML documentation, including API docs
-	rm -f docs/source/nvm.rst
-	rm -f docs/source/modules.rst
+docs: clean-docs  ## generate Sphinx HTML documentation, including API docs
 	sphinx-apidoc -o docs/source/ nvm
 	$(MAKE) -C docs clean
 	$(MAKE) -C docs html
 	$(BROWSER) docs/build/html/index.html
 
 servedocs: docs ## compile the docs watching for changes
 	watchmedo shell-command -p '*.rst' -c '$(MAKE) -C docs html' -R -D .
 
-check: dist ## check package (twine)
-	twine check dist/*
-
-release: dist ## package and upload a release
-	twine upload dist/*
-
-release-to-testpypi: dist ## package and upload a release to testpypi
-	twine upload -r test dist/*
-
 dist: clean ## builds source and wheel package
 #	python setup.py sdist
 #	python setup.py bdist_wheel
 	python -m build
 	ls -l dist
 
+build: dist ## builds source and wheel package (same as dist)
+
+check: dist ## check package dist/built (twine)
+	twine check dist/*
+
 install: clean ## install the package to the active Python's site-packages
 #	python setup.py install
 	pip install .
 
 install-editable: clean ## install the package in editable mode
 	pip install --editable .
 
+prep: clean lint test docs dist check install-editable
+
+release: dist ## package and upload a release
+	twine upload dist/*
+
 version: ## display git versioning tags and the actual current version from versioneer
 	@git tag | grep "nvm-v" | sed -e "s|nvm-v||g"
 	@echo "----------------"
 	@python -c "import nvm; print(nvm.__version__+' [← current]')"
```

### Comparing `nvm-1.0.4/PKG-INFO` & `nvm-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvm
-Version: 1.0.4
+Version: 1.0.5
 Summary: Plenty little helpers.
 Home-page: https://github.com/cogsys-io/nvm
 Author: cogsys.io
 Author-email: cogsys@cogsys.io
 License: GNU General Public License v3
 Keywords: nvm
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nvm-1.0.4/README.rst` & `nvm-1.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `nvm-1.0.4/data/emacs-logo/emacs-128x128.png` & `nvm-1.0.5/nvm/data/emacs-logo/emacs-128x128.png`

 * *Files identical despite different names*

### Comparing `nvm-1.0.4/data/emacs-logo/emacs.svg` & `nvm-1.0.5/nvm/data/emacs-logo/emacs.svg`

 * *Files identical despite different names*

### Comparing `nvm-1.0.4/docs/Makefile` & `nvm-1.0.5/docs/Makefile`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Minimal makefile for Sphinx documentation
 
 # You can set these variables from the command line.
-SPHINXOPTS    =
+SPHINXOPTS    = -a -E
 SPHINXBUILD   = python -msphinx
 SPHINXPROJ    = nvm
 SOURCEDIR     = source
 BUILDDIR      = build
 
 # Put it first so that "make" without argument is like "make help".
 help:
```

### Comparing `nvm-1.0.4/docs/build/html/_static/css/fonts/fontawesome-webfont.svg` & `nvm-1.0.5/docs/build/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `nvm-1.0.4/docs/requirements.txt` & `nvm-1.0.5/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `nvm-1.0.4/docs/source/conf.py` & `nvm-1.0.5/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.viewcode",
     "sphinx_copybutton",
     # "numpydoc",
     "sphinx.ext.napoleon",
     "sphinx.ext.mathjax",
+    # "sphinxcontrib.fulltoc",
 ]
 
 # numpydoc
 numpydoc_show_class_members = True
 
 # Control napoleon
 napoleon_google_docstring = False
```

### Comparing `nvm-1.0.4/docs/source/installation.rst` & `nvm-1.0.5/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `nvm-1.0.4/nvm/aux_log/aux_log.py` & `nvm-1.0.5/nvm/aux_log/aux_log.py`

 * *Files identical despite different names*

### Comparing `nvm-1.0.4/nvm/aux_str/clean_str_mappings.py` & `nvm-1.0.5/nvm/aux_str/clean_str_mappings.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,25 @@
 #!/usr/bin/env python3
 
+CLEAN_STR_MAPPINGS_SPACE = [
+    {
+        " ": [  # Unicode Character 'SPACE' (U+0020)
+            "-",
+            "_",
+        ],
+    },
+]
+
+CLEAN_STR_MAPPINGS_DROP_HASHTAGS = [
+    {
+        " ": [  # Unicode Character 'SPACE' (U+0020)
+            r"\B#\w*[a-zA-Z]+\w*",
+        ],
+    },
+]
 
 CLEAN_STR_MAPPINGS_TINY = [
     {
         " ": [  # Unicode Character 'SPACE' (U+0020)
             "\n",  # LF (Line Feed)
             "\r",  # CR (Carriage Return)
             "\t",  # HT (Horizontal Tab)
```

### Comparing `nvm-1.0.4/nvm/aux_sys/aux_sys.py` & `nvm-1.0.5/nvm/aux_sys/aux_sys.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 #!/usr/bin/env python3
 
 import os
+import sys
 import pwd
 import socket
 import pathlib
 import logging
+import contextlib
 
 
 from typing import (
     Dict,
+    Union,
     Optional,
 )
 
 
 def chdir(
-    locations: Dict[str, Dict[str, str]],
+    locations: Dict[str, Dict[str, Union[str, pathlib.Path]]],
     log0: Optional[logging.Logger] = logging.getLogger("dummy"),
 ) -> str:
     """Change current directory according to hostname and username.
 
     Target directory path is relative to user's ``${HOME}`` directory.
 
     Parameters
     ----------
-    locations : Dict[str, Dict[str, str]]
+    locations : Dict[str, Dict[str, Union[str, pathlib.Path]]]
         Dictionary containing locations, usernames and paths.
     log0 : Optional[logging.Logger]
         Logger.
 
     Examples
     --------
     >>> import srsly
@@ -49,7 +52,37 @@
     # TODO: add warning if mach is found for hostname or username
     if hostname in locations.keys():
         if username in locations[hostname].keys():
             os.chdir(pathlib.Path.home() / locations[hostname][username])
             log0.info(f"{os.getcwd() = }")
 
     return pathlib.Path.cwd()
+
+
+@contextlib.contextmanager
+def pushdir(new_dir: Union[str, pathlib.Path]) -> None:
+    """Change dir context (WARNING: non thread-safe).
+
+    Parameters
+    ----------
+    new_dir : Union[str, pathlib.Path]
+        New (temporary path) paths.
+
+    Examples
+    --------
+    >>> import os
+    >>> from nvm import pushdir
+    >>> print(os.getcwd())
+    >>> with pushdir('/home/'):
+    >>>     print(os.getcwd())
+    >>>
+    >>> print(os.getcwd())
+
+    """
+    old_dir = os.getcwd()
+    try:
+        os.chdir(new_dir)
+        sys.path.insert(0, new_dir)
+        yield
+    finally:
+        del sys.path[0]
+        os.chdir(old_dir)
```

### Comparing `nvm-1.0.4/nvm.egg-info/PKG-INFO` & `nvm-1.0.5/nvm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvm
-Version: 1.0.4
+Version: 1.0.5
 Summary: Plenty little helpers.
 Home-page: https://github.com/cogsys-io/nvm
 Author: cogsys.io
 Author-email: cogsys@cogsys.io
 License: GNU General Public License v3
 Keywords: nvm
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nvm-1.0.4/nvm.egg-info/requires.txt` & `nvm-1.0.5/nvm.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `nvm-1.0.4/pyproject.toml` & `nvm-1.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nvm-1.0.4/setup.cfg` & `nvm-1.0.5/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 	.tox
 per-file-ignores = 
 	nvm/__init__.py: F401
 	nvm/aux_str/__init__.py: F401
 	nvm/aux_sys/__init__.py: F401
 	nvm/aux_log/__init__.py: F401
 	nvm/aux_pandas/__init__.py: F401
+	nvm/aux_srsly/__init__.py: F401
+	nvm/aux_spacy/__init__.py: F401
 	nvm/nvm.py: F401
 	setup.py: E501,C901
 	versioneer.py: E501,C901
 	boilerplate/_version.py: E501,C901
 
 [egg_info]
 tag_build =
```

### Comparing `nvm-1.0.4/setup.py` & `nvm-1.0.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,30 +75,30 @@
         # "Programming Language :: Python :: 3.9",
         # "Programming Language :: Python :: 3.10",
         # "Programming Language :: Python :: 3.11",
     ],
     description="Plenty little helpers.",
     entry_points={
         "console_scripts": [
-            "nvm=bin.nvm:main",
+            "nvm=nvm.cli.nvm:main",
         ],
     },
     install_requires=requirements,
     setup_requires=setup_requirements,
     license="GNU General Public License v3",
     long_description=readme + "\n\n" + history,
     long_description_content_type="text/x-rst",
     include_package_data=True,
     keywords="nvm",
     name="nvm",
     packages=find_packages(
         include=["nvm", "nvm.*"],
         exclude=["tests", "*.tests", "*.tests.*"],
     ),
-    test_suite="tests",
+    test_suite="nvm.tests",
     tests_require=test_requirements,
     extras_require=extra_requirements,
     url="https://github.com/cogsys-io/nvm",
     version=versioneer.get_version(),
     cmdclass=versioneer.get_cmdclass(),
     zip_safe=False,
 )
```

### Comparing `nvm-1.0.4/tests/test_nvm.py` & `nvm-1.0.5/nvm/tests/test_nvm.py`

 * *Files identical despite different names*

### Comparing `nvm-1.0.4/versioneer.py` & `nvm-1.0.5/versioneer.py`

 * *Files identical despite different names*

