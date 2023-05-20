# Comparing `tmp/ScriptCollection-3.3.91-py3-none-any.whl.zip` & `tmp/ScriptCollection-3.3.92-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
 Zip file size: 57600 bytes, number of entries: 14
 -rw-rw-rw-  2.0 fat    18064 b- defN 23-Mar-05 15:39 ScriptCollection/Executables.py
 -rw-rw-rw-  2.0 fat    34139 b- defN 23-May-20 16:21 ScriptCollection/GeneralUtilities.py
 -rw-rw-rw-  2.0 fat     1937 b- defN 22-Aug-30 21:59 ScriptCollection/ProgramRunnerBase.py
 -rw-rw-rw-  2.0 fat     6273 b- defN 22-Oct-16 19:55 ScriptCollection/ProgramRunnerEpew.py
 -rw-rw-rw-  2.0 fat     3023 b- defN 22-Aug-30 21:59 ScriptCollection/ProgramRunnerPopen.py
--rw-rw-rw-  2.0 fat    86233 b- defN 23-May-20 18:20 ScriptCollection/ScriptCollectionCore.py
+-rw-rw-rw-  2.0 fat    86233 b- defN 23-May-20 18:53 ScriptCollection/ScriptCollectionCore.py
 -rw-rw-rw-  2.0 fat   129034 b- defN 23-May-20 18:20 ScriptCollection/TasksForCommonProjectStructure.py
 -rw-rw-rw-  2.0 fat     7918 b- defN 22-Aug-30 21:59 ScriptCollection/UpdateCertificates.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Aug-29 05:45 ScriptCollection/__init__.py
--rw-rw-rw-  2.0 fat     7864 b- defN 23-May-20 18:21 ScriptCollection-3.3.91.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-20 18:21 ScriptCollection-3.3.91.dist-info/WHEEL
--rw-rw-rw-  2.0 fat     1968 b- defN 23-May-20 18:21 ScriptCollection-3.3.91.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       17 b- defN 23-May-20 18:21 ScriptCollection-3.3.91.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1295 b- defN 23-May-20 18:21 ScriptCollection-3.3.91.dist-info/RECORD
+-rw-rw-rw-  2.0 fat     7864 b- defN 23-May-20 18:54 ScriptCollection-3.3.92.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-20 18:54 ScriptCollection-3.3.92.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat     1968 b- defN 23-May-20 18:54 ScriptCollection-3.3.92.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       17 b- defN 23-May-20 18:54 ScriptCollection-3.3.92.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1295 b- defN 23-May-20 18:54 ScriptCollection-3.3.92.dist-info/RECORD
 14 files, 297857 bytes uncompressed, 55408 bytes compressed:  81.4%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: ScriptCollection/UpdateCertificates.py
 Comment: 
 
 Filename: ScriptCollection/__init__.py
 Comment: 
 
-Filename: ScriptCollection-3.3.91.dist-info/METADATA
+Filename: ScriptCollection-3.3.92.dist-info/METADATA
 Comment: 
 
-Filename: ScriptCollection-3.3.91.dist-info/WHEEL
+Filename: ScriptCollection-3.3.92.dist-info/WHEEL
 Comment: 
 
-Filename: ScriptCollection-3.3.91.dist-info/entry_points.txt
+Filename: ScriptCollection-3.3.92.dist-info/entry_points.txt
 Comment: 
 
-Filename: ScriptCollection-3.3.91.dist-info/top_level.txt
+Filename: ScriptCollection-3.3.92.dist-info/top_level.txt
 Comment: 
 
-Filename: ScriptCollection-3.3.91.dist-info/RECORD
+Filename: ScriptCollection-3.3.92.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ScriptCollection/ScriptCollectionCore.py

```diff
@@ -21,15 +21,15 @@
 from PyPDF2 import PdfFileMerger
 from .GeneralUtilities import GeneralUtilities
 from .ProgramRunnerBase import ProgramRunnerBase
 from .ProgramRunnerPopen import ProgramRunnerPopen
 from .ProgramRunnerEpew import ProgramRunnerEpew, CustomEpewArgument
 
 
-version = "3.3.91"
+version = "3.3.92"
 __version__ = version
 
 
 class ScriptCollectionCore:
 
     # The purpose of this property is to use it when testing your code which uses scriptcollection for external program-calls.
     # Do not change this value for productive environments.
```

## Comparing `ScriptCollection-3.3.91.dist-info/METADATA` & `ScriptCollection-3.3.92.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ScriptCollection
-Version: 3.3.91
+Version: 3.3.92
 Summary: The ScriptCollection is the place for reusable scripts.
 Home-page: https://github.com/anionDev/ScriptCollection
 Author: Marius Göcke
 Author-email: marius.goecke@gmail.com
 Project-URL: Documentation, https://aniondev.github.io/ScriptCollectionReference/index.html
 Project-URL: Changelog, https://github.com/anionDev/ScriptCollection/tree/main/Other/Resources/Changelog
 Keywords: package release build management
@@ -18,17 +18,17 @@
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: System :: Archiving :: Packaging
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Terminals
 Classifier: Topic :: Utilities
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Requires-Dist: autopep8 (>=2.0.1)
+Requires-Dist: autopep8 (>=2.0.2)
 Requires-Dist: build (>=0.10.0)
-Requires-Dist: coverage (>=7.0.5)
+Requires-Dist: coverage (>=7.2.5)
 Requires-Dist: cyclonedx-bom (>=3.11.0)
 Requires-Dist: defusedxml (>=0.7.1)
 Requires-Dist: keyboard (>=0.13.5)
 Requires-Dist: lxml (>=4.9.2)
 Requires-Dist: ntplib (>=0.4.0)
 Requires-Dist: pycdlib (>=1.14.0)
 Requires-Dist: Pygments (>=2.15.1)
```

## Comparing `ScriptCollection-3.3.91.dist-info/entry_points.txt` & `ScriptCollection-3.3.92.dist-info/entry_points.txt`

 * *Files identical despite different names*

## Comparing `ScriptCollection-3.3.91.dist-info/RECORD` & `ScriptCollection-3.3.92.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ScriptCollection/Executables.py,sha256=kXTIX92KLeFuxnYOlsyFs5lkznsxkuoBMVrV3OU7FZU,18064
 ScriptCollection/GeneralUtilities.py,sha256=7-KuXjS_S-oiMcMM9bEDGx8n4RlnGxGpqHdhXhN47I8,34139
 ScriptCollection/ProgramRunnerBase.py,sha256=2kyOuoM3oFjBfLc9Q5t5RTz7Ya2CjUxFtB1rBBDmnjU,1937
 ScriptCollection/ProgramRunnerEpew.py,sha256=ZiBZVMcsphmo49z2BwUwQYXo2uTKXPu33QW3IxCT46E,6273
 ScriptCollection/ProgramRunnerPopen.py,sha256=HOs1QVnXiQtwXy1_xvH79bWBdd0i-2tUyyLloQBvMto,3023
-ScriptCollection/ScriptCollectionCore.py,sha256=IAMV4HvN-BBiMRgMerxDtsgIb-f3l8cGaVUv2shcnrM,86233
+ScriptCollection/ScriptCollectionCore.py,sha256=441FIJMhdYMpRRCSo223Qtr8G_ffPB6Go_9rq1XPkcg,86233
 ScriptCollection/TasksForCommonProjectStructure.py,sha256=Zg_aBGA5K8oA06l79HYT_Tm7lERE1Ym3JLtqUVyT7ys,129034
 ScriptCollection/UpdateCertificates.py,sha256=Go-JJK-YTi7aBB1phlLxypa8GHkmFHBEPB0_TT9G-bw,7918
 ScriptCollection/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ScriptCollection-3.3.91.dist-info/METADATA,sha256=F0pUTHib0IqOb5W6LgtS6ISu45kqfUyZagtf258sKTs,7864
-ScriptCollection-3.3.91.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-ScriptCollection-3.3.91.dist-info/entry_points.txt,sha256=VIuxVCOpX38lSJUwRRENBNgcGKTIBxQyrCfbJVRHP8g,1968
-ScriptCollection-3.3.91.dist-info/top_level.txt,sha256=hY2hOVH0V0Ce51WB76zKkIWTUNwMUdHo4XDkR2vYVwg,17
-ScriptCollection-3.3.91.dist-info/RECORD,,
+ScriptCollection-3.3.92.dist-info/METADATA,sha256=Y8ligCMf2s3o4k0XqbBkfXMwIMJXaI54VYsHEPYx4qA,7864
+ScriptCollection-3.3.92.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+ScriptCollection-3.3.92.dist-info/entry_points.txt,sha256=VIuxVCOpX38lSJUwRRENBNgcGKTIBxQyrCfbJVRHP8g,1968
+ScriptCollection-3.3.92.dist-info/top_level.txt,sha256=hY2hOVH0V0Ce51WB76zKkIWTUNwMUdHo4XDkR2vYVwg,17
+ScriptCollection-3.3.92.dist-info/RECORD,,
```

