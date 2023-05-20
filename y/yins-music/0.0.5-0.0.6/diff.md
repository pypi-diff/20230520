# Comparing `tmp/yins-music-0.0.5.tar.gz` & `tmp/yins-music-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yins-music-0.0.5.tar", last modified: Fri May 12 05:27:49 2023, max compression
+gzip compressed data, was "yins-music-0.0.6.tar", last modified: Sat May 20 07:56:28 2023, max compression
```

## Comparing `yins-music-0.0.5.tar` & `yins-music-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 05:27:49.543244 yins-music-0.0.5/
--rw-rw-rw-   0        0        0     7815 2023-05-12 05:05:19.000000 yins-music-0.0.5/LICENSE
--rw-rw-rw-   0        0        0       15 2023-05-12 05:05:19.000000 yins-music-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0    12226 2023-05-12 05:27:49.542245 yins-music-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0    10043 2023-05-12 05:05:19.000000 yins-music-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-05-12 05:27:49.544244 yins-music-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     8093 2023-05-12 05:27:46.000000 yins-music-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-12 05:27:49.538246 yins-music-0.0.5/yins_music.egg-info/
--rw-rw-rw-   0        0        0    12226 2023-05-12 05:27:49.000000 yins-music-0.0.5/yins_music.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2023-05-12 05:27:49.000000 yins-music-0.0.5/yins_music.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 05:27:49.000000 yins-music-0.0.5/yins_music.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      115 2023-05-12 05:27:49.000000 yins-music-0.0.5/yins_music.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 05:27:49.000000 yins-music-0.0.5/yins_music.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-20 07:56:28.514541 yins-music-0.0.6/
+-rw-rw-rw-   0        0        0     7815 2023-05-20 07:52:21.000000 yins-music-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0       15 2023-05-20 07:52:21.000000 yins-music-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0    12226 2023-05-20 07:56:28.513541 yins-music-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0    10043 2023-05-20 07:52:21.000000 yins-music-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-20 07:56:28.515541 yins-music-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     8093 2023-05-20 07:52:21.000000 yins-music-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 07:56:28.510547 yins-music-0.0.6/yins_music.egg-info/
+-rw-rw-rw-   0        0        0    12226 2023-05-20 07:56:28.000000 yins-music-0.0.6/yins_music.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      207 2023-05-20 07:56:28.000000 yins-music-0.0.6/yins_music.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 07:56:28.000000 yins-music-0.0.6/yins_music.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      115 2023-05-20 07:56:28.000000 yins-music-0.0.6/yins_music.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 07:56:28.000000 yins-music-0.0.6/yins_music.egg-info/top_level.txt
```

### Comparing `yins-music-0.0.5/LICENSE` & `yins-music-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `yins-music-0.0.5/PKG-INFO` & `yins-music-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yins-music
-Version: 0.0.5
+Version: 0.0.6
 Summary: a library connecting the tgcalls Python binding with MTProto
 Home-page: https://github.com/MarshalX/tgcalls
 Author: AyiinXd
 Author-email: ayiinxd0307@gmail.com
 License: LGPLv3
 Project-URL: Documentation, https://tgcalls.org/
 Project-URL: Telegram Channel, https://t.me/tgcallslib
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: yins-music Version: 0.0.5 Summary: a library
+Metadata-Version: 2.1 Name: yins-music Version: 0.0.6 Summary: a library
 connecting the tgcalls Python binding with MTProto Home-page: https://
 github.com/MarshalX/tgcalls Author: AyiinXd Author-email: ayiinxd0307@gmail.com
 License: LGPLv3 Project-URL: Documentation, https://tgcalls.org/ Project-URL:
 Telegram Channel, https://t.me/tgcallslib Project-URL: Telegram Chat, https://
 t.me/tgcallschat Project-URL: Author, https://github.com/AyiinXd Keywords:
 python,library,telegram,async,asynchronous,webrtc,lib,voice-chat,voip,group-
 chat,video-call,calls,fipper,telethon,pytgcalls,tgcalls Classifier: Development
```

### Comparing `yins-music-0.0.5/README.md` & `yins-music-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `yins-music-0.0.5/setup.py` & `yins-music-0.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
 
 
 with open(path.join(base_path, 'README.md'), 'r', encoding='utf-8') as f:
     readme = f.read()
 
 setup(
     name='tg-music',
-    version="1.0.0.dev4",
+    version="1.0.0.dev5",
     author='AyiinXd',
     author_email='ayiinxd0307@gmail.com',
     license='LGPLv3',
     url='https://github.com/AyiinXd/tgcalls',
     keywords='python, library, telegram, async, asynchronous, webrtc, lib, voice-chat, '
     'voip, group-chat, video-call, calls, fipper, telethon, pytgcalls, tgcalls',
     description='a Python binding for tgcalls C++ library',
```

### Comparing `yins-music-0.0.5/yins_music.egg-info/PKG-INFO` & `yins-music-0.0.6/yins_music.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yins-music
-Version: 0.0.5
+Version: 0.0.6
 Summary: a library connecting the tgcalls Python binding with MTProto
 Home-page: https://github.com/MarshalX/tgcalls
 Author: AyiinXd
 Author-email: ayiinxd0307@gmail.com
 License: LGPLv3
 Project-URL: Documentation, https://tgcalls.org/
 Project-URL: Telegram Channel, https://t.me/tgcallslib
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: yins-music Version: 0.0.5 Summary: a library
+Metadata-Version: 2.1 Name: yins-music Version: 0.0.6 Summary: a library
 connecting the tgcalls Python binding with MTProto Home-page: https://
 github.com/MarshalX/tgcalls Author: AyiinXd Author-email: ayiinxd0307@gmail.com
 License: LGPLv3 Project-URL: Documentation, https://tgcalls.org/ Project-URL:
 Telegram Channel, https://t.me/tgcallslib Project-URL: Telegram Chat, https://
 t.me/tgcallschat Project-URL: Author, https://github.com/AyiinXd Keywords:
 python,library,telegram,async,asynchronous,webrtc,lib,voice-chat,voip,group-
 chat,video-call,calls,fipper,telethon,pytgcalls,tgcalls Classifier: Development
```

