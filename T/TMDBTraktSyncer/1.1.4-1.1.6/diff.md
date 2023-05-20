# Comparing `tmp/TMDBTraktSyncer-1.1.4.tar.gz` & `tmp/TMDBTraktSyncer-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TMDBTraktSyncer-1.1.4.tar", last modified: Sat May 20 20:23:08 2023, max compression
+gzip compressed data, was "TMDBTraktSyncer-1.1.6.tar", last modified: Sat May 20 21:44:11 2023, max compression
```

## Comparing `TMDBTraktSyncer-1.1.4.tar` & `TMDBTraktSyncer-1.1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 20:23:08.668218 TMDBTraktSyncer-1.1.4/
--rw-rw-rw-   0        0        0     1079 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.1.4/LICENSE
--rw-rw-rw-   0        0        0     6468 2023-05-20 20:23:08.667218 TMDBTraktSyncer-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     5795 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-20 20:23:08.644504 TMDBTraktSyncer-1.1.4/TMDBTraktSyncer/
--rw-rw-rw-   0        0        0     5677 2023-05-20 20:12:07.000000 TMDBTraktSyncer-1.1.4/TMDBTraktSyncer/TMDBTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.1.4/TMDBTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     1928 2023-05-20 19:53:06.000000 TMDBTraktSyncer-1.1.4/TMDBTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0     8916 2023-05-20 19:53:06.000000 TMDBTraktSyncer-1.1.4/TMDBTraktSyncer/errorHandling.py
--rw-rw-rw-   0        0        0     2918 2023-05-20 20:21:56.000000 TMDBTraktSyncer-1.1.4/TMDBTraktSyncer/tmdbData.py
--rw-rw-rw-   0        0        0     2168 2023-05-20 19:53:04.000000 TMDBTraktSyncer-1.1.4/TMDBTraktSyncer/traktData.py
--rw-rw-rw-   0        0        0     1834 2023-05-20 19:53:05.000000 TMDBTraktSyncer-1.1.4/TMDBTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-05-20 20:23:08.665223 TMDBTraktSyncer-1.1.4/TMDBTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0     6468 2023-05-20 20:23:08.000000 TMDBTraktSyncer-1.1.4/TMDBTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      481 2023-05-20 20:23:08.000000 TMDBTraktSyncer-1.1.4/TMDBTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 20:23:08.000000 TMDBTraktSyncer-1.1.4/TMDBTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-05-20 20:23:08.000000 TMDBTraktSyncer-1.1.4/TMDBTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-05-20 20:23:08.000000 TMDBTraktSyncer-1.1.4/TMDBTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-20 20:23:08.000000 TMDBTraktSyncer-1.1.4/TMDBTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-20 20:23:08.668218 TMDBTraktSyncer-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1291 2023-05-20 20:23:04.000000 TMDBTraktSyncer-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 21:44:11.632901 TMDBTraktSyncer-1.1.6/
+-rw-rw-rw-   0        0        0     1079 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.1.6/LICENSE
+-rw-rw-rw-   0        0        0     6468 2023-05-20 21:44:11.631913 TMDBTraktSyncer-1.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     5795 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-20 21:44:11.611759 TMDBTraktSyncer-1.1.6/TMDBTraktSyncer/
+-rw-rw-rw-   0        0        0     5677 2023-05-20 20:12:07.000000 TMDBTraktSyncer-1.1.6/TMDBTraktSyncer/TMDBTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.1.6/TMDBTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     1928 2023-05-20 19:53:06.000000 TMDBTraktSyncer-1.1.6/TMDBTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0     8916 2023-05-20 19:53:06.000000 TMDBTraktSyncer-1.1.6/TMDBTraktSyncer/errorHandling.py
+-rw-rw-rw-   0        0        0     2918 2023-05-20 20:21:56.000000 TMDBTraktSyncer-1.1.6/TMDBTraktSyncer/tmdbData.py
+-rw-rw-rw-   0        0        0     2263 2023-05-20 21:38:06.000000 TMDBTraktSyncer-1.1.6/TMDBTraktSyncer/traktData.py
+-rw-rw-rw-   0        0        0     1834 2023-05-20 19:53:05.000000 TMDBTraktSyncer-1.1.6/TMDBTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-05-20 21:44:11.629900 TMDBTraktSyncer-1.1.6/TMDBTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0     6468 2023-05-20 21:44:11.000000 TMDBTraktSyncer-1.1.6/TMDBTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      481 2023-05-20 21:44:11.000000 TMDBTraktSyncer-1.1.6/TMDBTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 21:44:11.000000 TMDBTraktSyncer-1.1.6/TMDBTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-05-20 21:44:11.000000 TMDBTraktSyncer-1.1.6/TMDBTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-05-20 21:44:11.000000 TMDBTraktSyncer-1.1.6/TMDBTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-20 21:44:11.000000 TMDBTraktSyncer-1.1.6/TMDBTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-20 21:44:11.632901 TMDBTraktSyncer-1.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1291 2023-05-20 21:44:05.000000 TMDBTraktSyncer-1.1.6/setup.py
```

### Comparing `TMDBTraktSyncer-1.1.4/LICENSE` & `TMDBTraktSyncer-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.1.4/PKG-INFO` & `TMDBTraktSyncer-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TMDBTraktSyncer
-Version: 1.1.4
+Version: 1.1.6
 Summary: This python script will sync user ratings for Movies and TV Shows both ways between Trakt and TMDB.
 Home-page: https://github.com/RileyXX/TMDB-Trakt-Syncer
 Keywords: python,video,trakt,tmdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `TMDBTraktSyncer-1.1.4/README.md` & `TMDBTraktSyncer-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.1.4/TMDBTraktSyncer/TMDBTraktSyncer.py` & `TMDBTraktSyncer-1.1.6/TMDBTraktSyncer/TMDBTraktSyncer.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.1.4/TMDBTraktSyncer/authTrakt.py` & `TMDBTraktSyncer-1.1.6/TMDBTraktSyncer/authTrakt.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.1.4/TMDBTraktSyncer/errorHandling.py` & `TMDBTraktSyncer-1.1.6/TMDBTraktSyncer/errorHandling.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.1.4/TMDBTraktSyncer/tmdbData.py` & `TMDBTraktSyncer-1.1.6/TMDBTraktSyncer/tmdbData.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.1.4/TMDBTraktSyncer/traktData.py` & `TMDBTraktSyncer-1.1.6/TMDBTraktSyncer/traktData.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import json
 import requests
+import urllib.parse
 try:
     from TMDBTraktSyncer import errorHandling as EH
 except ImportError:
     import errorHandling as EH
 
 def getTraktRatings(trakt_client_id, trakt_access_token):
     # Get Trakt Ratings
     print('Processing Trakt Ratings')
 
     response = EH.make_trakt_request('https://api.trakt.tv/users/me')
     json_data = json.loads(response.text)
-    username = json_data['username']
-    response = EH.make_trakt_request(f'https://api.trakt.tv/users/{username}/ratings')
+    username_slug = json_data['ids']['slug']
+    encoded_username = urllib.parse.quote(username_slug)
+    response = EH.make_trakt_request(f'https://api.trakt.tv/users/{encoded_username}/ratings')
     json_data = json.loads(response.text)
 
     movie_ratings = []
     show_ratings = []
     episode_ratings = []
 
     for item in json_data:
```

### Comparing `TMDBTraktSyncer-1.1.4/TMDBTraktSyncer/verifyCredentials.py` & `TMDBTraktSyncer-1.1.6/TMDBTraktSyncer/verifyCredentials.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.1.4/TMDBTraktSyncer.egg-info/PKG-INFO` & `TMDBTraktSyncer-1.1.6/TMDBTraktSyncer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TMDBTraktSyncer
-Version: 1.1.4
+Version: 1.1.6
 Summary: This python script will sync user ratings for Movies and TV Shows both ways between Trakt and TMDB.
 Home-page: https://github.com/RileyXX/TMDB-Trakt-Syncer
 Keywords: python,video,trakt,tmdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `TMDBTraktSyncer-1.1.4/setup.py` & `TMDBTraktSyncer-1.1.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.1.4'
+VERSION = '1.1.6'
 DESCRIPTION = 'This python script will sync user ratings for Movies and TV Shows both ways between Trakt and TMDB.'
 
 # Setting up
 setup(
     name="TMDBTraktSyncer",
     version=VERSION,
     description=DESCRIPTION,
```

