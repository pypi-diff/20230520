# Comparing `tmp/alacorder-80.6.8.tar.gz` & `tmp/alacorder-80.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.6.8.tar", max compression
+gzip compressed data, was "alacorder-80.6.9.tar", max compression
```

## Comparing `alacorder-80.6.8.tar` & `alacorder-80.6.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.6.8/LICENSE
--rw-r--r--   0        0        0     6455 2023-05-17 18:00:53.819885 alacorder-80.6.8/README.md
--rw-r--r--   0        0        0      746 2023-05-19 18:58:42.123143 alacorder-80.6.8/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-05-19 17:06:52.624042 alacorder-80.6.8/src/alacorder/.DS_Store
--rw-r--r--   0        0        0   234455 2023-05-18 23:58:39.588863 alacorder-80.6.8/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py
--rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.6.8/src/alacorder/__init__.py
--rw-r--r--   0        0        0   235583 2023-05-19 18:58:32.980448 alacorder-80.6.8/src/alacorder/__main__.py
--rw-r--r--   0        0        0   235583 2023-05-19 18:58:16.860704 alacorder-80.6.8/src/alacorder/alac.py
--rw-r--r--   0        0        0     7426 1970-01-01 00:00:00.000000 alacorder-80.6.8/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.6.9/LICENSE
+-rw-r--r--   0        0        0     6455 2023-05-17 18:00:53.819885 alacorder-80.6.9/README.md
+-rw-r--r--   0        0        0      746 2023-05-20 14:44:29.028389 alacorder-80.6.9/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-05-20 14:44:20.349040 alacorder-80.6.9/src/alacorder/.DS_Store
+-rw-r--r--   0        0        0   234455 2023-05-18 23:58:39.588863 alacorder-80.6.9/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py
+-rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.6.9/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   237390 2023-05-20 14:44:03.709218 alacorder-80.6.9/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   237390 2023-05-20 14:43:32.982677 alacorder-80.6.9/src/alacorder/alac.py
+-rw-r--r--   0        0        0     7426 1970-01-01 00:00:00.000000 alacorder-80.6.9/PKG-INFO
```

### Comparing `alacorder-80.6.8/LICENSE` & `alacorder-80.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.6.8/README.md` & `alacorder-80.6.9/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-80.6.8/pyproject.toml` & `alacorder-80.6.9/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.6.8"
+version = "80.6.9"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-80.6.8/src/alacorder/.DS_Store` & `alacorder-80.6.9/src/alacorder/.DS_Store`

 * *Files identical despite different names*

### Comparing `alacorder-80.6.8/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py` & `alacorder-80.6.9/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py`

 * *Files identical despite different names*

### Comparing `alacorder-80.6.8/src/alacorder/__main__.py` & `alacorder-80.6.9/src/alacorder/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Optional dependencies:
     pyarrow required to export summary to .xls, .xlsx,
     Google Chrome required to fetch cases from Alacourt
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.6.8"
+version = "80.6.9"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -1318,38 +1318,79 @@
         ]
     )
     cases = cases.join(pairs, on="Name", how="outer")
     cases = cases.groupby("AIS / Unique ID").all()
     cases = cases.join(vrr, on="AIS / Unique ID", how="outer")
     cases = cases.join(conv, on="AIS / Unique ID", how="outer")
     cases = cases.join(fch, on="AIS / Unique ID", how="outer")
+    cases = cases.with_columns(
+        [
+            pl.col("CaseNumber").arr.join(", ")            
+            .str.replace_all(r"null,?", "")
+            .str.strip()
+            .str.replace(r",$", "")
+            .str.replace_all(r"\s+", " ")
+            .alias("Cases")
+        ]
+    )
+    cases = cases.with_columns(
+        [
+            pl.when(pl.col("CERVConvictionCount").eq(0) & pl.col("PardonToVoteConvictionCount").eq(0) & pl.col("PermanentDisqConvictionCount").eq(0) & pl.col("Cases").str.lengths().gt(0))
+            .then(True).otherwise(False)
+            .alias("EligibleToVote"),
+            pl.when(pl.col("CERVConvictionCount").gt(0) & pl.col("PardonToVoteConvictionCount").eq(0) & pl.col("PermanentDisqConvictionCount").eq(0))
+            .then(True).otherwise(False)
+            .alias("NeedsCERV"),
+            pl.when(pl.col("PardonToVoteConvictionCount") > 0 & pl.col("PermanentDisqConvictionCount").eq(0))
+            .then(True).otherwise(False)
+            .alias("NeedsPardon"),
+            pl.when(pl.col("PermanentDisqConvictionCount").gt(0))
+            .then(True).otherwise(False)
+            .alias("PermanentlyDisqualified")
+        ]
+    )
+    cases = cases.with_columns(
+        [
+            pl.when(pl.col("Cases").str.lengths().eq(0))
+            .then(None).otherwise(pl.col("EligibleToVote"))
+            .alias("EligibleToVote"),
+            pl.when(pl.col("Cases").str.lengths().eq(0))
+            .then(None).otherwise(pl.col("NeedsCERV"))
+            .alias("NeedsCERV"),
+            pl.when(pl.col("Cases").str.lengths().eq(0))
+            .then(None).otherwise(pl.col("NeedsPardon"))
+            .alias("NeedsPardon"),
+            pl.when(pl.col("Cases").str.lengths().eq(0))
+            .then(None).otherwise(pl.col("PermanentlyDisqualified"))
+            .alias("PermanentlyDisqualified"),
+        ]
+    )
     cases = cases.select(
         [
             pl.col("AIS / Unique ID"),
             pl.col("Name").arr.first(),
             pl.col("DOB").arr.first(),
             pl.col("Race").arr.first(),
             pl.col("Sex").arr.first(),
             pl.col("PaymentToRestore"),
+            pl.col("EligibleToVote"),
+            pl.col("NeedsCERV"),
+            pl.col("NeedsPardon"),
+            pl.col("PermanentlyDisqualified"),
             pl.col("ConvictionCount"),
             pl.col("CERVChargesCount"),
             pl.col("CERVConvictionCount"),
             pl.col("PardonToVoteChargesCount"),
             pl.col("PardonToVoteConvictionCount"),
             pl.col("PermanentDisqChargesCount"),
             pl.col("PermanentDisqConvictionCount"),
             pl.col("DisqualifyingConvictions"),
             pl.col("Convictions"),
             pl.col("FilingCharges"),
-            pl.col("CaseNumber").arr.join(", ")            
-            .str.replace_all(r"null,?", "")
-            .str.strip()
-            .str.replace(r",$", "")
-            .str.replace_all(r"\s+", " ")
-            .alias("Cases")
+            pl.col("Cases")
         ]
     )
     cases = cases.sort("Name")
     if dest == None:
         pass
     elif os.path.splitext(dest)[1] == '.csv':
         cases.write_csv(dest)
```

### Comparing `alacorder-80.6.8/src/alacorder/alac.py` & `alacorder-80.6.9/src/alacorder/alac.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Optional dependencies:
     pyarrow required to export summary to .xls, .xlsx,
     Google Chrome required to fetch cases from Alacourt
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.6.8"
+version = "80.6.9"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -1318,38 +1318,79 @@
         ]
     )
     cases = cases.join(pairs, on="Name", how="outer")
     cases = cases.groupby("AIS / Unique ID").all()
     cases = cases.join(vrr, on="AIS / Unique ID", how="outer")
     cases = cases.join(conv, on="AIS / Unique ID", how="outer")
     cases = cases.join(fch, on="AIS / Unique ID", how="outer")
+    cases = cases.with_columns(
+        [
+            pl.col("CaseNumber").arr.join(", ")            
+            .str.replace_all(r"null,?", "")
+            .str.strip()
+            .str.replace(r",$", "")
+            .str.replace_all(r"\s+", " ")
+            .alias("Cases")
+        ]
+    )
+    cases = cases.with_columns(
+        [
+            pl.when(pl.col("CERVConvictionCount").eq(0) & pl.col("PardonToVoteConvictionCount").eq(0) & pl.col("PermanentDisqConvictionCount").eq(0) & pl.col("Cases").str.lengths().gt(0))
+            .then(True).otherwise(False)
+            .alias("EligibleToVote"),
+            pl.when(pl.col("CERVConvictionCount").gt(0) & pl.col("PardonToVoteConvictionCount").eq(0) & pl.col("PermanentDisqConvictionCount").eq(0))
+            .then(True).otherwise(False)
+            .alias("NeedsCERV"),
+            pl.when(pl.col("PardonToVoteConvictionCount") > 0 & pl.col("PermanentDisqConvictionCount").eq(0))
+            .then(True).otherwise(False)
+            .alias("NeedsPardon"),
+            pl.when(pl.col("PermanentDisqConvictionCount").gt(0))
+            .then(True).otherwise(False)
+            .alias("PermanentlyDisqualified")
+        ]
+    )
+    cases = cases.with_columns(
+        [
+            pl.when(pl.col("Cases").str.lengths().eq(0))
+            .then(None).otherwise(pl.col("EligibleToVote"))
+            .alias("EligibleToVote"),
+            pl.when(pl.col("Cases").str.lengths().eq(0))
+            .then(None).otherwise(pl.col("NeedsCERV"))
+            .alias("NeedsCERV"),
+            pl.when(pl.col("Cases").str.lengths().eq(0))
+            .then(None).otherwise(pl.col("NeedsPardon"))
+            .alias("NeedsPardon"),
+            pl.when(pl.col("Cases").str.lengths().eq(0))
+            .then(None).otherwise(pl.col("PermanentlyDisqualified"))
+            .alias("PermanentlyDisqualified"),
+        ]
+    )
     cases = cases.select(
         [
             pl.col("AIS / Unique ID"),
             pl.col("Name").arr.first(),
             pl.col("DOB").arr.first(),
             pl.col("Race").arr.first(),
             pl.col("Sex").arr.first(),
             pl.col("PaymentToRestore"),
+            pl.col("EligibleToVote"),
+            pl.col("NeedsCERV"),
+            pl.col("NeedsPardon"),
+            pl.col("PermanentlyDisqualified"),
             pl.col("ConvictionCount"),
             pl.col("CERVChargesCount"),
             pl.col("CERVConvictionCount"),
             pl.col("PardonToVoteChargesCount"),
             pl.col("PardonToVoteConvictionCount"),
             pl.col("PermanentDisqChargesCount"),
             pl.col("PermanentDisqConvictionCount"),
             pl.col("DisqualifyingConvictions"),
             pl.col("Convictions"),
             pl.col("FilingCharges"),
-            pl.col("CaseNumber").arr.join(", ")            
-            .str.replace_all(r"null,?", "")
-            .str.strip()
-            .str.replace(r",$", "")
-            .str.replace_all(r"\s+", " ")
-            .alias("Cases")
+            pl.col("Cases")
         ]
     )
     cases = cases.sort("Name")
     if dest == None:
         pass
     elif os.path.splitext(dest)[1] == '.csv':
         cases.write_csv(dest)
```

### Comparing `alacorder-80.6.8/PKG-INFO` & `alacorder-80.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.6.8
+Version: 80.6.9
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

