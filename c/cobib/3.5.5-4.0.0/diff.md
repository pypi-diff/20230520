# Comparing `tmp/cobib-3.5.5.tar.gz` & `tmp/cobib-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cobib-3.5.5.tar", last modified: Tue Apr 11 19:23:01 2023, max compression
+gzip compressed data, was "cobib-4.0.0.tar", last modified: Sat May 20 14:28:46 2023, max compression
```

## Comparing `cobib-3.5.5.tar` & `cobib-4.0.0.tar`

### file list

```diff
@@ -1,175 +1,178 @@
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-11 19:23:01.059836 cobib-3.5.5/
--rw-r--r--   0 max       (1000) max       (1000)      217 2021-09-20 21:31:31.000000 cobib-3.5.5/.coveragerc
--rw-r--r--   0 max       (1000) max       (1000)      240 2021-09-20 21:31:31.000000 cobib-3.5.5/.gitignore
--rw-r--r--   0 max       (1000) max       (1000)     2717 2022-12-13 20:07:48.000000 cobib-3.5.5/.gitlab-ci.yml
--rw-r--r--   0 max       (1000) max       (1000)       48 2021-09-20 21:31:31.000000 cobib-3.5.5/.pydocstylerc
--rw-r--r--   0 max       (1000) max       (1000)     1281 2022-11-16 20:11:10.000000 cobib-3.5.5/.pylintdict
--rw-r--r--   0 max       (1000) max       (1000)    11213 2023-02-05 08:34:43.000000 cobib-3.5.5/.pylintrc
--rw-r--r--   0 max       (1000) max       (1000)    25714 2023-04-11 19:21:05.000000 cobib-3.5.5/CHANGELOG.md
--rw-r--r--   0 max       (1000) max       (1000)     2259 2021-12-01 22:02:28.000000 cobib-3.5.5/CONTRIBUTING.md
--rw-r--r--   0 max       (1000) max       (1000)     1063 2022-01-13 20:47:42.000000 cobib-3.5.5/LICENSE.txt
--rw-r--r--   0 max       (1000) max       (1000)      115 2021-09-20 21:31:31.000000 cobib-3.5.5/MANIFEST.in
--rw-r--r--   0 max       (1000) max       (1000)      187 2021-09-20 21:31:31.000000 cobib-3.5.5/Makefile
--rw-r--r--   0 max       (1000) max       (1000)    34981 2023-04-11 19:23:01.059836 cobib-3.5.5/PKG-INFO
--rw-r--r--   0 max       (1000) max       (1000)     8437 2022-01-13 21:08:20.000000 cobib-3.5.5/README.md
--rw-r--r--   0 max       (1000) max       (1000)      563 2021-09-20 21:31:31.000000 cobib-3.5.5/_cobib
--rw-r--r--   0 max       (1000) max       (1000)    26588 2023-04-11 19:20:32.000000 cobib-3.5.5/cobib.1
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-11 19:23:01.023169 cobib-3.5.5/html/
--rw-r--r--   0 max       (1000) max       (1000)    34915 2021-09-20 21:31:31.000000 cobib-3.5.5/html/cobib_book.svg
--rw-r--r--   0 max       (1000) max       (1000)    61955 2021-09-20 21:31:31.000000 cobib-3.5.5/html/cobib_logo.svg
--rw-r--r--   0 max       (1000) max       (1000)      558 2022-04-25 20:22:51.000000 cobib-3.5.5/html/index.html.jinja2
--rw-r--r--   0 max       (1000) max       (1000)      398 2022-04-25 20:43:18.000000 cobib-3.5.5/html/module.html.jinja2
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-11 19:23:01.026502 cobib-3.5.5/logo/
--rw-r--r--   0 max       (1000) max       (1000)    44669 2021-09-20 21:31:31.000000 cobib-3.5.5/logo/cobib_book-squared.png
--rw-r--r--   0 max       (1000) max       (1000)    40896 2021-09-20 21:31:31.000000 cobib-3.5.5/logo/cobib_book.png
--rw-r--r--   0 max       (1000) max       (1000)    34915 2021-09-20 21:31:31.000000 cobib-3.5.5/logo/cobib_book.svg
--rw-r--r--   0 max       (1000) max       (1000)    74851 2021-09-20 21:31:31.000000 cobib-3.5.5/logo/cobib_byline.png
--rw-r--r--   0 max       (1000) max       (1000)    27555 2021-09-20 21:31:31.000000 cobib-3.5.5/logo/cobib_byline.svg
--rw-r--r--   0 max       (1000) max       (1000)   126027 2021-09-20 21:31:31.000000 cobib-3.5.5/logo/cobib_logo.png
--rw-r--r--   0 max       (1000) max       (1000)    61955 2021-09-20 21:31:31.000000 cobib-3.5.5/logo/cobib_logo.svg
--rw-r--r--   0 max       (1000) max       (1000)      552 2021-12-01 20:44:34.000000 cobib-3.5.5/mypy.ini
--rw-r--r--   0 max       (1000) max       (1000)      328 2021-09-20 21:31:31.000000 cobib-3.5.5/pyproject.toml
--rw-r--r--   0 max       (1000) max       (1000)       27 2021-09-20 21:31:31.000000 cobib-3.5.5/pytest.ini
--rw-r--r--   0 max       (1000) max       (1000)       78 2021-12-01 20:44:34.000000 cobib-3.5.5/requirements.txt
--rw-r--r--   0 max       (1000) max       (1000)     1084 2023-04-11 19:23:01.063169 cobib-3.5.5/setup.cfg
--rw-r--r--   0 max       (1000) max       (1000)      296 2021-09-20 21:31:31.000000 cobib-3.5.5/setup.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-11 19:23:01.016502 cobib-3.5.5/src/
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-11 19:23:01.026502 cobib-3.5.5/src/cobib/
--rw-r--r--   0 max       (1000) max       (1000)      474 2023-04-11 19:20:12.000000 cobib-3.5.5/src/cobib/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     5477 2022-05-22 07:42:34.000000 cobib-3.5.5/src/cobib/__main__.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-11 19:23:01.033169 cobib-3.5.5/src/cobib/commands/
--rw-r--r--   0 max       (1000) max       (1000)      899 2021-12-01 20:44:34.000000 cobib-3.5.5/src/cobib/commands/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)    13875 2022-11-16 20:02:48.000000 cobib-3.5.5/src/cobib/commands/add.py
--rw-r--r--   0 max       (1000) max       (1000)     5643 2021-10-04 20:58:33.000000 cobib-3.5.5/src/cobib/commands/base_command.py
--rw-r--r--   0 max       (1000) max       (1000)     3511 2021-10-04 20:58:33.000000 cobib-3.5.5/src/cobib/commands/delete.py
--rw-r--r--   0 max       (1000) max       (1000)     7111 2021-10-04 20:58:33.000000 cobib-3.5.5/src/cobib/commands/edit.py
--rw-r--r--   0 max       (1000) max       (1000)     8061 2021-10-04 20:58:33.000000 cobib-3.5.5/src/cobib/commands/export.py
--rw-r--r--   0 max       (1000) max       (1000)     5981 2021-12-01 20:44:34.000000 cobib-3.5.5/src/cobib/commands/import_.py
--rw-r--r--   0 max       (1000) max       (1000)     4745 2021-10-04 20:58:33.000000 cobib-3.5.5/src/cobib/commands/init.py
--rw-r--r--   0 max       (1000) max       (1000)    14235 2021-10-04 21:00:16.000000 cobib-3.5.5/src/cobib/commands/list.py
--rw-r--r--   0 max       (1000) max       (1000)    17172 2021-10-12 20:39:32.000000 cobib-3.5.5/src/cobib/commands/modify.py
--rw-r--r--   0 max       (1000) max       (1000)     8418 2023-04-11 19:15:41.000000 cobib-3.5.5/src/cobib/commands/open.py
--rw-r--r--   0 max       (1000) max       (1000)     5322 2021-10-04 20:58:33.000000 cobib-3.5.5/src/cobib/commands/redo.py
--rw-r--r--   0 max       (1000) max       (1000)     8601 2021-10-04 20:58:33.000000 cobib-3.5.5/src/cobib/commands/search.py
--rw-r--r--   0 max       (1000) max       (1000)     3447 2021-10-04 20:58:33.000000 cobib-3.5.5/src/cobib/commands/show.py
--rw-r--r--   0 max       (1000) max       (1000)     6053 2021-10-04 20:58:33.000000 cobib-3.5.5/src/cobib/commands/undo.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-11 19:23:01.033169 cobib-3.5.5/src/cobib/config/
--rw-r--r--   0 max       (1000) max       (1000)     1210 2022-01-13 20:47:42.000000 cobib-3.5.5/src/cobib/config/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)    20453 2023-04-06 21:46:11.000000 cobib-3.5.5/src/cobib/config/config.py
--rw-r--r--   0 max       (1000) max       (1000)    27156 2022-04-25 18:46:40.000000 cobib-3.5.5/src/cobib/config/event.py
--rw-r--r--   0 max       (1000) max       (1000)    11521 2023-01-30 19:18:43.000000 cobib-3.5.5/src/cobib/config/example.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-11 19:23:01.033169 cobib-3.5.5/src/cobib/database/
--rw-r--r--   0 max       (1000) max       (1000)      283 2021-09-20 21:31:31.000000 cobib-3.5.5/src/cobib/database/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     9792 2022-06-03 21:13:52.000000 cobib-3.5.5/src/cobib/database/database.py
--rw-r--r--   0 max       (1000) max       (1000)    17270 2022-12-26 15:50:45.000000 cobib-3.5.5/src/cobib/database/entry.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-11 19:23:01.036502 cobib-3.5.5/src/cobib/importers/
--rw-r--r--   0 max       (1000) max       (1000)      275 2021-12-01 20:44:34.000000 cobib-3.5.5/src/cobib/importers/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)      930 2021-12-01 20:44:34.000000 cobib-3.5.5/src/cobib/importers/base_importer.py
--rw-r--r--   0 max       (1000) max       (1000)    13035 2022-08-27 17:46:24.000000 cobib-3.5.5/src/cobib/importers/zotero.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-11 19:23:01.036502 cobib-3.5.5/src/cobib/parsers/
--rw-r--r--   0 max       (1000) max       (1000)      520 2021-09-25 22:36:09.000000 cobib-3.5.5/src/cobib/parsers/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     5058 2022-01-13 20:47:42.000000 cobib-3.5.5/src/cobib/parsers/arxiv.py
--rw-r--r--   0 max       (1000) max       (1000)     2053 2021-09-20 21:31:31.000000 cobib-3.5.5/src/cobib/parsers/base_parser.py
--rw-r--r--   0 max       (1000) max       (1000)     3078 2022-11-16 20:17:18.000000 cobib-3.5.5/src/cobib/parsers/bibtex.py
--rw-r--r--   0 max       (1000) max       (1000)     3272 2022-12-20 16:58:30.000000 cobib-3.5.5/src/cobib/parsers/doi.py
--rw-r--r--   0 max       (1000) max       (1000)     4590 2022-06-28 20:53:45.000000 cobib-3.5.5/src/cobib/parsers/isbn.py
--rw-r--r--   0 max       (1000) max       (1000)     3553 2023-02-05 08:34:32.000000 cobib-3.5.5/src/cobib/parsers/url.py
--rw-r--r--   0 max       (1000) max       (1000)     2805 2022-04-25 18:48:18.000000 cobib-3.5.5/src/cobib/parsers/yaml.py
--rw-r--r--   0 max       (1000) max       (1000)        0 2021-09-20 21:31:31.000000 cobib-3.5.5/src/cobib/py.typed
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-11 19:23:01.036502 cobib-3.5.5/src/cobib/tui/
--rw-r--r--   0 max       (1000) max       (1000)     1119 2021-11-17 16:26:13.000000 cobib-3.5.5/src/cobib/tui/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)    14586 2022-12-26 15:50:59.000000 cobib-3.5.5/src/cobib/tui/buffer.py
--rw-r--r--   0 max       (1000) max       (1000)    11317 2022-01-13 20:47:42.000000 cobib-3.5.5/src/cobib/tui/frame.py
--rw-r--r--   0 max       (1000) max       (1000)     3581 2021-09-20 21:31:31.000000 cobib-3.5.5/src/cobib/tui/state.py
--rw-r--r--   0 max       (1000) max       (1000)    29627 2022-01-13 20:47:42.000000 cobib-3.5.5/src/cobib/tui/tui.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-11 19:23:01.039836 cobib-3.5.5/src/cobib/utils/
--rw-r--r--   0 max       (1000) max       (1000)      242 2021-09-20 21:31:31.000000 cobib-3.5.5/src/cobib/utils/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     7761 2021-12-01 20:44:34.000000 cobib-3.5.5/src/cobib/utils/file_downloader.py
--rw-r--r--   0 max       (1000) max       (1000)     4533 2021-09-20 21:32:23.000000 cobib-3.5.5/src/cobib/utils/journal_abbreviations.py
--rw-r--r--   0 max       (1000) max       (1000)     5135 2022-04-25 19:41:11.000000 cobib-3.5.5/src/cobib/utils/logging.py
--rw-r--r--   0 max       (1000) max       (1000)     1837 2021-09-20 21:31:31.000000 cobib-3.5.5/src/cobib/utils/rel_path.py
--rw-r--r--   0 max       (1000) max       (1000)     7802 2021-09-26 19:17:19.000000 cobib-3.5.5/src/cobib/utils/shell_helper.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-11 19:23:01.029836 cobib-3.5.5/src/cobib.egg-info/
--rw-r--r--   0 max       (1000) max       (1000)    34981 2023-04-11 19:23:00.000000 cobib-3.5.5/src/cobib.egg-info/PKG-INFO
--rw-r--r--   0 max       (1000) max       (1000)     4000 2023-04-11 19:23:01.000000 cobib-3.5.5/src/cobib.egg-info/SOURCES.txt
--rw-r--r--   0 max       (1000) max       (1000)        1 2023-04-11 19:23:00.000000 cobib-3.5.5/src/cobib.egg-info/dependency_links.txt
--rw-r--r--   0 max       (1000) max       (1000)       46 2023-04-11 19:23:00.000000 cobib-3.5.5/src/cobib.egg-info/entry_points.txt
--rw-r--r--   0 max       (1000) max       (1000)       78 2023-04-11 19:23:00.000000 cobib-3.5.5/src/cobib.egg-info/requires.txt
--rw-r--r--   0 max       (1000) max       (1000)        6 2023-04-11 19:23:00.000000 cobib-3.5.5/src/cobib.egg-info/top_level.txt
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-11 19:23:01.039836 cobib-3.5.5/tests/
--rw-r--r--   0 max       (1000) max       (1000)     1508 2021-09-20 21:31:31.000000 cobib-3.5.5/tests/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)      809 2021-09-20 21:31:31.000000 cobib-3.5.5/tests/cmdline_test.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-11 19:23:01.049836 cobib-3.5.5/tests/commands/
--rw-r--r--   0 max       (1000) max       (1000)       68 2021-09-20 21:31:31.000000 cobib-3.5.5/tests/commands/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     5950 2023-02-05 08:34:32.000000 cobib-3.5.5/tests/commands/command_test.py
--rw-r--r--   0 max       (1000) max       (1000)      248 2021-09-20 21:31:31.000000 cobib-3.5.5/tests/commands/example_duplicate_entry.bib
--rw-r--r--   0 max       (1000) max       (1000)      261 2021-09-20 21:31:31.000000 cobib-3.5.5/tests/commands/example_duplicate_entry.yaml
--rw-r--r--   0 max       (1000) max       (1000)      134 2021-09-20 21:31:31.000000 cobib-3.5.5/tests/commands/example_multi_file_entry.bib
--rw-r--r--   0 max       (1000) max       (1000)      155 2021-09-20 21:31:31.000000 cobib-3.5.5/tests/commands/example_multi_file_entry.yaml
--rw-r--r--   0 max       (1000) max       (1000)    21339 2022-11-16 20:31:43.000000 cobib-3.5.5/tests/commands/test_add.py
--rw-r--r--   0 max       (1000) max       (1000)     8332 2022-06-03 21:13:52.000000 cobib-3.5.5/tests/commands/test_delete.py
--rw-r--r--   0 max       (1000) max       (1000)     7982 2022-06-03 21:13:52.000000 cobib-3.5.5/tests/commands/test_edit.py
--rw-r--r--   0 max       (1000) max       (1000)    10071 2022-07-12 20:53:48.000000 cobib-3.5.5/tests/commands/test_export.py
--rw-r--r--   0 max       (1000) max       (1000)     2815 2022-06-03 21:13:52.000000 cobib-3.5.5/tests/commands/test_git_commit_event.py
--rw-r--r--   0 max       (1000) max       (1000)     2806 2023-02-05 08:34:32.000000 cobib-3.5.5/tests/commands/test_import.py
--rw-r--r--   0 max       (1000) max       (1000)     6024 2022-06-03 21:13:52.000000 cobib-3.5.5/tests/commands/test_init.py
--rw-r--r--   0 max       (1000) max       (1000)    14719 2022-06-03 21:13:52.000000 cobib-3.5.5/tests/commands/test_list.py
--rw-r--r--   0 max       (1000) max       (1000)    10799 2022-06-03 21:13:52.000000 cobib-3.5.5/tests/commands/test_modify.py
--rw-r--r--   0 max       (1000) max       (1000)    16138 2023-04-11 19:15:46.000000 cobib-3.5.5/tests/commands/test_open.py
--rw-r--r--   0 max       (1000) max       (1000)     9514 2023-02-05 08:34:32.000000 cobib-3.5.5/tests/commands/test_redo.py
--rw-r--r--   0 max       (1000) max       (1000)     9949 2022-06-03 21:13:52.000000 cobib-3.5.5/tests/commands/test_search.py
--rw-r--r--   0 max       (1000) max       (1000)     5663 2022-06-03 21:13:52.000000 cobib-3.5.5/tests/commands/test_show.py
--rw-r--r--   0 max       (1000) max       (1000)     9066 2023-02-05 08:34:32.000000 cobib-3.5.5/tests/commands/test_undo.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-11 19:23:01.049836 cobib-3.5.5/tests/config/
--rw-r--r--   0 max       (1000) max       (1000)       28 2021-09-20 21:31:31.000000 cobib-3.5.5/tests/config/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)      119 2021-09-20 21:31:31.000000 cobib-3.5.5/tests/config/broken_config.py
--rw-r--r--   0 max       (1000) max       (1000)    11310 2022-01-13 20:47:42.000000 cobib-3.5.5/tests/config/test_config.py
--rw-r--r--   0 max       (1000) max       (1000)     2420 2021-12-01 20:44:34.000000 cobib-3.5.5/tests/config/test_event.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-11 19:23:01.053169 cobib-3.5.5/tests/database/
--rw-r--r--   0 max       (1000) max       (1000)       30 2021-09-20 21:31:31.000000 cobib-3.5.5/tests/database/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)       59 2021-09-20 21:31:31.000000 cobib-3.5.5/tests/database/example_entry_umlaut.bib
--rw-r--r--   0 max       (1000) max       (1000)     8168 2023-02-05 08:34:32.000000 cobib-3.5.5/tests/database/test_database.py
--rw-r--r--   0 max       (1000) max       (1000)    13859 2022-12-26 15:50:50.000000 cobib-3.5.5/tests/database/test_entry.py
--rw-r--r--   0 max       (1000) max       (1000)      444 2022-12-20 16:58:30.000000 cobib-3.5.5/tests/debug.py
--rw-r--r--   0 max       (1000) max       (1000)      651 2021-09-20 21:31:31.000000 cobib-3.5.5/tests/example_entry.bib
--rw-r--r--   0 max       (1000) max       (1000)      621 2021-09-20 21:31:31.000000 cobib-3.5.5/tests/example_entry.yaml
--rw-r--r--   0 max       (1000) max       (1000)      723 2022-07-12 20:53:54.000000 cobib-3.5.5/tests/example_literature.bib
--rw-r--r--   0 max       (1000) max       (1000)      636 2023-04-06 21:46:08.000000 cobib-3.5.5/tests/example_literature.yaml
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-11 19:23:01.053169 cobib-3.5.5/tests/importers/
--rw-r--r--   0 max       (1000) max       (1000)       71 2021-12-01 20:44:34.000000 cobib-3.5.5/tests/importers/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)      274 2022-06-03 21:13:52.000000 cobib-3.5.5/tests/importers/importer_test.py
--rw-r--r--   0 max       (1000) max       (1000)     4541 2023-02-05 08:34:32.000000 cobib-3.5.5/tests/importers/test_zotero.py
--rw-r--r--   0 max       (1000) max       (1000)     2609 2021-12-01 20:44:34.000000 cobib-3.5.5/tests/importers/zotero_database.yaml
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-11 19:23:01.056502 cobib-3.5.5/tests/parsers/
--rw-r--r--   0 max       (1000) max       (1000)       65 2021-09-20 21:31:31.000000 cobib-3.5.5/tests/parsers/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     1395 2022-06-03 21:13:52.000000 cobib-3.5.5/tests/parsers/parser_test.py
--rw-r--r--   0 max       (1000) max       (1000)     5767 2022-06-03 21:13:52.000000 cobib-3.5.5/tests/parsers/test_arxiv.py
--rw-r--r--   0 max       (1000) max       (1000)     3224 2022-06-03 21:13:52.000000 cobib-3.5.5/tests/parsers/test_bibtex.py
--rw-r--r--   0 max       (1000) max       (1000)     5017 2022-06-03 21:13:52.000000 cobib-3.5.5/tests/parsers/test_doi.py
--rw-r--r--   0 max       (1000) max       (1000)     5566 2022-06-28 20:53:45.000000 cobib-3.5.5/tests/parsers/test_isbn.py
--rw-r--r--   0 max       (1000) max       (1000)     4399 2022-11-16 20:47:00.000000 cobib-3.5.5/tests/parsers/test_url.py
--rw-r--r--   0 max       (1000) max       (1000)     3251 2022-06-03 21:13:52.000000 cobib-3.5.5/tests/parsers/test_yaml.py
--rw-r--r--   0 max       (1000) max       (1000)     4573 2021-09-20 21:31:31.000000 cobib-3.5.5/tests/test_main.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-11 19:23:01.056502 cobib-3.5.5/tests/tui/
--rw-r--r--   0 max       (1000) max       (1000)      125 2021-09-20 21:31:31.000000 cobib-3.5.5/tests/tui/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     4444 2021-11-17 16:25:08.000000 cobib-3.5.5/tests/tui/mock_curses.py
--rw-r--r--   0 max       (1000) max       (1000)     1176 2021-09-20 21:31:31.000000 cobib-3.5.5/tests/tui/mock_tui.py
--rw-r--r--   0 max       (1000) max       (1000)     1134 2021-09-20 21:31:31.000000 cobib-3.5.5/tests/tui/scrolling_database.yaml
--rw-r--r--   0 max       (1000) max       (1000)    19852 2022-12-26 15:50:59.000000 cobib-3.5.5/tests/tui/test_buffer.py
--rw-r--r--   0 max       (1000) max       (1000)    22582 2022-12-26 15:46:45.000000 cobib-3.5.5/tests/tui/test_frame.py
--rw-r--r--   0 max       (1000) max       (1000)     2420 2021-09-20 21:31:31.000000 cobib-3.5.5/tests/tui/test_state.py
--rw-r--r--   0 max       (1000) max       (1000)    41277 2022-09-29 20:29:54.000000 cobib-3.5.5/tests/tui/test_tui.py
--rw-r--r--   0 max       (1000) max       (1000)     8505 2021-12-01 20:44:34.000000 cobib-3.5.5/tests/tui/tui_test.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-11 19:23:01.059836 cobib-3.5.5/tests/utils/
--rw-r--r--   0 max       (1000) max       (1000)       29 2021-09-20 21:31:31.000000 cobib-3.5.5/tests/utils/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)      712 2021-09-20 21:31:31.000000 cobib-3.5.5/tests/utils/expected_changelog_printing.txt
--rw-r--r--   0 max       (1000) max       (1000)      172 2021-09-20 21:31:31.000000 cobib-3.5.5/tests/utils/fixed_database.yaml
--rw-r--r--   0 max       (1000) max       (1000)      163 2021-09-25 23:38:02.000000 cobib-3.5.5/tests/utils/linting_database.yaml
--rw-r--r--   0 max       (1000) max       (1000)     9133 2022-08-27 18:09:45.000000 cobib-3.5.5/tests/utils/test_file_downloader.py
--rw-r--r--   0 max       (1000) max       (1000)     3216 2021-09-20 21:31:31.000000 cobib-3.5.5/tests/utils/test_journal_abbreviations.py
--rw-r--r--   0 max       (1000) max       (1000)     3135 2022-04-25 19:44:59.000000 cobib-3.5.5/tests/utils/test_logging.py
--rw-r--r--   0 max       (1000) max       (1000)      964 2021-09-20 21:31:31.000000 cobib-3.5.5/tests/utils/test_rel_path.py
--rw-r--r--   0 max       (1000) max       (1000)    13561 2022-06-03 21:13:52.000000 cobib-3.5.5/tests/utils/test_shell_helper.py
--rw-r--r--   0 max       (1000) max       (1000)     1909 2021-10-12 20:39:32.000000 cobib-3.5.5/tests/utils/unified_database.yaml
--rw-r--r--   0 max       (1000) max       (1000)     1907 2021-10-12 20:39:32.000000 cobib-3.5.5/tests/utils/unifying_database.yaml
--rw-r--r--   0 max       (1000) max       (1000)     1567 2023-01-22 12:13:09.000000 cobib-3.5.5/tox.ini
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-20 14:28:46.008988 cobib-4.0.0/
+-rw-r--r--   0 max       (1000) max       (1000)      217 2021-09-20 21:31:31.000000 cobib-4.0.0/.coveragerc
+-rw-r--r--   0 max       (1000) max       (1000)      268 2023-04-15 10:28:42.000000 cobib-4.0.0/.gitignore
+-rw-r--r--   0 max       (1000) max       (1000)     2718 2023-04-15 20:38:04.000000 cobib-4.0.0/.gitlab-ci.yml
+-rw-r--r--   0 max       (1000) max       (1000)       75 2023-05-14 13:30:20.000000 cobib-4.0.0/.pydocstylerc
+-rw-r--r--   0 max       (1000) max       (1000)      888 2023-05-20 12:00:53.000000 cobib-4.0.0/.pylintdict
+-rw-r--r--   0 max       (1000) max       (1000)    11236 2023-04-15 10:28:42.000000 cobib-4.0.0/.pylintrc
+-rw-r--r--   0 max       (1000) max       (1000)    28312 2023-05-20 14:26:11.000000 cobib-4.0.0/CHANGELOG.md
+-rw-r--r--   0 max       (1000) max       (1000)     2247 2023-05-01 17:07:35.000000 cobib-4.0.0/CONTRIBUTING.md
+-rw-r--r--   0 max       (1000) max       (1000)     1076 2023-04-28 18:20:00.000000 cobib-4.0.0/LICENSE.txt
+-rw-r--r--   0 max       (1000) max       (1000)      115 2021-09-20 21:31:31.000000 cobib-4.0.0/MANIFEST.in
+-rw-r--r--   0 max       (1000) max       (1000)      187 2021-09-20 21:31:31.000000 cobib-4.0.0/Makefile
+-rw-r--r--   0 max       (1000) max       (1000)    37193 2023-05-20 14:28:46.008988 cobib-4.0.0/PKG-INFO
+-rw-r--r--   0 max       (1000) max       (1000)     7871 2023-05-20 12:00:53.000000 cobib-4.0.0/README.md
+-rw-r--r--   0 max       (1000) max       (1000)      563 2021-09-20 21:31:31.000000 cobib-4.0.0/_cobib
+-rw-r--r--   0 max       (1000) max       (1000)    24744 2023-05-20 14:26:50.000000 cobib-4.0.0/cobib.1
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-20 14:28:45.972322 cobib-4.0.0/html/
+-rw-r--r--   0 max       (1000) max       (1000)    34915 2023-05-07 10:49:25.000000 cobib-4.0.0/html/cobib_book.svg
+-rw-r--r--   0 max       (1000) max       (1000)    61955 2023-05-07 10:49:25.000000 cobib-4.0.0/html/cobib_logo.svg
+-rw-r--r--   0 max       (1000) max       (1000)      554 2023-05-07 10:49:25.000000 cobib-4.0.0/html/index.html.jinja2
+-rw-r--r--   0 max       (1000) max       (1000)      398 2023-05-07 10:49:25.000000 cobib-4.0.0/html/module.html.jinja2
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-20 14:28:45.972322 cobib-4.0.0/logo/
+-rw-r--r--   0 max       (1000) max       (1000)    44669 2021-09-20 21:31:31.000000 cobib-4.0.0/logo/cobib_book-squared.png
+-rw-r--r--   0 max       (1000) max       (1000)    40896 2021-09-20 21:31:31.000000 cobib-4.0.0/logo/cobib_book.png
+-rw-r--r--   0 max       (1000) max       (1000)    34915 2021-09-20 21:31:31.000000 cobib-4.0.0/logo/cobib_book.svg
+-rw-r--r--   0 max       (1000) max       (1000)    74851 2021-09-20 21:31:31.000000 cobib-4.0.0/logo/cobib_byline.png
+-rw-r--r--   0 max       (1000) max       (1000)    27555 2021-09-20 21:31:31.000000 cobib-4.0.0/logo/cobib_byline.svg
+-rw-r--r--   0 max       (1000) max       (1000)   126027 2021-09-20 21:31:31.000000 cobib-4.0.0/logo/cobib_logo.png
+-rw-r--r--   0 max       (1000) max       (1000)    61955 2021-09-20 21:31:31.000000 cobib-4.0.0/logo/cobib_logo.svg
+-rw-r--r--   0 max       (1000) max       (1000)      507 2023-04-15 20:38:04.000000 cobib-4.0.0/mypy.ini
+-rw-r--r--   0 max       (1000) max       (1000)      356 2023-04-15 20:14:50.000000 cobib-4.0.0/pyproject.toml
+-rw-r--r--   0 max       (1000) max       (1000)       27 2021-09-20 21:31:31.000000 cobib-4.0.0/pytest.ini
+-rw-r--r--   0 max       (1000) max       (1000)      115 2023-05-14 13:30:20.000000 cobib-4.0.0/requirements.txt
+-rw-r--r--   0 max       (1000) max       (1000)     1221 2023-05-20 14:28:46.012322 cobib-4.0.0/setup.cfg
+-rw-r--r--   0 max       (1000) max       (1000)      296 2021-09-20 21:31:31.000000 cobib-4.0.0/setup.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-20 14:28:45.958988 cobib-4.0.0/src/
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-20 14:28:45.975655 cobib-4.0.0/src/cobib/
+-rw-r--r--   0 max       (1000) max       (1000)      474 2023-05-20 14:27:06.000000 cobib-4.0.0/src/cobib/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)      648 2023-05-20 12:00:53.000000 cobib-4.0.0/src/cobib/__main__.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-20 14:28:45.978988 cobib-4.0.0/src/cobib/commands/
+-rw-r--r--   0 max       (1000) max       (1000)      903 2023-05-20 12:00:53.000000 cobib-4.0.0/src/cobib/commands/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)    20549 2023-05-14 19:24:23.000000 cobib-4.0.0/src/cobib/commands/add.py
+-rw-r--r--   0 max       (1000) max       (1000)     7832 2023-05-20 13:33:32.000000 cobib-4.0.0/src/cobib/commands/base_command.py
+-rw-r--r--   0 max       (1000) max       (1000)     2983 2023-05-14 13:30:20.000000 cobib-4.0.0/src/cobib/commands/delete.py
+-rw-r--r--   0 max       (1000) max       (1000)     6675 2023-05-14 13:30:20.000000 cobib-4.0.0/src/cobib/commands/edit.py
+-rw-r--r--   0 max       (1000) max       (1000)     7740 2023-05-20 13:36:34.000000 cobib-4.0.0/src/cobib/commands/export.py
+-rw-r--r--   0 max       (1000) max       (1000)     6083 2023-05-14 20:12:11.000000 cobib-4.0.0/src/cobib/commands/import_.py
+-rw-r--r--   0 max       (1000) max       (1000)     4786 2023-05-14 13:30:20.000000 cobib-4.0.0/src/cobib/commands/init.py
+-rw-r--r--   0 max       (1000) max       (1000)    12093 2023-05-20 13:30:05.000000 cobib-4.0.0/src/cobib/commands/list_.py
+-rw-r--r--   0 max       (1000) max       (1000)    16872 2023-05-20 13:36:20.000000 cobib-4.0.0/src/cobib/commands/modify.py
+-rw-r--r--   0 max       (1000) max       (1000)     9080 2023-05-14 13:30:20.000000 cobib-4.0.0/src/cobib/commands/open.py
+-rw-r--r--   0 max       (1000) max       (1000)     4772 2023-05-14 13:30:20.000000 cobib-4.0.0/src/cobib/commands/redo.py
+-rw-r--r--   0 max       (1000) max       (1000)     9070 2023-05-20 13:40:05.000000 cobib-4.0.0/src/cobib/commands/search.py
+-rw-r--r--   0 max       (1000) max       (1000)     2369 2023-05-14 13:30:20.000000 cobib-4.0.0/src/cobib/commands/show.py
+-rw-r--r--   0 max       (1000) max       (1000)     5469 2023-05-14 13:30:20.000000 cobib-4.0.0/src/cobib/commands/undo.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-20 14:28:45.978988 cobib-4.0.0/src/cobib/config/
+-rw-r--r--   0 max       (1000) max       (1000)     1210 2022-01-13 20:47:42.000000 cobib-4.0.0/src/cobib/config/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)    23787 2023-05-14 13:30:20.000000 cobib-4.0.0/src/cobib/config/config.py
+-rw-r--r--   0 max       (1000) max       (1000)    29728 2023-05-15 16:25:02.000000 cobib-4.0.0/src/cobib/config/event.py
+-rw-r--r--   0 max       (1000) max       (1000)     8140 2023-05-11 19:09:33.000000 cobib-4.0.0/src/cobib/config/example.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-20 14:28:45.982322 cobib-4.0.0/src/cobib/database/
+-rw-r--r--   0 max       (1000) max       (1000)      283 2021-09-20 21:31:31.000000 cobib-4.0.0/src/cobib/database/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     9818 2023-05-11 19:09:33.000000 cobib-4.0.0/src/cobib/database/database.py
+-rw-r--r--   0 max       (1000) max       (1000)    17670 2023-05-14 13:30:20.000000 cobib-4.0.0/src/cobib/database/entry.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-20 14:28:45.982322 cobib-4.0.0/src/cobib/importers/
+-rw-r--r--   0 max       (1000) max       (1000)      275 2021-12-01 20:44:34.000000 cobib-4.0.0/src/cobib/importers/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     3086 2023-05-20 12:00:53.000000 cobib-4.0.0/src/cobib/importers/base_importer.py
+-rw-r--r--   0 max       (1000) max       (1000)    12858 2023-05-20 12:00:53.000000 cobib-4.0.0/src/cobib/importers/zotero.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-20 14:28:45.985655 cobib-4.0.0/src/cobib/parsers/
+-rw-r--r--   0 max       (1000) max       (1000)      520 2021-09-25 22:36:09.000000 cobib-4.0.0/src/cobib/parsers/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     5039 2023-05-14 13:30:20.000000 cobib-4.0.0/src/cobib/parsers/arxiv.py
+-rw-r--r--   0 max       (1000) max       (1000)     2053 2021-09-20 21:31:31.000000 cobib-4.0.0/src/cobib/parsers/base_parser.py
+-rw-r--r--   0 max       (1000) max       (1000)     2994 2023-05-14 13:30:20.000000 cobib-4.0.0/src/cobib/parsers/bibtex.py
+-rw-r--r--   0 max       (1000) max       (1000)     3267 2023-05-14 13:30:20.000000 cobib-4.0.0/src/cobib/parsers/doi.py
+-rw-r--r--   0 max       (1000) max       (1000)     4559 2023-05-14 13:30:20.000000 cobib-4.0.0/src/cobib/parsers/isbn.py
+-rw-r--r--   0 max       (1000) max       (1000)     3522 2023-05-14 13:30:20.000000 cobib-4.0.0/src/cobib/parsers/url.py
+-rw-r--r--   0 max       (1000) max       (1000)     2996 2023-05-14 13:30:20.000000 cobib-4.0.0/src/cobib/parsers/yaml.py
+-rw-r--r--   0 max       (1000) max       (1000)        0 2021-09-20 21:31:31.000000 cobib-4.0.0/src/cobib/py.typed
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-20 14:28:45.985655 cobib-4.0.0/src/cobib/ui/
+-rw-r--r--   0 max       (1000) max       (1000)      611 2023-05-20 12:00:53.000000 cobib-4.0.0/src/cobib/ui/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     3395 2023-05-20 12:00:53.000000 cobib-4.0.0/src/cobib/ui/cli.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-20 14:28:45.988988 cobib-4.0.0/src/cobib/ui/components/
+-rw-r--r--   0 max       (1000) max       (1000)      991 2023-05-20 12:00:53.000000 cobib-4.0.0/src/cobib/ui/components/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     1448 2023-05-20 12:00:53.000000 cobib-4.0.0/src/cobib/ui/components/argument_parser.py
+-rw-r--r--   0 max       (1000) max       (1000)      963 2023-05-20 12:00:53.000000 cobib-4.0.0/src/cobib/ui/components/entry_view.py
+-rw-r--r--   0 max       (1000) max       (1000)     2673 2023-05-20 12:00:53.000000 cobib-4.0.0/src/cobib/ui/components/help_popup.py
+-rw-r--r--   0 max       (1000) max       (1000)     1438 2023-05-20 12:00:53.000000 cobib-4.0.0/src/cobib/ui/components/input.py
+-rw-r--r--   0 max       (1000) max       (1000)     1173 2023-05-20 12:00:53.000000 cobib-4.0.0/src/cobib/ui/components/main_view.py
+-rw-r--r--   0 max       (1000) max       (1000)     2035 2023-05-20 12:00:53.000000 cobib-4.0.0/src/cobib/ui/components/popup.py
+-rw-r--r--   0 max       (1000) max       (1000)     1405 2023-05-20 12:00:53.000000 cobib-4.0.0/src/cobib/ui/components/popup_logging_handler.py
+-rw-r--r--   0 max       (1000) max       (1000)      668 2023-05-20 12:00:53.000000 cobib-4.0.0/src/cobib/ui/components/popup_panel.py
+-rw-r--r--   0 max       (1000) max       (1000)     1082 2023-05-20 12:00:53.000000 cobib-4.0.0/src/cobib/ui/components/progress.py
+-rw-r--r--   0 max       (1000) max       (1000)     3482 2023-05-20 12:00:53.000000 cobib-4.0.0/src/cobib/ui/components/prompt.py
+-rw-r--r--   0 max       (1000) max       (1000)     1415 2023-05-20 12:00:53.000000 cobib-4.0.0/src/cobib/ui/components/selection_filter.py
+-rw-r--r--   0 max       (1000) max       (1000)     1733 2023-05-20 12:00:53.000000 cobib-4.0.0/src/cobib/ui/shell_helper.py
+-rw-r--r--   0 max       (1000) max       (1000)    20649 2023-05-20 12:00:53.000000 cobib-4.0.0/src/cobib/ui/tui.py
+-rw-r--r--   0 max       (1000) max       (1000)     4273 2023-05-20 12:00:53.000000 cobib-4.0.0/src/cobib/ui/ui.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-20 14:28:45.992322 cobib-4.0.0/src/cobib/utils/
+-rw-r--r--   0 max       (1000) max       (1000)      242 2021-09-20 21:31:31.000000 cobib-4.0.0/src/cobib/utils/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     6731 2023-05-14 19:24:23.000000 cobib-4.0.0/src/cobib/utils/diff_renderer.py
+-rw-r--r--   0 max       (1000) max       (1000)     8653 2023-05-14 19:24:23.000000 cobib-4.0.0/src/cobib/utils/file_downloader.py
+-rw-r--r--   0 max       (1000) max       (1000)     4533 2021-09-20 21:32:23.000000 cobib-4.0.0/src/cobib/utils/journal_abbreviations.py
+-rw-r--r--   0 max       (1000) max       (1000)     5128 2023-05-14 13:30:20.000000 cobib-4.0.0/src/cobib/utils/logging.py
+-rw-r--r--   0 max       (1000) max       (1000)     1837 2021-09-20 21:31:31.000000 cobib-4.0.0/src/cobib/utils/rel_path.py
+-rw-r--r--   0 max       (1000) max       (1000)     8212 2023-05-14 13:30:20.000000 cobib-4.0.0/src/cobib/utils/shell_helper.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-20 14:28:45.975655 cobib-4.0.0/src/cobib.egg-info/
+-rw-r--r--   0 max       (1000) max       (1000)    37193 2023-05-20 14:28:45.000000 cobib-4.0.0/src/cobib.egg-info/PKG-INFO
+-rw-r--r--   0 max       (1000) max       (1000)     4226 2023-05-20 14:28:45.000000 cobib-4.0.0/src/cobib.egg-info/SOURCES.txt
+-rw-r--r--   0 max       (1000) max       (1000)        1 2023-05-20 14:28:45.000000 cobib-4.0.0/src/cobib.egg-info/dependency_links.txt
+-rw-r--r--   0 max       (1000) max       (1000)       47 2023-05-20 14:28:45.000000 cobib-4.0.0/src/cobib.egg-info/entry_points.txt
+-rw-r--r--   0 max       (1000) max       (1000)      115 2023-05-20 14:28:45.000000 cobib-4.0.0/src/cobib.egg-info/requires.txt
+-rw-r--r--   0 max       (1000) max       (1000)        6 2023-05-20 14:28:45.000000 cobib-4.0.0/src/cobib.egg-info/top_level.txt
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-20 14:28:45.995655 cobib-4.0.0/tests/
+-rw-r--r--   0 max       (1000) max       (1000)     1508 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)      872 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/cmdline_test.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-20 14:28:46.002322 cobib-4.0.0/tests/commands/
+-rw-r--r--   0 max       (1000) max       (1000)       68 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/commands/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     5831 2023-05-14 13:30:20.000000 cobib-4.0.0/tests/commands/command_test.py
+-rw-r--r--   0 max       (1000) max       (1000)      248 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/commands/example_duplicate_entry.bib
+-rw-r--r--   0 max       (1000) max       (1000)      261 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/commands/example_duplicate_entry.yaml
+-rw-r--r--   0 max       (1000) max       (1000)      134 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/commands/example_multi_file_entry.bib
+-rw-r--r--   0 max       (1000) max       (1000)      155 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/commands/example_multi_file_entry.yaml
+-rw-r--r--   0 max       (1000) max       (1000)    24929 2023-05-14 13:30:20.000000 cobib-4.0.0/tests/commands/test_add.py
+-rw-r--r--   0 max       (1000) max       (1000)     6251 2023-05-14 13:30:20.000000 cobib-4.0.0/tests/commands/test_delete.py
+-rw-r--r--   0 max       (1000) max       (1000)     7555 2023-05-14 13:30:20.000000 cobib-4.0.0/tests/commands/test_edit.py
+-rw-r--r--   0 max       (1000) max       (1000)     8218 2023-05-14 13:30:20.000000 cobib-4.0.0/tests/commands/test_export.py
+-rw-r--r--   0 max       (1000) max       (1000)     3058 2023-05-14 13:30:20.000000 cobib-4.0.0/tests/commands/test_git_commit_event.py
+-rw-r--r--   0 max       (1000) max       (1000)     2167 2023-05-14 19:24:23.000000 cobib-4.0.0/tests/commands/test_import.py
+-rw-r--r--   0 max       (1000) max       (1000)     6102 2023-05-14 13:30:20.000000 cobib-4.0.0/tests/commands/test_init.py
+-rw-r--r--   0 max       (1000) max       (1000)     9171 2023-05-14 13:30:20.000000 cobib-4.0.0/tests/commands/test_list.py
+-rw-r--r--   0 max       (1000) max       (1000)     8757 2023-05-14 13:30:20.000000 cobib-4.0.0/tests/commands/test_modify.py
+-rw-r--r--   0 max       (1000) max       (1000)    14520 2023-05-14 13:30:20.000000 cobib-4.0.0/tests/commands/test_open.py
+-rw-r--r--   0 max       (1000) max       (1000)     8550 2023-05-14 13:30:20.000000 cobib-4.0.0/tests/commands/test_redo.py
+-rw-r--r--   0 max       (1000) max       (1000)     7131 2023-05-20 13:40:09.000000 cobib-4.0.0/tests/commands/test_search.py
+-rw-r--r--   0 max       (1000) max       (1000)     4232 2023-05-14 13:30:20.000000 cobib-4.0.0/tests/commands/test_show.py
+-rw-r--r--   0 max       (1000) max       (1000)     7831 2023-05-14 13:30:20.000000 cobib-4.0.0/tests/commands/test_undo.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-20 14:28:46.002322 cobib-4.0.0/tests/config/
+-rw-r--r--   0 max       (1000) max       (1000)       28 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/config/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)      147 2023-05-11 19:09:33.000000 cobib-4.0.0/tests/config/broken_config.py
+-rw-r--r--   0 max       (1000) max       (1000)     3312 2023-05-11 19:09:33.000000 cobib-4.0.0/tests/config/test_config.py
+-rw-r--r--   0 max       (1000) max       (1000)     2401 2023-05-11 19:09:33.000000 cobib-4.0.0/tests/config/test_event.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-20 14:28:46.002322 cobib-4.0.0/tests/database/
+-rw-r--r--   0 max       (1000) max       (1000)       30 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/database/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)       59 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/database/example_entry_umlaut.bib
+-rw-r--r--   0 max       (1000) max       (1000)     8136 2023-05-11 19:09:33.000000 cobib-4.0.0/tests/database/test_database.py
+-rw-r--r--   0 max       (1000) max       (1000)    14623 2023-05-08 19:51:42.000000 cobib-4.0.0/tests/database/test_entry.py
+-rw-r--r--   0 max       (1000) max       (1000)      444 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/debug.py
+-rw-r--r--   0 max       (1000) max       (1000)      651 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/example_entry.bib
+-rw-r--r--   0 max       (1000) max       (1000)      621 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/example_entry.yaml
+-rw-r--r--   0 max       (1000) max       (1000)      723 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/example_literature.bib
+-rw-r--r--   0 max       (1000) max       (1000)      636 2023-05-08 19:47:05.000000 cobib-4.0.0/tests/example_literature.yaml
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-20 14:28:46.005655 cobib-4.0.0/tests/importers/
+-rw-r--r--   0 max       (1000) max       (1000)       71 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/importers/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)      274 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/importers/importer_test.py
+-rw-r--r--   0 max       (1000) max       (1000)     4802 2023-05-14 20:12:11.000000 cobib-4.0.0/tests/importers/test_zotero.py
+-rw-r--r--   0 max       (1000) max       (1000)     2609 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/importers/zotero_database.yaml
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-20 14:28:46.005655 cobib-4.0.0/tests/parsers/
+-rw-r--r--   0 max       (1000) max       (1000)       65 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/parsers/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     1395 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/parsers/parser_test.py
+-rw-r--r--   0 max       (1000) max       (1000)     5763 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/parsers/test_arxiv.py
+-rw-r--r--   0 max       (1000) max       (1000)     3224 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/parsers/test_bibtex.py
+-rw-r--r--   0 max       (1000) max       (1000)     5017 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/parsers/test_doi.py
+-rw-r--r--   0 max       (1000) max       (1000)     5562 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/parsers/test_isbn.py
+-rw-r--r--   0 max       (1000) max       (1000)     4374 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/parsers/test_url.py
+-rw-r--r--   0 max       (1000) max       (1000)     3251 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/parsers/test_yaml.py
+-rw-r--r--   0 max       (1000) max       (1000)     4353 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/test_main.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-05-20 14:28:46.008988 cobib-4.0.0/tests/utils/
+-rw-r--r--   0 max       (1000) max       (1000)       29 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/utils/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)      172 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/utils/fixed_database.yaml
+-rw-r--r--   0 max       (1000) max       (1000)      163 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/utils/linting_database.yaml
+-rw-r--r--   0 max       (1000) max       (1000)     8992 2023-05-14 19:24:23.000000 cobib-4.0.0/tests/utils/test_file_downloader.py
+-rw-r--r--   0 max       (1000) max       (1000)     3216 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/utils/test_journal_abbreviations.py
+-rw-r--r--   0 max       (1000) max       (1000)     2990 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/utils/test_logging.py
+-rw-r--r--   0 max       (1000) max       (1000)      964 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/utils/test_rel_path.py
+-rw-r--r--   0 max       (1000) max       (1000)    13477 2023-05-14 13:30:20.000000 cobib-4.0.0/tests/utils/test_shell_helper.py
+-rw-r--r--   0 max       (1000) max       (1000)     1909 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/utils/unified_database.yaml
+-rw-r--r--   0 max       (1000) max       (1000)     1907 2023-05-07 10:49:48.000000 cobib-4.0.0/tests/utils/unifying_database.yaml
+-rw-r--r--   0 max       (1000) max       (1000)     1287 2023-05-11 19:09:33.000000 cobib-4.0.0/tox.ini
```

### Comparing `cobib-3.5.5/.gitlab-ci.yml` & `cobib-4.0.0/.gitlab-ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
             coverage_format: cobertura
             path: cobertura.xml
 
 test:
     stage: test
     parallel:
         matrix:
-            - PYTHON_VERSION: ['3.7', '3.8', '3.9', '3.10']
+            - PYTHON_VERSION: ['3.8', '3.9', '3.10', '3.11']
     image: python:$PYTHON_VERSION
     script:
         - tox -e py$PYTHON_VERSION
     artifacts:
         when: always
         expire_in: 30 days
         paths:
```

### Comparing `cobib-3.5.5/.pylintdict` & `cobib-4.0.0/.pylintdict`

 * *Files 22% similar despite different names*

```diff
@@ -1,157 +1,113 @@
-abstractmethod
-addcommand
 aip
-ansi
 api
-archlinux
 arg
 argparse
 args
-argumenterror
-argumentparser
-argv
 arxiv
 ast
+async
 attr
-aug
-aur
 automagically
+awaitable
 backend
 backends
 biblatex
 bibtex
 bibtexexpression
 bibtexparser
-bool
-boolean
 caplog
 capsys
 changelog
 cli
+cmd
 cobib
 config
 configfile
-configparser
 configpath
-cov
 dat
+dataclass
+dataclasses
 deepcopied
-defaultdict
+diff
 disambiguated
 docstring
 doi
-dois
 dotless
 downloader
-editcommand
-einstein
 enum
-esc
-fmt
 formatter
-getter
+func
 github
 gitlab
 html
 https
-infoline
-ini
 init
-initcommand
 initializer
-initscr
 io
 isbn
-isbns
 json
+keybind
 kwargs
-listcommand
+largs
+layouting
+lexing
 logfile
-logrecord
 md
-mendeley
 monkeypatch
 monkeypatching
 mrossinek
 msg
 mypy
-noqa
+namespace
 oauth
 openable
 openlibrary
-ordereddict
 os
-parametrized
 parsers
 pathlib
 pdf
 pdoc
 phiresky
-pmincol
-pminrow
 postarxivparse
 postdoiparse
 postgitcommit
 postinitcommand
 postisbnparse
 pragma
 pre
-purepath
 py
-pylatexenc
 pypi
-pyte
 pytest
-readline
 readme
 readthedocs
-rgb
+renderable
+renderer
 ripgrep
 rossmannek
-rrggbb
 ruamel
-runtime
 scitation
-scrolloff
-searchcommand
 sha
-showcommand
-signum
-smaxcol
-smaxrow
-smincol
-sminrow
-stateful
-statusbar
-statusline
-stderr
-stdin
-stdout
-stdscr
+src
 str
 stringify
+subclasses
 subcommand
 subcommands
 submodule
 submodules
-subprocess
 subscribable
-sys
-textbuffer
-textiowrapper
-tmp
-topstatus
+textual's
+textualize
 tox
 tui
-undocommand
-unittest
+ui
+uis
 unittests
+unmount
 url
 viewport
 vpn
 www
 xdg
 yaml
-yamlparser
 zotero
-zsh
```

### Comparing `cobib-3.5.5/.pylintrc` & `cobib-4.0.0/.pylintrc`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 # all. Valid levels: HIGH, INFERENCE, INFERENCE_FAILURE, UNDEFINED
 confidence=
 
 # Enable the message, report, category or checker with the given id(s). You can
 # either give multiple identifier separated by comma (,) or put this option
 # multiple time (only on the command line, not in the configuration file where
 # it should appear only once). See also the "--disable" option for examples.
-#enable=
+enable=useless-suppression
 
 # Disable the message, report, category or checker with the given id(s). You
 # can either give multiple identifiers separated by comma (,) or put this
 # option multiple times (only on the command line, not in the configuration
 # file where it should appear only once).You can also use "--disable=all" to
 # disable everything first and then reenable specific checks. For example, if
 # you want to run only the similarities checker, you can use "--disable=all
@@ -337,15 +337,15 @@
 int-import-graph=
 
 # Force import order to recognize a module as part of the standard
 # compatibility libraries.
 known-standard-library=
 
 # Force import order to recognize a module as part of a third party library.
-known-third-party=enchant
+known-third-party=enchant,rich
 
 # Analyse import fallback blocks. This can be used to support both Python 2 and
 # 3 compatible code, which means that the block might have code that exists
 # only in one or another interpreter, leading to false positives when analysed.
 analyse-fallback-blocks=no
```

### Comparing `cobib-3.5.5/CHANGELOG.md` & `cobib-4.0.0/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,75 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
-The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
+The format is based on [Keep a Changelog](https://keepachangelog.com/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+
+## [4.0.0] - 2023-05-20
+
+Pypi: https://pypi.org/project/cobib/3.5.5/
+
+### **Breaking Changes**
+- Configuration settings can no longer be set by item access and instead must
+  use attribute syntax. For example you need to change:
+  ```python
+  config["database"]["git"] = True
+  ```
+  to
+  ```python
+  config.database.git = True
+  ```
+  - the `config.commands.list` section had to be renamed to `config.commands.list_`
+  - the `config.tui` section has been entirely removed
+- The `cobib.commands.list` module was moved to `cobib.commands.list_`.
+- The function signature of all command- and importer-related events has changed!
+  For more details please refer to the
+  [online documentation](https://cobib.gitlab.io/cobib/cobib/config/event.html).
+
+### Added
+- Python 3.11 is now officially tested and supported
+- Full rewrite of all commands to use `rich` for a nicer CLI (#78,!51)
+- Full rewrite of the TUI based on `textual` (#78,!51)
+- the `--disambiguation` argument of the `add` command (#99,!58)
+- the `--ignore-case` argument of the `list` command (#105)
+  - this also comes with the new `config.commands.list_.ignore_case` setting
+- the `search` command now accepts multiple query strings at once which will be
+  searched over independently (#106)
+
+### Changed
+- the new default value of `config.parsers.yaml.use_c_lib_yaml` is now `True` as announced in version [3.4.0]
+- refactored the entire config as a dataclass (!63)
+  - this implies that settings can only be set via attributes
+  - but as a benefit the maintainability and documentation have improved significantly
+- The function signature of all command-related events has changed! Please refer to the
+  [online documentation](https://cobib.gitlab.io/cobib/cobib/config/event.html)
+  for more details. (!63)
+- The function signature of all importer-related events has changed! Please refer to the
+  [online documentation](https://cobib.gitlab.io/cobib/cobib/config/event.html)
+  for more details. (!66)
+- the API of the `cobib.commands` and `cobib.importers` module has been improved (!64)
+  - this should not have any end-user facing effects
+- the `cobib.commands.list` module was moved to `cobib.commands.list_`
+
+### Deprecated
+- the `--update` argument of the `add` command is deprecated in favor of `--disambiguation update`
+- the `--skip-existing` argument of the `add` command is deprecated in favor of `--disambiguation keep`
+
+### Fixed
+- the detection whether an entry already exists broke when label disambiguation was added in [3.3.0]
+  and is now fixed by means of an interactive prompt during the `add` command
+
+### Removed
+- the warning triggered upon setting `config.database.format.month` which got removed in [3.1.0]
+- Python 3.7 is no longer supported
+
+
 ## [3.5.5] - 2023-04-11
 
 Pypi: https://pypi.org/project/cobib/3.5.5/
 
 ### Fixed
 - opening of non-list type fields (#100)
 
@@ -57,15 +117,15 @@
 This will open up some great possibilities for a much more modern UI.
 
 However, this change will require some *major* refactoring including breaking changes of the API
 and some of the user configuration options. It will also be a rather drastic change in style.
 Thus, I will attempt to support v3.5 with bugfix releases until 1.1.2023
 
 It will likely take a few months until v4.0 gets released but I am starting development on it now.
-You can follow the progress here: <https://gitlab.com/mrossinek/cobib/-/issues/78>
+You can follow the progress here: <https://gitlab.com/cobib/cobib/-/issues/78>
 
 [rich]: https://github.com/Textualize/rich
 [textual]: https://github.com/Textualize/textual
 
 ### Added
 - the configuration loading can be disabled via the environment variable `COBIB_CONFIG`
     - values which disable the loading entirely are: `"", 0, f, false, nil, none`
@@ -143,15 +203,15 @@
 * the `config.database.format.label_default` and `config.database.format.label_suffix` options (#85,!45)
     - labels will automatically be formatted according to the default option
     - if labels conflict with existing ones, the suffix option will be used for disambiguation
     - the `AddCommand` has a new `--skip-existing` option which disables automatic label disambiguation
     - use `cobib _unify_labels --apply` to unify all labels in your database
 - subscribable events (#71,!46)
     - allows registering of hooks to be executed in certain situation
-    - more information is provided at the [online documentation](https://mrossinek.gitlab.io/cobib/cobib/config/event.html)
+    - more information is provided at the [online documentation](https://cobib.gitlab.io/cobib/cobib/config/event.html)
 
 ### Changed
 - when an unknown variable is encountered in the modification of the `modify` command it falls back to an empty string rather than the name of the attempted variable
 
 ### Removed
 - the `-s` option of the `AddCommand` is no longer available. You need to write out `--skip-download`
 - the `ID` filter argument on the `list` command (deprecated in v3.2.0 in favor of the `label` filter)
@@ -242,15 +302,15 @@
 ## [3.0.0] - 2021-04-10
 
 Pypi: https://pypi.org/project/cobib/3.0.0/
 
 - From now on, `coBib` is the official way of spelling!
 
 ### Added
-- coBib's documentation is now generated by [`pdoc`](https://pdoc.dev/) and hosted at https://mrossinek.gitlab.io/cobib/cobib.html
+- coBib's documentation is now generated by [`pdoc`](https://pdoc.dev/) and hosted at https://cobib.gitlab.io/cobib/cobib.html
 - (DEV): the `cobib.database.Database`-Singleton has been added to centrally manage the bibliographic runtime data (!28)
 - the new option `config.database.format.suppress_latex_warnings`
 - the new option `config.commands.edit.editor` which takes precedence over the `$EDITOR` variable
 
 ### Changed
 - the `INI`-style configuration is replaced with a `Python`-based configuration (#54,!25)
     - for guidance on how to migrate an existing configuration please read https://mrossinek.gitlab.io/programming/cobibs-new-configuration/
@@ -646,51 +706,52 @@
 
 ## [0.1] - 2019-04-29
 
 ### Added
 - initial version with a basic `sqlite3`-based database
 
 
-[Unreleased]: https://gitlab.com/mrossinek/cobib/-/compare/v3.5.5...master
-[3.5.5]: https://gitlab.com/mrossinek/cobib/-/compare/v3.5.5
-[3.5.4]: https://gitlab.com/mrossinek/cobib/-/compare/v3.5.4
-[3.5.3]: https://gitlab.com/mrossinek/cobib/-/compare/v3.5.3
-[3.5.2]: https://gitlab.com/mrossinek/cobib/-/compare/v3.5.2
-[3.5.1]: https://gitlab.com/mrossinek/cobib/-/compare/v3.5.1
-[3.5.0]: https://gitlab.com/mrossinek/cobib/-/compare/v3.5.0
-[3.4.0]: https://gitlab.com/mrossinek/cobib/-/compare/v3.4.0
-[3.3.2]: https://gitlab.com/mrossinek/cobib/-/compare/v3.3.2
-[3.3.1]: https://gitlab.com/mrossinek/cobib/-/compare/v3.3.1
-[3.3.0]: https://gitlab.com/mrossinek/cobib/-/compare/v3.3.0
-[3.2.1]: https://gitlab.com/mrossinek/cobib/-/compare/v3.2.1
-[3.2.0]: https://gitlab.com/mrossinek/cobib/-/compare/v3.2.0
-[3.1.1]: https://gitlab.com/mrossinek/cobib/-/compare/v3.1.1
-[3.1.0]: https://gitlab.com/mrossinek/cobib/-/compare/v3.1.0
-[3.0.0]: https://gitlab.com/mrossinek/cobib/-/compare/v3.0.0
-[2.6.1]: https://gitlab.com/mrossinek/cobib/-/compare/v2.6.1
-[2.6.0]: https://gitlab.com/mrossinek/cobib/-/tags/v2.6.0
-[2.5.0]: https://gitlab.com/mrossinek/cobib/-/tags/v2.5.0
-[2.4.1]: https://gitlab.com/mrossinek/cobib/-/tags/v2.4.1
-[2.4.0]: https://gitlab.com/mrossinek/cobib/-/tags/v2.4.0
-[2.3.4]: https://gitlab.com/mrossinek/cobib/-/tags/v2.3.4
-[2.3.3]: https://gitlab.com/mrossinek/cobib/-/tags/v2.3.3
-[2.3.2]: https://gitlab.com/mrossinek/cobib/-/tags/v2.3.2
-[2.3.1]: https://gitlab.com/mrossinek/cobib/-/tags/v2.3.1
-[2.3.0]: https://gitlab.com/mrossinek/cobib/-/tags/v2.3.0
-[2.2.2]: https://gitlab.com/mrossinek/cobib/-/tags/v2.2.2
-[2.2.1]: https://gitlab.com/mrossinek/cobib/-/tags/v2.2.1
-[2.2.0]: https://gitlab.com/mrossinek/cobib/-/tags/v2.2.0
-[2.1.0]: https://gitlab.com/mrossinek/cobib/-/tags/v2.1.0
-[2.0.0]: https://gitlab.com/mrossinek/cobib/-/tags/v2.0.0
-[2.0.0b4]: https://gitlab.com/mrossinek/cobib/-/tags/v2.0.0b4
-[2.0.0b3]: https://gitlab.com/mrossinek/cobib/-/tags/v2.0.0b3
-[2.0.0b2]: https://gitlab.com/mrossinek/cobib/-/tags/v2.0.0b2
-[2.0.0b1]: https://gitlab.com/mrossinek/cobib/-/tags/v2.0.0b1
-[2.0.0b0]: https://gitlab.com/mrossinek/cobib/-/tags/v2.0.0b0
-[2.0.0a2]: https://gitlab.com/mrossinek/cobib/-/tags/v2.0.0a2
-[2.0.0a1]: https://gitlab.com/mrossinek/cobib/-/tags/v2.0.0a1
-[1.1.0]: https://gitlab.com/mrossinek/cobib/-/tags/v1.1.0
-[1.0.2]: https://gitlab.com/mrossinek/cobib/-/tags/v1.0.2
-[1.0.1]: https://gitlab.com/mrossinek/cobib/-/tags/v1.0.1
-[1.0.0]: https://gitlab.com/mrossinek/cobib/-/tags/v1.0.0
-[0.2]: https://gitlab.com/mrossinek/cobib/-/tags/v0.2
-[0.1]: https://gitlab.com/mrossinek/cobib/-/tags/v0.1
+[Unreleased]: https://gitlab.com/cobib/cobib/-/compare/v4.0.0...master
+[4.0.0]: https://gitlab.com/cobib/cobib/-/compare/v4.0.0
+[3.5.5]: https://gitlab.com/cobib/cobib/-/compare/v3.5.5
+[3.5.4]: https://gitlab.com/cobib/cobib/-/compare/v3.5.4
+[3.5.3]: https://gitlab.com/cobib/cobib/-/compare/v3.5.3
+[3.5.2]: https://gitlab.com/cobib/cobib/-/compare/v3.5.2
+[3.5.1]: https://gitlab.com/cobib/cobib/-/compare/v3.5.1
+[3.5.0]: https://gitlab.com/cobib/cobib/-/compare/v3.5.0
+[3.4.0]: https://gitlab.com/cobib/cobib/-/compare/v3.4.0
+[3.3.2]: https://gitlab.com/cobib/cobib/-/compare/v3.3.2
+[3.3.1]: https://gitlab.com/cobib/cobib/-/compare/v3.3.1
+[3.3.0]: https://gitlab.com/cobib/cobib/-/compare/v3.3.0
+[3.2.1]: https://gitlab.com/cobib/cobib/-/compare/v3.2.1
+[3.2.0]: https://gitlab.com/cobib/cobib/-/compare/v3.2.0
+[3.1.1]: https://gitlab.com/cobib/cobib/-/compare/v3.1.1
+[3.1.0]: https://gitlab.com/cobib/cobib/-/compare/v3.1.0
+[3.0.0]: https://gitlab.com/cobib/cobib/-/compare/v3.0.0
+[2.6.1]: https://gitlab.com/cobib/cobib/-/compare/v2.6.1
+[2.6.0]: https://gitlab.com/cobib/cobib/-/tags/v2.6.0
+[2.5.0]: https://gitlab.com/cobib/cobib/-/tags/v2.5.0
+[2.4.1]: https://gitlab.com/cobib/cobib/-/tags/v2.4.1
+[2.4.0]: https://gitlab.com/cobib/cobib/-/tags/v2.4.0
+[2.3.4]: https://gitlab.com/cobib/cobib/-/tags/v2.3.4
+[2.3.3]: https://gitlab.com/cobib/cobib/-/tags/v2.3.3
+[2.3.2]: https://gitlab.com/cobib/cobib/-/tags/v2.3.2
+[2.3.1]: https://gitlab.com/cobib/cobib/-/tags/v2.3.1
+[2.3.0]: https://gitlab.com/cobib/cobib/-/tags/v2.3.0
+[2.2.2]: https://gitlab.com/cobib/cobib/-/tags/v2.2.2
+[2.2.1]: https://gitlab.com/cobib/cobib/-/tags/v2.2.1
+[2.2.0]: https://gitlab.com/cobib/cobib/-/tags/v2.2.0
+[2.1.0]: https://gitlab.com/cobib/cobib/-/tags/v2.1.0
+[2.0.0]: https://gitlab.com/cobib/cobib/-/tags/v2.0.0
+[2.0.0b4]: https://gitlab.com/cobib/cobib/-/tags/v2.0.0b4
+[2.0.0b3]: https://gitlab.com/cobib/cobib/-/tags/v2.0.0b3
+[2.0.0b2]: https://gitlab.com/cobib/cobib/-/tags/v2.0.0b2
+[2.0.0b1]: https://gitlab.com/cobib/cobib/-/tags/v2.0.0b1
+[2.0.0b0]: https://gitlab.com/cobib/cobib/-/tags/v2.0.0b0
+[2.0.0a2]: https://gitlab.com/cobib/cobib/-/tags/v2.0.0a2
+[2.0.0a1]: https://gitlab.com/cobib/cobib/-/tags/v2.0.0a1
+[1.1.0]: https://gitlab.com/cobib/cobib/-/tags/v1.1.0
+[1.0.2]: https://gitlab.com/cobib/cobib/-/tags/v1.0.2
+[1.0.1]: https://gitlab.com/cobib/cobib/-/tags/v1.0.1
+[1.0.0]: https://gitlab.com/cobib/cobib/-/tags/v1.0.0
+[0.2]: https://gitlab.com/cobib/cobib/-/tags/v0.2
+[0.1]: https://gitlab.com/cobib/cobib/-/tags/v0.1
```

### Comparing `cobib-3.5.5/CONTRIBUTING.md` & `cobib-4.0.0/CONTRIBUTING.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Contributing
-If you want to contribute to coBib feel free to open a [PR on Gitlab](https://gitlab.com/mrossinek/cobib/-/merge_requests).
+If you want to contribute to coBib feel free to open a [PR on Gitlab](https://gitlab.com/cobib/cobib/-/merge_requests).
 Bug fixes and feature additions are always welcome!
-If you need some inspiration you also take a look at the [list of open issues](https://gitlab.com/mrossinek/cobib/-/issues) to see whether there is something you can help with.
+If you need some inspiration you also take a look at the [list of open issues](https://gitlab.com/cobib/cobib/-/issues) to see whether there is something you can help with.
 
 ## Setup
 We are using [`tox`](https://tox.readthedocs.io/en/latest/index.html) for a unified testing experience between local installations and the CI.
 Thus, after installing tox (`pip install tox`) you can inspect the available environments with `tox -l`.
 You can also inspect `tox.ini` and install the required development tools manually.
 I choose not to duplicate the information in another file, because this is likely to become outdated when it is not being used regularly.
 
@@ -26,15 +26,15 @@
 ## Coverage
 You can check the coverage with:
 ```
 tox -e coverage
 ```
 
 ## Documentation
-When working on coBib you may find the online documentation at https://mrossinek.gitlab.io/cobib/cobib.html or a locally generated version, useful.
+When working on coBib you may find the online documentation at https://cobib.gitlab.io/cobib/cobib.html or a locally generated version, useful.
 For the latter, please refer to the README.
 
 Once you have opened a merge request on GitLab, you can also view an automatically generated version of the documentation for your branch through the `View App` button below the `Pipeline` results.
 
 ## Releasing [Repository admins only]
 To create a new release you should do the following steps:
 0. Update the version number in `src/cobib/__init__.py` and the man page
```

### Comparing `cobib-3.5.5/LICENSE.txt` & `cobib-4.0.0/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-Copyright (c) 2019-2022 Max Rossmannek
+MIT License
+
+Copyright (c) 2019-2023 Max Rossmannek
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 the Software, and to permit persons to whom the Software is furnished to do so,
 subject to the following conditions:
```

### Comparing `cobib-3.5.5/PKG-INFO` & `cobib-4.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,95 +1,84 @@
 Metadata-Version: 2.1
 Name: cobib
-Version: 3.5.5
+Version: 4.0.0
 Summary: Console Bibliography
-Home-page: https://gitlab.com/mrossinek/cobib
+Home-page: https://gitlab.com/cobib/cobib
 Author: Max Rossmannek
 Author-email: max.rossmannek@uzh.ch
 License: MIT License
-Project-URL: Bug Tracker, https://gitlab.com/mrossinek/cobib/-/issues
-Project-URL: Documentation, https://mrossinek.gitlab.io/cobib/cobib.html
+Project-URL: Bug Tracker, https://gitlab.com/cobib/cobib/-/issues
+Project-URL: Documentation, https://cobib.gitlab.io/cobib/cobib.html
 Keywords: reference-manager, citation-manager, bibliography, cli, tui, command-line,,terminal, console, bibtex, doi, arxiv, isbn
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
-Classifier: Environment :: Console :: Curses
+Classifier: Environment :: Console
 Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-[![coBib](https://gitlab.com/mrossinek/cobib/-/raw/master/logo/cobib_logo.svg)](https://mrossinek.gitlab.io/cobib/cobib.html)
+[![coBib](https://gitlab.com/cobib/cobib/-/raw/master/logo/cobib_logo.svg)](https://cobib.gitlab.io/cobib/cobib.html)
 
 # coBib
 
-[![pipeline](https://gitlab.com/mrossinek/cobib/badges/master/pipeline.svg)](https://gitlab.com/mrossinek/cobib/-/pipelines)
-[![coverage](https://gitlab.com/mrossinek/cobib/badges/master/coverage.svg)](https://gitlab.com/mrossinek/cobib/-/graphs/master/charts)
+[![pipeline](https://gitlab.com/cobib/cobib/badges/master/pipeline.svg)](https://gitlab.com/cobib/cobib/-/pipelines)
+[![coverage](https://gitlab.com/cobib/cobib/badges/master/coverage.svg)](https://gitlab.com/cobib/cobib/-/graphs/master/charts)
 [![PyPI](https://img.shields.io/pypi/v/cobib)](https://pypi.org/project/cobib/)
 
 coBib is a simple, command-line based bibliography management tool.
 It is the result of the need for an easy-to-use alternative to full-blown reference managers like Mendeley or Zotero.
 As such it follows some basic design goals:
 
 * **plain-text database**: which means you get full access and control over the database.
 * **git-integration**: as a benefit of the above, you can keep track of your database through version control.
 * **centralized database, location-independent library**: this means, that coBib *only* manages the
   database file in a centralized fashion but allows you to spread the actual contents of your
   library across the entire file system (this is the major different to
   [papis](https://papis.readthedocs.io/en/latest/library_structure.html)).
-* **command-line and TUI support**: all features are available through the command-line as well as a curses-based TUI.
+* **command-line and TUI support**: all features are available through the command-line as well as a
+  [textual](https://textual.textualize.io/)-based TUI
 
 
-### **News:** coBib v4.0 will come with a new UI!
-The plan is to switch to [rich][rich] and [textual][textual] instead of the current curses TUI.
-This will open up some great possibilities for a much more modern UI.
-
-However, this change will require some *major* refactoring including breaking changes of the API
-and some of the user configuration options. It will also be a rather drastic change in style.
-Thus, I will attempt to support v3.5 with bugfix releases until 1.1.2023
-
-It will likely take a few months until v4.0 gets released but I am starting development on it now.
-You can follow the progress here: <https://gitlab.com/mrossinek/cobib/-/issues/78>
-
-[rich]: https://github.com/Textualize/rich
-[textual]: https://github.com/Textualize/textual
-
 ## Installation
 
 For all common purposes you can install coBib via `pip`:
 
 ```
 pip install cobib
 ```
 
 Note: Use `pip3` if you still have Python 2 installed.
 
 If you would also like to install the man-page and (crude!) Zsh completion,
 you need to download the source code and do the following:
 
 ```
-git clone https://gitlab.com/mrossinek/cobib
+git clone https://gitlab.com/cobib/cobib
 cd cobib
 make install_extras
 ```
 
 ### Arch Linux
 
 coBib is packaged in the AUR.
 * [cobib](https://aur.archlinux.org/packages/cobib/)
 * [cobib-git](https://aur.archlinux.org/packages/cobib-git/)
 
 ### Windows
 
-Windows is **only partially** supported!
-This is due to the fact that [Python under Windows does not ship with the `curses` module][1].
-Thus, you cannot run coBib's _TUI_ on Windows.
-However, if you are using Windows 10 you should be able to install and use coBib's full
-functionality within the Linux subsystem.
+coBib _should_ mostly work on Windows as is, but it is not being tested so no guarantees are given.
+If you are using Windows 10 or later and are running into issues, you should be able to install and
+use coBib's full functionality within the Linux subsystem.
 
 
 ## Getting started
 
 To get started, you must initialize the database:
 
 ```
@@ -141,15 +130,15 @@
 cobib add --isbn <some ISBN>
 ```
 
 **Note**: when adding data from a `.bib` file, make sure that it is in the Bib**La**Tex format!
 
 ### Viewing your database and entries
 
-You can view the contents of your database with (see also `cobib.commands.list`):
+You can view the contents of your database with (see also `cobib.commands.list_`):
 
 ```
 cobib list
 ```
 
 You can show a specific entry with (see also `cobib.commands.show`):
 
@@ -221,26 +210,33 @@
 
 ```
 man cobib
 ```
 
 ### TUI
 
-Finally, you can also use coBib's TUI for a more interactive experience (see also `cobib.tui`), by
-simply typing
-
+Finally, you can also use coBib's TUI for a more interactive experience (see also `cobib.ui.tui`),
+by simply typing
 ```
 cobib
 ```
 
+Here is an example screenshot of the TUI when listing the entires in your database:
+
+![coBib TUI List](https://gitlab.com/cobib/cobib/-/raw/master/html/cobib_tui_list.svg)
+
+And here is an example screenshot for listing search results:
+
+![coBib TUI Search](https://gitlab.com/cobib/cobib/-/raw/master/html/cobib_tui_search.svg)
+
 
 ## Configuration
 
 You can overwrite the default configuration by placing a `config.py` file in `~/.config/cobib/`.
-The easiest way to get started with this file is by copying [`example.py`](https://gitlab.com/mrossinek/cobib/-/blob/master/src/cobib/config/example.py)
+The easiest way to get started with this file is by copying [`example.py`](https://gitlab.com/cobib/cobib/-/blob/master/src/cobib/config/example.py)
 or by using:
 
 ```
 cobib _example_config > ~/.config/cobib/config.py
 ```
 
 You can then modify it to your liking.
@@ -249,23 +245,23 @@
 You can also disable loading of _any_ configuration file be setting this environment variable to one of the following values: `"", 0, "f", "false", "nil", "none"`.
 
 Finally, be sure to take a look at the man page (`man cobib`) and/or the online documentation for more information.
 
 
 ## Documentation
 
-coBib's documentation is hosted [here](https://mrossinek.gitlab.io/cobib/cobib.html).
+coBib's documentation is hosted [here](https://cobib.gitlab.io/cobib/cobib.html).
 
 If you would like to generate a local version during development, you need to clone the source code, and install [`pdoc`](https://github.com/mitmproxy/pdoc) in order to generate it:
 
 ```
-git clone https://gitlab.com/mrossinek/cobib.git
+git clone https://gitlab.com/cobib/cobib.git
 cd cobib
 pip install pdoc
-pdoc -d google -e cobib=https://gitlab.com/mrossinek/cobib/-/blob/master/src/cobib/ -t html -o docs src/cobib tests
+pdoc -d google -e cobib=https://gitlab.com/cobib/cobib/-/blob/master/src/cobib/ -t html -o docs src/cobib tests
 ```
 
 You can then browse the documentation from `docs/cobib.html`.
 
 
 ## History
 
@@ -273,35 +269,93 @@
 which has more features than I use on a regular basis and does not allow me to work from the command line which is where I spent most of the time that I spent on the computer.
 
 Hence, I have decided to make it my own task of implementing a simple, yet fast, reference manager.
 coBib is written in Python and uses a YAML file to store its bibliography in a plain text format.
 
 ### Changelog
 
-You can find the detailed changes throughout coBib's history in [the Changelog](https://gitlab.com/mrossinek/cobib/-/blob/master/CHANGELOG.md).
+You can find the detailed changes throughout coBib's history in [the Changelog](https://gitlab.com/cobib/cobib/-/blob/master/CHANGELOG.md).
 
 
 ## License
 
-coBib is licensed under the [MIT License](https://gitlab.com/mrossinek/cobib/-/blob/master/LICENSE.txt).
+coBib is licensed under the [MIT License](https://gitlab.com/cobib/cobib/-/blob/master/LICENSE.txt).
 
-[^1]: References like this one get interpreted by the documentation generator. If you are reading this as the README page, you may find the [online documentation](https://mrossinek.gitlab.io/cobib/cobib.html) more enjoyable.
-
-[1]: https://docs.python.org/3/howto/curses.html#what-is-curses
+[^1]: References like this one get interpreted by the documentation generator. If you are reading this as the README page, you may find the [online documentation](https://cobib.gitlab.io/cobib/cobib.html) more enjoyable.
 
 [//]: # ( vim: set ft=markdown: )
 
 # Changelog
 All notable changes to this project will be documented in this file.
 
-The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
+The format is based on [Keep a Changelog](https://keepachangelog.com/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+
+## [4.0.0] - 2023-05-20
+
+Pypi: https://pypi.org/project/cobib/3.5.5/
+
+### **Breaking Changes**
+- Configuration settings can no longer be set by item access and instead must
+  use attribute syntax. For example you need to change:
+  ```python
+  config["database"]["git"] = True
+  ```
+  to
+  ```python
+  config.database.git = True
+  ```
+  - the `config.commands.list` section had to be renamed to `config.commands.list_`
+  - the `config.tui` section has been entirely removed
+- The `cobib.commands.list` module was moved to `cobib.commands.list_`.
+- The function signature of all command- and importer-related events has changed!
+  For more details please refer to the
+  [online documentation](https://cobib.gitlab.io/cobib/cobib/config/event.html).
+
+### Added
+- Python 3.11 is now officially tested and supported
+- Full rewrite of all commands to use `rich` for a nicer CLI (#78,!51)
+- Full rewrite of the TUI based on `textual` (#78,!51)
+- the `--disambiguation` argument of the `add` command (#99,!58)
+- the `--ignore-case` argument of the `list` command (#105)
+  - this also comes with the new `config.commands.list_.ignore_case` setting
+- the `search` command now accepts multiple query strings at once which will be
+  searched over independently (#106)
+
+### Changed
+- the new default value of `config.parsers.yaml.use_c_lib_yaml` is now `True` as announced in version [3.4.0]
+- refactored the entire config as a dataclass (!63)
+  - this implies that settings can only be set via attributes
+  - but as a benefit the maintainability and documentation have improved significantly
+- The function signature of all command-related events has changed! Please refer to the
+  [online documentation](https://cobib.gitlab.io/cobib/cobib/config/event.html)
+  for more details. (!63)
+- The function signature of all importer-related events has changed! Please refer to the
+  [online documentation](https://cobib.gitlab.io/cobib/cobib/config/event.html)
+  for more details. (!66)
+- the API of the `cobib.commands` and `cobib.importers` module has been improved (!64)
+  - this should not have any end-user facing effects
+- the `cobib.commands.list` module was moved to `cobib.commands.list_`
+
+### Deprecated
+- the `--update` argument of the `add` command is deprecated in favor of `--disambiguation update`
+- the `--skip-existing` argument of the `add` command is deprecated in favor of `--disambiguation keep`
+
+### Fixed
+- the detection whether an entry already exists broke when label disambiguation was added in [3.3.0]
+  and is now fixed by means of an interactive prompt during the `add` command
+
+### Removed
+- the warning triggered upon setting `config.database.format.month` which got removed in [3.1.0]
+- Python 3.7 is no longer supported
+
+
 ## [3.5.5] - 2023-04-11
 
 Pypi: https://pypi.org/project/cobib/3.5.5/
 
 ### Fixed
 - opening of non-list type fields (#100)
 
@@ -349,15 +403,15 @@
 This will open up some great possibilities for a much more modern UI.
 
 However, this change will require some *major* refactoring including breaking changes of the API
 and some of the user configuration options. It will also be a rather drastic change in style.
 Thus, I will attempt to support v3.5 with bugfix releases until 1.1.2023
 
 It will likely take a few months until v4.0 gets released but I am starting development on it now.
-You can follow the progress here: <https://gitlab.com/mrossinek/cobib/-/issues/78>
+You can follow the progress here: <https://gitlab.com/cobib/cobib/-/issues/78>
 
 [rich]: https://github.com/Textualize/rich
 [textual]: https://github.com/Textualize/textual
 
 ### Added
 - the configuration loading can be disabled via the environment variable `COBIB_CONFIG`
     - values which disable the loading entirely are: `"", 0, f, false, nil, none`
@@ -435,15 +489,15 @@
 * the `config.database.format.label_default` and `config.database.format.label_suffix` options (#85,!45)
     - labels will automatically be formatted according to the default option
     - if labels conflict with existing ones, the suffix option will be used for disambiguation
     - the `AddCommand` has a new `--skip-existing` option which disables automatic label disambiguation
     - use `cobib _unify_labels --apply` to unify all labels in your database
 - subscribable events (#71,!46)
     - allows registering of hooks to be executed in certain situation
-    - more information is provided at the [online documentation](https://mrossinek.gitlab.io/cobib/cobib/config/event.html)
+    - more information is provided at the [online documentation](https://cobib.gitlab.io/cobib/cobib/config/event.html)
 
 ### Changed
 - when an unknown variable is encountered in the modification of the `modify` command it falls back to an empty string rather than the name of the attempted variable
 
 ### Removed
 - the `-s` option of the `AddCommand` is no longer available. You need to write out `--skip-download`
 - the `ID` filter argument on the `list` command (deprecated in v3.2.0 in favor of the `label` filter)
@@ -534,15 +588,15 @@
 ## [3.0.0] - 2021-04-10
 
 Pypi: https://pypi.org/project/cobib/3.0.0/
 
 - From now on, `coBib` is the official way of spelling!
 
 ### Added
-- coBib's documentation is now generated by [`pdoc`](https://pdoc.dev/) and hosted at https://mrossinek.gitlab.io/cobib/cobib.html
+- coBib's documentation is now generated by [`pdoc`](https://pdoc.dev/) and hosted at https://cobib.gitlab.io/cobib/cobib.html
 - (DEV): the `cobib.database.Database`-Singleton has been added to centrally manage the bibliographic runtime data (!28)
 - the new option `config.database.format.suppress_latex_warnings`
 - the new option `config.commands.edit.editor` which takes precedence over the `$EDITOR` variable
 
 ### Changed
 - the `INI`-style configuration is replaced with a `Python`-based configuration (#54,!25)
     - for guidance on how to migrate an existing configuration please read https://mrossinek.gitlab.io/programming/cobibs-new-configuration/
@@ -938,51 +992,52 @@
 
 ## [0.1] - 2019-04-29
 
 ### Added
 - initial version with a basic `sqlite3`-based database
 
 
-[Unreleased]: https://gitlab.com/mrossinek/cobib/-/compare/v3.5.5...master
-[3.5.5]: https://gitlab.com/mrossinek/cobib/-/compare/v3.5.5
-[3.5.4]: https://gitlab.com/mrossinek/cobib/-/compare/v3.5.4
-[3.5.3]: https://gitlab.com/mrossinek/cobib/-/compare/v3.5.3
-[3.5.2]: https://gitlab.com/mrossinek/cobib/-/compare/v3.5.2
-[3.5.1]: https://gitlab.com/mrossinek/cobib/-/compare/v3.5.1
-[3.5.0]: https://gitlab.com/mrossinek/cobib/-/compare/v3.5.0
-[3.4.0]: https://gitlab.com/mrossinek/cobib/-/compare/v3.4.0
-[3.3.2]: https://gitlab.com/mrossinek/cobib/-/compare/v3.3.2
-[3.3.1]: https://gitlab.com/mrossinek/cobib/-/compare/v3.3.1
-[3.3.0]: https://gitlab.com/mrossinek/cobib/-/compare/v3.3.0
-[3.2.1]: https://gitlab.com/mrossinek/cobib/-/compare/v3.2.1
-[3.2.0]: https://gitlab.com/mrossinek/cobib/-/compare/v3.2.0
-[3.1.1]: https://gitlab.com/mrossinek/cobib/-/compare/v3.1.1
-[3.1.0]: https://gitlab.com/mrossinek/cobib/-/compare/v3.1.0
-[3.0.0]: https://gitlab.com/mrossinek/cobib/-/compare/v3.0.0
-[2.6.1]: https://gitlab.com/mrossinek/cobib/-/compare/v2.6.1
-[2.6.0]: https://gitlab.com/mrossinek/cobib/-/tags/v2.6.0
-[2.5.0]: https://gitlab.com/mrossinek/cobib/-/tags/v2.5.0
-[2.4.1]: https://gitlab.com/mrossinek/cobib/-/tags/v2.4.1
-[2.4.0]: https://gitlab.com/mrossinek/cobib/-/tags/v2.4.0
-[2.3.4]: https://gitlab.com/mrossinek/cobib/-/tags/v2.3.4
-[2.3.3]: https://gitlab.com/mrossinek/cobib/-/tags/v2.3.3
-[2.3.2]: https://gitlab.com/mrossinek/cobib/-/tags/v2.3.2
-[2.3.1]: https://gitlab.com/mrossinek/cobib/-/tags/v2.3.1
-[2.3.0]: https://gitlab.com/mrossinek/cobib/-/tags/v2.3.0
-[2.2.2]: https://gitlab.com/mrossinek/cobib/-/tags/v2.2.2
-[2.2.1]: https://gitlab.com/mrossinek/cobib/-/tags/v2.2.1
-[2.2.0]: https://gitlab.com/mrossinek/cobib/-/tags/v2.2.0
-[2.1.0]: https://gitlab.com/mrossinek/cobib/-/tags/v2.1.0
-[2.0.0]: https://gitlab.com/mrossinek/cobib/-/tags/v2.0.0
-[2.0.0b4]: https://gitlab.com/mrossinek/cobib/-/tags/v2.0.0b4
-[2.0.0b3]: https://gitlab.com/mrossinek/cobib/-/tags/v2.0.0b3
-[2.0.0b2]: https://gitlab.com/mrossinek/cobib/-/tags/v2.0.0b2
-[2.0.0b1]: https://gitlab.com/mrossinek/cobib/-/tags/v2.0.0b1
-[2.0.0b0]: https://gitlab.com/mrossinek/cobib/-/tags/v2.0.0b0
-[2.0.0a2]: https://gitlab.com/mrossinek/cobib/-/tags/v2.0.0a2
-[2.0.0a1]: https://gitlab.com/mrossinek/cobib/-/tags/v2.0.0a1
-[1.1.0]: https://gitlab.com/mrossinek/cobib/-/tags/v1.1.0
-[1.0.2]: https://gitlab.com/mrossinek/cobib/-/tags/v1.0.2
-[1.0.1]: https://gitlab.com/mrossinek/cobib/-/tags/v1.0.1
-[1.0.0]: https://gitlab.com/mrossinek/cobib/-/tags/v1.0.0
-[0.2]: https://gitlab.com/mrossinek/cobib/-/tags/v0.2
-[0.1]: https://gitlab.com/mrossinek/cobib/-/tags/v0.1
+[Unreleased]: https://gitlab.com/cobib/cobib/-/compare/v4.0.0...master
+[4.0.0]: https://gitlab.com/cobib/cobib/-/compare/v4.0.0
+[3.5.5]: https://gitlab.com/cobib/cobib/-/compare/v3.5.5
+[3.5.4]: https://gitlab.com/cobib/cobib/-/compare/v3.5.4
+[3.5.3]: https://gitlab.com/cobib/cobib/-/compare/v3.5.3
+[3.5.2]: https://gitlab.com/cobib/cobib/-/compare/v3.5.2
+[3.5.1]: https://gitlab.com/cobib/cobib/-/compare/v3.5.1
+[3.5.0]: https://gitlab.com/cobib/cobib/-/compare/v3.5.0
+[3.4.0]: https://gitlab.com/cobib/cobib/-/compare/v3.4.0
+[3.3.2]: https://gitlab.com/cobib/cobib/-/compare/v3.3.2
+[3.3.1]: https://gitlab.com/cobib/cobib/-/compare/v3.3.1
+[3.3.0]: https://gitlab.com/cobib/cobib/-/compare/v3.3.0
+[3.2.1]: https://gitlab.com/cobib/cobib/-/compare/v3.2.1
+[3.2.0]: https://gitlab.com/cobib/cobib/-/compare/v3.2.0
+[3.1.1]: https://gitlab.com/cobib/cobib/-/compare/v3.1.1
+[3.1.0]: https://gitlab.com/cobib/cobib/-/compare/v3.1.0
+[3.0.0]: https://gitlab.com/cobib/cobib/-/compare/v3.0.0
+[2.6.1]: https://gitlab.com/cobib/cobib/-/compare/v2.6.1
+[2.6.0]: https://gitlab.com/cobib/cobib/-/tags/v2.6.0
+[2.5.0]: https://gitlab.com/cobib/cobib/-/tags/v2.5.0
+[2.4.1]: https://gitlab.com/cobib/cobib/-/tags/v2.4.1
+[2.4.0]: https://gitlab.com/cobib/cobib/-/tags/v2.4.0
+[2.3.4]: https://gitlab.com/cobib/cobib/-/tags/v2.3.4
+[2.3.3]: https://gitlab.com/cobib/cobib/-/tags/v2.3.3
+[2.3.2]: https://gitlab.com/cobib/cobib/-/tags/v2.3.2
+[2.3.1]: https://gitlab.com/cobib/cobib/-/tags/v2.3.1
+[2.3.0]: https://gitlab.com/cobib/cobib/-/tags/v2.3.0
+[2.2.2]: https://gitlab.com/cobib/cobib/-/tags/v2.2.2
+[2.2.1]: https://gitlab.com/cobib/cobib/-/tags/v2.2.1
+[2.2.0]: https://gitlab.com/cobib/cobib/-/tags/v2.2.0
+[2.1.0]: https://gitlab.com/cobib/cobib/-/tags/v2.1.0
+[2.0.0]: https://gitlab.com/cobib/cobib/-/tags/v2.0.0
+[2.0.0b4]: https://gitlab.com/cobib/cobib/-/tags/v2.0.0b4
+[2.0.0b3]: https://gitlab.com/cobib/cobib/-/tags/v2.0.0b3
+[2.0.0b2]: https://gitlab.com/cobib/cobib/-/tags/v2.0.0b2
+[2.0.0b1]: https://gitlab.com/cobib/cobib/-/tags/v2.0.0b1
+[2.0.0b0]: https://gitlab.com/cobib/cobib/-/tags/v2.0.0b0
+[2.0.0a2]: https://gitlab.com/cobib/cobib/-/tags/v2.0.0a2
+[2.0.0a1]: https://gitlab.com/cobib/cobib/-/tags/v2.0.0a1
+[1.1.0]: https://gitlab.com/cobib/cobib/-/tags/v1.1.0
+[1.0.2]: https://gitlab.com/cobib/cobib/-/tags/v1.0.2
+[1.0.1]: https://gitlab.com/cobib/cobib/-/tags/v1.0.1
+[1.0.0]: https://gitlab.com/cobib/cobib/-/tags/v1.0.0
+[0.2]: https://gitlab.com/cobib/cobib/-/tags/v0.2
+[0.1]: https://gitlab.com/cobib/cobib/-/tags/v0.1
```

### Comparing `cobib-3.5.5/README.md` & `cobib-4.0.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,74 +1,59 @@
-[![coBib](https://gitlab.com/mrossinek/cobib/-/raw/master/logo/cobib_logo.svg)](https://mrossinek.gitlab.io/cobib/cobib.html)
+[![coBib](https://gitlab.com/cobib/cobib/-/raw/master/logo/cobib_logo.svg)](https://cobib.gitlab.io/cobib/cobib.html)
 
 # coBib
 
-[![pipeline](https://gitlab.com/mrossinek/cobib/badges/master/pipeline.svg)](https://gitlab.com/mrossinek/cobib/-/pipelines)
-[![coverage](https://gitlab.com/mrossinek/cobib/badges/master/coverage.svg)](https://gitlab.com/mrossinek/cobib/-/graphs/master/charts)
+[![pipeline](https://gitlab.com/cobib/cobib/badges/master/pipeline.svg)](https://gitlab.com/cobib/cobib/-/pipelines)
+[![coverage](https://gitlab.com/cobib/cobib/badges/master/coverage.svg)](https://gitlab.com/cobib/cobib/-/graphs/master/charts)
 [![PyPI](https://img.shields.io/pypi/v/cobib)](https://pypi.org/project/cobib/)
 
 coBib is a simple, command-line based bibliography management tool.
 It is the result of the need for an easy-to-use alternative to full-blown reference managers like Mendeley or Zotero.
 As such it follows some basic design goals:
 
 * **plain-text database**: which means you get full access and control over the database.
 * **git-integration**: as a benefit of the above, you can keep track of your database through version control.
 * **centralized database, location-independent library**: this means, that coBib *only* manages the
   database file in a centralized fashion but allows you to spread the actual contents of your
   library across the entire file system (this is the major different to
   [papis](https://papis.readthedocs.io/en/latest/library_structure.html)).
-* **command-line and TUI support**: all features are available through the command-line as well as a curses-based TUI.
+* **command-line and TUI support**: all features are available through the command-line as well as a
+  [textual](https://textual.textualize.io/)-based TUI
 
 
-### **News:** coBib v4.0 will come with a new UI!
-The plan is to switch to [rich][rich] and [textual][textual] instead of the current curses TUI.
-This will open up some great possibilities for a much more modern UI.
-
-However, this change will require some *major* refactoring including breaking changes of the API
-and some of the user configuration options. It will also be a rather drastic change in style.
-Thus, I will attempt to support v3.5 with bugfix releases until 1.1.2023
-
-It will likely take a few months until v4.0 gets released but I am starting development on it now.
-You can follow the progress here: <https://gitlab.com/mrossinek/cobib/-/issues/78>
-
-[rich]: https://github.com/Textualize/rich
-[textual]: https://github.com/Textualize/textual
-
 ## Installation
 
 For all common purposes you can install coBib via `pip`:
 
 ```
 pip install cobib
 ```
 
 Note: Use `pip3` if you still have Python 2 installed.
 
 If you would also like to install the man-page and (crude!) Zsh completion,
 you need to download the source code and do the following:
 
 ```
-git clone https://gitlab.com/mrossinek/cobib
+git clone https://gitlab.com/cobib/cobib
 cd cobib
 make install_extras
 ```
 
 ### Arch Linux
 
 coBib is packaged in the AUR.
 * [cobib](https://aur.archlinux.org/packages/cobib/)
 * [cobib-git](https://aur.archlinux.org/packages/cobib-git/)
 
 ### Windows
 
-Windows is **only partially** supported!
-This is due to the fact that [Python under Windows does not ship with the `curses` module][1].
-Thus, you cannot run coBib's _TUI_ on Windows.
-However, if you are using Windows 10 you should be able to install and use coBib's full
-functionality within the Linux subsystem.
+coBib _should_ mostly work on Windows as is, but it is not being tested so no guarantees are given.
+If you are using Windows 10 or later and are running into issues, you should be able to install and
+use coBib's full functionality within the Linux subsystem.
 
 
 ## Getting started
 
 To get started, you must initialize the database:
 
 ```
@@ -120,15 +105,15 @@
 cobib add --isbn <some ISBN>
 ```
 
 **Note**: when adding data from a `.bib` file, make sure that it is in the Bib**La**Tex format!
 
 ### Viewing your database and entries
 
-You can view the contents of your database with (see also `cobib.commands.list`):
+You can view the contents of your database with (see also `cobib.commands.list_`):
 
 ```
 cobib list
 ```
 
 You can show a specific entry with (see also `cobib.commands.show`):
 
@@ -200,26 +185,33 @@
 
 ```
 man cobib
 ```
 
 ### TUI
 
-Finally, you can also use coBib's TUI for a more interactive experience (see also `cobib.tui`), by
-simply typing
-
+Finally, you can also use coBib's TUI for a more interactive experience (see also `cobib.ui.tui`),
+by simply typing
 ```
 cobib
 ```
 
+Here is an example screenshot of the TUI when listing the entires in your database:
+
+![coBib TUI List](https://gitlab.com/cobib/cobib/-/raw/master/html/cobib_tui_list.svg)
+
+And here is an example screenshot for listing search results:
+
+![coBib TUI Search](https://gitlab.com/cobib/cobib/-/raw/master/html/cobib_tui_search.svg)
+
 
 ## Configuration
 
 You can overwrite the default configuration by placing a `config.py` file in `~/.config/cobib/`.
-The easiest way to get started with this file is by copying [`example.py`](https://gitlab.com/mrossinek/cobib/-/blob/master/src/cobib/config/example.py)
+The easiest way to get started with this file is by copying [`example.py`](https://gitlab.com/cobib/cobib/-/blob/master/src/cobib/config/example.py)
 or by using:
 
 ```
 cobib _example_config > ~/.config/cobib/config.py
 ```
 
 You can then modify it to your liking.
@@ -228,23 +220,23 @@
 You can also disable loading of _any_ configuration file be setting this environment variable to one of the following values: `"", 0, "f", "false", "nil", "none"`.
 
 Finally, be sure to take a look at the man page (`man cobib`) and/or the online documentation for more information.
 
 
 ## Documentation
 
-coBib's documentation is hosted [here](https://mrossinek.gitlab.io/cobib/cobib.html).
+coBib's documentation is hosted [here](https://cobib.gitlab.io/cobib/cobib.html).
 
 If you would like to generate a local version during development, you need to clone the source code, and install [`pdoc`](https://github.com/mitmproxy/pdoc) in order to generate it:
 
 ```
-git clone https://gitlab.com/mrossinek/cobib.git
+git clone https://gitlab.com/cobib/cobib.git
 cd cobib
 pip install pdoc
-pdoc -d google -e cobib=https://gitlab.com/mrossinek/cobib/-/blob/master/src/cobib/ -t html -o docs src/cobib tests
+pdoc -d google -e cobib=https://gitlab.com/cobib/cobib/-/blob/master/src/cobib/ -t html -o docs src/cobib tests
 ```
 
 You can then browse the documentation from `docs/cobib.html`.
 
 
 ## History
 
@@ -252,19 +244,17 @@
 which has more features than I use on a regular basis and does not allow me to work from the command line which is where I spent most of the time that I spent on the computer.
 
 Hence, I have decided to make it my own task of implementing a simple, yet fast, reference manager.
 coBib is written in Python and uses a YAML file to store its bibliography in a plain text format.
 
 ### Changelog
 
-You can find the detailed changes throughout coBib's history in [the Changelog](https://gitlab.com/mrossinek/cobib/-/blob/master/CHANGELOG.md).
+You can find the detailed changes throughout coBib's history in [the Changelog](https://gitlab.com/cobib/cobib/-/blob/master/CHANGELOG.md).
 
 
 ## License
 
-coBib is licensed under the [MIT License](https://gitlab.com/mrossinek/cobib/-/blob/master/LICENSE.txt).
-
-[^1]: References like this one get interpreted by the documentation generator. If you are reading this as the README page, you may find the [online documentation](https://mrossinek.gitlab.io/cobib/cobib.html) more enjoyable.
+coBib is licensed under the [MIT License](https://gitlab.com/cobib/cobib/-/blob/master/LICENSE.txt).
 
-[1]: https://docs.python.org/3/howto/curses.html#what-is-curses
+[^1]: References like this one get interpreted by the documentation generator. If you are reading this as the README page, you may find the [online documentation](https://cobib.gitlab.io/cobib/cobib.html) more enjoyable.
 
 [//]: # ( vim: set ft=markdown: )
```

### Comparing `cobib-3.5.5/_cobib` & `cobib-4.0.0/_cobib`

 * *Files identical despite different names*

### Comparing `cobib-3.5.5/cobib.1` & `cobib-4.0.0/cobib.1`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH COBIB 1 2023-04-11 v3.5.5
+.TH COBIB 1 2023-05-20 v4.0.0
 .SH NAME
 coBib \- Console-based Bibliography Management
 .SH SYNOPSIS
 .B cobib
 [\fB\-\-version\fR]
 [\fB\-h\fR|\fB\-\-help\fR]
 [\fB\-v\fR|\fB\-\-verbose\fR]
@@ -11,15 +11,15 @@
 .SH DESCRIPTION
 coBib is a console-based bibliography manager written in Python.
 It maintains a plain-text database of literature data in YAML format at
 \fI$HOME/.local/share/cobib/literature.yaml\fR.
 .PP
 coBib provides a variety of \fBSUBCOMMANDS\fR through which you may
 investigate and manage the database.
-For easy of use it also comes with a curses-based \fBTUI\fR which is
+For easy of use it also comes with a textual-based \fBTUI\fR which is
 automatically started when no other subcommand is found (more information is
 provided in that section).
 .PP
 coBib also provides some "meta"-commands. These are expained in the \fBSHELL
 UTILITIES\fR section.
 .SH OPTIONS
 .TP
@@ -32,14 +32,18 @@
 .BR \-v ", " \-\-verbose
 Increases the verbosity level of the logging. This option may be provided up to
 two times (increasing the logging to \fIinfo\fR and \fIdebug\fR, respectively).
 By default, the verbosity of coBib's CLI is set to \fIwarning\fR but if the TUI
 is started, logging will be increased to \fIinfo\fR and redirected to
 \fIconfig.logging.logfile\fR.
 .TP
+.BR \-p ", " \-\-porcelain
+Switches the output that will be printed to the terminal to "porcelain" mode.
+This is meant to be useful for parsing and testing purposes.
+.TP
 .BR \-c ", " \-\-config " " \fI<path>\fR
 Run with an alternate configuration file at \fI<path>\fR.
 .TP
 .BR \-l ", " \-\-log " " \fI<path>\fR
 Run with an alternate log file at \fI<path>\fR.
 .SH SUBCOMMANDS
 All subcommands listed below also provide the \fI\-h\fR and \fI\-\-help\fR
@@ -94,41 +98,48 @@
 .PP
 .in +8n
 .BR \-l ", " \-\-label  " " \fI<label>\fR
 .in +4n
 Store the newly added entry under the specified \fIlabel\fR.
 .PP
 .in +8n
-.BR \-u ", " \-\-update
-.in +4n
-Updates an existing entry with the newly added data. Existing fields will be
-overwritten.
-.PP
-.in +8n
 .BR \-f ", " \-\-file " " \fI<path>\fR
 .in +4n
 Associate the newly added entry with the \fIfile\fR at the provided path.
 As of version 2.5 you can specify multiple files, too.
 .PP
 .in +8n
 .BR \-p ", " \-\-path " " \fI<path>\fR
 .in +4n
 Overwrites the location for the automatically downloaded file. If not specified,
 this setting defaults to \fIconfig.utils.file_downloader.default_location\fR.
 .PP
 .in +8n
-.BR \-\-skip\-download
+.BR \-\-disambiguation " " \fI<reply>\fR
 .in +4n
-Skips attempting to automatically download an associated file for the entry.
+Sets the reply for the interactive prompt if an addition needs to be
+disambiguated. The possible values for \fI<reply>\fR are the following:
+.in +4n
+.IR keep
+to keep the existing entry
+.in +0n
+.IR replace
+to replace the existing entry
+.in +0n
+.IR update
+to update the existing entry
+.in +0n
+.IR disambiguate
+to disambiguate the new label from the existing one by adding a label suffix
+(see also \fIconfig.database.format.label_suffix\fR)
 .PP
 .in +8n
-.BR \-\-skip\-existing
+.BR \-\-skip\-download
 .in +4n
-Skips entry addition if the label already exists instead of using label
-disambiguation to find a new label.
+Skips attempting to automatically download an associated file for the entry.
 .TP
 .B cobib delete \fI<label>\fR
 Deletes the entry with the given \fIlabel\fR.
 .PP
 .in +8n
 .BR \-\-preserve\-files
 .in +4n
@@ -244,22 +255,27 @@
 .PP
 .in +8n
 .BR \-r ", " \-\-reverse
 .in +4n
 Reverses the sorting order.
 .PP
 .in +8n
+.BR \-i ", " \-\-ignore-case
+.in +4n
+Makes the entry matching case-insensitive.
+.PP
+.in +8n
 .BR \-x ", " \-\-or
 .in +4n
 Concatenate the filters using logical \fIOR\fR rather than the default
 \fIAND\fR.
 .TP
 .B cobib search \fI<args>\fR ...
 Searches the database recursively (i.e. including any associated files) for the
-specified keyword.
+specified keywords (if multiple are given, these will be search independently).
 The positional arguments may be used to provide \fBFILTERS\fR which the entries
 must match in order to be included in the export.
 Additionally, the following \fI<args>\fR are also allowed:
 .PP
 .in +8n
 .BR \-c ", " \-\-context " " \fI<int>\fI
 .in +4n
@@ -382,79 +398,85 @@
 .TP
 .B cobib list ++year 2019 ++tags quantum
 Lists only entries with the `quantum` tag from the year 2019.
 .TP
 .B cobib list -x ++year 2019 ++year 2020
 Lists only entries published in 2019 or 2020.
 .SH TUI
-The curses-based TUI is started automatically when no other subcommand is
+The textual-based TUI is started automatically when no other subcommand is
 supplied, i.e. by simply running \fBcobib\fR.
-By default, it lists all entries of the database in a buffer which may be
-scrolled in vim-fashion with \fIh,j,k,l,^B,^U,^D,^F\fR.
-The arrow and paging keys are also available for scrolling.
-The following default key bindings are available:
+By default, it lists all entries of the database in a scrollable view and
+displays the bibtex-representation of the entry under the cursor in a side
+panel. You can scroll using vim-like keybindings \fIh,j,k,l\fR or the arrow
+keys.
+The following key bindings are available:
 .TP
 .BR q " " quit
-Quits one level of the viewing buffer.
+Quits the TUI.
 .TP
 .BR ? " " help
 Opens a small window providing help for the key bindings.
 .TP
-.BR ENTER " " show
-Populates the viewing buffer with a BibLaTex view of the selected entry.
+.BR _ " " layout
+Toggles between a horizontally and vertically split layout.
 .TP
-.BR o " " open
-Opens the current (or \fIselected\fR) label(s).
+.BR SPACE " " folds
+When displaying search results, toggles the visibility of any tree node.
+.TP
+.BR : " " prompt
+Opens a command prompt allowing the user to execute an arbitrary coBib CLI
+command.
+.TP
+.BR v " " select
+Adds the current label to the \fIselection\fR.
 .TP
-.BR w " " wrap
-Toggles wrapping of the viewing buffer.
+.BR / " " search
+Opens a search prompt and views the results in an interactive tree structure.
 .TP
 .BR a " " add
 Opens a command prompt which allows running the \fBadd\fR command as if outside
 of the TUI.
 .TP
 .BR d " " delete
 Deletes the current (or \fIselected\fR) label(s).
 .TP
 .BR e " " edit
 Opens the current label in an external editor.
 .TP
+.BR f " " filter
+Allows adding filters to the list of displayed entries.
+.TP
+.BR i " " import
+Opens a command prompt which allows running the \fBimport\fR command as if
+outside of the TUI.
+.TP
 .BR m " " modify
 Opens a command prompt which allows running the \fBmodify\fR command as if
 outside of the TUI. If a \fIselection\fR is present, the \fI-s\fR argument will
 be set automatically.
 .TP
-.BR u " " undo
-Undoes the last auto-committed change to the database file.
-This requires the git-integration (since v2.6.0) to be enabled!
+.BR o " " open
+Opens the current (or \fIselected\fR) label(s).
 .TP
 .BR r " " redo
 Reapplies the last undone change.
 This requires the git-integration (since v2.6.0) to be enabled!
 .TP
-.BR / " " search
-Opens a search prompt and views the results in the viewing buffer.
-.TP
-.BR f " " filter
-Allows adding filters to the list view.
-.TP
 .BR s " " sort
 Allows sorting the list view.
 .TP
-.BR v " " select
-Adds the current label to the \fIselection\fR.
+.BR u " " undo
+Undoes the last auto-committed change to the database file.
+This requires the git-integration (since v2.6.0) to be enabled!
 .TP
 .BR x " " export
 Opens a command prompt which allows running the \fBexport\fR command as if
 outside of the TUI. If a \fIselection\fR is present, the \fI-s\fR argument will
 be set automatically.
-.TP
-.BR : " " prompt
-Opens a command prompt allowing the user to execute an arbitrary coBib CLI
-command.
+Opens a small window providing help for the key bindings.
 .SH CONFIGURATION
 Since version 3.0, coBib can be configured directly via \fIPython\fR. To do so,
 you must place the configuration file at \fI$HOME/.config/cobib/config.py\fR.
 If you don't have a configuration file yet, you can get started by copying the
 well-documented example configuration to the right location via:
 .in +4n
     \fIcobib _example_config > ~/.config/cobib/config.py\fR
@@ -468,35 +490,33 @@
 disable the loading of a configuration file entirely by setting it to one of the
 following values: \fI"", 0, "f", "false", "nil", "none"\fR.
 .PP
 The following section summarizes the syntax and all possibly settings, for
 completeness.
 .TP
 .BR Configuration " " Syntax
-Internally, coBib's configuration is nothing but a (nested) Python dictionary.
+Internally, coBib's configuration is nothing but a (nested) Python dataclass.
 Thus, after importing the config with
 .in +4n
     \fIfrom cobib.config import config\fR
 .in -4n
 it is very straight forward to change any setting by simply changing the value
-stored in the dictionary. For example:
-.in +4n
-    \fIconfig['database']['git'] = True\fR
-.in -4n
-However, for ease of use, all of the fields are also exposed as attributes. This
-means, the same can be achieved via:
+of an attribute. For example:
 .in +4n
     \fIconfig.database.git = True\fR
 .in -4n
 .PP
 .BR LOGGING
 .TP
+.IR config.logging.cache = '~/.cache/cobib/cache'
+This settings sets the path to the default cache file.
+.TP
 .IR config.logging.logfile = '~/.cache/cobib/cobib.log'
-This setting sets the path to the default logfile. This logfile can be
-overwritten using the \fI--logfile\fR command-line argument.
+This setting sets the path to the default logfile. This setting can be
+overwritten at runtime using the \fI--logfile\fR command-line argument.
 .TP
 .IR config.logging.version = '~/.cache/cobib/version'
 In this file, the last run version of coBib gets cached. After an update, coBib
 automtically prints the newest section of the Changelog. To disable this
 functionality entirely, set this option to \fINone\fR.
 .PP
 .BR COMMANDS
@@ -506,25 +526,43 @@
 entered entries.
 .TP
 .IR config.commands.edit.editor = $EDITOR " if available else " 'vim'
 This setting can be used to overwrite the external editor used for manual
 editing of database entries. It defaults to the environment variable
 \fI$EDITOR\fR and falls back to \fIvim\fR if that is not set either.
 .TP
+.IR config.commands.list_.default_columns = ['label',\ 'title']
+Specifies the default columns displayed during the \fIlist\fR command.
+.TP
+.IR config.commands.list_.ignore_case = False
+Specifies whether filter matching should be performed case-insensitive.
+.TP
 .IR config.commands.open.command = 'xdg-open' " (on Linux); " 'open' " (on Mac OS)"
 Specifies the program used to open associated files.
 .TP
+.IR config.commands.open.fields = ['file',\ 'url']
+Specifies the names of the data fields which are to be checked for openable
+URLs.
+.TP
 .IR config.commands.search.grep = 'grep'
 Specifies the program used to search in associated files.
 .TP
 .IR config.commands.search.grep_args = []
 Allows the specification of additional arguments for the \fIgrep\fR command.
 .TP
 .IR config.commands.search.ignore_case = False
 This boolean setting indicates whether search defaults to be case-insensitive.
+.TP
+.IR config.commands.search.highlights.label = 'blue'
+Specifies the color used to highlight the entry labels when displaying search
+rsults.
+.TP
+.IR config.commands.search.highlights.label = 'red'
+Specifies the color used to highlight the query matches when displaying search
+rsults.
 .PP
 .BR DATABASE
 .TP
 .IR config.database.file = '~/.local/share/cobib/literature.yaml'
 This setting sets the path to the database file. You can use \fI~\fR to
 represent your \fI$HOME\fR directory.
 .TP
@@ -565,125 +603,20 @@
 .PP
 .BR PARSERS
 .TP
 .IR config.parsers.bibtex.ignore_non_standard_types = False
 This boolean setting indicates whether non-standard BibLaTex entry types should
 be ignored or not.
 .TP
-.IR config.parsers.yaml.use_c_lib_yaml = False
+.IR config.parsers.yaml.use_c_lib_yaml = True
 This boolean setting indicates whether to use the C-based implementation of the
 YAML parser. For this to work, additional packages may need to be installed.
 Read https://yaml.readthedocs.io/en/latest/install.html#optional-requirements
 for more details.
 .PP
-.BR TUI
-.TP
-.IR config.tui.default_list_args = ['\-l']
-This can be set to a list of default arguments to use for the TUI's list view.
-.TP
-.IR config.tui.prompt_before_quit = True
-This setting specifies whether the user is prompted to verify the final quit
-operation.
-.TP
-.IR config.tui.reverse_order = True
-This setting specifies whether the database is listed in reverse order by
-default. This is useful because the most recently added entries will be at the
-top.
-.TP
-.IR config.tui.scroll_offset = 3
-This setting specifies the scrolling offset used to prevent the cursor line from
-coming too close to the ends of the screen while scrolling.  The intent of this
-setting is to provide a similar behavior as the 'scrolloff' option available in
-Vim. Note, that you can pin the cursor line to the center of the screen by
-setting this option to a very large value (e.g. 99).
-.PP
-.BR TUI.COLORS
-With the following settings you can change the look of the TUI. Each of these
-settings accepts any of the following color names: \fIblack\fR, \fIred\fR,
-\fIgreen\fR, \fIyellow\fR, \fIblue\fR, \fImagenta\fR, \fIcyan\fR and
-\fIwhite\fR.
-.TP
-.IR config.tui.colors.cursor_line_fg = 'white'
-.TP
-.IR config.tui.colors.cursor_line_bg = 'cyan'
-.TP
-.IR config.tui.colors.top_statusbar_fg = 'black'
-.TP
-.IR config.tui.colors.top_statusbar_bg = 'yellow'
-.TP
-.IR config.tui.colors.bottom_statusbar_fg = 'black'
-.TP
-.IR config.tui.colors.bottom_statusbar_bg = 'yellow'
-.TP
-.IR config.tui.colors.search_label_fg = 'blue'
-.TP
-.IR config.tui.colors.search_label_bg = 'black'
-.TP
-.IR config.tui.colors.search_query_fg = 'red'
-.TP
-.IR config.tui.colors.search_query_bg = 'black'
-.TP
-.IR config.tui.colors.popup_help_fg = 'white'
-.TP
-.IR config.tui.colors.popup_help_bg = 'green'
-.TP
-.IR config.tui.colors.popup_stdout_fg = 'white'
-.TP
-.IR config.tui.colors.popup_stdout_bg = 'blue'
-.TP
-.IR config.tui.colors.popup_stderr_fg = 'white'
-.TP
-.IR config.tui.colors.popup_stderr_bg = 'red'
-.TP
-.IR config.tui.colors.selection_fg = 'white'
-.TP
-.IR config.tui.colors.selection_bg = 'magenta'
-.PP
-.BR TUI.KEY_BINDINGS
-You can change the default key bindings of the TUI by overwriting any of the
-following settings with a different key. Any setting will interpret the provided
-string as a single character whose ASCII value is used for triggering the
-command.
-The only exception is the \fIENTER\fR string, which will be internally mapped to
-the ASCII codes 10 (\fIline feed\fR) and 13 (\fIcarriage return\fR).
-.TP
-.IR config.tui.key_bindings.prompt = ':'
-.TP
-.IR config.tui.key_bindings.search = '/'
-.TP
-.IR config.tui.key_bindings.help = '?'
-.TP
-.IR config.tui.key_bindings.add = 'a'
-.TP
-.IR config.tui.key_bindings.delete = 'd'
-.TP
-.IR config.tui.key_bindings.edit = 'e'
-.TP
-.IR config.tui.key_bindings.filter = 'f'
-.TP
-.IR config.tui.key_bindings.modify = 'm'
-.TP
-.IR config.tui.key_bindings.open = 'o'
-.TP
-.IR config.tui.key_bindings.quit = 'q'
-.TP
-.IR config.tui.key_bindings.redo = 'r'
-.TP
-.IR config.tui.key_bindings.sort = 's'
-.TP
-.IR config.tui.key_bindings.undo = 'u'
-.TP
-.IR config.tui.key_bindings.select = 'v'
-.TP
-.IR config.tui.key_bindings.wrap = 'w'
-.TP
-.IR config.tui.key_bindings.export = 'x'
-.TP
-.IR config.tui.key_bindings.show = 'ENTER'
-.PP
 .BR UTILS
 .TP
 .IR config.utils.file_downloader.default_location = '~/.local/share/cobib'
 This setting sets the default location for any downloaded associated files.
 .TP
 .IR config.utils.file_downloader.url_map = {}
 You can provide rules to map from a journal's landing page URL to its PDF URL.
@@ -707,15 +640,15 @@
 should include any necessary punctuation which can be excluded upon export (see
 also \fIcobib export --help\fR).
 .PP
 .BR EVENTS
 .TP
 Since v3.3.0 coBib comes with a number of subscribable events. Their
 configuration is detailed in the online documentation,
-https://mrossinek.gitlab.io/cobib/cobib/config/event.html, and will not be
+https://cobib.gitlab.io/cobib/cobib/config/event.html, and will not be
 repeated here.
 .PP
 .SH SHELL UTILITIES
 In addition to the \fISUBCOMMANDS\fR coBib also provides some "meta"-commands
 for varying purposes.
 .TP
 .B cobib _example_config
@@ -753,9 +686,9 @@
 The configuration file.
 .TP
 .IR $HOME/.local/share/cobib/literature.yaml
 The default location of the database file.
 .SH SEE ALSO
 The internal help documentation via the \fI\-\-help\fR arguments.
 .PP
-The source code and issue tracker at https://gitlab.com/mrossinek/cobib
+The source code and issue tracker at https://gitlab.com/cobib/cobib
 .\" vim: tw=80
```

### Comparing `cobib-3.5.5/html/cobib_book.svg` & `cobib-4.0.0/html/cobib_book.svg`

 * *Files identical despite different names*

### Comparing `cobib-3.5.5/html/cobib_logo.svg` & `cobib-4.0.0/html/cobib_logo.svg`

 * *Files identical despite different names*

### Comparing `cobib-3.5.5/html/index.html.jinja2` & `cobib-4.0.0/html/index.html.jinja2`

 * *Files 4% similar despite different names*

```diff
@@ -3,13 +3,13 @@
 {% block title %}coBib Documentation{% endblock %}
 
 {% block favicon %}
     <link rel="icon" type="image/svg+xml" href="data:image/svg+xml,{% filter urlencode %}{% include "cobib_book.svg" %}{% endfilter %}"/>
 {% endblock %}
 
 {% block logo %}
-    <a id="pdoc-logo" title="coBib" href="https://gitlab.com/mrossinek/cobib"></a>
+    <a id="pdoc-logo" title="coBib" href="https://gitlab.com/cobib/cobib"></a>
         <img src="data:image/svg+xml,{% filter urlencode %}{% include "cobib_logo.svg" %}{% endfilter %}" alt="coBib logo" width="600"/>
     </a>
 {% endblock %}
 
 <!-- vim: set ft=html: -->
```

### Comparing `cobib-3.5.5/logo/cobib_book-squared.png` & `cobib-4.0.0/logo/cobib_book-squared.png`

 * *Files identical despite different names*

### Comparing `cobib-3.5.5/logo/cobib_book.png` & `cobib-4.0.0/logo/cobib_book.png`

 * *Files identical despite different names*

### Comparing `cobib-3.5.5/logo/cobib_book.svg` & `cobib-4.0.0/logo/cobib_book.svg`

 * *Files identical despite different names*

### Comparing `cobib-3.5.5/logo/cobib_byline.png` & `cobib-4.0.0/logo/cobib_byline.png`

 * *Files identical despite different names*

### Comparing `cobib-3.5.5/logo/cobib_byline.svg` & `cobib-4.0.0/logo/cobib_byline.svg`

 * *Files identical despite different names*

### Comparing `cobib-3.5.5/logo/cobib_logo.png` & `cobib-4.0.0/logo/cobib_logo.png`

 * *Files identical despite different names*

### Comparing `cobib-3.5.5/logo/cobib_logo.svg` & `cobib-4.0.0/logo/cobib_logo.svg`

 * *Files identical despite different names*

### Comparing `cobib-3.5.5/src/cobib/commands/__init__.py` & `cobib-4.0.0/src/cobib/commands/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """coBib's commands.
 
 coBib provides a series of commands, all of which are available both, from the command-line as well
-as through the text user interface (see also `cobib.tui`).
+as through the text user interface (see also `cobib.ui.tui`).
 The abstract interface which should be implemented is defined by the `cobib.commands.base_command`.
 """
 
 from .add import AddCommand as AddCommand
 from .delete import DeleteCommand as DeleteCommand
 from .edit import EditCommand as EditCommand
 from .export import ExportCommand as ExportCommand
 from .import_ import ImportCommand as ImportCommand
 from .init import InitCommand as InitCommand
-from .list import ListCommand as ListCommand
+from .list_ import ListCommand as ListCommand
 from .modify import ModifyCommand as ModifyCommand
 from .open import OpenCommand as OpenCommand
 from .redo import RedoCommand as RedoCommand
 from .search import SearchCommand as SearchCommand
 from .show import ShowCommand as ShowCommand
 from .undo import UndoCommand as UndoCommand
```

### Comparing `cobib-3.5.5/src/cobib/commands/add.py` & `cobib-4.0.0/src/cobib/commands/add.py`

 * *Files 24% similar despite different names*

```diff
@@ -25,14 +25,26 @@
 Furthermore, most of these parsers will set the entry label automatically.
 If you would like to prevent that and specify a custom label directly, you can add the `--label`
 keyword argument to your command like so:
 ```
 cobib add --doi <some DOI> --label "MyLabel"
 ```
 
+.. note::
+   Since this command adds new entries to the database, its outcome can be affected by your
+   `cobib.config.config.DatabaseConfig` settings. In particular, pay attention to the
+   `cobib.config.config.EntryStringifyConfig` settings which affect how entries are converted
+   to/from strings. In particular, the following setting will affect how multiple files are split
+   into a list of files:
+   ```
+   config.database.stringify.list_separator.file = ", "
+   ```
+   The above will separate file paths using `, ` but if you use a different separator (for example
+   `;`) be sure to update this setting accordingly.
+
 ### 2. Manual entry addition
 
 If you want to add a new entry manually, you *must* omit any of the parser keyword arguments and
 instead specify a new label like so:
 ```
 cobib add --label <some new label>
 ```
@@ -51,143 +63,183 @@
 You can also specify `cobib.database.Entry.tags` using *positional* arguments like so:
 ```
 cobib add --doi <some DOI> -- tag1 "multi-word tag2" ...
 ```
 
 Since v3.2.0 coBib attempts to download PDF files for newly added entries (if the corresponding
 parser supports this feature). The default location where this file will be stored can be configured
-via `config.utils.file_downloader.default_location`, but it can be changed at runtime using the
-`--path` argument like so:
+via `cobib.config.config.FileDownloaderConfig.default_location`, but it can be changed at runtime
+using the `--path` argument like so:
 ```
 cobib add --path <some custom path> --arxiv <some arXiv ID>
 ```
 If you want to manually suppress the automatic download, specify the `--skip-download` argument:
 ```
 cobib add --skip-download --arxiv <some arXiv ID>
 ```
 
-Since v3.3.0 you can also update existing entries by using the `--update` argument:
+Since v4.0.0 coBib will ask you what to do when encountering a conflict at runtime. That means, when
+a label already exists in your database, you have various choices how to handle it:
+
+1. you can `keep` the existing entry and skip the addition of the new one.
+   .. note::
+      This is equivalent to the old `--skip-existing` argument (added in v3.3.0) which is now
+      deprecated and will be removed in a future version.
+
+2. you can `replace` the existing entry.
+
+3. you can `update` the existing entry.
+   ```
+   cobib add --doi <some DOI> --disambiguation update --label <some existing label>```
+
+   This will take the existing entry and combine it with all new information found in the freshly
+   added entry. Existing fields will be overwritten. If you have an automatically downloaded file
+   associated with this entry, that will also be overwritten.
+   This feature is especially useful if you want to update an entry which you previously added from
+   the arXiv with its newly published version.
+   .. note::
+      This is equivalent to the `--update` argument (added in v3.3.0) which is now deprecated and
+      will be removed in a future version.
+
+4. you can `disambiguate` the entries. This will be done based on the
+   `cobib.config.config.DatabaseFormatConfig.label_suffix` setting. It defaults to appending `_a`,
+   `_b`, etc. to the label in order to differentiate (disambiguate) it from the already existing
+   one.
+
+When running into such a case, coBib will generate a side-by-side comparison of the existing and new
+entry and give you the choice of how to proceed. The default choice is to *cancel* the addition
+(i.e. `keep`) in order to prevent data loss.
+
+If you already know that you will run into this case, you can bypass the prompt via the
+`--disambiguation` argument and provide the intended answer ahead of time, for example like so:
 ```
-cobib add --doi <some DOI> --update --label <some existing label>
+cobib add --doi <some DOI> --disambiguation replace --label <some existing label>
 ```
-This will take the existing entry and combine it with all new information found in the freshly added
-entry. Existing fields will be overwritten. If you have an automatically downloaded file associated
-with this entry, that will also be overwritten.
-This feature is especially useful if you want to update an entry which you previously added from the
-arXiv with its newly published version.
-
-If you don't specify `--update` and run into a situation where the label which you are trying to add
-already exists, coBib will disambiguate it based on the `config.database.format.label_suffix`
-setting. It defaults to appending `_a`, `_b`, etc.
-You can disable this disambiguation by passing `--skip-existing` to the add command.
 
 ### TUI
 
-You can also trigger this command from the `cobib.tui.tui.TUI`.
+You can also trigger this command from the `cobib.ui.tui.TUI`.
 By default, it is bound to the `a` key which will drop you into the prompt where you can type out a
 normal command-line command:
 ```
 :add <arguments go here>
 ```
 """
 
 from __future__ import annotations
 
 import argparse
+import asyncio
 import inspect
 import logging
-import sys
 from collections import OrderedDict
-from typing import IO, TYPE_CHECKING, Any, Dict, List
+from functools import wraps
+from typing import Callable, Dict, Tuple, Type, cast
+
+from rich.console import Console
+from rich.prompt import InvalidResponse, Prompt, PromptBase, PromptType
+from textual.app import App
+from textual.widget import AwaitMount, Widget
+from typing_extensions import override
 
 from cobib import parsers
 from cobib.config import Event, config
 from cobib.database import Database, Entry
+from cobib.parsers import BibtexParser
+from cobib.utils.diff_renderer import Differ
 from cobib.utils.file_downloader import FileDownloader
 from cobib.utils.journal_abbreviations import JournalAbbreviations
 
 from .base_command import ArgumentParser, Command
 from .edit import EditCommand
 from .modify import evaluate_as_f_string
 
 LOGGER = logging.getLogger(__name__)
 
-if TYPE_CHECKING:
-    import cobib.tui
-
 
 class AddCommand(Command):
-    """The Add Command."""
+    """The Add Command.
 
-    name = "add"
+    This command can parse the following arguments:
 
-    # pylint: disable=too-many-branches,too-many-statements
-    def execute(self, args: List[str], out: IO[Any] = sys.stdout) -> None:
-        """Adds a new entry.
-
-        Depending on the `args`, if a keyword for one of the available `cobib.parsers` was used
-        together with a matching input, that parser will be used to create the new entry.
-        Otherwise, the command is only valid if the `--label` option was used to specify a new entry
-        label, in which case this command will trigger the `cobib.commands.edit.EditCommand` for a
-        manual entry addition.
+        * `-l`, `--label`: the label to give to the new entry.
+        * `-d`, `--disambiguation`: hard-codes the reply to be used if a disambiguation prompt would
+          occur.
+        * `-f`, `--file`: one or multiple files to associate with this entry. This data will be
+          stored in the `cobib.database.Entry.file` property.
+        * `-p`, `--path`: the path to store the downloaded associated file in. This can be used to
+          overwrite the `cobib.config.config.FileDownloaderConfig.default_location`.
+        * `--skip-download`: skips the automatic download of an associated file.
+        * `--skip-existing`: **DEPRECATED** use `--disambiguation keep` instead!
+        * `-u`, `--update`: **DEPRECATED** use `--disambiguation update` instead!
+        * in addition to the options above, a *mutually exclusive group* of keyword arguments for
+          all available `cobib.parsers` are registered at runtime. Please check the output of
+          `cobib add --help` for the exact list.
+        * any *positional* arguments (i.e. those, not preceded by a keyword) are interpreted as tags
+          and will be stored in the `cobib.database.Entry.tags` property.
+    """
 
-        Args:
-            args: a sequence of additional arguments used for the execution. The following values
-                are allowed for this command:
-                    * `-l`, `--label`: the label to give to the new entry.
-                    * `-u`, `--update`: updates an existing database entry if it already exists.
-                    * `-f`, `--file`: one or multiple files to associate with this entry. This data
-                      will be stored in the `cobib.database.Entry.file` property.
-                    * `-p`, `--path`: the path to store the downloaded associated file in. This can
-                      be used to overwrite the `config.utils.file_downloader.default_location`.
-                    * `--skip-download`: skips the automatic download of an associated file.
-                    * `--skip-existing`: skips entry if label exists instead of running label
-                      disambiguation.
-                    * in addition to the options above, a *mutually exclusive group* of keyword
-                      arguments for all available `cobib.parsers` are registered at runtime. Please
-                      check the output of `cobib add --help` for the exact list.
-                    * any *positional* arguments (i.e. those, not preceded by a keyword) are
-                      interpreted as tags and will be stored in the `cobib.database.Entry.tags`
-                      property.
-            out: the output IO stream. This defaults to `sys.stdout`.
-        """
-        LOGGER.debug("Starting Add command.")
+    name = "add"
+
+    _avail_parsers = {
+        cls.name: cls for _, cls in inspect.getmembers(parsers) if inspect.isclass(cls)
+    }
+    """The available parsers."""
+
+    @override
+    def __init__(
+        self,
+        *args: str,
+        console: Console | App[None] | None = None,
+        prompt: Type[PromptBase[str]] | None = None,
+    ) -> None:
+        super().__init__(*args, console=console, prompt=prompt)
+
+        self.new_entries: Dict[str, Entry] = OrderedDict()
+        """An `OrderedDict` mapping labels to `cobib.database.Entry` instances which were added by
+        this command."""
+
+    @override
+    @classmethod
+    def init_argparser(cls) -> None:
         parser = ArgumentParser(prog="add", description="Add subcommand parser.")
         parser.add_argument("-l", "--label", type=str, help="the label for the new database entry")
         parser.add_argument(
-            "-u",
-            "--update",
-            action="store_true",
-            help="update an entry if the label exists already",
-        )
-        file_action = "extend" if sys.version_info[1] >= 8 else "append"
-        parser.add_argument(
             "-f",
             "--file",
             type=str,
             nargs="+",
-            action=file_action,
+            action="extend",
             help="files associated with this entry",
         )
-        parser.add_argument("-p", "--path", type=str, help="the path for the associated file")
+        parser.add_argument("-p", "--path", type=str, help="the path for the downloaded file")
+        parser.add_argument(
+            "--disambiguation",
+            type=str,
+            choices=["keep", "replace", "update", "disambiguate"],
+            help="the reply in case of a disambiguation prompt",
+        )
         parser.add_argument(
             "--skip-download",
             action="store_true",
             help="skip the automatic download of an associated file",
         )
         parser.add_argument(
             "--skip-existing",
             action="store_true",
-            help="skips entry addition if existent instead of using label disambiguation",
+            help="DEPRECATED: use '--disambiguation keep' instead!",
+        )
+        parser.add_argument(
+            "-u",
+            "--update",
+            action="store_true",
+            help="DEPRECATED: use '--disambiguation update' instead!",
         )
         group_add = parser.add_mutually_exclusive_group()
-        avail_parsers = {
-            cls.name: cls for _, cls in inspect.getmembers(parsers) if inspect.isclass(cls)
-        }
-        for name in avail_parsers.keys():
+        for name in cls._avail_parsers.keys():
             try:
                 group_add.add_argument(
                     f"-{name[0]}", f"--{name}", type=str, help=f"{name} object identfier"
                 )
             except argparse.ArgumentError:
                 try:
                     group_add.add_argument(f"--{name}", type=str, help=f"{name} object identfier")
@@ -195,146 +247,254 @@
                     continue
         parser.add_argument(
             "tags",
             nargs=argparse.REMAINDER,
             help="A list of space-separated tags to associate with this entry."
             "\nYou can use quotes to specify tags with spaces in them.",
         )
-        if not args:
-            parser.print_usage(sys.stderr)
-            sys.exit(1)
-
-        try:
-            largs = parser.parse_args(args)
-        except argparse.ArgumentError as exc:
-            LOGGER.error(exc.message)
-            return
 
-        Event.PreAddCommand.fire(largs)
+        cls.argparser = parser
 
-        new_entries: Dict[str, Entry] = OrderedDict()
+    @classmethod
+    def _parse_args(cls, args: tuple[str, ...]) -> argparse.Namespace:
+        largs = super()._parse_args(args)
+
+        if largs.skip_existing:
+            msg = (
+                "The '--skip-existing' argument of the 'add' command is deprecated! "
+                "Instead you should use '--disambiguation keep'."
+            )
+            LOGGER.warning(msg)
+            largs.disambiguation = "keep"
+
+        if largs.update:
+            msg = (
+                "The '--update' argument of the 'add' command is deprecated! "
+                "Instead you should use '--disambiguation update'."
+            )
+            LOGGER.warning(msg)
+            largs.disambiguation = "update"
+
+        return largs
+
+    # pylint: disable=invalid-overridden-method,too-many-statements,too-many-branches
+    @override
+    async def execute(self) -> None:  # type: ignore[override]
+        LOGGER.debug("Starting Add command.")
+
+        Event.PreAddCommand.fire(self)
 
         edit_entries = False
-        for name, cls in avail_parsers.items():
-            string = getattr(largs, name, None)
+        for name, cls in AddCommand._avail_parsers.items():
+            string = getattr(self.largs, name, None)
             if string is None:
                 continue
             LOGGER.debug("Adding entries from %s: '%s'.", name, string)
-            new_entries = cls().parse(string)
+            self.new_entries = cls().parse(string)
             break
         else:
-            if largs.label is not None:
-                LOGGER.warning("No input to parse. Creating new entry '%s' manually.", largs.label)
-                new_entries = {
-                    largs.label: Entry(
-                        largs.label,
+            if self.largs.label is not None:
+                LOGGER.warning(
+                    "No input to parse. Creating new entry '%s' manually.", self.largs.label
+                )
+                self.new_entries = {
+                    self.largs.label: Entry(
+                        self.largs.label,
                         {"ENTRYTYPE": config.commands.edit.default_entry_type},
                     )
                 }
                 edit_entries = True
             else:
                 msg = "Neither an input to parse nor a label for manual creation specified!"
                 LOGGER.error(msg)
                 return
 
-        if largs.label is not None:
-            assert len(new_entries.values()) == 1
-            for value in new_entries.values():
+        if self.largs.label is not None:
+            assert len(self.new_entries.values()) == 1
+            for value in self.new_entries.copy().values():
                 # logging done by cobib/database/entry.py
-                value.label = largs.label
-            new_entries = OrderedDict((largs.label, value) for value in new_entries.values())
+                value.label = self.largs.label
+            self.new_entries = OrderedDict(
+                (self.largs.label, value) for value in self.new_entries.values()
+            )
         else:
             formatted_entries = OrderedDict()
-            for label, value in new_entries.items():
+            for label, value in self.new_entries.items():
                 formatted_label = evaluate_as_f_string(
                     config.database.format.label_default, {"label": label, **value.data.copy()}
                 )
                 value.label = formatted_label
                 formatted_entries[formatted_label] = value
-            new_entries = formatted_entries
+            self.new_entries = formatted_entries
 
-        if largs.file is not None:
-            if file_action == "append":
-                # We need to flatten the potentially nested list.
-                # pylint: disable=import-outside-toplevel
-                from itertools import chain
-
-                largs.file = list(chain.from_iterable(largs.file))
-            assert len(new_entries.values()) == 1
-            for value in new_entries.values():
+        if self.largs.file is not None:
+            assert len(self.new_entries.values()) == 1
+            for value in self.new_entries.values():
                 # logging done by cobib/database/entry.py
-                value.file = largs.file
+                value.file = self.largs.file
 
-        if largs.tags != []:
-            assert len(new_entries.values()) == 1
-            for value in new_entries.values():
+        if self.largs.tags != []:
+            assert len(self.new_entries.values()) == 1
+            for value in self.new_entries.values():
                 # logging done by cobib/database/entry.py
-                value.tags = largs.tags
+                value.tags = self.largs.tags
 
         bib = Database()
         existing_labels = set(bib.keys())
 
-        for lbl, entry in new_entries.copy().items():
+        for lbl, entry in self.new_entries.copy().items():
+            overwrite_file = False
             # check if label already exists
             if lbl in existing_labels:
-                if not largs.update:
-                    msg = f"You tried to add a new entry '{lbl}' which already exists!"
+                # if it does, we have multiple cases to differentiate:
+                if edit_entries:
+                    # the user tried to manually add an entry which already exists, point them to
+                    # the edit command instead
+                    msg = (
+                        f"You tried to add the '{lbl}' entry manually, but it already exists, "
+                        f"please use `cobib edit {lbl}` instead!"
+                    )
                     LOGGER.warning(msg)
-                    if edit_entries or largs.skip_existing:
-                        msg = f"Please use `cobib edit {lbl}` instead!"
-                        LOGGER.warning(msg)
-                        continue
+                    continue
+                # in all other cases, we enter an interactive prompt to let the user decide how
+                # to proceed
+                msg = f"You tried to add a new entry '{lbl}' which already exists!"
+                LOGGER.warning(msg)
+                res = self.largs.disambiguation
+                # if the user provided the reply at runtime using the --disambiguation argument, the
+                # following condition is not met
+                if res is None:
+                    parser = BibtexParser()
+                    left = parser.dump(bib[lbl])
+                    right = parser.dump(entry)
+                    diff = Differ(left, right)
+                    diff.compute()
+                    table = diff.render("bibtex")
+
+                    # pylint: disable=assignment-from-no-return
+                    print_ret = self.console.print(table)  # type: ignore[union-attr]
+
+                    prompt_text = "How would you like to handle this conflict?"
+                    choices = ["keep", "replace", "update", "disambiguate", "help"]
+                    default = "keep"
+
+                    # pylint: disable=line-too-long
+                    self.prompt.process_response = self._wrap_prompt_process_response(  # type: ignore[method-assign]
+                        self.prompt.process_response  # type: ignore[assignment]
+                    )
+
+                    if self.prompt is not Prompt:
+                        res = await self.prompt.ask(  # type: ignore[call-overload]
+                            prompt_text,
+                            choices=choices,
+                            default=default,
+                            console=cast(App[None], self.console),
+                        )
+                        popup, _ = cast(Tuple[Widget, AwaitMount], print_ret)
+                        popup.remove()
+                    else:
+                        res = self.prompt.ask(
+                            prompt_text,
+                            choices=choices,
+                            default=default,
+                            console=cast(Console, self.console),
+                        )
+
+                    self.prompt.process_response = (  # type: ignore[method-assign]
+                        self.prompt.process_response.__wrapped__  # type: ignore[attr-defined]
+                    )
+
+                if res == "update":
+                    msg = f"Updating the already existing entry '{lbl}' with the new data."
+                    LOGGER.info(msg)
+                    existing_data = bib[lbl].data.copy()
+                    existing_data.update(entry.data)
+                    entry.data = existing_data.copy()
+                    overwrite_file = True
+                elif res == "disambiguate":
                     msg = (
                         "The label will be disambiguated based on the configuration option: "
                         "config.database.format.label_suffix"
                     )
                     LOGGER.warning(msg)
                     new_label = bib.disambiguate_label(lbl, entry)
                     entry.label = new_label
-                    new_entries[new_label] = entry
-                    new_entries.pop(lbl)
-                else:
-                    # label exists but the user asked to update an existing entry
-                    existing_data = bib[lbl].data.copy()
-                    existing_data.update(entry.data)
-                    entry.data = existing_data.copy()
+                    self.new_entries[new_label] = entry
+                    self.new_entries.pop(lbl)
+                elif res == "replace":
+                    msg = f"Overwriting the already existing entry '{lbl}' with the new data."
+                    LOGGER.info(msg)
+                elif res == "keep":
+                    msg = f"Skipping addition of the already existing entry '{lbl}'."
+                    LOGGER.info(msg)
+                    self.new_entries.pop(lbl)
+                    continue
+
             # download associated file (if requested)
             if "_download" in entry.data.keys():
-                if largs.skip_download:
+                if self.largs.skip_download:
                     entry.data.pop("_download")
                 else:
-                    path = FileDownloader().download(
-                        entry.data.pop("_download"),
-                        entry.label,
-                        folder=largs.path,
-                        overwrite=largs.update,
+                    task = asyncio.create_task(
+                        FileDownloader().download(
+                            entry.data.pop("_download"),
+                            entry.label,
+                            folder=self.largs.path,
+                            overwrite=overwrite_file,
+                        )
                     )
+                    path = await task
                     if path is not None:
                         entry.data["file"] = str(path)
             # check journal abbreviation
             if "journal" in entry.data.keys():
                 entry.data["journal"] = JournalAbbreviations.elongate(entry.data["journal"])
 
-        Event.PostAddCommand.fire(new_entries)
+        Event.PostAddCommand.fire(self)
 
-        bib.update(new_entries)
+        bib.update(self.new_entries)
         if edit_entries:
-            EditCommand().execute([largs.label])
+            EditCommand(self.largs.label).execute()
 
         bib.save()
 
-        self.git(args=vars(largs))
+        self.git()
 
-        for label in new_entries:
+        for label in self.new_entries:
             msg = f"'{label}' was added to the database."
             LOGGER.info(msg)
 
     @staticmethod
-    def tui(tui: cobib.tui.TUI) -> None:
-        # pdoc will inherit the docstring from the base class
-        # noqa: D102
-        LOGGER.debug("Add command triggered from TUI.")
-        # handle input via prompt
-        tui.execute_command("add")
-        # update database list
-        LOGGER.debug("Updating list after Add command.")
-        tui.viewport.update_list()
+    def _wrap_prompt_process_response(
+        func: Callable[[PromptBase[PromptType], str], PromptType]
+    ) -> Callable[[PromptBase[PromptType], str], PromptType]:
+        """A method to wrap a `PromptBase.process_response` method.
+
+        This method wraps a `PromptBase.process_response` method in order to handle a user's request
+        for additional help.
+
+        Args:
+            func: the `PromptBase.process_response` method to be wrapped.
+
+        Returns:
+            The wrapped `PromptBase.process_response` method.
+        """
+
+        @override
+        @wraps(func)
+        def process_response(prompt: PromptBase[PromptType], value: str) -> PromptType:
+            return_value: PromptType = func(prompt, value)
+
+            if return_value == "help":
+                LOGGER.debug("User requested help.")
+                raise InvalidResponse(
+                    "[yellow]A conflict between an existing (left) and newly added entry (right) "
+                    "occurred. These are your options:\n"
+                    "  'keep' the existing entry and discard the new addition (default)\n"
+                    "  'replace' the existing entry with the new one\n"
+                    "  'update' the existing entry with the new data\n"
+                    "  'disambiguate' the new entry from the existing one by adding a label suffix"
+                )
+
+            return return_value
+
+        return process_response
```

### Comparing `cobib-3.5.5/src/cobib/commands/base_command.py` & `cobib-4.0.0/src/cobib/commands/base_command.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,96 +5,183 @@
 import argparse
 import json
 import logging
 import os
 import shlex
 import sys
 from abc import ABC, abstractmethod
-from typing import IO, TYPE_CHECKING, Any, Dict, Generator, List, NoReturn, Optional
+from typing import List, Optional, Type
+
+from rich.console import Console, ConsoleRenderable
+from rich.prompt import Prompt, PromptBase
+from textual.app import App
+from textual.widget import Widget
 
 from cobib.config import Event, config
+from cobib.ui.components import ArgumentParser as ArgumentParser
 from cobib.utils.rel_path import RelPath
 
 LOGGER = logging.getLogger(__name__)
 
-if TYPE_CHECKING:
-    import cobib.tui
-
 
 class Command(ABC):
     """The Command interface.
 
     This interface should be implemented by all concrete command implementations.
-    In order to provide both, command-line and TUI usability, the `execute` and `tui` functions must
-    be implemented, respectively.
     """
 
     name = "base"
     """The commands `name` is used to extract the available commands for the command-line interface.
     """
 
-    def __init__(self) -> None:
-        """The initializer of any concrete implementation should *not* take any arguments!"""
+    argparser: ArgumentParser
+    """Every command has its own `argparse.ArgumentParser` which is used to parse the arguments
+    provided to the command. This is done no matter how the command is executed, whether
+    programmatically via Python, from the command-line or any other UI."""
+
+    def __init__(
+        self,
+        *args: str,
+        console: Console | App[None] | None = None,
+        prompt: Type[PromptBase[str]] | None = None,
+    ) -> None:
+        """Initializes a command instance.
+
+        Args:
+            *args: the sequence of additional command arguments. These will be passed on to the
+                `argparser` of this command for further parsing.
+            console: a command may be in need of printing something for the user during its
+                execution (and before its final result rendering). If so, it should use the `print`
+                method of this console object.
+            prompt: a command may be in need of prompting the user for an input. If so, it will use
+                this prompt kind. It is important that this is respected, as different UIs may
+                inject specific prompt classes to implement different runtime behavior.
+        """
+        self.args: tuple[str, ...] = args
+        """The raw provided command arguments."""
+
+        self.largs: argparse.Namespace = self.__class__._parse_args(args)
+        """The parsed (local) arguments."""
+
+        self.console: Console | App[None] = console if console is not None else Console()
+        """The object via which to print output to the user during runtime execution."""
+
+        self.prompt: Type[PromptBase[str]] = prompt if prompt is not None else Prompt
+        """The object via which to prompt the user for input during runtime execution."""
+
+    @classmethod
+    @abstractmethod
+    def init_argparser(cls) -> None:
+        """Initializes this command's `argparse.ArgumentParser`.
+
+        This method needs to be overwritten by every subclass and handles the registration of all
+        available command arguments.
+        """
+
+    @classmethod
+    def _get_argparser(cls) -> ArgumentParser:
+        """Returns this command's `argparse.ArgumentParser`.
+
+        The reason for having this method is to handle the parser initialization such that it only
+        needs to be done once.
+
+        Returns:
+            This command's initialized `argparser` object.
+        """
+        if hasattr(cls, "argparser"):
+            return cls.argparser
+
+        cls.init_argparser()
+        return cls.argparser
+
+    @classmethod
+    def _parse_args(cls, args: tuple[str, ...]) -> argparse.Namespace:
+        """Parses the provided command arguments.
+
+        Args:
+            args: the sequence of additional command arguments provided to the command upon
+                initialization.
+
+        Returns:
+            The parsed arguments namespace.
+        """
+        try:
+            largs = cls._get_argparser().parse_args(args)
+        except argparse.ArgumentError as exc:
+            LOGGER.error(exc.message)
+            sys.exit(1)
+
+        return largs
 
     @abstractmethod
-    def execute(self, args: List[str], out: IO[Any] = sys.stdout) -> Any:
+    def execute(self) -> None:
         """Actually executes the command.
 
         This means, all of the command-specific logic and action needs to be implemented by this
         method.
-        It also poses as the pure interface triggered from the command-line.
-        The arguments given to this function are parsed by `argparse` which also means that each
-        subcommand should provide an additional `--help` menu for the command-line interface.
-        ```
-        cobib <subcommand> --help
-        ```
+
+        .. note::
+           This method is **not** in charge of presenting the final result to the user. Refer to the
+           various `render_*` methods, instead.
+
+        As a consequence, resulting data should be stored on the command instance (which also has
+        the benefit of exposing this data to the various `Post*Command` `cobib.config.event.Event`
+        hooks.
 
         This function may *not* raise any errors!
         This also means it should take care of catching all potential errors triggered by internally
         used methods.
         Such encountered errors should be logged and the method should return gracefully.
+        """
 
-        Args:
-            args: a sequence of additional arguments used for the execution.
-            out: the output IO stream. This defaults to `sys.stdout`.
+    def render_porcelain(self) -> List[str]:
+        """Renders the command results in "porcelain" mode.
+
+        This method is called when the `--porcelain` argument has been provided.
+        The idea is to provide an output mode which is easily parse-able by another program or
+        function.
 
         Returns:
-            Usually `None` but some complex commands may choose to return some of their runtime data
-            for ease of additional post-processing in (e.g.) the `tui` wrapper.
+            A list of strings where each entry should be considered one line of output.
         """
+        return []
 
-    @staticmethod
-    @abstractmethod
-    def tui(tui: cobib.tui.TUI) -> Optional[Generator[List[str], None, None]]:
-        """TUI command interface.
+    def render_rich(self) -> Optional[ConsoleRenderable]:
+        """Renders the command results as a `rich` object.
+
+        This method is called when a command is run via the command-line interface.
 
-        This function serves as the commands entry-point from the `cobib.tui.tui.TUI` instance.
-        It should take care of any pre- and/or post-processing before calling `execute` internally
-        to do the actual work.
+        Returns:
+            An optional `ConsoleRenderable` to be presented to the user.
+        """
+        return None
 
-        The processing may involve handling of highlighting as well as general screen buffer
-        contents.
+    def render_textual(self) -> Optional[Widget]:
+        """Renders the command results as a `textual` widget.
 
-        Args:
-            tui: the runtime-instance of coBib's TUI.
+        This method is called when a command is run via the terminal user interface.
+        It is the responsibility of the TUI to deal with the returned widget.
 
-        Yields:
-            Optionally, this method may `yield` the command arguments for further processing.
+        Returns:
+            An optional `Widget` to be rendered in the TUI.
         """
+        return None
 
-    def git(self, args: Optional[Dict[str, Any]] = None, force: bool = False) -> None:
+    def git(self, force: bool = False) -> None:
         """Generates a git commit to track the commands changes.
 
-        This function only has an effect when `config.database.git` is enabled *and* the database
-        has been initialized correctly with `cobib.commands.init.InitCommand`.
+        This function only has an effect when `cobib.config.config.DatabaseConfig.git` is enabled
+        *and* the database has been initialized correctly with `cobib.commands.init`.
         Otherwise, a warning will be printed and no commit will be generated.
         Nonetheless, the changes applied by the commit will have taken effect in the database.
 
+        This method uses the parsed arguments (`largs`) to include command execution information in
+        the generated commit message.
+
         Args:
-            args: a dictionary containing the *parsed* command arguments.
             force: whether to ignore the configuration setting. This option is mainly used by the
                 `cobib.commands.init.InitCommand`.
         """
         git_tracked = config.database.git
         if not git_tracked and not force:
             return
 
@@ -106,14 +193,15 @@
                 msg = (
                     "You have configured coBib to track your database with git."
                     "\nPlease run `cobib init --git`, to initialize this tracking."
                 )
                 LOGGER.warning(msg)
                 return
 
+        args = vars(self.largs)
         msg = f"Auto-commit: {self.name.title()}Command"
         if args:
             msg += "\n\n"
             msg += json.dumps(args, indent=2, default=str)
 
         msg = Event.PreGitCommit.fire(msg, args) or msg
 
@@ -122,32 +210,7 @@
             f"git add -- {file}",
             f"git commit --no-gpg-sign --quiet --message {shlex.quote(msg)}",
         ]
         LOGGER.debug("Auto-commit to git from %s command.", self.name)
         os.system("; ".join(commands))
 
         Event.PostGitCommit.fire(root, file)
-
-
-class ArgumentParser(argparse.ArgumentParser):
-    """Wrapper of the `argparse.ArgumentParser` to allow catching of error messages.
-
-    Note, this class will be removed once Python 3.9 becomes the minimal supported version as it
-    added the [`exit_on_error`](https://docs.python.org/3/library/argparse.html#exit-on-error)
-    keyword argument.
-    """
-
-    # TODO: once Python 3.9 becomes the default, make use of the exit_on_error argument.
-
-    def exit(self, status: int = 0, message: Optional[str] = None) -> NoReturn:
-        """Overwrite the exit method to raise an error rather than exit.
-
-        Args:
-            status: the status code. If non-zero, an `argparse.ArgumentError` will be raised.
-            message: the message of the error.
-
-        Raises:
-            An `argparse.ArgumentError`.
-        """
-        if status:
-            raise argparse.ArgumentError(None, f"Error: {message}")
-        super().exit(status, message)  # pragma: no cover
```

### Comparing `cobib-3.5.5/src/cobib/commands/delete.py` & `cobib-4.0.0/src/cobib/commands/delete.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,113 +1,104 @@
 """coBib's Delete command.
 
 This command can be used to deleted entries from the database.
 ```
 cobib delete <label 1> [<label 2> ...]
 ```
 
-You can also trigger this command from the `cobib.tui.tui.TUI`.
+If you want to preserve the files associated with the deleted entries, you can provide the
+`--preserve-files` argument like so:
+```
+cobib delete --preserve-files <label 1> [<label 2> ...]
+```
+
+### TUI
+
+You can also trigger this command from the `cobib.ui.tui.TUI`.
 By default, it is bound to the `d` key.
 """
 
 from __future__ import annotations
 
-import argparse
 import logging
 import os
-import sys
-from typing import IO, TYPE_CHECKING, Any, List
+from typing import Set, Type
+
+from rich.console import Console
+from rich.prompt import PromptBase
+from textual.app import App
+from typing_extensions import override
 
 from cobib.config import Event
 from cobib.database import Database
 from cobib.utils.rel_path import RelPath
 
 from .base_command import ArgumentParser, Command
 
 LOGGER = logging.getLogger(__name__)
 
-if TYPE_CHECKING:
-    import cobib.tui
-
 
 class DeleteCommand(Command):
-    """The Delete Command."""
+    """The Delete Command.
 
-    name = "delete"
+    This command can parse the following arguments:
 
-    def execute(self, args: List[str], out: IO[Any] = sys.stdout) -> None:
-        """Deletes an entry.
+        * `labels`: one (or multiple) labels of the entries to be deleted.
+        * `--preserve-files`: skips the deletion of any associated files.
+    """
 
-        This command deletes one (or multiple) entries from the database.
+    name = "delete"
 
-        Args:
-            args: a sequence of additional arguments used for the execution. The following values
-                are allowed for this command:
-                    * `labels`: one (or multiple) labels of the entries to be deleted.
-            out: the output IO stream. This defaults to `sys.stdout`.
-        """
-        LOGGER.debug("Starting Delete command.")
+    @override
+    def __init__(
+        self,
+        *args: str,
+        console: Console | App[None] | None = None,
+        prompt: Type[PromptBase[str]] | None = None,
+    ) -> None:
+        super().__init__(*args, console=console, prompt=prompt)
+
+        self.deleted_entries: Set[str] = set()
+        """A set of labels which were deleted by this command."""
+
+    @override
+    @classmethod
+    def init_argparser(cls) -> None:
         parser = ArgumentParser(prog="delete", description="Delete subcommand parser.")
         parser.add_argument("labels", type=str, nargs="+", help="labels of the entries")
         parser.add_argument(
             "--preserve-files", action="store_true", help="do not delete associated files"
         )
+        cls.argparser = parser
 
-        if not args:
-            parser.print_usage(sys.stderr)
-            sys.exit(1)
-
-        try:
-            largs = parser.parse_args(args)
-        except argparse.ArgumentError as exc:
-            LOGGER.error(exc.message)
-            return
-
-        Event.PreDeleteCommand.fire(largs)
+    @override
+    def execute(self) -> None:
+        LOGGER.debug("Starting Delete command.")
 
-        deleted_entries = set()
+        Event.PreDeleteCommand.fire(self)
 
         bib = Database()
-        for label in largs.labels:
+        for label in self.largs.labels:
             try:
                 LOGGER.debug("Attempting to delete entry '%s'.", label)
                 entry = bib.pop(label)
-                if not largs.preserve_files:
+                if not self.largs.preserve_files:
                     for file in entry.file:
                         path = RelPath(file)
                         try:
                             LOGGER.debug("Attempting to remove associated file '%s'.", str(path))
                             os.remove(path.path)
                         except FileNotFoundError:
                             pass
 
-                deleted_entries.add(label)
+                self.deleted_entries.add(label)
             except KeyError:
                 pass
 
-        Event.PostDeleteCommand.fire(deleted_entries)
+        Event.PostDeleteCommand.fire(self)
         bib.save()
 
-        self.git(args=vars(largs))
+        self.git()
 
-        for label in deleted_entries:
+        for label in self.deleted_entries:
             msg = f"'{label}' was removed from the database."
             LOGGER.info(msg)
-
-    @staticmethod
-    def tui(tui: cobib.tui.TUI) -> None:
-        # pdoc will inherit the docstring from the base class
-        # noqa: D102
-        LOGGER.debug("Delete command triggered from TUI.")
-        if tui.selection:
-            # use selection for command
-            labels = list(tui.selection)
-            tui.selection.clear()
-        else:
-            # get current label
-            label, _ = tui.viewport.get_current_label()
-            labels = [label]
-        # delete selected entry
-        tui.execute_command(["delete"] + labels, skip_prompt=True)
-        # update database list
-        LOGGER.debug("Updating list after Delete command.")
-        tui.viewport.update_list()
```

### Comparing `cobib-3.5.5/src/cobib/commands/edit.py` & `cobib-4.0.0/src/cobib/commands/edit.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,130 +1,142 @@
 """coBib's Edit command.
 
 This command can be used to manually edit database entries in their easily-readable YAML format.
 To get started, simply type:
 ```
 cobib edit <label>
 ```
-which will open the YAML-formatted version of the specified Entry for editing.
+which will open the YAML-formatted version of the specified `cobib.database.Entry` for editing.
 
-You can configure which editor will be used via the `config.commands.edit.editor` setting which will
-default to using your `$EDITOR` environment setting (and fall back to `vim` if that is not set).
+You can configure which editor will be used via the `cobib.config.config.EditCommandConfig.editor`
+setting which will default to using your `$EDITOR` environment setting (and fall back to `vim` if
+that is not set).
 
 You can even add entirely new entries to the database by specifying an unused entry label *and*
 adding the `--add` command-line argument:
 ```
 cobib edit --add <new label>
 ```
 This entry will be entirely empty except for the one field which is always present:
-* `ENTRYTYPE`: set to the default value configured via `config.commands.edit.default_entry_type`.
+    * `ENTRYTYPE`: set to the default value configured via
+      `cobib.config.config.EditCommandConfig.default_entry_type`.
 
-You can also trigger this command from the `cobib.tui.tui.TUI`.
+If you change the label of the entry during editing and you do *not* want your associated files to
+automatically be renamed, you can provide the `--preserve-files` argument like so:
+```
+cobib edit --preserve-files <label>
+```
+
+### TUI
+
+You can also trigger this command from the `cobib.ui.tui.TUI`.
 By default, it is bound to the `e` key.
 If you want to add a new entry manually, you will have to enter the prompt (defaults to `:`) and
 then type out the command mentioned above:
 ```
 :edit --add <new label>
 ```
 """
 
 from __future__ import annotations
 
-import argparse
 import logging
 import os
-import sys
 import tempfile
 from pathlib import Path
-from typing import IO, TYPE_CHECKING, Any, List
+from typing import Type
+
+from rich.console import Console
+from rich.prompt import PromptBase
+from textual.app import App
+from typing_extensions import override
 
 from cobib.config import Event, config
 from cobib.database import Database, Entry
 from cobib.parsers.yaml import YAMLParser
 from cobib.utils.rel_path import RelPath
 
 from .base_command import ArgumentParser, Command
 
 LOGGER = logging.getLogger(__name__)
 
-if TYPE_CHECKING:
-    import cobib.tui
-
 
 class EditCommand(Command):
-    """The Edit Command."""
+    """The Edit Command.
 
-    name = "edit"
+    This command can parse the following arguments:
 
-    def execute(self, args: List[str], out: IO[Any] = sys.stdout) -> None:
-        """Opens an entry for manual editing.
+        * `label`: the label of the entry to edit.
+        * `-a`, `--add`: if specified, allows adding a new entry for a non-existent label. The
+          default entry type of this new entry can be configured via
+          `cobib.config.config.EditCommandConfig.default_entry_type`.
+        * `--preserve-files`: skips the renaming of any associated files in case you manually rename
+            the entry label during editing.
+    """
 
-        This command opens an `cobib.database.Entry` in YAML format for manual editing.
-        The editor program can be configured via `config.commands.edit.editor`.
-        By default, this setting will respect your `$EDITOR` environment variable, but fall back to
-        using `vim` if that variable is not set.
-
-        Args:
-            args: a sequence of additional arguments used for the execution. The following values
-                are allowed for this command:
-                    * `label`: the label of the entry to edit.
-                    * `-a`, `--add`: if specified, allows adding new entries for non-existent
-                      labels. The default entry type of this new entry can be configured via
-                      `config.commands.edit.default_entry_type`.
-            out: the output IO stream. This defaults to `sys.stdout`.
-        """
-        LOGGER.debug("Starting Edit command.")
+    name = "edit"
+
+    @override
+    def __init__(
+        self,
+        *args: str,
+        console: Console | App[None] | None = None,
+        prompt: Type[PromptBase[str]] | None = None,
+    ) -> None:
+        super().__init__(*args, console=console, prompt=prompt)
+
+        self.new_entry: Entry
+        """A `cobib.database.Entry` instance edited by this command."""
+
+    @override
+    @classmethod
+    def init_argparser(cls) -> None:
         parser = ArgumentParser(prog="edit", description="Edit subcommand parser.")
         parser.add_argument("label", type=str, help="label of the entry")
         parser.add_argument(
             "-a",
             "--add",
             action="store_true",
             help="if specified, will add a new entry for unknown labels",
         )
         parser.add_argument(
             "--preserve-files", action="store_true", help="do not rename associated files"
         )
+        cls.argparser = parser
 
-        if not args:
-            parser.print_usage(sys.stderr)
-            sys.exit(1)
-
-        try:
-            largs = parser.parse_args(args)
-        except argparse.ArgumentError as exc:
-            LOGGER.error(exc.message)
-            return
+    @override
+    def execute(self) -> None:
+        LOGGER.debug("Starting Edit command.")
 
-        Event.PreEditCommand.fire(largs)
+        Event.PreEditCommand.fire(self)
 
         yml = YAMLParser()
 
         bib = Database()
 
         try:
-            entry = bib[largs.label]
+            entry = bib[self.largs.label]
             prv = yml.dump(entry)
-            if largs.add:
+            if self.largs.add:
                 LOGGER.warning(
-                    "Entry '%s' already exists! Ignoring the `--add` argument.", largs.label
+                    "Entry '%s' already exists! Ignoring the `--add` argument.", self.largs.label
                 )
-                largs.add = False
+                self.largs.add = False
         except KeyError:
             # No entry for given label found
-            if largs.add:
+            if self.largs.add:
                 # add a new entry for the unknown label
                 entry = Entry(
-                    largs.label,
+                    self.largs.label,
                     {"ENTRYTYPE": config.commands.edit.default_entry_type},
                 )
                 prv = yml.dump(entry)
             else:
                 msg = (
-                    f"No entry with the label '{largs.label}' could be found."
+                    f"No entry with the label '{self.largs.label}' could be found."
                     "\nUse `--add` to add a new entry with this label."
                 )
                 LOGGER.error(msg)
                 return
         if prv is None:
             # No entry found to be edited. This should never occur unless the YAMLParser experiences
             # an unexpected error.
@@ -136,54 +148,39 @@
             tmp_file.write(prv)
             tmp_file.flush()
             LOGGER.debug('Starting editor "%s".', config.commands.edit.editor)
             status = os.system(config.commands.edit.editor + " " + tmp_file.name)
             assert status == 0
             LOGGER.debug("Editor finished successfully.")
             new_entries = YAMLParser().parse(tmp_file.name)
-            new_entry = list(new_entries.values())[0]
+            self.new_entry = list(new_entries.values())[0]
         assert not Path(tmp_file_name).exists()
-        if entry == new_entry and not largs.add:
+        if entry == self.new_entry and not self.largs.add:
             LOGGER.info("No changes detected.")
             return
 
-        bib.update({new_entry.label: new_entry})
-        if new_entry.label != largs.label:
-            bib.rename(largs.label, new_entry.label)
-            if not largs.preserve_files:
+        bib.update({self.new_entry.label: self.new_entry})
+        if self.new_entry.label != self.largs.label:
+            bib.rename(self.largs.label, self.new_entry.label)
+            if not self.largs.preserve_files:
                 new_files = []
-                for file in new_entry.file:
+                for file in self.new_entry.file:
                     path = RelPath(file)
-                    if path.path.stem == largs.label:
+                    if path.path.stem == self.largs.label:
                         LOGGER.info("Also renaming associated file '%s'.", str(path))
-                        target = RelPath(path.path.parent / f"{new_entry.label}.pdf")
+                        target = RelPath(path.path.parent / f"{self.new_entry.label}.pdf")
                         if target.path.exists():
                             LOGGER.warning("Found conflicting file, not renaming '%s'.", str(path))
                         else:
                             path.path.rename(target.path)
                             new_files.append(str(target))
                             continue
                     new_files.append(file)
-                new_entry.file = new_files
+                self.new_entry.file = new_files
 
-        Event.PostEditCommand.fire(new_entry)
+        Event.PostEditCommand.fire(self)
         bib.save()
 
-        self.git(args=vars(largs))
+        self.git()
 
-        msg = f"'{largs.label}' was successfully edited."
+        msg = f"'{self.largs.label}' was successfully edited."
         LOGGER.info(msg)
-
-    @staticmethod
-    def tui(tui: cobib.tui.TUI) -> None:
-        # pdoc will inherit the docstring from the base class
-        # noqa: D102
-        LOGGER.debug("Edit command triggered from TUI.")
-        # get current label
-        label, _ = tui.viewport.get_current_label()
-        # populate buffer with entry data
-        EditCommand().execute([label])
-        # redraw total screen after closing external editor
-        LOGGER.debug("Manually redrawing TUI to clear out any editor artifacts.")
-        tui.resize_handler(None, None)
-        # update database list
-        tui.viewport.update_list()
```

### Comparing `cobib-3.5.5/src/cobib/commands/export.py` & `cobib-4.0.0/src/cobib/commands/export.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,96 +14,112 @@
 cobib export --zip my_references.zip
 ```
 This is an important feature because coBib (by design) allows you to spread associated files across
 your entire file system.
 With this command you can gather them in a neat package for sharing or transferring.
 
 You can also limit the export to a subset of your database in one of two ways:
+
 1. through filters:
-```
-cobib export --bibtex my_private_database.bib -- ++tags private
-```
-2. through a custom selection (using `--selection`)
-```
-cobib export --selection --bibtex some_other_database.bib -- Label1 Label2
-```
-While this latter case is usable via the command-line interface it is more a side-effect of the TUI
-integration which provides a visual selection (defaults to the `v` key).
-The proper and arguably more useful case is the first case using filters.
+   ```
+   cobib export --bibtex my_private_database.bib -- ++tags private
+   ```
+
+2. through a custom selection (using `--selection` or the short-hand option `-s`)
+   ```
+   cobib export --selection --bibtex some_other_database.bib -- Label1 Label2
+   ```
+
+.. note::
+   While this latter case is usable via the command-line interface it is more a side-effect of the
+   TUI integration which provides a visual selection (defaults to the `v` key).
+   The proper and arguably more useful case is the first case using filters.
 
 Since v3.2.0, coBib supports automatic Journal abbreviations. After configuring them as explained in
-`config.utils.journal_abbreviations` you can leverage them during exporting like so:
+`cobib.config.config.UtilsConfig.journal_abbreviations` you can leverage them during exporting like
+so:
 ```
 cobib export --abbreviate --bibtex my_database.bib
 # or
 cobib export --abbreviate --dotless --bibtex my_database.bib
 ```
 
-You can also trigger this command from the `cobib.tui.tui.TUI`.
+### TUI
+
+You can also trigger this command from the `cobib.ui.tui.TUI`.
 By default, it is bound to the `x` key which will drop you into the prompt where you can type out a
 normal command-line command:
 ```
 :export <arguments go here>
 ```
+
+.. note::
+   If you have already selected one or more entries, the `--selection` argument will automatically
+   be added.
 """
 
 from __future__ import annotations
 
 import argparse
 import logging
-import os
-import sys
-from typing import IO, TYPE_CHECKING, Any, List
+from typing import List, Type
 from zipfile import ZipFile
 
+from rich.console import Console
+from rich.prompt import PromptBase
+from textual.app import App
+from typing_extensions import override
+
 from cobib.config import Event
-from cobib.database import Database
+from cobib.database import Database, Entry
 from cobib.parsers.bibtex import BibtexParser
 from cobib.utils.journal_abbreviations import JournalAbbreviations
 from cobib.utils.rel_path import RelPath
 
 from .base_command import ArgumentParser, Command
-from .list import ListCommand
+from .list_ import ListCommand
 
 LOGGER = logging.getLogger(__name__)
 
-if TYPE_CHECKING:
-    import cobib.tui
-
 
 class ExportCommand(Command):
-    """The Export Command."""
+    """The Export Command.
 
-    name = "export"
+    This command can parse the following arguments:
 
-    def execute(self, args: List[str], out: IO[Any] = sys.stdout) -> None:
-        """Exports the database.
+        * `-b`, `--bibtex`: specifies a BibLaTex filename into which to export.
+        * `-z`, `--zip`: specifies a Zip-filename into which to export associated files.
+        * `-a`, `--abbreviate`: abbreviate the Journal names before exporting. See also
+          `cobib.config.config.UtilsConfig.journal_abbreviations`.
+        * `--dotless`: remove punctuation from the Journal abbreviations.
+        * `-s`, `--selection`: when specified, the positional arguments will *not* be
+          interpreted as filters but rather as a direct list of entry labels. This can
+          be used on the command-line but is mainly meant for the TUIs visual selection
+          interface (hence the name).
+        * in addition to the above, you can add `filters` to specify a subset of your
+          database for exporting. For more information refer to `cobib.commands.list_`.
+    """
 
-        This command exports the database (or a selected subset of entries).
-        You can choose the exported formats from the following list:
-        * BibLaTex (via the `--bibtex` argument)
-        * Zip archive (via the `--zip` argument)
-
-        Args:
-            args: a sequence of additional arguments used for the execution. The following values
-                are allowed for this command:
-                    * `-b`, `--bibtex`: specifies a BibLaTex filename into which to export.
-                    * `-z`, `--zip`: specifies a Zip-filename into which to export associated files.
-                    * `-a`, `--abbreviate`: abbreviate the Journal names before exporting. See also
-                      `config.utils.journal_abbreviations`.
-                    * `--dotless`: remove punctuation from the Journal abbreviations.
-                    * `-s`, `--selection`: when specified, the positional arguments will *not* be
-                      interpreted as filters but rather as a direct list of entry labels. This can
-                      be used on the command-line but is mainly meant for the TUIs visual selection
-                      interface (hence the name).
-                    * in addition to the above, you can add `filters` to specify a subset of your
-                      database for exporting. For more information refer to `cobib.commands.list`.
-            out: the output IO stream. This defaults to `sys.stdout`.
-        """
-        LOGGER.debug("Starting Export command.")
+    name = "export"
+
+    @override
+    def __init__(
+        self,
+        *args: str,
+        console: Console | App[None] | None = None,
+        prompt: Type[PromptBase[str]] | None = None,
+    ) -> None:
+        super().__init__(*args, console=console, prompt=prompt)
+
+        self.exported_entries: List[Entry] = []
+        """A list of `cobib.database.Entry` objects which were exported by this command."""
+
+    @override
+    @classmethod
+    def init_argparser(cls) -> None:
         parser = ArgumentParser(prog="export", description="Export subcommand parser.")
         parser.add_argument(
             "-b", "--bibtex", type=argparse.FileType("a"), help="BibLaTeX output file"
         )
         parser.add_argument("-z", "--zip", type=argparse.FileType("a"), help="zip output file")
         parser.add_argument(
             "-s",
@@ -122,80 +138,67 @@
         )
         parser.add_argument(
             "-a", "--abbreviate", action="store_true", help="Abbreviate journal names"
         )
         parser.add_argument(
             "--dotless", action="store_true", help="Remove punctuation from journal abbreviations"
         )
+        cls.argparser = parser
 
-        if not args:
-            parser.print_usage(sys.stderr)
-            sys.exit(1)
-
-        try:
-            largs = parser.parse_intermixed_args(args)
-        except argparse.ArgumentError as exc:
-            LOGGER.error(exc.message)
-            return
+    @override
+    def execute(self) -> None:
+        LOGGER.debug("Starting Export command.")
 
-        Event.PreExportCommand.fire(largs)
+        Event.PreExportCommand.fire(self)
 
-        if largs.bibtex is None and largs.zip is None:
+        if self.largs.bibtex is None and self.largs.zip is None:
             msg = "No output file specified!"
             LOGGER.error(msg)
             return
-        if largs.zip is not None:
-            largs.zip = ZipFile(largs.zip.name, "w")  # pylint: disable=consider-using-with
+        if self.largs.zip is not None:
+            self.largs.zip = ZipFile(  # pylint: disable=consider-using-with
+                self.largs.zip.name, "w"
+            )
 
-        if largs.selection:
+        if self.largs.selection:
             LOGGER.info("Selection given. Interpreting `filter` as a list of labels")
-            labels = largs.filter
+            labels = self.largs.filter
+            bib = Database()
+            for label in labels:
+                try:
+                    self.exported_entries.append(bib[label])
+                except KeyError:
+                    msg = f"No entry with the label '{label}' could be found."
+                    LOGGER.warning(msg)
         else:
             LOGGER.debug("Gathering filtered list of entries to be exported.")
-            with open(os.devnull, "w", encoding="utf-8") as devnull:
-                labels = ListCommand().execute(largs.filter, out=devnull)
+            self.exported_entries, _ = ListCommand(*self.largs.filter).filter_entries()
 
         bibtex_parser = BibtexParser()
 
-        bib = Database()
-
-        for label in labels:
-            try:
-                LOGGER.info('Exporting entry "%s".', label)
-                entry = bib[label]
-                if largs.bibtex is not None:
-                    if largs.abbreviate and "journal" in entry.data.keys():
-                        entry.data["journal"] = JournalAbbreviations.abbreviate(
-                            entry.data["journal"], dotless=largs.dotless
+        for entry in self.exported_entries:
+            LOGGER.info('Exporting entry "%s".', entry.label)
+            if self.largs.bibtex is not None:
+                if self.largs.abbreviate and "journal" in entry.data.keys():
+                    entry.data["journal"] = JournalAbbreviations.abbreviate(
+                        entry.data["journal"], dotless=self.largs.dotless
+                    )
+                entry_str = bibtex_parser.dump(entry)
+                self.largs.bibtex.write(entry_str)
+            if self.largs.zip is not None:
+                if "file" in entry.data.keys() and entry.file is not None:
+                    files = entry.file
+                    if not isinstance(files, list):
+                        files = [files]
+                    for file in files:
+                        path = RelPath(file).path
+                        LOGGER.debug(
+                            'Adding "%s" associated with "%s" to the zip file.', path, entry.label
                         )
-                    entry_str = bibtex_parser.dump(entry)
-                    largs.bibtex.write(entry_str)
-                if largs.zip is not None:
-                    if "file" in entry.data.keys() and entry.file is not None:
-                        files = entry.file
-                        if not isinstance(files, list):
-                            files = [files]
-                        for file in files:
-                            path = RelPath(file).path
-                            LOGGER.debug(
-                                'Adding "%s" associated with "%s" to the zip file.', path, label
-                            )
-                            largs.zip.write(path, path.name)
-            except KeyError:
-                msg = f"No entry with the label '{label}' could be found."
-                LOGGER.warning(msg)
-
-        Event.PostExportCommand.fire(labels, largs)
-
-        if largs.zip is not None:
-            largs.zip.close()
-
-    @staticmethod
-    def tui(tui: cobib.tui.TUI) -> None:
-        # pdoc will inherit the docstring from the base class
-        # noqa: D102
-        LOGGER.debug("Export command triggered from TUI.")
-        # handle input via prompt
-        if tui.selection:
-            tui.execute_command("export -s", pass_selection=True)
-        else:
-            tui.execute_command("export")
+                        self.largs.zip.write(path, path.name)
+
+        Event.PostExportCommand.fire(self)
+
+        if self.largs.bibtex is not None:
+            self.largs.bibtex.close()
+        if self.largs.zip is not None:
+            self.largs.zip.close()
```

### Comparing `cobib-3.5.5/src/cobib/commands/import_.py` & `cobib-4.0.0/src/cobib/commands/import_.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,155 +9,160 @@
 separate module, `cobib.importers`.
 The various backends are registered (at runtime) in a *mutually exclusive* group of keyword
 arguments, which you can use like so:
 ```
 cobib import --zotero
 ```
 
+.. note::
+   Since this command adds new entries to the database, its outcome can be affected by your
+   `cobib.config.config.DatabaseConfig` settings. In particular, pay attention to the
+   `cobib.config.config.EntryStringifyConfig` settings which affect how entries are converted
+   to/from strings. In particular, the following setting will affect how multiple files are split
+   into a list of files:
+   ```
+   config.database.stringify.list_separator.file = ", "
+   ```
+   The above will separate file paths using `, ` but if you use a different separator (for example
+   `;`) be sure to update this setting accordingly.
+
 ### Additional Options
 
 If you want to suppress the automatic download of attachments, specify the `--skip-download`
 argument like so:
 ```
 cobib import --skip-download --zotero
 ```
 
 The various importers may take even more command line arguments. Please check out their
 documentation at `cobib.importers` for more details.
 
 ### TUI
 
-You can also trigger this command from the `cobib.tui.tui.TUI`.
+You can also trigger this command from the `cobib.ui.tui.TUI`.
 By default, it is bound to the `i` key which will drop you into the prompt where you can type out a
 normal command-line command:
 ```
 :import <arguments go here>
 ```
 """
 
 from __future__ import annotations
 
 import argparse
 import inspect
 import logging
-import sys
 from collections import OrderedDict
-from typing import IO, TYPE_CHECKING, Any, Dict, List
+from typing import Dict, List, Type
+
+from rich.console import Console
+from rich.prompt import PromptBase
+from textual.app import App
+from typing_extensions import override
 
 from cobib import importers
 from cobib.config import Event
 from cobib.database import Database, Entry
 
 from .base_command import ArgumentParser, Command
 
 LOGGER = logging.getLogger(__name__)
 
-if TYPE_CHECKING:
-    import cobib.tui
-
 
 class ImportCommand(Command):
-    """The ImportCommand."""
+    """The ImportCommand.
+
+    This command can parse the following arguments:
+
+        * `--skip-download`: skips the automatic download of attached files (like PDFs).
+        * in addition to the options above, a *mutually exclusive group* of keyword arguments for
+          all available `cobib.importers` are registered at runtime. Please check the output of
+          `cobib import --help` for the exact list.
+        * finally, you can add another set of positional arguments (preceded by `--`) which will be
+          passed on to the chosen importer. For more details see for example
+          `cobib import --zotero -- --help`.
+    """
 
     name = "import"
 
-    # pylint: disable=too-many-branches,too-many-statements
-    def execute(self, args: List[str], out: IO[Any] = sys.stdout) -> None:
-        """Imports new entries from another bibliography manager.
-
-        The source from which to import new entries is configured via the `args`. The available
-        importers are provided by the `cobib.importers` module.
-
-        Args:
-            args: a sequence of additional arguments used for the execution. The following values
-                are allowed for this command:
-                    * `--skip-download`: skips the automatic download of attached files (like PDFs).
-                    * in addition to the options above, a *mutually exclusive group* of keyword
-                      arguments for all available `cobib.importers` are registered at runtime.
-                      Please check the output of `cobib import --help` for the exact list.
-                    * finally, you can add another set of positional arguments (preceded by `--`)
-                      which will be passed on to the chosen importer. For more details see for
-                      example `cobib import --zotero -- --help`.
-            out: the output IO stream. This defaults to `sys.stdout`.
-        """
-        LOGGER.debug("Starting Import command.")
+    _avail_importers = {
+        cls.name: cls for _, cls in inspect.getmembers(importers) if inspect.isclass(cls)
+    }
+    """The available importers."""
+
+    @override
+    def __init__(
+        self,
+        *args: str,
+        console: Console | App[None] | None = None,
+        prompt: Type[PromptBase[str]] | None = None,
+    ) -> None:
+        super().__init__(*args, console=console, prompt=prompt)
+
+        self.new_entries: Dict[str, Entry] = OrderedDict()
+        """An `OrderedDict` mapping labels to `cobib.database.Entry` instances which were imported
+        by this command."""
+
+    @override
+    @classmethod
+    def init_argparser(cls) -> None:
         parser = ArgumentParser(prog="import", description="Import subcommand parser.")
         parser.add_argument(
             "--skip-download",
             action="store_true",
             help="skip the automatic download of encountered PDF attachments",
         )
         parser.add_argument(
             "importer_arguments",
             nargs="*",
             help="You can pass additional arguments to the chosen importer. To ensure this works as"
             " expected you should add the pseudo-argument '--' before the remaining arguments.",
         )
         group_import = parser.add_mutually_exclusive_group()
-        avail_parsers = {
-            cls.name: cls for _, cls in inspect.getmembers(importers) if inspect.isclass(cls)
-        }
-        for name in avail_parsers.keys():
+        for name in cls._avail_importers.keys():
             try:
                 group_import.add_argument(f"--{name}", action="store_true", help=f"{name} importer")
             except argparse.ArgumentError:
                 continue
+        cls.argparser = parser
 
-        if not args:
-            parser.print_usage(sys.stderr)
-            sys.exit(1)
-
-        try:
-            largs = parser.parse_args(args)
-        except argparse.ArgumentError as exc:
-            LOGGER.error(exc.message)
-            return
+    @override
+    async def execute(self) -> None:  # type: ignore[override]
+        # pylint: disable=invalid-overridden-method
+        LOGGER.debug("Starting Import command.")
 
-        Event.PreImportCommand.fire(largs)
+        Event.PreImportCommand.fire(self)
 
         imported_entries: List[Entry] = []
 
-        for name, cls in avail_parsers.items():
-            enabled = getattr(largs, name, False)
+        for name, cls in ImportCommand._avail_importers.items():
+            enabled = getattr(self.largs, name, False)
             if not enabled:
                 continue
             LOGGER.debug("Importing entries from %s.", name)
-            imported_entries = cls().fetch(
-                largs.importer_arguments, skip_download=largs.skip_download
-            )
+            imported_entries = await cls(
+                *self.largs.importer_arguments, skip_download=self.largs.skip_download
+            ).fetch()
             break
 
         bib = Database()
         existing_labels = set(bib.keys())
 
-        new_entries: Dict[str, Entry] = OrderedDict()
-
         for entry in imported_entries:
             # check if label already exists
             if entry.label in existing_labels:
                 msg = (
                     f"The label '{entry.label}' already exists. It will be disambiguated based on "
                     "the configuration option: config.database.format.label_suffix"
                 )
                 LOGGER.warning(msg)
                 new_label = bib.disambiguate_label(entry.label, entry)
                 entry.label = new_label
 
             bib.update({entry.label: entry})
             existing_labels.add(entry.label)
-            new_entries[entry.label] = entry
+            self.new_entries[entry.label] = entry
 
-        Event.PostImportCommand.fire(new_entries)
-        bib.update(new_entries)
+        Event.PostImportCommand.fire(self)
+        bib.update(self.new_entries)
 
         bib.save()
-
-    @staticmethod
-    def tui(tui: cobib.tui.TUI) -> None:
-        # pdoc will inherit the docstring from the base class
-        # noqa: D102
-        LOGGER.debug("Import command triggered from TUI.")
-        # handle input via prompt
-        tui.execute_command("import")
-        # update database list
-        LOGGER.debug("Updating list after Import command.")
-        tui.viewport.update_list()
```

### Comparing `cobib-3.5.5/src/cobib/commands/init.py` & `cobib-4.0.0/src/cobib/commands/init.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,102 +5,118 @@
 Generally, you will only ever need to run this command once, but it is safe to run it multiple times
 (although it will likely have no effect).
 
 To get started with coBib you must run:
 ```
 cobib init
 ```
-This will initialize the database in the location specified by `config.database.file`.
+This will initialize the database in the location specified by
+`cobib.config.config.DatabaseConfig.file`.
 
-If you enabled the automatic git-integration of coBib via `config.database.git`, you must initialize
-this separately via:
+If you enabled the automatic git-integration of coBib via `cobib.config.config.DatabaseConfig.git`,
+you must initialize this separately via:
 ```
 cobib init --git
 ```
 If you have not run the first command yet, you can directly initialize the database *and* the
 git-integration by only running the second command.
+
+.. warning::
+   You can**not** run this command from the TUI, because the database must have already been
+   initialized *before* you can start the TUI in the first place.
 """
 
 from __future__ import annotations
 
-import argparse
 import logging
 import os
 import sys
-from typing import IO, TYPE_CHECKING, Any, List
+from pathlib import Path
+from typing import Type
+
+from rich.console import Console
+from rich.prompt import PromptBase
+from textual.app import App
+from typing_extensions import override
 
 from cobib.config import Event, config
 from cobib.utils.rel_path import RelPath
 
 from .base_command import ArgumentParser, Command
 
 LOGGER = logging.getLogger(__name__)
 
-if TYPE_CHECKING:
-    import cobib.tui
-
 
 class InitCommand(Command):
-    """The Init Command."""
+    """The Init Command.
 
-    name = "init"
+    This command can parse the following arguments:
 
-    def execute(self, args: List[str], out: IO[Any] = sys.stdout) -> None:
-        """Initializes the database.
+        * `-g`, `--git`: initializes the git-integration.
+    """
 
-        Initializes the YAML database in the location specified by `config.database.file`.
-        If you enabled `config.database.git` *and* you specify the `--git` command-line argument,
-        the git-integration will be initialized, too.
-
-        Args:
-            args: a sequence of additional arguments used for the execution. The following values
-                are allowed for this command:
-                    * `-g`, `--git`: initializes the git-integration.
-            out: the output IO stream. This defaults to `sys.stdout`.
-        """
-        LOGGER.debug("Starting Init command.")
+    name = "init"
+
+    @override
+    def __init__(
+        self,
+        *args: str,
+        console: Console | App[None] | None = None,
+        prompt: Type[PromptBase[str]] | None = None,
+    ) -> None:
+        super().__init__(*args, console=console, prompt=prompt)
+
+        self.file: Path
+        """The path to the database file."""
+
+        self.root: Path
+        """The parent directory where the database file resides. This is where the git repository
+        gets initialized (if the git integration was enabled)."""
+
+    @override
+    @classmethod
+    def init_argparser(cls) -> None:
         parser = ArgumentParser(prog="init", description="Init subcommand parser.")
         parser.add_argument("-g", "--git", action="store_true", help="initialize git repository")
+        cls.argparser = parser
 
-        try:
-            largs = parser.parse_args(args)
-        except argparse.ArgumentError as exc:
-            LOGGER.error(exc.message)
-            return
+    @override
+    def execute(self) -> None:
+        LOGGER.debug("Starting Init command.")
 
-        Event.PreInitCommand.fire(largs)
+        Event.PreInitCommand.fire(self)
 
-        file = RelPath(config.database.file).path
-        root = file.parent
+        self.file = RelPath(config.database.file).path
+        self.root = self.file.parent
 
-        file_exists = file.exists()
-        git_tracked = (root / ".git").exists()
+        file_exists = self.file.exists()
+        git_tracked = (self.root / ".git").exists()
 
         if file_exists:
             if git_tracked:
                 msg = (
                     "Database file already exists and is being tracked by git. There is nothing "
                     "else to do."
                 )
                 LOGGER.info(msg)
                 return
 
-            if not git_tracked and not largs.git:
+            if not git_tracked and not self.largs.git:
                 msg = "Database file already exists! Use --git to start tracking it with git."
                 LOGGER.warning(msg)
                 return
 
         else:
-            LOGGER.debug('Creating path for database file: "%s"', root)
-            root.mkdir(parents=True, exist_ok=True)
+            LOGGER.debug('Creating path for database file: "%s"', self.root)
+            self.root.mkdir(parents=True, exist_ok=True)
 
-            LOGGER.debug('Creating empty database file: "%s"', file)
-            open(file, "w", encoding="utf-8").close()  # pylint: disable=consider-using-with
+            LOGGER.debug('Creating empty database file: "%s"', self.file)
+            open(self.file, "w", encoding="utf-8").close()  # pylint: disable=consider-using-with
 
-        if largs.git:
+        if self.largs.git:
             if not config.database.git:
                 msg = (
                     "You are about to initialize the git tracking of your database, but this will "
                     "only have effect if you also enable the DATABASE/git setting in your "
                     "configuration file!"
                 )
                 LOGGER.warning(msg)
@@ -114,19 +130,12 @@
             if name_set != 0 or email_set != 0:
                 msg = (
                     "In order to use git you must configure your name and email first! For more "
                     "information please consult `man gittutorial`."
                 )
                 LOGGER.warning(msg)
                 sys.exit(1)
-            LOGGER.debug('Initializing git repository in "%s"', root)
-            os.system(f"git init {root}")
-            self.git(args=vars(largs), force=True)
-
-        Event.PostInitCommand.fire(root, file)
-
-    @staticmethod
-    def tui(tui: cobib.tui.TUI) -> None:
-        """🛑 This command is *not* available via the TUI.
+            LOGGER.debug('Initializing git repository in "%s"', self.root)
+            os.system(f"git init {self.root}")
+            self.git(force=True)
 
-        This is the case because the TUI cannot be started before the database has been initialized.
-        """
+        Event.PostInitCommand.fire(self)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cobib-3.5.5/src/cobib/commands/modify.py` & `cobib-4.0.0/src/cobib/commands/modify.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 r"""coBib's Modify command.
 
 This command allows you to perform bulk modification to multiple entries.
 Thus, it provides faster means to apply simple edits to many entries at once, without having to open
 each entry for editing one-by-one or having to edit the database file manually.
 
-A simple example is the following:
+It takes a modification in the form `<field>:<value>` and will overwrite the `field` of all matching
+entries with the new `value`. A simple example is the following:
 ```
 cobib modify tags:private --selection -- Label1 Label2 ...
 ```
 which will set the tags of all listed entries to `private`.
 
 You can use the `--add` option to not overwrite but append to existing values of a field. `str`
 fields will be concatenated with*out* any spaces, lists will be appended, and numeric fields will be
 added. Any other kind of field will be converted to a `str`.
 
-As with other commands, you can also use filters (see also `cobib.commands.list`) rather than a
+As with other commands, you can also use filters (see also `cobib.commands.list_`) rather than a
 manual selection to specify the entries which to modify:
 ```
 cobib modify tags:first_author -- ++author Rossmannek
 ```
 
 As of v3.2.0 the `value` provided as part of the modification is interpreted as an "f"-string.[^1]
 This means you can even use placeholder variables and perform simple operations on them. The
@@ -29,14 +30,21 @@
 # Rewrite the 'pages' field with a single-dash separator
 cobib modify "pages:{pages.replace('--', '-')}" -- ...
 
 # Rename an entry according to the first author's surname and year
 cobib modify "label:{author.split()[1]}{year}" -- ...
 ```
 
+In case you are applying a modification to your entry labels, but you want to avoid renaming all of
+your associated files, you can use the `--preserve-files` argument, like so:
+```
+# Rename an entry according to the first author's surname and year, but preserve the original file
+cobib modify "label:{author.split()[1]}{year}" --preserve-files -- ...
+```
+
 In combination with the regex-support for filters added during the same release, you can even unify
 your database's label convention:
 ```
 cobib modify "label:{label.replace('_', '')}" -- ++label "\D+_\d+"
 ```
 
 If you happen to use an undefined variable as part of your modification, coBib will handle this
@@ -51,173 +59,110 @@
 actually applying them.
 ```
 cobib modify --dry <modification> -- ...
 ```
 This is useful if you want to test large bulk modifications before running them in order to prevent
 mistakes.
 
-You can also trigger this command from the `cobib.tui.tui.TUI`.
+### TUI
+
+You can also trigger this command from the `cobib.ui.tui.TUI`.
 By default, it is bound to the `m` key which will drop you into the prompt where you can type out a
 normal command-line command:
 ```
 :modify <arguments go here>
 ```
 
 [^1]: <https://docs.python.org/3/reference/lexical_analysis.html#formatted-string-literals>
 """
 
 from __future__ import annotations
 
-import argparse
 import ast
 import logging
-import os
-import sys
-from typing import IO, TYPE_CHECKING, Any, Callable, Dict, List, Optional, Tuple
+from typing import Any, Callable, Dict, List, Optional, Tuple, Type
+
+from rich.console import Console
+from rich.prompt import PromptBase
+from textual.app import App
+from typing_extensions import override
 
 from cobib.config import Event
-from cobib.database import Database
+from cobib.database import Database, Entry
 from cobib.utils.logging import get_stream_handler
 from cobib.utils.rel_path import RelPath
 
 from .base_command import ArgumentParser, Command
-from .list import ListCommand
+from .list_ import ListCommand
 
 LOGGER = logging.getLogger(__name__)
 
-if TYPE_CHECKING:
-    import cobib.tui
 
+class ModifyCommand(Command):
+    """The Modify Command.
 
-def evaluate_ast_node(node: ast.expr, locals_: Optional[Dict[str, Any]] = None) -> str:
-    """Evaluates an AST node representing an f-string.
-
-    Args:
-        node: the AST expression extracted from an f-string.
-        locals_: the dictionary of local variables to be used as context for the expression
-            evaluation.
-
-    Returns:
-        The evaluated AST node expression.
-    """
-    try:
-        # pylint: disable=eval-used
-        return eval(  # type: ignore
-            compile(ast.Expression(node), filename="<string>", mode="eval"), locals_
-        )
-    except NameError as err:
-        LOGGER.warning("You tried use an undefined variable. Falling back to an empty string.")
-        LOGGER.error(err)
-        return ""
-
-
-def evaluate_as_f_string(value: str, locals_: Optional[Dict[str, Any]] = None) -> str:
-    """Evaluates a string as if it were a literal f-string.
-
-    Args:
-        value: the string to be evaluated.
-        locals_: the dictionary of local variables to be used as context for the expression
-            evaluation.
-
-    Returns:
-        The evaluated f-string.
-
-    Raises:
-        ValueError: if an unexpected AST component type is encountered.
+    This command can parse the following arguments:
 
-    References:
-        <https://stackoverflow.com/a/61190684>
+        * `modification`: a string conforming to `<field>:<value>` indicating the modification that
+          should be applied to all matching entries. By default, the modification will overwrite any
+          existing data in the specified `field` with the new `value`. For more information about
+          formatting options of `<value>` refer to the module documentation or the man-page.
+        * `--dry`: run in "dry"-mode which lists modifications without applying them.
+        * `-a`, `--add`: when specified, the modification's value will be added to the entry's field
+          rather than overwrite it. If the field in question is numeric, the numbers will be added.
+        * `--preserve-files`: skips the renaming of any associated files in case the applied
+            modification acted on the entry labels.
+        * `-s`, `--selection`: when specified, the positional arguments will *not* be interpreted as
+          filters but rather as a direct list of entry labels. This can be used on the command-line
+          but is mainly meant for the TUIs visual selection interface (hence the name).
+        * in addition to the above, you can add `filters` to specify a subset of your database for
+          exporting. For more information refer to `cobib.commands.list_`.
     """
-    result: List[str] = []
-    for part in ast.parse(f"f'''{value}'''").body[0].value.values:  # type: ignore
-        typ = type(part)
 
-        if typ is ast.Constant:
-            result.append(part.value)
-
-        elif typ is ast.Str:
-            # TODO: remove once support for Python 3.7 will be dropped
-            result.append(part.s)
-
-        elif typ is ast.FormattedValue:
-            value = evaluate_ast_node(part.value, locals_)
-
-            if part.conversion >= 0:
-                conversions: Dict[str, Callable[[Any], str]] = {"a": ascii, "r": repr, "s": str}
-                value = conversions[chr(part.conversion)](value)
-
-            if part.format_spec:
-                value = format(value, evaluate_ast_node(part.format_spec))
-
-            result.append(str(value))
-
-        else:
-            LOGGER.warning("Unexpected AST node expression type '%s' for an f-string.", typ)
-            raise ValueError
+    name = "modify"
 
-    return "".join(result)
+    @override
+    def __init__(
+        self,
+        *args: str,
+        console: Console | App[None] | None = None,
+        prompt: Type[PromptBase[str]] | None = None,
+    ) -> None:
+        super().__init__(*args, console=console, prompt=prompt)
 
-
-class ModifyCommand(Command):
-    """The Modify Command."""
-
-    name = "modify"
+        self.modified_entries: List[Entry] = []
+        """A list of `cobib.database.Entry` objects which were modified by this command."""
 
     @staticmethod
     def field_value_pair(string: str) -> Tuple[str, str]:
         """Utility method to assert the field-value pair argument type.
 
         This method is given to the `argparse.ArgumentParser` instance as its `type` specifier.
         An input argument is considered valid if it passes through this function without raising any
         errors, which means it conforms to the `<field>:<value>` notation.
 
         Args:
             string: the argument string to check.
+
+        Returns:
+            The pair of strings: `field` and `value`.
         """
         # try splitting the string into field and value, any errors will be handled by argparse
         field, *value = string.split(":")
         # NOTE: we split only the first field off in case the value contains f-string format
         # specifications
         return (field, ":".join(value))
 
-    # pylint: disable=too-many-branches,too-many-statements
-    def execute(self, args: List[str], out: IO[Any] = sys.stdout) -> None:
-        """Modifies multiple entries in bulk.
-
-        This command allows bulk modification of multiple entries.
-        It takes a modification in the form `<field>:<value>` and will overwrite the `field` of all
-        matching entries with the new `value`.
-        The entries can be specified as a manual selection (when using `--selection` or the visual
-        selection of the TUI) or through filters (see also `cobib.commands.list`).
-
-        Args:
-            args: a sequence of additional arguments used for the execution. The following values
-                are allowed for this command:
-                    * `modification`: a string conforming to `<field>:<value>` indicating the
-                      modification that should be applied to all matching entries. By default, the
-                      modification will overwrite any existing data in the specified `field` with
-                      the new `value`. For more information about formatting options of `<value>`
-                      refer to the module documentation or the man-page.
-                    * `--dry`: run in "dry"-mode which lists modifications without applying them.
-                    * `-a`, `--add`: when specified, the modification's value will be added to the
-                      entry's field rather than overwrite it. If the field in question is numeric,
-                      the numbers will be added.
-                    * `-s`, `--selection`: when specified, the positional arguments will *not* be
-                      interpreted as filters but rather as a direct list of entry labels. This can
-                      be used on the command-line but is mainly meant for the TUIs visual selection
-                      interface (hence the name).
-                    * in addition to the above, you can add `filters` to specify a subset of your
-                      database for exporting. For more information refer to `cobib.commands.list`.
-            out: the output IO stream. This defaults to `sys.stdout`.
-        """
-        LOGGER.debug("Starting Modify command.")
+    @override
+    @classmethod
+    def init_argparser(cls) -> None:
         parser = ArgumentParser(prog="modify", description="Modify subcommand parser.")
         parser.add_argument(
             "modification",
-            type=self.field_value_pair,
+            type=ModifyCommand.field_value_pair,
             help="Modification to apply to the specified entries."
             "\nThis argument must be a string formatted as <field>:<value> where field can be any "
             "field of the entries and value can be any string which should be placed in that "
             "field. Be sure to escape this field-value pair properly, especially if the value "
             "contains spaces.",
         )
         parser.add_argument(
@@ -228,80 +173,76 @@
         parser.add_argument(
             "-a",
             "--add",
             action="store_true",
             help="Adds to the modified field rather than overwriting it.",
         )
         parser.add_argument(
+            "--preserve-files", action="store_true", help="do not rename associated files"
+        )
+        parser.add_argument(
             "-s",
             "--selection",
             action="store_true",
             help="When specified, the `filter` argument will be interpreted as a list of entry "
             "labels rather than arguments for the `list` command.",
         )
         parser.add_argument(
             "filter",
             nargs="+",
             help="You can specify filters as used by the `list` command in order to select a "
             "subset of labels to be modified. To ensure this works as expected you should add the "
             "pseudo-argument '--' before the list of filters. See also `list --help` for more "
             "information.",
         )
-        parser.add_argument(
-            "--preserve-files", action="store_true", help="do not rename associated files"
-        )
+        cls.argparser = parser
 
-        if not args:
-            parser.print_usage(sys.stderr)
-            sys.exit(1)
-
-        try:
-            largs = parser.parse_intermixed_args(args)
-        except argparse.ArgumentError as exc:
-            LOGGER.error(exc.message)
-            return
+    # pylint: disable=too-many-branches
+    @override
+    def execute(self) -> None:
+        LOGGER.debug("Starting Modify command.")
 
-        Event.PreModifyCommand.fire(largs)
+        Event.PreModifyCommand.fire(self)
 
         info_handler: logging.Handler
-        if largs.dry:
+        if self.largs.dry:
             info_handler = get_stream_handler(logging.INFO)
 
             class ModifyInfoFilter(logging.Filter):
                 """A logging filter to only print ModifyCommand INFO messages."""
 
                 def filter(self, record: logging.LogRecord) -> bool:
                     return record.name == "cobib.commands.modify" and record.levelname == "INFO"
 
             info_handler.addFilter(ModifyInfoFilter())
             LOGGER.addHandler(info_handler)
 
-        if largs.selection:
+        if self.largs.selection:
             LOGGER.info("Selection given. Interpreting `filter` as a list of labels")
-            labels = largs.filter
+            labels = self.largs.filter
         else:
             LOGGER.debug("Gathering filtered list of entries to be modified.")
-            with open(os.devnull, "w", encoding="utf-8") as devnull:
-                labels = ListCommand().execute(largs.filter, out=devnull)
+            filtered_entries, _ = ListCommand(*self.largs.filter).filter_entries()
+            labels = [entry.label for entry in filtered_entries]
 
-        field, value = largs.modification
+        field, value = self.largs.modification
 
         bib = Database()
 
         for label in labels:  # pylint: disable=too-many-nested-blocks
             try:
                 entry = bib[label]
                 local_value = evaluate_as_f_string(value, {"label": label, **entry.data.copy()})
 
                 if hasattr(entry, field):
                     prev_value = getattr(entry, field, None)
                 else:
                     prev_value = entry.data.get(field, None)
 
-                if not largs.add:
+                if not self.largs.add:
                     new_value = local_value
                     if local_value.isnumeric():
                         new_value = int(local_value)  # type: ignore
                 else:
                     try:
                         if prev_value is None:
                             new_value = local_value
@@ -333,85 +274,140 @@
                 if new_value == prev_value:
                     LOGGER.info(
                         "New and previous values match. Skipping modification of entry '%s'.", label
                     )
                     continue
 
                 if hasattr(entry, field):
-                    if largs.dry:
+                    if self.largs.dry:
                         LOGGER.info(
                             "%s: changing field '%s' from %s to %s",
                             entry.label,
                             field,
                             getattr(entry, field),
                             new_value,
                         )
                     setattr(entry, field, new_value)
                 else:
-                    if largs.dry:
+                    if self.largs.dry:
                         LOGGER.info(
                             "%s: adding field '%s' = %s",
                             entry.label,
                             field,
                             new_value,
                         )
                     entry.data[field] = new_value
 
                 bib.update({entry.label: entry})
 
                 if entry.label != label:
                     bib.rename(label, entry.label)
-                    if not largs.preserve_files:
+                    if not self.largs.preserve_files:
                         new_files = []
                         for file in entry.file:
                             path = RelPath(file)
                             if path.path.stem == label:
                                 LOGGER.info("Also renaming associated file '%s'.", str(path))
                                 target = RelPath(path.path.parent / f"{entry.label}.pdf")
                                 if target.path.exists():
                                     LOGGER.warning(
                                         "Found conflicting file, not renaming '%s'.", str(path)
                                     )
                                 else:
-                                    if largs.dry:
+                                    if self.largs.dry:
                                         LOGGER.info(
                                             "%s: renaming associated file '%s' to '%s'",
                                             entry.label,
                                             path.path,
                                             target.path,
                                         )
                                     else:
                                         path.path.rename(target.path)
                                         new_files.append(str(target))
                                     continue
-                            if not largs.dry:
+                            if not self.largs.dry:
                                 new_files.append(file)
-                        if not largs.dry and new_files:
+                        if not self.largs.dry and new_files:
                             entry.file = new_files
 
-                if not largs.dry:
+                if not self.largs.dry:
+                    self.modified_entries.append(entry)
                     msg = f"'{label}' was modified."
                     LOGGER.info(msg)
             except KeyError:
                 msg = f"No entry with the label '{label}' could be found."
                 LOGGER.warning(msg)
 
-        Event.PostModifyCommand.fire(labels, largs.dry)
+        Event.PostModifyCommand.fire(self)
 
-        if largs.dry:
+        if self.largs.dry:
             LOGGER.removeHandler(info_handler)
             # read also functions as a restoring method
             bib.read()
         else:
             bib.save()
-            self.git(args=vars(largs))
+            self.git()
+
+
+def evaluate_ast_node(node: ast.expr, locals_: Optional[Dict[str, Any]] = None) -> str:
+    """Evaluates an AST node representing an f-string.
+
+    Args:
+        node: the AST expression extracted from an f-string.
+        locals_: the dictionary of local variables to be used as context for the expression
+            evaluation.
+
+    Returns:
+        The evaluated AST node expression.
+    """
+    try:
+        # pylint: disable=eval-used
+        return eval(  # type: ignore
+            compile(ast.Expression(node), filename="<string>", mode="eval"), locals_
+        )
+    except NameError as err:
+        LOGGER.warning("You tried use an undefined variable. Falling back to an empty string.")
+        LOGGER.error(err)
+        return ""
+
+
+def evaluate_as_f_string(value: str, locals_: Optional[Dict[str, Any]] = None) -> str:
+    """Evaluates a string as if it were a literal f-string.
+
+    Args:
+        value: the string to be evaluated.
+        locals_: the dictionary of local variables to be used as context for the expression
+            evaluation.
+
+    Returns:
+        The evaluated f-string.
+
+    Raises:
+        ValueError: if an unexpected AST component type is encountered.
+
+    References:
+        <https://stackoverflow.com/a/61190684>
+    """
+    result: List[str] = []
+    for part in ast.parse(f"f'''{value}'''").body[0].value.values:  # type: ignore
+        typ = type(part)
+
+        if typ is ast.Constant:
+            result.append(part.value)
+
+        elif typ is ast.FormattedValue:
+            value = evaluate_ast_node(part.value, locals_)
+
+            if part.conversion >= 0:
+                conversions: Dict[str, Callable[[Any], str]] = {"a": ascii, "r": repr, "s": str}
+                value = conversions[chr(part.conversion)](value)
+
+            if part.format_spec:
+                value = format(value, evaluate_ast_node(part.format_spec))
+
+            result.append(str(value))
 
-    @staticmethod
-    def tui(tui: cobib.tui.TUI) -> None:
-        # pdoc will inherit the docstring from the base class
-        # noqa: D102
-        LOGGER.debug("Modify command triggered from TUI.")
-        # handle input via prompt
-        if tui.selection:
-            tui.execute_command("modify -s", pass_selection=True)
         else:
-            tui.execute_command("modify")
+            LOGGER.warning("Unexpected AST node expression type '%s' for an f-string.", typ)
+            raise ValueError
+
+    return "".join(result)
```

### Comparing `cobib-3.5.5/src/cobib/commands/open.py` & `cobib-4.0.0/src/cobib/commands/open.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,112 +1,103 @@
 """coBib's Open command.
 
-This command can be used to open associated files of an entry.
+This command can be used to open associated file(s) of one (or multiple) entries.
 ```
 cobib open <label 1> [<label 2> ...]
 ```
 
 The keys of `cobib.database.Entry.data` which are queried for paths or URL strings can be configured
-via the `config.commands.open.fields` setting (defaulting to `["file", "url"]`).
+via the `cobib.config.config.OpenCommandConfig.fields` setting (defaulting to `["file", "url"]`).
 If one such string is found, it is automatically opened with the program configured by
-`config.commands.open.command`.
+`cobib.config.config.OpenCommandConfig.command`.
 If multiple matches are found, the user will be presented with a menu to choose one or multiple
 matches.
 
 This menu will look similar to the following after querying for `help`:
 ```
-You can specify one of the following options:
-  1. a url number
-  2. a field name provided in '[...]'
-  3. or simply 'all'
-  4. ENTER will abort the command
+Multiple targets were found. You may select the following:
+  1. an individual URL number
+  2. a target type (provided in '[...]')
+  3. 'all'
+  4. or 'cancel' to abort the command
 
   1: [file] /path/to/a/file.pdf
   2: [file] /path/to/another/file.pdf
   3: [url] https://example.org/
-Entry to open [Type 'help' for more info]:
+[all,help,cancel]:
 ```
 
 With the above options, here is what will happen depending on the users choice:
 * `1`, `2`, or `3`: will open the respective file or URL.
 * `file` or `url`: will open the respective group.
 * `all`: will open all matches.
 * `help`: will print the detailed help-menu again.
-* `ENTER`: will abort the command.
+* `cancel`: will abort the command.
 
-You can also trigger this command from the `cobib.tui.tui.TUI`.
+### TUI
+
+You can also trigger this command from the `cobib.ui.tui.TUI`.
 By default, it is bound to the `o` key.
 """
 
 from __future__ import annotations
 
-import argparse
 import logging
 import os
 import subprocess
-import sys
+import warnings
 from collections import defaultdict
-from typing import IO, TYPE_CHECKING, Any, Dict, List
+from functools import wraps
+from typing import Callable, cast
 from urllib.parse import ParseResult, urlparse
 
+from rich.console import Console
+from rich.prompt import InvalidResponse, Prompt, PromptBase, PromptType
+from rich.text import Text
+from textual.app import App
+from typing_extensions import override
+
 from cobib.config import Event, config
 from cobib.database import Database
 from cobib.utils.rel_path import RelPath
 
 from .base_command import ArgumentParser, Command
 
 LOGGER = logging.getLogger(__name__)
 
-if TYPE_CHECKING:
-    import cobib.tui
-
 
 class OpenCommand(Command):
-    """The Open Command."""
+    """The Open Command.
 
-    name = "open"
+    This command can parse the following arguments:
 
-    # pylint: disable=too-many-branches
-    def execute(self, args: List[str], out: IO[Any] = sys.stderr) -> None:
-        """Opens associated files of an entry.
-
-        This command opens the associated file(s) of one (or multiple) entries.
-        It does so by querying the `file` and `url` fields of `cobib.database.Entry.data`.
-        If multiple such files are found, the user is presented with a menu allowing him to choose
-        one or multiple files to be opened.
+        * `labels`: one (or multiple) labels of the entries to be opened.
+    """
 
-        The command for opening can be configured via `config.commands.open.command`.
+    name = "open"
 
-        Args:
-            args: a sequence of additional arguments used for the execution. The following values
-                are allowed for this command:
-                    * `labels`: one (or multiple) labels of the entries to be opened.
-            out: the output IO stream. This defaults to `sys.stdout`.
-        """
-        LOGGER.debug("Starting Open command.")
+    @override
+    @classmethod
+    def init_argparser(cls) -> None:
         parser = ArgumentParser(prog="open", description="Open subcommand parser.")
         parser.add_argument("labels", type=str, nargs="+", help="labels of the entries")
+        cls.argparser = parser
 
-        if not args:
-            parser.print_usage(sys.stderr)
-            sys.exit(1)
-
-        try:
-            largs = parser.parse_args(args)
-        except argparse.ArgumentError as exc:
-            LOGGER.error(exc.message)
-            return
+    # TODO: can we make the implementation cleaner and avoid the type ignore comment below?
+    @override
+    async def execute(self) -> None:  # type: ignore[override]
+        # pylint: disable=invalid-overridden-method
+        LOGGER.debug("Starting Open command.")
 
-        Event.PreOpenCommand.fire(largs)
+        Event.PreOpenCommand.fire(self)
 
         bib = Database()
 
-        # pylint: disable=too-many-nested-blocks
-        for label in largs.labels:
-            things_to_open: Dict[str, List[ParseResult]] = defaultdict(list)
+        for label in self.largs.labels:
+            things_to_open: dict[str, list[ParseResult]] = defaultdict(list)
             count = 0
             # first: find all possible things to open
             try:
                 entry = bib[label]
                 for field in config.commands.open.fields:
                     if field in entry.data.keys() and entry.data[field]:
                         value = entry.data[field]
@@ -129,86 +120,121 @@
                 continue
 
             if count == 1:
                 # we found a single URL to open
                 self._open_url(list(things_to_open.values())[0][0])
             else:
                 # we query the user what to do
-                idx = 1
-                url_list = []
-                prompt: List[str] = []
+                idx = 0
+                url_list: list[ParseResult] = []
+                prompt_text = Text()
+                choices = ["all"] + config.commands.open.fields + ["help", "cancel"]
+
                 # print formatted list of available URLs
                 for field, urls in things_to_open.items():
                     for url in urls:
-                        prompt.append(f"{idx:3}: [{field}] {url.geturl()}")
-                        url_list.append(url)
                         idx += 1
-                # loop until the user picks a valid choice
-                help_requested = False
-                while True:
-                    prompt_copy = prompt.copy()
-                    prompt_copy.append("Entry to open [Type 'help' for more info]: ")
-                    try:
-                        choice = input("\n".join(prompt_copy)).strip()
-                    except EOFError:
-                        choice = ""
-                    if not choice:
-                        # empty input
-                        msg = "User aborted open command."
-                        LOGGER.warning(msg)
-                        break
-                    if choice == "help":
-                        LOGGER.debug("User requested help.")
-                        if not help_requested:
-                            prompt = [
-                                "You can specify one of the following options:",
-                                "  1. a url number",
-                                "  2. a field name provided in '[...]'",
-                                "  3. or simply 'all'",
-                                "  4. ENTER will abort the command",
-                                "",
-                            ] + prompt
-                        help_requested = True
-                    elif choice == "all":
-                        LOGGER.debug("User selected all urls.")
-                        for url in url_list:
-                            self._open_url(url)
-                        break
-                    elif choice in things_to_open.keys():
-                        LOGGER.debug("User selected the %s set of urls.", choice)
-                        for url in things_to_open[choice]:
-                            self._open_url(url)
-                        break
-                    elif choice.isdigit() and int(choice) > 0 and int(choice) <= count:
-                        LOGGER.debug("User selected url %s", choice)
-                        self._open_url(url_list[int(choice) - 1])
-                        break
+                        url_list.append(url)
+                        choices.append(str(idx))
+                        prompt_text.append(f"{idx:3}", "prompt.choices")
+                        prompt_text.append(": [")
+                        prompt_text.append(field, "prompt.choices")
+                        prompt_text.append(f"] {url.geturl()}\n")
+                prompt_text.append("[all,help,cancel]", "prompt.choices")
+
+                # pylint: disable=line-too-long
+                self.prompt.process_response = self._wrap_prompt_process_response(  # type: ignore[method-assign]
+                    self.prompt.process_response  # type: ignore[assignment]
+                )
+                if self.prompt is not Prompt:
+                    choice = await self.prompt.ask(  # type: ignore[call-overload]
+                        prompt_text,
+                        choices=choices,
+                        show_choices=False,
+                        console=cast(App[None], self.console),
+                    )
+                else:
+                    choice = self.prompt.ask(
+                        prompt_text,
+                        choices=choices,
+                        show_choices=False,
+                        console=cast(Console, self.console),
+                    )
 
-        Event.PostOpenCommand.fire(largs.labels)
+                self.prompt.process_response = (  # type: ignore[method-assign]
+                    self.prompt.process_response.__wrapped__  # type: ignore[attr-defined]
+                )
+
+                if choice == "cancel":
+                    LOGGER.warning("User aborted open command.")
+                elif choice == "all":
+                    LOGGER.debug("User selected all urls.")
+                    for url in url_list:
+                        self._open_url(url)
+                elif choice in things_to_open.keys():
+                    LOGGER.debug("User selected the %s set of urls.", choice)
+                    for url in things_to_open[choice]:
+                        self._open_url(url)
+                elif choice.isdigit():
+                    LOGGER.debug("User selected url %s", choice)
+                    self._open_url(url_list[int(choice) - 1])
+
+        Event.PostOpenCommand.fire(self)
 
     @staticmethod
     def _open_url(url: ParseResult) -> None:
-        """Opens a URL."""
+        """Opens a URL.
+
+        Args:
+            url: the URL to be opened.
+        """
         opener = config.commands.open.command
         try:
             url_str: str = url.geturl() if url.scheme else str(RelPath(url.geturl()).path)
             LOGGER.debug('Opening "%s" with %s.', url_str, opener)
             with open(os.devnull, "w", encoding="utf-8") as devnull:
-                subprocess.Popen(  # pylint: disable=consider-using-with
-                    [opener, url_str], stdout=devnull, stderr=devnull, stdin=devnull, close_fds=True
-                )
+                with warnings.catch_warnings():
+                    warnings.filterwarnings("ignore", category=ResourceWarning)
+                    subprocess.Popen(  # pylint: disable=consider-using-with
+                        [opener, url_str],
+                        stdout=devnull,
+                        stderr=devnull,
+                        stdin=devnull,
+                        close_fds=True,
+                    )
         except FileNotFoundError as err:
             LOGGER.error(err)
 
     @staticmethod
-    def tui(tui: cobib.tui.TUI) -> None:
-        # pdoc will inherit the docstring from the base class
-        # noqa: D102
-        LOGGER.debug("Open command triggered from TUI.")
-        if tui.selection:
-            # use selection for command
-            labels = list(tui.selection)
-        else:
-            # get current label
-            label, _ = tui.viewport.get_current_label()
-            labels = [label]
-        tui.execute_command(["open"] + labels, skip_prompt=True)
+    def _wrap_prompt_process_response(
+        func: Callable[[PromptBase[PromptType], str], PromptType]
+    ) -> Callable[[PromptBase[PromptType], str], PromptType]:
+        """A method to wrap a `PromptBase.process_response` method.
+
+        This method wraps a `PromptBase.process_response` method in order to handle a user's request
+        for additional help.
+
+        Args:
+            func: the `PromptBase.process_response` method to be wrapped.
+
+        Returns:
+            The wrapped `PromptBase.process_response` method.
+        """
+
+        @override
+        @wraps(func)
+        def process_response(prompt: PromptBase[PromptType], value: str) -> PromptType:
+            return_value: PromptType = func(prompt, value)
+
+            if return_value == "help":
+                LOGGER.debug("User requested help.")
+                raise InvalidResponse(
+                    "[yellow]Multiple targets were found. You may select the following:\n"
+                    "  1. an individual URL number\n"
+                    "  2. a target type (provided in '[...]')\n"
+                    "  3. 'all'\n"
+                    "  4. or 'cancel' to abort the command"
+                )
+
+            return return_value
+
+        return process_response
```

### Comparing `cobib-3.5.5/src/cobib/commands/redo.py` & `cobib-4.0.0/src/cobib/commands/redo.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,125 +1,134 @@
 """coBib's Redo command.
 
-This command can be used to re-apply the changes *of a previously undone* command:
+This command can be used to re-apply the changes *of a previously undone* command (see
+`cobib.commands.undo`):
 ```
 cobib redo
 ```
 This command takes *no* additional arguments!
 
 Note, that if you have not used `cobib undo` previously, this command will have no effect!
 
-Furthermore, this command is *only* available if coBib's git-integration has been enabled and
-initialized.
-Refer to the documentation of `cobib.commands.init.InitCommand` for more details on that topic.
+.. warning::
+   This command is *only* available if coBib's git-integration has been enabled via
+   `cobib.config.config.DatabaseConfig.git` *and* initialized properly (see `cobib.commands.init`).
 
-You can also trigger this command from the `cobib.tui.tui.TUI`.
+### TUI
+
+You can also trigger this command from the `cobib.ui.tui.TUI`.
 By default, it is bound to the `r` key.
 """
 
 from __future__ import annotations
 
-import argparse
 import logging
 import subprocess
 import sys
-from typing import IO, TYPE_CHECKING, Any, List
+from pathlib import Path
+from typing import Type
+
+from rich.console import Console
+from rich.prompt import PromptBase
+from textual.app import App
+from typing_extensions import override
 
 from cobib.config import Event, config
 from cobib.database import Database
 from cobib.utils.rel_path import RelPath
 
 from .base_command import ArgumentParser, Command
 
 LOGGER = logging.getLogger(__name__)
 
-if TYPE_CHECKING:
-    import cobib.tui
-
 
 class RedoCommand(Command):
-    """The Redo Command."""
+    """The Redo Command.
+
+    This command does not parse any additional arguments.
+    """
 
     name = "redo"
 
-    def execute(self, args: List[str], out: IO[Any] = sys.stdout) -> None:
-        """Redoes the last undone change.
+    @override
+    def __init__(
+        self,
+        *args: str,
+        console: Console | App[None] | None = None,
+        prompt: Type[PromptBase[str]] | None = None,
+    ) -> None:
+        super().__init__(*args, console=console, prompt=prompt)
+
+        self.root: Path
+        """The path to the root of the git repository tracking the database."""
+
+        self.sha: str
+        """The git commit SHA which was reverted by this command."""
+
+    @override
+    @classmethod
+    def init_argparser(cls) -> None:
+        parser = ArgumentParser(prog="redo", description="Redo subcommand parser.")
+        cls.argparser = parser
 
-        This command is *only* available if coBib's git-integration has been enabled via
-        `config.database.git` *and* initialized properly (see `cobib.commands.init.InitCommand`).
-        If that is the case, this command will re-apply the changes *of a previously undone* command
-        (see `cobib.commands.undo.UndoCommand`).
-
-        Args:
-            args: a sequence of additional arguments used for the execution. The following values
-                are allowed for this command:
-                    * **no** additional arguments are required for this subcommand!
-            out: the output IO stream. This defaults to `sys.stdout`.
-        """
+    @override
+    def execute(self) -> None:
         git_tracked = config.database.git
         if not git_tracked:
             msg = (
                 "You must enable coBib's git-tracking in order to use the `Redo` command."
                 "\nPlease refer to the man-page for more information on how to do so."
             )
             LOGGER.error(msg)
             return
 
         file = RelPath(config.database.file).path
-        root = file.parent
-        if not (root / ".git").exists():
+        self.root = file.parent
+        if not (self.root / ".git").exists():
             msg = (
                 "You have configured, but not initialized coBib's git-tracking."
                 "\nPlease consult `cobib init --help` for more information on how to do so."
             )
             LOGGER.error(msg)
             return
 
         LOGGER.debug("Starting Redo command.")
-        parser = ArgumentParser(prog="redo", description="Redo subcommand parser.")
-
-        try:
-            # pylint: disable=unused-variable
-            largs = parser.parse_args(args)
-        except argparse.ArgumentError as exc:
-            LOGGER.error(exc.message)
-            return
 
-        Event.PreRedoCommand.fire(largs)
+        Event.PreRedoCommand.fire(self)
 
         LOGGER.debug("Obtaining git log.")
         lines = subprocess.check_output(
             [
                 "git",
                 "--no-pager",
                 "-C",
-                f"{root}",
+                f"{self.root}",
                 "log",
                 "--oneline",
                 "--no-decorate",
                 "--no-abbrev",
             ]
         )
         redone_shas = set()
         for commit in lines.decode().strip().split("\n"):
             LOGGER.debug("Processing commit %s", commit)
-            sha, *message = commit.split()
+            self.sha, *message = commit.split()
             if message[0] == "Redo":
                 # Store already redone commit sha
                 LOGGER.debug("Storing redone commit sha: %s", message[-1])
                 redone_shas.add(message[-1])
                 continue
-            if sha in redone_shas:
-                LOGGER.info("Skipping %s as it was already redone", sha)
+            if self.sha in redone_shas:
+                LOGGER.info("Skipping %s as it was already redone", self.sha)
                 continue
             if message[0] == "Undo":
-                LOGGER.debug("Attempting to redo %s.", sha)
+                LOGGER.debug("Attempting to redo %s.", self.sha)
                 commands = [
-                    f"git -C {root} revert --no-commit {sha}",
-                    f"git -C {root} commit --no-gpg-sign --quiet --message 'Redo {sha}'",
+                    f"git -C {self.root} revert --no-commit {self.sha}",
+                    f"git -C {self.root} commit --no-gpg-sign --quiet --message 'Redo {self.sha}'",
                 ]
                 with subprocess.Popen(
                     "; ".join(commands), shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE
                 ) as redo:
                     redo.communicate()
                     if redo.returncode != 0:
                         LOGGER.error(  # pragma: no cover
@@ -131,18 +140,8 @@
                         Database().read()
                 break
         else:
             msg = "Could not find a commit to redo. You must have undone something first!"
             LOGGER.warning(msg)
             sys.exit(1)
 
-        Event.PostRedoCommand.fire(root, sha)
-
-    @staticmethod
-    def tui(tui: cobib.tui.TUI) -> None:
-        # pdoc will inherit the docstring from the base class
-        # noqa: D102
-        LOGGER.debug("Redo command triggered from TUI.")
-        tui.execute_command(["redo"], skip_prompt=True)
-        # update database list
-        LOGGER.debug("Updating list after Redo command.")
-        tui.viewport.update_list()
+        Event.PostRedoCommand.fire(self)
```

### Comparing `cobib-3.5.5/src/cobib/commands/search.py` & `cobib-4.0.0/src/cobib/commands/search.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """coBib's Search command.
 
-This command allows you to search your database for a regex-interpreted query.
-While doing so, it uses the `config.commands.search.grep` tool to search associated files, too.
+This command allows you to search your database for one or more regex-interpreted queries.
+While doing so, it uses the `cobib.config.config.SearchCommandConfig.grep` tool to search associated
+files, too.
 
 As a simple example, you can query for a simple author name like so:
 ```
 cobib search Einstein
 ```
 You can make the search case *in*sensitive in two ways:
-1. By enabling `config.commands.search.ignore_case`.
+
+1. By enabling `cobib.config.config.SearchCommandConfig.ignore_case`.
+
 2. By providing the `--ignore-case` command-line argument:
 ```
 cobib search --ignore-case Einstein
 ```
 
 By default, the search command will provide you with 1 line of context above and below the actual
 matches. You can change this number of lines by setting the `--context` option:
@@ -24,78 +27,98 @@
 to a subset of your database:
 ```
 cobib search Einstein -- ++year 2020
 ```
 Note, that we use the auxiliary `--` argument to separate the filters from the actual arguments.
 While this is not strictly necessary it helps to disambiguate the origin of the arguments.
 
-You can also trigger this command from the `cobib.tui.tui.TUI`.
+### Associated files
+
+The search will also be performed on any associated files of your entries.
+You can configure the tool which is used to perform this search via the
+`cobib.config.config.SearchCommandConfig.grep` setting (defaults to `grep`).
+
+### TUI
+
+You can also trigger this command from the `cobib.ui.tui.TUI`.
 By default, it is bound to the `/` key.
+
+.. note::
+   For more information on the searching mechanisms see also `cobib.database.Entry.search`.
 """
 
 from __future__ import annotations
 
 import argparse
 import logging
-import os
-import re
-import shlex
-import sys
-from typing import IO, TYPE_CHECKING, Any, List, Optional, Tuple
+from typing import List, Type
+
+from rich.console import Console, ConsoleRenderable
+from rich.prompt import PromptBase
+from rich.text import Text
+from rich.tree import Tree as RichTree
+from textual.app import App
+from textual.widgets import Tree as TextualTree
+from typing_extensions import override
 
 from cobib import __version__
 from cobib.config import Event, config
-from cobib.database import Database
+from cobib.database import Entry
 
 from .base_command import ArgumentParser, Command
-from .list import ListCommand
+from .list_ import ListCommand
 
 LOGGER = logging.getLogger(__name__)
 
-if TYPE_CHECKING:
-    import cobib.tui
-
 
 class SearchCommand(Command):
-    """The Search Command."""
+    """The Search Command.
+
+    This command can parse the following arguments:
+
+        * `query`: the required positional argument corresponds to the regex-interpreted text which
+          will be searched for. You may provide multiple separate queries which will be searched for
+          independently.
+        * `-i`, `--ignore-case`: if specified, the search will be case *in*sensitive. You can enable
+          this setting permanently with `cobib.config.config.SearchCommandConfig.ignore_case`.
+        * `-c`, `--context`: you can specify the number of lines of "context" which is the number of
+          lines before and after the actual match to be included in the output. This is similar to
+          the `-C` option of `grep`.
+        * in addition to the above, you can add `filters` to narrow the search down to a subset of
+          your database. For more information refer to `cobib.commands.list_`.
+    """
 
     name = "search"
 
-    def execute(
-        self, args: List[str], out: Optional[IO[Any]] = None
-    ) -> Optional[Tuple[int, List[str]]]:
-        """Searches in the database.
-
-        This command searches the database for a regex-interpreted query.
-        It leverages `cobib.database.Entry.search` to perform the actual search.
-
-        You can configure the search-tool which searches through associated files via
-        `config.commands.search.grep`.
-
-        Args:
-            args: a sequence of additional arguments used for the execution. The following values
-                are allowed for this command:
-                    * `query`: the required positional argument corresponds to the regex-interpreted
-                      text which will be searched for.
-                    * `-i`, `--ignore-case`: if specified, the search will be case *in*sensitive.
-                      You can enable this setting permanently with
-                      `config.commands.search.ignore_case`.
-                    * `-c`, `--context`: you can specify the number of lines of "context" which
-                      is the number of lines before and after the actual match to be included in the
-                      output. This is similar to `grep`s `-C` option.
-                    * in addition to the above, you can add `filters` to narrow the search down to a
-                      subset of your database. For more information refer to `cobib.commands.list`.
-            out: the output IO stream. This defaults to `None`.
-
-        Returns:
-            A tuple containing the number of hits and matching labels.
-        """
-        LOGGER.debug("Starting Search command.")
+    @override
+    def __init__(
+        self,
+        *args: str,
+        console: Console | App[None] | None = None,
+        prompt: Type[PromptBase[str]] | None = None,
+    ) -> None:
+        super().__init__(*args, console=console, prompt=prompt)
+
+        self.entries: List[Entry] = []
+        """A filtered list of entries searched over by this command."""
+
+        self.matches: List[List[List[str]]] = []
+        """The search matches detected by this command. This is a nested list of the following
+        structure: the first list level iterates over the entries; the second list level iterates
+        over the matches of any given entry; the third list level iterates the (context) lines of
+        any given match."""
+
+        self.hits: int = 0
+        """The number of search hits detected by this command."""
+
+    @override
+    @classmethod
+    def init_argparser(cls) -> None:
         parser = ArgumentParser(prog="search", description="Search subcommand parser.")
-        parser.add_argument("query", type=str, help="text to search for")
+        parser.add_argument("query", type=str, nargs="+", help="text to search for")
         parser.add_argument(
             "-i", "--ignore-case", action="store_true", help="ignore case for searching"
         )
         parser.add_argument(
             "-c",
             "--context",
             type=int,
@@ -106,110 +129,124 @@
             "filter",
             nargs="*",
             help="You can specify filters as used by the `list` command in order to select a "
             "subset of labels to be modified. To ensure this works as expected you should add the "
             "pseudo-argument '--' before the list of filters. See also `list --help` for more "
             "information.",
         )
+        cls.argparser = parser
 
-        if not args:
-            parser.print_usage(sys.stderr)
-            sys.exit(1)
-
-        try:
-            largs = parser.parse_intermixed_args(args)
-        except argparse.ArgumentError as exc:
-            LOGGER.error(exc.message)
-            return None
-
-        Event.PreSearchCommand.fire(largs)
-
-        with open(os.devnull, "w", encoding="utf-8") as devnull:
-            labels = ListCommand().execute(largs.filter, out=devnull)
-        if labels is None:
-            return None  # pragma: no cover
-        LOGGER.debug("Available entries to search: %s", labels)
+    @override
+    @classmethod
+    def _parse_args(cls, args: tuple[str, ...]) -> argparse.Namespace:
+        search_args = []
+        filter_args = []
+        found_sep = False
+        for arg in args:
+            if arg == "--":
+                found_sep = True
+                continue
+            if found_sep:
+                filter_args.append(arg)
+            else:
+                search_args.append(arg)
 
-        ignore_case = config.commands.search.ignore_case or largs.ignore_case
-        re_flags = re.IGNORECASE if ignore_case else 0
-        LOGGER.debug("The search will be performed case %ssensitive", "in" if ignore_case else "")
+        largs = super()._parse_args(tuple(search_args))
+        largs.filter = filter_args
+        return largs
 
-        bib = Database()
+    @override
+    def execute(self) -> None:
+        LOGGER.debug("Starting Search command.")
 
-        hits = 0
-        output = []
-        for label in labels.copy():
-            entry = bib[label]
-            matches = entry.search(largs.query, largs.context, ignore_case)
+        Event.PreSearchCommand.fire(self)
+
+        self.entries, _ = ListCommand(*self.largs.filter).filter_entries()
+
+        ignore_case = config.commands.search.ignore_case or self.largs.ignore_case
+        LOGGER.debug("The search will be performed case %ssensitive", "in" if ignore_case else "")
+
+        for entry in self.entries.copy():
+            matches = entry.search(self.largs.query, self.largs.context, ignore_case)
             if not matches:
-                labels.remove(label)
+                self.entries.remove(entry)
                 continue
 
-            hits += len(matches)
-            LOGGER.debug('Entry "%s" includes %d hits.', label, hits)
-            title = f"{label} - {len(matches)} match" + ("es" if len(matches) > 1 else "")
-            title = title.replace(label, config.get_ansi_color("search_label") + label + "\x1b[0m")
+            self.matches.append(matches)
+            self.hits += len(matches)
+
+            LOGGER.debug('Entry "%s" includes %d hits.', entry.label, len(matches))
+
+        Event.PostSearchCommand.fire(self)
+
+    @override
+    def render_porcelain(self) -> List[str]:
+        output = []
+        for entry, matches in zip(self.entries, self.matches):
+            title = f"{entry.label}::{len(matches)}"
             output.append(title)
 
             for idx, match in enumerate(matches):
                 for line in match:
-                    line = re.sub(
-                        rf"({largs.query})",
-                        config.get_ansi_color("search_query") + r"\1" + "\x1b[0m",
-                        line,
-                        flags=re_flags,
-                    )
-                    output.append(f"[{idx+1}]\t".expandtabs(8) + line)
+                    output.append(f"{idx+1}::" + line.strip())
+
+        return output
+
+    @override
+    def render_rich(self) -> ConsoleRenderable:
+        ignore_case = config.commands.search.ignore_case or self.largs.ignore_case
+
+        tree = RichTree(".", hide_root=True)
+        for entry, matches in zip(self.entries, self.matches):
+            subtree = tree.add(
+                Text.assemble(
+                    (entry.label, config.commands.search.highlights.label),
+                    f" - {len(matches)} match" + ("es" if len(matches) > 1 else ""),
+                )
+            )
 
-        print("\n".join(output), file=out)
+            for idx, match in enumerate(matches):
+                matchtree = subtree.add(str(idx + 1))
+                for line in match:
+                    line_text = Text(line)
+                    line_text.highlight_words(
+                        self.largs.query,
+                        config.commands.search.highlights.query,
+                        case_sensitive=not ignore_case,
+                    )
+                    matchtree.add(line_text)
 
-        Event.PostSearchCommand.fire(hits, labels)
+        return tree
 
-        return (hits, labels)
+    @override
+    def render_textual(self) -> TextualTree[Text]:
+        ignore_case = config.commands.search.ignore_case or self.largs.ignore_case
+
+        # TODO: figure out how to deal with multi-line tree node contents
+        tree: TextualTree[Text] = TextualTree(".")
+        tree.show_root = False
+        for entry, matches in zip(self.entries, self.matches):
+            subtree = tree.root.add(
+                Text.assemble(
+                    (entry.label, config.commands.search.highlights.label),
+                    f" - {len(matches)} match" + ("es" if len(matches) > 1 else ""),
+                ),
+                # TODO: make configurable
+                expand=False,
+            )
 
-    @staticmethod
-    def tui(tui: cobib.tui.TUI) -> None:
-        # pdoc will inherit the docstring from the base class
-        # noqa: D102
-        LOGGER.debug("Search command triggered from TUI.")
-        tui.viewport.clear()
-        # handle input via prompt
-        command, results = tui.execute_command("search", out=tui.viewport.buffer)  # type: ignore
-        if tui.viewport.buffer.lines and results is not None:
-            hits, labels = results
-            tui.STATE.mode = "search"
-            cur_y, _ = tui.viewport.pad.getyx()
-            tui.STATE.previous_line = cur_y
-            tui.viewport.buffer.split()
-            LOGGER.debug("Applying selection highlighting in search results.")
-            for label in labels:
-                if label not in tui.selection:
-                    continue
-                # we match the label including its 'search_label' highlight to ensure that we really
-                # only match this specific occurrence of whatever the label may be
-                tui.viewport.buffer.replace(
-                    range(tui.viewport.buffer.height),
-                    re.escape(config.get_ansi_color("search_label")) + label + re.escape("\x1b[0m"),
-                    config.get_ansi_color("search_label")
-                    + config.get_ansi_color("selection")
-                    + label
-                    + "\x1b[0m\x1b[0m",
+            for idx, match in enumerate(matches):
+                matchtree = subtree.add(
+                    str(idx + 1),
+                    # TODO: make configurable
+                    expand=True,
                 )
-            LOGGER.debug("Populating viewport with search results.")
-            tui.viewport.view(ansi_map=tui.ANSI_MAP)
-            # reset current cursor position
-            LOGGER.debug("Resetting cursor position to top.")
-            tui.STATE.top_line = 0
-            tui.STATE.current_line = 0
-            # update top statusbar
-            tui.STATE.topstatus = f"coBib v{__version__} - {hits} hit{'s' if hits > 1 else ''}"
-            tui.statusbar(tui.topbar, tui.STATE.topstatus)
-            tui.STATE.inactive_commands = ["Add", "Filter", "Sort"]
-        elif command[1:]:
-            if sys.version_info[1] >= 8:
-                joined_command = shlex.join(command[1:])
-            else:
-                joined_command = shlex.quote(" ".join(command[1:]))
-            msg = f"No search hits for '{joined_command}'!"
-            LOGGER.info(msg)
-            tui.prompt_print(msg)
-            tui.viewport.update_list()
+                for line in match:
+                    line_text = Text(line)
+                    line_text.highlight_words(
+                        self.largs.query,
+                        config.commands.search.highlights.query,
+                        case_sensitive=not ignore_case,
+                    )
+                    matchtree.add_leaf(line_text)
+
+        return tree
```

### Comparing `cobib-3.5.5/src/cobib/commands/undo.py` & `cobib-4.0.0/src/cobib/commands/undo.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,132 +4,144 @@
 ```
 cobib undo
 ```
 For obvious reasons, this will only undo commands which had an effect on the contents of the
 database file.
 Moreover, as a safety measure, this command will only undo those changes, which have been committed
 by coBib *automatically*.
-You can disable this be setting the `--force` argument which *always* undoes the last commit.
+You can disable this be setting the `--force` argument which *always* undoes the last commit:
+```
+cobib undo --force
+```
+
+.. warning::
+   This command is *only* available if coBib's git-integration has been enabled via
+   `cobib.config.config.DatabaseConfig.git` *and* initialized properly (see `cobib.commands.init`).
 
-Furthermore, this command is *only* available if coBib's git-integration has been enabled and
-initialized.
-Refer to the documentation of `cobib.commands.init.InitCommand` for more details on that topic.
+### TUI
 
-You can also trigger this command from the `cobib.tui.tui.TUI`.
+You can also trigger this command from the `cobib.ui.tui.TUI`.
 By default, it is bound to the `u` key.
 """
 
 from __future__ import annotations
 
-import argparse
 import logging
 import subprocess
 import sys
-from typing import IO, TYPE_CHECKING, Any, List
+from pathlib import Path
+from typing import Type
+
+from rich.console import Console
+from rich.prompt import PromptBase
+from textual.app import App
+from typing_extensions import override
 
 from cobib.config import Event, config
 from cobib.database import Database
 from cobib.utils.rel_path import RelPath
 
 from .base_command import ArgumentParser, Command
 
 LOGGER = logging.getLogger(__name__)
 
-if TYPE_CHECKING:
-    import cobib.tui
-
 
 class UndoCommand(Command):
-    """The Undo Command."""
+    """The Undo Command.
+
+    This command can parse the following arguments:
+
+        * `-f`, `--force`: if specified, this will also revert changes which have *not* been
+          auto-committed by coBib.
+    """
 
     name = "undo"
 
-    def execute(self, args: List[str], out: IO[Any] = sys.stdout) -> None:
-        """Undoes the last change.
+    @override
+    def __init__(
+        self,
+        *args: str,
+        console: Console | App[None] | None = None,
+        prompt: Type[PromptBase[str]] | None = None,
+    ) -> None:
+        super().__init__(*args, console=console, prompt=prompt)
+
+        self.root: Path
+        """The path to the root of the git repository tracking the database."""
+
+        self.sha: str
+        """The git commit SHA which was reverted by this command."""
+
+    @override
+    @classmethod
+    def init_argparser(cls) -> None:
+        parser = ArgumentParser(prog="undo", description="Undo subcommand parser.")
+        parser.add_argument(
+            "-f", "--force", action="store_true", help="allow undoing non auto-committed changes"
+        )
+        cls.argparser = parser
 
-        This command is *only* available if coBib's git-integration has been enabled via
-        `config.database.git` *and* initialized properly (see `cobib.commands.init.InitCommand`).
-        If that is the case, this command will undo the changes of a previous command.
-        Note, that this *only* applies to commands whose changes have been committed by coBib
-        *automatically*.
-        This is a safety measure which you can disable by setting the `--force` argument.
-
-        Args:
-            args: a sequence of additional arguments used for the execution. The following values
-                are allowed for this command:
-                    * `-f`, `--force`: if specified, this will also revert changes which have *not*
-                      been auto-committed by coBib.
-            out: the output IO stream. This defaults to `sys.stdout`.
-        """
+    @override
+    def execute(self) -> None:
         git_tracked = config.database.git
         if not git_tracked:
             msg = (
                 "You must enable coBib's git-tracking in order to use the `Undo` command."
                 "\nPlease refer to the man-page for more information on how to do so."
             )
             LOGGER.error(msg)
             return
 
         file = RelPath(config.database.file).path
-        root = file.parent
-        if not (root / ".git").exists():
+        self.root = file.parent
+        if not (self.root / ".git").exists():
             msg = (
                 "You have configured, but not initialized coBib's git-tracking."
                 "\nPlease consult `cobib init --help` for more information on how to do so."
             )
             LOGGER.error(msg)
             return
 
         LOGGER.debug("Starting Undo command.")
-        parser = ArgumentParser(prog="undo", description="Undo subcommand parser.")
-        parser.add_argument(
-            "-f", "--force", action="store_true", help="allow undoing non auto-committed changes"
-        )
-
-        try:
-            largs = parser.parse_args(args)
-        except argparse.ArgumentError as exc:
-            LOGGER.error(exc.message)
-            return
 
-        Event.PreUndoCommand.fire(largs)
+        Event.PreUndoCommand.fire(self)
 
         LOGGER.debug("Obtaining git log.")
         lines = subprocess.check_output(
             [
                 "git",
                 "--no-pager",
                 "-C",
-                f"{root}",
+                f"{self.root}",
                 "log",
                 "--oneline",
                 "--no-decorate",
                 "--no-abbrev",
             ]
         )
         undone_shas = set()
         for commit in lines.decode().strip().split("\n"):
             LOGGER.debug("Processing commit %s", commit)
-            sha, *message = commit.split()
+            self.sha, *message = commit.split()
             if message[0] == "Undo":
                 # Store already undone commit sha
                 LOGGER.debug("Storing undone commit sha: %s", message[-1])
                 undone_shas.add(message[-1])
                 continue
-            if sha in undone_shas:
-                LOGGER.info("Skipping %s as it was already undone", sha)
+            if self.sha in undone_shas:
+                LOGGER.info("Skipping %s as it was already undone", self.sha)
                 continue
-            if largs.force or (message[0] == "Auto-commit:" and message[-1] != "InitCommand"):
+            if self.largs.force or (message[0] == "Auto-commit:" and message[-1] != "InitCommand"):
                 # we undo a commit if and only if:
                 #  - the `force` argument is specified OR
                 #  - the commit is an `auto-committed` change which is NOT from `InitCommand`
-                LOGGER.debug("Attempting to undo %s.", sha)
+                LOGGER.debug("Attempting to undo %s.", self.sha)
                 commands = [
-                    f"git -C {root} revert --no-commit {sha}",
-                    f"git -C {root} commit --no-gpg-sign --quiet --message 'Undo {sha}'",
+                    f"git -C {self.root} revert --no-commit {self.sha}",
+                    f"git -C {self.root} commit --no-gpg-sign --quiet --message 'Undo {self.sha}'",
                 ]
                 with subprocess.Popen(
                     "; ".join(commands), shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE
                 ) as undo:
                     undo.communicate()
                     if undo.returncode != 0:
                         LOGGER.error(  # pragma: no cover
@@ -141,18 +153,8 @@
                         Database().read()
                 break
         else:
             msg = "Could not find a commit to undo. Please commit something first!"
             LOGGER.warning(msg)
             sys.exit(1)
 
-        Event.PostUndoCommand.fire(root, sha)
-
-    @staticmethod
-    def tui(tui: cobib.tui.TUI) -> None:
-        # pdoc will inherit the docstring from the base class
-        # noqa: D102
-        LOGGER.debug("Undo command triggered from TUI.")
-        tui.execute_command(["undo"], skip_prompt=True)
-        # update database list
-        LOGGER.debug("Updating list after Undo command.")
-        tui.viewport.update_list()
+        Event.PostUndoCommand.fire(self)
```

### Comparing `cobib-3.5.5/src/cobib/config/__init__.py` & `cobib-4.0.0/src/cobib/config/__init__.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.5/src/cobib/config/config.py` & `cobib-4.0.0/src/cobib/config/config.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,557 +1,609 @@
+# pylint: disable=unnecessary-lambda,missing-docstring
 """coBib's configuration.
 
-This file contains both, the actual implementation of the `Config` class, as well as the runtime
+This file contains both, the actual implementation of the `Config` classes, as well as the runtime
 `config` object, which gets exposed on the module level as `cobib.config.config`.
 Note, that this last link will not point to the correct location in the online documentation due to
 the nature of the lower-level import.
 """
 
-import copy
+from __future__ import annotations
+
 import importlib.util
 import io
 import logging
 import os
 import sys
+from abc import abstractmethod
+from dataclasses import MISSING, dataclass, field
 from enum import Enum
 from pathlib import Path
-from typing import Any, Dict, Optional, TextIO, Union
-
-from cobib.utils.rel_path import RelPath
-
-LOGGER = logging.getLogger(__name__)
-
-ANSI_COLORS = [
-    "black",
-    "red",
-    "green",
-    "yellow",
-    "blue",
-    "magenta",
-    "cyan",
-    "white",
-]
-
-
-class LabelSuffix(Enum):
-    """Suffixes to disambiguate Entry labels."""
+from typing import TYPE_CHECKING, Callable, Optional, TextIO, Union
 
-    ALPHA = lambda count: chr(96 + count)  # pylint: disable=unnecessary-lambda-assignment
-    CAPTIAL = lambda count: chr(64 + count)  # pylint: disable=unnecessary-lambda-assignment
-    # pylint: disable=unnecessary-lambda,unnecessary-lambda-assignment
-    NUMERIC = lambda count: str(count)
-
-
-class Config(Dict[str, Any]):
-    """coBib's configuration class.
-
-    This class wraps the `dict` type and exposes the dictionary keys as attributes to ease access
-    (for both, getting and setting).
-    Furthermore, nested attributes can be set directly without having to ensure that the parent
-    attribute is already present.
-
-    References:
-        [Recursively access dict via attributes](https://stackoverflow.com/a/3031270)
-    """
+from typing_extensions import override
 
-    XDG_CONFIG_FILE: str = "~/.config/cobib/config.py"
-    """The XDG-based standard configuration location."""
-
-    DEFAULTS: Dict[str, Any] = {
-        "logging": {
-            "cache": "~/.cache/cobib/cache",
-            "logfile": "~/.cache/cobib/cobib.log",
-            "version": "~/.cache/cobib/version",
-        },
-        "commands": {
-            "edit": {
-                "default_entry_type": "article",
-                "editor": os.environ.get("EDITOR", "vim"),
-            },
-            "open": {
-                "command": "xdg-open" if sys.platform.lower() == "linux" else "open",
-                "fields": ["file", "url"],
-            },
-            "search": {
-                "grep": "grep",
-                "grep_args": [],
-                "ignore_case": False,
-            },
-        },
-        "database": {
-            "file": "~/.local/share/cobib/literature.yaml",
-            "format": {
-                "label_default": "{label}",
-                "label_suffix": ("_", LabelSuffix.ALPHA),
-                "suppress_latex_warnings": True,
-            },
-            "git": False,
-            "stringify": {
-                "list_separator": {
-                    "file": ", ",
-                    "tags": ", ",
-                    "url": ", ",
-                },
-            },
-        },
-        "events": {},
-        "parsers": {
-            "bibtex": {
-                "ignore_non_standard_types": False,
-            },
-            "yaml": {
-                "use_c_lib_yaml": False,
-            },
-        },
-        "tui": {
-            "default_list_args": ["-l"],
-            "prompt_before_quit": True,
-            "reverse_order": True,
-            "scroll_offset": 3,
-            "colors": {
-                "cursor_line_fg": "white",
-                "cursor_line_bg": "cyan",
-                "top_statusbar_fg": "black",
-                "top_statusbar_bg": "yellow",
-                "bottom_statusbar_fg": "black",
-                "bottom_statusbar_bg": "yellow",
-                "search_label_fg": "blue",
-                "search_label_bg": "black",
-                "search_query_fg": "red",
-                "search_query_bg": "black",
-                "popup_help_fg": "white",
-                "popup_help_bg": "green",
-                "popup_stdout_fg": "white",
-                "popup_stdout_bg": "blue",
-                "popup_stderr_fg": "white",
-                "popup_stderr_bg": "red",
-                "selection_fg": "white",
-                "selection_bg": "magenta",
-            },
-            "key_bindings": {
-                "prompt": ":",
-                "search": "/",
-                "help": "?",
-                "add": "a",
-                "delete": "d",
-                "edit": "e",
-                "filter": "f",
-                "import": "i",
-                "modify": "m",
-                "open": "o",
-                "quit": "q",
-                "redo": "r",
-                "sort": "s",
-                "undo": "u",
-                "select": "v",
-                "wrap": "w",
-                "export": "x",
-                "show": "ENTER",
-            },
-        },
-        "utils": {
-            "file_downloader": {
-                "default_location": "~/.local/share/cobib",
-                "url_map": {},
-            },
-            "journal_abbreviations": [],
-        },
-    }
-    """The default settings."""
-
-    # pylint: disable=super-init-not-called
-    def __init__(self, value: Optional[Dict[str, Any]] = None) -> None:
-        """Initializer of the recursive, attribute-access, dict-like configuration object.
-
-        The initializer does nothing when `None` is given.
-        When a dict is given, all values are set as attributes.
-
-        Args:
-            value: a dictionary of settings.
-        """
-        if value is None:
-            pass
-        elif isinstance(value, dict):
-            self.update(**value)
-        else:
-            raise TypeError("expected dict")
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        """Sets a key, value pair in the object's dictionary.
-
-        Args:
-            key: the attributes' name.
-            value: the attributes' value.
-        """
-        if isinstance(value, dict) and not isinstance(value, Config):
-            value = Config(value)
-        super().__setitem__(key, value)
-
-    def __setattr__(self, key: str, value: Any) -> None:
-        """Use `__setitem__` to set attributes unless it is a private (`__`) field.
-
-        This is necessary in order to avoid a RecursionError during the pdoc generation.
-
-        Args:
-            key: the attributes' name.
-            value: the attributes' value.
-        """
-        if key[0:2] == "__":
-            super().__setattr__(key, value)
-        else:
-            self.__setitem__(key, value)
-
-    MARKER = object()
-    """A helper object for detecting the nested recursion-threshold."""
-
-    EXCEPTIONAL_KEYS = {"events", "url_map"}
-    """A set of exceptional keys which do not cause automatic item creation. This is required in
-    order to support `dict`-like configuration options properly."""
-
-    def __getitem__(self, key: str) -> Any:
-        """Gets a key from the configuration object's dictionary.
-
-        If the key is not present yet, it is automagically initialized with an empty configuration
-        object to allow recursive attribute-setting.
-
-        Args:
-            key: the queried attributes' name.
-
-        Returns:
-            The value of the queried attribute.
-        """
-        found = self.get(key, Config.MARKER)
-        if found is Config.MARKER and key not in Config.EXCEPTIONAL_KEYS:
-            found = Config()
-            super().__setitem__(key, found)
-        return found
-
-    def __getattr__(self, key: str) -> Any:
-        """Use `__getitem__` to get attributes unless it is a private (`__`) field.
-
-        This is necessary in order to avoid a RecursionError during the pdoc generation.
-
-        Args:
-            key: the queried attributes' name.
+from cobib.utils.rel_path import RelPath
 
-        Returns:
-            The value of the queried attribute.
-        """
-        if key[0:2] == "__":
-            return self.get(key)
-        return self.__getitem__(key)
+if TYPE_CHECKING:
+    from .event import Event
 
-    def update(self, **kwargs) -> None:  # type: ignore
-        """Updates the configuration with a dictionary of settings.
+LOGGER = logging.getLogger(__name__)
 
-        This function ensures values are deepcopied, too.
 
-        Args:
-            kwargs: key, value pairs to be added to the configuration data.
-        """
-        for key, value in kwargs.items():
-            self[key] = copy.deepcopy(value)
+@dataclass
+class _ConfigBase:
+    """Base class for configuration section dataclasses."""
 
     @staticmethod
-    def load(configpath: Optional[Union[str, Path, TextIO, io.TextIOWrapper]] = None) -> None:
-        """Loads another configuration object at runtime.
-
-        WARNING: The new Python-like configuration allows essentially arbitrary Python code so it is
-        the user's responsibility to treat this with care!
+    def _assert(expression: bool, error: str) -> None:
+        """Asserts the expression is True.
 
         Args:
-            configpath: the path to the configuration.
-        """
-        if configpath is not None:
-            if isinstance(configpath, (TextIO, io.TextIOWrapper)):
-                configpath = configpath.name
-        elif "COBIB_CONFIG" in os.environ:
-            configpath_env = os.environ["COBIB_CONFIG"]
-            if configpath_env.lower() in ("", "0", "f", "false", "nil", "none"):
-                LOGGER.info(
-                    "Skipping configuration loading because negative COBIB_CONFIG environment "
-                    "variable was detected."
-                )
-                return
-            configpath = RelPath(configpath_env).path
-        elif RelPath(Config.XDG_CONFIG_FILE).exists():
-            configpath = RelPath(Config.XDG_CONFIG_FILE).path
-        else:  # pragma: no cover
-            return  # pragma: no cover
-        LOGGER.info("Loading configuration from default location: %s", configpath)
-
-        spec = importlib.util.spec_from_file_location("config", configpath)
-        if spec is None:
-            LOGGER.error(
-                "The config at %s could not be interpreted as a Python module.", configpath
-            )
-            sys.exit(1)
-        else:
-            cfg = importlib.util.module_from_spec(spec)
-            spec.loader.exec_module(cfg)  # type: ignore
+            expression: the expression to assert.
+            error: the message of the `RuntimeError` upon assertion failure.
 
-        try:
-            # validate config
-            config.validate()
-        except RuntimeError as exc:
-            LOGGER.error(exc)
-            sys.exit(1)
+        Raises:
+            RuntimeError with the specified error string.
+        """
+        if not expression:
+            raise RuntimeError(error)
 
+    @abstractmethod
     def validate(self) -> None:
         """Validates the configuration at runtime.
 
         Raises:
             RuntimeError when an invalid setting is encountered.
         """
-        LOGGER.info("Validating the runtime configuration.")
 
-        # LOGGING section
+    def defaults(self) -> None:
+        """Resets the configuration to the default settings."""
+        # pylint: disable=no-member
+        for name, field_ in self.__dataclass_fields__.items():
+            if field_.default != MISSING:
+                setattr(self, name, field_.default)
+            else:
+                setattr(self, name, field_.default_factory())  # type: ignore[misc]
+
+
+@dataclass
+class LoggingConfig(_ConfigBase):
+    """The `config.logging` section."""
+
+    cache: str | Path = "~/.cache/cobib/cache"
+    """Specifies the default cache location."""
+    logfile: str | Path = "~/.cache/cobib/cobib.log"
+    """Specifies the default logfile location."""
+    version: str | None = "~/.cache/cobib/version"
+    """Specifies the location for the cached version number based on which coBib shows the latest
+    changes. Set this to `None` to disable this functionality entirely."""
+
+    @override
+    def validate(self) -> None:
         LOGGER.debug("Validating the LOGGING configuration section.")
         self._assert(
-            isinstance(self.logging.cache, str), "config.logging.cache should be a string."
+            isinstance(self.cache, (str, Path)), "config.logging.cache should be a string."
         )
         self._assert(
-            isinstance(self.logging.logfile, str), "config.logging.logfile should be a string."
+            isinstance(self.logfile, (str, Path)), "config.logging.logfile should be a string."
         )
         self._assert(
-            self.logging.version is None or isinstance(self.logging.version, str),
+            self.version is None or isinstance(self.version, str),
             "config.logging.version should be a string or `None`.",
         )
 
-        # COMMANDS section
-        LOGGER.debug("Validating the COMMANDS configuration section.")
-        # COMMANDS.EDIT section
+
+@dataclass
+class EditCommandConfig(_ConfigBase):
+    """The `config.commands.edit` section."""
+
+    default_entry_type: str = "article"
+    """Specifies the default bibtex entry type."""
+    editor: str = os.environ.get("EDITOR", "vim")
+    """Specifies the editor program. Note, that this default will respect your `$EDITOR`
+    environment setting and fall back to `vim` if that variable is not set."""
+
+    @override
+    def validate(self) -> None:
         LOGGER.debug("Validating the COMMANDS.EDIT configuration section.")
         self._assert(
-            isinstance(self.commands.edit.default_entry_type, str),
+            isinstance(self.default_entry_type, str),
             "config.commands.edit.default_entry_type should be a string.",
         )
         self._assert(
-            isinstance(self.commands.edit.editor, str),
+            isinstance(self.editor, str),
             "config.commands.edit.editor should be a string.",
         )
-        # COMMANDS.OPEN section
+
+
+@dataclass
+class ListCommandConfig(_ConfigBase):
+    """The `config.commands.list_` section."""
+
+    default_columns: list[str] = field(default_factory=lambda: ["label", "title"])
+    """Specifies the default columns shown during the `list` command."""
+    ignore_case: bool = False
+    """Specifies whether filter matching should be performed case-insensitive."""
+
+    @override
+    def validate(self) -> None:
+        LOGGER.debug("Validating the COMMANDS.LIST configuration section.")
+        self._assert(
+            isinstance(self.default_columns, list),
+            "config.commands.list_.default_columns should be a list.",
+        )
+        self._assert(
+            isinstance(self.ignore_case, bool),
+            "config.commands.list_.ignore_case should be a boolean.",
+        )
+
+
+@dataclass
+class OpenCommandConfig(_ConfigBase):
+    """The `config.commands.open` section."""
+
+    command: str = "xdg-open" if sys.platform.lower() == "linux" else "open"
+    """Specifies the command used for opening files associated with your entries."""
+    fields: list[str] = field(default_factory=lambda: ["file", "url"])
+    """Specifies the entry fields which are to be checked for openable URLs."""
+
+    @override
+    def validate(self) -> None:
         LOGGER.debug("Validating the COMMANDS.OPEN configuration section.")
         self._assert(
-            isinstance(self.commands.open.command, str),
+            isinstance(self.command, str),
             "config.commands.open.command should be a string.",
         )
         self._assert(
-            isinstance(self.commands.open.fields, list),
+            isinstance(self.fields, list),
             "config.commands.open.fields should be a list.",
         )
-        # COMMANDS.SEARCH section
+
+
+@dataclass
+class SearchHighlightConfig(_ConfigBase):
+    """The `config.commands.search.highlights` section."""
+
+    label: str = "blue"
+    """Specifies the color with which to highlight the labels of search results."""
+    query: str = "red"
+    """Specifies the color with which to highlight the query matches of a search."""
+
+    @override
+    def validate(self) -> None:
+        LOGGER.debug("Validating the COMMANDS.SEARCH.HIGHLIGHTS configuration section.")
+        self._assert(
+            isinstance(self.label, str),
+            "config.commands.search.highlights.label should be a string.",
+        )
+        self._assert(
+            isinstance(self.query, str),
+            "config.commands.search.highlights.query should be a string.",
+        )
+
+
+@dataclass
+class SearchCommandConfig(_ConfigBase):
+    """The `config.commands.search` section."""
+
+    grep: str = "grep"
+    """Specifies the grep tool used for searching through your database and associated files. The
+    default tool (`grep`) will not provide results for attached PDFs but other tools such as
+    [ripgrep-all](https://github.com/phiresky/ripgrep-all) will."""
+    grep_args: list[str] = field(default_factory=list)
+    """Specifies additional arguments for your grep command. Note, that GNU's grep understands
+    extended regex patterns even without specifying `-E`."""
+    ignore_case: bool = False
+    """Specifies whether searches should be performed case-insensitive."""
+    highlights: SearchHighlightConfig = field(default_factory=lambda: SearchHighlightConfig())
+    """The nested section for highlights used when displaying search results."""
+
+    @override
+    def validate(self) -> None:
         LOGGER.debug("Validating the COMMANDS.SEARCH configuration section.")
         self._assert(
-            isinstance(self.commands.search.grep, str),
+            isinstance(self.grep, str),
             "config.commands.search.grep should be a string.",
         )
         self._assert(
-            isinstance(self.commands.search.grep_args, list),
+            isinstance(self.grep_args, list),
             "config.commands.search.grep_args should be a list.",
         )
         self._assert(
-            isinstance(self.commands.search.ignore_case, bool),
+            isinstance(self.ignore_case, bool),
             "config.commands.search.ignore_case should be a boolean.",
         )
+        self.highlights.validate()
 
-        # DATABASE section
-        self._assert(
-            isinstance(self.database.file, str), "config.database.file should be a string."
-        )
-        self._assert(
-            isinstance(self.database.git, bool), "config.database.git should be a boolean."
-        )
-        # DATABASE.FORMAT section
-        if "month" in self["database"]["format"].keys():
-            LOGGER.warning(
-                "The config.database.format.month setting is deprecated as of version 3.1.0! "
-                "Instead, coBib will store the month as a three-letter code which is a common "
-                "format for which most citation styles include macros. See also "
-                "https://www.bibtex.com/f/month-field/"
-            )
+
+@dataclass
+class CommandConfig(_ConfigBase):
+    """The `config.commands` section."""
+
+    edit: EditCommandConfig = field(default_factory=lambda: EditCommandConfig())
+    """The nested section for settings related to the `edit` command."""
+    list_: ListCommandConfig = field(default_factory=lambda: ListCommandConfig())
+    """The nested section for settings related to the `list` command. Note the trailing underscore
+    of its name, since this attribute would otherwise clash with the builtin `list` keyword."""
+    open: OpenCommandConfig = field(default_factory=lambda: OpenCommandConfig())
+    """The nested section for settings related to the `open` command."""
+    search: SearchCommandConfig = field(default_factory=lambda: SearchCommandConfig())
+    """The nested section for settings related to the `search` command."""
+
+    @override
+    def validate(self) -> None:
+        LOGGER.debug("Validating the COMMANDS configuration section.")
+        self.edit.validate()
+        self.list_.validate()
+        self.open.validate()
+        self.search.validate()
+
+
+class LabelSuffix(Enum):
+    """Suffixes to disambiguate `cobib.database.Entry` labels."""
+
+    ALPHA = lambda count: chr(96 + count)  # pylint: disable=unnecessary-lambda-assignment
+    CAPTIAL = lambda count: chr(64 + count)  # pylint: disable=unnecessary-lambda-assignment
+    # pylint: disable=unnecessary-lambda,unnecessary-lambda-assignment
+    NUMERIC = lambda count: str(count)
+
+
+@dataclass
+class DatabaseFormatConfig(_ConfigBase):
+    """The `config.database.format` section."""
+
+    label_default: str = "{label}"
+    """Specifies a default label format which will be used for database entry keys. The format of
+    this option follows the f-string like formatting of modifications (see also the documentation
+    of the `cobib.commands.modify.ModifyCommand`). The default configuration value leaves the label
+    unchanged compared to the metadata provided by the source from which the entry gets added. A
+    more useful example is `"{author.split(' and ')[0].split()[-1]}{year}"` which takes the surname
+    of the first author and immediately appends the publication year."""
+    label_suffix: tuple[str, LabelSuffix] = field(default_factory=lambda: ("_", LabelSuffix.ALPHA))
+    """Specifies the suffix format which is used to disambiguate labels if a conflict would occur.
+    This option takes a tuple of length 2, where the first entry is the string separating the
+    proposed label from the enumerator and the second one is one of the enumerators provided by the
+    `LabelSuffix` object. The available enumerators are:
+        - ALPHA: a, b, ...
+        - CAPTIAL: A, B, ...
+        - NUMERIC: 1, 2, ...
+    """
+    suppress_latex_warnings: bool = True
+    """Specifies whether latex warnings should not be ignored during the escaping of special
+    characters. This is a simple option which gets passed on to the internally used `pylatexenc`
+    library."""
+
+    @override
+    def validate(self) -> None:
+        LOGGER.debug("Validating the DATABASE.FORMAT configuration section.")
         self._assert(
-            isinstance(self.database.format.label_default, str),
+            isinstance(self.label_default, str),
             "config.database.format.label_default should be a string.",
         )
         self._assert(
-            isinstance(self.database.format.label_suffix, tuple)
-            and len(self.database.format.label_suffix) == 2,
+            isinstance(self.label_suffix, tuple) and len(self.label_suffix) == 2,
             "config.database.format.label_suffix should be a tuple of length 2.",
         )
         self._assert(
-            isinstance(self.database.format.label_suffix[0], str),
+            isinstance(self.label_suffix[0], str),
             "The first entry of config.database.format.label_suffix should be a string.",
         )
         self._assert(
-            callable(self.database.format.label_suffix[1]),
+            callable(self.label_suffix[1]),
             "The first entry of config.database.format.label_suffix should be a function.",
         )
         self._assert(
-            isinstance(self.database.format.suppress_latex_warnings, bool),
+            isinstance(self.suppress_latex_warnings, bool),
             "config.database.format.suppress_latex_warnings should be a boolean.",
         )
+
+
+@dataclass
+class EntryListSeparatorConfig(_ConfigBase):
+    """The `config.database.stringify.list_separator` section.
+
+    These settings configure how list-based `cobib.database.Entry` fields are transformed into
+    strings when converting to the BibTeX format. Each of these fields will be joined by the
+    respective values.
+    """
+
+    file: str = ", "
+    """Specifies the string used to join the list of files into a single string representation."""
+    tags: str = ", "
+    """Specifies the string used to join the list of tags into a single string representation."""
+    url: str = ", "
+    """Specifies the string used to join the list of URLs into a single string representation."""
+
+    @override
+    def validate(self) -> None:
+        LOGGER.debug("Validating the DATABASE.STRINGIFY.LIST_SEPARATOR configuration section.")
         self._assert(
-            isinstance(self.database.stringify.list_separator.file, str),
+            isinstance(self.file, str),
             "config.database.stringify.list_separator.file should be a string.",
         )
         self._assert(
-            isinstance(self.database.stringify.list_separator.tags, str),
+            isinstance(self.tags, str),
             "config.database.stringify.list_separator.tags should be a string.",
         )
         self._assert(
-            isinstance(self.database.stringify.list_separator.url, str),
+            isinstance(self.url, str),
             "config.database.stringify.list_separator.url should be a string.",
         )
 
-        # EVENTS section
-        self._assert(isinstance(self.events, dict), "config.events should be a dict.")
-        for event in self.events:
-            self._assert(
-                event.validate(),
-                f"config.events.{event} did not pass its validation check.",
-            )
 
-        # PARSER section
+@dataclass
+class EntryStringifyConfig(_ConfigBase):
+    """The `config.database.stringify` section."""
+
+    list_separator: EntryListSeparatorConfig = field(
+        default_factory=lambda: EntryListSeparatorConfig()
+    )
+    """The nested section for list separator values."""
+
+    @override
+    def validate(self) -> None:
+        LOGGER.debug("Validating the DATABASE.STRINGIFY configuration section.")
+        self.list_separator.validate()
+
+
+@dataclass
+class DatabaseConfig(_ConfigBase):
+    """The `config.database` section."""
+
+    file: str | Path = "~/.local/share/cobib/literature.yaml"
+    """Specifies the path to the database YAML file. You can use `~` to represent your `$HOME`
+    directory."""
+    format: DatabaseFormatConfig = field(default_factory=lambda: DatabaseFormatConfig())
+    """The nested section for database formatting settings."""
+    git: bool = False
+    """coBib can integrate with `git` in order to automatically track the history of the database.
+    However, by default, this option is disabled. In order to make use of this, enable this setting
+    and initialize your database with `cobib init --git`.
+
+    .. warning::
+       Before enabling this setting you must ensure that you have set up git properly by setting
+       your name and email address."""
+    stringify: EntryStringifyConfig = field(default_factory=lambda: EntryStringifyConfig())
+    """The nested section for database string-formatting settings."""
+
+    @override
+    def validate(self) -> None:
+        LOGGER.debug("Validating the DATABASE configuration section.")
+        self._assert(isinstance(self.file, str), "config.database.file should be a string.")
+        self._assert(isinstance(self.git, bool), "config.database.git should be a boolean.")
+        self.format.validate()
+        self.stringify.validate()
+
+
+@dataclass
+class BibtexParserConfig(_ConfigBase):
+    """The `config.parsers.bibtex` section."""
+
+    ignore_non_standard_types: bool = False
+    """Specifies whether the BibTeX-parser should ignore non-standard BibTeX entry types."""
+
+    @override
+    def validate(self) -> None:
+        LOGGER.debug("Validating the PARSERS.BIBTEX configuration section.")
         self._assert(
-            isinstance(self.parsers.bibtex.ignore_non_standard_types, bool),
+            isinstance(self.ignore_non_standard_types, bool),
             "config.parsers.bibtex.ignore_non_standard_types should be a boolean.",
         )
+
+
+@dataclass
+class YAMLParserConfig(_ConfigBase):
+    """The `config.parsers.yaml` section."""
+
+    use_c_lib_yaml: bool = True
+    """Specifies whether the C-based implementation of the YAML parser (called `LibYAML`) shall be
+    used, *significantly* increasing the performance of the parsing.
+
+    .. note::
+       This requires manual installation of the C-based parser:
+       https://yaml.readthedocs.io/en/latest/install.html#optional-requirements
+    """
+
+    @override
+    def validate(self) -> None:
+        LOGGER.debug("Validating the PARSERS.YAML configuration section.")
         self._assert(
-            isinstance(self.parsers.yaml.use_c_lib_yaml, bool),
+            isinstance(self.use_c_lib_yaml, bool),
             "config.parsers.yaml.use_c_lib_yaml should be a boolean.",
         )
-        if self.parsers.yaml.use_c_lib_yaml is False:
-            LOGGER.warning(
-                "The config.parsers.yaml.use_c_lib_yaml setting (introduced in version 3.4.0) will "
-                "change its default value to `True` in version 4.0.0!"
-            )
 
-        # TUI section
-        self._assert(
-            isinstance(self.tui.default_list_args, list),
-            "config.tui.default_list_args should be a list.",
-        )
-        self._assert(
-            isinstance(self.tui.prompt_before_quit, bool),
-            "config.tui.prompt_before_quit should be a boolean.",
-        )
-        self._assert(
-            isinstance(self.tui.reverse_order, bool),
-            "config.tui.reverse_order should be a boolean.",
-        )
-        self._assert(
-            isinstance(self.tui.scroll_offset, int),
-            "config.tui.scroll_offset should be an integer.",
-        )
 
-        # TUI.COLORS section
-        LOGGER.debug("Validating the TUI.COLORS configuration section.")
-        for name in self.DEFAULTS["tui"]["colors"]:
-            self._assert(
-                name in self.tui.colors.keys(), f"Missing config.tui.colors.{name} specification!"
-            )
+@dataclass
+class ParserConfig(_ConfigBase):
+    """The `config.parsers` section."""
+
+    bibtex: BibtexParserConfig = field(default_factory=lambda: BibtexParserConfig())
+    """The nested section for the BibTeX parser settings."""
+    yaml: YAMLParserConfig = field(default_factory=lambda: YAMLParserConfig())
+    """The nested section for the YAML parser settings."""
 
-        for name, color in self.tui.colors.items():
-            if name not in self.DEFAULTS["tui"]["colors"] and name not in ANSI_COLORS:
-                LOGGER.warning("Ignoring unknown TUI color: %s.", name)
-            self._assert(
-                bool(
-                    (color in ANSI_COLORS)
-                    or (
-                        len(color.strip("#")) == 6
-                        and tuple(int(color.strip("#")[i : i + 2], 16) for i in (0, 2, 4))
-                    )
-                ),
-                f"Unknown color specification: {color}",
-            )
+    @override
+    def validate(self) -> None:
+        LOGGER.debug("Validating the PARSERS configuration section.")
+        self.bibtex.validate()
+        self.yaml.validate()
+
+
+@dataclass
+class FileDownloaderConfig(_ConfigBase):
+    """The `config.utils.file_downloader` section."""
+
+    default_location: str = "~/.local/share/cobib"
+    """Specifies the default download location for associated files."""
+    url_map: dict[str, str] = field(default_factory=dict)
+    """Permits providing rules to map from a journal's landing page URL to its PDF URL. To do so,
+    insert an entry into this dictionary, with a regex-pattern matching the journal's landing page
+    URL and a value being the PDF URL. E.g.:
+
+    ```python
+    config.utils.file_downloader.url_map[
+        r"(.+)://aip.scitation.org/doi/([^/]+)"
+    ] = r"\1://aip.scitation.org/doi/pdf/\2"
+
+    config.utils.file_downloader.url_map[
+        r"(.+)://quantum-journal.org/papers/([^/]+)"
+    ] = r"\1://quantum-journal.org/papers/\2/pdf/"
+    ```
 
-        # TUI.KEY_BINDINGS section
-        LOGGER.debug("Validating the TUI.KEY_BINDINGS configuration section.")
-        for command in self.DEFAULTS["tui"]["key_bindings"]:
-            self._assert(
-                command in self.tui.key_bindings.keys(),
-                f"Missing config.tui.key_bindings.{command} key binding!",
-            )
-        for command, key in self.DEFAULTS["tui"]["key_bindings"].items():
-            self._assert(
-                isinstance(key, str), f"config.tui.key_bindings.{command} should be a string."
-            )
+    Make sure to use raw Python strings to ensure proper backslash-escaping."""
 
-        # UTILS section
-        LOGGER.debug("Validating the UTILS configuration section.")
+    @override
+    def validate(self) -> None:
+        LOGGER.debug("Validating the UTILS.FILE_DOWNLOADER configuration section.")
         self._assert(
-            isinstance(self.utils.file_downloader.default_location, str),
+            isinstance(self.default_location, str),
             "config.utils.file_downloader.default_location should be a string.",
         )
         self._assert(
-            isinstance(self.utils.file_downloader.url_map, dict),
+            isinstance(self.url_map, dict),
             "config.utils.file_downloader.url_map should be a dict.",
         )
-        for pattern, repl in self.utils.file_downloader.url_map.items():
+        for pattern, repl in self.url_map.items():
             self._assert(
                 isinstance(pattern, str) and isinstance(repl, str),
                 "config.utils.file_downloader.url_map should be a dict[str, str].",
             )
 
+
+@dataclass
+class UtilsConfig(_ConfigBase):
+    """The `config.utils` section."""
+
+    file_downloader: FileDownloaderConfig = field(default_factory=lambda: FileDownloaderConfig())
+    """The nested section for the `cobib.utils.FileDownloader` utils settings."""
+    journal_abbreviations: list[tuple[str, str]] = field(default_factory=list)
+    """Permits providing a list of journal abbreviations. This list should be formatted as tuples of
+    the form: `(full journal name, abbreviation)`. The abbreviation should include any necessary
+    punctuation which can be excluded upon export (see also `cobib export --help`)."""
+
+    @override
+    def validate(self) -> None:
+        LOGGER.debug("Validating the UTILS configuration section.")
+        self.file_downloader.validate()
         self._assert(
-            isinstance(self.utils.journal_abbreviations, list),
+            isinstance(self.journal_abbreviations, list),
             "config.utils.journal_abbreviations should be a list.",
         )
-        for abbrev in self.utils.journal_abbreviations:
+        for abbrev in self.journal_abbreviations:
             self._assert(
                 isinstance(abbrev, tuple),
                 "config.utils.journal_abbreviations should be a list of tuples.",
             )
 
-    @staticmethod
-    def _assert(expression: bool, error: str) -> None:
-        """Asserts the expression is True.
 
-        Args:
-            expression: the expression to assert.
-            error: the message of the `RuntimeError` upon assertion failure.
+@dataclass
+class Config(_ConfigBase):
+    """The `config` dataclass."""
+
+    logging: LoggingConfig = field(default_factory=lambda: LoggingConfig())
+    """The nested section for the logging settings."""
+    commands: CommandConfig = field(default_factory=lambda: CommandConfig())
+    """The nested section for the commands settings."""
+    database: DatabaseConfig = field(default_factory=lambda: DatabaseConfig())
+    """The nested section for the database settings."""
+    events: dict["Event", list[Callable]] = field(default_factory=dict)  # type: ignore[type-arg]
+    """It is possible to register hooks on various events. Although this can be done manually using
+    this dictionary, it is preferred to use the function-decorators like so:
+    To subscribe to a certain event do something similar to the following:
+
+    ```python
+    from os import system
+    from cobib.config import Event
+    from cobib.commands import InitCommand
+
+    @Event.PostInitCommand.subscribe
+    def add_remote(cmd: InitCommand) -> None:
+        system(f"git -C {cmd.root} remote add origin https://github.com/user/repo")
+    ```
 
-        Raises:
-            RuntimeError with the specified error string.
-        """
-        if not expression:
-            raise RuntimeError(error)
+    Note, that the typing is required for the config validation to pass!
+    For more information refer to the `cobib.config.Event` documentation.
+    """
+    parsers: ParserConfig = field(default_factory=lambda: ParserConfig())
+    """The nested section for the parsers settings."""
+    utils: UtilsConfig = field(default_factory=lambda: UtilsConfig())
+    """The nested section for the utils settings."""
+
+    # pylint: disable=invalid-name
+    XDG_CONFIG_FILE: str | Path = field(
+        default="~/.config/cobib/config.py", init=False, repr=False, compare=False
+    )
+    """The XDG-based standard configuration location."""
 
-    def defaults(self) -> None:
-        """Resets the configuration to the default settings."""
-        # pylint: disable=consider-using-dict-items
-        for section in self.DEFAULTS:
-            if section == "events":
-                # manually reset events
-                self["events"] = {}
-                continue
-            self[section].update(**self.DEFAULTS[section])
-
-    def get_ansi_color(self, name: str) -> str:
-        r"""Returns an ANSI color code for the named color.
-
-        Appending `_fg` and `_bg` to the color name will yield the configured colors for the fore-
-        and background property, respectively.
-        The [ANSI color code](https://en.wikipedia.org/wiki/ANSI_escape_code#3-bit_and_4-bit) can
-        then be constructed using the formula `\x1b[{FG};{BG}m`.
+    @override
+    def validate(self) -> None:
+        LOGGER.info("Validating the runtime configuration.")
+        self.logging.validate()
+        self.commands.validate()
+        self.database.validate()
+        self.parsers.validate()
+        self.utils.validate()
 
-        Args:
-            name: a named color as specified in the configuration *excluding* the `_fg` or `_bg`
-                  suffix.
+        LOGGER.debug("Validating the EVENTS configuration section.")
+        self._assert(isinstance(self.events, dict), "config.events should be a dict.")
+        for event in self.events:
+            self._assert(
+                event.validate(),
+                f"config.events.{event} did not pass its validation check.",
+            )
+
+    @staticmethod
+    def load(configpath: Optional[Union[str, Path, TextIO, io.TextIOWrapper]] = None) -> None:
+        """Loads another configuration object at runtime.
+
+        WARNING: The new Python-like configuration allows essentially arbitrary Python code so it is
+        the user's responsibility to treat this with care!
 
-        Returns:
-            A string representing the foreground and background ANSI color code.
+        Args:
+            configpath: the path to the configuration.
         """
-        fg_color = 30 + ANSI_COLORS.index(self.tui.colors.get(name + "_fg"))
-        bg_color = 40 + ANSI_COLORS.index(self.tui.colors.get(name + "_bg"))
+        LOGGER.info(configpath)
+        if configpath is not None:
+            if isinstance(configpath, (TextIO, io.TextIOWrapper)):
+                configpath.close()
+                configpath = configpath.name
+        elif "COBIB_CONFIG" in os.environ:
+            configpath_env = os.environ["COBIB_CONFIG"]
+            if configpath_env.lower() in ("", "0", "f", "false", "nil", "none"):
+                LOGGER.info(
+                    "Skipping configuration loading because negative COBIB_CONFIG environment "
+                    "variable was detected."
+                )
+                return
+            configpath = RelPath(configpath_env).path
+        elif Config.XDG_CONFIG_FILE and RelPath(Config.XDG_CONFIG_FILE).exists():
+            configpath = RelPath(Config.XDG_CONFIG_FILE).path
+        else:  # pragma: no cover
+            return  # pragma: no cover
+        LOGGER.info("Loading configuration from default location: %s", configpath)
 
-        return f"\x1b[{fg_color};{bg_color}m"
+        spec = importlib.util.spec_from_file_location("config", configpath)
+        if spec is None:
+            LOGGER.error(
+                "The config at %s could not be interpreted as a Python module.", configpath
+            )
+            sys.exit(1)
+        else:
+            cfg = importlib.util.module_from_spec(spec)
+            spec.loader.exec_module(cfg)  # type: ignore
+
+        try:
+            # validate config
+            config.validate()
+        except RuntimeError as exc:
+            LOGGER.error(exc)
+            sys.exit(1)
 
 
-config: Config = Config()
+config = Config()
 """This is the runtime configuration object. It is exposed on the module level via:
 ```python
 from cobib.config import config
 ```
 """
 config.defaults()
```

### Comparing `cobib-3.5.5/src/cobib/config/event.py` & `cobib-4.0.0/src/cobib/config/event.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,44 +1,59 @@
 """coBib's subscribable events.
 
 ### Available Events
 
 There are various kinds of event types:
     - Pre*Command: these fire before a command gets executed. Hooks subscribing to these events
-      are passed the argument dictionary which they can modify to their desire.
+      are passed an instance of the command which will be populated with the original command-line
+      arguments as well as the resulting `argparse.Namespace`.
     - Post*Command: these fire after a command got executed but (generally) **before** the
       Database gets written to file, allowing final touch-ups and modifications to take place.
-      The inputs to these hooks depend on the specific command firing the event (see below).
+      Just like the `Pre*Command` events, the input will be an instance of the command through which
+      a user can modify the command data at runtime.
+    - Pre*Import: these fire before an importer gets executed. Hooks subscribing to these events
+      are passed an instance of the importer which will be populated with the original command-line
+      arguments as well as the resulting `argparse.Namespace`.
+    - Post*Import: these fire after an importer got executed but (generally) **before** the
+      Database gets written to file, allowing final touch-ups and modifications to take place.
+      Just like the `Pre*Import` events, the input will be an instance of the importer through which
+      a user can modify the command data at runtime.
     - Pre*Parse: just like the Pre-Command events, these fire before a parser runs. As an input
       they generally get the driver input.
     - Post*Parse: these fire after a parser ran. They again allow final touch-ups of the
       generated dictionary of new entries.
     - Pre*Dump: these fire before an entry gets dumped. The hook can pre-process the entry to
       its desire. Changes will not become persistent in the Database.
     - Post*Dump: these fire after an entry got formatted as a string. The string can be
       post-processed with some final touch-ups.
+    - and finally there a few specific events not belonging to any of the categories mentioned
+      above, examples of which are the `PreGitCommit` and `PostGitCommit` events.
 
 All events are listed below.
 
 ### Usage
 
 You can register a function to be executed when a certain event gets triggered as shown in the
 following example:
 ```python
-from pathlib import Path
 from os import system
 from cobib.config import Event
+from cobib.commands import InitCommand
 
 @Event.PostInitCommand.subscribe
-def add_remote(root: Path, file: Path) -> None:
-    system(f"git -C {root} remote add origin https://github.com/user/repo")
+def add_remote(cmd: InitCommand) -> None:
+    system(f"git -C {cmd.root} remote add origin https://github.com/user/repo")
 ```
 The above example gets run after the `init` command has finished. It adds a remote to the git
 repository. This can be useful in combination with automatic pushing to the remote like done here:
 ```python
+from pathlib import Path
+from os import system
+from cobib.config import Event
+
 @Event.PostGitCommit.subscribe
 def push_to_remote(root: Path, file: Path) -> None:
     system(f"git -C {root} push origin master")
 ```
 
 It is important that you include the type hints as part of the function definition because these are
 used during the config validation.
@@ -56,41 +71,54 @@
     print("New entries being added: ", list(bib.keys()))
 ```
 """
 
 from __future__ import annotations
 
 import logging
-from argparse import Namespace
 from enum import Enum
 from itertools import zip_longest
 from pathlib import Path
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     ForwardRef,
     List,
     Optional,
-    Set,
     Tuple,
     get_type_hints,
 )
 
 from cobib.utils.rel_path import RelPath
 
 from .config import config
 
 _FORWARD_REFS: Dict[str, str] = {}
 if TYPE_CHECKING:
+    from cobib import commands, importers
     from cobib.database import Entry
 else:
     _FORWARD_REFS = {
         "ForwardRef('Entry')": "Entry",
+        "ForwardRef('commands.AddCommand')": "cobib.commands.add.AddCommand",
+        "ForwardRef('commands.DeleteCommand')": "cobib.commands.delete.DeleteCommand",
+        "ForwardRef('commands.EditCommand')": "cobib.commands.edit.EditCommand",
+        "ForwardRef('commands.ExportCommand')": "cobib.commands.export.ExportCommand",
+        "ForwardRef('commands.ImportCommand')": "cobib.commands.import_.ImportCommand",
+        "ForwardRef('commands.InitCommand')": "cobib.commands.init.InitCommand",
+        "ForwardRef('commands.ListCommand')": "cobib.commands.list_.ListCommand",
+        "ForwardRef('commands.ModifyCommand')": "cobib.commands.modify.ModifyCommand",
+        "ForwardRef('commands.OpenCommand')": "cobib.commands.open.OpenCommand",
+        "ForwardRef('commands.RedoCommand')": "cobib.commands.redo.RedoCommand",
+        "ForwardRef('commands.SearchCommand')": "cobib.commands.search.SearchCommand",
+        "ForwardRef('commands.ShowCommand')": "cobib.commands.show.ShowCommand",
+        "ForwardRef('commands.UndoCommand')": "cobib.commands.undo.UndoCommand",
+        "ForwardRef('importers.ZoteroImporter')": "cobib.importers.zotero.ZoteroImporter",
     }
 
 LOGGER = logging.getLogger(__name__)
 
 
 class Event(Enum):
     # pylint: disable=invalid-name
@@ -119,314 +147,323 @@
         """
         value = len(cls.__members__) + 1
         obj = object.__new__(cls)
         obj._value_ = (value, annotation)
         obj._annotation_ = annotation
         return obj
 
-    PreAddCommand: Event = Callable[[Namespace], None]  # type: ignore[assignment]
+    PreAddCommand: Event = Callable[["commands.AddCommand"], None]  # type: ignore[assignment]
     """
     Fires:
         Before starting the `cobib.commands.add.AddCommand`.
 
     Arguments:
-        - `largs`: the `Namespace` dictionary of command arguments.
+        - `cobib.commands.add.AddCommand`: the command instance that is about to run.
 
     Returns:
-        Nothing. But the `Namespace` can be modified, affecting the command execution.
+        Nothing. But the command attributes can be modified, affecting the execution.
     """
-    PostAddCommand: Event = Callable[[Dict[str, "Entry"]], None]  # type: ignore[assignment]
+    PostAddCommand: Event = Callable[["commands.AddCommand"], None]  # type: ignore[assignment]
     """
     Fires:
         Before finishing the `cobib.commands.add.AddCommand`.
 
     Arguments:
-        - `new_entries`: the dictionary of new entries to be added to the database.
+        - `cobib.commands.add.AddCommand`: the command instance that just ran.
 
     Returns:
-        Nothing. But the dictionary of new entries can be modified before the changes are made
-        persistent in the database.
+        Nothing. But the command attributes can be modified, affecting the execution.
 
     Note:
         This event fires *before* starting the `cobib.commands.edit.EditCommand` which starts if
         manual entry addition is requested.
     """
 
-    PreDeleteCommand: Event = Callable[[Namespace], None]  # type: ignore[assignment]
+    PreDeleteCommand: Event = Callable[["commands.DeleteCommand"], None]  # type: ignore[assignment]
     """
     Fires:
         Before starting the `cobib.commands.delete.DeleteCommand`.
 
     Arguments:
-        - `largs`: the `Namespace` dictionary of command arguments.
+        - `cobib.commands.delete.DeleteCommand`: the command instance that is about to run.
+
+    Returns:
+        Nothing. But the command attributes can be modified, affecting the execution.
+    """
+    PostDeleteCommand: Event = Callable[  # type: ignore[assignment]
+        ["commands.DeleteCommand"], None
+    ]
+    """
+    Fires:
+        Before finishing the `cobib.commands.delete.DeleteCommand`.
+
+    Arguments:
+        - `cobib.commands.delete.DeleteCommand`: the command instance that just ran.
 
     Returns:
-        Nothing. But the `Namespace` can be modified, affecting the command execution.
+        Nothing. While the deleted entry labels are accessible, modifying them has no effect.
     """
-    PostDeleteCommand: Event = Callable[[Set[str]], None]  # type: ignore[assignment]
-    """Gets fired before finishing the `cobib.commands.DeleteCommand`. The deleted entry labels are
-    provided as input. Modifying them has no effect."""
 
-    PreEditCommand: Event = Callable[[Namespace], None]  # type: ignore[assignment]
+    PreEditCommand: Event = Callable[["commands.EditCommand"], None]  # type: ignore[assignment]
     """
     Fires:
         Before starting the `cobib.commands.edit.EditCommand`.
 
     Arguments:
-        - `largs`: the `Namespace` dictionary of command arguments.
+        - `cobib.commands.edit.EditCommand`: the command instance that is about to run.
+
+    Returns:
+        Nothing. But the command attributes can be modified, affecting the execution.
+    """
+    PostEditCommand: Event = Callable[["commands.EditCommand"], None]  # type: ignore[assignment]
+    """
+    Fires:
+        Before finishing the `cobib.commands.edit.EditCommand`.
+
+    Arguments:
+        - `cobib.commands.edit.EditCommand`: the command instance that just ran.
 
     Returns:
-        Nothing. But the `Namespace` can be modified, affecting the command execution.
+        Nothing. While the edited entry is accessible, modifying it has no effect.
     """
-    PostEditCommand: Event = Callable[["Entry"], None]  # type: ignore[assignment]
-    """Gets fired before finishing the `cobib.commands.EditCommand`. The new entry gets provided as
-    input and it may be modified. However, renaming the label will no longer be possible."""
 
-    PreExportCommand: Event = Callable[[Namespace], None]  # type: ignore[assignment]
+    PreExportCommand: Event = Callable[["commands.ExportCommand"], None]  # type: ignore[assignment]
     """
     Fires:
         Before starting the `cobib.commands.export.ExportCommand`.
 
     Arguments:
-        - `largs`: the `Namespace` dictionary of command arguments.
+        - `cobib.commands.export.ExportCommand`: the command instance that is about to run.
 
     Returns:
-        Nothing. But the `Namespace` can be modified, affecting the command execution.
+        Nothing. But the command attributes can be modified, affecting the execution.
     """
-    PostExportCommand: Event = Callable[[List[str], Namespace], None]  # type: ignore[assignment]
+    PostExportCommand: Event = Callable[  # type: ignore[assignment]
+        ["commands.ExportCommand"], None
+    ]
     """
     Fires:
         Before finishing the `cobib.commands.export.ExportCommand`.
 
     Arguments:
-        - `labels`: the list of exported labels.
-        - `largs`: the `Namespace` dictionary of command arguments.
+        - `cobib.commands.export.ExportCommand`: the command instance that just ran.
 
     Returns:
-        Nothing.
-
-    Note:
-        If exporting to a zip file, it will only be closed *after* this event got fired.
+        Nothing. The files to which has been exported are still accessible and open.
     """
 
-    PreImportCommand: Event = Callable[[Namespace], None]  # type: ignore[assignment]
+    PreImportCommand: Event = Callable[["commands.ImportCommand"], None]  # type: ignore[assignment]
     """
     Fires:
         Before starting the `cobib.commands.import_.ImportCommand`.
 
     Arguments:
-        - `largs`: the `Namespace` dictionary of command arguments.
+        - `cobib.commands.import_.ImportCommand`: the command instance that is about to run.
 
     Returns:
-        Nothing. But the `Namespace` can be modified, affecting the command execution.
+        Nothing. But the command attributes can be modified, affecting the execution.
     """
-    PostImportCommand: Event = Callable[[Dict[str, "Entry"]], None]  # type: ignore[assignment]
+    PostImportCommand: Event = Callable[  # type: ignore[assignment]
+        ["commands.ImportCommand"], None
+    ]
     """
     Fires:
         Before finishing the `cobib.commands.import_.ImportCommand`.
 
     Arguments:
-        - `new_entries`: the dictionary of new entries to be imported into the database.
+        - `cobib.commands.import_.ImportCommand`: the command instance that just ran.
 
     Returns:
         Nothing. But the dictionary of new entries can be modified before the changes are made
         persistent in the database.
     """
 
-    PreInitCommand: Event = Callable[[Namespace], None]  # type: ignore[assignment]
+    PreInitCommand: Event = Callable[["commands.InitCommand"], None]  # type: ignore[assignment]
     """
     Fires:
         Before starting the `cobib.commands.init.InitCommand`.
 
     Arguments:
-        - `largs`: the `Namespace` dictionary of command arguments.
+        - `cobib.commands.init.InitCommand`: the command instance that is about to run.
 
     Returns:
-        Nothing. But the `Namespace` can be modified, affecting the command execution.
+        Nothing. But the command attributes can be modified, affecting the execution.
     """
-    PostInitCommand: Event = Callable[[Path, Path], None]  # type: ignore[assignment]
+    PostInitCommand: Event = Callable[["commands.InitCommand"], None]  # type: ignore[assignment]
     """
     Fires:
         Before finishing the `cobib.commands.init.InitCommand`.
 
     Arguments:
-        - `root`: the `Path` to the root directory where the database file resides.
-        - `file`: the `Path` to the database file.
+        - `cobib.commands.init.InitCommand`: the command instance that just ran.
 
     Returns:
         Nothing.
     """
 
-    PreListCommand: Event = Callable[[Namespace], None]  # type: ignore[assignment]
+    PreListCommand: Event = Callable[["commands.ListCommand"], None]  # type: ignore[assignment]
     """
     Fires:
-        Before starting the `cobib.commands.list.ListCommand`.
+        Before starting the `cobib.commands.list_.ListCommand`.
 
     Arguments:
-        - `largs`: the `Namespace` dictionary of command arguments.
+        - `cobib.commands.list_.ListCommand`: the command instance that is about to run.
 
     Returns:
-        Nothing. But the `Namespace` can be modified, affecting the command execution.
+        Nothing. But the command attributes can be modified, affecting the execution.
     """
-    PostListCommand: Event = Callable[[List[str]], None]  # type: ignore[assignment]
+    PostListCommand: Event = Callable[["commands.ListCommand"], None]  # type: ignore[assignment]
     """
     Fires:
-        Before finishing the `cobib.commands.list.ListCommand`.
+        Before finishing the `cobib.commands.list_.ListCommand`.
 
     Arguments:
-        - `labels`: the list of labels.
+        - `cobib.commands.list_.ListCommand`: the command instance that just ran.
 
     Returns:
         Nothing.
     """
 
-    PreModifyCommand: Event = Callable[[Namespace], None]  # type: ignore[assignment]
+    PreModifyCommand: Event = Callable[["commands.ModifyCommand"], None]  # type: ignore[assignment]
     """
     Fires:
         Before starting the `cobib.commands.modify.ModifyCommand`.
 
     Arguments:
-        - `largs`: the `Namespace` dictionary of command arguments.
+        - `cobib.commands.modify.ModifyCommand`: the command instance that is about to run.
 
     Returns:
-        Nothing. But the `Namespace` can be modified, affecting the command execution.
+        Nothing. But the command attributes can be modified, affecting the execution.
     """
-    PostModifyCommand: Event = Callable[[List[str], bool], None]  # type: ignore[assignment]
+    PostModifyCommand: Event = Callable[  # type: ignore[assignment]
+        ["commands.ModifyCommand"], None
+    ]
     """
     Fires:
         Before finishing the `cobib.commands.modify.ModifyCommand`.
 
     Arguments:
-        - `labels`: the list of modified labels.
-        - `dry`: whether the command was run in dry-mode.
+        - `cobib.commands.modify.ModifyCommand`: the command instance that just ran.
 
     Returns:
-        Nothing.
+        Nothing. But the modified entries are still accessible before written to the database.
     """
 
-    PreOpenCommand: Event = Callable[[Namespace], None]  # type: ignore[assignment]
+    PreOpenCommand: Event = Callable[["commands.OpenCommand"], None]  # type: ignore[assignment]
     """
     Fires:
         Before starting the `cobib.commands.open.OpenCommand`.
 
     Arguments:
-        - `largs`: the `Namespace` dictionary of command arguments.
+        - `cobib.commands.open.OpenCommand`: the command instance that is about to run.
 
     Returns:
-        Nothing. But the `Namespace` can be modified, affecting the command execution.
+        Nothing. But the command attributes can be modified, affecting the execution.
     """
-    PostOpenCommand: Event = Callable[[List[str]], None]  # type: ignore[assignment]
+    PostOpenCommand: Event = Callable[["commands.OpenCommand"], None]  # type: ignore[assignment]
     """
     Fires:
         Before finishing the `cobib.commands.open.OpenCommand`.
 
     Arguments:
-        - `labels`: the list of opened labels.
+        - `cobib.commands.open.OpenCommand`: the command instance that just ran.
 
     Returns:
         Nothing.
     """
 
-    PreRedoCommand: Event = Callable[[Namespace], None]  # type: ignore[assignment]
+    PreRedoCommand: Event = Callable[["commands.RedoCommand"], None]  # type: ignore[assignment]
     """
     Fires:
         Before starting the `cobib.commands.redo.RedoCommand`.
 
     Arguments:
-        - `largs`: the `Namespace` dictionary of command arguments.
+        - `cobib.commands.redo.RedoCommand`: the command instance that is about to run.
 
     Returns:
-        Nothing. But the `Namespace` can be modified, affecting the command execution.
-
-    Note:
-        As of right now, the `redo` command does not take any arguments, so there is nothing to
-        modify here.
+        Nothing. But the command attributes can be modified, affecting the execution.
     """
-    PostRedoCommand: Event = Callable[[Path, str], None]  # type: ignore[assignment]
+    PostRedoCommand: Event = Callable[["commands.RedoCommand"], None]  # type: ignore[assignment]
     """
     Fires:
         Before finishing the `cobib.commands.redo.RedoCommand`.
 
     Arguments:
-        - `root`: the `Path` to the root directory where the database file resides.
-        - `sha`: the SHA of the redone git-commit.
+        - `cobib.commands.redo.RedoCommand`: the command instance that just ran.
 
     Returns:
         Nothing.
     """
 
-    PreSearchCommand: Event = Callable[[Namespace], None]  # type: ignore[assignment]
+    PreSearchCommand: Event = Callable[["commands.SearchCommand"], None]  # type: ignore[assignment]
     """
     Fires:
         Before starting the `cobib.commands.search.SearchCommand`.
 
     Arguments:
-        - `largs`: the `Namespace` dictionary of command arguments.
+        - `cobib.commands.search.SearchCommand`: the command instance that is about to run.
 
     Returns:
-        Nothing. But the `Namespace` can be modified, affecting the command execution.
+        Nothing. But the command attributes can be modified, affecting the execution.
     """
-    PostSearchCommand: Event = Callable[[int, List[str]], None]  # type: ignore[assignment]
+    PostSearchCommand: Event = Callable[  # type: ignore[assignment]
+        ["commands.SearchCommand"], None
+    ]
     """
     Fires:
         Before finishing the `cobib.commands.search.SearchCommand`.
 
     Arguments:
-        - `hits`: the number of matches found in the database.
-        - `labels`: the list of matching labels.
+        - `cobib.commands.search.SearchCommand`: the command instance that just ran.
 
     Returns:
-        Nothing.
+        Nothing. But the search results are still accessible before being rendered for the user.
     """
 
-    PreShowCommand: Event = Callable[[Namespace], None]  # type: ignore[assignment]
+    PreShowCommand: Event = Callable[["commands.ShowCommand"], None]  # type: ignore[assignment]
     """
     Fires:
         Before starting the `cobib.commands.show.ShowCommand`.
 
     Arguments:
-        - `largs`: the `Namespace` dictionary of command arguments.
+        - `cobib.commands.show.ShowCommand`: the command instance that is about to run.
 
     Returns:
-        Nothing. But the `Namespace` can be modified, affecting the command execution.
+        Nothing. But the command attributes can be modified, affecting the execution.
     """
-    PostShowCommand: Event = Callable[[str], Optional[str]]  # type: ignore[assignment]
+    PostShowCommand: Event = Callable[["commands.ShowCommand"], None]  # type: ignore[assignment]
     """
     Fires:
         Before finishing the `cobib.commands.show.ShowCommand`.
 
     Arguments:
-        - `entry_str`: the formatted string-representation of the shown `Entry`.
+        - `cobib.commands.show.ShowCommand`: the command instance that just ran.
 
     Returns:
-        Optionally a new (or updated) string to represent the shown `Entry`.
-
-    Note:
-        If a registered hook returns a new string, no subsequent hooks will be run!
+        Nothing. But the string-represented entry is still accessible before being rendered.
     """
 
-    PreUndoCommand: Event = Callable[[Namespace], None]  # type: ignore[assignment]
+    PreUndoCommand: Event = Callable[["commands.UndoCommand"], None]  # type: ignore[assignment]
     """
     Fires:
         Before starting the `cobib.commands.undo.UndoCommand`.
 
     Arguments:
-        - `largs`: the `Namespace` dictionary of command arguments.
+        - `cobib.commands.undo.UndoCommand`: the command instance that is about to run.
 
     Returns:
-        Nothing. But the `Namespace` can be modified, affecting the command execution.
+        Nothing. But the command attributes can be modified, affecting the execution.
     """
-    PostUndoCommand: Event = Callable[[Path, str], None]  # type: ignore[assignment]
+    PostUndoCommand: Event = Callable[["commands.UndoCommand"], None]  # type: ignore[assignment]
     """
     Fires:
         Before finishing the `cobib.commands.undo.UndoCommand`.
 
     Arguments:
-        - `root`: the `Path` to the root directory where the database file resides.
-        - `sha`: the SHA of the undone git-commit.
+        - `cobib.commands.undo.UndoCommand`: the command instance that just ran.
 
     Returns:
         Nothing.
     """
 
     PreBibtexParse: Event = Callable[[str], Optional[str]]  # type: ignore[assignment]
     """
@@ -456,15 +493,15 @@
     """
     PreBibtexDump: Event = Callable[["Entry"], None]  # type: ignore[assignment]
     """
     Fires:
         Before starting `cobib.parsers.bibtex.BibtexParser.dump`.
 
     Arguments:
-        - `Entry`: the `Entry` object to be dumped in BibTeX format.
+        - `cobib.database.Entry`: the `Entry` object to be dumped in BibTeX format.
 
     Returns:
         Nothing. But the object can be modified in-place. Changes will *not* become persistent in
         the database.
     """
     PostBibtexDump: Event = Callable[[str], Optional[str]]  # type: ignore[assignment]
     """
@@ -509,15 +546,15 @@
     """
     PreYAMLDump: Event = Callable[["Entry"], None]  # type: ignore[assignment]
     """
     Fires:
         Before starting `cobib.parsers.yaml.YAMLParser.dump`.
 
     Arguments:
-        - `Entry`: the `Entry` object to be dumped in YAML format.
+        - `cobib.database.Entry`: the `Entry` object to be dumped in YAML format.
 
     Returns:
         Nothing. But the object can be modified in-place. Changes will *not* become persistent in
         the database.
     """
     PostYAMLDump: Event = Callable[[str], Optional[str]]  # type: ignore[assignment]
     """
@@ -639,47 +676,41 @@
 
     Returns:
         Nothing. But the dictionary can be modified in-place such that the changes will be
         propagated to the database.
     """
 
     PreZoteroImport: Event = Callable[  # type: ignore[assignment]
-        [str, Dict[str, str]], Optional[Tuple[str, Dict[str, str]]]
+        ["importers.ZoteroImporter"], None
     ]
     """
     Fires:
         Before starting `cobib.importers.zotero.ZoteroImporter.fetch`.
 
     Arguments:
-        - `url`: the URL from which to fetch the Zotero library.
-        - `authentication`: the authentication dictionary header for the GET request.
+        - `cobib.importers.zotero.ZoteroImporter`: the importer instance that is about to run.
 
     Returns:
-        This can optionally return a tuple overwriting the input arguments.
-
-    Note:
-        If a registered hook returns a new tuple of arguments, no subsequent hooks will be run!
+        Nothing. But the importer attributes can be modified, affecting the execution.
     """
-
     PostZoteroImport: Event = Callable[  # type: ignore[assignment]
-        [List["Entry"]], Optional[List["Entry"]]
+        ["importers.ZoteroImporter"], None
     ]
     """
     Fires:
         Before finishing `cobib.importers.zotero.ZoteroImporter.fetch`.
 
     Arguments:
-        - `imported_entries`: the list of entries to be imported.
+        - `cobib.importers.zotero.ZoteroImporter`: the importer instance that is about to run.
 
     Returns:
-        This can optionally return an updated list of imported entries.
+        Nothing. But the importer attributes can be modified, affecting the execution.
 
     Note:
         - The entry labels will not have been mapped or disambiguated at this point.
-        - If a registered hook returns a new tuple of arguments, no subsequent hooks will be run!
     """
 
     PreFileDownload: Event = Callable[  # type: ignore[assignment]
         [str, str, Optional[str], Optional[Dict[str, str]]],
         Optional[Tuple[str, str, Optional[str], Optional[Dict[str, str]]]],
     ]
     """
```

### Comparing `cobib-3.5.5/src/cobib/database/database.py` & `cobib-4.0.0/src/cobib/database/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,15 @@
             return label
 
         LOGGER.warning("Label '%s' already exists in database. Running disambiguation.", label)
         separator, enumerator = config.database.format.label_suffix
         offset = 0
         while True:
             offset += 1
-            new_label: str = label + separator + enumerator(offset)
+            new_label: str = label + separator + enumerator(offset)  # type: ignore[operator]
             if new_label not in self.keys():
                 LOGGER.info("Found new unique label: %s", new_label)
                 return new_label
 
     @classmethod
     def read(cls) -> None:
         """Reads the database file.
```

### Comparing `cobib-3.5.5/src/cobib/database/entry.py` & `cobib-4.0.0/src/cobib/database/entry.py`

 * *Files 2% similar despite different names*

```diff
@@ -232,19 +232,16 @@
 
         Returns:
             An `Entry` with purely string fields.
         """
         data = {}
         data["label"] = self.label
         for field, value in self.data.items():
-            if (
-                isinstance(value, list)
-                and field in config["database"]["stringify"]["list_separator"].keys()
-            ):
-                data[field] = config["database"]["stringify"]["list_separator"][field].join(value)
+            if isinstance(value, list) and hasattr(config.database.stringify.list_separator, field):
+                data[field] = getattr(config.database.stringify.list_separator, field).join(value)
             else:
                 data[field] = str(value)
         return data
 
     def escape_special_chars(self, suppress_warnings: bool = True) -> None:
         """Escapes special characters in the bibliographic data.
 
@@ -292,24 +289,26 @@
         if parser is None:
             # pylint: disable=import-outside-toplevel,cyclic-import
             from cobib.parsers.yaml import YAMLParser
 
             parser = YAMLParser()
         return parser.dump(self) or ""  # `dump` may return `None`
 
-    def matches(self, filter_: Dict[Tuple[str, bool], List[str]], or_: bool) -> bool:
+    def matches(
+        self, filter_: Dict[Tuple[str, bool], List[str]], or_: bool, ignore_case: bool = False
+    ) -> bool:
         """Check whether this entry matches the supplied filter.
 
         coBib provides an extensive filtering implementation. The filter is specified in the form
         of a dictionary whose keys consist of pairs of `(str, bool)` entries where the string
         indicates the field to match against and the boolean whether a positive (`true`) or negative
         (`false`) match is required. The values of the dictionary must be a `List[str]`. This means
         that field types are always compared on a string-basis (this is a limitation of the targeted
         command-line interface). However, as of v3.2.0 these strings are interpreted as regex
-        patterns providing the most powerful within this framework.
+        patterns providing the most power within this framework.
 
         Some examples:
 
         | `filter_`                             | `or_`    | Meaning                               |
         | ------------------------------------- | -------- | ------------------------------------- |
         | `{('year', True): ['2020']}`          | *either* | `year` contains 2020                  |
         | `{('year', False): ['2020']}`         | *either* | `year` does not contain 2020          |
@@ -317,102 +316,107 @@
         | `{('year', True): ['2020', '2021']}`  | False    | cannot match anything                 |
         | `{('year', False): ['2020', '2021']}` | False    | `year` contains neither 2020 nor 2021 |
 
         Args:
             filter_: dictionary describing the filter as explained above.
             or_ : boolean indicating whether logical OR (`true`) or AND (`false`) is used to combine
                 multiple filter items.
+            ignore_case: if True, the matching will be case-*in*sensitive.
 
         Returns:
             Boolean indicating whether this entry matches the filter.
         """
         LOGGER.debug("Checking whether entry %s matches.", self.label)
+        re_flags = re.IGNORECASE if ignore_case else 0
         match_list = []
         stringified_data = self.stringify()
         for key, values in filter_.items():
             if key[0] not in stringified_data:
                 match_list.append(not key[1])
                 continue
             for val in values:
-                if re.search(rf"{val}", stringified_data[key[0]]):
+                if re.search(rf"{val}", stringified_data[key[0]], flags=re_flags):
                     match_list.append(key[1])
                 else:
                     match_list.append(not key[1])
         if or_:
             return any(m for m in match_list)
         return all(m for m in match_list)
 
-    def search(self, query: str, context: int = 1, ignore_case: bool = False) -> List[List[str]]:
-        """Search entry contents for the query string.
+    def search(
+        self, query: List[str], context: int = 1, ignore_case: bool = False
+    ) -> List[List[str]]:
+        """Search entry contents for the query strings.
 
         The entry will *always* be converted to a searchable string using the
-        `cobib.parsers.BibtexParser.dump` method. This text will then be search for `query` which
-        will be interpreted as a regex pattern.
+        `cobib.parsers.BibtexParser.dump` method. This text will then be search for each item in
+        `query` and will interpret these as regex patterns.
         If a `file` is associated with this entry, the search will try its best to recursively query
         its contents, too. However, the success of this depends highly on the configured search
-        tool, `config.commands.search.grep`.
+        tool, `cobib.config.config.SearchCommandConfig.grep`.
 
         Args:
-            query: the text to search for.
+            query: the list of regex patterns to search for.
             context: the number of context lines to provide for each match. This behaves similarly
                 to the *Context Line Control* available for the UNIX `grep` command (`--context`).
             ignore_case: if True, the search will be case-*in*sensitive.
 
         Returns:
             A list of lists containing the context for each match associated with this entry.
         """
-        LOGGER.debug("Searching entry %s for %s.", self.label, query)
+        LOGGER.debug("Searching entry %s.", self.label)
         matches: List[List[str]] = []
         # pylint: disable=import-outside-toplevel,cyclic-import
         from cobib.parsers.bibtex import BibtexParser
 
         bibtex = BibtexParser().dump(self).split("\n")
         re_flags = re.IGNORECASE if ignore_case else 0
-        re_compiled = re.compile(rf"{query}", flags=re_flags)
-        for idx, line in enumerate(bibtex):
-            if re_compiled.search(line):
-                # add new match
-                matches.append([])
-                # upper context; (we iterate in reverse in order to ensure that we abort on the
-                # first previous occurrence of the query pattern)
-                for string in reversed(bibtex[max(idx - context, 0) : min(idx, len(bibtex))]):
-                    if re_compiled.search(string):
-                        break
-                    matches[-1].insert(0, string)
-                # matching line itself
-                matches[-1].append(line)
-                # lower context
-                for string in bibtex[max(idx + 1, 0) : min(idx + context + 1, len(bibtex))]:
-                    if re_compiled.search(string):
-                        break
-                    matches[-1].append(string)
-
-        for file_ in self.file:
-            grep_prog = config.commands.search.grep
-            path = RelPath(file_).path
-            if not path.exists():
-                LOGGER.warning(
-                    "The associated file %s of entry %s does not exist!", file_, self.label
-                )
-                continue
-
-            LOGGER.debug("Searching associated file %s with %s", file_, grep_prog)
-            with subprocess.Popen(
-                [
-                    grep_prog,
-                    *config.commands.search.grep_args,
-                    f"-C{context}",
-                    query,
-                    RelPath(file_).path,
-                ],
-                stdout=subprocess.PIPE,
-            ) as grep:
-                if grep.stdout is None:
+        for query_str in query:
+            re_compiled = re.compile(rf"{query_str}", flags=re_flags)
+            for idx, line in enumerate(bibtex):
+                if re_compiled.search(line):
+                    # add new match
+                    matches.append([])
+                    # upper context; (we iterate in reverse in order to ensure that we abort on the
+                    # first previous occurrence of the query pattern)
+                    for string in reversed(bibtex[max(idx - context, 0) : min(idx, len(bibtex))]):
+                        if re_compiled.search(string):
+                            break
+                        matches[-1].insert(0, string)
+                    # matching line itself
+                    matches[-1].append(line)
+                    # lower context
+                    for string in bibtex[max(idx + 1, 0) : min(idx + context + 1, len(bibtex))]:
+                        if re_compiled.search(string):
+                            break
+                        matches[-1].append(string)
+
+            for file_ in self.file:
+                grep_prog = config.commands.search.grep
+                path = RelPath(file_).path
+                if not path.exists():
+                    LOGGER.warning(
+                        "The associated file %s of entry %s does not exist!", file_, self.label
+                    )
                     continue
-                stdout = grep.stdout
-                # extract results
-                results = stdout.read().decode().split("\n--\n")
-            for match in results:
-                if match:
-                    matches.append([line.strip() for line in match.split("\n") if line.strip()])
+
+                LOGGER.debug("Searching associated file %s with %s", file_, grep_prog)
+                with subprocess.Popen(
+                    [
+                        grep_prog,
+                        *config.commands.search.grep_args,
+                        f"-C{context}",
+                        query_str,
+                        RelPath(file_).path,
+                    ],
+                    stdout=subprocess.PIPE,
+                ) as grep:
+                    if grep.stdout is None:
+                        continue
+                    stdout = grep.stdout
+                    # extract results
+                    results = stdout.read().decode().split("\n--\n")
+                for match in results:
+                    if match:
+                        matches.append([line.strip() for line in match.split("\n") if line.strip()])
 
         return matches
```

### Comparing `cobib-3.5.5/src/cobib/importers/zotero.py` & `cobib-4.0.0/src/cobib/importers/zotero.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """coBib's Zotero importer.
 
 This importer handles migrating from [Zotero][1] to coBib.
 Normally, you would only need to trigger this migration once, but for convenience, coBib will store
 the OAuth authentication tokens provided by the Zotero API in its cache (whose location is
-configurable via `config.logging.cache`).
+configurable via `cobib.config.config.LoggingConfig.cache`).
 
 The importer is registered under the `--zotero` command-line argument of the
 `cobib.commands.import_.ImportCommand`. Thus, you can trigger it like so:
 ```
 cobib import --zotero
 ```
 
@@ -35,39 +35,52 @@
 ```
 cobib import --zotero -- --user-id <user ID> --api-key <API key>
 ```
 
 [1]: https://www.zotero.org/
 """
 
-import argparse
+from __future__ import annotations
+
 import json
 import logging
 import os
 import subprocess
 import sys
 from typing import Dict, List
 
 import requests
 from requests_oauthlib import OAuth1Session
+from typing_extensions import override
 
-from cobib.commands.base_command import ArgumentParser
 from cobib.config import Event, config
 from cobib.database import Entry
 from cobib.parsers import BibtexParser
 from cobib.utils.file_downloader import FileDownloader
 from cobib.utils.rel_path import RelPath
 
-from .base_importer import Importer
+from .base_importer import ArgumentParser, Importer
 
 LOGGER = logging.getLogger(__name__)
 
 
 class ZoteroImporter(Importer):
-    """The Zotero Importer."""
+    """The Zotero Importer.
+
+    This importer can parse the following arguments:
+
+        * `--no-cache`: disables the use of any cached OAuth tokens.
+        * `--user-id`: the Zotero user ID used for API calls. You can find your user ID at
+          <https://www.zotero.org/settings/keys>. Unless you also specify `--no-cache`, this value
+          will be stored in coBib's internal cache. If you do not also provide an `--api-key`, you
+          can only read publicly available Zotero databases.
+        * `--api-key`: overwrites the user-specific Zotero API key for the coBib application. Unless
+          you also specify `--no-cache`, this value will be stored in coBib's internal cache. This
+          argument only takes effect if `--user-id` is also provided.
+    """
 
     name = "zotero"
 
     _CLIENT_KEY = "94a2f739acd6be46df50"
     """The key given to the coBib application by the Zotero API."""
     _CLIENT_SECRET = "8d2659a20871036a462f"
     """The secret given to the coBib application by the Zotero API."""
@@ -75,14 +88,130 @@
     OAUTH_REQUEST_URL = "https://www.zotero.org/oauth/request"
     """The URL from which to initiate OAuth authentication token requests."""
     OAUTH_ACCESS_URL = "https://www.zotero.org/oauth/access"
     """The URL from which to fetch generated OAuth authentication token."""
     OAUTH_AUTHORIZE_URL = "https://www.zotero.org/oauth/authorize"
     """The URL where the user must be redirected in order to authenticate the coBib appliation."""
 
+    @override
+    def __init__(self, *args: str, skip_download: bool = False) -> None:
+        super().__init__(*args, skip_download=skip_download)
+
+        self.authentication: dict[str, str] = {}
+        """The authentication dictionary used as a header during the `GET` request of the Zotero
+        API."""
+
+        self.protected_url: str = ""
+        """The protected URL via which the Zotero API gets accessed."""
+
+        self.imported_entries: list[Entry] = []
+        """A list of `cobib.database.Entry` objects which were imported by this importer."""
+
+    @override
+    @classmethod
+    def init_argparser(cls) -> None:
+        parser = ArgumentParser(prog="zotero", description="Zotero migration parser.")
+        parser.add_argument(
+            "--no-cache", action="store_true", help="disable use of cached OAuth tokens"
+        )
+        parser.add_argument(
+            "--api-key", type=str, help="the user-specific Zotero API key for the coBib application"
+        )
+        parser.add_argument("--user-id", type=str, help="the Zotero user ID used for API calls")
+
+        cls.argparser = parser
+
+    @override
+    async def fetch(self) -> List[Entry]:  # type: ignore[override]
+        # pylint: disable=invalid-overridden-method
+        LOGGER.debug("Starting Zotero fetching.")
+
+        if self.largs.user_id is not None:
+            self.authentication["UserID"] = self.largs.user_id
+            if self.largs.api_key is not None:
+                self.authentication["Zotero-API-Key"] = self.largs.api_key
+
+            if not self.largs.no_cache:
+                self._store_oauth_tokens(self.authentication)
+        else:
+            self.authentication = self._get_authentication_tokens(self.largs.no_cache)
+
+        user_id = self.authentication.pop("UserID")
+
+        LOGGER.info("Requesting items from Zotero user via API v3.")
+        self.protected_url = f"https://api.zotero.org/users/{user_id}/items?include=biblatex&v=3"
+
+        Event.PreZoteroImport.fire(self)
+
+        raw_result = requests.get(self.protected_url, headers=self.authentication, timeout=30)
+
+        bibtex_parser = BibtexParser()
+
+        results = json.loads(raw_result.content)
+
+        encountered_attachments: Dict[str, Dict[str, str]] = {}
+
+        for res in results:
+            biblatex = res.get("biblatex", "").strip()
+            if not bool(biblatex):
+                # check if this is an attachment
+                try:
+                    attachment_enclosure = res.get("links", {}).get("enclosure", {})
+                    LOGGER.info("Storing encountered attachment: %s", res["key"])
+                    encountered_attachments[res["key"]] = {
+                        "href": attachment_enclosure["href"],
+                        "title": attachment_enclosure["title"],
+                    }
+                except KeyError:
+                    pass
+                continue
+
+            LOGGER.info("Parsing encountered BibLaTeX entry: %s", res["key"])
+            # biblatex contains exactly one entry so we can pop it from the OrderedDict
+            _, new_entry = bibtex_parser.parse(biblatex).popitem()
+
+            # Zotero-specific `journal` keyword handling
+            new_entry.data.pop("shortjournal")
+            new_entry.data["journal"] = new_entry.data.pop("journaltitle")
+
+            # check attachment
+            try:
+                attachment = res.get("links", {}).get("attachment", {})
+            except KeyError:
+                pass
+
+            if attachment.get("attachmentType", None) == "application/pdf":
+                LOGGER.info("Queuing associated attachment for download.")
+                new_entry.data["_download"] = attachment["href"].split("/")[-1]
+
+            self.imported_entries.append(new_entry)
+
+        for entry in self.imported_entries:  # pragma: no cover
+            if "_download" not in entry.data.keys():
+                continue
+
+            key = entry.data.pop("_download")
+            if self.skip_download:
+                LOGGER.info("Skipping attachment download.")
+                continue
+            if key not in encountered_attachments:
+                LOGGER.warning("Skipping unknown attachment: %s", key)
+                continue
+
+            url = encountered_attachments[key]["href"]
+            filename = encountered_attachments[key]["title"]
+
+            path = await FileDownloader().download(url, filename, headers=self.authentication)
+            if path is not None:
+                entry.data["file"] = str(path)
+
+        Event.PostZoteroImport.fire(self)
+
+        return self.imported_entries
+
     @staticmethod
     def _get_fresh_oauth_tokens() -> Dict[str, str]:  # pragma: no cover
         """Obtain new OAuth authentication tokens from the Zotero API.
 
         Returns:
             A dictionary containing the authentication information. More specifically, two values
             will be stored:
@@ -185,135 +314,7 @@
             LOGGER.info("Successfully obtained OAuth tokens for Zotero from cache.")
         else:  # pragma: no cover
             authentication = ZoteroImporter._get_fresh_oauth_tokens()
             if not no_cache:
                 ZoteroImporter._store_oauth_tokens(authentication)
 
         return authentication
-
-    def fetch(self, args: List[str], skip_download: bool = False) -> List[Entry]:
-        """Fetches a list of entries from Zotero.
-
-        Args:
-            args: a sequence of additional arguments used during execution. The following values are
-                allowed for this importer:
-                    * `--no-cache`: disables the use of any cached OAuth tokens.
-                    * `--user-id`: the Zotero user ID used for API calls. You can find your user ID
-                        at <https://www.zotero.org/settings/keys>. Unless you also specify
-                        `--no-cache`, this value will be stored in coBib's internal cache. If you do
-                        not also provide an `--api-key`, you can only read publicly available Zotero
-                        databases.
-                    * `--api-key`: overwrites the user-specific Zotero API key for the coBib
-                        application. Unless you also specify `--no-cache`, this value will be stored
-                        in coBib's internal cache. This argument only takes effect if `--user-id` is
-                        also provided.
-            skip_download: whether or not to skip downloading of additional files such as attached
-                PDF files or notes.
-
-        Returns:
-            A list of entries.
-        """
-        LOGGER.debug("Starting Zotero fetching.")
-        arg_parser = ArgumentParser(prog="zotero", description="Zotero migration parser.")
-        arg_parser.add_argument(
-            "--no-cache", action="store_true", help="disable use of cached OAuth tokens"
-        )
-        arg_parser.add_argument(
-            "--api-key", type=str, help="the user-specific Zotero API key for the coBib application"
-        )
-        arg_parser.add_argument("--user-id", type=str, help="the Zotero user ID used for API calls")
-
-        try:
-            largs = arg_parser.parse_args(args)
-        except argparse.ArgumentError as exc:
-            LOGGER.error(exc.message)
-            return []
-
-        authentication: Dict[str, str] = {}
-        if largs.user_id is not None:
-            authentication["UserID"] = largs.user_id
-            if largs.api_key is not None:
-                authentication["Zotero-API-Key"] = largs.api_key
-
-            if not largs.no_cache:
-                self._store_oauth_tokens(authentication)
-        else:
-            authentication = self._get_authentication_tokens(largs.no_cache)
-
-        user_id = authentication.pop("UserID")
-
-        LOGGER.info("Requesting items from Zotero user via API v3.")
-        protected_url = f"https://api.zotero.org/users/{user_id}/items?include=biblatex&v=3"
-
-        pre_hook_result = Event.PreZoteroImport.fire(protected_url, authentication)
-        if pre_hook_result is not None:
-            protected_url, authentication = pre_hook_result
-
-        raw_result = requests.get(protected_url, headers=authentication, timeout=30)
-
-        bibtex_parser = BibtexParser()
-
-        results = json.loads(raw_result.content)
-
-        imported_entries: List[Entry] = []
-
-        encountered_attachments: Dict[str, Dict[str, str]] = {}
-
-        for res in results:
-            biblatex = res.get("biblatex", "").strip()
-            if not bool(biblatex):
-                # check if this is an attachment
-                try:
-                    attachment_enclosure = res.get("links", {}).get("enclosure", {})
-                    LOGGER.info("Storing encountered attachment: %s", res["key"])
-                    encountered_attachments[res["key"]] = {
-                        "href": attachment_enclosure["href"],
-                        "title": attachment_enclosure["title"],
-                    }
-                except KeyError:
-                    pass
-                continue
-
-            LOGGER.info("Parsing encountered BibLaTeX entry: %s", res["key"])
-            # biblatex contains exactly one entry so we can pop it from the OrderedDict
-            _, new_entry = bibtex_parser.parse(biblatex).popitem()
-
-            # Zotero-specific `journal` keyword handling
-            new_entry.data.pop("shortjournal")
-            new_entry.data["journal"] = new_entry.data.pop("journaltitle")
-
-            # check attachment
-            try:
-                attachment = res.get("links", {}).get("attachment", {})
-            except KeyError:
-                pass
-
-            if attachment.get("attachmentType", None) == "application/pdf":
-                LOGGER.info("Queuing associated attachment for download.")
-                new_entry.data["_download"] = attachment["href"].split("/")[-1]
-
-            imported_entries.append(new_entry)
-
-        for entry in imported_entries:  # pragma: no cover
-            if "_download" not in entry.data.keys():
-                continue
-
-            key = entry.data.pop("_download")
-            if skip_download:
-                LOGGER.info("Skipping attachment download.")
-                continue
-            if key not in encountered_attachments:
-                LOGGER.warning("Skipping unknown attachment: %s", key)
-                continue
-
-            url = encountered_attachments[key]["href"]
-            filename = encountered_attachments[key]["title"]
-
-            path = FileDownloader().download(url, filename, headers=authentication)
-            if path is not None:
-                entry.data["file"] = str(path)
-
-        post_hook_result = Event.PostZoteroImport.fire(imported_entries)
-        if post_hook_result is not None:
-            imported_entries = post_hook_result
-
-        return imported_entries
```

### Comparing `cobib-3.5.5/src/cobib/parsers/__init__.py` & `cobib-4.0.0/src/cobib/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.5/src/cobib/parsers/arxiv.py` & `cobib-4.0.0/src/cobib/parsers/arxiv.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """coBib's arXiv parser.
 
 This parser is capable of generating `cobib.database.Entry` instances from a given arXiv ID.
 It gathers the BibTex-encoded data from the arXiv API and parses the raw XML data.
 
 Since v3.2.0 coBib will also automatically download the PDF version of the new entry. You can
-configure the default download location via `config.utils.file_downloader.default_location`.
+configure the default download location via
+`cobib.config.config.FileDownloaderConfig.default_location`.
 
 Since v3.3.0 this parser even supports URLs from which an arXiv ID can be extracted directly.
 
 The parser is registered under the `-a` and `--arxiv` command-line arguments of the
 `cobib.commands.add.AddCommand`.
 
 The following documentation is mostly inherited from the abstract interface
@@ -18,14 +19,15 @@
 import logging
 import re
 from collections import OrderedDict
 from typing import Any, Dict
 
 import requests
 from bs4 import BeautifulSoup
+from typing_extensions import override
 
 from cobib.config import Event
 from cobib.database import Entry
 
 from .base_parser import Parser
 
 LOGGER = logging.getLogger(__name__)
@@ -37,18 +39,16 @@
 
 
 class ArxivParser(Parser):
     """The arXiv Parser."""
 
     name = "arxiv"
 
+    @override
     def parse(self, string: str) -> Dict[str, Entry]:
-        # pdoc will inherit the docstring from the base class
-        # noqa: D102
-
         string = Event.PreArxivParse.fire(string) or string
 
         try:
             match = re.search(ARXIV_REGEX, string)
             if match is None:
                 raise AssertionError
         except AssertionError:
```

### Comparing `cobib-3.5.5/src/cobib/parsers/base_parser.py` & `cobib-4.0.0/src/cobib/parsers/base_parser.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.5/src/cobib/parsers/bibtex.py` & `cobib-4.0.0/src/cobib/parsers/bibtex.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,45 +1,44 @@
 """coBib's BibTex parser.
 
 This parser leverages the [`bibtexparser`](https://pypi.org/project/bibtexparser/) library to
 convert between `cobib.database.Entry` instances and raw BibTex strings.
 
 Non-standard BibTex types can be configured to be ignored via
-`config.parsers.bibtex.ignore_non_standard_types`.
+`cobib.config.config.BibtexParserConfig.ignore_non_standard_types`.
 
 The parser is registered under the `-b` and `--bibtex` command-line arguments of the
 `cobib.commands.add.AddCommand`.
 
 The following documentation is mostly inherited from the abstract interface
 `cobib.parsers.base_parser`.
 """
 
 import logging
 from collections import OrderedDict
 from typing import Dict
 
 import bibtexparser
+from typing_extensions import override
 
 from cobib.config import Event, config
 from cobib.database import Entry
 
 from .base_parser import Parser
 
 LOGGER = logging.getLogger(__name__)
 
 
 class BibtexParser(Parser):
     """The BibTex Parser."""
 
     name = "bibtex"
 
+    @override
     def parse(self, string: str) -> Dict[str, Entry]:
-        # pdoc will inherit the docstring from the base class
-        # noqa: D102
-
         string = Event.PreBibtexParse.fire(string) or string
 
         bparser = bibtexparser.bparser.BibTexParser()
         bparser.ignore_nonstandard_types = config.parsers.bibtex.ignore_non_standard_types
         bparser.common_strings = True
         bparser.interpolate_strings = False
         try:
@@ -58,18 +57,16 @@
             label = entry.pop("ID")
             bib[label] = Entry(label, entry)
 
         Event.PostBibtexParse.fire(bib)
 
         return bib
 
+    @override
     def dump(self, entry: Entry) -> str:
-        # pdoc will inherit the docstring from the base class
-        # noqa: D102
-
         Event.PreBibtexDump.fire(entry)
 
         database = bibtexparser.bibdatabase.BibDatabase()
         stringified_entry = entry.stringify()
         stringified_entry["ID"] = stringified_entry.pop("label")
         if "month" in stringified_entry.keys():
             # convert month to bibtexexpression
```

### Comparing `cobib-3.5.5/src/cobib/parsers/doi.py` & `cobib-4.0.0/src/cobib/parsers/doi.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """coBib's DOI parser.
 
 This parser is capable of generating `cobib.database.Entry` instances from a given DOI.
 It gathers the BibTex-encoded data from https://doi.org/ and parses it directly using the
 `cobib.parsers.bibtex.BibtexParser`.
 
 Since v3.2.0 coBib will also attempt to download the PDF version of the new entry. You can
-configure the default download location via `config.utils.file_downloader.default_location`.
+configure the default download location via
+`cobib.config.config.FileDownloaderConfig.default_location`.
 Since in general the PDF may not be freely available, your mileage with this feature may vary. Until
 coBib supports internal proxy configurations, make sure you are logged in to a VPN for the smoothest
 experience with closed-source journals.
-Furthermore, you should look into the `config.utils.file_downloader.url_map` setting, through which
-you tell coBib how to map from journal landing page URLs to the corresponding PDF URLs. For more
-information check out `cobib.config.example` and the man-page.
+Furthermore, you should look into the `cobib.config.config.FileDownloaderConfig.url_map` setting,
+through which you tell coBib how to map from journal landing page URLs to the corresponding PDF
+URLs. For more information check out `cobib.config.example` and the man-page.
 
 Since v3.3.0 this parser even supports URLs from which a DOI can be extracted directly.
 
 The parser is registered under the `-d` and `--doi` command-line arguments of the
 `cobib.commands.add.AddCommand`.
 
 The following documentation is mostly inherited from the abstract interface
@@ -24,40 +25,39 @@
 
 import logging
 import re
 from collections import OrderedDict
 from typing import Dict
 
 import requests
+from typing_extensions import override
 
 from cobib.config import Event
 from cobib.database import Entry
 
 from .base_parser import Parser
 from .bibtex import BibtexParser
 
 LOGGER = logging.getLogger(__name__)
 
 DOI_URL = "https://doi.org/"
 """The DOI 'API' URL."""
 DOI_HEADER = {"Accept": "application/x-bibtex"}
 """The DOI 'API' header taken from [here](https://crosscite.org/docs.html)."""
-DOI_REGEX = r'(10\.[0-9a-zA-Z]+\/(?:(?!["&\'])\S)+)\b'
+DOI_REGEX = r'(10\.[0-9a-zA-Z]+\/(?:(?!["&\'\?])\S)+)\b'
 """A regex pattern used to match valid DOIs."""
 
 
 class DOIParser(Parser):
     """The DOI Parser."""
 
     name = "doi"
 
+    @override
     def parse(self, string: str) -> Dict[str, Entry]:
-        # pdoc will inherit the docstring from the base class
-        # noqa: D102
-
         string = Event.PreDOIParse.fire(string) or string
 
         try:
             match = re.search(DOI_REGEX, string)
             if match is None:
                 raise AssertionError
         except AssertionError:
```

### Comparing `cobib-3.5.5/src/cobib/parsers/isbn.py` & `cobib-4.0.0/src/cobib/parsers/isbn.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import json
 import logging
 import re
 from collections import OrderedDict
 from typing import Dict
 
 import requests
+from typing_extensions import override
 
 from cobib.config import Event
 from cobib.database import Entry
 
 from .base_parser import Parser
 
 LOGGER = logging.getLogger(__name__)
@@ -41,18 +42,16 @@
 
 
 class ISBNParser(Parser):
     """The ISBN Parser."""
 
     name = "isbn"
 
+    @override
     def parse(self, string: str) -> Dict[str, Entry]:
-        # pdoc will inherit the docstring from the base class
-        # noqa: D102
-
         string = Event.PreISBNParse.fire(string) or string
 
         try:
             match = re.search(ISBN_REGEX, string)
             if match is None:
                 raise AssertionError
         except AssertionError:
```

### Comparing `cobib-3.5.5/src/cobib/parsers/url.py` & `cobib-4.0.0/src/cobib/parsers/url.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 import logging
 import re
 from collections import Counter, OrderedDict
 from typing import Dict
 
 import requests
+from typing_extensions import override
 
 from cobib.config import Event
 from cobib.database import Entry
 
 from .arxiv import ARXIV_REGEX, ArxivParser
 from .base_parser import Parser
 from .doi import DOI_REGEX, DOIParser
@@ -33,18 +34,16 @@
 
 class URLParser(Parser):
     # pylint: disable=too-many-return-statements
     """The URL Parser."""
 
     name = "url"
 
+    @override
     def parse(self, string: str) -> Dict[str, Entry]:
-        # pdoc will inherit the docstring from the base class
-        # noqa: D102
-
         string = Event.PreURLParse.fire(string) or string
 
         if re.search(ARXIV_REGEX, string):
             LOGGER.debug("URL contains an arXiv ID")
             entries = ArxivParser().parse(string)
             if entries:
                 LOGGER.debug("Successfully extracted metadata from URL with ArxivParser")
```

### Comparing `cobib-3.5.5/src/cobib/parsers/yaml.py` & `cobib-4.0.0/src/cobib/parsers/yaml.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# mypy: warn-unused-ignores=False
 """coBib's YAML parser.
 
 This parser leverages the [`ruamel.yaml`](https://pypi.org/project/ruamel.yaml/) library to convert
 between `cobib.database.Entry` instances and YAML representations of their `dict`-like data
 structure.
 
 The parser is registered under the `-y` and `--yaml` command-line arguments of the
@@ -9,19 +10,23 @@
 
 The following documentation is mostly inherited from the abstract interface
 `cobib.parsers.base_parser`.
 """
 
 import io
 import logging
+import sys
 from collections import OrderedDict
 from pathlib import Path
 from typing import IO, Dict, Optional, Union
 
+from rich.console import Console
+from rich.progress import track
 from ruamel import yaml
+from typing_extensions import override
 
 from cobib.config import Event, config
 from cobib.database.entry import Entry
 
 from .base_parser import Parser
 
 LOGGER = logging.getLogger(__name__)
@@ -39,42 +44,43 @@
         if YAMLParser._yaml is None:
             # we need to lazily construct this in order to be able to respect the config setting
             YAMLParser._yaml = yaml.YAML(typ="safe", pure=not config.parsers.yaml.use_c_lib_yaml)
             YAMLParser._yaml.explicit_start = True  # type: ignore[assignment]
             YAMLParser._yaml.explicit_end = True  # type: ignore[assignment]
             YAMLParser._yaml.default_flow_style = False
 
+    @override
     def parse(self, string: Union[str, Path]) -> Dict[str, Entry]:
-        # pdoc will inherit the docstring from the base class
-        # noqa: D102
-
         string = Event.PreYAMLParse.fire(string) or string
 
         bib = OrderedDict()
         LOGGER.debug("Loading YAML data from file: %s.", string)
         try:
             stream: IO = io.StringIO(Path(string))  # type: ignore[arg-type,type-arg]
         except TypeError:
             try:
                 stream = open(string, "r", encoding="utf-8")  # pylint: disable=consider-using-with
             except FileNotFoundError as exc:
                 raise exc
-        for entry in self._yaml.load_all(stream):  # type: ignore[union-attr]
+        for entry in track(
+            self._yaml.load_all(stream),  # type: ignore[union-attr]
+            description="Reading database...",
+            transient=True,
+            console=Console(file=sys.stderr),  # TODO: do not hard-code this
+        ):
             for label, data in entry.items():
                 bib[label] = Entry(label, data)
         stream.close()
 
         Event.PostYAMLParse.fire(bib)
 
         return bib
 
+    @override
     def dump(self, entry: Entry) -> Optional[str]:
-        # pdoc will inherit the docstring from the base class
-        # noqa: D102
-
         Event.PreYAMLDump.fire(entry)
 
         LOGGER.debug("Converting entry %s to YAML format.", entry.label)
         stream = io.StringIO()
         self._yaml.dump(  # type: ignore[union-attr]
             {entry.label: dict(sorted(entry.data.items()))}, stream=stream
         )
```

### Comparing `cobib-3.5.5/src/cobib/utils/file_downloader.py` & `cobib-4.0.0/src/cobib/utils/file_downloader.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,135 +1,93 @@
 """coBib's file downloader utility."""
 
 from __future__ import annotations
 
 import logging
 import re
-import sys
 import tempfile
+from functools import partial
 from pathlib import Path
-from typing import Callable, Dict, Optional
+from typing import Callable, Dict, Optional, Type
 
 import requests
+from rich.console import Console
+from rich.progress import DownloadColumn, Progress, SpinnerColumn, TimeElapsedColumn
+from textual.widgets import ProgressBar
 
 from cobib.config import Event, config
 
 from .rel_path import RelPath
 
 LOGGER = logging.getLogger(__name__)
 
 
 class FileDownloader:
     """The file downloader singleton.
 
-    This utility centralizes the downloading of associated files. It implements the singleton
-    pattern to allow simple log method replacement (via `set_logger`).
+    This utility centralizes the downloading of associated files.
     """
 
     _instance: Optional[FileDownloader] = None
     """The singleton instance of this class."""
 
-    _logger: Callable[[str], None] = lambda text: print(text, end="", flush=True, file=sys.stdout)
-    """The logging method used to display the downloading progress bar."""
-
     def __new__(cls) -> FileDownloader:
         """Singleton constructor.
 
         This method gets called when accessing `FileDownloader` and enforces the singleton pattern
         implemented by this class.
         """
         if cls._instance is None:
             cls._instance = super().__new__(cls)
         return cls._instance
 
-    @staticmethod
-    def set_logger(log_method: Callable[[str], None]) -> None:
-        """Sets the class-wide logging method (see also `FileDownloader._logger`).
-
-        This method is used to display the progress bar of the file downloading.
-
-        Args:
-            log_method: the logging method.
-        """
-        FileDownloader._logger = log_method
-
-    # bytes pretty-printing
-    _UNITS_MAPPING = [
-        (1 << 50, " PB"),
-        (1 << 40, " TB"),
-        (1 << 30, " GB"),
-        (1 << 20, " MB"),
-        (1 << 10, " KB"),
-        (1, " B"),
-    ]
-    """Maps byte sizes to units."""
-
-    @staticmethod
-    def _size(bytes_: int) -> str:
-        """Human-readable file size.
-
-        Args:
-            bytes_: the size in bytes.
-
-        Returns:
-            The size formatted for easy human readability.
-
-        Reference:
-            https://stackoverflow.com/a/12912296
-        """
-        for factor, suffix in FileDownloader._UNITS_MAPPING:
-            if bytes_ >= factor:
-                break
-        amount = int(bytes_ / factor)
-        return str(amount) + suffix
+    progress: Type[Progress] | Type[ProgressBar] = Progress
+    """The type of progress bar to use when displaying the downloading progress."""
 
     _PDF_MARKER = bytes("%PDF", "utf-8")
     """A marker which the downloaded file's beginning is checked against, to determine that it is
     indeed a PDF file."""
 
     @staticmethod
     def _assert_pdf(content: bytes) -> bool:
         """Asserts that the `content` starts with the `_PDF_MARKER`.
 
         Args:
             content: the string of bytes to check.
 
         Returns:
-            Whether the`content` matches.
+            Whether the `content` matches.
         """
         if not content.startswith(FileDownloader._PDF_MARKER):
             LOGGER.warning("The URL did not provide a PDF file. Aborting download!")
             return False
         return True
 
     @staticmethod
     def _unlink(path: RelPath) -> None:
         """Remove a file and ignore any error.
 
         Args:
             path: the file to remove.
         """
-        try:
-            # TODO: once Python 3.7 is dropped, leverage `missing_ok` argument
-            path.path.unlink()
-        except FileNotFoundError:
-            pass
+        path.path.unlink(missing_ok=True)
 
-    def download(
-        self,
+    @staticmethod
+    async def download(
         url: str,
         label: str,
         folder: Optional[str] = None,
         overwrite: bool = False,
         headers: Optional[Dict[str, str]] = None,
     ) -> Optional[RelPath]:
+        # pylint: disable=too-many-function-args,unexpected-keyword-arg,no-member
         """Downloads a file.
 
         The path of the downloaded file is `folder/label.pdf`. The path can be configured via
-        `cobib.config.commands.add.download_location`.
+        `cobib.config.config.FileDownloaderConfig.default_location`.
 
         Args:
             url: the link to the file to be downloaded.
             label: the name of the entry.
             folder: an optional folder where the downloaded file will be stored.
             overwrite: whether or not to overwrite an existing file.
             headers: optional headers for the download `GET` request.
@@ -150,73 +108,134 @@
         backup = None
         if path.path.exists():
             if not overwrite:
                 LOGGER.warning(
                     "A file at '%s' already exists! Using that rather than downloading.", path
                 )
                 return path
-            # we make a copy of the existing file in case downloading a new one fails
-            backup = tempfile.NamedTemporaryFile()  # pylint: disable=consider-using-with
-            backup.write(path.path.read_bytes())
-            backup.seek(0)
+            backup = FileDownloader._backup_file(path)
 
-        for pattern_url, repl_url in config.utils.file_downloader.url_map.items():
-            if re.match(pattern_url, url):
-                new_url = re.sub(pattern_url, repl_url, url)
-                LOGGER.info(
-                    "Matched the file's URL to your pattern URL %s and replaced it to become %s",
-                    pattern_url,
-                    new_url,
-                )
-                url = new_url
-                break
+        url = FileDownloader._map_url(url)
 
         with open(path.path, "wb") as file:
             LOGGER.info("Downloading %s to %s", url, path)
+
             try:
                 response = requests.get(url, timeout=10, stream=True, headers=headers)
-                total_length = int(response.headers.get("content-length", -1))
+                total_length = response.headers.get("content-length", None)
+                total_length = int(total_length) if total_length is not None else None
             except requests.exceptions.RequestException as err:
                 msg = f"An Exception occurred while downloading the file located at {url}"
                 LOGGER.warning(msg)
                 LOGGER.error(err)
-                FileDownloader._unlink(path)
-                if backup is not None:
-                    path.path.write_bytes(backup.read())
-                    backup.close()
+                FileDownloader._recover(path, backup)
                 return None
-            if total_length < 0:
+
+            advance: Callable[[int], None]
+            progress_bar: Progress | ProgressBar
+            if issubclass(FileDownloader.progress, ProgressBar):
+                progress_bar = FileDownloader.progress(total_length)
+                _, await_mount = progress_bar.console.print(  # type: ignore[attr-defined]
+                    progress_bar
+                )
+                await await_mount
+                advance = progress_bar.advance
+            else:
+                progress_bar = FileDownloader.progress(
+                    SpinnerColumn(),
+                    *Progress.get_default_columns(),
+                    TimeElapsedColumn(),
+                    DownloadColumn(),
+                    transient=False,
+                    # TODO: the unittests fail when this remains `None` because it appears as though
+                    # too many Live sessions are opened at once. How can we deal with this properly?
+                    # Can we simply assume the user is not going to do this in parallel?
+                    console=Console(),
+                )
+                progress_bar.start()
+                task = progress_bar.add_task("Downloading...", total=total_length)
+                advance = partial(progress_bar.advance, task)
+
+            accumulated_length = 0
+
+            if total_length is None:
                 if not FileDownloader._assert_pdf(response.content):
-                    FileDownloader._unlink(path)
-                    if backup is not None:
-                        path.path.write_bytes(backup.read())
-                        backup.close()
+                    FileDownloader._recover(path, backup)
                     return None
                 file.write(response.content)
             else:
-                accumulated_length = 0
-                total_size = self._size(total_length)
                 for data in response.iter_content(chunk_size=4096):
                     if accumulated_length == 0 and not FileDownloader._assert_pdf(data):
-                        FileDownloader._unlink(path)
-                        if backup is not None:
-                            path.path.write_bytes(backup.read())
-                            backup.close()
+                        FileDownloader._recover(path, backup)
                         return None
                     accumulated_length += len(data)
+                    advance(len(data))
                     file.write(data)
-                    percentage = accumulated_length / total_length
-                    progress = int(40 * percentage)
-                    FileDownloader._logger(
-                        "\rDownloading:"
-                        f" [{'=' * progress}{' ' * (40 - progress)}] "
-                        f"{100*percentage:6.1f}%"
-                        f"{self._size(accumulated_length): >7} / {total_size: <7}",
-                    )
-                FileDownloader._logger("\n")
+
+            if isinstance(progress_bar, ProgressBar):
+                progress_bar.set_timer(5.0, progress_bar.remove)
+            else:
+                progress_bar.stop()
+
             msg = f"Successfully downloaded {path}"
             print(msg)
             LOGGER.info(msg)
 
             path = Event.PostFileDownload.fire(path) or path
 
             return path
+
+    @staticmethod
+    def _map_url(url: str) -> str:
+        """Maps a URL according to `cobib.config.config.FileDownloaderConfig.url_map`.
+
+        Args:
+            url: the URL to be mapped.
+
+        Returns:
+            The mapped URL.
+        """
+        for pattern_url, repl_url in config.utils.file_downloader.url_map.items():
+            if re.match(pattern_url, url):
+                new_url: str = re.sub(pattern_url, repl_url, url)
+                LOGGER.info(
+                    "Matched the file's URL to your pattern URL %s and replaced it to become %s",
+                    pattern_url,
+                    new_url,
+                )
+                return new_url
+        return url
+
+    @staticmethod
+    # pylint: disable=unsubscriptable-object
+    def _backup_file(path: RelPath) -> tempfile._TemporaryFileWrapper[bytes]:
+        """Create a backup of an existing file.
+
+        Args:
+            path: the path to the file to be backed up.
+
+        Returns:
+            The temporary backup file.
+        """
+        # we make a copy of the existing file in case downloading a new one fails
+        backup = tempfile.NamedTemporaryFile(delete=False)  # pylint: disable=consider-using-with
+        backup.write(path.path.read_bytes())
+        backup.seek(0)
+        return backup
+
+    @staticmethod
+    # pylint: disable=unsubscriptable-object
+    def _recover(path: RelPath, backup: Optional[tempfile._TemporaryFileWrapper[bytes]]) -> None:
+        """Recovers from a backup file.
+
+        If not `backup` exists, the file location which was supposed to be recovered is properly
+        removed.
+
+        Args:
+            path: the path to the file to be recovered.
+            backup: the temporary backup file.
+        """
+        FileDownloader._unlink(path)
+        if backup is not None:
+            path.path.write_bytes(backup.read())
+            backup.close()
+            Path(backup.name).unlink()
```

### Comparing `cobib-3.5.5/src/cobib/utils/journal_abbreviations.py` & `cobib-4.0.0/src/cobib/utils/journal_abbreviations.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.5/src/cobib/utils/logging.py` & `cobib-4.0.0/src/cobib/utils/logging.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,32 +3,36 @@
 This module provides utility methods to set up logging to different handlers.
 """
 
 import logging
 import logging.handlers
 import sys
 from pathlib import Path
-from typing import Optional, Union
+from typing import List, Optional, Union
 
 from pkg_resources import get_distribution
+from rich.console import ConsoleRenderable, Group
+from rich.markdown import Markdown
+from rich.panel import Panel
+from rich.text import Text
+from typing_extensions import override
 
 from .rel_path import RelPath
 
 
 class _StderrHandler(logging.StreamHandler):  # type: ignore[type-arg]
     """A logging handler hard-coded to `sys.stderr`.
 
     The reason for explicitly deriving this class, is that Python's `logging.StreamHandler` does not
     respect stream redirection. However, for coBib's TUI this is an important requirement which can
     be achieved by a runtime check of the stream during the `emit` method.
     """
 
+    @override
     def emit(self, record: logging.LogRecord) -> None:
-        # pdoc will inherit the docstring from the base class
-        # noqa: D102
         self.stream = sys.stderr
         super().emit(record)
 
 
 def get_stream_handler(
     level: int = logging.WARNING,
 ) -> logging.StreamHandler:  # type: ignore[type-arg]
@@ -75,28 +79,31 @@
     )
     handler.setLevel(level)
     handler.setFormatter(formatter)
 
     return handler
 
 
-def print_changelog(version: str, cached_version_path: Optional[str]) -> None:
-    """Prints the latest section of the CHANGELOG to stdout.
+def print_changelog(version: str, cached_version_path: Optional[str]) -> Optional[Panel]:
+    """Generates a `rich.Panel` to display the changelog since the last displayed version.
 
     This function prints the contents of the CHANGELOG (extracted from the PKG-INFO metadata)
     between the current version (`version`) and the latest cached version (extracted from the
     provided file path).
 
     Args:
         version: the currently running version of coBib.
         cached_version_path: the path to the file which caches the previously executed version of
             coBib. If `None`, this method exits early (thereby silencing this feature).
+
+    Returns:
+        An optional `rich.Panel` with the rendered Markdown.
     """
     if cached_version_path is None:
-        return
+        return None
 
     _cached_version_path = RelPath(cached_version_path).path
     if not _cached_version_path.parent.exists():
         _cached_version_path.parent.mkdir(parents=True)
 
     try:
         current_version = version[: version.index("+")]
@@ -107,53 +114,52 @@
     try:
         with open(_cached_version_path, "r", encoding="utf-8") as version_file:
             cached_version = version_file.read().strip()
     except FileNotFoundError:
         pass
 
     if current_version == cached_version:
-        return
+        return None
 
     with open(_cached_version_path, "w", encoding="utf-8") as version_file:
         version_file.write(current_version)
 
-    lines = ["\x1b[1mHi there! It looks like you have updated coBib; here is what's new:\x1b[22m\n"]
+    groups: List[ConsoleRenderable] = []
+    groups.append(
+        Text(
+            "Hi there! It looks like you have updated coBib; here is what's new:",
+            style="bold yellow",
+        )
+    )
 
     metadata = ""
     try:
         metadata = get_distribution("cobib").get_metadata("METADATA")
     except FileNotFoundError:
         try:
             metadata = get_distribution("cobib").get_metadata("PKG-INFO")
         except FileNotFoundError:
-            lines += [
-                "I wanted to show you the new changes here but was unable to query ",
-                "them from your installation. You can look them up yourself, here: ",
-                "https://gitlab.com/mrossinek/cobib/-/blob/master/CHANGELOG.md",
-            ]
+            groups.append(
+                Text(
+                    "I wanted to show you the new changes here but was unable to query them from "
+                    + "your installation. You can look them up yourself, here:\n"
+                    + "https://gitlab.com/coBib/cobib/-/blob/master/CHANGELOG.md",
+                    style="bold red",
+                )
+            )
+            return Panel(Group(*groups), width=80)
 
-    num_printed_lines = -1
+    lines: List[str] = []
+    started = False
     for line in metadata.splitlines():
         line = line.strip()
         if line.startswith(f"## [{current_version}]"):
-            num_printed_lines = 0
+            started = True
         elif line.startswith(f"## [{cached_version}]"):
-            num_printed_lines = -1
-        elif num_printed_lines >= 20:
-            num_printed_lines = -1
-            lines.extend(
-                [
-                    "\n...\n\x1b[31m",
-                    "This output is shortened for the sake of brevity! For more information visit:",
-                    "https://gitlab.com/mrossinek/cobib/-/blob/master/CHANGELOG.md",
-                ]
-            )
+            break
 
-        if num_printed_lines >= 0:
+        if started:
             lines.append(line)
-            num_printed_lines += 1
 
-    print("\x1b[33m", end="")
-    print("\n".join(lines).strip())
-    print("\x1b[0m", end="", flush=True)
+    groups.append(Markdown("\n".join(lines)))
 
-    input("\nPress Enter to continue...")
+    return Panel(Group(*groups))
```

### Comparing `cobib-3.5.5/src/cobib/utils/rel_path.py` & `cobib-4.0.0/src/cobib/utils/rel_path.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.5/src/cobib/utils/shell_helper.py` & `cobib-4.0.0/src/cobib/utils/shell_helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,45 @@
 """coBib's shell helpers.
 
 This module provides a variety of shell helper utilities.
 """
 # pylint: disable=unused-argument
 
+from __future__ import annotations
+
 import argparse
 import contextlib
 import inspect
 import logging
 from io import StringIO
-from typing import List, Set
+from typing import List, Set, Type
+
+from rich.console import Console
+from rich.prompt import PromptBase
+from textual.app import App
 
 from .rel_path import RelPath
 
 
-def list_commands(args: List[str]) -> List[str]:
+def list_commands(*args: str) -> List[str]:
     """Lists all available subcommands.
 
     Args:
         args: a sequence of additional arguments used for the execution. None are supported yet.
 
     Returns:
         The list of available commands.
     """
     # pylint: disable=import-outside-toplevel
     from cobib import commands
 
     return [cls.name for _, cls in inspect.getmembers(commands) if inspect.isclass(cls)]
 
 
-def list_labels(args: List[str]) -> List[str]:
+def list_labels(*args: str) -> List[str]:
     """List all available labels in the database.
 
     Args:
         args: a sequence of additional arguments used for the execution. None are supported yet.
 
     Returns:
         The list of all labels.
@@ -41,15 +47,15 @@
     # pylint: disable=import-outside-toplevel
     from cobib.database import Database
 
     labels = list(Database().keys())
     return labels
 
 
-def list_filters(args: List[str]) -> Set[str]:
+def list_filters(*args: str) -> Set[str]:
     """Lists all field names available for filtering.
 
     Args:
         args: a sequence of additional arguments used for the execution. None are supported yet.
 
     Returns:
         The list of all available filters.
@@ -59,15 +65,15 @@
 
     filters: Set[str] = {"label"}
     for entry in Database().values():
         filters.update(entry.data.keys())
     return filters
 
 
-def example_config(args: List[str]) -> List[str]:
+def example_config(*args: str) -> List[str]:
     """Shows the (well-commented) example configuration.
 
     Args:
         args: a sequence of additional arguments used for the execution. None are supported yet.
 
     Returns:
         The lines of the example config file.
@@ -118,15 +124,15 @@
             while not line.strip().startswith(field):
                 line_no, line = next(raw_db)
             return f"{self._database_path}:{line_no+1} {record.getMessage()}"
         except AttributeError:
             return ""
 
 
-def lint_database(args: List[str]) -> List[str]:
+def lint_database(*args: str) -> List[str]:
     """Lints the users database.
 
     Args:
         args: a sequence of additional arguments used for the execution. Currently, only a single
             optional value is allowed:
                 * `-f`, `--format`: if specified, the database will be formatted to automatically
                     resolve all lint messages.
@@ -186,29 +192,38 @@
 
         # generate automatic git commit
         class LintCommand(Command):
             """The linting command."""
 
             name = "lint"
 
-            def execute(self, args, out=None):  # type: ignore
+            def __init__(
+                self,
+                *args: str,
+                console: Console | App[None] | None = None,
+                prompt: Type[PromptBase[str]] | None = None,
+            ) -> None:
+                # pylint: disable=super-init-not-called
+                self.largs = largs
+
+            @classmethod
+            def init_argparser(cls) -> None:
                 pass
 
-            @staticmethod
-            def tui(tui):  # type: ignore
+            def execute(self):  # type: ignore
                 pass
 
-        LintCommand().git(args=vars(largs))
+        LintCommand().git()
 
         return ["The following lint messages have successfully been resolved:"] + lint_messages
 
     return lint_messages
 
 
-def unify_labels(args: List[str]) -> List[str]:
+def unify_labels(*args: str) -> List[str]:
     """Unifies all labels of the database according to `config.database.format.label_default`.
 
     Without the `--apply` argument this will only print the modification which would be performed!
 
     Args:
         args: a sequence of additional arguments used for the execution. Currently, only a single
             optional value is allowed:
@@ -238,10 +253,11 @@
         "--label",
         "some_non_existend_label",  # this ensures that the command gets run on the entire database
     ]
     if largs.apply:
         modify_args = modify_args[1:]
 
     with contextlib.redirect_stderr(StringIO()) as out:
-        ModifyCommand().execute(modify_args)
+        cmd = ModifyCommand(*modify_args)
+        cmd.execute()
 
     return out.getvalue().strip().split("\n")
```

### Comparing `cobib-3.5.5/src/cobib.egg-info/PKG-INFO` & `cobib-4.0.0/src/cobib.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,95 +1,84 @@
 Metadata-Version: 2.1
 Name: cobib
-Version: 3.5.5
+Version: 4.0.0
 Summary: Console Bibliography
-Home-page: https://gitlab.com/mrossinek/cobib
+Home-page: https://gitlab.com/cobib/cobib
 Author: Max Rossmannek
 Author-email: max.rossmannek@uzh.ch
 License: MIT License
-Project-URL: Bug Tracker, https://gitlab.com/mrossinek/cobib/-/issues
-Project-URL: Documentation, https://mrossinek.gitlab.io/cobib/cobib.html
+Project-URL: Bug Tracker, https://gitlab.com/cobib/cobib/-/issues
+Project-URL: Documentation, https://cobib.gitlab.io/cobib/cobib.html
 Keywords: reference-manager, citation-manager, bibliography, cli, tui, command-line,,terminal, console, bibtex, doi, arxiv, isbn
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
-Classifier: Environment :: Console :: Curses
+Classifier: Environment :: Console
 Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-[![coBib](https://gitlab.com/mrossinek/cobib/-/raw/master/logo/cobib_logo.svg)](https://mrossinek.gitlab.io/cobib/cobib.html)
+[![coBib](https://gitlab.com/cobib/cobib/-/raw/master/logo/cobib_logo.svg)](https://cobib.gitlab.io/cobib/cobib.html)
 
 # coBib
 
-[![pipeline](https://gitlab.com/mrossinek/cobib/badges/master/pipeline.svg)](https://gitlab.com/mrossinek/cobib/-/pipelines)
-[![coverage](https://gitlab.com/mrossinek/cobib/badges/master/coverage.svg)](https://gitlab.com/mrossinek/cobib/-/graphs/master/charts)
+[![pipeline](https://gitlab.com/cobib/cobib/badges/master/pipeline.svg)](https://gitlab.com/cobib/cobib/-/pipelines)
+[![coverage](https://gitlab.com/cobib/cobib/badges/master/coverage.svg)](https://gitlab.com/cobib/cobib/-/graphs/master/charts)
 [![PyPI](https://img.shields.io/pypi/v/cobib)](https://pypi.org/project/cobib/)
 
 coBib is a simple, command-line based bibliography management tool.
 It is the result of the need for an easy-to-use alternative to full-blown reference managers like Mendeley or Zotero.
 As such it follows some basic design goals:
 
 * **plain-text database**: which means you get full access and control over the database.
 * **git-integration**: as a benefit of the above, you can keep track of your database through version control.
 * **centralized database, location-independent library**: this means, that coBib *only* manages the
   database file in a centralized fashion but allows you to spread the actual contents of your
   library across the entire file system (this is the major different to
   [papis](https://papis.readthedocs.io/en/latest/library_structure.html)).
-* **command-line and TUI support**: all features are available through the command-line as well as a curses-based TUI.
+* **command-line and TUI support**: all features are available through the command-line as well as a
+  [textual](https://textual.textualize.io/)-based TUI
 
 
-### **News:** coBib v4.0 will come with a new UI!
-The plan is to switch to [rich][rich] and [textual][textual] instead of the current curses TUI.
-This will open up some great possibilities for a much more modern UI.
-
-However, this change will require some *major* refactoring including breaking changes of the API
-and some of the user configuration options. It will also be a rather drastic change in style.
-Thus, I will attempt to support v3.5 with bugfix releases until 1.1.2023
-
-It will likely take a few months until v4.0 gets released but I am starting development on it now.
-You can follow the progress here: <https://gitlab.com/mrossinek/cobib/-/issues/78>
-
-[rich]: https://github.com/Textualize/rich
-[textual]: https://github.com/Textualize/textual
-
 ## Installation
 
 For all common purposes you can install coBib via `pip`:
 
 ```
 pip install cobib
 ```
 
 Note: Use `pip3` if you still have Python 2 installed.
 
 If you would also like to install the man-page and (crude!) Zsh completion,
 you need to download the source code and do the following:
 
 ```
-git clone https://gitlab.com/mrossinek/cobib
+git clone https://gitlab.com/cobib/cobib
 cd cobib
 make install_extras
 ```
 
 ### Arch Linux
 
 coBib is packaged in the AUR.
 * [cobib](https://aur.archlinux.org/packages/cobib/)
 * [cobib-git](https://aur.archlinux.org/packages/cobib-git/)
 
 ### Windows
 
-Windows is **only partially** supported!
-This is due to the fact that [Python under Windows does not ship with the `curses` module][1].
-Thus, you cannot run coBib's _TUI_ on Windows.
-However, if you are using Windows 10 you should be able to install and use coBib's full
-functionality within the Linux subsystem.
+coBib _should_ mostly work on Windows as is, but it is not being tested so no guarantees are given.
+If you are using Windows 10 or later and are running into issues, you should be able to install and
+use coBib's full functionality within the Linux subsystem.
 
 
 ## Getting started
 
 To get started, you must initialize the database:
 
 ```
@@ -141,15 +130,15 @@
 cobib add --isbn <some ISBN>
 ```
 
 **Note**: when adding data from a `.bib` file, make sure that it is in the Bib**La**Tex format!
 
 ### Viewing your database and entries
 
-You can view the contents of your database with (see also `cobib.commands.list`):
+You can view the contents of your database with (see also `cobib.commands.list_`):
 
 ```
 cobib list
 ```
 
 You can show a specific entry with (see also `cobib.commands.show`):
 
@@ -221,26 +210,33 @@
 
 ```
 man cobib
 ```
 
 ### TUI
 
-Finally, you can also use coBib's TUI for a more interactive experience (see also `cobib.tui`), by
-simply typing
-
+Finally, you can also use coBib's TUI for a more interactive experience (see also `cobib.ui.tui`),
+by simply typing
 ```
 cobib
 ```
 
+Here is an example screenshot of the TUI when listing the entires in your database:
+
+![coBib TUI List](https://gitlab.com/cobib/cobib/-/raw/master/html/cobib_tui_list.svg)
+
+And here is an example screenshot for listing search results:
+
+![coBib TUI Search](https://gitlab.com/cobib/cobib/-/raw/master/html/cobib_tui_search.svg)
+
 
 ## Configuration
 
 You can overwrite the default configuration by placing a `config.py` file in `~/.config/cobib/`.
-The easiest way to get started with this file is by copying [`example.py`](https://gitlab.com/mrossinek/cobib/-/blob/master/src/cobib/config/example.py)
+The easiest way to get started with this file is by copying [`example.py`](https://gitlab.com/cobib/cobib/-/blob/master/src/cobib/config/example.py)
 or by using:
 
 ```
 cobib _example_config > ~/.config/cobib/config.py
 ```
 
 You can then modify it to your liking.
@@ -249,23 +245,23 @@
 You can also disable loading of _any_ configuration file be setting this environment variable to one of the following values: `"", 0, "f", "false", "nil", "none"`.
 
 Finally, be sure to take a look at the man page (`man cobib`) and/or the online documentation for more information.
 
 
 ## Documentation
 
-coBib's documentation is hosted [here](https://mrossinek.gitlab.io/cobib/cobib.html).
+coBib's documentation is hosted [here](https://cobib.gitlab.io/cobib/cobib.html).
 
 If you would like to generate a local version during development, you need to clone the source code, and install [`pdoc`](https://github.com/mitmproxy/pdoc) in order to generate it:
 
 ```
-git clone https://gitlab.com/mrossinek/cobib.git
+git clone https://gitlab.com/cobib/cobib.git
 cd cobib
 pip install pdoc
-pdoc -d google -e cobib=https://gitlab.com/mrossinek/cobib/-/blob/master/src/cobib/ -t html -o docs src/cobib tests
+pdoc -d google -e cobib=https://gitlab.com/cobib/cobib/-/blob/master/src/cobib/ -t html -o docs src/cobib tests
 ```
 
 You can then browse the documentation from `docs/cobib.html`.
 
 
 ## History
 
@@ -273,35 +269,93 @@
 which has more features than I use on a regular basis and does not allow me to work from the command line which is where I spent most of the time that I spent on the computer.
 
 Hence, I have decided to make it my own task of implementing a simple, yet fast, reference manager.
 coBib is written in Python and uses a YAML file to store its bibliography in a plain text format.
 
 ### Changelog
 
-You can find the detailed changes throughout coBib's history in [the Changelog](https://gitlab.com/mrossinek/cobib/-/blob/master/CHANGELOG.md).
+You can find the detailed changes throughout coBib's history in [the Changelog](https://gitlab.com/cobib/cobib/-/blob/master/CHANGELOG.md).
 
 
 ## License
 
-coBib is licensed under the [MIT License](https://gitlab.com/mrossinek/cobib/-/blob/master/LICENSE.txt).
+coBib is licensed under the [MIT License](https://gitlab.com/cobib/cobib/-/blob/master/LICENSE.txt).
 
-[^1]: References like this one get interpreted by the documentation generator. If you are reading this as the README page, you may find the [online documentation](https://mrossinek.gitlab.io/cobib/cobib.html) more enjoyable.
-
-[1]: https://docs.python.org/3/howto/curses.html#what-is-curses
+[^1]: References like this one get interpreted by the documentation generator. If you are reading this as the README page, you may find the [online documentation](https://cobib.gitlab.io/cobib/cobib.html) more enjoyable.
 
 [//]: # ( vim: set ft=markdown: )
 
 # Changelog
 All notable changes to this project will be documented in this file.
 
-The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
+The format is based on [Keep a Changelog](https://keepachangelog.com/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+
+## [4.0.0] - 2023-05-20
+
+Pypi: https://pypi.org/project/cobib/3.5.5/
+
+### **Breaking Changes**
+- Configuration settings can no longer be set by item access and instead must
+  use attribute syntax. For example you need to change:
+  ```python
+  config["database"]["git"] = True
+  ```
+  to
+  ```python
+  config.database.git = True
+  ```
+  - the `config.commands.list` section had to be renamed to `config.commands.list_`
+  - the `config.tui` section has been entirely removed
+- The `cobib.commands.list` module was moved to `cobib.commands.list_`.
+- The function signature of all command- and importer-related events has changed!
+  For more details please refer to the
+  [online documentation](https://cobib.gitlab.io/cobib/cobib/config/event.html).
+
+### Added
+- Python 3.11 is now officially tested and supported
+- Full rewrite of all commands to use `rich` for a nicer CLI (#78,!51)
+- Full rewrite of the TUI based on `textual` (#78,!51)
+- the `--disambiguation` argument of the `add` command (#99,!58)
+- the `--ignore-case` argument of the `list` command (#105)
+  - this also comes with the new `config.commands.list_.ignore_case` setting
+- the `search` command now accepts multiple query strings at once which will be
+  searched over independently (#106)
+
+### Changed
+- the new default value of `config.parsers.yaml.use_c_lib_yaml` is now `True` as announced in version [3.4.0]
+- refactored the entire config as a dataclass (!63)
+  - this implies that settings can only be set via attributes
+  - but as a benefit the maintainability and documentation have improved significantly
+- The function signature of all command-related events has changed! Please refer to the
+  [online documentation](https://cobib.gitlab.io/cobib/cobib/config/event.html)
+  for more details. (!63)
+- The function signature of all importer-related events has changed! Please refer to the
+  [online documentation](https://cobib.gitlab.io/cobib/cobib/config/event.html)
+  for more details. (!66)
+- the API of the `cobib.commands` and `cobib.importers` module has been improved (!64)
+  - this should not have any end-user facing effects
+- the `cobib.commands.list` module was moved to `cobib.commands.list_`
+
+### Deprecated
+- the `--update` argument of the `add` command is deprecated in favor of `--disambiguation update`
+- the `--skip-existing` argument of the `add` command is deprecated in favor of `--disambiguation keep`
+
+### Fixed
+- the detection whether an entry already exists broke when label disambiguation was added in [3.3.0]
+  and is now fixed by means of an interactive prompt during the `add` command
+
+### Removed
+- the warning triggered upon setting `config.database.format.month` which got removed in [3.1.0]
+- Python 3.7 is no longer supported
+
+
 ## [3.5.5] - 2023-04-11
 
 Pypi: https://pypi.org/project/cobib/3.5.5/
 
 ### Fixed
 - opening of non-list type fields (#100)
 
@@ -349,15 +403,15 @@
 This will open up some great possibilities for a much more modern UI.
 
 However, this change will require some *major* refactoring including breaking changes of the API
 and some of the user configuration options. It will also be a rather drastic change in style.
 Thus, I will attempt to support v3.5 with bugfix releases until 1.1.2023
 
 It will likely take a few months until v4.0 gets released but I am starting development on it now.
-You can follow the progress here: <https://gitlab.com/mrossinek/cobib/-/issues/78>
+You can follow the progress here: <https://gitlab.com/cobib/cobib/-/issues/78>
 
 [rich]: https://github.com/Textualize/rich
 [textual]: https://github.com/Textualize/textual
 
 ### Added
 - the configuration loading can be disabled via the environment variable `COBIB_CONFIG`
     - values which disable the loading entirely are: `"", 0, f, false, nil, none`
@@ -435,15 +489,15 @@
 * the `config.database.format.label_default` and `config.database.format.label_suffix` options (#85,!45)
     - labels will automatically be formatted according to the default option
     - if labels conflict with existing ones, the suffix option will be used for disambiguation
     - the `AddCommand` has a new `--skip-existing` option which disables automatic label disambiguation
     - use `cobib _unify_labels --apply` to unify all labels in your database
 - subscribable events (#71,!46)
     - allows registering of hooks to be executed in certain situation
-    - more information is provided at the [online documentation](https://mrossinek.gitlab.io/cobib/cobib/config/event.html)
+    - more information is provided at the [online documentation](https://cobib.gitlab.io/cobib/cobib/config/event.html)
 
 ### Changed
 - when an unknown variable is encountered in the modification of the `modify` command it falls back to an empty string rather than the name of the attempted variable
 
 ### Removed
 - the `-s` option of the `AddCommand` is no longer available. You need to write out `--skip-download`
 - the `ID` filter argument on the `list` command (deprecated in v3.2.0 in favor of the `label` filter)
@@ -534,15 +588,15 @@
 ## [3.0.0] - 2021-04-10
 
 Pypi: https://pypi.org/project/cobib/3.0.0/
 
 - From now on, `coBib` is the official way of spelling!
 
 ### Added
-- coBib's documentation is now generated by [`pdoc`](https://pdoc.dev/) and hosted at https://mrossinek.gitlab.io/cobib/cobib.html
+- coBib's documentation is now generated by [`pdoc`](https://pdoc.dev/) and hosted at https://cobib.gitlab.io/cobib/cobib.html
 - (DEV): the `cobib.database.Database`-Singleton has been added to centrally manage the bibliographic runtime data (!28)
 - the new option `config.database.format.suppress_latex_warnings`
 - the new option `config.commands.edit.editor` which takes precedence over the `$EDITOR` variable
 
 ### Changed
 - the `INI`-style configuration is replaced with a `Python`-based configuration (#54,!25)
     - for guidance on how to migrate an existing configuration please read https://mrossinek.gitlab.io/programming/cobibs-new-configuration/
@@ -938,51 +992,52 @@
 
 ## [0.1] - 2019-04-29
 
 ### Added
 - initial version with a basic `sqlite3`-based database
 
 
-[Unreleased]: https://gitlab.com/mrossinek/cobib/-/compare/v3.5.5...master
-[3.5.5]: https://gitlab.com/mrossinek/cobib/-/compare/v3.5.5
-[3.5.4]: https://gitlab.com/mrossinek/cobib/-/compare/v3.5.4
-[3.5.3]: https://gitlab.com/mrossinek/cobib/-/compare/v3.5.3
-[3.5.2]: https://gitlab.com/mrossinek/cobib/-/compare/v3.5.2
-[3.5.1]: https://gitlab.com/mrossinek/cobib/-/compare/v3.5.1
-[3.5.0]: https://gitlab.com/mrossinek/cobib/-/compare/v3.5.0
-[3.4.0]: https://gitlab.com/mrossinek/cobib/-/compare/v3.4.0
-[3.3.2]: https://gitlab.com/mrossinek/cobib/-/compare/v3.3.2
-[3.3.1]: https://gitlab.com/mrossinek/cobib/-/compare/v3.3.1
-[3.3.0]: https://gitlab.com/mrossinek/cobib/-/compare/v3.3.0
-[3.2.1]: https://gitlab.com/mrossinek/cobib/-/compare/v3.2.1
-[3.2.0]: https://gitlab.com/mrossinek/cobib/-/compare/v3.2.0
-[3.1.1]: https://gitlab.com/mrossinek/cobib/-/compare/v3.1.1
-[3.1.0]: https://gitlab.com/mrossinek/cobib/-/compare/v3.1.0
-[3.0.0]: https://gitlab.com/mrossinek/cobib/-/compare/v3.0.0
-[2.6.1]: https://gitlab.com/mrossinek/cobib/-/compare/v2.6.1
-[2.6.0]: https://gitlab.com/mrossinek/cobib/-/tags/v2.6.0
-[2.5.0]: https://gitlab.com/mrossinek/cobib/-/tags/v2.5.0
-[2.4.1]: https://gitlab.com/mrossinek/cobib/-/tags/v2.4.1
-[2.4.0]: https://gitlab.com/mrossinek/cobib/-/tags/v2.4.0
-[2.3.4]: https://gitlab.com/mrossinek/cobib/-/tags/v2.3.4
-[2.3.3]: https://gitlab.com/mrossinek/cobib/-/tags/v2.3.3
-[2.3.2]: https://gitlab.com/mrossinek/cobib/-/tags/v2.3.2
-[2.3.1]: https://gitlab.com/mrossinek/cobib/-/tags/v2.3.1
-[2.3.0]: https://gitlab.com/mrossinek/cobib/-/tags/v2.3.0
-[2.2.2]: https://gitlab.com/mrossinek/cobib/-/tags/v2.2.2
-[2.2.1]: https://gitlab.com/mrossinek/cobib/-/tags/v2.2.1
-[2.2.0]: https://gitlab.com/mrossinek/cobib/-/tags/v2.2.0
-[2.1.0]: https://gitlab.com/mrossinek/cobib/-/tags/v2.1.0
-[2.0.0]: https://gitlab.com/mrossinek/cobib/-/tags/v2.0.0
-[2.0.0b4]: https://gitlab.com/mrossinek/cobib/-/tags/v2.0.0b4
-[2.0.0b3]: https://gitlab.com/mrossinek/cobib/-/tags/v2.0.0b3
-[2.0.0b2]: https://gitlab.com/mrossinek/cobib/-/tags/v2.0.0b2
-[2.0.0b1]: https://gitlab.com/mrossinek/cobib/-/tags/v2.0.0b1
-[2.0.0b0]: https://gitlab.com/mrossinek/cobib/-/tags/v2.0.0b0
-[2.0.0a2]: https://gitlab.com/mrossinek/cobib/-/tags/v2.0.0a2
-[2.0.0a1]: https://gitlab.com/mrossinek/cobib/-/tags/v2.0.0a1
-[1.1.0]: https://gitlab.com/mrossinek/cobib/-/tags/v1.1.0
-[1.0.2]: https://gitlab.com/mrossinek/cobib/-/tags/v1.0.2
-[1.0.1]: https://gitlab.com/mrossinek/cobib/-/tags/v1.0.1
-[1.0.0]: https://gitlab.com/mrossinek/cobib/-/tags/v1.0.0
-[0.2]: https://gitlab.com/mrossinek/cobib/-/tags/v0.2
-[0.1]: https://gitlab.com/mrossinek/cobib/-/tags/v0.1
+[Unreleased]: https://gitlab.com/cobib/cobib/-/compare/v4.0.0...master
+[4.0.0]: https://gitlab.com/cobib/cobib/-/compare/v4.0.0
+[3.5.5]: https://gitlab.com/cobib/cobib/-/compare/v3.5.5
+[3.5.4]: https://gitlab.com/cobib/cobib/-/compare/v3.5.4
+[3.5.3]: https://gitlab.com/cobib/cobib/-/compare/v3.5.3
+[3.5.2]: https://gitlab.com/cobib/cobib/-/compare/v3.5.2
+[3.5.1]: https://gitlab.com/cobib/cobib/-/compare/v3.5.1
+[3.5.0]: https://gitlab.com/cobib/cobib/-/compare/v3.5.0
+[3.4.0]: https://gitlab.com/cobib/cobib/-/compare/v3.4.0
+[3.3.2]: https://gitlab.com/cobib/cobib/-/compare/v3.3.2
+[3.3.1]: https://gitlab.com/cobib/cobib/-/compare/v3.3.1
+[3.3.0]: https://gitlab.com/cobib/cobib/-/compare/v3.3.0
+[3.2.1]: https://gitlab.com/cobib/cobib/-/compare/v3.2.1
+[3.2.0]: https://gitlab.com/cobib/cobib/-/compare/v3.2.0
+[3.1.1]: https://gitlab.com/cobib/cobib/-/compare/v3.1.1
+[3.1.0]: https://gitlab.com/cobib/cobib/-/compare/v3.1.0
+[3.0.0]: https://gitlab.com/cobib/cobib/-/compare/v3.0.0
+[2.6.1]: https://gitlab.com/cobib/cobib/-/compare/v2.6.1
+[2.6.0]: https://gitlab.com/cobib/cobib/-/tags/v2.6.0
+[2.5.0]: https://gitlab.com/cobib/cobib/-/tags/v2.5.0
+[2.4.1]: https://gitlab.com/cobib/cobib/-/tags/v2.4.1
+[2.4.0]: https://gitlab.com/cobib/cobib/-/tags/v2.4.0
+[2.3.4]: https://gitlab.com/cobib/cobib/-/tags/v2.3.4
+[2.3.3]: https://gitlab.com/cobib/cobib/-/tags/v2.3.3
+[2.3.2]: https://gitlab.com/cobib/cobib/-/tags/v2.3.2
+[2.3.1]: https://gitlab.com/cobib/cobib/-/tags/v2.3.1
+[2.3.0]: https://gitlab.com/cobib/cobib/-/tags/v2.3.0
+[2.2.2]: https://gitlab.com/cobib/cobib/-/tags/v2.2.2
+[2.2.1]: https://gitlab.com/cobib/cobib/-/tags/v2.2.1
+[2.2.0]: https://gitlab.com/cobib/cobib/-/tags/v2.2.0
+[2.1.0]: https://gitlab.com/cobib/cobib/-/tags/v2.1.0
+[2.0.0]: https://gitlab.com/cobib/cobib/-/tags/v2.0.0
+[2.0.0b4]: https://gitlab.com/cobib/cobib/-/tags/v2.0.0b4
+[2.0.0b3]: https://gitlab.com/cobib/cobib/-/tags/v2.0.0b3
+[2.0.0b2]: https://gitlab.com/cobib/cobib/-/tags/v2.0.0b2
+[2.0.0b1]: https://gitlab.com/cobib/cobib/-/tags/v2.0.0b1
+[2.0.0b0]: https://gitlab.com/cobib/cobib/-/tags/v2.0.0b0
+[2.0.0a2]: https://gitlab.com/cobib/cobib/-/tags/v2.0.0a2
+[2.0.0a1]: https://gitlab.com/cobib/cobib/-/tags/v2.0.0a1
+[1.1.0]: https://gitlab.com/cobib/cobib/-/tags/v1.1.0
+[1.0.2]: https://gitlab.com/cobib/cobib/-/tags/v1.0.2
+[1.0.1]: https://gitlab.com/cobib/cobib/-/tags/v1.0.1
+[1.0.0]: https://gitlab.com/cobib/cobib/-/tags/v1.0.0
+[0.2]: https://gitlab.com/cobib/cobib/-/tags/v0.2
+[0.1]: https://gitlab.com/cobib/cobib/-/tags/v0.1
```

### Comparing `cobib-3.5.5/src/cobib.egg-info/SOURCES.txt` & `cobib-4.0.0/src/cobib.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 src/cobib/commands/add.py
 src/cobib/commands/base_command.py
 src/cobib/commands/delete.py
 src/cobib/commands/edit.py
 src/cobib/commands/export.py
 src/cobib/commands/import_.py
 src/cobib/commands/init.py
-src/cobib/commands/list.py
+src/cobib/commands/list_.py
 src/cobib/commands/modify.py
 src/cobib/commands/open.py
 src/cobib/commands/redo.py
 src/cobib/commands/search.py
 src/cobib/commands/show.py
 src/cobib/commands/undo.py
 src/cobib/config/__init__.py
@@ -68,20 +68,33 @@
 src/cobib/parsers/arxiv.py
 src/cobib/parsers/base_parser.py
 src/cobib/parsers/bibtex.py
 src/cobib/parsers/doi.py
 src/cobib/parsers/isbn.py
 src/cobib/parsers/url.py
 src/cobib/parsers/yaml.py
-src/cobib/tui/__init__.py
-src/cobib/tui/buffer.py
-src/cobib/tui/frame.py
-src/cobib/tui/state.py
-src/cobib/tui/tui.py
+src/cobib/ui/__init__.py
+src/cobib/ui/cli.py
+src/cobib/ui/shell_helper.py
+src/cobib/ui/tui.py
+src/cobib/ui/ui.py
+src/cobib/ui/components/__init__.py
+src/cobib/ui/components/argument_parser.py
+src/cobib/ui/components/entry_view.py
+src/cobib/ui/components/help_popup.py
+src/cobib/ui/components/input.py
+src/cobib/ui/components/main_view.py
+src/cobib/ui/components/popup.py
+src/cobib/ui/components/popup_logging_handler.py
+src/cobib/ui/components/popup_panel.py
+src/cobib/ui/components/progress.py
+src/cobib/ui/components/prompt.py
+src/cobib/ui/components/selection_filter.py
 src/cobib/utils/__init__.py
+src/cobib/utils/diff_renderer.py
 src/cobib/utils/file_downloader.py
 src/cobib/utils/journal_abbreviations.py
 src/cobib/utils/logging.py
 src/cobib/utils/rel_path.py
 src/cobib/utils/shell_helper.py
 tests/__init__.py
 tests/cmdline_test.py
@@ -127,25 +140,15 @@
 tests/parsers/parser_test.py
 tests/parsers/test_arxiv.py
 tests/parsers/test_bibtex.py
 tests/parsers/test_doi.py
 tests/parsers/test_isbn.py
 tests/parsers/test_url.py
 tests/parsers/test_yaml.py
-tests/tui/__init__.py
-tests/tui/mock_curses.py
-tests/tui/mock_tui.py
-tests/tui/scrolling_database.yaml
-tests/tui/test_buffer.py
-tests/tui/test_frame.py
-tests/tui/test_state.py
-tests/tui/test_tui.py
-tests/tui/tui_test.py
 tests/utils/__init__.py
-tests/utils/expected_changelog_printing.txt
 tests/utils/fixed_database.yaml
 tests/utils/linting_database.yaml
 tests/utils/test_file_downloader.py
 tests/utils/test_journal_abbreviations.py
 tests/utils/test_logging.py
 tests/utils/test_rel_path.py
 tests/utils/test_shell_helper.py
```

### Comparing `cobib-3.5.5/tests/__init__.py` & `cobib-4.0.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.5/tests/cmdline_test.py` & `cobib-4.0.0/tests/cmdline_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 """coBib's command-line test class."""
 
 from __future__ import annotations
 
+import os
 import runpy
 from typing import TYPE_CHECKING, List
 
 if TYPE_CHECKING:
     import pytest
 
 
 class CmdLineTest:
     """A command-line test runs coBib's command-line interface."""
 
     @staticmethod
-    def run_module(monkeypatch: pytest.MonkeyPatch, main: str, sys_argv: List[str]) -> None:
+    async def run_module(monkeypatch: pytest.MonkeyPatch, main: str, sys_argv: List[str]) -> None:
         """Gets the coBib runtime module after monkeypatching `sys.argv`.
 
         Args:
             monkeypatch: the built-in pytest fixture.
             main: the name of the `main` executable of the module to run.
             sys_argv: the list of values with which to monkeypatch `sys.argv`.
         """
+        os.environ["COBIB_CONFIG"] = "0"
         monkeypatch.setattr("sys.argv", sys_argv)
         module = runpy.run_module("cobib")
-        module.get(main)()  # type: ignore
+        await module.get(main)()  # type: ignore
```

### Comparing `cobib-3.5.5/tests/commands/command_test.py` & `cobib-4.0.0/tests/commands/command_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,18 +42,14 @@
     def get_command(self) -> Type[cobib.commands.base_command.Command]:
         """Get the command tested by this class.
 
         Returns:
             The command to be tested by this class.
         """
 
-    def get_safe_command_name(self) -> str:
-        """Returns the safe command name."""
-        return self.get_command().name
-
     @abstractmethod
     def test_command(self) -> None:
         """Test the command itself."""
 
     @pytest.fixture
     def setup(self, request: _pytest.fixtures.SubRequest) -> Generator[Dict[str, Any], None, None]:
         """Setup testing environment.
@@ -156,18 +152,20 @@
     def test_handle_argument_error(self, caplog: pytest.LogCaptureFixture) -> None:
         """Test handling of ArgumentError.
 
         Args:
             caplog: the built-in pytest fixture.
         """
         command_cls = self.get_command()
-        command_cls().execute(["--dummy"])
+        try:
+            command_cls("--dummy").execute()
+        except SystemExit:
+            pass
         name = command_cls.name
-        safe_name = self.get_safe_command_name()
         for source, level, message in caplog.record_tuples:
-            if (f"cobib.commands.{safe_name}", logging.ERROR) == (
+            if ("cobib.commands.base_command", logging.ERROR) == (
                 source,
                 level,
             ) and f"Error: {name}: error:" in message:
                 break
         else:
             pytest.fail("No Error logged from ArgumentParser.")
```

### Comparing `cobib-3.5.5/tests/commands/test_add.py` & `cobib-4.0.0/tests/commands/test_add.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,46 +2,68 @@
 # pylint: disable=unused-argument
 
 from __future__ import annotations
 
 import logging
 import os
 import tempfile
-from argparse import Namespace
 from itertools import zip_longest
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Type
+from typing import TYPE_CHECKING, Any, Dict, Generator, List, Optional, Type
 
 import pytest
+from typing_extensions import override
 
 from cobib.commands import AddCommand
 from cobib.config import Event, config
-from cobib.database import Database, Entry
+from cobib.database import Database
 from cobib.utils.rel_path import RelPath
 
-from .. import get_resource
-from ..tui.tui_test import TUITest
+from .. import MockStdin, get_resource
 from .command_test import CommandTest
 
 EXAMPLE_LITERATURE = get_resource("example_literature.yaml")
 EXAMPLE_DUPLICATE_ENTRY_BIB = get_resource("example_duplicate_entry.bib", "commands")
 EXAMPLE_DUPLICATE_ENTRY_YAML = get_resource("example_duplicate_entry.yaml", "commands")
 EXAMPLE_MULTI_FILE_ENTRY_BIB = get_resource("example_multi_file_entry.bib", "commands")
 EXAMPLE_MULTI_FILE_ENTRY_YAML = get_resource("example_multi_file_entry.yaml", "commands")
 
 if TYPE_CHECKING:
+    import _pytest.fixtures
+
     import cobib.commands
 
 
-class TestAddCommand(CommandTest, TUITest):
+class TestAddCommand(CommandTest):
     """Tests for coBib's AddCommand."""
 
+    @override
     def get_command(self) -> Type[cobib.commands.base_command.Command]:
-        # noqa: D102
         return AddCommand
 
+    @pytest.fixture
+    def post_setup(
+        self, monkeypatch: pytest.MonkeyPatch, request: _pytest.fixtures.SubRequest
+    ) -> Generator[Dict[str, Any], None, None]:
+        """Additional setup instructions.
+
+        Args:
+            monkeypatch: the built-in pytest fixture.
+            request: a pytest sub-request providing access to nested parameters.
+
+        Yields:
+            The internally used parameters for potential later re-use during the actual test.
+        """
+        if not hasattr(request, "param"):
+            # use default settings
+            request.param = {"stdin_list": None}
+
+        monkeypatch.setattr("sys.stdin", MockStdin(request.param.get("stdin_list", None)))
+
+        yield request.param
+
     def _assert(self, extra_filename: str) -> None:
         """Common assertion utility method.
 
         Args:
             extra_filename: path to an additional filename whose contents are to be added to the
                 expected lines.
         """
@@ -63,14 +85,15 @@
             kwargs: additional keyword arguments whose contents are checked against the Entry's
                 `data contents.
         """
         entry = Database()[label]
         for key, value in kwargs.items():
             assert entry.data.get(key, None) == value
 
+    @pytest.mark.asyncio
     @pytest.mark.parametrize(
         ["setup"],
         [
             [{"git": False}],
             [{"git": True}],
         ],
         indirect=["setup"],
@@ -84,15 +107,18 @@
                 {"file": [str(RelPath("test/debug.py"))]},
             ],
             [["-l", "dummy_label"], {}],
             [["tag"], {"tags": ["tag"]}],
             [["tag", "tag2"], {"tags": ["tag", "tag2"]}],
         ],
     )
-    def test_command(self, setup: Any, more_args: List[str], entry_kwargs: Dict[str, Any]) -> None:
+    async def test_command(
+        self, setup: Any, more_args: List[str], entry_kwargs: Dict[str, Any]
+    ) -> None:
+        # pylint: disable=invalid-overridden-method
         """Test the command itself.
 
         Args:
             setup: the `tests.commands.command_test.CommandTest.setup` fixture.
             more_args: additional arguments to be passed to the command.
             entry_kwargs: the expected contents of the resulting `Entry`.
         """
@@ -100,53 +126,55 @@
 
         try:
             label = more_args[more_args.index("-l") + 1]
         except ValueError:
             label = "example_multi_file_entry"
         args = ["-b", EXAMPLE_MULTI_FILE_ENTRY_BIB] + more_args
 
-        AddCommand().execute(args)
+        await AddCommand(*args).execute()
 
         assert Database()[label]
 
         if entry_kwargs or label != "example_multi_file_entry":
             self._assert_entry(label, **entry_kwargs)
         else:
             # only when we don't use extra arguments the files will match
             self._assert(EXAMPLE_MULTI_FILE_ENTRY_YAML)
 
         if git:
             # assert the git commit message
             # Note: we do not assert the arguments, because they depend on the available parsers
             self.assert_git_commit_message("add", None)
 
-    def test_add_new_entry(self, setup: Any, caplog: pytest.LogCaptureFixture) -> None:
+    @pytest.mark.asyncio
+    async def test_add_new_entry(self, setup: Any, caplog: pytest.LogCaptureFixture) -> None:
         """Test adding a new plain entry.
 
         Args:
             setup: the `tests.commands.command_test.CommandTest.setup` fixture.
             caplog: the built-in pytest fixture.
         """
-        AddCommand().execute(["-l", "dummy"])
+        await AddCommand("-l", "dummy").execute()
         assert (
             "cobib.commands.add",
             30,
             "No input to parse. Creating new entry 'dummy' manually.",
         ) in caplog.record_tuples
 
         with open(config.database.file, "r", encoding="utf-8") as file:
             lines = file.readlines()
             dummy_start = lines.index("dummy:\n")
             assert dummy_start > 0
             assert lines[dummy_start - 1] == "---\n"
             assert lines[dummy_start + 1] == "  ENTRYTYPE: article\n"
             assert lines[dummy_start + 2] == "...\n"
 
+    @pytest.mark.asyncio
     @pytest.mark.parametrize("folder", [None, "."])
-    def test_add_with_download(
+    async def test_add_with_download(
         self,
         folder: Optional[str],
         setup: Any,
         capsys: pytest.CaptureFixture[str],
         caplog: pytest.LogCaptureFixture,
     ) -> None:
         """Test adding a new entry with an associated file automatically downloaded.
@@ -164,15 +192,15 @@
         except FileNotFoundError:
             pass
         try:
             args = ["-a", "1812.09976"]
             if folder:
                 args += ["-p", folder]
 
-            AddCommand().execute(args)
+            await AddCommand(*args).execute()
 
             if (
                 "cobib.parsers.arxiv",
                 logging.ERROR,
                 "An Exception occurred while trying to query the arXiv ID: 1812.09976.",
             ) in caplog.record_tuples:
                 pytest.skip("The requests API encountered an error. Skipping test.")
@@ -186,26 +214,27 @@
             assert os.path.exists(path.path)
         finally:
             try:
                 os.remove(path.path)
             except FileNotFoundError:
                 pass
 
-    def test_add_skip_download(self, setup: Any, caplog: pytest.LogCaptureFixture) -> None:
+    @pytest.mark.asyncio
+    async def test_add_skip_download(self, setup: Any, caplog: pytest.LogCaptureFixture) -> None:
         """Test adding a new entry and skipping the automatic download.
 
         Args:
             setup: the `tests.commands.command_test.CommandTest.setup` fixture.
             caplog: the built-in pytest fixture.
         """
         path = RelPath("/tmp/Cao2018.pdf")
         try:
             args = ["-a", "1812.09976", "--skip-download"]
 
-            AddCommand().execute(args)
+            await AddCommand(*args).execute()
 
             if (
                 "cobib.parsers.arxiv",
                 logging.ERROR,
                 "An Exception occurred while trying to query the arXiv ID: 1812.09976.",
             ) in caplog.record_tuples:
                 pytest.skip("The requests API encountered an error. Skipping test.")
@@ -218,31 +247,36 @@
             assert not os.path.exists(path.path)
         finally:
             try:
                 os.remove(path.path)
             except FileNotFoundError:
                 pass
 
+    @pytest.mark.asyncio
+    @pytest.mark.parametrize("deprecated", (True, False))
     @pytest.mark.parametrize(
         ["setup"],
         [
             [{"git": False}],
             [{"git": True}],
         ],
         indirect=["setup"],
     )
-    def test_add_with_update(self, setup: Any, caplog: pytest.LogCaptureFixture) -> None:
+    async def test_add_with_update(
+        self, setup: Any, deprecated: bool, caplog: pytest.LogCaptureFixture
+    ) -> None:
         """Test update option of AddCommand.
 
         Args:
             setup: the `tests.commands.command_test.CommandTest.setup` fixture.
+            deprecated: whether to test the deprecated or new means.
             caplog: the built-in pytest fixture.
         """
         git = setup.get("git", False)
-        AddCommand().execute(["-a", "1812.09976", "--skip-download"])
+        await AddCommand("-a", "1812.09976", "--skip-download").execute()
 
         if (
             "cobib.parsers.arxiv",
             logging.ERROR,
             "An Exception occurred while trying to query the arXiv ID: 1812.09976.",
         ) in caplog.record_tuples:
             pytest.skip("The requests API encountered an error. Skipping test.")
@@ -261,24 +295,42 @@
 
         assert "journal" not in entry.data.keys()
         assert "month" not in entry.data.keys()
         assert "number" not in entry.data.keys()
         assert "pages" not in entry.data.keys()
         assert "volume" not in entry.data.keys()
 
-        args = ["-d", "10.1021/acs.chemrev.8b00803", "-l", "Cao2018", "--skip-download", "--update"]
-        AddCommand().execute(args)
+        args = [
+            "-d",
+            "10.1021/acs.chemrev.8b00803",
+            "-l",
+            "Cao2018",
+            "--skip-download",
+        ]
+        if deprecated:
+            args += ["--update"]
+        else:
+            args += ["--disambiguation", "update"]
+        await AddCommand(*args).execute()
 
         if (
             "cobib.parsers.doi",
             logging.ERROR,
             "An Exception occurred while trying to query the DOI: 10.1021/acs.chemrev.8b00803.",
         ) in caplog.record_tuples:
             pytest.skip("The requests API encountered an error. Skipping test.")
 
+        if deprecated:
+            assert (
+                "cobib.commands.add",
+                logging.WARNING,
+                "The '--update' argument of the 'add' command is deprecated! "
+                "Instead you should use '--disambiguation update'.",
+            ) in caplog.record_tuples
+
         # assert final state
         entry = Database()["Cao2018"]
 
         assert entry.data["author"].startswith("Yudong Cao")
         assert entry.data["title"].startswith("Quantum Chemistry in the Age of Quantum Computing")
         assert entry.data["arxivid"].startswith("1812.09976")
         assert entry.data["primaryClass"] == "quant-ph"
@@ -294,152 +346,180 @@
         assert entry.data["year"] == 2019
 
         if git:
             # assert the git commit message
             # Note: we do not assert the arguments, because they depend on the available parsers
             self.assert_git_commit_message("add", None)
 
-    def test_skip_manual_add_if_exists(self, setup: Any, caplog: pytest.LogCaptureFixture) -> None:
+    @pytest.mark.asyncio
+    async def test_skip_manual_add_if_exists(
+        self, setup: Any, caplog: pytest.LogCaptureFixture
+    ) -> None:
         """Test manual addition is skipped if the label exists already.
 
         Args:
             setup: the `tests.commands.command_test.CommandTest.setup` fixture.
             caplog: the built-in pytest fixture.
         """
-        AddCommand().execute(["-l", "einstein"])
+        await AddCommand("-l", "einstein").execute()
         assert (
             "cobib.commands.add",
             30,
-            "You tried to add a new entry 'einstein' which already exists!",
-        ) in caplog.record_tuples
-        assert (
-            "cobib.commands.add",
-            30,
-            "Please use `cobib edit einstein` instead!",
+            (
+                "You tried to add the 'einstein' entry manually, but it already exists, "
+                "please use `cobib edit einstein` instead!"
+            ),
         ) in caplog.record_tuples
 
-    def test_continue_after_skip_exists(self, setup: Any, caplog: pytest.LogCaptureFixture) -> None:
+    @pytest.mark.asyncio
+    @pytest.mark.parametrize("deprecated", (True, False))
+    async def test_continue_after_skip_exists(
+        self, setup: Any, deprecated: bool, caplog: pytest.LogCaptureFixture
+    ) -> None:
         """Test entry addition continues after skipping over existing entry.
 
         Regression test against #83
 
         Args:
             setup: the `tests.commands.command_test.CommandTest.setup` fixture.
+            deprecated: whether to test the deprecated or new means.
             caplog: the built-in pytest fixture.
         """
         with tempfile.NamedTemporaryFile("w") as file:
             with open(EXAMPLE_DUPLICATE_ENTRY_BIB, "r", encoding="utf-8") as existing:
                 file.writelines(existing.readlines())
             file.writelines(["@article{dummy,\nauthor = {Dummy},\n}"])
             file.flush()
-            AddCommand().execute(["--skip-existing", "-b", file.name])
+            args = ["-b", file.name]
+            if deprecated:
+                args += ["--skip-existing"]
+            else:
+                args += ["--disambiguation", "keep"]
+            await AddCommand(*args).execute()
         assert (
             "cobib.commands.add",
-            30,
-            "You tried to add a new entry 'einstein' which already exists!",
-        ) in caplog.record_tuples
-        assert (
-            "cobib.commands.add",
-            30,
-            "Please use `cobib edit einstein` instead!",
+            20,
+            "Skipping addition of the already existing entry 'einstein'.",
         ) in caplog.record_tuples
         assert (
             "cobib.database.database",
             10,
             "Updating entry dummy",
         ) in caplog.record_tuples
 
-    def test_warning_missing_label(self, setup: Any, caplog: pytest.LogCaptureFixture) -> None:
+        if deprecated:
+            assert (
+                "cobib.commands.add",
+                logging.WARNING,
+                "The '--skip-existing' argument of the 'add' command is deprecated! "
+                "Instead you should use '--disambiguation keep'.",
+            ) in caplog.record_tuples
+
+    @pytest.mark.asyncio
+    async def test_warning_missing_label(
+        self, setup: Any, caplog: pytest.LogCaptureFixture
+    ) -> None:
         """Test warning for missing label and any other input.
 
         Args:
             setup: the `tests.commands.command_test.CommandTest.setup` fixture.
             caplog: the built-in pytest fixture.
         """
-        AddCommand().execute([""])
+        await AddCommand().execute()
         assert (
             "cobib.commands.add",
             40,
             "Neither an input to parse nor a label for manual creation specified!",
         ) in caplog.record_tuples
 
+    @pytest.mark.asyncio
     @pytest.mark.parametrize(
         ["setup"],
         [
             [{"git": False}],
             [{"git": True}],
         ],
         indirect=["setup"],
     )
-    def test_overwrite_label(self, setup: Any) -> None:
+    async def test_overwrite_label(self, setup: Any) -> None:
         """Test add command while specifying a label manually.
 
         Regression test against #4.
 
         The duplicate entry has been adapted to also assert the elongation of Journal names.
 
         Args:
             setup: the `tests.commands.command_test.CommandTest.setup` fixture.
         """
         config.utils.journal_abbreviations = [("Annalen der Physik", "Ann. Phys.")]
         git = setup.get("git", False)
         # add potentially duplicate entry
-        AddCommand().execute(["-b", EXAMPLE_DUPLICATE_ENTRY_BIB, "--label", "duplicate_resolver"])
+        await AddCommand(
+            "-b", EXAMPLE_DUPLICATE_ENTRY_BIB, "--label", "duplicate_resolver"
+        ).execute()
 
         assert Database()["duplicate_resolver"]
 
         self._assert(EXAMPLE_DUPLICATE_ENTRY_YAML)
 
         if git:
             # assert the git commit message
             self.assert_git_commit_message("add", None)
 
+    @pytest.mark.asyncio
     @pytest.mark.parametrize(
         ["setup"],
         [
             [{"git": False}],
             [{"git": True}],
         ],
         indirect=["setup"],
     )
-    def test_configured_label_default(self, setup: Any) -> None:
+    async def test_configured_label_default(self, setup: Any) -> None:
         """Test add command when a `label_default` is pre-configured.
 
         Args:
             setup: the `tests.commands.command_test.CommandTest.setup` fixture.
         """
         config.database.format.label_default = "{author.split()[1]}{year}"
         git = setup.get("git", False)
 
-        AddCommand().execute(["-b", EXAMPLE_DUPLICATE_ENTRY_BIB])
+        await AddCommand("-b", EXAMPLE_DUPLICATE_ENTRY_BIB).execute()
 
         assert Database()["Einstein1905"]
 
         if git:
             # assert the git commit message
             self.assert_git_commit_message("add", None)
 
+    @pytest.mark.asyncio
     @pytest.mark.parametrize(
-        ["setup"],
+        ["setup", "post_setup", "args"],
         [
-            [{"git": False}],
-            [{"git": True}],
+            [{"git": False}, {"stdin_list": ["disambiguate"]}, []],
+            [{"git": True}, {"stdin_list": ["disambiguate"]}, []],
+            [{"git": False}, {}, ["--disambiguation", "disambiguate"]],
+            [{"git": True}, {}, ["--disambiguation", "disambiguate"]],
         ],
-        indirect=["setup"],
+        indirect=["setup", "post_setup"],
     )
-    def test_disambiguate_label(self, setup: Any, caplog: pytest.LogCaptureFixture) -> None:
+    async def test_disambiguate_label(
+        self, setup: Any, post_setup: Any, args: list[str], caplog: pytest.LogCaptureFixture
+    ) -> None:
         """Test label disambiguation if the provided one already exists.
 
         Args:
             setup: the `tests.commands.command_test.CommandTest.setup` fixture.
+            post_setup: an additional setup fixture.
+            args: additional arguments for the AddCommand.
             caplog: the built-in pytest fixture.
         """
         git = setup.get("git", False)
 
-        AddCommand().execute(["-b", EXAMPLE_DUPLICATE_ENTRY_BIB])
+        await AddCommand("-b", EXAMPLE_DUPLICATE_ENTRY_BIB, *args).execute()
 
         assert (
             "cobib.commands.add",
             30,
             "You tried to add a new entry 'einstein' which already exists!",
         ) in caplog.record_tuples
         assert (
@@ -451,26 +531,36 @@
 
         assert Database()["einstein_a"]
 
         if git:
             # assert the git commit message
             self.assert_git_commit_message("add", None)
 
-    def test_disambiguate_download(
+    @pytest.mark.asyncio
+    @pytest.mark.parametrize(
+        ["post_setup"],
+        [
+            [{"stdin_list": ["disambiguate"]}],
+        ],
+        indirect=["post_setup"],
+    )
+    async def test_disambiguate_download(
         self,
         setup: Any,
+        post_setup: Any,
         capsys: pytest.CaptureFixture[str],
         caplog: pytest.LogCaptureFixture,
     ) -> None:
         """Test label disambiguation is propagated to downloaded files.
 
-        This is a regression test against https://gitlab.com/mrossinek/cobib/-/issues/96.
+        This is a regression test against https://gitlab.com/cobib/cobib/-/issues/96.
 
         Args:
             setup: the `tests.commands.command_test.CommandTest.setup` fixture.
+            post_setup: an additional setup fixture.
             capsys: the built-in pytest fixture.
             caplog: the built-in pytest fixture.
         """
         database = Database()
 
         for label in ("Cao2018", "Cao2018_a"):
             try:
@@ -478,15 +568,15 @@
                 try:
                     # ensure file does not exist yet
                     os.remove(path.path)
                 except FileNotFoundError:
                     pass
 
                 # by repeatedly calling the same add command, we trigger the label disambiguation
-                AddCommand().execute(["-a", "1812.09976"])
+                await AddCommand("-a", "1812.09976").execute()
 
                 if (
                     "cobib.parsers.arxiv",
                     logging.ERROR,
                     "An Exception occurred while trying to query the arXiv ID: 1812.09976.",
                 ) in caplog.record_tuples:
                     pytest.skip("The requests API encountered an error. Skipping test.")
@@ -506,78 +596,103 @@
 
             finally:
                 try:
                     os.remove(path.path)
                 except FileNotFoundError:
                     pass
 
+    @pytest.mark.asyncio
     @pytest.mark.parametrize(
         ["setup"],
         [
             [{"git": False}],
         ],
         indirect=["setup"],
     )
     # other variants are already covered by test_command
-    def test_cmdline(self, setup: Any, monkeypatch: pytest.MonkeyPatch) -> None:
+    async def test_cmdline(self, setup: Any, monkeypatch: pytest.MonkeyPatch) -> None:
         """Test the command-line access of the command.
 
         Args:
             setup: the `tests.commands.command_test.CommandTest.setup` fixture.
             monkeypatch: the built-in pytest fixture.
         """
-        self.run_module(monkeypatch, "main", ["cobib", "add", "-b", EXAMPLE_MULTI_FILE_ENTRY_BIB])
+        await self.run_module(
+            monkeypatch, "main", ["cobib", "add", "-b", EXAMPLE_MULTI_FILE_ENTRY_BIB]
+        )
         self._assert(EXAMPLE_MULTI_FILE_ENTRY_YAML)
 
-    def test_tui(self, setup: Any) -> None:
-        """Test the TUI access of the command.
-
-        Args:
-            setup: the `tests.commands.command_test.CommandTest.setup` fixture.
-        """
-
-        def assertion(screen, logs, **kwargs):  # type: ignore
-            self._assert(EXAMPLE_MULTI_FILE_ENTRY_YAML)
-
-            assert "example_multi_file_entry" in screen.display[1]
-
-            expected_log = [
-                ("cobib.commands.add", 10, "Add command triggered from TUI."),
-                ("cobib.commands.add", 10, "Starting Add command."),
-                (
-                    "cobib.commands.add",
-                    10,
-                    "Adding entries from bibtex: '" + EXAMPLE_MULTI_FILE_ENTRY_BIB + "'.",
-                ),
-                ("cobib.commands.add", 20, "'example_multi_file_entry' was added to the database."),
-                ("cobib.commands.add", 10, "Updating list after Add command."),
-            ]
-            assert [log for log in logs if log[0] == "cobib.commands.add"] == expected_log
-
-        keys = "a-b " + EXAMPLE_MULTI_FILE_ENTRY_BIB + "\n"
-        self.run_tui(keys, assertion, {})
-
-    def test_event_pre_add_command(self, setup: Any) -> None:
+    @pytest.mark.asyncio
+    async def test_event_pre_add_command(self, setup: Any) -> None:
         """Tests the PreAddCommand event."""
 
         @Event.PreAddCommand.subscribe
-        def hook(largs: Namespace) -> None:
-            largs.label = "dummy"
+        def hook(command: AddCommand) -> None:
+            command.largs.label = "dummy"
 
         assert Event.PreAddCommand.validate()
 
-        AddCommand().execute(["-b", EXAMPLE_DUPLICATE_ENTRY_BIB])
+        await AddCommand("-b", EXAMPLE_DUPLICATE_ENTRY_BIB).execute()
 
         assert "dummy" in Database().keys()
 
-    def test_event_post_add_command(self, setup: Any) -> None:
+    @pytest.mark.asyncio
+    @pytest.mark.parametrize(
+        ["post_setup"],
+        [
+            [{"stdin_list": ["disambiguate"]}],
+        ],
+        indirect=["post_setup"],
+    )
+    async def test_event_post_add_command(self, setup: Any, post_setup: Any) -> None:
         """Tests the PostAddCommand event."""
 
         @Event.PostAddCommand.subscribe
-        def hook(new_entries: Dict[str, Entry]) -> None:
-            new_entries["dummy"] = new_entries.pop("einstein_a")
+        def hook(command: AddCommand) -> None:
+            command.new_entries["dummy"] = command.new_entries.pop("einstein_a")
 
         assert Event.PostAddCommand.validate()
 
-        AddCommand().execute(["-b", EXAMPLE_DUPLICATE_ENTRY_BIB])
+        await AddCommand("-b", EXAMPLE_DUPLICATE_ENTRY_BIB).execute()
 
         assert "dummy" in Database().keys()
+
+    @pytest.mark.asyncio
+    @pytest.mark.parametrize(
+        [
+            "args",
+            "msg_string",
+        ],
+        [
+            [
+                ["--skip-existing"],
+                "The '--skip-existing' argument of the 'add' command is deprecated! "
+                "Instead you should use '--disambiguation keep'.",
+            ],
+            [
+                ["--update"],
+                "The '--update' argument of the 'add' command is deprecated! "
+                "Instead you should use '--disambiguation update'.",
+            ],
+        ],
+    )
+    async def test_warn_deprecated_args(
+        self, setup: Any, args: list[str], msg_string: str, caplog: pytest.LogCaptureFixture
+    ) -> None:
+        """Test the warning upon usage of deprecated arguments.
+
+        Args:
+            setup: the `tests.commands.command_test.CommandTest.setup` fixture.
+            args: arguments for the AddCommand.
+            msg_string: the string which the warning message must match.
+            caplog: the built-in pytest fixture.
+        """
+        args = ["-b", EXAMPLE_MULTI_FILE_ENTRY_BIB] + args
+
+        await AddCommand(*args).execute()
+
+        for source, level, msg in caplog.record_tuples:
+            if source == "cobib.commands.add" and level == 30:
+                if msg == msg_string:
+                    break
+        else:
+            pytest.fail("No Warning logged from AddCommand.")
```

### Comparing `cobib-3.5.5/tests/commands/test_delete.py` & `cobib-4.0.0/tests/commands/test_delete.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 """Tests for coBib's DeleteCommand."""
 # pylint: disable=unused-argument
 
 from __future__ import annotations
 
 import contextlib
 import tempfile
-from argparse import Namespace
 from io import StringIO
 from typing import TYPE_CHECKING, Any, List, Type
 
 import pytest
+from typing_extensions import override
 
 from cobib.commands import DeleteCommand
 from cobib.config import Event, config
 from cobib.database import Database
 from cobib.utils.rel_path import RelPath
 
 from .. import get_resource
-from ..tui.tui_test import TUITest
 from .command_test import CommandTest
 
 if TYPE_CHECKING:
     import cobib.commands
 
 
-class TestDeleteCommand(CommandTest, TUITest):
+class TestDeleteCommand(CommandTest):
     """Tests for coBib's DeleteCommand."""
 
+    @override
     def get_command(self) -> Type[cobib.commands.base_command.Command]:
-        # noqa: D102
         return DeleteCommand
 
     def _assert(self, labels: List[str]) -> None:
         """Common assertion utility method.
 
         Args:
             labels: the list of labels to be deleted.
@@ -75,15 +74,15 @@
             setup: the `tests.commands.command_test.CommandTest.setup` fixture.
             labels: the list of labels to be deleted.
             skip_commit: whether to skip asserting the git commit message.
         """
         git = setup.get("git", False)
 
         # delete some data (for testing simplicity we delete the entries from the end)
-        DeleteCommand().execute(labels)
+        DeleteCommand(*labels).execute()
         self._assert(labels)
 
         if git and not skip_commit:
             # assert the git commit message
             self.assert_git_commit_message("delete", {"labels": labels, "preserve_files": False})
 
     @pytest.mark.parametrize("preserve_files", [True, False])
@@ -99,15 +98,15 @@
             open(path.path, "w", encoding="utf-8").close()  # pylint: disable=consider-using-with
 
             Database()["knuthwebsite"].file = str(path)
 
             args = ["knuthwebsite"]
             if preserve_files:
                 args += ["--preserve-files"]
-            DeleteCommand().execute(args)
+            DeleteCommand(*args).execute()
 
             assert path.path.exists() is preserve_files
 
     @pytest.mark.parametrize(["setup"], [[{"git": False}]], indirect=["setup"])
     def test_base_cmd_insufficient_git(self, setup: Any, caplog: pytest.LogCaptureFixture) -> None:
         """Test warning is raised by BaseCommand during insufficient git-configuration.
 
@@ -116,120 +115,67 @@
 
         Args:
             setup: the `tests.commands.command_test.CommandTest.setup` fixture.
             caplog: the built-in pytest fixture.
         """
         config.database.git = True
 
-        DeleteCommand().execute(["knuthwebsite"])
+        DeleteCommand("knuthwebsite").execute()
         self._assert(["knuthwebsite"])
 
         assert (
             "cobib.commands.base_command",
             30,
             "You have configured coBib to track your database with git."
             "\nPlease run `cobib init --git`, to initialize this tracking.",
         ) in caplog.record_tuples
 
+    @pytest.mark.asyncio
     @pytest.mark.parametrize(
         ["labels"],
         [
             [["knuthwebsite"]],
             [["knuthwebsite", "latexcompanion"]],
         ],
     )
     # other variants are already covered by test_command
-    def test_cmdline(self, setup: Any, monkeypatch: pytest.MonkeyPatch, labels: List[str]) -> None:
+    async def test_cmdline(
+        self, setup: Any, monkeypatch: pytest.MonkeyPatch, labels: List[str]
+    ) -> None:
         """Test the command-line access of the command.
 
         Args:
             setup: the `tests.commands.command_test.CommandTest.setup` fixture.
             monkeypatch: the built-in pytest fixture.
             labels: the list of labels to be deleted.
         """
-        self.run_module(monkeypatch, "main", ["cobib", "delete"] + labels)
+        await self.run_module(monkeypatch, "main", ["cobib", "delete"] + labels)
         self._assert(labels)
 
-    @pytest.mark.parametrize(
-        ["select", "keys", "labels"],
-        [
-            [False, "vjvdq", ["knuthwebsite", "latexcompanion"]],
-            [True, "d", ["knuthwebsite"]],
-        ],
-    )
-    def test_tui(self, setup: Any, select: bool, keys: str, labels: List[str]) -> None:
-        """Test the TUI access of the command.
-
-        Args:
-            setup: the `tests.commands.command_test.CommandTest.setup` fixture.
-            select: whether to use the TUI selection.
-            keys: the string of keys to pass to the TUI.
-            labels: the list of labels to be deleted.
-        """
-
-        def assertion(screen, logs, **kwargs):  # type: ignore
-            labels = kwargs.get("labels", [])
-            self._assert(labels)
-
-            true_log = [log for log in logs if log[0] == "cobib.commands.delete"]
-
-            expected_log = [
-                ("cobib.commands.delete", 10, "Delete command triggered from TUI."),
-                ("cobib.commands.delete", 10, "Starting Delete command."),
-            ]
-
-            assert true_log[0:2] == expected_log
-
-            # we cannot constructed a unique expected log because we do not know in which order the
-            # labels are being removed (because the list of labels gets converted from an unordered
-            # set)
-            for label in labels:
-                assert (
-                    "cobib.commands.delete",
-                    10,
-                    f"Attempting to delete entry '{label}'.",
-                ) in true_log
-                assert (
-                    "cobib.commands.delete",
-                    20,
-                    f"'{label}' was removed from the database.",
-                ) in true_log
-
-                # also assert that the label is no longer visible on screen
-                assert all(label not in line for line in screen.display[1:-3])
-
-            assert true_log[-1] == (
-                "cobib.commands.delete",
-                10,
-                "Updating list after Delete command.",
-            )
-
-        self.run_tui(keys, assertion, {"labels": labels})
-
     def test_event_pre_delete_command(self, setup: Any) -> None:
         """Tests the PreDeleteCommand event."""
 
         @Event.PreDeleteCommand.subscribe
-        def hook(largs: Namespace) -> None:
-            largs.labels = ["einstein"]
+        def hook(command: DeleteCommand) -> None:
+            command.largs.labels = ["einstein"]
 
         assert Event.PreDeleteCommand.validate()
 
-        DeleteCommand().execute(["knuthwebsite"])
+        DeleteCommand("knuthwebsite").execute()
 
         assert "einstein" not in Database().keys()
         assert "knuthwebsite" in Database().keys()
 
     def test_event_post_delete_command(self, setup: Any) -> None:
         """Tests the PostDeleteCommand event."""
 
         @Event.PostDeleteCommand.subscribe
-        def hook(deleted_entries: List[str]) -> None:
-            for label in deleted_entries:
+        def hook(command: DeleteCommand) -> None:
+            for label in command.deleted_entries:
                 print(f"WARNING: deleted entry '{label}'")
 
         with contextlib.redirect_stdout(StringIO()) as out:
-            DeleteCommand().execute(["knuthwebsite"])
+            DeleteCommand("knuthwebsite").execute()
 
         assert Event.PostDeleteCommand.validate()
 
         assert out.getvalue().strip() == "WARNING: deleted entry 'knuthwebsite'"
```

### Comparing `cobib-3.5.5/tests/commands/test_edit.py` & `cobib-4.0.0/tests/commands/test_edit.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 """Tests for coBib's EditCommand."""
 # pylint: disable=unused-argument
 
 from __future__ import annotations
 
 import tempfile
-from argparse import Namespace
 from typing import TYPE_CHECKING, Any, List, Optional, Tuple, Type
 
 import pytest
+from typing_extensions import override
 
 from cobib.commands import EditCommand
 from cobib.config import Event, config
-from cobib.database import Database, Entry
+from cobib.database import Database
 from cobib.utils.rel_path import RelPath
 
-from ..tui.tui_test import TUITest
 from .command_test import CommandTest
 
 if TYPE_CHECKING:
     import cobib.commands
 
 
-class TestEditCommand(CommandTest, TUITest):
+class TestEditCommand(CommandTest):
     """Tests for coBib's EditCommand.
 
     Note: in order to be able to test this command to at least a minimal degree, the test
     configuration sets the "editor" to be "cat". Thus, no changes will ever actually be made through
     this "editor".
     Nonetheless, this allows us to test the case where no changes are made (obviously), while also
     being able to test that the EditCommand actually writes to the database when (e.g.) the `--add`
     keyword argument is being used.
     """
 
+    @override
     def get_command(self) -> Type[cobib.commands.base_command.Command]:
-        # noqa: D102
         return EditCommand
 
     @staticmethod
     def _assert(
         changes: bool, logs: Optional[List[Tuple[str, int, str]]] = None, label: str = "dummy"
     ) -> None:
         """Common assertion utility method.
@@ -86,15 +85,15 @@
             setup: the `tests.commands.command_test.CommandTest.setup` fixture.
             caplog: the built-in pytest fixture.
             args: the arguments to pass to the command.
             changes: whether actual changes will be applied.
         """
         git = setup.get("git", False)
 
-        EditCommand().execute(args)
+        EditCommand(*args).execute()
 
         true_log = [rec for rec in caplog.record_tuples if rec[0] == "cobib.commands.edit"]
 
         # check common log
         expected_log = [
             ("cobib.commands.edit", 10, "Starting Edit command."),
             ("cobib.commands.edit", 10, "Creating temporary file."),
@@ -114,15 +113,15 @@
     def test_ignore_add_if_label_exists(self, setup: Any, caplog: pytest.LogCaptureFixture) -> None:
         """Test that the `add` argument is ignored if the label already exists.
 
         Args:
             setup: the `tests.commands.command_test.CommandTest.setup` fixture.
             caplog: the built-in pytest fixture.
         """
-        EditCommand().execute(["-a", "einstein"])
+        EditCommand("-a", "einstein").execute()
         assert (
             "cobib.commands.edit",
             30,
             "Entry 'einstein' already exists! Ignoring the `--add` argument.",
         ) in caplog.record_tuples
 
     @pytest.mark.parametrize("preserve_files", [True, False])
@@ -143,15 +142,15 @@
                 ).close()
 
                 Database()["einstein"].file = str(path)
 
                 args = ["einstein"]
                 if preserve_files:
                     args.insert(2, "--preserve-files")
-                EditCommand().execute(args)
+                EditCommand(*args).execute()
                 assert "dummy" in Database().keys()
 
                 target = RelPath(tmpdirname + "/dummy.pdf")
                 if preserve_files:
                     assert path.path.exists()
                 else:
                     assert target.path.exists()
@@ -161,71 +160,59 @@
     def test_warning_missing_label(self, setup: Any, caplog: pytest.LogCaptureFixture) -> None:
         """Test warning for missing label.
 
         Args:
             setup: the `tests.commands.command_test.CommandTest.setup` fixture.
             caplog: the built-in pytest fixture.
         """
-        EditCommand().execute(["dummy"])
+        EditCommand("dummy").execute()
         assert (
             "cobib.commands.edit",
             40,
             "No entry with the label 'dummy' could be found.\n"
             "Use `--add` to add a new entry with this label.",
         ) in caplog.record_tuples
 
+    @pytest.mark.asyncio
     @pytest.mark.parametrize(
         ["setup"],
         [
             [{"git": False}],
         ],
         indirect=["setup"],
     )
-    def test_cmdline(self, setup: Any, monkeypatch: pytest.MonkeyPatch) -> None:
+    async def test_cmdline(self, setup: Any, monkeypatch: pytest.MonkeyPatch) -> None:
         """Test the command-line access of the command.
 
         Args:
             setup: the `tests.commands.command_test.CommandTest.setup` fixture.
             monkeypatch: the built-in pytest fixture.
         """
-        self.run_module(monkeypatch, "main", ["cobib", "edit", "-a", "dummy"])
+        await self.run_module(monkeypatch, "main", ["cobib", "edit", "-a", "dummy"])
         self._assert(changes=True, logs=None)
 
-    def test_tui(self, setup: Any) -> None:
-        """Test the TUI access of the command.
-
-        Args:
-            setup: the `tests.commands.command_test.CommandTest.setup` fixture.
-        """
-
-        def assertion(screen, logs, **kwargs):  # type: ignore
-            true_log = [log for log in logs if log[0] == "cobib.commands.edit"]
-            self._assert(changes=False, logs=true_log)
-
-        self.run_tui("e", assertion, {})
-
     def test_event_pre_edit_command(self, setup: Any) -> None:
         """Tests the PreEditCommand event."""
 
         @Event.PreEditCommand.subscribe
-        def hook(largs: Namespace) -> None:
-            largs.add = True
-            largs.label = "dummy"
+        def hook(command: EditCommand) -> None:
+            command.largs.add = True
+            command.largs.label = "dummy"
 
         assert Event.PreEditCommand.validate()
 
-        EditCommand().execute(["einstein"])
+        EditCommand("einstein").execute()
 
         self._assert(changes=True)
 
     def test_event_post_edit_command(self, setup: Any) -> None:
         """Tests the PostEditCommand event."""
 
         @Event.PostEditCommand.subscribe
-        def hook(new_entry: Entry) -> None:
-            new_entry.data["tags"] = "test"
+        def hook(command: EditCommand) -> None:
+            command.new_entry.data["tags"] = "test"
 
         assert Event.PostEditCommand.validate()
 
-        EditCommand().execute(["-a", "dummy"])
+        EditCommand("-a", "dummy").execute()
 
         assert Database()["dummy"].data["tags"] == "test"
```

### Comparing `cobib-3.5.5/tests/commands/test_export.py` & `cobib-4.0.0/tests/commands/test_export.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 """Tests for coBib's ExportCommand."""
 # pylint: disable=unused-argument
 
 from __future__ import annotations
 
 import os
 import tempfile
-from argparse import Namespace
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, List, Type
 from zipfile import ZipFile
 
 import pytest
+from typing_extensions import override
 
 from cobib.commands import ExportCommand
 from cobib.config import Event, config
 from cobib.database import Database
 
 from .. import get_resource
-from ..tui.tui_test import TUITest
 from .command_test import CommandTest
 
 TMPDIR = Path(tempfile.gettempdir())
 
 if TYPE_CHECKING:
     import cobib.commands
 
 
-class TestExportCommand(CommandTest, TUITest):
+class TestExportCommand(CommandTest):
     """Tests for coBib's ExportCommand."""
 
+    @override
     def get_command(self) -> Type[cobib.commands.base_command.Command]:
-        # noqa: D102
         return ExportCommand
 
     def _assert(self, args: List[str]) -> None:
         """Common assertion utility method.
 
         Args:
             args: the arguments which were passed to the command.
@@ -109,30 +108,30 @@
             setup: the `tests.commands.command_test.CommandTest.setup` fixture.
             args: the arguments to pass to the command.
         """
         if "-z" in args:
             # add a dummy file to the `einstein` entry
             entry = Database()["einstein"]
             entry.file = get_resource("debug.py")
-        ExportCommand().execute(args)
+        ExportCommand(*args).execute()
         self._assert(args)
 
     @pytest.mark.parametrize("dotless", [False, True])
     def test_journal_abbreviation(self, setup: Any, dotless: bool) -> None:
         """Test journal abbreviation.
 
         Args:
             setup: the `tests.commands.command_test.CommandTest.setup` fixture.
             dotless: whether to abbreviate with or without punctuation.
         """
         config.utils.journal_abbreviations = [("Annalen der Physik", "Ann. Phys.")]
         args = ["-a", "-b", str(TMPDIR / "cobib_test_export.bib"), "-s", "--", "einstein"]
         if dotless:
             args.insert(1, "--dotless")
-        ExportCommand().execute(args)
+        ExportCommand(*args).execute()
         self._assert_journal_abbreviation(dotless)
 
     def _assert_journal_abbreviation(self, dotless: bool) -> None:
         """Assertion utility method for bibtex output.
 
         Args:
             dotless: whether to abbreviate with or without punctuation.
@@ -152,121 +151,74 @@
         """Test warning for missing label.
 
         Args:
             setup: the `tests.commands.command_test.CommandTest.setup` fixture.
             caplog: the built-in pytest fixture.
         """
         args = ["-b", str(TMPDIR / "cobib_test_export.bib"), "-s", "--", "dummy"]
-        ExportCommand().execute(args)
+        ExportCommand(*args).execute()
         assert (
             "cobib.commands.export",
             30,
             "No entry with the label 'dummy' could be found.",
         ) in caplog.record_tuples
 
     def test_warning_missing_output(self, setup: Any, caplog: pytest.LogCaptureFixture) -> None:
         """Test warning for missing output format.
 
         Args:
             setup: the `tests.commands.command_test.CommandTest.setup` fixture.
             caplog: the built-in pytest fixture.
         """
         args = ["-s", "--", "einstein"]
-        ExportCommand().execute(args)
+        ExportCommand(*args).execute()
         assert ("cobib.commands.export", 40, "No output file specified!") in caplog.record_tuples
 
+    @pytest.mark.asyncio
     @pytest.mark.parametrize(
         ["args"],
         [
             [["-b", str(TMPDIR / "cobib_test_export.bib")]],
         ],
     )
     # other variants are already covered by test_command
-    def test_cmdline(self, setup: Any, monkeypatch: pytest.MonkeyPatch, args: List[str]) -> None:
+    async def test_cmdline(
+        self, setup: Any, monkeypatch: pytest.MonkeyPatch, args: List[str]
+    ) -> None:
         """Test the command-line access of the command.
 
         Args:
             setup: the `tests.commands.command_test.CommandTest.setup` fixture.
             monkeypatch: the built-in pytest fixture.
             args: additional arguments to pass to the command.
         """
-        self.run_module(monkeypatch, "main", ["cobib", "export"] + args)
+        await self.run_module(monkeypatch, "main", ["cobib", "export"] + args)
         self._assert(args)
 
-    @pytest.mark.parametrize(
-        ["select", "keys"],
-        [
-            [False, "x-b" + str(TMPDIR / "cobib_test_export.bib") + " -- ++label einstein\n"],
-            [True, "Gvx-b" + str(TMPDIR / "cobib_test_export.bib") + "\n"],
-        ],
-    )
-    def test_tui(self, setup: Any, select: bool, keys: str) -> None:
-        """Test the TUI access of the command.
-
-        Args:
-            setup: the `tests.commands.command_test.CommandTest.setup` fixture.
-            select: whether to use the TUI selection.
-            keys: the string of keys to pass to the TUI.
-        """
-
-        def assertion(screen, logs, **kwargs):  # type: ignore
-            dummy_args = ["-b"]
-            if kwargs.get("selection", False):
-                dummy_args += ["-s"]
-            self._assert(dummy_args)
-
-            expected_log = [
-                ("cobib.commands.export", 10, "Export command triggered from TUI."),
-                ("cobib.commands.export", 10, "Starting Export command."),
-                ("cobib.commands.export", 20, 'Exporting entry "einstein".'),
-            ]
-            if kwargs.get("selection", False):
-                expected_log.insert(
-                    2,
-                    (
-                        "cobib.commands.export",
-                        20,
-                        "Selection given. Interpreting `filter` as a list of labels",
-                    ),
-                )
-            else:
-                expected_log.insert(
-                    2,
-                    (
-                        "cobib.commands.export",
-                        10,
-                        "Gathering filtered list of entries to be exported.",
-                    ),
-                )
-
-            assert [log for log in logs if log[0] == "cobib.commands.export"] == expected_log
-
-        self.run_tui(keys, assertion, {"selection": select})
-
     def test_event_pre_export_command(self, setup: Any) -> None:
         """Tests the PreExportCommand event."""
         args = ["-b", str(TMPDIR / "cobib_test_export.bib")]
 
         @Event.PreExportCommand.subscribe
-        def hook(largs: Namespace) -> None:
-            largs.selection = True
-            largs.filter = ["einstein"]
+        def hook(command: ExportCommand) -> None:
+            command.largs.selection = True
+            command.largs.filter = ["einstein"]
 
         assert Event.PreExportCommand.validate()
 
-        ExportCommand().execute(args)
+        ExportCommand(*args).execute()
 
         self._assert_bib(["-s"] + args + ["--", "einstein"])
 
     def test_event_post_export_command(self, setup: Any) -> None:
         """Tests the PostExportCommand event."""
         args = ["-b", str(TMPDIR / "cobib_test_export.bib")]
 
         @Event.PostExportCommand.subscribe
-        def hook(labels: List[str], largs: Namespace) -> None:
+        def hook(command: ExportCommand) -> None:
             os.remove(str(TMPDIR / "cobib_test_export.bib"))
 
         assert Event.PostExportCommand.validate()
 
-        ExportCommand().execute(args)
+        ExportCommand(*args).execute()
 
         assert not os.path.exists(str(TMPDIR / "cobib_test_export.bib"))
```

### Comparing `cobib-3.5.5/tests/commands/test_git_commit_event.py` & `cobib-4.0.0/tests/commands/test_git_commit_event.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,66 +1,78 @@
 """coBib GitCommit event tests."""
 # pylint: disable=unused-argument
 
 from __future__ import annotations
 
-import sys
+import argparse
 from pathlib import Path
-from typing import IO, TYPE_CHECKING, Any, Dict, List, Optional, Type
+from typing import TYPE_CHECKING, Any, Dict, Optional, Type
 
 import pytest
+from rich.console import Console
+from rich.prompt import PromptBase
+from textual.app import App
+from typing_extensions import override
 
 from cobib.commands.base_command import Command
 from cobib.config import Event, config
 from cobib.utils.rel_path import RelPath
 
 from .command_test import CommandTest
 
 if TYPE_CHECKING:
     import cobib.commands
-    import cobib.tui
 
 
 class DummyCommand(Command):
     """A dummy command to test the GitCommit events."""
 
     name = "dummy"
 
-    def execute(self, args: List[str], out: IO[Any] = sys.stdout) -> None:
+    @override
+    def __init__(
+        self,
+        *args: str,
+        console: Console | App[None] | None = None,
+        prompt: Type[PromptBase[str]] | None = None,
+    ) -> None:
+        # pylint: disable=super-init-not-called
+        self.largs = argparse.Namespace()
+
+    @override
+    @classmethod
+    def init_argparser(cls) -> None:
+        pass
+
+    def execute(self) -> None:
         """Does nothing but generate a dummy git commit.
 
         Args:
             args: a sequence of additional arguments used for the execution.
             out: the output IO stream. This defaults to `sys.stdout`.
         """
         with open(config.database.file, "a", encoding="utf-8") as file:
             file.write("dummy")
 
         self.git()
 
-    @staticmethod
-    def tui(tui: cobib.tui.TUI) -> None:
-        # pdoc will inherit the docstring from the base class
-        # noqa: D102
-        pass
-
 
 class TestGitCommitEvent(CommandTest):
     """Tests for the automatic git-commit related events."""
 
+    @override
     def get_command(self) -> Type[cobib.commands.base_command.Command]:
-        # noqa: D102
         return DummyCommand
 
+    @override
     def test_command(self) -> None:
-        # noqa: D102
         pytest.skip("The dummy command has no actual command.")
 
+    @override
     def test_handle_argument_error(self, caplog: pytest.LogCaptureFixture) -> None:
-        # noqa: D102
         pytest.skip("The dummy command has no argument parser.")
 
     @pytest.mark.parametrize("setup", [{"git": True}], indirect=["setup"])
     def test_event_pre_git_commit(self, setup: Any) -> None:
         """Test the PreGitCommit event.
 
         Args:
@@ -69,15 +81,15 @@
 
         @Event.PreGitCommit.subscribe
         def hook(msg: str, args: Optional[Dict[str, Any]] = None) -> Optional[str]:
             return "Hello world!"
 
         assert Event.PreGitCommit.validate()
 
-        DummyCommand().execute([])
+        DummyCommand().execute()
 
         self.assert_git_commit_message("dummy", msg="Hello world!\n")
 
     @pytest.mark.parametrize("setup", [{"git": True}], indirect=["setup"])
     def test_event_post_git_commit(self, setup: Any) -> None:
         """Test the PostGitCommit event.
 
@@ -87,10 +99,10 @@
 
         @Event.PostGitCommit.subscribe
         def hook(root: Path, file: Path) -> None:
             file.unlink()
 
         assert Event.PostGitCommit.validate()
 
-        DummyCommand().execute([])
+        DummyCommand().execute()
 
         assert not RelPath(config.database.file).path.exists()
```

### Comparing `cobib-3.5.5/tests/commands/test_import.py` & `cobib-4.0.0/tests/commands/test_import.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,93 +1,71 @@
 """Tests for coBib's ImportCommand."""
 # pylint: disable=unused-argument
 
 from __future__ import annotations
 
-import logging
-from argparse import Namespace
-from typing import TYPE_CHECKING, Any, Dict, Type
+from typing import TYPE_CHECKING, Any, Type
 
 import pytest
+from typing_extensions import override
 
 from cobib.commands import ImportCommand
 from cobib.config import Event
-from cobib.database import Entry
 
-from ..tui.tui_test import TUITest
 from .command_test import CommandTest
 
 if TYPE_CHECKING:
     import cobib.commands
 
 
-class TestImportCommand(CommandTest, TUITest):
+class TestImportCommand(CommandTest):
     """Tests for coBib's ImportCommand."""
 
+    @override
     def get_command(self) -> Type[cobib.commands.base_command.Command]:
-        # noqa: D102
         return ImportCommand
 
-    def get_safe_command_name(self) -> str:
-        # noqa: D102
-        return "import_"
-
-    def test_command(self) -> None:
+    @pytest.mark.asyncio
+    async def test_command(self) -> None:  # type: ignore[override]
+        # pylint: disable=invalid-overridden-method
         """Test the command itself."""
         with pytest.raises(SystemExit):
-            ImportCommand().execute(["-h"])
+            await ImportCommand("-h").execute()
 
-    def test_cmdline(self, setup: Any, monkeypatch: pytest.MonkeyPatch) -> None:
+    @pytest.mark.asyncio
+    async def test_cmdline(self, setup: Any, monkeypatch: pytest.MonkeyPatch) -> None:
         """Test the command-line access of the command.
 
         Args:
             setup: the `tests.commands.command_test.CommandTest.setup` fixture.
             monkeypatch: the built-in pytest fixture.
         """
         with pytest.raises(SystemExit):
-            self.run_module(monkeypatch, "main", ["cobib", "import", "-h"])
-
-    def test_tui(self, setup: Any) -> None:
-        """Test the TUI access of the command.
-
-        Args:
-            setup: the `tests.commands.command_test.CommandTest.setup` fixture.
-        """
-
-        def assertion(screen, logs, **kwargs):  # type: ignore
-            for source, level, message in logs:
-                if ("cobib.tui.tui", logging.INFO) == (
-                    source,
-                    level,
-                ) and "sys.stderr contains:usage: import [-h] [--skip-download]" in message:
-                    break
-            else:
-                pytest.fail("No help message logged to sys.stderr.")
-
-        keys = "i\n"
-        self.run_tui(keys, assertion, {})
+            await self.run_module(monkeypatch, "main", ["cobib", "import", "-h"])
 
-    def test_event_pre_import_command(self, setup: Any) -> None:
+    @pytest.mark.asyncio
+    async def test_event_pre_import_command(self, setup: Any) -> None:
         """Tests the PreImportCommand event."""
 
         @Event.PreImportCommand.subscribe
-        def hook(largs: Namespace) -> None:
-            largs.zotero = False
+        def hook(command: ImportCommand) -> None:
+            command.largs.zotero = False
 
         assert Event.PreImportCommand.validate()
 
-        ImportCommand().execute(["--zotero"])
+        await ImportCommand("--zotero").execute()
 
-    def test_event_post_import_command(self, setup: Any) -> None:
+    @pytest.mark.asyncio
+    async def test_event_post_import_command(self, setup: Any) -> None:
         """Tests the PostImportCommand event."""
 
         @Event.PostImportCommand.subscribe
-        def hook(new_entries: Dict[str, Entry]) -> None:
+        def hook(command: ImportCommand) -> None:
             pass
 
         assert Event.PostImportCommand.validate()
 
         @Event.PreImportCommand.subscribe
-        def aux_hook(largs: Namespace) -> None:
-            largs.zotero = False
+        def aux_hook(command: ImportCommand) -> None:
+            command.largs.zotero = False
 
-        ImportCommand().execute(["--zotero"])
+        await ImportCommand("--zotero").execute()
```

### Comparing `cobib-3.5.5/tests/commands/test_init.py` & `cobib-4.0.0/tests/commands/test_init.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 """Tests for coBib's InitCommand."""
 # pylint: disable=unused-argument
 
 from __future__ import annotations
 
 import os
-from argparse import Namespace
 from datetime import datetime
-from pathlib import Path
 from shutil import rmtree
 from typing import TYPE_CHECKING, Any, Type
 
 import pytest
+from typing_extensions import override
 
 from cobib.commands import InitCommand
 from cobib.config import Event, config
 
 from .command_test import CommandTest
 
 if TYPE_CHECKING:
     import cobib.commands
 
 
 class TestInitCommand(CommandTest):
     """Tests for coBib's InitCommand."""
 
+    @override
     def get_command(self) -> Type[cobib.commands.base_command.Command]:
-        # noqa: D102
         return InitCommand
 
     @pytest.mark.parametrize(
         ["setup"],
         [
             [{"git": False, "database": False}],
             [{"git": True, "database": False}],
@@ -48,15 +47,18 @@
         if safe:
             # fill database file
             with open(config.database.file, "w", encoding="utf-8") as file:
                 file.write("test")
         # store current time
         now = float(datetime.now().timestamp())
         # try running init
-        InitCommand().execute(["--git"] if setup["git"] else [])
+        if setup["git"]:
+            InitCommand("--git").execute()
+        else:
+            InitCommand().execute()
         if safe:
             # check database file still contains 'test'
             with open(config.database.file, "r", encoding="utf-8") as file:
                 assert file.read() == "test"
         else:
             # check creation time of temporary database file
             ctime = os.stat(config.database.file).st_ctime
@@ -86,15 +88,15 @@
             setup: the `tests.commands.command_test.CommandTest.setup` fixture.
             caplog: the built-in pytest fixture.
         """
         try:
             # store current time
             now = float(datetime.now().timestamp())
             # try running init
-            InitCommand().execute(["--git"])
+            InitCommand("--git").execute()
 
             # assert warning is printed
             assert (
                 "cobib.commands.init",
                 30,
                 "You are about to initialize the git tracking of your database, but this will only "
                 "have effect if you also enable the DATABASE/git setting in your configuration "
@@ -114,57 +116,58 @@
             assert self.COBIB_TEST_DIR_GIT.is_dir()
             # assert the git commit message
             self.assert_git_commit_message("init", {"git": True})
         finally:
             # clean up file system
             rmtree(self.COBIB_TEST_DIR_GIT)
 
+    @pytest.mark.asyncio
     @pytest.mark.parametrize(
         ["setup"],
         [
             [{"git": False, "database": False}],
         ],
         indirect=["setup"],
     )
     # other variants are already covered by test_command
-    def test_cmdline(self, setup: Any, monkeypatch: pytest.MonkeyPatch) -> None:
+    async def test_cmdline(self, setup: Any, monkeypatch: pytest.MonkeyPatch) -> None:
         """Test the command-line access of the command.
 
         Args:
             setup: the `tests.commands.command_test.CommandTest.setup` fixture.
             monkeypatch: the built-in pytest fixture.
         """
         # store current time
         now = float(datetime.now().timestamp())
         # try calling init
-        self.run_module(monkeypatch, "main", ["cobib", "init"])
+        await self.run_module(monkeypatch, "main", ["cobib", "init"])
         # try running init
         # check creation time of temporary database file
         ctime = os.stat(config.database.file).st_ctime
         # assert these times are close
         assert ctime - now < 0.1 or now - ctime < 0.1
 
     def test_event_pre_init_command(self, setup: Any) -> None:
         """Tests the PreInitCommand event."""
 
         @Event.PreInitCommand.subscribe
-        def hook(largs: Namespace) -> None:
-            largs.git = True
+        def hook(command: InitCommand) -> None:
+            command.largs.git = True
 
         assert Event.PreInitCommand.validate()
 
-        InitCommand().execute([])
+        InitCommand().execute()
 
         self.assert_git_commit_message("init", {"git": True})
 
     def test_event_post_init_command(self, setup: Any) -> None:
         """Tests the PostInitCommand event."""
 
         @Event.PostInitCommand.subscribe
-        def hook(root: Path, file: Path) -> None:
-            os.remove(file)
+        def hook(command: InitCommand) -> None:
+            os.remove(command.file)
 
         assert Event.PostInitCommand.validate()
 
-        InitCommand().execute([])
+        InitCommand().execute()
 
         assert not os.path.exists(self.COBIB_TEST_DIR_GIT / "literature.yaml")
```

### Comparing `cobib-3.5.5/tests/commands/test_modify.py` & `cobib-4.0.0/tests/commands/test_modify.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 """Tests for coBib's ModifyCommand."""
 # pylint: disable=unused-argument
 
 from __future__ import annotations
 
 import contextlib
 import tempfile
-from argparse import Namespace
 from io import StringIO
 from typing import TYPE_CHECKING, Any, List, Type
 
 import pytest
+from typing_extensions import override
 
 from cobib.commands import ModifyCommand
 from cobib.config import Event
 from cobib.database import Database
 from cobib.utils.rel_path import RelPath
 
-from ..tui.tui_test import TUITest
 from .command_test import CommandTest
 
 if TYPE_CHECKING:
     import cobib.commands
 
 
-class TestModifyCommand(CommandTest, TUITest):
+class TestModifyCommand(CommandTest):
     """Tests for coBib's ModifyCommand."""
 
+    @override
     def get_command(self) -> Type[cobib.commands.base_command.Command]:
-        # noqa: D102
         return ModifyCommand
 
     @pytest.mark.parametrize(
         ["setup"],
         [
             [{"git": False}],
             [{"git": True}],
@@ -73,22 +72,22 @@
         if selection:
             args = ["-s"] + args
 
         expected = ["test"]
 
         if add:
             # first insert something to add to
-            ModifyCommand().execute(["tags:dummy", "++label", "einstein"])
+            ModifyCommand("tags:dummy", "++label", "einstein").execute()
             args = ["-a"] + args
             expected = ["dummy"] + expected
 
         if dry:
             args.insert(0, "--dry")
 
-        ModifyCommand().execute(args)
+        ModifyCommand(*args).execute()
 
         if dry:
             if add:
                 assert Database()["einstein"].data["tags"] == ["dummy"]
             else:
                 assert "tags" not in Database()["einstein"].data.keys()
         else:
@@ -96,19 +95,19 @@
 
         if git:
             try:
                 # assert the git commit message
                 self.assert_git_commit_message(
                     "modify",
                     {
+                        "modification": modification.split(":"),
                         "dry": False,
                         "add": add,
-                        "selection": selection,
                         "preserve_files": False,
-                        "modification": modification.split(":"),
+                        "selection": selection,
                         "filter": filters,
                     },
                 )
             except AssertionError:
                 assert dry
 
     @pytest.mark.parametrize(
@@ -129,15 +128,15 @@
             expected: the expected final `Entry` field.
         """
         # modify some data
         args = ["-a", modification, "++label", "einstein"]
 
         field, _ = modification.split(":")
 
-        ModifyCommand().execute(args)
+        ModifyCommand(*args).execute()
 
         assert Database()["einstein"].data[field] == expected
 
     @pytest.mark.parametrize(
         ["modification", "expected"],
         [
             ["pages:{pages.replace('--', '-')}", "891-921"],
@@ -157,15 +156,15 @@
             expected: the expected final `Entry` field.
         """
         # modify some data
         args = [modification, "++label", "einstein"]
 
         field, *_ = modification.split(":")
 
-        ModifyCommand().execute(args)
+        ModifyCommand(*args).execute()
 
         if field != "label":
             assert Database()["einstein"].data[field] == expected
         else:
             assert "eistein" not in Database().keys()
             assert expected in Database().keys()
             assert Database()[expected].label == expected
@@ -183,15 +182,15 @@
             open(path.path, "w", encoding="utf-8").close()  # pylint: disable=consider-using-with
 
             Database()["knuthwebsite"].file = str(path)
 
             args = ["label:dummy", "-s", "--", "knuthwebsite"]
             if preserve_files:
                 args.insert(2, "--preserve-files")
-            ModifyCommand().execute(args)
+            ModifyCommand(*args).execute()
             assert "dummy" in Database().keys()
 
             target = RelPath(tmpdirname + "/dummy.pdf")
             if preserve_files:
                 assert path.path.exists()
             else:
                 assert target.path.exists()
@@ -201,21 +200,22 @@
 
         Args:
             setup: the `tests.commands.command_test.CommandTest.setup` fixture.
             caplog: the built-in pytest fixture.
         """
         # Note: when using a filter, no non-existent label can occur
         args = ["-s", "tags:test", "--", "dummy"]
-        ModifyCommand().execute(args)
+        ModifyCommand(*args).execute()
         assert (
             "cobib.commands.modify",
             30,
             "No entry with the label 'dummy' could be found.",
         ) in caplog.record_tuples
 
+    @pytest.mark.asyncio
     @pytest.mark.parametrize(
         ["setup"],
         [
             [{"git": False}],
         ],
         indirect=["setup"],
     )
@@ -223,99 +223,45 @@
         ["args"],
         [
             [["-s", "tags:test", "--", "einstein"]],
             [["tags:test", "--", "++label", "einstein"]],
         ],
     )
     # other variants are already covered by test_command
-    def test_cmdline(self, setup: Any, monkeypatch: pytest.MonkeyPatch, args: List[str]) -> None:
+    async def test_cmdline(
+        self, setup: Any, monkeypatch: pytest.MonkeyPatch, args: List[str]
+    ) -> None:
         """Test the command-line access of the command.
 
         Args:
             setup: the `tests.commands.command_test.CommandTest.setup` fixture.
             monkeypatch: the built-in pytest fixture.
             args: additional arguments to pass to the command.
         """
-        self.run_module(monkeypatch, "main", ["cobib", "modify"] + args)
+        await self.run_module(monkeypatch, "main", ["cobib", "modify"] + args)
         assert Database()["einstein"].data["tags"] == ["test"]
 
-    @pytest.mark.parametrize(
-        ["select", "keys"],
-        [
-            [False, "mtags:test -- ++label knuthwebsite\n\n"],
-            [True, "vmtags:test\n\n"],
-        ],
-    )
-    def test_tui(self, setup: Any, select: bool, keys: str) -> None:
-        """Test the TUI access of the command.
-
-        Args:
-            setup: the `tests.commands.command_test.CommandTest.setup` fixture.
-            select: whether to use the TUI selection.
-            keys: the string of keys to pass to the TUI.
-        """
-
-        def assertion(screen, logs, **kwargs):  # type: ignore
-            expected_screen = [
-                "@misc{knuthwebsite,",
-                "author = {Donald Knuth},",
-                "tags = {test},",
-                "title = {Knuth: Computers and Typesetting},",
-                r"url = {http://www-cs-faculty.stanford.edu/\~{}uno/abcde.html}",
-                "}",
-            ]
-            for line, truth in zip(expected_screen, screen.display[1:]):
-                assert line == truth.strip()
-
-            expected_log = [
-                ("cobib.commands.modify", 10, "Modify command triggered from TUI."),
-                ("cobib.commands.modify", 10, "Starting Modify command."),
-                ("cobib.commands.modify", 20, "'knuthwebsite' was modified."),
-            ]
-            if kwargs.get("selection", False):
-                expected_log.insert(
-                    2,
-                    (
-                        "cobib.commands.modify",
-                        20,
-                        "Selection given. Interpreting `filter` as a list of labels",
-                    ),
-                )
-            else:
-                expected_log.insert(
-                    2,
-                    (
-                        "cobib.commands.modify",
-                        10,
-                        "Gathering filtered list of entries to be modified.",
-                    ),
-                )
-            assert [log for log in logs if log[0] == "cobib.commands.modify"] == expected_log
-
-        self.run_tui(keys, assertion, {"selection": select})
-
     def test_event_pre_modify_command(self, setup: Any) -> None:
         """Tests the PreModifyCommand event."""
 
         @Event.PreModifyCommand.subscribe
-        def hook(largs: Namespace) -> None:
-            largs.modification = ("number", "2")
+        def hook(command: ModifyCommand) -> None:
+            command.largs.modification = ("number", "2")
 
         assert Event.PreModifyCommand.validate()
 
-        ModifyCommand().execute(["-a", "number:3", "++label", "einstein"])
+        ModifyCommand("-a", "number:3", "++label", "einstein").execute()
 
         assert Database()["einstein"].data["number"] == 12
 
     def test_event_post_modify_command(self, setup: Any) -> None:
         """Tests the PostModifyCommand event."""
 
         @Event.PostModifyCommand.subscribe
-        def hook(labels: List[str], dry: bool) -> None:
-            print(labels)
+        def hook(command: ModifyCommand) -> None:
+            print([entry.label for entry in command.modified_entries])
 
         assert Event.PostModifyCommand.validate()
 
         with contextlib.redirect_stdout(StringIO()) as out:
-            ModifyCommand().execute(["-a", "number:3", "++label", "einstein"])
-
+            ModifyCommand("-a", "number:3", "++label", "einstein").execute()
             assert out.getvalue() == "['einstein']\n"
```

### Comparing `cobib-3.5.5/tests/commands/test_open.py` & `cobib-4.0.0/tests/commands/test_open.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 """Tests for coBib's OpenCommand."""
 # pylint: disable=unused-argument
 
 from __future__ import annotations
 
 import sys
-from argparse import Namespace
 from typing import TYPE_CHECKING, Any, Dict, Generator, List, Optional, Tuple, Type
 
 import pytest
+from typing_extensions import override
 
 from cobib.commands import OpenCommand
 from cobib.config import Event, config
 from cobib.database import Database
 
 from .. import MockStdin, get_resource
-from ..tui.tui_test import TUITest
 from .command_test import CommandTest
 
 if TYPE_CHECKING:
     import _pytest.fixtures
 
     import cobib.commands
 
 
-class TestOpenCommand(CommandTest, TUITest):
+class TestOpenCommand(CommandTest):
     """Tests for coBib's OpenCommand."""
 
     # Note: we can hard-code the `/tmp` path here, because we never really create these files.
     # We just need some absolute paths to test against.
     TMP_FILE_A = "/tmp/a.txt"
     TMP_FILE_B = "/tmp/b.txt"
 
+    @override
     def get_command(self) -> Type[cobib.commands.base_command.Command]:
-        # noqa: D102
         return OpenCommand
 
     @pytest.fixture
     def post_setup(
         self, monkeypatch: pytest.MonkeyPatch, request: _pytest.fixtures.SubRequest
     ) -> Generator[Dict[str, Any], None, None]:
         """Additional setup instructions.
@@ -92,44 +91,43 @@
                 assert logs == expected_log
         else:
             expected_out = [
                 "  1: [file] " + self.TMP_FILE_A,
                 "  2: [file] " + self.TMP_FILE_B,
                 "  3: [url] https://www.duckduckgo.com",
                 "  4: [url] https://www.google.com",
-                "Entry to open [Type 'help' for more info]: ",
+                "[all,help,cancel]: ",
             ]
 
             expected_log = [
                 ("cobib.commands.open", 10, "Starting Open command."),
                 ("cobib.commands.open", 10, 'Parsing "' + self.TMP_FILE_A + '" for URLs.'),
                 ("cobib.commands.open", 10, 'Parsing "' + self.TMP_FILE_B + '" for URLs.'),
                 ("cobib.commands.open", 10, 'Parsing "https://www.duckduckgo.com" for URLs.'),
                 ("cobib.commands.open", 10, 'Parsing "https://www.google.com" for URLs.'),
             ]
 
             stdin_list = kwargs.get("stdin_list", [])
             extra_logs = None
-            if not stdin_list:
-                expected_log.append(("cobib.commands.open", 30, "User aborted open command."))
-            elif "help" in stdin_list:
+            if "help" in stdin_list:
                 expected_out += expected_out.copy()
-                expected_out[4] += "You can specify one of the following options:"
+                expected_out[4] += "Multiple targets were found. You may select the following:"
                 extra_out = [
-                    "  1. a url number",
-                    "  2. a field name provided in '[...]'",
-                    "  3. or simply 'all'",
-                    "  4. ENTER will abort the command",
-                    "",
+                    "  1. an individual URL number",
+                    "  2. a target type (provided in '[...]')",
+                    "  3. 'all'",
+                    "  4. or 'cancel' to abort the command",
                 ]
                 for line in reversed(extra_out):
                     expected_out.insert(5, line)
 
                 expected_log.append(("cobib.commands.open", 10, "User requested help."))
                 expected_log.append(("cobib.commands.open", 30, "User aborted open command."))
+            elif "cancel" in stdin_list:
+                expected_log.append(("cobib.commands.open", 30, "User aborted open command."))
             elif "all" in stdin_list:
                 extra_logs = [
                     ("cobib.commands.open", 10, "User selected all urls."),
                     ("cobib.commands.open", 10, 'Opening "' + self.TMP_FILE_A + '" with cat.'),
                     ("cobib.commands.open", 10, 'Opening "' + self.TMP_FILE_B + '" with cat.'),
                     ("cobib.commands.open", 10, 'Opening "https://www.duckduckgo.com" with cat.'),
                     ("cobib.commands.open", 10, 'Opening "https://www.google.com" with cat.'),
@@ -150,27 +148,28 @@
                 expected_log.extend(extra_logs)
 
             for line, truth in zip(output, expected_out):
                 assert line == truth
             if logs is not None:
                 assert logs == expected_log
 
+    @pytest.mark.asyncio
     @pytest.mark.parametrize(
         ["args", "post_setup"],
         [
             [["knuthwebsite"], {"multi_file": False}],
-            [["example_multi_file_entry"], {"multi_file": True}],
-            [["example_multi_file_entry"], {"multi_file": True, "stdin_list": ["help"]}],
+            [["example_multi_file_entry"], {"multi_file": True, "stdin_list": ["cancel"]}],
+            [["example_multi_file_entry"], {"multi_file": True, "stdin_list": ["help", "cancel"]}],
             [["example_multi_file_entry"], {"multi_file": True, "stdin_list": ["all"]}],
             [["example_multi_file_entry"], {"multi_file": True, "stdin_list": ["url"]}],
             [["example_multi_file_entry"], {"multi_file": True, "stdin_list": ["1"]}],
         ],
         indirect=["post_setup"],
     )
-    def test_command(
+    async def test_command(  # pylint: disable=invalid-overridden-method
         self,
         setup: Any,
         post_setup: Any,
         caplog: pytest.LogCaptureFixture,
         capsys: pytest.CaptureFixture[str],
         args: List[str],
     ) -> None:
@@ -179,50 +178,57 @@
         Args:
             setup: the `tests.commands.command_test.CommandTest.setup` fixture.
             post_setup: an additional setup fixture.
             caplog: the built-in pytest fixture.
             capsys: the built-in pytest fixture.
             args: the arguments to pass to the command.
         """
-        OpenCommand().execute(args)
+        await OpenCommand(*args).execute()
 
         true_log = [rec for rec in caplog.record_tuples if rec[0] == "cobib.commands.open"]
         true_out = capsys.readouterr().out.split("\n")
 
         self._assert(true_out, true_log, **post_setup)
 
-    def test_warning_missing_label(self, setup: Any, caplog: pytest.LogCaptureFixture) -> None:
+    @pytest.mark.asyncio
+    async def test_warning_missing_label(
+        self, setup: Any, caplog: pytest.LogCaptureFixture
+    ) -> None:
         """Test warning for missing label.
 
         Args:
             setup: the `tests.commands.command_test.CommandTest.setup` fixture.
             caplog: the built-in pytest fixture.
         """
-        OpenCommand().execute(["dummy"])
+        await OpenCommand("dummy").execute()
         assert (
             "cobib.commands.open",
             30,
             "No entry with the label 'dummy' could be found.",
         ) in caplog.record_tuples
 
-    def test_warning_nothing_to_open(self, setup: Any, caplog: pytest.LogCaptureFixture) -> None:
+    @pytest.mark.asyncio
+    async def test_warning_nothing_to_open(
+        self, setup: Any, caplog: pytest.LogCaptureFixture
+    ) -> None:
         """Test warning for label with nothing to open.
 
         Args:
             setup: the `tests.commands.command_test.CommandTest.setup` fixture.
             caplog: the built-in pytest fixture.
         """
-        OpenCommand().execute(["einstein"])
+        await OpenCommand("einstein").execute()
         assert (
             "cobib.commands.open",
             30,
             "The entry 'einstein' has no actionable field associated with it.",
         ) in caplog.record_tuples
 
-    def test_config_openable_fields(
+    @pytest.mark.asyncio
+    async def test_config_openable_fields(
         self,
         setup: Any,
         monkeypatch: pytest.MonkeyPatch,
         capsys: pytest.CaptureFixture[str],
     ) -> None:
         """Test the `config.commands.open.fields` setting.
 
@@ -241,38 +247,39 @@
                     if line == "  file:\n":
                         database.write("  note:\n")
                     else:
                         database.write(line)
 
         Database().read()
 
-        monkeypatch.setattr("sys.stdin", MockStdin())
+        monkeypatch.setattr("sys.stdin", MockStdin(["cancel"]))
 
-        OpenCommand().execute(["example_multi_file_entry"])
+        await OpenCommand("example_multi_file_entry").execute()
 
         true_out = capsys.readouterr().out.split("\n")
 
         expected_out = [
             "  1: [note] " + self.TMP_FILE_A,
             "  2: [note] " + self.TMP_FILE_B,
-            "Entry to open [Type 'help' for more info]: ",
+            "[all,help,cancel]: ",
         ]
 
         for line, truth in zip(true_out, expected_out):
             assert line == truth
 
-    def test_open_non_list_field(
+    @pytest.mark.asyncio
+    async def test_open_non_list_field(
         self,
         setup: Any,
         monkeypatch: pytest.MonkeyPatch,
         caplog: pytest.LogCaptureFixture,
     ) -> None:
         """Test opening of non-list type fields.
 
-        This is a regression test against https://gitlab.com/mrossinek/cobib/-/issues/100
+        This is a regression test against https://gitlab.com/cobib/cobib/-/issues/100
 
         Args:
             setup: the `tests.commands.command_test.CommandTest.setup` fixture.
             monkeypatch: the built-in pytest fixture.
             caplog: the built-in pytest fixture.
         """
         config.commands.open.fields = ["note"]
@@ -288,15 +295,15 @@
                         break
                     database.write(line)
 
         Database().read()
 
         monkeypatch.setattr("sys.stdin", MockStdin())
 
-        OpenCommand().execute(["example_multi_file_entry"])
+        await OpenCommand("example_multi_file_entry").execute()
 
         true_log = [rec for rec in caplog.record_tuples if rec[0] == "cobib.commands.open"]
 
         expected_log = [
             ("cobib.commands.open", 10, "Starting Open command."),
             (
                 "cobib.commands.open",
@@ -307,135 +314,83 @@
                 "cobib.commands.open",
                 10,
                 'Opening "/tmp/a.txt" with cat.',
             ),
         ]
         assert true_log == expected_log
 
+    @pytest.mark.asyncio
     @pytest.mark.parametrize(
         ["post_setup"],
         [
             [{"multi_file": False}],
         ],
         indirect=["post_setup"],
     )
-    def test_cmdline(
+    async def test_cmdline(
         self,
         setup: Any,
         post_setup: Any,
         monkeypatch: pytest.MonkeyPatch,
         capsys: pytest.CaptureFixture[str],
     ) -> None:
         """Test the command-line access of the command.
 
         Args:
             setup: the `tests.commands.command_test.CommandTest.setup` fixture.
             post_setup: an additional setup fixture.
             monkeypatch: the built-in pytest fixture.
             capsys: the built-in pytest fixture.
         """
-        self.run_module(monkeypatch, "main", ["cobib", "open", "knuthwebsite"])
+        await self.run_module(monkeypatch, "main", ["cobib", "open", "knuthwebsite"])
 
         true_out = capsys.readouterr().out.split("\n")
 
         self._assert(true_out, logs=None, **post_setup)
 
-    @pytest.mark.parametrize(
-        ["select", "keys"],
-        [
-            [False, "o"],
-            [True, "Gvo"],
-        ],
-    )
-    def test_tui(self, setup: Any, select: bool, keys: str) -> None:
-        """Test the TUI access of the command.
-
-        Args:
-            setup: the `tests.commands.command_test.CommandTest.setup` fixture.
-            select: whether to use the TUI selection.
-            keys: the string of keys to pass to the TUI.
-        """
-
-        def assertion(screen, logs, **kwargs):  # type: ignore
-            expected_log = [
-                ("cobib.commands.open", 10, "Open command triggered from TUI."),
-                ("cobib.commands.open", 10, "Starting Open command."),
-            ]
-            if kwargs.get("selection", False):
-                expected_log.append(
-                    (
-                        "cobib.commands.open",
-                        30,
-                        "The entry 'einstein' has no actionable field associated with it.",
-                    )
-                )
-            else:
-                expected_log.append(
-                    (
-                        "cobib.commands.open",
-                        10,
-                        # fmt: off
-                        'Parsing "http://www-cs-faculty.stanford.edu/\\~{}uno/abcde.html" for '
-                        'URLs.',
-                        # fmt: on
-                    )
-                )
-                expected_log.append(
-                    (
-                        "cobib.commands.open",
-                        10,
-                        # fmt: off
-                        'Opening "http://www-cs-faculty.stanford.edu/\\~{}uno/abcde.html" with '
-                        'cat.',
-                        # fmt: on
-                    )
-                )
-
-            assert [log for log in logs if log[0] == "cobib.commands.open"] == expected_log
-
-        self.run_tui(keys, assertion, {"selection": select})
-
-    def test_event_pre_open_command(
+    @pytest.mark.asyncio
+    async def test_event_pre_open_command(
         self,
         setup: Any,
         post_setup: Any,
         caplog: pytest.LogCaptureFixture,
         capsys: pytest.CaptureFixture[str],
     ) -> None:
         """Tests the PreOpenCommand event."""
 
         @Event.PreOpenCommand.subscribe
-        def hook(largs: Namespace) -> None:
-            largs.labels = ["knuthwebsite"]
+        def hook(command: OpenCommand) -> None:
+            command.largs.labels = ["knuthwebsite"]
 
         assert Event.PreOpenCommand.validate()
 
-        OpenCommand().execute(["einstein"])
+        await OpenCommand("einstein").execute()
 
         true_log = [rec for rec in caplog.record_tuples if rec[0] == "cobib.commands.open"]
         true_out = capsys.readouterr().out.split("\n")
 
         self._assert(true_out, true_log, multi_file=False)
 
-    def test_event_post_open_command(
+    @pytest.mark.asyncio
+    async def test_event_post_open_command(
         self,
         setup: Any,
         post_setup: Any,
         caplog: pytest.LogCaptureFixture,
         capsys: pytest.CaptureFixture[str],
     ) -> None:
         """Tests the PostOpenCommand event."""
 
         @Event.PostOpenCommand.subscribe
-        def hook(labels: List[str]) -> None:
-            print(labels, file=sys.stderr)
+        def hook(command: OpenCommand) -> None:
+            print(command.largs.labels, file=sys.stderr)
 
         assert Event.PostOpenCommand.validate()
 
-        OpenCommand().execute(["knuthwebsite"])
+        await OpenCommand("knuthwebsite").execute()
 
         true_log = [rec for rec in caplog.record_tuples if rec[0] == "cobib.commands.open"]
         outerr = capsys.readouterr()
         true_out = outerr.out.split("\n")
 
         self._assert(true_out, true_log, multi_file=False)
```

### Comparing `cobib-3.5.5/tests/commands/test_redo.py` & `cobib-4.0.0/tests/commands/test_redo.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,41 +3,39 @@
 
 from __future__ import annotations
 
 import contextlib
 import logging
 import os
 import subprocess
-from argparse import Namespace
 from io import StringIO
-from pathlib import Path
 from shutil import rmtree
 from typing import TYPE_CHECKING, Any, Type
 
 import pytest
+from typing_extensions import override
 
 from cobib.commands import AddCommand, RedoCommand, UndoCommand
 from cobib.config import Event, config
 from cobib.database import Database
 
 from .. import get_resource
-from ..tui.tui_test import TUITest
 from .command_test import CommandTest
 
 EXAMPLE_MULTI_FILE_ENTRY_BIB = get_resource("example_multi_file_entry.bib", "commands")
 
 if TYPE_CHECKING:
     import cobib.commands
 
 
-class TestRedoCommand(CommandTest, TUITest):
+class TestRedoCommand(CommandTest):
     """Tests for coBib's RedoCommand."""
 
+    @override
     def get_command(self) -> Type[cobib.commands.base_command.Command]:
-        # noqa: D102
         return RedoCommand
 
     def _assert(self) -> None:
         """Common assertion utility method."""
         assert Database().get("example_multi_file_entry", None) is not None
 
         # get last commit message
@@ -47,91 +45,96 @@
         ) as proc:
             message, _ = proc.communicate()
             # decode it
             split_message = message.decode("utf-8").split("\n")
             # assert subject line
             assert "Redo" in split_message[0]
 
+    @pytest.mark.asyncio
     @pytest.mark.parametrize(
         ["setup", "expected_exit"],
         [
             [{"git": False}, False],
             [{"git": True}, False],
             [{"git": True}, True],
         ],
         indirect=["setup"],
     )
-    def test_command(
+    async def test_command(
         self, setup: Any, expected_exit: bool, caplog: pytest.LogCaptureFixture
     ) -> None:
+        # pylint: disable=invalid-overridden-method
         """Test the command itself.
 
         Args:
             setup: the `tests.commands.command_test.CommandTest.setup` fixture.
             expected_exit: whether to expect an early exit.
             caplog: the built-in pytest fixture.
         """
         git = setup.get("git", False)
 
         if not git:
-            RedoCommand().execute([])
+            RedoCommand().execute()
             for source, level, message in caplog.record_tuples:
                 if ("cobib.commands.redo", logging.ERROR) == (
                     source,
                     level,
                 ) and "git-tracking" in message:
                     break
             else:
                 pytest.fail("No Error logged from RedoCommand.")
         elif expected_exit:
             # Regression test against #65
-            AddCommand().execute(["-b", EXAMPLE_MULTI_FILE_ENTRY_BIB])
+            await AddCommand("-b", EXAMPLE_MULTI_FILE_ENTRY_BIB).execute()
             with pytest.raises(SystemExit):
-                RedoCommand().execute([])
+                RedoCommand().execute()
             for source, level, message in caplog.record_tuples:
                 if ("cobib.commands.redo", logging.WARNING) == (
                     source,
                     level,
                 ) and "Could not find a commit to redo." in message:
                     break
             else:
                 pytest.fail("No Error logged from UndoCommand.")
         else:
-            AddCommand().execute(["-b", EXAMPLE_MULTI_FILE_ENTRY_BIB])
-            UndoCommand().execute([])
+            await AddCommand("-b", EXAMPLE_MULTI_FILE_ENTRY_BIB).execute()
+            UndoCommand().execute()
 
             if Database().get("example_multi_file_entry", None) is not None:
                 pytest.skip("UndoCommand failed. No point in attempting Redo.")
 
-            RedoCommand().execute([])
+            RedoCommand().execute()
 
             self._assert()
 
+    @pytest.mark.asyncio
     @pytest.mark.parametrize(
         ["setup"],
         [
             [{"git": True}],
         ],
         indirect=["setup"],
     )
-    def test_skipping_redone_commits(self, setup: Any, caplog: pytest.LogCaptureFixture) -> None:
+    async def test_skipping_redone_commits(
+        self, setup: Any, caplog: pytest.LogCaptureFixture
+    ) -> None:
         """Test skipping already redone commits.
 
         Args:
             setup: the `tests.commands.command_test.CommandTest.setup` fixture.
             caplog: the built-in pytest fixture.
         """
-        AddCommand().execute(["-b", EXAMPLE_MULTI_FILE_ENTRY_BIB])
-        AddCommand().execute(["-b", get_resource("example_entry.bib")])
-        UndoCommand().execute([])
-        UndoCommand().execute([])
-        RedoCommand().execute([])
+        await AddCommand("-b", EXAMPLE_MULTI_FILE_ENTRY_BIB).execute()
+        await AddCommand("-b", get_resource("example_entry.bib")).execute()
+        UndoCommand().execute()
+        UndoCommand().execute()
+        RedoCommand().execute()
         caplog.clear()
 
-        RedoCommand().execute([])
+        RedoCommand().execute()
         self._assert()
         assert "Storing redone commit" in caplog.record_tuples[4][2]
         assert "Skipping" in caplog.record_tuples[6][2]
 
     @pytest.mark.parametrize(
         ["setup"],
         [
@@ -143,49 +146,50 @@
         """Test warning in case of insufficient setup.
 
         Args:
             setup: the `tests.commands.command_test.CommandTest.setup` fixture.
             caplog: the built-in pytest fixture.
         """
         rmtree(self.COBIB_TEST_DIR_GIT)
-        RedoCommand().execute([])
+        RedoCommand().execute()
         for source, level, message in caplog.record_tuples:
             if ("cobib.commands.redo", logging.ERROR) == (
                 source,
                 level,
             ) and "configured, but not initialized" in message:
                 break
         else:
             pytest.fail("No Error logged from RedoCommand.")
 
+    @pytest.mark.asyncio
     @pytest.mark.parametrize(
         ["setup"],
         [
             [{"git": True}],
         ],
         indirect=["setup"],
     )
     # other variants are already covered by test_command
-    def test_cmdline(
+    async def test_cmdline(
         self, setup: Any, monkeypatch: pytest.MonkeyPatch, caplog: pytest.LogCaptureFixture
     ) -> None:
         """Test the command-line access of the command.
 
         Args:
             setup: the `tests.commands.command_test.CommandTest.setup` fixture.
             monkeypatch: the built-in pytest fixture.
             caplog: the built-in pytest fixture.
         """
-        AddCommand().execute(["-b", EXAMPLE_MULTI_FILE_ENTRY_BIB])
-        UndoCommand().execute([])
+        await AddCommand("-b", EXAMPLE_MULTI_FILE_ENTRY_BIB).execute()
+        UndoCommand().execute()
 
         if Database().get("example_multi_file_entry", None) is not None:
             pytest.skip("UndoCommand failed. No point in attempting Redo.")
 
-        self.run_module(monkeypatch, "main", ["cobib", "redo"])
+        await self.run_module(monkeypatch, "main", ["cobib", "redo"])
 
         self._assert()
 
     # manually overwrite this test because we must enable git integration
     def test_handle_argument_error(self, caplog: pytest.LogCaptureFixture) -> None:
         """Test handling of ArgumentError.
 
@@ -207,75 +211,46 @@
             super().test_handle_argument_error(caplog)
         finally:
             # clean up file system
             rmtree(self.COBIB_TEST_DIR_GIT)
             # clean up config
             config.defaults()
 
-    @pytest.mark.parametrize(
-        ["setup"],
-        [
-            [{"git": True}],
-        ],
-        indirect=["setup"],
-    )
-    def test_tui(self, setup: Any) -> None:
-        """Test the TUI access of the command.
-
-        Args:
-            setup: the `tests.commands.command_test.CommandTest.setup` fixture.
-        """
-
-        def assertion(screen, logs, **kwargs):  # type: ignore
-            assert "example_multi_file_entry" in screen.display[1]
-
-            expected_log = [
-                ("cobib.commands.redo", 10, "Redo command triggered from TUI."),
-                ("cobib.commands.redo", 10, "Starting Redo command."),
-                ("cobib.commands.redo", 10, "Obtaining git log."),
-            ]
-            # we only assert the first three messages because the following ones will contain always
-            # changing commit SHAs
-            assert [log for log in logs if log[0] == "cobib.commands.redo"][0:3] == expected_log
-
-        AddCommand().execute(["-b", EXAMPLE_MULTI_FILE_ENTRY_BIB])
-        UndoCommand().execute([])
-        self.run_tui("r", assertion, {})
-
     @pytest.mark.parametrize("setup", [{"git": True}], indirect=["setup"])
     def test_event_pre_redo_command(self, setup: Any) -> None:
         """Tests the PreRedoCommand event."""
 
         @Event.PreRedoCommand.subscribe
-        def hook(largs: Namespace) -> None:
+        def hook(command: RedoCommand) -> None:
             print("Hello world!")
 
         assert Event.PreRedoCommand.validate()
 
         with contextlib.redirect_stdout(StringIO()) as out:
             with pytest.raises(SystemExit):
-                RedoCommand().execute([])
+                RedoCommand().execute()
 
             assert out.getvalue() == "Hello world!\n"
 
+    @pytest.mark.asyncio
     @pytest.mark.parametrize("setup", [{"git": True}], indirect=["setup"])
-    def test_event_post_redo_command(self, setup: Any) -> None:
+    async def test_event_post_redo_command(self, setup: Any) -> None:
         """Tests the PostRedoCommand event."""
 
         @Event.PostRedoCommand.subscribe
-        def hook(root: Path, sha: str) -> None:
-            print(root)
+        def hook(command: RedoCommand) -> None:
+            print(command.root)
 
         assert Event.PostRedoCommand.validate()
 
         with contextlib.redirect_stdout(StringIO()) as out:
-            AddCommand().execute(["-b", EXAMPLE_MULTI_FILE_ENTRY_BIB])
-            UndoCommand().execute([])
+            await AddCommand("-b", EXAMPLE_MULTI_FILE_ENTRY_BIB).execute()
+            UndoCommand().execute()
 
             if Database().get("example_multi_file_entry", None) is not None:
                 pytest.skip("UndoCommand failed. No point in attempting Redo.")
 
-            RedoCommand().execute([])
+            RedoCommand().execute()
 
             self._assert()
 
             assert out.getvalue() == f"{self.COBIB_TEST_DIR}\n"
```

### Comparing `cobib-3.5.5/tests/config/test_event.py` & `cobib-4.0.0/tests/config/test_event.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
     """Setup debugging configuration.
 
     Yields:
         Access to the local fixture variables.
     """
     config.load(get_resource("debug.py"))
     yield setup
-    config.clear()
     config.defaults()
 
 
 @pytest.mark.parametrize(
     "event",
     [
         Event.PreAddCommand,
```

### Comparing `cobib-3.5.5/tests/database/test_database.py` & `cobib-4.0.0/tests/database/test_database.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import copy
 import logging
 import os
 import tempfile
 from pathlib import Path
 from shutil import copyfile
-from typing import Any, Callable, Generator, Tuple
+from typing import Any, Generator, Tuple
 
 import pytest
 
 from cobib.config import LabelSuffix, config
 from cobib.database import Database, Entry
 
 from .. import get_resource
@@ -124,20 +124,18 @@
         [("_", LabelSuffix.CAPTIAL), "test_A"],
         [("_", LabelSuffix.NUMERIC), "test_1"],
         [(".", LabelSuffix.ALPHA), "test.a"],
         [(".", LabelSuffix.CAPTIAL), "test.A"],
         [(".", LabelSuffix.NUMERIC), "test.1"],
     ],
 )
-def test_database_disambiguate_label(
-    label_suffix: Tuple[str, Callable[[str], str]], expected: str
-) -> None:
+def test_database_disambiguate_label(label_suffix: Tuple[str, LabelSuffix], expected: str) -> None:
     # pylint: disable=invalid-name
     """Test the `cobib.database.Database.disambiguate_label` method."""
-    config.database.format.default_label_format = "test"
+    config.database.format.label_default = "test"
     config.database.format.label_suffix = label_suffix
 
     entries = {"dummy": "test", "test": "no"}
     bib = Database()
     bib.update(entries)  # type: ignore
 
     new_label = Database().disambiguate_label("test", entries["dummy"])  # type: ignore
```

### Comparing `cobib-3.5.5/tests/database/test_entry.py` & `cobib-4.0.0/tests/database/test_entry.py`

 * *Files 3% similar despite different names*

```diff
@@ -186,35 +186,38 @@
         "cobib.database.entry",
         20,
         f"Converting field 'month' of entry 'Cao_2019' from '{month[1]}' to '{expected}'.",
     ) in caplog.record_tuples
 
 
 @pytest.mark.parametrize(
-    ["filter_", "or_"],
+    ["filter_", "or_", "ignore_case"],
     [
-        [{("author", True): ["Cao"]}, False],
-        [{("author", False): ["wrong_author"]}, False],
-        [{("author", True): ["Cao"], ("year", True): ["2019"]}, False],
-        [{("author", True): ["Cao"], ("year", True): ["2020"]}, True],
-        [{("author", True): ["wrong_author"], ("year", True): ["2019"]}, True],
-        [{("author", False): ["wrong_author"], ("year", True): ["2019"]}, False],
-        [{("label", True): [r"\D+_\d+"]}, True],
+        [{("author", True): ["cao"]}, False, True],
+        [{("author", True): ["Cao"]}, False, False],
+        [{("author", False): ["wrong_author"]}, False, False],
+        [{("author", True): ["cao"], ("year", True): ["2019"]}, False, True],
+        [{("author", True): ["Cao"], ("year", True): ["2019"]}, False, False],
+        [{("author", True): ["Cao"], ("year", True): ["2020"]}, True, False],
+        [{("author", True): ["wrong_author"], ("year", True): ["2019"]}, True, False],
+        [{("author", False): ["wrong_author"], ("year", True): ["2019"]}, False, False],
+        [{("label", True): [r"\D+_\d+"]}, True, False],
     ],
 )
-def test_entry_matches(filter_: Dict[Tuple[str, bool], Any], or_: bool) -> None:
+def test_entry_matches(filter_: Dict[Tuple[str, bool], Any], or_: bool, ignore_case: bool) -> None:
     """Test match filter.
 
     Args:
         filter_: a filter as explained be `cobib.database.Entry.matches`.
         or_: whether to use logical `OR` rather than `AND` for filter combination.
+        ignore_case: whether to perform the filter matching case *in*sensitive.
     """
     entry = Entry("Cao_2019", EXAMPLE_ENTRY_DICT)
     # author must match
-    assert entry.matches(filter_, or_=or_)
+    assert entry.matches(filter_, or_=or_, ignore_case=ignore_case)
 
 
 def test_match_with_wrong_key() -> None:
     """Asserts issue #1 is fixed.
 
     When `cobib.database.Entry.matches` is called with a key in the filter which does not exist in
     the entry, the key should be ignored and the function should return normally.
@@ -224,46 +227,46 @@
     assert entry.matches(filter_, or_=False)
 
 
 @pytest.mark.parametrize(
     ["query", "context", "ignore_case", "expected"],
     [
         [
-            "search_query",
+            ["search_query"],
             1,
             False,
             [
                 ["@article{search_dummy,", " abstract = {search_query", "something else"],
                 ["something else", "search_query", "something else"],
             ],
         ],
         [
-            "search_query",
+            ["search_query"],
             1,
             True,
             [
                 ["@article{search_dummy,", " abstract = {search_query", "something else"],
                 ["something else", "Search_Query", "something else"],
                 ["something else", "search_query", "something else"],
                 ["something else", "Search_Query", "something else}"],
             ],
         ],
         [
-            "[sS]earch_[qQ]uery",
+            ["[sS]earch_[qQ]uery"],
             1,
             False,
             [
                 ["@article{search_dummy,", " abstract = {search_query", "something else"],
                 ["something else", "Search_Query", "something else"],
                 ["something else", "search_query", "something else"],
                 ["something else", "Search_Query", "something else}"],
             ],
         ],
         [
-            "search_query",
+            ["search_query"],
             2,
             False,
             [
                 [
                     "@article{search_dummy,",
                     " abstract = {search_query",
                     "something else",
@@ -277,28 +280,28 @@
                     "Search_Query",
                 ],
             ],
         ],
         # the following will look almost identical to the second scenarios because otherwise the
         # next match would be included within the context.
         [
-            "search_query",
+            ["search_query"],
             2,
             True,
             [
                 ["@article{search_dummy,", " abstract = {search_query", "something else"],
                 ["something else", "Search_Query", "something else"],
                 ["something else", "search_query", "something else"],
                 ["something else", "Search_Query", "something else}", "}"],
             ],
         ],
         # what we care about here, is that the second match does not include lines which occur
         # *before* the first match.
         [
-            "search_query",
+            ["search_query"],
             10,
             False,
             [
                 [
                     "@article{search_dummy,",
                     " abstract = {search_query",
                     "something else",
@@ -314,17 +317,30 @@
                     "Search_Query",
                     "something else}",
                     "}",
                     "",
                 ],
             ],
         ],
+        [
+            ["query", "Query"],
+            1,
+            False,
+            [
+                ["@article{search_dummy,", " abstract = {search_query", "something else"],
+                ["something else", "search_query", "something else"],
+                ["something else", "Search_Query", "something else"],
+                ["something else", "Search_Query", "something else}"],
+            ],
+        ],
     ],
 )
-def test_search(query: str, context: int, ignore_case: bool, expected: List[List[str]]) -> None:
+def test_search(
+    query: List[str], context: int, ignore_case: bool, expected: List[List[str]]
+) -> None:
     """Test search method.
 
     Args:
         query: the string to search for.
         context: the number of lines to provide as context for the search results.
         ignore_case: whether to perform a case-insensitive search.
         expected: the expected lines.
@@ -348,15 +364,15 @@
     assert results == expected
 
 
 def test_search_with_file() -> None:
     """Test the `cobib.database.Entry.search` method with associated file."""
     entry = Entry("Cao_2019", EXAMPLE_ENTRY_DICT)
     entry.file = EXAMPLE_YAML_FILE  # type: ignore
-    results = entry.search("Chemical", context=0)
+    results = entry.search(["Chemical"], context=0)
     expected = [
         [" journal = {Chemical Reviews},"],
         [" publisher = {American Chemical Society ({ACS})},"],
         ["journal: Chemical Reviews"],
         ["publisher: American Chemical Society ({ACS})"],
     ]
     for res, exp in zip(results, expected):
@@ -367,15 +383,15 @@
     """Test the `cobib.database.Entry.search` method with a missing file.
 
     Args:
         caplog: the built-in pytest fixture.
     """
     entry = Entry("Cao_2019", EXAMPLE_ENTRY_DICT)
     entry.file = "some_non_existent_file.txt"  # type: ignore
-    _ = entry.search("Chemical", context=0)
+    _ = entry.search(["Chemical"], context=0)
     for source, level, message in caplog.record_tuples:
         if level != 30 or source != "cobib.database.entry":
             continue
         if message.startswith("The associated file") and message.endswith(
             "of entry Cao_2019 does not exist!"
         ):
             break
```

### Comparing `cobib-3.5.5/tests/example_entry.bib` & `cobib-4.0.0/tests/example_entry.bib`

 * *Files identical despite different names*

### Comparing `cobib-3.5.5/tests/example_entry.yaml` & `cobib-4.0.0/tests/example_entry.yaml`

 * *Files identical despite different names*

### Comparing `cobib-3.5.5/tests/example_literature.bib` & `cobib-4.0.0/tests/example_literature.bib`

 * *Files identical despite different names*

### Comparing `cobib-3.5.5/tests/example_literature.yaml` & `cobib-4.0.0/tests/example_literature.yaml`

 * *Files identical despite different names*

### Comparing `cobib-3.5.5/tests/importers/test_zotero.py` & `cobib-4.0.0/tests/importers/test_zotero.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 # pylint: disable=unused-argument
 
 import json
 import logging
 import tempfile
 from itertools import zip_longest
 from pathlib import Path
-from typing import Dict, List, Optional, Tuple
+from typing import Dict, List
 
 import pytest
+from typing_extensions import override
 
 from cobib.config import Event, config
 from cobib.database import Entry
 from cobib.importers import ZoteroImporter
 from cobib.parsers import YAMLParser
 
 from .. import get_resource
@@ -20,17 +21,17 @@
 
 EXPECTED_DATABASE = get_resource("zotero_database.yaml", "importers")
 
 
 class MockZoteroImporter(ZoteroImporter):
     """This class mocks the `ZoteroImporter` by providing fake OAuth authentication tokens."""
 
+    @override
     @staticmethod
     def _get_authentication_tokens(no_cache: bool = False) -> Dict[str, str]:
-        # noqa: D102
         return {
             # NOTE: we are relying on the publicly accessible user `cobib` for testing purposes
             "UserID": "8608002",
         }
 
 
 class TestZoteroImporter(ImporterTest):
@@ -52,78 +53,87 @@
 
         with open(EXPECTED_DATABASE, "r", encoding="utf-8") as expected:
             for line, truth in zip_longest(
                 imported_database.splitlines(keepends=True), expected.readlines()
             ):
                 assert line == truth
 
-    def test_fetch(self) -> None:
+    @pytest.mark.asyncio
+    async def test_fetch(self) -> None:
         """Test fetching entries from the Zotero API."""
-        importer = MockZoteroImporter()
+        importer = MockZoteroImporter(skip_download=False)
         # NOTE: even though attachments are not accessible via public libraries, we explicitly skip
         # downloading them, just to be sure.
-        imported_entries = importer.fetch([], skip_download=False)
+        imported_entries = await importer.fetch()
 
         self._assert_results(imported_entries)
 
-    def test_fetch_custom_user_id(self) -> None:
+    @pytest.mark.asyncio
+    async def test_fetch_custom_user_id(self) -> None:
         """Test fetching with custom user ID."""
-        imported_entries = ZoteroImporter().fetch(["--user-id", "8608002", "--no-cache"])
+        imported_entries = await ZoteroImporter("--user-id", "8608002", "--no-cache").fetch()
         self._assert_results(imported_entries)
 
-    def test_cache(self) -> None:
+    @pytest.mark.asyncio
+    async def test_cache(self) -> None:
         """Test caching behavior."""
         try:
             config.logging.cache = str(Path(tempfile.gettempdir()) / "cache")
-            imported_entries = ZoteroImporter().fetch(["--user-id", "8608002"], skip_download=True)
+            imported_entries = await ZoteroImporter(
+                "--user-id", "8608002", skip_download=True
+            ).fetch()
             self._assert_results(imported_entries)
 
             with open(config.logging.cache, "r", encoding="utf-8") as cache:
                 cached_data = json.load(cache)
                 assert "Zotero" in cached_data.keys()
                 assert "UserID" in cached_data["Zotero"].keys()
                 assert cached_data["Zotero"]["UserID"] == "8608002"
         finally:
             config.defaults()
 
-    def test_handle_argument_error(self, caplog: pytest.LogCaptureFixture) -> None:
+    @pytest.mark.asyncio
+    async def test_handle_argument_error(self, caplog: pytest.LogCaptureFixture) -> None:
         """Test handling of ArgumentError.
 
         Args:
             caplog: the built-in pytest fixture.
         """
-        ZoteroImporter().fetch(["--dummy"])
+        try:
+            await ZoteroImporter("--dummy").fetch()
+        except SystemExit:
+            pass
         for source, level, message in caplog.record_tuples:
-            if ("cobib.importers.zotero", logging.ERROR) == (
+            if ("cobib.importers.base_importer", logging.ERROR) == (
                 source,
                 level,
             ) and "Error: zotero: error:" in message:
                 break
         else:
             pytest.fail("No Error logged from ArgumentParser.")
 
-    def test_event_pre_zotero_import(self) -> None:
+    @pytest.mark.asyncio
+    async def test_event_pre_zotero_import(self) -> None:
         """Tests the PreZoteroImport event."""
 
         @Event.PreZoteroImport.subscribe
-        def hook(
-            protected_url: str, authentication: Dict[str, str]
-        ) -> Optional[Tuple[str, Dict[str, str]]]:
-            return (protected_url.replace("test", "8608002"), {})
+        def hook(importer: ZoteroImporter) -> None:
+            importer.protected_url = importer.protected_url.replace("test", "8608002")
 
         assert Event.PreZoteroImport.validate()
 
-        imported_entries = ZoteroImporter().fetch(["--user-id", "test", "--no-cache"])
+        imported_entries = await ZoteroImporter("--user-id", "test", "--no-cache").fetch()
 
         self._assert_results(imported_entries)
 
-    def test_event_post_zotero_import(self) -> None:
+    @pytest.mark.asyncio
+    async def test_event_post_zotero_import(self) -> None:
         """Tests the PostZoteroImport event."""
 
         @Event.PostZoteroImport.subscribe
-        def hook(imported_entries: List[Entry]) -> Optional[List[Entry]]:
-            return []
+        def hook(importer: ZoteroImporter) -> None:
+            importer.imported_entries = []
 
         assert Event.PostZoteroImport.validate()
 
-        imported_entries = MockZoteroImporter().fetch(["--no-cache"])
+        imported_entries = await MockZoteroImporter("--no-cache").fetch()
         assert imported_entries == []
```

### Comparing `cobib-3.5.5/tests/importers/zotero_database.yaml` & `cobib-4.0.0/tests/importers/zotero_database.yaml`

 * *Files identical despite different names*

### Comparing `cobib-3.5.5/tests/parsers/parser_test.py` & `cobib-4.0.0/tests/parsers/parser_test.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.5/tests/parsers/test_arxiv.py` & `cobib-4.0.0/tests/parsers/test_arxiv.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
             "An Exception occurred while trying to query the arXiv ID: 1812.09976.",
         ) in caplog.record_tuples:
             pytest.skip("The requests API encountered an error. Skipping test.")
 
         entry = list(entries.values())[0]
         assert_default_test_entry(entry)
 
-    # regression test for https://gitlab.com/mrossinek/cobib/-/issues/57
+    # regression test for https://gitlab.com/cobib/cobib/-/issues/57
     def test_invalid_arxiv_id(self) -> None:
         """Test parsing an invalid arXiv ID."""
         entries = ArxivParser().parse("10.1021/acs.chemrev.8b00803")
         assert not entries
         assert entries == {}  # pylint: disable=C1803
 
     def test_arxiv_without_doi(self) -> None:
```

### Comparing `cobib-3.5.5/tests/parsers/test_bibtex.py` & `cobib-4.0.0/tests/parsers/test_bibtex.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.5/tests/parsers/test_doi.py` & `cobib-4.0.0/tests/parsers/test_doi.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.5/tests/parsers/test_isbn.py` & `cobib-4.0.0/tests/parsers/test_isbn.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             s == "cobib.parsers.isbn" and t == logging.ERROR for s, t, _ in caplog.record_tuples
         ):
             pytest.skip("The requests API encountered an error. Skipping test.")
 
         entry = list(entries.values())[0]
         assert_default_test_entry(entry)
 
-    # regression test for https://gitlab.com/mrossinek/cobib/-/issues/53
+    # regression test for https://gitlab.com/cobib/cobib/-/issues/53
     def test_from_empty_isbn(self, caplog: pytest.LogCaptureFixture) -> None:
         """Test parsing an empty ISBN.
 
         Args:
             caplog: the built-in pytest fixture.
         """
         entries = ISBNParser().parse("3860704443")
```

### Comparing `cobib-3.5.5/tests/parsers/test_url.py` & `cobib-4.0.0/tests/parsers/test_url.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
         assertion(entry)
 
     def test_invalid_url(self) -> None:
         """Test parsing an invalid URL."""
         entries = URLParser().parse("https://github.com/")
         assert not entries
-        assert entries == {}  # pylint: disable=C1803
+        assert entries == {}
 
     def test_dump(self, caplog: pytest.LogCaptureFixture) -> None:
         """Test dumping.
 
         Args:
             caplog: the built-in pytest fixture.
         """
```

### Comparing `cobib-3.5.5/tests/parsers/test_yaml.py` & `cobib-4.0.0/tests/parsers/test_yaml.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.5/tests/test_main.py` & `cobib-4.0.0/tests/test_main.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,110 +24,110 @@
 
     @staticmethod
     @pytest.fixture
     def setup() -> None:
         """Load testing config."""
         config.load(get_resource("debug.py"))
 
-    def test_version(
+    @pytest.mark.asyncio
+    async def test_version(
         self, setup: Any, monkeypatch: pytest.MonkeyPatch, capsys: pytest.CaptureFixture[str]
     ) -> None:
         """Tests the version parser argument.
 
         Args:
             setup: a local pytest fixture.
             monkeypatch: the built-in pytest fixture.
             capsys: the built-in pytest fixture.
         """
         with pytest.raises(SystemExit):
-            self.run_module(monkeypatch, "main", ["cobib", "--version"])
+            await self.run_module(monkeypatch, "main", ["cobib", "--version"])
         # pylint: disable=import-outside-toplevel
         from cobib import __version__
 
         assert capsys.readouterr().out.strip() == f"coBib v{__version__}"
 
+    @pytest.mark.asyncio
     @pytest.mark.parametrize(
-        ["main", "args"],
+        "args",
         [
-            ["main", ["open", "einstein"]],
-            ["helper_main", ["_example_config"]],
+            ["open", "einstein"],
+            ["_example_config"],
         ],
     )
     @pytest.mark.parametrize(
         ["verbosity_arg", "level"],
         [
             ["-v", logging.INFO],
             ["-vv", logging.DEBUG],
         ],
     )
-    def test_verbosity(
+    async def test_verbosity(
         self,
         setup: Any,
         monkeypatch: pytest.MonkeyPatch,
-        main: str,
         args: List[str],
         verbosity_arg: str,
         level: int,
     ) -> None:
         """Tests the verbosity parser argument.
 
         Args:
             setup: a local pytest fixture.
             monkeypatch: the built-in pytest fixture.
-            main: the name of the `main` executable of the module to run.
             args: the list of values with which to monkeypatch `sys.argv`.
             verbosity_arg: the value of the verbosity argument.
             level: the level of the verbosity argument.
         """
         # we choose the open command as an arbitrary choice which has minimal side effects
         args = ["cobib"] + args
         if verbosity_arg:
             args.insert(1, verbosity_arg)
-        self.run_module(monkeypatch, main, args)
+        await self.run_module(monkeypatch, "main", args)
         assert logging.getLogger().getEffectiveLevel() == logging.DEBUG
         assert logging.getLogger().handlers[-1].level == level
 
+    @pytest.mark.asyncio
     @pytest.mark.parametrize(
-        ["main", "args"],
+        "args",
         [
-            ["main", ["open", "einstein"]],
-            ["helper_main", ["_example_config"]],
+            ["open", "einstein"],
+            ["_example_config"],
         ],
     )
-    def test_logfile(
-        self, setup: Any, monkeypatch: pytest.MonkeyPatch, main: str, args: List[str]
+    async def test_logfile(
+        self, setup: Any, monkeypatch: pytest.MonkeyPatch, args: List[str]
     ) -> None:
         """Tests the logfile parser argument.
 
         Args:
             setup: a local pytest fixture.
             monkeypatch: the built-in pytest fixture.
-            main: the name of the `main` executable of the module to run.
             args: the list of values with which to monkeypatch `sys.argv`.
         """
         logfile = str(Path(tempfile.gettempdir()) / "cobib_test_logging.log")
         # we choose the open command as an arbitrary choice which has minimal side effects
-        self.run_module(monkeypatch, main, ["cobib", "-l", logfile] + args)
+        await self.run_module(monkeypatch, "main", ["cobib", "-l", logfile] + args)
         try:
             assert isinstance(logging.getLogger().handlers[-1], logging.FileHandler)
             assert logging.getLogger().handlers[-1].baseFilename == logfile  # type: ignore
         finally:
             os.remove(logfile)
 
+    @pytest.mark.asyncio
     @pytest.mark.parametrize(
-        ["main", "args"],
+        "args",
         [
-            ["main", ["open", "einstein"]],
-            ["helper_main", ["_example_config"]],
+            ["open", "einstein"],
+            ["_example_config"],
         ],
     )
-    def test_configfile(self, monkeypatch: pytest.MonkeyPatch, main: str, args: List[str]) -> None:
+    async def test_configfile(self, monkeypatch: pytest.MonkeyPatch, args: List[str]) -> None:
         """Tests the configfile parser argument.
 
         Args:
             monkeypatch: the built-in pytest fixture.
-            main: the name of the `main` executable of the module to run.
             args: the list of values with which to monkeypatch `sys.argv`.
         """
         # we choose the open command as an arbitrary choice which has minimal side effects
-        self.run_module(monkeypatch, main, ["cobib", "-c", get_resource("debug.py")] + args)
+        await self.run_module(monkeypatch, "main", ["cobib", "-c", get_resource("debug.py")] + args)
         assert config.database.file == get_resource("example_literature.yaml")
```

### Comparing `cobib-3.5.5/tests/utils/test_file_downloader.py` & `cobib-4.0.0/tests/utils/test_file_downloader.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,89 +37,83 @@
 def test_downloader_singleton() -> None:
     """Test the FileDownloader is a Singleton."""
     f_d = FileDownloader()
     f_d2 = FileDownloader()
     assert f_d is f_d2
 
 
-def test_set_logger() -> None:
-    """Test the FileDownloader.set_logger method."""
-    f_d = FileDownloader()
-    logger = lambda text: f"test: {text}"  # pylint: disable=unnecessary-lambda-assignment
-    f_d.set_logger(logger)  # type: ignore
-    # pylint: disable=protected-access
-    assert FileDownloader._logger("") == "test: "  # type: ignore
-
-
-def test_download(monkeypatch: pytest.MonkeyPatch) -> None:
+@pytest.mark.asyncio
+async def test_download(monkeypatch: pytest.MonkeyPatch) -> None:
     """Test the FileDownloader.download method.
 
     Args:
         monkeypatch: the built-in pytest fixture.
     """
     with tempfile.TemporaryDirectory() as tmpdirname:
         try:
             # ensure file does not exist yet
             remove(tmpdirname + "/dummy.pdf")
         except FileNotFoundError:
             pass
         # disable the PDF assertion method
         monkeypatch.setattr(FileDownloader, "_assert_pdf", lambda _: True)
-        path = FileDownloader().download(
-            "https://gitlab.com/mrossinek/cobib/-/raw/master/tests/utils/__init__.py",
+        path = await FileDownloader().download(
+            "https://gitlab.com/cobib/cobib/-/raw/master/tests/utils/__init__.py",
             "dummy",
             tmpdirname,
         )
         if path is None:
             pytest.skip("Likely, a requests error occured.")
         with open(get_resource("__init__.py", "utils"), "r", encoding="utf-8") as expected:
             with open(tmpdirname + "/dummy.pdf", "r", encoding="utf-8") as truth:
                 assert expected.read() == truth.read()
 
 
+@pytest.mark.asyncio
 @pytest.mark.parametrize(
     ["setup_remove_content_length"],
     [
         [{"enable": False}],
         [{"enable": True}],
     ],
     indirect=["setup_remove_content_length"],
 )
 # pylint: disable=unused-argument,redefined-outer-name
-def test_skip_download_if_no_pdf(setup_remove_content_length: Any) -> None:
+async def test_skip_download_if_no_pdf(setup_remove_content_length: Any) -> None:
     """Test that download is skipped when file is not a PDF.
 
     Args:
         setup_remove_content_length: a custom fixture.
     """
     with tempfile.TemporaryDirectory() as tmpdirname:
         assert (
-            FileDownloader().download(
-                "https://gitlab.com/mrossinek/cobib/-/raw/master/tests/utils/__init__.py",
+            await FileDownloader().download(
+                "https://gitlab.com/cobib/cobib/-/raw/master/tests/utils/__init__.py",
                 "dummy",
                 tmpdirname,
             )
             is None
         )
 
 
+@pytest.mark.asyncio
 @pytest.mark.parametrize("overwrite", [False, True])
-def test_skip_download_if_exists(caplog: pytest.LogCaptureFixture, overwrite: bool) -> None:
+async def test_skip_download_if_exists(caplog: pytest.LogCaptureFixture, overwrite: bool) -> None:
     """Test that download is skipped when file already exists.
 
     Args:
         caplog: the built-in pytest fixture.
         overwrite: whether or not to overwrite the existing file.
     """
     with tempfile.TemporaryDirectory() as tmpdirname:
         open(  # pylint: disable=consider-using-with
             tmpdirname + "/dummy.pdf", "w", encoding="utf-8"
         ).close()
-        FileDownloader().download(
-            "https://gitlab.com/mrossinek/cobib/-/raw/master/tests/utils/__init__.py",
+        await FileDownloader().download(
+            "https://gitlab.com/cobib/cobib/-/raw/master/tests/utils/__init__.py",
             "dummy",
             folder=tmpdirname,
             overwrite=overwrite,
         )
         for mod, lvl, msg in caplog.record_tuples:
             if (
                 mod == "cobib.utils.file_downloader"
@@ -129,24 +123,25 @@
                 break
         else:
             assert overwrite, "This statement should only be reached when overwrite is enabled!"
             return
         assert not overwrite, "This statement should only be reached when overwrite is disabled!"
 
 
+@pytest.mark.asyncio
 @pytest.mark.parametrize(
     ["setup_remove_content_length"],
     [
         [{"enable": False}],
         [{"enable": True}],
     ],
     indirect=["setup_remove_content_length"],
 )
 # pylint: disable=unused-argument,redefined-outer-name
-def test_download_with_url_map(setup_remove_content_length: Any) -> None:
+async def test_download_with_url_map(setup_remove_content_length: Any) -> None:
     """Test the `config.utils.file_downloader.url_map` usage.
 
     We use a Quantum Journal article because they are open-source and, thus, do not require a Proxy
     to get access to.
 
     Args:
         setup_remove_content_length: a custom fixture.
@@ -155,53 +150,55 @@
         config.load(get_resource("debug.py"))
         with tempfile.TemporaryDirectory() as tmpdirname:
             try:
                 # ensure file does not exist yet
                 remove(tmpdirname + "/dummy.pdf")
             except FileNotFoundError:
                 pass
-            path = FileDownloader().download(
+            path = await FileDownloader().download(
                 "https://quantum-journal.org/papers/q-2021-06-17-479/",
                 "dummy",
                 tmpdirname,
             )
             if path is None:
                 pytest.skip("Likely, a requests error occured.")
             assert path.path.exists()
             with open(path.path, "rb") as file:
                 assert file.read().startswith(bytes("%PDF", "utf-8"))
     finally:
         config.defaults()
 
 
-def test_gracefully_fail_download(monkeypatch: pytest.MonkeyPatch) -> None:
+@pytest.mark.asyncio
+async def test_gracefully_fail_download(monkeypatch: pytest.MonkeyPatch) -> None:
     """Test gracefully failing downloads.
 
     Args:
         monkeypatch: the built-in pytest fixture.
     """
 
     def raise_exception(*args, **kwargs):  # type: ignore
         """Mock function to raise an Exception."""
         raise requests.exceptions.RequestException()
 
     monkeypatch.setattr(requests, "get", raise_exception)
 
     with tempfile.TemporaryDirectory() as tmpdirname:
         assert (
-            FileDownloader().download(
+            await FileDownloader().download(
                 "https://quantum-journal.org/papers/q-2021-06-17-479/",
                 "dummy",
                 tmpdirname,
             )
             is None
         )
 
 
-def test_event_pre_download(monkeypatch: pytest.MonkeyPatch) -> None:
+@pytest.mark.asyncio
+async def test_event_pre_download(monkeypatch: pytest.MonkeyPatch) -> None:
     """Test the PreFileDownload event.
 
     Args:
         monkeypatch: the built-in pytest fixture.
     """
 
     @Event.PreFileDownload.subscribe
@@ -217,27 +214,28 @@
         try:
             # ensure file does not exist yet
             remove(tmpdirname + "/test.pdf")
         except FileNotFoundError:
             pass
         # disable the PDF assertion method
         monkeypatch.setattr(FileDownloader, "_assert_pdf", lambda _: True)
-        path = FileDownloader().download(
-            "https://gitlab.com/mrossinek/cobib/-/raw/master/tests/utils/__init__.py",
+        path = await FileDownloader().download(
+            "https://gitlab.com/cobib/cobib/-/raw/master/tests/utils/__init__.py",
             "dummy",
             tmpdirname,
         )
         if path is None:
             pytest.skip("Likely, a requests error occured.")
         with open(get_resource("__init__.py", "utils"), "r", encoding="utf-8") as expected:
             with open(tmpdirname + "/test.pdf", "r", encoding="utf-8") as truth:
                 assert expected.read() == truth.read()
 
 
-def test_event_post_download(monkeypatch: pytest.MonkeyPatch) -> None:
+@pytest.mark.asyncio
+async def test_event_post_download(monkeypatch: pytest.MonkeyPatch) -> None:
     """Test the PostFileDownload event.
 
     Args:
         monkeypatch: the built-in pytest fixture.
     """
 
     @Event.PostFileDownload.subscribe
@@ -250,16 +248,16 @@
         try:
             # ensure file does not exist yet
             remove(tmpdirname + "/test.pdf")
         except FileNotFoundError:
             pass
         # disable the PDF assertion method
         monkeypatch.setattr(FileDownloader, "_assert_pdf", lambda _: True)
-        path = FileDownloader().download(
-            "https://gitlab.com/mrossinek/cobib/-/raw/master/tests/utils/__init__.py",
+        path = await FileDownloader().download(
+            "https://gitlab.com/cobib/cobib/-/raw/master/tests/utils/__init__.py",
             "dummy",
             tmpdirname,
         )
         if path is None:
             pytest.skip("Likely, a requests error occured.")
         with open(get_resource("__init__.py", "utils"), "r", encoding="utf-8") as expected:
             with open(tmpdirname + "/test.pdf", "r", encoding="utf-8") as truth:
```

### Comparing `cobib-3.5.5/tests/utils/test_journal_abbreviations.py` & `cobib-4.0.0/tests/utils/test_journal_abbreviations.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.5/tests/utils/test_logging.py` & `cobib-4.0.0/tests/utils/test_logging.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 """Tests for coBib's logging helper functions."""
 
 import logging
-import re
 import tempfile
 from pathlib import Path
 from typing import Optional
 
 import pytest
+from rich.console import Group
+from rich.markdown import Markdown
+from rich.panel import Panel
+from rich.text import Text
 
 from cobib.utils.logging import get_file_handler, get_stream_handler, print_changelog
 
-from .. import MockStdin, get_resource
+from .. import get_resource
 
 
 def test_get_stream_handler() -> None:
     """Test stream logging configuration."""
     handler = get_stream_handler()
     assert handler.level == 30
     assert isinstance(handler, logging.StreamHandler)
@@ -26,61 +29,54 @@
     assert handler.level == 20
     assert isinstance(handler, logging.FileHandler)
 
 
 @pytest.mark.parametrize("cached_version", [None, False, "", "0.1", "0.2"])
 def test_print_changelog(
     cached_version: Optional[str],
-    monkeypatch: pytest.MonkeyPatch,
-    capsys: pytest.CaptureFixture[str],
 ) -> None:
     """Test printing of the latest changelog section.
 
     Args:
         cached_version: the cached version to test against.
-        monkeypatch: the built-in pytest fixture.
-        capsys: the built-in pytest fixture.
     """
-    monkeypatch.setattr("sys.stdin", MockStdin())
-    ansi_regex = re.compile(r"(\x1b\[(\d+)+m)")
     if cached_version is None:
-        print_changelog("0.2", None)
-        assert capsys.readouterr().out == ""
+        panel = print_changelog("0.2", None)
+        assert panel is None
     else:
         with tempfile.NamedTemporaryFile("w") as file:
             path = Path(file.name)
             if not cached_version:
                 file.close()
             else:
                 file.write(cached_version)
                 file.flush()
-            print_changelog("0.2", str(path))
+            panel = print_changelog("0.2", str(path))
         # ensure we do not leave a temporary file behind
         if path.exists():
             path.unlink()
-        captured = ansi_regex.sub("", capsys.readouterr().out).splitlines()
         if cached_version == "0.2":
-            assert captured == []
-        with open(
-            get_resource("expected_changelog_printing.txt", "utils"), "r", encoding="utf-8"
-        ) as expected:
-            expected_lines = expected.read().splitlines()
-            for true, exp in zip(captured[:-10], expected_lines):
-                assert true == exp
-            for true, exp in zip(captured[-2:], expected_lines[-2:]):
-                assert true == exp
+            assert panel is None
+        else:
+            assert isinstance(panel, Panel)
+            assert isinstance(panel.renderable, Group)
+            assert isinstance(panel.renderable.renderables[0], Text)
+            assert isinstance(panel.renderable.renderables[1], Markdown)
+            with open(
+                get_resource("expected_changelog_printing.md", "utils"), "r", encoding="utf-8"
+            ) as expected:
+                expected_lines = expected.read().splitlines()
+                for true, exp in zip(
+                    panel.renderable.renderables[1].markup.splitlines(), expected_lines
+                ):
+                    assert true == exp
 
 
-def test_safe_cache_access(monkeypatch: pytest.MonkeyPatch) -> None:
-    """Regression test against #94.
-
-    Args:
-        monkeypatch: the built-in pytest fixture.
-    """
-    monkeypatch.setattr("sys.stdin", MockStdin())
+def test_safe_cache_access() -> None:
+    """Regression test against #94."""
     # create an empty temporary directory
     tmp_dir = tempfile.mkdtemp()
     # use a path which surely does not exist
     tmp_cache_file = Path(tmp_dir) / "cache/version"
     try:
         # try to read the version from a file whose parent directory does not exist
         print_changelog("0.2", str(tmp_cache_file))
```

### Comparing `cobib-3.5.5/tests/utils/test_rel_path.py` & `cobib-4.0.0/tests/utils/test_rel_path.py`

 * *Files identical despite different names*

### Comparing `cobib-3.5.5/tests/utils/test_shell_helper.py` & `cobib-4.0.0/tests/utils/test_shell_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,41 +52,41 @@
         if isinstance(self.EXPECTED, list):
             assert out.split() == self.EXPECTED
         elif isinstance(self.EXPECTED, set):
             assert set(out.split()) == self.EXPECTED
 
     def test_method(self) -> None:
         """Test the shell_helper method itself."""
-        args: List[str] = []
-        cmds = getattr(shell_helper, str(self.COMMAND))(args)
+        cmds = getattr(shell_helper, str(self.COMMAND))()
         self._assert("\n".join(cmds))
 
-    def test_cmdline(
+    @pytest.mark.asyncio
+    async def test_cmdline(
         self, monkeypatch: pytest.MonkeyPatch, capsys: pytest.CaptureFixture[str]
     ) -> None:
         """Test the command-line access of the helper method.
 
         Args:
             monkeypatch: the built-in pytest fixture.
             capsys: the built-in pytest fixture.
         """
-        CmdLineTest.run_module(monkeypatch, "helper_main", ["cobib", f"_{self.COMMAND}"])
+        await CmdLineTest.run_module(monkeypatch, "main", ["cobib", f"_{self.COMMAND}"])
         self._assert(capsys.readouterr().out)
 
-    def test_cmdline_via_main(
+    @pytest.mark.asyncio
+    async def test_cmdline_via_main(
         self, monkeypatch: pytest.MonkeyPatch, capsys: pytest.CaptureFixture[str]
     ) -> None:
         """Test the command-line access of the helper method via the main method.
 
         Args:
             monkeypatch: the built-in pytest fixture.
             capsys: the built-in pytest fixture.
         """
-        with pytest.raises(SystemExit):
-            CmdLineTest.run_module(monkeypatch, "main", ["cobib", f"_{self.COMMAND}"])
+        await CmdLineTest.run_module(monkeypatch, "main", ["cobib", f"_{self.COMMAND}"])
         self._assert(capsys.readouterr().out)
 
 
 class TestListCommands(ShellHelperTest):
     """Tests for the shell helper which lists the available commands."""
 
     @staticmethod
@@ -193,16 +193,15 @@
         for msg, truth in zip_longest(out.split("\n"), self.EXPECTED):
             if msg.strip() and truth:
                 assert msg == truth
 
     def test_no_lint_warnings(self) -> None:
         """Test the case of no raised lint warnings."""
         config.load(get_resource("debug.py"))
-        args: List[str] = []
-        lint_messages = shell_helper.lint_database(args)
+        lint_messages = shell_helper.lint_database()
         for msg, exp in zip_longest(
             lint_messages, ["Congratulations! Your database triggers no lint messages."]
         ):
             if msg.strip() and exp:
                 assert msg == exp
 
     @pytest.mark.parametrize("git", [False, True])
@@ -230,16 +229,15 @@
                 "git add -- database.yaml",
                 "git commit --no-gpg-sign --quiet --message 'Initial commit'",
             ]
             os.system("; ".join(commands))
 
         try:
             # apply linting with formatting and check for the expected lint messages
-            args: List[str] = ["--format"]
-            pre_lint_messages = shell_helper.lint_database(args)
+            pre_lint_messages = shell_helper.lint_database("--format")
             expected_messages = [
                 "The following lint messages have successfully been resolved:"
             ] + self.EXPECTED
             for msg, truth in zip_longest(pre_lint_messages, expected_messages):
                 if msg.strip() and truth:
                     assert msg == truth.replace(str(TestLintDatabase.REL_PATH), str(database_file))
 
@@ -270,15 +268,15 @@
                     split_msg = message.decode("utf-8").split("\n")
                     if split_msg is None:
                         return
                     # assert subject line
                     assert "Auto-commit: LintCommand" in split_msg[0]
 
             # recheck linting and assert no lint messages
-            post_lint_messages = shell_helper.lint_database([])
+            post_lint_messages = shell_helper.lint_database()
             for msg, exp in zip_longest(
                 post_lint_messages, ["Congratulations! Your database triggers no lint messages."]
             ):
                 if msg.strip() and exp:
                     assert msg == exp
 
         finally:
@@ -343,15 +341,15 @@
                 "git add -- database.yaml",
                 "git commit --no-gpg-sign --quiet --message 'Initial commit'",
             ]
             os.system("; ".join(commands))
 
         try:
             # apply label unification
-            shell_helper.unify_labels(["--apply"])
+            shell_helper.unify_labels("--apply")
 
             # assert unified database
             with open(database_file.path, "r", encoding="utf-8") as file:
                 with open(
                     RelPath(get_resource("unified_database.yaml", "utils")).path,
                     "r",
                     encoding="utf-8",
```

### Comparing `cobib-3.5.5/tests/utils/unified_database.yaml` & `cobib-4.0.0/tests/utils/unified_database.yaml`

 * *Files identical despite different names*

### Comparing `cobib-3.5.5/tests/utils/unifying_database.yaml` & `cobib-4.0.0/tests/utils/unifying_database.yaml`

 * *Files identical despite different names*

### Comparing `cobib-3.5.5/tox.ini` & `cobib-4.0.0/tox.ini`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 [tox]
-envlist = py3.7, py3.8, py3.9, py3.10, coverage, lint, docs
+envlist = py3.8, py3.9, py3.10, py3.11, coverage, lint, docs
 
 [testenv]
 deps =
     -r{toxinidir}/requirements.txt
-    !lint,!docs: pyte
-    !lint,!docs: pytest
+    -r{toxinidir}/dev-requirements.txt
 passenv =
     HOME
     TERM
     GIT_AUTHOR_NAME
     GIT_AUTHOR_EMAIL
 setenv =
     TMPDIR = {envdir}/tmp
@@ -18,50 +17,33 @@
 commands =
     pytest --basetemp="{envtmpdir}" --junitxml=report-{envname}.xml {posargs}
 
 [testenv:coverage]
 usedevelop = true
 basepython = python3
 changedir = {toxinidir}
-deps =
-    {[testenv]deps}
-    coverage<7
-    pytest-cov
 commands =
     pytest --cov --cov-config={toxinidir}/.coveragerc tests/
     coverage xml
     coverage html
 
 [testenv:lint]
 skip_install = true
 ignore_errors = true
 basepython = python3
 changedir = {toxinidir}
-deps =
-    {[testenv]deps}
-    black
-    isort
-    lxml
-    mypy
-    pydocstyle
-    pyenchant
-    pylint
 commands =
     black --check src tests
     isort --check src tests
     mypy --html-report htmlmypy --cobertura-xml . --strict src tests
     pydocstyle --config=.pydocstylerc src tests
     pylint -rn src tests --rcfile=.pylintrc
     pylint -rn src tests --disable=all --enable=spelling --spelling-dict=en_US \
         --spelling-private-dict-file=.pylintdict
 
 [testenv:docs]
 skip_install = true
 basepython = python3
 changedir = {toxinidir}
 allowlist_externals = sed
-deps =
-    {[testenv]deps}
-    pdoc
 commands =
-    pdoc -d google -e cobib=https://gitlab.com/mrossinek/cobib/-/blob/master/src/cobib/ -t html -o docs src/cobib tests
-    sed -i "s/<details>/<details open>/" docs/cobib/config/example.html
+    pdoc -d google -e cobib=https://gitlab.com/cobib/cobib/-/blob/master/src/cobib/ -t html -o docs src/cobib tests
```

