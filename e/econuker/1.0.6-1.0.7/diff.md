# Comparing `tmp/econuker-1.0.6.tar.gz` & `tmp/econuker-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "econuker-1.0.6.tar", last modified: Sat May 20 15:47:10 2023, max compression
+gzip compressed data, was "econuker-1.0.7.tar", last modified: Sat May 20 19:43:36 2023, max compression
```

## Comparing `econuker-1.0.6.tar` & `econuker-1.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 15:47:10.447713 econuker-1.0.6/
--rw-rw-rw-   0        0        0      819 2023-05-20 15:47:10.446714 econuker-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2612 2023-05-20 01:22:57.000000 econuker-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-20 15:47:10.437711 econuker-1.0.6/econuker/
--rw-rw-rw-   0        0        0     1368 2023-05-19 23:47:34.000000 econuker-1.0.6/econuker/Exceptions.py
--rw-rw-rw-   0        0        0      104 2023-05-20 00:09:50.000000 econuker-1.0.6/econuker/__init__.py
--rw-rw-rw-   0        0        0    14456 2023-05-20 15:46:49.000000 econuker-1.0.6/econuker/async_client.py
--rw-rw-rw-   0        0        0    13947 2023-05-20 15:45:37.000000 econuker-1.0.6/econuker/client.py
-drwxrwxrwx   0        0        0        0 2023-05-20 15:47:10.444710 econuker-1.0.6/econuker.egg-info/
--rw-rw-rw-   0        0        0      819 2023-05-20 15:47:10.000000 econuker-1.0.6/econuker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-05-20 15:47:10.000000 econuker-1.0.6/econuker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 15:47:10.000000 econuker-1.0.6/econuker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-20 15:47:10.000000 econuker-1.0.6/econuker.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-20 15:47:10.000000 econuker-1.0.6/econuker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-20 15:47:10.448712 econuker-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1037 2023-05-20 15:47:02.000000 econuker-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 19:43:36.818910 econuker-1.0.7/
+-rw-rw-rw-   0        0        0     3419 2023-05-20 19:43:36.816911 econuker-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2612 2023-05-20 01:22:57.000000 econuker-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-20 19:43:36.799909 econuker-1.0.7/econuker/
+-rw-rw-rw-   0        0        0     1368 2023-05-19 23:47:34.000000 econuker-1.0.7/econuker/Exceptions.py
+-rw-rw-rw-   0        0        0      104 2023-05-20 00:09:50.000000 econuker-1.0.7/econuker/__init__.py
+-rw-rw-rw-   0        0        0    14456 2023-05-20 15:46:49.000000 econuker-1.0.7/econuker/async_client.py
+-rw-rw-rw-   0        0        0    13947 2023-05-20 15:45:37.000000 econuker-1.0.7/econuker/client.py
+drwxrwxrwx   0        0        0        0 2023-05-20 19:43:36.814909 econuker-1.0.7/econuker.egg-info/
+-rw-rw-rw-   0        0        0     3419 2023-05-20 19:43:36.000000 econuker-1.0.7/econuker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-05-20 19:43:36.000000 econuker-1.0.7/econuker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 19:43:36.000000 econuker-1.0.7/econuker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-20 19:43:36.000000 econuker-1.0.7/econuker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-20 19:43:36.000000 econuker-1.0.7/econuker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-20 19:43:36.818910 econuker-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1165 2023-05-20 19:43:30.000000 econuker-1.0.7/setup.py
```

### Comparing `econuker-1.0.6/README.md` & `econuker-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `econuker-1.0.6/econuker/Exceptions.py` & `econuker-1.0.7/econuker/Exceptions.py`

 * *Files identical despite different names*

### Comparing `econuker-1.0.6/econuker/async_client.py` & `econuker-1.0.7/econuker/async_client.py`

 * *Files identical despite different names*

### Comparing `econuker-1.0.6/econuker/client.py` & `econuker-1.0.7/econuker/client.py`

 * *Files identical despite different names*

