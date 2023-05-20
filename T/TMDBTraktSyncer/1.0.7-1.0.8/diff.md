# Comparing `tmp/TMDBTraktSyncer-1.0.7.tar.gz` & `tmp/TMDBTraktSyncer-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TMDBTraktSyncer-1.0.7.tar", last modified: Sat May 20 16:59:45 2023, max compression
+gzip compressed data, was "TMDBTraktSyncer-1.0.8.tar", last modified: Sat May 20 17:11:23 2023, max compression
```

## Comparing `TMDBTraktSyncer-1.0.7.tar` & `TMDBTraktSyncer-1.0.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 16:59:45.397021 TMDBTraktSyncer-1.0.7/
--rw-rw-rw-   0        0        0     1079 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.0.7/LICENSE
--rw-rw-rw-   0        0        0     6468 2023-05-20 16:59:45.396021 TMDBTraktSyncer-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     5795 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-20 16:59:45.364022 TMDBTraktSyncer-1.0.7/TMDBTraktSyncer/
--rw-rw-rw-   0        0        0     5773 2023-05-20 16:47:55.000000 TMDBTraktSyncer-1.0.7/TMDBTraktSyncer/TMDBTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.0.7/TMDBTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     1915 2023-05-20 16:29:13.000000 TMDBTraktSyncer-1.0.7/TMDBTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0     8822 2023-05-20 16:56:20.000000 TMDBTraktSyncer-1.0.7/TMDBTraktSyncer/errorHandling.py
--rw-rw-rw-   0        0        0     2932 2023-05-20 16:50:29.000000 TMDBTraktSyncer-1.0.7/TMDBTraktSyncer/tmdbRatings.py
--rw-rw-rw-   0        0        0     2069 2023-05-20 16:25:11.000000 TMDBTraktSyncer-1.0.7/TMDBTraktSyncer/traktRatings.py
--rw-rw-rw-   0        0        0     1822 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.0.7/TMDBTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-05-20 16:59:45.394021 TMDBTraktSyncer-1.0.7/TMDBTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0     6468 2023-05-20 16:59:45.000000 TMDBTraktSyncer-1.0.7/TMDBTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      487 2023-05-20 16:59:45.000000 TMDBTraktSyncer-1.0.7/TMDBTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 16:59:45.000000 TMDBTraktSyncer-1.0.7/TMDBTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-05-20 16:59:45.000000 TMDBTraktSyncer-1.0.7/TMDBTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-05-20 16:59:45.000000 TMDBTraktSyncer-1.0.7/TMDBTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-20 16:59:45.000000 TMDBTraktSyncer-1.0.7/TMDBTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-20 16:59:45.397021 TMDBTraktSyncer-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1291 2023-05-20 16:59:20.000000 TMDBTraktSyncer-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 17:11:23.618399 TMDBTraktSyncer-1.0.8/
+-rw-rw-rw-   0        0        0     1079 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0     6468 2023-05-20 17:11:23.617399 TMDBTraktSyncer-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     5795 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-20 17:11:23.598002 TMDBTraktSyncer-1.0.8/TMDBTraktSyncer/
+-rw-rw-rw-   0        0        0     5773 2023-05-20 16:47:55.000000 TMDBTraktSyncer-1.0.8/TMDBTraktSyncer/TMDBTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.0.8/TMDBTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     1915 2023-05-20 16:29:13.000000 TMDBTraktSyncer-1.0.8/TMDBTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0     8793 2023-05-20 17:05:25.000000 TMDBTraktSyncer-1.0.8/TMDBTraktSyncer/errorHandling.py
+-rw-rw-rw-   0        0        0     2932 2023-05-20 16:50:29.000000 TMDBTraktSyncer-1.0.8/TMDBTraktSyncer/tmdbRatings.py
+-rw-rw-rw-   0        0        0     2069 2023-05-20 16:25:11.000000 TMDBTraktSyncer-1.0.8/TMDBTraktSyncer/traktRatings.py
+-rw-rw-rw-   0        0        0     1822 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.0.8/TMDBTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-05-20 17:11:23.616399 TMDBTraktSyncer-1.0.8/TMDBTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0     6468 2023-05-20 17:11:23.000000 TMDBTraktSyncer-1.0.8/TMDBTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      487 2023-05-20 17:11:23.000000 TMDBTraktSyncer-1.0.8/TMDBTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 17:11:23.000000 TMDBTraktSyncer-1.0.8/TMDBTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-05-20 17:11:23.000000 TMDBTraktSyncer-1.0.8/TMDBTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-05-20 17:11:23.000000 TMDBTraktSyncer-1.0.8/TMDBTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-20 17:11:23.000000 TMDBTraktSyncer-1.0.8/TMDBTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-20 17:11:23.618399 TMDBTraktSyncer-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1291 2023-05-20 17:05:42.000000 TMDBTraktSyncer-1.0.8/setup.py
```

### Comparing `TMDBTraktSyncer-1.0.7/LICENSE` & `TMDBTraktSyncer-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.0.7/PKG-INFO` & `TMDBTraktSyncer-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TMDBTraktSyncer
-Version: 1.0.7
+Version: 1.0.8
 Summary: This python script will sync user ratings for Movies and TV Shows both ways between Trakt and TMDB.
 Home-page: https://github.com/RileyXX/TMDB-Trakt-Syncer
 Keywords: python,video,trakt,tmdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `TMDBTraktSyncer-1.0.7/README.md` & `TMDBTraktSyncer-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.0.7/TMDBTraktSyncer/TMDBTraktSyncer.py` & `TMDBTraktSyncer-1.0.8/TMDBTraktSyncer/TMDBTraktSyncer.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.0.7/TMDBTraktSyncer/authTrakt.py` & `TMDBTraktSyncer-1.0.8/TMDBTraktSyncer/authTrakt.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.0.7/TMDBTraktSyncer/errorHandling.py` & `TMDBTraktSyncer-1.0.8/TMDBTraktSyncer/errorHandling.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import time
 try:
     from TMDBTraktSyncer import verifyCredentials
 except:
     import verifyCredentials
 
 def report_error(error_message):
-    github_issue_url = "https://github.com/RileyXX/TMDB-Trakt-Syncer/issues/new?assignees=&labels=&projects=&template=bug_report.yml"
+    github_issue_url = "https://github.com/RileyXX/TMDB-Trakt-Syncer/issues/new?template=bug_report.yml"
     traceback_info = traceback.format_exc()
 
     print("\n--- ERROR ---")
     print(error_message)
     print("Please submit the error to GitHub with the following information:")
     print("-" * 50)
     print(traceback_info)
```

### Comparing `TMDBTraktSyncer-1.0.7/TMDBTraktSyncer/tmdbRatings.py` & `TMDBTraktSyncer-1.0.8/TMDBTraktSyncer/tmdbRatings.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.0.7/TMDBTraktSyncer/traktRatings.py` & `TMDBTraktSyncer-1.0.8/TMDBTraktSyncer/traktRatings.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.0.7/TMDBTraktSyncer/verifyCredentials.py` & `TMDBTraktSyncer-1.0.8/TMDBTraktSyncer/verifyCredentials.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.0.7/TMDBTraktSyncer.egg-info/PKG-INFO` & `TMDBTraktSyncer-1.0.8/TMDBTraktSyncer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TMDBTraktSyncer
-Version: 1.0.7
+Version: 1.0.8
 Summary: This python script will sync user ratings for Movies and TV Shows both ways between Trakt and TMDB.
 Home-page: https://github.com/RileyXX/TMDB-Trakt-Syncer
 Keywords: python,video,trakt,tmdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `TMDBTraktSyncer-1.0.7/setup.py` & `TMDBTraktSyncer-1.0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.7'
+VERSION = '1.0.8'
 DESCRIPTION = 'This python script will sync user ratings for Movies and TV Shows both ways between Trakt and TMDB.'
 
 # Setting up
 setup(
     name="TMDBTraktSyncer",
     version=VERSION,
     description=DESCRIPTION,
```

