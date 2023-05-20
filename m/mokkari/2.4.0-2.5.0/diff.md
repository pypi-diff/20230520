# Comparing `tmp/mokkari-2.4.0.tar.gz` & `tmp/mokkari-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mokkari-2.4.0.tar", max compression
+gzip compressed data, was "mokkari-2.5.0.tar", max compression
```

## Comparing `mokkari-2.4.0.tar` & `mokkari-2.5.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0    35149 2023-05-18 12:27:13.789870 mokkari-2.4.0/LICENSE
--rw-r--r--   0        0        0     1946 2023-05-18 12:27:13.789870 mokkari-2.4.0/README.rst
--rw-r--r--   0        0        0      992 2023-05-18 12:27:13.789870 mokkari-2.4.0/mokkari/__init__.py
--rw-r--r--   0        0        0     2960 2023-05-18 12:27:13.789870 mokkari-2.4.0/mokkari/arc.py
--rw-r--r--   0        0        0     3553 2023-05-18 12:27:13.789870 mokkari-2.4.0/mokkari/character.py
--rw-r--r--   0        0        0     3338 2023-05-18 12:27:13.789870 mokkari-2.4.0/mokkari/creator.py
--rw-r--r--   0        0        0      750 2023-05-18 12:27:13.789870 mokkari-2.4.0/mokkari/exceptions.py
--rw-r--r--   0        0        0     1148 2023-05-18 12:27:13.789870 mokkari-2.4.0/mokkari/genre.py
--rw-r--r--   0        0        0     9157 2023-05-18 12:27:13.793870 mokkari-2.4.0/mokkari/issue.py
--rw-r--r--   0        0        0     3257 2023-05-18 12:27:13.793870 mokkari-2.4.0/mokkari/publisher.py
--rw-r--r--   0        0        0     1148 2023-05-18 12:27:13.793870 mokkari-2.4.0/mokkari/rating.py
--rw-r--r--   0        0        0     1213 2023-05-18 12:27:13.793870 mokkari-2.4.0/mokkari/reprint.py
--rw-r--r--   0        0        0     7499 2023-05-18 12:27:13.793870 mokkari-2.4.0/mokkari/series.py
--rw-r--r--   0        0        0    14156 2023-05-18 12:27:13.793870 mokkari-2.4.0/mokkari/session.py
--rw-r--r--   0        0        0     2103 2023-05-18 12:27:13.793870 mokkari-2.4.0/mokkari/sqlite_cache.py
--rw-r--r--   0        0        0     3138 2023-05-18 12:27:13.793870 mokkari-2.4.0/mokkari/team.py
--rw-r--r--   0        0        0     1259 2023-05-18 12:27:13.793870 mokkari-2.4.0/mokkari/variant.py
--rw-r--r--   0        0        0     2334 2023-05-18 12:27:13.793870 mokkari-2.4.0/pyproject.toml
--rw-r--r--   0        0        0      544 2023-05-18 12:27:13.793870 mokkari-2.4.0/tests/README.md
--rw-r--r--   0        0        0       25 2023-05-18 12:27:13.793870 mokkari-2.4.0/tests/__init__.py
--rw-r--r--   0        0        0      734 2023-05-18 12:27:13.793870 mokkari-2.4.0/tests/conftest.py
--rw-r--r--   0        0        0     2590 2023-05-18 12:27:13.793870 mokkari-2.4.0/tests/test_arcs.py
--rw-r--r--   0        0        0     2075 2023-05-18 12:27:13.793870 mokkari-2.4.0/tests/test_cache.py
--rw-r--r--   0        0        0     3087 2023-05-18 12:27:13.793870 mokkari-2.4.0/tests/test_characters.py
--rw-r--r--   0        0        0     2594 2023-05-18 12:27:13.793870 mokkari-2.4.0/tests/test_creator.py
--rw-r--r--   0        0        0      659 2023-05-18 12:27:13.793870 mokkari-2.4.0/tests/test_init.py
--rw-r--r--   0        0        0    10082 2023-05-18 12:27:13.793870 mokkari-2.4.0/tests/test_issues.py
--rw-r--r--   0        0        0     2476 2023-05-18 12:27:13.793870 mokkari-2.4.0/tests/test_publishers.py
--rw-r--r--   0        0        0      714 2023-05-18 12:27:13.793870 mokkari-2.4.0/tests/test_role.py
--rw-r--r--   0        0        0     4091 2023-05-18 12:27:13.793870 mokkari-2.4.0/tests/test_series.py
--rw-r--r--   0        0        0      734 2023-05-18 12:27:13.793870 mokkari-2.4.0/tests/test_series_type.py
--rw-r--r--   0        0        0     2648 2023-05-18 12:27:13.793870 mokkari-2.4.0/tests/test_teams.py
--rw-r--r--   0        0        0   544768 2023-05-18 12:27:13.797870 mokkari-2.4.0/tests/testing_mock.sqlite
--rw-r--r--   0        0        0     3615 1970-01-01 00:00:00.000000 mokkari-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-20 15:15:39.131600 mokkari-2.5.0/LICENSE
+-rw-r--r--   0        0        0     1946 2023-05-20 15:15:39.131600 mokkari-2.5.0/README.rst
+-rw-r--r--   0        0        0     1250 2023-05-20 15:15:39.131600 mokkari-2.5.0/mokkari/__init__.py
+-rw-r--r--   0        0        0     2960 2023-05-20 15:15:39.131600 mokkari-2.5.0/mokkari/arc.py
+-rw-r--r--   0        0        0     3553 2023-05-20 15:15:39.131600 mokkari-2.5.0/mokkari/character.py
+-rw-r--r--   0        0        0     3338 2023-05-20 15:15:39.131600 mokkari-2.5.0/mokkari/creator.py
+-rw-r--r--   0        0        0      750 2023-05-20 15:15:39.131600 mokkari-2.5.0/mokkari/exceptions.py
+-rw-r--r--   0        0        0     1148 2023-05-20 15:15:39.131600 mokkari-2.5.0/mokkari/genre.py
+-rw-r--r--   0        0        0     9157 2023-05-20 15:15:39.131600 mokkari-2.5.0/mokkari/issue.py
+-rw-r--r--   0        0        0     3257 2023-05-20 15:15:39.131600 mokkari-2.5.0/mokkari/publisher.py
+-rw-r--r--   0        0        0     1148 2023-05-20 15:15:39.131600 mokkari-2.5.0/mokkari/rating.py
+-rw-r--r--   0        0        0     1213 2023-05-20 15:15:39.131600 mokkari-2.5.0/mokkari/reprint.py
+-rw-r--r--   0        0        0     7499 2023-05-20 15:15:39.131600 mokkari-2.5.0/mokkari/series.py
+-rw-r--r--   0        0        0    14359 2023-05-20 15:15:39.131600 mokkari-2.5.0/mokkari/session.py
+-rw-r--r--   0        0        0     2103 2023-05-20 15:15:39.131600 mokkari-2.5.0/mokkari/sqlite_cache.py
+-rw-r--r--   0        0        0     3138 2023-05-20 15:15:39.131600 mokkari-2.5.0/mokkari/team.py
+-rw-r--r--   0        0        0     1259 2023-05-20 15:15:39.131600 mokkari-2.5.0/mokkari/variant.py
+-rw-r--r--   0        0        0     2334 2023-05-20 15:15:39.131600 mokkari-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0      544 2023-05-20 15:15:39.131600 mokkari-2.5.0/tests/README.md
+-rw-r--r--   0        0        0       25 2023-05-20 15:15:39.131600 mokkari-2.5.0/tests/__init__.py
+-rw-r--r--   0        0        0      734 2023-05-20 15:15:39.131600 mokkari-2.5.0/tests/conftest.py
+-rw-r--r--   0        0        0     2590 2023-05-20 15:15:39.131600 mokkari-2.5.0/tests/test_arcs.py
+-rw-r--r--   0        0        0     2075 2023-05-20 15:15:39.131600 mokkari-2.5.0/tests/test_cache.py
+-rw-r--r--   0        0        0     3087 2023-05-20 15:15:39.131600 mokkari-2.5.0/tests/test_characters.py
+-rw-r--r--   0        0        0     2594 2023-05-20 15:15:39.131600 mokkari-2.5.0/tests/test_creator.py
+-rw-r--r--   0        0        0      659 2023-05-20 15:15:39.131600 mokkari-2.5.0/tests/test_init.py
+-rw-r--r--   0        0        0    10082 2023-05-20 15:15:39.135600 mokkari-2.5.0/tests/test_issues.py
+-rw-r--r--   0        0        0     2476 2023-05-20 15:15:39.135600 mokkari-2.5.0/tests/test_publishers.py
+-rw-r--r--   0        0        0      714 2023-05-20 15:15:39.135600 mokkari-2.5.0/tests/test_role.py
+-rw-r--r--   0        0        0     4091 2023-05-20 15:15:39.135600 mokkari-2.5.0/tests/test_series.py
+-rw-r--r--   0        0        0      734 2023-05-20 15:15:39.135600 mokkari-2.5.0/tests/test_series_type.py
+-rw-r--r--   0        0        0     2648 2023-05-20 15:15:39.135600 mokkari-2.5.0/tests/test_teams.py
+-rw-r--r--   0        0        0   544768 2023-05-20 15:15:39.135600 mokkari-2.5.0/tests/testing_mock.sqlite
+-rw-r--r--   0        0        0     3464 1970-01-01 00:00:00.000000 mokkari-2.5.0/PKG-INFO
```

### Comparing `mokkari-2.4.0/LICENSE` & `mokkari-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mokkari-2.4.0/README.rst` & `mokkari-2.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `mokkari-2.4.0/mokkari/__init__.py` & `mokkari-2.5.0/mokkari/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,42 @@
 """Project entry file."""
 
 # Keep this at beginning of file to prevent circular import with session
-__version__ = "2.4.0"
+__version__ = "2.5.0"
 
 from typing import Optional
 
 from mokkari import exceptions, session, sqlite_cache
 
 
 def api(
     username: Optional[str] = None,
     passwd: Optional[str] = None,
     cache: sqlite_cache.SqliteCache = None,
+    user_agent: Optional[str] = None,
 ) -> session.Session:
     """Entry function the sets login credentials for metron.cloud.
 
     Args:
         username (str): The username used for metron.cloud.
         passwd (str): The password used for metron.cloud.
         SqliteCache optional: SqliteCache to use
+        user_agent optional(str): The user agent string for the application using Mokkari.
+        For example 'Foo Bar/1.0'.
 
     Returns:
         A :obj:`Session` object
 
     Raises:
         AuthenticationError: If Metron returns with an invalid API credentials response.
+
+    .. versionadded:: 2.5.0
+
+        - Added ``user_agent`` argument.
     """
     if username is None:
         raise exceptions.AuthenticationError("Missing username.")
 
     if passwd is None:
         raise exceptions.AuthenticationError("Missing passwd.")
 
-    return session.Session(username, passwd, cache=cache)
+    return session.Session(username, passwd, cache=cache, user_agent=user_agent)
```

### Comparing `mokkari-2.4.0/mokkari/arc.py` & `mokkari-2.5.0/mokkari/arc.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.4.0/mokkari/character.py` & `mokkari-2.5.0/mokkari/character.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.4.0/mokkari/creator.py` & `mokkari-2.5.0/mokkari/creator.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.4.0/mokkari/exceptions.py` & `mokkari-2.5.0/mokkari/exceptions.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.4.0/mokkari/genre.py` & `mokkari-2.5.0/mokkari/genre.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.4.0/mokkari/issue.py` & `mokkari-2.5.0/mokkari/issue.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.4.0/mokkari/publisher.py` & `mokkari-2.5.0/mokkari/publisher.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.4.0/mokkari/rating.py` & `mokkari-2.5.0/mokkari/rating.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.4.0/mokkari/reprint.py` & `mokkari-2.5.0/mokkari/reprint.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.4.0/mokkari/series.py` & `mokkari-2.5.0/mokkari/series.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.4.0/mokkari/session.py` & `mokkari-2.5.0/mokkari/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,27 +35,30 @@
     """
     Session to request api endpoints.
 
     Args:
         username (str): The username for authentication with metron.cloud
         passwd (str): The password used for authentication with metron.cloud
         cache (SqliteCache, optional): SqliteCache to use
+        user_agent optional(str): The user agent string for the application using Mokkari.
     """
 
     def __init__(
         self,
         username: str,
         passwd: str,
         cache: Optional[sqlite_cache.SqliteCache] = None,
+        user_agent: Optional[str] = None,
     ) -> None:
         """Initialize a new Session."""
         self.username = username
         self.passwd = passwd
         self.header = {
-            "User-Agent": f"Mokkari/{__version__} ({platform.system()}; {platform.release()})"
+            "User-Agent": f"{f'{user_agent} ' if user_agent is not None else ''}"
+            + f"Mokkari/{__version__} ({platform.system()}; {platform.release()})"
         }
         self.api_url = "https://metron.cloud/api/{}/"
         self.cache = cache
 
     def _call(
         self,
         endpoint: List[Union[str, int]],
```

### Comparing `mokkari-2.4.0/mokkari/sqlite_cache.py` & `mokkari-2.5.0/mokkari/sqlite_cache.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.4.0/mokkari/team.py` & `mokkari-2.5.0/mokkari/team.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.4.0/mokkari/variant.py` & `mokkari-2.5.0/mokkari/variant.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.4.0/pyproject.toml` & `mokkari-2.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mokkari"
-version = "2.4.0"
+version = "2.5.0"
 description = "Python wrapper for Metron API"
 authors = ["Brian Pepple <bdpepple@gmail.com>"]
 license = "GPL-3.0-or-later"
 maintainers = ["Brian Pepple <bdpepple@gmail.com>"]
 readme = "README.rst"
 packages = [
 	{ include = "mokkari" },
```

### Comparing `mokkari-2.4.0/tests/README.md` & `mokkari-2.5.0/tests/README.md`

 * *Files identical despite different names*

### Comparing `mokkari-2.4.0/tests/conftest.py` & `mokkari-2.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.4.0/tests/test_arcs.py` & `mokkari-2.5.0/tests/test_arcs.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.4.0/tests/test_cache.py` & `mokkari-2.5.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.4.0/tests/test_characters.py` & `mokkari-2.5.0/tests/test_characters.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.4.0/tests/test_creator.py` & `mokkari-2.5.0/tests/test_creator.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.4.0/tests/test_init.py` & `mokkari-2.5.0/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.4.0/tests/test_issues.py` & `mokkari-2.5.0/tests/test_issues.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.4.0/tests/test_publishers.py` & `mokkari-2.5.0/tests/test_publishers.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.4.0/tests/test_role.py` & `mokkari-2.5.0/tests/test_role.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.4.0/tests/test_series.py` & `mokkari-2.5.0/tests/test_series.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.4.0/tests/test_series_type.py` & `mokkari-2.5.0/tests/test_series_type.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.4.0/tests/test_teams.py` & `mokkari-2.5.0/tests/test_teams.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.4.0/tests/testing_mock.sqlite` & `mokkari-2.5.0/tests/testing_mock.sqlite`

 * *Files identical despite different names*

### Comparing `mokkari-2.4.0/PKG-INFO` & `mokkari-2.5.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mokkari
-Version: 2.4.0
+Version: 2.5.0
 Summary: Python wrapper for Metron API
 License: GPL-3.0-or-later
 Keywords: comics,comic,metadata
 Author: Brian Pepple
 Author-email: bdpepple@gmail.com
 Maintainer: Brian Pepple
 Maintainer-email: bdpepple@gmail.com
@@ -20,17 +20,14 @@
 Classifier: Operating System :: POSIX :: BSD
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet
 Provides-Extra: docs
 Requires-Dist: marshmallow (>=3.13.0,<4.0.0)
 Requires-Dist: ratelimit (>=2.2.1,<3.0.0)
 Requires-Dist: requests (>=2.26.0,<3.0.0)
 Requires-Dist: sphinx-rtd-theme (>=0.5.2,<0.6.0) ; extra == "docs"
 Requires-Dist: sphinxcontrib-napoleon (>=0.7,<0.8) ; extra == "docs"
```

