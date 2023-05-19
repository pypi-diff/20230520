# Comparing `tmp/TruMusic-1.1.1.tar.gz` & `tmp/TruMusic-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TruMusic-1.1.1.tar", last modified: Fri Nov 18 18:52:17 2022, max compression
+gzip compressed data, was "TruMusic-1.1.2.tar", last modified: Fri May 19 22:50:27 2023, max compression
```

## Comparing `TruMusic-1.1.1.tar` & `TruMusic-1.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 18:52:17.104928 TruMusic-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (121)      698 2022-11-18 18:52:17.104928 TruMusic-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      298 2022-11-18 18:51:58.000000 TruMusic-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 18:52:17.104928 TruMusic-1.1.1/TruMusic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      698 2022-11-18 18:52:17.000000 TruMusic-1.1.1/TruMusic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      338 2022-11-18 18:52:17.000000 TruMusic-1.1.1/TruMusic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-18 18:52:17.000000 TruMusic-1.1.1/TruMusic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-11-18 18:52:17.000000 TruMusic-1.1.1/TruMusic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-11-18 18:52:17.000000 TruMusic-1.1.1/TruMusic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-11-18 18:52:17.000000 TruMusic-1.1.1/TruMusic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      643 2022-11-18 18:51:58.000000 TruMusic-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-18 18:52:17.104928 TruMusic-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      261 2022-11-18 18:51:58.000000 TruMusic-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 18:52:17.104928 TruMusic-1.1.1/tru_music/
--rw-r--r--   0 runner    (1001) docker     (121)    12564 2022-11-18 18:51:58.000000 TruMusic-1.1.1/tru_music/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 18:52:17.104928 TruMusic-1.1.1/tru_music/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-18 18:51:58.000000 TruMusic-1.1.1/tru_music/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1026 2022-11-18 18:51:58.000000 TruMusic-1.1.1/tru_music/scripts/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (121)     3331 2022-11-18 18:51:58.000000 TruMusic-1.1.1/tru_music/scripts/trumusic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:50:27.142629 TruMusic-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-19 22:50:27.142629 TruMusic-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-19 22:50:13.000000 TruMusic-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:50:27.142629 TruMusic-1.1.2/TruMusic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-19 22:50:27.000000 TruMusic-1.1.2/TruMusic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-19 22:50:27.000000 TruMusic-1.1.2/TruMusic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 22:50:27.000000 TruMusic-1.1.2/TruMusic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-19 22:50:27.000000 TruMusic-1.1.2/TruMusic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-19 22:50:27.000000 TruMusic-1.1.2/TruMusic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-19 22:50:27.000000 TruMusic-1.1.2/TruMusic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-19 22:50:13.000000 TruMusic-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 22:50:27.142629 TruMusic-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-19 22:50:13.000000 TruMusic-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:50:27.142629 TruMusic-1.1.2/tru_music/
+-rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-05-19 22:50:13.000000 TruMusic-1.1.2/tru_music/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:50:27.142629 TruMusic-1.1.2/tru_music/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 22:50:13.000000 TruMusic-1.1.2/tru_music/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-19 22:50:13.000000 TruMusic-1.1.2/tru_music/scripts/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-05-19 22:50:13.000000 TruMusic-1.1.2/tru_music/scripts/trumusic.py
```

### Comparing `TruMusic-1.1.1/PKG-INFO` & `TruMusic-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TruMusic
-Version: 1.1.1
+Version: 1.1.2
 Summary: Audio file auto-tagger
 Author-email: Jacob Truman <jacob.truman@gmail.com>
 Project-URL: homepage, https://github.com/jacobtruman/TruMusic
 Project-URL: documentation, https://github.com/jacobtruman/TruMusic
 Project-URL: repository, https://github.com/jacobtruman/TruMusic
 Requires-Python: <4,>=3.7
 Description-Content-Type: text/markdown
```

### Comparing `TruMusic-1.1.1/TruMusic.egg-info/PKG-INFO` & `TruMusic-1.1.2/TruMusic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TruMusic
-Version: 1.1.1
+Version: 1.1.2
 Summary: Audio file auto-tagger
 Author-email: Jacob Truman <jacob.truman@gmail.com>
 Project-URL: homepage, https://github.com/jacobtruman/TruMusic
 Project-URL: documentation, https://github.com/jacobtruman/TruMusic
 Project-URL: repository, https://github.com/jacobtruman/TruMusic
 Requires-Python: <4,>=3.7
 Description-Content-Type: text/markdown
```

### Comparing `TruMusic-1.1.1/pyproject.toml` & `TruMusic-1.1.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = 'TruMusic'
-version = '1.1.1'
+version = '1.1.2'
 description='Audio file auto-tagger'
 
 authors = [
     {name = "Jacob Truman", email="jacob.truman@gmail.com"},
 ]
 
 dependencies = [
```

### Comparing `TruMusic-1.1.1/tru_music/__init__.py` & `TruMusic-1.1.2/tru_music/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import logging
+
 import mutagen
 import os.path
 import re
 import requests
 import shutil
 import sys
 
@@ -109,29 +111,54 @@
 
     def _get_album_info(self, album_artist: str, album_title: str):
         network = pylast.LastFMNetwork(
             api_key=os.environ.get('LASTFM_API_KEY', None),
             api_secret=os.environ.get('LASTFM_API_SECRET', None),
         )
 
-        album = network.get_album(
-            album_artist,
-            self._clean_search_string(album_title),
-        )
+        album_search = network.search_for_album(album_title)
+        results = album_search.get_next_page()
+        matching_results = []
+        for res in results:
+            if str(res.artist).casefold() == album_artist.casefold():
+                matching_results.append(res)
+                if not self.quiet:
+                    print(f"\t{len(matching_results)}. {album_artist} {res.title} ({len(res.get_tracks())} tracks)")
+
+        album = None
+        match_count = len(matching_results)
+        if match_count == 1 or (match_count > 0 and self.quiet):
+            album = matching_results[0]
+        elif match_count > 1:
+            while album is None:
+                selection = int(input(f"{match_count} matching results found; select one: ")) - 1
+                if 0 <= selection < match_count:
+                    album = matching_results[selection]
+                else:
+                    print(f"Invalid selection {selection + 1}")
+        else:
+            self.logger.error(f"No match found for \"{album_artist}\" - \"{album_title}\"")
+            return False
 
         try:
-            release = musicbrainzngs.get_release_by_id(id=album.get_mbid())
+            release_date = None
+            mbid = album.get_mbid()
+            if mbid is not None:
+                release = musicbrainzngs.get_release_by_id(id=mbid)
+                release_date = release['release']['date']
+
             # get tracks and sort them by title length, preserving track number
             album_tracks = {num: track.title for num, track in enumerate(album.get_tracks(), start=1)}
             album_tracks_list = sorted(list(album_tracks.items()), key=lambda key: len(key[1]), reverse=True)
             album_tracks_sorted = {track[0]: {"title": self._clean_string(track[1])} for track in album_tracks_list}
 
-            release_date = release['release']['date']
-            if not self.quiet:
-                rd_input = input(f"Enter '{album_artist}: {album_title}' release date ({release['release']['date']}): ")
+            if not self.quiet or release_date is None:
+                rd_input = input(
+                    f"Enter '{album_artist}: {album_title}' release date ({release_date or 'YYYY-MM-DD'}): "
+                )
                 if rd_input:
                     release_date = rd_input
 
             self.album_info = {
                 "artist": album_artist,
                 "title": self._clean_string(album_title),
                 "release_date": release_date,
```

### Comparing `TruMusic-1.1.1/tru_music/scripts/cleanup.py` & `TruMusic-1.1.2/tru_music/scripts/cleanup.py`

 * *Files identical despite different names*

### Comparing `TruMusic-1.1.1/tru_music/scripts/trumusic.py` & `TruMusic-1.1.2/tru_music/scripts/trumusic.py`

 * *Files identical despite different names*

