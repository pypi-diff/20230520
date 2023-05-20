# Comparing `tmp/czapi-0.1.8.tar.gz` & `tmp/czapi-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\czapi-0.1.8.tar", last modified: Sat May 20 20:38:44 2023, max compression
+gzip compressed data, was "dist\czapi-0.1.9.tar", last modified: Sat May 20 20:55:04 2023, max compression
```

## Comparing `czapi-0.1.8.tar` & `czapi-0.1.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 20:38:44.000000 czapi-0.1.8/
--rw-rw-rw-   0        0        0     2381 2022-02-26 15:53:17.000000 czapi-0.1.8/CONTRIBUTING.md
--rw-rw-rw-   0        0        0    11558 2022-02-26 15:53:17.000000 czapi-0.1.8/LICENSE
--rw-rw-rw-   0        0        0      116 2022-02-26 15:53:17.000000 czapi-0.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0    34990 2023-05-20 20:38:44.000000 czapi-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0    34232 2023-05-20 20:34:08.000000 czapi-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-20 20:38:44.000000 czapi-0.1.8/czapi/
--rw-rw-rw-   0        0        0       23 2023-05-20 20:38:16.000000 czapi-0.1.8/czapi/__init__.py
--rw-rw-rw-   0        0        0     1418 2023-05-20 20:33:44.000000 czapi-0.1.8/czapi/_nbdev.py
--rw-rw-rw-   0        0        0      249 2023-05-20 20:33:44.000000 czapi-0.1.8/czapi/api.py
-drwxrwxrwx   0        0        0        0 2023-05-20 20:38:44.000000 czapi-0.1.8/czapi/core/
--rw-rw-rw-   0        0        0        0 2023-03-10 03:45:51.000000 czapi-0.1.8/czapi/core/__init__.py
--rw-rw-rw-   0        0        0     1140 2023-05-20 20:33:44.000000 czapi-0.1.8/czapi/core/errors.py
-drwxrwxrwx   0        0        0        0 2023-05-20 20:38:44.000000 czapi-0.1.8/czapi/core/scraping/
--rw-rw-rw-   0        0        0        0 2022-12-21 13:02:35.000000 czapi-0.1.8/czapi/core/scraping/__init__.py
--rw-rw-rw-   0        0        0    11339 2023-05-20 20:33:44.000000 czapi-0.1.8/czapi/core/scraping/base.py
--rw-rw-rw-   0        0        0     1641 2023-05-20 20:33:44.000000 czapi-0.1.8/czapi/core/testing.py
--rw-rw-rw-   0        0        0      633 2023-05-20 20:33:44.000000 czapi-0.1.8/czapi/core/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-20 20:38:44.000000 czapi-0.1.8/czapi.egg-info/
--rw-rw-rw-   0        0        0    34990 2023-05-20 20:38:44.000000 czapi-0.1.8/czapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      464 2023-05-20 20:38:44.000000 czapi-0.1.8/czapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 20:38:44.000000 czapi-0.1.8/czapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-05-20 20:38:44.000000 czapi-0.1.8/czapi.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2022-02-26 16:04:21.000000 czapi-0.1.8/czapi.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       34 2023-05-20 20:38:44.000000 czapi-0.1.8/czapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-20 20:38:44.000000 czapi-0.1.8/czapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      612 2023-05-20 20:38:16.000000 czapi-0.1.8/settings.ini
--rw-rw-rw-   0        0        0       42 2023-05-20 20:38:44.000000 czapi-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     3158 2022-02-26 15:53:17.000000 czapi-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 20:55:04.000000 czapi-0.1.9/
+-rw-rw-rw-   0        0        0     2381 2022-02-26 15:53:17.000000 czapi-0.1.9/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0    11558 2022-02-26 15:53:17.000000 czapi-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0      116 2022-02-26 15:53:17.000000 czapi-0.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0    34990 2023-05-20 20:55:04.000000 czapi-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0    34232 2023-05-20 20:53:19.000000 czapi-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-20 20:55:04.000000 czapi-0.1.9/czapi/
+-rw-rw-rw-   0        0        0       23 2023-05-20 20:54:48.000000 czapi-0.1.9/czapi/__init__.py
+-rw-rw-rw-   0        0        0     1418 2023-05-20 20:53:06.000000 czapi-0.1.9/czapi/_nbdev.py
+-rw-rw-rw-   0        0        0      249 2023-05-20 20:53:06.000000 czapi-0.1.9/czapi/api.py
+drwxrwxrwx   0        0        0        0 2023-05-20 20:55:04.000000 czapi-0.1.9/czapi/core/
+-rw-rw-rw-   0        0        0        0 2023-03-10 03:45:51.000000 czapi-0.1.9/czapi/core/__init__.py
+-rw-rw-rw-   0        0        0     1140 2023-05-20 20:53:06.000000 czapi-0.1.9/czapi/core/errors.py
+drwxrwxrwx   0        0        0        0 2023-05-20 20:55:04.000000 czapi-0.1.9/czapi/core/scraping/
+-rw-rw-rw-   0        0        0        0 2022-12-21 13:02:35.000000 czapi-0.1.9/czapi/core/scraping/__init__.py
+-rw-rw-rw-   0        0        0    11369 2023-05-20 20:53:06.000000 czapi-0.1.9/czapi/core/scraping/base.py
+-rw-rw-rw-   0        0        0     1641 2023-05-20 20:53:06.000000 czapi-0.1.9/czapi/core/testing.py
+-rw-rw-rw-   0        0        0      633 2023-05-20 20:53:06.000000 czapi-0.1.9/czapi/core/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-20 20:55:04.000000 czapi-0.1.9/czapi.egg-info/
+-rw-rw-rw-   0        0        0    34990 2023-05-20 20:55:04.000000 czapi-0.1.9/czapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2023-05-20 20:55:04.000000 czapi-0.1.9/czapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 20:55:04.000000 czapi-0.1.9/czapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-05-20 20:55:04.000000 czapi-0.1.9/czapi.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2022-02-26 16:04:21.000000 czapi-0.1.9/czapi.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       34 2023-05-20 20:55:04.000000 czapi-0.1.9/czapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-20 20:55:04.000000 czapi-0.1.9/czapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      612 2023-05-20 20:54:48.000000 czapi-0.1.9/settings.ini
+-rw-rw-rw-   0        0        0       42 2023-05-20 20:55:04.000000 czapi-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     3158 2022-02-26 15:53:17.000000 czapi-0.1.9/setup.py
```

### Comparing `czapi-0.1.8/CONTRIBUTING.md` & `czapi-0.1.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `czapi-0.1.8/LICENSE` & `czapi-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `czapi-0.1.8/PKG-INFO` & `czapi-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: czapi
-Version: 0.1.8
+Version: 0.1.9
 Summary: CurlingZone scraper API.
 Home-page: https://github.com/calicorob/czapi/tree/master/
 Author: Robert Currie
 Author-email: robert.art.currie@gmail.com
 License: Apache Software License 2.0
 Keywords: curling,stats
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: czapi Version: 0.1.8 Summary: CurlingZone scraper
+Metadata-Version: 2.1 Name: czapi Version: 0.1.9 Summary: CurlingZone scraper
 API. Home-page: https://github.com/calicorob/czapi/tree/master/ Author: Robert
 Currie Author-email: robert.art.currie@gmail.com License: Apache Software
 License 2.0 Keywords: curling,stats Platform: UNKNOWN Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
 Natural Language :: English Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: License :: OSI Approved :: Apache
```

### Comparing `czapi-0.1.8/README.md` & `czapi-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `czapi-0.1.8/czapi/_nbdev.py` & `czapi-0.1.9/czapi/_nbdev.py`

 * *Files identical despite different names*

### Comparing `czapi-0.1.8/czapi/core/errors.py` & `czapi-0.1.9/czapi/core/errors.py`

 * *Files identical despite different names*

### Comparing `czapi-0.1.8/czapi/core/scraping/base.py` & `czapi-0.1.9/czapi/core/scraping/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -314,14 +314,16 @@
 game_data_column_headers = (
 
      'team_name'
     ,'href'
     ,'hammer_start'
     ,'score'
     ,'final_score'
+    ,'draw_num'
+    ,'draw'
     ,'hammer_progression'
     ,'relative_score'
     ,'guid'
 
 
 )
```

### Comparing `czapi-0.1.8/czapi/core/testing.py` & `czapi-0.1.9/czapi/core/testing.py`

 * *Files identical despite different names*

### Comparing `czapi-0.1.8/czapi/core/utils.py` & `czapi-0.1.9/czapi/core/utils.py`

 * *Files identical despite different names*

### Comparing `czapi-0.1.8/czapi.egg-info/PKG-INFO` & `czapi-0.1.9/czapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: czapi
-Version: 0.1.8
+Version: 0.1.9
 Summary: CurlingZone scraper API.
 Home-page: https://github.com/calicorob/czapi/tree/master/
 Author: Robert Currie
 Author-email: robert.art.currie@gmail.com
 License: Apache Software License 2.0
 Keywords: curling,stats
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: czapi Version: 0.1.8 Summary: CurlingZone scraper
+Metadata-Version: 2.1 Name: czapi Version: 0.1.9 Summary: CurlingZone scraper
 API. Home-page: https://github.com/calicorob/czapi/tree/master/ Author: Robert
 Currie Author-email: robert.art.currie@gmail.com License: Apache Software
 License 2.0 Keywords: curling,stats Platform: UNKNOWN Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
 Natural Language :: English Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: License :: OSI Approved :: Apache
```

### Comparing `czapi-0.1.8/settings.ini` & `czapi-0.1.9/settings.ini`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 user = calicorob
 description = CurlingZone scraper API.
 keywords = curling, stats
 author = Robert Currie
 author_email = robert.art.currie@gmail.com
 copyright = Robert Currie
 branch = master
-version = 0.1.8
+version = 0.1.9
 min_python = 3.6
 audience = Developers
 language = English
 custom_sidebar = False
 license = apache2
 status = 2
 requirements = bs4 requests
```

### Comparing `czapi-0.1.8/setup.py` & `czapi-0.1.9/setup.py`

 * *Files identical despite different names*

