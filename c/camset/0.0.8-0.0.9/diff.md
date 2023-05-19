# Comparing `tmp/camset-0.0.8-py3-none-any.whl.zip` & `tmp/camset-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 66609 bytes, number of entries: 12
+Zip file size: 66613 bytes, number of entries: 12
 -rw-r--r--  2.0 unx        0 b- defN 20-Apr-04 05:50 camset/__init__.py
--rw-rw-r--  2.0 unx    20553 b- defN 20-Sep-28 18:02 camset/camset.py
--rw-r--r--  2.0 unx      737 b- defN 20-Apr-07 11:32 camset/test_gstream.py
--rw-r--r--  2.0 unx    62832 b- defN 20-Apr-07 01:30 camset/v4l2.py
--rw-r--r--  2.0 unx      177 b- defN 20-Apr-04 13:02 camset-0.0.8.data/data/share/applications/camset.desktop
--rw-r--r--  2.0 unx    33163 b- defN 20-Apr-04 13:54 camset-0.0.8.data/data/share/icons/camset.png
--rw-r--r--  2.0 unx    35149 b- defN 20-Sep-28 18:08 camset-0.0.8.dist-info/LICENSE
--rw-rw-r--  2.0 unx     2089 b- defN 20-Sep-28 18:08 camset-0.0.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 20-Sep-28 18:08 camset-0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       47 b- defN 20-Sep-28 18:08 camset-0.0.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 20-Sep-28 18:08 camset-0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      986 b- defN 20-Sep-28 18:08 camset-0.0.8.dist-info/RECORD
-12 files, 155832 bytes uncompressed, 64947 bytes compressed:  58.3%
+-rw-rw-r--  2.0 unx    20561 b- defN 20-Oct-08 16:08 camset/camset.py
+-rw-rw-r--  2.0 unx      737 b- defN 20-Apr-07 11:32 camset/test_gstream.py
+-rw-rw-r--  2.0 unx    62832 b- defN 20-Apr-07 01:30 camset/v4l2.py
+-rw-r--r--  2.0 unx      177 b- defN 20-Apr-04 13:02 camset-0.0.9.data/data/share/applications/camset.desktop
+-rw-r--r--  2.0 unx    33163 b- defN 20-Apr-04 13:54 camset-0.0.9.data/data/share/icons/camset.png
+-rw-r--r--  2.0 unx    35149 b- defN 20-Oct-08 16:11 camset-0.0.9.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     2089 b- defN 20-Oct-08 16:11 camset-0.0.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 20-Oct-08 16:11 camset-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       47 b- defN 20-Oct-08 16:11 camset-0.0.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 20-Oct-08 16:11 camset-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      986 b- defN 20-Oct-08 16:11 camset-0.0.9.dist-info/RECORD
+12 files, 155840 bytes uncompressed, 64951 bytes compressed:  58.3%
```

## zipnote {}

```diff
@@ -6,32 +6,32 @@
 
 Filename: camset/test_gstream.py
 Comment: 
 
 Filename: camset/v4l2.py
 Comment: 
 
-Filename: camset-0.0.8.data/data/share/applications/camset.desktop
+Filename: camset-0.0.9.data/data/share/applications/camset.desktop
 Comment: 
 
-Filename: camset-0.0.8.data/data/share/icons/camset.png
+Filename: camset-0.0.9.data/data/share/icons/camset.png
 Comment: 
 
-Filename: camset-0.0.8.dist-info/LICENSE
+Filename: camset-0.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: camset-0.0.8.dist-info/METADATA
+Filename: camset-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: camset-0.0.8.dist-info/WHEEL
+Filename: camset-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: camset-0.0.8.dist-info/entry_points.txt
+Filename: camset-0.0.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: camset-0.0.8.dist-info/top_level.txt
+Filename: camset-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: camset-0.0.8.dist-info/RECORD
+Filename: camset-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## camset/camset.py

```diff
@@ -242,15 +242,15 @@
         clear_and_rebuild()
         init_camera_feed()
 
 def set_int_value(callback, card, setting):
     value = str(int(callback.get_value()))
     subprocess.run(['v4l2-ctl', '-d', card, '-c', '{0}={1}'.format(setting, value)], check=True, universal_newlines=True)
     
-def set_bool_value(callback, card, setting):
+def set_bool_value(callback, active, card, setting):
     if callback.get_active():
         subprocess.run(['v4l2-ctl', '-d', card, '-c', '{0}=1'.format(setting)], check=True, universal_newlines=True)
     else:
         subprocess.run(['v4l2-ctl', '-d', card, '-c', '{0}=0'.format(setting)], check=True, universal_newlines=True)
     set_sensitivity(card)
 
 def on_ctrl_combo_changed(callback, card, setting): # change combobox values except resolution
```

## Comparing `camset-0.0.8.data/data/share/icons/camset.png` & `camset-0.0.9.data/data/share/icons/camset.png`

 * *Files identical despite different names*

## Comparing `camset-0.0.8.dist-info/LICENSE` & `camset-0.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `camset-0.0.8.dist-info/METADATA` & `camset-0.0.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: camset
-Version: 0.0.8
+Version: 0.0.9
 Summary: GUI for v4l2-ctl
 Home-page: https://github.com/azeam/camset
 Author: Dennis Hägg
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

## Comparing `camset-0.0.8.dist-info/RECORD` & `camset-0.0.9.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 camset/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-camset/camset.py,sha256=hS30xyy8ZBs3zN5GjAYkJerYLgTrkv3aIWJRtoWp_Kg,20553
+camset/camset.py,sha256=zTHL98EgGIZZUhKbj__OLppMjnwrmkgb44K8-YwfIow,20561
 camset/test_gstream.py,sha256=ekRzPVzR0zrgdKI0VDBF7AsmN2HSbZtO7UTbTc10VvU,737
 camset/v4l2.py,sha256=Ki3NqfBstRBbGsjZKtsBPWhQm3XfSRyykINCKdLGvTQ,62832
-camset-0.0.8.data/data/share/applications/camset.desktop,sha256=fgCj_n7bLOCHz8azi-DskX_RIWx75FEDwEwSsc_YYwU,177
-camset-0.0.8.data/data/share/icons/camset.png,sha256=ClhAeI9HGjVS_JIrqg2KxWynynkq9NL5ZG6xwwjQ-Xk,33163
-camset-0.0.8.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-camset-0.0.8.dist-info/METADATA,sha256=rHUvxsdfuJ-j4rUsaRJZ2XP0A5bbUWvX3LKb3lfX0o4,2089
-camset-0.0.8.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-camset-0.0.8.dist-info/entry_points.txt,sha256=jE9ONYs8_TEW6oPU4aPEvoXdal_v3te7zpevHcK5m0c,47
-camset-0.0.8.dist-info/top_level.txt,sha256=C9zfPpu60tYSUL2D9SH6fec0wxJB8ynqtolHIledMgE,7
-camset-0.0.8.dist-info/RECORD,,
+camset-0.0.9.data/data/share/applications/camset.desktop,sha256=fgCj_n7bLOCHz8azi-DskX_RIWx75FEDwEwSsc_YYwU,177
+camset-0.0.9.data/data/share/icons/camset.png,sha256=ClhAeI9HGjVS_JIrqg2KxWynynkq9NL5ZG6xwwjQ-Xk,33163
+camset-0.0.9.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+camset-0.0.9.dist-info/METADATA,sha256=U_9vYwCfxajMzQSqPnqrcZ__Jqd7TWYMihcv6vkNY3k,2089
+camset-0.0.9.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+camset-0.0.9.dist-info/entry_points.txt,sha256=jE9ONYs8_TEW6oPU4aPEvoXdal_v3te7zpevHcK5m0c,47
+camset-0.0.9.dist-info/top_level.txt,sha256=C9zfPpu60tYSUL2D9SH6fec0wxJB8ynqtolHIledMgE,7
+camset-0.0.9.dist-info/RECORD,,
```

