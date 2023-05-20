# Comparing `tmp/batpy-0.1.0.tar.gz` & `tmp/batpy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batpy-0.1.0.tar", max compression
+gzip compressed data, was "batpy-0.2.0.tar", max compression
```

## Comparing `batpy-0.1.0.tar` & `batpy-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,25 @@
--rwxr-xr-x   0        0        0     1073 2023-05-08 01:57:49.005917 batpy-0.1.0/LICENSE
--rw-r--r--   0        0        0     5605 2023-05-08 01:57:49.005917 batpy-0.1.0/README.md
--rw-r--r--   0        0        0     1827 2023-05-08 01:58:24.470527 batpy-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      236 2023-05-08 01:57:49.009917 batpy-0.1.0/src/batpy/__init__.py
--rw-r--r--   0        0        0     5810 2023-05-08 01:57:49.009917 batpy-0.1.0/src/batpy/batpac_battery.py
--rw-r--r--   0        0        0     3979 2023-05-08 01:57:49.009917 batpy-0.1.0/src/batpy/batpac_datasets.py
--rw-r--r--   0        0        0    31170 2023-05-08 01:57:49.009917 batpy-0.1.0/src/batpy/batpac_tool.py
--rw-r--r--   0        0        0   209566 2023-05-08 01:57:49.009917 batpy-0.1.0/src/batpy/data/0.0.0/batpy_batpac_battery_design.toml
--rw-r--r--   0        0        0     2158 2023-05-08 01:57:49.009917 batpy-0.1.0/src/batpy/data/0.0.0/batpy_batpac_calculation_and_validation_results.toml
--rw-r--r--   0        0        0    30666 2023-05-08 01:57:49.009917 batpy-0.1.0/src/batpy/data/0.0.0/batpy_batpac_config.toml
--rw-r--r--   0        0        0    57647 2023-05-08 01:57:49.009917 batpy-0.1.0/src/batpy/data/0.0.0/batpy_batpac_summary_of_results.toml
--rw-r--r--   0        0        0    83193 2023-05-08 01:57:49.009917 batpy-0.1.0/src/batpy/data/0.0.0/batpy_batpac_user_input_cells.toml
--rw-r--r--   0        0        0    48449 2023-05-08 01:57:49.009917 batpy-0.1.0/src/batpy/data/0.0.0/batpy_batteries_config.toml
--rw-r--r--   0        0        0   209566 2023-05-08 01:57:49.013918 batpy-0.1.0/src/batpy/data/0.1.0/batpy_batpac_battery_design.toml
--rw-r--r--   0        0        0     2158 2023-05-08 01:57:49.013918 batpy-0.1.0/src/batpy/data/0.1.0/batpy_batpac_calculation_and_validation_results.toml
--rw-r--r--   0        0        0    30666 2023-05-08 01:57:49.013918 batpy-0.1.0/src/batpy/data/0.1.0/batpy_batpac_config.toml
--rw-r--r--   0        0        0    57647 2023-05-08 01:57:49.013918 batpy-0.1.0/src/batpy/data/0.1.0/batpy_batpac_summary_of_results.toml
--rw-r--r--   0        0        0    83193 2023-05-08 01:57:49.013918 batpy-0.1.0/src/batpy/data/0.1.0/batpy_batpac_user_input_cells.toml
--rw-r--r--   0        0        0    48449 2023-05-08 01:57:49.013918 batpy-0.1.0/src/batpy/data/0.1.0/batpy_batteries_config.toml
--rw-r--r--   0        0        0      145 2023-05-08 01:57:49.013918 batpy-0.1.0/src/batpy/data/__init__.py
--rw-r--r--   0        0        0     1939 2023-05-08 01:57:49.013918 batpy-0.1.0/src/batpy/is_version_compatible.py
--rw-r--r--   0        0        0     6511 1970-01-01 00:00:00.000000 batpy-0.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1073 2023-05-20 15:23:23.687684 batpy-0.2.0/LICENSE
+-rw-r--r--   0        0        0     5818 2023-05-20 15:23:23.687684 batpy-0.2.0/README.md
+-rw-r--r--   0        0        0     1922 2023-05-20 15:23:59.608070 batpy-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      236 2023-05-20 15:23:23.695684 batpy-0.2.0/src/batpy/__init__.py
+-rw-r--r--   0        0        0     5658 2023-05-20 15:23:23.695684 batpy-0.2.0/src/batpy/batpac_battery.py
+-rw-r--r--   0        0        0    30838 2023-05-20 15:23:23.695684 batpy-0.2.0/src/batpy/batpac_tool.py
+-rw-r--r--   0        0        0    12208 2023-05-20 15:23:23.695684 batpy-0.2.0/src/batpy/brightway.py
+-rw-r--r--   0        0        0   209566 2023-05-20 15:23:23.695684 batpy-0.2.0/src/batpy/data/0.0.0/batpy_batpac_battery_design.toml
+-rw-r--r--   0        0        0     2158 2023-05-20 15:23:23.695684 batpy-0.2.0/src/batpy/data/0.0.0/batpy_batpac_calculation_and_validation_results.toml
+-rw-r--r--   0        0        0    30666 2023-05-20 15:23:23.695684 batpy-0.2.0/src/batpy/data/0.0.0/batpy_batpac_config.toml
+-rw-r--r--   0        0        0    57647 2023-05-20 15:23:23.695684 batpy-0.2.0/src/batpy/data/0.0.0/batpy_batpac_summary_of_results.toml
+-rw-r--r--   0        0        0    83193 2023-05-20 15:23:23.695684 batpy-0.2.0/src/batpy/data/0.0.0/batpy_batpac_user_input_cells.toml
+-rw-r--r--   0        0        0    48449 2023-05-20 15:23:23.695684 batpy-0.2.0/src/batpy/data/0.0.0/batpy_batteries_config.toml
+-rw-r--r--   0        0        0     2232 2023-05-20 15:23:23.695684 batpy-0.2.0/src/batpy/data/0.1.0/batpy_batpac2brightway.toml
+-rw-r--r--   0        0        0   209566 2023-05-20 15:23:23.695684 batpy-0.2.0/src/batpy/data/0.1.0/batpy_batpac_battery_design.toml
+-rw-r--r--   0        0        0     2158 2023-05-20 15:23:23.695684 batpy-0.2.0/src/batpy/data/0.1.0/batpy_batpac_calculation_and_validation_results.toml
+-rw-r--r--   0        0        0    30666 2023-05-20 15:23:23.695684 batpy-0.2.0/src/batpy/data/0.1.0/batpy_batpac_config.toml
+-rw-r--r--   0        0        0    57647 2023-05-20 15:23:23.695684 batpy-0.2.0/src/batpy/data/0.1.0/batpy_batpac_summary_of_results.toml
+-rw-r--r--   0        0        0    83193 2023-05-20 15:23:23.695684 batpy-0.2.0/src/batpy/data/0.1.0/batpy_batpac_user_input_cells.toml
+-rw-r--r--   0        0        0    48449 2023-05-20 15:23:23.695684 batpy-0.2.0/src/batpy/data/0.1.0/batpy_batteries_config.toml
+-rw-r--r--   0        0        0      145 2023-05-20 15:23:23.695684 batpy-0.2.0/src/batpy/data/__init__.py
+-rw-r--r--   0        0        0     3979 2023-05-20 15:23:23.695684 batpy-0.2.0/src/batpy/datasets.py
+-rw-r--r--   0        0        0    10048 2023-05-20 15:23:23.695684 batpy-0.2.0/src/batpy/formula_engine.py
+-rw-r--r--   0        0        0     3799 2023-05-20 15:23:23.695684 batpy-0.2.0/src/batpy/utility_functions.py
+-rw-r--r--   0        0        0     6724 1970-01-01 00:00:00.000000 batpy-0.2.0/PKG-INFO
```

### Comparing `batpy-0.1.0/LICENSE` & `batpy-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `batpy-0.1.0/README.md` & `batpy-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,25 @@
-[![ci-cd](https://github.com/rginster/batpy/actions/workflows/ci-cd.yaml/badge.svg)](https://github.com/rginster/batpy/actions/workflows/ci-cd.yaml)
+![BatPy](https://raw.githubusercontent.com/rginster/batpy/main/BatPy.svg)
+[![ci](https://github.com/rginster/batpy/actions/workflows/ci.yaml/badge.svg)](https://github.com/rginster/batpy/actions/workflows/ci.yaml)
+[![cd](https://github.com/rginster/batpy/actions/workflows/ci-cd.yaml/badge.svg)](https://github.com/rginster/batpy/actions/workflows/ci-cd.yaml)
 [![Docs](https://github.com/rginster/batpy/actions/workflows/documentation.yaml/badge.svg)](https://github.com/rginster/batpy/actions/workflows/documentation.yaml)
 [![pages-build-deployment](https://github.com/rginster/batpy/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/rginster/batpy/actions/workflows/pages/pages-build-deployment)
 [![codecov](https://codecov.io/gh/rginster/batpy/branch/main/graph/badge.svg?token=JH8L3B14AW)](https://codecov.io/gh/rginster/batpy)
+
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/batpy)
 [![PyPi](https://img.shields.io/pypi/v/batpy.svg)](https://pypi.python.org/pypi/batpy)
 [![PyPi](https://img.shields.io/pypi/dm/batpy.svg)](https://pypi.python.org/pypi/batpy)
 
 # batpy
 
 `batpy` is a Python wrapper for [Argonne National Laboratory's](https://www.anl.gov) Microsoft Excel-based [software modeling tool BatPaC](https://www.anl.gov/partnerships/batpac-battery-manufacturing-cost-estimation).
 
 ## Installation
 
-`batpy` is available from [PyPI](https://pypi.org/project/batpy/), and currently requires Python 3.9 or newer. It can be installed with:
+`batpy` is available from [PyPI](https://pypi.org/project/batpy/), and currently requires Python 3.10 or newer. It can be installed with:
 ```bash
 $ pip install batpy
 ```
 
 ## Documentation
 
 Documentation for `batpy` is available at [GitHub Pages](https://rginster.github.io/batpy/), including an example and documentation on all the modules and functions.
```

### Comparing `batpy-0.1.0/pyproject.toml` & `batpy-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "batpy"
-version = "0.1.0"
+version = "0.2.0"
 description = "A python package to read, write, and calculate batteries in the BatPaC tool."
 authors = ["Raphael Ginster <r.ginster@tu-braunschweig.de>"]
 license = "MIT"
 readme = "README.md"
 documentation = "https://rginster.github.io/batpy/"
 repository = "https://github.com/rginster/batpy"
 
@@ -54,7 +54,13 @@
 upload_to_release = true                    # auto-create GitHub release
 upload_to_pypi = false                      # don't auto-upload to PyPI
 remove_dist = false                         # don't remove dists
 patch_without_tag = false                   # patch release by default
 
 [tool.black]
 line-length = 79
+
+[tool.bandit.assert_used]
+skips = ['*_test.py', '*test_*.py']
+
+[tool.isort]
+profile = "black"
```

### Comparing `batpy-0.1.0/src/batpy/batpac_battery.py` & `batpy-0.2.0/src/batpy/batpac_battery.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # -*- coding: UTF-8 -*-
 """Module, which includes the class BatpacBattery
 """
 import logging
 from pathlib import Path
 
 import semantic_version
-import toml
 
 import batpy
-from batpy.is_version_compatible import is_version_compatible
+from batpy.utility_functions import is_version_compatible, load_configuration
 
 
 class BatpacBattery:
     """Battery class for interaction with BatPaC
 
     This battery class is used to interact with BatPaC and stores battery
     parameters in the dictionary properties.
@@ -89,19 +88,15 @@
             )
         """
         logging.info(
             "[ ] Load battery config for %s from %s",
             battery_name,
             path_to_battery_file,
         )
-        try:
-            Path.exists(Path(path_to_battery_file))
-            config = toml.load(path_to_battery_file)
-        except (AttributeError, OSError):
-            config = toml.loads(path_to_battery_file)
+        config = load_configuration(path_to_battery_file)
         config_metadata = config.pop("batpy")
         if is_version_compatible(
             self.version,
             semantic_version.Version(config_metadata["BatPaC SemVer"]),
         ):
             loaded = False
             if battery_name in config:
```

### Comparing `batpy-0.1.0/src/batpy/batpac_datasets.py` & `batpy-0.2.0/src/batpy/datasets.py`

 * *Files identical despite different names*

### Comparing `batpy-0.1.0/src/batpy/batpac_tool.py` & `batpy-0.2.0/src/batpy/batpac_tool.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,25 +8,47 @@
 import toml
 import xlwings as xw
 from prettytable import PrettyTable
 from tqdm import tqdm
 
 import batpy
 from batpy.batpac_battery import BatpacBattery
-from batpy.is_version_compatible import is_version_compatible
+from batpy.utility_functions import is_version_compatible, load_configuration
 
 
 class BatpacTool:
     """BatPaC class which interacts with the BatPaC Excel tool
 
     This BatPaC class is used to interact directly with the BatPaC Excel tool
     and can store individual batteries (class BatPaC_battery) and additional
     parameters of the BatPaC Excel tool in the dictionary properties.
     """
 
+    def _load_user_file(self, path_to_user_file: Path | str) -> dict:
+        """Load user file configuration
+
+        Load the user configuration from a TOML user file.
+
+        Parameters
+        ----------
+        path_to_user_file : Path | str
+            Path to the TOML user file or configuration as string.
+
+        Returns
+        -------
+        dict
+            Returns dictionary representation of read TOML file.
+        """
+        config = load_configuration(path_to_user_file)
+        config_metadata = config.pop("batpy")
+        self.is_version_compatible(
+            semantic_version.Version(config_metadata["BatPaC SemVer"])
+        )
+        return config
+
     def __init__(
         self,
         batpac_workbook_path: Path,
         cell_definition_user_input_toml_path: Path | str,
         cell_definition_calculation_validation_results: Path | str = None,
         # cell_definition_additional_user_input_toml_path: Path = None,
         # cell_definition_additional_user_results_toml_path: Path = None,
@@ -63,19 +85,19 @@
         logging.info(
             "[ ] Create BatPaC from %s and load cell references from %s",
             batpac_workbook_path,
             cell_definition_user_input_toml_path,
         )
         self.version = semantic_version.Version(batpy.__version__)
 
-        self.excel_cells = self.load_user_file(
+        self.excel_cells = self._load_user_file(
             cell_definition_user_input_toml_path
         )
         if cell_definition_calculation_validation_results:
-            self.toml_calculation_validation_results = self.load_user_file(
+            self.toml_calculation_validation_results = self._load_user_file(
                 cell_definition_calculation_validation_results
             )
         self.batteries = []
         self.workbook = xw.Book(batpac_workbook_path)
         # self.app = self.workbook.app
         self.workbook.app.visible = excel_visible
         self.max_batteries = 7
@@ -132,44 +154,14 @@
         ValueError
             If version is not compatible a ValueError will occur.
         """
         return is_version_compatible(
             self.version, version_to_check, include_minor
         )
 
-    def load_user_file(self, path_to_user_file: Path | str) -> dict:
-        """Load user file configuration
-
-        Load the user configuration from a TOML user file.
-
-        Parameters
-        ----------
-        path_to_user_file : Path | str
-            Path to the TOML user file or string (default dataset).
-
-        Returns
-        -------
-        dict
-            Returns dictionary representation of read TOML file.
-        """
-        logging.info("[ ] Load BatPaC file from %s", path_to_user_file)
-
-        try:
-            Path.exists(Path(path_to_user_file))
-            config = toml.load(path_to_user_file)
-        except (AttributeError, OSError):
-            config = toml.loads(path_to_user_file)
-        config_metadata = config.pop("batpy")
-        self.is_version_compatible(
-            semantic_version.Version(config_metadata["BatPaC SemVer"])
-        )
-        logging.info("[+] Loaded user file from %s", path_to_user_file)
-        logging.debug("[ ] Config properties %s", config)
-        return config
-
     def load_batpac_file(self, path_to_batpac_file: Path | str) -> None:
         """Load BatPaC configuration
 
         Load the properties for the BatPaC object from a TOML battery
         configuration file.
 
         Parameters
@@ -355,15 +347,15 @@
             found.
         """
         try:
             if additional_cell_config is not None:
                 if isinstance(additional_cell_config, dict):
                     range_dict = additional_cell_config
                 else:
-                    range_dict = self.load_user_file(additional_cell_config)
+                    range_dict = self._load_user_file(additional_cell_config)
             else:
                 range_dict = self.excel_cells
 
             if battery is None:
                 cell_range = range_dict[worksheet][name]
             else:
                 cell_range = range_dict[worksheet][
@@ -537,15 +529,15 @@
 
         Returns
         -------
         dict
             Dictionary in the format {"sheet" : {"name" : value} }
         """
 
-        additional_cells = self.load_user_file(user_read_file)
+        additional_cells = self._load_user_file(user_read_file)
         values_dict = additional_cells
         for sheet_name, sheet_key in additional_cells.items():
             for batpac_key, batpac_cell_range in sheet_key.items():
                 if isinstance(batpac_cell_range, dict):
                     for (
                         battery_key,
                         battery_cell_range,
@@ -592,15 +584,15 @@
                 logging.warning(
                     "[!] No toml file for calculation and validation found."
                 )
                 raise KeyError(
                     "No configuration for calculation and validation found."
                 )
         else:
-            self.toml_calculation_validation_results = self.load_user_file(
+            self.toml_calculation_validation_results = self._load_user_file(
                 toml_file_calculation_validation_results
             )
 
         config_errors = ["Configuration Errors (see table to right)"]
         config_warnings = ["Configuration Warnings (see table  to right)"]
         plant_size = ["Plant Size, GWh"]
         power_to_energy = ["Power-to-energy ratio"]
```

### Comparing `batpy-0.1.0/src/batpy/data/0.0.0/batpy_batpac_battery_design.toml` & `batpy-0.2.0/src/batpy/data/0.0.0/batpy_batpac_battery_design.toml`

 * *Files identical despite different names*

### Comparing `batpy-0.1.0/src/batpy/data/0.0.0/batpy_batpac_calculation_and_validation_results.toml` & `batpy-0.2.0/src/batpy/data/0.0.0/batpy_batpac_calculation_and_validation_results.toml`

 * *Files identical despite different names*

### Comparing `batpy-0.1.0/src/batpy/data/0.0.0/batpy_batpac_config.toml` & `batpy-0.2.0/src/batpy/data/0.0.0/batpy_batpac_config.toml`

 * *Files identical despite different names*

### Comparing `batpy-0.1.0/src/batpy/data/0.0.0/batpy_batpac_summary_of_results.toml` & `batpy-0.2.0/src/batpy/data/0.0.0/batpy_batpac_summary_of_results.toml`

 * *Files identical despite different names*

### Comparing `batpy-0.1.0/src/batpy/data/0.0.0/batpy_batpac_user_input_cells.toml` & `batpy-0.2.0/src/batpy/data/0.0.0/batpy_batpac_user_input_cells.toml`

 * *Files identical despite different names*

### Comparing `batpy-0.1.0/src/batpy/data/0.0.0/batpy_batteries_config.toml` & `batpy-0.2.0/src/batpy/data/0.0.0/batpy_batteries_config.toml`

 * *Files identical despite different names*

### Comparing `batpy-0.1.0/src/batpy/data/0.1.0/batpy_batpac_battery_design.toml` & `batpy-0.2.0/src/batpy/data/0.1.0/batpy_batpac_battery_design.toml`

 * *Files identical despite different names*

### Comparing `batpy-0.1.0/src/batpy/data/0.1.0/batpy_batpac_calculation_and_validation_results.toml` & `batpy-0.2.0/src/batpy/data/0.1.0/batpy_batpac_calculation_and_validation_results.toml`

 * *Files identical despite different names*

### Comparing `batpy-0.1.0/src/batpy/data/0.1.0/batpy_batpac_config.toml` & `batpy-0.2.0/src/batpy/data/0.1.0/batpy_batpac_config.toml`

 * *Files identical despite different names*

### Comparing `batpy-0.1.0/src/batpy/data/0.1.0/batpy_batpac_summary_of_results.toml` & `batpy-0.2.0/src/batpy/data/0.1.0/batpy_batpac_summary_of_results.toml`

 * *Files identical despite different names*

### Comparing `batpy-0.1.0/src/batpy/data/0.1.0/batpy_batpac_user_input_cells.toml` & `batpy-0.2.0/src/batpy/data/0.1.0/batpy_batpac_user_input_cells.toml`

 * *Files identical despite different names*

### Comparing `batpy-0.1.0/src/batpy/data/0.1.0/batpy_batteries_config.toml` & `batpy-0.2.0/src/batpy/data/0.1.0/batpy_batteries_config.toml`

 * *Files identical despite different names*

### Comparing `batpy-0.1.0/PKG-INFO` & `batpy-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batpy
-Version: 0.1.0
+Version: 0.2.0
 Summary: A python package to read, write, and calculate batteries in the BatPaC tool.
 Home-page: https://github.com/rginster/batpy
 License: MIT
 Author: Raphael Ginster
 Author-email: r.ginster@tu-braunschweig.de
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -17,29 +17,32 @@
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: xlwings (>=0.30.4,<0.31.0)
 Project-URL: Documentation, https://rginster.github.io/batpy/
 Project-URL: Repository, https://github.com/rginster/batpy
 Description-Content-Type: text/markdown
 
-[![ci-cd](https://github.com/rginster/batpy/actions/workflows/ci-cd.yaml/badge.svg)](https://github.com/rginster/batpy/actions/workflows/ci-cd.yaml)
+![BatPy](https://raw.githubusercontent.com/rginster/batpy/main/BatPy.svg)
+[![ci](https://github.com/rginster/batpy/actions/workflows/ci.yaml/badge.svg)](https://github.com/rginster/batpy/actions/workflows/ci.yaml)
+[![cd](https://github.com/rginster/batpy/actions/workflows/ci-cd.yaml/badge.svg)](https://github.com/rginster/batpy/actions/workflows/ci-cd.yaml)
 [![Docs](https://github.com/rginster/batpy/actions/workflows/documentation.yaml/badge.svg)](https://github.com/rginster/batpy/actions/workflows/documentation.yaml)
 [![pages-build-deployment](https://github.com/rginster/batpy/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/rginster/batpy/actions/workflows/pages/pages-build-deployment)
 [![codecov](https://codecov.io/gh/rginster/batpy/branch/main/graph/badge.svg?token=JH8L3B14AW)](https://codecov.io/gh/rginster/batpy)
+
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/batpy)
 [![PyPi](https://img.shields.io/pypi/v/batpy.svg)](https://pypi.python.org/pypi/batpy)
 [![PyPi](https://img.shields.io/pypi/dm/batpy.svg)](https://pypi.python.org/pypi/batpy)
 
 # batpy
 
 `batpy` is a Python wrapper for [Argonne National Laboratory's](https://www.anl.gov) Microsoft Excel-based [software modeling tool BatPaC](https://www.anl.gov/partnerships/batpac-battery-manufacturing-cost-estimation).
 
 ## Installation
 
-`batpy` is available from [PyPI](https://pypi.org/project/batpy/), and currently requires Python 3.9 or newer. It can be installed with:
+`batpy` is available from [PyPI](https://pypi.org/project/batpy/), and currently requires Python 3.10 or newer. It can be installed with:
 ```bash
 $ pip install batpy
 ```
 
 ## Documentation
 
 Documentation for `batpy` is available at [GitHub Pages](https://rginster.github.io/batpy/), including an example and documentation on all the modules and functions.
```

