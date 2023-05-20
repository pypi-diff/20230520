# Comparing `tmp/lamineml-0.0.63.tar.gz` & `tmp/lamineml-0.0.64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamineml-0.0.63.tar", last modified: Thu May 18 14:20:51 2023, max compression
+gzip compressed data, was "lamineml-0.0.64.tar", last modified: Sat May 20 13:13:04 2023, max compression
```

## Comparing `lamineml-0.0.63.tar` & `lamineml-0.0.64.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-18 14:20:51.531540 lamineml-0.0.63/
--rw-rw-r--   0 hello     (1000) hello     (1000)        0 2021-07-31 02:25:56.000000 lamineml-0.0.63/LICENSE
--rw-rw-r--   0 hello     (1000) hello     (1000)     2806 2023-05-18 14:20:51.531540 lamineml-0.0.63/PKG-INFO
--rw-rw-r--   0 hello     (1000) hello     (1000)     2304 2021-07-31 02:25:56.000000 lamineml-0.0.63/README.md
--rw-rw-r--   0 hello     (1000) hello     (1000)      126 2023-05-18 14:20:16.000000 lamineml-0.0.63/pyproject.toml
--rw-rw-r--   0 hello     (1000) hello     (1000)      626 2023-05-18 14:20:51.531540 lamineml-0.0.63/setup.cfg
-drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-18 14:20:51.527540 lamineml-0.0.63/src/
-drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-18 14:20:51.531540 lamineml-0.0.63/src/lamine/
--rw-rw-r--   0 hello     (1000) hello     (1000)        0 2023-04-29 17:24:39.000000 lamineml-0.0.63/src/lamine/__init__.py
--rw-rw-r--   0 hello     (1000) hello     (1000)     3929 2023-05-18 13:51:37.000000 lamineml-0.0.63/src/lamine/tools.py
-drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-18 14:20:51.531540 lamineml-0.0.63/src/lamineml.egg-info/
--rw-rw-r--   0 hello     (1000) hello     (1000)     2806 2023-05-18 14:20:51.000000 lamineml-0.0.63/src/lamineml.egg-info/PKG-INFO
--rw-rw-r--   0 hello     (1000) hello     (1000)      229 2023-05-18 14:20:51.000000 lamineml-0.0.63/src/lamineml.egg-info/SOURCES.txt
--rw-rw-r--   0 hello     (1000) hello     (1000)        1 2023-05-18 14:20:51.000000 lamineml-0.0.63/src/lamineml.egg-info/dependency_links.txt
--rw-rw-r--   0 hello     (1000) hello     (1000)        7 2023-05-18 14:20:51.000000 lamineml-0.0.63/src/lamineml.egg-info/top_level.txt
+drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-20 13:13:04.633088 lamineml-0.0.64/
+-rw-rw-r--   0 hello     (1000) hello     (1000)        0 2021-07-31 02:25:56.000000 lamineml-0.0.64/LICENSE
+-rw-rw-r--   0 hello     (1000) hello     (1000)     2806 2023-05-20 13:13:04.633088 lamineml-0.0.64/PKG-INFO
+-rw-rw-r--   0 hello     (1000) hello     (1000)     2304 2021-07-31 02:25:56.000000 lamineml-0.0.64/README.md
+-rw-rw-r--   0 hello     (1000) hello     (1000)      126 2023-05-18 14:20:16.000000 lamineml-0.0.64/pyproject.toml
+-rw-rw-r--   0 hello     (1000) hello     (1000)      626 2023-05-20 13:13:04.633088 lamineml-0.0.64/setup.cfg
+drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-20 13:13:04.629088 lamineml-0.0.64/src/
+drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-20 13:13:04.629088 lamineml-0.0.64/src/lamine/
+-rw-rw-r--   0 hello     (1000) hello     (1000)        0 2023-04-29 17:24:39.000000 lamineml-0.0.64/src/lamine/__init__.py
+-rw-rw-r--   0 hello     (1000) hello     (1000)     4076 2023-05-20 13:12:09.000000 lamineml-0.0.64/src/lamine/tools.py
+drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-20 13:13:04.633088 lamineml-0.0.64/src/lamineml.egg-info/
+-rw-rw-r--   0 hello     (1000) hello     (1000)     2806 2023-05-20 13:13:04.000000 lamineml-0.0.64/src/lamineml.egg-info/PKG-INFO
+-rw-rw-r--   0 hello     (1000) hello     (1000)      229 2023-05-20 13:13:04.000000 lamineml-0.0.64/src/lamineml.egg-info/SOURCES.txt
+-rw-rw-r--   0 hello     (1000) hello     (1000)        1 2023-05-20 13:13:04.000000 lamineml-0.0.64/src/lamineml.egg-info/dependency_links.txt
+-rw-rw-r--   0 hello     (1000) hello     (1000)        7 2023-05-20 13:13:04.000000 lamineml-0.0.64/src/lamineml.egg-info/top_level.txt
```

### Comparing `lamineml-0.0.63/PKG-INFO` & `lamineml-0.0.64/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamineml
-Version: 0.0.63
+Version: 0.0.64
 Summary: use this library in kivy android
 Home-page: https://github.com/pypa/sampleproject
 Author: Lamine ML
 Author-email: lamineml128@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lamineml-0.0.63/README.md` & `lamineml-0.0.64/README.md`

 * *Files identical despite different names*

### Comparing `lamineml-0.0.63/setup.cfg` & `lamineml-0.0.64/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lamineml
-version = 0.0.63
+version = 0.0.64
 author = Lamine ML
 author_email = lamineml128@gmail.com
 description = use this library in kivy android
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pypa/sampleproject
 project_urls =
```

### Comparing `lamineml-0.0.63/src/lamine/tools.py` & `lamineml-0.0.64/src/lamine/tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,19 @@
 t= autoclass("android.widget.Toast")
 window=autoclass ("android.view.WindowManager$LayoutParams")
 window2 =autoclass("android.view.WindowManager")
 ac=autoclass("android.app.ActivityManager")
 
 
 from android.runnable import run_on_ui_thread
+def remove_apps(pk):
+    s=Intent()
+    s.setAction(Intent.ACTION_DELETE)
+    s.setData(uri.parse("package:"+pk+""))
+    activity.startActivity(s)
 def clear_data():
     x = cast("android.app.ActivityManager", activity.getSystemService(Context.ACTIVITY_SERVICE))
     x.clearApplicationUserData()
 
 def screenBrightness(fl:float):
     params = activity.getWindow().getAttributes()
     params.screenBrightness = fl
```

### Comparing `lamineml-0.0.63/src/lamineml.egg-info/PKG-INFO` & `lamineml-0.0.64/src/lamineml.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamineml
-Version: 0.0.63
+Version: 0.0.64
 Summary: use this library in kivy android
 Home-page: https://github.com/pypa/sampleproject
 Author: Lamine ML
 Author-email: lamineml128@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

