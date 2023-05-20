# Comparing `tmp/flanaapis-1.6.1.tar.gz` & `tmp/flanaapis-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flanaapis-1.6.1.tar", last modified: Sat May  6 18:44:24 2023, max compression
+gzip compressed data, was "flanaapis-1.6.2.tar", last modified: Sat May 20 04:38:04 2023, max compression
```

## Comparing `flanaapis-1.6.1.tar` & `flanaapis-1.6.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:44:24.158690 flanaapis-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-06 18:44:08.000000 flanaapis-1.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-05-06 18:44:24.158690 flanaapis-1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-05-06 18:44:08.000000 flanaapis-1.6.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:44:24.158690 flanaapis-1.6.1/flanaapis/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-06 18:44:08.000000 flanaapis-1.6.1/flanaapis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-06 18:44:08.000000 flanaapis-1.6.1/flanaapis/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:44:24.158690 flanaapis-1.6.1/flanaapis/geolocation/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-06 18:44:08.000000 flanaapis-1.6.1/flanaapis/geolocation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-05-06 18:44:08.000000 flanaapis-1.6.1/flanaapis/geolocation/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-05-06 18:44:08.000000 flanaapis-1.6.1/flanaapis/geolocation/google_maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-06 18:44:08.000000 flanaapis-1.6.1/flanaapis/geolocation/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-05-06 18:44:08.000000 flanaapis-1.6.1/flanaapis/geolocation/open_street_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-06 18:44:08.000000 flanaapis-1.6.1/flanaapis/geolocation/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-06 18:44:08.000000 flanaapis-1.6.1/flanaapis/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:44:24.158690 flanaapis-1.6.1/flanaapis/scraping/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-06 18:44:08.000000 flanaapis-1.6.1/flanaapis/scraping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-06 18:44:08.000000 flanaapis-1.6.1/flanaapis/scraping/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-06 18:44:08.000000 flanaapis-1.6.1/flanaapis/scraping/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11856 2023-05-06 18:44:08.000000 flanaapis-1.6.1/flanaapis/scraping/google_weather_scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-05-06 18:44:08.000000 flanaapis-1.6.1/flanaapis/scraping/instagram.py
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-05-06 18:44:08.000000 flanaapis-1.6.1/flanaapis/scraping/reddit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-06 18:44:08.000000 flanaapis-1.6.1/flanaapis/scraping/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-05-06 18:44:08.000000 flanaapis-1.6.1/flanaapis/scraping/tiktok.py
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-05-06 18:44:08.000000 flanaapis-1.6.1/flanaapis/scraping/twitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-05-06 18:44:08.000000 flanaapis-1.6.1/flanaapis/scraping/yt_dlp_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:44:24.158690 flanaapis-1.6.1/flanaapis/weather/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-06 18:44:08.000000 flanaapis-1.6.1/flanaapis/weather/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-06 18:44:08.000000 flanaapis-1.6.1/flanaapis/weather/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-05-06 18:44:08.000000 flanaapis-1.6.1/flanaapis/weather/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-05-06 18:44:08.000000 flanaapis-1.6.1/flanaapis/weather/google.py
--rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-05-06 18:44:08.000000 flanaapis-1.6.1/flanaapis/weather/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     9427 2023-05-06 18:44:08.000000 flanaapis-1.6.1/flanaapis/weather/open_weather_map.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-06 18:44:08.000000 flanaapis-1.6.1/flanaapis/weather/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-05-06 18:44:08.000000 flanaapis-1.6.1/flanaapis/weather/visual_crossing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:44:24.158690 flanaapis-1.6.1/flanaapis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-05-06 18:44:24.000000 flanaapis-1.6.1/flanaapis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-06 18:44:24.000000 flanaapis-1.6.1/flanaapis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 18:44:24.000000 flanaapis-1.6.1/flanaapis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-06 18:44:24.000000 flanaapis-1.6.1/flanaapis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-06 18:44:24.000000 flanaapis-1.6.1/flanaapis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-06 18:44:08.000000 flanaapis-1.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-06 18:44:24.162690 flanaapis-1.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 04:38:04.877261 flanaapis-1.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-20 04:37:50.000000 flanaapis-1.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-05-20 04:38:04.877261 flanaapis-1.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-05-20 04:37:50.000000 flanaapis-1.6.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 04:38:04.873261 flanaapis-1.6.2/flanaapis/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-20 04:37:50.000000 flanaapis-1.6.2/flanaapis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-20 04:37:50.000000 flanaapis-1.6.2/flanaapis/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 04:38:04.873261 flanaapis-1.6.2/flanaapis/geolocation/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-20 04:37:50.000000 flanaapis-1.6.2/flanaapis/geolocation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-05-20 04:37:50.000000 flanaapis-1.6.2/flanaapis/geolocation/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-05-20 04:37:50.000000 flanaapis-1.6.2/flanaapis/geolocation/google_maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-20 04:37:50.000000 flanaapis-1.6.2/flanaapis/geolocation/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-05-20 04:37:50.000000 flanaapis-1.6.2/flanaapis/geolocation/open_street_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-20 04:37:50.000000 flanaapis-1.6.2/flanaapis/geolocation/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-20 04:37:50.000000 flanaapis-1.6.2/flanaapis/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 04:38:04.877261 flanaapis-1.6.2/flanaapis/scraping/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-20 04:37:50.000000 flanaapis-1.6.2/flanaapis/scraping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-20 04:37:50.000000 flanaapis-1.6.2/flanaapis/scraping/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-20 04:37:50.000000 flanaapis-1.6.2/flanaapis/scraping/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11856 2023-05-20 04:37:50.000000 flanaapis-1.6.2/flanaapis/scraping/google_weather_scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6759 2023-05-20 04:37:50.000000 flanaapis-1.6.2/flanaapis/scraping/instagram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-05-20 04:37:50.000000 flanaapis-1.6.2/flanaapis/scraping/reddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-20 04:37:50.000000 flanaapis-1.6.2/flanaapis/scraping/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-05-20 04:37:50.000000 flanaapis-1.6.2/flanaapis/scraping/tiktok.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-05-20 04:37:50.000000 flanaapis-1.6.2/flanaapis/scraping/twitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5192 2023-05-20 04:37:50.000000 flanaapis-1.6.2/flanaapis/scraping/yt_dlp_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 04:38:04.877261 flanaapis-1.6.2/flanaapis/weather/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-20 04:37:50.000000 flanaapis-1.6.2/flanaapis/weather/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-20 04:37:50.000000 flanaapis-1.6.2/flanaapis/weather/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-05-20 04:37:50.000000 flanaapis-1.6.2/flanaapis/weather/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-05-20 04:37:50.000000 flanaapis-1.6.2/flanaapis/weather/google.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-05-20 04:37:50.000000 flanaapis-1.6.2/flanaapis/weather/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9427 2023-05-20 04:37:50.000000 flanaapis-1.6.2/flanaapis/weather/open_weather_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-20 04:37:50.000000 flanaapis-1.6.2/flanaapis/weather/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-05-20 04:37:50.000000 flanaapis-1.6.2/flanaapis/weather/visual_crossing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 04:38:04.873261 flanaapis-1.6.2/flanaapis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-05-20 04:38:04.000000 flanaapis-1.6.2/flanaapis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-20 04:38:04.000000 flanaapis-1.6.2/flanaapis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 04:38:04.000000 flanaapis-1.6.2/flanaapis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-20 04:38:04.000000 flanaapis-1.6.2/flanaapis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-20 04:38:04.000000 flanaapis-1.6.2/flanaapis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-20 04:37:50.000000 flanaapis-1.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-20 04:38:04.877261 flanaapis-1.6.2/setup.cfg
```

### Comparing `flanaapis-1.6.1/LICENSE` & `flanaapis-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flanaapis-1.6.1/PKG-INFO` & `flanaapis-1.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flanaapis
-Version: 1.6.1
+Version: 1.6.2
 Summary: Set of functions that can be used as an imported library or as an api rest running the main.py. There is currently an instance of the api running at https://flanaserver.ddns.net/flanaapis.
 Home-page: https://github.com/AlberLC/flanaapis
 Author: AlberLC
 Project-URL: Bug Tracker, https://github.com/AlberLC/flanaapis/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `flanaapis-1.6.1/README.rst` & `flanaapis-1.6.2/README.rst`

 * *Files identical despite different names*

### Comparing `flanaapis-1.6.1/flanaapis/exceptions.py` & `flanaapis-1.6.2/flanaapis/exceptions.py`

 * *Files identical despite different names*

### Comparing `flanaapis-1.6.1/flanaapis/geolocation/functions.py` & `flanaapis-1.6.2/flanaapis/geolocation/functions.py`

 * *Files identical despite different names*

### Comparing `flanaapis-1.6.1/flanaapis/geolocation/google_maps.py` & `flanaapis-1.6.2/flanaapis/geolocation/google_maps.py`

 * *Files identical despite different names*

### Comparing `flanaapis-1.6.1/flanaapis/geolocation/models.py` & `flanaapis-1.6.2/flanaapis/geolocation/models.py`

 * *Files identical despite different names*

### Comparing `flanaapis-1.6.1/flanaapis/geolocation/open_street_map.py` & `flanaapis-1.6.2/flanaapis/geolocation/open_street_map.py`

 * *Files identical despite different names*

### Comparing `flanaapis-1.6.1/flanaapis/geolocation/routes.py` & `flanaapis-1.6.2/flanaapis/geolocation/routes.py`

 * *Files identical despite different names*

### Comparing `flanaapis-1.6.1/flanaapis/main.py` & `flanaapis-1.6.2/flanaapis/main.py`

 * *Files identical despite different names*

### Comparing `flanaapis-1.6.1/flanaapis/scraping/constants.py` & `flanaapis-1.6.2/flanaapis/scraping/constants.py`

 * *Files identical despite different names*

### Comparing `flanaapis-1.6.1/flanaapis/scraping/functions.py` & `flanaapis-1.6.2/flanaapis/scraping/functions.py`

 * *Files identical despite different names*

### Comparing `flanaapis-1.6.1/flanaapis/scraping/google_weather_scraper.py` & `flanaapis-1.6.2/flanaapis/scraping/google_weather_scraper.py`

 * *Files identical despite different names*

### Comparing `flanaapis-1.6.1/flanaapis/scraping/instagram.py` & `flanaapis-1.6.2/flanaapis/scraping/instagram.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,19 +20,19 @@
     sid = None
     last_url = ''
     selected_urls = {}
     thumbnail_urls = set()
 
     for media_url in media_urls:
         if (
-                not re.findall('(?:-15/.*=dst-jpg_e\d{2}|mp4).*sid=\w+$', media_url)
-                or
-                sid
-                and
-                sid != get_media_url_sid(media_url)
+            not re.findall('(?:-15/.*=dst-jpg_e\d{2}|mp4).*sid=\w+$', media_url)
+            or
+            sid
+            and
+            sid != get_media_url_sid(media_url)
         ):
             last_url = ''
             continue
 
         if not sid:
             sid = get_media_url_sid(media_url)
 
@@ -61,17 +61,17 @@
     last_url = ''
     last_video_url = ''
     last_video_id = ''
     final_urls = OrderedSet()
     thumbnail_urls = OrderedSet()
     for media_url in media_urls:
         if (
-                not re.findall('-15/.*=dst-jpg', media_url)
-                and
-                'mp4' not in media_url
+            not re.findall('-15/.*=dst-jpg', media_url)
+            and
+            'mp4' not in media_url
         ):
             last_url = ''
             continue
 
         if 'jpg' in media_url:
             if 'mp4' in last_url:
                 thumbnail_urls.add(media_url)
@@ -129,20 +129,28 @@
             )
             context.set_default_timeout(5000)
 
             page = await context.new_page()
             await page.goto(url, timeout=30000)
 
             try:
-                await page.click("'Permitir solo cookies necesarias'")
+                await page.locator("button:text('cookies')").nth(1).click()
             except playwright.async_api.Error:
                 pass
             await page.wait_for_load_state('networkidle')
 
             try:
+                await page.wait_for_selector("'Vídeo restringido'")
+            except playwright.async_api.Error:
+                if page.locator("'mayor de 18 para ver'").count():
+                    raise InstagramMediaNotFoundError('age restricted')
+            else:
+                raise InstagramMediaNotFoundError('age restricted')
+
+            try:
                 button = await page.wait_for_selector("button[aria-label='Siguiente']")
                 while True:
                     await button.click()
                     await asyncio.sleep(0.2)
             except playwright.async_api.Error:
                 pass
 
@@ -163,15 +171,19 @@
 async def get_medias(ids: Iterable[str], audio_only=False) -> OrderedSet[Media]:
     medias: OrderedSet[Media] = OrderedSet()
 
     if not (urls := make_urls(OrderedSet(ids))):
         return medias
 
     for url in urls:
-        medias |= filter_media_urls(find_media_urls(await get_html(url)))
+        try:
+            medias |= filter_media_urls(find_media_urls(await get_html(url)))
+        except InstagramMediaNotFoundError as e:
+            if 'age restricted' in str(e):
+                medias.add(Media(find_ids(url)[0], MediaType.ERROR, source=Source.INSTAGRAM))
 
     if not medias:
         raise InstagramMediaNotFoundError
 
     if audio_only:
         medias = await functions.filter_audios(medias)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `flanaapis-1.6.1/flanaapis/scraping/reddit.py` & `flanaapis-1.6.2/flanaapis/scraping/reddit.py`

 * *Files identical despite different names*

### Comparing `flanaapis-1.6.1/flanaapis/scraping/routes.py` & `flanaapis-1.6.2/flanaapis/scraping/routes.py`

 * *Files identical despite different names*

### Comparing `flanaapis-1.6.1/flanaapis/scraping/tiktok.py` & `flanaapis-1.6.2/flanaapis/scraping/tiktok.py`

 * *Files identical despite different names*

### Comparing `flanaapis-1.6.1/flanaapis/scraping/twitter.py` & `flanaapis-1.6.2/flanaapis/scraping/twitter.py`

 * *Files identical despite different names*

### Comparing `flanaapis-1.6.1/flanaapis/scraping/yt_dlp_wrapper.py` & `flanaapis-1.6.2/flanaapis/scraping/yt_dlp_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,42 +73,45 @@
         output_file_path = next(flanautils.find_paths_by_stem(output_file_stem, lazy=True))
     except StopIteration:
         return
 
     bytes_ = output_file_path.read_bytes()
 
     if (
-            not (extension := output_file_path.suffix.strip('.'))
-            and
-            not (extension := media_info.get('final_extension'))
-            and
-            (output_file_name := media_info.get('output_file_name'))
+        not (extension := output_file_path.suffix.strip('.'))
+        and
+        not (extension := media_info.get('final_extension'))
+        and
+        (output_file_name := media_info.get('output_file_name'))
     ):
         extension = pathlib.Path(output_file_name).suffix.strip('.')
 
     extractor_key = media_info.get('extractor_key', '')
+    image_formats = ('jfif', 'jpeg', 'jpg', 'png', 'tiff')
+    video_formats = ('avchd', 'avi', 'flv', 'mkv', 'mov', 'mp4', 'webm', 'wmv')
+    audio_formats = ('aac', 'flac', 'm4a', 'mp3', 'wav')
     if 'generic' == extractor_key.lower():
         bytes_format = await flanautils.get_format(bytes_)
-        if any(format_ in bytes_format for format_ in ('jfif', 'jpeg', 'jpg', 'png', 'tiff')):
+        if any(format_ in bytes_format for format_ in image_formats):
             type_ = MediaType.IMAGE
         elif 'gif' in bytes_format:
             type_ = MediaType.GIF
-        elif any(format_ in bytes_format for format_ in ('avchd', 'avi', 'flv', 'mkv', 'mov', 'mp4', 'webm', 'wmv')):
+        elif any(format_ in bytes_format for format_ in video_formats):
             type_ = MediaType.VIDEO
-        elif any(format_ in bytes_format for format_ in ('aac', 'flac', 'm4a', 'mp3', 'wav')):
+        elif any(format_ in bytes_format for format_ in audio_formats):
             type_ = MediaType.AUDIO
         else:
             type_ = None
 
         if domains := flanautils.find_url_domains(url):
             source = domains[0]
         else:
             source = None
     else:
-        if audio_only:
+        if audio_only or extension in audio_formats:
             type_ = MediaType.AUDIO
         elif extension == 'gif':
             type_ = MediaType.GIF
         else:
             type_ = MediaType.VIDEO
 
         try:
```

### Comparing `flanaapis-1.6.1/flanaapis/weather/functions.py` & `flanaapis-1.6.2/flanaapis/weather/functions.py`

 * *Files identical despite different names*

### Comparing `flanaapis-1.6.1/flanaapis/weather/google.py` & `flanaapis-1.6.2/flanaapis/weather/google.py`

 * *Files identical despite different names*

### Comparing `flanaapis-1.6.1/flanaapis/weather/models.py` & `flanaapis-1.6.2/flanaapis/weather/models.py`

 * *Files identical despite different names*

### Comparing `flanaapis-1.6.1/flanaapis/weather/open_weather_map.py` & `flanaapis-1.6.2/flanaapis/weather/open_weather_map.py`

 * *Files identical despite different names*

### Comparing `flanaapis-1.6.1/flanaapis/weather/routes.py` & `flanaapis-1.6.2/flanaapis/weather/routes.py`

 * *Files identical despite different names*

### Comparing `flanaapis-1.6.1/flanaapis/weather/visual_crossing.py` & `flanaapis-1.6.2/flanaapis/weather/visual_crossing.py`

 * *Files identical despite different names*

### Comparing `flanaapis-1.6.1/flanaapis.egg-info/PKG-INFO` & `flanaapis-1.6.2/flanaapis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flanaapis
-Version: 1.6.1
+Version: 1.6.2
 Summary: Set of functions that can be used as an imported library or as an api rest running the main.py. There is currently an instance of the api running at https://flanaserver.ddns.net/flanaapis.
 Home-page: https://github.com/AlberLC/flanaapis
 Author: AlberLC
 Project-URL: Bug Tracker, https://github.com/AlberLC/flanaapis/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `flanaapis-1.6.1/flanaapis.egg-info/SOURCES.txt` & `flanaapis-1.6.2/flanaapis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flanaapis-1.6.1/setup.cfg` & `flanaapis-1.6.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = flanaapis
-version = v1.6.1
+version = v1.6.2
 author = AlberLC
 description = Set of functions that can be used as an imported library or as an api rest running the main.py. There is currently an instance of the api running at https://flanaserver.ddns.net/flanaapis.
 long_description = file: README.rst
 url = https://github.com/AlberLC/flanaapis
 project_urls = 
 	Bug Tracker = https://github.com/AlberLC/flanaapis/issues
 classifiers =
```

