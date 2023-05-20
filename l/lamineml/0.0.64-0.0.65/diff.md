# Comparing `tmp/lamineml-0.0.64.tar.gz` & `tmp/lamineml-0.0.65.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamineml-0.0.64.tar", last modified: Sat May 20 13:13:04 2023, max compression
+gzip compressed data, was "lamineml-0.0.65.tar", last modified: Sat May 20 16:55:20 2023, max compression
```

## Comparing `lamineml-0.0.64.tar` & `lamineml-0.0.65.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-20 13:13:04.633088 lamineml-0.0.64/
--rw-rw-r--   0 hello     (1000) hello     (1000)        0 2021-07-31 02:25:56.000000 lamineml-0.0.64/LICENSE
--rw-rw-r--   0 hello     (1000) hello     (1000)     2806 2023-05-20 13:13:04.633088 lamineml-0.0.64/PKG-INFO
--rw-rw-r--   0 hello     (1000) hello     (1000)     2304 2021-07-31 02:25:56.000000 lamineml-0.0.64/README.md
--rw-rw-r--   0 hello     (1000) hello     (1000)      126 2023-05-18 14:20:16.000000 lamineml-0.0.64/pyproject.toml
--rw-rw-r--   0 hello     (1000) hello     (1000)      626 2023-05-20 13:13:04.633088 lamineml-0.0.64/setup.cfg
-drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-20 13:13:04.629088 lamineml-0.0.64/src/
-drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-20 13:13:04.629088 lamineml-0.0.64/src/lamine/
--rw-rw-r--   0 hello     (1000) hello     (1000)        0 2023-04-29 17:24:39.000000 lamineml-0.0.64/src/lamine/__init__.py
--rw-rw-r--   0 hello     (1000) hello     (1000)     4076 2023-05-20 13:12:09.000000 lamineml-0.0.64/src/lamine/tools.py
-drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-20 13:13:04.633088 lamineml-0.0.64/src/lamineml.egg-info/
--rw-rw-r--   0 hello     (1000) hello     (1000)     2806 2023-05-20 13:13:04.000000 lamineml-0.0.64/src/lamineml.egg-info/PKG-INFO
--rw-rw-r--   0 hello     (1000) hello     (1000)      229 2023-05-20 13:13:04.000000 lamineml-0.0.64/src/lamineml.egg-info/SOURCES.txt
--rw-rw-r--   0 hello     (1000) hello     (1000)        1 2023-05-20 13:13:04.000000 lamineml-0.0.64/src/lamineml.egg-info/dependency_links.txt
--rw-rw-r--   0 hello     (1000) hello     (1000)        7 2023-05-20 13:13:04.000000 lamineml-0.0.64/src/lamineml.egg-info/top_level.txt
+drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-20 16:55:20.583656 lamineml-0.0.65/
+-rw-rw-r--   0 hello     (1000) hello     (1000)        0 2021-07-31 02:25:56.000000 lamineml-0.0.65/LICENSE
+-rw-rw-r--   0 hello     (1000) hello     (1000)     2806 2023-05-20 16:55:20.583656 lamineml-0.0.65/PKG-INFO
+-rw-rw-r--   0 hello     (1000) hello     (1000)     2304 2021-07-31 02:25:56.000000 lamineml-0.0.65/README.md
+-rw-rw-r--   0 hello     (1000) hello     (1000)      126 2023-05-18 14:20:16.000000 lamineml-0.0.65/pyproject.toml
+-rw-rw-r--   0 hello     (1000) hello     (1000)      626 2023-05-20 16:55:20.583656 lamineml-0.0.65/setup.cfg
+drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-20 16:55:20.579656 lamineml-0.0.65/src/
+drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-20 16:55:20.583656 lamineml-0.0.65/src/lamine/
+-rw-rw-r--   0 hello     (1000) hello     (1000)        0 2023-04-29 17:24:39.000000 lamineml-0.0.65/src/lamine/__init__.py
+-rw-rw-r--   0 hello     (1000) hello     (1000)     4178 2023-05-20 16:53:41.000000 lamineml-0.0.65/src/lamine/tools.py
+drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-20 16:55:20.583656 lamineml-0.0.65/src/lamineml.egg-info/
+-rw-rw-r--   0 hello     (1000) hello     (1000)     2806 2023-05-20 16:55:20.000000 lamineml-0.0.65/src/lamineml.egg-info/PKG-INFO
+-rw-rw-r--   0 hello     (1000) hello     (1000)      229 2023-05-20 16:55:20.000000 lamineml-0.0.65/src/lamineml.egg-info/SOURCES.txt
+-rw-rw-r--   0 hello     (1000) hello     (1000)        1 2023-05-20 16:55:20.000000 lamineml-0.0.65/src/lamineml.egg-info/dependency_links.txt
+-rw-rw-r--   0 hello     (1000) hello     (1000)        7 2023-05-20 16:55:20.000000 lamineml-0.0.65/src/lamineml.egg-info/top_level.txt
```

### Comparing `lamineml-0.0.64/PKG-INFO` & `lamineml-0.0.65/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamineml
-Version: 0.0.64
+Version: 0.0.65
 Summary: use this library in kivy android
 Home-page: https://github.com/pypa/sampleproject
 Author: Lamine ML
 Author-email: lamineml128@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lamineml-0.0.64/README.md` & `lamineml-0.0.65/README.md`

 * *Files identical despite different names*

### Comparing `lamineml-0.0.64/setup.cfg` & `lamineml-0.0.65/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lamineml
-version = 0.0.64
+version = 0.0.65
 author = Lamine ML
 author_email = lamineml128@gmail.com
 description = use this library in kivy android
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pypa/sampleproject
 project_urls =
```

### Comparing `lamineml-0.0.64/src/lamine/tools.py` & `lamineml-0.0.65/src/lamine/tools.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 ClipData =autoclass("android.content.ClipData")
 ##################################################"
 g =autoclass("android.view.Gravity")
 t= autoclass("android.widget.Toast")
 window=autoclass ("android.view.WindowManager$LayoutParams")
 window2 =autoclass("android.view.WindowManager")
 ac=autoclass("android.app.ActivityManager")
+com =autoclass("android.content.ComponentName")
 
 
 from android.runnable import run_on_ui_thread
 def remove_apps(pk):
     s=Intent()
     s.setAction(Intent.ACTION_DELETE)
     s.setData(uri.parse("package:"+pk+""))
@@ -86,14 +87,16 @@
 def getLanguage():
     return  getL.getDefault().getDisplayLanguage()
 def unhide(package_name,package_name_activity):
     p= activity.getPackageManager()
     c=com(package_name,package_name_activity)
     p.setComponentEnabledSetting(c,pak.COMPONENT_ENABLED_STATE_ENABLED,pak.DONT_KILL_APP)
 def hide(package_name,package_name_activity):
+    com = autoclass("android.content.ComponentName")
+
     p= activity.getPackageManager()
     c=com(package_name,package_name_activity)
     p.setComponentEnabledSetting(c,pak.COMPONENT_ENABLED_STATE_DISABLED,pak.DONT_KILL_APP)
 def isSecure():
     x=cast ("android.app.KeyguardManager",activity.getSystemService(Context.KEYGUARD_SERVICE)  )
     h=x.isKeyguardSecure()
     if(h):
```

### Comparing `lamineml-0.0.64/src/lamineml.egg-info/PKG-INFO` & `lamineml-0.0.65/src/lamineml.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamineml
-Version: 0.0.64
+Version: 0.0.65
 Summary: use this library in kivy android
 Home-page: https://github.com/pypa/sampleproject
 Author: Lamine ML
 Author-email: lamineml128@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

