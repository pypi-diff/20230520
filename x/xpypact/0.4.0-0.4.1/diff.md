# Comparing `tmp/xpypact-0.4.0.tar.gz` & `tmp/xpypact-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xpypact-0.4.0.tar", max compression
+gzip compressed data, was "xpypact-0.4.1.tar", max compression
```

## Comparing `xpypact-0.4.0.tar` & `xpypact-0.4.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1063 2023-04-30 12:22:42.233936 xpypact-0.4.0/LICENSE
--rw-r--r--   0        0        0     3296 2023-04-30 12:22:42.233936 xpypact-0.4.0/README.rst
--rw-r--r--   0        0        0    17341 2023-04-30 12:23:06.746078 xpypact-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1199 2023-04-30 12:22:42.241937 xpypact-0.4.0/src/xpypact/__init__.py
--rw-r--r--   0        0        0      174 2023-04-30 12:22:42.241937 xpypact-0.4.0/src/xpypact/dao/__init__.py
--rw-r--r--   0        0        0     2241 2023-04-30 12:22:42.241937 xpypact-0.4.0/src/xpypact/dao/api.py
--rw-r--r--   0        0        0      168 2023-04-30 12:22:42.241937 xpypact-0.4.0/src/xpypact/dao/duckdb/__init__.py
--rw-r--r--   0        0        0     2870 2023-04-30 12:22:42.241937 xpypact-0.4.0/src/xpypact/dao/duckdb/create_schema.sql
--rw-r--r--   0        0        0     7971 2023-04-30 12:23:06.746078 xpypact-0.4.0/src/xpypact/dao/duckdb/implementation.py
--rw-r--r--   0        0        0    14156 2023-04-30 12:22:42.241937 xpypact-0.4.0/src/xpypact/data_arrays.py
--rw-r--r--   0        0        0     5307 2023-04-30 12:22:42.241937 xpypact-0.4.0/src/xpypact/data_frames.py
--rw-r--r--   0        0        0    12337 2023-04-30 12:22:42.241937 xpypact-0.4.0/src/xpypact/fluxes.py
--rw-r--r--   0        0        0     5862 2023-04-30 12:22:42.241937 xpypact-0.4.0/src/xpypact/inventory.py
--rw-r--r--   0        0        0     1965 2023-04-30 12:22:42.241937 xpypact-0.4.0/src/xpypact/nuclide.py
--rw-r--r--   0        0        0        0 2023-04-30 12:22:42.241937 xpypact-0.4.0/src/xpypact/py.typed
--rw-r--r--   0        0        0      515 2023-04-30 12:22:42.241937 xpypact-0.4.0/src/xpypact/run_data.py
--rw-r--r--   0        0        0     4924 2023-04-30 12:22:42.241937 xpypact-0.4.0/src/xpypact/time_step.py
--rw-r--r--   0        0        0       29 2023-04-30 12:22:42.241937 xpypact-0.4.0/src/xpypact/utils/__init__.py
--rw-r--r--   0        0        0      809 2023-04-30 12:22:42.241937 xpypact-0.4.0/src/xpypact/utils/io.py
--rw-r--r--   0        0        0        0 2023-04-30 12:22:42.241937 xpypact-0.4.0/src/xpypact/utils/py.typed
--rw-r--r--   0        0        0      768 2023-04-30 12:22:42.241937 xpypact-0.4.0/src/xpypact/utils/resource.py
--rw-r--r--   0        0        0      270 2023-04-30 12:22:42.241937 xpypact-0.4.0/src/xpypact/utils/types.py
--rw-r--r--   0        0        0     4789 1970-01-01 00:00:00.000000 xpypact-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-05-20 11:43:57.656528 xpypact-0.4.1/LICENSE
+-rw-r--r--   0        0        0     3296 2023-05-20 11:43:57.656528 xpypact-0.4.1/README.rst
+-rw-r--r--   0        0        0    17470 2023-05-20 11:44:11.505156 xpypact-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1199 2023-05-20 11:43:57.664529 xpypact-0.4.1/src/xpypact/__init__.py
+-rw-r--r--   0        0        0      174 2023-05-20 11:43:57.664529 xpypact-0.4.1/src/xpypact/dao/__init__.py
+-rw-r--r--   0        0        0     2241 2023-05-20 11:43:57.664529 xpypact-0.4.1/src/xpypact/dao/api.py
+-rw-r--r--   0        0        0      168 2023-05-20 11:43:57.664529 xpypact-0.4.1/src/xpypact/dao/duckdb/__init__.py
+-rw-r--r--   0        0        0     2870 2023-05-20 11:43:57.664529 xpypact-0.4.1/src/xpypact/dao/duckdb/create_schema.sql
+-rw-r--r--   0        0        0     7978 2023-05-20 11:44:11.505156 xpypact-0.4.1/src/xpypact/dao/duckdb/implementation.py
+-rw-r--r--   0        0        0    14156 2023-05-20 11:43:57.664529 xpypact-0.4.1/src/xpypact/data_arrays.py
+-rw-r--r--   0        0        0     5307 2023-05-20 11:43:57.664529 xpypact-0.4.1/src/xpypact/data_frames.py
+-rw-r--r--   0        0        0    12337 2023-05-20 11:43:57.664529 xpypact-0.4.1/src/xpypact/fluxes.py
+-rw-r--r--   0        0        0     5862 2023-05-20 11:43:57.664529 xpypact-0.4.1/src/xpypact/inventory.py
+-rw-r--r--   0        0        0     1965 2023-05-20 11:43:57.664529 xpypact-0.4.1/src/xpypact/nuclide.py
+-rw-r--r--   0        0        0        0 2023-05-20 11:43:57.664529 xpypact-0.4.1/src/xpypact/py.typed
+-rw-r--r--   0        0        0      515 2023-05-20 11:43:57.664529 xpypact-0.4.1/src/xpypact/run_data.py
+-rw-r--r--   0        0        0     4924 2023-05-20 11:43:57.664529 xpypact-0.4.1/src/xpypact/time_step.py
+-rw-r--r--   0        0        0       29 2023-05-20 11:43:57.664529 xpypact-0.4.1/src/xpypact/utils/__init__.py
+-rw-r--r--   0        0        0      809 2023-05-20 11:43:57.664529 xpypact-0.4.1/src/xpypact/utils/io.py
+-rw-r--r--   0        0        0        0 2023-05-20 11:43:57.664529 xpypact-0.4.1/src/xpypact/utils/py.typed
+-rw-r--r--   0        0        0      768 2023-05-20 11:43:57.664529 xpypact-0.4.1/src/xpypact/utils/resource.py
+-rw-r--r--   0        0        0      270 2023-05-20 11:43:57.664529 xpypact-0.4.1/src/xpypact/utils/types.py
+-rw-r--r--   0        0        0     4789 1970-01-01 00:00:00.000000 xpypact-0.4.1/PKG-INFO
```

### Comparing `xpypact-0.4.0/LICENSE` & `xpypact-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xpypact-0.4.0/README.rst` & `xpypact-0.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `xpypact-0.4.0/pyproject.toml` & `xpypact-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xpypact"
-version = "0.4.0"
+version = "0.4.1"
 description = "\"Python tools to work with elements and isotopes\""
 authors = ["dvp <dmitri_portnov@yahoo.com>"]
 license = "MIT"
 homepage = "https://github.com/MC-kit/xpypact"
 repository = "https://github.com/MC-kit/xpypact"
 documentation = "https://xpypact.readthedocs.io"
 keywords = [
@@ -42,15 +42,15 @@
 [tool.poetry.urls]
 documentation = "https://xpypact.readthedocs.io"
 Changelog = "https://github.com/MC-kit/xpypact/releases"
 
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-duckdb = ">=0.7.1"
+duckdb = ">=0.8.0"
 h5netcdf = ">=0.13.1"
 mckit-nuclides = {version = ">=0.1.1", allow-prereleases = true}
 numpy = ">=1.24.2"
 openpyxl = ">=3.0.9"
 orjson = ">=3.6.7"
 pandas = ">=2.0.0"
 xarray = ">=2022.3.0"
@@ -408,15 +408,15 @@
     "DJ", # flake8-django
     "D", # pydocstyle
     "DTZ", # flake8-datetimez
     "EM", # flake8-errmsg
     "ERA", # eradicate
     "E", # pycodestyle
     "EXE", # flake8-executable
-    "FBT", # flake8-boolean-trap
+    "FBT", # flake8-boolean-trap  https://adamj.eu/tech/2021/07/10/python-type-hints-how-to-avoid-the-boolean-trap
     "F", # Pyflakes
     "G", # flake8-logging-format
     "ICN", # flake8-import-conventions
     "I", # isort
     "INP", # flake8-no-pep420
     "ISC", # flake8-implicit-str-concat
     "N", # pep8-naming
@@ -458,14 +458,16 @@
     # "ARG001", # Unused function argument: `expected`
 
     "B905",   # B905 `zip()` without an explicit `strict=` parameter - ignore while support 3.8, 3.9
 
     # "C812",   # C812 Missing trailing comma: black compatibility
     # "C901",   # too complex - ...
 
+    # "COM812", #  [*] Trailing comma missing
+
     # "D100",   # Missing docstring in public module
     # "D101",   # Missing docstring in public class
     # "D102",   # Missing docstring in public method
     # "D103",   # Missing docstring in public function
     "D105",   # D105 Missing docstring in magic method (__hash__, __eq__)
     # "D104",   # Missing docstring in public package
     # "D106",   # Missing docstring in public nested class
```

### Comparing `xpypact-0.4.0/src/xpypact/__init__.py` & `xpypact-0.4.1/src/xpypact/__init__.py`

 * *Files identical despite different names*

### Comparing `xpypact-0.4.0/src/xpypact/dao/api.py` & `xpypact-0.4.1/src/xpypact/dao/api.py`

 * *Files identical despite different names*

### Comparing `xpypact-0.4.0/src/xpypact/dao/duckdb/create_schema.sql` & `xpypact-0.4.1/src/xpypact/dao/duckdb/create_schema.sql`

 * *Files identical despite different names*

### Comparing `xpypact-0.4.0/src/xpypact/dao/duckdb/implementation.py` & `xpypact-0.4.1/src/xpypact/dao/duckdb/implementation.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,15 +208,15 @@
             sql = f"""
                 copy
                 (select * from frame)
                 to '{path}'
                 (
                     format parquet,
                     partition_by ({time_step_partition}material_id, case_id),
-                    allow_overwrite 1
+                    overwrite_or_ignore true
                 )
                 """  # noqa: S608 - sql injection
             con.execute(sql)
     finally:
         con.close()
```

### Comparing `xpypact-0.4.0/src/xpypact/data_arrays.py` & `xpypact-0.4.1/src/xpypact/data_arrays.py`

 * *Files identical despite different names*

### Comparing `xpypact-0.4.0/src/xpypact/data_frames.py` & `xpypact-0.4.1/src/xpypact/data_frames.py`

 * *Files identical despite different names*

### Comparing `xpypact-0.4.0/src/xpypact/fluxes.py` & `xpypact-0.4.1/src/xpypact/fluxes.py`

 * *Files identical despite different names*

### Comparing `xpypact-0.4.0/src/xpypact/inventory.py` & `xpypact-0.4.1/src/xpypact/inventory.py`

 * *Files identical despite different names*

### Comparing `xpypact-0.4.0/src/xpypact/nuclide.py` & `xpypact-0.4.1/src/xpypact/nuclide.py`

 * *Files identical despite different names*

### Comparing `xpypact-0.4.0/src/xpypact/run_data.py` & `xpypact-0.4.1/src/xpypact/run_data.py`

 * *Files identical despite different names*

### Comparing `xpypact-0.4.0/src/xpypact/time_step.py` & `xpypact-0.4.1/src/xpypact/time_step.py`

 * *Files identical despite different names*

### Comparing `xpypact-0.4.0/src/xpypact/utils/io.py` & `xpypact-0.4.1/src/xpypact/utils/io.py`

 * *Files identical despite different names*

### Comparing `xpypact-0.4.0/src/xpypact/utils/resource.py` & `xpypact-0.4.1/src/xpypact/utils/resource.py`

 * *Files identical despite different names*

### Comparing `xpypact-0.4.0/PKG-INFO` & `xpypact-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xpypact
-Version: 0.4.0
+Version: 0.4.1
 Summary: "Python tools to work with elements and isotopes"
 Home-page: https://github.com/MC-kit/xpypact
 License: MIT
 Keywords: element,nuclide,isotope,abundance,FISPACT,activation,duckdb,parquet
 Author: dvp
 Author-email: dmitri_portnov@yahoo.com
 Requires-Python: >=3.8.1,<4.0
@@ -16,15 +16,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Dist: duckdb (>=0.7.1)
+Requires-Dist: duckdb (>=0.8.0)
 Requires-Dist: h5netcdf (>=0.13.1)
 Requires-Dist: mckit-nuclides (>=0.1.1)
 Requires-Dist: multipledispatch (>=0.6.0)
 Requires-Dist: numpy (>=1.24.2)
 Requires-Dist: openpyxl (>=3.0.9)
 Requires-Dist: orjson (>=3.6.7)
 Requires-Dist: pandas (>=2.0.0)
```

