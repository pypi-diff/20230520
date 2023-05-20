# Comparing `tmp/NotionLab-1.1.1.tar.gz` & `tmp/NotionLab-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NotionLab-1.1.1.tar", last modified: Sat Apr  1 11:17:40 2023, max compression
+gzip compressed data, was "NotionLab-1.1.3.tar", last modified: Sat May 20 08:50:44 2023, max compression
```

## Comparing `NotionLab-1.1.1.tar` & `NotionLab-1.1.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 11:17:40.756862 NotionLab-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-01 11:17:26.000000 NotionLab-1.1.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 11:17:40.756862 NotionLab-1.1.1/NotionLab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-01 11:17:40.000000 NotionLab-1.1.1/NotionLab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-01 11:17:40.000000 NotionLab-1.1.1/NotionLab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-01 11:17:40.000000 NotionLab-1.1.1/NotionLab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-01 11:17:40.000000 NotionLab-1.1.1/NotionLab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-01 11:17:40.000000 NotionLab-1.1.1/NotionLab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-01 11:17:40.756862 NotionLab-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-01 11:17:26.000000 NotionLab-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 11:17:40.756862 NotionLab-1.1.1/notion_lab/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 11:17:26.000000 NotionLab-1.1.1/notion_lab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 11:17:40.756862 NotionLab-1.1.1/notion_lab/converter/
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-01 11:17:26.000000 NotionLab-1.1.1/notion_lab/converter/Converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-04-01 11:17:26.000000 NotionLab-1.1.1/notion_lab/converter/HtmlCvt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-04-01 11:17:26.000000 NotionLab-1.1.1/notion_lab/converter/MDCvt.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-01 11:17:26.000000 NotionLab-1.1.1/notion_lab/converter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 11:17:40.756862 NotionLab-1.1.1/notion_lab/converter/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 11:17:26.000000 NotionLab-1.1.1/notion_lab/converter/util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 11:17:40.756862 NotionLab-1.1.1/notion_lab/converter/util/html/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-01 11:17:26.000000 NotionLab-1.1.1/notion_lab/converter/util/html/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 11:17:40.756862 NotionLab-1.1.1/notion_lab/converter/util/html/elements/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-01 11:17:26.000000 NotionLab-1.1.1/notion_lab/converter/util/html/elements/Code.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-01 11:17:26.000000 NotionLab-1.1.1/notion_lab/converter/util/html/elements/Image.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-01 11:17:26.000000 NotionLab-1.1.1/notion_lab/converter/util/html/elements/List.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-01 11:17:26.000000 NotionLab-1.1.1/notion_lab/converter/util/html/elements/TableRow.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-01 11:17:26.000000 NotionLab-1.1.1/notion_lab/converter/util/html/elements/Text.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-01 11:17:26.000000 NotionLab-1.1.1/notion_lab/converter/util/html/elements/Toggle.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-01 11:17:26.000000 NotionLab-1.1.1/notion_lab/converter/util/html/elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-01 11:17:26.000000 NotionLab-1.1.1/notion_lab/converter/util/html/html.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 11:17:40.756862 NotionLab-1.1.1/notion_lab/converter/util/md/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-01 11:17:26.000000 NotionLab-1.1.1/notion_lab/converter/util/md/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-01 11:17:26.000000 NotionLab-1.1.1/notion_lab/converter/util/md/md.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 11:17:40.756862 NotionLab-1.1.1/notion_lab/database/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-01 11:17:26.000000 NotionLab-1.1.1/notion_lab/database/DB.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-01 11:17:26.000000 NotionLab-1.1.1/notion_lab/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-01 11:17:40.756862 NotionLab-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-01 11:17:26.000000 NotionLab-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:50:44.063879 NotionLab-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-20 08:50:32.000000 NotionLab-1.1.3/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:50:44.059879 NotionLab-1.1.3/NotionLab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-20 08:50:44.000000 NotionLab-1.1.3/NotionLab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-20 08:50:44.000000 NotionLab-1.1.3/NotionLab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 08:50:44.000000 NotionLab-1.1.3/NotionLab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-20 08:50:44.000000 NotionLab-1.1.3/NotionLab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-20 08:50:44.000000 NotionLab-1.1.3/NotionLab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-20 08:50:44.063879 NotionLab-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-20 08:50:32.000000 NotionLab-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:50:44.059879 NotionLab-1.1.3/notion_lab/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 08:50:32.000000 NotionLab-1.1.3/notion_lab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:50:44.059879 NotionLab-1.1.3/notion_lab/converter/
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-20 08:50:32.000000 NotionLab-1.1.3/notion_lab/converter/Converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-05-20 08:50:32.000000 NotionLab-1.1.3/notion_lab/converter/HtmlCvt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-05-20 08:50:32.000000 NotionLab-1.1.3/notion_lab/converter/MDCvt.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-20 08:50:32.000000 NotionLab-1.1.3/notion_lab/converter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:50:44.063879 NotionLab-1.1.3/notion_lab/converter/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 08:50:32.000000 NotionLab-1.1.3/notion_lab/converter/util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:50:44.063879 NotionLab-1.1.3/notion_lab/converter/util/html/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-20 08:50:32.000000 NotionLab-1.1.3/notion_lab/converter/util/html/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:50:44.063879 NotionLab-1.1.3/notion_lab/converter/util/html/elements/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-20 08:50:32.000000 NotionLab-1.1.3/notion_lab/converter/util/html/elements/Code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-20 08:50:32.000000 NotionLab-1.1.3/notion_lab/converter/util/html/elements/Image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-20 08:50:32.000000 NotionLab-1.1.3/notion_lab/converter/util/html/elements/List.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-20 08:50:32.000000 NotionLab-1.1.3/notion_lab/converter/util/html/elements/TableRow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-20 08:50:32.000000 NotionLab-1.1.3/notion_lab/converter/util/html/elements/Text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-20 08:50:32.000000 NotionLab-1.1.3/notion_lab/converter/util/html/elements/Toggle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-20 08:50:32.000000 NotionLab-1.1.3/notion_lab/converter/util/html/elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-20 08:50:32.000000 NotionLab-1.1.3/notion_lab/converter/util/html/html.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:50:44.063879 NotionLab-1.1.3/notion_lab/converter/util/md/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-20 08:50:32.000000 NotionLab-1.1.3/notion_lab/converter/util/md/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-20 08:50:32.000000 NotionLab-1.1.3/notion_lab/converter/util/md/md.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:50:44.063879 NotionLab-1.1.3/notion_lab/database/
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-05-20 08:50:32.000000 NotionLab-1.1.3/notion_lab/database/DB.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-20 08:50:32.000000 NotionLab-1.1.3/notion_lab/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 08:50:44.063879 NotionLab-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-20 08:50:32.000000 NotionLab-1.1.3/setup.py
```

### Comparing `NotionLab-1.1.1/LICENSE` & `NotionLab-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `NotionLab-1.1.1/NotionLab.egg-info/PKG-INFO` & `NotionLab-1.1.3/NotionLab.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NotionLab
-Version: 1.1.1
+Version: 1.1.3
 Summary: A kit for Notion based on Notion Python SDK.
 Home-page: https://github.com/ElaBosak233/NotionLab
 Author: ElaBosak233
 Author-email: ElaBosak233@gmail.com
 License: MIT Licence
 Keywords: notion,kit,parser,html,markdown,lab
 Platform: any
```

### Comparing `NotionLab-1.1.1/NotionLab.egg-info/SOURCES.txt` & `NotionLab-1.1.3/NotionLab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NotionLab-1.1.1/PKG-INFO` & `NotionLab-1.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NotionLab
-Version: 1.1.1
+Version: 1.1.3
 Summary: A kit for Notion based on Notion Python SDK.
 Home-page: https://github.com/ElaBosak233/NotionLab
 Author: ElaBosak233
 Author-email: ElaBosak233@gmail.com
 License: MIT Licence
 Keywords: notion,kit,parser,html,markdown,lab
 Platform: any
```

### Comparing `NotionLab-1.1.1/README.md` & `NotionLab-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `NotionLab-1.1.1/notion_lab/converter/Converter.py` & `NotionLab-1.1.3/notion_lab/converter/Converter.py`

 * *Files identical despite different names*

### Comparing `NotionLab-1.1.1/notion_lab/converter/HtmlCvt.py` & `NotionLab-1.1.3/notion_lab/converter/HtmlCvt.py`

 * *Files identical despite different names*

### Comparing `NotionLab-1.1.1/notion_lab/converter/MDCvt.py` & `NotionLab-1.1.3/notion_lab/converter/MDCvt.py`

 * *Files identical despite different names*

### Comparing `NotionLab-1.1.1/notion_lab/converter/util/html/elements/TableRow.py` & `NotionLab-1.1.3/notion_lab/converter/util/html/elements/TableRow.py`

 * *Files identical despite different names*

### Comparing `NotionLab-1.1.1/notion_lab/converter/util/html/html.py` & `NotionLab-1.1.3/notion_lab/converter/util/html/html.py`

 * *Files identical despite different names*

### Comparing `NotionLab-1.1.1/notion_lab/converter/util/md/md.py` & `NotionLab-1.1.3/notion_lab/converter/util/md/md.py`

 * *Files identical despite different names*

### Comparing `NotionLab-1.1.1/setup.py` & `NotionLab-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="NotionLab",
-    version="1.1.1",
+    version="1.1.3",
     keywords=["notion", "kit", "parser", "html", "markdown", "lab"],
     description="A kit for Notion based on Notion Python SDK.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     license="MIT Licence",
 
     url="https://github.com/ElaBosak233/NotionLab",
```

