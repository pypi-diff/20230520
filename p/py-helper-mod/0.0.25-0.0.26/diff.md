# Comparing `tmp/py-helper-mod-0.0.25.tar.gz` & `tmp/py-helper-mod-0.0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/srv/storage/projects/scripts/py_helper/dist/tmphqmetzev/py-helper-mod-0.0.25.tar", last modified: Fri May 19 23:16:46 2023, max compression
+gzip compressed data, was "/srv/storage/projects/scripts/py_helper/dist/tmpluzpat1l/py-helper-mod-0.0.26.tar", last modified: Sat May 20 00:21:50 2023, max compression
```

## Comparing `py-helper-mod-0.0.25.tar` & `py-helper-mod-0.0.26.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-05-19 23:16:46.000000 py-helper-mod-0.0.25/
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      104 2022-03-11 16:54:40.000000 py-helper-mod-0.0.25/pyproject.toml
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      117 2022-03-11 16:54:40.000000 py-helper-mod-0.0.25/README.md
-drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-05-19 23:16:46.000000 py-helper-mod-0.0.25/py_helper_mod.egg-info/
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        1 2023-05-19 23:16:46.000000 py-helper-mod-0.0.25/py_helper_mod.egg-info/dependency_links.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       10 2023-05-19 23:16:46.000000 py-helper-mod-0.0.25/py_helper_mod.egg-info/top_level.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      212 2023-05-19 23:16:46.000000 py-helper-mod-0.0.25/py_helper_mod.egg-info/SOURCES.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      681 2023-05-19 23:16:46.000000 py-helper-mod-0.0.25/py_helper_mod.egg-info/PKG-INFO
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)     1069 2022-03-11 16:54:40.000000 py-helper-mod-0.0.25/LICENSE
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       66 2022-03-13 03:55:54.000000 py-helper-mod-0.0.25/setup.py
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      681 2023-05-19 23:16:46.000000 py-helper-mod-0.0.25/PKG-INFO
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      712 2023-05-19 23:16:46.000000 py-helper-mod-0.0.25/setup.cfg
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)    80632 2023-05-19 23:15:39.000000 py-helper-mod-0.0.25/py_helper.py
+drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-05-20 00:21:50.000000 py-helper-mod-0.0.26/
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      104 2022-03-11 16:54:40.000000 py-helper-mod-0.0.26/pyproject.toml
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      117 2022-03-11 16:54:40.000000 py-helper-mod-0.0.26/README.md
+drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-05-20 00:21:50.000000 py-helper-mod-0.0.26/py_helper_mod.egg-info/
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        1 2023-05-20 00:21:50.000000 py-helper-mod-0.0.26/py_helper_mod.egg-info/dependency_links.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       10 2023-05-20 00:21:50.000000 py-helper-mod-0.0.26/py_helper_mod.egg-info/top_level.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      212 2023-05-20 00:21:50.000000 py-helper-mod-0.0.26/py_helper_mod.egg-info/SOURCES.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      681 2023-05-20 00:21:50.000000 py-helper-mod-0.0.26/py_helper_mod.egg-info/PKG-INFO
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)     1069 2022-03-11 16:54:40.000000 py-helper-mod-0.0.26/LICENSE
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       66 2022-03-13 03:55:54.000000 py-helper-mod-0.0.26/setup.py
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      681 2023-05-20 00:21:50.000000 py-helper-mod-0.0.26/PKG-INFO
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      712 2023-05-20 00:21:50.000000 py-helper-mod-0.0.26/setup.cfg
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)    80711 2023-05-20 00:20:43.000000 py-helper-mod-0.0.26/py_helper.py
```

### Comparing `py-helper-mod-0.0.25/py_helper_mod.egg-info/PKG-INFO` & `py-helper-mod-0.0.26/py_helper_mod.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-helper-mod
-Version: 0.0.25
+Version: 0.0.26
 Summary: Collection of my helpers (functions, classes, etc)
 Home-page: https://github.com/ejohnfel/py_helper
 Author: Eric Johnfelt
 Author-email: ejohnfel@hotmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ejohnfel/py_helper/issues
 Platform: UNKNOWN
```

### Comparing `py-helper-mod-0.0.25/LICENSE` & `py-helper-mod-0.0.26/LICENSE`

 * *Files identical despite different names*

### Comparing `py-helper-mod-0.0.25/PKG-INFO` & `py-helper-mod-0.0.26/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-helper-mod
-Version: 0.0.25
+Version: 0.0.26
 Summary: Collection of my helpers (functions, classes, etc)
 Home-page: https://github.com/ejohnfel/py_helper
 Author: Eric Johnfelt
 Author-email: ejohnfel@hotmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ejohnfel/py_helper/issues
 Platform: UNKNOWN
```

### Comparing `py-helper-mod-0.0.25/setup.cfg` & `py-helper-mod-0.0.26/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 formats = zip,tar
 
 [bdist_wheel]
 universal = 1
 
 [metadata]
 name = py-helper-mod
-version = 0.0.25
+version = 0.0.26
 author = Eric Johnfelt
 author_email = ejohnfel@hotmail.com
 description = Collection of my helpers (functions, classes, etc)
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ejohnfel/py_helper
 project_urls =
```

### Comparing `py-helper-mod-0.0.25/py_helper.py` & `py-helper-mod-0.0.26/py_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -899,15 +899,15 @@
 		return self.gap
 
 #
 # Module Variables and Constants
 #
 
 # Version (Mine, and PEP defactos)
-VERSION=(0,0,25)
+VERSION=(0,0,26)
 Version = __version__ = ".".join([ str(x) for x in VERSION ])
 
 # Start Random Generator
 random.seed()
 
 # Signals Debug mode operations
 __DebugMode__ = False
@@ -1124,15 +1124,15 @@
 	if os.path.exists(filename):
 		DebugEnabled = dict()
 
 		with open(filename,"r",newline='') as csvfile:
 			reader = csv.reader(csvfile)
 
 			for row in reader:
-				DebugEnabled[row[0]] = bool(row[1])
+				DebugEnabled[row[0]] = True if row[1] in [ "True","true","TRUE","Yes","yes","y","Y" ] else False
 
 def IsDebugEnabled(dbglabel):
 	"""Check if Debug Label is Enabled"""
 
 	global DebugEnabled
 
 	enabled = True
@@ -1207,15 +1207,15 @@
 	fast debugging. It is INTENDED that they will be removed once the debugging sequence
 	is completed.
 	"""
 
 	if callerframe == None:
 		callerframe = inspect.currentframe().f_back
 
-	DbgMsg(f"{msg}",prefix=prefix,timestamp=timestamp,end=end,file=file,flush=flush,break_point=break_point,iftrue=iftrue,iffalse=iffalse,callerframe=callerframe)
+	DbgMsg(f"{msg}",prefix=prefix,timestamp=timestamp,end=end,file=file,flush=flush,break_point=break_point,iftrue=iftrue,iffalse=iffalse,callerframe=callerframe,dbglabel=dbglabel)
 
 # Not Implemented yet Convenience Function
 def NotImplementedYet(msg=None,prefix=">>>"):
 	"""Not Implemented yet Convenience Function"""
 
 	Msg("{} Not Implemented Yet : {}".format(prefix,msg) if msg != None else "{} Not Implemented Yet".format(prefix))
```

