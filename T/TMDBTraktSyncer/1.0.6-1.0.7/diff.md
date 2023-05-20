# Comparing `tmp/TMDBTraktSyncer-1.0.6.tar.gz` & `tmp/TMDBTraktSyncer-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TMDBTraktSyncer-1.0.6.tar", last modified: Thu May 18 22:53:08 2023, max compression
+gzip compressed data, was "TMDBTraktSyncer-1.0.7.tar", last modified: Sat May 20 16:59:45 2023, max compression
```

## Comparing `TMDBTraktSyncer-1.0.6.tar` & `TMDBTraktSyncer-1.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 22:53:08.287369 TMDBTraktSyncer-1.0.6/
--rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 TMDBTraktSyncer-1.0.6/LICENSE
--rw-rw-rw-   0        0        0     6468 2023-05-18 22:53:08.286383 TMDBTraktSyncer-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     5795 2023-05-18 21:09:58.000000 TMDBTraktSyncer-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 22:53:08.256369 TMDBTraktSyncer-1.0.6/TMDBTraktSyncer/
--rw-rw-rw-   0        0        0     7096 2023-05-18 22:51:39.000000 TMDBTraktSyncer-1.0.6/TMDBTraktSyncer/TMDBTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 TMDBTraktSyncer-1.0.6/TMDBTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     1805 2023-05-18 21:06:55.000000 TMDBTraktSyncer-1.0.6/TMDBTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0      517 2023-05-18 22:24:38.000000 TMDBTraktSyncer-1.0.6/TMDBTraktSyncer/errorHandling.py
--rw-rw-rw-   0        0        0     2997 2023-05-18 21:06:57.000000 TMDBTraktSyncer-1.0.6/TMDBTraktSyncer/tmdbRatings.py
--rw-rw-rw-   0        0        0     2181 2023-05-18 21:06:45.000000 TMDBTraktSyncer-1.0.6/TMDBTraktSyncer/traktRatings.py
--rw-rw-rw-   0        0        0     1822 2023-05-18 21:06:52.000000 TMDBTraktSyncer-1.0.6/TMDBTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-05-18 22:53:08.284368 TMDBTraktSyncer-1.0.6/TMDBTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0     6468 2023-05-18 22:53:08.000000 TMDBTraktSyncer-1.0.6/TMDBTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      487 2023-05-18 22:53:08.000000 TMDBTraktSyncer-1.0.6/TMDBTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 22:53:08.000000 TMDBTraktSyncer-1.0.6/TMDBTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-05-18 22:53:08.000000 TMDBTraktSyncer-1.0.6/TMDBTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-05-18 22:53:08.000000 TMDBTraktSyncer-1.0.6/TMDBTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-18 22:53:08.000000 TMDBTraktSyncer-1.0.6/TMDBTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 22:53:08.287369 TMDBTraktSyncer-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1291 2023-05-18 22:52:32.000000 TMDBTraktSyncer-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 16:59:45.397021 TMDBTraktSyncer-1.0.7/
+-rw-rw-rw-   0        0        0     1079 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0     6468 2023-05-20 16:59:45.396021 TMDBTraktSyncer-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     5795 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-20 16:59:45.364022 TMDBTraktSyncer-1.0.7/TMDBTraktSyncer/
+-rw-rw-rw-   0        0        0     5773 2023-05-20 16:47:55.000000 TMDBTraktSyncer-1.0.7/TMDBTraktSyncer/TMDBTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.0.7/TMDBTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     1915 2023-05-20 16:29:13.000000 TMDBTraktSyncer-1.0.7/TMDBTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0     8822 2023-05-20 16:56:20.000000 TMDBTraktSyncer-1.0.7/TMDBTraktSyncer/errorHandling.py
+-rw-rw-rw-   0        0        0     2932 2023-05-20 16:50:29.000000 TMDBTraktSyncer-1.0.7/TMDBTraktSyncer/tmdbRatings.py
+-rw-rw-rw-   0        0        0     2069 2023-05-20 16:25:11.000000 TMDBTraktSyncer-1.0.7/TMDBTraktSyncer/traktRatings.py
+-rw-rw-rw-   0        0        0     1822 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.0.7/TMDBTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-05-20 16:59:45.394021 TMDBTraktSyncer-1.0.7/TMDBTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0     6468 2023-05-20 16:59:45.000000 TMDBTraktSyncer-1.0.7/TMDBTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      487 2023-05-20 16:59:45.000000 TMDBTraktSyncer-1.0.7/TMDBTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 16:59:45.000000 TMDBTraktSyncer-1.0.7/TMDBTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-05-20 16:59:45.000000 TMDBTraktSyncer-1.0.7/TMDBTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-05-20 16:59:45.000000 TMDBTraktSyncer-1.0.7/TMDBTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-20 16:59:45.000000 TMDBTraktSyncer-1.0.7/TMDBTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-20 16:59:45.397021 TMDBTraktSyncer-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1291 2023-05-20 16:59:20.000000 TMDBTraktSyncer-1.0.7/setup.py
```

### Comparing `TMDBTraktSyncer-1.0.6/LICENSE` & `TMDBTraktSyncer-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.0.6/PKG-INFO` & `TMDBTraktSyncer-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TMDBTraktSyncer
-Version: 1.0.6
+Version: 1.0.7
 Summary: This python script will sync user ratings for Movies and TV Shows both ways between Trakt and TMDB.
 Home-page: https://github.com/RileyXX/TMDB-Trakt-Syncer
 Keywords: python,video,trakt,tmdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `TMDBTraktSyncer-1.0.6/README.md` & `TMDBTraktSyncer-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.0.6/TMDBTraktSyncer/TMDBTraktSyncer.py` & `TMDBTraktSyncer-1.0.7/TMDBTraktSyncer/TMDBTraktSyncer.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     try:
 
         #Get credentials
         trakt_client_id = verifyCredentials.trakt_client_id
         trakt_client_secret = verifyCredentials.trakt_client_secret
         trakt_access_token = verifyCredentials.trakt_access_token
         tmdb_v4_token = verifyCredentials.tmdb_v4_token
+        
             
         trakt_ratings = traktRatings.getTraktRatings(trakt_client_id, trakt_access_token)
         tmdb_ratings = tmdbRatings.getTMDBRatings(tmdb_v4_token)
 
         #Get trakt and tmdb ratings and filter out trakt ratings with missing tmdb id
         trakt_ratings = [rating for rating in trakt_ratings if rating['ID'] is not None]
         tmdb_ratings = [rating for rating in tmdb_ratings if rating['ID'] is not None]
@@ -39,19 +40,14 @@
             num_items = len(tmdb_ratings_to_set)
             item_count = 0
             
             # Set TMDB Rating
             for item in tmdb_ratings_to_set:
                 item_count += 1
 
-                headers = {
-                    'accept': 'application/json',
-                    'Content-Type': 'application/json;charset=utf-8',
-                    'Authorization': f'Bearer {tmdb_v4_token}'
-                }
                 if item['Type'] == 'movie':
                     payload = {
                         'value': item['Rating']
                     }
                     url = f"https://api.themoviedb.org/3/movie/{item['ID']}/rating"
                     print(f"Rating movie ({item_count} of {num_items}): {item['Title']} ({item['Year']}): {item['Rating']}/10 on TMDB")
 
@@ -65,41 +61,25 @@
                 elif item['Type'] == 'episode':
                     payload = {
                         'value': item['Rating']
                     }
                     url = f"https://api.themoviedb.org/3/tv/{item['ShowID']}/season/{item['Season']}/episode/{item['Episode']}/rating"
                     print(f"Rating episode ({item_count} of {num_items}): {item['Title']} ({item['Year']}) [S{item['Season']:02d}E{item['Episode']:02d}]: {item['Rating']}/10 on TMDB")
 
-                response = requests.post(url, headers=headers, json=payload)
-
-                while response.status_code == 429:
-                    print("Rate limit exceeded. Waiting for 1 second...")
-                    time.sleep(1)
-                    response = requests.post(url, headers=headers, json=payload)
-                if response.status_code != 201:
-                    print(f"Error rating {item}: {response.content}")
+                response = errorHandling.make_tmdb_request(url, payload=payload)
 
             print('Setting TMDB Ratings Complete')
         else:
             print('No TMDB Ratings To Set')
 
         if trakt_ratings_to_set:
             print('Setting Trakt Ratings')
 
             # Set the API endpoints
-            oauth_url = "https://api.trakt.tv/oauth/token"
             rate_url = "https://api.trakt.tv/sync/ratings"
-
-            # Set the headers
-            headers = {
-                "Content-Type": "application/json",
-                "trakt-api-version": "2",
-                "trakt-api-key": trakt_client_id,
-                "Authorization": f"Bearer {trakt_access_token}"
-            }
             
             # Count the total number of items to rate
             num_items = len(trakt_ratings_to_set)
             item_count = 0
                     
             # Loop through your data table and rate each item on Trakt
             for item in trakt_ratings_to_set:
@@ -135,22 +115,15 @@
                             },
                             "rating": item["Rating"]
                         }]
                     }
                     print(f"Rating episode ({item_count} of {num_items}): {item['Title']} ({item['Year']}) [S{item['Season']:02d}E{item['Episode']:02d}]: {item['Rating']}/10 on Trakt")
 
                 # Make the API call to rate the item
-                response = requests.post(rate_url, headers=headers, json=data)
-                time.sleep(1)
-                while response.status_code == 429:
-                    print("Rate limit exceeded. Waiting for 1 second...")
-                    time.sleep(1)
-                    response = requests.post(rate_url, headers=headers, json=data)
-                if response.status_code != 201:
-                    print(f"Error rating {item}: {response.content}")
+                response = errorHandling.make_trakt_request(rate_url, payload=data)
 
             print('Setting Trakt Ratings Complete')
         else:
             print('No Trakt Ratings To Set')
 
     except Exception as e:
         error_message = "An error occurred while running the script."
```

### Comparing `TMDBTraktSyncer-1.0.6/TMDBTraktSyncer/authTrakt.py` & `TMDBTraktSyncer-1.0.7/TMDBTraktSyncer/authTrakt.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 import requests
 import os
+try:
+    from TMDBTraktSyncer import errorHandling
+except:
+    import errorHandling
 
 def authenticate(client_id, client_secret):
     CLIENT_ID = client_id
     CLIENT_SECRET = client_secret
     REDIRECT_URI = 'urn:ietf:wg:oauth:2.0:oob'
 
     # Set up the authorization endpoint URL
@@ -34,15 +38,15 @@
         'client_id': CLIENT_ID,
         'client_secret': CLIENT_SECRET,
         'redirect_uri': REDIRECT_URI,
         'grant_type': 'authorization_code'
     }
 
     # Make the request to get the access token
-    response = requests.post('https://api.trakt.tv/oauth/token', headers=headers, json=data)
+    response = errorHandling.make_trakt_request('https://api.trakt.tv/oauth/token', headers=headers, payload=data)
 
     # Parse the JSON response from the API
     json_data = response.json()
 
     # Extract the access token from the response
     ACCESS_TOKEN = json_data['access_token']
```

### Comparing `TMDBTraktSyncer-1.0.6/TMDBTraktSyncer/tmdbRatings.py` & `TMDBTraktSyncer-1.0.7/TMDBTraktSyncer/tmdbRatings.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,73 +1,72 @@
 import requests
 import json
 import time
+try:
+    from TMDBTraktSyncer import errorHandling
+except:
+    import errorHandling
 
-def fetch_data(url, headers):
-    response = requests.get(url, headers=headers)
+def fetch_data(url):
+    response = errorHandling.make_tmdb_request(url)
     json_data = json.loads(response.text)
     results = json_data['results']
     total_pages = json_data['total_pages']
     current_page = json_data['page']
     return results, total_pages, current_page
 
 def getTMDBRatings(tmdb_v4_token):
     # Get TMDB Ratings
     print('Getting TMDB Ratings')
 
-    headers = {
-        'Content-Type': 'application/json',
-        'Authorization': f'Bearer {tmdb_v4_token}'
-    }
-
-    response = requests.get('https://api.themoviedb.org/3/account', headers=headers)
+    response = errorHandling.make_tmdb_request('https://api.themoviedb.org/3/account')
     json_data = json.loads(response.text)
     account_id = json_data['id']
 
     movie_ratings = []
     page = 1
     total_pages = 1
 
     while page <= total_pages:
         url = f'https://api.themoviedb.org/3/account/{account_id}/rated/movies?page={page}'
-        results, total_pages, _ = fetch_data(url, headers)
+        results, total_pages, _ = fetch_data(url)
         
         for movie in results:
             movie_ratings.append({'Title': movie['title'], 'Year': movie['release_date'][:4], 'Rating': movie['rating'], 'ID': movie['id'], 'Type': 'movie'})
         
         page += 1
         time.sleep(1)
 
     # Fetch TV show ratings
     show_ratings = []
     page = 1
     total_pages = 1
 
     while page <= total_pages:
         url = f'https://api.themoviedb.org/3/account/{account_id}/rated/tv?page={page}'
-        results, total_pages, _ = fetch_data(url, headers)
+        results, total_pages, _ = fetch_data(url)
         
         for show in results:
             show_ratings.append({'Title': show['name'], 'Year': show['first_air_date'][:4], 'Rating': show['rating'], 'ID': show['id'], 'Type': 'show'})
         
         page += 1
         time.sleep(1)
 
     # Fetch episode ratings
     episode_ratings = []
     page = 1
     total_pages = 1
 
     while page <= total_pages:
         url = f'https://api.themoviedb.org/3/account/{account_id}/rated/tv/episodes?page={page}'
-        results, total_pages, _ = fetch_data(url, headers)
+        results, total_pages, _ = fetch_data(url)
         
         for episode in results:
             show_id = episode['show_id']
-            response = requests.get(f'https://api.themoviedb.org/3/tv/{show_id}', headers=headers)
+            response = errorHandling.make_tmdb_request(f'https://api.themoviedb.org/3/tv/{show_id}')
             show_info = json.loads(response.text)
             show_name = show_info['name'] if 'name' in show_info else ''
             episode_title = f"{show_name}: {episode['name']}"
             episode_ratings.append({
                 'Title': episode_title,
                 'Year': episode['air_date'][:4],
                 'Rating': episode['rating'],
```

### Comparing `TMDBTraktSyncer-1.0.6/TMDBTraktSyncer/traktRatings.py` & `TMDBTraktSyncer-1.0.7/TMDBTraktSyncer/traktRatings.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 import json
 import requests
+try:
+    from TMDBTraktSyncer import errorHandling
+except:
+    import errorHandling
 
 def getTraktRatings(trakt_client_id, trakt_access_token):
     # Get Trakt Ratings
     print('Getting Trakt Ratings')
 
-    headers = {
-        'Content-Type': 'application/json',
-        'trakt-api-version': '2',
-        'trakt-api-key': trakt_client_id,
-        'Authorization': f'Bearer {trakt_access_token}'
-    }
-
-    response = requests.get('https://api.trakt.tv/users/me', headers=headers)
+    response = errorHandling.make_trakt_request('https://api.trakt.tv/users/me')
     json_data = json.loads(response.text)
     username = json_data['username']
-    response = requests.get(f'https://api.trakt.tv/users/{username}/ratings', headers=headers)
+    response = errorHandling.make_trakt_request(f'https://api.trakt.tv/users/{username}/ratings')
     json_data = json.loads(response.text)
 
     movie_ratings = []
     show_ratings = []
     episode_ratings = []
 
     for item in json_data:
```

### Comparing `TMDBTraktSyncer-1.0.6/TMDBTraktSyncer/verifyCredentials.py` & `TMDBTraktSyncer-1.0.7/TMDBTraktSyncer/verifyCredentials.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.0.6/TMDBTraktSyncer.egg-info/PKG-INFO` & `TMDBTraktSyncer-1.0.7/TMDBTraktSyncer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TMDBTraktSyncer
-Version: 1.0.6
+Version: 1.0.7
 Summary: This python script will sync user ratings for Movies and TV Shows both ways between Trakt and TMDB.
 Home-page: https://github.com/RileyXX/TMDB-Trakt-Syncer
 Keywords: python,video,trakt,tmdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `TMDBTraktSyncer-1.0.6/setup.py` & `TMDBTraktSyncer-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.6'
+VERSION = '1.0.7'
 DESCRIPTION = 'This python script will sync user ratings for Movies and TV Shows both ways between Trakt and TMDB.'
 
 # Setting up
 setup(
     name="TMDBTraktSyncer",
     version=VERSION,
     description=DESCRIPTION,
```

