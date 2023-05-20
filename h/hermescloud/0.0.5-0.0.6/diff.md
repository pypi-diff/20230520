# Comparing `tmp/hermescloud-0.0.5.tar.gz` & `tmp/hermescloud-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hermescloud-0.0.5.tar", last modified: Sat May 20 10:27:13 2023, max compression
+gzip compressed data, was "hermescloud-0.0.6.tar", last modified: Sat May 20 11:22:19 2023, max compression
```

## Comparing `hermescloud-0.0.5.tar` & `hermescloud-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 tristan    (501) staff       (20)        0 2023-05-20 10:27:13.765195 hermescloud-0.0.5/
--rw-r--r--   0 tristan    (501) staff       (20)     1064 2023-05-06 23:54:25.000000 hermescloud-0.0.5/LICENSE
--rw-r--r--   0 tristan    (501) staff       (20)    13108 2023-05-20 10:27:13.765621 hermescloud-0.0.5/PKG-INFO
--rw-r--r--   0 tristan    (501) staff       (20)    12570 2023-05-19 22:42:11.000000 hermescloud-0.0.5/README.md
--rw-r--r--   0 tristan    (501) staff       (20)       86 2023-05-06 23:49:25.000000 hermescloud-0.0.5/pyproject.toml
--rw-r--r--   0 tristan    (501) staff       (20)      663 2023-05-20 10:27:13.770496 hermescloud-0.0.5/setup.cfg
-drwxr-xr-x   0 tristan    (501) staff       (20)        0 2023-05-20 10:27:13.745459 hermescloud-0.0.5/src/
-drwxr-xr-x   0 tristan    (501) staff       (20)        0 2023-05-20 10:27:13.756919 hermescloud-0.0.5/src/hermescloud/
--rw-r--r--   0 tristan    (501) staff       (20)       20 2023-05-19 23:39:47.000000 hermescloud-0.0.5/src/hermescloud/__init__.py
--rw-r--r--   0 tristan    (501) staff       (20)     8104 2023-05-20 09:58:15.000000 hermescloud-0.0.5/src/hermescloud/cache.py
--rw-r--r--   0 tristan    (501) staff       (20)      177 2023-05-19 23:15:37.000000 hermescloud-0.0.5/src/hermescloud/utils.py
-drwxr-xr-x   0 tristan    (501) staff       (20)        0 2023-05-20 10:27:13.764349 hermescloud-0.0.5/src/hermescloud.egg-info/
--rw-r--r--   0 tristan    (501) staff       (20)    13108 2023-05-20 10:27:13.000000 hermescloud-0.0.5/src/hermescloud.egg-info/PKG-INFO
--rw-r--r--   0 tristan    (501) staff       (20)      276 2023-05-20 10:27:13.000000 hermescloud-0.0.5/src/hermescloud.egg-info/SOURCES.txt
--rw-r--r--   0 tristan    (501) staff       (20)        1 2023-05-20 10:27:13.000000 hermescloud-0.0.5/src/hermescloud.egg-info/dependency_links.txt
--rw-r--r--   0 tristan    (501) staff       (20)       12 2023-05-20 10:27:13.000000 hermescloud-0.0.5/src/hermescloud.egg-info/top_level.txt
+drwxr-xr-x   0 tristan    (501) staff       (20)        0 2023-05-20 11:22:19.950011 hermescloud-0.0.6/
+-rw-r--r--   0 tristan    (501) staff       (20)     1064 2023-05-06 23:54:25.000000 hermescloud-0.0.6/LICENSE
+-rw-r--r--   0 tristan    (501) staff       (20)    13108 2023-05-20 11:22:19.955262 hermescloud-0.0.6/PKG-INFO
+-rw-r--r--   0 tristan    (501) staff       (20)    12570 2023-05-19 22:42:11.000000 hermescloud-0.0.6/README.md
+-rw-r--r--   0 tristan    (501) staff       (20)       86 2023-05-06 23:49:25.000000 hermescloud-0.0.6/pyproject.toml
+-rw-r--r--   0 tristan    (501) staff       (20)      663 2023-05-20 11:22:19.956606 hermescloud-0.0.6/setup.cfg
+drwxr-xr-x   0 tristan    (501) staff       (20)        0 2023-05-20 11:22:19.930175 hermescloud-0.0.6/src/
+drwxr-xr-x   0 tristan    (501) staff       (20)        0 2023-05-20 11:22:19.940057 hermescloud-0.0.6/src/hermescloud/
+-rw-r--r--   0 tristan    (501) staff       (20)       20 2023-05-19 23:39:47.000000 hermescloud-0.0.6/src/hermescloud/__init__.py
+-rw-r--r--   0 tristan    (501) staff       (20)    11367 2023-05-20 11:10:28.000000 hermescloud-0.0.6/src/hermescloud/cache.py
+-rw-r--r--   0 tristan    (501) staff       (20)      177 2023-05-19 23:15:37.000000 hermescloud-0.0.6/src/hermescloud/utils.py
+drwxr-xr-x   0 tristan    (501) staff       (20)        0 2023-05-20 11:22:19.948373 hermescloud-0.0.6/src/hermescloud.egg-info/
+-rw-r--r--   0 tristan    (501) staff       (20)    13108 2023-05-20 11:22:19.000000 hermescloud-0.0.6/src/hermescloud.egg-info/PKG-INFO
+-rw-r--r--   0 tristan    (501) staff       (20)      276 2023-05-20 11:22:19.000000 hermescloud-0.0.6/src/hermescloud.egg-info/SOURCES.txt
+-rw-r--r--   0 tristan    (501) staff       (20)        1 2023-05-20 11:22:19.000000 hermescloud-0.0.6/src/hermescloud.egg-info/dependency_links.txt
+-rw-r--r--   0 tristan    (501) staff       (20)       12 2023-05-20 11:22:19.000000 hermescloud-0.0.6/src/hermescloud.egg-info/top_level.txt
```

### Comparing `hermescloud-0.0.5/LICENSE` & `hermescloud-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hermescloud-0.0.5/PKG-INFO` & `hermescloud-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hermescloud
-Version: 0.0.5
+Version: 0.0.6
 Summary: Extremely fast full-text-search algorithm and caching system
 Home-page: https://github.com/realTristan/Hermes
 Author: Tristan Simpson
 Author-email: heytristaann@gmail.com
 Project-URL: Bug Tracker, https://github.com/realTristan/Hermes/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hermescloud-0.0.5/README.md` & `hermescloud-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `hermescloud-0.0.5/setup.cfg` & `hermescloud-0.0.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hermescloud
-version = 0.0.5
+version = 0.0.6
 author = Tristan Simpson
 author_email = heytristaann@gmail.com
 description = Extremely fast full-text-search algorithm and caching system
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/realTristan/Hermes
 project_urls =
```

### Comparing `hermescloud-0.0.5/src/hermescloud.egg-info/PKG-INFO` & `hermescloud-0.0.6/src/hermescloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hermescloud
-Version: 0.0.5
+Version: 0.0.6
 Summary: Extremely fast full-text-search algorithm and caching system
 Home-page: https://github.com/realTristan/Hermes
 Author: Tristan Simpson
 Author-email: heytristaann@gmail.com
 Project-URL: Bug Tracker, https://github.com/realTristan/Hermes/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

