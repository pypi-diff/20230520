# Comparing `tmp/TruMusic-1.1.5.tar.gz` & `tmp/TruMusic-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TruMusic-1.1.5.tar", last modified: Fri May 19 23:36:26 2023, max compression
+gzip compressed data, was "TruMusic-1.1.6.tar", last modified: Sat May 20 00:33:04 2023, max compression
```

## Comparing `TruMusic-1.1.5.tar` & `TruMusic-1.1.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 23:36:26.441673 TruMusic-1.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-19 23:36:26.441673 TruMusic-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-19 23:36:12.000000 TruMusic-1.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 23:36:26.437673 TruMusic-1.1.5/TruMusic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-19 23:36:26.000000 TruMusic-1.1.5/TruMusic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-19 23:36:26.000000 TruMusic-1.1.5/TruMusic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 23:36:26.000000 TruMusic-1.1.5/TruMusic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-19 23:36:26.000000 TruMusic-1.1.5/TruMusic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-19 23:36:26.000000 TruMusic-1.1.5/TruMusic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-19 23:36:26.000000 TruMusic-1.1.5/TruMusic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-19 23:36:12.000000 TruMusic-1.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 23:36:26.441673 TruMusic-1.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-19 23:36:12.000000 TruMusic-1.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 23:36:26.437673 TruMusic-1.1.5/tru_music/
--rw-r--r--   0 runner    (1001) docker     (123)    14090 2023-05-19 23:36:12.000000 TruMusic-1.1.5/tru_music/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 23:36:26.441673 TruMusic-1.1.5/tru_music/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 23:36:12.000000 TruMusic-1.1.5/tru_music/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-19 23:36:12.000000 TruMusic-1.1.5/tru_music/scripts/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-05-19 23:36:12.000000 TruMusic-1.1.5/tru_music/scripts/trumusic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:33:04.198783 TruMusic-1.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-20 00:33:04.198783 TruMusic-1.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-20 00:32:49.000000 TruMusic-1.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:33:04.198783 TruMusic-1.1.6/TruMusic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-20 00:33:04.000000 TruMusic-1.1.6/TruMusic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-20 00:33:04.000000 TruMusic-1.1.6/TruMusic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 00:33:04.000000 TruMusic-1.1.6/TruMusic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-20 00:33:04.000000 TruMusic-1.1.6/TruMusic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-20 00:33:04.000000 TruMusic-1.1.6/TruMusic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-20 00:33:04.000000 TruMusic-1.1.6/TruMusic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-20 00:32:49.000000 TruMusic-1.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 00:33:04.198783 TruMusic-1.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-20 00:32:49.000000 TruMusic-1.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:33:04.198783 TruMusic-1.1.6/tru_music/
+-rw-r--r--   0 runner    (1001) docker     (123)    14664 2023-05-20 00:32:49.000000 TruMusic-1.1.6/tru_music/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:33:04.198783 TruMusic-1.1.6/tru_music/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 00:32:49.000000 TruMusic-1.1.6/tru_music/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-20 00:32:49.000000 TruMusic-1.1.6/tru_music/scripts/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-05-20 00:32:49.000000 TruMusic-1.1.6/tru_music/scripts/trumusic.py
```

### Comparing `TruMusic-1.1.5/PKG-INFO` & `TruMusic-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TruMusic
-Version: 1.1.5
+Version: 1.1.6
 Summary: Audio file auto-tagger
 Author-email: Jacob Truman <jacob.truman@gmail.com>
 Project-URL: homepage, https://github.com/jacobtruman/TruMusic
 Project-URL: documentation, https://github.com/jacobtruman/TruMusic
 Project-URL: repository, https://github.com/jacobtruman/TruMusic
 Requires-Python: <4,>=3.7
 Description-Content-Type: text/markdown
```

### Comparing `TruMusic-1.1.5/TruMusic.egg-info/PKG-INFO` & `TruMusic-1.1.6/TruMusic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TruMusic
-Version: 1.1.5
+Version: 1.1.6
 Summary: Audio file auto-tagger
 Author-email: Jacob Truman <jacob.truman@gmail.com>
 Project-URL: homepage, https://github.com/jacobtruman/TruMusic
 Project-URL: documentation, https://github.com/jacobtruman/TruMusic
 Project-URL: repository, https://github.com/jacobtruman/TruMusic
 Requires-Python: <4,>=3.7
 Description-Content-Type: text/markdown
```

### Comparing `TruMusic-1.1.5/pyproject.toml` & `TruMusic-1.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = 'TruMusic'
-version = '1.1.5'
+version = '1.1.6'
 description='Audio file auto-tagger'
 
 authors = [
     {name = "Jacob Truman", email="jacob.truman@gmail.com"},
 ]
 
 dependencies = [
```

### Comparing `TruMusic-1.1.5/tru_music/__init__.py` & `TruMusic-1.1.6/tru_music/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-import logging
-
-import mutagen
 import os.path
 import re
-import requests
+import readline  # this is imported to fix input usage
 import shutil
 import sys
 
+import requests
+
 import trulogger
 
 import musicbrainzngs
 
+import mutagen
 from mutagen.id3 import APIC, TIT2, TALB, TPE1, TPE2, TRCK, TDRC, TPOS, TCON
 from mutagen.mp4 import MP4Cover
 
 import pylast
 
 
 class TruMusic:
@@ -40,26 +40,27 @@
             "track": TRCK,
             "disk": TPOS,
             "cover": APIC,
             # "genre": TCON,
         }
     }
 
+    # pylint: disable=too-many-arguments
     def __init__(
             self,
             lastfm_api_key: str,
             lastfm_api_secret: str,
             ext: str = '.mp3',
             dry_run: bool = False,
             quiet: bool = False,
             verbose: bool = False,
     ):
         musicbrainzngs.set_useragent("TruMusic", 1.0)
         if lastfm_api_key is None or lastfm_api_secret is None:
-            raise Exception("Must provide last.fm api key and secret")
+            raise pylast.PyLastError("Must provide last.fm api key and secret")
         self.ext = ext
         self.dry_run = dry_run
         self.logger = trulogger.TruLogger({'verbose': verbose})
         self.quiet = quiet
 
         self._image_file: str = None
 
@@ -68,20 +69,20 @@
     @property
     def image_file(self):
         if self._image_file is None:
             album_art_file = f"{self.album_info['path']}/art.jpg"
             album_art_url = self.album_info['image_url']
             try:
                 if album_art_url is not None:
-                    r = requests.get(album_art_url, stream=True)
-                    if r.status_code == 200:
+                    req = requests.get(album_art_url, stream=True, timeout=10)
+                    if req.status_code == 200:
                         # Set decode_content value to True, otherwise the downloaded image file's size will be zero.
-                        r.raw.decode_content = True
-                        with open(album_art_file, 'wb') as f:
-                            shutil.copyfileobj(r.raw, f)
+                        req.raw.decode_content = True
+                        with open(album_art_file, 'wb') as file_handle:
+                            shutil.copyfileobj(req.raw, file_handle)
                             self._image_file = album_art_file
             except pylast.WSError as err:
                 print(err)
         return self._image_file
 
     @staticmethod
     def _clean_string(title):
@@ -105,14 +106,15 @@
 
     def _cleanup(self):
         if self.image_file is not None and os.path.exists(self.image_file):
             os.remove(self.image_file)
             self._image_file = None
             self.album_info = {}
 
+    # pylint: disable=too-many-branches,too-many-locals)
     def _get_album_info(self, album_artist: str, album_title: str):
         network = pylast.LastFMNetwork(
             api_key=os.environ.get('LASTFM_API_KEY', None),
             api_secret=os.environ.get('LASTFM_API_SECRET', None),
         )
 
         album_search = network.search_for_album(album_title)
@@ -176,14 +178,15 @@
             }
             return True
         except AttributeError as attrerr:
             self.logger.debug(album.get_url())
             self.logger.error(attrerr)
             return False
 
+    # pylint: disable=too-many-statements,too-many-branches,too-many-locals
     def tag_files(self, artist: str, album: str, track_files: list):
         """
         Tag audio files based on directory structure
         :param artist:
         :param album:
         :param track_files:
         :return:
@@ -202,14 +205,15 @@
             "album": album,
             "album_artist": artist,
             "year": self.album_info['release_date'],
             "cover": self.image_file
         }
 
         track_count = len(self.album_info['tracks'])
+        # pylint: disable=too-many-nested-blocks
         for num, track in self.album_info['tracks'].items():
             num = str(num).zfill(2)
             for track_file in track_files:
                 if track["title"].lower() in self._clean_string(track_file.lower()):
                     track_file_path = f"{self.album_info['path']}/{track_file}"
                     new_track_file_path = f"{self.album_info['path']}/{num} - {track['title']}{self.ext}"
                     if track_file_path != new_track_file_path:
@@ -236,51 +240,58 @@
                         del audiofile.tags
                     audiofile.add_tags()
 
                     file_type = audiofile.__class__.__name__
                     if file_type not in self.field_maps:
                         self.logger.error(f"Unsupported file type: {file_type}")
                         return False
-                    else:
-                        field_map = self.field_maps[file_type]
-                        for field in field_map:
-                            if field in track_tags:
-                                _field = field_map[field]
-                                if field == "cover":
-                                    if os.path.exists(track_tags[field]):
-                                        with open(track_tags[field], "rb") as f:
-                                            if file_type == "MP4":
-                                                audiofile.tags[_field] = [
-                                                    MP4Cover(f.read(), imageformat=MP4Cover.FORMAT_JPEG)
-                                                ]
-                                            elif file_type == "MP3":
-                                                audiofile.tags.add(
-                                                    APIC(mime='image/jpeg', type=3, desc=u'Cover', data=f.read()))
-                                            else:
-                                                self.logger.warning(f"Unsupported file type (cover art): {file_type}")
-                                    else:
-                                        self.logger.warning(f"Album art is missing: {track_tags[field]}")
+
+                    field_map = self.field_maps[file_type]
+                    for field in field_map:
+                        if field in track_tags:
+                            _field = field_map[field]
+                            if field == "cover":
+                                if os.path.exists(track_tags[field]):
+                                    with open(track_tags[field], "rb") as file_handle:
+                                        if file_type == "MP4":
+                                            audiofile.tags[_field] = [
+                                                MP4Cover(file_handle.read(), imageformat=MP4Cover.FORMAT_JPEG)
+                                            ]
+                                        elif file_type == "MP3":
+                                            audiofile.tags.add(
+                                                APIC(
+                                                    mime='image/jpeg',
+                                                    type=3,
+                                                    desc='Cover',
+                                                    data=file_handle.read()
+                                                )
+                                            )
+                                        else:
+                                            self.logger.warning(f"Unsupported file type (cover art): {file_type}")
                                 else:
-                                    if file_type == "MP3":
-                                        if field == "track" or field == "disk":
-                                            track_tags[field] = f"{track_tags[field][0]}/{track_tags[field][1]}"
-                                        audiofile.tags[_field] = field_map[field](encoding=3, text=track_tags[field])
-                                    elif file_type == "MP4":
-                                        audiofile.tags[_field] = [track_tags[field]]
+                                    self.logger.warning(f"Album art is missing: {track_tags[field]}")
                             else:
-                                self.logger.warning(f"Field not found in data: {field}")
+                                if file_type == "MP3":
+                                    if field in ["track", "disk"]:
+                                        track_tags[field] = f"{track_tags[field][0]}/{track_tags[field][1]}"
+                                    audiofile.tags[_field] = field_map[field](encoding=3, text=track_tags[field])
+                                elif file_type == "MP4":
+                                    audiofile.tags[_field] = [track_tags[field]]
+                        else:
+                            self.logger.warning(f"Field not found in data: {field}")
 
-                        if not self.dry_run:
-                            audiofile.save()
+                    if not self.dry_run:
+                        audiofile.save()
         if len(track_files) > 0:
             print(self.album_info['tracks'])
             self.logger.warning(f"{len(track_files)} files not processed:\n{track_files}")
         self._cleanup()
         return True
 
+    # pylint: disable=too-many-branches
     def clean_tags(self, _file_path):
         """
         Tag audio files based on directory structure
         :param _file_path:
         :return:
         """
 
@@ -290,14 +301,15 @@
 
         file_type = audiofile.__class__.__name__
         if file_type not in self.field_maps:
             self.logger.error(f"Unsupported file type: {file_type}")
             return False
 
         field_map = self.field_maps[file_type]
+        # pylint: disable=too-many-nested-blocks
         if hasattr(audiofile, "tags"):
             tags = {}
             for field, _field in field_map.items():
                 if _field in audiofile.tags:
                     field_data = audiofile.tags[_field]
                     if field == "cover":
                         if file_type == "MP4":
@@ -309,15 +321,15 @@
                             #audiofile.tags.add(
                             #    APIC(mime='image/jpeg', type=3, desc=u'Cover', data=field_data))
                         else:
                             self.logger.warning(f"Unsupported file type (cover art): {file_type}")
                     else:
                         if file_type == "MP3":
                             module = getattr(sys.modules[__name__], field_map[field])
-                            if field == "track" or field == "disk":
+                            if field in ["track", "disk"]:
                                 if str(field_data).endswith("/0") or str(field_data).startswith("0/"):
                                     field_data = "1/1"
                             tags[_field] = module(encoding=3, text=str(field_data))
                         elif file_type == "MP4":
                             tags[_field] = [field_data]
                 else:
                     self.logger.warning(f"Field not found in data: {field}/{_field}")
```

### Comparing `TruMusic-1.1.5/tru_music/scripts/trumusic.py` & `TruMusic-1.1.6/tru_music/scripts/trumusic.py`

 * *Files identical despite different names*

