# Comparing `tmp/spotigrabber-0.0.1.tar.gz` & `tmp/spotigrabber-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\bebis\Dropbox\Code\spotigrabber\dist\.tmp-94jr9bs2\spotigrabber-0.0.1.tar", last modified: Thu May 18 10:02:16 2023, max compression
+gzip compressed data, was "spotigrabber-0.0.2.tar", last modified: Fri May 19 22:02:29 2023, max compression
```

## Comparing `spotigrabber-0.0.1.tar` & `spotigrabber-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 10:02:16.000000 spotigrabber-0.0.1/
--rw-rw-rw-   0        0        0     1091 2023-04-25 09:38:20.000000 spotigrabber-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     3650 2023-05-18 10:02:16.000000 spotigrabber-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3152 2023-05-18 09:57:56.000000 spotigrabber-0.0.1/README.md
--rw-rw-rw-   0        0        0     1004 2023-05-18 05:20:40.000000 spotigrabber-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-18 10:02:16.000000 spotigrabber-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-18 10:02:16.000000 spotigrabber-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-18 10:02:16.000000 spotigrabber-0.0.1/src/spotigrabber/
--rw-rw-rw-   0        0        0     9379 2023-05-18 09:53:53.000000 spotigrabber-0.0.1/src/spotigrabber/spotigrabber.py
-drwxrwxrwx   0        0        0        0 2023-05-18 10:02:16.000000 spotigrabber-0.0.1/src/spotigrabber.egg-info/
--rw-rw-rw-   0        0        0     3650 2023-05-18 10:02:16.000000 spotigrabber-0.0.1/src/spotigrabber.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2023-05-18 10:02:16.000000 spotigrabber-0.0.1/src/spotigrabber.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 10:02:16.000000 spotigrabber-0.0.1/src/spotigrabber.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      310 2023-05-18 10:02:16.000000 spotigrabber-0.0.1/src/spotigrabber.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-18 10:02:16.000000 spotigrabber-0.0.1/src/spotigrabber.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 22:02:29.355559 spotigrabber-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-04-25 09:38:20.000000 spotigrabber-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     3653 2023-05-19 22:02:29.355559 spotigrabber-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3155 2023-05-19 06:43:57.000000 spotigrabber-0.0.2/README.md
+-rw-rw-rw-   0        0        0     1004 2023-05-19 22:02:01.000000 spotigrabber-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-19 22:02:29.355559 spotigrabber-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-19 22:02:29.308686 spotigrabber-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-19 22:02:29.324311 spotigrabber-0.0.2/src/spotigrabber/
+-rw-rw-rw-   0        0        0     9379 2023-05-18 09:53:53.000000 spotigrabber-0.0.2/src/spotigrabber/spotigrabber.py
+drwxrwxrwx   0        0        0        0 2023-05-19 22:02:29.355559 spotigrabber-0.0.2/src/spotigrabber.egg-info/
+-rw-rw-rw-   0        0        0     3653 2023-05-19 22:02:29.000000 spotigrabber-0.0.2/src/spotigrabber.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2023-05-19 22:02:29.000000 spotigrabber-0.0.2/src/spotigrabber.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 22:02:29.000000 spotigrabber-0.0.2/src/spotigrabber.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      310 2023-05-19 22:02:29.000000 spotigrabber-0.0.2/src/spotigrabber.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-19 22:02:29.000000 spotigrabber-0.0.2/src/spotigrabber.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `spotigrabber-0.0.1/LICENSE.txt` & `spotigrabber-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `spotigrabber-0.0.1/PKG-INFO` & `spotigrabber-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: spotigrabber
-Version: 0.0.1
+Version: 0.0.2
 Summary: Grabber your spotify playlists and recently played songs.
 Author-email: bebissig <bebissig@gmail.com>
 Project-URL: Homepage, https://github.com/bebissig/spotify_grab_current_playlists
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Spotigrabber - Exporting your Spotify tracklists
 
-This Python package allows you to export your Spotify playlists and recently played tracks as an Excel file. It uses the Spotipy library to interact with the Spotify Web API. Due limitations of the spotify API, at maximum the last 50 played songs can be exported. Also, only songs that were listended all to the end are in the record.
+This Python package allows you to export your Spotify playlists and recently played tracks as an Excel file. It uses the Spotipy library to interact with the Spotify Web API. Due limitations of the spotify API, at maximum the last 50 played songs can be exported. Also, only songs that were listended all to the end are in the record. []
 
 ## Installation
 
 ### Setting up Spotify API credentials
 
 To access the Spotify API, you need to have API credentials in the form of a `client_id`, `client_secret`, and a `redirect_uri`. Here's how you can get your credentials:
```

### Comparing `spotigrabber-0.0.1/README.md` & `spotigrabber-0.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Spotigrabber - Exporting your Spotify tracklists
 
-This Python package allows you to export your Spotify playlists and recently played tracks as an Excel file. It uses the Spotipy library to interact with the Spotify Web API. Due limitations of the spotify API, at maximum the last 50 played songs can be exported. Also, only songs that were listended all to the end are in the record.
+This Python package allows you to export your Spotify playlists and recently played tracks as an Excel file. It uses the Spotipy library to interact with the Spotify Web API. Due limitations of the spotify API, at maximum the last 50 played songs can be exported. Also, only songs that were listended all to the end are in the record. []
 
 ## Installation
 
 ### Setting up Spotify API credentials
 
 To access the Spotify API, you need to have API credentials in the form of a `client_id`, `client_secret`, and a `redirect_uri`. Here's how you can get your credentials:
```

### Comparing `spotigrabber-0.0.1/pyproject.toml` & `spotigrabber-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "spotigrabber"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="bebissig", email="bebissig@gmail.com" },
 ]
 description = "Grabber your spotify playlists and recently played songs."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `spotigrabber-0.0.1/src/spotigrabber/spotigrabber.py` & `spotigrabber-0.0.2/src/spotigrabber/spotigrabber.py`

 * *Files identical despite different names*

### Comparing `spotigrabber-0.0.1/src/spotigrabber.egg-info/PKG-INFO` & `spotigrabber-0.0.2/src/spotigrabber.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: spotigrabber
-Version: 0.0.1
+Version: 0.0.2
 Summary: Grabber your spotify playlists and recently played songs.
 Author-email: bebissig <bebissig@gmail.com>
 Project-URL: Homepage, https://github.com/bebissig/spotify_grab_current_playlists
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Spotigrabber - Exporting your Spotify tracklists
 
-This Python package allows you to export your Spotify playlists and recently played tracks as an Excel file. It uses the Spotipy library to interact with the Spotify Web API. Due limitations of the spotify API, at maximum the last 50 played songs can be exported. Also, only songs that were listended all to the end are in the record.
+This Python package allows you to export your Spotify playlists and recently played tracks as an Excel file. It uses the Spotipy library to interact with the Spotify Web API. Due limitations of the spotify API, at maximum the last 50 played songs can be exported. Also, only songs that were listended all to the end are in the record. []
 
 ## Installation
 
 ### Setting up Spotify API credentials
 
 To access the Spotify API, you need to have API credentials in the form of a `client_id`, `client_secret`, and a `redirect_uri`. Here's how you can get your credentials:
```

