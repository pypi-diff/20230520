# Comparing `tmp/GenomicRanges-0.2.8.tar.gz` & `tmp/GenomicRanges-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GenomicRanges-0.2.8.tar", last modified: Tue Mar 21 06:40:32 2023, max compression
+gzip compressed data, was "GenomicRanges-0.2.9.tar", last modified: Thu Mar 23 07:26:31 2023, max compression
```

## Comparing `GenomicRanges-0.2.8.tar` & `GenomicRanges-0.2.9.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-03-21 06:40:32.455570 GenomicRanges-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-03-21 06:39:19.000000 GenomicRanges-0.2.8/.coveragerc
-drwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-03-21 06:40:32.427570 GenomicRanges-0.2.8/.github/
-drwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-03-21 06:40:32.439570 GenomicRanges-0.2.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-03-21 06:39:19.000000 GenomicRanges-0.2.8/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-03-21 06:39:19.000000 GenomicRanges-0.2.8/.github/workflows/pypi-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-03-21 06:39:19.000000 GenomicRanges-0.2.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-03-21 06:39:19.000000 GenomicRanges-0.2.8/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-21 06:39:19.000000 GenomicRanges-0.2.8/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-03-21 06:39:19.000000 GenomicRanges-0.2.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    13937 2023-03-21 06:39:19.000000 GenomicRanges-0.2.8/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-03-21 06:39:19.000000 GenomicRanges-0.2.8/LICENSE.txt
--rw-rw-rw-   0 runner    (1001) docker     (123)     2785 2023-03-21 06:40:32.455570 GenomicRanges-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-03-21 06:39:19.000000 GenomicRanges-0.2.8/README.md
-drwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-03-21 06:40:32.443570 GenomicRanges-0.2.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-03-21 06:39:19.000000 GenomicRanges-0.2.8/docs/Makefile
-drwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-03-21 06:40:32.443570 GenomicRanges-0.2.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-21 06:39:19.000000 GenomicRanges-0.2.8/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-21 06:39:19.000000 GenomicRanges-0.2.8/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-03-21 06:39:19.000000 GenomicRanges-0.2.8/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)    10316 2023-03-21 06:39:19.000000 GenomicRanges-0.2.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-21 06:39:19.000000 GenomicRanges-0.2.8/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-03-21 06:39:19.000000 GenomicRanges-0.2.8/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-21 06:39:19.000000 GenomicRanges-0.2.8/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-03-21 06:39:19.000000 GenomicRanges-0.2.8/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-03-21 06:39:19.000000 GenomicRanges-0.2.8/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10403 2023-03-21 06:39:19.000000 GenomicRanges-0.2.8/docs/tutorial.md
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-03-21 06:39:19.000000 GenomicRanges-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-03-21 06:40:32.455570 GenomicRanges-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-03-21 06:39:19.000000 GenomicRanges-0.2.8/setup.py
-drwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-03-21 06:40:32.431570 GenomicRanges-0.2.8/src/
-drwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-03-21 06:40:32.447570 GenomicRanges-0.2.8/src/GenomicRanges.egg-info/
--rw-rw-rw-   0 runner    (1001) docker     (123)     2785 2023-03-21 06:40:32.000000 GenomicRanges-0.2.8/src/GenomicRanges.egg-info/PKG-INFO
--rw-rw-rw-   0 runner    (1001) docker     (123)     1463 2023-03-21 06:40:32.000000 GenomicRanges-0.2.8/src/GenomicRanges.egg-info/SOURCES.txt
--rw-rw-rw-   0 runner    (1001) docker     (123)        1 2023-03-21 06:40:32.000000 GenomicRanges-0.2.8/src/GenomicRanges.egg-info/dependency_links.txt
--rw-rw-rw-   0 runner    (1001) docker     (123)        1 2023-03-21 06:39:31.000000 GenomicRanges-0.2.8/src/GenomicRanges.egg-info/not-zip-safe
--rw-rw-rw-   0 runner    (1001) docker     (123)      123 2023-03-21 06:40:32.000000 GenomicRanges-0.2.8/src/GenomicRanges.egg-info/requires.txt
--rw-rw-rw-   0 runner    (1001) docker     (123)       14 2023-03-21 06:40:32.000000 GenomicRanges-0.2.8/src/GenomicRanges.egg-info/top_level.txt
-drwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-03-21 06:40:32.447570 GenomicRanges-0.2.8/src/genomicranges/
--rw-r--r--   0 runner    (1001) docker     (123)    71618 2023-03-21 06:39:19.000000 GenomicRanges-0.2.8/src/genomicranges/GenomicRanges.py
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-03-21 06:39:19.000000 GenomicRanges-0.2.8/src/genomicranges/SeqInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-03-21 06:39:19.000000 GenomicRanges-0.2.8/src/genomicranges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7304 2023-03-21 06:39:19.000000 GenomicRanges-0.2.8/src/genomicranges/_utils.py
-drwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-03-21 06:40:32.451570 GenomicRanges-0.2.8/src/genomicranges/io/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-21 06:39:19.000000 GenomicRanges-0.2.8/src/genomicranges/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-03-21 06:39:19.000000 GenomicRanges-0.2.8/src/genomicranges/io/gtf.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-03-21 06:39:19.000000 GenomicRanges-0.2.8/src/genomicranges/io/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-03-21 06:39:19.000000 GenomicRanges-0.2.8/src/genomicranges/io/tiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-03-21 06:39:19.000000 GenomicRanges-0.2.8/src/genomicranges/io/ucsc.py
--rw-r--r--   0 runner    (1001) docker     (123)    20218 2023-03-21 06:39:19.000000 GenomicRanges-0.2.8/src/genomicranges/utils.py
-drwxrwxrwx   0 runner    (1001) docker     (123)        0 2023-03-21 06:40:32.455570 GenomicRanges-0.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-03-21 06:39:19.000000 GenomicRanges-0.2.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-03-21 06:39:19.000000 GenomicRanges-0.2.8/tests/test_gr_binnedAvg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-03-21 06:39:19.000000 GenomicRanges-0.2.8/tests/test_gr_comparisons.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-03-21 06:39:19.000000 GenomicRanges-0.2.8/tests/test_gr_initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-03-21 06:39:19.000000 GenomicRanges-0.2.8/tests/test_gr_inter_range_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-03-21 06:39:19.000000 GenomicRanges-0.2.8/tests/test_gr_methods_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-03-21 06:39:19.000000 GenomicRanges-0.2.8/tests/test_gr_methods_coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-03-21 06:39:19.000000 GenomicRanges-0.2.8/tests/test_gr_methods_flank.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-03-21 06:39:19.000000 GenomicRanges-0.2.8/tests/test_gr_methods_other.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-03-21 06:39:19.000000 GenomicRanges-0.2.8/tests/test_gr_methods_resize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-03-21 06:39:19.000000 GenomicRanges-0.2.8/tests/test_gr_methods_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-03-21 06:39:19.000000 GenomicRanges-0.2.8/tests/test_gr_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-03-21 06:39:19.000000 GenomicRanges-0.2.8/tests/test_gr_overlaps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-03-21 06:39:19.000000 GenomicRanges-0.2.8/tests/test_gr_seqInfo_trim.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-03-21 06:39:19.000000 GenomicRanges-0.2.8/tests/test_gr_set_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-03-21 06:39:19.000000 GenomicRanges-0.2.8/tests/test_gr_tiling.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-03-21 06:39:19.000000 GenomicRanges-0.2.8/tests/test_seqInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-03-21 06:39:19.000000 GenomicRanges-0.2.8/tests/test_ucsc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-03-21 06:39:19.000000 GenomicRanges-0.2.8/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-03-21 06:39:19.000000 GenomicRanges-0.2.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 07:26:31.120940 GenomicRanges-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-03-23 07:25:25.000000 GenomicRanges-0.2.9/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 07:26:31.088939 GenomicRanges-0.2.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 07:26:31.100939 GenomicRanges-0.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-03-23 07:25:25.000000 GenomicRanges-0.2.9/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-03-23 07:25:25.000000 GenomicRanges-0.2.9/.github/workflows/pypi-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-03-23 07:25:25.000000 GenomicRanges-0.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-03-23 07:25:25.000000 GenomicRanges-0.2.9/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-23 07:25:25.000000 GenomicRanges-0.2.9/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-03-23 07:25:25.000000 GenomicRanges-0.2.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13937 2023-03-23 07:25:25.000000 GenomicRanges-0.2.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-03-23 07:25:25.000000 GenomicRanges-0.2.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-03-23 07:26:31.120940 GenomicRanges-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-03-23 07:25:25.000000 GenomicRanges-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 07:26:31.104939 GenomicRanges-0.2.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-03-23 07:25:25.000000 GenomicRanges-0.2.9/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 07:26:31.104939 GenomicRanges-0.2.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-23 07:25:25.000000 GenomicRanges-0.2.9/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-23 07:25:25.000000 GenomicRanges-0.2.9/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-03-23 07:25:25.000000 GenomicRanges-0.2.9/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10316 2023-03-23 07:25:25.000000 GenomicRanges-0.2.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-23 07:25:25.000000 GenomicRanges-0.2.9/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-03-23 07:25:25.000000 GenomicRanges-0.2.9/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-23 07:25:25.000000 GenomicRanges-0.2.9/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-03-23 07:25:25.000000 GenomicRanges-0.2.9/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-03-23 07:25:25.000000 GenomicRanges-0.2.9/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10403 2023-03-23 07:25:25.000000 GenomicRanges-0.2.9/docs/tutorial.md
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-03-23 07:25:25.000000 GenomicRanges-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-03-23 07:26:31.124940 GenomicRanges-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-03-23 07:25:25.000000 GenomicRanges-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 07:26:31.092939 GenomicRanges-0.2.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 07:26:31.108940 GenomicRanges-0.2.9/src/GenomicRanges.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-03-23 07:26:31.000000 GenomicRanges-0.2.9/src/GenomicRanges.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-03-23 07:26:31.000000 GenomicRanges-0.2.9/src/GenomicRanges.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 07:26:31.000000 GenomicRanges-0.2.9/src/GenomicRanges.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 07:25:35.000000 GenomicRanges-0.2.9/src/GenomicRanges.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-03-23 07:26:31.000000 GenomicRanges-0.2.9/src/GenomicRanges.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-23 07:26:31.000000 GenomicRanges-0.2.9/src/GenomicRanges.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 07:26:31.108940 GenomicRanges-0.2.9/src/genomicranges/
+-rw-r--r--   0 runner    (1001) docker     (123)    71424 2023-03-23 07:25:25.000000 GenomicRanges-0.2.9/src/genomicranges/GenomicRanges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-03-23 07:25:25.000000 GenomicRanges-0.2.9/src/genomicranges/SeqInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-03-23 07:25:25.000000 GenomicRanges-0.2.9/src/genomicranges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7304 2023-03-23 07:25:25.000000 GenomicRanges-0.2.9/src/genomicranges/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 07:26:31.112939 GenomicRanges-0.2.9/src/genomicranges/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-23 07:25:25.000000 GenomicRanges-0.2.9/src/genomicranges/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-03-23 07:25:25.000000 GenomicRanges-0.2.9/src/genomicranges/io/gtf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-03-23 07:25:25.000000 GenomicRanges-0.2.9/src/genomicranges/io/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-03-23 07:25:25.000000 GenomicRanges-0.2.9/src/genomicranges/io/tiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-03-23 07:25:25.000000 GenomicRanges-0.2.9/src/genomicranges/io/ucsc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19373 2023-03-23 07:25:25.000000 GenomicRanges-0.2.9/src/genomicranges/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 07:26:31.120940 GenomicRanges-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-03-23 07:25:25.000000 GenomicRanges-0.2.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-03-23 07:25:25.000000 GenomicRanges-0.2.9/tests/test_gr_binnedAvg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-03-23 07:25:25.000000 GenomicRanges-0.2.9/tests/test_gr_comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-03-23 07:25:25.000000 GenomicRanges-0.2.9/tests/test_gr_initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-03-23 07:25:25.000000 GenomicRanges-0.2.9/tests/test_gr_inter_range_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-03-23 07:25:25.000000 GenomicRanges-0.2.9/tests/test_gr_methods_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-03-23 07:25:25.000000 GenomicRanges-0.2.9/tests/test_gr_methods_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-03-23 07:25:25.000000 GenomicRanges-0.2.9/tests/test_gr_methods_flank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-03-23 07:25:25.000000 GenomicRanges-0.2.9/tests/test_gr_methods_other.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-03-23 07:25:25.000000 GenomicRanges-0.2.9/tests/test_gr_methods_resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-03-23 07:25:25.000000 GenomicRanges-0.2.9/tests/test_gr_methods_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-03-23 07:25:25.000000 GenomicRanges-0.2.9/tests/test_gr_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-03-23 07:25:25.000000 GenomicRanges-0.2.9/tests/test_gr_overlaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-03-23 07:25:25.000000 GenomicRanges-0.2.9/tests/test_gr_seqInfo_trim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-03-23 07:25:25.000000 GenomicRanges-0.2.9/tests/test_gr_set_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-03-23 07:25:25.000000 GenomicRanges-0.2.9/tests/test_gr_tiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-03-23 07:25:25.000000 GenomicRanges-0.2.9/tests/test_seqInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-03-23 07:25:25.000000 GenomicRanges-0.2.9/tests/test_ucsc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-03-23 07:25:25.000000 GenomicRanges-0.2.9/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-03-23 07:25:25.000000 GenomicRanges-0.2.9/tox.ini
```

### Comparing `GenomicRanges-0.2.8/.coveragerc` & `GenomicRanges-0.2.9/.coveragerc`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.2.8/.github/workflows/pypi-publish.yml` & `GenomicRanges-0.2.9/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.2.8/.github/workflows/pypi-test.yml` & `GenomicRanges-0.2.9/.github/workflows/pypi-test.yml`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.2.8/.gitignore` & `GenomicRanges-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.2.8/CONTRIBUTING.rst` & `GenomicRanges-0.2.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.2.8/LICENSE.txt` & `GenomicRanges-0.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.2.8/PKG-INFO` & `GenomicRanges-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GenomicRanges
-Version: 0.2.8
+Version: 0.2.9
 Summary: Represent genomic annotations in Python. Equivalent to Bioconductors [GRanges](https://bioconductor.org/packages/release/bioc/html/GenomicRanges.html)
 Home-page: https://github.com/BiocPy/GenomicRanges
 Author: jkanche
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/BiocPy/GenomicRanges
 Platform: any
```

### Comparing `GenomicRanges-0.2.8/README.md` & `GenomicRanges-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.2.8/docs/Makefile` & `GenomicRanges-0.2.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.2.8/docs/conf.py` & `GenomicRanges-0.2.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.2.8/docs/index.md` & `GenomicRanges-0.2.9/docs/index.md`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.2.8/docs/readme.md` & `GenomicRanges-0.2.9/docs/readme.md`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.2.8/docs/tutorial.md` & `GenomicRanges-0.2.9/docs/tutorial.md`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.2.8/setup.cfg` & `GenomicRanges-0.2.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 include_package_data = True
 package_dir = 
 	=src
 install_requires = 
 	importlib-metadata; python_version<"3.8"
 	pandas
 	joblib
-	biocframe>=0.2.8
+	biocframe>=0.2.10
 	numpy
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
```

### Comparing `GenomicRanges-0.2.8/setup.py` & `GenomicRanges-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.2.8/src/GenomicRanges.egg-info/PKG-INFO` & `GenomicRanges-0.2.9/src/GenomicRanges.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GenomicRanges
-Version: 0.2.8
+Version: 0.2.9
 Summary: Represent genomic annotations in Python. Equivalent to Bioconductors [GRanges](https://bioconductor.org/packages/release/bioc/html/GenomicRanges.html)
 Home-page: https://github.com/BiocPy/GenomicRanges
 Author: jkanche
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/BiocPy/GenomicRanges
 Platform: any
```

### Comparing `GenomicRanges-0.2.8/src/GenomicRanges.egg-info/SOURCES.txt` & `GenomicRanges-0.2.9/src/GenomicRanges.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.2.8/src/genomicranges/GenomicRanges.py` & `GenomicRanges-0.2.9/src/genomicranges/GenomicRanges.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,19 +42,19 @@
 __license__ = "MIT"
 
 
 class GenomicRanges(BiocFrame):
     """Class `GenomicRanges` represents genomic regions and annotations.
     
     Methods are available to load genome annotations from UCSC or 
-        from a pandas DataFrame.
+    from a pandas DataFrame.
 
     Note: Pandas DataFrame must contain columns seqnames, starts, ends and strand.
-        If strand column is not provided, * is used as the default value for each 
-        genomic interval.
+    If strand column is not provided, * is used as the default value for each 
+    genomic interval.
 
     ***Intervals are inclusive on both ends.***
 
     Additionally, `GenomicRanges` can also contain `Sequence Information` as 
     part of its metadata. In most cases, it usually contains for each sequence name 
     (or chromosome) in the object, its length. Sequence Information can also 
     contain additional metadata about the `genome`, and if its circular 
@@ -84,15 +84,15 @@
         Note: `data` must contain `seqnames`, `starts` and `ends` columns.
         If `strand` column is not provided, `*` is used as the default value
         for each genomic interval.
 
         Args:
             data (Mapping[str, Union[List[Any], Mapping]]): 
                 columns as dictionary, Must contain `seqnames`, `starts` and 
-                    `ends` columns.
+                `ends` columns.
             numberOfRows (int, optional): Number of genomic 
                 intervals (or rows). Defaults to None.
             rowNames (Sequence[str], optional): Row index. 
                 Defaults to None.
             columnNames (Sequence[str], optional): column names, 
                 automatically inferred from `data`. Defaults to None.
             metadata (Mapping, optional): metadata. Defaults to None.
@@ -187,15 +187,15 @@
                 return returnType(obj)
             except Exception as e:
                 raise ValueError(f"{returnType} not supported, {str(e)}")
 
     @property
     def strand(self) -> Sequence[str]:
         """Get strand information. If strand is originally not provided, 
-            we use '*' as a default value for each interval.
+        we use '*' as a default value for each interval.
 
         Returns:
             Sequence[str]: strand across all positions.
         """
         return self.column("strand")
 
     @property
@@ -321,15 +321,15 @@
         if self._metadata and "seqInfo" in self._metadata:
             return self._metadata["seqInfo"].genome
 
         return None
 
     def granges(self) -> "GenomicRanges":
         """Creates a new `GenomicRanges` object with only ranges 
-            (`seqnames`, `starts, `ends` and `strand`).
+        (`seqnames`, `starts, `ends` and `strand`).
 
         Returns:
             GenomicRanges: `GenomicRanges` with only ranges.
         """
         return GenomicRanges(
             {
                 "seqnames": self.column("seqnames"),
@@ -354,15 +354,15 @@
                 or any callable representation that takes a dictionary as an input.
 
         Raises:
             ValueError: if `returnType` is not supported.
 
         Returns:
             Union[pd.DataFrame, MutableMapping, Any]: metadata columns without 
-                genomic positions.
+            genomic positions.
         """
 
         new_data = OrderedDict()
         for k in self.columnNames:
             if k not in self.required_columns:
                 new_data[k] = self.column(k)
 
@@ -412,28 +412,27 @@
         self,
         width: int,
         start: bool = True,
         both: bool = False,
         ignoreStrand: bool = False,
     ) -> "GenomicRanges":
         """Generates flanking ranges for each range in the `GenomicRanges` 
-            object. The logic for this - 
+        object. The logic for this - 
 
         (from the R/GenomicRanges & IRanges packages)
 
         - If `start` is `True` for a given range, the flanking occurs at the start, 
-            otherwise the end. 
+        otherwise the end. 
         - The `widths` of the flanks are given by the `width` parameter. 
-            The widths can be negative, in which case the flanking region is 
-            reversed so that it represents a prefix or suffix of the range. 
+        The widths can be negative, in which case the flanking region is 
+        reversed so that it represents a prefix or suffix of the range. 
 
         Example:
-            gr.flank(3, True), 
-                where x indicates a range in gr and - indicates the resulting 
-                flanking region:
+            gr.flank(3, True), where x indicates a range in gr and 
+            - indicates the resulting flanking region:
 
                 ---xxxxxxx
 
             If start were FALSE, the range in gr becomes
 
                 xxxxxxx---
             
@@ -508,15 +507,15 @@
             metadata=self._metadata,
         )
 
     def resize(
         self, width: int, fix: str = "start", ignoreStrand: bool = False,
     ) -> "GenomicRanges":
         """Resize ranges to the specified `width` where either the `start`, 
-            `end`, or `center` is used as an anchor.
+        `end`, or `center` is used as an anchor.
 
         Args:
             width (int): width to resize, cannot be negative!.
             fix (str, optional): fix positions by `start`, `end` or `center`. 
                 Defaults to "start".
             ignoreStrand (bool, optional): ignore strand?. Defaults to False.
 
@@ -633,15 +632,15 @@
             upstream (int, optional): number of positions to extend in the 5' 
                 direction. Defaults to 2000.
             downstream (int, optional): number of positions to extend in the 3' 
                 direction. Defaults to 200.
 
         Returns:
             GenomicRanges: a new `GenomicRanges` object with ranges replaced 
-                by promoter regions.
+            by promoter regions.
         """
         all_starts = self.column("starts")
         all_ends = self.column("ends")
         all_strands = self.column("strand")
 
         start_flags = [all_strands[i] != "-" for i in range(len(all_strands))]
 
@@ -1015,20 +1014,19 @@
         """Identify gaps in genomic positions for each distinct 
         `seqname` (chromosome) and `strand` combination.
 
         Args:
             start (int, optional): restrict chromosome start position. Defaults to 1.
             end (Optional[MutableMapping[str, int]], optional): restrict end 
                 position for each chromosome. Defaults to None.
-                
                 If None, it uses the `SeqInfo` object if available.
 
         Returns:
             Optional["GenomicRanges"]: A new `GenomicRanges` containing 
-                gaps across chromosome and strand. If there are no gaps, returns None.
+            gaps across chromosome and strand. If there are no gaps, returns None.
         """
 
         # seqlengths = self._computeSeqLengths()
         seqlengths = self.seqlengths
 
         if end is None:
             end = seqlengths
@@ -1090,15 +1088,15 @@
         Args:
             withRevMap (bool, optional):return map of indices back to 
                 original object? . Defaults to False.
             ignoreStrand (bool, optional): ignore strand?. Defaults to False.
 
         Returns:
             Optional["GenomicRanges"]: A new `GenomicRanges` containing 
-                disjoint ranges across chromosome and strand.
+            disjoint ranges across chromosome and strand.
         """
 
         df_gr = self._generic_pandas_ranges(ignoreStrand=ignoreStrand, sort=True)
         groups = df_gr.groupby(["seqnames", "strand"])
 
         disjoin_intervals = []
         for name, group in groups:
@@ -1195,16 +1193,16 @@
             other (GenomicRanges): the other `GenomicRanges` object.
 
         Raises:
             TypeError: if other is not of type `GenomicRanges`.
 
         Returns:
             Optional["GenomicRanges"]: a new `GenomicRanges` object 
-                with intersection ranges. If there are no 
-                overlapping intervals, returns None.
+            with intersection ranges. If there are no 
+            overlapping intervals, returns None.
         """
 
         if not isinstance(other, GenomicRanges):
             raise TypeError("other is not a `GenomicRanges` object")
 
         a_df_gr = self._generic_pandas_ranges(sort=False)
         b_df_gr = other._generic_pandas_ranges(sort=False)
@@ -1244,15 +1242,15 @@
 
         Raises:
             TypeError: if other is not of type `GenomicRanges`.
             
         
         Returns:
             Optional["GenomicRanges"]: a new `GenomicRanges` object 
-                with the diff ranges. If there are intervals, returns None.
+            with the diff ranges. If there are intervals, returns None.
         """
 
         if not isinstance(other, GenomicRanges):
             raise TypeError("other is not a `GenomicRanges` object")
 
         a_df_gr = self._generic_pandas_ranges(sort=False)
         b_df_gr = other._generic_pandas_ranges(sort=False)
@@ -1302,29 +1300,29 @@
         final_df = final_df.sort_values(["seqnames", "strand", "starts", "ends"])
         return genomicranges.fromPandas(final_df)
 
     def binnedAverage(
         self, scorename: str, bins: "GenomicRanges", outname: str
     ) -> "GenomicRanges":
         """Calculate average for a column across all bins, then
-            set a column called `outname` with those values.
+        set a column called `outname` with those values.
 
         Args:
             scorename (str): the column to compute averages on.
             bins (GenomicRanges): bins you want to use.
             outname (str): new column name to add to the object.
 
         Raises:
             ValueError: if scorename column does not exist.
             Exception: scorename is not all ints or floats.
             TypeError: if bins is not of type `GenomicRanges`.
 
         Returns:
             GenomicRanges: a new `GenomicRanges` similar to bins, 
-                with a new column containing the averages.
+            with a new column containing the averages.
         """
 
         if not isinstance(bins, GenomicRanges):
             raise TypeError("bins is not a `GenomicRanges` object")
 
         if scorename not in self.columnNames:
             raise ValueError(f"{scorename} is not a valid column name")
@@ -1387,15 +1385,15 @@
         raise NotImplementedError
 
     # integer range methods
     def coverage(
         self, shift: int = 0, width: Optional[int] = None, weight: int = 1
     ) -> MutableMapping[str, np.ndarray]:
         """Calculate coverage for each chromosome, For each position, 
-            counts the number of ranges that cover it.
+        counts the number of ranges that cover it.
 
         Args:
             shift (int, optional): shift all genomic positions. Defaults to 0.
             width (int, optional): restrict the width of all 
                 chromosomes. Defaults to None.
             weight (int, optional): weight to use. Defaults to 1.
 
@@ -1441,30 +1439,30 @@
         ignoreStrand: bool = False,
     ) -> Optional["GenomicRanges"]:
         """Find overlaps between subject (self) and a query `GenomicRanges`.
 
         Args:
             query (GenomicRanges): query `GenomicRanges`.
             queryType (str, optional): overlap query type, must be one of 
-                "any": any overlap is good
-                "start": overlap at the beginning of the intervals
-                "end": must overlap at the end of the intervals
-                "within": Fully contain the query interval. 
+                - "any": any overlap is good
+                - "start": overlap at the beginning of the intervals
+                - "end": must overlap at the end of the intervals
+                - "within": Fully contain the query interval. 
                 Defaults to any.
             maxGap (int, optional): maximum gap allowed in the overlap. 
                 Defaults to -1 (no gap allowed).
             minOverlap (int, optional): minimum overlap with query. Defaults to 1. 
             ignoreStrand (bool, optional): ignore strand?. Defaults to False.
 
         Raises:
             TypeError: if query is not of type `GenomicRanges`.
             
         Returns:
             Optional["GenomicRanges"]: A new `GenomicRanges` object 
-                with the same length as query, containing hits to overlapping indices.
+            with the same length as query, containing hits to overlapping indices.
         """
 
         if not isinstance(query, GenomicRanges):
             raise TypeError("query is not a `GenomicRanges` object")
 
         if queryType not in OVERLAP_QUERY_TYPES:
             raise ValueError(f"{queryType} must be one of {OVERLAP_QUERY_TYPES}")
@@ -1530,18 +1528,18 @@
         ignoreStrand: bool = False,
     ) -> List[int]:
         """Count overlaps between `subject` (self) and a `query` genomic ranges.
 
         Args:
             query (GenomicRanges): query `GenomicRanges`.
             queryType (str, optional): overlap query type, must be one of 
-                    "any": any overlap is good
-                    "start": overlap at the beginning of the intervals
-                    "end": must overlap at the end of the intervals
-                    "within": Fully contain the query interval. 
+                - "any": any overlap is good
+                - "start": overlap at the beginning of the intervals
+                - "end": must overlap at the end of the intervals
+                - "within": Fully contain the query interval. 
                 Defaults to any.
             maxGap (int, optional): maximum gap allowed in the overlap. 
                 Defaults to -1 (no gap allowed).
             minOverlap (int, optional): minimum overlap with query. Defaults to 1. 
             ignoreStrand (bool, optional): ignore strand?. Defaults to False.
 
         Raises:
@@ -1577,30 +1575,30 @@
         ignoreStrand: bool = False,
     ) -> Optional["GenomicRanges"]:
         """Subset `subject` (self) with overlaps in `query` genomic ranges.
 
         Args:
             query (GenomicRanges): query `GenomicRanges`.
             queryType (str, optional): overlap query type, must be one of 
-                    "any": any overlap is good
-                    "start": overlap at the beginning of the intervals
-                    "end": must overlap at the end of the intervals
-                    "within": Fully contain the query interval. 
+                - "any": any overlap is good
+                - "start": overlap at the beginning of the intervals
+                - "end": must overlap at the end of the intervals
+                - "within": Fully contain the query interval. 
                 Defaults to any.
             maxGap (int, optional): maximum gap allowed in the overlap. 
                 Defaults to -1 (no gap allowed).
             minOverlap (int, optional): minimum overlap with query. Defaults to 1. 
             ignoreStrand (bool, optional): ignore strand?. Defaults to False.
 
         Raises:
             TypeError: if query is not of type `GenomicRanges`.
             
         Returns:
             Optional["GenomicRanges"]: A new `GenomicRanges` object 
-                containing only subsets for overlaps in query.
+            containing only subsets for overlaps in query.
         """
 
         if not isinstance(query, GenomicRanges):
             raise TypeError("query is not a `GenomicRanges` object")
 
         result = self.findOverlaps(
             query=query,
@@ -1629,16 +1627,16 @@
         """Internal function to search self and a query `GenomicRanges` object.
 
         Raises:
             TypeError: if query is not of type `GenomicRanges`
             
         Returns:
             Optional["GenomicRanges"]: a new `GenomicRanges` object that has 
-                the same length as query but contains `hits` to 
-                `indices` and `distance`.
+            the same length as query but contains `hits` to 
+            `indices` and `distance`.
         """
 
         if not isinstance(query, GenomicRanges):
             raise TypeError("query is not a `GenomicRanges` object")
 
         subject_gr = self._generic_pandas_ranges(ignoreStrand=ignoreStrand, sort=True)
         query_gr = query._generic_pandas_ranges(ignoreStrand=ignoreStrand, sort=True)
@@ -1687,93 +1685,93 @@
         final_df = final_df.sort_values(["seqnames", "strand", "starts", "ends"])
         return genomicranges.fromPandas(final_df)
 
     def nearest(
         self, query: "GenomicRanges", ignoreStrand: bool = False,
     ) -> Optional["GenomicRanges"]:
         """Search nearest positions both upstream and downstream that overlap with 
-            each range in `query`. 
+        each range in `query`. 
             
         Adds a new column to query called `hits`.
 
         Args:
             query (GenomicRanges): query `GenomicRanges` to find nearest positions.
             ignoreStrand (bool, optional): ignore strand? Defaults to False.
 
         Raises:
             TypeError: if query is not of type `GenomicRanges`.
             
         Returns:
             "GenomicRanges": a new `GenomicRanges` containing list of 
-                possible `hits` indices for each range in `query`.
+            possible `hits` indices for each range in `query`.
         """
         return self._generic_search(query=query, ignoreStrand=ignoreStrand)
 
     def precede(
         self, query: "GenomicRanges", ignoreStrand: bool = False,
     ) -> Optional["GenomicRanges"]:
         """Search nearest positions only downstream that overlap with 
-            each range in `query`.
-            
+        each range in `query`.
+
         Adds a new column to query called `hits`.
 
         Args:
             query (GenomicRanges): query `GenomicRanges` to find nearest positions.
             ignoreStrand (bool, optional): ignore strand? Defaults to False.
 
         Raises:
             TypeError: if query is not of type `GenomicRanges`.
             
         Returns:
             "GenomicRanges": a new `GenomicRanges` containing list of possible 
-                `hits` indices for each range in `query`
+            `hits` indices for each range in `query`
         """
         return self._generic_search(query=query, ignoreStrand=ignoreStrand, stepend=0)
 
     def follow(
         self, query: "GenomicRanges", ignoreStrand: bool = False,
     ) -> Optional["GenomicRanges"]:
         """Search nearest positions only upstream that overlap with 
-            each range in `query`. 
+        each range in `query`. 
             
         Adds a new column to query called `hits`.
 
         Args:
             query (GenomicRanges): query `GenomicRanges` to find nearest positions.
             ignoreStrand (bool, optional): ignore strand? Defaults to False.
 
         Raises:
             TypeError: if query is not of type `GenomicRanges`.
             
         Returns:
             "GenomicRanges": a new `GenomicRanges` containing list of possible 
-                `hits` indices for each range in `query`.
+            `hits` indices for each range in `query`.
         """
         return self._generic_search(query=query, ignoreStrand=ignoreStrand, stepstart=0)
 
     def distanceToNearest(
         self, query: "GenomicRanges", ignoreStrand: bool = False,
     ) -> Optional["GenomicRanges"]:
         """Search nearest positions only downstream that overlap with 
-            each range in `query`. 
+        each range in `query`. 
             
         Adds a new column to query called `hits`.
         
         Note: Technically same as nearest since we also return `distances`.
 
         Args:
             query (GenomicRanges): query `GenomicRanges` to find nearest positions.
             ignoreStrand (bool, optional): ignore strand? Defaults to False.
 
         Raises:
             TypeError: if query is not of type `GenomicRanges`.
             
         Returns:
             "GenomicRanges": a new `GenomicRanges` containing list of possible 
-                `hits` indices for each range in `query`.
+            `hits` indices for each range in `query`.
         """
         return self._generic_search(query=query, ignoreStrand=ignoreStrand)
 
     # compare and order methods
     def duplicated(self,) -> Sequence[bool]:
         """Element wise comparison to find duplicate ranges.
 
@@ -1908,15 +1906,15 @@
             order = order[::-1]
 
         new_order = order.to_list()
         return self[new_order, :]
 
     def rank(self) -> Sequence[int]:
         """Get rank of the `GenomicRanges` object. 
-            for each ranges identifies its position is a sorted order.
+        for each ranges identifies its position is a sorted order.
 
         Returns:
             Sequence[int]: list of indices identifying rank.
         """
         order = self._generic_order().to_list()
         rank = [order.index(x) for x in range(len(order))]
         return rank
```

### Comparing `GenomicRanges-0.2.8/src/genomicranges/SeqInfo.py` & `GenomicRanges-0.2.9/src/genomicranges/SeqInfo.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 class SeqInfo(BiocFrame):
     required_columns = ["seqnames"]
     can_contain = ["seqnames", "seqlengths", "isCircular", "genome"]
 
     def __init__(
         self,
-        data: Optional[MutableMapping[str, Union[List[Any], MutableMapping]]] = None,
+        data: MutableMapping[str, Union[List[Any], MutableMapping]],
         numberOfRows: Optional[int] = None,
         rowNames: Optional[Sequence[str]] = None,
         columnNames: Optional[Sequence[str]] = None,
         metadata: Optional[MutableMapping] = None,
     ) -> None:
         super().__init__(data, numberOfRows, rowNames, columnNames, metadata)
```

### Comparing `GenomicRanges-0.2.8/src/genomicranges/__init__.py` & `GenomicRanges-0.2.9/src/genomicranges/__init__.py`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.2.8/src/genomicranges/_utils.py` & `GenomicRanges-0.2.9/src/genomicranges/_utils.py`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.2.8/src/genomicranges/io/gtf.py` & `GenomicRanges-0.2.9/src/genomicranges/io/gtf.py`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.2.8/src/genomicranges/io/pdf.py` & `GenomicRanges-0.2.9/src/genomicranges/io/pdf.py`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.2.8/src/genomicranges/io/tiling.py` & `GenomicRanges-0.2.9/src/genomicranges/io/tiling.py`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.2.8/src/genomicranges/io/ucsc.py` & `GenomicRanges-0.2.9/src/genomicranges/io/ucsc.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 __author__ = "jkanche"
 __copyright__ = "jkanche"
 __license__ = "MIT"
 
 
 def access_gtf_ucsc(genome: str, type: str = "refGene") -> str:
     """Generate a path to a genome gtf file from UCSC 
-        e.g. (http://hgdownload.cse.ucsc.edu/goldenPath/hg19/bigZips/genes/).
+    e.g. (http://hgdownload.cse.ucsc.edu/goldenPath/hg19/bigZips/genes/).
 
     Args:
         genome (str): genome shortcode; e.g. hg19, hg38, mm10 etc.
         type (str): One of refGene, ensGene, knownGene or ncbiRefSeq.
 
     Raises:
         Exception: ValueError, when `type` does not match with a valid input.
```

### Comparing `GenomicRanges-0.2.8/src/genomicranges/utils.py` & `GenomicRanges-0.2.9/src/genomicranges/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from random import random
 
 
 def calc_row_gapwidth(
     a: MutableMapping[str, Any], b: MutableMapping[str, Any]
 ) -> Optional[int]:
     """Given two genomic positions from GenomicRanges, calculates gapwidth
-        returns 
+    returns 
         - `nan` if the sequences are not comparable
         - 0 if they overlap
         - a number if there is a gap
 
     Args:
         a (MutableMapping[str, Any]): a row from `GenomicRanges`.
         b (MutableMapping[str, Any]): a row from `GenomicRanges`.
@@ -38,15 +38,15 @@
 
     Args:
         ary (np.ndarray): a numpy array.
         step (int, optional): value to split consecutive intervals by.
 
     Returns:
         Tuple(List[np.ndarray], List[np.ndarray]): tuple with indices 
-            and their coverage.
+        and their coverage.
     """
     return [
         (x[0], x[1])
         for x in zip(
             np.split(range(len(ary)), np.where(np.diff(ary) != step)[0] + 1),
             np.split(ary, np.where(np.diff(ary) != step)[0] + 1),
         )
@@ -67,15 +67,15 @@
         withRevMap (bool, optional): return map of indices. Defaults to False.
         forceSize (int, optional): force size of the array.
         dontSum (bool, optional): do not sum. Defaults to False.
         value (int, optional): default value to increment. Defaults to 1.
 
     Returns:
         Tuple[np.ndarray, Optional[List]]: a numpy array representing 
-            coverage from the intervals.
+        coverage from the intervals.
     """
     if len(intervals) < 1:
         return intervals
 
     max_end = forceSize
     if max_end is None:
         max_end = max([x[1] for x in intervals])
@@ -106,15 +106,15 @@
 
     Args:
         intervals (List[Tuple[int, int]]): input interval vector.
         withRevMap (bool, optional): return map of indices. Defaults to False.
 
     Returns:
         Union[List[Tuple[int, int, Optional[List[int]]]], List[Tuple[int, int]]]: List 
-            containing tuples with (start, end, indices) for each contiguous region.
+        containing tuples with (start, end, indices) for each contiguous region.
     """
     np_intvals, revmap = create_np_interval_vector(
         intervals=intervals, withRevMap=withRevMap
     )
 
     # splitting intervals by where gaps=0 gives us the union of all intervals
     groups = [
@@ -161,15 +161,15 @@
     Args:
         intervals (List[Tuple[int, int]]): input interval vector.
         start_limit (int, optional): start for identifying gaps. Defaults to 1.
         end_limit (int, optional): end interval. Defaults to None.
 
     Returns:
         List[Tuple[int, int]]: List of tuples with 
-            (start, end) for each gap.
+        (start, end) for each gap.
     """
 
     min_start = start_limit
     if min_start is None:
         min_start = min([x[0] for x in intervals])
 
     max_end = end_limit
@@ -215,15 +215,15 @@
 
     Args:
         intervals (List[Tuple[int, int]]): input interval vector.
         withRevMap (bool, optional): return map of indices. Defaults to False.
 
     Returns:
         Union[List[Tuple[int, int, Optional[List[int]]]], List[Tuple[int, int]]]: List 
-            of tuples with (start, end).
+        of tuples with (start, end).
     """
     np_intvals, revmap = create_np_interval_vector(
         intervals=intervals, withRevMap=withRevMap
     )
 
     # its isn't enough, so lets add some randomless to distinguish each interval
     for itval in intervals:
@@ -279,15 +279,15 @@
     Args:
         intervals (List[Tuple[int, int]]): input interval vector.
         withRevMap (bool, optional): return map of indices?. Defaults to False.
         threshold (int, optional): threshold for cutoff. Defaults to 1.
 
     Returns:
         Union[List[Tuple[int, int, Optional[List[int]]]], List[Tuple[int, int]]]: List 
-            containing tuples with (start, end, indices) for each contiguous region.
+        containing tuples with (start, end, indices) for each contiguous region.
     """
     np_intvals, revmap = create_np_interval_vector(
         intervals=intervals, withRevMap=withRevMap
     )
 
     min_start = min([x[0] for x in intervals])
     max_end = max(x[1] for x in intervals)
@@ -417,42 +417,14 @@
 def compute_mean(
     intervals: List[Tuple[int, int]], values: Union[List[int], List[float]]
 ) -> Tuple[np.ndarray, np.ndarray]:
     """Compute coverage and sum ndarrays.
 
     Args:
         intervals (List[Tuple[int, int]]): input interval list.
-        values (Union[List[int], List[float]]): an int or float vector with the 
-            same size as intervals.
-
-    Returns:
-        Tuple[np.ndarray, np.ndarray]: a tuple with coverage and sum noarrays.
-    """
-    max_end = None
-    if max_end is None:
-        max_end = max([x[1] for x in intervals])
-
-    np_cov = np.zeros(max_end)
-    np_sum = np.zeros(max_end)
-
-    for idx in range(len(intervals)):
-        i = intervals[idx]
-        np_cov[i[0] - 1 : i[1]] += 1
-        np_sum[i[0] - 1 : i[1]] += values[idx]
-
-    return (np_cov, np_sum)
-
-
-def compute_mean(
-    intervals: List[Tuple[int, int]], values: Union[List[int], List[float]]
-) -> Tuple[np.ndarray, np.ndarray]:
-    """Compute coverage and sum ndarrays.
-
-    Args:
-        intervals (List[Tuple[int, int]]): input interval list.
         values (Union[List[int], List[float]]): an int or float vector with 
             the same size as intervals.
 
     Returns:
         Tuple[np.ndarray, np.ndarray]: a tuple with coverage and sum noarrays.
     """
     max_end = None
@@ -496,15 +468,15 @@
             Defaults to "any".
 
     Raises:
         ValueError: query type is incorrect.
 
     Returns:
         List[Tuple[Tuple[int, int], int, List[int]]]: list of query intervals 
-            with their overlaps.
+        with their overlaps.
     """
     if queryType not in OVERLAP_QUERY_TYPES:
         raise ValueError(f"{queryType} must be one of {OVERLAP_QUERY_TYPES}")
 
     subject_ints, subject_revmap = create_np_interval_vector(
         intervals=subject, withRevMap=True
     )
@@ -551,15 +523,15 @@
         query (List[Tuple[int, int]]): query intervals.
         maxGap (int, optional): maximum gap allowed. Defaults to -1 for no gaps.
         stepstart (int, optional): step start. Defaults to 3.
         stepend (int, optional): step end. Defaults to 3.
 
     Returns:
         List[Tuple[Tuple[int, int], int, List[int]]]: list of query intervals 
-            with their overlaps.
+        with their overlaps.
     """
     _, subject_revmap = create_np_interval_vector(intervals=subject, withRevMap=True)
 
     hits = []
     for idx in range(len(query)):
         q = query[idx]
 
@@ -599,15 +571,15 @@
     return hits
 
 
 def split_intervals(
     chrom: str, strand: str, start: int, end: int, step: int
 ) -> List[Tuple]:
     """split an interval range into equal bins. pretty much a fancy range function.
-        realizes the range.
+    realizes the range.
 
     Args:
         chrom (str): chrom.
         strand (str): strand.
         start (int): start interval.
         end (int): end interval.
         step (int): width or step of each interval.
@@ -622,15 +594,15 @@
     return bins
 
 
 def slide_intervals(
     chrom: str, strand: str, start: int, end: int, width: int, step: int
 ):
     """Sliding intervals. pretty much a fancy range function.
-        realizes the range.
+    realizes the range.
 
     Args:
         chrom (str): chrom.
         strand (str): strand.
         start (int): start interval.
         end (int): end interval.
         step (int): width or step of each interval.
```

### Comparing `GenomicRanges-0.2.8/tests/test_gr_binnedAvg.py` & `GenomicRanges-0.2.9/tests/test_gr_binnedAvg.py`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.2.8/tests/test_gr_comparisons.py` & `GenomicRanges-0.2.9/tests/test_gr_comparisons.py`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.2.8/tests/test_gr_initialize.py` & `GenomicRanges-0.2.9/tests/test_gr_initialize.py`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.2.8/tests/test_gr_inter_range_methods.py` & `GenomicRanges-0.2.9/tests/test_gr_inter_range_methods.py`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.2.8/tests/test_gr_methods_basic.py` & `GenomicRanges-0.2.9/tests/test_gr_methods_basic.py`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.2.8/tests/test_gr_methods_coverage.py` & `GenomicRanges-0.2.9/tests/test_gr_methods_coverage.py`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.2.8/tests/test_gr_methods_flank.py` & `GenomicRanges-0.2.9/tests/test_gr_methods_flank.py`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.2.8/tests/test_gr_methods_other.py` & `GenomicRanges-0.2.9/tests/test_gr_methods_other.py`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.2.8/tests/test_gr_methods_resize.py` & `GenomicRanges-0.2.9/tests/test_gr_methods_resize.py`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.2.8/tests/test_gr_methods_search.py` & `GenomicRanges-0.2.9/tests/test_gr_methods_search.py`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.2.8/tests/test_gr_misc.py` & `GenomicRanges-0.2.9/tests/test_gr_misc.py`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.2.8/tests/test_gr_overlaps.py` & `GenomicRanges-0.2.9/tests/test_gr_overlaps.py`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.2.8/tests/test_gr_seqInfo_trim.py` & `GenomicRanges-0.2.9/tests/test_gr_seqInfo_trim.py`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.2.8/tests/test_gr_set_ops.py` & `GenomicRanges-0.2.9/tests/test_gr_set_ops.py`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.2.8/tests/test_gr_tiling.py` & `GenomicRanges-0.2.9/tests/test_gr_tiling.py`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.2.8/tests/test_seqInfo.py` & `GenomicRanges-0.2.9/tests/test_seqInfo.py`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.2.8/tests/test_utils.py` & `GenomicRanges-0.2.9/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `GenomicRanges-0.2.8/tox.ini` & `GenomicRanges-0.2.9/tox.ini`

 * *Files identical despite different names*

