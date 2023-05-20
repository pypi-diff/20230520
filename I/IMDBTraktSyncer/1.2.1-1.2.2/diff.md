# Comparing `tmp/IMDBTraktSyncer-1.2.1.tar.gz` & `tmp/IMDBTraktSyncer-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IMDBTraktSyncer-1.2.1.tar", last modified: Sat May 20 18:54:16 2023, max compression
+gzip compressed data, was "IMDBTraktSyncer-1.2.2.tar", last modified: Sat May 20 20:51:37 2023, max compression
```

## Comparing `IMDBTraktSyncer-1.2.1.tar` & `IMDBTraktSyncer-1.2.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 18:54:16.820654 IMDBTraktSyncer-1.2.1/
-drwxrwxrwx   0        0        0        0 2023-05-20 18:54:16.779655 IMDBTraktSyncer-1.2.1/IMDBTraktSyncer/
--rw-rw-rw-   0        0        0    16494 2023-05-20 18:35:47.000000 IMDBTraktSyncer-1.2.1/IMDBTraktSyncer/IMDBTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDBTraktSyncer-1.2.1/IMDBTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     1900 2023-05-20 18:47:25.000000 IMDBTraktSyncer-1.2.1/IMDBTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0     4079 2023-05-16 01:53:33.000000 IMDBTraktSyncer-1.2.1/IMDBTraktSyncer/checkChromedriver.py
--rw-rw-rw-   0        0        0     3851 2023-05-20 18:51:56.000000 IMDBTraktSyncer-1.2.1/IMDBTraktSyncer/errorHandling.py
--rw-rw-rw-   0        0        0     5452 2023-05-20 18:48:39.000000 IMDBTraktSyncer-1.2.1/IMDBTraktSyncer/imdbData.py
--rw-rw-rw-   0        0        0     4254 2023-05-20 18:47:44.000000 IMDBTraktSyncer-1.2.1/IMDBTraktSyncer/traktData.py
--rw-rw-rw-   0        0        0     5476 2023-05-20 02:05:00.000000 IMDBTraktSyncer-1.2.1/IMDBTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-05-20 18:54:16.817655 IMDBTraktSyncer-1.2.1/IMDBTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0     7755 2023-05-20 18:54:16.000000 IMDBTraktSyncer-1.2.1/IMDBTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      518 2023-05-20 18:54:16.000000 IMDBTraktSyncer-1.2.1/IMDBTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 18:54:16.000000 IMDBTraktSyncer-1.2.1/IMDBTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-05-20 18:54:16.000000 IMDBTraktSyncer-1.2.1/IMDBTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-05-20 18:54:16.000000 IMDBTraktSyncer-1.2.1/IMDBTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-20 18:54:16.000000 IMDBTraktSyncer-1.2.1/IMDBTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDBTraktSyncer-1.2.1/LICENSE
--rw-rw-rw-   0        0        0     7755 2023-05-20 18:54:16.819654 IMDBTraktSyncer-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     7095 2023-05-20 18:20:58.000000 IMDBTraktSyncer-1.2.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-20 18:54:16.820654 IMDBTraktSyncer-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1317 2023-05-20 18:53:59.000000 IMDBTraktSyncer-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 20:51:37.546074 IMDBTraktSyncer-1.2.2/
+drwxrwxrwx   0        0        0        0 2023-05-20 20:51:37.521037 IMDBTraktSyncer-1.2.2/IMDBTraktSyncer/
+-rw-rw-rw-   0        0        0    16437 2023-05-20 20:44:52.000000 IMDBTraktSyncer-1.2.2/IMDBTraktSyncer/IMDBTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDBTraktSyncer-1.2.2/IMDBTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     1913 2023-05-20 20:45:01.000000 IMDBTraktSyncer-1.2.2/IMDBTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0     4079 2023-05-16 01:53:33.000000 IMDBTraktSyncer-1.2.2/IMDBTraktSyncer/checkChromedriver.py
+-rw-rw-rw-   0        0        0     3845 2023-05-20 20:45:06.000000 IMDBTraktSyncer-1.2.2/IMDBTraktSyncer/errorHandling.py
+-rw-rw-rw-   0        0        0     5388 2023-05-20 20:44:48.000000 IMDBTraktSyncer-1.2.2/IMDBTraktSyncer/imdbData.py
+-rw-rw-rw-   0        0        0     4528 2023-05-20 20:47:54.000000 IMDBTraktSyncer-1.2.2/IMDBTraktSyncer/traktData.py
+-rw-rw-rw-   0        0        0     5488 2023-05-20 20:44:57.000000 IMDBTraktSyncer-1.2.2/IMDBTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-05-20 20:51:37.543074 IMDBTraktSyncer-1.2.2/IMDBTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0     7755 2023-05-20 20:51:37.000000 IMDBTraktSyncer-1.2.2/IMDBTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      518 2023-05-20 20:51:37.000000 IMDBTraktSyncer-1.2.2/IMDBTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 20:51:37.000000 IMDBTraktSyncer-1.2.2/IMDBTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-05-20 20:51:37.000000 IMDBTraktSyncer-1.2.2/IMDBTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2023-05-20 20:51:37.000000 IMDBTraktSyncer-1.2.2/IMDBTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-20 20:51:37.000000 IMDBTraktSyncer-1.2.2/IMDBTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDBTraktSyncer-1.2.2/LICENSE
+-rw-rw-rw-   0        0        0     7755 2023-05-20 20:51:37.545074 IMDBTraktSyncer-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     7095 2023-05-20 18:20:58.000000 IMDBTraktSyncer-1.2.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-20 20:51:37.546074 IMDBTraktSyncer-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1317 2023-05-20 20:51:05.000000 IMDBTraktSyncer-1.2.2/setup.py
```

### Comparing `IMDBTraktSyncer-1.2.1/IMDBTraktSyncer/IMDBTraktSyncer.py` & `IMDBTraktSyncer-1.2.2/IMDBTraktSyncer/IMDBTraktSyncer.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,33 +9,33 @@
 from selenium.common.exceptions import StaleElementReferenceException
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.common.exceptions import SessionNotCreatedException
 try:
     from IMDBTraktSyncer import checkChromedriver
-    from IMDBTraktSyncer import verifyCredentials
+    from IMDBTraktSyncer import verifyCredentials as VC
     from IMDBTraktSyncer import traktData
     from IMDBTraktSyncer import imdbData
-    from IMDBTraktSyncer import errorHandling
-except:
+    from IMDBTraktSyncer import errorHandling as EH
+except ImportError:
     import checkChromedriver
-    import verifyCredentials
+    import verifyCredentials as VC
     import traktData
     import imdbData
-    import errorHandling
+    import errorHandling as EH
 from chromedriver_py import binary_path
 
 
 def main():
     try:
 
         #Get credentials
-        imdb_username = verifyCredentials.imdb_username
-        imdb_password = verifyCredentials.imdb_password
+        imdb_username = VC.imdb_username
+        imdb_password = VC.imdb_password
         
         directory = os.path.dirname(os.path.realpath(__file__))
         
         logging.getLogger('selenium.webdriver').setLevel(logging.WARNING)
         
         #Start web driver
         print('Starting webdriver...')
@@ -155,15 +155,15 @@
                 except:
                     pass
 
             print('Setting IMDB Ratings Complete')
         else:
             print('No IMDB Ratings To Set')
 
-        if verifyCredentials.sync_reviews_value:
+        if VC.sync_reviews_value:
             #Set Trakt Ratings
             if trakt_ratings_to_set:
                 print('Setting Trakt Ratings')
 
                 # Set the API endpoints
                 rate_url = "https://api.trakt.tv/sync/ratings"
                 
@@ -205,26 +205,26 @@
                                 },
                                 "rating": item["Rating"]
                             }]
                         }
                         print(f"Rating episode ({item_count} of {num_items}): {item['Title']} ({item['Year']}): {item['Rating']}/10 on Trakt")
 
                     # Make the API call to rate the item
-                    response = errorHandling.make_trakt_request(rate_url, payload=data)
+                    response = EH.make_trakt_request(rate_url, payload=data)
 
                     if response is None:
                         print(f"Error rating {item}: {response.content}")
 
                 print('Setting Trakt Ratings Complete')
             else:
                 print('No Trakt Ratings To Set')
             
             if imdb_reviews_to_set:
                 # Call the check_last_run() function
-                if verifyCredentials.check_imdb_reviews_last_submitted():
+                if VC.check_imdb_reviews_last_submitted():
                     print('Setting IMDB Reviews')
                     
                     for review in imdb_reviews_to_set:
                     
                         driver.get(f'https://contribute.imdb.com/review/{review["ID"]}/add?bus=imdb')
                         
                         review_title_input = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, "input.klondike-input")))
@@ -288,15 +288,15 @@
                     elif media_type == 'episode':
                         data['episode'] = {
                             "ids": {
                                 "imdb": episode_id
                             }
                         }
                     
-                    response = errorHandling.make_trakt_request(url, payload=data)
+                    response = EH.make_trakt_request(url, payload=data)
                     if response:
                         print(f"Submitted comment ({item_count} of {num_items}): {review['Title']} ({review['Year']}) on Trakt")
                     else:
                         print(f"Failed to submit comment ({item_count} of {num_items}): {review['Title']} ({review['Year']}) on Trakt")
                         print("Error Response:", response.content, response.status_code)
 
                 print('Trakt Reviews Set Successfully')
@@ -306,11 +306,11 @@
         #Close web driver
         print("Closing webdriver...")
         driver.quit()
         service.stop()
     
     except Exception as e:
         error_message = "An error occurred while running the script."
-        errorHandling.report_error(error_message)
+        EH.report_error(error_message)
 
 if __name__ == '__main__':
     main()
```

### Comparing `IMDBTraktSyncer-1.2.1/IMDBTraktSyncer/authTrakt.py` & `IMDBTraktSyncer-1.2.2/IMDBTraktSyncer/authTrakt.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import requests
 import time
 try:
-    from IMDBTraktSyncer import errorHandling
-except:
-    import errorHandling
+    from IMDBTraktSyncer import errorHandling as EH
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
-    response = errorHandling.make_trakt_request('https://api.trakt.tv/oauth/token', payload=data)
+    response = EH.make_trakt_request('https://api.trakt.tv/oauth/token', payload=data)
 
     # Parse the JSON response from the API
     json_data = response.json()
 
     # Extract the access token from the response
     ACCESS_TOKEN = json_data['access_token']
```

### Comparing `IMDBTraktSyncer-1.2.1/IMDBTraktSyncer/checkChromedriver.py` & `IMDBTraktSyncer-1.2.2/IMDBTraktSyncer/checkChromedriver.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.2.1/IMDBTraktSyncer/errorHandling.py` & `IMDBTraktSyncer-1.2.2/IMDBTraktSyncer/errorHandling.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import traceback
 import requests
 try:
-    from IMDBTraktSyncer import verifyCredentials
-except:
-    import verifyCredentials
+    from IMDBTraktSyncer import verifyCredentials as VC
+except ImportError:
+    import verifyCredentials as VC
 
 def report_error(error_message):
     github_issue_url = "https://github.com/RileyXX/IMDB-Trakt-Syncer/issues/new?template=bug_report.yml"
     traceback_info = traceback.format_exc()
 
     print("\n--- ERROR ---")
     print(error_message)
@@ -19,16 +19,16 @@
     print("-" * 50)
 
 def make_trakt_request(url, headers=None, params=None, payload=None, max_retries=3):
     if headers is None:
         headers = {
             'Content-Type': 'application/json',
             'trakt-api-version': '2',
-            'trakt-api-key': verifyCredentials.trakt_client_id,
-            'Authorization': f'Bearer {verifyCredentials.trakt_access_token}'
+            'trakt-api-key': VC.trakt_client_id,
+            'Authorization': f'Bearer {VC.trakt_access_token}'
         }
 
     retry_delay = 5  # seconds between retries
     retry_attempts = 0
 
     while retry_attempts < max_retries:
         response = None
```

### Comparing `IMDBTraktSyncer-1.2.1/IMDBTraktSyncer/imdbData.py` & `IMDBTraktSyncer-1.2.2/IMDBTraktSyncer/imdbData.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,17 @@
 from selenium.webdriver.common.by import By
 from selenium.common.exceptions import NoSuchElementException, TimeoutException, StaleElementReferenceException
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
 from chromedriver_py import binary_path
 try:
-    from IMDBTraktSyncer import verifyCredentials
-    from IMDBTraktSyncer import errorHandling
-except:
-    import verifyCredentials
-    import errorHandling
+    from IMDBTraktSyncer import errorHandling as EH
+except ImportError:
+    import errorHandling as EH
 
 def getImdbData(imdb_username, imdb_password, driver, directory, wait):
     # Process IMDB Ratings and Reviews
     print('Processing IMDB Ratings and Reviews')
 
     driver.get('https://www.imdb.com/list/ratings')
 
@@ -66,19 +64,19 @@
     #Get IMDB Reviews
     driver.get('https://www.imdb.com/profile')
     reviews_link = driver.find_element(By.CSS_SELECTOR, "div.aux-content-widget-2 div.subNavItem a[href*='comments-index']")
     reviews_link.click()
     
     def get_media_type(imdb_id):
         url = f"https://api.trakt.tv/search/imdb/{imdb_id}"
-        response = errorHandling.make_trakt_request(url)
+        response = EH.make_trakt_request(url)
         if response:
             results = response.json()
             if results:
-                media_type = results[0]['type']
+                media_type = results[0].get('type')
                 return media_type
         return None
 
     reviews = []
 
     while True:
         try:
```

### Comparing `IMDBTraktSyncer-1.2.1/IMDBTraktSyncer/traktData.py` & `IMDBTraktSyncer-1.2.2/IMDBTraktSyncer/traktData.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,77 +1,84 @@
 import json
 import requests
 import time
 try:
-    from IMDBTraktSyncer import errorHandling
-except:
-    import errorHandling
+    from IMDBTraktSyncer import errorHandling as EH
+except ImportError:
+    import errorHandling as EH
 
 def getTraktData():
     # Process Trakt Ratings and Comments
     print('Processing Trakt Ratings and Comments')
 
-    response = errorHandling.make_trakt_request('https://api.trakt.tv/users/me')
+    response = EH.make_trakt_request('https://api.trakt.tv/users/me')
     json_data = json.loads(response.text)
     username = json_data['username']
 
     # Get Trakt Ratings
-    response = errorHandling.make_trakt_request(f'https://api.trakt.tv/users/{username}/ratings')
+    response = EH.make_trakt_request(f'https://api.trakt.tv/users/{username}/ratings')
     json_data = json.loads(response.text)
 
     movie_ratings = []
     show_ratings = []
     episode_ratings = []
 
     for item in json_data:
         if item['type'] == 'movie':
-            movie = item['movie']
-            movie_id = movie['ids']['imdb']
-            movie_ratings.append({'Title': movie['title'], 'Year': movie['year'], 'Rating': item['rating'], 'ID': movie_id, 'Type': 'movie'})
+            movie = item.get('movie')
+            movie_id = movie.get('ids', {}).get('imdb')
+            movie_ratings.append({'Title': movie.get('title'), 'Year': movie.get('year'), 'Rating': item.get('rating'), 'ID': movie_id, 'Type': 'movie'})
         elif item['type'] == 'show':
-            show = item['show']
-            show_id = show['ids']['imdb']
-            show_ratings.append({'Title': show['title'], 'Year': show['year'], 'Rating': item['rating'], 'ID': show_id, 'Type': 'show'})
+            show = item.get('show')
+            show_id = show.get('ids', {}).get('imdb')
+            show_ratings.append({'Title': show.get('title'), 'Year': show.get('year'), 'Rating': item.get('rating'), 'ID': show_id, 'Type': 'show'})
         elif item['type'] == 'episode':
-            show = item['show']
-            show_title = show['title']
-            episode = item['episode']
-            episode_id = episode['ids']['imdb']
-            episode_title = f'{show_title}: {episode["title"]}'
-            episode_ratings.append({'Title': episode_title, 'Year': episode.get('year'), 'Rating': item['rating'], 'ID': episode_id, 'Type': 'episode'})
+            show = item.get('show')
+            show_title = show.get('title')
+            episode = item.get('episode')
+            episode_id = episode.get('ids', {}).get('imdb')
+            episode_title = f'{show_title}: {episode.get("title")}'
+            episode_ratings.append({'Title': episode_title, 'Year': episode.get('year'), 'Rating': item.get('rating'), 'ID': episode_id, 'Type': 'episode'})
 
     trakt_ratings = movie_ratings + show_ratings + episode_ratings
 
     # Get Trakt Comments
-    response = errorHandling.make_trakt_request(f'https://api.trakt.tv/users/{username}/comments')
+    response = EH.make_trakt_request(f'https://api.trakt.tv/users/{username}/comments')
     json_data = json.loads(response.text)
     total_pages = response.headers.get('X-Pagination-Page-Count')
     trakt_comments = []
 
     for page in range(1, int(total_pages) + 1):
-        response = errorHandling.make_trakt_request(f'https://api.trakt.tv/users/{username}/comments', params={'page': page})
+        response = EH.make_trakt_request(f'https://api.trakt.tv/users/{username}/comments', params={'page': page})
         json_data = json.loads(response.text)
 
         for comment in json_data:
             comment_type = comment['type']
             spoiler = comment.get('spoiler', False)
+
             if comment_type == 'movie':
-                show_movie_or_episode_title = comment['movie']['title']
-                show_movie_or_episode_year = comment['movie'].get('year')
-                show_movie_or_episode_imdb_id = comment['movie']['ids']['imdb']
+                movie = comment.get('movie')
+                show_movie_or_episode_title = movie.get('title')
+                show_movie_or_episode_year = movie.get('year')
+                show_movie_or_episode_imdb_id = movie.get('ids', {}).get('imdb')
             elif comment_type == 'episode':
-                show_movie_or_episode_title = f"{comment['show']['title']}: {comment['episode']['title']}"
-                show_movie_or_episode_year = comment['show'].get('year')
-                show_movie_or_episode_imdb_id = comment['episode']['ids']['imdb']
+                show = comment.get('show')
+                episode = comment.get('episode')
+                show_movie_or_episode_title = f"{show.get('title')}: {episode.get('title')}"
+                show_movie_or_episode_year = show.get('year')
+                show_movie_or_episode_imdb_id = episode.get('ids', {}).get('imdb')
             elif comment_type == 'show':
-                show_movie_or_episode_title = comment['show']['title']
-                show_movie_or_episode_year = comment['show'].get('year')
-                show_movie_or_episode_imdb_id = comment['show']['ids']['imdb']
+                show = comment.get('show')
+                show_movie_or_episode_title = show.get('title')
+                show_movie_or_episode_year = show.get('year')
+                show_movie_or_episode_imdb_id = show.get('ids', {}).get('imdb')
             elif comment_type == 'season':
-                show_movie_or_episode_title = f"{comment['show']['title']}: Season {comment['season']['number']}"
+                show = comment.get('show')
+                season = comment.get('season')
+                show_movie_or_episode_title = f"{show.get('title')}: Season {season.get('number')}"
                 show_movie_or_episode_year = None
                 show_movie_or_episode_imdb_id = None
             else:
                 show_movie_or_episode_title = None
                 show_movie_or_episode_year = None
                 show_movie_or_episode_imdb_id = None
```

### Comparing `IMDBTraktSyncer-1.2.1/IMDBTraktSyncer/verifyCredentials.py` & `IMDBTraktSyncer-1.2.2/IMDBTraktSyncer/verifyCredentials.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import json
 import datetime
 try:
     from IMDBTraktSyncer import authTrakt
-except:
+except ImportError:
     import authTrakt
 
 # Define the file path
 here = os.path.abspath(os.path.dirname(__file__))
 file_path = os.path.join(here, 'credentials.txt')
 
 # Old version support (v1.0.6 and below). Convert old credentials.txt format to json
```

### Comparing `IMDBTraktSyncer-1.2.1/IMDBTraktSyncer.egg-info/PKG-INFO` & `IMDBTraktSyncer-1.2.2/IMDBTraktSyncer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDBTraktSyncer
-Version: 1.2.1
+Version: 1.2.2
 Summary: This python script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDB.
 Home-page: https://github.com/RileyXX/IMDB-Trakt-Syncer
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `IMDBTraktSyncer-1.2.1/IMDBTraktSyncer.egg-info/SOURCES.txt` & `IMDBTraktSyncer-1.2.2/IMDBTraktSyncer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.2.1/LICENSE` & `IMDBTraktSyncer-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.2.1/PKG-INFO` & `IMDBTraktSyncer-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDBTraktSyncer
-Version: 1.2.1
+Version: 1.2.2
 Summary: This python script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDB.
 Home-page: https://github.com/RileyXX/IMDB-Trakt-Syncer
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `IMDBTraktSyncer-1.2.1/README.md` & `IMDBTraktSyncer-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.2.1/setup.py` & `IMDBTraktSyncer-1.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.2.1'
+VERSION = '1.2.2'
 DESCRIPTION = 'This python script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDB.'
 
 # Setting up
 setup(
     name="IMDBTraktSyncer",
     version=VERSION,
     description=DESCRIPTION,
```

