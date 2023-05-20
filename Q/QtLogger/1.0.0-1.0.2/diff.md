# Comparing `tmp/QtLogger-1.0.0-py3-none-any.whl.zip` & `tmp/QtLogger-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 6195 bytes, number of entries: 9
+Zip file size: 6174 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat       28 b- defN 23-Apr-17 16:09 QtLogger/__init__.py
 -rw-rw-rw-  2.0 fat     2561 b- defN 23-May-20 09:53 QtLogger/__main__.py
 -rw-rw-rw-  2.0 fat     9748 b- defN 23-May-20 09:55 QtLogger/base.py
 -rw-rw-rw-  2.0 fat      152 b- defN 23-Apr-18 07:00 QtLogger/exceptions.py
 -rw-rw-rw-  2.0 fat      180 b- defN 23-Apr-18 07:21 QtLogger/warnings.py
--rw-rw-rw-  2.0 fat     2028 b- defN 23-May-20 10:18 QtLogger-1.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-20 10:18 QtLogger-1.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-May-20 10:18 QtLogger-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      680 b- defN 23-May-20 10:18 QtLogger-1.0.0.dist-info/RECORD
-9 files, 15478 bytes uncompressed, 5029 bytes compressed:  67.5%
+-rw-rw-rw-  2.0 fat     1973 b- defN 23-May-20 10:23 QtLogger-1.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-20 10:23 QtLogger-1.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-May-20 10:23 QtLogger-1.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      680 b- defN 23-May-20 10:23 QtLogger-1.0.2.dist-info/RECORD
+9 files, 15423 bytes uncompressed, 5008 bytes compressed:  67.5%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: QtLogger/exceptions.py
 Comment: 
 
 Filename: QtLogger/warnings.py
 Comment: 
 
-Filename: QtLogger-1.0.0.dist-info/METADATA
+Filename: QtLogger-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: QtLogger-1.0.0.dist-info/WHEEL
+Filename: QtLogger-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: QtLogger-1.0.0.dist-info/top_level.txt
+Filename: QtLogger-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: QtLogger-1.0.0.dist-info/RECORD
+Filename: QtLogger-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `QtLogger-1.0.0.dist-info/METADATA` & `QtLogger-1.0.2.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: QtLogger
-Version: 1.0.0
+Version: 1.0.2
 Summary: A simple logger for PyQt6 that also has a nice UI
 Home-page: https://github.com/Advik-B/PyQt-Logger
 Author: Advik
 Author-email: <advik.b@gmail.com>
 Keywords: Logger,Qt,PyQt,Qt6,PyQt6,QtLogger
 Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: PyQt6
 
 
@@ -39,15 +38,15 @@
 
 ## Installation
 
 
 
 ```bash
 
-pip install PyQt-Logger
+pip install QtLogger
 
 ```
 
 
 
 ## Usage
```

