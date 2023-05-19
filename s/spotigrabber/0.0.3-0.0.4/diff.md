# Comparing `tmp/spotigrabber-0.0.3.tar.gz` & `tmp/spotigrabber-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotigrabber-0.0.3.tar", last modified: Fri May 19 22:11:22 2023, max compression
+gzip compressed data, was "spotigrabber-0.0.4.tar", last modified: Fri May 19 22:21:24 2023, max compression
```

## Comparing `spotigrabber-0.0.3.tar` & `spotigrabber-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 22:11:22.266555 spotigrabber-0.0.3/
--rw-rw-rw-   0        0        0     1091 2023-04-25 09:38:20.000000 spotigrabber-0.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0     3653 2023-05-19 22:11:22.266555 spotigrabber-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3155 2023-05-19 06:43:57.000000 spotigrabber-0.0.3/README.md
--rw-rw-rw-   0        0        0      996 2023-05-19 22:10:11.000000 spotigrabber-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-19 22:11:22.266555 spotigrabber-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-19 22:11:22.219685 spotigrabber-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-19 22:11:22.235306 spotigrabber-0.0.3/src/spotigrabber/
--rw-rw-rw-   0        0        0     9379 2023-05-18 09:53:53.000000 spotigrabber-0.0.3/src/spotigrabber/spotigrabber.py
-drwxrwxrwx   0        0        0        0 2023-05-19 22:11:22.266555 spotigrabber-0.0.3/src/spotigrabber.egg-info/
--rw-rw-rw-   0        0        0     3653 2023-05-19 22:11:22.000000 spotigrabber-0.0.3/src/spotigrabber.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2023-05-19 22:11:22.000000 spotigrabber-0.0.3/src/spotigrabber.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 22:11:22.000000 spotigrabber-0.0.3/src/spotigrabber.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      302 2023-05-19 22:11:22.000000 spotigrabber-0.0.3/src/spotigrabber.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-19 22:11:22.000000 spotigrabber-0.0.3/src/spotigrabber.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 22:21:24.330189 spotigrabber-0.0.4/
+-rw-rw-rw-   0        0        0     1091 2023-04-25 09:38:20.000000 spotigrabber-0.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     3653 2023-05-19 22:21:24.330189 spotigrabber-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3155 2023-05-19 06:43:57.000000 spotigrabber-0.0.4/README.md
+-rw-rw-rw-   0        0        0      925 2023-05-19 22:20:59.000000 spotigrabber-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-19 22:21:24.330189 spotigrabber-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-19 22:21:24.283318 spotigrabber-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-19 22:21:24.298941 spotigrabber-0.0.4/src/spotigrabber/
+-rw-rw-rw-   0        0        0     9379 2023-05-18 09:53:53.000000 spotigrabber-0.0.4/src/spotigrabber/spotigrabber.py
+drwxrwxrwx   0        0        0        0 2023-05-19 22:21:24.330189 spotigrabber-0.0.4/src/spotigrabber.egg-info/
+-rw-rw-rw-   0        0        0     3653 2023-05-19 22:21:24.000000 spotigrabber-0.0.4/src/spotigrabber.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2023-05-19 22:21:24.000000 spotigrabber-0.0.4/src/spotigrabber.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 22:21:24.000000 spotigrabber-0.0.4/src/spotigrabber.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      177 2023-05-19 22:21:24.000000 spotigrabber-0.0.4/src/spotigrabber.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-19 22:21:24.000000 spotigrabber-0.0.4/src/spotigrabber.egg-info/top_level.txt
```

### Comparing `spotigrabber-0.0.3/LICENSE.txt` & `spotigrabber-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `spotigrabber-0.0.3/PKG-INFO` & `spotigrabber-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotigrabber
-Version: 0.0.3
+Version: 0.0.4
 Summary: Grabber your spotify playlists and recently played songs.
 Author-email: bebissig <bebissig@gmail.com>
 Project-URL: Homepage, https://github.com/bebissig/spotify_grab_current_playlists
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `spotigrabber-0.0.3/README.md` & `spotigrabber-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `spotigrabber-0.0.3/pyproject.toml` & `spotigrabber-0.0.4/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "spotigrabber"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="bebissig", email="bebissig@gmail.com" },
 ]
 description = "Grabber your spotify playlists and recently played songs."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-	"async-timeout==4.0.2",
-	"certifi==2023.5.7",
-	"charset-normalizer==3.1.0",
-	"et-xmlfile==1.1.0",
-	"idna==3.4",
-	"importlib-metadata==6.6.0",
-	"numpy",
-	"openpyxl==3.1.2",
-	"pandas==1.3.5",
-	"python-dateutil==2.8.2",
-	"pytz==2023.3",
-	"redis==4.5.5",
-	"requests==2.30.0",
-	"six==1.16.0",
-	"spotipy==2.23.0",
-	"typing-extensions==4.5.0",
-	"urllib3==2.0.2",
-	"zipp==3.15.0"
+    "async-timeout",
+    "certifi",
+    "charset-normalizer",
+    "et-xmlfile",
+    "idna",
+    "importlib-metadata",
+    "numpy",
+    "openpyxl",
+    "pandas",
+    "python-dateutil",
+    "pytz",
+    "redis",
+    "requests",
+    "six",
+    "spotipy",
+    "typing-extensions",
+    "urllib3",
+    "zipp"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/bebissig/spotify_grab_current_playlists"
```

### Comparing `spotigrabber-0.0.3/src/spotigrabber/spotigrabber.py` & `spotigrabber-0.0.4/src/spotigrabber/spotigrabber.py`

 * *Files identical despite different names*

### Comparing `spotigrabber-0.0.3/src/spotigrabber.egg-info/PKG-INFO` & `spotigrabber-0.0.4/src/spotigrabber.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotigrabber
-Version: 0.0.3
+Version: 0.0.4
 Summary: Grabber your spotify playlists and recently played songs.
 Author-email: bebissig <bebissig@gmail.com>
 Project-URL: Homepage, https://github.com/bebissig/spotify_grab_current_playlists
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

