# Comparing `tmp/TMDBTraktSyncer-1.0.8.tar.gz` & `tmp/TMDBTraktSyncer-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TMDBTraktSyncer-1.0.8.tar", last modified: Sat May 20 17:11:23 2023, max compression
+gzip compressed data, was "TMDBTraktSyncer-1.0.9.tar", last modified: Sat May 20 17:38:16 2023, max compression
```

## Comparing `TMDBTraktSyncer-1.0.8.tar` & `TMDBTraktSyncer-1.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 17:11:23.618399 TMDBTraktSyncer-1.0.8/
--rw-rw-rw-   0        0        0     1079 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.0.8/LICENSE
--rw-rw-rw-   0        0        0     6468 2023-05-20 17:11:23.617399 TMDBTraktSyncer-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     5795 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-20 17:11:23.598002 TMDBTraktSyncer-1.0.8/TMDBTraktSyncer/
--rw-rw-rw-   0        0        0     5773 2023-05-20 16:47:55.000000 TMDBTraktSyncer-1.0.8/TMDBTraktSyncer/TMDBTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.0.8/TMDBTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     1915 2023-05-20 16:29:13.000000 TMDBTraktSyncer-1.0.8/TMDBTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0     8793 2023-05-20 17:05:25.000000 TMDBTraktSyncer-1.0.8/TMDBTraktSyncer/errorHandling.py
--rw-rw-rw-   0        0        0     2932 2023-05-20 16:50:29.000000 TMDBTraktSyncer-1.0.8/TMDBTraktSyncer/tmdbRatings.py
--rw-rw-rw-   0        0        0     2069 2023-05-20 16:25:11.000000 TMDBTraktSyncer-1.0.8/TMDBTraktSyncer/traktRatings.py
--rw-rw-rw-   0        0        0     1822 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.0.8/TMDBTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-05-20 17:11:23.616399 TMDBTraktSyncer-1.0.8/TMDBTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0     6468 2023-05-20 17:11:23.000000 TMDBTraktSyncer-1.0.8/TMDBTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      487 2023-05-20 17:11:23.000000 TMDBTraktSyncer-1.0.8/TMDBTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 17:11:23.000000 TMDBTraktSyncer-1.0.8/TMDBTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-05-20 17:11:23.000000 TMDBTraktSyncer-1.0.8/TMDBTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-05-20 17:11:23.000000 TMDBTraktSyncer-1.0.8/TMDBTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-20 17:11:23.000000 TMDBTraktSyncer-1.0.8/TMDBTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-20 17:11:23.618399 TMDBTraktSyncer-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1291 2023-05-20 17:05:42.000000 TMDBTraktSyncer-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 17:38:16.150781 TMDBTraktSyncer-1.0.9/
+-rw-rw-rw-   0        0        0     1079 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0     6468 2023-05-20 17:38:16.149781 TMDBTraktSyncer-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     5795 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-20 17:38:16.125778 TMDBTraktSyncer-1.0.9/TMDBTraktSyncer/
+-rw-rw-rw-   0        0        0     5773 2023-05-20 16:47:55.000000 TMDBTraktSyncer-1.0.9/TMDBTraktSyncer/TMDBTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.0.9/TMDBTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     1915 2023-05-20 16:29:13.000000 TMDBTraktSyncer-1.0.9/TMDBTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0     8831 2023-05-20 17:37:01.000000 TMDBTraktSyncer-1.0.9/TMDBTraktSyncer/errorHandling.py
+-rw-rw-rw-   0        0        0     2932 2023-05-20 16:50:29.000000 TMDBTraktSyncer-1.0.9/TMDBTraktSyncer/tmdbRatings.py
+-rw-rw-rw-   0        0        0     2069 2023-05-20 16:25:11.000000 TMDBTraktSyncer-1.0.9/TMDBTraktSyncer/traktRatings.py
+-rw-rw-rw-   0        0        0     1822 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.0.9/TMDBTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-05-20 17:38:16.148782 TMDBTraktSyncer-1.0.9/TMDBTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0     6468 2023-05-20 17:38:16.000000 TMDBTraktSyncer-1.0.9/TMDBTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      487 2023-05-20 17:38:16.000000 TMDBTraktSyncer-1.0.9/TMDBTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 17:38:16.000000 TMDBTraktSyncer-1.0.9/TMDBTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-05-20 17:38:16.000000 TMDBTraktSyncer-1.0.9/TMDBTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-05-20 17:38:16.000000 TMDBTraktSyncer-1.0.9/TMDBTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-20 17:38:16.000000 TMDBTraktSyncer-1.0.9/TMDBTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-20 17:38:16.150781 TMDBTraktSyncer-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1291 2023-05-20 17:37:48.000000 TMDBTraktSyncer-1.0.9/setup.py
```

### Comparing `TMDBTraktSyncer-1.0.8/LICENSE` & `TMDBTraktSyncer-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.0.8/PKG-INFO` & `TMDBTraktSyncer-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TMDBTraktSyncer
-Version: 1.0.8
+Version: 1.0.9
 Summary: This python script will sync user ratings for Movies and TV Shows both ways between Trakt and TMDB.
 Home-page: https://github.com/RileyXX/TMDB-Trakt-Syncer
 Keywords: python,video,trakt,tmdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `TMDBTraktSyncer-1.0.8/README.md` & `TMDBTraktSyncer-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.0.8/TMDBTraktSyncer/TMDBTraktSyncer.py` & `TMDBTraktSyncer-1.0.9/TMDBTraktSyncer/TMDBTraktSyncer.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.0.8/TMDBTraktSyncer/authTrakt.py` & `TMDBTraktSyncer-1.0.9/TMDBTraktSyncer/authTrakt.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.0.8/TMDBTraktSyncer/errorHandling.py` & `TMDBTraktSyncer-1.0.9/TMDBTraktSyncer/errorHandling.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         response = None
         try:
             if payload is None:
                 response = requests.get(url, headers=headers)
             else:
                 response = requests.post(url, headers=headers, json=payload)
 
-            if response.status_code == 200:
+            if response.status_code in [200, 201, 204]:
                 return response  # Request succeeded, return response
             elif response.status_code in [429, 502, 503, 504, 520, 521, 522]:
                 # Server overloaded or rate limit exceeded, retry after delay
                 retry_attempts += 1
                 time.sleep(retry_delay)
                 retry_delay *= 2  # Exponential backoff for retries
             else:
@@ -102,17 +102,17 @@
         try:
             if payload is None:
                 response = requests.get(url, headers=headers)
             else:
                 response = requests.post(url, headers=headers, json=payload)
 
             status_code = response.status_code
-            if status_code == 200:
+            if status_code in [1, 12, 13]:
                 return response  # Request succeeded, return response
-            elif status_code == 429:
+            elif status_code in [24, 25, 43, 46, 429]:
                 # Rate limit exceeded, retry after delay
                 retry_attempts += 1
                 time.sleep(retry_delay)
                 retry_delay *= 2  # Exponential backoff for retries
             elif status_code in [501, 401, 405, 422, 404, 403, 409, 503, 500, 504, 429, 400, 406,
                                  422, 504, 429, 400, 400, 400, 401, 401, 401, 500, 401, 401, 401,
                                  404, 401, 401, 404, 401, 401, 404, 401, 200, 422, 405, 502, 500,
```

### Comparing `TMDBTraktSyncer-1.0.8/TMDBTraktSyncer/tmdbRatings.py` & `TMDBTraktSyncer-1.0.9/TMDBTraktSyncer/tmdbRatings.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.0.8/TMDBTraktSyncer/traktRatings.py` & `TMDBTraktSyncer-1.0.9/TMDBTraktSyncer/traktRatings.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.0.8/TMDBTraktSyncer/verifyCredentials.py` & `TMDBTraktSyncer-1.0.9/TMDBTraktSyncer/verifyCredentials.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.0.8/TMDBTraktSyncer.egg-info/PKG-INFO` & `TMDBTraktSyncer-1.0.9/TMDBTraktSyncer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TMDBTraktSyncer
-Version: 1.0.8
+Version: 1.0.9
 Summary: This python script will sync user ratings for Movies and TV Shows both ways between Trakt and TMDB.
 Home-page: https://github.com/RileyXX/TMDB-Trakt-Syncer
 Keywords: python,video,trakt,tmdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `TMDBTraktSyncer-1.0.8/setup.py` & `TMDBTraktSyncer-1.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.8'
+VERSION = '1.0.9'
 DESCRIPTION = 'This python script will sync user ratings for Movies and TV Shows both ways between Trakt and TMDB.'
 
 # Setting up
 setup(
     name="TMDBTraktSyncer",
     version=VERSION,
     description=DESCRIPTION,
```

