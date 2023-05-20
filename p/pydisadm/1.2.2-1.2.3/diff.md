# Comparing `tmp/pydisadm-1.2.2.tar.gz` & `tmp/pydisadm-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydisadm-1.2.2.tar", max compression
+gzip compressed data, was "pydisadm-1.2.3.tar", max compression
```

## Comparing `pydisadm-1.2.2.tar` & `pydisadm-1.2.3.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0     2936 2023-05-19 03:51:07.933591 pydisadm-1.2.2/README.md
--rw-r--r--   0        0        0      111 2023-05-19 03:51:07.933591 pydisadm-1.2.2/pydisadm/__init__.py
--rw-r--r--   0        0        0     1130 2023-05-19 03:51:07.933591 pydisadm-1.2.2/pydisadm/__main__.py
--rw-r--r--   0        0        0     1541 2023-05-19 03:51:07.933591 pydisadm-1.2.2/pydisadm/bot/adm_bot.py
--rw-r--r--   0        0        0     7238 2023-05-19 03:51:07.933591 pydisadm-1.2.2/pydisadm/bot/adm_cog.py
--rw-r--r--   0        0        0     2649 2023-05-19 03:51:07.933591 pydisadm-1.2.2/pydisadm/bot/update_adm_modal.py
--rw-r--r--   0        0        0      702 2023-05-19 03:51:07.933591 pydisadm-1.2.2/pydisadm/bot/utils.py
--rw-r--r--   0        0        0     1413 2023-05-19 03:51:07.933591 pydisadm-1.2.2/pydisadm/configuration.py
--rw-r--r--   0        0        0     8044 2023-05-19 03:51:07.933591 pydisadm-1.2.2/pydisadm/controller/adm_controller.py
--rw-r--r--   0        0        0   368313 2023-05-19 03:51:07.933591 pydisadm-1.2.2/pydisadm/data/mapConstellations.csv
--rw-r--r--   0        0        0    34613 2023-05-19 03:51:07.933591 pydisadm-1.2.2/pydisadm/data/mapRegions.csv
--rw-r--r--   0        0        0  3277768 2023-05-19 03:51:07.953592 pydisadm-1.2.2/pydisadm/data/mapSolarSystems.csv
--rw-r--r--   0        0        0      607 2023-05-19 03:51:07.953592 pydisadm-1.2.2/pydisadm/loader/datasets.py
--rw-r--r--   0        0        0     1085 2023-05-19 03:51:07.953592 pydisadm-1.2.2/pydisadm/loader/static_data.py
--rw-r--r--   0        0        0     1294 2023-05-19 03:51:07.953592 pydisadm-1.2.2/pydisadm/runnable/runnable_refresh.py
--rw-r--r--   0        0        0     3814 2023-05-19 03:51:07.953592 pydisadm-1.2.2/pydisadm/services/database.py
--rw-r--r--   0        0        0     1543 2023-05-19 03:51:07.953592 pydisadm-1.2.2/pydisadm/services/esi.py
--rw-r--r--   0        0        0      484 2023-05-19 03:51:07.953592 pydisadm-1.2.2/pydisadm/utils/adm_utils.py
--rw-r--r--   0        0        0      472 2023-05-19 03:51:07.953592 pydisadm-1.2.2/pydisadm/utils/datetime_utils.py
--rw-r--r--   0        0        0      623 2023-05-19 03:51:07.953592 pydisadm-1.2.2/pydisadm/utils/plot_utils.py
--rw-r--r--   0        0        0      193 2023-05-19 03:51:07.953592 pydisadm-1.2.2/pydisadm/utils/thread_utils.py
--rw-r--r--   0        0        0      953 2023-05-19 03:51:35.694313 pydisadm-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     3792 1970-01-01 00:00:00.000000 pydisadm-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     2936 2023-05-20 02:10:54.449537 pydisadm-1.2.3/README.md
+-rw-r--r--   0        0        0      111 2023-05-20 02:10:54.453537 pydisadm-1.2.3/pydisadm/__init__.py
+-rw-r--r--   0        0        0     1130 2023-05-20 02:10:54.453537 pydisadm-1.2.3/pydisadm/__main__.py
+-rw-r--r--   0        0        0     1541 2023-05-20 02:10:54.453537 pydisadm-1.2.3/pydisadm/bot/adm_bot.py
+-rw-r--r--   0        0        0     7238 2023-05-20 02:10:54.453537 pydisadm-1.2.3/pydisadm/bot/adm_cog.py
+-rw-r--r--   0        0        0     2649 2023-05-20 02:10:54.453537 pydisadm-1.2.3/pydisadm/bot/update_adm_modal.py
+-rw-r--r--   0        0        0      702 2023-05-20 02:10:54.453537 pydisadm-1.2.3/pydisadm/bot/utils.py
+-rw-r--r--   0        0        0     1413 2023-05-20 02:10:54.453537 pydisadm-1.2.3/pydisadm/configuration.py
+-rw-r--r--   0        0        0     8044 2023-05-20 02:10:54.453537 pydisadm-1.2.3/pydisadm/controller/adm_controller.py
+-rw-r--r--   0        0        0        0 2023-05-20 02:10:54.453537 pydisadm-1.2.3/pydisadm/data/__init__.py
+-rw-r--r--   0        0        0   368313 2023-05-20 02:10:54.453537 pydisadm-1.2.3/pydisadm/data/mapConstellations.csv
+-rw-r--r--   0        0        0    34613 2023-05-20 02:10:54.453537 pydisadm-1.2.3/pydisadm/data/mapRegions.csv
+-rw-r--r--   0        0        0  3277768 2023-05-20 02:10:54.473537 pydisadm-1.2.3/pydisadm/data/mapSolarSystems.csv
+-rw-r--r--   0        0        0      607 2023-05-20 02:10:54.473537 pydisadm-1.2.3/pydisadm/loader/datasets.py
+-rw-r--r--   0        0        0     1085 2023-05-20 02:10:54.473537 pydisadm-1.2.3/pydisadm/loader/static_data.py
+-rw-r--r--   0        0        0     1294 2023-05-20 02:10:54.473537 pydisadm-1.2.3/pydisadm/runnable/runnable_refresh.py
+-rw-r--r--   0        0        0     3814 2023-05-20 02:10:54.473537 pydisadm-1.2.3/pydisadm/services/database.py
+-rw-r--r--   0        0        0     1543 2023-05-20 02:10:54.473537 pydisadm-1.2.3/pydisadm/services/esi.py
+-rw-r--r--   0        0        0      484 2023-05-20 02:10:54.473537 pydisadm-1.2.3/pydisadm/utils/adm_utils.py
+-rw-r--r--   0        0        0      472 2023-05-20 02:10:54.473537 pydisadm-1.2.3/pydisadm/utils/datetime_utils.py
+-rw-r--r--   0        0        0      623 2023-05-20 02:10:54.473537 pydisadm-1.2.3/pydisadm/utils/plot_utils.py
+-rw-r--r--   0        0        0      193 2023-05-20 02:10:54.473537 pydisadm-1.2.3/pydisadm/utils/thread_utils.py
+-rw-r--r--   0        0        0      953 2023-05-20 02:11:28.065882 pydisadm-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3842 1970-01-01 00:00:00.000000 pydisadm-1.2.3/PKG-INFO
```

### Comparing `pydisadm-1.2.2/README.md` & `pydisadm-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pydisadm-1.2.2/pydisadm/__main__.py` & `pydisadm-1.2.3/pydisadm/__main__.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.2.2/pydisadm/bot/adm_bot.py` & `pydisadm-1.2.3/pydisadm/bot/adm_bot.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.2.2/pydisadm/bot/adm_cog.py` & `pydisadm-1.2.3/pydisadm/bot/adm_cog.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.2.2/pydisadm/bot/update_adm_modal.py` & `pydisadm-1.2.3/pydisadm/bot/update_adm_modal.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.2.2/pydisadm/bot/utils.py` & `pydisadm-1.2.3/pydisadm/bot/utils.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.2.2/pydisadm/configuration.py` & `pydisadm-1.2.3/pydisadm/configuration.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.2.2/pydisadm/controller/adm_controller.py` & `pydisadm-1.2.3/pydisadm/controller/adm_controller.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.2.2/pydisadm/data/mapConstellations.csv` & `pydisadm-1.2.3/pydisadm/data/mapConstellations.csv`

 * *Files identical despite different names*

### Comparing `pydisadm-1.2.2/pydisadm/data/mapRegions.csv` & `pydisadm-1.2.3/pydisadm/data/mapRegions.csv`

 * *Files identical despite different names*

### Comparing `pydisadm-1.2.2/pydisadm/data/mapSolarSystems.csv` & `pydisadm-1.2.3/pydisadm/data/mapSolarSystems.csv`

 * *Files identical despite different names*

### Comparing `pydisadm-1.2.2/pydisadm/loader/datasets.py` & `pydisadm-1.2.3/pydisadm/loader/datasets.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.2.2/pydisadm/loader/static_data.py` & `pydisadm-1.2.3/pydisadm/loader/static_data.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.2.2/pydisadm/runnable/runnable_refresh.py` & `pydisadm-1.2.3/pydisadm/runnable/runnable_refresh.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.2.2/pydisadm/services/database.py` & `pydisadm-1.2.3/pydisadm/services/database.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.2.2/pydisadm/services/esi.py` & `pydisadm-1.2.3/pydisadm/services/esi.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.2.2/pydisadm/utils/plot_utils.py` & `pydisadm-1.2.3/pydisadm/utils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.2.2/pyproject.toml` & `pydisadm-1.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "pydisadm"
-version = "1.2.2"
+version = "1.2.3"
 description = "A Discord bot providing ADM summaries."
 repository = "https://github.com/agelito/adm-bot"
 authors = ["Axel Wettervik"]
 license = "MIT"
 readme = "README.md"
 include = ["data/*.csv"]
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.8"
 schedule = "^1.2.0"
 requests = "^2.30.0"
 discord = "^2.2.3"
 python-dotenv = "^1.0.0"
 pandas = "^2.0.1"
 tabulate = "^0.9.0"
 matplotlib = "^3.7.1"
```

### Comparing `pydisadm-1.2.2/PKG-INFO` & `pydisadm-1.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: pydisadm
-Version: 1.2.2
+Version: 1.2.3
 Summary: A Discord bot providing ADM summaries.
 Home-page: https://github.com/agelito/adm-bot
 License: MIT
 Author: Axel Wettervik
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: discord (>=2.2.3,<3.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
```

