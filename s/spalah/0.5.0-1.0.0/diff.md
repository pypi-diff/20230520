# Comparing `tmp/spalah-0.5.0.tar.gz` & `tmp/spalah-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spalah-0.5.0.tar", last modified: Sun Jan 22 09:27:54 2023, max compression
+gzip compressed data, was "spalah-1.0.0.tar", max compression
```

## Comparing `spalah-0.5.0.tar` & `spalah-1.0.0.tar`

### file list

```diff
@@ -1,43 +1,13 @@
-drwxr-xr-x   0 alexandrvolok   (501) staff       (20)        0 2023-01-22 09:27:54.129917 spalah-0.5.0/
--rw-r--r--   0 alexandrvolok   (501) staff       (20)    10244 2022-10-02 15:22:43.000000 spalah-0.5.0/.DS_Store
--rw-r--r--   0 alexandrvolok   (501) staff       (20)      292 2022-07-09 12:46:46.000000 spalah-0.5.0/.editorconfig
--rw-r--r--   0 alexandrvolok   (501) staff       (20)       80 2022-07-11 19:03:39.000000 spalah-0.5.0/.flake8
-drwxr-xr-x   0 alexandrvolok   (501) staff       (20)        0 2023-01-22 09:27:54.126451 spalah-0.5.0/.github/
--rw-r--r--   0 alexandrvolok   (501) staff       (20)      329 2022-07-09 12:46:46.000000 spalah-0.5.0/.github/ISSUE_TEMPLATE.md
-drwxr-xr-x   0 alexandrvolok   (501) staff       (20)        0 2023-01-22 09:27:54.126857 spalah-0.5.0/.github/workflows/
--rw-r--r--   0 alexandrvolok   (501) staff       (20)      499 2022-07-09 12:46:46.000000 spalah-0.5.0/.github/workflows/semantic_release.yaml
--rw-r--r--   0 alexandrvolok   (501) staff       (20)     1257 2022-07-17 14:04:38.000000 spalah-0.5.0/.github/workflows/spalah_ci.yaml
--rw-r--r--   0 alexandrvolok   (501) staff       (20)     1204 2022-07-09 12:46:46.000000 spalah-0.5.0/.gitignore
--rw-r--r--   0 alexandrvolok   (501) staff       (20)      974 2022-10-11 15:35:20.000000 spalah-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0 alexandrvolok   (501) staff       (20)     2208 2023-01-22 09:27:51.000000 spalah-0.5.0/CHANGELOG.md
--rw-r--r--   0 alexandrvolok   (501) staff       (20)     1217 2022-07-09 12:46:46.000000 spalah-0.5.0/LICENSE
--rw-r--r--   0 alexandrvolok   (501) staff       (20)     5992 2023-01-22 09:27:54.129994 spalah-0.5.0/PKG-INFO
--rw-r--r--   0 alexandrvolok   (501) staff       (20)     5258 2023-01-22 09:27:43.000000 spalah-0.5.0/README.md
--rw-r--r--   0 alexandrvolok   (501) staff       (20)    12244 2022-10-02 15:22:43.000000 spalah-0.5.0/delta.ipynb
-drwxr-xr-x   0 alexandrvolok   (501) staff       (20)        0 2023-01-22 09:27:54.127440 spalah-0.5.0/docs/
--rw-r--r--   0 alexandrvolok   (501) staff       (20)     8717 2023-01-22 09:27:43.000000 spalah-0.5.0/docs/examples_dataframe.md
--rw-r--r--   0 alexandrvolok   (501) staff       (20)     1477 2022-10-11 15:35:20.000000 spalah-0.5.0/docs/examples_datalake.md
--rw-r--r--   0 alexandrvolok   (501) staff       (20)    10426 2022-08-05 10:52:40.000000 spalah-0.5.0/docs/usage.ipynb
--rw-r--r--   0 alexandrvolok   (501) staff       (20)      209 2022-10-02 15:22:43.000000 spalah-0.5.0/requirements_dev.txt
--rw-r--r--   0 alexandrvolok   (501) staff       (20)      541 2023-01-22 09:27:54.130266 spalah-0.5.0/setup.cfg
--rw-r--r--   0 alexandrvolok   (501) staff       (20)     1279 2023-01-22 09:27:51.000000 spalah-0.5.0/setup.py
-drwxr-xr-x   0 alexandrvolok   (501) staff       (20)        0 2023-01-22 09:27:54.127892 spalah-0.5.0/spalah/
--rw-r--r--   0 alexandrvolok   (501) staff       (20)      118 2022-07-09 12:46:46.000000 spalah-0.5.0/spalah/__init__.py
--rw-r--r--   0 alexandrvolok   (501) staff       (20)    19836 2023-01-22 09:27:43.000000 spalah-0.5.0/spalah/dataframe.py
--rw-r--r--   0 alexandrvolok   (501) staff       (20)     5441 2022-10-11 15:35:20.000000 spalah-0.5.0/spalah/datalake.py
-drwxr-xr-x   0 alexandrvolok   (501) staff       (20)        0 2023-01-22 09:27:54.128666 spalah-0.5.0/spalah.egg-info/
--rw-r--r--   0 alexandrvolok   (501) staff       (20)     5992 2023-01-22 09:27:54.000000 spalah-0.5.0/spalah.egg-info/PKG-INFO
--rw-r--r--   0 alexandrvolok   (501) staff       (20)      796 2023-01-22 09:27:54.000000 spalah-0.5.0/spalah.egg-info/SOURCES.txt
--rw-r--r--   0 alexandrvolok   (501) staff       (20)        1 2023-01-22 09:27:54.000000 spalah-0.5.0/spalah.egg-info/dependency_links.txt
--rw-r--r--   0 alexandrvolok   (501) staff       (20)        1 2022-07-10 09:23:33.000000 spalah-0.5.0/spalah.egg-info/not-zip-safe
--rw-r--r--   0 alexandrvolok   (501) staff       (20)        7 2023-01-22 09:27:54.000000 spalah-0.5.0/spalah.egg-info/top_level.txt
-drwxr-xr-x   0 alexandrvolok   (501) staff       (20)        0 2023-01-22 09:27:54.129792 spalah-0.5.0/tests/
--rw-r--r--   0 alexandrvolok   (501) staff       (20)       36 2022-07-09 12:46:46.000000 spalah-0.5.0/tests/__init__.py
--rw-r--r--   0 alexandrvolok   (501) staff       (20)     6503 2023-01-22 09:27:43.000000 spalah-0.5.0/tests/conftest.py
--rw-r--r--   0 alexandrvolok   (501) staff       (20)     3202 2022-10-02 15:22:43.000000 spalah-0.5.0/tests/test_SchemaComparer.py
--rw-r--r--   0 alexandrvolok   (501) staff       (20)      987 2022-10-02 15:22:43.000000 spalah-0.5.0/tests/test_dataframe_script_dataframe.py
--rw-r--r--   0 alexandrvolok   (501) staff       (20)    12526 2023-01-22 09:27:43.000000 spalah-0.5.0/tests/test_dataframe_slice_dataframe.py
--rw-r--r--   0 alexandrvolok   (501) staff       (20)     1372 2022-10-11 15:35:20.000000 spalah-0.5.0/tests/test_datalake_get_table_properties.py
--rw-r--r--   0 alexandrvolok   (501) staff       (20)     3413 2022-10-11 15:35:20.000000 spalah-0.5.0/tests/test_datalake_set_table_properties.py
--rw-r--r--   0 alexandrvolok   (501) staff       (20)     2226 2022-10-02 15:22:43.000000 spalah-0.5.0/tests/test_flatten_schema.py
--rw-r--r--   0 alexandrvolok   (501) staff       (20)      537 2022-07-09 12:46:46.000000 spalah-0.5.0/tox.ini
+-rw-r--r--   0        0        0     1217 2022-07-09 12:46:46.000000 spalah-1.0.0/LICENSE
+-rw-r--r--   0        0        0     5356 2023-05-20 17:48:37.703026 spalah-1.0.0/README.md
+-rw-r--r--   0        0        0     1312 2023-05-20 17:50:57.279488 spalah-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      118 2022-07-09 12:46:46.000000 spalah-1.0.0/spalah/__init__.py
+-rw-r--r--   0        0        0      177 2023-05-20 17:33:36.517825 spalah-1.0.0/spalah/dataframe/__init__.py
+-rw-r--r--   0        0        0    23329 2023-05-20 17:33:36.518032 spalah-1.0.0/spalah/dataframe/dataframe.py
+-rw-r--r--   0        0        0     8813 2023-05-20 17:33:36.518182 spalah-1.0.0/spalah/dataset/DeltaProperty.py
+-rw-r--r--   0        0        0      144 2023-05-20 17:33:36.518286 spalah-1.0.0/spalah/dataset/__init__.py
+-rw-r--r--   0        0        0      999 2023-05-20 17:33:36.518399 spalah-1.0.0/spalah/dataset/dbfs.py
+-rw-r--r--   0        0        0       58 2023-05-20 17:33:36.518507 spalah-1.0.0/spalah/shared/__init__.py
+-rw-r--r--   0        0        0      407 2023-05-20 17:33:36.518606 spalah-1.0.0/spalah/shared/logging.py
+-rw-r--r--   0        0        0     6663 1970-01-01 00:00:00.000000 spalah-1.0.0/setup.py
+-rw-r--r--   0        0        0     6741 1970-01-01 00:00:00.000000 spalah-1.0.0/PKG-INFO
```

### Comparing `spalah-0.5.0/LICENSE` & `spalah-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spalah-0.5.0/PKG-INFO` & `spalah-1.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,50 @@
 Metadata-Version: 2.1
 Name: spalah
-Version: 0.5.0
+Version: 1.0.0
 Summary: Spalah is a set of PySpark dataframe helpers
 Home-page: https://github.com/avolok/spalah
+License: MIT
+Keywords: spalah
 Author: Alex Volok
 Author-email: alexandr.volok@gmail.com
-License: MIT license
-Keywords: spalah
-Platform: UNKNOWN
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Requires-Dist: black (==22.3.0)
+Requires-Dist: bump2version (==1.0.1)
+Requires-Dist: coverage (==6.4.1)
+Requires-Dist: delta-spark (==2.1.0)
+Requires-Dist: flake8 (==6.0.0)
+Requires-Dist: packaging
+Requires-Dist: pip
+Requires-Dist: pre-commit (==2.19.0)
+Requires-Dist: pyspark (==3.3.0)
+Requires-Dist: pytest (==7.1.2)
+Requires-Dist: pytest-cov (==3.0.0)
+Requires-Dist: ruff
+Requires-Dist: tox (==3.25.0)
+Requires-Dist: twine (==4.0.1)
+Requires-Dist: watchdog (==2.1.9)
+Requires-Dist: wheel
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # spalah
 
-Spalah is a set of python helpers to deal with PySpark dataframes, transformations, schemas etc.
+Spalah is a set of python helpers to deal with PySpark dataframes, transformations, schemas and Delta Tables.
 
 The word "spalah" means "spark" in Ukrainian 🇺🇦 
 
 # Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install spalah.
 
@@ -171,55 +189,55 @@
         data_type='StringType', 
         reason='The column exists only in the source schema'
     )
 ]
 """
 ```
 
-## spalah.datalake
+## spalah.dataset
 
-### get_delta_properties
+### Get delta table properties
 
 ```python
-from spalah.datalake import get_delta_properties
+from spalah.dataset import DeltaProperty
 
-table_properties = get_delta_properties(table_path="/path/dataset")
+dp = DeltaProperty(table_path="/path/dataset")
 
-print(table_properties) 
+print(dp.properties) 
 
 # output: 
 # {'delta.deletedFileRetentionDuration': 'interval 15 days'}
 ```
 
-### set_delta_properties
+### Set delta table properties
 
 ```python
-from spalah.datalake import set_delta_properties
+rom spalah.dataset import DeltaProperty
+
+dp = DeltaProperty(table_path="/path/dataset")
+
+dp.properties = {
+    "delta.logRetentionDuration": "interval 10 days",
+    "delta.deletedFileRetentionDuration": "interval 15 days"
+}
 
-set_delta_properties(
-    table_path='/path/dataset',
-    properties={
-        "delta.logRetentionDuration": "interval 10 days",
-        "delta.deletedFileRetentionDuration": "interval 15 days"
-    }
-)
 ```
 and the standard output is:
+
 ```
-Applying table properties on 'delta.`/path/dataset`':
- - Checking if 'delta.logRetentionDuration = interval 10 days' is set on delta.`/path/dataset`
-   Result: The property has been set
- - Checking if 'delta.deletedFileRetentionDuration = interval 15 days' is set on delta.`/path/dataset`
-   Result: The property has been set
+2023-05-20 18:27:42,070 INFO      Applying check constraints on 'delta.`/tmp/nested_schema_dataset`':
+2023-05-20 18:27:42,071 INFO      Checking if constraint 'id_is_not_null' was already set on delta.`/tmp/nested_schema_dataset`
+2023-05-20 18:27:42,433 INFO      The constraint id_is_not_null has been successfully added to 'delta.`/tmp/nested_schema_dataset`
 ```
 
-Check for more information in [examples: dataframe](docs/examples_dataframe.md), [examples: datalake](docs/examples_datalake.md) pages and related [notebook](docs/usage.ipynb)
+Please note that check constraints can be retrieved and set using property: `.check_constraints`
+
+Check for more information in [examples: dataframe](docs/examples/dataframe.md), [examples: datalake](docs/examples/dataset.md) pages and related [notebook](docs/usage.ipynb)
 
 ## Contributing
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
 
 ## License
 [MIT](https://choosealicense.com/licenses/mit/)
 
-
```

### Comparing `spalah-0.5.0/README.md` & `spalah-1.0.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # spalah
 
-Spalah is a set of python helpers to deal with PySpark dataframes, transformations, schemas etc.
+Spalah is a set of python helpers to deal with PySpark dataframes, transformations, schemas and Delta Tables.
 
 The word "spalah" means "spark" in Ukrainian 🇺🇦 
 
 # Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install spalah.
 
@@ -149,52 +149,53 @@
         data_type='StringType', 
         reason='The column exists only in the source schema'
     )
 ]
 """
 ```
 
-## spalah.datalake
+## spalah.dataset
 
-### get_delta_properties
+### Get delta table properties
 
 ```python
-from spalah.datalake import get_delta_properties
+from spalah.dataset import DeltaProperty
 
-table_properties = get_delta_properties(table_path="/path/dataset")
+dp = DeltaProperty(table_path="/path/dataset")
 
-print(table_properties) 
+print(dp.properties) 
 
 # output: 
 # {'delta.deletedFileRetentionDuration': 'interval 15 days'}
 ```
 
-### set_delta_properties
+### Set delta table properties
 
 ```python
-from spalah.datalake import set_delta_properties
+rom spalah.dataset import DeltaProperty
+
+dp = DeltaProperty(table_path="/path/dataset")
+
+dp.properties = {
+    "delta.logRetentionDuration": "interval 10 days",
+    "delta.deletedFileRetentionDuration": "interval 15 days"
+}
 
-set_delta_properties(
-    table_path='/path/dataset',
-    properties={
-        "delta.logRetentionDuration": "interval 10 days",
-        "delta.deletedFileRetentionDuration": "interval 15 days"
-    }
-)
 ```
 and the standard output is:
+
 ```
-Applying table properties on 'delta.`/path/dataset`':
- - Checking if 'delta.logRetentionDuration = interval 10 days' is set on delta.`/path/dataset`
-   Result: The property has been set
- - Checking if 'delta.deletedFileRetentionDuration = interval 15 days' is set on delta.`/path/dataset`
-   Result: The property has been set
+2023-05-20 18:27:42,070 INFO      Applying check constraints on 'delta.`/tmp/nested_schema_dataset`':
+2023-05-20 18:27:42,071 INFO      Checking if constraint 'id_is_not_null' was already set on delta.`/tmp/nested_schema_dataset`
+2023-05-20 18:27:42,433 INFO      The constraint id_is_not_null has been successfully added to 'delta.`/tmp/nested_schema_dataset`
 ```
 
-Check for more information in [examples: dataframe](docs/examples_dataframe.md), [examples: datalake](docs/examples_datalake.md) pages and related [notebook](docs/usage.ipynb)
+Please note that check constraints can be retrieved and set using property: `.check_constraints`
+
+Check for more information in [examples: dataframe](docs/examples/dataframe.md), [examples: datalake](docs/examples/dataset.md) pages and related [notebook](docs/usage.ipynb)
 
 ## Contributing
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
 
 ## License
```

### Comparing `spalah-0.5.0/spalah/dataframe.py` & `spalah-1.0.0/spalah/dataframe/dataframe.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+"""This module contains various dataframe specific functions and classes"""
+
 import copy
+from collections import namedtuple
 from pprint import pformat, pprint
-from typing import Union, List, Set
+from typing import List, Set, Union
 
 from pyspark.sql import DataFrame
 from pyspark.sql import functions as F
 from pyspark.sql import types as T
-from collections import namedtuple
-
 
 MatchedColumn = namedtuple("MatchedColumn", ["name", "data_type"])
 NotMatchedColumn = namedtuple("NotMatchedColumn", ["name", "data_type", "reason"])
 
 
 def __remove_suffix(input_string: str, suffix: str) -> str:
     """Remove suffix from string if it exists
@@ -86,19 +87,17 @@
         include_this_node = True
     # If no columns to include specified, then all columns are accepted
     elif not columns_to_include or len(columns_to_include) == 0:
         include_this_node = True
 
     # Structs
     if isinstance(node.dataType, T.StructType):
-
         children = []
 
         for field in node.dataType.fields:
-
             if isinstance(field.dataType, T.StructType) and array_element is not None:
                 array_col_child = array_element[field.name]
             elif array_element is not None:
                 array_col_child = array_element
             else:
                 array_col_child = None
 
@@ -122,15 +121,14 @@
     elif (
         isinstance(node.dataType, T.ArrayType)
         and isinstance(node.dataType.elementType, T.StructType)
         and
         # to include this node only when it must appear in the final projection
         (nullify_only or include_this_node)
     ):
-
         children = []
 
         def _transform_array(array_element: F.col) -> F.col:
             """Internal function to process elements of an array
             one by one and return the transformed array
 
             Args:
@@ -142,15 +140,17 @@
 
             # converts schema node array(struct()) -> struct()
             struct_in_array_node = copy.deepcopy(node)
             struct_in_array_node.dataType = node.dataType.elementType
 
             # removes the name of the array node from the element path
             # because the existence of the array does not create a new level in the path
-            column_prefix_new = __remove_suffix(__remove_suffix(column_prefix, node_name), ".")
+            column_prefix_new = __remove_suffix(
+                __remove_suffix(column_prefix, node_name), "."
+            )
 
             struct_extracted_from_array_element = __process_schema_node(
                 node=struct_in_array_node,
                 column_prefix=column_prefix_new,
                 columns_to_include=columns_to_include,
                 columns_to_exclude=columns_to_exclude,
                 nullify_only=nullify_only,
@@ -163,21 +163,20 @@
         # the array path is the element path
         # otherwise, the array path is child node of the parent array
         if array_element is None:
             array_path = column_prefix
         else:
             array_path = array_element[node_name]
 
-        col_expression = F.transform(array_path, lambda x: _transform_array(array_element=x)).alias(
-            node_name
-        )
+        col_expression = F.transform(
+            array_path, lambda x: _transform_array(array_element=x)
+        ).alias(node_name)
 
     # Regular columns
     else:
-
         # get node data type
         # In case of nullification of array it converted to a string null value
         if isinstance(node.dataType, T.ArrayType):
             node_type = T.StringType()  # arrays will be nullified and casted as strings
         else:
             node_type = node.dataType
 
@@ -195,15 +194,14 @@
 
     if include_this_node and debug:
         print(f" - {column_prefix}")
 
     if include_this_node and not is_struct_without_children:
         return col_expression
     if not include_this_node and nullify_only:
-
         if is_struct:
             return col_expression
         else:
             return nullified_col_expression
     else:
         return None
 
@@ -222,35 +220,60 @@
         input_dataframe (DataFrame): Input dataframe
         columns_to_include (list): Columns that must remain in the dataframe unchanged
         columns_to_exclude (list): Columns that must be removed (or nullified)
         nullify_only (bool, optional): Nullify columns instead of removing them. Defaults to False
         debug (bool, optional): For extra debug output. Defaults to False.
 
     Raises:
-        TypeError: If the 'column_to_include' or 'column_to_exclude' are not lists
+        TypeError: If the 'column_to_include' or 'column_to_exclude' are not type list
         ValueError: If the included columns overlay excluded columns, so nothing to return
 
     Returns:
         DataFrame: The processed dataframe
+
+    Examples:
+        >>> from spalah.dataframe import slice_dataframe
+        >>> df = spark.sql(
+        ...         'SELECT 1 as ID, "John" AS Name,
+        ...         struct("line1" AS Line1, "line2" AS Line2) AS Address'
+        ...     )
+        >>> df_sliced = slice_dataframe(
+        ...     input_dataframe=df,
+        ...     columns_to_include=["Name", "Address"],
+        ...     columns_to_exclude=["Address.Line2"]
+        ... )
+
+        As the result, the dataframe will contain only the columns `Name` and `Address.Line1` \
+            because `Name` and `Address` are included and a nested element `Address.Line2` is \
+            excluded
+        >>> df_result.printSchema()
+        root
+        |-- Name: string (nullable = false)
+        |-- Address: struct (nullable = false)
+        |    |-- Line1: string (nullable = false)
     """
 
     projection = []
     _schema = input_dataframe.schema
 
     if not columns_to_include:
         columns_to_include = []
 
     if not columns_to_exclude:
         columns_to_exclude = []
 
     if not (type(columns_to_include) is list and type(columns_to_exclude) is list):
         raise TypeError("'columns_to_include' and 'columns_to_exclude' must be a list")
 
-    if not all(isinstance(item, str) for item in columns_to_include + columns_to_exclude):
-        raise TypeError("Member of 'columns_to_include' and 'columns_to_exclude' must be a string")
+    if not all(
+        isinstance(item, str) for item in columns_to_include + columns_to_exclude
+    ):
+        raise TypeError(
+            "Member of 'columns_to_include' and 'columns_to_exclude' must be a string"
+        )
 
     if debug:
         print("The list of columns to include:")
         pprint(columns_to_include)
 
         print("The list of columns to exclude:")
         pprint(columns_to_exclude)
@@ -289,23 +312,31 @@
 
 
 def flatten_schema(
     schema: T.StructType,
     include_datatype: bool = False,
     column_prefix: Union[str, None] = None,
 ) -> list:
-    """Generates the flatten list of columns from the complex dataframe schema
+    """Parses spark dataframe schema and returns the list of columns
+    If the schema is nested, the columns are flattened
 
     Args:
-        schema (StructType): input dataframe's schema
-        include_type (bool, optional): Include column types
-        column_prefix (str, optional): The column name prefix. Defaults to None.
+        schema (StructType): Input dataframe schema
+        include_type (bool, optional): Flag to include column types
+        column_prefix (str, optional): Column name prefix. Defaults to None.
 
     Returns:
         The list of (flattened) column names
+
+    Examples:
+        >>> from spalah.dataframe import flatten_schema
+        >>> flatten_schema(schema=df_complex_schema.schema)
+
+        returns the list of columns, nested are flattened:
+        >>> ['ID', 'Name', 'Address.Line1', 'Address.Line2']
     """
 
     if not isinstance(schema, T.StructType):
         raise TypeError("Parameter schema must be a StructType")
 
     columns = []
 
@@ -333,25 +364,45 @@
                 result = name
 
             columns.append(result)
 
     return columns
 
 
-def script_dataframe(input_dataframe: DataFrame, suppress_print_output: bool = True) -> str:
+def script_dataframe(
+    input_dataframe: DataFrame, suppress_print_output: bool = True
+) -> str:
+    """Generate a script to recreate the dataframe
+    The script includes the schema and the data
+
+    Args:
+        input_dataframe (DataFrame): Input spark dataframe
+        suppress_print_output (bool, optional): Disable prints to console. \
+            Defaults to True.
 
-    """Generates a script of a dataframe"""
+    Raises:
+        ValueError: when the dataframe is too large (by default > 20 rows)
+
+    Returns:
+        The script to recreate the dataframe
+
+    Examples:
+        >>> from spalah.dataframe import script_dataframe
+        >>> script = script_dataframe(input_dataframe=df)
+        >>> print(script)
+    """
 
     MAX_ROWS_IN_SCRIPT = 20
 
     __dataframe = input_dataframe
 
     if __dataframe.count() > MAX_ROWS_IN_SCRIPT:
         raise ValueError(
-            "This method is limited to script up " f"to {MAX_ROWS_IN_SCRIPT} row(s) per call"
+            "This method is limited to script up "
+            f"to {MAX_ROWS_IN_SCRIPT} row(s) per call"
         )
 
     __schema = input_dataframe.schema.jsonValue()
 
     __script_lines = [
         "from pyspark.sql import Row",
         "import datetime",
@@ -379,19 +430,42 @@
         print("")
         print(__final_script)
 
     return __final_script
 
 
 class SchemaComparer:
-    def __init__(self, source_schema: T.StringType, target_schema: T.StringType) -> None:
+    """
+    The SchemaComparer is to compare two spark dataframe schemas and find matched
+    and not matched columns.
+    """
+
+    def __init__(
+        self, source_schema: T.StringType, target_schema: T.StringType
+    ) -> None:
+        """Constructs all the necessary input attributes for the SchemaComparer object.
+
+        Args:
+            source_schema (T.StringType): source schema to match
+            target_schema (T.StringType): target schema to match
+
+        Examples:
+            >>> from spalah.dataframe import SchemaComparer
+            >>> schema_comparer = SchemaComparer(
+            ...     source_schema = df_source.schema,
+            ...     target_schema = df_target.schema
+            ... )
+        """
         self._source = self.__import_schema(source_schema)
         self._target = self.__import_schema(target_schema)
+
         self.matched: List[tuple] = list()
+        """List of matched columns"""
         self.not_matched: List[tuple] = list()
+        """The list of not matched columns"""
 
     def __import_schema(self, input_schema: T.StructType) -> Set[tuple]:
         """Import StructType as the flatten set of tuples: (column_name, data_type)
 
         Args:
             input_schema (T.StructType): Schema to process
 
@@ -460,15 +534,15 @@
         """
 
         def _remove(input_value: Set[tuple], subtract_value: Set[tuple]) -> Set[tuple]:
             """Internal helper for removal of Tuples by the first member"""
             return {
                 (x, y)
                 for (x, y) in input_value
-                if not x.lower() in ([z[0].lower() for z in subtract_value])
+                if x.lower() not in [z[0].lower() for z in subtract_value]
             }
 
         self._source = _remove(self._source, subtract_value)  # type: ignore
         self._target = _remove(self._target, subtract_value)  # type: ignore
 
     def __lower_column_names(self, base_value: Set[tuple]) -> Set[tuple]:
         """Lower-case all column names of the input set
@@ -514,17 +588,21 @@
             result,  # type: ignore
             "The column exists in source and target schemas but it is not matched by a data type",
         )
 
     def __process_remaining_non_matched_columns(self) -> None:
         """Process remaining not matched columns"""
 
-        self.__populate_not_matched(self._source, "The column exists only in the source schema")
+        self.__populate_not_matched(
+            self._source, "The column exists only in the source schema"
+        )
 
-        self.__populate_not_matched(self._target, "The column exists only in the target schema")
+        self.__populate_not_matched(
+            self._target, "The column exists only in the target schema"
+        )
 
         self.__remove_matched_by_name(self._source)
         self.__remove_matched_by_name(self._target)
 
     def __populate_matched(self, input_value: Set[tuple]) -> None:
         """Populate class property 'matched' with a list of fully matched columns
 
@@ -538,25 +616,49 @@
     def __populate_not_matched(self, input_value: Set[tuple], reason: str) -> None:
         """Populate class property 'not_matched' with a list of columns that didn't match for some
         reason with included an actual reason
 
         Args:
             input_value (Set[tuple]): The set of tuples with a list of column names and data types
             reason (str): Reason for not match
+
         """
 
         for match in input_value:
             self.not_matched.append(
                 NotMatchedColumn(name=match[0], data_type=match[1], reason=reason)
             )
 
     def compare(self) -> None:
         """
-        Compares the source and target schemas and populates properties
-        'matched' and 'not_matched'
+        Compares the source and target schemas and populates properties `matched` and `not_matched`
+
+        Examples:
+            >>> # instantiate schema_comparer firstly, see example above
+            >>> schema_comparer.compare()
+
+            Get list of all columns that are matched by name and type:
+            >>> schema_comparer.matched
+            [MatchedColumn(name='Address.Line1',  data_type='StringType')]
+
+            Get unmatched columns:
+            >>> schema_comparer.not_matched
+            [
+                NotMatchedColumn(
+                    name='name',
+                    data_type='StringType',
+                    reason="The column exists in source and target schemas but it's name is \
+case-mismatched"
+                ),
+                NotMatchedColumn(
+                    name='Address.Line2',
+                    data_type='StringType',
+                    reason='The column exists only in the source schema'
+                )
+            ]
         """
 
         # Case 1: find columns that are matched by name and type and remove them
         # from further processing
         self.__match_by_name_and_type()
 
         # Case 2: find columns that match mismatched by name due to case: ID <-> Id
```

### Comparing `spalah-0.5.0/spalah.egg-info/PKG-INFO` & `spalah-1.0.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,225 +1,45 @@
-Metadata-Version: 2.1
-Name: spalah
-Version: 0.5.0
-Summary: Spalah is a set of PySpark dataframe helpers
-Home-page: https://github.com/avolok/spalah
-Author: Alex Volok
-Author-email: alexandr.volok@gmail.com
-License: MIT license
-Keywords: spalah
-Platform: UNKNOWN
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# spalah
-
-Spalah is a set of python helpers to deal with PySpark dataframes, transformations, schemas etc.
-
-The word "spalah" means "spark" in Ukrainian 🇺🇦 
-
-# Installation
-
-Use the package manager [pip](https://pip.pypa.io/en/stable/) to install spalah.
-
-```bash
-pip install spalah
-```
-
-# Examples of use
-Spalah currently has two different groups of helpers: `dataframe` and `datalake`.
-
-## spalah.dataframe
-
-### slice_dataframe
-
-```python
-from spalah.dataframe import slice_dataframe
-
-df = spark.sql(
-    'SELECT 1 as ID, "John" AS Name, struct("line1" AS Line1, "line2" AS Line2) AS Address'
-)
-df.printSchema()
-
-""" output:
-root
- |-- ID: integer (nullable = false)
- |-- Name: string (nullable = false)
- |-- Address: struct (nullable = false)
- |    |-- Line1: string (nullable = false)
- |    |-- Line2: string (nullable = false)
-"""
-
-# Create a new dataframe by cutting of root and nested attributes
-df_result = slice_dataframe(
-    input_dataframe=df,
-    columns_to_include=["Name", "Address"],
-    columns_to_exclude=["Address.Line2"]
-)
-df_result.printSchema()
-
-""" output:
-root
- |-- Name: string (nullable = false)
- |-- Address: struct (nullable = false)
- |    |-- Line1: string (nullable = false)
-"""
-```
-
-Beside of nested regular structs it also supported slicing of structs in arrays, including multiple levels of nesting
-
-
-### flatten_schema
-
-```python
-from spalah.dataframe import flatten_schema
-
-# Pass the sample dataframe to get the list of all attributes as single dimension list
-flatten_schema(df_complex_schema.schema)
-
-""" output:
-['ID', 'Name', 'Address.Line1', 'Address.Line2']
-"""
-
-
-# Alternatively, the function can return data types of the attributes
-flatten_schema(
-    schema=df_complex_schema.schema,
-    include_datatype=True
-)
-
-""" output:
-[
-    ('ID', 'IntegerType'),
-    ('Name', 'StringType'),
-    ('Address.Line1', 'StringType'),
-    ('Address.Line2', 'StringType')
-]
-"""
-```
-
-### script_dataframe
-
-```python
-from spalah.dataframe import script_dataframe
-
-script = script_dataframe(df)
-
-print(script)
-
-""" output:
-from pyspark.sql import Row
-import datetime
-from decimal import Decimal
-from pyspark.sql.types import *
-
-# Scripted data and schema:
-__data = [Row(ID=1, Name='John', Address=Row(Line1='line1', Line2='line2'))]
-
-__schema = {'type': 'struct', 'fields': [{'name': 'ID', 'type': 'integer', 'nullable': False, 'metadata': {}}, {'name': 'Name', 'type': 'string', 'nullable': False, 'metadata': {}}, {'name': 'Address', 'type': {'type': 'struct', 'fields': [{'name': 'Line1', 'type': 'string', 'nullable': False, 'metadata': {}}, {'name': 'Line2', 'type': 'string', 'nullable': False, 'metadata': {}}]}, 'nullable': False, 'metadata': {}}]}
-
-outcome_dataframe = spark.createDataFrame(__data, StructType.fromJson(__schema))
-"""
-```
-
-### SchemaComparer
-
-```python
-from spalah.dataframe import SchemaComparer
-
-schema_comparer = SchemaComparer(
-    source_schema = df_source.schema,
-    target_schema = df_target.schema
-)
-
-schema_comparer.compare()
-
-# The comparison results are stored in the class instance properties `matched` and `not_matched`
-
-# Contains a list of matched columns:
-schema_comparer.matched
-
-""" output:
-[MatchedColumn(name='Address.Line1',  data_type='StringType')]
-"""
-
-# Contains a list of all not matched columns with a reason as description of non-match:
-schema_comparer.not_matched
-
-""" output:
-[
-    NotMatchedColumn(
-        name='name', 
-        data_type='StringType', 
-        reason="The column exists in source and target schemas but it's name is case-mismatched"
-    ),
-    NotMatchedColumn(
-        name='ID', 
-        data_type='IntegerType <=> StringType', 
-        reason='The column exists in source and target schemas but it is not matched by a data type'
-    ),
-    NotMatchedColumn(
-        name='Address.Line2', 
-        data_type='StringType', 
-        reason='The column exists only in the source schema'
-    )
-]
-"""
-```
-
-## spalah.datalake
-
-### get_delta_properties
-
-```python
-from spalah.datalake import get_delta_properties
-
-table_properties = get_delta_properties(table_path="/path/dataset")
-
-print(table_properties) 
-
-# output: 
-# {'delta.deletedFileRetentionDuration': 'interval 15 days'}
-```
-
-### set_delta_properties
-
-```python
-from spalah.datalake import set_delta_properties
-
-set_delta_properties(
-    table_path='/path/dataset',
-    properties={
-        "delta.logRetentionDuration": "interval 10 days",
-        "delta.deletedFileRetentionDuration": "interval 15 days"
-    }
-)
-```
-and the standard output is:
-```
-Applying table properties on 'delta.`/path/dataset`':
- - Checking if 'delta.logRetentionDuration = interval 10 days' is set on delta.`/path/dataset`
-   Result: The property has been set
- - Checking if 'delta.deletedFileRetentionDuration = interval 15 days' is set on delta.`/path/dataset`
-   Result: The property has been set
-```
-
-Check for more information in [examples: dataframe](docs/examples_dataframe.md), [examples: datalake](docs/examples_datalake.md) pages and related [notebook](docs/usage.ipynb)
+# -*- coding: utf-8 -*-
+from setuptools import setup
 
-## Contributing
-Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
+packages = \
+['spalah', 'spalah.dataframe', 'spalah.dataset', 'spalah.shared']
 
-Please make sure to update tests as appropriate.
+package_data = \
+{'': ['*']}
 
-## License
-[MIT](https://choosealicense.com/licenses/mit/)
+install_requires = \
+['black==22.3.0',
+ 'bump2version==1.0.1',
+ 'coverage==6.4.1',
+ 'delta-spark==2.1.0',
+ 'flake8==6.0.0',
+ 'packaging',
+ 'pip',
+ 'pre-commit==2.19.0',
+ 'pyspark==3.3.0',
+ 'pytest-cov==3.0.0',
+ 'pytest==7.1.2',
+ 'ruff',
+ 'tox==3.25.0',
+ 'twine==4.0.1',
+ 'watchdog==2.1.9',
+ 'wheel']
+
+setup_kwargs = {
+    'name': 'spalah',
+    'version': '1.0.0',
+    'description': 'Spalah is a set of PySpark dataframe helpers',
+    'long_description': '# spalah\n\nSpalah is a set of python helpers to deal with PySpark dataframes, transformations, schemas and Delta Tables.\n\nThe word "spalah" means "spark" in Ukrainian 🇺🇦 \n\n# Installation\n\nUse the package manager [pip](https://pip.pypa.io/en/stable/) to install spalah.\n\n```bash\npip install spalah\n```\n\n# Examples of use\nSpalah currently has two different groups of helpers: `dataframe` and `datalake`.\n\n## spalah.dataframe\n\n### slice_dataframe\n\n```python\nfrom spalah.dataframe import slice_dataframe\n\ndf = spark.sql(\n    \'SELECT 1 as ID, "John" AS Name, struct("line1" AS Line1, "line2" AS Line2) AS Address\'\n)\ndf.printSchema()\n\n""" output:\nroot\n |-- ID: integer (nullable = false)\n |-- Name: string (nullable = false)\n |-- Address: struct (nullable = false)\n |    |-- Line1: string (nullable = false)\n |    |-- Line2: string (nullable = false)\n"""\n\n# Create a new dataframe by cutting of root and nested attributes\ndf_result = slice_dataframe(\n    input_dataframe=df,\n    columns_to_include=["Name", "Address"],\n    columns_to_exclude=["Address.Line2"]\n)\ndf_result.printSchema()\n\n""" output:\nroot\n |-- Name: string (nullable = false)\n |-- Address: struct (nullable = false)\n |    |-- Line1: string (nullable = false)\n"""\n```\n\nBeside of nested regular structs it also supported slicing of structs in arrays, including multiple levels of nesting\n\n\n### flatten_schema\n\n```python\nfrom spalah.dataframe import flatten_schema\n\n# Pass the sample dataframe to get the list of all attributes as single dimension list\nflatten_schema(df_complex_schema.schema)\n\n""" output:\n[\'ID\', \'Name\', \'Address.Line1\', \'Address.Line2\']\n"""\n\n\n# Alternatively, the function can return data types of the attributes\nflatten_schema(\n    schema=df_complex_schema.schema,\n    include_datatype=True\n)\n\n""" output:\n[\n    (\'ID\', \'IntegerType\'),\n    (\'Name\', \'StringType\'),\n    (\'Address.Line1\', \'StringType\'),\n    (\'Address.Line2\', \'StringType\')\n]\n"""\n```\n\n### script_dataframe\n\n```python\nfrom spalah.dataframe import script_dataframe\n\nscript = script_dataframe(df)\n\nprint(script)\n\n""" output:\nfrom pyspark.sql import Row\nimport datetime\nfrom decimal import Decimal\nfrom pyspark.sql.types import *\n\n# Scripted data and schema:\n__data = [Row(ID=1, Name=\'John\', Address=Row(Line1=\'line1\', Line2=\'line2\'))]\n\n__schema = {\'type\': \'struct\', \'fields\': [{\'name\': \'ID\', \'type\': \'integer\', \'nullable\': False, \'metadata\': {}}, {\'name\': \'Name\', \'type\': \'string\', \'nullable\': False, \'metadata\': {}}, {\'name\': \'Address\', \'type\': {\'type\': \'struct\', \'fields\': [{\'name\': \'Line1\', \'type\': \'string\', \'nullable\': False, \'metadata\': {}}, {\'name\': \'Line2\', \'type\': \'string\', \'nullable\': False, \'metadata\': {}}]}, \'nullable\': False, \'metadata\': {}}]}\n\noutcome_dataframe = spark.createDataFrame(__data, StructType.fromJson(__schema))\n"""\n```\n\n### SchemaComparer\n\n```python\nfrom spalah.dataframe import SchemaComparer\n\nschema_comparer = SchemaComparer(\n    source_schema = df_source.schema,\n    target_schema = df_target.schema\n)\n\nschema_comparer.compare()\n\n# The comparison results are stored in the class instance properties `matched` and `not_matched`\n\n# Contains a list of matched columns:\nschema_comparer.matched\n\n""" output:\n[MatchedColumn(name=\'Address.Line1\',  data_type=\'StringType\')]\n"""\n\n# Contains a list of all not matched columns with a reason as description of non-match:\nschema_comparer.not_matched\n\n""" output:\n[\n    NotMatchedColumn(\n        name=\'name\', \n        data_type=\'StringType\', \n        reason="The column exists in source and target schemas but it\'s name is case-mismatched"\n    ),\n    NotMatchedColumn(\n        name=\'ID\', \n        data_type=\'IntegerType <=> StringType\', \n        reason=\'The column exists in source and target schemas but it is not matched by a data type\'\n    ),\n    NotMatchedColumn(\n        name=\'Address.Line2\', \n        data_type=\'StringType\', \n        reason=\'The column exists only in the source schema\'\n    )\n]\n"""\n```\n\n## spalah.dataset\n\n### Get delta table properties\n\n```python\nfrom spalah.dataset import DeltaProperty\n\ndp = DeltaProperty(table_path="/path/dataset")\n\nprint(dp.properties) \n\n# output: \n# {\'delta.deletedFileRetentionDuration\': \'interval 15 days\'}\n```\n\n### Set delta table properties\n\n```python\nrom spalah.dataset import DeltaProperty\n\ndp = DeltaProperty(table_path="/path/dataset")\n\ndp.properties = {\n    "delta.logRetentionDuration": "interval 10 days",\n    "delta.deletedFileRetentionDuration": "interval 15 days"\n}\n\n```\nand the standard output is:\n\n```\n2023-05-20 18:27:42,070 INFO      Applying check constraints on \'delta.`/tmp/nested_schema_dataset`\':\n2023-05-20 18:27:42,071 INFO      Checking if constraint \'id_is_not_null\' was already set on delta.`/tmp/nested_schema_dataset`\n2023-05-20 18:27:42,433 INFO      The constraint id_is_not_null has been successfully added to \'delta.`/tmp/nested_schema_dataset`\n```\n\nPlease note that check constraints can be retrieved and set using property: `.check_constraints`\n\nCheck for more information in [examples: dataframe](docs/examples/dataframe.md), [examples: datalake](docs/examples/dataset.md) pages and related [notebook](docs/usage.ipynb)\n\n## Contributing\nPull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.\n\nPlease make sure to update tests as appropriate.\n\n## License\n[MIT](https://choosealicense.com/licenses/mit/)\n',
+    'author': 'Alex Volok',
+    'author_email': 'alexandr.volok@gmail.com',
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'https://github.com/avolok/spalah',
+    'packages': packages,
+    'package_data': package_data,
+    'install_requires': install_requires,
+    'python_requires': '>=3.8.1,<4.0.0',
+}
 
 
+setup(**setup_kwargs)
```

