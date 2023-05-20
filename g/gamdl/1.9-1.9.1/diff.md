# Comparing `tmp/gamdl-1.9.tar.gz` & `tmp/gamdl-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gamdl-1.9.tar", last modified: Thu Apr 20 01:50:40 2023, max compression
+gzip compressed data, was "gamdl-1.9.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gamdl-1.9.tar` & `gamdl-1.9.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1137 2023-04-20 01:50:35.698213 gamdl-1.9/.github/workflows/main.yml
--rw-r--r--   0        0        0       56 2023-04-20 01:50:35.698213 gamdl-1.9/.gitignore
--rw-r--r--   0        0        0     4041 2023-04-20 01:50:35.698213 gamdl-1.9/README.md
--rw-r--r--   0        0        0     7185 2023-04-20 01:50:35.698213 gamdl-1.9/gamdl/__init__.py
--rw-r--r--   0        0        0       58 2023-04-20 01:50:35.698213 gamdl-1.9/gamdl/__main__.py
--rw-r--r--   0        0        0    17627 2023-04-20 01:50:35.698213 gamdl-1.9/gamdl/gamdl.py
--rw-r--r--   0        0        0     2975 2023-04-20 01:50:35.698213 gamdl-1.9/gamdl/storefront_ids.py
--rw-r--r--   0        0        0      508 2023-04-20 01:50:35.698213 gamdl-1.9/pyproject.toml
--rw-r--r--   0        0        0       30 2023-04-20 01:50:35.698213 gamdl-1.9/requirements.txt
--rw-r--r--   0        0        0     4445 1970-01-01 00:00:00.000000 gamdl-1.9/PKG-INFO
+-rw-r--r--   0        0        0     1137 2023-05-20 17:20:04.878408 gamdl-1.9.1/.github/workflows/main.yml
+-rw-r--r--   0        0        0       56 2023-05-20 17:20:04.878408 gamdl-1.9.1/.gitignore
+-rw-r--r--   0        0        0     4016 2023-05-20 17:20:04.878408 gamdl-1.9.1/README.md
+-rw-r--r--   0        0        0     7318 2023-05-20 17:20:04.878408 gamdl-1.9.1/gamdl/__init__.py
+-rw-r--r--   0        0        0       58 2023-05-20 17:20:04.878408 gamdl-1.9.1/gamdl/__main__.py
+-rw-r--r--   0        0        0    17237 2023-05-20 17:20:04.878408 gamdl-1.9.1/gamdl/gamdl.py
+-rw-r--r--   0        0        0     2975 2023-05-20 17:20:04.878408 gamdl-1.9.1/gamdl/storefront_ids.py
+-rw-r--r--   0        0        0      508 2023-05-20 17:20:04.878408 gamdl-1.9.1/pyproject.toml
+-rw-r--r--   0        0        0       30 2023-05-20 17:20:04.878408 gamdl-1.9.1/requirements.txt
+-rw-r--r--   0        0        0     4422 1970-01-01 00:00:00.000000 gamdl-1.9.1/PKG-INFO
```

### Comparing `gamdl-1.9/.github/workflows/main.yml` & `gamdl-1.9.1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `gamdl-1.9/README.md` & `gamdl-1.9.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -38,56 +38,60 @@
             pywidevine create-device -t ANDROID -l 3 -k private_key.pem -c client_id.bin -o .
             ```
 6. (optional) Add aria2c to your PATH for faster downloads
     * You can get it from here: https://github.com/aria2/aria2/releases.
 
 ## Usage
 ```
-usage: gamdl [-h] [-u [URLS_TXT]] [-w WVD_LOCATION] [-f FINAL_PATH] [-t TEMP_PATH] [-c COOKIES_LOCATION] [-m]
-                   [-p] [-a] [-o] [-n] [-s] [-e] [-i] [-v]
+usage: __main__.py [-h] [-u [URLS_TXT]] [-w WVD_LOCATION] [-f FINAL_PATH]
+                   [-t TEMP_PATH] [-c COOKIES_LOCATION] [-m] [-p] [-o] [-n]
+                   [-l] [-s] [-e] [-v]
                    [url ...]
 
 Download Apple Music songs/music videos/albums/playlists
 
 positional arguments:
-  url                   Apple Music song/music video/album/playlist URL(s) (default: None)
+  url                   Apple Music song/music video/album/playlist URL(s)
+                        (default: None)
 
 options:
   -h, --help            show this help message and exit
   -u [URLS_TXT], --urls-txt [URLS_TXT]
                         Read URLs from a text file (default: None)
   -w WVD_LOCATION, --wvd-location WVD_LOCATION
-                        .wvd file location (default: *.wvd)
+                        .wvd file location (ignored if using -l/--lrc-only)
+                        (default: ./*.wvd)
   -f FINAL_PATH, --final-path FINAL_PATH
-                        Final Path (default: Apple Music)
+                        Final Path (default: ./Apple Music)
   -t TEMP_PATH, --temp-path TEMP_PATH
-                        Temp Path (default: temp)
+                        Temp Path (default: ./temp)
   -c COOKIES_LOCATION, --cookies-location COOKIES_LOCATION
-                        Cookies location (default: cookies.txt)
+                        Cookies location (default: ./cookies.txt)
   -m, --disable-music-video-skip
-                        Disable music video skip on playlists/albums (default: False)
+                        Disable music video skip on playlists/albums (default:
+                        False)
   -p, --prefer-hevc     Prefer HEVC over AVC (default: False)
-  -a, --heaac           Download songs/music videos with HE-AAC instead of AAC (default: False)
   -o, --overwrite       Overwrite existing files (default: False)
-  -n, --no-lrc          Don't create .lrc file (default: False)
+  -n, --no-lrc          Don't create .lrc file (ignored if using -l/--lrc-
+                        only) (default: False)
+  -l, --lrc-only        Skip downloading songs and only create .lrc files
+                        (default: False)
   -s, --skip-cleanup    Skip cleanup (default: False)
   -e, --print-exceptions
                         Print execeptions (default: False)
-  -i, --print-video-m3u8-url
-                        Print Video M3U8 URL (default: False)
   -v, --version         show program's version number and exit
 ```
 
 ## Songs/Music Videos quality
 * Songs:
-    * 256kbps AAC / HE-AAC 64kbps
+    * AAC 256kbps
 * Music Videos (varies depending on the video):
-    * 4K HEVC 20mbps, AAC 256kbps / HE-AAC 64kbps
-    * 4K HEVC 12mbps, AAC 256kbps / HE-AAC 64kbps
-    * 1080p AVC 10mbps, AAC 256kbps / HE-AAC 64kbps
-    * 1080p AVC 6.5bps, AAC 256kbps / HE-AAC 64kbps
-    * 720p AVC 4mbps, AAC 256kbps / HE-AAC 64kbps
-    * 576p AVC 2mbps, AAC 256kbps / HE-AAC 64kbps
-    * 480p AVC 1.5mbps, AAC 256kbps / HE-AAC 64kbps
-    * 360p AVC 1mbps, AAC 256kbps / HE-AAC 64kbps
+    * 4K HEVC 20mbps, AAC 256kbps
+    * 4K HEVC 12mbps, AAC 256kbps
+    * 1080p AVC 10mbps, AAC 256kbps
+    * 1080p AVC 6.5bps, AAC 256kbps
+    * 720p AVC 4mbps, AAC 256kbps
+    * 576p AVC 2mbps, AAC 256kbps
+    * 480p AVC 1.5mbps, AAC 256kbps
+    * 360p AVC 1mbps, AAC 256kbps
 
 Some videos may include EIA-608 closed captions.
```

### Comparing `gamdl-1.9/gamdl/__init__.py` & `gamdl-1.9.1/gamdl/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,128 +1,121 @@
 import shutil
 import argparse
 import traceback
 from .gamdl import Gamdl
 
-__version__ = '1.9'
+__version__ = '1.9.1'
 
 
 def main():
     if not shutil.which('mp4decrypt'):
         raise Exception('mp4decrypt is not on PATH')
     if not shutil.which('MP4Box'):
         raise Exception('MP4Box is not on PATH')
     parser = argparse.ArgumentParser(
-        description = 'Download Apple Music songs/music videos/albums/playlists',
-        formatter_class = argparse.ArgumentDefaultsHelpFormatter,
+        description='Download Apple Music songs/music videos/albums/playlists',
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
     parser.add_argument(
         'url',
-        help = 'Apple Music song/music video/album/playlist URL(s)',
-        nargs = '*',
+        help='Apple Music song/music video/album/playlist URL(s)',
+        nargs='*',
     )
     parser.add_argument(
         '-u',
         '--urls-txt',
-        help = 'Read URLs from a text file',
-        nargs = '?',
+        help='Read URLs from a text file',
+        nargs='?',
     )
     parser.add_argument(
         '-w',
         '--wvd-location',
-        default = '*.wvd',
-        help = '.wvd file location'
+        default='./*.wvd',
+        help='.wvd file location (ignored if using -l/--lrc-only)',
     )
     parser.add_argument(
         '-f',
         '--final-path',
-        default = 'Apple Music',
-        help = 'Final Path',
+        default='./Apple Music',
+        help='Final Path',
     )
     parser.add_argument(
         '-t',
         '--temp-path',
-        default = 'temp',
-        help = 'Temp Path',
+        default='./temp',
+        help='Temp Path',
     )
     parser.add_argument(
         '-c',
         '--cookies-location',
-        default = 'cookies.txt',
-        help = 'Cookies location',
+        default='./cookies.txt',
+        help='Cookies location',
     )
     parser.add_argument(
         '-m',
         '--disable-music-video-skip',
-        action = 'store_true',
-        help = 'Disable music video skip on playlists/albums',
+        action='store_true',
+        help='Disable music video skip on playlists/albums',
     )
     parser.add_argument(
         '-p',
         '--prefer-hevc',
-        action = 'store_true',
-        help = 'Prefer HEVC over AVC',
-    )
-    parser.add_argument(
-        '-a',
-        '--heaac',
-        action = 'store_true',
-        help = 'Download songs/music videos with HE-AAC instead of AAC',
+        action='store_true',
+        help='Prefer HEVC over AVC',
     )
     parser.add_argument(
         '-o',
         '--overwrite',
-        action = 'store_true',
-        help = 'Overwrite existing files',
+        action='store_true',
+        help='Overwrite existing files',
     )
     parser.add_argument(
         '-n',
         '--no-lrc',
-        action = 'store_true',
-        help = "Don't create .lrc file",
+        action='store_true',
+        help="Don't create .lrc file (ignored if using -l/--lrc-only)",
+    )
+    parser.add_argument(
+        '-l',
+        '--lrc-only',
+        action='store_true',
+        help='Skip downloading songs and only create .lrc files'
     )
     parser.add_argument(
         '-s',
         '--skip-cleanup',
-        action = 'store_true',
-        help = 'Skip cleanup',
+        action='store_true',
+        help='Skip cleanup',
     )
     parser.add_argument(
         '-e',
         '--print-exceptions',
-        action = 'store_true',
-        help = 'Print execeptions',
-    )
-    parser.add_argument(
-        '-i',
-        '--print-video-m3u8-url',
-        action = 'store_true',
-        help = 'Print Video M3U8 URL',
+        action='store_true',
+        help='Print execeptions',
     )
     parser.add_argument(
         '-v',
         '--version',
-        action = 'version',
-        version = f'%(prog)s {__version__}',
+        action='version',
+        version=f'%(prog)s {__version__}',
     )
     args = parser.parse_args()
     if not args.url and not args.urls_txt:
         parser.error('you must specify an url or a text file using -u/--urls-txt')
     if args.urls_txt:
-        with open(args.urls_txt, 'r', encoding = 'utf8') as f:
+        with open(args.urls_txt, 'r', encoding='utf8') as f:
             args.url = f.read().splitlines()
     dl = Gamdl(
         args.wvd_location,
         args.cookies_location,
         args.disable_music_video_skip,
         args.prefer_hevc,
-        args.heaac,
         args.temp_path,
         args.final_path,
-        args.no_lrc,
+        args.lrc_only,
         args.overwrite,
         args.skip_cleanup,
     )
     error_count = 0
     download_queue = []
     for i, url in enumerate(args.url):
         try:
@@ -137,50 +130,55 @@
     for i, url in enumerate(download_queue):
         for j, track in enumerate(url):
             print(f'Downloading "{track["attributes"]["name"]}" (track {j + 1}/{len(url)} from URL {i + 1}/{len(download_queue)})')
             track_id = track['id']
             try:
                 webplayback = dl.get_webplayback(track_id)
                 if track['type'] == 'music-videos':
-                    if args.print_video_m3u8_url:
-                        print(webplayback['hls-playlist-url'])
                     tags = dl.get_tags_music_video(track['attributes']['url'].split('/')[-1].split('?')[0])
                     final_location = dl.get_final_location('.m4v', tags)
-                    if dl.check_exists(final_location) and not args.overwrite:
+                    if final_location.exists() and not args.overwrite:
                         continue
                     stream_url_video, stream_url_audio = dl.get_stream_url_music_video(webplayback)
                     decryption_keys_audio = dl.get_decryption_keys_music_video(stream_url_audio, track_id)
                     encrypted_location_audio = dl.get_encrypted_location_audio(track_id)
                     dl.download(encrypted_location_audio, stream_url_audio)
                     decrypted_location_audio = dl.get_decrypted_location_audio(track_id)
                     dl.decrypt(encrypted_location_audio, decrypted_location_audio, decryption_keys_audio)
                     decryption_keys_video = dl.get_decryption_keys_music_video(stream_url_video, track_id)
                     encrypted_location_video = dl.get_encrypted_location_video(track_id)
                     dl.download(encrypted_location_video, stream_url_video)
                     decrypted_location_video = dl.get_decrypted_location_video(track_id)
                     dl.decrypt(encrypted_location_video, decrypted_location_video, decryption_keys_video)
                     fixed_location = dl.get_fixed_location(track_id, '.m4v')
                     dl.fixup_music_video(decrypted_location_audio, decrypted_location_video, fixed_location)
-                    dl.make_final(final_location, fixed_location, tags)
+                    final_location.parent.mkdir(parents=True, exist_ok=True)
+                    dl.move_final(final_location, fixed_location, tags)
                 else:
                     unsynced_lyrics, synced_lyrics = dl.get_lyrics(track_id)
                     tags = dl.get_tags_song(webplayback, unsynced_lyrics)
                     final_location = dl.get_final_location('.m4a', tags)
-                    if dl.check_exists(final_location) and not args.overwrite:
+                    if args.lrc_only:
+                        final_location.parent.mkdir(parents=True, exist_ok=True)
+                        dl.make_lrc(final_location, synced_lyrics)
+                        continue
+                    if final_location.exists() and not args.overwrite:
                         continue
                     stream_url = dl.get_stream_url_song(webplayback)
                     decryption_keys = dl.get_decryption_keys_song(stream_url, track_id)
                     encrypted_location = dl.get_encrypted_location_audio(track_id)
                     dl.download(encrypted_location, stream_url)
                     decrypted_location = dl.get_decrypted_location_audio(track_id)
                     dl.decrypt(encrypted_location, decrypted_location, decryption_keys)
                     fixed_location = dl.get_fixed_location(track_id, '.m4a')
                     dl.fixup_song(decrypted_location, fixed_location)
-                    dl.make_final(final_location, fixed_location, tags)
-                    dl.make_lrc(final_location, synced_lyrics)
+                    final_location.parent.mkdir(parents=True, exist_ok=True)
+                    dl.move_final(final_location, fixed_location, tags)
+                    if not args.no_lrc:
+                        dl.make_lrc(final_location, synced_lyrics)
             except KeyboardInterrupt:
                 exit(1)
             except:
                 error_count += 1
                 print(f'Failed to download "{track["attributes"]["name"]}" (track {j + 1}/{len(url)} from URL {i + 1}/{len(download_queue)})')
                 if args.print_exceptions:
                     traceback.print_exc()
```

### Comparing `gamdl-1.9/gamdl/gamdl.py` & `gamdl-1.9.1/gamdl/gamdl.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,34 +13,29 @@
 import requests
 import m3u8
 from yt_dlp import YoutubeDL
 from mutagen.mp4 import MP4, MP4Cover
 
 
 class Gamdl:
-    def __init__(self, wvd_location, cookies_location, disable_music_video_skip, prefer_hevc, heaac, temp_path, final_path, no_lrc, overwrite, skip_cleanup):
+    def __init__(self, wvd_location, cookies_location, disable_music_video_skip, prefer_hevc, temp_path, final_path, lrc_only, overwrite, skip_cleanup):
         self.disable_music_video_skip = disable_music_video_skip
         self.prefer_hevc = prefer_hevc
-        if heaac:
-            self.song_audio_quality = '32:ctrp64'
-            self.music_video_audio_quality = 'audio-HE-stereo-64'
-        else:
-            self.song_audio_quality = '28:ctrp256'
-            self.music_video_audio_quality = 'audio-stereo-256'
         self.temp_path = Path(temp_path)
         self.final_path = Path(final_path)
-        self.no_lrc = no_lrc
         self.overwrite = overwrite
         self.skip_cleanup = skip_cleanup
-        wvd_location = glob.glob(wvd_location)
-        if not wvd_location:
-            raise Exception('.wvd file not found')
-        self.cdm = Cdm.from_device(Device.load(Path(wvd_location[0])))
-        self.cdm_session = self.cdm.open()
-        cookies = MozillaCookieJar(Path(cookies_location))
+        self.lrc_only = lrc_only
+        if not self.lrc_only:
+            wvd_location = glob.glob(wvd_location)
+            if not wvd_location:
+                raise Exception('.wvd file not found')
+            self.cdm = Cdm.from_device(Device.load(wvd_location[0]))
+            self.cdm_session = self.cdm.open()
+        cookies = MozillaCookieJar(cookies_location)
         cookies.load(ignore_discard=True, ignore_expires=True)
         self.session = requests.Session()
         self.session.cookies.update(cookies)
         self.session.headers.update({
             'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:95.0) Gecko/20100101 Firefox/95.0',
             'Accept': 'application/json',
             'Accept-Language': 'en-US,en;q=0.5',
@@ -64,20 +59,22 @@
         self.storefront = getattr(gamdl.storefront_ids, self.country.upper())
     
 
     def get_download_queue(self, url):
         download_queue = []
         product_id = url.split('/')[-1].split('i=')[-1].split('&')[0].split('?')[0]
         response = self.session.get(f'https://amp-api.music.apple.com/v1/catalog/{self.country}/?ids[songs]={product_id}&ids[albums]={product_id}&ids[playlists]={product_id}&ids[music-videos]={product_id}').json()['data'][0]
-        if response['type'] in ('songs', 'music-videos') and 'playParams' in response['attributes']:
+        if response['type'] == 'songs' and 'playParams' in response['attributes']:
+            download_queue.append(response)
+        if response['type'] == 'music-videos' and 'playParams' in response['attributes'] and not self.lrc_only:
             download_queue.append(response)
         if response['type'] == 'albums' or response['type'] == 'playlists':
             for track in response['relationships']['tracks']['data']:
                 if 'playParams' in track['attributes']:
-                    if track['type'] == 'music-videos' and self.disable_music_video_skip:
+                    if track['type'] == 'music-videos' and self.disable_music_video_skip and not self.lrc_only:
                         download_queue.append(track)
                     if track['type'] == 'songs':
                         download_queue.append(track)
         if not download_queue:
             raise Exception('Criteria not met')
         return download_queue
 
@@ -90,36 +87,32 @@
                 'language': 'en-US',
             }
         ).json()["songList"][0]
         return response
     
 
     def get_stream_url_song(self, webplayback):
-        return next(i for i in webplayback["assets"] if i["flavor"] == self.song_audio_quality)['URL']
+        return next(i for i in webplayback["assets"] if i["flavor"] == '28:ctrp256')['URL']
     
 
     def get_stream_url_music_video(self, webplayback):
         with YoutubeDL({
             'allow_unplayable_formats': True,
             'quiet': True,
             'no_warnings': True,
         }) as ydl:
-            playlist = ydl.extract_info(webplayback['hls-playlist-url'], download = False)
+            playlist = ydl.extract_info(webplayback['hls-playlist-url'], download=False)
         if self.prefer_hevc:
             stream_url_video = playlist['formats'][-1]['url']
         else:
             stream_url_video = [i['url'] for i in playlist['formats'] if i['vcodec'] is not None and 'avc1' in i['vcodec']][-1]
-        stream_url_audio = next(i['url'] for i in playlist['formats'] if self.music_video_audio_quality in i['format_id'])
+        stream_url_audio = next(i['url'] for i in playlist['formats'] if 'audio-stereo-256' in i['format_id'])
         return stream_url_video, stream_url_audio
     
 
-    def check_exists(self, final_location):
-        return Path(final_location).exists()
-    
-
     def get_encrypted_location_video(self, track_id):
         return self.temp_path / f'{track_id}_encrypted_video.mp4'
     
 
     def get_encrypted_location_audio(self, track_id):
         return self.temp_path / f'{track_id}_encrypted_audio.mp4'
     
@@ -163,27 +156,27 @@
         ).json()['license']
 
 
     def get_decryption_keys_music_video(self, stream_url, track_id):
         playlist = m3u8.load(stream_url)
         track_uri = next(i for i in playlist.keys if i.keyformat == "urn:uuid:edef8ba9-79d6-4ace-a3c8-27dcd51d21ed").uri
         pssh = PSSH(track_uri.split(',')[1])
-        challenge = base64.b64encode(self.cdm.get_license_challenge(self.cdm_session, pssh)).decode('utf-8')
+        challenge = base64.b64encode(self.cdm.get_license_challenge(self.cdm_session, pssh)).decode()
         license_b64 = self.get_license_b64(challenge, track_uri, track_id)
         self.cdm.parse_license(self.cdm_session, license_b64)
         return f'1:{next(i for i in self.cdm.get_keys(self.cdm_session) if i.type == "CONTENT").key.hex()}'
 
     
     def get_decryption_keys_song(self, stream_url, track_id):
         track_uri = m3u8.load(stream_url).keys[0].uri
         widevine_pssh_data = WidevinePsshData()
         widevine_pssh_data.algorithm = 1
         widevine_pssh_data.key_ids.append(base64.b64decode(track_uri.split(",")[1]))
-        pssh = PSSH(base64.b64encode(widevine_pssh_data.SerializeToString()).decode('utf-8'))
-        challenge = base64.b64encode(self.cdm.get_license_challenge(self.cdm_session, pssh)).decode('utf-8')
+        pssh = PSSH(base64.b64encode(widevine_pssh_data.SerializeToString()).decode())
+        challenge = base64.b64encode(self.cdm.get_license_challenge(self.cdm_session, pssh)).decode()
         license_b64 = self.get_license_b64(challenge, track_uri, track_id)
         self.cdm.parse_license(self.cdm_session, license_b64)
         return f'1:{next(i for i in self.cdm.get_keys(self.cdm_session) if i.type == "CONTENT").key.hex()}'
 
 
     def decrypt(self, encrypted_location, decrypted_location, decryption_keys):
         subprocess.run(
@@ -234,16 +227,16 @@
 
     @functools.lru_cache()
     def get_cover(self, url):
         return requests.get(url).content
     
 
     def get_tags_song(self, webplayback, unsynced_lyrics):
-        metadata = next(i for i in webplayback["assets"] if i["flavor"] == self.song_audio_quality)['metadata']
-        cover_url = next(i for i in webplayback["assets"] if i["flavor"] == self.song_audio_quality)['artworkURL']
+        metadata = next(i for i in webplayback["assets"] if i["flavor"] == '28:ctrp256')['metadata']
+        cover_url = next(i for i in webplayback["assets"] if i["flavor"] == '28:ctrp256')['artworkURL'].replace('600x600bb', '1200x1200bb')
         tags = {
             '\xa9nam': [metadata['itemName']],
             '\xa9gen': [metadata['genre']],
             'aART': [metadata['playlistArtistName']],
             '\xa9alb': [metadata['playlistName']],
             'soar': [metadata['sort-artist']],
             'soal': [metadata['sort-album']],
@@ -255,15 +248,15 @@
             'cnID': [int(metadata['itemId'])],
             'sfID': [metadata['s']],
             'rtng': [metadata['explicit']],
             'pgap': metadata['gapless'],
             'cpil': metadata['compilation'],
             'disk': [(metadata['discNumber'], metadata['discCount'])],
             'trkn': [(metadata['trackNumber'], metadata['trackCount'])],
-            'covr': [MP4Cover(self.get_cover(cover_url), MP4Cover.FORMAT_JPEG)],
+            'covr': [MP4Cover(self.get_cover(cover_url))],
             'stik': [1],
         }
         if 'copyright' in metadata:
             tags['cprt'] = [metadata['copyright']]
         if 'releaseDate' in metadata:
             tags['\xa9day'] = [metadata['releaseDate']]
         if 'comments' in metadata:
@@ -288,15 +281,15 @@
             '\xa9day': [metadata[0]["releaseDate"]],
             '\xa9gen': [metadata[0]['primaryGenreName']],
             'stik': [6],
             'atID': [metadata[0]['artistId']],
             'cnID': [metadata[0]["trackId"]],
             'geID': [int(extra_metadata['genres'][0]['genreId'])],
             'sfID': [int(self.storefront.split('-')[0])],
-            'covr': [MP4Cover(self.get_cover(metadata[0]["artworkUrl30"].replace('30x30bb.jpg', '600x600bb.jpg')), MP4Cover.FORMAT_JPEG)],
+            'covr': [MP4Cover(self.get_cover(metadata[0]["artworkUrl30"].replace('30x30bb.jpg', '1280x720bb.jpg')))],
         }
         if 'copyright' in extra_metadata:
             tags['cprt'] = [extra_metadata['copyright']]
         if metadata[0]['trackExplicitness'] == 'notExplicit':
             tags['rtng'] = [0]
         elif metadata[0]['trackExplicitness'] == 'explicit':
             tags['rtng'] = [1]
@@ -308,19 +301,18 @@
             tags['plID'] = [metadata[1]["collectionId"]]
             tags['disk'] = [(metadata[0]["discNumber"], metadata[0]["discCount"])]
             tags['trkn'] = [(metadata[0]["trackNumber"], metadata[0]["trackCount"])]
         return tags
 
 
     def get_sanizated_string(self, dirty_string, is_folder):
-        for character in ['\\', '/', ':', '*', '?', '"', '<', '>', '|', ';']:
-            dirty_string = dirty_string.replace(character, '_')
+        dirty_string = re.sub(r'[\\/:\*\?"<>\|;]', '_', dirty_string)
         if is_folder:
             dirty_string = dirty_string[:40]
-            if dirty_string[-1:] == '.':
+            if dirty_string.endswith('.') == '.':
                 dirty_string = dirty_string[:-1] + '_'
         else:
             dirty_string = dirty_string[:36]
         return dirty_string.strip()
     
 
     def get_final_location_overwrite_prevented_music_video(self, final_location):
@@ -386,22 +378,21 @@
                 fixed_location,
             ],
             check=True
         )
     
 
     def make_lrc(self, final_location, synced_lyrics):
-        if synced_lyrics and not self.no_lrc:
-            with open(final_location.with_suffix('.lrc'), 'w', encoding = 'utf8') as f:
+        if synced_lyrics:
+            with open(final_location.with_suffix('.lrc'), 'w', encoding='utf8') as f:
                 f.write(synced_lyrics)
     
 
-    def make_final(self, final_location, fixed_location, tags):
-        final_location.parent.mkdir(parents = True, exist_ok = True)
-        shutil.copy(fixed_location, final_location)
+    def move_final(self, final_location, fixed_location, tags):
+        shutil.move(fixed_location, final_location)
         file = MP4(final_location)
         file.update(tags)
         file.save()
     
 
     def cleanup(self):
         if self.temp_path.exists() and not self.skip_cleanup:
```

### Comparing `gamdl-1.9/gamdl/storefront_ids.py` & `gamdl-1.9.1/gamdl/storefront_ids.py`

 * *Files identical despite different names*

### Comparing `gamdl-1.9/PKG-INFO` & `gamdl-1.9.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gamdl
-Version: 1.9
+Version: 1.9.1
 Summary: Download Apple Music songs/music videos/albums/playlists
 Author: glomatico
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: pywidevine
 Requires-Dist: pyyaml
 Requires-Dist: m3u8
@@ -52,57 +52,61 @@
             pywidevine create-device -t ANDROID -l 3 -k private_key.pem -c client_id.bin -o .
             ```
 6. (optional) Add aria2c to your PATH for faster downloads
     * You can get it from here: https://github.com/aria2/aria2/releases.
 
 ## Usage
 ```
-usage: gamdl [-h] [-u [URLS_TXT]] [-w WVD_LOCATION] [-f FINAL_PATH] [-t TEMP_PATH] [-c COOKIES_LOCATION] [-m]
-                   [-p] [-a] [-o] [-n] [-s] [-e] [-i] [-v]
+usage: __main__.py [-h] [-u [URLS_TXT]] [-w WVD_LOCATION] [-f FINAL_PATH]
+                   [-t TEMP_PATH] [-c COOKIES_LOCATION] [-m] [-p] [-o] [-n]
+                   [-l] [-s] [-e] [-v]
                    [url ...]
 
 Download Apple Music songs/music videos/albums/playlists
 
 positional arguments:
-  url                   Apple Music song/music video/album/playlist URL(s) (default: None)
+  url                   Apple Music song/music video/album/playlist URL(s)
+                        (default: None)
 
 options:
   -h, --help            show this help message and exit
   -u [URLS_TXT], --urls-txt [URLS_TXT]
                         Read URLs from a text file (default: None)
   -w WVD_LOCATION, --wvd-location WVD_LOCATION
-                        .wvd file location (default: *.wvd)
+                        .wvd file location (ignored if using -l/--lrc-only)
+                        (default: ./*.wvd)
   -f FINAL_PATH, --final-path FINAL_PATH
-                        Final Path (default: Apple Music)
+                        Final Path (default: ./Apple Music)
   -t TEMP_PATH, --temp-path TEMP_PATH
-                        Temp Path (default: temp)
+                        Temp Path (default: ./temp)
   -c COOKIES_LOCATION, --cookies-location COOKIES_LOCATION
-                        Cookies location (default: cookies.txt)
+                        Cookies location (default: ./cookies.txt)
   -m, --disable-music-video-skip
-                        Disable music video skip on playlists/albums (default: False)
+                        Disable music video skip on playlists/albums (default:
+                        False)
   -p, --prefer-hevc     Prefer HEVC over AVC (default: False)
-  -a, --heaac           Download songs/music videos with HE-AAC instead of AAC (default: False)
   -o, --overwrite       Overwrite existing files (default: False)
-  -n, --no-lrc          Don't create .lrc file (default: False)
+  -n, --no-lrc          Don't create .lrc file (ignored if using -l/--lrc-
+                        only) (default: False)
+  -l, --lrc-only        Skip downloading songs and only create .lrc files
+                        (default: False)
   -s, --skip-cleanup    Skip cleanup (default: False)
   -e, --print-exceptions
                         Print execeptions (default: False)
-  -i, --print-video-m3u8-url
-                        Print Video M3U8 URL (default: False)
   -v, --version         show program's version number and exit
 ```
 
 ## Songs/Music Videos quality
 * Songs:
-    * 256kbps AAC / HE-AAC 64kbps
+    * AAC 256kbps
 * Music Videos (varies depending on the video):
-    * 4K HEVC 20mbps, AAC 256kbps / HE-AAC 64kbps
-    * 4K HEVC 12mbps, AAC 256kbps / HE-AAC 64kbps
-    * 1080p AVC 10mbps, AAC 256kbps / HE-AAC 64kbps
-    * 1080p AVC 6.5bps, AAC 256kbps / HE-AAC 64kbps
-    * 720p AVC 4mbps, AAC 256kbps / HE-AAC 64kbps
-    * 576p AVC 2mbps, AAC 256kbps / HE-AAC 64kbps
-    * 480p AVC 1.5mbps, AAC 256kbps / HE-AAC 64kbps
-    * 360p AVC 1mbps, AAC 256kbps / HE-AAC 64kbps
+    * 4K HEVC 20mbps, AAC 256kbps
+    * 4K HEVC 12mbps, AAC 256kbps
+    * 1080p AVC 10mbps, AAC 256kbps
+    * 1080p AVC 6.5bps, AAC 256kbps
+    * 720p AVC 4mbps, AAC 256kbps
+    * 576p AVC 2mbps, AAC 256kbps
+    * 480p AVC 1.5mbps, AAC 256kbps
+    * 360p AVC 1mbps, AAC 256kbps
 
 Some videos may include EIA-608 closed captions.
```

