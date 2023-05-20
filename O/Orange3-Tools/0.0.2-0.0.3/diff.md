# Comparing `tmp/Orange3-Tools-0.0.2.tar.gz` & `tmp/Orange3-Tools-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Orange3-Tools-0.0.2.tar", last modified: Thu May 18 17:02:12 2023, max compression
+gzip compressed data, was "Orange3-Tools-0.0.3.tar", last modified: Sat May 20 10:52:20 2023, max compression
```

## Comparing `Orange3-Tools-0.0.2.tar` & `Orange3-Tools-0.0.3.tar`

### file list

```diff
@@ -1,38 +1,37 @@
-drwxr-xr-x   0 julioj.melero   (501) staff       (20)        0 2023-05-18 17:02:12.829624 Orange3-Tools-0.0.2/
--rw-rw-rw-   0 julioj.melero   (501) staff       (20)    35801 2023-03-07 11:54:58.000000 Orange3-Tools-0.0.2/LICENSE
-drwxr-xr-x   0 julioj.melero   (501) staff       (20)        0 2023-05-18 17:02:12.820266 Orange3-Tools-0.0.2/Orange3_Tools.egg-info/
--rw-r--r--   0 julioj.melero   (501) staff       (20)      336 2023-05-18 17:02:12.000000 Orange3-Tools-0.0.2/Orange3_Tools.egg-info/PKG-INFO
--rw-r--r--   0 julioj.melero   (501) staff       (20)     1126 2023-05-18 17:02:12.000000 Orange3-Tools-0.0.2/Orange3_Tools.egg-info/SOURCES.txt
--rw-r--r--   0 julioj.melero   (501) staff       (20)        1 2023-05-18 17:02:12.000000 Orange3-Tools-0.0.2/Orange3_Tools.egg-info/dependency_links.txt
--rw-r--r--   0 julioj.melero   (501) staff       (20)       98 2023-05-18 17:02:12.000000 Orange3-Tools-0.0.2/Orange3_Tools.egg-info/entry_points.txt
--rw-r--r--   0 julioj.melero   (501) staff       (20)        1 2023-05-17 10:38:08.000000 Orange3-Tools-0.0.2/Orange3_Tools.egg-info/not-zip-safe
--rw-r--r--   0 julioj.melero   (501) staff       (20)      200 2023-05-18 17:02:12.000000 Orange3-Tools-0.0.2/Orange3_Tools.egg-info/requires.txt
--rw-r--r--   0 julioj.melero   (501) staff       (20)       14 2023-05-18 17:02:12.000000 Orange3-Tools-0.0.2/Orange3_Tools.egg-info/top_level.txt
--rw-r--r--   0 julioj.melero   (501) staff       (20)      336 2023-05-18 17:02:12.829293 Orange3-Tools-0.0.2/PKG-INFO
--rw-rw-rw-   0 julioj.melero   (501) staff       (20)      100 2023-04-13 16:55:45.000000 Orange3-Tools-0.0.2/README.md
-drwxr-xr-x   0 julioj.melero   (501) staff       (20)        0 2023-05-18 17:02:12.820695 Orange3-Tools-0.0.2/orangecontrib/
--rw-rw-rw-   0 julioj.melero   (501) staff       (20)      169 2023-04-11 17:27:18.000000 Orange3-Tools-0.0.2/orangecontrib/__init__.py
--rw-r--r--   0 julioj.melero   (501) staff       (20)    20713 2023-05-18 08:25:22.000000 Orange3-Tools-0.0.2/orangecontrib/functions.py
-drwxr-xr-x   0 julioj.melero   (501) staff       (20)        0 2023-05-18 17:02:12.821158 Orange3-Tools-0.0.2/orangecontrib/tools/
--rw-rw-rw-   0 julioj.melero   (501) staff       (20)      654 2023-04-11 19:26:01.000000 Orange3-Tools-0.0.2/orangecontrib/tools/__init__.py
-drwxr-xr-x   0 julioj.melero   (501) staff       (20)        0 2023-05-18 17:02:12.825831 Orange3-Tools-0.0.2/orangecontrib/tools/widgets/
--rw-r--r--   0 julioj.melero   (501) staff       (20)     6970 2023-04-16 09:51:53.000000 Orange3-Tools-0.0.2/orangecontrib/tools/widgets/Barplot.py
--rw-r--r--   0 julioj.melero   (501) staff       (20)     6982 2023-04-16 09:52:23.000000 Orange3-Tools-0.0.2/orangecontrib/tools/widgets/Linesplot.py
--rw-rw-rw-   0 julioj.melero   (501) staff       (20)     6713 2023-04-16 09:22:31.000000 Orange3-Tools-0.0.2/orangecontrib/tools/widgets/MySqlOrange.py
--rw-r--r--   0 julioj.melero   (501) staff       (20)     9754 2023-04-16 15:10:09.000000 Orange3-Tools-0.0.2/orangecontrib/tools/widgets/Pairsplot.py
--rw-r--r--   0 julioj.melero   (501) staff       (20)     7281 2023-04-16 09:57:24.000000 Orange3-Tools-0.0.2/orangecontrib/tools/widgets/Scatterplot.py
--rw-rw-rw-   0 julioj.melero   (501) staff       (20)     1091 2023-04-13 17:01:11.000000 Orange3-Tools-0.0.2/orangecontrib/tools/widgets/__init__.py
-drwxr-xr-x   0 julioj.melero   (501) staff       (20)        0 2023-05-18 17:02:12.828957 Orange3-Tools-0.0.2/orangecontrib/tools/widgets/icons/
--rw-r--r--   0 julioj.melero   (501) staff       (20)    14469 2023-05-17 10:00:19.000000 Orange3-Tools-0.0.2/orangecontrib/tools/widgets/icons/ARIMA.svg
--rw-------   0 julioj.melero   (501) staff       (20)     1513 2023-04-16 09:12:55.000000 Orange3-Tools-0.0.2/orangecontrib/tools/widgets/icons/Barchart.svg
--rw-r--r--   0 julioj.melero   (501) staff       (20)     9756 2023-05-17 10:00:19.000000 Orange3-Tools-0.0.2/orangecontrib/tools/widgets/icons/Correlogram.svg
--rw-------   0 julioj.melero   (501) staff       (20)    15156 2023-04-16 09:04:28.000000 Orange3-Tools-0.0.2/orangecontrib/tools/widgets/icons/Pairs.svg
--rw-rw-rw-   0 julioj.melero   (501) staff       (20)     5586 2023-04-11 16:37:34.000000 Orange3-Tools-0.0.2/orangecontrib/tools/widgets/icons/Simple_scatterplot.svg
--rw-r--r--   0 julioj.melero   (501) staff       (20)    10454 2023-04-16 09:14:11.000000 Orange3-Tools-0.0.2/orangecontrib/tools/widgets/icons/category.svg
--rw-rw-rw-   0 julioj.melero   (501) staff       (20)     3595 2023-03-08 12:27:13.000000 Orange3-Tools-0.0.2/orangecontrib/tools/widgets/icons/mysql-orange.svg
--rw-r--r--   0 julioj.melero   (501) staff       (20)     4964 2023-04-11 17:00:16.000000 Orange3-Tools-0.0.2/orangecontrib/tools/widgets/icons/sscater.svg
--rw-r--r--   0 julioj.melero   (501) staff       (20)     5175 2023-05-18 08:35:35.000000 Orange3-Tools-0.0.2/orangecontrib/tools/widgets/owcorrelogram.py
--rw-r--r--   0 julioj.melero   (501) staff       (20)    30247 2023-05-18 16:46:54.000000 Orange3-Tools-0.0.2/orangecontrib/tools/widgets/owsarima.py
--rw-r--r--   0 julioj.melero   (501) staff       (20)     2212 2023-04-13 16:39:56.000000 Orange3-Tools-0.0.2/orangecontrib/tools/widgets/utils.py
--rw-r--r--   0 julioj.melero   (501) staff       (20)       38 2023-05-18 17:02:12.829673 Orange3-Tools-0.0.2/setup.cfg
--rw-rw-rw-   0 julioj.melero   (501) staff       (20)     3576 2023-05-18 08:27:14.000000 Orange3-Tools-0.0.2/setup.py
+drwxr-xr-x   0 julioj.melero   (501) staff       (20)        0 2023-05-20 10:52:20.148280 Orange3-Tools-0.0.3/
+-rw-rw-rw-   0 julioj.melero   (501) staff       (20)    35801 2023-03-07 11:54:58.000000 Orange3-Tools-0.0.3/LICENSE
+drwxr-xr-x   0 julioj.melero   (501) staff       (20)        0 2023-05-20 10:52:20.141695 Orange3-Tools-0.0.3/Orange3_Tools.egg-info/
+-rw-r--r--   0 julioj.melero   (501) staff       (20)      336 2023-05-20 10:52:20.000000 Orange3-Tools-0.0.3/Orange3_Tools.egg-info/PKG-INFO
+-rw-r--r--   0 julioj.melero   (501) staff       (20)     1092 2023-05-20 10:52:20.000000 Orange3-Tools-0.0.3/Orange3_Tools.egg-info/SOURCES.txt
+-rw-r--r--   0 julioj.melero   (501) staff       (20)        1 2023-05-20 10:52:20.000000 Orange3-Tools-0.0.3/Orange3_Tools.egg-info/dependency_links.txt
+-rw-r--r--   0 julioj.melero   (501) staff       (20)       98 2023-05-20 10:52:20.000000 Orange3-Tools-0.0.3/Orange3_Tools.egg-info/entry_points.txt
+-rw-r--r--   0 julioj.melero   (501) staff       (20)        1 2023-05-17 10:38:08.000000 Orange3-Tools-0.0.3/Orange3_Tools.egg-info/not-zip-safe
+-rw-r--r--   0 julioj.melero   (501) staff       (20)      200 2023-05-20 10:52:20.000000 Orange3-Tools-0.0.3/Orange3_Tools.egg-info/requires.txt
+-rw-r--r--   0 julioj.melero   (501) staff       (20)       14 2023-05-20 10:52:20.000000 Orange3-Tools-0.0.3/Orange3_Tools.egg-info/top_level.txt
+-rw-r--r--   0 julioj.melero   (501) staff       (20)      336 2023-05-20 10:52:20.148130 Orange3-Tools-0.0.3/PKG-INFO
+-rw-rw-rw-   0 julioj.melero   (501) staff       (20)      100 2023-04-13 16:55:45.000000 Orange3-Tools-0.0.3/README.md
+drwxr-xr-x   0 julioj.melero   (501) staff       (20)        0 2023-05-20 10:52:20.142111 Orange3-Tools-0.0.3/orangecontrib/
+-rw-rw-rw-   0 julioj.melero   (501) staff       (20)      169 2023-04-11 17:27:18.000000 Orange3-Tools-0.0.3/orangecontrib/__init__.py
+-rw-r--r--   0 julioj.melero   (501) staff       (20)    20713 2023-05-18 08:25:22.000000 Orange3-Tools-0.0.3/orangecontrib/functions.py
+drwxr-xr-x   0 julioj.melero   (501) staff       (20)        0 2023-05-20 10:52:20.142616 Orange3-Tools-0.0.3/orangecontrib/tools/
+-rw-rw-rw-   0 julioj.melero   (501) staff       (20)      654 2023-04-11 19:26:01.000000 Orange3-Tools-0.0.3/orangecontrib/tools/__init__.py
+drwxr-xr-x   0 julioj.melero   (501) staff       (20)        0 2023-05-20 10:52:20.145630 Orange3-Tools-0.0.3/orangecontrib/tools/widgets/
+-rw-rw-rw-   0 julioj.melero   (501) staff       (20)     6713 2023-04-16 09:22:31.000000 Orange3-Tools-0.0.3/orangecontrib/tools/widgets/MySqlOrange.py
+-rw-r--r--   0 julioj.melero   (501) staff       (20)     9754 2023-04-16 15:10:09.000000 Orange3-Tools-0.0.3/orangecontrib/tools/widgets/Pairsplot.py
+-rw-r--r--   0 julioj.melero   (501) staff       (20)     7281 2023-04-16 09:57:24.000000 Orange3-Tools-0.0.3/orangecontrib/tools/widgets/Scatterplot.py
+-rw-rw-rw-   0 julioj.melero   (501) staff       (20)     1091 2023-04-13 17:01:11.000000 Orange3-Tools-0.0.3/orangecontrib/tools/widgets/__init__.py
+drwxr-xr-x   0 julioj.melero   (501) staff       (20)        0 2023-05-20 10:52:20.147780 Orange3-Tools-0.0.3/orangecontrib/tools/widgets/icons/
+-rw-r--r--   0 julioj.melero   (501) staff       (20)    14469 2023-05-17 10:00:19.000000 Orange3-Tools-0.0.3/orangecontrib/tools/widgets/icons/ARIMA.svg
+-rw-------   0 julioj.melero   (501) staff       (20)     1513 2023-04-16 09:12:55.000000 Orange3-Tools-0.0.3/orangecontrib/tools/widgets/icons/Barchart.svg
+-rw-r--r--   0 julioj.melero   (501) staff       (20)     9756 2023-05-17 10:00:19.000000 Orange3-Tools-0.0.3/orangecontrib/tools/widgets/icons/Correlogram.svg
+-rw-------   0 julioj.melero   (501) staff       (20)    15156 2023-04-16 09:04:28.000000 Orange3-Tools-0.0.3/orangecontrib/tools/widgets/icons/Pairs.svg
+-rw-rw-rw-   0 julioj.melero   (501) staff       (20)     5586 2023-04-11 16:37:34.000000 Orange3-Tools-0.0.3/orangecontrib/tools/widgets/icons/Simple_scatterplot.svg
+-rw-r--r--   0 julioj.melero   (501) staff       (20)    10454 2023-04-16 09:14:11.000000 Orange3-Tools-0.0.3/orangecontrib/tools/widgets/icons/category.svg
+-rw-rw-rw-   0 julioj.melero   (501) staff       (20)     3595 2023-03-08 12:27:13.000000 Orange3-Tools-0.0.3/orangecontrib/tools/widgets/icons/mysql-orange.svg
+-rw-r--r--   0 julioj.melero   (501) staff       (20)     4964 2023-04-11 17:00:16.000000 Orange3-Tools-0.0.3/orangecontrib/tools/widgets/icons/sscater.svg
+-rw-r--r--   0 julioj.melero   (501) staff       (20)     5175 2023-05-18 08:35:35.000000 Orange3-Tools-0.0.3/orangecontrib/tools/widgets/owcorrelogram.py
+-rw-r--r--   0 julioj.melero   (501) staff       (20)    30238 2023-05-19 17:23:52.000000 Orange3-Tools-0.0.3/orangecontrib/tools/widgets/owsarima.py
+-rw-r--r--   0 julioj.melero   (501) staff       (20)     9715 2023-05-20 10:50:09.000000 Orange3-Tools-0.0.3/orangecontrib/tools/widgets/owstationarity.py
+-rw-r--r--   0 julioj.melero   (501) staff       (20)     2212 2023-04-13 16:39:56.000000 Orange3-Tools-0.0.3/orangecontrib/tools/widgets/utils.py
+-rw-r--r--   0 julioj.melero   (501) staff       (20)       38 2023-05-20 10:52:20.148330 Orange3-Tools-0.0.3/setup.cfg
+-rw-rw-rw-   0 julioj.melero   (501) staff       (20)     3576 2023-05-20 10:51:09.000000 Orange3-Tools-0.0.3/setup.py
```

### Comparing `Orange3-Tools-0.0.2/LICENSE` & `Orange3-Tools-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.2/Orange3_Tools.egg-info/SOURCES.txt` & `Orange3-Tools-0.0.3/Orange3_Tools.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -7,22 +7,21 @@
 Orange3_Tools.egg-info/entry_points.txt
 Orange3_Tools.egg-info/not-zip-safe
 Orange3_Tools.egg-info/requires.txt
 Orange3_Tools.egg-info/top_level.txt
 orangecontrib/__init__.py
 orangecontrib/functions.py
 orangecontrib/tools/__init__.py
-orangecontrib/tools/widgets/Barplot.py
-orangecontrib/tools/widgets/Linesplot.py
 orangecontrib/tools/widgets/MySqlOrange.py
 orangecontrib/tools/widgets/Pairsplot.py
 orangecontrib/tools/widgets/Scatterplot.py
 orangecontrib/tools/widgets/__init__.py
 orangecontrib/tools/widgets/owcorrelogram.py
 orangecontrib/tools/widgets/owsarima.py
+orangecontrib/tools/widgets/owstationarity.py
 orangecontrib/tools/widgets/utils.py
 orangecontrib/tools/widgets/icons/ARIMA.svg
 orangecontrib/tools/widgets/icons/Barchart.svg
 orangecontrib/tools/widgets/icons/Correlogram.svg
 orangecontrib/tools/widgets/icons/Pairs.svg
 orangecontrib/tools/widgets/icons/Simple_scatterplot.svg
 orangecontrib/tools/widgets/icons/category.svg
```

### Comparing `Orange3-Tools-0.0.2/orangecontrib/functions.py` & `Orange3-Tools-0.0.3/orangecontrib/functions.py`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.2/orangecontrib/tools/__init__.py` & `Orange3-Tools-0.0.3/orangecontrib/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.2/orangecontrib/tools/widgets/Barplot.py` & `Orange3-Tools-0.0.3/orangecontrib/tools/widgets/Scatterplot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,68 +1,65 @@
 import Orange.data
 import numpy as np
 import seaborn as sns
-
 from AnyQt.QtCore import Qt
-
 from orangewidget import gui
 from Orange.widgets.widget import OWWidget, Msg, Input
 from Orange.widgets import settings
 from Orange.widgets.utils.itemmodels import DomainModel
 from Orange.preprocess.preprocess import Normalize
 from Orange.data.pandas_compat import  table_to_frame
 from Orange.data import Table, Domain, ContinuousVariable
 from orangecontrib.tools.widgets.utils import MatplotlibWidget
 
-
-class Barplot1(OWWidget):
-    name = 'Bar plot'
-    description = 'Bar plot with some tunning features'
-    icon = 'icons/Barchart.svg'
+class Scaterplot(OWWidget):
+    # Nombre del widget como se verá en el lienzo
+    name = 'Scater plot'
+    description = 'Scater plot with some tunning features'
+    icon = 'icons/sscater.svg'
     keywords = ["widget", "tools"]
     category = 'Tools'
-    priority = 15
 
     class Inputs:
         data = Input("Data", Table)
 
-    #    class Outputs:
-    #        sample = Output("Sampled Data", Orange.data.Table)
+    class Outputs:
+        sample = None #Output("Sampled Data", Orange.data.Table)
 
     graph_name = "graph"  # QGraphicsView (pg.PlotWidget)
     settingsHandler = settings.DomainContextHandler(
         match_values=settings.DomainContextHandler.MATCH_VALUES_CLASS)
     attr_x = settings.ContextSetting(None)
     attr_y = settings.ContextSetting(None)
-
     attr_size = settings.Setting(5)
     key_size = settings.Setting(5)
     attr_col = settings.ContextSetting('b')
     key_col = settings.ContextSetting('Blue')
     attr_sym = settings.Setting('o')
     key_sym = settings.Setting('Circle')
     axes = None
 
     default_background_color = np.array([0, 0xbf, 0xff])
 
     SYMBOL_TYPES = (
         ('Circle', 'o'),
         ('Square', 's'),
-        ('Triangle', 't'),
-        ('Diamond', 'd'),
-        ('Plus', '+'),
-        ('Cross', 'x'),
+        ('Triangle', 'v'),
+        ('Diamond', 'D'),
+        ('Plus', 'P'),
+        ('Cross', 'X'),
     )
     COLOR_NAMES = (
         ('Blue', 'b'),
         ('Red', 'r'),
         ('Green', 'g'),
         ('Cyan', 'c'),
         ('Yellow', 'y'),
         ('Magenta', 'm'),
+        ('Black','k')
     )
 
     class Error(OWWidget.Error):
         num_features = Msg("Data must contain at least {}.")
         no_class = Msg("Data must have a single target variable.")
         no_class_values = Msg("Target variable must have at least two values.")
         no_nonnan_data = Msg("No points with defined values.")
@@ -70,35 +67,32 @@
 
     def __init__(self):
         super().__init__()
         self.data = None
         self.selected_data = None
         self.min_x = self.max_x = self.min_y = self.max_y = None
         self._add_graph()
-
         self.var_model = DomainModel(valid_types=ContinuousVariable,
                                      order=DomainModel.ATTRIBUTES)
         self.options_box = gui.widgetBox(self.controlArea, "Variables")
         opts = dict(
             widget=self.options_box, master=self, orientation=Qt.Horizontal,
             callback=self.change_attributes)
         gui.comboBox(value='attr_x', model=self.var_model, **opts)
         gui.comboBox(value='attr_y', model=self.var_model, **opts)
-
         self.parameters_box = gui.widgetBox(self.controlArea, "Parameters")
         opts1 = dict(
             widget=self.parameters_box, master=self, orientation=Qt.Horizontal,
             callback=self.change_parameters, sendSelectedValue=True, contentsLength=14)
         gui.comboBox(value='key_sym', label='Symbol',
                      items=[i[0] for i in self.SYMBOL_TYPES], **opts1)
         gui.comboBox(value='key_col', label='Color',
                      items=[i[0] for i in self.COLOR_NAMES], **opts1)
         gui.spin(widget=self.parameters_box, master=self, value='attr_size', minv=1, maxv=30, step=1, label="Size:",
                  alignment=Qt.AlignRight, controlWidth=80, callback=self.change_parameters)
-
         gui.rubber(self.controlArea)
 
     def change_parameters(self):
         self.attr_sym = dict(self.SYMBOL_TYPES)[self.key_sym]
         self.attr_col = dict(self.COLOR_NAMES)[self.key_col]
         self.restart()
 
@@ -112,14 +106,22 @@
     def restart(self):
         self.clear_plot()
         self.select_columns()
         if self.selected_data is None:
             return
         self.replot()
 
+    #def keyPressEvent(self, e):
+    #    """Bind 'back' key to step back"""
+    #    if (e.modifiers(), e.key()) in self.key_actions:
+    #        fun = self.key_actions[(e.modifiers(), e.key())]
+    #        fun(self)
+    #    else:
+    #        super().keyPressEvent(e)
+
     def resizeEvent(self, event):
         self.restart()
 
     ##############################
     # Signals and data-handling
 
     @Inputs.data
@@ -143,15 +145,14 @@
 
         self.data = data
         self.attr_x = self.var_model[0]
         self.attr_y = self.var_model[1]
         self.openContext(self.data)
         self.restart()
 
-    @property
 
     def select_columns(self):
         self.Error.no_nonnan_data.clear()
         self.Error.same_variable.clear()
         self.selected_data = None
         if self.data is None:
             return
@@ -169,15 +170,16 @@
             )
 
         if not valid_data.size:
             self.Error.no_nonnan_data()
             return
 
         data = data[valid_data]
-        self.selected_data = data
+        self.selected_data=data
+
 
     def send_report(self):
         if self.data is None:
             return
         self.report_plot()
 
     ##############################
@@ -211,8 +213,9 @@
             f"<b>Step {step}:</b><br/>" \
             f"{x:.3f}, {y:.3f}<br/>" \
             f"Cost: {self.learner.j(np.array([x, y])):.5f}"
 
 
 if __name__ == '__main__':
     from Orange.widgets.utils.widgetpreview import WidgetPreview  # since Orange 3.20.0
+
     WidgetPreview(Scaterplot).run(Orange.data.Table("iris"))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Orange3-Tools-0.0.2/orangecontrib/tools/widgets/Linesplot.py` & `Orange3-Tools-0.0.3/orangecontrib/tools/widgets/Pairsplot.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,65 +1,78 @@
 import Orange.data
 import numpy as np
+import pandas as pd
 import seaborn as sns
 from AnyQt.QtCore import Qt
 from orangewidget import gui
 from Orange.widgets.widget import OWWidget, Msg, Input
 from Orange.widgets import settings
 from Orange.widgets.utils.itemmodels import DomainModel
 from Orange.preprocess.preprocess import Normalize
 from Orange.data.pandas_compat import  table_to_frame
 from Orange.data import Table, Domain, ContinuousVariable
 from orangecontrib.tools.widgets.utils import MatplotlibWidget
 
-class Linesplot(OWWidget):
+class Pairsplot(OWWidget):
     # Nombre del widget como se verá en el lienzo
-    name = 'Lines plot'
-    description = 'Lines plot with some tunning features'
-    icon = 'icons/sscater.svg'
+    name = 'Pairs plot'
+    description = 'Pairs plot with some tunning features'
+    icon = 'icons/Pairs.svg'
     keywords = ["widget", "tools"]
     category = 'Tools'
 
     class Inputs:
         data = Input("Data", Table)
 
     class Outputs:
         sample = None #Output("Sampled Data", Orange.data.Table)
 
     graph_name = "graph"  # QGraphicsView (pg.PlotWidget)
     settingsHandler = settings.DomainContextHandler(
         match_values=settings.DomainContextHandler.MATCH_VALUES_CLASS)
+    attr_numvars=settings.ContextSetting(None)
     attr_x = settings.ContextSetting(None)
     attr_y = settings.ContextSetting(None)
-    attr_size = settings.Setting(5)
-    key_size = settings.Setting(5)
+    attr_size = settings.Setting(1)
+    key_size = settings.Setting(1)
     attr_col = settings.ContextSetting('b')
     key_col = settings.ContextSetting('Blue')
     attr_sym = settings.Setting('o')
     key_sym = settings.Setting('Circle')
+    attr_bins = settings.Setting(10)
+    key_bins = settings.Setting(10)
     axes = None
 
     default_background_color = np.array([0, 0xbf, 0xff])
 
     SYMBOL_TYPES = (
         ('Circle', 'o'),
         ('Square', 's'),
-        ('Triangle', 't'),
-        ('Diamond', 'd'),
-        ('Plus', '+'),
-        ('Cross', 'x'),
+        ('Triangle', 'v'),
+        ('Diamond', 'D'),
+        ('Plus', 'P'),
+        ('Cross', 'X'),
     )
     COLOR_NAMES = (
         ('Blue', 'b'),
         ('Red', 'r'),
         ('Green', 'g'),
         ('Cyan', 'c'),
         ('Yellow', 'y'),
         ('Magenta', 'm'),
+        ('Black','k')
     )
+    def resizeEvent(self,e):
+        #if not self._flag:
+        #    self._flag = True
+        #    self.scale_image()
+        #    QtCore.QTimer.singleShot(50, lambda: setattr(self,"_flag",False))
+        #super().resizeEvent(e)
+        self.restart()
+
 
     class Error(OWWidget.Error):
         num_features = Msg("Data must contain at least {}.")
         no_class = Msg("Data must have a single target variable.")
         no_class_values = Msg("Target variable must have at least two values.")
         no_nonnan_data = Msg("No points with defined values.")
         same_variable = Msg("Select two different variables.")
@@ -68,32 +81,31 @@
         super().__init__()
         self.data = None
         self.selected_data = None
         self.min_x = self.max_x = self.min_y = self.max_y = None
         self._add_graph()
         self.var_model = DomainModel(valid_types=ContinuousVariable,
                                      order=DomainModel.ATTRIBUTES)
-        self.options_box = gui.widgetBox(self.controlArea, "Variables")
-        opts = dict(
-            widget=self.options_box, master=self, orientation=Qt.Horizontal,
-            callback=self.change_attributes)
-        gui.comboBox(value='attr_x', model=self.var_model, **opts)
-        gui.comboBox(value='attr_y', model=self.var_model, **opts)
+        self.attr_numvars=len(self.var_model)
         self.parameters_box = gui.widgetBox(self.controlArea, "Parameters")
         opts1 = dict(
             widget=self.parameters_box, master=self, orientation=Qt.Horizontal,
             callback=self.change_parameters, sendSelectedValue=True, contentsLength=14)
-        gui.comboBox(value='key_sym', label='Symbol',
+        gui.comboBox(value='key_sym', label='Plot Symbol',
                      items=[i[0] for i in self.SYMBOL_TYPES], **opts1)
         gui.comboBox(value='key_col', label='Color',
                      items=[i[0] for i in self.COLOR_NAMES], **opts1)
-        gui.spin(widget=self.parameters_box, master=self, value='attr_size', minv=1, maxv=30, step=1, label="Size:",
+        gui.spin(widget=self.parameters_box, master=self, value='attr_size', minv=1, maxv=30, step=1, label="Symbol Size:",
                  alignment=Qt.AlignRight, controlWidth=80, callback=self.change_parameters)
+        gui.spin(widget=self.parameters_box, master=self, value='attr_bins', minv=2, maxv=500, step=1, label="Histogram Bins:",
+                 alignment=Qt.AlignRight, controlWidth=80, callback=self.change_parameters)
+
         gui.rubber(self.controlArea)
 
+
     def change_parameters(self):
         self.attr_sym = dict(self.SYMBOL_TYPES)[self.key_sym]
         self.attr_col = dict(self.COLOR_NAMES)[self.key_col]
         self.restart()
 
     def _add_graph(self):
         self.graph = MatplotlibWidget()
@@ -105,16 +117,24 @@
     def restart(self):
         self.clear_plot()
         self.select_columns()
         if self.selected_data is None:
             return
         self.replot()
 
-     def resizeEvent(self, event):
-        self.restart()
+    #def keyPressEvent(self, e):
+    #    """Bind 'back' key to step back"""
+    #    if (e.modifiers(), e.key()) in self.key_actions:
+    #        fun = self.key_actions[(e.modifiers(), e.key())]
+    #        fun(self)
+    #    else:
+    #        super().keyPressEvent(e)
+
+    #def resizeEvent(self, event):
+    #    self.restart()
 
     ##############################
     # Signals and data-handling
 
     @Inputs.data
     def set_data(self, data):
 
@@ -134,14 +154,15 @@
             self.var_model.set_domain(None)
             return
 
         self.data = data
         self.attr_x = self.var_model[0]
         self.attr_y = self.var_model[1]
         self.openContext(self.data)
+        self.attr_numvars=len(self.var_model)
         self.restart()
 
 
     def select_columns(self):
         self.Error.no_nonnan_data.clear()
         self.Error.same_variable.clear()
         self.selected_data = None
@@ -164,49 +185,90 @@
             self.Error.no_nonnan_data()
             return
 
         data = data[valid_data]
         self.selected_data=data
 
 
+
     def send_report(self):
         if self.data is None:
             return
         self.report_plot()
 
     ##############################
     # Plot-related methods
 
     def clear_plot(self):
         self.graph.getFigure().clf()
 
+
     def replot(self):
         if self.data is None or self.selected_data is None:
             self.clear_plot()
             return
         self.plot()
 
     def plot(self):
+        sns.set()
         self.graph.getFigure().clf()
         data = table_to_frame(self.data, include_metas=True)
-        x = self.selected_data.domain[0].name
-        y = self.selected_data.domain[1].name
-        sns.set()
-        self.axes = self.graph.getFigure().add_subplot(111)
-        self.axes.plot(data[x], data[y], marker=self.attr_sym, color=self.attr_col, markersize=self.attr_size,
-                       linestyle='None')
-        self.graph.getFigure().supxlabel(x)
-        self.graph.getFigure().supylabel(y)
-        self.graph.getFigure().tight_layout()
+
+        # A layout of nxn subplots where n= self.attr_numvars. For efficiency, maximum n=5, discard the others.
+        n = self.attr_numvars
+        if n>5:
+            n=5
+        #fig, axes = plt.subplots(4, 4, figsize=(12, 8), sharex="col", tight_layout=True)
+        self.graph.axes = self.graph.getFigure().subplots(n, n, sharex="col")
+
+        for i in range(n):
+            for j in range(n):
+                # If this is the lower-triangule, add a scatterlpot for each group.
+                if i > j:
+                    x=data[self.data.domain.attributes[i].name]
+                    y=data[self.data.domain.attributes[j].name]
+                    self.graph.axes[i,j].plot(x,y, marker=self.attr_sym, color=self.attr_col,markersize=self.attr_size,linestyle='None')
+                else:
+                    if i < j:
+                        # Remove axis and grid
+                        self.graph.axes[i, j].grid(False)
+                        self.graph.axes[i, j].axis('off')
+                        # Add correlation coefficient
+                        x = data[self.data.domain.attributes[i].name]
+                        y = data[self.data.domain.attributes[j].name]
+                        correlation = np.corrcoef(x, y)[0, 1]
+                        cor = 'Correlation coefficient:\n {:.4f}'.format(correlation)
+                        left, width = .25, .5
+                        bottom, height = .25, .5
+                        right = left + width
+                        top = bottom + height
+                        self.graph.axes[i, j].text(0.5 * (left + right), 0.5 * (bottom + top), cor,
+                                                   horizontalalignment='center',
+                                                   verticalalignment='center',
+                                                   transform=self.graph.axes[i, j].transAxes)
+                    else:
+                       # If this is the main diagonal, add histograms
+                         x=data[self.data.domain.attributes[i].name]
+                         self.graph.axes[i,j].hist(x,color=self.attr_col, bins=self.attr_bins, alpha=0.5)
+                if j == 0:
+                    self.graph.axes[i,j].set_ylabel(self.data.domain.attributes[i].name)
+                if i == (n-1):
+                    self.graph.axes[i,j].set_xlabel(self.data.domain.attributes[j].name)
+
+
+
+#        self.graph.getFigure().tight_layout()
         self.graph.draw()
 
     def _format_label(self, x, y, step):
         return \
             f"<b>Step {step}:</b><br/>" \
             f"{x:.3f}, {y:.3f}<br/>" \
             f"Cost: {self.learner.j(np.array([x, y])):.5f}"
 
 
 if __name__ == '__main__':
     from Orange.widgets.utils.widgetpreview import WidgetPreview  # since Orange 3.20.0
+    file = pd.read_csv('../datasets/auto-mpg.csv')
+    #WidgetPreview(Pairsplot).run(Orange.data.Table(file))
 
-    WidgetPreview(Linesplot).run(Orange.data.Table("iris"))
+    WidgetPreview(Pairsplot).run(Orange.data.Table("iris"))
```

### Comparing `Orange3-Tools-0.0.2/orangecontrib/tools/widgets/MySqlOrange.py` & `Orange3-Tools-0.0.3/orangecontrib/tools/widgets/MySqlOrange.py`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.2/orangecontrib/tools/widgets/__init__.py` & `Orange3-Tools-0.0.3/orangecontrib/tools/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.2/orangecontrib/tools/widgets/icons/ARIMA.svg` & `Orange3-Tools-0.0.3/orangecontrib/tools/widgets/icons/ARIMA.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.2/orangecontrib/tools/widgets/icons/Barchart.svg` & `Orange3-Tools-0.0.3/orangecontrib/tools/widgets/icons/Barchart.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.2/orangecontrib/tools/widgets/icons/Correlogram.svg` & `Orange3-Tools-0.0.3/orangecontrib/tools/widgets/icons/Correlogram.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.2/orangecontrib/tools/widgets/icons/Pairs.svg` & `Orange3-Tools-0.0.3/orangecontrib/tools/widgets/icons/Pairs.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.2/orangecontrib/tools/widgets/icons/Simple_scatterplot.svg` & `Orange3-Tools-0.0.3/orangecontrib/tools/widgets/icons/Simple_scatterplot.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.2/orangecontrib/tools/widgets/icons/category.svg` & `Orange3-Tools-0.0.3/orangecontrib/tools/widgets/icons/category.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.2/orangecontrib/tools/widgets/icons/mysql-orange.svg` & `Orange3-Tools-0.0.3/orangecontrib/tools/widgets/icons/mysql-orange.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.2/orangecontrib/tools/widgets/icons/sscater.svg` & `Orange3-Tools-0.0.3/orangecontrib/tools/widgets/icons/sscater.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.2/orangecontrib/tools/widgets/owcorrelogram.py` & `Orange3-Tools-0.0.3/orangecontrib/tools/widgets/owcorrelogram.py`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.2/orangecontrib/tools/widgets/owsarima.py` & `Orange3-Tools-0.0.3/orangecontrib/tools/widgets/owsarima.py`

 * *Files 0% similar despite different names*

```diff
@@ -817,8 +817,8 @@
         return ARIMA((self.p, self.d, self.q),(self.s_p,self.s_d,self.s_q,self.s_s), self.exog_data is not None)
 
 
 if __name__ == "__main__":
     data = TS.from_file('airpassengers')
     domain = Domain(data.domain.attributes[:-1], data.domain.attributes[-1])
     data = Timeseries.from_numpy(domain, data.X[:, :-1], data.X[:, -1])
-    WidgetPreview(OWSARIMAModel).run(set_data=data)
+    WidgetPreview(OWSARIMAModel).run(data)
```

### Comparing `Orange3-Tools-0.0.2/orangecontrib/tools/widgets/utils.py` & `Orange3-Tools-0.0.3/orangecontrib/tools/widgets/utils.py`

 * *Files identical despite different names*

### Comparing `Orange3-Tools-0.0.2/setup.py` & `Orange3-Tools-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from os import path, walk
 from setuptools import setup, find_packages
 from setuptools.dist import Distribution
 
 NAME = "Orange3-Tools"
 
-VERSION = "0.0.2"
+VERSION = "0.0.3"
 
 DESCRIPTION = "Tools para Asignatura Big Data Master EERR"
 LONG_DESCRIPTION = ""
 
 LICENSE = "GPL-3.0"
 
 KEYWORDS = (
```

