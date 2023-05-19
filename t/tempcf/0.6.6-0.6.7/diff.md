# Comparing `tmp/tempcf-0.6.6.tar.gz` & `tmp/tempcf-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\tempcf-0.6.6.tar", last modified: Fri May 19 22:12:28 2023, max compression
+gzip compressed data, was "dist\tempcf-0.6.7.tar", last modified: Fri May 19 22:17:07 2023, max compression
```

## Comparing `tempcf-0.6.6.tar` & `tempcf-0.6.7.tar`

### file list

```diff
@@ -1,42 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 22:12:28.412123 tempcf-0.6.6/
--rw-rw-rw-   0        0        0     3079 2023-05-19 22:12:28.409125 tempcf-0.6.6/PKG-INFO
--rw-rw-rw-   0        0        0     2146 2023-05-15 20:26:54.000000 tempcf-0.6.6/README.md
--rw-rw-rw-   0        0        0       42 2023-05-19 22:12:28.416127 tempcf-0.6.6/setup.cfg
--rw-rw-rw-   0        0        0     1379 2023-05-19 19:46:56.000000 tempcf-0.6.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-19 22:12:28.149694 tempcf-0.6.6/tempcf/
--rw-rw-rw-   0        0        0     2001 2023-02-20 22:21:11.000000 tempcf-0.6.6/tempcf/AboutDialog.py
--rw-rw-rw-   0        0        0     1317 2023-02-20 22:21:11.000000 tempcf-0.6.6/tempcf/ActionLogger.py
--rw-rw-rw-   0        0        0     7960 2023-03-16 21:24:19.000000 tempcf-0.6.6/tempcf/Dataframe.py
--rw-rw-rw-   0        0        0     2331 2023-02-20 22:21:11.000000 tempcf-0.6.6/tempcf/DatasetMetadata.py
--rw-rw-rw-   0        0        0     2651 2023-02-20 22:21:11.000000 tempcf-0.6.6/tempcf/DepthConfigure.py
--rw-rw-rw-   0        0        0     1154 2023-02-20 22:21:11.000000 tempcf-0.6.6/tempcf/EntryValidation.py
--rw-rw-rw-   0        0        0     6759 2023-05-19 17:57:12.000000 tempcf-0.6.6/tempcf/ExportType.py
--rw-rw-rw-   0        0        0      654 2023-03-16 21:24:19.000000 tempcf-0.6.6/tempcf/FileTypes.py
--rw-rw-rw-   0        0        0     3787 2023-03-16 16:46:32.000000 tempcf-0.6.6/tempcf/FilterConfigure.py
--rw-rw-rw-   0        0        0     1117 2023-02-20 22:21:11.000000 tempcf-0.6.6/tempcf/FilterContainer.py
--rw-rw-rw-   0        0        0     2781 2023-02-20 22:21:11.000000 tempcf-0.6.6/tempcf/FilterControl.py
--rw-rw-rw-   0        0        0     6212 2023-02-20 22:21:11.000000 tempcf-0.6.6/tempcf/FilterList.py
--rw-rw-rw-   0        0        0     3037 2023-05-19 19:48:13.000000 tempcf-0.6.6/tempcf/Filters.py
--rw-rw-rw-   0        0        0     7019 2023-02-20 22:21:11.000000 tempcf-0.6.6/tempcf/GraphView.py
--rw-rw-rw-   0        0        0     1520 2023-02-20 22:21:11.000000 tempcf-0.6.6/tempcf/HelpDialog.py
--rw-rw-rw-   0        0        0     4189 2023-03-16 21:24:19.000000 tempcf-0.6.6/tempcf/ImportType.py
--rw-rw-rw-   0        0        0     2928 2023-01-10 23:09:24.000000 tempcf-0.6.6/tempcf/LogParser.py
--rw-rw-rw-   0        0        0    10144 2023-03-16 21:24:19.000000 tempcf-0.6.6/tempcf/MainToolbar.py
--rw-rw-rw-   0        0        0      953 2023-02-20 22:21:11.000000 tempcf-0.6.6/tempcf/MetadataDialog.py
--rw-rw-rw-   0        0        0     4909 2023-02-20 22:21:11.000000 tempcf-0.6.6/tempcf/MetadataInputDialog.py
--rw-rw-rw-   0        0        0      687 2020-10-09 19:00:27.000000 tempcf-0.6.6/tempcf/Observable.py
--rw-rw-rw-   0        0        0      346 2023-02-20 22:21:11.000000 tempcf-0.6.6/tempcf/PopoutDialog.py
--rw-rw-rw-   0        0        0     1565 2023-02-20 22:21:11.000000 tempcf-0.6.6/tempcf/ScrollableFrame.py
--rw-rw-rw-   0        0        0     1781 2023-02-20 22:21:11.000000 tempcf-0.6.6/tempcf/TimeZoneConfigure.py
--rw-rw-rw-   0        0        0     1254 2023-01-13 18:53:29.000000 tempcf-0.6.6/tempcf/ToolTip.py
--rw-rw-rw-   0        0        0      485 2020-10-16 15:50:08.000000 tempcf-0.6.6/tempcf/Utils.py
--rw-rw-rw-   0        0        0       23 2023-05-19 21:58:43.000000 tempcf-0.6.6/tempcf/_version.py
--rw-rw-rw-   0        0        0    16042 2023-03-16 16:46:32.000000 tempcf-0.6.6/tempcf/main.py
--rw-rw-rw-   0        0        0     3319 2023-02-09 04:41:43.000000 tempcf-0.6.6/tempcf/tester.py
-drwxrwxrwx   0        0        0        0 2023-05-19 22:12:28.375127 tempcf-0.6.6/tempcf.egg-info/
--rw-rw-rw-   0        0        0     3079 2023-05-19 22:12:25.000000 tempcf-0.6.6/tempcf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      840 2023-05-19 22:12:26.000000 tempcf-0.6.6/tempcf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 22:12:25.000000 tempcf-0.6.6/tempcf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-05-19 22:12:25.000000 tempcf-0.6.6/tempcf.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       53 2023-05-19 22:12:25.000000 tempcf-0.6.6/tempcf.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-19 22:12:25.000000 tempcf-0.6.6/tempcf.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 22:17:07.633167 tempcf-0.6.7/
+-rw-rw-rw-   0        0        0     3079 2023-05-19 22:17:07.628164 tempcf-0.6.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2146 2023-05-15 20:26:54.000000 tempcf-0.6.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-19 22:17:07.635167 tempcf-0.6.7/setup.cfg
+-rw-rw-rw-   0        0        0     1382 2023-05-19 22:16:25.000000 tempcf-0.6.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 22:17:07.320180 tempcf-0.6.7/tempcf/
+-rw-rw-rw-   0        0        0     2001 2023-02-20 22:21:11.000000 tempcf-0.6.7/tempcf/AboutDialog.py
+-rw-rw-rw-   0        0        0     1317 2023-02-20 22:21:11.000000 tempcf-0.6.7/tempcf/ActionLogger.py
+-rw-rw-rw-   0        0        0     7960 2023-03-16 21:24:19.000000 tempcf-0.6.7/tempcf/Dataframe.py
+-rw-rw-rw-   0        0        0     2331 2023-02-20 22:21:11.000000 tempcf-0.6.7/tempcf/DatasetMetadata.py
+-rw-rw-rw-   0        0        0     2651 2023-02-20 22:21:11.000000 tempcf-0.6.7/tempcf/DepthConfigure.py
+-rw-rw-rw-   0        0        0     1154 2023-02-20 22:21:11.000000 tempcf-0.6.7/tempcf/EntryValidation.py
+-rw-rw-rw-   0        0        0     6759 2023-05-19 17:57:12.000000 tempcf-0.6.7/tempcf/ExportType.py
+-rw-rw-rw-   0        0        0      654 2023-03-16 21:24:19.000000 tempcf-0.6.7/tempcf/FileTypes.py
+-rw-rw-rw-   0        0        0     3787 2023-03-16 16:46:32.000000 tempcf-0.6.7/tempcf/FilterConfigure.py
+-rw-rw-rw-   0        0        0     1117 2023-02-20 22:21:11.000000 tempcf-0.6.7/tempcf/FilterContainer.py
+-rw-rw-rw-   0        0        0     2781 2023-02-20 22:21:11.000000 tempcf-0.6.7/tempcf/FilterControl.py
+-rw-rw-rw-   0        0        0     6212 2023-02-20 22:21:11.000000 tempcf-0.6.7/tempcf/FilterList.py
+-rw-rw-rw-   0        0        0     3037 2023-05-19 19:48:13.000000 tempcf-0.6.7/tempcf/Filters.py
+-rw-rw-rw-   0        0        0     7019 2023-02-20 22:21:11.000000 tempcf-0.6.7/tempcf/GraphView.py
+-rw-rw-rw-   0        0        0     1520 2023-02-20 22:21:11.000000 tempcf-0.6.7/tempcf/HelpDialog.py
+-rw-rw-rw-   0        0        0     4189 2023-03-16 21:24:19.000000 tempcf-0.6.7/tempcf/ImportType.py
+-rw-rw-rw-   0        0        0     2928 2023-01-10 23:09:24.000000 tempcf-0.6.7/tempcf/LogParser.py
+-rw-rw-rw-   0        0        0    10144 2023-03-16 21:24:19.000000 tempcf-0.6.7/tempcf/MainToolbar.py
+-rw-rw-rw-   0        0        0      953 2023-02-20 22:21:11.000000 tempcf-0.6.7/tempcf/MetadataDialog.py
+-rw-rw-rw-   0        0        0     4909 2023-02-20 22:21:11.000000 tempcf-0.6.7/tempcf/MetadataInputDialog.py
+-rw-rw-rw-   0        0        0      687 2020-10-09 19:00:27.000000 tempcf-0.6.7/tempcf/Observable.py
+-rw-rw-rw-   0        0        0      346 2023-02-20 22:21:11.000000 tempcf-0.6.7/tempcf/PopoutDialog.py
+-rw-rw-rw-   0        0        0     1565 2023-02-20 22:21:11.000000 tempcf-0.6.7/tempcf/ScrollableFrame.py
+-rw-rw-rw-   0        0        0     1781 2023-02-20 22:21:11.000000 tempcf-0.6.7/tempcf/TimeZoneConfigure.py
+-rw-rw-rw-   0        0        0     1254 2023-01-13 18:53:29.000000 tempcf-0.6.7/tempcf/ToolTip.py
+-rw-rw-rw-   0        0        0      485 2020-10-16 15:50:08.000000 tempcf-0.6.7/tempcf/Utils.py
+-rw-rw-rw-   0        0        0       23 2023-05-19 22:16:38.000000 tempcf-0.6.7/tempcf/_version.py
+drwxrwxrwx   0        0        0        0 2023-05-19 22:17:07.618177 tempcf-0.6.7/tempcf/assets/
+-rw-rw-rw-   0        0        0   277135 2020-12-11 16:52:50.000000 tempcf-0.6.7/tempcf/assets/demo_FG2.txt
+-rw-rw-rw-   0        0        0   563867 2020-12-11 16:52:50.000000 tempcf-0.6.7/tempcf/assets/demo_GP5W.txt
+-rw-rw-rw-   0        0        0     5694 2020-10-13 20:52:35.000000 tempcf-0.6.7/tempcf/assets/permafrostnet_logo.ico
+-rw-rw-rw-   0        0        0    17858 2020-11-16 15:50:16.000000 tempcf-0.6.7/tempcf/assets/permafrostnet_logo_text.png
+-rw-rw-rw-   0        0        0    16042 2023-03-16 16:46:32.000000 tempcf-0.6.7/tempcf/main.py
+-rw-rw-rw-   0        0        0     3319 2023-02-09 04:41:43.000000 tempcf-0.6.7/tempcf/tester.py
+drwxrwxrwx   0        0        0        0 2023-05-19 22:17:07.499190 tempcf-0.6.7/tempcf.egg-info/
+-rw-rw-rw-   0        0        0     3079 2023-05-19 22:17:05.000000 tempcf-0.6.7/tempcf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      974 2023-05-19 22:17:06.000000 tempcf-0.6.7/tempcf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 22:17:05.000000 tempcf-0.6.7/tempcf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-05-19 22:17:05.000000 tempcf-0.6.7/tempcf.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       53 2023-05-19 22:17:05.000000 tempcf-0.6.7/tempcf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-19 22:17:05.000000 tempcf-0.6.7/tempcf.egg-info/top_level.txt
```

### Comparing `tempcf-0.6.6/PKG-INFO` & `tempcf-0.6.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tempcf
-Version: 0.6.6
+Version: 0.6.7
 Summary: A toolbox for flagging and cleaning ground temperature data
 Home-page: UNKNOWN
 Author: Nick Brown
 Author-email: 
 License: UNKNOWN
 Project-URL: Source, https://gitlab.com/permafrostnet/permafrost-tempcf
 Project-URL: Documentation, https://permafrostnet.gitlab.io/permafrost-tempcf/
```

### Comparing `tempcf-0.6.6/README.md` & `tempcf-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `tempcf-0.6.6/setup.py` & `tempcf-0.6.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     classifiers=[
         'Development Status :: 4 - Beta',
     ],
 
     # Packages and depencies
     packages=['tempcf'],
 
-    package_data={'tsp': ['assets/*']},
+    package_data={'tempcf': ['assets/*']},
 
     install_requires=[
         'numpy',  # ==1.19.3',
         'matplotlib',  # ==3.2.2',
         'tsp>=1.5.0',
         'pfit',
         'pandas',
```

### Comparing `tempcf-0.6.6/tempcf/AboutDialog.py` & `tempcf-0.6.7/tempcf/AboutDialog.py`

 * *Files identical despite different names*

### Comparing `tempcf-0.6.6/tempcf/ActionLogger.py` & `tempcf-0.6.7/tempcf/ActionLogger.py`

 * *Files identical despite different names*

### Comparing `tempcf-0.6.6/tempcf/Dataframe.py` & `tempcf-0.6.7/tempcf/Dataframe.py`

 * *Files identical despite different names*

### Comparing `tempcf-0.6.6/tempcf/DatasetMetadata.py` & `tempcf-0.6.7/tempcf/DatasetMetadata.py`

 * *Files identical despite different names*

### Comparing `tempcf-0.6.6/tempcf/DepthConfigure.py` & `tempcf-0.6.7/tempcf/DepthConfigure.py`

 * *Files identical despite different names*

### Comparing `tempcf-0.6.6/tempcf/EntryValidation.py` & `tempcf-0.6.7/tempcf/EntryValidation.py`

 * *Files identical despite different names*

### Comparing `tempcf-0.6.6/tempcf/ExportType.py` & `tempcf-0.6.7/tempcf/ExportType.py`

 * *Files identical despite different names*

### Comparing `tempcf-0.6.6/tempcf/FileTypes.py` & `tempcf-0.6.7/tempcf/FileTypes.py`

 * *Files identical despite different names*

### Comparing `tempcf-0.6.6/tempcf/FilterConfigure.py` & `tempcf-0.6.7/tempcf/FilterConfigure.py`

 * *Files identical despite different names*

### Comparing `tempcf-0.6.6/tempcf/FilterContainer.py` & `tempcf-0.6.7/tempcf/FilterContainer.py`

 * *Files identical despite different names*

### Comparing `tempcf-0.6.6/tempcf/FilterControl.py` & `tempcf-0.6.7/tempcf/FilterControl.py`

 * *Files identical despite different names*

### Comparing `tempcf-0.6.6/tempcf/FilterList.py` & `tempcf-0.6.7/tempcf/FilterList.py`

 * *Files identical despite different names*

### Comparing `tempcf-0.6.6/tempcf/Filters.py` & `tempcf-0.6.7/tempcf/Filters.py`

 * *Files identical despite different names*

### Comparing `tempcf-0.6.6/tempcf/GraphView.py` & `tempcf-0.6.7/tempcf/GraphView.py`

 * *Files identical despite different names*

### Comparing `tempcf-0.6.6/tempcf/HelpDialog.py` & `tempcf-0.6.7/tempcf/HelpDialog.py`

 * *Files identical despite different names*

### Comparing `tempcf-0.6.6/tempcf/ImportType.py` & `tempcf-0.6.7/tempcf/ImportType.py`

 * *Files identical despite different names*

### Comparing `tempcf-0.6.6/tempcf/LogParser.py` & `tempcf-0.6.7/tempcf/LogParser.py`

 * *Files identical despite different names*

### Comparing `tempcf-0.6.6/tempcf/MainToolbar.py` & `tempcf-0.6.7/tempcf/MainToolbar.py`

 * *Files identical despite different names*

### Comparing `tempcf-0.6.6/tempcf/MetadataDialog.py` & `tempcf-0.6.7/tempcf/MetadataDialog.py`

 * *Files identical despite different names*

### Comparing `tempcf-0.6.6/tempcf/MetadataInputDialog.py` & `tempcf-0.6.7/tempcf/MetadataInputDialog.py`

 * *Files identical despite different names*

### Comparing `tempcf-0.6.6/tempcf/Observable.py` & `tempcf-0.6.7/tempcf/Observable.py`

 * *Files identical despite different names*

### Comparing `tempcf-0.6.6/tempcf/ScrollableFrame.py` & `tempcf-0.6.7/tempcf/ScrollableFrame.py`

 * *Files identical despite different names*

### Comparing `tempcf-0.6.6/tempcf/TimeZoneConfigure.py` & `tempcf-0.6.7/tempcf/TimeZoneConfigure.py`

 * *Files identical despite different names*

### Comparing `tempcf-0.6.6/tempcf/ToolTip.py` & `tempcf-0.6.7/tempcf/ToolTip.py`

 * *Files identical despite different names*

### Comparing `tempcf-0.6.6/tempcf/main.py` & `tempcf-0.6.7/tempcf/main.py`

 * *Files identical despite different names*

### Comparing `tempcf-0.6.6/tempcf/tester.py` & `tempcf-0.6.7/tempcf/tester.py`

 * *Files identical despite different names*

### Comparing `tempcf-0.6.6/tempcf.egg-info/PKG-INFO` & `tempcf-0.6.7/tempcf.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tempcf
-Version: 0.6.6
+Version: 0.6.7
 Summary: A toolbox for flagging and cleaning ground temperature data
 Home-page: UNKNOWN
 Author: Nick Brown
 Author-email: 
 License: UNKNOWN
 Project-URL: Source, https://gitlab.com/permafrostnet/permafrost-tempcf
 Project-URL: Documentation, https://permafrostnet.gitlab.io/permafrost-tempcf/
```

