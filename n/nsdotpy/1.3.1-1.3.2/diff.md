# Comparing `tmp/nsdotpy-1.3.1.tar.gz` & `tmp/nsdotpy-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsdotpy-1.3.1.tar", max compression
+gzip compressed data, was "nsdotpy-1.3.2.tar", max compression
```

## Comparing `nsdotpy-1.3.1.tar` & `nsdotpy-1.3.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    34354 2023-05-19 00:22:40.519294 nsdotpy-1.3.1/LICENSE.md
--rw-r--r--   0        0        0     2440 2023-05-19 00:22:40.519294 nsdotpy-1.3.1/README.md
--rw-r--r--   0        0        0      790 2023-05-19 00:22:40.535294 nsdotpy-1.3.1/nsdotpy/__init__.py
--rw-r--r--   0        0        0    44770 2023-05-19 00:22:40.535294 nsdotpy-1.3.1/nsdotpy/session.py
--rw-r--r--   0        0        0     4963 2023-05-19 00:22:40.535294 nsdotpy-1.3.1/nsdotpy/valid.py
--rw-r--r--   0        0        0      719 2023-05-19 00:22:40.535294 nsdotpy-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     3354 1970-01-01 00:00:00.000000 nsdotpy-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0    34354 2023-05-20 08:21:06.868322 nsdotpy-1.3.2/LICENSE.md
+-rw-r--r--   0        0        0     2440 2023-05-20 08:21:06.868322 nsdotpy-1.3.2/README.md
+-rw-r--r--   0        0        0      790 2023-05-20 08:21:06.884323 nsdotpy-1.3.2/nsdotpy/__init__.py
+-rw-r--r--   0        0        0    44907 2023-05-20 08:21:06.884323 nsdotpy-1.3.2/nsdotpy/session.py
+-rw-r--r--   0        0        0     4963 2023-05-20 08:21:06.884323 nsdotpy-1.3.2/nsdotpy/valid.py
+-rw-r--r--   0        0        0      719 2023-05-20 08:21:06.884323 nsdotpy-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0     3354 1970-01-01 00:00:00.000000 nsdotpy-1.3.2/PKG-INFO
```

### Comparing `nsdotpy-1.3.1/LICENSE.md` & `nsdotpy-1.3.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nsdotpy-1.3.1/README.md` & `nsdotpy-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `nsdotpy-1.3.1/nsdotpy/__init__.py` & `nsdotpy-1.3.2/nsdotpy/__init__.py`

 * *Files identical despite different names*

### Comparing `nsdotpy-1.3.1/nsdotpy/session.py` & `nsdotpy-1.3.2/nsdotpy/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
             script_version (str): Version number of your script
             script_author (str): Author of your script
             script_user (str): Nation name of the user running your script
             keybind (str, optional): Keybind to count as a user click. Defaults to "space".
             link_to_src (str, optional): Link to the source code of your script.
             logger (logging.Logger | None, optional): Logger to use. Will create its own with name "NSDotPy" if none is specified. Defaults to None.
         """
-        self.VERSION = "1.3.1"
+        self.VERSION = "1.3.2"
         # Initialize logger
         if not logger:
             self._init_logger()
         else:
             self.logger = logger
         # Attach the tendo singleton to the session object so it can
         # only be run once at a time, avoiding simultaneity issues
@@ -361,17 +361,19 @@
         response = self._session.post(url, data=data, auth=_auth)
         # if the server tells us to wait, wait
         head = response.headers
         if waiting_time := head.get("Retry-After"):
             self.logger.warning(f"Rate limited. Waiting {waiting_time} seconds.")
             time.sleep(int(waiting_time))
         # slow down requests so we dont hit the rate limit in the first place
-        requests_left = int(head["X-RateLimit-Remaining"])
-        seconds_until_reset = int(head["X-RateLimit-Reset"])
-        time.sleep(seconds_until_reset / requests_left)
+        requests_left = int(head["RateLimit-Remaining"])
+        seconds_until_reset = int(head["RateLimit-Reset"])
+        # only slow down if we're close to the limit to avoid slowing down one off or infrequent requests
+        if requests_left < 10:
+            time.sleep(seconds_until_reset / requests_left)
         # end rate limiting section
         return response
 
     def login(self, nation: str, password: str) -> bool:
         """Logs in to the nationstates site.
 
         Args:
```

### Comparing `nsdotpy-1.3.1/nsdotpy/valid.py` & `nsdotpy-1.3.2/nsdotpy/valid.py`

 * *Files identical despite different names*

### Comparing `nsdotpy-1.3.1/pyproject.toml` & `nsdotpy-1.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nsdotpy"
-version = "1.3.1"
+version = "1.3.2"
 description = "A wrapper around httpx that abstracts away interacting with the HTML nationstates.net site. Focused on legality, correctness, and ease of use."
 authors = ["audrey <audreyreal@proton.me>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 repository = "https://github.com/sw33ze/NSDotPy"
 
 [tool.poetry.dependencies]
```

### Comparing `nsdotpy-1.3.1/PKG-INFO` & `nsdotpy-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsdotpy
-Version: 1.3.1
+Version: 1.3.2
 Summary: A wrapper around httpx that abstracts away interacting with the HTML nationstates.net site. Focused on legality, correctness, and ease of use.
 Home-page: https://github.com/sw33ze/NSDotPy
 License: AGPL-3.0-or-later
 Author: audrey
 Author-email: audreyreal@proton.me
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

