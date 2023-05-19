# Comparing `tmp/py-helper-mod-0.0.24.tar.gz` & `tmp/py-helper-mod-0.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/srv/storage/projects/scripts/py_helper/dist/tmp5cciwnzh/py-helper-mod-0.0.24.tar", last modified: Sun May  7 03:27:35 2023, max compression
+gzip compressed data, was "/srv/storage/projects/scripts/py_helper/dist/tmphqmetzev/py-helper-mod-0.0.25.tar", last modified: Fri May 19 23:16:46 2023, max compression
```

## Comparing `py-helper-mod-0.0.24.tar` & `py-helper-mod-0.0.25.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-05-07 03:27:35.000000 py-helper-mod-0.0.24/
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      104 2022-03-11 16:54:40.000000 py-helper-mod-0.0.24/pyproject.toml
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      117 2022-03-11 16:54:40.000000 py-helper-mod-0.0.24/README.md
-drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-05-07 03:27:35.000000 py-helper-mod-0.0.24/py_helper_mod.egg-info/
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        1 2023-05-07 03:27:35.000000 py-helper-mod-0.0.24/py_helper_mod.egg-info/dependency_links.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       10 2023-05-07 03:27:35.000000 py-helper-mod-0.0.24/py_helper_mod.egg-info/top_level.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      212 2023-05-07 03:27:35.000000 py-helper-mod-0.0.24/py_helper_mod.egg-info/SOURCES.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      681 2023-05-07 03:27:35.000000 py-helper-mod-0.0.24/py_helper_mod.egg-info/PKG-INFO
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)     1069 2022-03-11 16:54:40.000000 py-helper-mod-0.0.24/LICENSE
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       66 2022-03-13 03:55:54.000000 py-helper-mod-0.0.24/setup.py
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      681 2023-05-07 03:27:35.000000 py-helper-mod-0.0.24/PKG-INFO
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      712 2023-05-07 03:27:35.000000 py-helper-mod-0.0.24/setup.cfg
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)    79547 2023-05-07 03:26:17.000000 py-helper-mod-0.0.24/py_helper.py
+drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-05-19 23:16:46.000000 py-helper-mod-0.0.25/
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      104 2022-03-11 16:54:40.000000 py-helper-mod-0.0.25/pyproject.toml
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      117 2022-03-11 16:54:40.000000 py-helper-mod-0.0.25/README.md
+drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-05-19 23:16:46.000000 py-helper-mod-0.0.25/py_helper_mod.egg-info/
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        1 2023-05-19 23:16:46.000000 py-helper-mod-0.0.25/py_helper_mod.egg-info/dependency_links.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       10 2023-05-19 23:16:46.000000 py-helper-mod-0.0.25/py_helper_mod.egg-info/top_level.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      212 2023-05-19 23:16:46.000000 py-helper-mod-0.0.25/py_helper_mod.egg-info/SOURCES.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      681 2023-05-19 23:16:46.000000 py-helper-mod-0.0.25/py_helper_mod.egg-info/PKG-INFO
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)     1069 2022-03-11 16:54:40.000000 py-helper-mod-0.0.25/LICENSE
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       66 2022-03-13 03:55:54.000000 py-helper-mod-0.0.25/setup.py
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      681 2023-05-19 23:16:46.000000 py-helper-mod-0.0.25/PKG-INFO
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      712 2023-05-19 23:16:46.000000 py-helper-mod-0.0.25/setup.cfg
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)    80632 2023-05-19 23:15:39.000000 py-helper-mod-0.0.25/py_helper.py
```

### Comparing `py-helper-mod-0.0.24/py_helper_mod.egg-info/PKG-INFO` & `py-helper-mod-0.0.25/py_helper_mod.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-helper-mod
-Version: 0.0.24
+Version: 0.0.25
 Summary: Collection of my helpers (functions, classes, etc)
 Home-page: https://github.com/ejohnfel/py_helper
 Author: Eric Johnfelt
 Author-email: ejohnfel@hotmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ejohnfel/py_helper/issues
 Platform: UNKNOWN
```

### Comparing `py-helper-mod-0.0.24/LICENSE` & `py-helper-mod-0.0.25/LICENSE`

 * *Files identical despite different names*

### Comparing `py-helper-mod-0.0.24/PKG-INFO` & `py-helper-mod-0.0.25/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-helper-mod
-Version: 0.0.24
+Version: 0.0.25
 Summary: Collection of my helpers (functions, classes, etc)
 Home-page: https://github.com/ejohnfel/py_helper
 Author: Eric Johnfelt
 Author-email: ejohnfel@hotmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ejohnfel/py_helper/issues
 Platform: UNKNOWN
```

### Comparing `py-helper-mod-0.0.24/setup.cfg` & `py-helper-mod-0.0.25/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 formats = zip,tar
 
 [bdist_wheel]
 universal = 1
 
 [metadata]
 name = py-helper-mod
-version = 0.0.24
+version = 0.0.25
 author = Eric Johnfelt
 author_email = ejohnfel@hotmail.com
 description = Collection of my helpers (functions, classes, etc)
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ejohnfel/py_helper
 project_urls =
```

### Comparing `py-helper-mod-0.0.24/py_helper.py` & `py-helper-mod-0.0.25/py_helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -899,22 +899,26 @@
 		return self.gap
 
 #
 # Module Variables and Constants
 #
 
 # Version (Mine, and PEP defactos)
-VERSION=(0,0,24)
+VERSION=(0,0,25)
 Version = __version__ = ".".join([ str(x) for x in VERSION ])
 
 # Start Random Generator
 random.seed()
 
 # Signals Debug mode operations
 __DebugMode__ = False
+
+# Debug/Breakpoint Flags
+DebugEnabled = None
+
 # Signals Module is being used in Cmd Line Mode
 __CmdLineMode__ = False
 
 # Notes:
 # DebugMode puts the module in DebugMode, i.e. it activates DbgMsg() to output
 # 	when DebugMode is false, DbgMsg does nothing.
 # CmdLineMode informs the module that it should behave like it was called as a script.
@@ -1085,26 +1089,80 @@
 	# Logfile/Teefile works no matter what mode module is in
 	if Logfile != None:
 		Log(msg,logfile=Logfile)
 
 	if Teefile != None:
 		Log(msg,logfile=Teefile)
 
+def SetDebugLabel(dbglabel,value):
+	"""Enable Debug Label"""
+
+	global DebugEnabled
+
+	if DebugEnabled is not None:
+		DebugEnabled[dbglabel] = value
+
+def EnableDebugLabel(dbglabel):
+	"""Enable Debug Label"""
+
+	SetDebugLabel(dbglabel,True)
+
+def DisableDebugLabel(dbglabel):
+	"""Disable Debug Label"""
+
+	SetDebugLabel(dbglabel,False)
+
+def LoadDebugEnableFile(filename):
+	"""Load Debug Enablement Data File"""
+
+	global DebugEnabled
+
+	if DebugEnabled is not None:
+		del DebugEnabled
+
+	DebugEnabled = None
+
+	if os.path.exists(filename):
+		DebugEnabled = dict()
+
+		with open(filename,"r",newline='') as csvfile:
+			reader = csv.reader(csvfile)
+
+			for row in reader:
+				DebugEnabled[row[0]] = bool(row[1])
+
+def IsDebugEnabled(dbglabel):
+	"""Check if Debug Label is Enabled"""
+
+	global DebugEnabled
+
+	enabled = True
+
+	if DebugEnabled is not None and dbglabel is not None:
+		if dbglabel in DebugEnabled:
+			enabled = DebugEnabled[dbglabel]
+
+	return enabled
+
 # A Centrally Controlled Debug Messaging System
 # msg : Message to print
 # func : A simple function to pass the message to (optional)
 # If "func" is supplied, DbgMsg uses it for output instead of printing to stdout
-def DbgMsg(msg,func=None,prefix="***",timestamp=False,end="\n",file=sys.stdout,flush=True,break_point=False,iftrue=None,iffalse=None,callerframe=None,interval_stamp=None):
+def DbgMsg(msg,func=None,prefix="***",timestamp=False,end="\n",file=sys.stdout,flush=True,break_point=False,iftrue=None,iffalse=None,callerframe=None,interval_stamp=None,dbglabel=None):
 	"""
 	Messaging function that only prints when in DebugMode.
 	Ignores CmdLineMode/ModuleMode.
 	"""
-	global __DebugMode__
+
+	global __DebugMode__, DebugEnabled
 
 	if __DebugMode__:
+		if not IsDebugEnabled(dbglabel):
+			return
+
 		delta = None
 
 		int_stamp = DbgMsg.__annotations__.get("interval_stamp",None)
 
 		if int_stamp != None:
 			delta = datetime.now() - int_stamp
 			DbgMsg.__annotations__["interval_stamp"] = None
@@ -1137,15 +1195,15 @@
 
 		Msg(adjusted,func,ignoreModuleMode=True,end=end,file=file,flush=flush)
 
 		if break_point:
 			breakpoint()
 
 # DbgAuto Messages
-def DbgAuto(msg="Auto Dbg",prefix="***",callerframe=None,timestamp=False,end="\n",file=sys.stdout,flush=True,break_point=False,iftrue=None,iffalse=None):
+def DbgAuto(msg="Auto Dbg",prefix="***",callerframe=None,timestamp=False,end="\n",file=sys.stdout,flush=True,break_point=False,iftrue=None,iffalse=None,dbglabel=None):
 	"""
 	Generate an Automated DbgMsg With File-Line number and optional msg
 
 	Generally the purpose here is generate temporary debug scaffolding messages for
 	fast debugging. It is INTENDED that they will be removed once the debugging sequence
 	is completed.
 	"""
```

