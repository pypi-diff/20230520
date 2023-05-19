# Comparing `tmp/tempcf-0.6.3.tar.gz` & `tmp/tempcf-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\tempcf-0.6.3.tar", last modified: Mon May 15 20:31:34 2023, max compression
+gzip compressed data, was "dist\tempcf-0.6.6.tar", last modified: Fri May 19 22:12:28 2023, max compression
```

## Comparing `tempcf-0.6.3.tar` & `tempcf-0.6.6.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 20:31:34.693035 tempcf-0.6.3/
--rw-rw-rw-   0        0        0     3079 2023-05-15 20:31:34.691033 tempcf-0.6.3/PKG-INFO
--rw-rw-rw-   0        0        0     2146 2023-05-15 20:26:54.000000 tempcf-0.6.3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-15 20:31:34.693035 tempcf-0.6.3/setup.cfg
--rw-rw-rw-   0        0        0     1328 2023-05-15 20:31:23.000000 tempcf-0.6.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-15 20:31:34.611035 tempcf-0.6.3/tempcf/
--rw-rw-rw-   0        0        0     2001 2023-02-20 22:21:11.000000 tempcf-0.6.3/tempcf/AboutDialog.py
--rw-rw-rw-   0        0        0     1317 2023-02-20 22:21:11.000000 tempcf-0.6.3/tempcf/ActionLogger.py
--rw-rw-rw-   0        0        0     7960 2023-03-16 21:24:19.000000 tempcf-0.6.3/tempcf/Dataframe.py
--rw-rw-rw-   0        0        0     2331 2023-02-20 22:21:11.000000 tempcf-0.6.3/tempcf/DatasetMetadata.py
--rw-rw-rw-   0        0        0     2651 2023-02-20 22:21:11.000000 tempcf-0.6.3/tempcf/DepthConfigure.py
--rw-rw-rw-   0        0        0     1154 2023-02-20 22:21:11.000000 tempcf-0.6.3/tempcf/EntryValidation.py
--rw-rw-rw-   0        0        0     6575 2023-03-16 21:26:02.000000 tempcf-0.6.3/tempcf/ExportType.py
--rw-rw-rw-   0        0        0      654 2023-03-16 21:24:19.000000 tempcf-0.6.3/tempcf/FileTypes.py
--rw-rw-rw-   0        0        0     3787 2023-03-16 16:46:32.000000 tempcf-0.6.3/tempcf/FilterConfigure.py
--rw-rw-rw-   0        0        0     1117 2023-02-20 22:21:11.000000 tempcf-0.6.3/tempcf/FilterContainer.py
--rw-rw-rw-   0        0        0     2781 2023-02-20 22:21:11.000000 tempcf-0.6.3/tempcf/FilterControl.py
--rw-rw-rw-   0        0        0     6212 2023-02-20 22:21:11.000000 tempcf-0.6.3/tempcf/FilterList.py
--rw-rw-rw-   0        0        0     3404 2023-03-16 16:46:32.000000 tempcf-0.6.3/tempcf/Filters.py
--rw-rw-rw-   0        0        0     7019 2023-02-20 22:21:11.000000 tempcf-0.6.3/tempcf/GraphView.py
--rw-rw-rw-   0        0        0     1520 2023-02-20 22:21:11.000000 tempcf-0.6.3/tempcf/HelpDialog.py
--rw-rw-rw-   0        0        0     4189 2023-03-16 21:24:19.000000 tempcf-0.6.3/tempcf/ImportType.py
--rw-rw-rw-   0        0        0     2928 2023-01-10 23:09:24.000000 tempcf-0.6.3/tempcf/LogParser.py
--rw-rw-rw-   0        0        0    10144 2023-03-16 21:24:19.000000 tempcf-0.6.3/tempcf/MainToolbar.py
--rw-rw-rw-   0        0        0      953 2023-02-20 22:21:11.000000 tempcf-0.6.3/tempcf/MetadataDialog.py
--rw-rw-rw-   0        0        0     4909 2023-02-20 22:21:11.000000 tempcf-0.6.3/tempcf/MetadataInputDialog.py
--rw-rw-rw-   0        0        0      687 2020-10-09 19:00:27.000000 tempcf-0.6.3/tempcf/Observable.py
--rw-rw-rw-   0        0        0      346 2023-02-20 22:21:11.000000 tempcf-0.6.3/tempcf/PopoutDialog.py
--rw-rw-rw-   0        0        0     1565 2023-02-20 22:21:11.000000 tempcf-0.6.3/tempcf/ScrollableFrame.py
--rw-rw-rw-   0        0        0     1781 2023-02-20 22:21:11.000000 tempcf-0.6.3/tempcf/TimeZoneConfigure.py
--rw-rw-rw-   0        0        0     1254 2023-01-13 18:53:29.000000 tempcf-0.6.3/tempcf/ToolTip.py
--rw-rw-rw-   0        0        0      485 2020-10-16 15:50:08.000000 tempcf-0.6.3/tempcf/Utils.py
--rw-rw-rw-   0        0        0       23 2023-05-15 20:31:10.000000 tempcf-0.6.3/tempcf/_version.py
--rw-rw-rw-   0        0        0    16042 2023-03-16 16:46:32.000000 tempcf-0.6.3/tempcf/main.py
--rw-rw-rw-   0        0        0     3319 2023-02-09 04:41:43.000000 tempcf-0.6.3/tempcf/tester.py
-drwxrwxrwx   0        0        0        0 2023-05-15 20:31:34.688036 tempcf-0.6.3/tempcf.egg-info/
--rw-rw-rw-   0        0        0     3079 2023-05-15 20:31:32.000000 tempcf-0.6.3/tempcf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      840 2023-05-15 20:31:33.000000 tempcf-0.6.3/tempcf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 20:31:32.000000 tempcf-0.6.3/tempcf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-05-15 20:31:32.000000 tempcf-0.6.3/tempcf.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       53 2023-05-15 20:31:32.000000 tempcf-0.6.3/tempcf.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-15 20:31:32.000000 tempcf-0.6.3/tempcf.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 22:12:28.412123 tempcf-0.6.6/
+-rw-rw-rw-   0        0        0     3079 2023-05-19 22:12:28.409125 tempcf-0.6.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2146 2023-05-15 20:26:54.000000 tempcf-0.6.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-19 22:12:28.416127 tempcf-0.6.6/setup.cfg
+-rw-rw-rw-   0        0        0     1379 2023-05-19 19:46:56.000000 tempcf-0.6.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 22:12:28.149694 tempcf-0.6.6/tempcf/
+-rw-rw-rw-   0        0        0     2001 2023-02-20 22:21:11.000000 tempcf-0.6.6/tempcf/AboutDialog.py
+-rw-rw-rw-   0        0        0     1317 2023-02-20 22:21:11.000000 tempcf-0.6.6/tempcf/ActionLogger.py
+-rw-rw-rw-   0        0        0     7960 2023-03-16 21:24:19.000000 tempcf-0.6.6/tempcf/Dataframe.py
+-rw-rw-rw-   0        0        0     2331 2023-02-20 22:21:11.000000 tempcf-0.6.6/tempcf/DatasetMetadata.py
+-rw-rw-rw-   0        0        0     2651 2023-02-20 22:21:11.000000 tempcf-0.6.6/tempcf/DepthConfigure.py
+-rw-rw-rw-   0        0        0     1154 2023-02-20 22:21:11.000000 tempcf-0.6.6/tempcf/EntryValidation.py
+-rw-rw-rw-   0        0        0     6759 2023-05-19 17:57:12.000000 tempcf-0.6.6/tempcf/ExportType.py
+-rw-rw-rw-   0        0        0      654 2023-03-16 21:24:19.000000 tempcf-0.6.6/tempcf/FileTypes.py
+-rw-rw-rw-   0        0        0     3787 2023-03-16 16:46:32.000000 tempcf-0.6.6/tempcf/FilterConfigure.py
+-rw-rw-rw-   0        0        0     1117 2023-02-20 22:21:11.000000 tempcf-0.6.6/tempcf/FilterContainer.py
+-rw-rw-rw-   0        0        0     2781 2023-02-20 22:21:11.000000 tempcf-0.6.6/tempcf/FilterControl.py
+-rw-rw-rw-   0        0        0     6212 2023-02-20 22:21:11.000000 tempcf-0.6.6/tempcf/FilterList.py
+-rw-rw-rw-   0        0        0     3037 2023-05-19 19:48:13.000000 tempcf-0.6.6/tempcf/Filters.py
+-rw-rw-rw-   0        0        0     7019 2023-02-20 22:21:11.000000 tempcf-0.6.6/tempcf/GraphView.py
+-rw-rw-rw-   0        0        0     1520 2023-02-20 22:21:11.000000 tempcf-0.6.6/tempcf/HelpDialog.py
+-rw-rw-rw-   0        0        0     4189 2023-03-16 21:24:19.000000 tempcf-0.6.6/tempcf/ImportType.py
+-rw-rw-rw-   0        0        0     2928 2023-01-10 23:09:24.000000 tempcf-0.6.6/tempcf/LogParser.py
+-rw-rw-rw-   0        0        0    10144 2023-03-16 21:24:19.000000 tempcf-0.6.6/tempcf/MainToolbar.py
+-rw-rw-rw-   0        0        0      953 2023-02-20 22:21:11.000000 tempcf-0.6.6/tempcf/MetadataDialog.py
+-rw-rw-rw-   0        0        0     4909 2023-02-20 22:21:11.000000 tempcf-0.6.6/tempcf/MetadataInputDialog.py
+-rw-rw-rw-   0        0        0      687 2020-10-09 19:00:27.000000 tempcf-0.6.6/tempcf/Observable.py
+-rw-rw-rw-   0        0        0      346 2023-02-20 22:21:11.000000 tempcf-0.6.6/tempcf/PopoutDialog.py
+-rw-rw-rw-   0        0        0     1565 2023-02-20 22:21:11.000000 tempcf-0.6.6/tempcf/ScrollableFrame.py
+-rw-rw-rw-   0        0        0     1781 2023-02-20 22:21:11.000000 tempcf-0.6.6/tempcf/TimeZoneConfigure.py
+-rw-rw-rw-   0        0        0     1254 2023-01-13 18:53:29.000000 tempcf-0.6.6/tempcf/ToolTip.py
+-rw-rw-rw-   0        0        0      485 2020-10-16 15:50:08.000000 tempcf-0.6.6/tempcf/Utils.py
+-rw-rw-rw-   0        0        0       23 2023-05-19 21:58:43.000000 tempcf-0.6.6/tempcf/_version.py
+-rw-rw-rw-   0        0        0    16042 2023-03-16 16:46:32.000000 tempcf-0.6.6/tempcf/main.py
+-rw-rw-rw-   0        0        0     3319 2023-02-09 04:41:43.000000 tempcf-0.6.6/tempcf/tester.py
+drwxrwxrwx   0        0        0        0 2023-05-19 22:12:28.375127 tempcf-0.6.6/tempcf.egg-info/
+-rw-rw-rw-   0        0        0     3079 2023-05-19 22:12:25.000000 tempcf-0.6.6/tempcf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      840 2023-05-19 22:12:26.000000 tempcf-0.6.6/tempcf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 22:12:25.000000 tempcf-0.6.6/tempcf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-05-19 22:12:25.000000 tempcf-0.6.6/tempcf.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       53 2023-05-19 22:12:25.000000 tempcf-0.6.6/tempcf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-19 22:12:25.000000 tempcf-0.6.6/tempcf.egg-info/top_level.txt
```

### Comparing `tempcf-0.6.3/PKG-INFO` & `tempcf-0.6.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tempcf
-Version: 0.6.3
+Version: 0.6.6
 Summary: A toolbox for flagging and cleaning ground temperature data
 Home-page: UNKNOWN
 Author: Nick Brown
 Author-email: 
 License: UNKNOWN
 Project-URL: Source, https://gitlab.com/permafrostnet/permafrost-tempcf
 Project-URL: Documentation, https://permafrostnet.gitlab.io/permafrost-tempcf/
```

### Comparing `tempcf-0.6.3/README.md` & `tempcf-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `tempcf-0.6.3/setup.py` & `tempcf-0.6.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,47 +7,50 @@
 
 setup(
     # Basic info
     name='tempcf',
     version=__version__,
     author='Nick Brown',
     author_email='',
-    project_urls = {
+    project_urls={
         "Source": 'https://gitlab.com/permafrostnet/permafrost-tempcf',
         "Documentation": "https://permafrostnet.gitlab.io/permafrost-tempcf/"
     },
     description='A toolbox for flagging and cleaning ground temperature data',
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     classifiers=[
         'Development Status :: 4 - Beta',
     ],
 
     # Packages and depencies
     packages=['tempcf'],
+
+    package_data={'tsp': ['assets/*']},
+
     install_requires=[
         'numpy',  # ==1.19.3',
         'matplotlib',  # ==3.2.2',
         'tsp>=1.5.0',
         'pfit',
         'pandas',
         'pillow',
         'scipy',
     ],
     extras_require={},
 
     # Data files
-    package_data={
-        'python_boilerplate': [
-            'templates/*.*',
-            'templates/license/*.*',
-            'templates/docs/*.*',
-            'templates/package/*.*'
-        ],
-    },
+#    package_data={
+#        'python_boilerplate': [
+#            'templates/*.*',
+#            'templates/license/*.*',
+#            'templates/docs/*.*',
+#            'templates/package/*.*'
+#        ],
+#    },
 
     # Scripts
     entry_points={
         'console_scripts': [
             'tempcf = tempcf.main:main']
     },
```

### Comparing `tempcf-0.6.3/tempcf/AboutDialog.py` & `tempcf-0.6.6/tempcf/AboutDialog.py`

 * *Files identical despite different names*

### Comparing `tempcf-0.6.3/tempcf/ActionLogger.py` & `tempcf-0.6.6/tempcf/ActionLogger.py`

 * *Files identical despite different names*

### Comparing `tempcf-0.6.3/tempcf/Dataframe.py` & `tempcf-0.6.6/tempcf/Dataframe.py`

 * *Files identical despite different names*

### Comparing `tempcf-0.6.3/tempcf/DatasetMetadata.py` & `tempcf-0.6.6/tempcf/DatasetMetadata.py`

 * *Files identical despite different names*

### Comparing `tempcf-0.6.3/tempcf/DepthConfigure.py` & `tempcf-0.6.6/tempcf/DepthConfigure.py`

 * *Files identical despite different names*

### Comparing `tempcf-0.6.3/tempcf/EntryValidation.py` & `tempcf-0.6.6/tempcf/EntryValidation.py`

 * *Files identical despite different names*

### Comparing `tempcf-0.6.3/tempcf/ExportType.py` & `tempcf-0.6.6/tempcf/ExportType.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,15 +131,18 @@
         df = df.reset_index()
         df.index += 1  # GeoPrecision files' "No" columns start at 1 instead of zero.
 
         header = "".join(self.make_header(self._meta))
 
         try:
             with open(f"{str(pathObj)}", 'w') as fp:
-                fp.write(header + df.to_csv(encoding="utf-8", float_format="%.4f", line_terminator="\n", index=False))
+                try:
+                    fp.write(header + df.to_csv(encoding="utf-8", float_format="%.4f", line_terminator="\n", index=False))
+                except TypeError:
+                    fp.write(header + df.to_csv(encoding="utf-8", float_format="%.4f", lineterminator="\n", index=False))
         except OSError:
             raise OSError(f"The file was unable to save at:\n{str(pathObj)}\nThe file may be open in another location.")
 
 
 class ExportGp5w(ExportGeoPrecision):
     
     REQUIRED_METADATA = {"logger_serial_number": ("serial_number", 'serial number of geoprecision logger', str, "")}
```

### Comparing `tempcf-0.6.3/tempcf/FileTypes.py` & `tempcf-0.6.6/tempcf/FileTypes.py`

 * *Files identical despite different names*

### Comparing `tempcf-0.6.3/tempcf/FilterConfigure.py` & `tempcf-0.6.6/tempcf/FilterConfigure.py`

 * *Files identical despite different names*

### Comparing `tempcf-0.6.3/tempcf/FilterContainer.py` & `tempcf-0.6.6/tempcf/FilterContainer.py`

 * *Files identical despite different names*

### Comparing `tempcf-0.6.3/tempcf/FilterControl.py` & `tempcf-0.6.6/tempcf/FilterControl.py`

 * *Files identical despite different names*

### Comparing `tempcf-0.6.3/tempcf/FilterList.py` & `tempcf-0.6.6/tempcf/FilterList.py`

 * *Files identical despite different names*

### Comparing `tempcf-0.6.3/tempcf/Filters.py` & `tempcf-0.6.6/tempcf/Filters.py`

 * *Files 6% similar despite different names*

```diff
@@ -103,19 +103,7 @@
     flag = (timestamps >= start) & (timestamps <= end)
 
     if invert:
         flag = ~flag
 
     return flag
 
-
-def ESJSD_filter(values, depths, n: int=7):
-    """
-    Flags data that deviates too far from the time series mean
-    """
-    result = np.zeros_like(values, dtype=bool)
-    for d in depths.unique():
-        i = (depths == d)
-        result[i] = values[i] > (np.nanmean(values[i]) + n * np.power(np.sqrt(np.nanstd(values)), 1.3))
-    
-    return result
-
```

### Comparing `tempcf-0.6.3/tempcf/GraphView.py` & `tempcf-0.6.6/tempcf/GraphView.py`

 * *Files identical despite different names*

### Comparing `tempcf-0.6.3/tempcf/HelpDialog.py` & `tempcf-0.6.6/tempcf/HelpDialog.py`

 * *Files identical despite different names*

### Comparing `tempcf-0.6.3/tempcf/ImportType.py` & `tempcf-0.6.6/tempcf/ImportType.py`

 * *Files identical despite different names*

### Comparing `tempcf-0.6.3/tempcf/LogParser.py` & `tempcf-0.6.6/tempcf/LogParser.py`

 * *Files identical despite different names*

### Comparing `tempcf-0.6.3/tempcf/MainToolbar.py` & `tempcf-0.6.6/tempcf/MainToolbar.py`

 * *Files identical despite different names*

### Comparing `tempcf-0.6.3/tempcf/MetadataDialog.py` & `tempcf-0.6.6/tempcf/MetadataDialog.py`

 * *Files identical despite different names*

### Comparing `tempcf-0.6.3/tempcf/MetadataInputDialog.py` & `tempcf-0.6.6/tempcf/MetadataInputDialog.py`

 * *Files identical despite different names*

### Comparing `tempcf-0.6.3/tempcf/Observable.py` & `tempcf-0.6.6/tempcf/Observable.py`

 * *Files identical despite different names*

### Comparing `tempcf-0.6.3/tempcf/ScrollableFrame.py` & `tempcf-0.6.6/tempcf/ScrollableFrame.py`

 * *Files identical despite different names*

### Comparing `tempcf-0.6.3/tempcf/TimeZoneConfigure.py` & `tempcf-0.6.6/tempcf/TimeZoneConfigure.py`

 * *Files identical despite different names*

### Comparing `tempcf-0.6.3/tempcf/ToolTip.py` & `tempcf-0.6.6/tempcf/ToolTip.py`

 * *Files identical despite different names*

### Comparing `tempcf-0.6.3/tempcf/main.py` & `tempcf-0.6.6/tempcf/main.py`

 * *Files identical despite different names*

### Comparing `tempcf-0.6.3/tempcf/tester.py` & `tempcf-0.6.6/tempcf/tester.py`

 * *Files identical despite different names*

### Comparing `tempcf-0.6.3/tempcf.egg-info/PKG-INFO` & `tempcf-0.6.6/tempcf.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tempcf
-Version: 0.6.3
+Version: 0.6.6
 Summary: A toolbox for flagging and cleaning ground temperature data
 Home-page: UNKNOWN
 Author: Nick Brown
 Author-email: 
 License: UNKNOWN
 Project-URL: Source, https://gitlab.com/permafrostnet/permafrost-tempcf
 Project-URL: Documentation, https://permafrostnet.gitlab.io/permafrost-tempcf/
```

### Comparing `tempcf-0.6.3/tempcf.egg-info/SOURCES.txt` & `tempcf-0.6.6/tempcf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

