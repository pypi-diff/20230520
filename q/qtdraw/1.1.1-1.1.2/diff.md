# Comparing `tmp/qtdraw-1.1.1.tar.gz` & `tmp/qtdraw-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtdraw-1.1.1.tar", last modified: Wed May 17 12:45:44 2023, max compression
+gzip compressed data, was "qtdraw-1.1.2.tar", last modified: Sat May 20 07:18:26 2023, max compression
```

## Comparing `qtdraw-1.1.1.tar` & `qtdraw-1.1.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-17 12:45:44.098284 qtdraw-1.1.1/
--rw-r--r--   0 hiro       (501) staff       (20)     1078 2023-05-09 03:18:56.000000 qtdraw-1.1.1/LICENSE
--rw-------   0 hiro       (501) staff       (20)      107 2023-05-15 22:04:32.000000 qtdraw-1.1.1/MANIFEST.in
--rw-r--r--   0 hiro       (501) staff       (20)     2414 2023-05-17 12:45:44.098375 qtdraw-1.1.1/PKG-INFO
--rw-r--r--   0 hiro       (501) staff       (20)     2034 2023-05-17 12:42:17.000000 qtdraw-1.1.1/README.md
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-17 12:45:44.091917 qtdraw-1.1.1/qtdraw/
--rw-r--r--   0 hiro       (501) staff       (20)       79 2023-05-17 01:26:21.000000 qtdraw-1.1.1/qtdraw/__init__.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-17 12:45:44.097700 qtdraw-1.1.1/qtdraw/core/
--rw-r--r--   0 hiro       (501) staff       (20)    11407 2023-05-15 12:36:33.000000 qtdraw-1.1.1/qtdraw/core/basic_object.py
--rw-r--r--   0 hiro       (501) staff       (20)      945 2023-05-09 03:18:56.000000 qtdraw-1.1.1/qtdraw/core/color_dialog.py
--rw-r--r--   0 hiro       (501) staff       (20)    15144 2023-05-15 12:36:33.000000 qtdraw-1.1.1/qtdraw/core/color_palette.py
--rw-r--r--   0 hiro       (501) staff       (20)     2443 2023-05-09 03:18:56.000000 qtdraw-1.1.1/qtdraw/core/default_panel.ui
--rw-r--r--   0 hiro       (501) staff       (20)     3719 2023-05-15 12:36:33.000000 qtdraw-1.1.1/qtdraw/core/dialog_about.py
--rw-r--r--   0 hiro       (501) staff       (20)    17447 2023-05-09 03:18:56.000000 qtdraw-1.1.1/qtdraw/core/dialog_preference.py
--rw-r--r--   0 hiro       (501) staff       (20)    16441 2023-05-15 12:36:33.000000 qtdraw-1.1.1/qtdraw/core/editable_widget.py
--rw-r--r--   0 hiro       (501) staff       (20)     8466 2023-05-09 03:18:56.000000 qtdraw-1.1.1/qtdraw/core/group_model.py
--rw-r--r--   0 hiro       (501) staff       (20)     2233 2023-05-09 03:18:56.000000 qtdraw-1.1.1/qtdraw/core/group_panel.ui
--rw-r--r--   0 hiro       (501) staff       (20)     1656 2023-05-09 03:18:56.000000 qtdraw-1.1.1/qtdraw/core/group_tab.py
--rw-r--r--   0 hiro       (501) staff       (20)     4632 2023-05-09 03:18:56.000000 qtdraw-1.1.1/qtdraw/core/group_view.py
--rw-r--r--   0 hiro       (501) staff       (20)     9744 2023-05-15 12:36:33.000000 qtdraw-1.1.1/qtdraw/core/line_edit.py
--rw-r--r--   0 hiro       (501) staff       (20)     2837 2023-05-15 12:36:33.000000 qtdraw-1.1.1/qtdraw/core/pixmap_converter.py
--rw-r--r--   0 hiro       (501) staff       (20)     2385 2023-05-09 03:18:56.000000 qtdraw-1.1.1/qtdraw/core/qt_logging.py
--rw-r--r--   0 hiro       (501) staff       (20)   187925 2023-05-09 03:18:56.000000 qtdraw-1.1.1/qtdraw/core/qtdraw.png
--rw-r--r--   0 hiro       (501) staff       (20)    31369 2023-05-09 03:18:56.000000 qtdraw-1.1.1/qtdraw/core/qtdraw.ui
--rw-r--r--   0 hiro       (501) staff       (20)    17478 2023-05-09 03:18:56.000000 qtdraw-1.1.1/qtdraw/core/setting.py
--rw-r--r--   0 hiro       (501) staff       (20)     2678 2023-05-09 03:18:56.000000 qtdraw-1.1.1/qtdraw/core/table_dialog.py
--rw-r--r--   0 hiro       (501) staff       (20)     4458 2023-05-09 03:18:56.000000 qtdraw-1.1.1/qtdraw/core/tree_item.py
--rw-r--r--   0 hiro       (501) staff       (20)    16260 2023-05-09 03:18:56.000000 qtdraw-1.1.1/qtdraw/core/tree_item_model.py
--rw-r--r--   0 hiro       (501) staff       (20)     7499 2023-05-15 12:36:33.000000 qtdraw-1.1.1/qtdraw/core/util.py
--rw-r--r--   0 hiro       (501) staff       (20)     4715 2023-05-09 03:18:56.000000 qtdraw-1.1.1/qtdraw/core/validator.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-17 12:45:44.098150 qtdraw-1.1.1/qtdraw/multipie/
--rw-r--r--   0 hiro       (501) staff       (20)    46964 2023-05-15 12:36:33.000000 qtdraw-1.1.1/qtdraw/multipie/dialog_group.py
--rw-r--r--   0 hiro       (501) staff       (20)     9646 2023-05-15 12:36:32.000000 qtdraw-1.1.1/qtdraw/multipie/dialog_group_info.py
--rw-r--r--   0 hiro       (501) staff       (20)     1839 2023-05-09 03:18:56.000000 qtdraw-1.1.1/qtdraw/multipie/setting.py
--rw-r--r--   0 hiro       (501) staff       (20)    91973 2023-05-15 12:36:32.000000 qtdraw-1.1.1/qtdraw/qt_draw.py
--rw-r--r--   0 hiro       (501) staff       (20)     9242 2023-05-09 03:18:56.000000 qtdraw-1.1.1/qtdraw/qt_draw_base.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-17 12:45:44.092650 qtdraw-1.1.1/qtdraw.egg-info/
--rw-r--r--   0 hiro       (501) staff       (20)     2414 2023-05-17 12:45:44.000000 qtdraw-1.1.1/qtdraw.egg-info/PKG-INFO
--rw-r--r--   0 hiro       (501) staff       (20)      944 2023-05-17 12:45:44.000000 qtdraw-1.1.1/qtdraw.egg-info/SOURCES.txt
--rw-r--r--   0 hiro       (501) staff       (20)        1 2023-05-17 12:45:44.000000 qtdraw-1.1.1/qtdraw.egg-info/dependency_links.txt
--rw-r--r--   0 hiro       (501) staff       (20)       96 2023-05-17 12:45:44.000000 qtdraw-1.1.1/qtdraw.egg-info/requires.txt
--rw-r--r--   0 hiro       (501) staff       (20)        7 2023-05-17 12:45:44.000000 qtdraw-1.1.1/qtdraw.egg-info/top_level.txt
--rw-r--r--   0 hiro       (501) staff       (20)      640 2023-05-17 12:45:44.098810 qtdraw-1.1.1/setup.cfg
--rw-r--r--   0 hiro       (501) staff       (20)       38 2023-05-09 03:18:56.000000 qtdraw-1.1.1/setup.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-20 07:18:26.047040 qtdraw-1.1.2/
+-rw-r--r--   0 hiro       (501) staff       (20)     1078 2023-05-09 03:18:56.000000 qtdraw-1.1.2/LICENSE
+-rw-------   0 hiro       (501) staff       (20)      107 2023-05-15 22:04:32.000000 qtdraw-1.1.2/MANIFEST.in
+-rw-r--r--   0 hiro       (501) staff       (20)     2414 2023-05-20 07:18:26.047137 qtdraw-1.1.2/PKG-INFO
+-rw-r--r--   0 hiro       (501) staff       (20)     2034 2023-05-17 12:42:17.000000 qtdraw-1.1.2/README.md
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-20 07:18:26.041273 qtdraw-1.1.2/qtdraw/
+-rw-r--r--   0 hiro       (501) staff       (20)       79 2023-05-20 07:17:57.000000 qtdraw-1.1.2/qtdraw/__init__.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-20 07:18:26.046435 qtdraw-1.1.2/qtdraw/core/
+-rw-r--r--   0 hiro       (501) staff       (20)    11407 2023-05-15 12:36:33.000000 qtdraw-1.1.2/qtdraw/core/basic_object.py
+-rw-r--r--   0 hiro       (501) staff       (20)      945 2023-05-09 03:18:56.000000 qtdraw-1.1.2/qtdraw/core/color_dialog.py
+-rw-r--r--   0 hiro       (501) staff       (20)    15144 2023-05-15 12:36:33.000000 qtdraw-1.1.2/qtdraw/core/color_palette.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2443 2023-05-09 03:18:56.000000 qtdraw-1.1.2/qtdraw/core/default_panel.ui
+-rw-r--r--   0 hiro       (501) staff       (20)     3719 2023-05-15 12:36:33.000000 qtdraw-1.1.2/qtdraw/core/dialog_about.py
+-rw-r--r--   0 hiro       (501) staff       (20)    17447 2023-05-09 03:18:56.000000 qtdraw-1.1.2/qtdraw/core/dialog_preference.py
+-rw-r--r--   0 hiro       (501) staff       (20)    16441 2023-05-15 12:36:33.000000 qtdraw-1.1.2/qtdraw/core/editable_widget.py
+-rw-r--r--   0 hiro       (501) staff       (20)     8466 2023-05-09 03:18:56.000000 qtdraw-1.1.2/qtdraw/core/group_model.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2233 2023-05-09 03:18:56.000000 qtdraw-1.1.2/qtdraw/core/group_panel.ui
+-rw-r--r--   0 hiro       (501) staff       (20)     1656 2023-05-09 03:18:56.000000 qtdraw-1.1.2/qtdraw/core/group_tab.py
+-rw-r--r--   0 hiro       (501) staff       (20)     4632 2023-05-09 03:18:56.000000 qtdraw-1.1.2/qtdraw/core/group_view.py
+-rw-r--r--   0 hiro       (501) staff       (20)     9744 2023-05-15 12:36:33.000000 qtdraw-1.1.2/qtdraw/core/line_edit.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2837 2023-05-15 12:36:33.000000 qtdraw-1.1.2/qtdraw/core/pixmap_converter.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2385 2023-05-09 03:18:56.000000 qtdraw-1.1.2/qtdraw/core/qt_logging.py
+-rw-r--r--   0 hiro       (501) staff       (20)   187925 2023-05-09 03:18:56.000000 qtdraw-1.1.2/qtdraw/core/qtdraw.png
+-rw-r--r--   0 hiro       (501) staff       (20)    31369 2023-05-09 03:18:56.000000 qtdraw-1.1.2/qtdraw/core/qtdraw.ui
+-rw-r--r--   0 hiro       (501) staff       (20)    17478 2023-05-09 03:18:56.000000 qtdraw-1.1.2/qtdraw/core/setting.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2678 2023-05-09 03:18:56.000000 qtdraw-1.1.2/qtdraw/core/table_dialog.py
+-rw-r--r--   0 hiro       (501) staff       (20)     4458 2023-05-09 03:18:56.000000 qtdraw-1.1.2/qtdraw/core/tree_item.py
+-rw-r--r--   0 hiro       (501) staff       (20)    16260 2023-05-09 03:18:56.000000 qtdraw-1.1.2/qtdraw/core/tree_item_model.py
+-rw-r--r--   0 hiro       (501) staff       (20)     7499 2023-05-15 12:36:33.000000 qtdraw-1.1.2/qtdraw/core/util.py
+-rw-r--r--   0 hiro       (501) staff       (20)     4715 2023-05-09 03:18:56.000000 qtdraw-1.1.2/qtdraw/core/validator.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-20 07:18:26.046900 qtdraw-1.1.2/qtdraw/multipie/
+-rw-r--r--   0 hiro       (501) staff       (20)    46964 2023-05-15 12:36:33.000000 qtdraw-1.1.2/qtdraw/multipie/dialog_group.py
+-rw-r--r--   0 hiro       (501) staff       (20)     9646 2023-05-15 12:36:32.000000 qtdraw-1.1.2/qtdraw/multipie/dialog_group_info.py
+-rw-r--r--   0 hiro       (501) staff       (20)     1839 2023-05-09 03:18:56.000000 qtdraw-1.1.2/qtdraw/multipie/setting.py
+-rw-------   0 hiro       (501) staff       (20)    92079 2023-05-20 07:09:31.000000 qtdraw-1.1.2/qtdraw/qt_draw.py
+-rw-r--r--   0 hiro       (501) staff       (20)     9242 2023-05-09 03:18:56.000000 qtdraw-1.1.2/qtdraw/qt_draw_base.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-05-20 07:18:26.042263 qtdraw-1.1.2/qtdraw.egg-info/
+-rw-r--r--   0 hiro       (501) staff       (20)     2414 2023-05-20 07:18:25.000000 qtdraw-1.1.2/qtdraw.egg-info/PKG-INFO
+-rw-r--r--   0 hiro       (501) staff       (20)      944 2023-05-20 07:18:26.000000 qtdraw-1.1.2/qtdraw.egg-info/SOURCES.txt
+-rw-r--r--   0 hiro       (501) staff       (20)        1 2023-05-20 07:18:26.000000 qtdraw-1.1.2/qtdraw.egg-info/dependency_links.txt
+-rw-r--r--   0 hiro       (501) staff       (20)       96 2023-05-20 07:18:26.000000 qtdraw-1.1.2/qtdraw.egg-info/requires.txt
+-rw-r--r--   0 hiro       (501) staff       (20)        7 2023-05-20 07:18:26.000000 qtdraw-1.1.2/qtdraw.egg-info/top_level.txt
+-rw-r--r--   0 hiro       (501) staff       (20)      640 2023-05-20 07:18:26.047561 qtdraw-1.1.2/setup.cfg
+-rw-r--r--   0 hiro       (501) staff       (20)       38 2023-05-09 03:18:56.000000 qtdraw-1.1.2/setup.py
```

### Comparing `qtdraw-1.1.1/LICENSE` & `qtdraw-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.1/PKG-INFO` & `qtdraw-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtdraw
-Version: 1.1.1
+Version: 1.1.2
 Summary: 3D drawing tool for molecules and crystals based on Pyvista and Qt.
 Home-page: https://github.com/CMT-MU/QtDraw
 Author: Hiroaki Kusunose
 Author-email: hiroaki.kusunose@gmail.com
 License: MIT
 Keywords: pyvista,qtpy5
 Requires-Python: >=3.8
```

### Comparing `qtdraw-1.1.1/README.md` & `qtdraw-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.1/qtdraw/core/basic_object.py` & `qtdraw-1.1.2/qtdraw/core/basic_object.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.1/qtdraw/core/color_dialog.py` & `qtdraw-1.1.2/qtdraw/core/color_dialog.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.1/qtdraw/core/color_palette.py` & `qtdraw-1.1.2/qtdraw/core/color_palette.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.1/qtdraw/core/default_panel.ui` & `qtdraw-1.1.2/qtdraw/core/default_panel.ui`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.1/qtdraw/core/dialog_about.py` & `qtdraw-1.1.2/qtdraw/core/dialog_about.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.1/qtdraw/core/dialog_preference.py` & `qtdraw-1.1.2/qtdraw/core/dialog_preference.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.1/qtdraw/core/editable_widget.py` & `qtdraw-1.1.2/qtdraw/core/editable_widget.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.1/qtdraw/core/group_model.py` & `qtdraw-1.1.2/qtdraw/core/group_model.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.1/qtdraw/core/group_panel.ui` & `qtdraw-1.1.2/qtdraw/core/group_panel.ui`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.1/qtdraw/core/group_tab.py` & `qtdraw-1.1.2/qtdraw/core/group_tab.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.1/qtdraw/core/group_view.py` & `qtdraw-1.1.2/qtdraw/core/group_view.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.1/qtdraw/core/line_edit.py` & `qtdraw-1.1.2/qtdraw/core/line_edit.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.1/qtdraw/core/pixmap_converter.py` & `qtdraw-1.1.2/qtdraw/core/pixmap_converter.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.1/qtdraw/core/qt_logging.py` & `qtdraw-1.1.2/qtdraw/core/qt_logging.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.1/qtdraw/core/qtdraw.png` & `qtdraw-1.1.2/qtdraw/core/qtdraw.png`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.1/qtdraw/core/qtdraw.ui` & `qtdraw-1.1.2/qtdraw/core/qtdraw.ui`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.1/qtdraw/core/setting.py` & `qtdraw-1.1.2/qtdraw/core/setting.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.1/qtdraw/core/table_dialog.py` & `qtdraw-1.1.2/qtdraw/core/table_dialog.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.1/qtdraw/core/tree_item.py` & `qtdraw-1.1.2/qtdraw/core/tree_item.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.1/qtdraw/core/tree_item_model.py` & `qtdraw-1.1.2/qtdraw/core/tree_item_model.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.1/qtdraw/core/util.py` & `qtdraw-1.1.2/qtdraw/core/util.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.1/qtdraw/core/validator.py` & `qtdraw-1.1.2/qtdraw/core/validator.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.1/qtdraw/multipie/dialog_group.py` & `qtdraw-1.1.2/qtdraw/multipie/dialog_group.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.1/qtdraw/multipie/dialog_group_info.py` & `qtdraw-1.1.2/qtdraw/multipie/dialog_group_info.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.1/qtdraw/multipie/setting.py` & `qtdraw-1.1.2/qtdraw/multipie/setting.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.1/qtdraw/qt_draw.py` & `qtdraw-1.1.2/qtdraw/qt_draw.py`

 * *Files 1% similar despite different names*

```diff
@@ -1786,18 +1786,20 @@
 
     # ==================================================
     def _show_actor(self, name, show):
         self._actorset[name].SetVisibility(show)
 
     # ==================================================
     def _remove_actor(self, name):
+        self._screen_off()
         if name in self._actorset.keys():
             obj_actor = self._actorset[name]
             self._layer.remove_actor(obj_actor)
             del self._actorset[name]
+        self._screen_on()
 
     # ==================================================
     def _remove_all_actor(self):
         names = list(self._actorset.keys())
         for name in names:
             self._remove_actor(name)
 
@@ -1940,14 +1942,15 @@
                 obj_id, lbl_id = row[-2:]
             if obj_id != "":
                 self._remove_actor(obj_id)
             if group not in ["caption", "text"] and lbl_id != "":
                 self._remove_actor(lbl_id)
             return
 
+        self._screen_off()
         if group == "caption":
             opt, obj_id, obj_show = self._data_to_object(group, row)
             if obj_id == "":
                 obj_id = self._actor_id()
                 self.dataset[group].iat[row_idx, -1] = obj_id
             obj_actor = self._layer.add_point_labels(name=obj_id, **opt)
             self._actorset[obj_id] = obj_actor
@@ -1971,14 +1974,15 @@
 
             if lbl_id == "":
                 lbl_id = self._actor_id()
                 self.dataset[group].iat[row_idx, -1] = lbl_id
             lbl_actor = self._layer.add_point_labels(name=lbl_id, **lbl_opt)
             self._actorset[lbl_id] = lbl_actor
             self._show_actor(lbl_id, lbl_show)
+        self._screen_on()
 
     # ==================================================
     def _check_in_view_range(self, obj):
         """
         check if object is in view range.
 
         Args:
```

### Comparing `qtdraw-1.1.1/qtdraw/qt_draw_base.py` & `qtdraw-1.1.2/qtdraw/qt_draw_base.py`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.1/qtdraw.egg-info/PKG-INFO` & `qtdraw-1.1.2/qtdraw.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtdraw
-Version: 1.1.1
+Version: 1.1.2
 Summary: 3D drawing tool for molecules and crystals based on Pyvista and Qt.
 Home-page: https://github.com/CMT-MU/QtDraw
 Author: Hiroaki Kusunose
 Author-email: hiroaki.kusunose@gmail.com
 License: MIT
 Keywords: pyvista,qtpy5
 Requires-Python: >=3.8
```

### Comparing `qtdraw-1.1.1/qtdraw.egg-info/SOURCES.txt` & `qtdraw-1.1.2/qtdraw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qtdraw-1.1.1/setup.cfg` & `qtdraw-1.1.2/setup.cfg`

 * *Files identical despite different names*

