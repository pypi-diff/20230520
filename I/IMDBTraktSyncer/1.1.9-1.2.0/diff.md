# Comparing `tmp/IMDBTraktSyncer-1.1.9.tar.gz` & `tmp/IMDBTraktSyncer-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IMDBTraktSyncer-1.1.9.tar", last modified: Thu May 18 22:19:29 2023, max compression
+gzip compressed data, was "IMDBTraktSyncer-1.2.0.tar", last modified: Sat May 20 02:08:50 2023, max compression
```

## Comparing `IMDBTraktSyncer-1.1.9.tar` & `IMDBTraktSyncer-1.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 22:19:29.555166 IMDBTraktSyncer-1.1.9/
-drwxrwxrwx   0        0        0        0 2023-05-18 22:19:29.522167 IMDBTraktSyncer-1.1.9/IMDBTraktSyncer/
--rw-rw-rw-   0        0        0    11742 2023-05-18 19:51:06.000000 IMDBTraktSyncer-1.1.9/IMDBTraktSyncer/IMDBTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-05-18 19:51:06.000000 IMDBTraktSyncer-1.1.9/IMDBTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     1794 2023-05-18 19:51:06.000000 IMDBTraktSyncer-1.1.9/IMDBTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0     4079 2023-05-18 19:51:06.000000 IMDBTraktSyncer-1.1.9/IMDBTraktSyncer/checkChromedriver.py
--rw-rw-rw-   0        0        0      517 2023-05-18 22:18:58.000000 IMDBTraktSyncer-1.1.9/IMDBTraktSyncer/errorHandling.py
--rw-rw-rw-   0        0        0     2256 2023-05-18 19:51:06.000000 IMDBTraktSyncer-1.1.9/IMDBTraktSyncer/imdbRatings.py
--rw-rw-rw-   0        0        0     1846 2023-05-18 19:51:06.000000 IMDBTraktSyncer-1.1.9/IMDBTraktSyncer/traktRatings.py
--rw-rw-rw-   0        0        0     2524 2023-05-18 19:51:06.000000 IMDBTraktSyncer-1.1.9/IMDBTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-05-18 22:19:29.553166 IMDBTraktSyncer-1.1.9/IMDBTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0     7729 2023-05-18 22:19:29.000000 IMDBTraktSyncer-1.1.9/IMDBTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      524 2023-05-18 22:19:29.000000 IMDBTraktSyncer-1.1.9/IMDBTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 22:19:29.000000 IMDBTraktSyncer-1.1.9/IMDBTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-05-18 22:19:29.000000 IMDBTraktSyncer-1.1.9/IMDBTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-05-18 22:19:29.000000 IMDBTraktSyncer-1.1.9/IMDBTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-18 22:19:29.000000 IMDBTraktSyncer-1.1.9/IMDBTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1079 2023-05-18 19:51:06.000000 IMDBTraktSyncer-1.1.9/LICENSE
--rw-rw-rw-   0        0        0     7729 2023-05-18 22:19:29.554166 IMDBTraktSyncer-1.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     7069 2023-05-18 19:51:06.000000 IMDBTraktSyncer-1.1.9/README.md
--rw-rw-rw-   0        0        0       42 2023-05-18 22:19:29.555166 IMDBTraktSyncer-1.1.9/setup.cfg
--rw-rw-rw-   0        0        0     1317 2023-05-18 22:18:00.000000 IMDBTraktSyncer-1.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 02:08:50.642959 IMDBTraktSyncer-1.2.0/
+drwxrwxrwx   0        0        0        0 2023-05-20 02:08:50.607959 IMDBTraktSyncer-1.2.0/IMDBTraktSyncer/
+-rw-rw-rw-   0        0        0    17942 2023-05-20 01:43:34.000000 IMDBTraktSyncer-1.2.0/IMDBTraktSyncer/IMDBTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDBTraktSyncer-1.2.0/IMDBTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     1968 2023-05-19 21:34:27.000000 IMDBTraktSyncer-1.2.0/IMDBTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0     4079 2023-05-16 01:53:33.000000 IMDBTraktSyncer-1.2.0/IMDBTraktSyncer/checkChromedriver.py
+-rw-rw-rw-   0        0        0      488 2023-05-19 06:55:38.000000 IMDBTraktSyncer-1.2.0/IMDBTraktSyncer/errorHandling.py
+-rw-rw-rw-   0        0        0     5719 2023-05-20 01:40:45.000000 IMDBTraktSyncer-1.2.0/IMDBTraktSyncer/imdbData.py
+-rw-rw-rw-   0        0        0     4575 2023-05-19 22:36:23.000000 IMDBTraktSyncer-1.2.0/IMDBTraktSyncer/traktData.py
+-rw-rw-rw-   0        0        0     5476 2023-05-20 02:05:00.000000 IMDBTraktSyncer-1.2.0/IMDBTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-05-20 02:08:50.639958 IMDBTraktSyncer-1.2.0/IMDBTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0     7755 2023-05-20 02:08:50.000000 IMDBTraktSyncer-1.2.0/IMDBTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      518 2023-05-20 02:08:50.000000 IMDBTraktSyncer-1.2.0/IMDBTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 02:08:50.000000 IMDBTraktSyncer-1.2.0/IMDBTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-05-20 02:08:50.000000 IMDBTraktSyncer-1.2.0/IMDBTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2023-05-20 02:08:50.000000 IMDBTraktSyncer-1.2.0/IMDBTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-20 02:08:50.000000 IMDBTraktSyncer-1.2.0/IMDBTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDBTraktSyncer-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0     7755 2023-05-20 02:08:50.641957 IMDBTraktSyncer-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7095 2023-05-20 02:07:19.000000 IMDBTraktSyncer-1.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-20 02:08:50.642959 IMDBTraktSyncer-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1317 2023-05-20 02:08:26.000000 IMDBTraktSyncer-1.2.0/setup.py
```

### Comparing `IMDBTraktSyncer-1.1.9/IMDBTraktSyncer/authTrakt.py` & `IMDBTraktSyncer-1.2.0/IMDBTraktSyncer/authTrakt.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import requests
+import time
 
 def authenticate(client_id, client_secret):
     CLIENT_ID = client_id
     CLIENT_SECRET = client_secret
     REDIRECT_URI = 'urn:ietf:wg:oauth:2.0:oob'
 
     # Set up the authorization endpoint URL
@@ -34,14 +35,17 @@
         'client_secret': CLIENT_SECRET,
         'redirect_uri': REDIRECT_URI,
         'grant_type': 'authorization_code'
     }
 
     # Make the request to get the access token
     response = requests.post('https://api.trakt.tv/oauth/token', headers=headers, json=data)
+    while response.status_code == 429:
+        time.sleep(1)
+        response = requests.post('https://api.trakt.tv/oauth/token', headers=headers, json=data)
 
     # Parse the JSON response from the API
     json_data = response.json()
 
     # Extract the access token from the response
     ACCESS_TOKEN = json_data['access_token']
```

### Comparing `IMDBTraktSyncer-1.1.9/IMDBTraktSyncer/checkChromedriver.py` & `IMDBTraktSyncer-1.2.0/IMDBTraktSyncer/checkChromedriver.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.1.9/IMDBTraktSyncer.egg-info/PKG-INFO` & `IMDBTraktSyncer-1.2.0/IMDBTraktSyncer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: IMDBTraktSyncer
-Version: 1.1.9
+Version: 1.2.0
 Summary: This python script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDB.
 Home-page: https://github.com/RileyXX/IMDB-Trakt-Syncer
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # IMDB-Trakt-Syncer
-This Python script syncs user ratings for Movies, TV Shows and Episodes both ways between [Trakt](https://trakt.tv/) and [IMDB](https://imdb.com/). Ratings already set will not be overwritten. The script is compatible with operating systems that support Python (v3.6 or later) and Chromedriver (Windows, Linux, Mac, and ChromeOS). If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer).
+This Python script syncs user ratings and comments for Movies, TV Shows and Episodes both ways between [Trakt](https://trakt.tv/) and [IMDB](https://imdb.com/). Ratings and comments already set will not be overwritten. The script is compatible with operating systems that support Python (v3.6 or later) and Chromedriver (Windows, Linux, Mac, and ChromeOS). If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer).
 
 ## Installation Instructions
 1. Install [Python](https://www.python.org/downloads/) (v3.6 or later) and [Google Chrome](https://www.google.com/chrome/). _If these are already installed, you can skip this step. Please note this script does not affect Chrome in anyway, it is simply required in order for chromedriver to work._
 2. Install the script by executing `python -m pip install IMDBTraktSyncer` in command line.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `IMDBTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Run the script by executing `IMDBTraktSyncer` in the command line.
 5. Follow the prompts during the first run. You will need to enter your Trakt client ID and client secret from step 3, as well as your IMDB username and password. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script. It is recommended to change your IMDB password to something unique beforehand.
```

### Comparing `IMDBTraktSyncer-1.1.9/IMDBTraktSyncer.egg-info/SOURCES.txt` & `IMDBTraktSyncer-1.2.0/IMDBTraktSyncer.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 README.md
 setup.py
 IMDBTraktSyncer/IMDBTraktSyncer.py
 IMDBTraktSyncer/__init__.py
 IMDBTraktSyncer/authTrakt.py
 IMDBTraktSyncer/checkChromedriver.py
 IMDBTraktSyncer/errorHandling.py
-IMDBTraktSyncer/imdbRatings.py
-IMDBTraktSyncer/traktRatings.py
+IMDBTraktSyncer/imdbData.py
+IMDBTraktSyncer/traktData.py
 IMDBTraktSyncer/verifyCredentials.py
 IMDBTraktSyncer.egg-info/PKG-INFO
 IMDBTraktSyncer.egg-info/SOURCES.txt
 IMDBTraktSyncer.egg-info/dependency_links.txt
 IMDBTraktSyncer.egg-info/entry_points.txt
 IMDBTraktSyncer.egg-info/requires.txt
 IMDBTraktSyncer.egg-info/top_level.txt
```

### Comparing `IMDBTraktSyncer-1.1.9/LICENSE` & `IMDBTraktSyncer-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.1.9/PKG-INFO` & `IMDBTraktSyncer-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: IMDBTraktSyncer
-Version: 1.1.9
+Version: 1.2.0
 Summary: This python script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDB.
 Home-page: https://github.com/RileyXX/IMDB-Trakt-Syncer
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # IMDB-Trakt-Syncer
-This Python script syncs user ratings for Movies, TV Shows and Episodes both ways between [Trakt](https://trakt.tv/) and [IMDB](https://imdb.com/). Ratings already set will not be overwritten. The script is compatible with operating systems that support Python (v3.6 or later) and Chromedriver (Windows, Linux, Mac, and ChromeOS). If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer).
+This Python script syncs user ratings and comments for Movies, TV Shows and Episodes both ways between [Trakt](https://trakt.tv/) and [IMDB](https://imdb.com/). Ratings and comments already set will not be overwritten. The script is compatible with operating systems that support Python (v3.6 or later) and Chromedriver (Windows, Linux, Mac, and ChromeOS). If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer).
 
 ## Installation Instructions
 1. Install [Python](https://www.python.org/downloads/) (v3.6 or later) and [Google Chrome](https://www.google.com/chrome/). _If these are already installed, you can skip this step. Please note this script does not affect Chrome in anyway, it is simply required in order for chromedriver to work._
 2. Install the script by executing `python -m pip install IMDBTraktSyncer` in command line.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `IMDBTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Run the script by executing `IMDBTraktSyncer` in the command line.
 5. Follow the prompts during the first run. You will need to enter your Trakt client ID and client secret from step 3, as well as your IMDB username and password. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script. It is recommended to change your IMDB password to something unique beforehand.
```

### Comparing `IMDBTraktSyncer-1.1.9/README.md` & `IMDBTraktSyncer-1.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # IMDB-Trakt-Syncer
-This Python script syncs user ratings for Movies, TV Shows and Episodes both ways between [Trakt](https://trakt.tv/) and [IMDB](https://imdb.com/). Ratings already set will not be overwritten. The script is compatible with operating systems that support Python (v3.6 or later) and Chromedriver (Windows, Linux, Mac, and ChromeOS). If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer).
+This Python script syncs user ratings and comments for Movies, TV Shows and Episodes both ways between [Trakt](https://trakt.tv/) and [IMDB](https://imdb.com/). Ratings and comments already set will not be overwritten. The script is compatible with operating systems that support Python (v3.6 or later) and Chromedriver (Windows, Linux, Mac, and ChromeOS). If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer).
 
 ## Installation Instructions
 1. Install [Python](https://www.python.org/downloads/) (v3.6 or later) and [Google Chrome](https://www.google.com/chrome/). _If these are already installed, you can skip this step. Please note this script does not affect Chrome in anyway, it is simply required in order for chromedriver to work._
 2. Install the script by executing `python -m pip install IMDBTraktSyncer` in command line.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `IMDBTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Run the script by executing `IMDBTraktSyncer` in the command line.
 5. Follow the prompts during the first run. You will need to enter your Trakt client ID and client secret from step 3, as well as your IMDB username and password. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script. It is recommended to change your IMDB password to something unique beforehand.
```

### Comparing `IMDBTraktSyncer-1.1.9/setup.py` & `IMDBTraktSyncer-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.1.9'
+VERSION = '1.2.0'
 DESCRIPTION = 'This python script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDB.'
 
 # Setting up
 setup(
     name="IMDBTraktSyncer",
     version=VERSION,
     description=DESCRIPTION,
```

