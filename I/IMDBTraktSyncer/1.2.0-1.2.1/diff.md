# Comparing `tmp/IMDBTraktSyncer-1.2.0.tar.gz` & `tmp/IMDBTraktSyncer-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IMDBTraktSyncer-1.2.0.tar", last modified: Sat May 20 02:08:50 2023, max compression
+gzip compressed data, was "IMDBTraktSyncer-1.2.1.tar", last modified: Sat May 20 18:54:16 2023, max compression
```

## Comparing `IMDBTraktSyncer-1.2.0.tar` & `IMDBTraktSyncer-1.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 02:08:50.642959 IMDBTraktSyncer-1.2.0/
-drwxrwxrwx   0        0        0        0 2023-05-20 02:08:50.607959 IMDBTraktSyncer-1.2.0/IMDBTraktSyncer/
--rw-rw-rw-   0        0        0    17942 2023-05-20 01:43:34.000000 IMDBTraktSyncer-1.2.0/IMDBTraktSyncer/IMDBTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDBTraktSyncer-1.2.0/IMDBTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     1968 2023-05-19 21:34:27.000000 IMDBTraktSyncer-1.2.0/IMDBTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0     4079 2023-05-16 01:53:33.000000 IMDBTraktSyncer-1.2.0/IMDBTraktSyncer/checkChromedriver.py
--rw-rw-rw-   0        0        0      488 2023-05-19 06:55:38.000000 IMDBTraktSyncer-1.2.0/IMDBTraktSyncer/errorHandling.py
--rw-rw-rw-   0        0        0     5719 2023-05-20 01:40:45.000000 IMDBTraktSyncer-1.2.0/IMDBTraktSyncer/imdbData.py
--rw-rw-rw-   0        0        0     4575 2023-05-19 22:36:23.000000 IMDBTraktSyncer-1.2.0/IMDBTraktSyncer/traktData.py
--rw-rw-rw-   0        0        0     5476 2023-05-20 02:05:00.000000 IMDBTraktSyncer-1.2.0/IMDBTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-05-20 02:08:50.639958 IMDBTraktSyncer-1.2.0/IMDBTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0     7755 2023-05-20 02:08:50.000000 IMDBTraktSyncer-1.2.0/IMDBTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      518 2023-05-20 02:08:50.000000 IMDBTraktSyncer-1.2.0/IMDBTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 02:08:50.000000 IMDBTraktSyncer-1.2.0/IMDBTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-05-20 02:08:50.000000 IMDBTraktSyncer-1.2.0/IMDBTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-05-20 02:08:50.000000 IMDBTraktSyncer-1.2.0/IMDBTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-20 02:08:50.000000 IMDBTraktSyncer-1.2.0/IMDBTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDBTraktSyncer-1.2.0/LICENSE
--rw-rw-rw-   0        0        0     7755 2023-05-20 02:08:50.641957 IMDBTraktSyncer-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     7095 2023-05-20 02:07:19.000000 IMDBTraktSyncer-1.2.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-20 02:08:50.642959 IMDBTraktSyncer-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1317 2023-05-20 02:08:26.000000 IMDBTraktSyncer-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 18:54:16.820654 IMDBTraktSyncer-1.2.1/
+drwxrwxrwx   0        0        0        0 2023-05-20 18:54:16.779655 IMDBTraktSyncer-1.2.1/IMDBTraktSyncer/
+-rw-rw-rw-   0        0        0    16494 2023-05-20 18:35:47.000000 IMDBTraktSyncer-1.2.1/IMDBTraktSyncer/IMDBTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDBTraktSyncer-1.2.1/IMDBTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     1900 2023-05-20 18:47:25.000000 IMDBTraktSyncer-1.2.1/IMDBTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0     4079 2023-05-16 01:53:33.000000 IMDBTraktSyncer-1.2.1/IMDBTraktSyncer/checkChromedriver.py
+-rw-rw-rw-   0        0        0     3851 2023-05-20 18:51:56.000000 IMDBTraktSyncer-1.2.1/IMDBTraktSyncer/errorHandling.py
+-rw-rw-rw-   0        0        0     5452 2023-05-20 18:48:39.000000 IMDBTraktSyncer-1.2.1/IMDBTraktSyncer/imdbData.py
+-rw-rw-rw-   0        0        0     4254 2023-05-20 18:47:44.000000 IMDBTraktSyncer-1.2.1/IMDBTraktSyncer/traktData.py
+-rw-rw-rw-   0        0        0     5476 2023-05-20 02:05:00.000000 IMDBTraktSyncer-1.2.1/IMDBTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-05-20 18:54:16.817655 IMDBTraktSyncer-1.2.1/IMDBTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0     7755 2023-05-20 18:54:16.000000 IMDBTraktSyncer-1.2.1/IMDBTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      518 2023-05-20 18:54:16.000000 IMDBTraktSyncer-1.2.1/IMDBTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 18:54:16.000000 IMDBTraktSyncer-1.2.1/IMDBTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-05-20 18:54:16.000000 IMDBTraktSyncer-1.2.1/IMDBTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2023-05-20 18:54:16.000000 IMDBTraktSyncer-1.2.1/IMDBTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-20 18:54:16.000000 IMDBTraktSyncer-1.2.1/IMDBTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDBTraktSyncer-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0     7755 2023-05-20 18:54:16.819654 IMDBTraktSyncer-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7095 2023-05-20 18:20:58.000000 IMDBTraktSyncer-1.2.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-20 18:54:16.820654 IMDBTraktSyncer-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1317 2023-05-20 18:53:59.000000 IMDBTraktSyncer-1.2.1/setup.py
```

### Comparing `IMDBTraktSyncer-1.2.0/IMDBTraktSyncer/IMDBTraktSyncer.py` & `IMDBTraktSyncer-1.2.1/IMDBTraktSyncer/IMDBTraktSyncer.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,17 +26,14 @@
 from chromedriver_py import binary_path
 
 
 def main():
     try:
 
         #Get credentials
-        trakt_client_id = verifyCredentials.trakt_client_id
-        trakt_client_secret = verifyCredentials.trakt_client_secret
-        trakt_access_token = verifyCredentials.trakt_access_token
         imdb_username = verifyCredentials.imdb_username
         imdb_password = verifyCredentials.imdb_password
         
         directory = os.path.dirname(os.path.realpath(__file__))
         
         logging.getLogger('selenium.webdriver').setLevel(logging.WARNING)
         
@@ -104,15 +101,15 @@
             print("\nPossible IMDB captcha check or IMDB login incorrect.")
             print("\nIf your login is correct then an IMDB captcha check likely the cause of this error. To fix this, simply login to the IMDB website in your browser, preferably Chrome, and from the same computer. If logged in, log out and log back in. It may ask you to fill in a captcha; complete it and finish logging in. After logging in successfully on your browser, run the script again and it should work. You may need to repeat this step once or twice if it still gives you issues.")
             print("\nIf your IMDB login is incorrect, simply edit the credentials.txt file with the correct login or delete the credentials file and run the script again.")
             print("\nSee this GitHub link for more details: https://github.com/RileyXX/IMDB-Trakt-Syncer/issues/2")
             print("\nStopping script...")
             raise SystemExit
         
-        trakt_ratings, trakt_reviews = traktData.getTraktData(trakt_client_id, trakt_access_token)
+        trakt_ratings, trakt_reviews = traktData.getTraktData()
         imdb_ratings, imdb_reviews = imdbData.getImdbData(imdb_username, imdb_password, driver, directory, wait)
 
         #Get trakt and imdb ratings and filter out trakt ratings with missing imdb id
         trakt_ratings = [rating for rating in trakt_ratings if rating['ID'] is not None]
         imdb_ratings = [rating for rating in imdb_ratings if rating['ID'] is not None]
         trakt_reviews = [review for review in trakt_reviews if review['ID'] is not None]
         imdb_reviews = [review for review in imdb_reviews if review['ID'] is not None]
@@ -164,24 +161,15 @@
 
         if verifyCredentials.sync_reviews_value:
             #Set Trakt Ratings
             if trakt_ratings_to_set:
                 print('Setting Trakt Ratings')
 
                 # Set the API endpoints
-                oauth_url = "https://api.trakt.tv/oauth/token"
                 rate_url = "https://api.trakt.tv/sync/ratings"
-
-                # Set the headers
-                headers = {
-                    "Content-Type": "application/json",
-                    "trakt-api-version": "2",
-                    "trakt-api-key": trakt_client_id,
-                    "Authorization": f"Bearer {trakt_access_token}"
-                }
                 
                 # Count the total number of items to rate
                 num_items = len(trakt_ratings_to_set)
                 item_count = 0
                         
                 # Loop through your data table and rate each item on Trakt
                 for item in trakt_ratings_to_set:
@@ -217,20 +205,17 @@
                                 },
                                 "rating": item["Rating"]
                             }]
                         }
                         print(f"Rating episode ({item_count} of {num_items}): {item['Title']} ({item['Year']}): {item['Rating']}/10 on Trakt")
 
                     # Make the API call to rate the item
-                    response = requests.post(rate_url, headers=headers, json=data)
-                    while response.status_code == 429:
-                        print("Rate limit exceeded. Waiting for 1 second...")
-                        time.sleep(1)
-                        response = requests.post(rate_url, headers=headers, json=data)
-                    if response.status_code != 201:
+                    response = errorHandling.make_trakt_request(rate_url, payload=data)
+
+                    if response is None:
                         print(f"Error rating {item}: {response.content}")
 
                 print('Setting Trakt Ratings Complete')
             else:
                 print('No Trakt Ratings To Set')
             
             if imdb_reviews_to_set:
@@ -277,21 +262,14 @@
                 item_count = 0
 
                 for review in trakt_reviews_to_set:
                     item_count += 1
                     imdb_id = review['ID']
                     comment = review['Comment']
                     media_type = review['Type']  # 'movie', 'show', or 'episode'
-                    
-                    headers = {
-                        "Content-Type": "application/json",
-                        "trakt-api-version": "2",
-                        "trakt-api-key": trakt_client_id,
-                        "Authorization": f"Bearer {trakt_access_token}"
-                    }
 
                     url = f"https://api.trakt.tv/comments"
 
                     data = {
                         "comment": comment
                     }
 
@@ -309,21 +287,17 @@
                         }
                     elif media_type == 'episode':
                         data['episode'] = {
                             "ids": {
                                 "imdb": episode_id
                             }
                         }
-
-                    response = requests.post(url, headers=headers, json=data)
-                    while response.status_code == 429:
-                        print("Rate limit exceeded. Waiting for 1 second...")
-                        time.sleep(1)
-                        response = requests.post(url, headers=headers, json=data)
-                    if response.status_code == 201:
+                    
+                    response = errorHandling.make_trakt_request(url, payload=data)
+                    if response:
                         print(f"Submitted comment ({item_count} of {num_items}): {review['Title']} ({review['Year']}) on Trakt")
                     else:
                         print(f"Failed to submit comment ({item_count} of {num_items}): {review['Title']} ({review['Year']}) on Trakt")
                         print("Error Response:", response.content, response.status_code)
 
                 print('Trakt Reviews Set Successfully')
             else:
```

### Comparing `IMDBTraktSyncer-1.2.0/IMDBTraktSyncer/authTrakt.py` & `IMDBTraktSyncer-1.2.1/IMDBTraktSyncer/authTrakt.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 import requests
 import time
+try:
+    from IMDBTraktSyncer import errorHandling
+except:
+    import errorHandling
 
 def authenticate(client_id, client_secret):
     CLIENT_ID = client_id
     CLIENT_SECRET = client_secret
     REDIRECT_URI = 'urn:ietf:wg:oauth:2.0:oob'
 
     # Set up the authorization endpoint URL
@@ -34,18 +38,15 @@
         'client_id': CLIENT_ID,
         'client_secret': CLIENT_SECRET,
         'redirect_uri': REDIRECT_URI,
         'grant_type': 'authorization_code'
     }
 
     # Make the request to get the access token
-    response = requests.post('https://api.trakt.tv/oauth/token', headers=headers, json=data)
-    while response.status_code == 429:
-        time.sleep(1)
-        response = requests.post('https://api.trakt.tv/oauth/token', headers=headers, json=data)
+    response = errorHandling.make_trakt_request('https://api.trakt.tv/oauth/token', payload=data)
 
     # Parse the JSON response from the API
     json_data = response.json()
 
     # Extract the access token from the response
     ACCESS_TOKEN = json_data['access_token']
```

### Comparing `IMDBTraktSyncer-1.2.0/IMDBTraktSyncer/checkChromedriver.py` & `IMDBTraktSyncer-1.2.1/IMDBTraktSyncer/checkChromedriver.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.2.0/IMDBTraktSyncer/imdbData.py` & `IMDBTraktSyncer-1.2.1/IMDBTraktSyncer/imdbData.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,16 +8,18 @@
 from selenium.common.exceptions import NoSuchElementException, TimeoutException, StaleElementReferenceException
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
 from chromedriver_py import binary_path
 try:
     from IMDBTraktSyncer import verifyCredentials
+    from IMDBTraktSyncer import errorHandling
 except:
     import verifyCredentials
+    import errorHandling
 
 def getImdbData(imdb_username, imdb_password, driver, directory, wait):
     # Process IMDB Ratings and Reviews
     print('Processing IMDB Ratings and Reviews')
 
     driver.get('https://www.imdb.com/list/ratings')
 
@@ -64,25 +66,16 @@
     #Get IMDB Reviews
     driver.get('https://www.imdb.com/profile')
     reviews_link = driver.find_element(By.CSS_SELECTOR, "div.aux-content-widget-2 div.subNavItem a[href*='comments-index']")
     reviews_link.click()
     
     def get_media_type(imdb_id):
         url = f"https://api.trakt.tv/search/imdb/{imdb_id}"
-        headers = {
-            "Content-Type": "application/json",
-            "trakt-api-version": "2",
-            "trakt-api-key": verifyCredentials.trakt_client_id
-        }
-        
-        response = requests.get(url, headers=headers)
-        while response.status_code == 429:
-            time.sleep(1)
-            response = requests.get(url, headers=headers)
-        if response.status_code == 200:
+        response = errorHandling.make_trakt_request(url)
+        if response:
             results = response.json()
             if results:
                 media_type = results[0]['type']
                 return media_type
         return None
 
     reviews = []
```

### Comparing `IMDBTraktSyncer-1.2.0/IMDBTraktSyncer/traktData.py` & `IMDBTraktSyncer-1.2.1/IMDBTraktSyncer/traktData.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 import json
 import requests
 import time
+try:
+    from IMDBTraktSyncer import errorHandling
+except:
+    import errorHandling
 
-def getTraktData(trakt_client_id, trakt_access_token):
+def getTraktData():
     # Process Trakt Ratings and Comments
     print('Processing Trakt Ratings and Comments')
 
-    headers = {
-        'Content-Type': 'application/json',
-        'trakt-api-version': '2',
-        'trakt-api-key': trakt_client_id,
-        'Authorization': f'Bearer {trakt_access_token}'
-    }
-
-    time.sleep(1) # avoid trakt rate limit
-    response = requests.get('https://api.trakt.tv/users/me', headers=headers)
+    response = errorHandling.make_trakt_request('https://api.trakt.tv/users/me')
     json_data = json.loads(response.text)
     username = json_data['username']
 
     # Get Trakt Ratings
-    time.sleep(1) # avoid trakt rate limit
-    response = requests.get(f'https://api.trakt.tv/users/{username}/ratings', headers=headers)
+    response = errorHandling.make_trakt_request(f'https://api.trakt.tv/users/{username}/ratings')
     json_data = json.loads(response.text)
 
     movie_ratings = []
     show_ratings = []
     episode_ratings = []
 
     for item in json_data:
@@ -43,23 +38,21 @@
             episode_id = episode['ids']['imdb']
             episode_title = f'{show_title}: {episode["title"]}'
             episode_ratings.append({'Title': episode_title, 'Year': episode.get('year'), 'Rating': item['rating'], 'ID': episode_id, 'Type': 'episode'})
 
     trakt_ratings = movie_ratings + show_ratings + episode_ratings
 
     # Get Trakt Comments
-    time.sleep(1) # avoid trakt rate limit
-    response = requests.get(f'https://api.trakt.tv/users/{username}/comments', headers=headers)
+    response = errorHandling.make_trakt_request(f'https://api.trakt.tv/users/{username}/comments')
     json_data = json.loads(response.text)
     total_pages = response.headers.get('X-Pagination-Page-Count')
     trakt_comments = []
 
     for page in range(1, int(total_pages) + 1):
-        time.sleep(1) # avoid trakt rate limit
-        response = requests.get(f'https://api.trakt.tv/users/{username}/comments', headers=headers, params={'page': page})
+        response = errorHandling.make_trakt_request(f'https://api.trakt.tv/users/{username}/comments', params={'page': page})
         json_data = json.loads(response.text)
 
         for comment in json_data:
             comment_type = comment['type']
             spoiler = comment.get('spoiler', False)
             if comment_type == 'movie':
                 show_movie_or_episode_title = comment['movie']['title']
```

### Comparing `IMDBTraktSyncer-1.2.0/IMDBTraktSyncer/verifyCredentials.py` & `IMDBTraktSyncer-1.2.1/IMDBTraktSyncer/verifyCredentials.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.2.0/IMDBTraktSyncer.egg-info/PKG-INFO` & `IMDBTraktSyncer-1.2.1/IMDBTraktSyncer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDBTraktSyncer
-Version: 1.2.0
+Version: 1.2.1
 Summary: This python script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDB.
 Home-page: https://github.com/RileyXX/IMDB-Trakt-Syncer
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `IMDBTraktSyncer-1.2.0/IMDBTraktSyncer.egg-info/SOURCES.txt` & `IMDBTraktSyncer-1.2.1/IMDBTraktSyncer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.2.0/LICENSE` & `IMDBTraktSyncer-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.2.0/PKG-INFO` & `IMDBTraktSyncer-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDBTraktSyncer
-Version: 1.2.0
+Version: 1.2.1
 Summary: This python script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDB.
 Home-page: https://github.com/RileyXX/IMDB-Trakt-Syncer
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `IMDBTraktSyncer-1.2.0/README.md` & `IMDBTraktSyncer-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.2.0/setup.py` & `IMDBTraktSyncer-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.2.0'
+VERSION = '1.2.1'
 DESCRIPTION = 'This python script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDB.'
 
 # Setting up
 setup(
     name="IMDBTraktSyncer",
     version=VERSION,
     description=DESCRIPTION,
```

