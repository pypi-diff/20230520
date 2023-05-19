# Comparing `tmp/arckit-0.0.3-py3-none-any.whl.zip` & `tmp/arckit-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,13 @@
-Zip file size: 8945 bytes, number of entries: 10
+Zip file size: 265350 bytes, number of entries: 11
 -rw-rw-r--  2.0 unx      110 b- defN 23-May-19 22:38 arckit/__init__.py
+-rw-rw-r--  2.0 unx  3826530 b- defN 23-May-19 22:38 arckit/arc1.json
 -rw-rw-r--  2.0 unx     1173 b- defN 23-May-19 22:38 arckit/cli.py
 -rw-rw-r--  2.0 unx    11202 b- defN 23-May-19 22:39 arckit/data.py
 -rw-rw-r--  2.0 unx    10790 b- defN 23-May-19 22:38 arckit/vis.py
--rw-rw-r--  2.0 unx      471 b- defN 23-May-19 23:01 arckit-0.0.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-19 23:01 arckit-0.0.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx       79 b- defN 23-May-19 23:01 arckit-0.0.3.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        7 b- defN 23-May-19 23:01 arckit-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx        1 b- defN 23-May-19 23:00 arckit-0.0.3.dist-info/zip-safe
--rw-rw-r--  2.0 unx      758 b- defN 23-May-19 23:01 arckit-0.0.3.dist-info/RECORD
-10 files, 24683 bytes uncompressed, 7659 bytes compressed:  69.0%
+-rw-rw-r--  2.0 unx      471 b- defN 23-May-19 23:08 arckit-0.0.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-19 23:08 arckit-0.0.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       79 b- defN 23-May-19 23:08 arckit-0.0.4.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        7 b- defN 23-May-19 23:08 arckit-0.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-May-19 23:00 arckit-0.0.4.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      834 b- defN 23-May-19 23:08 arckit-0.0.4.dist-info/RECORD
+11 files, 3851289 bytes uncompressed, 263956 bytes compressed:  93.2%
```

## zipnote {}

```diff
@@ -1,31 +1,34 @@
 Filename: arckit/__init__.py
 Comment: 
 
+Filename: arckit/arc1.json
+Comment: 
+
 Filename: arckit/cli.py
 Comment: 
 
 Filename: arckit/data.py
 Comment: 
 
 Filename: arckit/vis.py
 Comment: 
 
-Filename: arckit-0.0.3.dist-info/METADATA
+Filename: arckit-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: arckit-0.0.3.dist-info/WHEEL
+Filename: arckit-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: arckit-0.0.3.dist-info/entry_points.txt
+Filename: arckit-0.0.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: arckit-0.0.3.dist-info/top_level.txt
+Filename: arckit-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: arckit-0.0.3.dist-info/zip-safe
+Filename: arckit-0.0.4.dist-info/zip-safe
 Comment: 
 
-Filename: arckit-0.0.3.dist-info/RECORD
+Filename: arckit-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `arckit-0.0.3.dist-info/RECORD` & `arckit-0.0.4.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 arckit/__init__.py,sha256=TN6WmFGjVXSnEhjcmUy_wqDknUkRKgLAZ-iu8FOMfYY,110
+arckit/arc1.json,sha256=UyFPcc7OY1-LKpAD3qstp6K1G9DKC4FpXzfkuIiQPQQ,3826530
 arckit/cli.py,sha256=EadWRtGIC7jVUvT0fglLhIwoJBKoSHwgG3WkDhkhhAQ,1173
 arckit/data.py,sha256=V4WOg94PyuNZVR4nf_J_EhMpd8kJVr91Ckdx-0Lhj4I,11202
 arckit/vis.py,sha256=BszQBqeQSWfsievxPy8RszHusOBoy_5yobCJzEF6g6M,10790
-arckit-0.0.3.dist-info/METADATA,sha256=YTT71vFV2H8bJGl2C9rYE2wwSZFPTF76v4ELA86QP3o,471
-arckit-0.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-arckit-0.0.3.dist-info/entry_points.txt,sha256=2k0G8Jzb4Cj_9U0dvHxxgOGRgmmQe64QieiiI3Wqbgs,79
-arckit-0.0.3.dist-info/top_level.txt,sha256=fAJt_Fxb-oM5WePjq-hHd6iPrPUfO_3FzFxtnrtXvQY,7
-arckit-0.0.3.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-arckit-0.0.3.dist-info/RECORD,,
+arckit-0.0.4.dist-info/METADATA,sha256=CKcIenxGCWrSl91kfpgRBeDXlNvnGLk7PJPPZ4eKHKw,471
+arckit-0.0.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+arckit-0.0.4.dist-info/entry_points.txt,sha256=2k0G8Jzb4Cj_9U0dvHxxgOGRgmmQe64QieiiI3Wqbgs,79
+arckit-0.0.4.dist-info/top_level.txt,sha256=fAJt_Fxb-oM5WePjq-hHd6iPrPUfO_3FzFxtnrtXvQY,7
+arckit-0.0.4.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+arckit-0.0.4.dist-info/RECORD,,
```

