# Comparing `tmp/TruMusic-1.1.4.tar.gz` & `tmp/TruMusic-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TruMusic-1.1.4.tar", last modified: Fri May 19 23:28:45 2023, max compression
+gzip compressed data, was "TruMusic-1.1.5.tar", last modified: Fri May 19 23:36:26 2023, max compression
```

## Comparing `TruMusic-1.1.4.tar` & `TruMusic-1.1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 23:28:45.425399 TruMusic-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-19 23:28:45.425399 TruMusic-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-19 23:28:33.000000 TruMusic-1.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 23:28:45.425399 TruMusic-1.1.4/TruMusic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-19 23:28:45.000000 TruMusic-1.1.4/TruMusic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-19 23:28:45.000000 TruMusic-1.1.4/TruMusic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 23:28:45.000000 TruMusic-1.1.4/TruMusic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-19 23:28:45.000000 TruMusic-1.1.4/TruMusic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-19 23:28:45.000000 TruMusic-1.1.4/TruMusic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-19 23:28:45.000000 TruMusic-1.1.4/TruMusic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-19 23:28:33.000000 TruMusic-1.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 23:28:45.425399 TruMusic-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-19 23:28:33.000000 TruMusic-1.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 23:28:45.425399 TruMusic-1.1.4/tru_music/
--rw-r--r--   0 runner    (1001) docker     (123)    13977 2023-05-19 23:28:33.000000 TruMusic-1.1.4/tru_music/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 23:28:45.425399 TruMusic-1.1.4/tru_music/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 23:28:33.000000 TruMusic-1.1.4/tru_music/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-19 23:28:33.000000 TruMusic-1.1.4/tru_music/scripts/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-05-19 23:28:33.000000 TruMusic-1.1.4/tru_music/scripts/trumusic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 23:36:26.441673 TruMusic-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-19 23:36:26.441673 TruMusic-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-19 23:36:12.000000 TruMusic-1.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 23:36:26.437673 TruMusic-1.1.5/TruMusic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-19 23:36:26.000000 TruMusic-1.1.5/TruMusic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-19 23:36:26.000000 TruMusic-1.1.5/TruMusic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 23:36:26.000000 TruMusic-1.1.5/TruMusic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-19 23:36:26.000000 TruMusic-1.1.5/TruMusic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-19 23:36:26.000000 TruMusic-1.1.5/TruMusic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-19 23:36:26.000000 TruMusic-1.1.5/TruMusic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-19 23:36:12.000000 TruMusic-1.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 23:36:26.441673 TruMusic-1.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-19 23:36:12.000000 TruMusic-1.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 23:36:26.437673 TruMusic-1.1.5/tru_music/
+-rw-r--r--   0 runner    (1001) docker     (123)    14090 2023-05-19 23:36:12.000000 TruMusic-1.1.5/tru_music/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 23:36:26.441673 TruMusic-1.1.5/tru_music/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 23:36:12.000000 TruMusic-1.1.5/tru_music/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-19 23:36:12.000000 TruMusic-1.1.5/tru_music/scripts/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-05-19 23:36:12.000000 TruMusic-1.1.5/tru_music/scripts/trumusic.py
```

### Comparing `TruMusic-1.1.4/PKG-INFO` & `TruMusic-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TruMusic
-Version: 1.1.4
+Version: 1.1.5
 Summary: Audio file auto-tagger
 Author-email: Jacob Truman <jacob.truman@gmail.com>
 Project-URL: homepage, https://github.com/jacobtruman/TruMusic
 Project-URL: documentation, https://github.com/jacobtruman/TruMusic
 Project-URL: repository, https://github.com/jacobtruman/TruMusic
 Requires-Python: <4,>=3.7
 Description-Content-Type: text/markdown
```

### Comparing `TruMusic-1.1.4/TruMusic.egg-info/PKG-INFO` & `TruMusic-1.1.5/TruMusic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TruMusic
-Version: 1.1.4
+Version: 1.1.5
 Summary: Audio file auto-tagger
 Author-email: Jacob Truman <jacob.truman@gmail.com>
 Project-URL: homepage, https://github.com/jacobtruman/TruMusic
 Project-URL: documentation, https://github.com/jacobtruman/TruMusic
 Project-URL: repository, https://github.com/jacobtruman/TruMusic
 Requires-Python: <4,>=3.7
 Description-Content-Type: text/markdown
```

### Comparing `TruMusic-1.1.4/pyproject.toml` & `TruMusic-1.1.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = 'TruMusic'
-version = '1.1.4'
+version = '1.1.5'
 description='Audio file auto-tagger'
 
 authors = [
     {name = "Jacob Truman", email="jacob.truman@gmail.com"},
 ]
 
 dependencies = [
```

### Comparing `TruMusic-1.1.4/tru_music/__init__.py` & `TruMusic-1.1.5/tru_music/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,23 +121,25 @@
         for res in results:
             if str(res.artist).casefold() == album_artist.casefold():
                 try:
                     album_tracks = res.get_tracks()
                 except pylast.WSError as pye:
                     self.logger.debug(pye)
                     continue
+                release_date = None
+                mbid = res.get_mbid()
+                if mbid is not None:
+                    release = musicbrainzngs.get_release_by_id(id=mbid)
+                    release_date = release['release']['date']
+                # this is hacky...
+                res.release_date = release_date
                 matching_results.append(res)
                 if not self.quiet:
-                    release_date = None
-                    mbid = res.get_mbid()
-                    if mbid is not None:
-                        release = musicbrainzngs.get_release_by_id(id=mbid)
-                        release_date = release['release']['date']
                     print(f"\t{len(matching_results)}. {album_artist} {res.title} ({len(album_tracks)} tracks) "
-                          f"({release_date})")
+                          f"({res.release_date})")
 
         album = None
         match_count = len(matching_results)
         if match_count == 1 or (match_count > 0 and self.quiet):
             album = matching_results[0]
         elif match_count > 1:
             while album is None:
@@ -151,14 +153,15 @@
             return False
 
         try:
             # get tracks and sort them by title length, preserving track number
             album_tracks = {num: track.title for num, track in enumerate(album.get_tracks(), start=1)}
             album_tracks_list = sorted(list(album_tracks.items()), key=lambda key: len(key[1]), reverse=True)
             album_tracks_sorted = {track[0]: {"title": self._clean_string(track[1])} for track in album_tracks_list}
+            release_date = album.release_date
 
             if not self.quiet or release_date is None:
                 rd_input = input(
                     f"Enter '{album_artist}: {album_title}' release date ({release_date or 'YYYY-MM-DD'}): "
                 )
                 if rd_input:
                     release_date = rd_input
```

### Comparing `TruMusic-1.1.4/tru_music/scripts/cleanup.py` & `TruMusic-1.1.5/tru_music/scripts/cleanup.py`

 * *Files identical despite different names*

### Comparing `TruMusic-1.1.4/tru_music/scripts/trumusic.py` & `TruMusic-1.1.5/tru_music/scripts/trumusic.py`

 * *Files identical despite different names*

