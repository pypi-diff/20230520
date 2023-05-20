# Comparing `tmp/pointstorm-1.1.1.tar.gz` & `tmp/pointstorm-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pointstorm-1.1.1.tar", last modified: Sat May 20 00:54:41 2023, max compression
+gzip compressed data, was "pointstorm-1.1.2.tar", last modified: Sat May 20 00:59:57 2023, max compression
```

## Comparing `pointstorm-1.1.1.tar` & `pointstorm-1.1.2.tar`

### file list

```diff
@@ -1,26 +1,34 @@
-drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-05-20 00:54:41.617983 pointstorm-1.1.1/
--rw-r--r--   0 tesfa      (501) staff       (20)    11357 2023-04-16 03:52:15.000000 pointstorm-1.1.1/LICENSE
--rw-r--r--   0 tesfa      (501) staff       (20)    13918 2023-05-20 00:54:41.617761 pointstorm-1.1.1/PKG-INFO
--rw-r--r--   0 tesfa      (501) staff       (20)      350 2023-05-20 00:39:15.000000 pointstorm-1.1.1/README.md
-drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-05-20 00:54:41.615879 pointstorm-1.1.1/pointstorm/
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 03:52:45.000000 pointstorm-1.1.1/pointstorm/__init__.py
--rw-r--r--   0 tesfa      (501) staff       (20)      363 2023-04-16 22:54:08.000000 pointstorm-1.1.1/pointstorm/config.py
-drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-05-20 00:54:41.617003 pointstorm-1.1.1/pointstorm/destinations/
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:51:39.000000 pointstorm-1.1.1/pointstorm/destinations/__init__.py
-drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-05-20 00:54:41.617517 pointstorm-1.1.1/pointstorm/embedding/
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:21:31.000000 pointstorm-1.1.1/pointstorm/embedding/__init__.py
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 22:40:54.000000 pointstorm-1.1.1/pointstorm/embedding/abstract.py
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 22:40:36.000000 pointstorm-1.1.1/pointstorm/embedding/image.py
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 22:40:29.000000 pointstorm-1.1.1/pointstorm/embedding/text.py
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 22:40:42.000000 pointstorm-1.1.1/pointstorm/embedding/time.py
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 04:50:18.000000 pointstorm-1.1.1/pointstorm/monitoring.py
--rw-r--r--   0 tesfa      (501) staff       (20)       62 2023-04-30 00:21:05.000000 pointstorm-1.1.1/pointstorm/reference_db.py
-drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-05-20 00:54:41.616829 pointstorm-1.1.1/pointstorm.egg-info/
--rw-r--r--   0 tesfa      (501) staff       (20)    13918 2023-05-20 00:54:41.000000 pointstorm-1.1.1/pointstorm.egg-info/PKG-INFO
--rw-r--r--   0 tesfa      (501) staff       (20)      496 2023-05-20 00:54:41.000000 pointstorm-1.1.1/pointstorm.egg-info/SOURCES.txt
--rw-r--r--   0 tesfa      (501) staff       (20)        1 2023-05-20 00:54:41.000000 pointstorm-1.1.1/pointstorm.egg-info/dependency_links.txt
--rw-r--r--   0 tesfa      (501) staff       (20)       94 2023-05-20 00:54:41.000000 pointstorm-1.1.1/pointstorm.egg-info/requires.txt
--rw-r--r--   0 tesfa      (501) staff       (20)       11 2023-05-20 00:54:41.000000 pointstorm-1.1.1/pointstorm.egg-info/top_level.txt
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:22:49.000000 pointstorm-1.1.1/pyproject.toml
--rw-r--r--   0 tesfa      (501) staff       (20)       38 2023-05-20 00:54:41.618032 pointstorm-1.1.1/setup.cfg
--rw-r--r--   0 tesfa      (501) staff       (20)     1065 2023-05-20 00:53:14.000000 pointstorm-1.1.1/setup.py
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-05-20 00:59:57.143189 pointstorm-1.1.2/
+-rw-r--r--   0 tesfa      (501) staff       (20)    11357 2023-04-16 03:52:15.000000 pointstorm-1.1.2/LICENSE
+-rw-r--r--   0 tesfa      (501) staff       (20)    13918 2023-05-20 00:59:57.142905 pointstorm-1.1.2/PKG-INFO
+-rw-r--r--   0 tesfa      (501) staff       (20)      350 2023-05-20 00:39:15.000000 pointstorm-1.1.2/README.md
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-05-20 00:59:57.140195 pointstorm-1.1.2/pointstorm/
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 03:52:45.000000 pointstorm-1.1.2/pointstorm/__init__.py
+-rw-r--r--   0 tesfa      (501) staff       (20)      363 2023-04-16 22:54:08.000000 pointstorm-1.1.2/pointstorm/config.py
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-05-20 00:59:57.141236 pointstorm-1.1.2/pointstorm/destinations/
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:51:39.000000 pointstorm-1.1.2/pointstorm/destinations/__init__.py
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-05-20 00:59:57.141787 pointstorm-1.1.2/pointstorm/embedding/
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:21:31.000000 pointstorm-1.1.2/pointstorm/embedding/__init__.py
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 22:40:54.000000 pointstorm-1.1.2/pointstorm/embedding/abstract.py
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 22:40:36.000000 pointstorm-1.1.2/pointstorm/embedding/image.py
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 22:40:29.000000 pointstorm-1.1.2/pointstorm/embedding/text.py
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 22:40:42.000000 pointstorm-1.1.2/pointstorm/embedding/time.py
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-05-20 00:59:57.141899 pointstorm-1.1.2/pointstorm/ingestion/
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-05-20 00:59:06.000000 pointstorm-1.1.2/pointstorm/ingestion/__init__.py
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-05-20 00:59:57.142123 pointstorm-1.1.2/pointstorm/ingestion/cdc/
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:50:52.000000 pointstorm-1.1.2/pointstorm/ingestion/cdc/__init__.py
+-rw-r--r--   0 tesfa      (501) staff       (20)       78 2023-04-30 00:19:04.000000 pointstorm-1.1.2/pointstorm/ingestion/cdc/debezium.py
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-05-20 00:59:57.142518 pointstorm-1.1.2/pointstorm/ingestion/event/
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:02:57.000000 pointstorm-1.1.2/pointstorm/ingestion/event/__init__.py
+-rw-r--r--   0 tesfa      (501) staff       (20)     3649 2023-04-29 22:09:21.000000 pointstorm-1.1.2/pointstorm/ingestion/event/kafka.py
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 04:50:18.000000 pointstorm-1.1.2/pointstorm/monitoring.py
+-rw-r--r--   0 tesfa      (501) staff       (20)       62 2023-04-30 00:21:05.000000 pointstorm-1.1.2/pointstorm/reference_db.py
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-05-20 00:59:57.141116 pointstorm-1.1.2/pointstorm.egg-info/
+-rw-r--r--   0 tesfa      (501) staff       (20)    13918 2023-05-20 00:59:57.000000 pointstorm-1.1.2/pointstorm.egg-info/PKG-INFO
+-rw-r--r--   0 tesfa      (501) staff       (20)      678 2023-05-20 00:59:57.000000 pointstorm-1.1.2/pointstorm.egg-info/SOURCES.txt
+-rw-r--r--   0 tesfa      (501) staff       (20)        1 2023-05-20 00:59:57.000000 pointstorm-1.1.2/pointstorm.egg-info/dependency_links.txt
+-rw-r--r--   0 tesfa      (501) staff       (20)       94 2023-05-20 00:59:57.000000 pointstorm-1.1.2/pointstorm.egg-info/requires.txt
+-rw-r--r--   0 tesfa      (501) staff       (20)       11 2023-05-20 00:59:57.000000 pointstorm-1.1.2/pointstorm.egg-info/top_level.txt
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:22:49.000000 pointstorm-1.1.2/pyproject.toml
+-rw-r--r--   0 tesfa      (501) staff       (20)       38 2023-05-20 00:59:57.143276 pointstorm-1.1.2/setup.cfg
+-rw-r--r--   0 tesfa      (501) staff       (20)     1065 2023-05-20 00:53:14.000000 pointstorm-1.1.2/setup.py
```

### Comparing `pointstorm-1.1.1/LICENSE` & `pointstorm-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pointstorm-1.1.1/PKG-INFO` & `pointstorm-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pointstorm
-Version: 1.1.1
+Version: 1.1.2
 Summary: Embedding vectors for data on the move
 Home-page: https://github.com/xsfa/pointstorm
 Author: xsfa
 Author-email: tesfaaog@gmail.com
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `pointstorm-1.1.1/pointstorm.egg-info/PKG-INFO` & `pointstorm-1.1.2/pointstorm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pointstorm
-Version: 1.1.1
+Version: 1.1.2
 Summary: Embedding vectors for data on the move
 Home-page: https://github.com/xsfa/pointstorm
 Author: xsfa
 Author-email: tesfaaog@gmail.com
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `pointstorm-1.1.1/setup.py` & `pointstorm-1.1.2/setup.py`

 * *Files identical despite different names*

