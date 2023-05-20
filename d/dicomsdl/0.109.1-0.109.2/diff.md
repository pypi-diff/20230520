# Comparing `tmp/dicomsdl-0.109.1-cp39-cp39-win_amd64.whl.zip` & `tmp/dicomsdl-0.109.2-cp311-cp311-musllinux_1_1_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,19 @@
-Zip file size: 926869 bytes, number of entries: 12
--rw-rw-rw-  2.0 fat     6257 b- defN 22-Nov-06 10:43 dicomsdl/__init__.py
--rw-rw-rw-  2.0 fat  2309632 b- defN 22-Nov-06 11:20 dicomsdl/_dicomsdl.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   142848 b- defN 22-Nov-06 11:20 dicomsdl/_util.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat      574 b- defN 22-Nov-06 10:43 dicomsdl/dump.py
--rw-rw-rw-  2.0 fat      458 b- defN 22-Nov-06 10:43 dicomsdl/show.py
--rw-rw-rw-  2.0 fat      126 b- defN 22-Nov-06 10:43 dicomsdl/util.py
--rw-rw-rw-  2.0 fat     9800 b- defN 22-Nov-06 11:20 dicomsdl-0.109.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     6098 b- defN 22-Nov-06 11:20 dicomsdl-0.109.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 22-Nov-06 11:20 dicomsdl-0.109.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       81 b- defN 22-Nov-06 11:20 dicomsdl-0.109.1.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        9 b- defN 22-Nov-06 11:20 dicomsdl-0.109.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      981 b- defN 22-Nov-06 11:20 dicomsdl-0.109.1.dist-info/RECORD
-12 files, 2476964 bytes uncompressed, 925225 bytes compressed:  62.7%
+Zip file size: 1929536 bytes, number of entries: 17
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-20 03:31 dicomsdl/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-20 03:31 dicomsdl.libs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-20 03:31 dicomsdl-0.109.2.dist-info/
+-rw-r--r--  2.0 unx      126 b- defN 23-May-20 03:31 dicomsdl/util.py
+-rwxr-xr-x  2.0 unx  3700984 b- defN 23-May-20 03:31 dicomsdl/_dicomsdl.cpython-311-x86_64-linux-musl.so
+-rw-r--r--  2.0 unx      574 b- defN 23-May-20 03:31 dicomsdl/dump.py
+-rwxr-xr-x  2.0 unx   158664 b- defN 23-May-20 03:31 dicomsdl/_util.cpython-311-x86_64-linux-musl.so
+-rw-r--r--  2.0 unx      458 b- defN 23-May-20 03:31 dicomsdl/show.py
+-rw-r--r--  2.0 unx     6257 b- defN 23-May-20 03:31 dicomsdl/__init__.py
+-rw-r--r--  2.0 unx    81256 b- defN 23-May-20 03:31 dicomsdl.libs/libgcc_s-a04fdf82.so.1
+-rwxr-xr-x  2.0 unx  2447392 b- defN 23-May-20 03:31 dicomsdl.libs/libstdc++-a9383cce.so.6.0.28
+-rw-r--r--  2.0 unx      113 b- defN 23-May-20 03:31 dicomsdl-0.109.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx     6061 b- defN 23-May-20 03:31 dicomsdl-0.109.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx     1219 b- defN 23-May-20 03:31 dicomsdl-0.109.2.dist-info/RECORD
+-rw-r--r--  2.0 unx       80 b- defN 23-May-20 03:31 dicomsdl-0.109.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 23-May-20 03:31 dicomsdl-0.109.2.dist-info/top_level.txt
+-rw-r--r--  2.0 unx     9800 b- defN 23-May-20 03:31 dicomsdl-0.109.2.dist-info/LICENSE
+17 files, 6412993 bytes uncompressed, 1927200 bytes compressed:  70.0%
```

## zipnote {}

```diff
@@ -1,37 +1,52 @@
-Filename: dicomsdl/__init__.py
+Filename: dicomsdl/
+Comment: 
+
+Filename: dicomsdl.libs/
 Comment: 
 
-Filename: dicomsdl/_dicomsdl.cp39-win_amd64.pyd
+Filename: dicomsdl-0.109.2.dist-info/
 Comment: 
 
-Filename: dicomsdl/_util.cp39-win_amd64.pyd
+Filename: dicomsdl/util.py
+Comment: 
+
+Filename: dicomsdl/_dicomsdl.cpython-311-x86_64-linux-musl.so
 Comment: 
 
 Filename: dicomsdl/dump.py
 Comment: 
 
+Filename: dicomsdl/_util.cpython-311-x86_64-linux-musl.so
+Comment: 
+
 Filename: dicomsdl/show.py
 Comment: 
 
-Filename: dicomsdl/util.py
+Filename: dicomsdl/__init__.py
+Comment: 
+
+Filename: dicomsdl.libs/libgcc_s-a04fdf82.so.1
+Comment: 
+
+Filename: dicomsdl.libs/libstdc++-a9383cce.so.6.0.28
 Comment: 
 
-Filename: dicomsdl-0.109.1.dist-info/LICENSE
+Filename: dicomsdl-0.109.2.dist-info/WHEEL
 Comment: 
 
-Filename: dicomsdl-0.109.1.dist-info/METADATA
+Filename: dicomsdl-0.109.2.dist-info/METADATA
 Comment: 
 
-Filename: dicomsdl-0.109.1.dist-info/WHEEL
+Filename: dicomsdl-0.109.2.dist-info/RECORD
 Comment: 
 
-Filename: dicomsdl-0.109.1.dist-info/entry_points.txt
+Filename: dicomsdl-0.109.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: dicomsdl-0.109.1.dist-info/top_level.txt
+Filename: dicomsdl-0.109.2.dist-info/top_level.txt
 Comment: 
 
-Filename: dicomsdl-0.109.1.dist-info/RECORD
+Filename: dicomsdl-0.109.2.dist-info/LICENSE
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## Comparing `dicomsdl-0.109.1.dist-info/LICENSE` & `dicomsdl-0.109.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dicomsdl-0.109.1.dist-info/METADATA` & `dicomsdl-0.109.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: dicomsdl
-Version: 0.109.1
+Version: 0.109.2
 Summary: A fast and light-weighted DICOM software development library
 Home-page: https://github.com/tsangel/dicomsdl
 Author: Kim, Tae-Sung
 Author-email: taesung.angel@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
@@ -144,9 +142,7 @@
 '00020000'	UL	4	1	0x8c	212	# FileMetaInformationGroupLength
 '00020001'	OB	2	1	0x9c	'\x00\x01'	# FileMetaInformationVersion
 '00020002'	UI	26	1	0xa6	'1.2.840.10008.5.1.4.1.1.2' = CT Image Storage	# MediaStorageSOPClassUID
 ...
 
  
 ```
-
-
```

