# Comparing `tmp/TMDBTraktSyncer-1.1.1.tar.gz` & `tmp/TMDBTraktSyncer-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TMDBTraktSyncer-1.1.1.tar", last modified: Sat May 20 18:13:16 2023, max compression
+gzip compressed data, was "TMDBTraktSyncer-1.1.2.tar", last modified: Sat May 20 20:08:45 2023, max compression
```

## Comparing `TMDBTraktSyncer-1.1.1.tar` & `TMDBTraktSyncer-1.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 18:13:16.081125 TMDBTraktSyncer-1.1.1/
--rw-rw-rw-   0        0        0     1079 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     6468 2023-05-20 18:13:16.081125 TMDBTraktSyncer-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     5795 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-20 18:13:16.061105 TMDBTraktSyncer-1.1.1/TMDBTraktSyncer/
--rw-rw-rw-   0        0        0     5773 2023-05-20 16:47:55.000000 TMDBTraktSyncer-1.1.1/TMDBTraktSyncer/TMDBTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.1.1/TMDBTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     1915 2023-05-20 16:29:13.000000 TMDBTraktSyncer-1.1.1/TMDBTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0     8904 2023-05-20 17:58:42.000000 TMDBTraktSyncer-1.1.1/TMDBTraktSyncer/errorHandling.py
--rw-rw-rw-   0        0        0     2938 2023-05-20 18:12:36.000000 TMDBTraktSyncer-1.1.1/TMDBTraktSyncer/tmdbRatings.py
--rw-rw-rw-   0        0        0     2075 2023-05-20 18:12:15.000000 TMDBTraktSyncer-1.1.1/TMDBTraktSyncer/traktRatings.py
--rw-rw-rw-   0        0        0     1822 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.1.1/TMDBTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-05-20 18:13:16.079103 TMDBTraktSyncer-1.1.1/TMDBTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0     6468 2023-05-20 18:13:15.000000 TMDBTraktSyncer-1.1.1/TMDBTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      487 2023-05-20 18:13:15.000000 TMDBTraktSyncer-1.1.1/TMDBTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 18:13:15.000000 TMDBTraktSyncer-1.1.1/TMDBTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-05-20 18:13:15.000000 TMDBTraktSyncer-1.1.1/TMDBTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-05-20 18:13:15.000000 TMDBTraktSyncer-1.1.1/TMDBTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-20 18:13:15.000000 TMDBTraktSyncer-1.1.1/TMDBTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-20 18:13:16.082104 TMDBTraktSyncer-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1291 2023-05-20 18:12:52.000000 TMDBTraktSyncer-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 20:08:45.475974 TMDBTraktSyncer-1.1.2/
+-rw-rw-rw-   0        0        0     1079 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0     6468 2023-05-20 20:08:45.474972 TMDBTraktSyncer-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5795 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-20 20:08:45.447020 TMDBTraktSyncer-1.1.2/TMDBTraktSyncer/
+-rw-rw-rw-   0        0        0     5695 2023-05-20 19:53:04.000000 TMDBTraktSyncer-1.1.2/TMDBTraktSyncer/TMDBTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.1.2/TMDBTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     1928 2023-05-20 19:53:06.000000 TMDBTraktSyncer-1.1.2/TMDBTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0     8916 2023-05-20 19:53:06.000000 TMDBTraktSyncer-1.1.2/TMDBTraktSyncer/errorHandling.py
+-rw-rw-rw-   0        0        0     2991 2023-05-20 20:06:38.000000 TMDBTraktSyncer-1.1.2/TMDBTraktSyncer/tmdbRatings.py
+-rw-rw-rw-   0        0        0     2168 2023-05-20 19:53:04.000000 TMDBTraktSyncer-1.1.2/TMDBTraktSyncer/traktRatings.py
+-rw-rw-rw-   0        0        0     1834 2023-05-20 19:53:05.000000 TMDBTraktSyncer-1.1.2/TMDBTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-05-20 20:08:45.472978 TMDBTraktSyncer-1.1.2/TMDBTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0     6468 2023-05-20 20:08:45.000000 TMDBTraktSyncer-1.1.2/TMDBTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      487 2023-05-20 20:08:45.000000 TMDBTraktSyncer-1.1.2/TMDBTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 20:08:45.000000 TMDBTraktSyncer-1.1.2/TMDBTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-05-20 20:08:45.000000 TMDBTraktSyncer-1.1.2/TMDBTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-05-20 20:08:45.000000 TMDBTraktSyncer-1.1.2/TMDBTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-20 20:08:45.000000 TMDBTraktSyncer-1.1.2/TMDBTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-20 20:08:45.475974 TMDBTraktSyncer-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1291 2023-05-20 20:08:26.000000 TMDBTraktSyncer-1.1.2/setup.py
```

### Comparing `TMDBTraktSyncer-1.1.1/LICENSE` & `TMDBTraktSyncer-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.1.1/PKG-INFO` & `TMDBTraktSyncer-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TMDBTraktSyncer
-Version: 1.1.1
+Version: 1.1.2
 Summary: This python script will sync user ratings for Movies and TV Shows both ways between Trakt and TMDB.
 Home-page: https://github.com/RileyXX/TMDB-Trakt-Syncer
 Keywords: python,video,trakt,tmdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `TMDBTraktSyncer-1.1.1/README.md` & `TMDBTraktSyncer-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.1.1/TMDBTraktSyncer/TMDBTraktSyncer.py` & `TMDBTraktSyncer-1.1.2/TMDBTraktSyncer/TMDBTraktSyncer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 import json
 import requests
 import time
 try:
     from TMDBTraktSyncer import verifyCredentials
     from TMDBTraktSyncer import traktRatings
     from TMDBTraktSyncer import tmdbRatings
-    from TMDBTraktSyncer import errorHandling
-except:
+    from TMDBTraktSyncer import errorHandling as EH
+except ImportError:
     import verifyCredentials
     import traktRatings
     import tmdbRatings
-    import errorHandling
+    import errorHandling as EH
 
 
 def main():
     try:
 
         #Get credentials
         trakt_client_id = verifyCredentials.trakt_client_id
-        trakt_client_secret = verifyCredentials.trakt_client_secret
         trakt_access_token = verifyCredentials.trakt_access_token
         tmdb_v4_token = verifyCredentials.tmdb_v4_token
         
             
         trakt_ratings = traktRatings.getTraktRatings(trakt_client_id, trakt_access_token)
         tmdb_ratings = tmdbRatings.getTMDBRatings(tmdb_v4_token)
 
@@ -61,15 +60,15 @@
                 elif item['Type'] == 'episode':
                     payload = {
                         'value': item['Rating']
                     }
                     url = f"https://api.themoviedb.org/3/tv/{item['ShowID']}/season/{item['Season']}/episode/{item['Episode']}/rating"
                     print(f"Rating episode ({item_count} of {num_items}): {item['Title']} ({item['Year']}) [S{item['Season']:02d}E{item['Episode']:02d}]: {item['Rating']}/10 on TMDB")
 
-                response = errorHandling.make_tmdb_request(url, payload=payload)
+                response = EH.make_tmdb_request(url, payload=payload)
 
             print('Setting TMDB Ratings Complete')
         else:
             print('No TMDB Ratings To Set')
 
         if trakt_ratings_to_set:
             print('Setting Trakt Ratings')
@@ -115,19 +114,19 @@
                             },
                             "rating": item["Rating"]
                         }]
                     }
                     print(f"Rating episode ({item_count} of {num_items}): {item['Title']} ({item['Year']}) [S{item['Season']:02d}E{item['Episode']:02d}]: {item['Rating']}/10 on Trakt")
 
                 # Make the API call to rate the item
-                response = errorHandling.make_trakt_request(rate_url, payload=data)
+                response = EH.make_trakt_request(rate_url, payload=data)
 
             print('Setting Trakt Ratings Complete')
         else:
             print('No Trakt Ratings To Set')
 
     except Exception as e:
         error_message = "An error occurred while running the script."
-        errorHandling.report_error(error_message)
+        EH.report_error(error_message)
 
 if __name__ == '__main__':
     main()
```

### Comparing `TMDBTraktSyncer-1.1.1/TMDBTraktSyncer/authTrakt.py` & `TMDBTraktSyncer-1.1.2/TMDBTraktSyncer/authTrakt.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import requests
 import os
 try:
-    from TMDBTraktSyncer import errorHandling
-except:
-    import errorHandling
+    from TMDBTraktSyncer import errorHandling as EH
+except ImportError:
+    import errorHandling as EH
 
 def authenticate(client_id, client_secret):
     CLIENT_ID = client_id
     CLIENT_SECRET = client_secret
     REDIRECT_URI = 'urn:ietf:wg:oauth:2.0:oob'
 
     # Set up the authorization endpoint URL
@@ -38,15 +38,15 @@
         'client_id': CLIENT_ID,
         'client_secret': CLIENT_SECRET,
         'redirect_uri': REDIRECT_URI,
         'grant_type': 'authorization_code'
     }
 
     # Make the request to get the access token
-    response = errorHandling.make_trakt_request('https://api.trakt.tv/oauth/token', headers=headers, payload=data)
+    response = EH.make_trakt_request('https://api.trakt.tv/oauth/token', headers=headers, payload=data)
 
     # Parse the JSON response from the API
     json_data = response.json()
 
     # Extract the access token from the response
     ACCESS_TOKEN = json_data['access_token']
```

### Comparing `TMDBTraktSyncer-1.1.1/TMDBTraktSyncer/errorHandling.py` & `TMDBTraktSyncer-1.1.2/TMDBTraktSyncer/errorHandling.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import traceback
 import requests
 import time
 try:
     from TMDBTraktSyncer import verifyCredentials
-except:
+except ImportError:
     import verifyCredentials
 
 def report_error(error_message):
     github_issue_url = "https://github.com/RileyXX/TMDB-Trakt-Syncer/issues/new?template=bug_report.yml"
     traceback_info = traceback.format_exc()
 
     print("\n--- ERROR ---")
```

### Comparing `TMDBTraktSyncer-1.1.1/TMDBTraktSyncer/tmdbRatings.py` & `TMDBTraktSyncer-1.1.2/TMDBTraktSyncer/tmdbRatings.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import requests
 import json
 import time
 try:
-    from TMDBTraktSyncer import errorHandling
-except:
-    import errorHandling
+    from TMDBTraktSyncer import errorHandling as EH
+except ImportError:
+    import errorHandling as EH
 
 def fetch_data(url):
-    response = errorHandling.make_tmdb_request(url)
+    response = EH.make_tmdb_request(url)
     json_data = json.loads(response.text)
     results = json_data['results']
     total_pages = json_data['total_pages']
     current_page = json_data['page']
     return results, total_pages, current_page
 
 def getTMDBRatings(tmdb_v4_token):
     # Get TMDB Ratings
     print('Processing TMDB Ratings')
 
-    response = errorHandling.make_tmdb_request('https://api.themoviedb.org/3/account')
+    response = EH.make_tmdb_request('https://api.themoviedb.org/3/account')
     json_data = json.loads(response.text)
     account_id = json_data['id']
 
     movie_ratings = []
     page = 1
     total_pages = 1
 
@@ -58,30 +58,30 @@
 
     while page <= total_pages:
         url = f'https://api.themoviedb.org/3/account/{account_id}/rated/tv/episodes?page={page}'
         results, total_pages, _ = fetch_data(url)
         
         for episode in results:
             show_id = episode['show_id']
-            response = errorHandling.make_tmdb_request(f'https://api.themoviedb.org/3/tv/{show_id}')
+            response = EH.make_tmdb_request(f'https://api.themoviedb.org/3/tv/{show_id}')
             show_info = json.loads(response.text)
-            show_name = show_info['name'] if 'name' in show_info else ''
-            episode_title = f"{show_name}: {episode['name']}"
+            show_name = show_info.get('name', 'Show Name Not Found')
+            episode_title = f"{show_name}: {episode.get('name', 'Episode Name Not Found')}"
             episode_ratings.append({
                 'Title': episode_title,
-                'Year': episode['air_date'][:4],
-                'Rating': episode['rating'],
-                'ID': episode['id'],
-                'Season': episode['season_number'],
-                'Episode': episode['episode_number'],
+                'Year': episode.get('air_date', '')[:4],
+                'Rating': episode.get('rating'),
+                'ID': episode.get('id'),
+                'Season': episode.get('season_number'),
+                'Episode': episode.get('episode_number'),
                 'ShowID': show_id,
                 'Type': 'episode'
             })
-        
-        page += 1
-        time.sleep(1)
+            
+            page += 1
+            time.sleep(1)
 
     tmdb_ratings = movie_ratings + show_ratings + episode_ratings
 
     print('Processing TMDB Ratings Complete')
 
     return tmdb_ratings
```

### Comparing `TMDBTraktSyncer-1.1.1/TMDBTraktSyncer/verifyCredentials.py` & `TMDBTraktSyncer-1.1.2/TMDBTraktSyncer/verifyCredentials.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import json
 try:
     from TMDBTraktSyncer import authTrakt
-except:
+except ImportError:
     import authTrakt
 
 # Define the file path
 here = os.path.abspath(os.path.dirname(__file__))
 file_path = os.path.join(here, 'credentials.txt')
 
 # Check if the file exists
```

### Comparing `TMDBTraktSyncer-1.1.1/TMDBTraktSyncer.egg-info/PKG-INFO` & `TMDBTraktSyncer-1.1.2/TMDBTraktSyncer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TMDBTraktSyncer
-Version: 1.1.1
+Version: 1.1.2
 Summary: This python script will sync user ratings for Movies and TV Shows both ways between Trakt and TMDB.
 Home-page: https://github.com/RileyXX/TMDB-Trakt-Syncer
 Keywords: python,video,trakt,tmdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `TMDBTraktSyncer-1.1.1/setup.py` & `TMDBTraktSyncer-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.1.1'
+VERSION = '1.1.2'
 DESCRIPTION = 'This python script will sync user ratings for Movies and TV Shows both ways between Trakt and TMDB.'
 
 # Setting up
 setup(
     name="TMDBTraktSyncer",
     version=VERSION,
     description=DESCRIPTION,
```

