# Comparing `tmp/TruMusic-1.1.2.tar.gz` & `tmp/TruMusic-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TruMusic-1.1.2.tar", last modified: Fri May 19 22:50:27 2023, max compression
+gzip compressed data, was "TruMusic-1.1.3.tar", last modified: Fri May 19 23:23:37 2023, max compression
```

## Comparing `TruMusic-1.1.2.tar` & `TruMusic-1.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:50:27.142629 TruMusic-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-19 22:50:27.142629 TruMusic-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-19 22:50:13.000000 TruMusic-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:50:27.142629 TruMusic-1.1.2/TruMusic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-19 22:50:27.000000 TruMusic-1.1.2/TruMusic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-19 22:50:27.000000 TruMusic-1.1.2/TruMusic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 22:50:27.000000 TruMusic-1.1.2/TruMusic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-19 22:50:27.000000 TruMusic-1.1.2/TruMusic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-19 22:50:27.000000 TruMusic-1.1.2/TruMusic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-19 22:50:27.000000 TruMusic-1.1.2/TruMusic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-19 22:50:13.000000 TruMusic-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 22:50:27.142629 TruMusic-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-19 22:50:13.000000 TruMusic-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:50:27.142629 TruMusic-1.1.2/tru_music/
--rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-05-19 22:50:13.000000 TruMusic-1.1.2/tru_music/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:50:27.142629 TruMusic-1.1.2/tru_music/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 22:50:13.000000 TruMusic-1.1.2/tru_music/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-19 22:50:13.000000 TruMusic-1.1.2/tru_music/scripts/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-05-19 22:50:13.000000 TruMusic-1.1.2/tru_music/scripts/trumusic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 23:23:37.183331 TruMusic-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-19 23:23:37.183331 TruMusic-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-19 23:23:26.000000 TruMusic-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 23:23:37.183331 TruMusic-1.1.3/TruMusic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-19 23:23:37.000000 TruMusic-1.1.3/TruMusic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-19 23:23:37.000000 TruMusic-1.1.3/TruMusic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 23:23:37.000000 TruMusic-1.1.3/TruMusic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-19 23:23:37.000000 TruMusic-1.1.3/TruMusic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-19 23:23:37.000000 TruMusic-1.1.3/TruMusic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-19 23:23:37.000000 TruMusic-1.1.3/TruMusic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-19 23:23:26.000000 TruMusic-1.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 23:23:37.183331 TruMusic-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-19 23:23:26.000000 TruMusic-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 23:23:37.183331 TruMusic-1.1.3/tru_music/
+-rw-r--r--   0 runner    (1001) docker     (123)    13942 2023-05-19 23:23:26.000000 TruMusic-1.1.3/tru_music/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 23:23:37.183331 TruMusic-1.1.3/tru_music/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 23:23:26.000000 TruMusic-1.1.3/tru_music/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-19 23:23:26.000000 TruMusic-1.1.3/tru_music/scripts/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-05-19 23:23:26.000000 TruMusic-1.1.3/tru_music/scripts/trumusic.py
```

### Comparing `TruMusic-1.1.2/PKG-INFO` & `TruMusic-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TruMusic
-Version: 1.1.2
+Version: 1.1.3
 Summary: Audio file auto-tagger
 Author-email: Jacob Truman <jacob.truman@gmail.com>
 Project-URL: homepage, https://github.com/jacobtruman/TruMusic
 Project-URL: documentation, https://github.com/jacobtruman/TruMusic
 Project-URL: repository, https://github.com/jacobtruman/TruMusic
 Requires-Python: <4,>=3.7
 Description-Content-Type: text/markdown
```

### Comparing `TruMusic-1.1.2/TruMusic.egg-info/PKG-INFO` & `TruMusic-1.1.3/TruMusic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TruMusic
-Version: 1.1.2
+Version: 1.1.3
 Summary: Audio file auto-tagger
 Author-email: Jacob Truman <jacob.truman@gmail.com>
 Project-URL: homepage, https://github.com/jacobtruman/TruMusic
 Project-URL: documentation, https://github.com/jacobtruman/TruMusic
 Project-URL: repository, https://github.com/jacobtruman/TruMusic
 Requires-Python: <4,>=3.7
 Description-Content-Type: text/markdown
```

### Comparing `TruMusic-1.1.2/pyproject.toml` & `TruMusic-1.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = 'TruMusic'
-version = '1.1.2'
+version = '1.1.3'
 description='Audio file auto-tagger'
 
 authors = [
     {name = "Jacob Truman", email="jacob.truman@gmail.com"},
 ]
 
 dependencies = [
     "mutagen",
     "requests",
-    "pylast",
+    "pylast>=5.1.0",
     "musicbrainzngs",
     "TruLogger",
 ]
 
 requires-python = ">=3.7, <4"
 
 [project.urls]
```

### Comparing `TruMusic-1.1.2/tru_music/__init__.py` & `TruMusic-1.1.3/tru_music/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,17 +116,23 @@
         )
 
         album_search = network.search_for_album(album_title)
         results = album_search.get_next_page()
         matching_results = []
         for res in results:
             if str(res.artist).casefold() == album_artist.casefold():
+                try:
+                    album_tracks = res.get_tracks()
+                except pylast.WSError as pye:
+                    self.logger.debug(pye)
+                    continue
                 matching_results.append(res)
                 if not self.quiet:
-                    print(f"\t{len(matching_results)}. {album_artist} {res.title} ({len(res.get_tracks())} tracks)")
+                    print(f"\t{len(matching_results)}. {album_artist} {res.title} ({len(album_tracks)} tracks) "
+                          f"({res.get_mbid()})")
 
         album = None
         match_count = len(matching_results)
         if match_count == 1 or (match_count > 0 and self.quiet):
             album = matching_results[0]
         elif match_count > 1:
             while album is None:
```

### Comparing `TruMusic-1.1.2/tru_music/scripts/cleanup.py` & `TruMusic-1.1.3/tru_music/scripts/cleanup.py`

 * *Files identical despite different names*

### Comparing `TruMusic-1.1.2/tru_music/scripts/trumusic.py` & `TruMusic-1.1.3/tru_music/scripts/trumusic.py`

 * *Files identical despite different names*

