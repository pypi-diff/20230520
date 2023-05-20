# Comparing `tmp/edl-mod-0.0.33.tar.gz` & `tmp/edl-mod-0.0.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/srv/storage/projects/scripts/edl/dist/tmpz_fpwv28/edl-mod-0.0.33.tar", last modified: Fri May 19 17:24:41 2023, max compression
+gzip compressed data, was "/srv/storage/projects/scripts/edl/dist/tmpxu5_n4jb/edl-mod-0.0.34.tar", last modified: Sat May 20 03:14:47 2023, max compression
```

## Comparing `edl-mod-0.0.33.tar` & `edl-mod-0.0.34.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-05-19 17:24:41.000000 edl-mod-0.0.33/
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      104 2022-03-11 14:46:04.000000 edl-mod-0.0.33/pyproject.toml
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)    46538 2023-05-19 17:24:13.000000 edl-mod-0.0.33/edl.py
-drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-05-19 17:24:41.000000 edl-mod-0.0.33/edl_mod.egg-info/
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       14 2023-05-19 17:24:41.000000 edl-mod-0.0.33/edl_mod.egg-info/requires.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        1 2023-05-19 17:24:41.000000 edl-mod-0.0.33/edl_mod.egg-info/dependency_links.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        4 2023-05-19 17:24:41.000000 edl-mod-0.0.33/edl_mod.egg-info/top_level.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      212 2023-05-19 17:24:41.000000 edl-mod-0.0.33/edl_mod.egg-info/SOURCES.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      659 2023-05-19 17:24:41.000000 edl-mod-0.0.33/edl_mod.egg-info/PKG-INFO
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      100 2022-03-11 15:35:21.000000 edl-mod-0.0.33/README.md
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)     1070 2022-03-11 14:39:52.000000 edl-mod-0.0.33/LICENSE
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       66 2022-03-13 05:45:40.000000 edl-mod-0.0.33/setup.py
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      659 2023-05-19 17:24:41.000000 edl-mod-0.0.33/PKG-INFO
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      734 2023-05-19 17:24:41.000000 edl-mod-0.0.33/setup.cfg
+drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-05-20 03:14:47.000000 edl-mod-0.0.34/
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      104 2022-03-11 14:46:04.000000 edl-mod-0.0.34/pyproject.toml
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)    46637 2023-05-20 03:13:45.000000 edl-mod-0.0.34/edl.py
+drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-05-20 03:14:47.000000 edl-mod-0.0.34/edl_mod.egg-info/
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       14 2023-05-20 03:14:47.000000 edl-mod-0.0.34/edl_mod.egg-info/requires.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        1 2023-05-20 03:14:47.000000 edl-mod-0.0.34/edl_mod.egg-info/dependency_links.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        4 2023-05-20 03:14:47.000000 edl-mod-0.0.34/edl_mod.egg-info/top_level.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      212 2023-05-20 03:14:47.000000 edl-mod-0.0.34/edl_mod.egg-info/SOURCES.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      659 2023-05-20 03:14:47.000000 edl-mod-0.0.34/edl_mod.egg-info/PKG-INFO
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      100 2022-03-11 15:35:21.000000 edl-mod-0.0.34/README.md
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)     1070 2022-03-11 14:39:52.000000 edl-mod-0.0.34/LICENSE
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       66 2022-03-13 05:45:40.000000 edl-mod-0.0.34/setup.py
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      659 2023-05-20 03:14:47.000000 edl-mod-0.0.34/PKG-INFO
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      734 2023-05-20 03:14:47.000000 edl-mod-0.0.34/setup.cfg
```

### Comparing `edl-mod-0.0.33/edl.py` & `edl-mod-0.0.34/edl.py`

 * *Files 1% similar despite different names*

```diff
@@ -714,15 +714,15 @@
 # Explicit No Prompt
 NoPrompt=False
 
 # Autosave EDLFIle
 AutoSave=False
 
 # Version
-VERSION=(0,0,33)
+VERSION=(0,0,34)
 Version = __version__ = ".".join([ str(x) for x in VERSION ])
 
 # Parser
 __Parser__ = None
 
 # Config File
 __Config__ = "/etc/edl/config"
@@ -901,14 +901,16 @@
 def Excluded(ip,exclude_file=None):
 	"""
 	Determine if the supplied IP string appears inside the exclude file, if an exclude file is supplied and exists.
 	"""
 
 	global Excludes
 
+	DbgMsg("Entering edl::Excluded",dbglabel="edl")
+
 	excluded = False
 
 	if exclude_file == None: exclude_file = Excludes
 
 	if ValidIP(ip) and exclude_file and os.path.exists(exclude_file):
 		with open(exclude_file,"rt") as excludes:
 			for entry in excludes:
@@ -924,14 +926,16 @@
 						excluded = True
 						Audit(AuditMsg_Excluded.format(ip))
 						break
 				elif item == ip:
 					excluded = True
 					break
 
+	DbgMsg("Exiting edl::Excluded",dbglabel="edl")
+
 	return excluded
 
 # Find Single Entry
 def FindEntry(ip,masterfile=None):
 	"""
 	Find a Block Entry in the EDL
 	"""
```

### Comparing `edl-mod-0.0.33/edl_mod.egg-info/PKG-INFO` & `edl-mod-0.0.34/edl_mod.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edl-mod
-Version: 0.0.33
+Version: 0.0.34
 Summary: Module for editting and searching external dynamic lists (EDLs)
 Home-page: https://github.com/ejohnfel/edl
 Author: Eric Johnfelt
 Author-email: ejohnfel@hotmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ejohnfel/edl/issues
 Platform: UNKNOWN
```

### Comparing `edl-mod-0.0.33/LICENSE` & `edl-mod-0.0.34/LICENSE`

 * *Files identical despite different names*

### Comparing `edl-mod-0.0.33/PKG-INFO` & `edl-mod-0.0.34/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edl-mod
-Version: 0.0.33
+Version: 0.0.34
 Summary: Module for editting and searching external dynamic lists (EDLs)
 Home-page: https://github.com/ejohnfel/edl
 Author: Eric Johnfelt
 Author-email: ejohnfel@hotmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ejohnfel/edl/issues
 Platform: UNKNOWN
```

### Comparing `edl-mod-0.0.33/setup.cfg` & `edl-mod-0.0.34/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 formats = zip,tar
 
 [bdist_wheel]
 universal = 1
 
 [metadata]
 name = edl-mod
-version = 0.0.33
+version = 0.0.34
 author = Eric Johnfelt
 author_email = ejohnfel@hotmail.com
 description = Module for editting and searching external dynamic lists (EDLs)
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ejohnfel/edl
 project_urls =
```

