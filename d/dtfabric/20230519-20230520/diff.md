# Comparing `tmp/dtfabric-20230519.tar.gz` & `tmp/dtfabric-20230520.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtfabric-20230519.tar", last modified: Fri May 19 02:58:48 2023, max compression
+gzip compressed data, was "dtfabric-20230520.tar", last modified: Sat May 20 03:30:20 2023, max compression
```

## Comparing `dtfabric-20230519.tar` & `dtfabric-20230520.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 02:58:48.302414 dtfabric-20230519/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 02:58:47.998414 dtfabric-20230519/.github/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 02:58:48.076414 dtfabric-20230519/.github/workflows/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2541 2023-05-12 04:16:07.000000 dtfabric-20230519/.github/workflows/test_docker.yml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1378 2023-05-12 04:16:07.000000 dtfabric-20230519/.github/workflows/test_docs.yml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4107 2023-05-12 04:16:07.000000 dtfabric-20230519/.github/workflows/test_tox.yml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    22994 2023-05-12 04:16:07.000000 dtfabric-20230519/.pylintrc
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      149 2022-07-10 04:44:41.000000 dtfabric-20230519/.yamllint.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       92 2022-01-24 07:36:34.000000 dtfabric-20230519/ACKNOWLEDGEMENTS
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      265 2018-07-03 18:38:13.000000 dtfabric-20230519/AUTHORS
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11358 2016-09-25 06:41:25.000000 dtfabric-20230519/LICENSE
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      592 2021-08-22 05:30:09.000000 dtfabric-20230519/MANIFEST.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      583 2023-05-19 02:58:48.302414 dtfabric-20230519/PKG-INFO
--rw-r-----   0 lordyesta  (1000) lordyesta  (1000)      195 2020-06-21 05:38:03.000000 dtfabric-20230519/README
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2023-05-12 04:16:07.000000 dtfabric-20230519/appveyor.yml
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 02:58:47.998414 dtfabric-20230519/config/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 02:58:48.078414 dtfabric-20230519/config/appveyor/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      839 2023-05-12 04:16:07.000000 dtfabric-20230519/config/appveyor/install.ps1
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      125 2023-05-12 04:16:07.000000 dtfabric-20230519/config/appveyor/install.sh
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      620 2023-05-12 04:16:07.000000 dtfabric-20230519/config/appveyor/runtests.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 02:58:48.138414 dtfabric-20230519/config/dpkg/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      140 2023-05-19 02:56:42.000000 dtfabric-20230519/config/dpkg/changelog
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       38 2017-05-26 07:25:10.000000 dtfabric-20230519/config/dpkg/clean
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        2 2023-05-12 04:16:07.000000 dtfabric-20230519/config/dpkg/compat
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      786 2023-05-12 04:16:07.000000 dtfabric-20230519/config/dpkg/control
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      884 2017-04-14 13:14:48.000000 dtfabric-20230519/config/dpkg/copyright
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       20 2017-04-14 13:31:35.000000 dtfabric-20230519/config/dpkg/dtfabric-data.dirs
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       26 2017-04-14 13:32:40.000000 dtfabric-20230519/config/dpkg/dtfabric-data.install
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      144 2017-05-26 07:25:20.000000 dtfabric-20230519/config/dpkg/python-dtfabric.install
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      144 2017-05-26 07:25:27.000000 dtfabric-20230519/config/dpkg/python3-dtfabric.install
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      122 2023-05-12 04:16:07.000000 dtfabric-20230519/config/dpkg/rules
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 02:58:48.138414 dtfabric-20230519/config/dpkg/source/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       12 2017-04-14 13:14:48.000000 dtfabric-20230519/config/dpkg/source/format
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 02:58:48.139414 dtfabric-20230519/config/pylint/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      362 2020-06-21 09:14:13.000000 dtfabric-20230519/config/pylint/spelling-private-dict
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      151 2020-01-19 18:45:05.000000 dtfabric-20230519/dependencies.ini
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 02:58:48.155414 dtfabric-20230519/docs/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5061 2023-05-12 04:16:07.000000 dtfabric-20230519/docs/conf.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      566 2021-07-30 06:46:25.000000 dtfabric-20230519/docs/index.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      105 2023-05-12 04:16:16.000000 dtfabric-20230519/docs/requirements.txt
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 02:58:48.155414 dtfabric-20230519/docs/sources/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    15554 2022-07-10 05:53:49.000000 dtfabric-20230519/docs/sources/Format-specification.md
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 02:58:48.156414 dtfabric-20230519/docs/sources/api/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1097 2022-02-19 13:55:33.000000 dtfabric-20230519/docs/sources/api/dtfabric.rst
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      869 2021-07-30 06:46:25.000000 dtfabric-20230519/docs/sources/api/dtfabric.runtime.rst
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       61 2021-07-30 06:37:51.000000 dtfabric-20230519/docs/sources/api/modules.rst
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 02:58:48.156414 dtfabric-20230519/docs/sources/user/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1633 2021-12-28 03:59:54.000000 dtfabric-20230519/docs/sources/user/Installation-instructions.md
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      288 2021-07-30 06:37:51.000000 dtfabric-20230519/docs/sources/user/index.rst
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 02:58:48.158414 dtfabric-20230519/dtfabric/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       74 2023-05-19 02:56:42.000000 dtfabric-20230519/dtfabric/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31346 2023-05-14 14:27:49.000000 dtfabric-20230519/dtfabric/data_types.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      710 2022-09-18 09:38:10.000000 dtfabric-20230519/dtfabric/decorators.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1502 2021-07-30 10:44:15.000000 dtfabric-20230519/dtfabric/definitions.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1016 2021-07-30 06:46:25.000000 dtfabric-20230519/dtfabric/errors.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    52825 2023-05-18 03:12:53.000000 dtfabric-20230519/dtfabric/reader.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3192 2022-09-18 09:35:13.000000 dtfabric-20230519/dtfabric/registry.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 02:58:48.161414 dtfabric-20230519/dtfabric/runtime/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2018-03-18 06:58:01.000000 dtfabric-20230519/dtfabric/runtime/__init__.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2523 2022-09-18 09:36:04.000000 dtfabric-20230519/dtfabric/runtime/byte_operations.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    76538 2023-05-18 17:48:42.000000 dtfabric-20230519/dtfabric/runtime/data_maps.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2022-01-27 14:27:48.000000 dtfabric-20230519/dtfabric/runtime/fabric.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6233 2022-09-18 09:46:53.000000 dtfabric-20230519/dtfabric/runtime/runtime.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 02:58:48.160414 dtfabric-20230519/dtfabric.egg-info/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      583 2023-05-19 02:58:46.000000 dtfabric-20230519/dtfabric.egg-info/PKG-INFO
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2835 2023-05-19 02:58:47.000000 dtfabric-20230519/dtfabric.egg-info/SOURCES.txt
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        1 2023-05-19 02:58:46.000000 dtfabric-20230519/dtfabric.egg-info/dependency_links.txt
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-05-19 02:58:46.000000 dtfabric-20230519/dtfabric.egg-info/requires.txt
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        9 2023-05-19 02:58:46.000000 dtfabric-20230519/dtfabric.egg-info/top_level.txt
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      395 2019-02-03 12:58:57.000000 dtfabric-20230519/dtfabric.ini
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       28 2023-05-12 04:16:07.000000 dtfabric-20230519/requirements.txt
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      777 2022-09-18 09:32:38.000000 dtfabric-20230519/run_tests.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 02:58:48.161414 dtfabric-20230519/scripts/
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)     3218 2022-09-18 08:56:58.000000 dtfabric-20230519/scripts/validate-definitions.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      302 2023-05-19 02:58:48.303414 dtfabric-20230519/setup.cfg
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)     6782 2023-05-12 04:16:07.000000 dtfabric-20230519/setup.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 02:58:48.187414 dtfabric-20230519/test_data/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1426 2017-05-01 13:58:49.000000 dtfabric-20230519/test_data/Notepad.lnk
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       99 2022-07-10 05:55:10.000000 dtfabric-20230519/test_data/boolean.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      101 2022-07-10 05:55:12.000000 dtfabric-20230519/test_data/character.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      284 2022-07-10 05:55:13.000000 dtfabric-20230519/test_data/constant.yaml
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 02:58:48.188414 dtfabric-20230519/test_data/definitions/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      524 2022-07-10 05:54:56.000000 dtfabric-20230519/test_data/definitions/booleans.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      453 2022-07-10 05:54:58.000000 dtfabric-20230519/test_data/definitions/characters.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      405 2022-07-10 05:55:00.000000 dtfabric-20230519/test_data/definitions/floating-points.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1364 2022-07-10 05:55:01.000000 dtfabric-20230519/test_data/definitions/integers.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      812 2022-07-10 05:55:15.000000 dtfabric-20230519/test_data/enumeration.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      218 2022-07-10 05:55:16.000000 dtfabric-20230519/test_data/floating-point.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      555 2022-07-10 05:55:18.000000 dtfabric-20230519/test_data/format.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      399 2022-07-10 05:55:19.000000 dtfabric-20230519/test_data/integer.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       83 2022-07-10 05:55:23.000000 dtfabric-20230519/test_data/padding.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      457 2022-07-10 05:55:28.000000 dtfabric-20230519/test_data/sequence.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      572 2022-07-10 05:55:25.000000 dtfabric-20230519/test_data/sequence_with_context.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      433 2023-05-18 05:56:24.000000 dtfabric-20230519/test_data/sequence_with_structure.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      657 2022-07-10 05:55:29.000000 dtfabric-20230519/test_data/stream.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      707 2022-07-10 05:55:32.000000 dtfabric-20230519/test_data/string.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      818 2022-07-10 05:55:30.000000 dtfabric-20230519/test_data/string_array.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1059 2022-07-10 05:55:50.000000 dtfabric-20230519/test_data/structure.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2022-07-10 05:55:34.000000 dtfabric-20230519/test_data/structure_family.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1576 2022-07-10 05:55:35.000000 dtfabric-20230519/test_data/structure_group.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      651 2022-07-10 05:55:36.000000 dtfabric-20230519/test_data/structure_with_condition.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      496 2022-07-10 05:55:38.000000 dtfabric-20230519/test_data/structure_with_context.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      712 2022-07-10 05:57:13.000000 dtfabric-20230519/test_data/structure_with_padding.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      322 2022-07-10 05:55:41.000000 dtfabric-20230519/test_data/structure_with_section.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      468 2022-07-10 05:55:43.000000 dtfabric-20230519/test_data/structure_with_sequence.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      466 2022-07-10 05:55:44.000000 dtfabric-20230519/test_data/structure_with_stream.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      446 2022-07-10 05:55:45.000000 dtfabric-20230519/test_data/structure_with_string.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      370 2022-07-10 05:55:47.000000 dtfabric-20230519/test_data/structure_with_union.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      700 2022-07-10 05:55:49.000000 dtfabric-20230519/test_data/structure_with_values.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      383 2022-07-10 05:55:53.000000 dtfabric-20230519/test_data/union.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      380 2022-07-10 05:55:51.000000 dtfabric-20230519/test_data/union_with_condition.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      200 2022-07-10 05:55:54.000000 dtfabric-20230519/test_data/uuid.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      107 2022-12-18 07:46:44.000000 dtfabric-20230519/test_dependencies.ini
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       14 2023-05-12 04:16:07.000000 dtfabric-20230519/test_requirements.txt
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 02:58:48.241414 dtfabric-20230519/tests/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2018-03-18 06:58:01.000000 dtfabric-20230519/tests/__init__.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    19685 2022-02-13 10:09:16.000000 dtfabric-20230519/tests/data_types.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    62234 2023-05-18 03:22:07.000000 dtfabric-20230519/tests/reader.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3002 2021-07-30 06:46:25.000000 dtfabric-20230519/tests/registry.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 02:58:48.295414 dtfabric-20230519/tests/runtime/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2018-03-18 06:58:01.000000 dtfabric-20230519/tests/runtime/__init__.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1645 2021-07-30 09:04:50.000000 dtfabric-20230519/tests/runtime/byte_operations.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    84696 2023-05-18 15:50:47.000000 dtfabric-20230519/tests/runtime/data_maps.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      662 2021-07-30 06:46:25.000000 dtfabric-20230519/tests/runtime/fabric.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2494 2021-07-30 06:46:25.000000 dtfabric-20230519/tests/runtime/runtime.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2272 2022-09-18 09:32:59.000000 dtfabric-20230519/tests/test_lib.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1252 2023-05-12 04:16:07.000000 dtfabric-20230519/tox.ini
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-19 02:58:48.302414 dtfabric-20230519/utils/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       70 2018-03-18 06:58:04.000000 dtfabric-20230519/utils/__init__.py
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      422 2023-05-12 04:16:07.000000 dtfabric-20230519/utils/check_dependencies.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11583 2023-05-12 04:16:07.000000 dtfabric-20230519/utils/dependencies.py
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      616 2021-12-28 04:01:20.000000 dtfabric-20230519/utils/update_release.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-20 03:30:20.439226 dtfabric-20230520/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-20 03:30:20.167226 dtfabric-20230520/.github/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-20 03:30:20.261226 dtfabric-20230520/.github/workflows/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2541 2023-05-12 04:16:07.000000 dtfabric-20230520/.github/workflows/test_docker.yml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1378 2023-05-12 04:16:07.000000 dtfabric-20230520/.github/workflows/test_docs.yml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4107 2023-05-12 04:16:07.000000 dtfabric-20230520/.github/workflows/test_tox.yml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    22994 2023-05-12 04:16:07.000000 dtfabric-20230520/.pylintrc
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      149 2022-07-10 04:44:41.000000 dtfabric-20230520/.yamllint.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       92 2022-01-24 07:36:34.000000 dtfabric-20230520/ACKNOWLEDGEMENTS
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      265 2018-07-03 18:38:13.000000 dtfabric-20230520/AUTHORS
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11358 2016-09-25 06:41:25.000000 dtfabric-20230520/LICENSE
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      592 2021-08-22 05:30:09.000000 dtfabric-20230520/MANIFEST.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      583 2023-05-20 03:30:20.439226 dtfabric-20230520/PKG-INFO
+-rw-r-----   0 lordyesta  (1000) lordyesta  (1000)      195 2020-06-21 05:38:03.000000 dtfabric-20230520/README
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2023-05-12 04:16:07.000000 dtfabric-20230520/appveyor.yml
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-20 03:30:20.168226 dtfabric-20230520/config/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-20 03:30:20.262226 dtfabric-20230520/config/appveyor/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      839 2023-05-12 04:16:07.000000 dtfabric-20230520/config/appveyor/install.ps1
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      125 2023-05-12 04:16:07.000000 dtfabric-20230520/config/appveyor/install.sh
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      620 2023-05-12 04:16:07.000000 dtfabric-20230520/config/appveyor/runtests.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-20 03:30:20.331226 dtfabric-20230520/config/dpkg/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      140 2023-05-20 03:28:59.000000 dtfabric-20230520/config/dpkg/changelog
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       38 2017-05-26 07:25:10.000000 dtfabric-20230520/config/dpkg/clean
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        2 2023-05-12 04:16:07.000000 dtfabric-20230520/config/dpkg/compat
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      786 2023-05-12 04:16:07.000000 dtfabric-20230520/config/dpkg/control
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      884 2017-04-14 13:14:48.000000 dtfabric-20230520/config/dpkg/copyright
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       20 2017-04-14 13:31:35.000000 dtfabric-20230520/config/dpkg/dtfabric-data.dirs
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       26 2017-04-14 13:32:40.000000 dtfabric-20230520/config/dpkg/dtfabric-data.install
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      144 2017-05-26 07:25:20.000000 dtfabric-20230520/config/dpkg/python-dtfabric.install
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      144 2017-05-26 07:25:27.000000 dtfabric-20230520/config/dpkg/python3-dtfabric.install
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      122 2023-05-12 04:16:07.000000 dtfabric-20230520/config/dpkg/rules
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-20 03:30:20.331226 dtfabric-20230520/config/dpkg/source/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       12 2017-04-14 13:14:48.000000 dtfabric-20230520/config/dpkg/source/format
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-20 03:30:20.332226 dtfabric-20230520/config/pylint/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      362 2020-06-21 09:14:13.000000 dtfabric-20230520/config/pylint/spelling-private-dict
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      151 2020-01-19 18:45:05.000000 dtfabric-20230520/dependencies.ini
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-20 03:30:20.347226 dtfabric-20230520/docs/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5061 2023-05-12 04:16:07.000000 dtfabric-20230520/docs/conf.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      566 2021-07-30 06:46:25.000000 dtfabric-20230520/docs/index.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      105 2023-05-12 04:16:16.000000 dtfabric-20230520/docs/requirements.txt
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-20 03:30:20.347226 dtfabric-20230520/docs/sources/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    16090 2023-05-19 07:18:33.000000 dtfabric-20230520/docs/sources/Format-specification.md
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-20 03:30:20.348226 dtfabric-20230520/docs/sources/api/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1097 2022-02-19 13:55:33.000000 dtfabric-20230520/docs/sources/api/dtfabric.rst
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      869 2021-07-30 06:46:25.000000 dtfabric-20230520/docs/sources/api/dtfabric.runtime.rst
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       61 2021-07-30 06:37:51.000000 dtfabric-20230520/docs/sources/api/modules.rst
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-20 03:30:20.348226 dtfabric-20230520/docs/sources/user/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1633 2021-12-28 03:59:54.000000 dtfabric-20230520/docs/sources/user/Installation-instructions.md
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      288 2021-07-30 06:37:51.000000 dtfabric-20230520/docs/sources/user/index.rst
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-20 03:30:20.349226 dtfabric-20230520/dtfabric/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       74 2023-05-20 03:28:59.000000 dtfabric-20230520/dtfabric/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31766 2023-05-19 07:23:42.000000 dtfabric-20230520/dtfabric/data_types.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      710 2022-09-18 09:38:10.000000 dtfabric-20230520/dtfabric/decorators.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1502 2021-07-30 10:44:15.000000 dtfabric-20230520/dtfabric/definitions.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1016 2021-07-30 06:46:25.000000 dtfabric-20230520/dtfabric/errors.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    53251 2023-05-19 07:25:37.000000 dtfabric-20230520/dtfabric/reader.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3192 2022-09-18 09:35:13.000000 dtfabric-20230520/dtfabric/registry.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-20 03:30:20.350226 dtfabric-20230520/dtfabric/runtime/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2018-03-18 06:58:01.000000 dtfabric-20230520/dtfabric/runtime/__init__.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2523 2022-09-18 09:36:04.000000 dtfabric-20230520/dtfabric/runtime/byte_operations.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    76811 2023-05-19 07:28:29.000000 dtfabric-20230520/dtfabric/runtime/data_maps.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2022-01-27 14:27:48.000000 dtfabric-20230520/dtfabric/runtime/fabric.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6233 2022-09-18 09:46:53.000000 dtfabric-20230520/dtfabric/runtime/runtime.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-20 03:30:20.349226 dtfabric-20230520/dtfabric.egg-info/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      583 2023-05-20 03:30:18.000000 dtfabric-20230520/dtfabric.egg-info/PKG-INFO
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2835 2023-05-20 03:30:19.000000 dtfabric-20230520/dtfabric.egg-info/SOURCES.txt
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        1 2023-05-20 03:30:18.000000 dtfabric-20230520/dtfabric.egg-info/dependency_links.txt
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-05-20 03:30:18.000000 dtfabric-20230520/dtfabric.egg-info/requires.txt
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        9 2023-05-20 03:30:18.000000 dtfabric-20230520/dtfabric.egg-info/top_level.txt
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      395 2019-02-03 12:58:57.000000 dtfabric-20230520/dtfabric.ini
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       28 2023-05-12 04:16:07.000000 dtfabric-20230520/requirements.txt
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      777 2022-09-18 09:32:38.000000 dtfabric-20230520/run_tests.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-20 03:30:20.350226 dtfabric-20230520/scripts/
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)     3218 2022-09-18 08:56:58.000000 dtfabric-20230520/scripts/validate-definitions.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      302 2023-05-20 03:30:20.439226 dtfabric-20230520/setup.cfg
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)     6782 2023-05-12 04:16:07.000000 dtfabric-20230520/setup.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-20 03:30:20.365226 dtfabric-20230520/test_data/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1426 2017-05-01 13:58:49.000000 dtfabric-20230520/test_data/Notepad.lnk
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       99 2022-07-10 05:55:10.000000 dtfabric-20230520/test_data/boolean.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      101 2022-07-10 05:55:12.000000 dtfabric-20230520/test_data/character.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      284 2022-07-10 05:55:13.000000 dtfabric-20230520/test_data/constant.yaml
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-20 03:30:20.365226 dtfabric-20230520/test_data/definitions/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      524 2022-07-10 05:54:56.000000 dtfabric-20230520/test_data/definitions/booleans.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      453 2022-07-10 05:54:58.000000 dtfabric-20230520/test_data/definitions/characters.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      405 2022-07-10 05:55:00.000000 dtfabric-20230520/test_data/definitions/floating-points.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1364 2022-07-10 05:55:01.000000 dtfabric-20230520/test_data/definitions/integers.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      812 2022-07-10 05:55:15.000000 dtfabric-20230520/test_data/enumeration.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      218 2022-07-10 05:55:16.000000 dtfabric-20230520/test_data/floating-point.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      555 2022-07-10 05:55:18.000000 dtfabric-20230520/test_data/format.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      399 2022-07-10 05:55:19.000000 dtfabric-20230520/test_data/integer.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       83 2022-07-10 05:55:23.000000 dtfabric-20230520/test_data/padding.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      457 2022-07-10 05:55:28.000000 dtfabric-20230520/test_data/sequence.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      572 2022-07-10 05:55:25.000000 dtfabric-20230520/test_data/sequence_with_context.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      433 2023-05-18 05:56:24.000000 dtfabric-20230520/test_data/sequence_with_structure.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      657 2022-07-10 05:55:29.000000 dtfabric-20230520/test_data/stream.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      707 2022-07-10 05:55:32.000000 dtfabric-20230520/test_data/string.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      818 2022-07-10 05:55:30.000000 dtfabric-20230520/test_data/string_array.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1059 2022-07-10 05:55:50.000000 dtfabric-20230520/test_data/structure.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2022-07-10 05:55:34.000000 dtfabric-20230520/test_data/structure_family.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1576 2022-07-10 05:55:35.000000 dtfabric-20230520/test_data/structure_group.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      651 2022-07-10 05:55:36.000000 dtfabric-20230520/test_data/structure_with_condition.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      496 2022-07-10 05:55:38.000000 dtfabric-20230520/test_data/structure_with_context.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      712 2022-07-10 05:57:13.000000 dtfabric-20230520/test_data/structure_with_padding.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      322 2022-07-10 05:55:41.000000 dtfabric-20230520/test_data/structure_with_section.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      468 2022-07-10 05:55:43.000000 dtfabric-20230520/test_data/structure_with_sequence.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      466 2022-07-10 05:55:44.000000 dtfabric-20230520/test_data/structure_with_stream.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      446 2022-07-10 05:55:45.000000 dtfabric-20230520/test_data/structure_with_string.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      370 2022-07-10 05:55:47.000000 dtfabric-20230520/test_data/structure_with_union.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      700 2022-07-10 05:55:49.000000 dtfabric-20230520/test_data/structure_with_values.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      383 2022-07-10 05:55:53.000000 dtfabric-20230520/test_data/union.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      380 2022-07-10 05:55:51.000000 dtfabric-20230520/test_data/union_with_condition.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      200 2022-07-10 05:55:54.000000 dtfabric-20230520/test_data/uuid.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      107 2022-12-18 07:46:44.000000 dtfabric-20230520/test_dependencies.ini
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       14 2023-05-12 04:16:07.000000 dtfabric-20230520/test_requirements.txt
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-20 03:30:20.400226 dtfabric-20230520/tests/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2018-03-18 06:58:01.000000 dtfabric-20230520/tests/__init__.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    19713 2023-05-19 07:21:45.000000 dtfabric-20230520/tests/data_types.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    62234 2023-05-18 03:22:07.000000 dtfabric-20230520/tests/reader.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3002 2021-07-30 06:46:25.000000 dtfabric-20230520/tests/registry.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-20 03:30:20.432226 dtfabric-20230520/tests/runtime/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2018-03-18 06:58:01.000000 dtfabric-20230520/tests/runtime/__init__.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1645 2021-07-30 09:04:50.000000 dtfabric-20230520/tests/runtime/byte_operations.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    84696 2023-05-18 15:50:47.000000 dtfabric-20230520/tests/runtime/data_maps.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      662 2021-07-30 06:46:25.000000 dtfabric-20230520/tests/runtime/fabric.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2494 2021-07-30 06:46:25.000000 dtfabric-20230520/tests/runtime/runtime.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2272 2022-09-18 09:32:59.000000 dtfabric-20230520/tests/test_lib.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1252 2023-05-12 04:16:07.000000 dtfabric-20230520/tox.ini
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-20 03:30:20.439226 dtfabric-20230520/utils/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       70 2018-03-18 06:58:04.000000 dtfabric-20230520/utils/__init__.py
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      422 2023-05-12 04:16:07.000000 dtfabric-20230520/utils/check_dependencies.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11583 2023-05-12 04:16:07.000000 dtfabric-20230520/utils/dependencies.py
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      616 2021-12-28 04:01:20.000000 dtfabric-20230520/utils/update_release.sh
```

### Comparing `dtfabric-20230519/.github/workflows/test_docker.yml` & `dtfabric-20230520/.github/workflows/test_docker.yml`

 * *Files identical despite different names*

### Comparing `dtfabric-20230519/.github/workflows/test_docs.yml` & `dtfabric-20230520/.github/workflows/test_docs.yml`

 * *Files identical despite different names*

### Comparing `dtfabric-20230519/.github/workflows/test_tox.yml` & `dtfabric-20230520/.github/workflows/test_tox.yml`

 * *Files identical despite different names*

### Comparing `dtfabric-20230519/.pylintrc` & `dtfabric-20230520/.pylintrc`

 * *Files identical despite different names*

### Comparing `dtfabric-20230519/LICENSE` & `dtfabric-20230520/LICENSE`

 * *Files identical despite different names*

### Comparing `dtfabric-20230519/MANIFEST.in` & `dtfabric-20230520/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `dtfabric-20230519/PKG-INFO` & `dtfabric-20230520/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtfabric
-Version: 20230519
+Version: 20230520
 Summary: Data type fabric (dtfabric)
 Home-page: https://github.com/libyal/dtfabric
 Maintainer: Joachim Metz
 Maintainer-email: joachim.metz@gmail.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `dtfabric-20230519/appveyor.yml` & `dtfabric-20230520/appveyor.yml`

 * *Files identical despite different names*

### Comparing `dtfabric-20230519/config/appveyor/install.ps1` & `dtfabric-20230520/config/appveyor/install.ps1`

 * *Files identical despite different names*

### Comparing `dtfabric-20230519/config/appveyor/runtests.sh` & `dtfabric-20230520/config/appveyor/runtests.sh`

 * *Files identical despite different names*

### Comparing `dtfabric-20230519/config/dpkg/control` & `dtfabric-20230520/config/dpkg/control`

 * *Files identical despite different names*

### Comparing `dtfabric-20230519/config/dpkg/copyright` & `dtfabric-20230520/config/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `dtfabric-20230519/docs/conf.py` & `dtfabric-20230520/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230519/docs/index.rst` & `dtfabric-20230520/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dtfabric-20230519/docs/sources/Format-specification.md` & `dtfabric-20230520/docs/sources/Format-specification.md`

 * *Files 1% similar despite different names*

```diff
@@ -533,7 +533,14 @@
 members:
 - bsm_token_arg32
 - bsm_token_arg64
 ```
 
 The structure group members are required to define the identifier structure
 member with its values specific to the group member.
+
+Attribute name | Attribute type | Required | Description
+--- | --- | --- | ---
+base | string | Yes | Base data type. Note that this must be a structure data type.
+default | string | None | Default data type as fallback if no corresponding member data type is defined. Note that this must be a structure data type.
+identifier | string | Yes | Name of the member in the base (structure) data type that identified a (group) member.
+members | list | Yes | List of (group) member data types. Note that these must be a structure data types.
```

### Comparing `dtfabric-20230519/docs/sources/api/dtfabric.rst` & `dtfabric-20230520/docs/sources/api/dtfabric.rst`

 * *Files identical despite different names*

### Comparing `dtfabric-20230519/docs/sources/api/dtfabric.runtime.rst` & `dtfabric-20230520/docs/sources/api/dtfabric.runtime.rst`

 * *Files identical despite different names*

### Comparing `dtfabric-20230519/docs/sources/user/Installation-instructions.md` & `dtfabric-20230520/docs/sources/user/Installation-instructions.md`

 * *Files identical despite different names*

### Comparing `dtfabric-20230519/dtfabric/data_types.py` & `dtfabric-20230520/dtfabric/data_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -897,43 +897,50 @@
 
 
 class StructureGroupDefinition(LayoutDataTypeDefinition):
   """Structure group definition.
 
   Attributes:
     base (DataTypeDefinition): base data type definition.
+    byte_order (str): byte-order the data type.
+    default (DataTypeDefinition): default data type definition.
     identifier (str): name of the base structure member to identify the group
         members.
     members (list[DataTypeDefinition]): member data type definitions.
   """
 
   TYPE_INDICATOR: 'Union[str, None]' = (
       definitions.TYPE_INDICATOR_STRUCTURE_GROUP)
 
   def __init__(
       self, name: 'str', base_definition: 'StructureDefinition',
-      identifier: 'str', aliases: 'Optional[List[str]]' = None,
+      identifier: 'str', default_definition: 'StructureDefinition',
+      aliases: 'Optional[List[str]]' = None,
       description: 'Optional[str]' = None,
       urls: 'Optional[List[str]]' = None) -> 'None':
     """Initializes a structure group data type definition.
 
     Args:
       name (str): name.
       base_definition (StructureDefinition): base data type definition.
       identifier (str): name of the base structure member to identify the group
           members.
+      default_definition (StructureDefinition): default data type definition.
       aliases (Optional[list[str]]): aliases.
       description (Optional[str]): description.
       urls (Optional[list[str]]): URLs.
     """
     super(StructureGroupDefinition, self).__init__(
         name, aliases=aliases, description=description, urls=urls)
     self._members_by_name: 'OrderedDict[str, DataTypeDefinition]' = (
         collections.OrderedDict())
     self.base: 'Union[DataTypeDefinition, None]' = base_definition
+    self.byte_order: 'str' = getattr(
+        base_definition, 'byte_order', definitions.BYTE_ORDER_NATIVE)
+    self.default: 'Union[DataTypeDefinition, None]' = default_definition
     self.identifier: 'Union[str, None]' = identifier
 
   @property
   def members(self) -> 'List[DataTypeDefinition]':
     """members (list[DataTypeDefinition]): member data type definitions."""
     return list(self._members_by_name.values())
```

### Comparing `dtfabric-20230519/dtfabric/decorators.py` & `dtfabric-20230520/dtfabric/decorators.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230519/dtfabric/definitions.py` & `dtfabric-20230520/dtfabric/definitions.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230519/dtfabric/errors.py` & `dtfabric-20230520/dtfabric/errors.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230519/dtfabric/reader.py` & `dtfabric-20230520/dtfabric/reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
   _SUPPORTED_DEFINITION_VALUES_STRING_MEMBER = set([
       'encoding']).union(_SUPPORTED_DEFINITION_VALUES_ELEMENTS_MEMBER_DATA_TYPE)
 
   _SUPPORTED_DEFINITION_VALUES_STRUCTURE_FAMILY = set([
       'base', 'members']).union(_SUPPORTED_DEFINITION_VALUES_DATA_TYPE)
 
   _SUPPORTED_DEFINITION_VALUES_STRUCTURE_GROUP = set([
-      'base', 'identifier', 'members']).union(
+      'base', 'default', 'identifier', 'members']).union(
           _SUPPORTED_DEFINITION_VALUES_DATA_TYPE)
 
   _SUPPORTED_ATTRIBUTES_STORAGE_DATA_TYPE = set([
       'byte_order'])
 
   _SUPPORTED_ATTRIBUTES_FIXED_SIZE_DATA_TYPE = set([
       'size', 'units']).union(_SUPPORTED_ATTRIBUTES_STORAGE_DATA_TYPE)
@@ -1141,21 +1141,32 @@
       raise errors.DefinitionReaderError(definition_name, (
           f'undefined base: {base:s}'))
 
     identifier = definition_values.get('identifier', None)
     if not identifier:
       raise errors.DefinitionReaderError(definition_name, 'missing identifier')
 
+    default = definition_values.get('default', None)
+    if not default:
+      default_data_type_definition = None
+    else:
+      default_data_type_definition = definitions_registry.GetDefinitionByName(
+          default)
+      if not default_data_type_definition:
+        raise errors.DefinitionReaderError(definition_name, (
+            f'undefined default: {default:s}'))
+
     aliases = definition_values.get('aliases', None)
     description = definition_values.get('description', None)
     urls = definition_values.get('urls', None)
 
     definition_object = data_types.StructureGroupDefinition(
         definition_name, base_data_type_definition, identifier,
-        aliases=aliases, description=description, urls=urls)
+        default_data_type_definition, aliases=aliases, description=description,
+        urls=urls)
 
     members = definition_values.get('members', None)
     if not members:
       raise errors.DefinitionReaderError(definition_name, 'missing members')
 
     for member in members:
       member_data_type_definition = definitions_registry.GetDefinitionByName(
```

### Comparing `dtfabric-20230519/dtfabric/registry.py` & `dtfabric-20230520/dtfabric/registry.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230519/dtfabric/runtime/byte_operations.py` & `dtfabric-20230520/dtfabric/runtime/byte_operations.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230519/dtfabric/runtime/data_maps.py` & `dtfabric-20230520/dtfabric/runtime/data_maps.py`

 * *Files 0% similar despite different names*

```diff
@@ -2205,18 +2205,24 @@
     Args:
       data_type_definition (DataTypeDefinition): data type definition.
 
     Raises:
       FormatError: if the data type map cannot be determined from the data
           type definition.
     """
+    default_data_type_map = None
+    if data_type_definition.default:
+      default_data_type_map = DataTypeMapFactory.CreateDataTypeMapByType(
+          data_type_definition.default)
+
     super(StructureGroupMap, self).__init__(data_type_definition)
     self._base_data_type_map = DataTypeMapFactory.CreateDataTypeMapByType(
         data_type_definition.base)
     self._data_type_maps = None
+    self._default_data_type_map = default_data_type_map
 
     self._GetMemberDataTypeMaps(data_type_definition)
 
   def _GetMemberDataTypeMaps(self, data_type_definition):
     """Retrieves the member data type maps.
 
     Args:
@@ -2340,15 +2346,16 @@
       if member_identifier is None:
         raise errors.MappingError(
             f'Unable to determine value of '
             f'{self._data_type_definition.identifier:s}')
 
       context_state['member_identifier'] = member_identifier
 
-    member_data_type_map = self._data_type_maps.get(member_identifier, None)
+    member_data_type_map = self._data_type_maps.get(
+        member_identifier, self._default_data_type_map)
     if member_data_type_map is None:
       raise errors.MappingError(
           f'Missing member data type map for '
           f'{self._data_type_definition.identifier:s}: '
           f'{member_identifier!s}')
 
     subcontext = context_state.get('context', None)
```

### Comparing `dtfabric-20230519/dtfabric/runtime/fabric.py` & `dtfabric-20230520/dtfabric/runtime/fabric.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230519/dtfabric/runtime/runtime.py` & `dtfabric-20230520/dtfabric/runtime/runtime.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230519/dtfabric.egg-info/PKG-INFO` & `dtfabric-20230520/dtfabric.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtfabric
-Version: 20230519
+Version: 20230520
 Summary: Data type fabric (dtfabric)
 Home-page: https://github.com/libyal/dtfabric
 Maintainer: Joachim Metz
 Maintainer-email: joachim.metz@gmail.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `dtfabric-20230519/dtfabric.egg-info/SOURCES.txt` & `dtfabric-20230520/dtfabric.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dtfabric-20230519/run_tests.py` & `dtfabric-20230520/run_tests.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230519/scripts/validate-definitions.py` & `dtfabric-20230520/scripts/validate-definitions.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230519/setup.py` & `dtfabric-20230520/setup.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230519/test_data/Notepad.lnk` & `dtfabric-20230520/test_data/Notepad.lnk`

 * *Files identical despite different names*

### Comparing `dtfabric-20230519/test_data/definitions/booleans.yaml` & `dtfabric-20230520/test_data/definitions/booleans.yaml`

 * *Files identical despite different names*

### Comparing `dtfabric-20230519/test_data/definitions/integers.yaml` & `dtfabric-20230520/test_data/definitions/integers.yaml`

 * *Files identical despite different names*

### Comparing `dtfabric-20230519/test_data/enumeration.yaml` & `dtfabric-20230520/test_data/enumeration.yaml`

 * *Files identical despite different names*

### Comparing `dtfabric-20230519/test_data/format.yaml` & `dtfabric-20230520/test_data/format.yaml`

 * *Files identical despite different names*

### Comparing `dtfabric-20230519/test_data/sequence_with_context.yaml` & `dtfabric-20230520/test_data/sequence_with_context.yaml`

 * *Files identical despite different names*

### Comparing `dtfabric-20230519/test_data/stream.yaml` & `dtfabric-20230520/test_data/stream.yaml`

 * *Files identical despite different names*

### Comparing `dtfabric-20230519/test_data/string.yaml` & `dtfabric-20230520/test_data/string.yaml`

 * *Files identical despite different names*

### Comparing `dtfabric-20230519/test_data/string_array.yaml` & `dtfabric-20230520/test_data/string_array.yaml`

 * *Files identical despite different names*

### Comparing `dtfabric-20230519/test_data/structure.yaml` & `dtfabric-20230520/test_data/structure.yaml`

 * *Files identical despite different names*

### Comparing `dtfabric-20230519/test_data/structure_family.yaml` & `dtfabric-20230520/test_data/structure_family.yaml`

 * *Files identical despite different names*

### Comparing `dtfabric-20230519/test_data/structure_group.yaml` & `dtfabric-20230520/test_data/structure_group.yaml`

 * *Files identical despite different names*

### Comparing `dtfabric-20230519/test_data/structure_with_condition.yaml` & `dtfabric-20230520/test_data/structure_with_condition.yaml`

 * *Files identical despite different names*

### Comparing `dtfabric-20230519/test_data/structure_with_padding.yaml` & `dtfabric-20230520/test_data/structure_with_padding.yaml`

 * *Files identical despite different names*

### Comparing `dtfabric-20230519/test_data/structure_with_values.yaml` & `dtfabric-20230520/test_data/structure_with_values.yaml`

 * *Files identical despite different names*

### Comparing `dtfabric-20230519/tests/data_types.py` & `dtfabric-20230520/tests/data_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -531,24 +531,26 @@
 
   def testInitialize(self):
     """Tests the __init__ function."""
     base_definition = data_types.StructureDefinition(
         'base', description='my base structure type')
 
     data_type_definition = data_types.StructureGroupDefinition(
-        'group', base_definition, 'identifier', description='structure group')
+        'group', base_definition, 'identifier', None,
+        description='structure group')
     self.assertIsNotNone(data_type_definition)
 
   def testAddMemberDefinition(self):
     """Tests the AddMemberDefinition function."""
     base_definition = data_types.StructureDefinition(
         'base', description='my base structure type')
 
     data_type_definition = data_types.StructureGroupDefinition(
-        'group', base_definition, 'identifier', description='structure group')
+        'group', base_definition, 'identifier', None,
+        description='structure group')
     self.assertIsNotNone(data_type_definition)
 
     group_member_definition = data_types.StructureDefinition(
         'member', description='my member structure type')
 
     data_type_definition.AddMemberDefinition(group_member_definition)
```

### Comparing `dtfabric-20230519/tests/reader.py` & `dtfabric-20230520/tests/reader.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230519/tests/registry.py` & `dtfabric-20230520/tests/registry.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230519/tests/runtime/byte_operations.py` & `dtfabric-20230520/tests/runtime/byte_operations.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230519/tests/runtime/data_maps.py` & `dtfabric-20230520/tests/runtime/data_maps.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230519/tests/runtime/fabric.py` & `dtfabric-20230520/tests/runtime/fabric.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230519/tests/runtime/runtime.py` & `dtfabric-20230520/tests/runtime/runtime.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230519/tests/test_lib.py` & `dtfabric-20230520/tests/test_lib.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230519/tox.ini` & `dtfabric-20230520/tox.ini`

 * *Files identical despite different names*

### Comparing `dtfabric-20230519/utils/dependencies.py` & `dtfabric-20230520/utils/dependencies.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20230519/utils/update_release.sh` & `dtfabric-20230520/utils/update_release.sh`

 * *Files identical despite different names*

