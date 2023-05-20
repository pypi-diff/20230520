# Comparing `tmp/plugget-0.0.5.tar.gz` & `tmp/plugget-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plugget-0.0.5.tar", last modified: Wed May 17 21:21:50 2023, max compression
+gzip compressed data, was "plugget-0.0.6.tar", last modified: Sat May 20 10:22:57 2023, max compression
```

## Comparing `plugget-0.0.5.tar` & `plugget-0.0.6.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:21:50.086225 plugget-0.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:21:50.078225 plugget-0.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:21:50.082225 plugget-0.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-17 21:21:38.000000 plugget-0.0.5/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-05-17 21:21:38.000000 plugget-0.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-17 21:21:50.086225 plugget-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-05-17 21:21:38.000000 plugget-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:21:50.082225 plugget-0.0.5/plugget/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-17 21:21:38.000000 plugget-0.0.5/plugget/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:21:50.082225 plugget-0.0.5/plugget/actions/
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-17 21:21:38.000000 plugget-0.0.5/plugget/actions/_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-05-17 21:21:38.000000 plugget-0.0.5/plugget/actions/blender_addon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-17 21:21:38.000000 plugget-0.0.5/plugget/actions/blender_pip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-05-17 21:21:38.000000 plugget-0.0.5/plugget/actions/krita_pip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-05-17 21:21:38.000000 plugget-0.0.5/plugget/actions/krita_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-17 21:21:38.000000 plugget-0.0.5/plugget/actions/max_macroscript.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-05-17 21:21:38.000000 plugget-0.0.5/plugget/actions/unreal_pip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-17 21:21:38.000000 plugget-0.0.5/plugget/actions/unreal_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:21:50.086225 plugget-0.0.5/plugget/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 21:21:38.000000 plugget-0.0.5/plugget/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-05-17 21:21:38.000000 plugget-0.0.5/plugget/apps/blender.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:21:50.086225 plugget-0.0.5/plugget/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     9459 2023-05-17 21:21:38.000000 plugget-0.0.5/plugget/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:21:50.086225 plugget-0.0.5/plugget/data/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-17 21:21:38.000000 plugget-0.0.5/plugget/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13655 2023-05-17 21:21:38.000000 plugget-0.0.5/plugget/data/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-17 21:21:38.000000 plugget-0.0.5/plugget/data/packages_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:21:50.086225 plugget-0.0.5/plugget/github/
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-17 21:21:38.000000 plugget-0.0.5/plugget/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-17 21:21:38.000000 plugget-0.0.5/plugget/github/async.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:21:50.086225 plugget-0.0.5/plugget/gumroad/
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-17 21:21:38.000000 plugget-0.0.5/plugget/gumroad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-05-17 21:21:38.000000 plugget-0.0.5/plugget/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-17 21:21:38.000000 plugget-0.0.5/plugget/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:21:50.082225 plugget-0.0.5/plugget.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-17 21:21:50.000000 plugget-0.0.5/plugget.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-17 21:21:50.000000 plugget-0.0.5/plugget.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 21:21:50.000000 plugget-0.0.5/plugget.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-17 21:21:50.000000 plugget-0.0.5/plugget.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-17 21:21:50.000000 plugget-0.0.5/plugget.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-17 21:21:38.000000 plugget-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-17 21:21:38.000000 plugget-0.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 21:21:50.086225 plugget-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-17 21:21:38.000000 plugget-0.0.5/testcode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:22:57.249890 plugget-0.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:22:57.245890 plugget-0.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:22:57.245890 plugget-0.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-20 10:22:45.000000 plugget-0.0.6/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-05-20 10:22:45.000000 plugget-0.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-20 10:22:57.249890 plugget-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-05-20 10:22:45.000000 plugget-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:22:57.245890 plugget-0.0.6/plugget/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-20 10:22:45.000000 plugget-0.0.6/plugget/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:22:57.245890 plugget-0.0.6/plugget/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-20 10:22:45.000000 plugget-0.0.6/plugget/actions/_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-05-20 10:22:45.000000 plugget-0.0.6/plugget/actions/blender_addon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-20 10:22:45.000000 plugget-0.0.6/plugget/actions/blender_pip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-05-20 10:22:45.000000 plugget-0.0.6/plugget/actions/krita_pip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-05-20 10:22:45.000000 plugget-0.0.6/plugget/actions/krita_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-20 10:22:45.000000 plugget-0.0.6/plugget/actions/max_macroscript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-05-20 10:22:45.000000 plugget-0.0.6/plugget/actions/unreal_pip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-20 10:22:45.000000 plugget-0.0.6/plugget/actions/unreal_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:22:57.245890 plugget-0.0.6/plugget/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 10:22:45.000000 plugget-0.0.6/plugget/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-05-20 10:22:45.000000 plugget-0.0.6/plugget/apps/blender.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:22:57.245890 plugget-0.0.6/plugget/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     9558 2023-05-20 10:22:45.000000 plugget-0.0.6/plugget/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:22:57.249890 plugget-0.0.6/plugget/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-20 10:22:45.000000 plugget-0.0.6/plugget/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13655 2023-05-20 10:22:45.000000 plugget-0.0.6/plugget/data/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-20 10:22:45.000000 plugget-0.0.6/plugget/data/packages_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:22:57.249890 plugget-0.0.6/plugget/github/
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-20 10:22:45.000000 plugget-0.0.6/plugget/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-20 10:22:45.000000 plugget-0.0.6/plugget/github/async.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:22:57.249890 plugget-0.0.6/plugget/gumroad/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-20 10:22:45.000000 plugget-0.0.6/plugget/gumroad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-05-20 10:22:45.000000 plugget-0.0.6/plugget/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-20 10:22:45.000000 plugget-0.0.6/plugget/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 10:22:57.245890 plugget-0.0.6/plugget.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-20 10:22:57.000000 plugget-0.0.6/plugget.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-20 10:22:57.000000 plugget-0.0.6/plugget.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 10:22:57.000000 plugget-0.0.6/plugget.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-20 10:22:57.000000 plugget-0.0.6/plugget.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-20 10:22:57.000000 plugget-0.0.6/plugget.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-20 10:22:45.000000 plugget-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-20 10:22:45.000000 plugget-0.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 10:22:57.249890 plugget-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-20 10:22:45.000000 plugget-0.0.6/testcode.py
```

### Comparing `plugget-0.0.5/.github/workflows/python-publish.yml` & `plugget-0.0.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `plugget-0.0.5/.gitignore` & `plugget-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `plugget-0.0.5/PKG-INFO` & `plugget-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plugget
-Version: 0.0.5
+Version: 0.0.6
 Summary: detect which app the python interpreter is running in
 Author: Hannes
 Project-URL: Homepage, https://github.com/hannesdelbeke/plugget
 Project-URL: Source, https://github.com/hannesdelbeke/plugget
 Keywords: plugin,addon,add-on,extension,package,manager,resource,studio,dcc,app,application,pipeline,blender,krita,max
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.4
```

### Comparing `plugget-0.0.5/README.md` & `plugget-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `plugget-0.0.5/plugget/actions/_template.py` & `plugget-0.0.6/plugget/actions/_template.py`

 * *Files identical despite different names*

### Comparing `plugget-0.0.5/plugget/actions/blender_addon.py` & `plugget-0.0.6/plugget/actions/blender_addon.py`

 * *Files identical despite different names*

### Comparing `plugget-0.0.5/plugget/actions/blender_pip.py` & `plugget-0.0.6/plugget/actions/blender_pip.py`

 * *Files identical despite different names*

### Comparing `plugget-0.0.5/plugget/actions/krita_pip.py` & `plugget-0.0.6/plugget/actions/krita_pip.py`

 * *Files identical despite different names*

### Comparing `plugget-0.0.5/plugget/actions/krita_plugin.py` & `plugget-0.0.6/plugget/actions/krita_plugin.py`

 * *Files identical despite different names*

### Comparing `plugget-0.0.5/plugget/actions/max_macroscript.py` & `plugget-0.0.6/plugget/actions/max_macroscript.py`

 * *Files identical despite different names*

### Comparing `plugget-0.0.5/plugget/actions/unreal_pip.py` & `plugget-0.0.6/plugget/actions/unreal_pip.py`

 * *Files identical despite different names*

### Comparing `plugget-0.0.5/plugget/actions/unreal_plugin.py` & `plugget-0.0.6/plugget/actions/unreal_plugin.py`

 * *Files identical despite different names*

### Comparing `plugget-0.0.5/plugget/apps/blender.py` & `plugget-0.0.6/plugget/apps/blender.py`

 * *Files identical despite different names*

### Comparing `plugget-0.0.5/plugget/commands/__init__.py` & `plugget-0.0.6/plugget/commands/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         if not app:
             app_found = detect_app.detect_app()
             return app_found.id if app_found else None
     except:
         None
 
 
-def search(name=None, app=None, verbose=True, version=None, source_dirs=None):
+def search(name=None, app=None, verbose=True, version=None, source_dirs=None) -> PackagesMeta:
     """
     search if package is in sources
     :param name: pacakge name to search in manifest repo, return all packages if not set
     :param app: app name to search in, return all apps if not set
     :param verbose: print results if True
     """
 
@@ -155,19 +155,17 @@
     if run from an app, only list the apps installed packages, with option to list all app installed packages
 
     :param enabled: list enabled packages only if True
     :param disabled: list disabled packages only if True
     TODO :param source: list packages from specific source only if set
     """
     results = search(name=package_name, app=app, verbose=verbose, source_dirs=[settings.INSTALLED_DIR])
-
     return results
 
 
-#    plugin_name = plugin_name or plugin_name_from_manifest(package_name)
 def install(package_name, enable=True, app=None, version=None, **kwargs):
     """
     install package
     :param name: name of the manifest folder in the manifest repo
     :param enable: enable plugin after install
     """
     # todo
@@ -176,16 +174,21 @@
     #  install package, by running action(s) from manifest
     #  save manifest to installed packages dir
 
     # copy package to blender package folder
     # module = _get_app_module()
 
     # get package manifest from package repo
-    meta_collection = search(name=package_name, app=app, verbose=False, version=version)[0]
-    package = meta_collection.get_version(version)
+    result = search(name=package_name, app=app, verbose=False, version=version)
+    if not result:
+        logging.warning(f"Package {package_name} not found, failed install")
+        return
+
+    meta_collection = result[0]
+    package = meta_collection.get_version(version) or meta_collection.latest
 
     if not package:
         logging.warning("Package not found, cancelling install")
         return
 
     package.install(enable=enable, **kwargs)
     # uninstall if unsuccessful?
```

### Comparing `plugget-0.0.5/plugget/data/package.py` & `plugget-0.0.6/plugget/data/package.py`

 * *Files identical despite different names*

### Comparing `plugget-0.0.5/plugget/data/packages_meta.py` & `plugget-0.0.6/plugget/data/packages_meta.py`

 * *Files identical despite different names*

### Comparing `plugget-0.0.5/plugget/github/__init__.py` & `plugget-0.0.6/plugget/github/__init__.py`

 * *Files identical despite different names*

### Comparing `plugget-0.0.5/plugget/github/async.py` & `plugget-0.0.6/plugget/github/async.py`

 * *Files identical despite different names*

### Comparing `plugget-0.0.5/plugget/gumroad/__init__.py` & `plugget-0.0.6/plugget/gumroad/__init__.py`

 * *Files identical despite different names*

### Comparing `plugget-0.0.5/plugget/settings.py` & `plugget-0.0.6/plugget/settings.py`

 * *Files identical despite different names*

### Comparing `plugget-0.0.5/plugget.egg-info/PKG-INFO` & `plugget-0.0.6/plugget.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plugget
-Version: 0.0.5
+Version: 0.0.6
 Summary: detect which app the python interpreter is running in
 Author: Hannes
 Project-URL: Homepage, https://github.com/hannesdelbeke/plugget
 Project-URL: Source, https://github.com/hannesdelbeke/plugget
 Keywords: plugin,addon,add-on,extension,package,manager,resource,studio,dcc,app,application,pipeline,blender,krita,max
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.4
```

### Comparing `plugget-0.0.5/plugget.egg-info/SOURCES.txt` & `plugget-0.0.6/plugget.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plugget-0.0.5/pyproject.toml` & `plugget-0.0.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3.7",
 ]
 #dynamic = ["dependencies"]
 dependencies = ['importlib-metadata; python_version<"3.7"', "detect-app"]
 #dynamic = ["version"]
-version = "0.0.5"
+version = "0.0.6"
 
 #[project.optional-dependencies]
 #yaml = ["pyyaml"]
 
 #[project.scripts]
 #my-script = "my_package.module:function"
```

### Comparing `plugget-0.0.5/testcode.py` & `plugget-0.0.6/testcode.py`

 * *Files identical despite different names*

