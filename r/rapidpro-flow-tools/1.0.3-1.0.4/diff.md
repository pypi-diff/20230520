# Comparing `tmp/rapidpro_flow_tools-1.0.3.tar.gz` & `tmp/rapidpro_flow_tools-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapidpro_flow_tools-1.0.3.tar", last modified: Fri May 19 22:12:32 2023, max compression
+gzip compressed data, was "rapidpro_flow_tools-1.0.4.tar", last modified: Fri May 19 22:17:32 2023, max compression
```

## Comparing `rapidpro_flow_tools-1.0.3.tar` & `rapidpro_flow_tools-1.0.4.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 22:12:32.609087 rapidpro_flow_tools-1.0.3/
--rw-rw-rw-   0        0        0    27030 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     3518 2023-05-19 22:12:32.608080 rapidpro_flow_tools-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2906 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 22:12:32.501200 rapidpro_flow_tools-1.0.3/parsers/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.3/parsers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 22:12:32.508423 rapidpro_flow_tools-1.0.3/parsers/common/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.3/parsers/common/__init__.py
--rw-rw-rw-   0        0        0     4152 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.3/parsers/common/cellparser.py
--rw-rw-rw-   0        0        0     3205 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.3/parsers/common/rowdatasheet.py
--rw-rw-rw-   0        0        0    15945 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.3/parsers/common/rowparser.py
--rw-rw-rw-   0        0        0     1849 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.3/parsers/common/sheetparser.py
-drwxrwxrwx   0        0        0        0 2023-05-19 22:12:32.530005 rapidpro_flow_tools-1.0.3/parsers/common/tests/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.3/parsers/common/tests/__init__.py
--rw-rw-rw-   0        0        0      163 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.3/parsers/common/tests/mock_cell_parser.py
--rw-rw-rw-   0        0        0      292 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.3/parsers/common/tests/mock_row_parser.py
--rw-rw-rw-   0        0        0      826 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.3/parsers/common/tests/mock_sheetparser.py
--rw-rw-rw-   0        0        0      600 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.3/parsers/common/tests/models.py
--rw-rw-rw-   0        0        0     6080 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.3/parsers/common/tests/test_cellparser.py
--rw-rw-rw-   0        0        0     3508 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.3/parsers/common/tests/test_differentways.py
--rw-rw-rw-   0        0        0     5026 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.3/parsers/common/tests/test_full_rows.py
--rw-rw-rw-   0        0        0     3050 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.3/parsers/common/tests/test_rowdatasheet.py
--rw-rw-rw-   0        0        0     2022 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.3/parsers/common/tests/test_sheetparser.py
--rw-rw-rw-   0        0        0     4684 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.3/parsers/common/tests/test_unparse.py
-drwxrwxrwx   0        0        0        0 2023-05-19 22:12:32.559788 rapidpro_flow_tools-1.0.3/parsers/creation/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.3/parsers/creation/__init__.py
--rw-rw-rw-   0        0        0      152 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.3/parsers/creation/constants.py
--rw-rw-rw-   0        0        0     7020 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.3/parsers/creation/contentindexparser.py
--rw-rw-rw-   0        0        0      932 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.3/parsers/creation/contentindexrowmodel.py
--rw-rw-rw-   0        0        0      102 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.3/parsers/creation/datarowmodel.py
--rw-rw-rw-   0        0        0    26665 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.3/parsers/creation/flowparser.py
--rw-rw-rw-   0        0        0     5242 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.3/parsers/creation/flowrowmodel.py
--rw-rw-rw-   0        0        0     1016 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.3/parsers/creation/template_sheet_parser.py
-drwxrwxrwx   0        0        0        0 2023-05-19 22:12:32.571786 rapidpro_flow_tools-1.0.3/parsers/creation/tests/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.3/parsers/creation/tests/__init__.py
--rw-rw-rw-   0        0        0      478 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.3/parsers/creation/tests/mock_sheetreader.py
--rw-rw-rw-   0        0        0     1030 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.3/parsers/creation/tests/row_data.py
--rw-rw-rw-   0        0        0    17043 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.3/parsers/creation/tests/test_contentindexparser.py
--rw-rw-rw-   0        0        0    39668 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.3/parsers/creation/tests/test_flowparser.py
--rw-rw-rw-   0        0        0    14789 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.3/parsers/creation/tests/test_to_row_model.py
--rw-rw-rw-   0        0        0      259 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.3/parsers/creation/tests/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-19 22:12:32.578036 rapidpro_flow_tools-1.0.3/parsers/sheets/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.3/parsers/sheets/__init__.py
--rw-rw-rw-   0        0        0      626 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.3/parsers/sheets/csv_sheet_reader.py
--rw-rw-rw-   0        0        0     3199 2023-05-17 13:33:29.000000 rapidpro_flow_tools-1.0.3/parsers/sheets/google_sheet_reader.py
--rw-rw-rw-   0        0        0      711 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.3/parsers/sheets/xlsx_sheet_reader.py
--rw-rw-rw-   0        0        0      692 2023-05-19 22:11:24.000000 rapidpro_flow_tools-1.0.3/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-19 22:12:32.580034 rapidpro_flow_tools-1.0.3/rapidpro/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.3/rapidpro/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 22:12:32.588033 rapidpro_flow_tools-1.0.3/rapidpro/tests/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.3/rapidpro/tests/__init__.py
--rw-rw-rw-   0        0        0      542 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.3/rapidpro/tests/test_actions.py
--rw-rw-rw-   0        0        0     3453 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.3/rapidpro/tests/test_containers.py
--rw-rw-rw-   0        0        0     4525 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.3/rapidpro/tests/test_import_export.py
--rw-rw-rw-   0        0        0     1304 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.3/rapidpro/tests/test_nodes.py
--rw-rw-rw-   0        0        0     6368 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.3/rapidpro/tests/test_routers.py
--rw-rw-rw-   0        0        0       73 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.3/rapidpro/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-19 22:12:32.596564 rapidpro_flow_tools-1.0.3/rapidpro_flow_tools.egg-info/
--rw-rw-rw-   0        0        0     3518 2023-05-19 22:12:32.000000 rapidpro_flow_tools-1.0.3/rapidpro_flow_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1889 2023-05-19 22:12:32.000000 rapidpro_flow_tools-1.0.3/rapidpro_flow_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 22:12:32.000000 rapidpro_flow_tools-1.0.3/rapidpro_flow_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-05-19 22:12:32.000000 rapidpro_flow_tools-1.0.3/rapidpro_flow_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-19 22:12:32.609087 rapidpro_flow_tools-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      211 2023-05-19 22:11:31.000000 rapidpro_flow_tools-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-19 22:12:32.605563 rapidpro_flow_tools-1.0.3/tests/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.3/tests/__init__.py
--rw-rw-rw-   0        0        0     2194 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.3/tests/test_contentindexparser.py
--rw-rw-rw-   0        0        0     6373 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.3/tests/test_flowparser.py
--rw-rw-rw-   0        0        0     2997 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.3/tests/test_flowparser_reverse.py
--rw-rw-rw-   0        0        0     2437 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.3/tests/test_template_sheet_parser.py
--rw-rw-rw-   0        0        0    11693 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.3/tests/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-19 22:17:32.959803 rapidpro_flow_tools-1.0.4/
+-rw-rw-rw-   0        0        0    27030 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     3518 2023-05-19 22:17:32.958790 rapidpro_flow_tools-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2906 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-19 22:17:32.864763 rapidpro_flow_tools-1.0.4/parsers/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 22:17:32.871766 rapidpro_flow_tools-1.0.4/parsers/common/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/common/__init__.py
+-rw-rw-rw-   0        0        0     4152 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/common/cellparser.py
+-rw-rw-rw-   0        0        0     3205 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/common/rowdatasheet.py
+-rw-rw-rw-   0        0        0    15945 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/common/rowparser.py
+-rw-rw-rw-   0        0        0     1849 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/common/sheetparser.py
+drwxrwxrwx   0        0        0        0 2023-05-19 22:17:32.889052 rapidpro_flow_tools-1.0.4/parsers/common/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/common/tests/__init__.py
+-rw-rw-rw-   0        0        0      163 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/common/tests/mock_cell_parser.py
+-rw-rw-rw-   0        0        0      292 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/common/tests/mock_row_parser.py
+-rw-rw-rw-   0        0        0      826 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/common/tests/mock_sheetparser.py
+-rw-rw-rw-   0        0        0      600 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/common/tests/models.py
+-rw-rw-rw-   0        0        0     6080 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/common/tests/test_cellparser.py
+-rw-rw-rw-   0        0        0     3508 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/common/tests/test_differentways.py
+-rw-rw-rw-   0        0        0     5026 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/common/tests/test_full_rows.py
+-rw-rw-rw-   0        0        0     3050 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/common/tests/test_rowdatasheet.py
+-rw-rw-rw-   0        0        0     2022 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/common/tests/test_sheetparser.py
+-rw-rw-rw-   0        0        0     4684 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/common/tests/test_unparse.py
+drwxrwxrwx   0        0        0        0 2023-05-19 22:17:32.901113 rapidpro_flow_tools-1.0.4/parsers/creation/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/creation/__init__.py
+-rw-rw-rw-   0        0        0      152 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/creation/constants.py
+-rw-rw-rw-   0        0        0     7020 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/creation/contentindexparser.py
+-rw-rw-rw-   0        0        0      932 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/creation/contentindexrowmodel.py
+-rw-rw-rw-   0        0        0      102 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/creation/datarowmodel.py
+-rw-rw-rw-   0        0        0    26665 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/creation/flowparser.py
+-rw-rw-rw-   0        0        0     5242 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/creation/flowrowmodel.py
+-rw-rw-rw-   0        0        0     1016 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/creation/template_sheet_parser.py
+drwxrwxrwx   0        0        0        0 2023-05-19 22:17:32.912171 rapidpro_flow_tools-1.0.4/parsers/creation/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/creation/tests/__init__.py
+-rw-rw-rw-   0        0        0      478 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/creation/tests/mock_sheetreader.py
+-rw-rw-rw-   0        0        0     1030 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/creation/tests/row_data.py
+-rw-rw-rw-   0        0        0    17043 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/creation/tests/test_contentindexparser.py
+-rw-rw-rw-   0        0        0    39668 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/creation/tests/test_flowparser.py
+-rw-rw-rw-   0        0        0    14789 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/creation/tests/test_to_row_model.py
+-rw-rw-rw-   0        0        0      259 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/creation/tests/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-19 22:17:32.917171 rapidpro_flow_tools-1.0.4/parsers/sheets/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/sheets/__init__.py
+-rw-rw-rw-   0        0        0      626 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/sheets/csv_sheet_reader.py
+-rw-rw-rw-   0        0        0     3199 2023-05-17 13:33:29.000000 rapidpro_flow_tools-1.0.4/parsers/sheets/google_sheet_reader.py
+-rw-rw-rw-   0        0        0      711 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/sheets/xlsx_sheet_reader.py
+-rw-rw-rw-   0        0        0      692 2023-05-19 22:16:56.000000 rapidpro_flow_tools-1.0.4/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-19 22:17:32.920173 rapidpro_flow_tools-1.0.4/rapidpro/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/rapidpro/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 22:17:32.928703 rapidpro_flow_tools-1.0.4/rapidpro/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/rapidpro/tests/__init__.py
+-rw-rw-rw-   0        0        0      542 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/rapidpro/tests/test_actions.py
+-rw-rw-rw-   0        0        0     3453 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/rapidpro/tests/test_containers.py
+-rw-rw-rw-   0        0        0     4525 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/rapidpro/tests/test_import_export.py
+-rw-rw-rw-   0        0        0     1304 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/rapidpro/tests/test_nodes.py
+-rw-rw-rw-   0        0        0     6368 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/rapidpro/tests/test_routers.py
+-rw-rw-rw-   0        0        0       73 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/rapidpro/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-19 22:17:32.947284 rapidpro_flow_tools-1.0.4/rapidpro_flow_tools.egg-info/
+-rw-rw-rw-   0        0        0     3518 2023-05-19 22:17:32.000000 rapidpro_flow_tools-1.0.4/rapidpro_flow_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1889 2023-05-19 22:17:32.000000 rapidpro_flow_tools-1.0.4/rapidpro_flow_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 22:17:32.000000 rapidpro_flow_tools-1.0.4/rapidpro_flow_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-05-19 22:17:32.000000 rapidpro_flow_tools-1.0.4/rapidpro_flow_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-19 22:17:32.959803 rapidpro_flow_tools-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      211 2023-05-19 22:16:50.000000 rapidpro_flow_tools-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 22:17:32.957789 rapidpro_flow_tools-1.0.4/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/tests/__init__.py
+-rw-rw-rw-   0        0        0     2194 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/tests/test_contentindexparser.py
+-rw-rw-rw-   0        0        0     6373 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/tests/test_flowparser.py
+-rw-rw-rw-   0        0        0     2997 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/tests/test_flowparser_reverse.py
+-rw-rw-rw-   0        0        0     2437 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/tests/test_template_sheet_parser.py
+-rw-rw-rw-   0        0        0    11693 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/tests/utils.py
```

### Comparing `rapidpro_flow_tools-1.0.3/LICENSE` & `rapidpro_flow_tools-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.3/PKG-INFO` & `rapidpro_flow_tools-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidpro_flow_tools
-Version: 1.0.3
+Version: 1.0.4
 Summary: Toolkit for using spreadsheets to create and modify RapidPro flows
 Author-email: Ed Moss <ed.moss@eemengineering.com>
 Project-URL: Homepage, https://github.com/IDEMSInternational/rapidpro-flow-toolkit
 Project-URL: Bug Tracker, https://github.com/IDEMSInternational/rapidpro-flow-toolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rapidpro_flow_tools-1.0.3/README.md` & `rapidpro_flow_tools-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.3/parsers/common/cellparser.py` & `rapidpro_flow_tools-1.0.4/parsers/common/cellparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.3/parsers/common/rowdatasheet.py` & `rapidpro_flow_tools-1.0.4/parsers/common/rowdatasheet.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.3/parsers/common/rowparser.py` & `rapidpro_flow_tools-1.0.4/parsers/common/rowparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.3/parsers/common/sheetparser.py` & `rapidpro_flow_tools-1.0.4/parsers/common/sheetparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.3/parsers/common/tests/mock_sheetparser.py` & `rapidpro_flow_tools-1.0.4/parsers/common/tests/mock_sheetparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.3/parsers/common/tests/models.py` & `rapidpro_flow_tools-1.0.4/parsers/common/tests/models.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.3/parsers/common/tests/test_cellparser.py` & `rapidpro_flow_tools-1.0.4/parsers/common/tests/test_cellparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.3/parsers/common/tests/test_differentways.py` & `rapidpro_flow_tools-1.0.4/parsers/common/tests/test_differentways.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.3/parsers/common/tests/test_full_rows.py` & `rapidpro_flow_tools-1.0.4/parsers/common/tests/test_full_rows.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.3/parsers/common/tests/test_rowdatasheet.py` & `rapidpro_flow_tools-1.0.4/parsers/common/tests/test_rowdatasheet.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.3/parsers/common/tests/test_sheetparser.py` & `rapidpro_flow_tools-1.0.4/parsers/common/tests/test_sheetparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.3/parsers/common/tests/test_unparse.py` & `rapidpro_flow_tools-1.0.4/parsers/common/tests/test_unparse.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.3/parsers/creation/contentindexparser.py` & `rapidpro_flow_tools-1.0.4/parsers/creation/contentindexparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.3/parsers/creation/contentindexrowmodel.py` & `rapidpro_flow_tools-1.0.4/parsers/creation/contentindexrowmodel.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.3/parsers/creation/flowparser.py` & `rapidpro_flow_tools-1.0.4/parsers/creation/flowparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.3/parsers/creation/flowrowmodel.py` & `rapidpro_flow_tools-1.0.4/parsers/creation/flowrowmodel.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.3/parsers/creation/template_sheet_parser.py` & `rapidpro_flow_tools-1.0.4/parsers/creation/template_sheet_parser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.3/parsers/creation/tests/row_data.py` & `rapidpro_flow_tools-1.0.4/parsers/creation/tests/row_data.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.3/parsers/creation/tests/test_contentindexparser.py` & `rapidpro_flow_tools-1.0.4/parsers/creation/tests/test_contentindexparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.3/parsers/creation/tests/test_flowparser.py` & `rapidpro_flow_tools-1.0.4/parsers/creation/tests/test_flowparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.3/parsers/creation/tests/test_to_row_model.py` & `rapidpro_flow_tools-1.0.4/parsers/creation/tests/test_to_row_model.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.3/parsers/sheets/csv_sheet_reader.py` & `rapidpro_flow_tools-1.0.4/parsers/sheets/csv_sheet_reader.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.3/parsers/sheets/google_sheet_reader.py` & `rapidpro_flow_tools-1.0.4/parsers/sheets/google_sheet_reader.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.3/parsers/sheets/xlsx_sheet_reader.py` & `rapidpro_flow_tools-1.0.4/parsers/sheets/xlsx_sheet_reader.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.3/pyproject.toml` & `rapidpro_flow_tools-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rapidpro_flow_tools"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="Ed Moss", email="ed.moss@eemengineering.com" },
 ]
 description = "Toolkit for using spreadsheets to create and modify RapidPro flows"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `rapidpro_flow_tools-1.0.3/rapidpro/tests/test_actions.py` & `rapidpro_flow_tools-1.0.4/rapidpro/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.3/rapidpro/tests/test_containers.py` & `rapidpro_flow_tools-1.0.4/rapidpro/tests/test_containers.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.3/rapidpro/tests/test_import_export.py` & `rapidpro_flow_tools-1.0.4/rapidpro/tests/test_import_export.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.3/rapidpro/tests/test_nodes.py` & `rapidpro_flow_tools-1.0.4/rapidpro/tests/test_nodes.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.3/rapidpro/tests/test_routers.py` & `rapidpro_flow_tools-1.0.4/rapidpro/tests/test_routers.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.3/rapidpro_flow_tools.egg-info/PKG-INFO` & `rapidpro_flow_tools-1.0.4/rapidpro_flow_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidpro-flow-tools
-Version: 1.0.3
+Version: 1.0.4
 Summary: Toolkit for using spreadsheets to create and modify RapidPro flows
 Author-email: Ed Moss <ed.moss@eemengineering.com>
 Project-URL: Homepage, https://github.com/IDEMSInternational/rapidpro-flow-toolkit
 Project-URL: Bug Tracker, https://github.com/IDEMSInternational/rapidpro-flow-toolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rapidpro_flow_tools-1.0.3/rapidpro_flow_tools.egg-info/SOURCES.txt` & `rapidpro_flow_tools-1.0.4/rapidpro_flow_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.3/tests/test_contentindexparser.py` & `rapidpro_flow_tools-1.0.4/tests/test_contentindexparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.3/tests/test_flowparser.py` & `rapidpro_flow_tools-1.0.4/tests/test_flowparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.3/tests/test_flowparser_reverse.py` & `rapidpro_flow_tools-1.0.4/tests/test_flowparser_reverse.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.3/tests/test_template_sheet_parser.py` & `rapidpro_flow_tools-1.0.4/tests/test_template_sheet_parser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.3/tests/utils.py` & `rapidpro_flow_tools-1.0.4/tests/utils.py`

 * *Files identical despite different names*

