# Comparing `tmp/pointstorm-1.1.0.tar.gz` & `tmp/pointstorm-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pointstorm-1.1.0.tar", last modified: Sat Apr 29 22:42:22 2023, max compression
+gzip compressed data, was "pointstorm-1.1.1.tar", last modified: Sat May 20 00:54:41 2023, max compression
```

## Comparing `pointstorm-1.1.0.tar` & `pointstorm-1.1.1.tar`

### file list

```diff
@@ -1,13 +1,26 @@
-drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-04-29 22:42:22.056061 pointstorm-1.1.0/
--rw-r--r--   0 tesfa      (501) staff       (20)    11357 2023-04-16 03:52:15.000000 pointstorm-1.1.0/LICENSE
--rw-r--r--   0 tesfa      (501) staff       (20)      679 2023-04-29 22:42:22.055954 pointstorm-1.1.0/PKG-INFO
--rw-r--r--   0 tesfa      (501) staff       (20)      417 2023-04-29 22:29:18.000000 pointstorm-1.1.0/README.md
-drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-04-29 22:42:22.055800 pointstorm-1.1.0/pointstorm.egg-info/
--rw-r--r--   0 tesfa      (501) staff       (20)      679 2023-04-29 22:42:22.000000 pointstorm-1.1.0/pointstorm.egg-info/PKG-INFO
--rw-r--r--   0 tesfa      (501) staff       (20)      210 2023-04-29 22:42:22.000000 pointstorm-1.1.0/pointstorm.egg-info/SOURCES.txt
--rw-r--r--   0 tesfa      (501) staff       (20)        1 2023-04-29 22:42:22.000000 pointstorm-1.1.0/pointstorm.egg-info/dependency_links.txt
--rw-r--r--   0 tesfa      (501) staff       (20)       94 2023-04-29 22:42:22.000000 pointstorm-1.1.0/pointstorm.egg-info/requires.txt
--rw-r--r--   0 tesfa      (501) staff       (20)        1 2023-04-29 22:42:22.000000 pointstorm-1.1.0/pointstorm.egg-info/top_level.txt
--rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:22:49.000000 pointstorm-1.1.0/pyproject.toml
--rw-r--r--   0 tesfa      (501) staff       (20)       38 2023-04-29 22:42:22.056102 pointstorm-1.1.0/setup.cfg
--rw-r--r--   0 tesfa      (501) staff       (20)      925 2023-04-29 22:41:31.000000 pointstorm-1.1.0/setup.py
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-05-20 00:54:41.617983 pointstorm-1.1.1/
+-rw-r--r--   0 tesfa      (501) staff       (20)    11357 2023-04-16 03:52:15.000000 pointstorm-1.1.1/LICENSE
+-rw-r--r--   0 tesfa      (501) staff       (20)    13918 2023-05-20 00:54:41.617761 pointstorm-1.1.1/PKG-INFO
+-rw-r--r--   0 tesfa      (501) staff       (20)      350 2023-05-20 00:39:15.000000 pointstorm-1.1.1/README.md
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-05-20 00:54:41.615879 pointstorm-1.1.1/pointstorm/
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 03:52:45.000000 pointstorm-1.1.1/pointstorm/__init__.py
+-rw-r--r--   0 tesfa      (501) staff       (20)      363 2023-04-16 22:54:08.000000 pointstorm-1.1.1/pointstorm/config.py
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-05-20 00:54:41.617003 pointstorm-1.1.1/pointstorm/destinations/
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:51:39.000000 pointstorm-1.1.1/pointstorm/destinations/__init__.py
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-05-20 00:54:41.617517 pointstorm-1.1.1/pointstorm/embedding/
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:21:31.000000 pointstorm-1.1.1/pointstorm/embedding/__init__.py
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 22:40:54.000000 pointstorm-1.1.1/pointstorm/embedding/abstract.py
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 22:40:36.000000 pointstorm-1.1.1/pointstorm/embedding/image.py
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 22:40:29.000000 pointstorm-1.1.1/pointstorm/embedding/text.py
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 22:40:42.000000 pointstorm-1.1.1/pointstorm/embedding/time.py
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-16 04:50:18.000000 pointstorm-1.1.1/pointstorm/monitoring.py
+-rw-r--r--   0 tesfa      (501) staff       (20)       62 2023-04-30 00:21:05.000000 pointstorm-1.1.1/pointstorm/reference_db.py
+drwxr-xr-x   0 tesfa      (501) staff       (20)        0 2023-05-20 00:54:41.616829 pointstorm-1.1.1/pointstorm.egg-info/
+-rw-r--r--   0 tesfa      (501) staff       (20)    13918 2023-05-20 00:54:41.000000 pointstorm-1.1.1/pointstorm.egg-info/PKG-INFO
+-rw-r--r--   0 tesfa      (501) staff       (20)      496 2023-05-20 00:54:41.000000 pointstorm-1.1.1/pointstorm.egg-info/SOURCES.txt
+-rw-r--r--   0 tesfa      (501) staff       (20)        1 2023-05-20 00:54:41.000000 pointstorm-1.1.1/pointstorm.egg-info/dependency_links.txt
+-rw-r--r--   0 tesfa      (501) staff       (20)       94 2023-05-20 00:54:41.000000 pointstorm-1.1.1/pointstorm.egg-info/requires.txt
+-rw-r--r--   0 tesfa      (501) staff       (20)       11 2023-05-20 00:54:41.000000 pointstorm-1.1.1/pointstorm.egg-info/top_level.txt
+-rw-r--r--   0 tesfa      (501) staff       (20)        0 2023-04-29 22:22:49.000000 pointstorm-1.1.1/pyproject.toml
+-rw-r--r--   0 tesfa      (501) staff       (20)       38 2023-05-20 00:54:41.618032 pointstorm-1.1.1/setup.cfg
+-rw-r--r--   0 tesfa      (501) staff       (20)     1065 2023-05-20 00:53:14.000000 pointstorm-1.1.1/setup.py
```

### Comparing `pointstorm-1.1.0/LICENSE` & `pointstorm-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pointstorm-1.1.0/setup.py` & `pointstorm-1.1.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 from setuptools import setup, find_packages
 
+version = open('VERSION').read().strip()
+license = open('LICENSE').read().strip()
+
 setup(
     name="pointstorm",
-    version="1.1.0",
-    description="Emebedding vectors for real-time streaming data",
-    author="Tesfa Shenkute",
+    version=version,
+    license=license,
+    description="Embedding vectors for data on the move",
+    long_description=open('README.md').read().strip(),
+    author="xsfa",
     author_email="tesfaaog@gmail.com",
     url="https://github.com/xsfa/pointstorm",
     packages=find_packages(),
     install_requires=[
         'bytewax==0.10.1',
         'requests>=2.28.0',
         'kafka-python==2.0.2',
```

