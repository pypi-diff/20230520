# Comparing `tmp/mov_cli-1.3.9.tar.gz` & `tmp/mov_cli-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mov_cli-1.3.9.tar", max compression
+gzip compressed data, was "mov_cli-1.4.0.tar", max compression
```

## Comparing `mov_cli-1.3.9.tar` & `mov_cli-1.4.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0    35149 2023-05-19 19:35:19.953831 mov_cli-1.3.9/LICENSE
--rw-r--r--   0        0        0     7098 2023-05-19 19:35:19.953831 mov_cli-1.3.9/README.md
--rw-r--r--   0        0        0        0 2023-05-19 19:35:19.953831 mov_cli-1.3.9/mov_cli/__init__.py
--rw-r--r--   0        0        0     2701 2023-05-19 19:35:19.953831 mov_cli-1.3.9/mov_cli/__main__.py
--rw-r--r--   0        0        0        1 2023-05-19 19:35:19.953831 mov_cli-1.3.9/mov_cli/extractors/__init__.py
--rw-r--r--   0        0        0      823 2023-05-19 19:35:19.953831 mov_cli-1.3.9/mov_cli/extractors/doodstream.py
--rw-r--r--   0        0        0       71 2023-05-19 19:35:19.953831 mov_cli-1.3.9/mov_cli/extractors/scdn/NOTICE
--rw-r--r--   0        0        0        1 2023-05-19 19:35:19.953831 mov_cli-1.3.9/mov_cli/extractors/scdn/__init__.py
--rw-r--r--   0        0        0      169 2023-05-19 19:35:19.953831 mov_cli-1.3.9/mov_cli/extractors/scdn/allsportsdaily.py
--rw-r--r--   0        0        0      957 2023-05-19 19:35:19.953831 mov_cli-1.3.9/mov_cli/extractors/scdn/cr7sports.py
--rw-r--r--   0        0        0      256 2023-05-19 19:35:19.953831 mov_cli-1.3.9/mov_cli/extractors/scdn/enjoy4hd.py
--rw-r--r--   0        0        0      141 2023-05-19 19:35:19.953831 mov_cli-1.3.9/mov_cli/extractors/scdn/fabtech.py
--rw-r--r--   0        0        0      218 2023-05-19 19:35:19.953831 mov_cli-1.3.9/mov_cli/extractors/scdn/gameshdlive.py
--rw-r--r--   0        0        0      455 2023-05-19 19:35:19.953831 mov_cli-1.3.9/mov_cli/extractors/scdn/livestreames.py
--rw-r--r--   0        0        0      318 2023-05-19 19:35:19.953831 mov_cli-1.3.9/mov_cli/extractors/scdn/methstreams.py
--rw-r--r--   0        0        0      156 2023-05-19 19:35:19.953831 mov_cli-1.3.9/mov_cli/extractors/scdn/motornews.py
--rw-r--r--   0        0        0      873 2023-05-19 19:35:19.953831 mov_cli-1.3.9/mov_cli/extractors/scdn/onestream.py
--rw-r--r--   0        0        0      891 2023-05-19 19:35:19.953831 mov_cli-1.3.9/mov_cli/extractors/scdn/onionlive.py
--rw-r--r--   0        0        0      615 2023-05-19 19:35:19.953831 mov_cli-1.3.9/mov_cli/extractors/scdn/onionstream.py
--rw-r--r--   0        0        0      457 2023-05-19 19:35:19.953831 mov_cli-1.3.9/mov_cli/extractors/scdn/poscitech.py
--rw-r--r--   0        0        0      638 2023-05-19 19:35:19.953831 mov_cli-1.3.9/mov_cli/extractors/scdn/rainostreams.py
--rw-r--r--   0        0        0      358 2023-05-19 19:35:19.953831 mov_cli-1.3.9/mov_cli/extractors/scdn/ripple.py
--rw-r--r--   0        0        0      406 2023-05-19 19:35:19.957831 mov_cli-1.3.9/mov_cli/extractors/scdn/techclips.py
--rw-r--r--   0        0        0      417 2023-05-19 19:35:19.957831 mov_cli-1.3.9/mov_cli/extractors/scdn/techstips.py
--rw-r--r--   0        0        0     1333 2023-05-19 19:35:19.957831 mov_cli-1.3.9/mov_cli/extractors/scdn/weakstream.py
--rw-r--r--   0        0        0        0 2023-05-19 19:35:19.957831 mov_cli-1.3.9/mov_cli/players/__init__.py
--rw-r--r--   0        0        0     2238 2023-05-19 19:35:19.957831 mov_cli-1.3.9/mov_cli/players/player.py
--rw-r--r--   0        0        0        0 2023-05-19 19:35:19.957831 mov_cli-1.3.9/mov_cli/utils/__init__.py
--rw-r--r--   0        0        0     1481 2023-05-19 19:35:19.957831 mov_cli-1.3.9/mov_cli/utils/dbs.py
--rw-r--r--   0        0        0     2731 2023-05-19 19:35:19.957831 mov_cli-1.3.9/mov_cli/utils/httpclient.py
--rw-r--r--   0        0        0     6133 2023-05-19 19:35:19.957831 mov_cli-1.3.9/mov_cli/utils/jsunpack.py
--rw-r--r--   0        0        0     2269 2023-05-19 19:35:19.957831 mov_cli-1.3.9/mov_cli/utils/lang.py
--rw-r--r--   0        0        0     1592 2023-05-19 19:35:19.957831 mov_cli-1.3.9/mov_cli/utils/player.py
--rw-r--r--   0        0        0      941 2023-05-19 19:35:19.957831 mov_cli-1.3.9/mov_cli/utils/provider.py
--rw-r--r--   0        0        0     8712 2023-05-19 19:35:19.957831 mov_cli-1.3.9/mov_cli/utils/scraper.py
--rw-r--r--   0        0        0        0 2023-05-19 19:35:19.957831 mov_cli-1.3.9/mov_cli/websites/__init__.py
--rw-r--r--   0        0        0    11008 2023-05-19 19:35:19.957831 mov_cli-1.3.9/mov_cli/websites/actvid.py
--rw-r--r--   0        0        0     4169 2023-05-19 19:35:19.957831 mov_cli-1.3.9/mov_cli/websites/animefox.py
--rw-r--r--   0        0        0     4103 2023-05-19 19:35:19.957831 mov_cli-1.3.9/mov_cli/websites/dopebox.py
--rw-r--r--   0        0        0     1941 2023-05-19 19:35:19.957831 mov_cli-1.3.9/mov_cli/websites/einthusan.py
--rw-r--r--   0        0        0     1723 2023-05-19 19:35:19.957831 mov_cli-1.3.9/mov_cli/websites/eja.py
--rw-r--r--   0        0        0     3011 2023-05-19 19:35:19.957831 mov_cli-1.3.9/mov_cli/websites/gogoanime.py
--rw-r--r--   0        0        0     7119 2023-05-19 19:35:19.957831 mov_cli-1.3.9/mov_cli/websites/kinox.py
--rw-r--r--   0        0        0     3733 2023-05-19 19:35:19.957831 mov_cli-1.3.9/mov_cli/websites/kisscartoon.py
--rw-r--r--   0        0        0     2506 2023-05-19 19:35:19.957831 mov_cli-1.3.9/mov_cli/websites/openloadmov.py
--rw-r--r--   0        0        0     2560 2023-05-19 19:35:19.957831 mov_cli-1.3.9/mov_cli/websites/redundant_kimcartoon.py
--rw-r--r--   0        0        0     4656 2023-05-19 19:35:19.957831 mov_cli-1.3.9/mov_cli/websites/remotestream.py
--rw-r--r--   0        0        0     4421 2023-05-19 19:35:19.957831 mov_cli-1.3.9/mov_cli/websites/scdn.py
--rw-r--r--   0        0        0     4112 2023-05-19 19:35:19.957831 mov_cli-1.3.9/mov_cli/websites/sflix.py
--rw-r--r--   0        0        0     1619 2023-05-19 19:35:19.957831 mov_cli-1.3.9/mov_cli/websites/solar.py
--rw-r--r--   0        0        0     2130 2023-05-19 19:35:19.957831 mov_cli-1.3.9/mov_cli/websites/streamblasters.py
--rw-r--r--   0        0        0     1356 2023-05-19 19:35:19.957831 mov_cli-1.3.9/mov_cli/websites/tamilyogi.py
--rw-r--r--   0        0        0     2892 2023-05-19 19:35:19.957831 mov_cli-1.3.9/mov_cli/websites/turkish123.py
--rw-r--r--   0        0        0     4509 2023-05-19 19:35:19.957831 mov_cli-1.3.9/mov_cli/websites/viewasian.py
--rw-r--r--   0        0        0     3390 2023-05-19 19:35:19.957831 mov_cli-1.3.9/mov_cli/websites/watchasian.py
--rw-r--r--   0        0        0     3977 2023-05-19 19:35:19.957831 mov_cli-1.3.9/mov_cli/websites/wlext.py
--rw-r--r--   0        0        0     3499 2023-05-19 19:35:19.957831 mov_cli-1.3.9/mov_cli/websites/yoturkish.py
--rw-r--r--   0        0        0      743 2023-05-19 19:35:19.957831 mov_cli-1.3.9/pyproject.toml
--rw-r--r--   0        0        0     8093 1970-01-01 00:00:00.000000 mov_cli-1.3.9/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-19 23:35:55.147552 mov_cli-1.4.0/LICENSE
+-rw-r--r--   0        0        0     7098 2023-05-19 23:35:55.147552 mov_cli-1.4.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-19 23:35:55.147552 mov_cli-1.4.0/mov_cli/__init__.py
+-rw-r--r--   0        0        0     2701 2023-05-19 23:35:55.147552 mov_cli-1.4.0/mov_cli/__main__.py
+-rw-r--r--   0        0        0        1 2023-05-19 23:35:55.147552 mov_cli-1.4.0/mov_cli/extractors/__init__.py
+-rw-r--r--   0        0        0      823 2023-05-19 23:35:55.147552 mov_cli-1.4.0/mov_cli/extractors/doodstream.py
+-rw-r--r--   0        0        0       71 2023-05-19 23:35:55.147552 mov_cli-1.4.0/mov_cli/extractors/scdn/NOTICE
+-rw-r--r--   0        0        0        1 2023-05-19 23:35:55.147552 mov_cli-1.4.0/mov_cli/extractors/scdn/__init__.py
+-rw-r--r--   0        0        0      169 2023-05-19 23:35:55.147552 mov_cli-1.4.0/mov_cli/extractors/scdn/allsportsdaily.py
+-rw-r--r--   0        0        0      958 2023-05-19 23:35:55.147552 mov_cli-1.4.0/mov_cli/extractors/scdn/cr7sports.py
+-rw-r--r--   0        0        0      256 2023-05-19 23:35:55.147552 mov_cli-1.4.0/mov_cli/extractors/scdn/enjoy4hd.py
+-rw-r--r--   0        0        0      141 2023-05-19 23:35:55.147552 mov_cli-1.4.0/mov_cli/extractors/scdn/fabtech.py
+-rw-r--r--   0        0        0      218 2023-05-19 23:35:55.147552 mov_cli-1.4.0/mov_cli/extractors/scdn/gameshdlive.py
+-rw-r--r--   0        0        0      457 2023-05-19 23:35:55.147552 mov_cli-1.4.0/mov_cli/extractors/scdn/livestreames.py
+-rw-r--r--   0        0        0      318 2023-05-19 23:35:55.147552 mov_cli-1.4.0/mov_cli/extractors/scdn/methstreams.py
+-rw-r--r--   0        0        0      156 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/extractors/scdn/motornews.py
+-rw-r--r--   0        0        0      873 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/extractors/scdn/onestream.py
+-rw-r--r--   0        0        0      891 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/extractors/scdn/onionlive.py
+-rw-r--r--   0        0        0      615 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/extractors/scdn/onionstream.py
+-rw-r--r--   0        0        0      457 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/extractors/scdn/poscitech.py
+-rw-r--r--   0        0        0      638 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/extractors/scdn/rainostreams.py
+-rw-r--r--   0        0        0      358 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/extractors/scdn/ripple.py
+-rw-r--r--   0        0        0      406 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/extractors/scdn/techclips.py
+-rw-r--r--   0        0        0      417 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/extractors/scdn/techstips.py
+-rw-r--r--   0        0        0     1333 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/extractors/scdn/weakstream.py
+-rw-r--r--   0        0        0        0 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/players/__init__.py
+-rw-r--r--   0        0        0     2238 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/players/player.py
+-rw-r--r--   0        0        0        0 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/utils/__init__.py
+-rw-r--r--   0        0        0     1483 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/utils/dbs.py
+-rw-r--r--   0        0        0     2731 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/utils/httpclient.py
+-rw-r--r--   0        0        0     6133 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/utils/jsunpack.py
+-rw-r--r--   0        0        0     2269 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/utils/lang.py
+-rw-r--r--   0        0        0     1592 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/utils/player.py
+-rw-r--r--   0        0        0      941 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/utils/provider.py
+-rw-r--r--   0        0        0     8714 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/utils/scraper.py
+-rw-r--r--   0        0        0        0 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/websites/__init__.py
+-rw-r--r--   0        0        0    11020 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/websites/actvid.py
+-rw-r--r--   0        0        0     4177 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/websites/animefox.py
+-rw-r--r--   0        0        0     4112 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/websites/dopebox.py
+-rw-r--r--   0        0        0     1943 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/websites/einthusan.py
+-rw-r--r--   0        0        0     1724 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/websites/eja.py
+-rw-r--r--   0        0        0     3016 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/websites/gogoanime.py
+-rw-r--r--   0        0        0     7122 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/websites/kinox.py
+-rw-r--r--   0        0        0     3736 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/websites/kisscartoon.py
+-rw-r--r--   0        0        0     2509 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/websites/openloadmov.py
+-rw-r--r--   0        0        0     2563 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/websites/redundant_kimcartoon.py
+-rw-r--r--   0        0        0     4662 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/websites/remotestream.py
+-rw-r--r--   0        0        0     4422 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/websites/scdn.py
+-rw-r--r--   0        0        0     4121 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/websites/sflix.py
+-rw-r--r--   0        0        0     1622 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/websites/solar.py
+-rw-r--r--   0        0        0     2132 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/websites/streamblasters.py
+-rw-r--r--   0        0        0     1358 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/websites/tamilyogi.py
+-rw-r--r--   0        0        0     2895 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/websites/turkish123.py
+-rw-r--r--   0        0        0     4516 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/websites/viewasian.py
+-rw-r--r--   0        0        0     3395 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/websites/watchasian.py
+-rw-r--r--   0        0        0     3983 2023-05-19 23:35:55.151552 mov_cli-1.4.0/mov_cli/websites/wlext.py
+-rw-r--r--   0        0        0     3503 2023-05-19 23:35:55.155552 mov_cli-1.4.0/mov_cli/websites/yoturkish.py
+-rw-r--r--   0        0        0      743 2023-05-19 23:35:55.155552 mov_cli-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     8093 1970-01-01 00:00:00.000000 mov_cli-1.4.0/PKG-INFO
```

### Comparing `mov_cli-1.3.9/LICENSE` & `mov_cli-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mov_cli-1.3.9/README.md` & `mov_cli-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `mov_cli-1.3.9/mov_cli/__main__.py` & `mov_cli-1.4.0/mov_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.3.9/mov_cli/extractors/doodstream.py` & `mov_cli-1.4.0/mov_cli/extractors/doodstream.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.3.9/mov_cli/extractors/scdn/cr7sports.py` & `mov_cli-1.4.0/mov_cli/extractors/scdn/cr7sports.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     r2 = httpx.get(iframe).text
     iframe2 = re.findall(r"iframe src=\"(.*?)\"", r2)[0]
     r3 = httpx.get(iframe2, headers={"referer": "https://sportsembed.su/"}).text
     re_js = jsunpack.unpack(
         re.compile(r"(eval\(function\(p,a,c,k,e,d\).+?{}\)\))").findall(r3)[0]
     )
     m3u8 = re.findall(r"src=\"(.*?)\"", re_js)[0]
-    # soup = BeautifulSoup(r, 'self.parser')
+    # soup = BeautifulSoup(r, 'self.scraper')
     # iframe = soup.iframe
     # src = iframe['src']
     # r_src = httpx.get(src).text
     # fid = re.findall(r"t>fid='(.*?)'", r_src)[0]
     # n = re.findall(r"embed(.*?).j", r_src)[0]
     # php = f"https://vikistream.com/embed{n}.php?player=desktop&live={fid}"
     # r_php = httpx.get(php).text
```

### Comparing `mov_cli-1.3.9/mov_cli/extractors/scdn/onestream.py` & `mov_cli-1.4.0/mov_cli/extractors/scdn/onestream.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.3.9/mov_cli/extractors/scdn/onionlive.py` & `mov_cli-1.4.0/mov_cli/extractors/scdn/onionlive.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.3.9/mov_cli/extractors/scdn/onionstream.py` & `mov_cli-1.4.0/mov_cli/extractors/scdn/onionstream.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.3.9/mov_cli/extractors/scdn/rainostreams.py` & `mov_cli-1.4.0/mov_cli/extractors/scdn/rainostreams.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.3.9/mov_cli/extractors/scdn/weakstream.py` & `mov_cli-1.4.0/mov_cli/extractors/scdn/weakstream.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.3.9/mov_cli/players/player.py` & `mov_cli-1.4.0/mov_cli/players/player.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.3.9/mov_cli/utils/dbs.py` & `mov_cli-1.4.0/mov_cli/utils/dbs.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,22 +30,22 @@
     return title, img
 
 
 def get_season_seasons(tmdb_id: str, name: str) -> int:
     req = httpx.get(
         f"https://www.themoviedb.org/tv/{tmdb_id}-{parse(name)}/seasons"
     ).text
-    rem = BS(req, self.parser)
+    rem = BS(req, self.scraper)
     seasons = [i.text for i in rem.select(".flex > div.season_wrapper")]
     return len(seasons)
 
 
 def get_season_episodes(tmdb_id: str, name: str, season_number: str) -> int:
     req = httpx.get(
         f"https://www.themoviedb.org/tv/{tmdb_id}-{parse(name)}/season/{season_number}"
     ).text
-    episodes = int(BS(req, self.parser).select_one(".episode_sort.space > span").text)
+    episodes = int(BS(req, self.scraper).select_one(".episode_sort.space > span").text)
     return episodes
 
 
 def parse(text: str) -> str:
     return re.sub(r"\W+", "-", text.lower())
```

### Comparing `mov_cli-1.3.9/mov_cli/utils/httpclient.py` & `mov_cli-1.4.0/mov_cli/utils/httpclient.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.3.9/mov_cli/utils/jsunpack.py` & `mov_cli-1.4.0/mov_cli/utils/jsunpack.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.3.9/mov_cli/utils/lang.py` & `mov_cli-1.4.0/mov_cli/utils/lang.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.3.9/mov_cli/utils/player.py` & `mov_cli-1.4.0/mov_cli/utils/player.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.3.9/mov_cli/utils/provider.py` & `mov_cli-1.4.0/mov_cli/utils/provider.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.3.9/mov_cli/utils/scraper.py` & `mov_cli-1.4.0/mov_cli/utils/scraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         pass
 
     def parser(self):
         try:
             import lxml
             return "lxml"
         except ModuleNotFoundError:
-            return self.parser
+            return "html.parser"
         
     @staticmethod
     def parse(txt: str) -> str:
         return re.sub(r"\W+", "-", txt.lower())
 
     def dl(
         self,
```

### Comparing `mov_cli-1.3.9/mov_cli/websites/actvid.py` & `mov_cli-1.4.0/mov_cli/websites/actvid.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
     """def key_num(self, iframe_link: str) -> tuple:
         self.client.add_elem(
             {"Referer": self.base_url}
         )  # adding referer to the headers
         # self.client.headers['Referer'] = self.base_url
         req = self.client.get(iframe_link).text
-        soup = BS(req, self.parser)
+        soup = BS(req, self.scraper)
         k = list([i.text for i in soup.find_all("script")][-3].replace("var", ""))
         key, num = "".join(k[21:61]), k[-3]
         return key, num  # returns a tuple
 
     def auth_token(self, key: str) -> str:
         self.client.add_elem({"Referer": self.base_url})
         self.client.add_elem({"cacheTime": "0"})  # adding referer to the headers
@@ -50,15 +50,15 @@
         )
         s = r.text.replace("/* PLEASE DO NOT COPY AND PASTE THIS CODE. */", "")
         s = s.split(";")
         v_token = s[10].replace("po.src=", "").split("/")[-2]
         r = self.client.get(
             f"https://www.google.com/recaptcha/api2/anchor?ar=1&hl=en&size=invisible&cb=xxmovclix&k={key}&co={self.rab_domain}&v={v_token}"
         ).text
-        soup = BS(r, self.parser)
+        soup = BS(r, self.scraper)
         recap_token = [i["value"] for i in soup.select("#recaptcha-token")][0]
         data = {
             "v": v_token,
             "k": self.rep_key,
             "c": recap_token,
             "co": self.rab_domain,
             "sa": "",
@@ -73,15 +73,15 @@
 
     def search(self, q: str = None) -> str:
         q = input(f"[!] {self.translated[self.task]}") if q is None else q
         self.userinput = q
         return self.client.get(f"{self.base_url}/search/{self.parse(q)}").text
 
     def results(self, html: str) -> list:
-        soup = BS(html, self.parser)
+        soup = BS(html, self.scraper)
         urls = [i["href"] for i in soup.select(".film-poster-ahref")]
         mov_or_tv = [
             "MOVIE" if i["href"].__contains__("/movie/") else "TV"
             for i in soup.select(".film-poster-ahref")
         ]
         title = [
             re.sub(
@@ -92,30 +92,30 @@
             for i in urls
         ]
         ids = [i.split("-")[-1] for i in urls]
         return [list(sublist) for sublist in zip(title, urls, ids, mov_or_tv)]
 
     def ask(self, series_id: str) -> tuple:
         r = self.client.get(f"{self.base_url}/ajax/v2/tv/seasons/{series_id}")
-        season_ids = [i["data-id"] for i in BS(r, self.parser).select(".dropdown-item")]
+        season_ids = [i["data-id"] for i in BS(r, self.scraper).select(".dropdown-item")]
         season = self.askseason(len(season_ids))
         z = f"{self.base_url}/ajax/v2/season/episodes/{season_ids[int(season) - 1]}"
         rf = self.client.get(z)
-        episodes = [i["data-id"] for i in BS(rf, self.parser).select(".nav-item > a")]
+        episodes = [i["data-id"] for i in BS(rf, self.scraper).select(".nav-item > a")]
         episode = episodes[int(self.askepisode(len(episodes))) - 1]
         ep = self.getep(
             url=f"{self.base_url}/ajax/v2/season/episodes/{season_ids[int(season) - 1]}",
             data_id=f"{episode}",
         )
         return episode, season, ep
 
     def getep(self, url, data_id):
         source = self.client.get(f"{url}").text
 
-        soup = BS(source, self.parser)
+        soup = BS(source, self.scraper)
 
         unformated = soup.find("a", {"data-id": f"{data_id}"})["title"]
 
         formated = unformated.split("Eps")[1]
         formated = formated.split(":")[0]
 
         return formated
@@ -162,22 +162,22 @@
         if link.endswith("==") or link.endswith("="):
             n = json.loads(self.decrypt(data["sources"], self.gh_key()))
             return n[0]["file"]
         return source[0]["file"]
 
     def server_id(self, mov_id: str) -> str:
         req = self.client.get(f"{self.base_url}/ajax/movie/episodes/{mov_id}")
-        soup = BS(req, self.parser)
+        soup = BS(req, self.scraper)
         return [i["data-linkid"] for i in soup.select(".nav-item > a")][0]
 
     def ep_server_id(self, ep_id: str) -> str:
         req = self.client.get(
             f"{self.base_url}/ajax/v2/episode/servers/{ep_id}/#servers-list"
         )
-        soup = BS(req, self.parser)
+        soup = BS(req, self.scraper)
         return [i["data-id"] for i in soup.select(".nav-item > a")][0]
 
     def get_link(self, thing_id: str) -> tuple:
         req = self.client.get(f"{self.base_url}/ajax/get_link/{thing_id}").json()[
             "link"
         ]
         print(req)
@@ -226,34 +226,34 @@
         dec_key = k[:32]
         iv = k[32:]
         p = AES.new(dec_key, AES.MODE_CBC, iv=iv).decrypt(base64.b64decode(data)[16:])
         return self.unpad(p).decode()
 
     def ds(self, series_id: str, name):
         r = self.client.get(f"{self.base_url}/ajax/v2/tv/seasons/{series_id}")
-        season_ids = [i["data-id"] for i in BS(r, self.parser).select(".dropdown-item")]
+        season_ids = [i["data-id"] for i in BS(r, self.scraper).select(".dropdown-item")]
         season = self.askseason(len(season_ids))
         z = f"{self.base_url}/ajax/v2/season/episodes/{season_ids[int(season) - 1]}"
         rf = self.client.get(z)
-        episodes = [i["data-id"] for i in BS(rf, self.parser).select(".nav-item > a")]
+        episodes = [i["data-id"] for i in BS(rf, self.scraper).select(".nav-item > a")]
         for e in range(len(episodes)):
             episode = episodes[e]
             sid = self.ep_server_id(episode)
             iframe_url, tv_id = self.get_link(sid)
             iframe_link, iframe_id = self.rabbit_id(iframe_url)
             url = self.cdn_url(iframe_link, iframe_id)
             self.dl(url, name, season=season, episode=e + 1)
 
     def sd(self, series_id: str, name):
         r = self.client.get(f"{self.base_url}/ajax/v2/tv/seasons/{series_id}")
-        season_ids = [i["data-id"] for i in BS(r, self.parser).select(".dropdown-item")]
+        season_ids = [i["data-id"] for i in BS(r, self.scraper).select(".dropdown-item")]
         for s in range(len(season_ids)):
             z = f"{self.base_url}/ajax/v2/season/episodes/{season_ids[s]}"
             rf = self.client.get(z)
-            episodes = [i["data-id"] for i in BS(rf, self.parser).select(".nav-item > a")]
+            episodes = [i["data-id"] for i in BS(rf, self.scraper).select(".nav-item > a")]
             for e in range(len(episodes)):
                 episode = episodes[e]
                 sid = self.ep_server_id(episode)
                 iframe_url, tv_id = self.get_link(sid)
                 iframe_link, iframe_id = self.rabbit_id(iframe_url)
                 url = self.cdn_url(iframe_link, iframe_id)
                 self.dl(url, name, season=s + 1, episode=e + 1)
```

### Comparing `mov_cli-1.3.9/mov_cli/websites/animefox.py` & `mov_cli-1.4.0/mov_cli/websites/viewasian.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,108 +1,104 @@
-from ..utils.scraper import WebScraper
 from bs4 import BeautifulSoup as BS
+from ..utils.scraper import WebScraper
 import re
 
 
-class animefox(WebScraper):
+class viewasian(WebScraper):
     def __init__(self, base_url):
         super().__init__(base_url)
         self.base_url = base_url
 
-    def search(self, q: str = None) -> str:
+    def search(self, q: str):
         q = input(f"[!] {self.translated[self.task]}") if q is None else q
-        return q.replace(" ", "+")
+        return q.replace(" ", "-")
 
-    def results(self, data: str) -> list:
-        req = self.client.get(f"https://animefox.to/search?keyword={data}")
-        soup = BS(req, self.parser)
-        items = soup.findAll("a", {"class": "film-poster-ahref"})
-        urls = [items[i]["href"] for i in range(len(items))]
-        title = [items[i]["title"] for i in range(len(items))]
-        ids = [i for i in range(len(items))]
-        mov_or_tv = [
-            "MOVIE" if items[i].__contains__("Movie") else "TV"
-            for i in range(len(items))
-        ]
+    def results(self, data: str):
+        request = self.client.get(f"{self.base_url}/movie/search/{data}")
+        soup = BS(request, self.scraper)
+        streams = soup.findAll("a", {"class": "ml-mask jt"})
+        urls = [streams[i]["href"] for i in range(len(streams))]
+        title = [streams[i]["title"] for i in range(len(streams))]
+        ids = [streams[i]["class"] for i in range(len(streams))]
+        mov_or_tv = ["TV" for i in range(len(streams))]
         return [list(sublist) for sublist in zip(title, urls, ids, mov_or_tv)]
 
     def ask(self, url):
-        a = self.client.get(f"{self.base_url}{url}")
-        soup = BS(a, self.parser)
-        url = soup.find("div", {"class": "film-buttons"}).find("a")["href"]
-        req = self.client.get(self.base_url + url)
-        soup = BS(req, self.parser)
-        episodes = len(soup.find("div", {"id": "episodes-page-1"}).findAll("a"))
-        episode = self.askepisode(episodes)
-        return self.base_url + url[:-1] + episode, episode
-
-    def mov(self, url):
-        a = self.client.get(f"{self.base_url}{url}")
-        soup = BS(a, self.parser)
-        url = soup.find("div", {"class": "film-buttons"}).find("a")["href"]
-        return self.base_url + url
-
-    def cdn_url(self, url):
-        req = self.client.get(url)
-        soup = BS(req, self.parser)
-        goload = soup.find("select", {"id": "select-iframe-to-display"}).findAll(
-            "option"
-        )[-1]["value"]
-        url = f"https://{goload}".split("-")[0]
-        a = self.client.head(url, redirects=False).headers["location"]
-        a = self.client.get(a)
-        soup = BS(a, self.parser)
-        server = []
-        servers = soup.findAll("li", {"class": "linkserver"})
-        for video in servers:
-            if "dood.wf" in str(video["data-video"]):
-                server.append(video["data-video"])
-        return self.doodstream(server[0])
-
-    def doodstream(self, url):
-        domain = re.findall("""([^"']*)\/e""", url)[0]
-        req = self.client.get(url).text
-        pass_md = re.findall(r"/pass_md5/[^']*", req)[0]
-        token = pass_md.split("/")[-1]
-        self.client.set_headers(
-            {
-                "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:108.0) Gecko/20100101 Firefox/108.0",
-                "Referer": f"{url}",
-                "Accept-Language": "en-GB,en;q=0.5",
-            }
-        )
-        drylink = self.client.get(f"{domain}{pass_md}").text
-        streamlink = f"{drylink}zUEJeL3mUN?token={token}"
-        print(streamlink)
-        return streamlink
+        request = self.client.get(f"{self.base_url}{url}")
+        soup = BS(request, self.scraper)
+        href = soup.find("a", {"class": "bwac-btn"})["href"]
+        request = self.client.get(f"{self.base_url}{href}")
+        soup = BS(request, self.scraper)
+        episodes = soup.findAll("li", {"class": "ep-item"})
+        episode = int(self.askepisode(len(episodes)))
+        request = self.client.get(f"{self.base_url}{href}?ep={episode}").text
+        soup = BS(request, self.scraper)
+        if re.search("doodstream", request):
+            dood = soup.find("li", {"class": "doodstream"})["data-video"]
+            li = self.doodstream(dood)
+        elif re.search("streamtape", request):
+            streamtape = soup.find("li", {"class": "streamtape"})["data-video"]
+            li = self.streamtape(streamtape)
+        else:
+            raise Exception("Unable to find URL")
+        return li, episode
+
+    def streamtape(self, url):
+        string = re.findall("""v\/([^"']*)\/""", url)[0]
+        request = self.client.get(f"https://streamtape.com/e/{string}").text
+        if '<h1 class="white">Video not found!</h1>' not in request:
+            regex = r"""'robotlink'\)\.innerHTML = '(.*?)'\+ \('(.*?)'\)"""
+            results = re.findall(regex, request)
+            for tuple in results:
+                url = tuple[0]
+                rest = tuple[1]
+            li = f"https:{url}{rest[3:]}"
+            return li
+        raise Exception("Video not found or removed")
+
+    #    def doodstream(self, url):
+    #        domain = re.findall("""([^"']*)\/e""", url)[0]
+    #        req = self.client.get(url).text
+    #        pass_md = re.findall(r"/pass_md5/[^']*", req)[0]
+    #        token = pass_md.split("/")[-1]
+    #        self.client.set_headers(
+    #            {
+    #                "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:108.0) Gecko/20100101 Firefox/108.0",
+    #                "Referer": f"{url}",
+    #                "Accept-Language": "en-GB,en;q=0.5",
+    #            }
+    #        )
+    #        drylink = self.client.get(f"{domain}{pass_md}").text
+    #        streamlink = f"{drylink}zUEJeL3mUN?token={token}"
+    #        print(streamlink)
+    #        return streamlink
 
     def download(self, t):
-        a = self.client.get(f"{self.base_url}{t[self.url]}")
-        soup = BS(a, self.parser)
-        url = soup.find("div", {"class": "film-buttons"}).find("a")["href"]
-        req = self.client.get(self.base_url + url)
-        soup = BS(req, self.parser)
-        episodes = len(soup.find("div", {"id": "episodes-page-1"}).findAll("a"))
-        for e in range(episodes):
-            url = self.cdn_url(self.base_url + url[:-1] + e + 1)
-            self.dl(url, name=t[self.title], episode=e + 1)
+        request = self.client.get(f"{self.base_url}{t[self.url]}")
+        soup = BS(request, self.scraper)
+        href = soup.find("a", {"class": "bwac-btn"})["href"]
+        request = self.client.get(f"{self.base_url}{href}")
+        soup = BS(request, self.scraper)
+        episodes = soup.findAll("li", {"class": "ep-item"})
+        for e in range(len(episodes)):
+            request = self.client.get(f"{self.base_url}{href}?ep={e+1}").text
+            soup = BS(request, self.scraper)
+            if re.search("doodstream", request):
+                dood = soup.find("li", {"class": "doodstream"})["data-video"]
+                li = self.doodstream(dood)
+            elif re.search("streamtape", request):
+                streamtape = soup.find("li", {"class": "streamtape"})["data-video"]
+                li = self.streamtape(streamtape)
+            else:
+                raise Exception("Unable to find URL")
+            self.dl(li, t[self.title], episode=e + 1)
 
     def TV_PandDP(self, t: list, state: str = "d" or "p" or "sd"):
         if state == "sd":
             self.download(t)
             return
         name = t[self.title]
-        link, episode = self.ask(t[self.url])
-        url = self.cdn_url(link)
+        url, episode = self.ask(t[self.url])
         if state == "d":
             self.dl(url, name, season=".", episode=episode)
             return
         self.play(url, name)
-
-    def MOV_PandDP(self, t: list, state: str = "d" or "p"):
-        name = t[self.title]
-        link = self.mov(t[self.url])
-        url = self.cdn_url(link)
-        if state == "d":
-            self.dl(url, name)
-            return
-        self.play(url, name)
```

### Comparing `mov_cli-1.3.9/mov_cli/websites/dopebox.py` & `mov_cli-1.4.0/mov_cli/websites/dopebox.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,78 +19,78 @@
                 f"https://rabbitstream.net/ajax/embed-4/getSources?id={rabbid}&_token={rose}&_number={num}"
             ).text
         )["sources"][0]["file"]
         return data"""
 
     def ask(self, series_id):
         r = self.client.get(f"{self.base_url}/ajax/v2/tv/seasons/{series_id}")
-        season_ids = [i["data-id"] for i in BS(r, self.parser).select(".dropdown-item")]
+        season_ids = [i["data-id"] for i in BS(r, self.scraper).select(".dropdown-item")]
         season = self.askseason(len(season_ids))
         rf = self.client.get(
             f"{self.base_url}/ajax/v2/season/episodes/{season_ids[int(season) - 1]}"
         )
-        episodes = [i["data-id"] for i in BS(rf, self.parser).select(".episode-item")]
+        episodes = [i["data-id"] for i in BS(rf, self.scraper).select(".episode-item")]
         episode = episodes[int(self.askepisode(len(episodes))) - 1]
         ep = self.getep(
             f"{self.base_url}/ajax/v2/season/episodes/{season_ids[int(season) - 1]}",
             data_id=episode,
         )
         return episode, season, ep
 
     def getep(self, url, data_id):
         source = self.client.get(f"{url}").text
-        soup = BS(source, self.parser)
+        soup = BS(source, self.scraper)
 
         unformated = soup.find("div", {"data-id": f"{data_id}"})
 
         children = unformated.findChildren("div", {"class": "episode-number"})
         for child in children:
             text = child.text
 
         text = text.split("Episode")[1]
         text = text.split(":")[0]
 
         return text
 
     def server_id(self, mov_id):
         rem = self.client.get(f"{self.base_url}/ajax/movie/episodes/{mov_id}")
-        soup = BS(rem, self.parser)
+        soup = BS(rem, self.scraper)
         return [i["data-id"] for i in soup.select(".link-item")][0]
 
     def ep_server_id(self, ep_id):
         rem = self.client.get(
             f"{self.base_url}/ajax/v2/episode/servers/{ep_id}/#servers-list"
         )
-        soup = BS(rem, self.parser)
+        soup = BS(rem, self.scraper)
         return [i["data-id"] for i in soup.select(".link-item")][0]
 
     def ds(self, series_id: str, name):
         r = self.client.get(f"{self.base_url}/ajax/v2/tv/seasons/{series_id}")
-        season_ids = [i["data-id"] for i in BS(r, self.parser).select(".dropdown-item")]
+        season_ids = [i["data-id"] for i in BS(r, self.scraper).select(".dropdown-item")]
         season = self.askseason(len(season_ids))
         rf = self.client.get(
             f"{self.base_url}/ajax/v2/season/episodes/{season_ids[int(season) - 1]}"
         )
-        episodes = [i["data-id"] for i in BS(rf, self.parser).select(".episode-item")]
+        episodes = [i["data-id"] for i in BS(rf, self.scraper).select(".episode-item")]
         for e in range(len(episodes)):
             episode = episodes[e]
             sid = self.ep_server_id(episode)
             iframe_url, tv_id = self.get_link(sid)
             iframe_link, iframe_id = self.rabbit_id(iframe_url)
             url = self.cdn_url(iframe_link, iframe_id)
             self.dl(url, name, season=season, episode=e + 1)
 
     def sd(self, series_id: str, name):
         r = self.client.get(f"{self.base_url}/ajax/v2/tv/seasons/{series_id}")
-        season_ids = [i["data-id"] for i in BS(r, self.parser).select(".dropdown-item")]
+        season_ids = [i["data-id"] for i in BS(r, self.scraper).select(".dropdown-item")]
         for s in range(len(season_ids)):
             rf = self.client.get(
                 f"{self.base_url}/ajax/v2/season/episodes/{season_ids[s]}"
             )
-            episodes = [i["data-id"] for i in BS(rf, self.parser).select(".episode-item")]
+            episodes = [i["data-id"] for i in BS(rf, self.scraper).select(".episode-item")]
             for e in range(len(episodes)):
                 episode = episodes[e]
                 sid = self.ep_server_id(episode)
                 iframe_url, tv_id = self.get_link(sid)
                 iframe_link, iframe_id = self.rabbit_id(iframe_url)
                 url = self.cdn_url(iframe_link, iframe_id)
                 self.dl(url, name, season=s + 1, episode=e + 1)
```

### Comparing `mov_cli-1.3.9/mov_cli/websites/einthusan.py` & `mov_cli-1.4.0/mov_cli/websites/einthusan.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,29 +24,29 @@
             "marathi",
             "punjabi",
         ]
         lang = fzf_prompt(lang)
         req = self.client.get(
             f"{self.base_url}/movie/results/?lang={lang}&query={data}"
         )
-        soup = BS(req, self.parser)
+        soup = BS(req, self.scraper)
         items = soup.findAll("div", {"class": "block2"})
         urls = [items[i].find("a")["href"] for i in range(len(items))]
         title = [
             items[i].find("h3").text + " | " + items[i].find("span").text
             for i in range(len(items))
         ]
         ids = [i for i in range(len(items))]
         mov_or_tv = ["MOVIE" for i in range(len(items))]
         return [list(sublist) for sublist in zip(title, urls, ids, mov_or_tv)]
 
     def cdn_url(self, url):
         domain = "https://cdn4.einthusan.io"
         req = self.client.get(f"{self.base_url}{url}").text
-        soup = BS(req, self.parser)
+        soup = BS(req, self.scraper)
         etv = soup.find("section", {"id": "UIVideoPlayer"})["data-mp4-link"].replace(
             "amp;", ""
         )
         etv = re.findall(r"https:\/\/[^a-z]+(.*)", etv)[0]
         url = f"{domain}/{etv}"
         print(url)
         return url
```

### Comparing `mov_cli-1.3.9/mov_cli/websites/eja.py` & `mov_cli-1.4.0/mov_cli/websites/eja.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         q = input(f"[!] {self.translated[self.task]}") if q is None else q
         return q
 
     def results(self, q: str) -> list:
         q = q.replace(" ", "+")
         self.client.set_headers(self.headers)
         html = self.client.get(f"https://eja.tv/?search={q}").text
-        soup = BS(html, self.parser)
+        soup = BS(html, self.scraper)
         col = soup.findAll("div", {"class": "col-sm-4"})
         urls = [col[i].findAll("a")[1]["href"] for i in range(len(col))]
         title = [col[i].findAll("a")[1].text for i in range(len(col))]
         ids = [col[i].findAll("a")[1]["href"].strip("?") for i in range(len(col))]
         mov_or_tv = [col[i].findAll("img")[0]["alt"] for i in range(len(col))]
         return [list(sublist) for sublist in zip(title, urls, ids, mov_or_tv)]
```

### Comparing `mov_cli-1.3.9/mov_cli/websites/gogoanime.py` & `mov_cli-1.4.0/mov_cli/websites/gogoanime.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,30 +10,30 @@
 
     def search(self, q: str):
         q = input(f"[!] {self.translated[self.task]}") if q is None else q
         return q.replace(" ", "-")
 
     def results(self, data: str) -> list:
         req = self.client.get(f"{self.base_url}/search.html?keyword={data}")
-        soup = BS(req, self.parser)
+        soup = BS(req, self.scraper)
         items = soup.find("ul", {"class": "items"}).findAll("li")
         urls = [items[i].find("a")["href"] for i in range(len(items))]
         title = [items[i].find("a")["title"] for i in range(len(items))]
         ids = [items[i].find("a")["title"] for i in range(len(items))]
         mov_or_tv = ["TV" for i in range(len(items))]
         return [list(sublist) for sublist in zip(title, urls, ids, mov_or_tv)]
 
     def ask(self, url):
         req = self.client.get(f"{self.base_url}{url}")
-        soup = BS(req, self.parser)
+        soup = BS(req, self.scraper)
         episodes = soup.find("ul", {"id": "episode_page"}).find_all("a")[-1]["ep_end"]
         episode = self.askepisode(int(episodes))
         url = url.split("/")[-1]
         request = self.client.get(f"{self.base_url}/{url}-episode-{episode}")
-        soup = BS(request, self.parser)
+        soup = BS(request, self.scraper)
         url = self.doodstream(
             soup.find("li", {"class": "doodstream"}).find("a")["data-video"]
         )
         return url, episode
 
     def doodstream(self, url):
         domain = re.findall("""([^"']*)\/e""", url)[0]
@@ -50,20 +50,20 @@
         drylink = self.client.get(f"{domain}{pass_md}").text
         streamlink = f"{drylink}zUEJeL3mUN?token={token}"
         print(streamlink)
         return streamlink
 
     def download(self, t):
         req = self.client.get(f"{self.base_url}{t[self.url]}")
-        soup = BS(req, self.parser)
+        soup = BS(req, self.scraper)
         episodes = soup.find("ul", {"id": "episode_page"}).find("a")["ep_end"]
         for e in range(len(episodes)):
             url = url.split("/")[-1]
             request = self.client.get(f"{self.base_url}/{url}-episode-{e+1}")
-            soup = BS(request, self.parser)
+            soup = BS(request, self.scraper)
             url = self.doodstream(
                 soup.find("li", {"class": "doodstream"}).find("a")["data-video"]
             )
             self.dl(url, t[self.title], episode=e + 1)
 
     def TV_PandDP(self, t: list, state: str = "d" or "p" or "sd"):
         name = t[self.title]
```

### Comparing `mov_cli-1.3.9/mov_cli/websites/kinox.py` & `mov_cli-1.4.0/mov_cli/websites/kinox.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,15 +36,15 @@
             return "TV"
 
     def results(self, data: str):
         self.base_url = self.client.head(
             "https://kinox.to", redirects=False
         ).headers.get("location")[:-1]
         request = self.client.get(f"{self.base_url}/Search.html?q={data}").text
-        soup = BS(request, self.parser)
+        soup = BS(request, self.scraper)
         streams = soup.find("tbody").findAll("tr")
         urls = [streams[i].find("a")["href"] for i in range(len(streams))]
         title = [self.comp(streams[i]) for i in range(len(streams))]
         ids = [i for i in range(len(streams))]
         mov_or_tv = [self.mov_or_tv(streams[i]) for i in range(len(streams))]
         return [list(sublist) for sublist in zip(title, urls, ids, mov_or_tv)]
 
@@ -115,15 +115,15 @@
                         "location"
                     )
                     return url
         raise Exception("Video not found or removed")
 
     def ask(self, url):
         req = self.client.get(f"{self.base_url}{url}").text
-        soup = BS(req, self.parser)
+        soup = BS(req, self.scraper)
         select = soup.find("select", {"id": "SeasonSelection"}).findAll("option")
         rel = soup.find("select", {"id": "SeasonSelection"})["rel"]
         season = int(self.askseason(len(select)))
         option = select[season - 1]["rel"].split(",")
         episode = int(self.askepisode(len(option)))
         option = option[episode - 1]
         hostlist = self.client.get(
@@ -142,15 +142,15 @@
             url = self.streamz(
                 f"{self.base_url}/aGET/Mirror/{name}&Hoster=88&Season={season}&Episode={option}"
             )
         return url, episode, season
 
     def movie(self, url):
         req = self.client.get(f"{self.base_url}{url}").text
-        BS(req, self.parser)
+        BS(req, self.scraper)
         name = re.findall("\/Stream\/(.*)\.", url)[0]
         try:
             if re.search("Hoster_92", req):
                 url = self.voe(f"{self.base_url}/aGET/Mirror/{name}&Hoster=92")
             elif re.search("Hoster_95", req):
                 url = self.doodstream(f"{self.base_url}/aGET/Mirror/{name}&Hoster=95")
             else:
```

### Comparing `mov_cli-1.3.9/mov_cli/websites/kisscartoon.py` & `mov_cli-1.4.0/mov_cli/websites/kisscartoon.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,43 +13,43 @@
 
     def search(self, q: str = None) -> str:
         q = input(f"[!] {self.translated[self.task]}") if q is None else q
         return q
 
     def results(self, q):
         res = self.client.get(f"{self.base_url}/?s={q}")
-        soup = BS(res.text, self.parser)
+        soup = BS(res.text, self.scraper)
         cartoon_name = [i.text for i in soup.select("div.title > a")]
         urls = [i["href"] for i in soup.select("div.title > a")]
         discrim = [httpx.URL(i).path for i in urls]
         mov_or_tv = [
             i.text for i in soup.select("div.thumbnail.animation-2 > a > span")
         ]
         return [
             list(sublist) for sublist in zip(cartoon_name, urls, discrim, mov_or_tv)
         ]
 
     def ask(self, url):
         res = httpx.get(url).text
-        soup = BS(res, self.parser)
+        soup = BS(res, self.scraper)
         season_id = httpx.URL(soup.find("link", {"rel": "shortlink"})["href"]).params[
             "p"
         ]
         print(season_id)
         try:
             last_page = soup.select("ul.episode_list > li")[-1].text
         except IndexError:
             last_page = 0
         self.client.add_elem({"referer": url})
         self.client.add_elem({"x-requested-with": "XMLHttpRequest"})
         num_eps = BS(
             self.client.get(
                 f"https://thekisscartoon.com/ajax-episode/?page_sele={last_page}&id={season_id}"
             ).text,
-            self.parser,
+            self.scraper,
         )
         num_eps = num_eps.select("div.numerando")[-1].text
         episode = int(self.askepisode(int(num_eps)))
         url = url.strip("/")
         url = f"{url}-episode-{episode}/".replace("tvshows", "episode")
         return url, episode
```

### Comparing `mov_cli-1.3.9/mov_cli/websites/openloadmov.py` & `mov_cli-1.4.0/mov_cli/websites/openloadmov.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,39 +10,39 @@
 
     def search(self, q: str):
         q = input(f"[!] {self.translated[self.task]}") if q is None else q
         return q.replace(" ", "+")
 
     def results(self, data: str) -> list:
         req = self.client.get(f"{self.base_url}/?s={data}")
-        soup = BS(req, self.parser)
+        soup = BS(req, self.scraper)
         items = soup.findAll("div", {"class": "result-item"})
         title = [items[i].find("img")["alt"] for i in range(len(items))]
         urls = [items[i].find("a")["href"] for i in range(len(items))]
         ids = [i for i in range(len(items))]
         mov_or_tv = [
             "MOVIE" if items[i].find("span").text.__contains__("Movie") else "TV"
             for i in range(len(items))
         ]
         return [list(sublist) for sublist in zip(title, urls, ids, mov_or_tv)]
 
     def ask(self, url):
         req = self.client.get(url)
-        soup = BS(req, self.parser)
+        soup = BS(req, self.scraper)
         seasons = soup.findAll("div", {"class": "se-c"})
         season = int(self.askseason(len(seasons)))
         se_c = seasons[season - 1]
         episodes = se_c.find("ul").findAll("li")
         episode = int(self.askepisode(len(episodes)))
         ep = episodes[episode - 1].find("a")["href"]
         return ep, episode, season
 
     def cdn_url(self, url):
         req = self.client.get(url)
-        soup = BS(req, self.parser)
+        soup = BS(req, self.scraper)
         iframe = soup.find("iframe")["src"]
         vidhash = iframe.split("/")[-1]
         self.client.set_headers({"x-requested-with": "XMLHttpRequest"})
         awd = self.client.post(
             self.getvid.format(vidhash),
             data={"hash": vidhash, "r": self.base_url + "/"},
         ).json()["securedLink"]
```

### Comparing `mov_cli-1.3.9/mov_cli/websites/redundant_kimcartoon.py` & `mov_cli-1.4.0/mov_cli/websites/redundant_kimcartoon.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,35 +10,35 @@
 
     def search(self, q: str = None) -> str:
         q = input(f"[!] {self.translated[self.task]}") if q is None else q
         return q
 
     def results(self, q):
         res = self.client.post(f"{self.base_url}/Search/Cartoon", data={"keyword": q})
-        soup = BS(res.text, self.parser)
+        soup = BS(res.text, self.scraper)
         div = soup.find("div", {"class": "list-cartoon"})
         cartoons = div.findAll("div", {"class": "item"})
         title = [cartoons[i].find("span").text for i in range(len(cartoons))]
         urls = [cartoons[i].find("a")["href"] for i in range(len(cartoons))]
         ids = [i for i in range(len(cartoons))]
         mov_or_tv = ["TV" for i in range(len(cartoons))]
         return [list(sublist) for sublist in zip(title, urls, ids, mov_or_tv)]
 
     def ask(self, url):
         res = self.client.get(self.base_url + url)
-        soup = BS(res, self.parser)
+        soup = BS(res, self.scraper)
         table = soup.find("table", {"class": "listing"})
         episodes = table.findAll("a", {"rel": "noreferrer noopener"})
         episode = int(self.askepisode(len(episodes)))
         url = episodes[len(episodes) - episode]["href"]
         return url, episode
 
     def download(self, t: list):
         res = self.client.get(self.base_url + t[self.url])
-        soup = BS(res, self.parser)
+        soup = BS(res, self.scraper)
         table = soup.find("table", {"class": "listing"})
         episodes = table.findAll("a", {"rel": "noreferrer noopener"})
         for e in range(len(episodes)):
             epi = e + 1
             link = episodes[len(episodes) - epi]["href"]
             url = self.cdn_url(link)
             self.dl(url, t[self.title], episode=e + 1)
```

### Comparing `mov_cli-1.3.9/mov_cli/websites/remotestream.py` & `mov_cli-1.4.0/mov_cli/websites/remotestream.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,27 +19,27 @@
         ids = []
         mov_or_tv = []
         tv = self.client.get(self.movdb + f"/search/tv?query={data}&language=en").text
         movie = self.client.get(
             self.movdb + f"/search/movie?query={data}&language=en"
         ).text
         # MOVIE
-        soupm = BS(movie, self.parser)
+        soupm = BS(movie, self.scraper)
         mcards = soupm.findAll("div", {"class": "card v4 tight"})
         if mcards is not []:
             title.extend([mcards[i].find("h2").text for i in range(len(mcards))])
             urls.extend(["" for i in range(len(mcards))])
             ids.extend(
                 [
                     mcards[i].find("a")["href"].split("/")[-1].split("?")[0]
                     for i in range(len(mcards))
                 ]
             )
             mov_or_tv.extend(["MOVIE" for i in range(len(mcards))])
-        soups = BS(tv, self.parser)
+        soups = BS(tv, self.scraper)
         scards = soups.findAll("div", {"class": "card v4 tight"})
         if scards is not []:
             title.extend([scards[i].find("h2").text for i in range(len(scards))])
             urls.extend(["" for i in range(len(scards))])
             ids.extend(
                 [
                     scards[i].find("a")["href"].split("/")[-1].split("?")[0]
@@ -48,28 +48,28 @@
             )
             mov_or_tv.extend(["TV" for i in range(len(scards))])
         return [list(sublist) for sublist in zip(title, urls, ids, mov_or_tv)]
 
     def ask(self, id):
         rlurl = self.client.head(f"{self.movdb}/tv/{id}", redirects=True).url
         res = self.client.get(f"{rlurl}/seasons")
-        soup = BS(res, self.parser)
+        soup = BS(res, self.scraper)
         seasons = soup.findAll("div", {"class": "season"})
         s = []
         for season in seasons:
             title = season.find("h2").find("a").text
             if title == "Extras":
                 continue
             elif title == "Specials":
                 continue
             else:
                 s.append(season)
         season = self.askseason(len(s))
         req = self.client.get(f"{rlurl}/season/{season}").text
-        soup = BS(req, self.parser)
+        soup = BS(req, self.scraper)
         episodes = soup.find("h3", {"class": "episode_sort"}).find("span").text
         episode = self.askepisode(int(episodes))
         return season, episode
 
     def cdn_url(self, id=None, season=None, episode=None):
         if season is None:
             res = self.client.get(f"{self.base_url}/e/?tmdb={id}").text
@@ -83,23 +83,23 @@
             print("This show or movie is not available.")
             exit(1)
         return file
 
     def sd(self, name, id):
         rlurl = self.client.head(f"{self.movdb}/tv/{id}", redirects=True).url
         res = self.client.get(f"{rlurl}/seasons")
-        soup = BS(res, self.parser)
+        soup = BS(res, self.scraper)
         seasons = soup.findAll("div", {"class": "season"})
         for s in range(len(seasons)):
             title = seasons[s].find("h2").find("a").text
             if title == "Extras":
                 pass
             else:
                 req = self.client.get(f"{rlurl}/season/{s+1}").text
-                soup = BS(req, self.parser)
+                soup = BS(req, self.scraper)
                 episodes = soup.find("h3", {"class": "episode_sort"}).find("span").text
                 for e in range(int(episodes)):
                     url = self.cdn_url(id, s + 1, e + 1)
                     self.dl(url, name, season=s + 1, episode=e + 1)
 
     def MOV_PandDP(self, m: list, state: str = "d" or "p"):
         name = m[self.title]
```

### Comparing `mov_cli-1.3.9/mov_cli/websites/scdn.py` & `mov_cli-1.4.0/mov_cli/websites/scdn.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
             raise Exception("No Match was Found that is in progress.")
         return [list(sublist) for sublist in zip(title, urls, ids, mov_or_tv)]
 
     def cdn_url(self, id):
         req = self.client.get(
             f"https://scdn.dev/main-assets/{id}/{self.sport}?origin=sportsurge.club&="
         )
-        soup = BS(req, self.parser)
+        soup = BS(req, self.scraper)
         print(soup.prettify())
         ts = []
         tr = soup.find("tbody").find_all("tr")  #
         for i in range(len(tr)):
             h = self.client.get(tr[i].find("a")["href"]).text
             try:
                 url = re.findall('window.location.href = "(.*?)";', h)[0]
```

### Comparing `mov_cli-1.3.9/mov_cli/websites/sflix.py` & `mov_cli-1.4.0/mov_cli/websites/sflix.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,77 +19,77 @@
                 f"https://rabbitstream.net/ajax/embed-4/getSources?id={rabbid}&_token={rose}&_number={num}"
             ).text
         )["sources"][0]["file"]
         return data"""
 
     def ask(self, series_id):
         r = self.client.get(f"{self.base_url}/ajax/v2/tv/seasons/{series_id}")
-        season_ids = [i["data-id"] for i in BS(r, self.parser).select(".dropdown-item")]
+        season_ids = [i["data-id"] for i in BS(r, self.scraper).select(".dropdown-item")]
         season = self.askseason(len(season_ids))
         rf = self.client.get(
             f"{self.base_url}/ajax/v2/season/episodes/{season_ids[int(season) - 1]}"
         )
-        episodes = [i["data-id"] for i in BS(rf, self.parser).select(".episode-item")]
+        episodes = [i["data-id"] for i in BS(rf, self.scraper).select(".episode-item")]
         episode = episodes[int(self.askepisode(len(episodes))) - 1]
         ep = self.getep(
             f"{self.base_url}/ajax/v2/season/episodes/{season_ids[int(season) - 1]}",
             data_id=episode,
         )
         return episode, season, ep
 
     def getep(self, url, data_id):
         source = self.client.get(f"{url}").text
-        soup = BS(source, self.parser)
+        soup = BS(source, self.scraper)
 
         unformated = soup.find("div", {"data-id": f"{data_id}"})
 
         children = unformated.findChildren("div", {"class": "episode-number"})
         for child in children:
             text = child.text
             text = text.split("Episode")[1]
             text = text.split(":")[0]
 
             return text
 
     def server_id(self, mov_id):
         rem = self.client.get(f"{self.base_url}/ajax/movie/episodes/{mov_id}")
-        soup = BS(rem, self.parser)
+        soup = BS(rem, self.scraper)
         return [i["data-id"] for i in soup.select(".link-item")][0]
 
     def ep_server_id(self, ep_id):
         rem = self.client.get(
             f"{self.base_url}/ajax/v2/episode/servers/{ep_id}/#servers-list"
         )
-        soup = BS(rem, self.parser)
+        soup = BS(rem, self.scraper)
         return [i["data-id"] for i in soup.select(".link-item")][0]
 
     def ds(self, series_id: str, name):
         r = self.client.get(f"{self.base_url}/ajax/v2/tv/seasons/{series_id}")
-        season_ids = [i["data-id"] for i in BS(r, self.parser).select(".dropdown-item")]
+        season_ids = [i["data-id"] for i in BS(r, self.scraper).select(".dropdown-item")]
         season = self.askseason(len(season_ids))
         rf = self.client.get(
             f"{self.base_url}/ajax/v2/season/episodes/{season_ids[int(season) - 1]}"
         )
-        episodes = [i["data-id"] for i in BS(rf, self.parser).select(".episode-item")]
+        episodes = [i["data-id"] for i in BS(rf, self.scraper).select(".episode-item")]
         for e in range(len(episodes)):
             episode = episodes[e]
             sid = self.ep_server_id(episode)
             iframe_url, tv_id = self.get_link(sid)
             iframe_link, iframe_id = self.rabbit_id(iframe_url)
             url = self.cdn_url(iframe_link, iframe_id)
             self.dl(url, name, season=season, episode=e + 1)
 
     def sd(self, series_id: str, name):
         r = self.client.get(f"{self.base_url}/ajax/v2/tv/seasons/{series_id}")
-        season_ids = [i["data-id"] for i in BS(r, self.parser).select(".dropdown-item")]
+        season_ids = [i["data-id"] for i in BS(r, self.scraper).select(".dropdown-item")]
         for s in range(len(season_ids)):
             rf = self.client.get(
                 f"{self.base_url}/ajax/v2/season/episodes/{season_ids[s]}"
             )
-            episodes = [i["data-id"] for i in BS(rf, self.parser).select(".episode-item")]
+            episodes = [i["data-id"] for i in BS(rf, self.scraper).select(".episode-item")]
             for e in range(len(episodes)):
                 episode = episodes[e]
                 sid = self.ep_server_id(episode)
                 iframe_url, tv_id = self.get_link(sid)
                 iframe_link, iframe_id = self.rabbit_id(iframe_url)
                 url = self.cdn_url(iframe_link, iframe_id)
                 self.dl(url, name, season=s + 1, episode=e + 1)
```

### Comparing `mov_cli-1.3.9/mov_cli/websites/solar.py` & `mov_cli-1.4.0/mov_cli/websites/solar.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,31 +7,31 @@
         super().__init__(base_url)
         self.base_url = base_url
         self.rep_key = "6LeWLCYeAAAAAL1caYzkrIY-M59Vu41vIblXQZ48"
         self.redo()
 
     def ask(self, series_id):
         r = self.client.get(f"{self.base_url}/ajax/v2/tv/seasons/{series_id}")
-        season_ids = [i["data-id"] for i in BS(r, self.parser).select(".dropdown-item")]
+        season_ids = [i["data-id"] for i in BS(r, self.scraper).select(".dropdown-item")]
         season = self.askseason(len(season_ids))
         rf = self.client.get(
             f"{self.base_url}/ajax/v2/season/episodes/{season_ids[int(season) - 1]}"
         )
-        episodes = [i["data-id"] for i in BS(rf, self.parser).select(".eps-item")]
+        episodes = [i["data-id"] for i in BS(rf, self.scraper).select(".eps-item")]
         episode = episodes[int(self.askepisode(len(episodes))) - 1]
         ep = self.getep(
             f"{self.base_url}/ajax/v2/season/episodes/{season_ids[int(season) - 1]}",
             episode,
         )
         return episode, season, ep
 
     def getep(self, url, data_id):
         source = self.client.get(f"{url}").text
 
-        soup = BS(source, self.parser)
+        soup = BS(source, self.scraper)
 
         unformated = soup.find("a", {"data-id": f"{data_id}"})["title"]
 
         formated = unformated.split("Eps")[1]
         formated = formated.split(":")[0]
 
         return formated
```

### Comparing `mov_cli-1.3.9/mov_cli/websites/streamblasters.py` & `mov_cli-1.4.0/mov_cli/websites/streamblasters.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,25 +10,25 @@
 
     def search(self, q: str = None) -> str:
         q = input(f"[!] {self.translated[self.task]}") if q is None else q
         return q.replace(" ", "+")
 
     def results(self, data: str) -> list:
         req = self.client.get(f"{self.base_url}/?s={data}")
-        soup = BS(req, self.parser)
+        soup = BS(req, self.scraper)
         items = soup.findAll("div", {"class": "title"})
         urls = [items[i].find("a")["href"] for i in range(len(items))]
         title = [items[i].find("a").text for i in range(len(items))]
         ids = [i for i in range(len(items))]
         mov_or_tv = ["MOVIE" for i in range(len(items))]
         return [list(sublist) for sublist in zip(title, urls, ids, mov_or_tv)]
 
     def doodext(self, url):
         req = self.client.get(url).text
-        soup = BS(req, self.parser)
+        soup = BS(req, self.scraper)
         ply = soup.find("li", {"id": "player-option-1"})
         post = ply["data-post"]
         self.client.set_headers(
             {
                 "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:108.0) Gecko/20100101 Firefox/108.0",
                 "Referer": f"{url}",
                 "Accept-Language": "de,en-US;q=0.7,en;q=0.3",
```

### Comparing `mov_cli-1.3.9/mov_cli/websites/tamilyogi.py` & `mov_cli-1.4.0/mov_cli/websites/tamilyogi.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,25 +10,25 @@
 
     def search(self, q: str):
         q = input(f"[!] {self.translated[self.task]}") if q is None else q
         return q
 
     def results(self, data: str) -> list:
         req = self.client.get(f"{self.base_url}/?s={data}").text
-        soup = BS(req, self.parser)
+        soup = BS(req, self.scraper)
         items = soup.findAll("div", {"class": "cover"})
         urls = [items[i].find("a")["href"] for i in range(len(items))]
         title = [items[i].find("a")["title"] for i in range(len(items))]
         ids = [i for i in range(len(items))]
         mov_or_tv = ["MOVIE" for i in range(len(items))]
         return [list(sublist) for sublist in zip(title, urls, ids, mov_or_tv)]
 
     def cdn_url(self, url):
         req = self.client.get(url).text
-        soup = BS(req, self.parser)
+        soup = BS(req, self.scraper)
         iframe = soup.find("iframe")["src"]
         q = self.client.get(iframe).text
         url = re.findall('file:"(.*?)"', q)[0]
         return url
 
     def MOV_PandDP(self, m: list, state: str = "d" or "p"):
         name = m[self.title]
```

### Comparing `mov_cli-1.3.9/mov_cli/websites/turkish123.py` & `mov_cli-1.4.0/mov_cli/websites/turkish123.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     def search(self, q: str = None) -> str:
         q = input(f"[!] {self.translated[self.task]}") if q is None else q
         return q.replace(" ", "+")
 
     def results(self, data: str) -> list:
         req = self.client.get(f"{self.base_url}/?s={data}").text
-        soup = BS(req, self.parser)
+        soup = BS(req, self.scraper)
         mlitem = soup.findAll("div", {"class": "ml-item"})
         items = []
         for i in range(len(mlitem)):
             if str(mlitem[i]).__contains__("episode"):
                 pass
             else:
                 items.append(mlitem[i])
@@ -26,28 +26,28 @@
         title = [items[i].find("a")["oldtitle"] for i in range(len(items))]
         ids = [items[i]["class"] for i in range(len(items))]
         mov_or_tv = ["TV" for i in range(len(items))]
         return [list(sublist) for sublist in zip(title, urls, ids, mov_or_tv)]
 
     def ask(self, url):
         req = self.client.get(url).text
-        soup = BS(req, self.parser)
+        soup = BS(req, self.scraper)
         episodes = soup.findAll("a", {"class": "episodi"})
         episode = int(self.askepisode(len(episodes)))
         req = self.client.get(episodes[episode - 1]["href"]).text
         regex = r'''var copyTexti= \['<iframe width="100%" height="100%" src="https:\/\/tukipasti\.com(.*?)"'''
         s = re.findall(regex, req)[0]
         req = self.client.get(f"https://tukipasti.com{s}").text
         url = re.findall("var urlPlay = '(.*?)'", req)[0]
         print(url)
         return url, episode, f"https://tukipasti.com{s}"
 
     def download(self, t):
         req = self.client.get(t[self.url]).text
-        soup = BS(req, self.parser)
+        soup = BS(req, self.scraper)
         episodes = soup.findAll("a", {"class": "episodi"})
         for e in range(len(episodes)):
             req = self.client.get(episodes[e]["href"]).text
             regex = r'''var copyTexti= \['<iframe width="100%" height="100%" src="https:\/\/tukipasti\.com(.*?)"'''
             s = re.findall(regex, req)[0]
             req = self.client.get(f"https://tukipasti.com{s}").text
             url = re.findall("var urlPlay = '(.*?)'", req)[0]
```

### Comparing `mov_cli-1.3.9/mov_cli/websites/viewasian.py` & `mov_cli-1.4.0/mov_cli/websites/animefox.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,104 +1,108 @@
-from bs4 import BeautifulSoup as BS
 from ..utils.scraper import WebScraper
+from bs4 import BeautifulSoup as BS
 import re
 
 
-class viewasian(WebScraper):
+class animefox(WebScraper):
     def __init__(self, base_url):
         super().__init__(base_url)
         self.base_url = base_url
 
-    def search(self, q: str):
+    def search(self, q: str = None) -> str:
         q = input(f"[!] {self.translated[self.task]}") if q is None else q
-        return q.replace(" ", "-")
+        return q.replace(" ", "+")
 
-    def results(self, data: str):
-        request = self.client.get(f"{self.base_url}/movie/search/{data}")
-        soup = BS(request, self.parser)
-        streams = soup.findAll("a", {"class": "ml-mask jt"})
-        urls = [streams[i]["href"] for i in range(len(streams))]
-        title = [streams[i]["title"] for i in range(len(streams))]
-        ids = [streams[i]["class"] for i in range(len(streams))]
-        mov_or_tv = ["TV" for i in range(len(streams))]
+    def results(self, data: str) -> list:
+        req = self.client.get(f"https://animefox.to/search?keyword={data}")
+        soup = BS(req, self.scraper)
+        items = soup.findAll("a", {"class": "film-poster-ahref"})
+        urls = [items[i]["href"] for i in range(len(items))]
+        title = [items[i]["title"] for i in range(len(items))]
+        ids = [i for i in range(len(items))]
+        mov_or_tv = [
+            "MOVIE" if items[i].__contains__("Movie") else "TV"
+            for i in range(len(items))
+        ]
         return [list(sublist) for sublist in zip(title, urls, ids, mov_or_tv)]
 
     def ask(self, url):
-        request = self.client.get(f"{self.base_url}{url}")
-        soup = BS(request, self.parser)
-        href = soup.find("a", {"class": "bwac-btn"})["href"]
-        request = self.client.get(f"{self.base_url}{href}")
-        soup = BS(request, self.parser)
-        episodes = soup.findAll("li", {"class": "ep-item"})
-        episode = int(self.askepisode(len(episodes)))
-        request = self.client.get(f"{self.base_url}{href}?ep={episode}").text
-        soup = BS(request, self.parser)
-        if re.search("doodstream", request):
-            dood = soup.find("li", {"class": "doodstream"})["data-video"]
-            li = self.doodstream(dood)
-        elif re.search("streamtape", request):
-            streamtape = soup.find("li", {"class": "streamtape"})["data-video"]
-            li = self.streamtape(streamtape)
-        else:
-            raise Exception("Unable to find URL")
-        return li, episode
-
-    def streamtape(self, url):
-        string = re.findall("""v\/([^"']*)\/""", url)[0]
-        request = self.client.get(f"https://streamtape.com/e/{string}").text
-        if '<h1 class="white">Video not found!</h1>' not in request:
-            regex = r"""'robotlink'\)\.innerHTML = '(.*?)'\+ \('(.*?)'\)"""
-            results = re.findall(regex, request)
-            for tuple in results:
-                url = tuple[0]
-                rest = tuple[1]
-            li = f"https:{url}{rest[3:]}"
-            return li
-        raise Exception("Video not found or removed")
-
-    #    def doodstream(self, url):
-    #        domain = re.findall("""([^"']*)\/e""", url)[0]
-    #        req = self.client.get(url).text
-    #        pass_md = re.findall(r"/pass_md5/[^']*", req)[0]
-    #        token = pass_md.split("/")[-1]
-    #        self.client.set_headers(
-    #            {
-    #                "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:108.0) Gecko/20100101 Firefox/108.0",
-    #                "Referer": f"{url}",
-    #                "Accept-Language": "en-GB,en;q=0.5",
-    #            }
-    #        )
-    #        drylink = self.client.get(f"{domain}{pass_md}").text
-    #        streamlink = f"{drylink}zUEJeL3mUN?token={token}"
-    #        print(streamlink)
-    #        return streamlink
+        a = self.client.get(f"{self.base_url}{url}")
+        soup = BS(a, self.scraper)
+        url = soup.find("div", {"class": "film-buttons"}).find("a")["href"]
+        req = self.client.get(self.base_url + url)
+        soup = BS(req, self.scraper)
+        episodes = len(soup.find("div", {"id": "episodes-page-1"}).findAll("a"))
+        episode = self.askepisode(episodes)
+        return self.base_url + url[:-1] + episode, episode
+
+    def mov(self, url):
+        a = self.client.get(f"{self.base_url}{url}")
+        soup = BS(a, self.scraper)
+        url = soup.find("div", {"class": "film-buttons"}).find("a")["href"]
+        return self.base_url + url
+
+    def cdn_url(self, url):
+        req = self.client.get(url)
+        soup = BS(req, self.scraper)
+        goload = soup.find("select", {"id": "select-iframe-to-display"}).findAll(
+            "option"
+        )[-1]["value"]
+        url = f"https://{goload}".split("-")[0]
+        a = self.client.head(url, redirects=False).headers["location"]
+        a = self.client.get(a)
+        soup = BS(a, self.scraper)
+        server = []
+        servers = soup.findAll("li", {"class": "linkserver"})
+        for video in servers:
+            if "dood.wf" in str(video["data-video"]):
+                server.append(video["data-video"])
+        return self.doodstream(server[0])
+
+    def doodstream(self, url):
+        domain = re.findall("""([^"']*)\/e""", url)[0]
+        req = self.client.get(url).text
+        pass_md = re.findall(r"/pass_md5/[^']*", req)[0]
+        token = pass_md.split("/")[-1]
+        self.client.set_headers(
+            {
+                "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:108.0) Gecko/20100101 Firefox/108.0",
+                "Referer": f"{url}",
+                "Accept-Language": "en-GB,en;q=0.5",
+            }
+        )
+        drylink = self.client.get(f"{domain}{pass_md}").text
+        streamlink = f"{drylink}zUEJeL3mUN?token={token}"
+        print(streamlink)
+        return streamlink
 
     def download(self, t):
-        request = self.client.get(f"{self.base_url}{t[self.url]}")
-        soup = BS(request, self.parser)
-        href = soup.find("a", {"class": "bwac-btn"})["href"]
-        request = self.client.get(f"{self.base_url}{href}")
-        soup = BS(request, self.parser)
-        episodes = soup.findAll("li", {"class": "ep-item"})
-        for e in range(len(episodes)):
-            request = self.client.get(f"{self.base_url}{href}?ep={e+1}").text
-            soup = BS(request, self.parser)
-            if re.search("doodstream", request):
-                dood = soup.find("li", {"class": "doodstream"})["data-video"]
-                li = self.doodstream(dood)
-            elif re.search("streamtape", request):
-                streamtape = soup.find("li", {"class": "streamtape"})["data-video"]
-                li = self.streamtape(streamtape)
-            else:
-                raise Exception("Unable to find URL")
-            self.dl(li, t[self.title], episode=e + 1)
+        a = self.client.get(f"{self.base_url}{t[self.url]}")
+        soup = BS(a, self.scraper)
+        url = soup.find("div", {"class": "film-buttons"}).find("a")["href"]
+        req = self.client.get(self.base_url + url)
+        soup = BS(req, self.scraper)
+        episodes = len(soup.find("div", {"id": "episodes-page-1"}).findAll("a"))
+        for e in range(episodes):
+            url = self.cdn_url(self.base_url + url[:-1] + e + 1)
+            self.dl(url, name=t[self.title], episode=e + 1)
 
     def TV_PandDP(self, t: list, state: str = "d" or "p" or "sd"):
         if state == "sd":
             self.download(t)
             return
         name = t[self.title]
-        url, episode = self.ask(t[self.url])
+        link, episode = self.ask(t[self.url])
+        url = self.cdn_url(link)
         if state == "d":
             self.dl(url, name, season=".", episode=episode)
             return
         self.play(url, name)
+
+    def MOV_PandDP(self, t: list, state: str = "d" or "p"):
+        name = t[self.title]
+        link = self.mov(t[self.url])
+        url = self.cdn_url(link)
+        if state == "d":
+            self.dl(url, name)
+            return
+        self.play(url, name)
```

### Comparing `mov_cli-1.3.9/mov_cli/websites/watchasian.py` & `mov_cli-1.4.0/mov_cli/websites/watchasian.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,33 +10,33 @@
 
     def search(self, q: str):
         q = input(f"[!] {self.translated[self.task]}") if q is None else q
         return q.replace(" ", "+")
 
     def results(self, data: str):
         req = self.client.get(f"{self.base_url}/search?type=movies&keyword={data}").text
-        soup = BS(req, self.parser)
+        soup = BS(req, self.scraper)
         ul = soup.find("ul", {"class": "switch-block list-episode-item"}).findAll("li")
         urls = [ul[i].find("a")["href"] for i in range(len(ul))]
         title = [ul[i].find("h3").text for i in range(len(ul))]
         ids = ["1" for i in range(len(ul))]
         mov_or_tv = ["TV" for i in range(len(ul))]
         return [list(sublist) for sublist in zip(title, urls, ids, mov_or_tv)]
 
     def ask(self, url):
         req = self.client.get(f"{self.base_url}{url}").text
-        soup = BS(req, self.parser)
+        soup = BS(req, self.scraper)
         episodes = soup.find(
             "ul", {"class": "list-episode-item-2 all-episode"}
         ).findAll("li")
         episode = int(self.askepisode(len(episodes)))
         episodes = episodes[::-1]
         href = episodes[episode - 1].find("a")["href"]
         q = self.client.get(self.base_url + href).text
-        soup = BS(q, self.parser)
+        soup = BS(q, self.scraper)
         if re.search("doodstream", q):
             li = soup.find("li", {"class": "doodstream"})["data-video"]
         else:
             raise Exception("Unable to find URL")
         return li, episode
 
     def doodstream(self, url):
@@ -54,23 +54,23 @@
         drylink = self.client.get(f"{domain}{pass_md}").text
         streamlink = f"{drylink}zUEJeL3mUN?token={token}"
         print(streamlink)
         return streamlink
 
     def download(self, t):
         req = self.client.get(f"{self.base_url}{t[self.url]}").text
-        soup = BS(req, self.parser)
+        soup = BS(req, self.scraper)
         episodes = soup.find(
             "ul", {"class": "list-episode-item-2 all-episode"}
         ).findAll("li")
         episodes = episodes[::-1]
         for e in range(len(episodes)):
             href = episodes[e].find("a")["href"]
             q = self.client.get(self.base_url + href).text
-            soup = BS(q, self.parser)
+            soup = BS(q, self.scraper)
             if re.search("doodstream", q):
                 li = soup.find("li", {"class": "doodstream"})["data-video"]
             else:
                 raise Exception("Unable to find URL")
             url = self.doodstream(li)
             self.dl(url, t[self.title], episode=e + 1)
```

### Comparing `mov_cli-1.3.9/mov_cli/websites/wlext.py` & `mov_cli-1.4.0/mov_cli/websites/wlext.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,17 @@
     def results(self, data: str) -> list:
         m = self.client.get(
             f"{self.base_url}/ptb-search/?f=search_movies&ptb-search=1&title={data}"
         )
         s = self.client.get(
             f"{self.base_url}/ptb-search/?f=search_series_1&ptb-search=1&title={data}"
         )
-        show = BS(s, self.parser)
+        show = BS(s, self.scraper)
         shows = show.findAll("h5", {"class": "ptb_post_title"})
-        movie = BS(m, self.parser)
+        movie = BS(m, self.scraper)
         movies = movie.findAll("h5", {"class": "ptb_post_title"})
         urls = [movies[i].find("a")["href"] for i in range(len(movies))] + [
             shows[i].find("a")["href"] for i in range(len(shows))
         ]
         title = [movies[i].find("a").text for i in range(len(movies))] + [
             shows[i].find("a").text for i in range(len(shows))
         ]
@@ -33,23 +33,23 @@
         mov_or_tv = ["MOVIE" for i in range(len(movies))] + [
             "TV" for i in range(len(shows))
         ]
         return [list(sublist) for sublist in zip(title, urls, ids, mov_or_tv)]
 
     def ask(self, url):
         req = self.client.get(url)
-        soup = BS(req, self.parser)
+        soup = BS(req, self.scraper)
         t = soup.find("select", {"id": "loadepisode"})
         try:
             episodes = len(t.findAll("option"))
         except:
             return print("Episode unavailable")
         episode = int(self.askepisode(episodes))
         req = self.client.get(f"{url}?server=cajitatop&episode={episode}").text
-        soup = BS(req, self.parser)
+        soup = BS(req, self.scraper)
         try:
             t = soup.find("iframe", {"loading": "lazy"})["src"]
             print(t)
         except:
             return print("Couldn't find cajita.to provider.")
         return t, episode
 
@@ -66,23 +66,23 @@
             exit(1)
         else:
             file = request["data"][-1]["file"]
         return file
 
     def download(self, t):
         req = self.client.get(t[self.url])
-        soup = BS(req, self.parser)
+        soup = BS(req, self.scraper)
         t = soup.find("select", {"id": "loadepisode"})
         try:
             episodes = len(t.findAll("option"))
         except:
             return print("Episode unavailable")
         for e in range(len(episodes)):
             req = self.client.get(f"{[self.url]}?server=cajitatop&episode={e+1}").text
-            soup = BS(req, self.parser)
+            soup = BS(req, self.scraper)
             try:
                 t = soup.find("iframe", {"loading": "lazy"})["src"]
             except:
                 return print("Couldn't find cajita.to provider.")
             url = str(self.cdn_url(t))
             self.dl(url, t[self.title], episode=e + 1)
```

### Comparing `mov_cli-1.3.9/mov_cli/websites/yoturkish.py` & `mov_cli-1.4.0/mov_cli/websites/yoturkish.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,55 +10,55 @@
 
     def search(self, q: str):
         q = input(f"[!] {self.translated[self.task]}") if q is None else q
         return q.replace(" ", "+")
 
     def results(self, data: str) -> list:
         req = self.client.get(f"{self.base_url}/?s={data}").text
-        soup = BS(req, self.parser)
+        soup = BS(req, self.scraper)
         items = []
         mlitem = soup.findAll("div", {"class": "item"})
         for i in range(len(mlitem)):
             if str(mlitem[i]).__contains__("episode"):
                 pass
             else:
                 items.append(mlitem[i])
         if soup.find_all("ul", {"class": "pagination"}):
             pagination = soup.find("ul", {"class": "pagination"}).findAll("li")[1:]
             for page in pagination:
                 req = self.client.get(page.find("a")["href"]).text
-                soup = BS(req, self.parser)
+                soup = BS(req, self.scraper)
                 pageitem = soup.findAll("div", {"class": "item"})
                 for i in range(len(pageitem)):
                     if str(pageitem[i]).__contains__("episode"):
                         pass
                     else:
                         items.append(pageitem[i])
         urls = [items[i].find("a")["href"] for i in range(len(items))]
         title = [items[i].find("a")["title"] for i in range(len(items))]
         ids = [items[i]["class"] for i in range(len(items))]
         mov_or_tv = ["TV" for i in range(len(items))]
         return [list(sublist) for sublist in zip(title, urls, ids, mov_or_tv)]
 
     def ask(self, url):
         req = self.client.get(url, True).text
-        soup = BS(req, self.parser)
+        soup = BS(req, self.scraper)
         episodes = soup.findAll("a", {"class": "episod"})
         episode = int(self.askepisode(len(episodes)))
         req = self.client.get(episodes[episode - 1]["href"], True).text
         regex = r'''<iframe width="100%" height="100%" src="https:\/\/tukipasti\.com(.*?)"'''
         s = re.findall(regex, req)[0]
         req = self.client.get(f"https://tukipasti.com{s}").text
         url = re.findall("var urlPlay = '(.*?)'", req)[0]
         print(url)
         return url, episode, f"https://tukipasti.com{s}"
 
     def download(self, t):
         req = self.client.get(t[self.url]).text
-        soup = BS(req, self.parser)
+        soup = BS(req, self.scraper)
         episodes = soup.findAll("a", {"class": "episod"})
         for e in range(len(episodes)):
             req = self.client.get(episodes[e]["href"]).text
             regex = r'''<iframe width="100%" height="100%" src="https:\/\/tukipasti\.com(.*?)"'''
             s = re.findall(regex, req)[0]
             req = self.client.get(f"https://tukipasti.com{s}").text
             url = re.findall("var urlPlay = '(.*?)'", req)[0]
```

### Comparing `mov_cli-1.3.9/pyproject.toml` & `mov_cli-1.4.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mov-cli"
-version = "1.3.9"
+version = "1.4.0"
 description = "A cli tool to browse and watch Movies/Shows/TV/Sports."
 authors = ["Pain <painedposeidon444@gmail.com>"]
 maintainers = ["Ananas <ananas@historylifeonline.xyz>"]
 license = "GPLv3"
 readme = "README.md"
 packages = [{include = "mov_cli"}]
 repository = "https://github.com/mov-cli/mov-cli"
```

### Comparing `mov_cli-1.3.9/PKG-INFO` & `mov_cli-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli
-Version: 1.3.9
+Version: 1.4.0
 Summary: A cli tool to browse and watch Movies/Shows/TV/Sports.
 Home-page: https://github.com/mov-cli/mov-cli
 License: GPLv3
 Author: Pain
 Author-email: painedposeidon444@gmail.com
 Maintainer: Ananas
 Maintainer-email: ananas@historylifeonline.xyz
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mov-cli Version: 1.3.9 Summary: A cli tool to
+Metadata-Version: 2.1 Name: mov-cli Version: 1.4.0 Summary: A cli tool to
 browse and watch Movies/Shows/TV/Sports. Home-page: https://github.com/mov-cli/
 mov-cli License: GPLv3 Author: Pain Author-email: painedposeidon444@gmail.com
 Maintainer: Ananas Maintainer-email: ananas@historylifeonline.xyz Requires-
 Python: >=3.9,<4.0 Classifier: License :: Other/Proprietary License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: beautifulsoup4
```

