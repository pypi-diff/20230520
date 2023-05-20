# Comparing `tmp/flanabot-1.5.1.tar.gz` & `tmp/flanabot-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flanabot-1.5.1.tar", last modified: Sat May  6 18:44:59 2023, max compression
+gzip compressed data, was "flanabot-1.5.2.tar", last modified: Sat May 20 04:37:27 2023, max compression
```

## Comparing `flanabot-1.5.1.tar` & `flanabot-1.5.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:44:59.363792 flanabot-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-06 18:44:42.000000 flanabot-1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-06 18:44:59.363792 flanabot-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-06 18:44:42.000000 flanabot-1.5.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:44:59.359792 flanabot-1.5.1/flanabot/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:44:59.363792 flanabot-1.5.1/flanabot/bots/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-06 18:44:42.000000 flanabot-1.5.1/flanabot/bots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22365 2023-05-06 18:44:42.000000 flanabot-1.5.1/flanabot/bots/connect_4_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)    22534 2023-05-06 18:44:42.000000 flanabot-1.5.1/flanabot/bots/flana_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-05-06 18:44:42.000000 flanabot-1.5.1/flanabot/bots/flana_disc_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-05-06 18:44:42.000000 flanabot-1.5.1/flanabot/bots/flana_tele_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8831 2023-05-06 18:44:42.000000 flanabot-1.5.1/flanabot/bots/penalty_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)    13114 2023-05-06 18:44:42.000000 flanabot-1.5.1/flanabot/bots/poll_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)    18368 2023-05-06 18:44:42.000000 flanabot-1.5.1/flanabot/bots/scraper_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-05-06 18:44:42.000000 flanabot-1.5.1/flanabot/bots/ubereats_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)    11563 2023-05-06 18:44:42.000000 flanabot-1.5.1/flanabot/bots/weather_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8956 2023-05-06 18:44:42.000000 flanabot-1.5.1/flanabot/connect_4_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-05-06 18:44:42.000000 flanabot-1.5.1/flanabot/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-06 18:44:42.000000 flanabot-1.5.1/flanabot/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:44:59.363792 flanabot-1.5.1/flanabot/models/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-06 18:44:42.000000 flanabot-1.5.1/flanabot/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-06 18:44:42.000000 flanabot-1.5.1/flanabot/models/bot_action.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-06 18:44:42.000000 flanabot-1.5.1/flanabot/models/chat.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-06 18:44:42.000000 flanabot-1.5.1/flanabot/models/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-06 18:44:42.000000 flanabot-1.5.1/flanabot/models/message.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-06 18:44:42.000000 flanabot-1.5.1/flanabot/models/player.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-06 18:44:42.000000 flanabot-1.5.1/flanabot/models/punishment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-05-06 18:44:42.000000 flanabot-1.5.1/flanabot/models/weather_chart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:44:59.363792 flanabot-1.5.1/flanabot/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    82944 2023-05-06 18:44:42.000000 flanabot-1.5.1/flanabot/resources/mucho_texto.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:44:59.359792 flanabot-1.5.1/flanabot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-06 18:44:59.000000 flanabot-1.5.1/flanabot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-06 18:44:59.000000 flanabot-1.5.1/flanabot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 18:44:59.000000 flanabot-1.5.1/flanabot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-06 18:44:59.000000 flanabot-1.5.1/flanabot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-06 18:44:59.000000 flanabot-1.5.1/flanabot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-06 18:44:42.000000 flanabot-1.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-06 18:44:59.367792 flanabot-1.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 04:37:27.521725 flanabot-1.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-20 04:37:11.000000 flanabot-1.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-20 04:37:27.521725 flanabot-1.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-20 04:37:11.000000 flanabot-1.5.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 04:37:27.513725 flanabot-1.5.2/flanabot/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 04:37:27.517725 flanabot-1.5.2/flanabot/bots/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-20 04:37:11.000000 flanabot-1.5.2/flanabot/bots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22365 2023-05-20 04:37:11.000000 flanabot-1.5.2/flanabot/bots/connect_4_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22473 2023-05-20 04:37:11.000000 flanabot-1.5.2/flanabot/bots/flana_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-05-20 04:37:11.000000 flanabot-1.5.2/flanabot/bots/flana_disc_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-05-20 04:37:11.000000 flanabot-1.5.2/flanabot/bots/flana_tele_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8831 2023-05-20 04:37:11.000000 flanabot-1.5.2/flanabot/bots/penalty_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13114 2023-05-20 04:37:11.000000 flanabot-1.5.2/flanabot/bots/poll_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18728 2023-05-20 04:37:11.000000 flanabot-1.5.2/flanabot/bots/scraper_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-05-20 04:37:11.000000 flanabot-1.5.2/flanabot/bots/ubereats_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11563 2023-05-20 04:37:11.000000 flanabot-1.5.2/flanabot/bots/weather_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8956 2023-05-20 04:37:11.000000 flanabot-1.5.2/flanabot/connect_4_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-05-20 04:37:11.000000 flanabot-1.5.2/flanabot/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-20 04:37:11.000000 flanabot-1.5.2/flanabot/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 04:37:27.517725 flanabot-1.5.2/flanabot/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-20 04:37:11.000000 flanabot-1.5.2/flanabot/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-20 04:37:11.000000 flanabot-1.5.2/flanabot/models/bot_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-20 04:37:11.000000 flanabot-1.5.2/flanabot/models/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-20 04:37:11.000000 flanabot-1.5.2/flanabot/models/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-20 04:37:11.000000 flanabot-1.5.2/flanabot/models/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-20 04:37:11.000000 flanabot-1.5.2/flanabot/models/player.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-20 04:37:11.000000 flanabot-1.5.2/flanabot/models/punishment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-05-20 04:37:11.000000 flanabot-1.5.2/flanabot/models/weather_chart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 04:37:27.517725 flanabot-1.5.2/flanabot/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    82944 2023-05-20 04:37:11.000000 flanabot-1.5.2/flanabot/resources/mucho_texto.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 04:37:27.517725 flanabot-1.5.2/flanabot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-20 04:37:27.000000 flanabot-1.5.2/flanabot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-20 04:37:27.000000 flanabot-1.5.2/flanabot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 04:37:27.000000 flanabot-1.5.2/flanabot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-20 04:37:27.000000 flanabot-1.5.2/flanabot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-20 04:37:27.000000 flanabot-1.5.2/flanabot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-20 04:37:11.000000 flanabot-1.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-20 04:37:27.521725 flanabot-1.5.2/setup.cfg
```

### Comparing `flanabot-1.5.1/LICENSE` & `flanabot-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flanabot-1.5.1/PKG-INFO` & `flanabot-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flanabot
-Version: 1.5.1
+Version: 1.5.2
 Summary: Bot based on https://github.com/AlberLC/multibot to manage Discord, Telegram and Twitch chats, moderate them and add functionalities.
 Home-page: https://github.com/AlberLC/flanabot
 Author: AlberLC
 Project-URL: Bug Tracker, https://github.com/AlberLC/flanabot/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `flanabot-1.5.1/README.rst` & `flanabot-1.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `flanabot-1.5.1/flanabot/bots/connect_4_bot.py` & `flanabot-1.5.2/flanabot/bots/connect_4_bot.py`

 * *Files identical despite different names*

### Comparing `flanabot-1.5.1/flanabot/bots/flana_bot.py` & `flanabot-1.5.2/flanabot/bots/flana_bot.py`

 * *Files 0% similar despite different names*

```diff
@@ -221,22 +221,21 @@
     async def _on_deactivate_tunnel(self, message: Message):
         self.tunnel_chat = None
         await self.send('Túnel cerrado.', message)
 
     @inline(False)
     async def _on_delete(self, message: Message):
         if message.replied_message:
-            if (
-                self.is_bot_mentioned(message)
-                and
-                (message.author.is_admin or message.replied_message.author.id == self.id)
-            ):
+            if not self.is_bot_mentioned(message):
+                return
+
+            if message.author.is_admin or message.replied_message.author.id == self.id:
                 flanautils.do_later(flanautils.text_to_time(message.text).total_seconds(), self.delete_message, message.replied_message)
                 await self.delete_message(message)
-            elif message.chat.is_group and self.is_bot_mentioned(message):
+            elif message.chat.is_group:
                 await self.send_negative(message)
         elif (
             (message.chat.is_private or self.is_bot_mentioned(message))
             and
             (n_messages := flanautils.text_to_number(message.text))
         ):
             if message.author.is_admin is False:
```

### Comparing `flanabot-1.5.1/flanabot/bots/flana_disc_bot.py` & `flanabot-1.5.2/flanabot/bots/flana_disc_bot.py`

 * *Files identical despite different names*

### Comparing `flanabot-1.5.1/flanabot/bots/flana_tele_bot.py` & `flanabot-1.5.2/flanabot/bots/flana_tele_bot.py`

 * *Files identical despite different names*

### Comparing `flanabot-1.5.1/flanabot/bots/penalty_bot.py` & `flanabot-1.5.2/flanabot/bots/penalty_bot.py`

 * *Files identical despite different names*

### Comparing `flanabot-1.5.1/flanabot/bots/poll_bot.py` & `flanabot-1.5.2/flanabot/bots/poll_bot.py`

 * *Files identical despite different names*

### Comparing `flanabot-1.5.1/flanabot/bots/scraper_bot.py` & `flanabot-1.5.2/flanabot/bots/scraper_bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,29 +221,40 @@
             twitter.get_medias(tweet_ids, audio_only),
             tiktok.get_medias(tiktok_users_and_ids, tiktok_download_urls, 'h264', 'mp4', force, audio_only, timeout_for_media),
             yt_dlp_wrapper.get_medias(media_urls, 'h264', 'mp4', force, audio_only, timeout_for_media),
             return_exceptions=True
         )
 
         instagram_results = []
+        instagram_restricted_age_ids = []
         if instagram_ids:
             can_instagram_v1 = not self.instagram_ban_date or datetime.datetime.now(datetime.timezone.utc) - self.instagram_ban_date >= constants.INSTAGRAM_BAN_SLEEP
             if can_instagram_v1:
                 try:
                     instagram_results = await instagram.get_medias(instagram_ids, audio_only)
                 except InstagramMediaNotFoundError:
                     pass
+                else:
+                    instagram_restricted_age_ids = [media.content for media in instagram_results if media.type_ is MediaType.ERROR]
+
             if not instagram_results:
+                v2_ids = instagram_ids
+            elif instagram_restricted_age_ids:
+                v2_ids = instagram_restricted_age_ids
+            else:
+                v2_ids = []
+
+            if v2_ids:
                 try:
                     instagram_results = await instagram.get_medias_v2(instagram_ids, audio_only)
                 except InstagramMediaNotFoundError as e:
                     if not (instagram_results := await yt_dlp_wrapper.get_medias(instagram.make_urls(instagram_ids), 'h264', 'mp4', force, audio_only, timeout_for_media)):
                         exceptions.append(e)
 
-                if instagram_results and can_instagram_v1:
+                if instagram_results and can_instagram_v1 and not instagram_restricted_age_ids:
                     self.instagram_ban_date = datetime.datetime.now(datetime.timezone.utc)
                     await self.send('Límite de Instagram excedido.', await self.owner_chat)
 
         gather_results = await gather_future
         await self.delete_message(bot_state_message)
 
         gather_medias, gather_exceptions = flanautils.filter_exceptions(gather_results + instagram_results)
@@ -373,28 +384,28 @@
 
         if not message.is_inline:
             bot_state_message: Message = await self.send('Enviando...', message)
 
         if message.chat.is_group:
             sended_info_message = await self.send(f"{message.author.name.split('#')[0]} compartió{self._medias_sended_info(medias)}", message, reply_to=message.replied_message)
             if (
-                    send_user_context
-                    and
-                    (user_text := ' '.join(
-                        [word for word in message.text.split()
-                         if (
-                                 not any(await self._find_ids(word))
-                                 and
-                                 not flanautils.find_urls(word)
-                                 and
-                                 not flanautils.cartesian_product_string_matching(word, keywords, multibot_constants.PARSER_MIN_SCORE_DEFAULT)
-                                 and
-                                 flanautils.remove_symbols(word).lower() not in (str(self.id), self.name.lower())
-                         )]
-                    ))
+                send_user_context
+                and
+                (user_text := ' '.join(
+                    [word for word in message.text.split()
+                     if (
+                         not any(await self._find_ids(word))
+                         and
+                         not flanautils.find_urls(word)
+                         and
+                         not flanautils.cartesian_product_string_matching(word, keywords, multibot_constants.PARSER_MIN_SCORE_DEFAULT)
+                         and
+                         flanautils.remove_symbols(word).lower() not in (str(self.id), self.name.lower())
+                     )]
+                ))
             ):
                 user_text_bot_message = await self.send(user_text, message, reply_to=message.replied_message)
 
         for media in medias:
             if not media.content:
                 fails += 1
                 continue
```

### Comparing `flanabot-1.5.1/flanabot/bots/ubereats_bot.py` & `flanabot-1.5.2/flanabot/bots/ubereats_bot.py`

 * *Files identical despite different names*

### Comparing `flanabot-1.5.1/flanabot/bots/weather_bot.py` & `flanabot-1.5.2/flanabot/bots/weather_bot.py`

 * *Files identical despite different names*

### Comparing `flanabot-1.5.1/flanabot/connect_4_frontend.py` & `flanabot-1.5.2/flanabot/connect_4_frontend.py`

 * *Files identical despite different names*

### Comparing `flanabot-1.5.1/flanabot/constants.py` & `flanabot-1.5.2/flanabot/constants.py`

 * *Files identical despite different names*

### Comparing `flanabot-1.5.1/flanabot/models/bot_action.py` & `flanabot-1.5.2/flanabot/models/bot_action.py`

 * *Files identical despite different names*

### Comparing `flanabot-1.5.1/flanabot/models/chat.py` & `flanabot-1.5.2/flanabot/models/chat.py`

 * *Files identical despite different names*

### Comparing `flanabot-1.5.1/flanabot/models/message.py` & `flanabot-1.5.2/flanabot/models/message.py`

 * *Files identical despite different names*

### Comparing `flanabot-1.5.1/flanabot/models/weather_chart.py` & `flanabot-1.5.2/flanabot/models/weather_chart.py`

 * *Files identical despite different names*

### Comparing `flanabot-1.5.1/flanabot/resources/mucho_texto.png` & `flanabot-1.5.2/flanabot/resources/mucho_texto.png`

 * *Files identical despite different names*

### Comparing `flanabot-1.5.1/flanabot.egg-info/PKG-INFO` & `flanabot-1.5.2/flanabot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flanabot
-Version: 1.5.1
+Version: 1.5.2
 Summary: Bot based on https://github.com/AlberLC/multibot to manage Discord, Telegram and Twitch chats, moderate them and add functionalities.
 Home-page: https://github.com/AlberLC/flanabot
 Author: AlberLC
 Project-URL: Bug Tracker, https://github.com/AlberLC/flanabot/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `flanabot-1.5.1/flanabot.egg-info/SOURCES.txt` & `flanabot-1.5.2/flanabot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flanabot-1.5.1/setup.cfg` & `flanabot-1.5.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = flanabot
-version = v1.5.1
+version = v1.5.2
 author = AlberLC
 description = Bot based on https://github.com/AlberLC/multibot to manage Discord, Telegram and Twitch chats, moderate them and add functionalities.
 long_description = file: README.rst
 url = https://github.com/AlberLC/flanabot
 project_urls = 
 	Bug Tracker = https://github.com/AlberLC/flanabot/issues
 classifiers =
```

