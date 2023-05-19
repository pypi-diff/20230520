# Comparing `tmp/rapidpro_flow_tools-1.0.4.tar.gz` & `tmp/rapidpro_flow_tools-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapidpro_flow_tools-1.0.4.tar", last modified: Fri May 19 22:17:32 2023, max compression
+gzip compressed data, was "rapidpro_flow_tools-1.0.5.tar", last modified: Fri May 19 22:19:31 2023, max compression
```

## Comparing `rapidpro_flow_tools-1.0.4.tar` & `rapidpro_flow_tools-1.0.5.tar`

### file list

```diff
@@ -1,71 +1,100 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 22:17:32.959803 rapidpro_flow_tools-1.0.4/
--rw-rw-rw-   0        0        0    27030 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     3518 2023-05-19 22:17:32.958790 rapidpro_flow_tools-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2906 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 22:17:32.864763 rapidpro_flow_tools-1.0.4/parsers/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 22:17:32.871766 rapidpro_flow_tools-1.0.4/parsers/common/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/common/__init__.py
--rw-rw-rw-   0        0        0     4152 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/common/cellparser.py
--rw-rw-rw-   0        0        0     3205 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/common/rowdatasheet.py
--rw-rw-rw-   0        0        0    15945 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/common/rowparser.py
--rw-rw-rw-   0        0        0     1849 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/common/sheetparser.py
-drwxrwxrwx   0        0        0        0 2023-05-19 22:17:32.889052 rapidpro_flow_tools-1.0.4/parsers/common/tests/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/common/tests/__init__.py
--rw-rw-rw-   0        0        0      163 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/common/tests/mock_cell_parser.py
--rw-rw-rw-   0        0        0      292 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/common/tests/mock_row_parser.py
--rw-rw-rw-   0        0        0      826 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/common/tests/mock_sheetparser.py
--rw-rw-rw-   0        0        0      600 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/common/tests/models.py
--rw-rw-rw-   0        0        0     6080 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/common/tests/test_cellparser.py
--rw-rw-rw-   0        0        0     3508 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/common/tests/test_differentways.py
--rw-rw-rw-   0        0        0     5026 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/common/tests/test_full_rows.py
--rw-rw-rw-   0        0        0     3050 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/common/tests/test_rowdatasheet.py
--rw-rw-rw-   0        0        0     2022 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/common/tests/test_sheetparser.py
--rw-rw-rw-   0        0        0     4684 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/common/tests/test_unparse.py
-drwxrwxrwx   0        0        0        0 2023-05-19 22:17:32.901113 rapidpro_flow_tools-1.0.4/parsers/creation/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/creation/__init__.py
--rw-rw-rw-   0        0        0      152 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/creation/constants.py
--rw-rw-rw-   0        0        0     7020 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/creation/contentindexparser.py
--rw-rw-rw-   0        0        0      932 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/creation/contentindexrowmodel.py
--rw-rw-rw-   0        0        0      102 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/creation/datarowmodel.py
--rw-rw-rw-   0        0        0    26665 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/creation/flowparser.py
--rw-rw-rw-   0        0        0     5242 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/creation/flowrowmodel.py
--rw-rw-rw-   0        0        0     1016 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/creation/template_sheet_parser.py
-drwxrwxrwx   0        0        0        0 2023-05-19 22:17:32.912171 rapidpro_flow_tools-1.0.4/parsers/creation/tests/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/creation/tests/__init__.py
--rw-rw-rw-   0        0        0      478 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/creation/tests/mock_sheetreader.py
--rw-rw-rw-   0        0        0     1030 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/creation/tests/row_data.py
--rw-rw-rw-   0        0        0    17043 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/creation/tests/test_contentindexparser.py
--rw-rw-rw-   0        0        0    39668 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/creation/tests/test_flowparser.py
--rw-rw-rw-   0        0        0    14789 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/creation/tests/test_to_row_model.py
--rw-rw-rw-   0        0        0      259 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/creation/tests/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-19 22:17:32.917171 rapidpro_flow_tools-1.0.4/parsers/sheets/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/sheets/__init__.py
--rw-rw-rw-   0        0        0      626 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/sheets/csv_sheet_reader.py
--rw-rw-rw-   0        0        0     3199 2023-05-17 13:33:29.000000 rapidpro_flow_tools-1.0.4/parsers/sheets/google_sheet_reader.py
--rw-rw-rw-   0        0        0      711 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/parsers/sheets/xlsx_sheet_reader.py
--rw-rw-rw-   0        0        0      692 2023-05-19 22:16:56.000000 rapidpro_flow_tools-1.0.4/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-19 22:17:32.920173 rapidpro_flow_tools-1.0.4/rapidpro/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/rapidpro/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 22:17:32.928703 rapidpro_flow_tools-1.0.4/rapidpro/tests/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/rapidpro/tests/__init__.py
--rw-rw-rw-   0        0        0      542 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/rapidpro/tests/test_actions.py
--rw-rw-rw-   0        0        0     3453 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/rapidpro/tests/test_containers.py
--rw-rw-rw-   0        0        0     4525 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/rapidpro/tests/test_import_export.py
--rw-rw-rw-   0        0        0     1304 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/rapidpro/tests/test_nodes.py
--rw-rw-rw-   0        0        0     6368 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/rapidpro/tests/test_routers.py
--rw-rw-rw-   0        0        0       73 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/rapidpro/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-19 22:17:32.947284 rapidpro_flow_tools-1.0.4/rapidpro_flow_tools.egg-info/
--rw-rw-rw-   0        0        0     3518 2023-05-19 22:17:32.000000 rapidpro_flow_tools-1.0.4/rapidpro_flow_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1889 2023-05-19 22:17:32.000000 rapidpro_flow_tools-1.0.4/rapidpro_flow_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 22:17:32.000000 rapidpro_flow_tools-1.0.4/rapidpro_flow_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-05-19 22:17:32.000000 rapidpro_flow_tools-1.0.4/rapidpro_flow_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-19 22:17:32.959803 rapidpro_flow_tools-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      211 2023-05-19 22:16:50.000000 rapidpro_flow_tools-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-19 22:17:32.957789 rapidpro_flow_tools-1.0.4/tests/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/tests/__init__.py
--rw-rw-rw-   0        0        0     2194 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/tests/test_contentindexparser.py
--rw-rw-rw-   0        0        0     6373 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/tests/test_flowparser.py
--rw-rw-rw-   0        0        0     2997 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/tests/test_flowparser_reverse.py
--rw-rw-rw-   0        0        0     2437 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/tests/test_template_sheet_parser.py
--rw-rw-rw-   0        0        0    11693 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.4/tests/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-19 22:19:31.650119 rapidpro_flow_tools-1.0.5/
+-rw-rw-rw-   0        0        0    27030 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     3518 2023-05-19 22:19:31.650119 rapidpro_flow_tools-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2906 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/README.md
+-rw-rw-rw-   0        0        0      692 2023-05-19 22:19:10.000000 rapidpro_flow_tools-1.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-19 22:19:31.651121 rapidpro_flow_tools-1.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-19 22:19:31.510239 rapidpro_flow_tools-1.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-05-19 22:19:31.534169 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/__init__.py
+-rw-rw-rw-   0        0        0     1222 2023-05-17 15:46:39.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/flow_converter.py
+drwxrwxrwx   0        0        0        0 2023-05-19 22:19:31.554728 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 22:19:31.561270 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/common/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/common/__init__.py
+-rw-rw-rw-   0        0        0     4152 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/common/cellparser.py
+-rw-rw-rw-   0        0        0     3205 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/common/rowdatasheet.py
+-rw-rw-rw-   0        0        0    15945 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/common/rowparser.py
+-rw-rw-rw-   0        0        0     1849 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/common/sheetparser.py
+drwxrwxrwx   0        0        0        0 2023-05-19 22:19:31.577817 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/common/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/common/tests/__init__.py
+-rw-rw-rw-   0        0        0      163 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/common/tests/mock_cell_parser.py
+-rw-rw-rw-   0        0        0      292 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/common/tests/mock_row_parser.py
+-rw-rw-rw-   0        0        0      826 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/common/tests/mock_sheetparser.py
+-rw-rw-rw-   0        0        0      600 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/common/tests/models.py
+-rw-rw-rw-   0        0        0     6080 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/common/tests/test_cellparser.py
+-rw-rw-rw-   0        0        0     3508 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/common/tests/test_differentways.py
+-rw-rw-rw-   0        0        0     5026 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/common/tests/test_full_rows.py
+-rw-rw-rw-   0        0        0     3050 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/common/tests/test_rowdatasheet.py
+-rw-rw-rw-   0        0        0     2022 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/common/tests/test_sheetparser.py
+-rw-rw-rw-   0        0        0     4684 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/common/tests/test_unparse.py
+drwxrwxrwx   0        0        0        0 2023-05-19 22:19:31.587821 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/creation/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/creation/__init__.py
+-rw-rw-rw-   0        0        0      152 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/creation/constants.py
+-rw-rw-rw-   0        0        0     7020 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/creation/contentindexparser.py
+-rw-rw-rw-   0        0        0      932 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/creation/contentindexrowmodel.py
+-rw-rw-rw-   0        0        0      102 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/creation/datarowmodel.py
+-rw-rw-rw-   0        0        0    26665 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/creation/flowparser.py
+-rw-rw-rw-   0        0        0     5242 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/creation/flowrowmodel.py
+-rw-rw-rw-   0        0        0     1016 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/creation/template_sheet_parser.py
+drwxrwxrwx   0        0        0        0 2023-05-19 22:19:31.598345 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/creation/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/creation/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 22:19:31.603348 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/creation/tests/datarowmodels/
+-rw-rw-rw-   0        0        0      179 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/creation/tests/datarowmodels/evalmodels.py
+-rw-rw-rw-   0        0        0      444 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/creation/tests/datarowmodels/listmodel.py
+-rw-rw-rw-   0        0        0      557 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/creation/tests/datarowmodels/nestedmodel.py
+-rw-rw-rw-   0        0        0      133 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/creation/tests/datarowmodels/simplemodel.py
+-rw-rw-rw-   0        0        0      478 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/creation/tests/mock_sheetreader.py
+-rw-rw-rw-   0        0        0     1030 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/creation/tests/row_data.py
+-rw-rw-rw-   0        0        0    17043 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/creation/tests/test_contentindexparser.py
+-rw-rw-rw-   0        0        0    39668 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/creation/tests/test_flowparser.py
+-rw-rw-rw-   0        0        0    14789 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/creation/tests/test_to_row_model.py
+-rw-rw-rw-   0        0        0      259 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/creation/tests/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-19 22:19:31.608878 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/sheets/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/sheets/__init__.py
+-rw-rw-rw-   0        0        0      626 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/sheets/csv_sheet_reader.py
+-rw-rw-rw-   0        0        0     3199 2023-05-17 13:33:29.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/sheets/google_sheet_reader.py
+-rw-rw-rw-   0        0        0      711 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/sheets/xlsx_sheet_reader.py
+drwxrwxrwx   0        0        0        0 2023-05-19 22:19:31.610878 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/rapidpro/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/rapidpro/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 22:19:31.617877 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/rapidpro/models/
+-rw-rw-rw-   0        0        0    11728 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/rapidpro/models/actions.py
+-rw-rw-rw-   0        0        0     1004 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/rapidpro/models/common.py
+-rw-rw-rw-   0        0        0    10931 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/rapidpro/models/containers.py
+-rw-rw-rw-   0        0        0    20809 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/rapidpro/models/nodes.py
+-rw-rw-rw-   0        0        0    18753 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/rapidpro/models/routers.py
+drwxrwxrwx   0        0        0        0 2023-05-19 22:19:31.626598 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/rapidpro/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/rapidpro/tests/__init__.py
+-rw-rw-rw-   0        0        0      542 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/rapidpro/tests/test_actions.py
+-rw-rw-rw-   0        0        0     3453 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/rapidpro/tests/test_containers.py
+-rw-rw-rw-   0        0        0     4525 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/rapidpro/tests/test_import_export.py
+-rw-rw-rw-   0        0        0     1304 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/rapidpro/tests/test_nodes.py
+-rw-rw-rw-   0        0        0     6368 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/rapidpro/tests/test_routers.py
+-rw-rw-rw-   0        0        0       73 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/rapidpro/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-19 22:19:31.634590 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 22:19:31.526162 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/tests/input/
+drwxrwxrwx   0        0        0        0 2023-05-19 22:19:31.636595 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/tests/input/epicsa_chatbot/
+-rw-rw-rw-   0        0        0      282 2023-05-09 00:55:58.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/tests/input/epicsa_chatbot/epicsa_models.py
+drwxrwxrwx   0        0        0        0 2023-05-19 22:19:31.637593 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/tests/input/example1/
+-rw-rw-rw-   0        0        0      557 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/tests/input/example1/nestedmodel.py
+drwxrwxrwx   0        0        0        0 2023-05-19 22:19:31.641117 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/tests/input/parenttext/
+-rw-rw-rw-   0        0        0     5926 2023-05-09 00:55:58.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/tests/input/parenttext/parenttext_models.py
+-rw-rw-rw-   0        0        0     2231 2023-05-09 00:55:58.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/tests/input/parenttext/parenttext_models_delivery.py
+drwxrwxrwx   0        0        0        0 2023-05-19 22:19:31.642115 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/tests/input/srh_chatbot/
+-rw-rw-rw-   0        0        0     1818 2023-05-09 00:55:58.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/tests/input/srh_chatbot/srh_models.py
+-rw-rw-rw-   0        0        0     2194 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/tests/test_contentindexparser.py
+-rw-rw-rw-   0        0        0     6373 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/tests/test_flowparser.py
+-rw-rw-rw-   0        0        0     2997 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/tests/test_flowparser_reverse.py
+-rw-rw-rw-   0        0        0     2437 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/tests/test_template_sheet_parser.py
+-rw-rw-rw-   0        0        0    11693 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/tests/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-19 22:19:31.552722 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools.egg-info/
+-rw-rw-rw-   0        0        0     3518 2023-05-19 22:19:31.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4192 2023-05-19 22:19:31.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 22:19:31.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-05-19 22:19:31.000000 rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 22:19:31.648119 rapidpro_flow_tools-1.0.5/tests/
+-rw-rw-rw-   0        0        0     2194 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/tests/test_contentindexparser.py
+-rw-rw-rw-   0        0        0     6373 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/tests/test_flowparser.py
+-rw-rw-rw-   0        0        0     2997 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/tests/test_flowparser_reverse.py
+-rw-rw-rw-   0        0        0     2437 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.5/tests/test_template_sheet_parser.py
```

### Comparing `rapidpro_flow_tools-1.0.4/LICENSE` & `rapidpro_flow_tools-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.4/PKG-INFO` & `rapidpro_flow_tools-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidpro_flow_tools
-Version: 1.0.4
+Version: 1.0.5
 Summary: Toolkit for using spreadsheets to create and modify RapidPro flows
 Author-email: Ed Moss <ed.moss@eemengineering.com>
 Project-URL: Homepage, https://github.com/IDEMSInternational/rapidpro-flow-toolkit
 Project-URL: Bug Tracker, https://github.com/IDEMSInternational/rapidpro-flow-toolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rapidpro_flow_tools-1.0.4/README.md` & `rapidpro_flow_tools-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.4/parsers/common/cellparser.py` & `rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/common/cellparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.4/parsers/common/rowdatasheet.py` & `rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/common/rowdatasheet.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.4/parsers/common/rowparser.py` & `rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/common/rowparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.4/parsers/common/sheetparser.py` & `rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/common/sheetparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.4/parsers/common/tests/mock_sheetparser.py` & `rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/common/tests/mock_sheetparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.4/parsers/common/tests/models.py` & `rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/common/tests/models.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.4/parsers/common/tests/test_cellparser.py` & `rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/common/tests/test_cellparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.4/parsers/common/tests/test_differentways.py` & `rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/common/tests/test_differentways.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.4/parsers/common/tests/test_full_rows.py` & `rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/common/tests/test_full_rows.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.4/parsers/common/tests/test_rowdatasheet.py` & `rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/common/tests/test_rowdatasheet.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.4/parsers/common/tests/test_sheetparser.py` & `rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/common/tests/test_sheetparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.4/parsers/common/tests/test_unparse.py` & `rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/common/tests/test_unparse.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.4/parsers/creation/contentindexparser.py` & `rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/creation/contentindexparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.4/parsers/creation/contentindexrowmodel.py` & `rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/creation/contentindexrowmodel.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.4/parsers/creation/flowparser.py` & `rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/creation/flowparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.4/parsers/creation/flowrowmodel.py` & `rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/creation/flowrowmodel.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.4/parsers/creation/template_sheet_parser.py` & `rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/creation/template_sheet_parser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.4/parsers/creation/tests/row_data.py` & `rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/creation/tests/row_data.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.4/parsers/creation/tests/test_contentindexparser.py` & `rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/creation/tests/test_contentindexparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.4/parsers/creation/tests/test_flowparser.py` & `rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/creation/tests/test_flowparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.4/parsers/creation/tests/test_to_row_model.py` & `rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/creation/tests/test_to_row_model.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.4/parsers/sheets/csv_sheet_reader.py` & `rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/sheets/csv_sheet_reader.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.4/parsers/sheets/google_sheet_reader.py` & `rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/sheets/google_sheet_reader.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.4/parsers/sheets/xlsx_sheet_reader.py` & `rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/parsers/sheets/xlsx_sheet_reader.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.4/pyproject.toml` & `rapidpro_flow_tools-1.0.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rapidpro_flow_tools"
-version = "1.0.4"
+version = "1.0.5"
 authors = [
   { name="Ed Moss", email="ed.moss@eemengineering.com" },
 ]
 description = "Toolkit for using spreadsheets to create and modify RapidPro flows"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `rapidpro_flow_tools-1.0.4/rapidpro/tests/test_actions.py` & `rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/rapidpro/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.4/rapidpro/tests/test_containers.py` & `rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/rapidpro/tests/test_containers.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.4/rapidpro/tests/test_import_export.py` & `rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/rapidpro/tests/test_import_export.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.4/rapidpro/tests/test_nodes.py` & `rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/rapidpro/tests/test_nodes.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.4/rapidpro/tests/test_routers.py` & `rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/rapidpro/tests/test_routers.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.4/rapidpro_flow_tools.egg-info/PKG-INFO` & `rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidpro-flow-tools
-Version: 1.0.4
+Version: 1.0.5
 Summary: Toolkit for using spreadsheets to create and modify RapidPro flows
 Author-email: Ed Moss <ed.moss@eemengineering.com>
 Project-URL: Homepage, https://github.com/IDEMSInternational/rapidpro-flow-toolkit
 Project-URL: Bug Tracker, https://github.com/IDEMSInternational/rapidpro-flow-toolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rapidpro_flow_tools-1.0.4/tests/test_contentindexparser.py` & `rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/tests/test_contentindexparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.4/tests/test_flowparser.py` & `rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/tests/test_flowparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.4/tests/test_flowparser_reverse.py` & `rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/tests/test_flowparser_reverse.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.4/tests/test_template_sheet_parser.py` & `rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/tests/test_template_sheet_parser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.4/tests/utils.py` & `rapidpro_flow_tools-1.0.5/src/rapidpro_flow_tools/tests/utils.py`

 * *Files identical despite different names*

