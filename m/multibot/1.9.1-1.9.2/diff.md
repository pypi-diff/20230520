# Comparing `tmp/multibot-1.9.1.tar.gz` & `tmp/multibot-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multibot-1.9.1.tar", last modified: Sat May  6 18:45:29 2023, max compression
+gzip compressed data, was "multibot-1.9.2.tar", last modified: Sat May 20 04:32:50 2023, max compression
```

## Comparing `multibot-1.9.1.tar` & `multibot-1.9.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:45:29.423969 multibot-1.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-06 18:45:10.000000 multibot-1.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18536 2023-05-06 18:45:29.423969 multibot-1.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17861 2023-05-06 18:45:10.000000 multibot-1.9.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:45:29.415969 multibot-1.9.1/multibot/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-06 18:45:10.000000 multibot-1.9.1/multibot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:45:29.419968 multibot-1.9.1/multibot/bots/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-06 18:45:10.000000 multibot-1.9.1/multibot/bots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28838 2023-05-06 18:45:10.000000 multibot-1.9.1/multibot/bots/discord_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)    41050 2023-05-06 18:45:10.000000 multibot-1.9.1/multibot/bots/multi_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)    26591 2023-05-06 18:45:10.000000 multibot-1.9.1/multibot/bots/telegram_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)    12498 2023-05-06 18:45:10.000000 multibot-1.9.1/multibot/bots/twitch_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-05-06 18:45:10.000000 multibot-1.9.1/multibot/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-06 18:45:10.000000 multibot-1.9.1/multibot/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:45:29.423969 multibot-1.9.1/multibot/models/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-06 18:45:10.000000 multibot-1.9.1/multibot/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-06 18:45:10.000000 multibot-1.9.1/multibot/models/buttons.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-06 18:45:10.000000 multibot-1.9.1/multibot/models/chat.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-06 18:45:10.000000 multibot-1.9.1/multibot/models/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-06 18:45:10.000000 multibot-1.9.1/multibot/models/event_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-06 18:45:10.000000 multibot-1.9.1/multibot/models/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-06 18:45:10.000000 multibot-1.9.1/multibot/models/penalties.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-06 18:45:10.000000 multibot-1.9.1/multibot/models/registered_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-06 18:45:10.000000 multibot-1.9.1/multibot/models/role.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-06 18:45:10.000000 multibot-1.9.1/multibot/models/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:45:29.419968 multibot-1.9.1/multibot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18536 2023-05-06 18:45:29.000000 multibot-1.9.1/multibot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-06 18:45:29.000000 multibot-1.9.1/multibot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 18:45:29.000000 multibot-1.9.1/multibot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-06 18:45:29.000000 multibot-1.9.1/multibot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-06 18:45:29.000000 multibot-1.9.1/multibot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-06 18:45:10.000000 multibot-1.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-06 18:45:29.423969 multibot-1.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 04:32:50.096953 multibot-1.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-20 04:32:36.000000 multibot-1.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18536 2023-05-20 04:32:50.096953 multibot-1.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17861 2023-05-20 04:32:36.000000 multibot-1.9.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 04:32:50.092953 multibot-1.9.2/multibot/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-20 04:32:36.000000 multibot-1.9.2/multibot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 04:32:50.096953 multibot-1.9.2/multibot/bots/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-20 04:32:36.000000 multibot-1.9.2/multibot/bots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28838 2023-05-20 04:32:36.000000 multibot-1.9.2/multibot/bots/discord_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41554 2023-05-20 04:32:36.000000 multibot-1.9.2/multibot/bots/multi_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26591 2023-05-20 04:32:36.000000 multibot-1.9.2/multibot/bots/telegram_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12498 2023-05-20 04:32:36.000000 multibot-1.9.2/multibot/bots/twitch_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-05-20 04:32:36.000000 multibot-1.9.2/multibot/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-20 04:32:36.000000 multibot-1.9.2/multibot/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 04:32:50.096953 multibot-1.9.2/multibot/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-20 04:32:36.000000 multibot-1.9.2/multibot/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-20 04:32:36.000000 multibot-1.9.2/multibot/models/buttons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-20 04:32:36.000000 multibot-1.9.2/multibot/models/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-20 04:32:36.000000 multibot-1.9.2/multibot/models/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-20 04:32:36.000000 multibot-1.9.2/multibot/models/event_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-20 04:32:36.000000 multibot-1.9.2/multibot/models/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-20 04:32:36.000000 multibot-1.9.2/multibot/models/penalties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-20 04:32:36.000000 multibot-1.9.2/multibot/models/registered_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-20 04:32:36.000000 multibot-1.9.2/multibot/models/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-20 04:32:36.000000 multibot-1.9.2/multibot/models/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 04:32:50.096953 multibot-1.9.2/multibot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18536 2023-05-20 04:32:50.000000 multibot-1.9.2/multibot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-20 04:32:50.000000 multibot-1.9.2/multibot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 04:32:50.000000 multibot-1.9.2/multibot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-20 04:32:50.000000 multibot-1.9.2/multibot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-20 04:32:50.000000 multibot-1.9.2/multibot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-20 04:32:36.000000 multibot-1.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-20 04:32:50.096953 multibot-1.9.2/setup.cfg
```

### Comparing `multibot-1.9.1/LICENSE` & `multibot-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `multibot-1.9.1/PKG-INFO` & `multibot-1.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multibot
-Version: 1.9.1
+Version: 1.9.2
 Summary: Platform agnostic high-level bot infrastructure. Develop one bot and you will have three: one for Discord, another one for Telegram and another one for Twitch. All bots use the same objects and logic.  For now there are adapters for three platforms but more may be added in the future.
 Home-page: https://github.com/AlberLC/multibot
 Author: AlberLC
 Project-URL: Bug Tracker, https://github.com/AlberLC/multibot/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `multibot-1.9.1/README.rst` & `multibot-1.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `multibot-1.9.1/multibot/bots/discord_bot.py` & `multibot-1.9.2/multibot/bots/discord_bot.py`

 * *Files identical despite different names*

### Comparing `multibot-1.9.1/multibot/bots/multi_bot.py` & `multibot-1.9.2/multibot/bots/multi_bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -557,16 +557,23 @@
         media: Media = None,
         buttons: list[str | tuple[str, bool] | Button | list[str | tuple[str, bool] | Button]] | None = None,
         chat: int | str | User | Chat | Message | None = None,
         buttons_key: Any = None,
         data: dict = None,
         update_last_edit=False
     ):
-        if media is not None and (not media.bytes_ or len(media.bytes_) <= constants.PYMONGO_MEDIA_MAX_BYTES):
-            message.medias = [media]
+        if media is not None:
+            if len(bytes(media)) <= constants.PYMONGO_MEDIA_MAX_BYTES:
+                message.medias = [media]
+            else:
+                empty_media = Media.from_dict({k: v for k, v in media.to_dict().items() if k not in ('bytes_', 'song_info')})
+                if media.song_info:
+                    empty_song_info = Media.from_dict({k: v for k, v in media.song_info.to_dict().items() if k != 'bytes_'})
+                    empty_media.song_info = empty_song_info
+                message.medias = [empty_media]
         try:
             if buttons is not None:
                 self._message_cache[message.id, chat.id].buttons_info.buttons = buttons
             if buttons_key is not None:
                 self._message_cache[message.id, chat.id].buttons_info.key = buttons_key
         except (AttributeError, KeyError):
             message.buttons_info = ButtonsInfo(buttons=buttons, key=buttons_key)
@@ -857,24 +864,24 @@
     @property
     async def owner_chat(self) -> Chat:
         if not self._owner_chat:
             self._owner_chat = await self.get_chat(self.owner_id) or await self.get_chat(await self.get_user(self.owner_id))
         return self._owner_chat
 
     @overload
-    def register(self, func_: Callable = None, keywords=(), priority: int | float = 1, min_score=constants.PARSER_MIN_SCORE_DEFAULT, always=False, default=False):
+    def register(self, func_: Callable = None, keywords: str | Iterable[str | Iterable[str]] = (), priority: int | float = 1, min_score=constants.PARSER_MIN_SCORE_DEFAULT, always=False, default=False):
         pass
 
     @overload
-    def register(self, keywords=(), priority: int | float = 1, min_score=constants.PARSER_MIN_SCORE_DEFAULT, always=False, default=False):
+    def register(self, keywords: str | Iterable[str | Iterable[str]] = (), priority: int | float = 1, min_score=constants.PARSER_MIN_SCORE_DEFAULT, always=False, default=False):
         pass
 
     @shift_args_if_called(exclude_self_types='MultiBot', globals_=globals())
     def register(self, func_: Callable = None, keywords: str | Iterable[str | Iterable[str]] = (), priority: int | float = 1, min_score=constants.PARSER_MIN_SCORE_DEFAULT, always=False, default=False):
-        def decorator(func):
+        def decorator(func: Callable):
             self._registered_callbacks.append(RegisteredCallback(func, keywords, priority, min_score, always, default))
             return func
 
         return decorator(func_) if func_ else decorator
 
     @overload
     def register_button(self, func_: Callable = None, key: Any = None):
@@ -882,15 +889,15 @@
 
     @overload
     def register_button(self, key: Any = None):
         pass
 
     @shift_args_if_called(exclude_self_types='MultiBot', globals_=globals())
     def register_button(self, func_: Callable = None, key: Any = None):
-        def decorator(func):
+        def decorator(func: Callable):
             self._registered_button_callbacks[key].append(func)
             return func
 
         return decorator(func_) if func_ else decorator
 
     async def remove_role(self, user: int | str | User, group_: int | str | Chat | Message, role: int | str | Role):
         pass
```

### Comparing `multibot-1.9.1/multibot/bots/telegram_bot.py` & `multibot-1.9.2/multibot/bots/telegram_bot.py`

 * *Files identical despite different names*

### Comparing `multibot-1.9.1/multibot/bots/twitch_bot.py` & `multibot-1.9.2/multibot/bots/twitch_bot.py`

 * *Files identical despite different names*

### Comparing `multibot-1.9.1/multibot/constants.py` & `multibot-1.9.2/multibot/constants.py`

 * *Files identical despite different names*

### Comparing `multibot-1.9.1/multibot/models/buttons.py` & `multibot-1.9.2/multibot/models/buttons.py`

 * *Files identical despite different names*

### Comparing `multibot-1.9.1/multibot/models/chat.py` & `multibot-1.9.2/multibot/models/chat.py`

 * *Files identical despite different names*

### Comparing `multibot-1.9.1/multibot/models/event_component.py` & `multibot-1.9.2/multibot/models/event_component.py`

 * *Files identical despite different names*

### Comparing `multibot-1.9.1/multibot/models/message.py` & `multibot-1.9.2/multibot/models/message.py`

 * *Files identical despite different names*

### Comparing `multibot-1.9.1/multibot/models/penalties.py` & `multibot-1.9.2/multibot/models/penalties.py`

 * *Files identical despite different names*

### Comparing `multibot-1.9.1/multibot/models/registered_callback.py` & `multibot-1.9.2/multibot/models/registered_callback.py`

 * *Files identical despite different names*

### Comparing `multibot-1.9.1/multibot/models/user.py` & `multibot-1.9.2/multibot/models/user.py`

 * *Files identical despite different names*

### Comparing `multibot-1.9.1/multibot.egg-info/PKG-INFO` & `multibot-1.9.2/multibot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multibot
-Version: 1.9.1
+Version: 1.9.2
 Summary: Platform agnostic high-level bot infrastructure. Develop one bot and you will have three: one for Discord, another one for Telegram and another one for Twitch. All bots use the same objects and logic.  For now there are adapters for three platforms but more may be added in the future.
 Home-page: https://github.com/AlberLC/multibot
 Author: AlberLC
 Project-URL: Bug Tracker, https://github.com/AlberLC/multibot/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `multibot-1.9.1/multibot.egg-info/SOURCES.txt` & `multibot-1.9.2/multibot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `multibot-1.9.1/setup.cfg` & `multibot-1.9.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = multibot
-version = v1.9.1
+version = v1.9.2
 author = AlberLC
 description = Platform agnostic high-level bot infrastructure. Develop one bot and you will have three: one for Discord, another one for Telegram and another one for Twitch. All bots use the same objects and logic.  For now there are adapters for three platforms but more may be added in the future.
 long_description = file: README.rst
 url = https://github.com/AlberLC/multibot
 project_urls = 
 	Bug Tracker = https://github.com/AlberLC/multibot/issues
 classifiers =
```

