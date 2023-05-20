# Comparing `tmp/goyabu-cli-1.0.8.tar.gz` & `tmp/goyabu-cli-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goyabu-cli-1.0.8.tar", last modified: Wed Dec 28 15:18:50 2022, max compression
+gzip compressed data, was "goyabu-cli-1.0.9.tar", last modified: Tue Jan 10 21:19:52 2023, max compression
```

## Comparing `goyabu-cli-1.0.8.tar` & `goyabu-cli-1.0.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-12-28 15:18:50.549321 goyabu-cli-1.0.8/
--rwxrwxrwx   0 root         (0) root         (0)     1067 2022-12-11 01:44:04.000000 goyabu-cli-1.0.8/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     5691 2022-12-28 15:18:50.549857 goyabu-cli-1.0.8/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     4178 2022-12-20 15:53:09.000000 goyabu-cli-1.0.8/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-12-28 15:18:50.530973 goyabu-cli-1.0.8/goyabu_cli.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     5691 2022-12-28 15:18:50.000000 goyabu-cli-1.0.8/goyabu_cli.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      721 2022-12-28 15:18:50.000000 goyabu-cli-1.0.8/goyabu_cli.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2022-12-28 15:18:50.000000 goyabu-cli-1.0.8/goyabu_cli.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       50 2022-12-28 15:18:50.000000 goyabu-cli-1.0.8/goyabu_cli.egg-info/entry_points.txt
--rwxrwxrwx   0 root         (0) root         (0)      106 2022-12-28 15:18:50.000000 goyabu-cli-1.0.8/goyabu_cli.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       10 2022-12-28 15:18:50.000000 goyabu-cli-1.0.8/goyabu_cli.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-12-28 15:18:50.547227 goyabu-cli-1.0.8/goyabucli/
--rwxrwxrwx   0 root         (0) root         (0)        0 2022-12-20 16:47:01.000000 goyabu-cli-1.0.8/goyabucli/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     6487 2022-12-26 15:37:58.000000 goyabu-cli-1.0.8/goyabucli/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)     9863 2022-12-28 14:18:22.000000 goyabu-cli-1.0.8/goyabucli/anilistManager.py
--rwxrwxrwx   0 root         (0) root         (0)     9779 2022-12-28 15:02:31.000000 goyabu-cli-1.0.8/goyabucli/cli.py
--rwxrwxrwx   0 root         (0) root         (0)    15033 2022-12-25 01:21:59.000000 goyabu-cli-1.0.8/goyabucli/dropdown.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-12-28 15:18:50.547937 goyabu-cli-1.0.8/goyabucli/extractors/
--rwxrwxrwx   0 root         (0) root         (0)        0 2022-12-11 13:52:36.000000 goyabu-cli-1.0.8/goyabucli/extractors/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      584 2022-12-20 13:02:26.000000 goyabu-cli-1.0.8/goyabucli/extractors/blogger.py
--rwxrwxrwx   0 root         (0) root         (0)     3587 2022-12-28 15:01:26.000000 goyabu-cli-1.0.8/goyabucli/playerManager.py
--rwxrwxrwx   0 root         (0) root         (0)     1661 2022-12-24 23:57:46.000000 goyabu-cli-1.0.8/goyabucli/progress.py
--rwxrwxrwx   0 root         (0) root         (0)     2639 2022-11-02 19:38:31.000000 goyabu-cli-1.0.8/goyabucli/rawserver.py
--rwxrwxrwx   0 root         (0) root         (0)     6132 2022-12-20 14:27:44.000000 goyabu-cli-1.0.8/goyabucli/scraper.py
--rwxrwxrwx   0 root         (0) root         (0)     1097 2022-12-20 13:46:47.000000 goyabu-cli-1.0.8/goyabucli/scraperManager.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-12-28 15:18:50.548976 goyabu-cli-1.0.8/goyabucli/scrapers/
--rwxrwxrwx   0 root         (0) root         (0)        0 2022-12-11 00:31:56.000000 goyabu-cli-1.0.8/goyabucli/scrapers/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     2780 2022-12-20 14:50:58.000000 goyabu-cli-1.0.8/goyabucli/scrapers/animefire.py
--rwxrwxrwx   0 root         (0) root         (0)     2139 2022-12-20 15:15:42.000000 goyabu-cli-1.0.8/goyabucli/scrapers/goyabuNew.py
--rwxrwxrwx   0 root         (0) root         (0)     8801 2022-12-28 14:41:27.000000 goyabu-cli-1.0.8/goyabucli/sessionManager.py
--rwxrwxrwx   0 root         (0) root         (0)     2356 2022-12-26 15:32:37.000000 goyabu-cli-1.0.8/goyabucli/translation.py
--rwxrwxrwx   0 root         (0) root         (0)     2628 2022-12-26 13:42:35.000000 goyabu-cli-1.0.8/goyabucli/utils.py
--rwxrwxrwx   0 root         (0) root         (0)      634 2022-12-28 15:18:27.000000 goyabu-cli-1.0.8/pyproject.toml
--rwxrwxrwx   0 root         (0) root         (0)       79 2022-12-28 15:18:50.551092 goyabu-cli-1.0.8/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      357 2022-12-11 01:38:59.000000 goyabu-cli-1.0.8/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-10 21:19:52.263379 goyabu-cli-1.0.9/
+-rwxrwxrwx   0 root         (0) root         (0)     1067 2022-12-11 01:44:04.000000 goyabu-cli-1.0.9/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)     5691 2023-01-10 21:19:52.263737 goyabu-cli-1.0.9/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     4178 2022-12-20 15:53:09.000000 goyabu-cli-1.0.9/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-10 21:19:52.254423 goyabu-cli-1.0.9/goyabu_cli.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     5691 2023-01-10 21:19:52.000000 goyabu-cli-1.0.9/goyabu_cli.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      721 2023-01-10 21:19:52.000000 goyabu-cli-1.0.9/goyabu_cli.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-01-10 21:19:52.000000 goyabu-cli-1.0.9/goyabu_cli.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       50 2023-01-10 21:19:52.000000 goyabu-cli-1.0.9/goyabu_cli.egg-info/entry_points.txt
+-rwxrwxrwx   0 root         (0) root         (0)      106 2023-01-10 21:19:52.000000 goyabu-cli-1.0.9/goyabu_cli.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       10 2023-01-10 21:19:52.000000 goyabu-cli-1.0.9/goyabu_cli.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-10 21:19:52.261251 goyabu-cli-1.0.9/goyabucli/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2022-12-20 16:47:01.000000 goyabu-cli-1.0.9/goyabucli/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     6667 2023-01-10 21:13:19.000000 goyabu-cli-1.0.9/goyabucli/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)    10154 2023-01-09 22:57:41.000000 goyabu-cli-1.0.9/goyabucli/anilistManager.py
+-rwxrwxrwx   0 root         (0) root         (0)     9781 2023-01-10 21:08:43.000000 goyabu-cli-1.0.9/goyabucli/cli.py
+-rwxrwxrwx   0 root         (0) root         (0)    17672 2023-01-10 21:07:06.000000 goyabu-cli-1.0.9/goyabucli/dropdown.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-10 21:19:52.261914 goyabu-cli-1.0.9/goyabucli/extractors/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2022-12-11 13:52:36.000000 goyabu-cli-1.0.9/goyabucli/extractors/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      584 2022-12-20 13:02:26.000000 goyabu-cli-1.0.9/goyabucli/extractors/blogger.py
+-rwxrwxrwx   0 root         (0) root         (0)     3587 2022-12-28 15:01:26.000000 goyabu-cli-1.0.9/goyabucli/playerManager.py
+-rwxrwxrwx   0 root         (0) root         (0)     1661 2022-12-24 23:57:46.000000 goyabu-cli-1.0.9/goyabucli/progress.py
+-rwxrwxrwx   0 root         (0) root         (0)     2639 2022-11-02 19:38:31.000000 goyabu-cli-1.0.9/goyabucli/rawserver.py
+-rwxrwxrwx   0 root         (0) root         (0)     6143 2023-01-09 20:51:48.000000 goyabu-cli-1.0.9/goyabucli/scraper.py
+-rwxrwxrwx   0 root         (0) root         (0)     1097 2022-12-20 13:46:47.000000 goyabu-cli-1.0.9/goyabucli/scraperManager.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-01-10 21:19:52.263042 goyabu-cli-1.0.9/goyabucli/scrapers/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2022-12-11 00:31:56.000000 goyabu-cli-1.0.9/goyabucli/scrapers/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2780 2022-12-20 14:50:58.000000 goyabu-cli-1.0.9/goyabucli/scrapers/animefire.py
+-rwxrwxrwx   0 root         (0) root         (0)     2139 2022-12-20 15:15:42.000000 goyabu-cli-1.0.9/goyabucli/scrapers/goyabuNew.py
+-rwxrwxrwx   0 root         (0) root         (0)    10024 2023-01-10 21:09:05.000000 goyabu-cli-1.0.9/goyabucli/sessionManager.py
+-rwxrwxrwx   0 root         (0) root         (0)     2356 2022-12-26 15:32:37.000000 goyabu-cli-1.0.9/goyabucli/translation.py
+-rwxrwxrwx   0 root         (0) root         (0)     2628 2022-12-26 13:42:35.000000 goyabu-cli-1.0.9/goyabucli/utils.py
+-rwxrwxrwx   0 root         (0) root         (0)      634 2023-01-09 22:59:14.000000 goyabu-cli-1.0.9/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)       79 2023-01-10 21:19:52.264641 goyabu-cli-1.0.9/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      357 2022-12-11 01:38:59.000000 goyabu-cli-1.0.9/setup.py
```

### Comparing `goyabu-cli-1.0.8/LICENSE` & `goyabu-cli-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `goyabu-cli-1.0.8/PKG-INFO` & `goyabu-cli-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goyabu-cli
-Version: 1.0.8
+Version: 1.0.9
 Summary: quickly play anime from terminal
 Home-page: https://github.com/AlanJs26/goyabu-cli
 Author: AlanJS26
 Author-email: AlanJS26 <alanjoses.29@gmail.com>
 License: MIT License
         
         Copyright (c) 2018 Alan José
```

### Comparing `goyabu-cli-1.0.8/README.md` & `goyabu-cli-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `goyabu-cli-1.0.8/goyabu_cli.egg-info/PKG-INFO` & `goyabu-cli-1.0.9/goyabu_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goyabu-cli
-Version: 1.0.8
+Version: 1.0.9
 Summary: quickly play anime from terminal
 Home-page: https://github.com/AlanJs26/goyabu-cli
 Author: AlanJS26
 Author-email: AlanJS26 <alanjoses.29@gmail.com>
 License: MIT License
         
         Copyright (c) 2018 Alan José
```

### Comparing `goyabu-cli-1.0.8/goyabu_cli.egg-info/SOURCES.txt` & `goyabu-cli-1.0.9/goyabu_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `goyabu-cli-1.0.8/goyabucli/__main__.py` & `goyabu-cli-1.0.9/goyabucli/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,18 +67,20 @@
                     help='change config using the cli')
 parser.add_argument('--config-dir',    action='store', default='~/.goyabucli',    type=dir_path, metavar='config directory',
                     help='directory for the watch list')
 
 args = parser.parse_args()
 
 # TODO -> implement on demand server TUI
-# TODO -> implement scraper filter to anime selection
+# TODO -> add 'planning to watch' animes in main list as a filter
+# DONE -> implement scraper filter to anime selection
 # DONE -> implement configuration TUI
 #   DONE -> config file
 # DONE -> anilist integration
+# TODO -> finish translation
 
 def main():
 
     config = Config(config_dir=args.config_dir, player=args.player, anilist_username='', token='', silent=False)
 
     if path.isfile(path.join(args.config_dir, 'config.json')):
         with open(path.join(args.config_dir, 'config.json')) as file:
@@ -114,16 +116,18 @@
         try: 
             if args.anilist_sync == 'prefer_local':
                 anilistManager.merge_session(sessionmanager)
             elif args.anilist_sync == 'prefer_remote':
                 anilistManager.merge_session(sessionmanager, preferRemote=True)
             elif args.anilist_sync == 'replace_local':
                 sessionmanager.session_items = []
-                watching_animes = list(map(lambda x:x.anime, anilistManager.get_watching()))
-                sessionmanager.add(watching_animes)
+                # watching_animes = list(map(lambda x:x.anime, anilistManager.get_watching()))
+                # sessionmanager.add(watching_animes)
+
+                sessionmanager.add_session_items(anilistManager.get_watching())
             elif args.anilist_sync == 'replace_remote':
                 anilistManager.set_watching(sessionmanager.session_items)
 
             sessionmanager.dump(verbose=True)
         except MissingToken:
             if not config.silent:
                 warning("wasn't possible sync with anilist. Missing authentification token")
```

### Comparing `goyabu-cli-1.0.8/goyabucli/anilistManager.py` & `goyabu-cli-1.0.9/goyabucli/anilistManager.py`

 * *Files 3% similar despite different names*

```diff
@@ -115,15 +115,15 @@
                 if foundAnime:
                     session_item.anilist_id = foundAnime.anilist_id
                     session_item.episodesInTotal = foundAnime.episodesInTotal
                     return
 
             episodesInTotal = self.getTotalEpisodesCount(title=session_item.title, id=session_item.anilist_id)
 
-            session_item.episodesInTotal = episodesInTotal or session_item.episodesInTotal
+            session_item.episodesInTotal = episodesInTotal or session_item.episodesInTotal or session_item.availableEpisodes
 
         pbar = None
         if verbose:
             pbar = ProgressBar(total=len(session.session_items), postfix='Sincronizando com Anilist', leave=False)
 
         with ThreadPoolExecutor(max_workers=4) as executor:
             futures = [executor.submit(updateSessionItem, session_item) for session_item in session.session_items]
@@ -166,16 +166,16 @@
 
         for item in result:
             media = item['media']
             watch_list.append(
                 SessionItem(
                     Anime(media['title']['romaji'], media['title']['romaji']),
                     media['episodes'],
-                    media['nextAiringEpisode']['episode'] if media['nextAiringEpisode'] else media['episodes'],
-                    item['progress'],
+                    media['nextAiringEpisode']['episode']-1 if media['nextAiringEpisode'] else media['episodes'],
+                    item['progress'] or 1,
                     '',
                     anilist_id=media['id'],
                     duration=media['duration']*60
                 )
             )
 
         return watch_list
@@ -217,24 +217,28 @@
     def merge_session(self, session:SessionManager, preferRemote=False):
         watch_list = self.get_watching()
 
         intersecting_items:List[SessionItem] = []
         new_items:List[SessionItem] = []
 
         for watch_item in watch_list:
-            if session.has_anime(watch_item.anime):
+            if session.has_anime(watch_item.anime, anilist_id=watch_item.anilist_id):
                 intersecting_items.append(watch_item)
             else:
                 new_items.append(watch_item)
 
         if preferRemote:
             for watch_item in intersecting_items:
-                session.update(watch_item.anime, watch_item.lastEpisode, watch_item.watchTime, watch_item.duration)
+                session.update(watch_item.anime, watch_item.lastEpisode, watch_item.watchTime, watch_item.duration, episodesInTotal=watch_item.episodesInTotal)
+        else:
+            for watch_item in intersecting_items:
+                session.update(watch_item.anime, episodesInTotal=watch_item.episodesInTotal)
+
 
-        session.add_session_items(new_items)
+        session.add_session_items(new_items, inplace=True)
 
     def _request(self, query, variables):
         if not self.username:
             raise MissingUsername("Missing anilist username")
         res = requests.post(
             'https://graphql.anilist.co',
             json = {
```

### Comparing `goyabu-cli-1.0.8/goyabucli/cli.py` & `goyabu-cli-1.0.9/goyabucli/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,15 +201,15 @@
     except MissingToken:
         if not config.silent:
             warning("wasn't possible sync with anilist. Missing authentification token")
             warning("to get rid of this message, mark the option 'silent' to True in the config")
             warning("    eg: anime --config")
 
     print(t('Atualizando o histórico...'))
-    anilistManager.update_session(sessionmanager, True)
+    # anilistManager.update_session(sessionmanager, True)
     sessionmanager.dump(verbose=True, number_to_update=10)
 
     anime_session_item = sessionmanager.find(anime)
 
     if anime_session_item:
         anilistManager.set_watching([anime_session_item])
```

### Comparing `goyabu-cli-1.0.8/goyabucli/extractors/blogger.py` & `goyabu-cli-1.0.9/goyabucli/extractors/blogger.py`

 * *Files identical despite different names*

### Comparing `goyabu-cli-1.0.8/goyabucli/playerManager.py` & `goyabu-cli-1.0.9/goyabucli/playerManager.py`

 * *Files identical despite different names*

### Comparing `goyabu-cli-1.0.8/goyabucli/progress.py` & `goyabu-cli-1.0.9/goyabucli/progress.py`

 * *Files identical despite different names*

### Comparing `goyabu-cli-1.0.8/goyabucli/rawserver.py` & `goyabu-cli-1.0.9/goyabucli/rawserver.py`

 * *Files identical despite different names*

### Comparing `goyabu-cli-1.0.8/goyabucli/scraper.py` & `goyabu-cli-1.0.9/goyabucli/scraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
 
         for source in episode.sources:
             self.addSource(source[0], source[1])
 
 class Anime():
     def __init__(self, title:str, id:str, source='', pageUrl='', scrapers:List['Scraper']=[]):
         self.scrapers=scrapers
-        self.id = id
+        self.id = id.casefold()
         self.title = title
         self.episodes:Dict[str,Episode] = {
             # 'id1' : Episode('title', 'id1')
         }
         self.availableScrapers = [source]
 
         self.source = source
```

### Comparing `goyabu-cli-1.0.8/goyabucli/scraperManager.py` & `goyabu-cli-1.0.9/goyabucli/scraperManager.py`

 * *Files identical despite different names*

### Comparing `goyabu-cli-1.0.8/goyabucli/scrapers/animefire.py` & `goyabu-cli-1.0.9/goyabucli/scrapers/animefire.py`

 * *Files identical despite different names*

### Comparing `goyabu-cli-1.0.8/goyabucli/scrapers/goyabuNew.py` & `goyabu-cli-1.0.9/goyabucli/scrapers/goyabuNew.py`

 * *Files identical despite different names*

### Comparing `goyabu-cli-1.0.8/goyabucli/sessionManager.py` & `goyabu-cli-1.0.9/goyabucli/sessionManager.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from .scraper import Anime,Scraper
 from typing import List,Union,Optional
 from datetime import datetime, timezone
 from os import path, makedirs
 import json
-from .dropdown import interactiveTable,bcolors
+from .dropdown import interactiveTable,bcolors,HighlightedTable
 from .translation import t
 from .progress import ProgressBar
 from concurrent.futures import ThreadPoolExecutor, as_completed
+from rich import print as rprint
 
 
 
 class SessionItem():
     def __init__(self, anime:Anime, episodesInTotal:int, availableEpisodes:int, lastEpisode:int, lastSource:str, watchTime=0, duration=0, anilist_id:Optional[int]=None, date_utc=int(datetime.now().timestamp())):
         self.anime = anime
 
@@ -57,16 +58,16 @@
         if not path.isfile(path.join(root,self.filename)):
             with open(path.join(root,self.filename), 'w') as file:
                 json.dump({}, file)
 
         self.session_items:List[SessionItem] = []
         self.session_items = self.load()
 
-    def find(self, anime:Anime) -> Union[SessionItem,None]:
-        found_anime = next((item for item in self.session_items if item.anime.id == anime.id), None)
+    def find(self, anime:Anime, anilist_id:Optional[int]=None) -> Union[SessionItem,None]:
+        found_anime = next((item for item in self.session_items if item.anime.id == anime.id or (anilist_id and (item.anilist_id == anilist_id))), None)
 
         return found_anime
 
     def add(self, animes:List[Anime]):
         all_ids = [item.id for item in self.session_items]
         for anime in animes:
             if anime.id in all_ids: 
@@ -85,46 +86,48 @@
                         0,
                         len(anime.episodes),
                         0,
                         anime.source
                     )
                 )
 
-    def add_session_items(self, session_items:List[SessionItem]):
+    def add_session_items(self, session_items:List[SessionItem], inplace=False):
         all_ids = [item.id for item in self.session_items]
         for session_item in session_items:
             if session_item.id in all_ids: 
                 right_sessionItem = self.session_items[all_ids.index(session_item.id)]
                 right_sessionItem.lastSource = session_item.lastSource
                 right_sessionItem.availableEpisodes = session_item.availableEpisodes
                 right_sessionItem.anime = session_item.anime
 
                 # Move session item to the end of the list
-                self.session_items.remove(right_sessionItem)
-                self.session_items.append(right_sessionItem)
+                if not inplace:
+                    self.session_items.remove(right_sessionItem)
+                    self.session_items.append(right_sessionItem)
             else:
                 self.session_items.append(
                     session_item
                 )
 
-    def has_anime(self, anime:Anime) -> bool:
+    def has_anime(self, anime:Anime, anilist_id:Optional[int]=None) -> bool:
         for session_item in self.session_items:
-            if session_item.id == anime.id:
+            if session_item.id == anime.id or (anilist_id and (session_item.anilist_id == anilist_id)):
                 return True
         return False
 
-    def update(self, anime:Anime, lastEpisode:int, watchTime=0, duration=0):
+    def update(self, anime:Anime, lastEpisode=0, watchTime=0, duration=0, episodesInTotal=0):
         right_sessionItem = next(item for item in self.session_items if item.id == anime.id)
 
         if not right_sessionItem:
             raise IndexError(f"Cannot find '{anime.title}' in session items")
 
-        right_sessionItem.lastEpisode = lastEpisode
-        right_sessionItem.watchTime = watchTime
-        right_sessionItem.duration = duration
+        right_sessionItem.lastEpisode = lastEpisode or right_sessionItem.lastEpisode or 1
+        right_sessionItem.watchTime = watchTime or right_sessionItem.watchTime
+        right_sessionItem.duration = duration or right_sessionItem.duration
+        right_sessionItem.episodesInTotal = episodesInTotal or right_sessionItem.episodesInTotal
 
     def remove(self, id:str):
         right_sessionItem = next(item for item in self.session_items if item.id == id)
         self.session_items.remove(right_sessionItem)
 
     def load(self) -> List[SessionItem]:
         with open(path.join(self.root,self.filename)) as file:
@@ -206,36 +209,46 @@
             return status
 
         if not self.session_items:
             return str(input(hintText))
 
         table_rows = [[str(len(self.session_items)-index),item.title, format_status(item)] for index,item in enumerate(self.session_items)]
 
+        def myfilter(filter_name:str, items:List[List[str]], table:HighlightedTable):
+            table.clear()
+            if filter_name == 'incomplete':
+                table.update(list(filter(lambda x: 'Completo' not in x[2], items)), message=f'filter: {filter_name}', maxListSize=maxListSize)
+            elif filter_name == 'available':
+                table.update(list(filter(lambda x: bcolors['grey'] not in x[2] and bcolors['green'] not in x[2], items)), message=f'filter: {filter_name}', maxListSize=maxListSize)
+            else:
+                table.update(items, message='filter: none', maxListSize=maxListSize)
 
         results = interactiveTable(
             table_rows,
             ['' ,t("Sessoes anteriores"), t("Status")],
             "ccc",
             behaviour='multiSelectWithText',
             maxListSize=maxListSize,
             width=width,
             flexColumn=1,
             highlightRange=(2,2),
-            hintText=hintText
+            hintText=hintText,
+            filters=['none', 'incomplete', 'available'],
+            filter_callback=myfilter
         )
 
         
         if results.text:
             if results.text.isdigit():
                 return self.session_items[len(self.session_items)-int(results.text)]
             return results.text
 
-        if results.selectedPos is None:
+        if results.realSelectedPos is None:
             raise Exception('Invalid position')
 
-        return self.session_items[results.selectedPos]
+        return self.session_items[results.realSelectedPos]
```

### Comparing `goyabu-cli-1.0.8/goyabucli/translation.py` & `goyabu-cli-1.0.9/goyabucli/translation.py`

 * *Files identical despite different names*

### Comparing `goyabu-cli-1.0.8/goyabucli/utils.py` & `goyabu-cli-1.0.9/goyabucli/utils.py`

 * *Files identical despite different names*

### Comparing `goyabu-cli-1.0.8/pyproject.toml` & `goyabu-cli-1.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name="goyabu-cli"
-version="1.0.8"
+version="1.0.9"
 license = { file = "LICENSE" }
 readme = "README.md"
 authors=[{ name = "AlanJS26", email = "alanjoses.29@gmail.com" }]
 description="quickly play anime from terminal"
 keywords = ["python", "cli", "anime"]
 requires-python = ">=3.6"
```

