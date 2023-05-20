# Comparing `tmp/TMDBTraktSyncer-1.1.0.tar.gz` & `tmp/TMDBTraktSyncer-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TMDBTraktSyncer-1.1.0.tar", last modified: Sat May 20 17:59:39 2023, max compression
+gzip compressed data, was "TMDBTraktSyncer-1.1.1.tar", last modified: Sat May 20 18:13:16 2023, max compression
```

## Comparing `TMDBTraktSyncer-1.1.0.tar` & `TMDBTraktSyncer-1.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 17:59:39.793807 TMDBTraktSyncer-1.1.0/
--rw-rw-rw-   0        0        0     1079 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     6468 2023-05-20 17:59:39.793807 TMDBTraktSyncer-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     5795 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-20 17:59:39.772822 TMDBTraktSyncer-1.1.0/TMDBTraktSyncer/
--rw-rw-rw-   0        0        0     5773 2023-05-20 16:47:55.000000 TMDBTraktSyncer-1.1.0/TMDBTraktSyncer/TMDBTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.1.0/TMDBTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     1915 2023-05-20 16:29:13.000000 TMDBTraktSyncer-1.1.0/TMDBTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0     8904 2023-05-20 17:58:42.000000 TMDBTraktSyncer-1.1.0/TMDBTraktSyncer/errorHandling.py
--rw-rw-rw-   0        0        0     2932 2023-05-20 16:50:29.000000 TMDBTraktSyncer-1.1.0/TMDBTraktSyncer/tmdbRatings.py
--rw-rw-rw-   0        0        0     2069 2023-05-20 16:25:11.000000 TMDBTraktSyncer-1.1.0/TMDBTraktSyncer/traktRatings.py
--rw-rw-rw-   0        0        0     1822 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.1.0/TMDBTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-05-20 17:59:39.791808 TMDBTraktSyncer-1.1.0/TMDBTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0     6468 2023-05-20 17:59:39.000000 TMDBTraktSyncer-1.1.0/TMDBTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      487 2023-05-20 17:59:39.000000 TMDBTraktSyncer-1.1.0/TMDBTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 17:59:39.000000 TMDBTraktSyncer-1.1.0/TMDBTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-05-20 17:59:39.000000 TMDBTraktSyncer-1.1.0/TMDBTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-05-20 17:59:39.000000 TMDBTraktSyncer-1.1.0/TMDBTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-20 17:59:39.000000 TMDBTraktSyncer-1.1.0/TMDBTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-20 17:59:39.794807 TMDBTraktSyncer-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1291 2023-05-20 17:59:14.000000 TMDBTraktSyncer-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 18:13:16.081125 TMDBTraktSyncer-1.1.1/
+-rw-rw-rw-   0        0        0     1079 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0     6468 2023-05-20 18:13:16.081125 TMDBTraktSyncer-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5795 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-20 18:13:16.061105 TMDBTraktSyncer-1.1.1/TMDBTraktSyncer/
+-rw-rw-rw-   0        0        0     5773 2023-05-20 16:47:55.000000 TMDBTraktSyncer-1.1.1/TMDBTraktSyncer/TMDBTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.1.1/TMDBTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     1915 2023-05-20 16:29:13.000000 TMDBTraktSyncer-1.1.1/TMDBTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0     8904 2023-05-20 17:58:42.000000 TMDBTraktSyncer-1.1.1/TMDBTraktSyncer/errorHandling.py
+-rw-rw-rw-   0        0        0     2938 2023-05-20 18:12:36.000000 TMDBTraktSyncer-1.1.1/TMDBTraktSyncer/tmdbRatings.py
+-rw-rw-rw-   0        0        0     2075 2023-05-20 18:12:15.000000 TMDBTraktSyncer-1.1.1/TMDBTraktSyncer/traktRatings.py
+-rw-rw-rw-   0        0        0     1822 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.1.1/TMDBTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-05-20 18:13:16.079103 TMDBTraktSyncer-1.1.1/TMDBTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0     6468 2023-05-20 18:13:15.000000 TMDBTraktSyncer-1.1.1/TMDBTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      487 2023-05-20 18:13:15.000000 TMDBTraktSyncer-1.1.1/TMDBTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 18:13:15.000000 TMDBTraktSyncer-1.1.1/TMDBTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-05-20 18:13:15.000000 TMDBTraktSyncer-1.1.1/TMDBTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-05-20 18:13:15.000000 TMDBTraktSyncer-1.1.1/TMDBTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-20 18:13:15.000000 TMDBTraktSyncer-1.1.1/TMDBTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-20 18:13:16.082104 TMDBTraktSyncer-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1291 2023-05-20 18:12:52.000000 TMDBTraktSyncer-1.1.1/setup.py
```

### Comparing `TMDBTraktSyncer-1.1.0/LICENSE` & `TMDBTraktSyncer-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.1.0/PKG-INFO` & `TMDBTraktSyncer-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TMDBTraktSyncer
-Version: 1.1.0
+Version: 1.1.1
 Summary: This python script will sync user ratings for Movies and TV Shows both ways between Trakt and TMDB.
 Home-page: https://github.com/RileyXX/TMDB-Trakt-Syncer
 Keywords: python,video,trakt,tmdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `TMDBTraktSyncer-1.1.0/README.md` & `TMDBTraktSyncer-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.1.0/TMDBTraktSyncer/TMDBTraktSyncer.py` & `TMDBTraktSyncer-1.1.1/TMDBTraktSyncer/TMDBTraktSyncer.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.1.0/TMDBTraktSyncer/authTrakt.py` & `TMDBTraktSyncer-1.1.1/TMDBTraktSyncer/authTrakt.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.1.0/TMDBTraktSyncer/errorHandling.py` & `TMDBTraktSyncer-1.1.1/TMDBTraktSyncer/errorHandling.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.1.0/TMDBTraktSyncer/tmdbRatings.py` & `TMDBTraktSyncer-1.1.1/TMDBTraktSyncer/tmdbRatings.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     results = json_data['results']
     total_pages = json_data['total_pages']
     current_page = json_data['page']
     return results, total_pages, current_page
 
 def getTMDBRatings(tmdb_v4_token):
     # Get TMDB Ratings
-    print('Getting TMDB Ratings')
+    print('Processing TMDB Ratings')
 
     response = errorHandling.make_tmdb_request('https://api.themoviedb.org/3/account')
     json_data = json.loads(response.text)
     account_id = json_data['id']
 
     movie_ratings = []
     page = 1
@@ -78,10 +78,10 @@
             })
         
         page += 1
         time.sleep(1)
 
     tmdb_ratings = movie_ratings + show_ratings + episode_ratings
 
-    print('Getting TMDB Ratings Complete')
+    print('Processing TMDB Ratings Complete')
 
     return tmdb_ratings
```

### Comparing `TMDBTraktSyncer-1.1.0/TMDBTraktSyncer/traktRatings.py` & `TMDBTraktSyncer-1.1.1/TMDBTraktSyncer/traktRatings.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 try:
     from TMDBTraktSyncer import errorHandling
 except:
     import errorHandling
 
 def getTraktRatings(trakt_client_id, trakt_access_token):
     # Get Trakt Ratings
-    print('Getting Trakt Ratings')
+    print('Processing Trakt Ratings')
 
     response = errorHandling.make_trakt_request('https://api.trakt.tv/users/me')
     json_data = json.loads(response.text)
     username = json_data['username']
     response = errorHandling.make_trakt_request(f'https://api.trakt.tv/users/{username}/ratings')
     json_data = json.loads(response.text)
 
@@ -44,10 +44,10 @@
                 'Episode': episode['number'],
                 'ShowID': show_tmdb_id,
                 'Type': 'episode'
             })
 
     trakt_ratings = movie_ratings + show_ratings + episode_ratings
 
-    print('Getting Trakt Ratings Complete')
+    print('Processing Trakt Ratings Complete')
     
     return trakt_ratings
```

### Comparing `TMDBTraktSyncer-1.1.0/TMDBTraktSyncer/verifyCredentials.py` & `TMDBTraktSyncer-1.1.1/TMDBTraktSyncer/verifyCredentials.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.1.0/TMDBTraktSyncer.egg-info/PKG-INFO` & `TMDBTraktSyncer-1.1.1/TMDBTraktSyncer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TMDBTraktSyncer
-Version: 1.1.0
+Version: 1.1.1
 Summary: This python script will sync user ratings for Movies and TV Shows both ways between Trakt and TMDB.
 Home-page: https://github.com/RileyXX/TMDB-Trakt-Syncer
 Keywords: python,video,trakt,tmdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `TMDBTraktSyncer-1.1.0/setup.py` & `TMDBTraktSyncer-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.1.0'
+VERSION = '1.1.1'
 DESCRIPTION = 'This python script will sync user ratings for Movies and TV Shows both ways between Trakt and TMDB.'
 
 # Setting up
 setup(
     name="TMDBTraktSyncer",
     version=VERSION,
     description=DESCRIPTION,
```

