# Comparing `tmp/EOmaps-6.4.1.tar.gz` & `tmp/EOmaps-6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/EOmaps-6.4.1.tar", last modified: Tue May  2 11:41:34 2023, max compression
+gzip compressed data, was "dist/EOmaps-6.5.tar", last modified: Fri May 19 22:13:11 2023, max compression
```

## Comparing `EOmaps-6.4.1.tar` & `EOmaps-6.5.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:41:34.000000 EOmaps-6.4.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:41:34.000000 EOmaps-6.4.1/EOmaps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13044 2023-05-02 11:41:33.000000 EOmaps-6.4.1/EOmaps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-02 11:41:34.000000 EOmaps-6.4.1/EOmaps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 11:41:33.000000 EOmaps-6.4.1/EOmaps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-02 11:41:33.000000 EOmaps-6.4.1/EOmaps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-02 11:41:33.000000 EOmaps-6.4.1/EOmaps.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-02 11:41:21.000000 EOmaps-6.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13044 2023-05-02 11:41:34.000000 EOmaps-6.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10507 2023-05-02 11:41:21.000000 EOmaps-6.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:41:34.000000 EOmaps-6.4.1/eomaps/
--rw-r--r--   0 runner    (1001) docker     (123)    17356 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/NE_features.json
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    68730 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/_cb_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/_containers.py
--rw-r--r--   0 runner    (1001) docker     (123)    27548 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/_data_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    62949 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/_shapes.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    46463 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/_webmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    81704 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/_webmap_containers.py
--rw-r--r--   0 runner    (1001) docker     (123)    40682 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    44442 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/colorbar.py
--rw-r--r--   0 runner    (1001) docker     (123)    19138 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/compass.py
--rw-r--r--   0 runner    (1001) docker     (123)    27961 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/draw.py
--rw-r--r--   0 runner    (1001) docker     (123)   176338 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/eomaps.py
--rw-r--r--   0 runner    (1001) docker     (123)    13143 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    82477 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    86617 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    16949 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/mapsgrid.py
--rw-r--r--   0 runner    (1001) docker     (123)    20044 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/ne_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/projections.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:41:34.000000 EOmaps-6.4.1/eomaps/qtcompanion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/base.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:41:34.000000 EOmaps-6.4.1/eomaps/qtcompanion/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/icons/close.png
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/icons/eye_closed.png
--rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/icons/eye_open.png
--rw-r--r--   0 runner    (1001) docker     (123)    86617 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/icons/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/icons/maximize.png
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/icons/peek_bottom.png
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/icons/peek_bottom_active.png
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/icons/peek_circle.png
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/icons/peek_circle_active.png
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/icons/peek_ellipse.png
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/icons/peek_ellipse_active.png
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/icons/peek_left.png
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/icons/peek_left_active.png
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/icons/peek_rectangle.png
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/icons/peek_rectangle_active.png
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/icons/peek_right.png
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/icons/peek_right_active.png
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/icons/peek_square.png
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/icons/peek_square_active.png
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/icons/peek_top.png
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/icons/peek_top_active.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:41:34.000000 EOmaps-6.4.1/eomaps/qtcompanion/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/widgets/annotate.py
--rw-r--r--   0 runner    (1001) docker     (123)    18878 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/widgets/click_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    12045 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/widgets/draw.py
--rw-r--r--   0 runner    (1001) docker     (123)    47567 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/widgets/editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/widgets/extent.py
--rw-r--r--   0 runner    (1001) docker     (123)    36930 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/widgets/files.py
--rw-r--r--   0 runner    (1001) docker     (123)    11221 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/widgets/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    18529 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/widgets/peek.py
--rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/widgets/save.py
--rw-r--r--   0 runner    (1001) docker     (123)    12801 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/widgets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    28994 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/qtcompanion/widgets/wms.py
--rw-r--r--   0 runner    (1001) docker     (123)    46756 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    56021 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/scalebar.py
--rw-r--r--   0 runner    (1001) docker     (123)    20486 2023-05-02 11:41:21.000000 EOmaps-6.4.1/eomaps/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 11:41:34.000000 EOmaps-6.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-05-02 11:41:21.000000 EOmaps-6.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:13:11.000000 EOmaps-6.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:13:11.000000 EOmaps-6.5/EOmaps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-05-19 22:13:11.000000 EOmaps-6.5/EOmaps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-19 22:13:11.000000 EOmaps-6.5/EOmaps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 22:13:11.000000 EOmaps-6.5/EOmaps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-19 22:13:11.000000 EOmaps-6.5/EOmaps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-19 22:13:11.000000 EOmaps-6.5/EOmaps.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-19 22:13:01.000000 EOmaps-6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-05-19 22:13:11.000000 EOmaps-6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11451 2023-05-19 22:13:01.000000 EOmaps-6.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:13:11.000000 EOmaps-6.5/eomaps/
+-rw-r--r--   0 runner    (1001) docker     (123)    17356 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/NE_features.json
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68730 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/_cb_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/_containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27548 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/_data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62949 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46463 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/_webmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81704 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/_webmap_containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40642 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47507 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/colorbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19769 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/compass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27961 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/draw.py
+-rw-r--r--   0 runner    (1001) docker     (123)   182461 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/eomaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32256 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82477 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86617 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16949 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/mapsgrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20422 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/ne_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/projections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:13:11.000000 EOmaps-6.5/eomaps/qtcompanion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:13:11.000000 EOmaps-6.5/eomaps/qtcompanion/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/icons/close.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/icons/eye_closed.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/icons/eye_open.png
+-rw-r--r--   0 runner    (1001) docker     (123)    86617 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/icons/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/icons/maximize.png
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/icons/peek_bottom.png
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/icons/peek_bottom_active.png
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/icons/peek_circle.png
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/icons/peek_circle_active.png
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/icons/peek_ellipse.png
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/icons/peek_ellipse_active.png
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/icons/peek_left.png
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/icons/peek_left_active.png
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/icons/peek_rectangle.png
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/icons/peek_rectangle_active.png
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/icons/peek_right.png
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/icons/peek_right_active.png
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/icons/peek_square.png
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/icons/peek_square_active.png
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/icons/peek_top.png
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/icons/peek_top_active.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:13:11.000000 EOmaps-6.5/eomaps/qtcompanion/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/widgets/annotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18878 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/widgets/click_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12045 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/widgets/draw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47565 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/widgets/editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/widgets/extent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36930 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/widgets/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11221 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/widgets/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18529 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/widgets/peek.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/widgets/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12801 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/widgets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28994 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/qtcompanion/widgets/wms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52347 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56021 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/scalebar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20639 2023-05-19 22:13:01.000000 EOmaps-6.5/eomaps/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 22:13:11.000000 EOmaps-6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-05-19 22:13:01.000000 EOmaps-6.5/setup.py
```

### Comparing `EOmaps-6.4.1/EOmaps.egg-info/PKG-INFO` & `EOmaps-6.5/EOmaps.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EOmaps
-Version: 6.4.1
+Version: 6.5
 Summary: A library to create interactive maps of geographical datasets.
 Home-page: https://github.com/raphaelquast/maps
 Author: Raphael Quast
 Author-email: raphael.quast@geo.tuwien.ac.at
 Maintainer: Raphael Quast
 Maintainer-email: raphael.quast@geo.tuwien.ac.at
 License: GNU General Public License v3 or later (GPLv3+)
@@ -29,27 +29,35 @@
         
         <a href="https://zenodo.org/badge/latestdoi/410829039" target="_blank"><img src="https://zenodo.org/badge/410829039.svg" alt="DOI: 10.5281/zenodo.6459598" align="right" style="height: 20px !important;" ></a>
         
         ----
         
         # EOmaps - Interactive maps in python!
         
-        EOmaps is a <tt>python</tt> package to visualize and analyze geographical datasets.
+        **EOmaps** is a <tt>python</tt> package to visualize and analyze geographical datasets.
         
-        It is built on top of [matplotlib](matplotlib.org/) and [cartopy](https://scitools.org.uk/cartopy/docs/latest/) and aims to provide an
-        intuitive and easy-to-use interface to speed up and simplify the creation and comparison of maps.
+        It is built on top of [matplotlib](matplotlib.org/) and [cartopy](https://scitools.org.uk/cartopy/docs/latest/) and provides an intuitive and easy-to-use interface to speed up and simplify the creation and comparison of maps.
+        
+        ### What can EOmaps do for you?
+        - Create [▤ multi-layered maps](https://eomaps.readthedocs.io/en/dev/api.html#basics) and interactively compare different layers with each other
+        - [🔴 Visualize datasets](https://eomaps.readthedocs.io/en/dev/api.html#data-visualization) with  millions of datapoints and handle reprojections
+        - Provide a comprehensive set of tools to customize the map
+          - [🌵NaturalEarth features](https://eomaps.readthedocs.io/en/dev/api.html#naturalearth-features)
+          - [📏Scalebars](https://eomaps.readthedocs.io/en/dev/api.html#scalebars)
+          - [▦ Gridlines](https://eomaps.readthedocs.io/en/dev/api.html#gridlines)
+          - [🛰 WebMap layers](https://eomaps.readthedocs.io/en/dev/api.html#webmap-layers)
+          - [🏕 Annotations, Markers, Lines, Logos...](https://eomaps.readthedocs.io/en/latest/api.html#annotations-markers-lines-logos-etc)
+          - . . .
+        - Use [🛸 Callbacks](https://eomaps.readthedocs.io/en/latest/api.html#callbacks-make-the-map-interactive) and the [🧰 CompanionWidget](https://eomaps.readthedocs.io/en/dev/api.html#companion-widget) to interact with the figure
+        - Interactively re-arrange multiple maps in a figure with the [🏗️ LayoutEditor](https://eomaps.readthedocs.io/en/dev/api.html#layout-editor)
+        - [🗺 Export](https://eomaps.readthedocs.io/en/dev/api.html#export-the-map-as-jpeg-png-etc) publication ready high resolution images (png, jpeg etc.)
+        - . . . and much more!  
+        
+        Checkout the [🚀 Basics](https://eomaps.readthedocs.io/en/dev/api.html#basics) in the documentation to get started!
         
-        - Visualize small datasets as well as millions of datapoints
-        - Handle 1D and 2D datasets with the same interface and create plots from NetCDF, GeoTIFF or CSV files
-        - Take care of re-projecting the data
-        - Compare, combine or (transparently) overlay multiple plot-layers
-        - Turn the maps into interactive data-analysis widgets with a few lines of code
-        - Provide a versatile set of tools to customize the maps (Features, WebMaps, Markers, Annotations etc.)
-        - Simplify the process of composing multiple maps (and other plots/images) in a single figure
-        - Export high resolution images (png, jpeg etc.)
         
         ## 🔨 Installation
         
         To install EOmaps (and all its dependencies) via the [conda](https://docs.conda.io/projects/conda/en/stable/) package-manager, simply use:
         ```python
         conda install -c conda-forge eomaps
         ```
@@ -60,15 +68,15 @@
         ```
         Need more information?
         - Have a look at the [🐛Installation](https://eomaps.readthedocs.io/en/latest/general.html#installation) instructions in the docs.
         - Checkout the quickstart guide [🚀 From 0 to EOmaps](https://eomaps.readthedocs.io/en/latest/FAQ.html#from-0-to-eomaps-a-quickstart-guide).
         
         ## 📖 Documentation
         
-        Make sure to have a look at the <a href=https://eomaps.readthedocs.io/en/latest><b>🌳 Documentation 🌳</b></a> which provides a lot of <a href=https://eomaps.readthedocs.io/en/latest/EOmaps_examples.html><b>🌐Examples</b></a> on how to create awesome interactive maps (incl. 🐍 source code)!
+        Make sure to have a look at the <a href=https://eomaps.readthedocs.io/en/latest><b>📖 Documentation </b></a> which provides a lot of <a href=https://eomaps.readthedocs.io/en/latest/EOmaps_examples.html><b>🌐Examples</b></a> on how to create awesome interactive maps (incl. 🐍 source code)!
         
         ## ✔️ Citation
         Did EOmaps help in your research?  
         Support the development and add a citation to your publication!
         
         [![https://doi.org/10.5281/zenodo.6459598](https://zenodo.org/badge/410829039.svg)](https://zenodo.org/badge/latestdoi/410829039)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EOmaps Version: 6.4.1 Summary: A library to create
+Metadata-Version: 2.1 Name: EOmaps Version: 6.5 Summary: A library to create
 interactive maps of geographical datasets. Home-page: https://github.com/
 raphaelquast/maps Author: Raphael Quast Author-email:
 raphael.quast@geo.tuwien.ac.at Maintainer: Raphael Quast Maintainer-email:
 raphael.quast@geo.tuwien.ac.at License: GNU General Public License v3 or later
 (GPLv3+) Description:
                                  [EOmaps_logo]
 [![tests](https://github.com/raphaelquast/EOmaps/actions/workflows/
@@ -11,54 +11,67 @@
 EOmaps/graph/badge.svg)](https://codecov.io/gh/raphaelquast/EOmaps)       [!
 [pypi](https://img.shields.io/pypi/v/eomaps)](https://pypi.org/project/eomaps/
 ) [![Conda Version](https://img.shields.io/conda/vn/conda-forge/eomaps.svg)]
 (https://anaconda.org/conda-forge/eomaps)       [![Documentation Status](https:
 //readthedocs.org/projects/eomaps/badge/?version=latest)](https://
 eomaps.readthedocs.io/en/latest/?badge=latest)       [Buy_Me_A_Coffee] [chat_on
 gitter] [DOI:_10.5281/zenodo.6459598] ---- # EOmaps - Interactive maps in
-python! EOmaps is a python package to visualize and analyze geographical
+python! **EOmaps** is a python package to visualize and analyze geographical
 datasets. It is built on top of [matplotlib](matplotlib.org/) and [cartopy]
-(https://scitools.org.uk/cartopy/docs/latest/) and aims to provide an intuitive
-and easy-to-use interface to speed up and simplify the creation and comparison
-of maps. - Visualize small datasets as well as millions of datapoints - Handle
-1D and 2D datasets with the same interface and create plots from NetCDF,
-GeoTIFF or CSV files - Take care of re-projecting the data - Compare, combine
-or (transparently) overlay multiple plot-layers - Turn the maps into
-interactive data-analysis widgets with a few lines of code - Provide a
-versatile set of tools to customize the maps (Features, WebMaps, Markers,
-Annotations etc.) - Simplify the process of composing multiple maps (and other
-plots/images) in a single figure - Export high resolution images (png, jpeg
-etc.) ## ð¨ Installation To install EOmaps (and all its dependencies) via the
-[conda](https://docs.conda.io/projects/conda/en/stable/) package-manager,
-simply use: ```python conda install -c conda-forge eomaps ``` ... to get a
-**huge_speedup**, use [mamba](https://mamba.readthedocs.io/en/latest/) to solve
-the dependencies! ```python conda install -c conda-forge mamba mamba install -
-c conda-forge eomaps ``` Need more information? - Have a look at the
-[ðInstallation](https://eomaps.readthedocs.io/en/latest/
-general.html#installation) instructions in the docs. - Checkout the quickstart
-guide [ð From 0 to EOmaps](https://eomaps.readthedocs.io/en/latest/
-FAQ.html#from-0-to-eomaps-a-quickstart-guide). ## ð Documentation Make sure
-to have a look at the ð³_Documentation_ð³ which provides a lot of
-ðExamples on how to create awesome interactive maps (incl. ð source
-code)! ## âï¸ Citation Did EOmaps help in your research? Support the
-development and add a citation to your publication! [![https://doi.org/10.5281/
-zenodo.6459598](https://zenodo.org/badge/410829039.svg)](https://zenodo.org/
-badge/latestdoi/410829039) ## ð Contribute Found a bug or got an idea for an
-interesting feature? Open an [issue](https://github.com/raphaelquast/EOmaps/
-issues) or start a [discussion](https://github.com/raphaelquast/EOmaps/
-discussions), and I'll see what I can do! Interested in actively contributing
-to the library? Awesome! - Any contributions are welcome! - New features (or
-ideas for new features) - Enhancements for existing features - Bug-fixes, code-
-style improvements, unittests etc. - Documentation updates - Outreach (e.g.
-blog-posts, tutorials, talks ... ) - Have a look at existing [Issues](https://
-github.com/raphaelquast/EOmaps/contribute) or this [ð overview project]
-(https://github.com/users/raphaelquast/projects/5/views/8) to see where EOmaps
-could use your help. - Get in touch by opening a discussion in the [ð
-Contribution](https://github.com/raphaelquast/EOmaps/discussions/categories/
-contribution) section! ---------------
+(https://scitools.org.uk/cartopy/docs/latest/) and provides an intuitive and
+easy-to-use interface to speed up and simplify the creation and comparison of
+maps. ### What can EOmaps do for you? - Create [â¤ multi-layered maps](https:/
+/eomaps.readthedocs.io/en/dev/api.html#basics) and interactively compare
+different layers with each other - [ð´ Visualize datasets](https://
+eomaps.readthedocs.io/en/dev/api.html#data-visualization) with millions of
+datapoints and handle reprojections - Provide a comprehensive set of tools to
+customize the map - [ðµNaturalEarth features](https://eomaps.readthedocs.io/
+en/dev/api.html#naturalearth-features) - [ðScalebars](https://
+eomaps.readthedocs.io/en/dev/api.html#scalebars) - [â¦ Gridlines](https://
+eomaps.readthedocs.io/en/dev/api.html#gridlines) - [ð° WebMap layers](https:/
+/eomaps.readthedocs.io/en/dev/api.html#webmap-layers) - [ð Annotations,
+Markers, Lines, Logos...](https://eomaps.readthedocs.io/en/latest/
+api.html#annotations-markers-lines-logos-etc) - . . . - Use [ð¸ Callbacks]
+(https://eomaps.readthedocs.io/en/latest/api.html#callbacks-make-the-map-
+interactive) and the [ð§° CompanionWidget](https://eomaps.readthedocs.io/en/
+dev/api.html#companion-widget) to interact with the figure - Interactively re-
+arrange multiple maps in a figure with the [ðï¸ LayoutEditor](https://
+eomaps.readthedocs.io/en/dev/api.html#layout-editor) - [ðº Export](https://
+eomaps.readthedocs.io/en/dev/api.html#export-the-map-as-jpeg-png-etc)
+publication ready high resolution images (png, jpeg etc.) - . . . and much
+more! Checkout the [ð Basics](https://eomaps.readthedocs.io/en/dev/
+api.html#basics) in the documentation to get started! ## ð¨ Installation To
+install EOmaps (and all its dependencies) via the [conda](https://
+docs.conda.io/projects/conda/en/stable/) package-manager, simply use: ```python
+conda install -c conda-forge eomaps ``` ... to get a **huge_speedup**, use
+[mamba](https://mamba.readthedocs.io/en/latest/) to solve the dependencies!
+```python conda install -c conda-forge mamba mamba install -c conda-forge
+eomaps ``` Need more information? - Have a look at the [ðInstallation]
+(https://eomaps.readthedocs.io/en/latest/general.html#installation)
+instructions in the docs. - Checkout the quickstart guide [ð From 0 to
+EOmaps](https://eomaps.readthedocs.io/en/latest/FAQ.html#from-0-to-eomaps-a-
+quickstart-guide). ## ð Documentation Make sure to have a look at the ð
+Documentation which provides a lot of ðExamples on how to create awesome
+interactive maps (incl. ð source code)! ## âï¸ Citation Did EOmaps help
+in your research? Support the development and add a citation to your
+publication! [![https://doi.org/10.5281/zenodo.6459598](https://zenodo.org/
+badge/410829039.svg)](https://zenodo.org/badge/latestdoi/410829039) ## ð
+Contribute Found a bug or got an idea for an interesting feature? Open an
+[issue](https://github.com/raphaelquast/EOmaps/issues) or start a [discussion]
+(https://github.com/raphaelquast/EOmaps/discussions), and I'll see what I can
+do! Interested in actively contributing to the library? Awesome! - Any
+contributions are welcome! - New features (or ideas for new features) -
+Enhancements for existing features - Bug-fixes, code-style improvements,
+unittests etc. - Documentation updates - Outreach (e.g. blog-posts, tutorials,
+talks ... ) - Have a look at existing [Issues](https://github.com/raphaelquast/
+EOmaps/contribute) or this [ð overview project](https://github.com/users/
+raphaelquast/projects/5/views/8) to see where EOmaps could use your help. - Get
+in touch by opening a discussion in the [ð Contribution](https://github.com/
+raphaelquast/EOmaps/discussions/categories/contribution) section! -------------
+--
 [EOmaps example 6]  [EOmaps example 2]
 [EOmaps example 9]  [EOmaps example 4]
 [EOmaps example 7]  [EOmaps example 8]
 [EOmaps inset-maps] [EOmaps example 3]
 [EOmaps example 9]  [EOmaps example 4]
 ## ð³ Basic usage **Checkout the [ð Basics](https://eomaps.readthedocs.io/
 en/latest/api.html)** in the documentation! ```python from eomaps import Maps
```

### Comparing `EOmaps-6.4.1/EOmaps.egg-info/SOURCES.txt` & `EOmaps-6.5/EOmaps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4.1/LICENSE` & `EOmaps-6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4.1/PKG-INFO` & `EOmaps-6.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EOmaps
-Version: 6.4.1
+Version: 6.5
 Summary: A library to create interactive maps of geographical datasets.
 Home-page: https://github.com/raphaelquast/maps
 Author: Raphael Quast
 Author-email: raphael.quast@geo.tuwien.ac.at
 Maintainer: Raphael Quast
 Maintainer-email: raphael.quast@geo.tuwien.ac.at
 License: GNU General Public License v3 or later (GPLv3+)
@@ -29,27 +29,35 @@
         
         <a href="https://zenodo.org/badge/latestdoi/410829039" target="_blank"><img src="https://zenodo.org/badge/410829039.svg" alt="DOI: 10.5281/zenodo.6459598" align="right" style="height: 20px !important;" ></a>
         
         ----
         
         # EOmaps - Interactive maps in python!
         
-        EOmaps is a <tt>python</tt> package to visualize and analyze geographical datasets.
+        **EOmaps** is a <tt>python</tt> package to visualize and analyze geographical datasets.
         
-        It is built on top of [matplotlib](matplotlib.org/) and [cartopy](https://scitools.org.uk/cartopy/docs/latest/) and aims to provide an
-        intuitive and easy-to-use interface to speed up and simplify the creation and comparison of maps.
+        It is built on top of [matplotlib](matplotlib.org/) and [cartopy](https://scitools.org.uk/cartopy/docs/latest/) and provides an intuitive and easy-to-use interface to speed up and simplify the creation and comparison of maps.
+        
+        ### What can EOmaps do for you?
+        - Create [▤ multi-layered maps](https://eomaps.readthedocs.io/en/dev/api.html#basics) and interactively compare different layers with each other
+        - [🔴 Visualize datasets](https://eomaps.readthedocs.io/en/dev/api.html#data-visualization) with  millions of datapoints and handle reprojections
+        - Provide a comprehensive set of tools to customize the map
+          - [🌵NaturalEarth features](https://eomaps.readthedocs.io/en/dev/api.html#naturalearth-features)
+          - [📏Scalebars](https://eomaps.readthedocs.io/en/dev/api.html#scalebars)
+          - [▦ Gridlines](https://eomaps.readthedocs.io/en/dev/api.html#gridlines)
+          - [🛰 WebMap layers](https://eomaps.readthedocs.io/en/dev/api.html#webmap-layers)
+          - [🏕 Annotations, Markers, Lines, Logos...](https://eomaps.readthedocs.io/en/latest/api.html#annotations-markers-lines-logos-etc)
+          - . . .
+        - Use [🛸 Callbacks](https://eomaps.readthedocs.io/en/latest/api.html#callbacks-make-the-map-interactive) and the [🧰 CompanionWidget](https://eomaps.readthedocs.io/en/dev/api.html#companion-widget) to interact with the figure
+        - Interactively re-arrange multiple maps in a figure with the [🏗️ LayoutEditor](https://eomaps.readthedocs.io/en/dev/api.html#layout-editor)
+        - [🗺 Export](https://eomaps.readthedocs.io/en/dev/api.html#export-the-map-as-jpeg-png-etc) publication ready high resolution images (png, jpeg etc.)
+        - . . . and much more!  
+        
+        Checkout the [🚀 Basics](https://eomaps.readthedocs.io/en/dev/api.html#basics) in the documentation to get started!
         
-        - Visualize small datasets as well as millions of datapoints
-        - Handle 1D and 2D datasets with the same interface and create plots from NetCDF, GeoTIFF or CSV files
-        - Take care of re-projecting the data
-        - Compare, combine or (transparently) overlay multiple plot-layers
-        - Turn the maps into interactive data-analysis widgets with a few lines of code
-        - Provide a versatile set of tools to customize the maps (Features, WebMaps, Markers, Annotations etc.)
-        - Simplify the process of composing multiple maps (and other plots/images) in a single figure
-        - Export high resolution images (png, jpeg etc.)
         
         ## 🔨 Installation
         
         To install EOmaps (and all its dependencies) via the [conda](https://docs.conda.io/projects/conda/en/stable/) package-manager, simply use:
         ```python
         conda install -c conda-forge eomaps
         ```
@@ -60,15 +68,15 @@
         ```
         Need more information?
         - Have a look at the [🐛Installation](https://eomaps.readthedocs.io/en/latest/general.html#installation) instructions in the docs.
         - Checkout the quickstart guide [🚀 From 0 to EOmaps](https://eomaps.readthedocs.io/en/latest/FAQ.html#from-0-to-eomaps-a-quickstart-guide).
         
         ## 📖 Documentation
         
-        Make sure to have a look at the <a href=https://eomaps.readthedocs.io/en/latest><b>🌳 Documentation 🌳</b></a> which provides a lot of <a href=https://eomaps.readthedocs.io/en/latest/EOmaps_examples.html><b>🌐Examples</b></a> on how to create awesome interactive maps (incl. 🐍 source code)!
+        Make sure to have a look at the <a href=https://eomaps.readthedocs.io/en/latest><b>📖 Documentation </b></a> which provides a lot of <a href=https://eomaps.readthedocs.io/en/latest/EOmaps_examples.html><b>🌐Examples</b></a> on how to create awesome interactive maps (incl. 🐍 source code)!
         
         ## ✔️ Citation
         Did EOmaps help in your research?  
         Support the development and add a citation to your publication!
         
         [![https://doi.org/10.5281/zenodo.6459598](https://zenodo.org/badge/410829039.svg)](https://zenodo.org/badge/latestdoi/410829039)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EOmaps Version: 6.4.1 Summary: A library to create
+Metadata-Version: 2.1 Name: EOmaps Version: 6.5 Summary: A library to create
 interactive maps of geographical datasets. Home-page: https://github.com/
 raphaelquast/maps Author: Raphael Quast Author-email:
 raphael.quast@geo.tuwien.ac.at Maintainer: Raphael Quast Maintainer-email:
 raphael.quast@geo.tuwien.ac.at License: GNU General Public License v3 or later
 (GPLv3+) Description:
                                  [EOmaps_logo]
 [![tests](https://github.com/raphaelquast/EOmaps/actions/workflows/
@@ -11,54 +11,67 @@
 EOmaps/graph/badge.svg)](https://codecov.io/gh/raphaelquast/EOmaps)       [!
 [pypi](https://img.shields.io/pypi/v/eomaps)](https://pypi.org/project/eomaps/
 ) [![Conda Version](https://img.shields.io/conda/vn/conda-forge/eomaps.svg)]
 (https://anaconda.org/conda-forge/eomaps)       [![Documentation Status](https:
 //readthedocs.org/projects/eomaps/badge/?version=latest)](https://
 eomaps.readthedocs.io/en/latest/?badge=latest)       [Buy_Me_A_Coffee] [chat_on
 gitter] [DOI:_10.5281/zenodo.6459598] ---- # EOmaps - Interactive maps in
-python! EOmaps is a python package to visualize and analyze geographical
+python! **EOmaps** is a python package to visualize and analyze geographical
 datasets. It is built on top of [matplotlib](matplotlib.org/) and [cartopy]
-(https://scitools.org.uk/cartopy/docs/latest/) and aims to provide an intuitive
-and easy-to-use interface to speed up and simplify the creation and comparison
-of maps. - Visualize small datasets as well as millions of datapoints - Handle
-1D and 2D datasets with the same interface and create plots from NetCDF,
-GeoTIFF or CSV files - Take care of re-projecting the data - Compare, combine
-or (transparently) overlay multiple plot-layers - Turn the maps into
-interactive data-analysis widgets with a few lines of code - Provide a
-versatile set of tools to customize the maps (Features, WebMaps, Markers,
-Annotations etc.) - Simplify the process of composing multiple maps (and other
-plots/images) in a single figure - Export high resolution images (png, jpeg
-etc.) ## ð¨ Installation To install EOmaps (and all its dependencies) via the
-[conda](https://docs.conda.io/projects/conda/en/stable/) package-manager,
-simply use: ```python conda install -c conda-forge eomaps ``` ... to get a
-**huge_speedup**, use [mamba](https://mamba.readthedocs.io/en/latest/) to solve
-the dependencies! ```python conda install -c conda-forge mamba mamba install -
-c conda-forge eomaps ``` Need more information? - Have a look at the
-[ðInstallation](https://eomaps.readthedocs.io/en/latest/
-general.html#installation) instructions in the docs. - Checkout the quickstart
-guide [ð From 0 to EOmaps](https://eomaps.readthedocs.io/en/latest/
-FAQ.html#from-0-to-eomaps-a-quickstart-guide). ## ð Documentation Make sure
-to have a look at the ð³_Documentation_ð³ which provides a lot of
-ðExamples on how to create awesome interactive maps (incl. ð source
-code)! ## âï¸ Citation Did EOmaps help in your research? Support the
-development and add a citation to your publication! [![https://doi.org/10.5281/
-zenodo.6459598](https://zenodo.org/badge/410829039.svg)](https://zenodo.org/
-badge/latestdoi/410829039) ## ð Contribute Found a bug or got an idea for an
-interesting feature? Open an [issue](https://github.com/raphaelquast/EOmaps/
-issues) or start a [discussion](https://github.com/raphaelquast/EOmaps/
-discussions), and I'll see what I can do! Interested in actively contributing
-to the library? Awesome! - Any contributions are welcome! - New features (or
-ideas for new features) - Enhancements for existing features - Bug-fixes, code-
-style improvements, unittests etc. - Documentation updates - Outreach (e.g.
-blog-posts, tutorials, talks ... ) - Have a look at existing [Issues](https://
-github.com/raphaelquast/EOmaps/contribute) or this [ð overview project]
-(https://github.com/users/raphaelquast/projects/5/views/8) to see where EOmaps
-could use your help. - Get in touch by opening a discussion in the [ð
-Contribution](https://github.com/raphaelquast/EOmaps/discussions/categories/
-contribution) section! ---------------
+(https://scitools.org.uk/cartopy/docs/latest/) and provides an intuitive and
+easy-to-use interface to speed up and simplify the creation and comparison of
+maps. ### What can EOmaps do for you? - Create [â¤ multi-layered maps](https:/
+/eomaps.readthedocs.io/en/dev/api.html#basics) and interactively compare
+different layers with each other - [ð´ Visualize datasets](https://
+eomaps.readthedocs.io/en/dev/api.html#data-visualization) with millions of
+datapoints and handle reprojections - Provide a comprehensive set of tools to
+customize the map - [ðµNaturalEarth features](https://eomaps.readthedocs.io/
+en/dev/api.html#naturalearth-features) - [ðScalebars](https://
+eomaps.readthedocs.io/en/dev/api.html#scalebars) - [â¦ Gridlines](https://
+eomaps.readthedocs.io/en/dev/api.html#gridlines) - [ð° WebMap layers](https:/
+/eomaps.readthedocs.io/en/dev/api.html#webmap-layers) - [ð Annotations,
+Markers, Lines, Logos...](https://eomaps.readthedocs.io/en/latest/
+api.html#annotations-markers-lines-logos-etc) - . . . - Use [ð¸ Callbacks]
+(https://eomaps.readthedocs.io/en/latest/api.html#callbacks-make-the-map-
+interactive) and the [ð§° CompanionWidget](https://eomaps.readthedocs.io/en/
+dev/api.html#companion-widget) to interact with the figure - Interactively re-
+arrange multiple maps in a figure with the [ðï¸ LayoutEditor](https://
+eomaps.readthedocs.io/en/dev/api.html#layout-editor) - [ðº Export](https://
+eomaps.readthedocs.io/en/dev/api.html#export-the-map-as-jpeg-png-etc)
+publication ready high resolution images (png, jpeg etc.) - . . . and much
+more! Checkout the [ð Basics](https://eomaps.readthedocs.io/en/dev/
+api.html#basics) in the documentation to get started! ## ð¨ Installation To
+install EOmaps (and all its dependencies) via the [conda](https://
+docs.conda.io/projects/conda/en/stable/) package-manager, simply use: ```python
+conda install -c conda-forge eomaps ``` ... to get a **huge_speedup**, use
+[mamba](https://mamba.readthedocs.io/en/latest/) to solve the dependencies!
+```python conda install -c conda-forge mamba mamba install -c conda-forge
+eomaps ``` Need more information? - Have a look at the [ðInstallation]
+(https://eomaps.readthedocs.io/en/latest/general.html#installation)
+instructions in the docs. - Checkout the quickstart guide [ð From 0 to
+EOmaps](https://eomaps.readthedocs.io/en/latest/FAQ.html#from-0-to-eomaps-a-
+quickstart-guide). ## ð Documentation Make sure to have a look at the ð
+Documentation which provides a lot of ðExamples on how to create awesome
+interactive maps (incl. ð source code)! ## âï¸ Citation Did EOmaps help
+in your research? Support the development and add a citation to your
+publication! [![https://doi.org/10.5281/zenodo.6459598](https://zenodo.org/
+badge/410829039.svg)](https://zenodo.org/badge/latestdoi/410829039) ## ð
+Contribute Found a bug or got an idea for an interesting feature? Open an
+[issue](https://github.com/raphaelquast/EOmaps/issues) or start a [discussion]
+(https://github.com/raphaelquast/EOmaps/discussions), and I'll see what I can
+do! Interested in actively contributing to the library? Awesome! - Any
+contributions are welcome! - New features (or ideas for new features) -
+Enhancements for existing features - Bug-fixes, code-style improvements,
+unittests etc. - Documentation updates - Outreach (e.g. blog-posts, tutorials,
+talks ... ) - Have a look at existing [Issues](https://github.com/raphaelquast/
+EOmaps/contribute) or this [ð overview project](https://github.com/users/
+raphaelquast/projects/5/views/8) to see where EOmaps could use your help. - Get
+in touch by opening a discussion in the [ð Contribution](https://github.com/
+raphaelquast/EOmaps/discussions/categories/contribution) section! -------------
+--
 [EOmaps example 6]  [EOmaps example 2]
 [EOmaps example 9]  [EOmaps example 4]
 [EOmaps example 7]  [EOmaps example 8]
 [EOmaps inset-maps] [EOmaps example 3]
 [EOmaps example 9]  [EOmaps example 4]
 ## ð³ Basic usage **Checkout the [ð Basics](https://eomaps.readthedocs.io/
 en/latest/api.html)** in the documentation! ```python from eomaps import Maps
```

### Comparing `EOmaps-6.4.1/README.md` & `EOmaps-6.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -19,27 +19,35 @@
 
 <a href="https://zenodo.org/badge/latestdoi/410829039" target="_blank"><img src="https://zenodo.org/badge/410829039.svg" alt="DOI: 10.5281/zenodo.6459598" align="right" style="height: 20px !important;" ></a>
 
 ----
 
 # EOmaps - Interactive maps in python!
 
-EOmaps is a <tt>python</tt> package to visualize and analyze geographical datasets.
+**EOmaps** is a <tt>python</tt> package to visualize and analyze geographical datasets.
 
-It is built on top of [matplotlib](matplotlib.org/) and [cartopy](https://scitools.org.uk/cartopy/docs/latest/) and aims to provide an
-intuitive and easy-to-use interface to speed up and simplify the creation and comparison of maps.
+It is built on top of [matplotlib](matplotlib.org/) and [cartopy](https://scitools.org.uk/cartopy/docs/latest/) and provides an intuitive and easy-to-use interface to speed up and simplify the creation and comparison of maps.
+
+### What can EOmaps do for you?
+- Create [▤ multi-layered maps](https://eomaps.readthedocs.io/en/dev/api.html#basics) and interactively compare different layers with each other
+- [🔴 Visualize datasets](https://eomaps.readthedocs.io/en/dev/api.html#data-visualization) with  millions of datapoints and handle reprojections
+- Provide a comprehensive set of tools to customize the map
+  - [🌵NaturalEarth features](https://eomaps.readthedocs.io/en/dev/api.html#naturalearth-features)
+  - [📏Scalebars](https://eomaps.readthedocs.io/en/dev/api.html#scalebars)
+  - [▦ Gridlines](https://eomaps.readthedocs.io/en/dev/api.html#gridlines)
+  - [🛰 WebMap layers](https://eomaps.readthedocs.io/en/dev/api.html#webmap-layers)
+  - [🏕 Annotations, Markers, Lines, Logos...](https://eomaps.readthedocs.io/en/latest/api.html#annotations-markers-lines-logos-etc)
+  - . . .
+- Use [🛸 Callbacks](https://eomaps.readthedocs.io/en/latest/api.html#callbacks-make-the-map-interactive) and the [🧰 CompanionWidget](https://eomaps.readthedocs.io/en/dev/api.html#companion-widget) to interact with the figure
+- Interactively re-arrange multiple maps in a figure with the [🏗️ LayoutEditor](https://eomaps.readthedocs.io/en/dev/api.html#layout-editor)
+- [🗺 Export](https://eomaps.readthedocs.io/en/dev/api.html#export-the-map-as-jpeg-png-etc) publication ready high resolution images (png, jpeg etc.)
+- . . . and much more!  
+
+Checkout the [🚀 Basics](https://eomaps.readthedocs.io/en/dev/api.html#basics) in the documentation to get started!
 
-- Visualize small datasets as well as millions of datapoints
-- Handle 1D and 2D datasets with the same interface and create plots from NetCDF, GeoTIFF or CSV files
-- Take care of re-projecting the data
-- Compare, combine or (transparently) overlay multiple plot-layers
-- Turn the maps into interactive data-analysis widgets with a few lines of code
-- Provide a versatile set of tools to customize the maps (Features, WebMaps, Markers, Annotations etc.)
-- Simplify the process of composing multiple maps (and other plots/images) in a single figure
-- Export high resolution images (png, jpeg etc.)
 
 ## 🔨 Installation
 
 To install EOmaps (and all its dependencies) via the [conda](https://docs.conda.io/projects/conda/en/stable/) package-manager, simply use:
 ```python
 conda install -c conda-forge eomaps
 ```
@@ -50,15 +58,15 @@
 ```
 Need more information?
 - Have a look at the [🐛Installation](https://eomaps.readthedocs.io/en/latest/general.html#installation) instructions in the docs.
 - Checkout the quickstart guide [🚀 From 0 to EOmaps](https://eomaps.readthedocs.io/en/latest/FAQ.html#from-0-to-eomaps-a-quickstart-guide).
 
 ## 📖 Documentation
 
-Make sure to have a look at the <a href=https://eomaps.readthedocs.io/en/latest><b>🌳 Documentation 🌳</b></a> which provides a lot of <a href=https://eomaps.readthedocs.io/en/latest/EOmaps_examples.html><b>🌐Examples</b></a> on how to create awesome interactive maps (incl. 🐍 source code)!
+Make sure to have a look at the <a href=https://eomaps.readthedocs.io/en/latest><b>📖 Documentation </b></a> which provides a lot of <a href=https://eomaps.readthedocs.io/en/latest/EOmaps_examples.html><b>🌐Examples</b></a> on how to create awesome interactive maps (incl. 🐍 source code)!
 
 ## ✔️ Citation
 Did EOmaps help in your research?  
 Support the development and add a citation to your publication!
 
 [![https://doi.org/10.5281/zenodo.6459598](https://zenodo.org/badge/410829039.svg)](https://zenodo.org/badge/latestdoi/410829039)
```

#### html2text {}

```diff
@@ -5,54 +5,67 @@
 EOmaps/graph/badge.svg)](https://codecov.io/gh/raphaelquast/EOmaps)       [!
 [pypi](https://img.shields.io/pypi/v/eomaps)](https://pypi.org/project/eomaps/
 ) [![Conda Version](https://img.shields.io/conda/vn/conda-forge/eomaps.svg)]
 (https://anaconda.org/conda-forge/eomaps)       [![Documentation Status](https:
 //readthedocs.org/projects/eomaps/badge/?version=latest)](https://
 eomaps.readthedocs.io/en/latest/?badge=latest)       [Buy_Me_A_Coffee] [chat_on
 gitter] [DOI:_10.5281/zenodo.6459598] ---- # EOmaps - Interactive maps in
-python! EOmaps is a python package to visualize and analyze geographical
+python! **EOmaps** is a python package to visualize and analyze geographical
 datasets. It is built on top of [matplotlib](matplotlib.org/) and [cartopy]
-(https://scitools.org.uk/cartopy/docs/latest/) and aims to provide an intuitive
-and easy-to-use interface to speed up and simplify the creation and comparison
-of maps. - Visualize small datasets as well as millions of datapoints - Handle
-1D and 2D datasets with the same interface and create plots from NetCDF,
-GeoTIFF or CSV files - Take care of re-projecting the data - Compare, combine
-or (transparently) overlay multiple plot-layers - Turn the maps into
-interactive data-analysis widgets with a few lines of code - Provide a
-versatile set of tools to customize the maps (Features, WebMaps, Markers,
-Annotations etc.) - Simplify the process of composing multiple maps (and other
-plots/images) in a single figure - Export high resolution images (png, jpeg
-etc.) ## ð¨ Installation To install EOmaps (and all its dependencies) via the
-[conda](https://docs.conda.io/projects/conda/en/stable/) package-manager,
-simply use: ```python conda install -c conda-forge eomaps ``` ... to get a
-**huge_speedup**, use [mamba](https://mamba.readthedocs.io/en/latest/) to solve
-the dependencies! ```python conda install -c conda-forge mamba mamba install -
-c conda-forge eomaps ``` Need more information? - Have a look at the
-[ðInstallation](https://eomaps.readthedocs.io/en/latest/
-general.html#installation) instructions in the docs. - Checkout the quickstart
-guide [ð From 0 to EOmaps](https://eomaps.readthedocs.io/en/latest/
-FAQ.html#from-0-to-eomaps-a-quickstart-guide). ## ð Documentation Make sure
-to have a look at the ð³_Documentation_ð³ which provides a lot of
-ðExamples on how to create awesome interactive maps (incl. ð source
-code)! ## âï¸ Citation Did EOmaps help in your research? Support the
-development and add a citation to your publication! [![https://doi.org/10.5281/
-zenodo.6459598](https://zenodo.org/badge/410829039.svg)](https://zenodo.org/
-badge/latestdoi/410829039) ## ð Contribute Found a bug or got an idea for an
-interesting feature? Open an [issue](https://github.com/raphaelquast/EOmaps/
-issues) or start a [discussion](https://github.com/raphaelquast/EOmaps/
-discussions), and I'll see what I can do! Interested in actively contributing
-to the library? Awesome! - Any contributions are welcome! - New features (or
-ideas for new features) - Enhancements for existing features - Bug-fixes, code-
-style improvements, unittests etc. - Documentation updates - Outreach (e.g.
-blog-posts, tutorials, talks ... ) - Have a look at existing [Issues](https://
-github.com/raphaelquast/EOmaps/contribute) or this [ð overview project]
-(https://github.com/users/raphaelquast/projects/5/views/8) to see where EOmaps
-could use your help. - Get in touch by opening a discussion in the [ð
-Contribution](https://github.com/raphaelquast/EOmaps/discussions/categories/
-contribution) section! ---------------
+(https://scitools.org.uk/cartopy/docs/latest/) and provides an intuitive and
+easy-to-use interface to speed up and simplify the creation and comparison of
+maps. ### What can EOmaps do for you? - Create [â¤ multi-layered maps](https:/
+/eomaps.readthedocs.io/en/dev/api.html#basics) and interactively compare
+different layers with each other - [ð´ Visualize datasets](https://
+eomaps.readthedocs.io/en/dev/api.html#data-visualization) with millions of
+datapoints and handle reprojections - Provide a comprehensive set of tools to
+customize the map - [ðµNaturalEarth features](https://eomaps.readthedocs.io/
+en/dev/api.html#naturalearth-features) - [ðScalebars](https://
+eomaps.readthedocs.io/en/dev/api.html#scalebars) - [â¦ Gridlines](https://
+eomaps.readthedocs.io/en/dev/api.html#gridlines) - [ð° WebMap layers](https:/
+/eomaps.readthedocs.io/en/dev/api.html#webmap-layers) - [ð Annotations,
+Markers, Lines, Logos...](https://eomaps.readthedocs.io/en/latest/
+api.html#annotations-markers-lines-logos-etc) - . . . - Use [ð¸ Callbacks]
+(https://eomaps.readthedocs.io/en/latest/api.html#callbacks-make-the-map-
+interactive) and the [ð§° CompanionWidget](https://eomaps.readthedocs.io/en/
+dev/api.html#companion-widget) to interact with the figure - Interactively re-
+arrange multiple maps in a figure with the [ðï¸ LayoutEditor](https://
+eomaps.readthedocs.io/en/dev/api.html#layout-editor) - [ðº Export](https://
+eomaps.readthedocs.io/en/dev/api.html#export-the-map-as-jpeg-png-etc)
+publication ready high resolution images (png, jpeg etc.) - . . . and much
+more! Checkout the [ð Basics](https://eomaps.readthedocs.io/en/dev/
+api.html#basics) in the documentation to get started! ## ð¨ Installation To
+install EOmaps (and all its dependencies) via the [conda](https://
+docs.conda.io/projects/conda/en/stable/) package-manager, simply use: ```python
+conda install -c conda-forge eomaps ``` ... to get a **huge_speedup**, use
+[mamba](https://mamba.readthedocs.io/en/latest/) to solve the dependencies!
+```python conda install -c conda-forge mamba mamba install -c conda-forge
+eomaps ``` Need more information? - Have a look at the [ðInstallation]
+(https://eomaps.readthedocs.io/en/latest/general.html#installation)
+instructions in the docs. - Checkout the quickstart guide [ð From 0 to
+EOmaps](https://eomaps.readthedocs.io/en/latest/FAQ.html#from-0-to-eomaps-a-
+quickstart-guide). ## ð Documentation Make sure to have a look at the ð
+Documentation which provides a lot of ðExamples on how to create awesome
+interactive maps (incl. ð source code)! ## âï¸ Citation Did EOmaps help
+in your research? Support the development and add a citation to your
+publication! [![https://doi.org/10.5281/zenodo.6459598](https://zenodo.org/
+badge/410829039.svg)](https://zenodo.org/badge/latestdoi/410829039) ## ð
+Contribute Found a bug or got an idea for an interesting feature? Open an
+[issue](https://github.com/raphaelquast/EOmaps/issues) or start a [discussion]
+(https://github.com/raphaelquast/EOmaps/discussions), and I'll see what I can
+do! Interested in actively contributing to the library? Awesome! - Any
+contributions are welcome! - New features (or ideas for new features) -
+Enhancements for existing features - Bug-fixes, code-style improvements,
+unittests etc. - Documentation updates - Outreach (e.g. blog-posts, tutorials,
+talks ... ) - Have a look at existing [Issues](https://github.com/raphaelquast/
+EOmaps/contribute) or this [ð overview project](https://github.com/users/
+raphaelquast/projects/5/views/8) to see where EOmaps could use your help. - Get
+in touch by opening a discussion in the [ð Contribution](https://github.com/
+raphaelquast/EOmaps/discussions/categories/contribution) section! -------------
+--
 [EOmaps example 6]  [EOmaps example 2]
 [EOmaps example 9]  [EOmaps example 4]
 [EOmaps example 7]  [EOmaps example 8]
 [EOmaps inset-maps] [EOmaps example 3]
 [EOmaps example 9]  [EOmaps example 4]
 ## ð³ Basic usage **Checkout the [ð Basics](https://eomaps.readthedocs.io/
 en/latest/api.html)** in the documentation! ```python from eomaps import Maps
```

### Comparing `EOmaps-6.4.1/eomaps/NE_features.json` & `EOmaps-6.5/eomaps/NE_features.json`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4.1/eomaps/__init__.py` & `EOmaps-6.5/eomaps/__init__.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4.1/eomaps/_cb_container.py` & `EOmaps-6.5/eomaps/_cb_container.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4.1/eomaps/_containers.py` & `EOmaps-6.5/eomaps/_containers.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4.1/eomaps/_data_manager.py` & `EOmaps-6.5/eomaps/_data_manager.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4.1/eomaps/_shapes.py` & `EOmaps-6.5/eomaps/_shapes.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4.1/eomaps/_webmap.py` & `EOmaps-6.5/eomaps/_webmap.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4.1/eomaps/_webmap_containers.py` & `EOmaps-6.5/eomaps/_webmap_containers.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4.1/eomaps/callbacks.py` & `EOmaps-6.5/eomaps/callbacks.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,18 +128,16 @@
                 paramname = "val"
             printstr += f"{paramname} = {self._fmt(val)}"
         else:
             lon, lat = self.m._transf_plot_to_lonlat.transform(*pos)
 
             printstr = (
                 "---------------\n"
-                f"x = {self._fmt(pos[0], **kwargs)}\n"
-                f"y = {self._fmt(pos[1], **kwargs)}\n"
-                f"lon = {self._fmt(lon, **kwargs)}\n"
-                f"lat = {self._fmt(lat, **kwargs)}"
+                f"xy = ({self._fmt(pos[0], **kwargs)}, {self._fmt(pos[1], **kwargs)})\n"
+                f"lonlat = ({self._fmt(lon, **kwargs)}, {self._fmt(lat, **kwargs)})\n"
             )
 
         print(printstr)
 
     def annotate(
         self,
         pos_precision=4,
```

### Comparing `EOmaps-6.4.1/eomaps/colorbar.py` & `EOmaps-6.5/eomaps/colorbar.py`

 * *Files 3% similar despite different names*

```diff
@@ -218,25 +218,27 @@
               min/max bins of the histogram)
 
             The default is "clip"
         hist_kwargs : dict
             A dictionary with keyword-arguments passed to the creation of the histogram
             (e.g. passed to `plt.hist()` )
         label : str, optional
-            The label used for the colorbar. The default is None
+            The label used for the colorbar.
+            Use `ColorBar.set_labels()` to set the labels (and styling) for the
+            colorbar and the histogram.
+            The default is None.
         ylabel : str, optional
             The label used for the y-axis of the colorbar. The default is None
         kwargs :
             All additional kwargs are passed to the creation of the colorbar
             (e.g. `plt.colorbar()`)
 
         See Also
         --------
-
-        - label_bin_center
+        set_bin_labels:  Use custom names for classified colorbar bins.
 
         Examples
         --------
 
         >>> x = y = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
         >>> data = [1, 2, 6, 6, 6, 8, 7, 3, 9, 10]
         >>> m = Maps()
@@ -252,14 +254,15 @@
         >>> m.plot_map()
         >>> m.add_colorbar(hist_bins="bins", label="some data")
 
         """
         self._m = m
         self._pos = pos
         self._margin = margin
+        self._orientation = orientation
 
         self._init_extend = extend
         self._extend_frac = extend_frac
 
         self._parent_cb = self._identify_parent_cb()
 
         if inherit_position is None:
@@ -280,16 +283,17 @@
         if hist_kwargs is None:
             self._hist_kwargs = dict()
         else:
             self._hist_kwargs = copy.deepcopy(hist_kwargs)
 
         self._histogram_plotted = False  # indicator if histogram has been plotted
 
-        self._orientation = orientation
         self._dynamic_shade_indicator = dynamic_shade_indicator
+        self._hist_label_kwargs = None
+
         self._show_outline = show_outline
         self._tick_precision = tick_precision
         self._tick_formatter = tick_formatter
         self._log = log
         self._out_of_range_vals = out_of_range_vals
 
         kwargs["label"] = label
@@ -317,15 +321,15 @@
         self._setup_axes()
 
         if ylabel is not None:
             self.ax_cb_plot.set_ylabel(ylabel)
 
     def set_visible(self, vis):
         """
-        Set the visibility of the colorbar
+        Set the visibility of the colorbar.
 
         Parameters
         ----------
         vis : bool
             - True: colorbar visible
             - False: colorbar not visible
         """
@@ -335,14 +339,76 @@
             ax.set_visible(vis)
 
         if self._hist_size <= 0.0001:
             self.ax_cb_plot.set_visible(False)
         else:
             self.ax_cb_plot.set_visible(vis)
 
+    def _set_labels(self, cb_label=None, hist_label=None, **kwargs):
+        if self._dynamic_shade_indicator and hist_label is not None:
+            # remember kwargs to re-draw the histogram
+            self._hist_label_kwargs = {
+                "cb_label": None,
+                "hist_label": hist_label,
+                **kwargs,
+            }
+
+        if self._orientation == "horizontal":
+            if cb_label:
+                self._cb_label = self.ax_cb.set_xlabel(cb_label, **kwargs)
+            if hist_label:
+                self._hist_label = self.ax_cb_plot.set_ylabel(hist_label, **kwargs)
+        else:
+            if cb_label:
+                self._cb_label = self.ax_cb.set_ylabel(cb_label, **kwargs)
+            if hist_label:
+                self._hist_label = self.ax_cb_plot.set_xlabel(hist_label, **kwargs)
+
+    def set_labels(self, cb_label=None, hist_label=None, **kwargs):
+        """
+        Set the labels (and the styling) for the colorbar (and the histogram).
+
+        For more details, see `ColorBar.ax_cb.set_xlabel(..)` and matplotlib's `.Text`
+        properties.
+
+        Parameters
+        ----------
+        cb_label : str or None
+            The label of the colorbar. If None, the existing label is maintained.
+            The default is None.
+        hist_label : str or None
+            The label of the histogram. If None, the existing label is maintained.
+            The default is None.
+
+        Other Parameters
+        ----------------
+        kwargs :
+           Additional kwargs passed to `Axes.set_xlabel` to control the appearance of
+           the label (e.g. color, fontsize, labelpad etc.).
+
+        Examples
+        --------
+        Set both colorbar and histogram label in one go
+
+        >>> cb.set_labels("The parameter", "histogram count", fontsize=10, color="r")
+
+        Use different styles for the colorbar and histogram labels
+
+        >>> cb.set_labels(cb_label="The parameter", color="r", labelpad=10)
+        >>> cb.set_labels(hist_label="histogram count", fontsize=6, color="k")
+
+        """
+        self._set_labels(cb_label=cb_label, hist_label=hist_label, **kwargs)
+
+        if not self._dynamic_shade_indicator:
+            # no need to redraw the background for dynamically updated artists
+            self._m.redraw(self._m.layer)
+        else:
+            self._m.BM.update()
+
     def _default_cb_tick_formatter(self, x, pos, precision=None):
         """
         A formatter to format the tick-labels of the colorbar for encoded datasets.
         (used in xaxis.set_major_formatter() )
         """
         # if precision=None the shortest representation of the number is used
         return np.format_float_positional(self._m._decode_values(x), precision)
@@ -443,16 +509,18 @@
             # that already has a colorbar assigned
             for m in [self._m.parent, *self._m.parent._children]:
                 if m is not self._m and m.ax is self._m.ax:
                     if m.colorbar is not None:
                         if m.colorbar._parent_cb is None:
                             parent_cb = m.colorbar
                             break
-
-        return parent_cb
+        if parent_cb and parent_cb._orientation == self._orientation:
+            return parent_cb
+        else:
+            return None
 
     def _get_parent_cb(self):
         if self._parent_cb is None:
             return self
         else:
             parent = self
             while parent._parent_cb is not None:
@@ -821,17 +889,15 @@
             **self._kwargs,
         )
 
         self.cb.outline.set_visible(False)
 
         # ensure that ticklabels are correct if a classification is used
         if self._classified and "ticks" not in self._kwargs:
-            self.cb.set_ticks(
-                [i for i in self._bins if i >= self._vmin and i <= self._vmax]
-            )
+            self.cb.set_ticks(np.unique(np.clip(self._bins, self._vmin, self._vmax)))
 
             if self._tick_formatter is None:
                 self._tick_formatter = self._classified_cb_tick_formatter
         else:
             self.cb.set_ticks(self.cb.get_ticks())
 
         if self._tick_formatter is None:
@@ -1015,14 +1081,17 @@
         if self._m.layer not in self._m.BM.bg_layer.split("|"):
             return
 
         self._set_data()
         self.ax_cb_plot.clear()
         self._plot_histogram()
 
+        if self._hist_label_kwargs:
+            self._set_labels(**self._hist_label_kwargs)
+
     def set_bin_labels(self, bins, names, tick_lines="center", show_values=False):
         """
         Set the tick-labels of the colorbar to custom names with respect to a given
         set of bins.
 
         The labels will be placed at the center of each bin.
 
@@ -1143,30 +1212,40 @@
 
             else:
                 self.ax_cb.yaxis.set_minor_formatter(minor_tick_formatter)
                 self.ax_cb_plot.xaxis.set_minor_formatter(minor_tick_formatter)
                 self.ax_cb.tick_params(
                     labelright=True, which="minor", labelsize="xx-small"
                 )
+
         else:
             if horizontal:
                 self.ax_cb.tick_params(
                     labelbottom=False,
                     which="minor",
                 )
 
             else:
                 self.ax_cb.tick_params(
                     labelright=False,
                     which="minor",
                 )
 
-        self.ax_cb_plot.tick_params(
-            right=False, bottom=False, labelright=False, labelbottom=False, which="both"
-        )
+        if horizontal:
+            self.ax_cb_plot.tick_params(
+                right=False,
+                bottom=False,
+                labelright=False,
+                labelbottom=False,
+                which="both",
+            )
+        else:
+            self.ax_cb_plot.tick_params(
+                left=False, top=False, labelleft=False, labeltop=False, which="both"
+            )
 
         self._m.BM._refetch_layer(self._m.layer)
 
     def remove(self):
         """
         Remove the colorbar from the map.
         """
@@ -1199,14 +1278,15 @@
             self.ax_cb.tick_params(**kwargs)
         elif what == "histogram":
             self.ax_cb_plot.tick_params(**kwargs)
 
         self._m.redraw(self._m.layer)
 
     tick_params.__doc__ = (
+        "Set the appearance of the colorbar (or histogram) ticks.\n\n"
         "NOTE\n"
         "----\n"
         "This is a wrapper for `m.colorbar.ax_cb.tick_params` or "
         "`m.colorbar.ax_cb_plot.tick_params` to set the appearance of the ticks for "
         "the colorbar or the histogram."
         "You can select what you want to edit with the additional parameter:"
         "\n\n"
```

### Comparing `EOmaps-6.4.1/eomaps/compass.py` & `EOmaps-6.5/eomaps/compass.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,17 @@
         self._m = m
 
         self._scale = 10
         self._style = "north arrow"
         self._patch = False
         self._txt = "N"
 
+        self._last_patch_ec = None
+        self._last_patch_lw = None
+
     def __call__(
         self,
         pos=None,
         pos_transform="axes",
         scale=10,
         style="compass",
         patch=None,
@@ -63,16 +66,16 @@
         style : str, optional
 
             - "north arrow" : draw only a north-arrow
             - "compass": draw a compass with arrows in all 4 directions
 
             The default is "compass".
         patch : False, str or tuple, optional
-            The color of the background-patch.
-            (can be any color specification supported by matplotlib)
+            The color of the background-patch (can be any color specification supported
+            by matplotlib). See `Compass.set_patch(...)` for more styling options.
             The default is "w".
         txt : str, optional
             Indicator which directions should be indicated.
             - "NESW" : add letters for all 4 directions
             - "NE" : add only letters for North and East (same for other combinations)
             - None : don't add any letters
             The default is "N".
@@ -149,14 +152,16 @@
             self._canvas.mpl_connect("button_release_event", self._on_release),
             self._canvas.mpl_connect("scroll_event", self._on_scroll),
         ]
 
         if self._update_offset not in self._m.BM._before_fetch_bg_actions:
             self._m.BM._before_fetch_bg_actions.append(self._update_offset)
 
+        self._m.BM.update()
+
     def _get_artist(self, pos):
         if self._style == "north arrow":
             bg_patch = PolyCollection(
                 [[[-1.5, -0.5], [-1.5, 5], [1.5, 5], [1.5, -0.5]]],
                 facecolors=[self._patch] if self._patch else ["none"],
                 edgecolors=["k"] if self._patch else ["none"],
             )
@@ -315,26 +320,34 @@
     def _on_scroll(self, event):
         if not self._layer_visible:
             return
 
         if self._check_still_parented() and self._got_artist:
             self.set_scale(max(1, self._scale + event.step))
 
+            self._m.BM.update(artists=[self._artist])
+
     def _on_pick(self, evt):
         if not self._layer_visible:
             return
 
         if evt.mouseevent.button != 1:
             return
 
         if self._check_still_parented() and evt.artist == self._artist:
             self._got_artist = True
             self._c1 = self._canvas.mpl_connect("motion_notify_event", self._on_motion)
             self._c2 = self._canvas.mpl_connect("key_press_event", self._on_keypress)
 
+            # make red 1pt edgecolor while compass is picked
+            self._last_patch_ec = self._artist.get_children()[0].get_edgecolor()
+            self._last_patch_lw = self._artist.get_children()[0].get_linewidth()[0]
+
+            self.set_patch(edgecolor="r", linewidth=1)
+
     def _on_keypress(self, event):
         if not self._layer_visible:
             return
 
         if event.key == "delete":
             self.remove()
         if event.key == "d":
@@ -357,14 +370,20 @@
 
             try:
                 c2 = self._c2
             except AttributeError:
                 pass
             else:
                 self._canvas.mpl_disconnect(c2)
+
+            self.set_patch(
+                edgecolor=self._last_patch_ec,
+                linewidth=self._last_patch_lw,
+            )
+
             self._m.BM.update()
 
     def _check_still_parented(self):
         if self._artist.figure is None:
             self._disconnect()
             return False
         else:
```

### Comparing `EOmaps-6.4.1/eomaps/draw.py` & `EOmaps-6.5/eomaps/draw.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4.1/eomaps/eomaps.py` & `EOmaps-6.5/eomaps/eomaps.py`

 * *Files 1% similar despite different names*

```diff
@@ -815,14 +815,15 @@
         plot_size=0.5,
         inset_crs=4326,
         layer=None,
         boundary=True,
         background_color="w",
         shape="ellipses",
         indicate_extent=True,
+        indicator_line=False,
     ):
         """
         Create a new (empty) inset-map that shows a zoomed-in view on a given extent.
 
         The returned Maps-object can then be used to populate the inset-map with
         features, datasets etc.
 
@@ -871,18 +872,20 @@
         inset_crs : any, optional
             The crs that is used in the inset-map.
             The default is 4326.
         layer : str or None, optional
             The layer associated with the inset-map.
             If None (the default), the layer of the Maps-object used to create
             the inset-map is used.
-        boundary: bool or dict, optional
+        boundary: bool, str or dict, optional
             - If True: indicate the boundary of the inset-map with default colors
               (e.g.: {"ec":"r", "lw":2})
             - If False: don't add edgecolors to the boundary of the inset-map
+            - If a string is provided, it is identified as the edge-color of the
+              boundary (e.g. any named matplotlib color like "r", "g", "darkblue"...)
             - if dict: use the provided values for "ec" (e.g. edgecolor) and
               "lw" (e.g. linewidth)
 
             The default is True.
         background_color: str, tuple or None
             The background color to use.
 
@@ -899,23 +902,35 @@
             - If True: add a polygon representing the inset-extent to the parent map.
             - If a dict is provided, it will be used to update the appearance of the
               added polygon (e.g. facecolor, edgecolor, linewidth etc.)
 
             NOTE: you can also use `m_inset.indicate_inset_extent(...)` to manually
             indicate the inset-shape on arbitrary Maps-objects.
 
+            The default is True.
+        indicator_line : bool or dict, optional
+
+            - If True: add a line that connects the inset-map to the indicated extent
+              on the parent map
+            - If a dict is provided, it is used to update the appearance of the line
+              (e.g. c="r", lw=2, ...)
+
+            NOTE: you can also use `m_inset.add_indicator_line(...)` to manually
+            indicate the inset-shape on arbitrary Maps-objects.
+
+            The default is False.
         Returns
         -------
         m : eomaps.Maps
             A eomaps.Maps-object of the inset-map.
             (use it just like any other Maps-object)
 
         See Also
         --------
-        The following additional methods are defined on `_InsetMaps` objects
+        The following additional methods are defined on `InsetMaps` objects
 
         m.indicate_inset_extent :
             Plot a polygon representing the extent of the inset map on another Maps
             object.
         m.set_inset_position :
             Set the (center) position and size of the inset-map.
 
@@ -964,28 +979,29 @@
         >>> # visible if the "second" layer is visible
         >>> m3 = m2.new_layer(layer="second")
         >>> m3.add_feature.preset.coastline()
         >>> m3.add_feature.preset.land()
 
         >>> m.util.layer_selector()
         """
-        m2 = _InsetMaps(
+        m2 = InsetMaps(
             parent=self,
             crs=inset_crs,
             layer=layer,
             xy=xy,
             radius=radius,
             plot_position=plot_position,
             plot_size=plot_size,
             xy_crs=xy_crs,
             radius_crs=radius_crs,
             boundary=boundary,
             background_color=background_color,
             shape=shape,
             indicate_extent=indicate_extent,
+            indicator_line=indicator_line,
         )
 
         return m2
 
     @property
     @wraps(shapes)
     def set_shape(self):
@@ -1141,59 +1157,71 @@
         if parameter is not None:
             self.data_specs.parameter = parameter
 
     set_data = set_data_specs
 
     @property
     def set_classify(self):
-        """Accessor to set the data-classification."""
+        """
+        Interface to the classifiers provided by the 'mapclassify' module.
+
+        To set a classification scheme for a given Maps-object, simply use:
+
+        >>> m.set_classify.< SCHEME >(...)
+
+        Where `< SCHEME >` is the name of the desired classification and additional
+        parameters are passed in the call. (check docstrings for more info!)
+
+        A list of available classification-schemes is accessible via
+        `m.classify_specs.SCHEMES`
+
+            - BoxPlot (hinge)
+            - EqualInterval (k)
+            - FisherJenks (k)
+            - FisherJenksSampled (k, pct, truncate)
+            - HeadTailBreaks ()
+            - JenksCaspall (k)
+            - JenksCaspallForced (k)
+            - JenksCaspallSampled (k, pct)
+            - MaxP (k, initial)
+            - MaximumBreaks (k, mindiff)
+            - NaturalBreaks (k, initial)
+            - Quantiles (k)
+            - Percentiles (pct)
+            - StdMean (multiples)
+            - UserDefined (bins)
+
+        Examples
+        --------
+        >>> m.set_classify.Quantiles(k=5)
+
+        >>> m.set_classify.EqualInterval(k=5)
+
+        >>> m.set_classify.UserDefined(bins=[5, 10, 25, 50])
+
+        """
         assert _register_mapclassify(), (
             "EOmaps: Missing dependency: 'mapclassify' \n ... please install"
             + " (conda install -c conda-forge mapclassify) to use data-classifications."
         )
 
         s = SimpleNamespace(
             **{
                 i: self._get_mcl_subclass(getattr(mapclassify, i))
                 for i in mapclassify.CLASSIFIERS
             }
         )
 
-        s.__doc__ = dedent(
-            """
-            Interface to the classifiers provided by the 'mapclassify' module.
-
-            To set a classification scheme for a given Maps-object, simply use:
-
-            >>> m.set_classify.<SCHEME>(...)
-
-            Where `<SCHEME>` is the name of the desired classification and additional
-            parameters are passed in the call. (check docstrings for more info!)
-
-
-            Note
-            ----
-            The following calls have the same effect:
-
-            >>> m.set_classify.Quantiles(k=5)
-            >>> m.set_classify_specs(scheme="Quantiles", k=5)
-
-            Using `m.set_classify()` is the same as using `m.set_classify_specs()`!
-            However, `m.set_classify()` will provide autocompletion and proper
-            docstrings once the Maps-object is initialized which greatly enhances
-            the usability.
-
-            """
-        )
+        s.__doc__ = Maps.set_classify.__doc__
 
         return s
 
     def set_classify_specs(self, scheme=None, **kwargs):
         """
-        Set classification specifications for the data.
+        Optional way to set classification specifications for the data.
 
         The classification is ultimately performed by the `mapclassify` module!
 
         Note
         ----
         The following calls have the same effect:
 
@@ -1229,14 +1257,15 @@
                 - StdMean (multiples)
                 - UserDefined (bins)
 
         kwargs :
             kwargs passed to the call to the respective mapclassify classifier
             (dependent on the selected scheme... see above)
         """
+
         assert _register_mapclassify(), (
             "EOmaps: Missing dependency: 'mapclassify' \n ... please install"
             + " (conda install -c conda-forge mapclassify) to use data-classifications."
         )
 
         self.classify_specs._set_scheme_and_args(scheme, **kwargs)
 
@@ -2354,18 +2383,58 @@
         if crs is not None:
             crs = self._get_cartopy_crs(crs)
         else:
             crs = Maps.CRS.PlateCarree()
 
         return self.ax.get_extent(crs=crs)
 
+    def _calc_vmin_vmax(self, vmin=None, vmax=None):
+        if self._data_manager.z_data is None:
+            return vmin, vmax
+
+        calc_min, calc_max = vmin is None, vmax is None
+
+        # ignore fill_values when evaluating vmin/vmax on integer-encoded datasets
+        if (
+            self.data_specs.encoding is not None
+            and isinstance(self._data_manager.z_data, np.ndarray)
+            and issubclass(self._data_manager.z_data.dtype.type, np.integer)
+        ):
+
+            # note the specific way how to check for integer-dtype based on issubclass
+            # since isinstance() fails to identify all integer dtypes!!
+            #   isinstance(np.dtype("uint8"), np.integer)       (incorrect) False
+            #   issubclass(np.dtype("uint8").type, np.integer)  (correct)   True
+            # for details, see https://stackoverflow.com/a/934652/9703451
+
+            fill_value = self.data_specs.encoding.get("_FillValue", None)
+            if fill_value:
+                # find values that are not fill-values
+                use_vals = self._data_manager.z_data[
+                    self._data_manager.z_data != fill_value
+                ]
+
+                if calc_min:
+                    vmin = np.min(use_vals)
+                if calc_max:
+                    vmax = np.max(use_vals)
+        else:
+            # use nanmin/nanmax for all other arrays
+            if calc_min:
+                vmin = np.nanmin(self._data_manager.z_data)
+            if calc_max:
+                vmax = np.nanmax(self._data_manager.z_data)
+
+        return vmin, vmax
+
     def _set_vmin_vmax(self, vmin=None, vmax=None):
         self._vmin = self._encode_values(vmin)
         self._vmax = self._encode_values(vmax)
 
+        # handle inherited bounds
         if self._inherit_classification is not None:
             if not (vmin is None and vmax is None):
                 raise TypeError(
                     "EOmaps: 'vmin' and 'vmax' cannot be set explicitly "
                     "if the classification is inherited!"
                 )
 
@@ -2375,30 +2444,24 @@
                 print("EOmaps: Warning, inherited value for 'vmax' is None!")
 
             self._vmin = self._inherit_classification._vmin
             self._vmax = self._inherit_classification._vmax
             return
 
         if not self.shape.name.startswith("shade_"):
-            if vmin is None and self.data is not None:
-                self._vmin = np.nanmin(self._data_manager.z_data)
-            if vmax is None and self.data is not None:
-                self._vmax = np.nanmax(self._data_manager.z_data)
+            # ignore fill_values when evaluating vmin/vmax on integer-encoded datasets
+            self._vmin, self._vmax = self._calc_vmin_vmax(vmin=vmin, vmax=vmax)
         else:
             # get the name of the used aggretation reduction
             aggname = self.shape.aggregator.__class__.__name__
             if aggname in ["first", "last", "max", "min", "mean", "mode"]:
                 # set vmin/vmax in case the aggregation still represents data-values
-                if vmin is None:
-                    self._vmin = np.nanmin(self._data_manager.z_data)
-                if vmax is None:
-                    self._vmax = np.nanmax(self._data_manager.z_data)
+                self._vmin, self._vmax = self._calc_vmin_vmax(vmin=vmin, vmax=vmax)
             else:
                 # set vmin/vmax for aggregations that do NOT represent data values
-
                 # allow vmin/vmax = None (e.g. autoscaling)
                 if "count" in aggname:
                     # if the reduction represents a count, don't count empty pixels
                     if vmin and vmin <= 0:
                         print(
                             "EOmaps: setting vmin=1 to avoid counting empty pixels..."
                         )
@@ -2562,15 +2625,14 @@
         if verbose > 0 and not self._inherit_classification:
             if self.classify_specs.scheme is not None:
                 print("EOmaps: Classifying...")
 
         self._set_vmin_vmax(
             vmin=kwargs.pop("vmin", None), vmax=kwargs.pop("vmax", None)
         )
-
         cbcmap, norm, bins, classified = self._classify_data(
             vmin=self._vmin,
             vmax=self._vmax,
             cmap=cmap,
             classify_specs=self.classify_specs,
         )
 
@@ -4630,23 +4692,28 @@
         if isinstance(crs, Maps.CRS.CRS):  # already a cartopy CRS
             cartopy_proj = crs
         elif crs == 4326:
             cartopy_proj = ccrs.PlateCarree()
         elif isinstance(crs, (int, np.integer)):
             cartopy_proj = ccrs.epsg(crs)
         elif isinstance(crs, CRS):  # pyproj CRS
+            cartopy_proj = None
             for (
                 subgrid,
                 equi7crs,
             ) in Maps.CRS.Equi7Grid_projection._pyproj_crs_generator():
                 if equi7crs == crs:
                     cartopy_proj = Maps.CRS.Equi7Grid_projection(subgrid)
                     break
+            if cartopy_proj is None:
+                cartopy_proj = ccrs.CRS(crs)
+
         else:
             raise AssertionError(f"EOmaps: cannot identify the CRS for: {crs}")
+
         return cartopy_proj
 
     @staticmethod
     def _get_transformer(crs_from, crs_to):
         # create a pyproj Transformer object or return a cached version of it
         # if it has already been created.
         c_from = Maps._transformer_cache.setdefault(hash(crs_from), dict())
@@ -4738,15 +4805,15 @@
 
         @wraps(refetch_wms_on_size_change)
         def refetch_wms_on_size_change(self, *args, **kwargs):
             """Set the behavior for WebMap services on axis or figure size changes."""
             refetch_wms_on_size_change(*args, **kwargs)
 
 
-class _InsetMaps(Maps):
+class InsetMaps(Maps):
     # a subclass of Maps that includes some special functions for inset maps
 
     def __init__(
         self,
         parent,
         crs=4326,
         layer=None,
@@ -4754,23 +4821,26 @@
         xy_crs=4326,
         radius=5,
         radius_crs=None,
         plot_position=(0.5, 0.5),
         plot_size=0.5,
         shape="ellipses",
         indicate_extent=True,
+        indicator_line=False,
         boundary=True,
         background_color="w",
         **kwargs,
     ):
 
+        self._parent = self._proxy(parent)
+
         # inherit the layer from the parent Maps-object if not explicitly
         # provided
         if layer is None:
-            layer = parent.layer
+            layer = self._parent.layer
 
         # put all inset-map artists on dedicated layers
         # NOTE: all artists of inset-map axes are put on a dedicated layer
         # with a "__inset_" prefix to ensure they appear on top of other artists
         # (AND on top of spines of normal maps)!
         # layer = "__inset_" + str(layer)
 
@@ -4785,37 +4855,47 @@
                 + "used as shape! (the radius for `geod_circles` is always in meters!)"
             )
 
         if radius_crs is None:
             radius_crs = xy_crs
 
         extent_kwargs = dict(ec="r", lw=1, fc="none")
+        line_kwargs = dict(c="r", lw=2)
         boundary_kwargs = dict(ec="r", lw=2)
 
         if isinstance(boundary, dict):
             assert (
                 len(set(boundary.keys()).difference({"ec", "lw"})) == 0
             ), "EOmaps: only 'ec' and 'lw' keys are allowed for the 'boundary' dict!"
 
             boundary_kwargs.update(boundary)
             # use same edgecolor for boundary and indicator by default
             extent_kwargs["ec"] = boundary["ec"]
+            line_kwargs["c"] = boundary["ec"]
+        elif isinstance(boundary, str):
+            boundary_kwargs.update({"ec": boundary})
+            # use same edgecolor for boundary and indicator by default
+            extent_kwargs["ec"] = boundary
+            line_kwargs["c"] = boundary
 
         if isinstance(indicate_extent, dict):
             extent_kwargs.update(indicate_extent)
 
+        if isinstance(indicator_line, dict):
+            line_kwargs.update(indicator_line)
+
         x, y = xy
         plot_x, plot_y = plot_position
         left = plot_x - plot_size / 2
         bottom = plot_y - plot_size / 2
 
         # initialize a new maps-object with a new axis
         super().__init__(
             crs=crs,
-            f=parent.f,
+            f=self._parent.f,
             ax=(left, bottom, plot_size, plot_size),
             layer=layer,
             **kwargs,
         )
 
         # get the boundary of a ellipse in the inset_crs
         bnd, bnd_verts = self._get_inset_boundary(
@@ -4840,17 +4920,21 @@
 
         self._inset_props = dict(
             xy=xy, xy_crs=xy_crs, radius=radius, radius_crs=radius_crs, shape=shape
         )
 
         if indicate_extent is not False:
             self.indicate_inset_extent(
-                parent, layer=parent.layer, permanent=True, **extent_kwargs
+                self._parent, layer=self._parent.layer, permanent=True, **extent_kwargs
             )
 
+        self._indicator_lines = []
+        if indicator_line is not False:
+            self.add_indicator_line(**line_kwargs)
+
         # add a background patch to the "all" layer
         if background_color is not None:
             self._bg_patch = self._add_background_patch(
                 color=background_color, layer="all"
             )
         else:
             self._bg_patch = None
@@ -4913,14 +4997,87 @@
             xy_crs=self._inset_props["xy_crs"],
             radius=self._inset_props["radius"],
             radius_crs=self._inset_props["radius_crs"],
             n=n,
             **kwargs,
         )
 
+    def add_indicator_line(self, m=None, **kwargs):
+        """
+        Add a line that connects the inset-map to the inset location on a given map.
+
+        The line connects the current inset-map (center) position to the center of the
+        inset extent on the provided Maps-object.
+
+        It is possible to add multiple indicator-lines for different maps!
+
+        The lines will be automatically updated if axes sizes or positions change.
+
+        Parameters
+        ----------
+        m : eomaps.Maps or None
+            The Maps object for which the inset-line should be added.
+            If None, the parent Maps-object that was used to create the inset-map
+            is used. The default is None.
+
+        kwargs :
+            Additional kwargs are passed to plt.Line2D to style the appearance of the
+            line (e.g. "c", "ls", "lw", ...)
+
+
+        Examples
+        --------
+
+        """
+        if m is None:
+            m = self._parent
+
+        kwargs.setdefault("c", "r")
+        kwargs.setdefault("lw", 2)
+        kwargs.setdefault("zorder", -np.inf)
+
+        l = plt.Line2D([0, 0], [1, 1], **kwargs)
+        l = self.f.add_artist(l)
+        self.BM.add_bg_artist(l, "__inset_all")
+        self._indicator_lines.append((l, m))
+
+        if isinstance(m, InsetMaps):
+            # in order to make the line visible on top of another inset-map
+            # but NOT on the inset-map whose extent is indicated, the line has to
+            # be drawn on the inset-map explicitly.
+
+            # This is because all artists on inset-map axes are always on top of other
+            # (normal map) artists... (and so the line would be behind the background)
+
+            kwargs["zorder"] = np.inf
+            l2 = plt.Line2D([0, 0], [1, 1], **kwargs, transform=m.f.transFigure)
+            l2 = m.ax.add_artist(l2)
+            self.BM.add_bg_artist(l2, "__inset_all")
+            self._indicator_lines.append((l2, m))
+
+        self._update_indicator_lines()
+        self.BM._before_fetch_bg_actions.append(self._update_indicator_lines)
+
+    def _update_indicator_lines(self, *args, **kwargs):
+        props = self._inset_props
+        bbox = self.ax.get_position()
+        # get current inset-map position
+        x1 = (bbox.x1 + bbox.x0) / 2
+        y1 = (bbox.y1 + bbox.y0) / 2
+
+        for l, m in self._indicator_lines:
+            # get inset map extent in ax projection
+            t = m._get_transformer(props["xy_crs"], m.ax.projection)
+            xy = t.transform(*props["xy"])
+            # get inset map extent in figure coordinates
+            x0, y0 = (m.ax.transData + m.f.transFigure.inverted()).transform(xy)
+
+            l.set_xdata([x0, x1])
+            l.set_ydata([y0, y1])
+
     # a convenience-method to set the position based on the center of the axis
     def set_inset_position(self, x=None, y=None, size=None):
         """
         Set the (center) position and size of the inset-map.
 
         Parameters
         ----------
@@ -4983,14 +5140,17 @@
                 crs=xy_crs,
                 radius=radius,
                 radius_crs=radius_crs,
                 n=n,
             )
             bnd_verts = np.stack(shp_pts[:2], axis=2)[0]
 
+            # make sure vertices are right-handed
+            bnd_verts = bnd_verts[::-1]
+
         elif shape == "rectangles":
             shp_pts = shp._get_rectangle_verts(
                 x=np.atleast_1d(x),
                 y=np.atleast_1d(y),
                 crs=xy_crs,
                 radius=radius,
                 radius_crs=radius_crs,
@@ -5004,10 +5164,13 @@
                 y=np.atleast_1d(y),
                 crs=xy_crs,
                 radius=radius,
                 # radius_crs=radius_crs,
                 n=n,
             )
             bnd_verts = np.stack(shp_pts[:2], axis=2).squeeze()
+            # make sure vertices are right-handed
+            bnd_verts = bnd_verts[::-1]
+
         boundary = mpl.path.Path(bnd_verts)
 
         return boundary, bnd_verts
```

### Comparing `EOmaps-6.4.1/eomaps/helpers.py` & `EOmaps-6.5/eomaps/helpers.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4.1/eomaps/logo.png` & `EOmaps-6.5/eomaps/logo.png`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4.1/eomaps/mapsgrid.py` & `EOmaps-6.5/eomaps/mapsgrid.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4.1/eomaps/ne_features.py` & `EOmaps-6.5/eomaps/ne_features.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,25 +201,31 @@
                 The default is "auto"
             """
 
             self.__doc__ = combdoc(
                 f"PRESET using {kwargs} \n", self.feature.__doc__, add_params
             )
 
+        def _handle_synonyms(self, kwargs):
+            # make sure to replace shortcuts with long names
+            # (since "facecolor=..." will override "fc=..." if both are specified)
+            subst = dict(fc="facecolor", ec="edgecolor", lw="linewidth", ls="linestyle")
+            return {subst.get(key, key): val for key, val in kwargs.items()}
+
         def __call__(self, scale=50, **kwargs):
             k = dict(**self.kwargs)
             k.update(kwargs)
 
             if scale != "auto":
                 self.feature = self._m.add_feature._get_feature(
                     category=self.category, name=self.name
                 )
 
             self.__doc__ = self.feature.__doc__
-            return self.feature(scale=scale, **k)
+            return self.feature(scale=scale, **self._handle_synonyms(k))
 
 
 _NE_features_path = Path(__file__).parent / "NE_features.json"
 
 try:
     with open(_NE_features_path, "r") as file:
         _NE_features = json.load(file)
```

### Comparing `EOmaps-6.4.1/eomaps/projections.py` & `EOmaps-6.5/eomaps/projections.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4.1/eomaps/qtcompanion/app.py` & `EOmaps-6.5/eomaps/qtcompanion/app.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4.1/eomaps/qtcompanion/base.py` & `EOmaps-6.5/eomaps/qtcompanion/base.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4.1/eomaps/qtcompanion/icons/eye_closed.png` & `EOmaps-6.5/eomaps/qtcompanion/icons/eye_closed.png`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4.1/eomaps/qtcompanion/icons/eye_open.png` & `EOmaps-6.5/eomaps/qtcompanion/icons/eye_open.png`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4.1/eomaps/qtcompanion/icons/logo.png` & `EOmaps-6.5/eomaps/qtcompanion/icons/logo.png`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4.1/eomaps/qtcompanion/icons/peek_circle.png` & `EOmaps-6.5/eomaps/qtcompanion/icons/peek_circle.png`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4.1/eomaps/qtcompanion/icons/peek_circle_active.png` & `EOmaps-6.5/eomaps/qtcompanion/icons/peek_circle_active.png`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4.1/eomaps/qtcompanion/icons/peek_ellipse.png` & `EOmaps-6.5/eomaps/qtcompanion/icons/peek_ellipse.png`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4.1/eomaps/qtcompanion/icons/peek_ellipse_active.png` & `EOmaps-6.5/eomaps/qtcompanion/icons/peek_ellipse_active.png`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4.1/eomaps/qtcompanion/widgets/annotate.py` & `EOmaps-6.5/eomaps/qtcompanion/widgets/annotate.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4.1/eomaps/qtcompanion/widgets/click_callbacks.py` & `EOmaps-6.5/eomaps/qtcompanion/widgets/click_callbacks.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4.1/eomaps/qtcompanion/widgets/draw.py` & `EOmaps-6.5/eomaps/qtcompanion/widgets/draw.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4.1/eomaps/qtcompanion/widgets/editor.py` & `EOmaps-6.5/eomaps/qtcompanion/widgets/editor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from PyQt5 import QtCore, QtWidgets, QtGui
 from PyQt5.QtCore import Qt, pyqtSignal, pyqtSlot, QSize
 
 from matplotlib.colors import to_rgba_array
 
-from ...eomaps import _InsetMaps
+from ...eomaps import InsetMaps
 from ..common import iconpath
 from .wms import AddWMSMenuButton
 from .utils import GetColorWidget, AlphaSlider
 from .annotate import AddAnnotationInput
 from .draw import DrawerTabs
 
 
@@ -1169,15 +1169,15 @@
             return
 
         if layer is None:
             layer = self.tabText(self.currentIndex())
 
         # make sure we fetch artists of inset-maps from the layer with
         # the "__inset_" prefix
-        if isinstance(self.m, _InsetMaps) and not layer.startswith("__inset_"):
+        if isinstance(self.m, InsetMaps) and not layer.startswith("__inset_"):
             layer = "__inset_" + layer
         widget = self.currentWidget()
 
         if widget is None:
             # ignore events without tabs (they happen on re-population of the tabs)
             return
```

### Comparing `EOmaps-6.4.1/eomaps/qtcompanion/widgets/extent.py` & `EOmaps-6.5/eomaps/qtcompanion/widgets/extent.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4.1/eomaps/qtcompanion/widgets/files.py` & `EOmaps-6.5/eomaps/qtcompanion/widgets/files.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4.1/eomaps/qtcompanion/widgets/layer.py` & `EOmaps-6.5/eomaps/qtcompanion/widgets/layer.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4.1/eomaps/qtcompanion/widgets/peek.py` & `EOmaps-6.5/eomaps/qtcompanion/widgets/peek.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4.1/eomaps/qtcompanion/widgets/save.py` & `EOmaps-6.5/eomaps/qtcompanion/widgets/save.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4.1/eomaps/qtcompanion/widgets/utils.py` & `EOmaps-6.5/eomaps/qtcompanion/widgets/utils.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4.1/eomaps/qtcompanion/widgets/wms.py` & `EOmaps-6.5/eomaps/qtcompanion/widgets/wms.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4.1/eomaps/reader.py` & `EOmaps-6.5/eomaps/reader.py`

 * *Files 7% similar despite different names*

```diff
@@ -115,14 +115,15 @@
         path_or_dataset,
         crs_key=None,
         data_crs=None,
         sel=None,
         isel=None,
         set_data=None,
         mask_and_scale=False,
+        fill_values="mask",
     ):
         """
         Read all relevant information necessary to add a GeoTIFF to the map.
 
         Parameters
         ----------
         path_or_dataset : str, pathlib.Path or xar.Dataset
@@ -165,14 +166,37 @@
 
             NOTE: using `mask_and_scale=True` results in a conversion of the data-values
             to floats!! For very large datasets this can cause a huge increase in
             memory-usage! EOmaps handles the scaling internally to show correct
             values for callbacks and colorbars, even if `mask_and_scale=False`!
 
             The default is False.
+        fill_values : str ("mask", "keep")
+            Indicator how to treat fill-values to avoid performance issues for
+            extremely large (integer encoded) datasets.
+
+            Only relevant for integer-encoded data if "mask_and_scale" is False
+            and a "_FillValue" is provided in the metadata.
+
+            - If "mask", a "numpy.masked_array" is used to incorporate fill-value
+              masking while maintaining integer dtype. NOTE that this can lead to
+              performance issues for very large datasets due to the increased memory
+              usage (and reduced performance) of masked_arrays.
+            - If "keep", no masking with respect to fill-values is performed and a
+              normal "numpy.array" is returned that still contains fill_values.
+
+              The fill-value is accessible via `m.data_specs.encoding["_FillValue"]`
+
+              To adjust the color of fill_values in the plot without explicit masking,
+              set the "over" and "unuder" colors of the used colorbar:
+
+               - `plt.cm.viridis.with_extremes(over=... under=...)`
+               - `cmap.set_over(...)`, `cmap.set_under(...)`)
+
+              (fill-values are excluded when evaluating data-limits)
 
         Returns
         -------
         dict (if set_data is False) or None (if set_data is True)
             A dict that contains the data required for plotting.
 
         Examples
@@ -271,16 +295,24 @@
 
             # only use masked arrays if mask_and_scale is False!
             # (otherwise the mask is already applied as NaN's in the float-array)
             # Using masked-arrays ensures that we can deal with integers as well!
             if mask_and_scale is False:
                 encoding = usencfile.attrs
                 fill_value = encoding.get("_FillValue", None)
-                if fill_value:
-                    data = np.ma.masked_where(data == fill_value, data, copy=False)
+
+                if fill_value and fill_values == "mask":
+                    data = np.ma.MaskedArray(
+                        data=data,
+                        mask=data == fill_value,
+                        copy=False,
+                        fill_value=fill_value,
+                        hard_mask=True,
+                    )
+
             else:
                 encoding = None
 
             if set_data is not None:
                 set_data.set_data(
                     data=data,
                     x=x,
@@ -307,14 +339,15 @@
         coords=None,
         crs_key=None,
         data_crs=None,
         sel=None,
         isel=None,
         set_data=None,
         mask_and_scale=False,
+        fill_values="mask",
     ):
         """
         Read all relevant information necessary to add a NetCDF to the map.
 
         Parameters
         ----------
         path_or_dataset : str, pathlib.Path or xar.Dataset
@@ -366,14 +399,37 @@
 
             NOTE: using `mask_and_scale=True` results in a conversion of the data-values
             to floats!! For very large datasets this can cause a huge increase in
             memory-usage! EOmaps handles the scaling internally to show correct
             values for callbacks and colorbars, even if `mask_and_scale=False`!
 
             The default is False.
+        fill_values : str ("mask", "keep")
+            Indicator how to treat fill-values to avoid performance issues for
+            extremely large (integer encoded) datasets.
+
+            Only relevant for integer-encoded data if "mask_and_scale" is False
+            and a "_FillValue" is provided in the metadata.
+
+            - If "mask", a "numpy.masked_array" is used to incorporate fill-value
+              masking while maintaining integer dtype. NOTE that this can lead to
+              performance issues for very large datasets due to the increased memory
+              usage (and reduced performance) of masked_arrays.
+            - If "keep", no masking with respect to fill-values is performed and a
+              normal "numpy.array" is returned that still contains fill_values.
+
+              The fill-value is accessible via `m.data_specs.encoding["_FillValue"]`
+
+              To adjust the color of fill_values in the plot without explicit masking,
+              set the "over" and "unuder" colors of the used colorbar:
+
+               - `plt.cm.viridis.with_extremes(over=... under=...)`
+               - `cmap.set_over(...)`, `cmap.set_under(...)`)
+
+              (fill-values are excluded when evaluating data-limits)
 
         Returns
         -------
         dict (if set_data is False) or None (if set_data is True)
             A dict that contains the data required for plotting.
 
         Examples
@@ -510,16 +566,23 @@
             if mask_and_scale is False:
                 encoding = dict(
                     scale_factor=getattr(usencfile[parameter], "scale_factor", 1),
                     add_offset=getattr(usencfile[parameter], "add_offset", 0),
                     _FillValue=getattr(usencfile[parameter], "_FillValue", None),
                 )
                 fill_value = encoding.get("_FillValue", None)
-                if fill_value:
-                    data = np.ma.masked_where(data == fill_value, data, copy=False)
+                if fill_value and fill_values == "mask":
+                    data = np.ma.MaskedArray(
+                        data=data,
+                        mask=data == fill_value,
+                        copy=False,
+                        fill_value=fill_value,
+                        hard_mask=True,
+                    )
+
             else:
                 encoding = None
 
             if set_data is not None:
                 set_data.set_data(
                     data=data,
                     x=x.values,
@@ -792,14 +855,15 @@
         isel=None,
         plot_crs=None,
         shape=None,
         classify_specs=None,
         val_transform=None,
         coastline=False,
         mask_and_scale=False,
+        fill_values="mask",
         extent=None,
         **kwargs,
     ):
         """
         Convenience function to initialize a new Maps-object from a NetCDF file.
 
         If no explicit shape is provided, EOmaps will try several attempts to plot
@@ -891,14 +955,37 @@
 
             NOTE: using `mask_and_scale=True` results in a conversion of the data-values
             to floats!! For very large datasets this can cause a huge increase in
             memory-usage! EOmaps handles the scaling internally to show correct
             values for callbacks and colorbars, even if `mask_and_scale=False`!
 
             The default is False.
+        fill_values : str ("mask", "keep")
+            Indicator how to treat fill-values to avoid performance issues for
+            extremely large (integer encoded) datasets.
+
+            Only relevant for integer-encoded data if "mask_and_scale" is False
+            and a "_FillValue" is provided in the metadata.
+
+            - If "mask", a "numpy.masked_array" is used to incorporate fill-value
+              masking while maintaining integer dtype. NOTE that this can lead to
+              performance issues for very large datasets due to the increased memory
+              usage (and reduced performance) of masked_arrays.
+            - If "keep", no masking with respect to fill-values is performed and a
+              normal "numpy.array" is returned that still contains fill_values.
+
+              The fill-value is accessible via `m.data_specs.encoding["_FillValue"]`
+
+              To adjust the color of fill_values in the plot without explicit masking,
+              set the "over" and "unuder" colors of the used colorbar:
+
+               - `plt.cm.viridis.with_extremes(over=... under=...)`
+               - `cmap.set_over(...)`, `cmap.set_under(...)`)
+
+              (fill-values are excluded when evaluating data-limits)
         extent : tuple or string
             Set the extent of the map prior to plotting
             (can provide great speedups if only a subset of the dataset is shown!)
 
             - If a tuple is provided, it is used to set the plot-extent
               before plotting via `m.set_extent(extent)`
 
@@ -955,14 +1042,15 @@
             coords=coords,
             crs_key=data_crs_key,
             data_crs=data_crs,
             sel=sel,
             isel=isel,
             set_data=None,
             mask_and_scale=mask_and_scale,
+            fill_values=fill_values,
         )
 
         if val_transform:
             data["data"] = val_transform(data["data"])
 
         return _from_file(
             data,
@@ -984,14 +1072,15 @@
         isel=None,
         plot_crs=None,
         shape=None,
         classify_specs=None,
         val_transform=None,
         coastline=False,
         mask_and_scale=False,
+        fill_values="mask",
         extent=None,
         **kwargs,
     ):
         """
         Convenience function to initialize a new Maps-object from a GeoTIFF file.
 
         If no explicit shape is provided, EOmaps will try several attempts to plot
@@ -1071,14 +1160,37 @@
 
             NOTE: using `mask_and_scale=True` results in a conversion of the data-values
             to floats!! For very large datasets this can cause a huge increase in
             memory-usage! EOmaps handles the scaling internally to show correct
             values for callbacks and colorbars, even if `mask_and_scale=False`!
 
             The default is False.
+        fill_values : str ("mask", "keep")
+            Indicator how to treat fill-values to avoid performance issues for
+            extremely large (integer encoded) datasets.
+
+            Only relevant for integer-encoded data if "mask_and_scale" is False
+            and a "_FillValue" is provided in the metadata.
+
+            - If "mask", a "numpy.masked_array" is used to incorporate fill-value
+              masking while maintaining integer dtype. NOTE that this can lead to
+              performance issues for very large datasets due to the increased memory
+              usage (and reduced performance) of masked_arrays.
+            - If "keep", no masking with respect to fill-values is performed and a
+              normal "numpy.array" is returned that still contains fill_values.
+
+              The fill-value is accessible via `m.data_specs.encoding["_FillValue"]`
+
+              To adjust the color of fill_values in the plot without explicit masking,
+              set the "over" and "unuder" colors of the used colorbar:
+
+               - `plt.cm.viridis.with_extremes(over=... under=...)`
+               - `cmap.set_over(...)`, `cmap.set_under(...)`)
+
+              (fill-values are excluded when evaluating data-limits)
         extent : tuple or string
             Set the extent of the map prior to plotting
             (can provide great speedups if only a subset of the dataset is shown!)
 
             - If a tuple is provided, it is used to set the plot-extent
               before plotting via `m.set_extent(extent)`
 
@@ -1131,14 +1243,15 @@
             path_or_dataset,
             sel=sel,
             isel=isel,
             set_data=None,
             data_crs=data_crs,
             crs_key=data_crs_key,
             mask_and_scale=mask_and_scale,
+            fill_values=fill_values,
         )
 
         if val_transform:
             data["data"] = val_transform(data["data"])
 
         if (
             classify_specs is None
```

### Comparing `EOmaps-6.4.1/eomaps/scalebar.py` & `EOmaps-6.5/eomaps/scalebar.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.4.1/eomaps/utilities.py` & `EOmaps-6.5/eomaps/utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -561,15 +561,22 @@
         del self._m.util._sliders[self._init_args["name"]]
 
         self._m.BM.update()
 
 
 class utilities:
     """
-    A collection of utility tools that can be added to EOmaps plots
+    A collection of utility tools that can be added to EOmaps plots.
+
+    Methods
+    -------
+    layer_selector: A legend-like widget to switch between layers
+
+    layer_slider: A slider widget to switch between layers
+
     """
 
     def __init__(self, m):
         self._m = m
 
         self._selectors = dict()
         self._sliders = dict()
```

### Comparing `EOmaps-6.4.1/setup.py` & `EOmaps-6.5/setup.py`

 * *Files identical despite different names*

