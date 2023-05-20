# Comparing `tmp/TMDBTraktSyncer-1.0.9.tar.gz` & `tmp/TMDBTraktSyncer-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TMDBTraktSyncer-1.0.9.tar", last modified: Sat May 20 17:38:16 2023, max compression
+gzip compressed data, was "TMDBTraktSyncer-1.1.0.tar", last modified: Sat May 20 17:59:39 2023, max compression
```

## Comparing `TMDBTraktSyncer-1.0.9.tar` & `TMDBTraktSyncer-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 17:38:16.150781 TMDBTraktSyncer-1.0.9/
--rw-rw-rw-   0        0        0     1079 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.0.9/LICENSE
--rw-rw-rw-   0        0        0     6468 2023-05-20 17:38:16.149781 TMDBTraktSyncer-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     5795 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-05-20 17:38:16.125778 TMDBTraktSyncer-1.0.9/TMDBTraktSyncer/
--rw-rw-rw-   0        0        0     5773 2023-05-20 16:47:55.000000 TMDBTraktSyncer-1.0.9/TMDBTraktSyncer/TMDBTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.0.9/TMDBTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     1915 2023-05-20 16:29:13.000000 TMDBTraktSyncer-1.0.9/TMDBTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0     8831 2023-05-20 17:37:01.000000 TMDBTraktSyncer-1.0.9/TMDBTraktSyncer/errorHandling.py
--rw-rw-rw-   0        0        0     2932 2023-05-20 16:50:29.000000 TMDBTraktSyncer-1.0.9/TMDBTraktSyncer/tmdbRatings.py
--rw-rw-rw-   0        0        0     2069 2023-05-20 16:25:11.000000 TMDBTraktSyncer-1.0.9/TMDBTraktSyncer/traktRatings.py
--rw-rw-rw-   0        0        0     1822 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.0.9/TMDBTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-05-20 17:38:16.148782 TMDBTraktSyncer-1.0.9/TMDBTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0     6468 2023-05-20 17:38:16.000000 TMDBTraktSyncer-1.0.9/TMDBTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      487 2023-05-20 17:38:16.000000 TMDBTraktSyncer-1.0.9/TMDBTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 17:38:16.000000 TMDBTraktSyncer-1.0.9/TMDBTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-05-20 17:38:16.000000 TMDBTraktSyncer-1.0.9/TMDBTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-05-20 17:38:16.000000 TMDBTraktSyncer-1.0.9/TMDBTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-20 17:38:16.000000 TMDBTraktSyncer-1.0.9/TMDBTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-20 17:38:16.150781 TMDBTraktSyncer-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1291 2023-05-20 17:37:48.000000 TMDBTraktSyncer-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 17:59:39.793807 TMDBTraktSyncer-1.1.0/
+-rw-rw-rw-   0        0        0     1079 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     6468 2023-05-20 17:59:39.793807 TMDBTraktSyncer-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5795 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-20 17:59:39.772822 TMDBTraktSyncer-1.1.0/TMDBTraktSyncer/
+-rw-rw-rw-   0        0        0     5773 2023-05-20 16:47:55.000000 TMDBTraktSyncer-1.1.0/TMDBTraktSyncer/TMDBTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.1.0/TMDBTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     1915 2023-05-20 16:29:13.000000 TMDBTraktSyncer-1.1.0/TMDBTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0     8904 2023-05-20 17:58:42.000000 TMDBTraktSyncer-1.1.0/TMDBTraktSyncer/errorHandling.py
+-rw-rw-rw-   0        0        0     2932 2023-05-20 16:50:29.000000 TMDBTraktSyncer-1.1.0/TMDBTraktSyncer/tmdbRatings.py
+-rw-rw-rw-   0        0        0     2069 2023-05-20 16:25:11.000000 TMDBTraktSyncer-1.1.0/TMDBTraktSyncer/traktRatings.py
+-rw-rw-rw-   0        0        0     1822 2023-05-19 02:25:08.000000 TMDBTraktSyncer-1.1.0/TMDBTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-05-20 17:59:39.791808 TMDBTraktSyncer-1.1.0/TMDBTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0     6468 2023-05-20 17:59:39.000000 TMDBTraktSyncer-1.1.0/TMDBTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      487 2023-05-20 17:59:39.000000 TMDBTraktSyncer-1.1.0/TMDBTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 17:59:39.000000 TMDBTraktSyncer-1.1.0/TMDBTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-05-20 17:59:39.000000 TMDBTraktSyncer-1.1.0/TMDBTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-05-20 17:59:39.000000 TMDBTraktSyncer-1.1.0/TMDBTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-20 17:59:39.000000 TMDBTraktSyncer-1.1.0/TMDBTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-20 17:59:39.794807 TMDBTraktSyncer-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1291 2023-05-20 17:59:14.000000 TMDBTraktSyncer-1.1.0/setup.py
```

### Comparing `TMDBTraktSyncer-1.0.9/LICENSE` & `TMDBTraktSyncer-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.0.9/PKG-INFO` & `TMDBTraktSyncer-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TMDBTraktSyncer
-Version: 1.0.9
+Version: 1.1.0
 Summary: This python script will sync user ratings for Movies and TV Shows both ways between Trakt and TMDB.
 Home-page: https://github.com/RileyXX/TMDB-Trakt-Syncer
 Keywords: python,video,trakt,tmdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `TMDBTraktSyncer-1.0.9/README.md` & `TMDBTraktSyncer-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.0.9/TMDBTraktSyncer/TMDBTraktSyncer.py` & `TMDBTraktSyncer-1.1.0/TMDBTraktSyncer/TMDBTraktSyncer.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.0.9/TMDBTraktSyncer/authTrakt.py` & `TMDBTraktSyncer-1.1.0/TMDBTraktSyncer/authTrakt.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.0.9/TMDBTraktSyncer/errorHandling.py` & `TMDBTraktSyncer-1.1.0/TMDBTraktSyncer/errorHandling.py`

 * *Files 16% similar despite different names*

```diff
@@ -37,15 +37,15 @@
             if payload is None:
                 response = requests.get(url, headers=headers)
             else:
                 response = requests.post(url, headers=headers, json=payload)
 
             if response.status_code in [200, 201, 204]:
                 return response  # Request succeeded, return response
-            elif response.status_code in [429, 502, 503, 504, 520, 521, 522]:
+            elif response.status_code in [429, 500, 502, 503, 504, 520, 521, 522]:
                 # Server overloaded or rate limit exceeded, retry after delay
                 retry_attempts += 1
                 time.sleep(retry_delay)
                 retry_delay *= 2  # Exponential backoff for retries
             else:
                 # Handle other status codes as needed
                 error_message = get_trakt_message(response.status_code)
@@ -102,17 +102,17 @@
         try:
             if payload is None:
                 response = requests.get(url, headers=headers)
             else:
                 response = requests.post(url, headers=headers, json=payload)
 
             status_code = response.status_code
-            if status_code in [1, 12, 13]:
+            if status_code in [200, 201]:
                 return response  # Request succeeded, return response
-            elif status_code in [24, 25, 43, 46, 429]:
+            elif status_code in [504, 429, 502, 503]:
                 # Rate limit exceeded, retry after delay
                 retry_attempts += 1
                 time.sleep(retry_delay)
                 retry_delay *= 2  # Exponential backoff for retries
             elif status_code in [501, 401, 405, 422, 404, 403, 409, 503, 500, 504, 429, 400, 406,
                                  422, 504, 429, 400, 400, 400, 401, 401, 401, 500, 401, 401, 401,
                                  404, 401, 401, 404, 401, 401, 404, 401, 200, 422, 405, 502, 500,
@@ -131,57 +131,58 @@
             return None
 
     print("Max retry attempts reached with TMDB API, request failed.")
     return None
 
 def get_tmdb_message(status_code):
     error_messages = {
-        1: "Success",
-        2: "Invalid service: this service does not exist",
-        3: "Authentication failed: You do not have permissions to access the service",
-        4: "Invalid format: This service doesn't exist in that format",
-        5: "Invalid parameters: Your request parameters are incorrect",
-        6: "Invalid id: The pre-requisite id is invalid or not found",
-        7: "Invalid API key: You must be granted a valid key",
-        8: "Duplicate entry: The data you tried to submit already exists",
-        9: "Service offline: This service is temporarily offline, try again later",
-        10: "Suspended API key: Access to your account has been suspended, contact TMDB",
-        11: "Internal error: Something went wrong, contact TMDB",
-        12: "The item/record was updated successfully",
-        13: "The item/record was deleted successfully",
-        14: "Authentication failed",
-        15: "Failed",
-        16: "Device denied",
-        17: "Session denied",
-        18: "Validation failed",
-        19: "Invalid accept header",
-        20: "Invalid date range: Should be a range no longer than 14 days",
-        21: "Entry not found: The item you are trying to edit cannot be found",
-        22: "Invalid page: Pages start at 1 and max at 1000. They are expected to be an integer",
-        23: "Invalid date: Format needs to be YYYY-MM-DD",
-        24: "Your request to the backend server timed out. Try again",
-        25: "Your request count is over the allowed limit",
-        26: "You must provide a username and password",
-        27: "Too many append to response objects: The maximum number of remote calls is 20",
-        28: "Invalid timezone: Please consult the documentation for a valid timezone",
-        29: "You must confirm this action: Please provide a confirm=true parameter",
-        30: "Invalid username and/or password: You did not provide a valid login",
-        31: "Account disabled: Your account is no longer active. Contact TMDB if this is an error",
-        32: "Email not verified: Your email address has not been verified",
-        33: "Invalid request token: The request token is either expired or invalid",
-        34: "The resource you requested could not be found",
-        35: "Invalid token",
-        36: "This token hasn't been granted write permission by the user",
-        37: "The requested session could not be found",
-        38: "You don't have permission to edit this resource",
-        39: "This resource is private",
-        40: "Nothing to update",
-        41: "This request token hasn't been approved by the user",
-        42: "This request method is not supported for this resource",
-        43: "Couldn't connect to the backend server",
-        44: "The ID is invalid",
-        45: "This user has been suspended",
-        46: "The API is undergoing maintenance. Try again later",
-        47: "The input is not valid"
+        200: "Success",
+        501: "Invalid service: this service does not exist",
+        401: "Authentication failed: You do not have permissions to access the service",
+        405: "Invalid format: This service doesn't exist in that format",
+        422: "Invalid parameters: Your request parameters are incorrect",
+        404: "Invalid id: The pre-requisite id is invalid or not found",
+        401: "Invalid API key: You must be granted a valid key",
+        403: "Duplicate entry: The data you tried to submit already exists",
+        503: "Service offline: This service is temporarily offline, try again later",
+        401: "Suspended API key: Access to your account has been suspended, contact TMDB",
+        500: "Internal error: Something went wrong, contact TMDB",
+        201: "The item/record was updated successfully",
+        200: "The item/record was deleted successfully",
+        401: "Authentication failed",
+        500: "Failed",
+        401: "Device denied",
+        401: "Session denied",
+        400: "Validation failed",
+        406: "Invalid accept header",
+        422: "Invalid date range: Should be a range no longer than 14 days",
+        200: "Entry not found: The item you are trying to edit cannot be found",
+        400: "Invalid page: Pages start at 1 and max at 1000. They are expected to be an integer",
+        400: "Invalid date: Format needs to be YYYY-MM-DD",
+        504: "Your request to the backend server timed out. Try again",
+        429: "Your request count (#) is over the allowed limit of (40)",
+        400: "You must provide a username and password",
+        400: "Too many append to response objects: The maximum number of remote calls is 20",
+        400: "Invalid timezone: Please consult the documentation for a valid timezone",
+        400: "You must confirm this action: Please provide a confirm=true parameter",
+        401: "Invalid username and/or password: You did not provide a valid login",
+        401: "Account disabled: Your account is no longer active. Contact TMDB if this is an error",
+        401: "Email not verified: Your email address has not been verified",
+        401: "Invalid request token: The request token is either expired or invalid",
+        404: "The resource you requested could not be found",
+        401: "Invalid token",
+        401: "This token hasn't been granted write permission by the user",
+        404: "The requested session could not be found",
+        401: "You don't have permission to edit this resource",
+        401: "This resource is private",
+        200: "Nothing to update",
+        422: "This request token hasn't been approved by the user",
+        405: "This request method is not supported for this resource",
+        502: "Couldn't connect to the backend server",
+        500: "The ID is invalid",
+        403: "This user has been suspended",
+        503: "The API is undergoing maintenance. Try again later",
+        400: "The input is not valid"
     }
 
     return error_messages.get(status_code, "Unknown error")
+
```

### Comparing `TMDBTraktSyncer-1.0.9/TMDBTraktSyncer/tmdbRatings.py` & `TMDBTraktSyncer-1.1.0/TMDBTraktSyncer/tmdbRatings.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.0.9/TMDBTraktSyncer/traktRatings.py` & `TMDBTraktSyncer-1.1.0/TMDBTraktSyncer/traktRatings.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.0.9/TMDBTraktSyncer/verifyCredentials.py` & `TMDBTraktSyncer-1.1.0/TMDBTraktSyncer/verifyCredentials.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.0.9/TMDBTraktSyncer.egg-info/PKG-INFO` & `TMDBTraktSyncer-1.1.0/TMDBTraktSyncer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TMDBTraktSyncer
-Version: 1.0.9
+Version: 1.1.0
 Summary: This python script will sync user ratings for Movies and TV Shows both ways between Trakt and TMDB.
 Home-page: https://github.com/RileyXX/TMDB-Trakt-Syncer
 Keywords: python,video,trakt,tmdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `TMDBTraktSyncer-1.0.9/setup.py` & `TMDBTraktSyncer-1.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.9'
+VERSION = '1.1.0'
 DESCRIPTION = 'This python script will sync user ratings for Movies and TV Shows both ways between Trakt and TMDB.'
 
 # Setting up
 setup(
     name="TMDBTraktSyncer",
     version=VERSION,
     description=DESCRIPTION,
```

