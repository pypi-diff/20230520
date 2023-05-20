# Comparing `tmp/NodeGraphQt-0.6.0.tar.gz` & `tmp/NodeGraphQt-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NodeGraphQt-0.6.0.tar", last modified: Fri May 19 08:55:01 2023, max compression
+gzip compressed data, was "NodeGraphQt-0.6.1.tar", last modified: Sat May 20 11:33:44 2023, max compression
```

## Comparing `NodeGraphQt-0.6.0.tar` & `NodeGraphQt-0.6.1.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 08:55:01.458956 NodeGraphQt-0.6.0/
--rw-rw-rw-   0        0        0     1102 2021-06-18 10:54:50.000000 NodeGraphQt-0.6.0/LICENSE.md
--rw-rw-rw-   0        0        0       49 2022-05-22 21:37:50.000000 NodeGraphQt-0.6.0/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-05-19 08:55:01.186585 NodeGraphQt-0.6.0/NodeGraphQt/
--rw-rw-rw-   0        0        0     2469 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.0/NodeGraphQt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 08:55:01.237596 NodeGraphQt-0.6.0/NodeGraphQt/base/
--rw-rw-rw-   0        0        0        0 2022-10-18 20:17:59.000000 NodeGraphQt-0.6.0/NodeGraphQt/base/__init__.py
--rw-rw-rw-   0        0        0    12642 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.0/NodeGraphQt/base/commands.py
--rw-rw-rw-   0        0        0     2816 2022-10-18 20:17:59.000000 NodeGraphQt-0.6.0/NodeGraphQt/base/factory.py
--rw-rw-rw-   0        0        0   102277 2023-05-19 08:52:52.000000 NodeGraphQt-0.6.0/NodeGraphQt/base/graph.py
--rw-rw-rw-   0        0        0     8273 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.0/NodeGraphQt/base/menu.py
--rw-rw-rw-   0        0        0    20817 2023-05-19 08:52:52.000000 NodeGraphQt-0.6.0/NodeGraphQt/base/model.py
--rw-rw-rw-   0        0        0    15016 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.0/NodeGraphQt/base/node.py
--rw-rw-rw-   0        0        0    16292 2023-05-19 08:52:52.000000 NodeGraphQt-0.6.0/NodeGraphQt/base/port.py
--rw-rw-rw-   0        0        0     7417 2023-05-09 09:46:08.000000 NodeGraphQt-0.6.0/NodeGraphQt/constants.py
-drwxrwxrwx   0        0        0        0 2023-05-19 08:55:01.251600 NodeGraphQt-0.6.0/NodeGraphQt/custom_widgets/
--rw-rw-rw-   0        0        0        0 2022-05-08 02:47:52.000000 NodeGraphQt-0.6.0/NodeGraphQt/custom_widgets/__init__.py
--rw-rw-rw-   0        0        0    11914 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.0/NodeGraphQt/custom_widgets/nodes_palette.py
--rw-rw-rw-   0        0        0     4749 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.0/NodeGraphQt/custom_widgets/nodes_tree.py
-drwxrwxrwx   0        0        0        0 2023-05-19 08:55:01.309614 NodeGraphQt-0.6.0/NodeGraphQt/custom_widgets/properties_bin/
--rw-rw-rw-   0        0        0        0 2022-12-21 22:27:30.000000 NodeGraphQt-0.6.0/NodeGraphQt/custom_widgets/properties_bin/__init__.py
--rw-rw-rw-   0        0        0     3550 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.0/NodeGraphQt/custom_widgets/properties_bin/custom_widget_color_picker.py
--rw-rw-rw-   0        0        0     2455 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.0/NodeGraphQt/custom_widgets/properties_bin/custom_widget_file_paths.py
--rw-rw-rw-   0        0        0     4995 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.0/NodeGraphQt/custom_widgets/properties_bin/custom_widget_slider.py
--rw-rw-rw-   0        0        0     6304 2022-12-21 22:27:30.000000 NodeGraphQt-0.6.0/NodeGraphQt/custom_widgets/properties_bin/custom_widget_value_edit.py
--rw-rw-rw-   0        0        0     2948 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.0/NodeGraphQt/custom_widgets/properties_bin/custom_widget_vectors.py
--rw-rw-rw-   0        0        0     2489 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.0/NodeGraphQt/custom_widgets/properties_bin/node_property_factory.py
--rw-rw-rw-   0        0        0    20765 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.0/NodeGraphQt/custom_widgets/properties_bin/node_property_widgets.py
--rw-rw-rw-   0        0        0      761 2022-12-21 22:27:30.000000 NodeGraphQt-0.6.0/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_abstract.py
--rw-rw-rw-   0        0        0     7267 2022-12-21 22:27:30.000000 NodeGraphQt-0.6.0/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_base.py
--rw-rw-rw-   0        0        0      406 2022-10-18 20:17:59.000000 NodeGraphQt-0.6.0/NodeGraphQt/errors.py
-drwxrwxrwx   0        0        0        0 2023-05-19 08:55:01.329616 NodeGraphQt-0.6.0/NodeGraphQt/nodes/
--rw-rw-rw-   0        0        0        0 2022-05-08 02:47:52.000000 NodeGraphQt-0.6.0/NodeGraphQt/nodes/__init__.py
--rw-rw-rw-   0        0        0     4465 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.0/NodeGraphQt/nodes/backdrop_node.py
--rw-rw-rw-   0        0        0    27546 2023-05-19 08:52:52.000000 NodeGraphQt-0.6.0/NodeGraphQt/nodes/base_node.py
--rw-rw-rw-   0        0        0     1253 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.0/NodeGraphQt/nodes/base_node_circle.py
--rw-rw-rw-   0        0        0     5817 2023-05-07 11:27:54.000000 NodeGraphQt-0.6.0/NodeGraphQt/nodes/group_node.py
--rw-rw-rw-   0        0        0     4409 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.0/NodeGraphQt/nodes/port_node.py
--rw-rw-rw-   0        0        0      239 2023-05-19 08:52:52.000000 NodeGraphQt-0.6.0/NodeGraphQt/pkg_info.py
-drwxrwxrwx   0        0        0        0 2023-05-19 08:55:01.385630 NodeGraphQt-0.6.0/NodeGraphQt/qgraphics/
--rw-rw-rw-   0        0        0        0 2021-06-18 10:54:50.000000 NodeGraphQt-0.6.0/NodeGraphQt/qgraphics/__init__.py
--rw-rw-rw-   0        0        0     7060 2023-04-19 08:52:02.000000 NodeGraphQt-0.6.0/NodeGraphQt/qgraphics/node_abstract.py
--rw-rw-rw-   0        0        0    11022 2023-05-08 10:29:06.000000 NodeGraphQt-0.6.0/NodeGraphQt/qgraphics/node_backdrop.py
--rw-rw-rw-   0        0        0    37021 2023-05-19 08:52:52.000000 NodeGraphQt-0.6.0/NodeGraphQt/qgraphics/node_base.py
--rw-rw-rw-   0        0        0    21204 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.0/NodeGraphQt/qgraphics/node_circle.py
--rw-rw-rw-   0        0        0    12346 2022-10-18 20:17:59.000000 NodeGraphQt-0.6.0/NodeGraphQt/qgraphics/node_group.py
--rw-rw-rw-   0        0        0     4273 2022-05-08 02:47:52.000000 NodeGraphQt-0.6.0/NodeGraphQt/qgraphics/node_overlay_disabled.py
--rw-rw-rw-   0        0        0     8159 2022-10-18 20:17:59.000000 NodeGraphQt-0.6.0/NodeGraphQt/qgraphics/node_port_in.py
--rw-rw-rw-   0        0        0     8158 2022-10-18 20:17:59.000000 NodeGraphQt-0.6.0/NodeGraphQt/qgraphics/node_port_out.py
--rw-rw-rw-   0        0        0     3749 2022-05-08 02:47:52.000000 NodeGraphQt-0.6.0/NodeGraphQt/qgraphics/node_text_item.py
--rw-rw-rw-   0        0        0    23761 2023-05-19 08:52:52.000000 NodeGraphQt-0.6.0/NodeGraphQt/qgraphics/pipe.py
--rw-rw-rw-   0        0        0    10582 2023-04-30 08:29:15.000000 NodeGraphQt-0.6.0/NodeGraphQt/qgraphics/port.py
--rw-rw-rw-   0        0        0     2885 2023-05-03 09:02:56.000000 NodeGraphQt-0.6.0/NodeGraphQt/qgraphics/slicer.py
-drwxrwxrwx   0        0        0        0 2023-05-19 08:55:01.431950 NodeGraphQt-0.6.0/NodeGraphQt/widgets/
--rw-rw-rw-   0        0        0        0 2022-10-18 20:17:59.000000 NodeGraphQt-0.6.0/NodeGraphQt/widgets/__init__.py
--rw-rw-rw-   0        0        0     3709 2022-12-21 07:01:38.000000 NodeGraphQt-0.6.0/NodeGraphQt/widgets/actions.py
--rw-rw-rw-   0        0        0     1873 2022-10-18 20:17:59.000000 NodeGraphQt-0.6.0/NodeGraphQt/widgets/dialogs.py
-drwxrwxrwx   0        0        0        0 2023-05-19 08:55:01.432951 NodeGraphQt-0.6.0/NodeGraphQt/widgets/icons/
--rw-rw-rw-   0        0        0    17542 2021-06-18 10:54:50.000000 NodeGraphQt-0.6.0/NodeGraphQt/widgets/icons/node_base.png
--rw-rw-rw-   0        0        0     4550 2023-05-03 09:15:23.000000 NodeGraphQt-0.6.0/NodeGraphQt/widgets/node_graph.py
--rw-rw-rw-   0        0        0    14045 2023-05-07 22:11:12.000000 NodeGraphQt-0.6.0/NodeGraphQt/widgets/node_widgets.py
--rw-rw-rw-   0        0        0     5681 2022-10-18 20:17:59.000000 NodeGraphQt-0.6.0/NodeGraphQt/widgets/scene.py
--rw-rw-rw-   0        0        0    11436 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.0/NodeGraphQt/widgets/tab_search.py
--rw-rw-rw-   0        0        0    55886 2023-05-19 08:52:52.000000 NodeGraphQt-0.6.0/NodeGraphQt/widgets/viewer.py
--rw-rw-rw-   0        0        0     6914 2023-05-07 11:27:54.000000 NodeGraphQt-0.6.0/NodeGraphQt/widgets/viewer_nav.py
-drwxrwxrwx   0        0        0        0 2023-05-19 08:55:01.205588 NodeGraphQt-0.6.0/NodeGraphQt.egg-info/
--rw-rw-rw-   0        0        0     2746 2023-05-19 08:55:01.000000 NodeGraphQt-0.6.0/NodeGraphQt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2543 2023-05-19 08:55:01.000000 NodeGraphQt-0.6.0/NodeGraphQt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 08:55:01.000000 NodeGraphQt-0.6.0/NodeGraphQt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-05-19 08:55:01.000000 NodeGraphQt-0.6.0/NodeGraphQt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-05-19 08:55:01.000000 NodeGraphQt-0.6.0/NodeGraphQt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2746 2023-05-19 08:55:01.458956 NodeGraphQt-0.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     2042 2023-05-07 23:03:54.000000 NodeGraphQt-0.6.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 08:55:01.163579 NodeGraphQt-0.6.0/examples/
-drwxrwxrwx   0        0        0        0 2023-05-19 08:55:01.439952 NodeGraphQt-0.6.0/examples/hotkeys/
--rw-rw-rw-   0        0        0        0 2022-10-18 20:17:59.000000 NodeGraphQt-0.6.0/examples/hotkeys/__init__.py
--rw-rw-rw-   0        0        0     6199 2023-05-07 11:27:54.000000 NodeGraphQt-0.6.0/examples/hotkeys/hotkey_functions.py
-drwxrwxrwx   0        0        0        0 2023-05-19 08:55:01.457956 NodeGraphQt-0.6.0/examples/nodes/
--rw-rw-rw-   0        0        0        0 2022-10-18 20:17:59.000000 NodeGraphQt-0.6.0/examples/nodes/__init__.py
--rw-rw-rw-   0        0        0     2157 2023-05-19 07:23:03.000000 NodeGraphQt-0.6.0/examples/nodes/basic_nodes.py
--rw-rw-rw-   0        0        0     3671 2022-10-18 20:17:59.000000 NodeGraphQt-0.6.0/examples/nodes/custom_ports_node.py
--rw-rw-rw-   0        0        0      507 2022-10-18 20:17:59.000000 NodeGraphQt-0.6.0/examples/nodes/group_node.py
--rw-rw-rw-   0        0        0     1822 2023-05-02 10:58:55.000000 NodeGraphQt-0.6.0/examples/nodes/widget_nodes.py
--rw-rw-rw-   0        0        0     1070 2023-05-19 08:55:01.464958 NodeGraphQt-0.6.0/setup.cfg
--rw-rw-rw-   0        0        0      123 2022-12-21 06:31:06.000000 NodeGraphQt-0.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 11:33:44.313837 NodeGraphQt-0.6.1/
+-rw-rw-rw-   0        0        0     1102 2021-06-18 10:54:50.000000 NodeGraphQt-0.6.1/LICENSE.md
+-rw-rw-rw-   0        0        0       49 2022-05-22 21:37:50.000000 NodeGraphQt-0.6.1/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-05-20 11:33:43.979762 NodeGraphQt-0.6.1/NodeGraphQt/
+-rw-rw-rw-   0        0        0     2469 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.1/NodeGraphQt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-20 11:33:44.038775 NodeGraphQt-0.6.1/NodeGraphQt/base/
+-rw-rw-rw-   0        0        0        0 2022-10-18 20:17:59.000000 NodeGraphQt-0.6.1/NodeGraphQt/base/__init__.py
+-rw-rw-rw-   0        0        0    12642 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.1/NodeGraphQt/base/commands.py
+-rw-rw-rw-   0        0        0     2816 2022-10-18 20:17:59.000000 NodeGraphQt-0.6.1/NodeGraphQt/base/factory.py
+-rw-rw-rw-   0        0        0   103281 2023-05-20 11:27:20.000000 NodeGraphQt-0.6.1/NodeGraphQt/base/graph.py
+-rw-rw-rw-   0        0        0     8273 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.1/NodeGraphQt/base/menu.py
+-rw-rw-rw-   0        0        0    20908 2023-05-20 10:49:23.000000 NodeGraphQt-0.6.1/NodeGraphQt/base/model.py
+-rw-rw-rw-   0        0        0    15016 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.1/NodeGraphQt/base/node.py
+-rw-rw-rw-   0        0        0    16292 2023-05-19 08:52:52.000000 NodeGraphQt-0.6.1/NodeGraphQt/base/port.py
+-rw-rw-rw-   0        0        0     7417 2023-05-09 09:46:08.000000 NodeGraphQt-0.6.1/NodeGraphQt/constants.py
+drwxrwxrwx   0        0        0        0 2023-05-20 11:33:44.054778 NodeGraphQt-0.6.1/NodeGraphQt/custom_widgets/
+-rw-rw-rw-   0        0        0        0 2022-05-08 02:47:52.000000 NodeGraphQt-0.6.1/NodeGraphQt/custom_widgets/__init__.py
+-rw-rw-rw-   0        0        0    11914 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.1/NodeGraphQt/custom_widgets/nodes_palette.py
+-rw-rw-rw-   0        0        0     4749 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.1/NodeGraphQt/custom_widgets/nodes_tree.py
+drwxrwxrwx   0        0        0        0 2023-05-20 11:33:44.114791 NodeGraphQt-0.6.1/NodeGraphQt/custom_widgets/properties_bin/
+-rw-rw-rw-   0        0        0        0 2022-12-21 22:27:30.000000 NodeGraphQt-0.6.1/NodeGraphQt/custom_widgets/properties_bin/__init__.py
+-rw-rw-rw-   0        0        0     3550 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.1/NodeGraphQt/custom_widgets/properties_bin/custom_widget_color_picker.py
+-rw-rw-rw-   0        0        0     2455 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.1/NodeGraphQt/custom_widgets/properties_bin/custom_widget_file_paths.py
+-rw-rw-rw-   0        0        0     4995 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.1/NodeGraphQt/custom_widgets/properties_bin/custom_widget_slider.py
+-rw-rw-rw-   0        0        0     6304 2022-12-21 22:27:30.000000 NodeGraphQt-0.6.1/NodeGraphQt/custom_widgets/properties_bin/custom_widget_value_edit.py
+-rw-rw-rw-   0        0        0     2948 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.1/NodeGraphQt/custom_widgets/properties_bin/custom_widget_vectors.py
+-rw-rw-rw-   0        0        0     2489 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.1/NodeGraphQt/custom_widgets/properties_bin/node_property_factory.py
+-rw-rw-rw-   0        0        0    20765 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.1/NodeGraphQt/custom_widgets/properties_bin/node_property_widgets.py
+-rw-rw-rw-   0        0        0      761 2022-12-21 22:27:30.000000 NodeGraphQt-0.6.1/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_abstract.py
+-rw-rw-rw-   0        0        0     7267 2022-12-21 22:27:30.000000 NodeGraphQt-0.6.1/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_base.py
+-rw-rw-rw-   0        0        0      406 2022-10-18 20:17:59.000000 NodeGraphQt-0.6.1/NodeGraphQt/errors.py
+drwxrwxrwx   0        0        0        0 2023-05-20 11:33:44.147800 NodeGraphQt-0.6.1/NodeGraphQt/nodes/
+-rw-rw-rw-   0        0        0        0 2022-05-08 02:47:52.000000 NodeGraphQt-0.6.1/NodeGraphQt/nodes/__init__.py
+-rw-rw-rw-   0        0        0     4465 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.1/NodeGraphQt/nodes/backdrop_node.py
+-rw-rw-rw-   0        0        0    27550 2023-05-20 01:32:47.000000 NodeGraphQt-0.6.1/NodeGraphQt/nodes/base_node.py
+-rw-rw-rw-   0        0        0     1253 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.1/NodeGraphQt/nodes/base_node_circle.py
+-rw-rw-rw-   0        0        0     5817 2023-05-07 11:27:54.000000 NodeGraphQt-0.6.1/NodeGraphQt/nodes/group_node.py
+-rw-rw-rw-   0        0        0     4409 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.1/NodeGraphQt/nodes/port_node.py
+-rw-rw-rw-   0        0        0      239 2023-05-20 10:45:33.000000 NodeGraphQt-0.6.1/NodeGraphQt/pkg_info.py
+drwxrwxrwx   0        0        0        0 2023-05-20 11:33:44.221816 NodeGraphQt-0.6.1/NodeGraphQt/qgraphics/
+-rw-rw-rw-   0        0        0        0 2021-06-18 10:54:50.000000 NodeGraphQt-0.6.1/NodeGraphQt/qgraphics/__init__.py
+-rw-rw-rw-   0        0        0     7060 2023-04-19 08:52:02.000000 NodeGraphQt-0.6.1/NodeGraphQt/qgraphics/node_abstract.py
+-rw-rw-rw-   0        0        0    11022 2023-05-08 10:29:06.000000 NodeGraphQt-0.6.1/NodeGraphQt/qgraphics/node_backdrop.py
+-rw-rw-rw-   0        0        0    37021 2023-05-19 08:52:52.000000 NodeGraphQt-0.6.1/NodeGraphQt/qgraphics/node_base.py
+-rw-rw-rw-   0        0        0    21204 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.1/NodeGraphQt/qgraphics/node_circle.py
+-rw-rw-rw-   0        0        0    12346 2022-10-18 20:17:59.000000 NodeGraphQt-0.6.1/NodeGraphQt/qgraphics/node_group.py
+-rw-rw-rw-   0        0        0     4273 2022-05-08 02:47:52.000000 NodeGraphQt-0.6.1/NodeGraphQt/qgraphics/node_overlay_disabled.py
+-rw-rw-rw-   0        0        0     8159 2022-10-18 20:17:59.000000 NodeGraphQt-0.6.1/NodeGraphQt/qgraphics/node_port_in.py
+-rw-rw-rw-   0        0        0     8158 2022-10-18 20:17:59.000000 NodeGraphQt-0.6.1/NodeGraphQt/qgraphics/node_port_out.py
+-rw-rw-rw-   0        0        0     3749 2022-05-08 02:47:52.000000 NodeGraphQt-0.6.1/NodeGraphQt/qgraphics/node_text_item.py
+-rw-rw-rw-   0        0        0    23761 2023-05-19 08:52:52.000000 NodeGraphQt-0.6.1/NodeGraphQt/qgraphics/pipe.py
+-rw-rw-rw-   0        0        0    10582 2023-04-30 08:29:15.000000 NodeGraphQt-0.6.1/NodeGraphQt/qgraphics/port.py
+-rw-rw-rw-   0        0        0     2885 2023-05-03 09:02:56.000000 NodeGraphQt-0.6.1/NodeGraphQt/qgraphics/slicer.py
+drwxrwxrwx   0        0        0        0 2023-05-20 11:33:44.278828 NodeGraphQt-0.6.1/NodeGraphQt/widgets/
+-rw-rw-rw-   0        0        0        0 2022-10-18 20:17:59.000000 NodeGraphQt-0.6.1/NodeGraphQt/widgets/__init__.py
+-rw-rw-rw-   0        0        0     3709 2022-12-21 07:01:38.000000 NodeGraphQt-0.6.1/NodeGraphQt/widgets/actions.py
+-rw-rw-rw-   0        0        0     1873 2022-10-18 20:17:59.000000 NodeGraphQt-0.6.1/NodeGraphQt/widgets/dialogs.py
+drwxrwxrwx   0        0        0        0 2023-05-20 11:33:44.279829 NodeGraphQt-0.6.1/NodeGraphQt/widgets/icons/
+-rw-rw-rw-   0        0        0    17542 2021-06-18 10:54:50.000000 NodeGraphQt-0.6.1/NodeGraphQt/widgets/icons/node_base.png
+-rw-rw-rw-   0        0        0     4550 2023-05-03 09:15:23.000000 NodeGraphQt-0.6.1/NodeGraphQt/widgets/node_graph.py
+-rw-rw-rw-   0        0        0    14045 2023-05-07 22:11:12.000000 NodeGraphQt-0.6.1/NodeGraphQt/widgets/node_widgets.py
+-rw-rw-rw-   0        0        0     5681 2022-10-18 20:17:59.000000 NodeGraphQt-0.6.1/NodeGraphQt/widgets/scene.py
+-rw-rw-rw-   0        0        0    11436 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.1/NodeGraphQt/widgets/tab_search.py
+-rw-rw-rw-   0        0        0    55886 2023-05-19 08:52:52.000000 NodeGraphQt-0.6.1/NodeGraphQt/widgets/viewer.py
+-rw-rw-rw-   0        0        0     6914 2023-05-07 11:27:54.000000 NodeGraphQt-0.6.1/NodeGraphQt/widgets/viewer_nav.py
+drwxrwxrwx   0        0        0        0 2023-05-20 11:33:43.999765 NodeGraphQt-0.6.1/NodeGraphQt.egg-info/
+-rw-rw-rw-   0        0        0     2746 2023-05-20 11:33:43.000000 NodeGraphQt-0.6.1/NodeGraphQt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2543 2023-05-20 11:33:43.000000 NodeGraphQt-0.6.1/NodeGraphQt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 11:33:43.000000 NodeGraphQt-0.6.1/NodeGraphQt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-05-20 11:33:43.000000 NodeGraphQt-0.6.1/NodeGraphQt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-20 11:33:43.000000 NodeGraphQt-0.6.1/NodeGraphQt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2746 2023-05-20 11:33:44.313837 NodeGraphQt-0.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2042 2023-05-07 23:03:54.000000 NodeGraphQt-0.6.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-20 11:33:43.946753 NodeGraphQt-0.6.1/examples/
+drwxrwxrwx   0        0        0        0 2023-05-20 11:33:44.286831 NodeGraphQt-0.6.1/examples/hotkeys/
+-rw-rw-rw-   0        0        0        0 2022-10-18 20:17:59.000000 NodeGraphQt-0.6.1/examples/hotkeys/__init__.py
+-rw-rw-rw-   0        0        0     6199 2023-05-07 11:27:54.000000 NodeGraphQt-0.6.1/examples/hotkeys/hotkey_functions.py
+drwxrwxrwx   0        0        0        0 2023-05-20 11:33:44.312838 NodeGraphQt-0.6.1/examples/nodes/
+-rw-rw-rw-   0        0        0        0 2022-10-18 20:17:59.000000 NodeGraphQt-0.6.1/examples/nodes/__init__.py
+-rw-rw-rw-   0        0        0     2157 2023-05-19 07:23:03.000000 NodeGraphQt-0.6.1/examples/nodes/basic_nodes.py
+-rw-rw-rw-   0        0        0     3671 2022-10-18 20:17:59.000000 NodeGraphQt-0.6.1/examples/nodes/custom_ports_node.py
+-rw-rw-rw-   0        0        0      507 2022-10-18 20:17:59.000000 NodeGraphQt-0.6.1/examples/nodes/group_node.py
+-rw-rw-rw-   0        0        0     1822 2023-05-02 10:58:55.000000 NodeGraphQt-0.6.1/examples/nodes/widget_nodes.py
+-rw-rw-rw-   0        0        0     1070 2023-05-20 11:33:44.319837 NodeGraphQt-0.6.1/setup.cfg
+-rw-rw-rw-   0        0        0      123 2022-12-21 06:31:06.000000 NodeGraphQt-0.6.1/setup.py
```

### Comparing `NodeGraphQt-0.6.0/LICENSE.md` & `NodeGraphQt-0.6.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.0/NodeGraphQt/__init__.py` & `NodeGraphQt-0.6.1/NodeGraphQt/__init__.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.0/NodeGraphQt/base/commands.py` & `NodeGraphQt-0.6.1/NodeGraphQt/base/commands.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.0/NodeGraphQt/base/factory.py` & `NodeGraphQt-0.6.1/NodeGraphQt/base/factory.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.0/NodeGraphQt/base/graph.py` & `NodeGraphQt-0.6.1/NodeGraphQt/base/graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,38 +132,44 @@
             parent (object): object parent.
             **kwargs (dict): Used for overriding internal objects at init time.
         """
         super(NodeGraph, self).__init__(parent)
         self.setObjectName('NodeGraph')
         self._model = (
             kwargs.get('model') or NodeGraphModel())
+        self._node_factory = (
+            kwargs.get('node_factory') or NodeFactory())
+        self._undo_view = None
+        self._undo_stack = (
+            kwargs.get('undo_stack') or QtWidgets.QUndoStack(self)
+        )
+        self._widget = None
+        self._sub_graphs = {}
+        self._viewer = (
+            kwargs.get('viewer') or NodeViewer(undo_stack=self._undo_stack)
+        )
 
         layout_direction = kwargs.get('layout_direction')
         if layout_direction:
             if layout_direction not in [e.value for e in LayoutDirectionEnum]:
                 layout_direction = LayoutDirectionEnum.HORIZONTAL.value
             self._model.layout_direction = layout_direction
         else:
             layout_direction = self._model.layout_direction
-
-        self._node_factory = (
-            kwargs.get('node_factory') or NodeFactory())
-
-        self._undo_view = None
-        self._undo_stack = (
-            kwargs.get('undo_stack') or QtWidgets.QUndoStack(self))
-
-        self._widget = None
-
-        self._sub_graphs = {}
-
-        self._viewer = (
-            kwargs.get('viewer') or NodeViewer(undo_stack=self._undo_stack))
         self._viewer.set_layout_direction(layout_direction)
 
+        pipe_style = kwargs.get('pipe_style')
+        if pipe_style is not None:
+            if pipe_style not in [e.value for e in PipeLayoutEnum]:
+                pipe_style = PipeLayoutEnum.CURVED.value
+            self._model.pipe_style = pipe_style
+        else:
+            pipe_style = self._model.pipe_style
+        self._viewer.set_pipe_layout(pipe_style)
+
         # viewer needs a reference to the model port connection constrains
         # for the user interaction with the live pipe.
         self._viewer.accept_connection_types = self._model.accept_connection_types
         self._viewer.reject_connection_types = self._model.reject_connection_types
 
         self._context_menu = {}
 
@@ -949,14 +955,26 @@
 
         Args:
             mode (bool): False to disable the slicer pipe.
         """
         self._model.pipe_slicing = mode
         self._viewer.pipe_slicing = self._model.pipe_slicing
 
+    def pipe_style(self):
+        """
+        Returns the current pipe layout style.
+
+        See Also:
+            :meth:`NodeGraph.set_pipe_style`
+
+        Returns:
+            int: pipe style value. :attr:`NodeGraphQt.constants.PipeLayoutEnum`
+        """
+        return self._model.pipe_style
+
     def set_pipe_style(self, style=PipeLayoutEnum.CURVED.value):
         """
         Set node graph pipes to be drawn as curved `(default)`, straight or angled.
 
         .. code-block:: python
             :linenos:
 
@@ -972,29 +990,30 @@
         Args:
             style (int): pipe layout style.
         """
         pipe_max = max([PipeLayoutEnum.CURVED.value,
                         PipeLayoutEnum.STRAIGHT.value,
                         PipeLayoutEnum.ANGLE.value])
         style = style if 0 <= style <= pipe_max else PipeLayoutEnum.CURVED.value
+        self._model.pipe_style = style
         self._viewer.set_pipe_layout(style)
 
     def layout_direction(self):
         """
         Return the current node graph layout direction.
 
         `Implemented in` ``v0.3.0``
 
         See Also:
             :meth:`NodeGraph.set_layout_direction`
 
         Returns:
             int: layout direction.
         """
-        return self.model.layout_direction
+        return self._model.layout_direction
 
     def set_layout_direction(self, direction):
         """
         Sets the node graph layout direction to horizontal or vertical.
         This function will also override the layout direction on all
         nodes in the current node graph.
 
@@ -1620,14 +1639,15 @@
         nodes_data = {}
 
         # serialize graph session.
         serial_data['graph']['layout_direction'] = self.layout_direction()
         serial_data['graph']['acyclic'] = self.acyclic()
         serial_data['graph']['pipe_collision'] = self.pipe_collision()
         serial_data['graph']['pipe_slicing'] = self.pipe_slicing()
+        serial_data['graph']['pipe_style'] = self.pipe_style()
 
         # connection constrains.
         serial_data['graph']['accept_connection_types'] = self.model.accept_connection_types
         serial_data['graph']['reject_connection_types'] = self.model.reject_connection_types
 
         # serialize nodes.
         for n in nodes:
@@ -1688,14 +1708,16 @@
                 self.set_layout_direction(attr_value)
             elif attr_name == 'acyclic':
                 self.set_acyclic(attr_value)
             elif attr_name == 'pipe_collision':
                 self.set_pipe_collision(attr_value)
             elif attr_name == 'pipe_slicing':
                 self.set_pipe_slicing(attr_value)
+            elif attr_name == 'pipe_style':
+                self.set_pipe_style(attr_value)
 
             # connection constrains.
             elif attr_name == 'accept_connection_types':
                 self.model.accept_connection_types = attr_value
             elif attr_name == 'reject_connection_types':
                 self.model.reject_connection_types = attr_value
 
@@ -2312,18 +2334,22 @@
             tab_index = self._widget.indexOf(sub_graph.widget)
             self._widget.setCurrentIndex(tab_index)
             return sub_graph
 
         # build new sub graph.
         node_factory = copy.deepcopy(self.node_factory)
         layout_direction = self.layout_direction()
+        kwargs = {
+            'layout_direction': self.layout_direction(),
+            'pipe_style': self.pipe_style(),
+        }
         sub_graph = SubGraph(self,
                              node=node,
                              node_factory=node_factory,
-                             layout_direction=layout_direction)
+                             **kwargs)
 
         # populate the sub graph.
         session = node.get_sub_graph_session()
         sub_graph.deserialize_session(session)
 
         # store reference to expanded.
         self._sub_graphs[node.id] = sub_graph
```

### Comparing `NodeGraphQt-0.6.0/NodeGraphQt/base/menu.py` & `NodeGraphQt-0.6.1/NodeGraphQt/base/menu.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.0/NodeGraphQt/base/model.py` & `NodeGraphQt-0.6.1/NodeGraphQt/base/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 #!/usr/bin/python
 import json
 from collections import defaultdict
 
-from NodeGraphQt.constants import LayoutDirectionEnum, NodePropWidgetEnum
+from NodeGraphQt.constants import (
+    LayoutDirectionEnum,
+    NodePropWidgetEnum,
+    PipeLayoutEnum
+)
 from NodeGraphQt.errors import NodePropertyError
 
 
 class PortModel(object):
     """
     Data dump for a port object.
     """
@@ -440,14 +444,15 @@
         self.reject_connection_types = {}
 
         self.nodes = {}
         self.session = ''
         self.acyclic = True
         self.pipe_collision = False
         self.pipe_slicing = True
+        self.pipe_style = PipeLayoutEnum.CURVED.value
         self.layout_direction = LayoutDirectionEnum.HORIZONTAL.value
 
     def common_properties(self):
         """
         Return all common node properties.
 
         Returns:
```

### Comparing `NodeGraphQt-0.6.0/NodeGraphQt/base/node.py` & `NodeGraphQt-0.6.1/NodeGraphQt/base/node.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.0/NodeGraphQt/base/port.py` & `NodeGraphQt-0.6.1/NodeGraphQt/base/port.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.0/NodeGraphQt/constants.py` & `NodeGraphQt-0.6.1/NodeGraphQt/constants.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.0/NodeGraphQt/custom_widgets/nodes_palette.py` & `NodeGraphQt-0.6.1/NodeGraphQt/custom_widgets/nodes_palette.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.0/NodeGraphQt/custom_widgets/nodes_tree.py` & `NodeGraphQt-0.6.1/NodeGraphQt/custom_widgets/nodes_tree.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.0/NodeGraphQt/custom_widgets/properties_bin/custom_widget_color_picker.py` & `NodeGraphQt-0.6.1/NodeGraphQt/custom_widgets/properties_bin/custom_widget_color_picker.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.0/NodeGraphQt/custom_widgets/properties_bin/custom_widget_file_paths.py` & `NodeGraphQt-0.6.1/NodeGraphQt/custom_widgets/properties_bin/custom_widget_file_paths.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.0/NodeGraphQt/custom_widgets/properties_bin/custom_widget_slider.py` & `NodeGraphQt-0.6.1/NodeGraphQt/custom_widgets/properties_bin/custom_widget_slider.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.0/NodeGraphQt/custom_widgets/properties_bin/custom_widget_value_edit.py` & `NodeGraphQt-0.6.1/NodeGraphQt/custom_widgets/properties_bin/custom_widget_value_edit.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.0/NodeGraphQt/custom_widgets/properties_bin/custom_widget_vectors.py` & `NodeGraphQt-0.6.1/NodeGraphQt/custom_widgets/properties_bin/custom_widget_vectors.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.0/NodeGraphQt/custom_widgets/properties_bin/node_property_factory.py` & `NodeGraphQt-0.6.1/NodeGraphQt/custom_widgets/properties_bin/node_property_factory.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.0/NodeGraphQt/custom_widgets/properties_bin/node_property_widgets.py` & `NodeGraphQt-0.6.1/NodeGraphQt/custom_widgets/properties_bin/node_property_widgets.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.0/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_abstract.py` & `NodeGraphQt-0.6.1/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_abstract.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.0/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_base.py` & `NodeGraphQt-0.6.1/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_base.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.0/NodeGraphQt/nodes/backdrop_node.py` & `NodeGraphQt-0.6.1/NodeGraphQt/nodes/backdrop_node.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.0/NodeGraphQt/nodes/base_node.py` & `NodeGraphQt-0.6.1/NodeGraphQt/nodes/base_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -664,14 +664,15 @@
         Once a constrain has been added only ports of that type specified will
         be allowed a pipe connection.
 
         port type data example
 
         .. highlight:: python
         .. code-block:: python
+
             {
                 'port_name': 'foo'
                 'port_type': PortTypeEnum.IN.value
                 'node_type': 'io.github.jchanvfx.NodeClass'
             }
 
         See Also:
@@ -723,14 +724,15 @@
         Once a constrain has been added only ports of that type specified will
         NOT be allowed a pipe connection.
 
         port type data example
 
         .. highlight:: python
         .. code-block:: python
+
             {
                 'port_name': 'foo'
                 'port_type': PortTypeEnum.IN.value
                 'node_type': 'io.github.jchanvfx.NodeClass'
             }
 
         See Also:
```

### Comparing `NodeGraphQt-0.6.0/NodeGraphQt/nodes/base_node_circle.py` & `NodeGraphQt-0.6.1/NodeGraphQt/nodes/base_node_circle.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.0/NodeGraphQt/nodes/group_node.py` & `NodeGraphQt-0.6.1/NodeGraphQt/nodes/group_node.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.0/NodeGraphQt/nodes/port_node.py` & `NodeGraphQt-0.6.1/NodeGraphQt/nodes/port_node.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.0/NodeGraphQt/qgraphics/node_abstract.py` & `NodeGraphQt-0.6.1/NodeGraphQt/qgraphics/node_abstract.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.0/NodeGraphQt/qgraphics/node_backdrop.py` & `NodeGraphQt-0.6.1/NodeGraphQt/qgraphics/node_backdrop.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.0/NodeGraphQt/qgraphics/node_base.py` & `NodeGraphQt-0.6.1/NodeGraphQt/qgraphics/node_base.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.0/NodeGraphQt/qgraphics/node_circle.py` & `NodeGraphQt-0.6.1/NodeGraphQt/qgraphics/node_circle.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.0/NodeGraphQt/qgraphics/node_group.py` & `NodeGraphQt-0.6.1/NodeGraphQt/qgraphics/node_group.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.0/NodeGraphQt/qgraphics/node_overlay_disabled.py` & `NodeGraphQt-0.6.1/NodeGraphQt/qgraphics/node_overlay_disabled.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.0/NodeGraphQt/qgraphics/node_port_in.py` & `NodeGraphQt-0.6.1/NodeGraphQt/qgraphics/node_port_in.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.0/NodeGraphQt/qgraphics/node_port_out.py` & `NodeGraphQt-0.6.1/NodeGraphQt/qgraphics/node_port_out.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.0/NodeGraphQt/qgraphics/node_text_item.py` & `NodeGraphQt-0.6.1/NodeGraphQt/qgraphics/node_text_item.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.0/NodeGraphQt/qgraphics/pipe.py` & `NodeGraphQt-0.6.1/NodeGraphQt/qgraphics/pipe.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.0/NodeGraphQt/qgraphics/port.py` & `NodeGraphQt-0.6.1/NodeGraphQt/qgraphics/port.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.0/NodeGraphQt/qgraphics/slicer.py` & `NodeGraphQt-0.6.1/NodeGraphQt/qgraphics/slicer.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.0/NodeGraphQt/widgets/actions.py` & `NodeGraphQt-0.6.1/NodeGraphQt/widgets/actions.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.0/NodeGraphQt/widgets/dialogs.py` & `NodeGraphQt-0.6.1/NodeGraphQt/widgets/dialogs.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.0/NodeGraphQt/widgets/icons/node_base.png` & `NodeGraphQt-0.6.1/NodeGraphQt/widgets/icons/node_base.png`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.0/NodeGraphQt/widgets/node_graph.py` & `NodeGraphQt-0.6.1/NodeGraphQt/widgets/node_graph.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.0/NodeGraphQt/widgets/node_widgets.py` & `NodeGraphQt-0.6.1/NodeGraphQt/widgets/node_widgets.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.0/NodeGraphQt/widgets/scene.py` & `NodeGraphQt-0.6.1/NodeGraphQt/widgets/scene.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.0/NodeGraphQt/widgets/tab_search.py` & `NodeGraphQt-0.6.1/NodeGraphQt/widgets/tab_search.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.0/NodeGraphQt/widgets/viewer.py` & `NodeGraphQt-0.6.1/NodeGraphQt/widgets/viewer.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.0/NodeGraphQt/widgets/viewer_nav.py` & `NodeGraphQt-0.6.1/NodeGraphQt/widgets/viewer_nav.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.0/NodeGraphQt.egg-info/PKG-INFO` & `NodeGraphQt-0.6.1/NodeGraphQt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NodeGraphQt
-Version: 0.6.0
+Version: 0.6.1
 Summary: Node graph framework for PySide2/PyQt5 that can be
 Home-page: https://github.com/jchanvfx/NodeGraphQt
 Author: Johnny Chan
 License: MIT License
 Project-URL: Documentation, https://jchanvfx.github.io/NodeGraphQt/api/html/index.html
 Project-URL: Source, https://github.com/jchanvfx/NodeGraphQt/
 Project-URL: Tracker, https://github.com/jchanvfx/NodeGraphQt/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: NodeGraphQt Version: 0.6.0 Summary: Node graph
+Metadata-Version: 2.1 Name: NodeGraphQt Version: 0.6.1 Summary: Node graph
 framework for PySide2/PyQt5 that can be Home-page: https://github.com/jchanvfx/
 NodeGraphQt Author: Johnny Chan License: MIT License Project-URL:
 Documentation, https://jchanvfx.github.io/NodeGraphQt/api/html/index.html
 Project-URL: Source, https://github.com/jchanvfx/NodeGraphQt/ Project-URL:
 Tracker, https://github.com/jchanvfx/NodeGraphQt/issues Classifier: Operating
 System :: OS Independent Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6 Requires-Python: >=3.6
```

### Comparing `NodeGraphQt-0.6.0/NodeGraphQt.egg-info/SOURCES.txt` & `NodeGraphQt-0.6.1/NodeGraphQt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.0/PKG-INFO` & `NodeGraphQt-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NodeGraphQt
-Version: 0.6.0
+Version: 0.6.1
 Summary: Node graph framework for PySide2/PyQt5 that can be
 Home-page: https://github.com/jchanvfx/NodeGraphQt
 Author: Johnny Chan
 License: MIT License
 Project-URL: Documentation, https://jchanvfx.github.io/NodeGraphQt/api/html/index.html
 Project-URL: Source, https://github.com/jchanvfx/NodeGraphQt/
 Project-URL: Tracker, https://github.com/jchanvfx/NodeGraphQt/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: NodeGraphQt Version: 0.6.0 Summary: Node graph
+Metadata-Version: 2.1 Name: NodeGraphQt Version: 0.6.1 Summary: Node graph
 framework for PySide2/PyQt5 that can be Home-page: https://github.com/jchanvfx/
 NodeGraphQt Author: Johnny Chan License: MIT License Project-URL:
 Documentation, https://jchanvfx.github.io/NodeGraphQt/api/html/index.html
 Project-URL: Source, https://github.com/jchanvfx/NodeGraphQt/ Project-URL:
 Tracker, https://github.com/jchanvfx/NodeGraphQt/issues Classifier: Operating
 System :: OS Independent Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6 Requires-Python: >=3.6
```

### Comparing `NodeGraphQt-0.6.0/README.md` & `NodeGraphQt-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.0/examples/hotkeys/hotkey_functions.py` & `NodeGraphQt-0.6.1/examples/hotkeys/hotkey_functions.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.0/examples/nodes/basic_nodes.py` & `NodeGraphQt-0.6.1/examples/nodes/basic_nodes.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.0/examples/nodes/custom_ports_node.py` & `NodeGraphQt-0.6.1/examples/nodes/custom_ports_node.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.0/examples/nodes/widget_nodes.py` & `NodeGraphQt-0.6.1/examples/nodes/widget_nodes.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.0/setup.cfg` & `NodeGraphQt-0.6.1/setup.cfg`

 * *Files identical despite different names*

