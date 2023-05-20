# Comparing `tmp/TMDBTraktSyncer-1.1.2.tar.gz` & `tmp/TMDBTraktSyncer-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TMDBTraktSyncer-1.1.2.tar", last modified: Sat May 20 20:08:45 2023, max compression
+gzip compressed data, was "TMDBTraktSyncer-1.1.3.tar", last modified: Sat May 20 20:13:38 2023, max compression
```

## Comparing `TMDBTraktSyncer-1.1.2.tar` & `TMDBTraktSyncer-1.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 20:08:45.475974 TMDBTraktSyncer-1.1.2/
--rw-rw-rw-   0        0        0     1079 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.1.2/LICENSE
--rw-rw-rw-   0        0        0     6468 2023-05-20 20:08:45.474972 TMDBTraktSyncer-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     5795 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-20 20:08:45.447020 TMDBTraktSyncer-1.1.2/TMDBTraktSyncer/
--rw-rw-rw-   0        0        0     5695 2023-05-20 19:53:04.000000 TMDBTraktSyncer-1.1.2/TMDBTraktSyncer/TMDBTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.1.2/TMDBTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     1928 2023-05-20 19:53:06.000000 TMDBTraktSyncer-1.1.2/TMDBTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0     8916 2023-05-20 19:53:06.000000 TMDBTraktSyncer-1.1.2/TMDBTraktSyncer/errorHandling.py
--rw-rw-rw-   0        0        0     2991 2023-05-20 20:06:38.000000 TMDBTraktSyncer-1.1.2/TMDBTraktSyncer/tmdbRatings.py
--rw-rw-rw-   0        0        0     2168 2023-05-20 19:53:04.000000 TMDBTraktSyncer-1.1.2/TMDBTraktSyncer/traktRatings.py
--rw-rw-rw-   0        0        0     1834 2023-05-20 19:53:05.000000 TMDBTraktSyncer-1.1.2/TMDBTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-05-20 20:08:45.472978 TMDBTraktSyncer-1.1.2/TMDBTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0     6468 2023-05-20 20:08:45.000000 TMDBTraktSyncer-1.1.2/TMDBTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      487 2023-05-20 20:08:45.000000 TMDBTraktSyncer-1.1.2/TMDBTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 20:08:45.000000 TMDBTraktSyncer-1.1.2/TMDBTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-05-20 20:08:45.000000 TMDBTraktSyncer-1.1.2/TMDBTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-05-20 20:08:45.000000 TMDBTraktSyncer-1.1.2/TMDBTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-20 20:08:45.000000 TMDBTraktSyncer-1.1.2/TMDBTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-20 20:08:45.475974 TMDBTraktSyncer-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1291 2023-05-20 20:08:26.000000 TMDBTraktSyncer-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 20:13:38.132576 TMDBTraktSyncer-1.1.3/
+-rw-rw-rw-   0        0        0     1079 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0     6468 2023-05-20 20:13:38.131566 TMDBTraktSyncer-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5795 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-20 20:13:38.102288 TMDBTraktSyncer-1.1.3/TMDBTraktSyncer/
+-rw-rw-rw-   0        0        0     5677 2023-05-20 20:12:07.000000 TMDBTraktSyncer-1.1.3/TMDBTraktSyncer/TMDBTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.1.3/TMDBTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     1928 2023-05-20 19:53:06.000000 TMDBTraktSyncer-1.1.3/TMDBTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0     8916 2023-05-20 19:53:06.000000 TMDBTraktSyncer-1.1.3/TMDBTraktSyncer/errorHandling.py
+-rw-rw-rw-   0        0        0     2991 2023-05-20 20:06:38.000000 TMDBTraktSyncer-1.1.3/TMDBTraktSyncer/tmdbData.py
+-rw-rw-rw-   0        0        0     2168 2023-05-20 19:53:04.000000 TMDBTraktSyncer-1.1.3/TMDBTraktSyncer/traktData.py
+-rw-rw-rw-   0        0        0     1834 2023-05-20 19:53:05.000000 TMDBTraktSyncer-1.1.3/TMDBTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-05-20 20:13:38.129566 TMDBTraktSyncer-1.1.3/TMDBTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0     6468 2023-05-20 20:13:37.000000 TMDBTraktSyncer-1.1.3/TMDBTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      481 2023-05-20 20:13:38.000000 TMDBTraktSyncer-1.1.3/TMDBTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 20:13:37.000000 TMDBTraktSyncer-1.1.3/TMDBTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-05-20 20:13:37.000000 TMDBTraktSyncer-1.1.3/TMDBTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-05-20 20:13:37.000000 TMDBTraktSyncer-1.1.3/TMDBTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-20 20:13:37.000000 TMDBTraktSyncer-1.1.3/TMDBTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-20 20:13:38.132576 TMDBTraktSyncer-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1291 2023-05-20 20:13:05.000000 TMDBTraktSyncer-1.1.3/setup.py
```

### Comparing `TMDBTraktSyncer-1.1.2/LICENSE` & `TMDBTraktSyncer-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.1.2/PKG-INFO` & `TMDBTraktSyncer-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TMDBTraktSyncer
-Version: 1.1.2
+Version: 1.1.3
 Summary: This python script will sync user ratings for Movies and TV Shows both ways between Trakt and TMDB.
 Home-page: https://github.com/RileyXX/TMDB-Trakt-Syncer
 Keywords: python,video,trakt,tmdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `TMDBTraktSyncer-1.1.2/README.md` & `TMDBTraktSyncer-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.1.2/TMDBTraktSyncer/TMDBTraktSyncer.py` & `TMDBTraktSyncer-1.1.3/TMDBTraktSyncer/TMDBTraktSyncer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import json
 import requests
 import time
 try:
     from TMDBTraktSyncer import verifyCredentials
-    from TMDBTraktSyncer import traktRatings
-    from TMDBTraktSyncer import tmdbRatings
+    from TMDBTraktSyncer import traktData
+    from TMDBTraktSyncer import tmdbData
     from TMDBTraktSyncer import errorHandling as EH
 except ImportError:
     import verifyCredentials
-    import traktRatings
-    import tmdbRatings
+    import traktData
+    import tmdbData
     import errorHandling as EH
 
 
 def main():
     try:
 
         #Get credentials
         trakt_client_id = verifyCredentials.trakt_client_id
         trakt_access_token = verifyCredentials.trakt_access_token
         tmdb_v4_token = verifyCredentials.tmdb_v4_token
         
             
-        trakt_ratings = traktRatings.getTraktRatings(trakt_client_id, trakt_access_token)
-        tmdb_ratings = tmdbRatings.getTMDBRatings(tmdb_v4_token)
+        trakt_ratings = traktData.getTraktRatings(trakt_client_id, trakt_access_token)
+        tmdb_ratings = tmdbData.getTMDBRatings(tmdb_v4_token)
 
         #Get trakt and tmdb ratings and filter out trakt ratings with missing tmdb id
         trakt_ratings = [rating for rating in trakt_ratings if rating['ID'] is not None]
         tmdb_ratings = [rating for rating in tmdb_ratings if rating['ID'] is not None]
         #Filter out ratings already set
         tmdb_ratings_to_set = [rating for rating in trakt_ratings if rating['ID'] not in [tmdb_rating['ID'] for tmdb_rating in tmdb_ratings]]
         trakt_ratings_to_set = [rating for rating in tmdb_ratings if rating['ID'] not in [trakt_rating['ID'] for trakt_rating in trakt_ratings]]
```

### Comparing `TMDBTraktSyncer-1.1.2/TMDBTraktSyncer/authTrakt.py` & `TMDBTraktSyncer-1.1.3/TMDBTraktSyncer/authTrakt.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.1.2/TMDBTraktSyncer/errorHandling.py` & `TMDBTraktSyncer-1.1.3/TMDBTraktSyncer/errorHandling.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.1.2/TMDBTraktSyncer/tmdbRatings.py` & `TMDBTraktSyncer-1.1.3/TMDBTraktSyncer/tmdbData.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.1.2/TMDBTraktSyncer/traktRatings.py` & `TMDBTraktSyncer-1.1.3/TMDBTraktSyncer/traktData.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.1.2/TMDBTraktSyncer/verifyCredentials.py` & `TMDBTraktSyncer-1.1.3/TMDBTraktSyncer/verifyCredentials.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.1.2/TMDBTraktSyncer.egg-info/PKG-INFO` & `TMDBTraktSyncer-1.1.3/TMDBTraktSyncer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TMDBTraktSyncer
-Version: 1.1.2
+Version: 1.1.3
 Summary: This python script will sync user ratings for Movies and TV Shows both ways between Trakt and TMDB.
 Home-page: https://github.com/RileyXX/TMDB-Trakt-Syncer
 Keywords: python,video,trakt,tmdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `TMDBTraktSyncer-1.1.2/setup.py` & `TMDBTraktSyncer-1.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.1.2'
+VERSION = '1.1.3'
 DESCRIPTION = 'This python script will sync user ratings for Movies and TV Shows both ways between Trakt and TMDB.'
 
 # Setting up
 setup(
     name="TMDBTraktSyncer",
     version=VERSION,
     description=DESCRIPTION,
```

