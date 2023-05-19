# Comparing `tmp/hermescloud-0.0.1.tar.gz` & `tmp/hermescloud-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hermescloud-0.0.1.tar", last modified: Fri May 19 22:31:20 2023, max compression
+gzip compressed data, was "hermescloud-0.0.2.tar", last modified: Fri May 19 22:51:17 2023, max compression
```

## Comparing `hermescloud-0.0.1.tar` & `hermescloud-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,16 @@
-drwxr-xr-x   0 tristan    (501) staff       (20)        0 2023-05-19 22:31:20.809861 hermescloud-0.0.1/
--rw-r--r--   0 tristan    (501) staff       (20)     1064 2023-05-06 23:54:25.000000 hermescloud-0.0.1/LICENSE
--rw-r--r--   0 tristan    (501) staff       (20)     4100 2023-05-19 22:31:20.810091 hermescloud-0.0.1/PKG-INFO
--rw-r--r--   0 tristan    (501) staff       (20)     3540 2023-05-07 21:03:33.000000 hermescloud-0.0.1/README.md
--rw-r--r--   0 tristan    (501) staff       (20)       86 2023-05-06 23:49:25.000000 hermescloud-0.0.1/pyproject.toml
--rw-r--r--   0 tristan    (501) staff       (20)      685 2023-05-19 22:31:20.812305 hermescloud-0.0.1/setup.cfg
-drwxr-xr-x   0 tristan    (501) staff       (20)        0 2023-05-19 22:31:20.796095 hermescloud-0.0.1/src/
-drwxr-xr-x   0 tristan    (501) staff       (20)        0 2023-05-19 22:31:20.808741 hermescloud-0.0.1/src/hermescloud.egg-info/
--rw-r--r--   0 tristan    (501) staff       (20)     4100 2023-05-19 22:31:20.000000 hermescloud-0.0.1/src/hermescloud.egg-info/PKG-INFO
--rw-r--r--   0 tristan    (501) staff       (20)      198 2023-05-19 22:31:20.000000 hermescloud-0.0.1/src/hermescloud.egg-info/SOURCES.txt
--rw-r--r--   0 tristan    (501) staff       (20)        1 2023-05-19 22:31:20.000000 hermescloud-0.0.1/src/hermescloud.egg-info/dependency_links.txt
--rw-r--r--   0 tristan    (501) staff       (20)        1 2023-05-19 22:31:20.000000 hermescloud-0.0.1/src/hermescloud.egg-info/top_level.txt
+drwxr-xr-x   0 tristan    (501) staff       (20)        0 2023-05-19 22:51:17.413650 hermescloud-0.0.2/
+-rw-r--r--   0 tristan    (501) staff       (20)     1064 2023-05-06 23:54:25.000000 hermescloud-0.0.2/LICENSE
+-rw-r--r--   0 tristan    (501) staff       (20)    13130 2023-05-19 22:51:17.413972 hermescloud-0.0.2/PKG-INFO
+-rw-r--r--   0 tristan    (501) staff       (20)    12570 2023-05-19 22:42:11.000000 hermescloud-0.0.2/README.md
+-rw-r--r--   0 tristan    (501) staff       (20)       86 2023-05-06 23:49:25.000000 hermescloud-0.0.2/pyproject.toml
+-rw-r--r--   0 tristan    (501) staff       (20)      685 2023-05-19 22:51:17.415277 hermescloud-0.0.2/setup.cfg
+drwxr-xr-x   0 tristan    (501) staff       (20)        0 2023-05-19 22:51:17.395741 hermescloud-0.0.2/src/
+drwxr-xr-x   0 tristan    (501) staff       (20)        0 2023-05-19 22:51:17.407353 hermescloud-0.0.2/src/hermescloud/
+-rw-r--r--   0 tristan    (501) staff       (20)       21 2023-05-19 22:40:17.000000 hermescloud-0.0.2/src/hermescloud/__init__.py
+-rw-r--r--   0 tristan    (501) staff       (20)     8331 2023-05-19 22:21:47.000000 hermescloud-0.0.2/src/hermescloud/hermes.py
+-rw-r--r--   0 tristan    (501) staff       (20)      106 2023-05-06 23:36:50.000000 hermescloud-0.0.2/src/hermescloud/utils.py
+drwxr-xr-x   0 tristan    (501) staff       (20)        0 2023-05-19 22:51:17.413053 hermescloud-0.0.2/src/hermescloud.egg-info/
+-rw-r--r--   0 tristan    (501) staff       (20)    13130 2023-05-19 22:51:17.000000 hermescloud-0.0.2/src/hermescloud.egg-info/PKG-INFO
+-rw-r--r--   0 tristan    (501) staff       (20)      277 2023-05-19 22:51:17.000000 hermescloud-0.0.2/src/hermescloud.egg-info/SOURCES.txt
+-rw-r--r--   0 tristan    (501) staff       (20)        1 2023-05-19 22:51:17.000000 hermescloud-0.0.2/src/hermescloud.egg-info/dependency_links.txt
+-rw-r--r--   0 tristan    (501) staff       (20)       12 2023-05-19 22:51:17.000000 hermescloud-0.0.2/src/hermescloud.egg-info/top_level.txt
```

### Comparing `hermescloud-0.0.1/LICENSE` & `hermescloud-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hermescloud-0.0.1/setup.cfg` & `hermescloud-0.0.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hermescloud
-version = 0.0.1
+version = 0.0.2
 author = Tristan Simpson
 author_email = heytristaann@gmail.com
 description = Extremely fast full-text-search algorithm and caching system
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/realTristan/Hermes/cloud/wrappers/python
 project_urls =
```

