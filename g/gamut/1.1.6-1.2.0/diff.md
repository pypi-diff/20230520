# Comparing `tmp/gamut-1.1.6.tar.gz` & `tmp/gamut-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gamut-1.1.6.tar", last modified: Fri Mar 10 20:43:18 2023, max compression
+gzip compressed data, was "gamut-1.2.0.tar", last modified: Sat May 20 21:52:45 2023, max compression
```

## Comparing `gamut-1.1.6.tar` & `gamut-1.2.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 felipe-tovar-henao   (501) staff       (20)        0 2023-03-10 20:43:18.149434 gamut-1.1.6/
--rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)      748 2022-01-29 14:56:29.000000 gamut-1.1.6/LICENSE
--rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)       46 2023-03-02 17:06:54.000000 gamut-1.1.6/MANIFEST.in
--rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)     2292 2023-03-10 20:43:18.149016 gamut-1.1.6/PKG-INFO
--rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)     1596 2023-03-04 14:45:27.000000 gamut-1.1.6/README.md
-drwxr-xr-x   0 felipe-tovar-henao   (501) staff       (20)        0 2023-03-10 20:43:18.113087 gamut-1.1.6/docs/
-drwxr-xr-x   0 felipe-tovar-henao   (501) staff       (20)        0 2023-03-10 20:43:18.119370 gamut-1.1.6/docs/source/
--rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)     1937 2023-03-04 14:36:59.000000 gamut-1.1.6/docs/source/conf.py
-drwxr-xr-x   0 felipe-tovar-henao   (501) staff       (20)        0 2023-03-10 20:43:18.130404 gamut-1.1.6/gamut/
--rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)    19822 2023-03-07 15:21:31.000000 gamut-1.1.6/gamut/__init__.py
--rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)       65 2023-02-13 15:32:24.000000 gamut-1.1.6/gamut/__main__.py
--rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)       21 2023-03-10 20:43:07.000000 gamut-1.1.6/gamut/__version__.py
--rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)     4448 2023-03-02 17:06:54.000000 gamut-1.1.6/gamut/audio.py
--rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)     1120 2023-03-04 19:48:52.000000 gamut-1.1.6/gamut/config.py
--rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)     5565 2023-03-02 17:06:54.000000 gamut-1.1.6/gamut/controls.py
--rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)     3965 2023-02-13 15:32:24.000000 gamut-1.1.6/gamut/data.py
--rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)    31431 2023-03-07 15:21:31.000000 gamut-1.1.6/gamut/features.py
-drwxr-xr-x   0 felipe-tovar-henao   (501) staff       (20)        0 2023-03-10 20:43:18.139579 gamut-1.1.6/gamut/gui/
--rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)      812 2023-03-02 17:06:54.000000 gamut-1.1.6/gamut/gui/__gui_init__.py
--rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)     1397 2023-03-04 14:25:59.000000 gamut-1.1.6/gamut/gui/__init__.py
--rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)     3560 2023-03-07 15:21:31.000000 gamut-1.1.6/gamut/gui/audio.py
--rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)     1197 2023-03-03 23:56:46.000000 gamut-1.1.6/gamut/gui/buttons.py
--rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)     2279 2023-03-04 14:25:59.000000 gamut-1.1.6/gamut/gui/config.py
--rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)     7557 2023-03-04 19:48:52.000000 gamut-1.1.6/gamut/gui/corpus.py
-drwxr-xr-x   0 felipe-tovar-henao   (501) staff       (20)        0 2023-03-10 20:43:18.140174 gamut-1.1.6/gamut/gui/data/
--rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)    10244 2023-03-05 01:50:01.000000 gamut-1.1.6/gamut/gui/data/.DS_Store
-drwxr-xr-x   0 felipe-tovar-henao   (501) staff       (20)        0 2023-03-10 20:43:18.140822 gamut-1.1.6/gamut/gui/data/audio/
--rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)    20312 2023-03-04 19:48:52.000000 gamut-1.1.6/gamut/gui/data/audio/silence.mp3
-drwxr-xr-x   0 felipe-tovar-henao   (501) staff       (20)        0 2023-03-10 20:43:18.143197 gamut-1.1.6/gamut/gui/data/images/
--rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)     6148 2023-02-28 14:46:49.000000 gamut-1.1.6/gamut/gui/data/images/.DS_Store
--rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)   121083 2023-03-02 17:06:54.000000 gamut-1.1.6/gamut/gui/data/images/icon.png
--rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)    22746 2023-03-02 17:06:54.000000 gamut-1.1.6/gamut/gui/data/images/logo.png
-drwxr-xr-x   0 felipe-tovar-henao   (501) staff       (20)        0 2023-03-10 20:43:18.147412 gamut-1.1.6/gamut/gui/data/widgets/
--rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)     3496 2023-03-03 18:59:50.000000 gamut-1.1.6/gamut/gui/data/widgets/audio.kv
--rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)     4241 2023-03-04 19:48:52.000000 gamut-1.1.6/gamut/gui/data/widgets/corpus.kv
--rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)     3492 2023-03-10 20:43:07.000000 gamut-1.1.6/gamut/gui/data/widgets/dialogs.kv
--rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)     2907 2023-03-04 14:25:59.000000 gamut-1.1.6/gamut/gui/data/widgets/main.kv
--rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)     2927 2023-03-04 19:48:52.000000 gamut-1.1.6/gamut/gui/data/widgets/mosaic.kv
--rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)      524 2023-03-03 23:56:46.000000 gamut-1.1.6/gamut/gui/data/widgets/param.kv
--rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)     4279 2023-03-03 23:56:46.000000 gamut-1.1.6/gamut/gui/data/widgets/widgets.kv
--rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)     3489 2023-03-07 15:21:31.000000 gamut-1.1.6/gamut/gui/dialogs.py
--rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)     6873 2023-03-04 19:48:52.000000 gamut-1.1.6/gamut/gui/mosaic.py
--rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)     2110 2023-03-03 23:56:46.000000 gamut-1.1.6/gamut/gui/theme.py
--rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)     3194 2023-03-02 17:06:54.000000 gamut-1.1.6/gamut/gui/utils.py
--rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)     4683 2023-03-02 17:06:54.000000 gamut-1.1.6/gamut/sys.py
--rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)     2303 2023-02-24 23:09:28.000000 gamut-1.1.6/gamut/utils.py
-drwxr-xr-x   0 felipe-tovar-henao   (501) staff       (20)        0 2023-03-10 20:43:18.132587 gamut-1.1.6/gamut.egg-info/
--rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)     2292 2023-03-10 20:43:18.000000 gamut-1.1.6/gamut.egg-info/PKG-INFO
--rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)     1034 2023-03-10 20:43:18.000000 gamut-1.1.6/gamut.egg-info/SOURCES.txt
--rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)        1 2023-03-10 20:43:18.000000 gamut-1.1.6/gamut.egg-info/dependency_links.txt
--rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)       57 2023-03-10 20:43:18.000000 gamut-1.1.6/gamut.egg-info/entry_points.txt
--rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)      232 2023-03-10 20:43:18.000000 gamut-1.1.6/gamut.egg-info/requires.txt
--rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)       30 2023-03-10 20:43:18.000000 gamut-1.1.6/gamut.egg-info/top_level.txt
--rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)     1145 2023-03-09 16:07:40.000000 gamut-1.1.6/pyproject.toml
--rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)      231 2023-03-04 00:12:59.000000 gamut-1.1.6/requirements.txt
--rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)       38 2023-03-10 20:43:18.149531 gamut-1.1.6/setup.cfg
--rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)       38 2023-03-09 16:07:40.000000 gamut-1.1.6/setup.py
-drwxr-xr-x   0 felipe-tovar-henao   (501) staff       (20)        0 2023-03-10 20:43:18.147811 gamut-1.1.6/tests/
--rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)      137 2023-03-04 14:28:04.000000 gamut-1.1.6/tests/main.py
+drwxr-xr-x   0 felipe-tovar-henao   (501) staff       (20)        0 2023-05-20 21:52:45.127173 gamut-1.2.0/
+-rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)      748 2022-01-29 14:56:29.000000 gamut-1.2.0/LICENSE
+-rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)       46 2023-03-02 17:06:54.000000 gamut-1.2.0/MANIFEST.in
+-rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)     2292 2023-05-20 21:52:45.126939 gamut-1.2.0/PKG-INFO
+-rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)     1596 2023-03-04 14:45:27.000000 gamut-1.2.0/README.md
+drwxr-xr-x   0 felipe-tovar-henao   (501) staff       (20)        0 2023-05-20 21:52:45.105119 gamut-1.2.0/docs/
+drwxr-xr-x   0 felipe-tovar-henao   (501) staff       (20)        0 2023-05-20 21:52:45.111078 gamut-1.2.0/docs/source/
+-rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)     1937 2023-03-04 14:36:59.000000 gamut-1.2.0/docs/source/conf.py
+drwxr-xr-x   0 felipe-tovar-henao   (501) staff       (20)        0 2023-05-20 21:52:45.115915 gamut-1.2.0/gamut/
+-rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)    19822 2023-03-07 15:21:31.000000 gamut-1.2.0/gamut/__init__.py
+-rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)       65 2023-02-13 15:32:24.000000 gamut-1.2.0/gamut/__main__.py
+-rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)       21 2023-05-20 20:22:42.000000 gamut-1.2.0/gamut/__version__.py
+-rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)     4448 2023-03-02 17:06:54.000000 gamut-1.2.0/gamut/audio.py
+-rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)     1120 2023-03-04 19:48:52.000000 gamut-1.2.0/gamut/config.py
+-rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)     5565 2023-03-02 17:06:54.000000 gamut-1.2.0/gamut/controls.py
+-rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)     3965 2023-02-13 15:32:24.000000 gamut-1.2.0/gamut/data.py
+-rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)    31431 2023-03-07 15:21:31.000000 gamut-1.2.0/gamut/features.py
+drwxr-xr-x   0 felipe-tovar-henao   (501) staff       (20)        0 2023-05-20 21:52:45.120982 gamut-1.2.0/gamut/gui/
+-rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)      812 2023-03-02 17:06:54.000000 gamut-1.2.0/gamut/gui/__gui_init__.py
+-rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)     1397 2023-03-04 14:25:59.000000 gamut-1.2.0/gamut/gui/__init__.py
+-rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)     3560 2023-03-07 15:21:31.000000 gamut-1.2.0/gamut/gui/audio.py
+-rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)     1197 2023-03-03 23:56:46.000000 gamut-1.2.0/gamut/gui/buttons.py
+-rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)     2279 2023-03-04 14:25:59.000000 gamut-1.2.0/gamut/gui/config.py
+-rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)     7557 2023-03-04 19:48:52.000000 gamut-1.2.0/gamut/gui/corpus.py
+drwxr-xr-x   0 felipe-tovar-henao   (501) staff       (20)        0 2023-05-20 21:52:45.121261 gamut-1.2.0/gamut/gui/data/
+-rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)    10244 2023-03-05 01:50:01.000000 gamut-1.2.0/gamut/gui/data/.DS_Store
+drwxr-xr-x   0 felipe-tovar-henao   (501) staff       (20)        0 2023-05-20 21:52:45.121528 gamut-1.2.0/gamut/gui/data/audio/
+-rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)    20312 2023-03-04 19:48:52.000000 gamut-1.2.0/gamut/gui/data/audio/silence.mp3
+drwxr-xr-x   0 felipe-tovar-henao   (501) staff       (20)        0 2023-05-20 21:52:45.122921 gamut-1.2.0/gamut/gui/data/images/
+-rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)     6148 2023-02-28 14:46:49.000000 gamut-1.2.0/gamut/gui/data/images/.DS_Store
+-rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)   121083 2023-03-02 17:06:54.000000 gamut-1.2.0/gamut/gui/data/images/icon.png
+-rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)    22746 2023-03-02 17:06:54.000000 gamut-1.2.0/gamut/gui/data/images/logo.png
+drwxr-xr-x   0 felipe-tovar-henao   (501) staff       (20)        0 2023-05-20 21:52:45.126137 gamut-1.2.0/gamut/gui/data/widgets/
+-rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)     3496 2023-03-03 18:59:50.000000 gamut-1.2.0/gamut/gui/data/widgets/audio.kv
+-rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)     4241 2023-03-04 19:48:52.000000 gamut-1.2.0/gamut/gui/data/widgets/corpus.kv
+-rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)     3492 2023-03-10 20:43:07.000000 gamut-1.2.0/gamut/gui/data/widgets/dialogs.kv
+-rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)     2907 2023-03-04 14:25:59.000000 gamut-1.2.0/gamut/gui/data/widgets/main.kv
+-rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)     2927 2023-03-04 19:48:52.000000 gamut-1.2.0/gamut/gui/data/widgets/mosaic.kv
+-rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)      524 2023-03-03 23:56:46.000000 gamut-1.2.0/gamut/gui/data/widgets/param.kv
+-rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)     4279 2023-03-03 23:56:46.000000 gamut-1.2.0/gamut/gui/data/widgets/widgets.kv
+-rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)     3489 2023-03-07 15:21:31.000000 gamut-1.2.0/gamut/gui/dialogs.py
+-rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)     6873 2023-03-04 19:48:52.000000 gamut-1.2.0/gamut/gui/mosaic.py
+-rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)     2110 2023-03-03 23:56:46.000000 gamut-1.2.0/gamut/gui/theme.py
+-rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)     3194 2023-03-02 17:06:54.000000 gamut-1.2.0/gamut/gui/utils.py
+-rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)     4683 2023-03-02 17:06:54.000000 gamut-1.2.0/gamut/sys.py
+-rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)     2303 2023-02-24 23:09:28.000000 gamut-1.2.0/gamut/utils.py
+drwxr-xr-x   0 felipe-tovar-henao   (501) staff       (20)        0 2023-05-20 21:52:45.118234 gamut-1.2.0/gamut.egg-info/
+-rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)     2292 2023-05-20 21:52:45.000000 gamut-1.2.0/gamut.egg-info/PKG-INFO
+-rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)     1034 2023-05-20 21:52:45.000000 gamut-1.2.0/gamut.egg-info/SOURCES.txt
+-rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)        1 2023-05-20 21:52:45.000000 gamut-1.2.0/gamut.egg-info/dependency_links.txt
+-rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)       57 2023-05-20 21:52:45.000000 gamut-1.2.0/gamut.egg-info/entry_points.txt
+-rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)      232 2023-05-20 21:52:45.000000 gamut-1.2.0/gamut.egg-info/requires.txt
+-rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)       30 2023-05-20 21:52:45.000000 gamut-1.2.0/gamut.egg-info/top_level.txt
+-rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)     1145 2023-03-09 16:07:40.000000 gamut-1.2.0/pyproject.toml
+-rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)      231 2023-05-04 20:05:06.000000 gamut-1.2.0/requirements.txt
+-rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)       38 2023-05-20 21:52:45.127273 gamut-1.2.0/setup.cfg
+-rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)       38 2023-03-09 16:07:40.000000 gamut-1.2.0/setup.py
+drwxr-xr-x   0 felipe-tovar-henao   (501) staff       (20)        0 2023-05-20 21:52:45.126503 gamut-1.2.0/tests/
+-rw-r--r--   0 felipe-tovar-henao   (501) staff       (20)      137 2023-03-04 14:28:04.000000 gamut-1.2.0/tests/main.py
```

### Comparing `gamut-1.1.6/LICENSE` & `gamut-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gamut-1.1.6/PKG-INFO` & `gamut-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gamut
-Version: 1.1.6
+Version: 1.2.0
 Summary: Granular Audio Musaicing Toolkit for Python
 Author-email: Felipe Tovar-Henao <felipe.tovar.henao@gmail.com>
 License: OSI Approved :: ISC License (ISCL)
 Keywords: DSP,audio musaicking,granulation,machine learning,ML,MIR,music,sound design,concatenative synthesis
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Other Audience
 Classifier: Natural Language :: English
```

### Comparing `gamut-1.1.6/README.md` & `gamut-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `gamut-1.1.6/docs/source/conf.py` & `gamut-1.2.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `gamut-1.1.6/gamut/__init__.py` & `gamut-1.2.0/gamut/__init__.py`

 * *Files identical despite different names*

### Comparing `gamut-1.1.6/gamut/audio.py` & `gamut-1.2.0/gamut/audio.py`

 * *Files identical despite different names*

### Comparing `gamut-1.1.6/gamut/config.py` & `gamut-1.2.0/gamut/config.py`

 * *Files identical despite different names*

### Comparing `gamut-1.1.6/gamut/controls.py` & `gamut-1.2.0/gamut/controls.py`

 * *Files identical despite different names*

### Comparing `gamut-1.1.6/gamut/data.py` & `gamut-1.2.0/gamut/data.py`

 * *Files identical despite different names*

### Comparing `gamut-1.1.6/gamut/features.py` & `gamut-1.2.0/gamut/features.py`

 * *Files identical despite different names*

### Comparing `gamut-1.1.6/gamut/gui/__gui_init__.py` & `gamut-1.2.0/gamut/gui/__gui_init__.py`

 * *Files identical despite different names*

### Comparing `gamut-1.1.6/gamut/gui/__init__.py` & `gamut-1.2.0/gamut/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `gamut-1.1.6/gamut/gui/audio.py` & `gamut-1.2.0/gamut/gui/audio.py`

 * *Files identical despite different names*

### Comparing `gamut-1.1.6/gamut/gui/buttons.py` & `gamut-1.2.0/gamut/gui/buttons.py`

 * *Files identical despite different names*

### Comparing `gamut-1.1.6/gamut/gui/config.py` & `gamut-1.2.0/gamut/gui/config.py`

 * *Files identical despite different names*

### Comparing `gamut-1.1.6/gamut/gui/corpus.py` & `gamut-1.2.0/gamut/gui/corpus.py`

 * *Files identical despite different names*

### Comparing `gamut-1.1.6/gamut/gui/data/.DS_Store` & `gamut-1.2.0/gamut/gui/data/.DS_Store`

 * *Files identical despite different names*

### Comparing `gamut-1.1.6/gamut/gui/data/audio/silence.mp3` & `gamut-1.2.0/gamut/gui/data/audio/silence.mp3`

 * *Files identical despite different names*

### Comparing `gamut-1.1.6/gamut/gui/data/images/.DS_Store` & `gamut-1.2.0/gamut/gui/data/images/.DS_Store`

 * *Files identical despite different names*

### Comparing `gamut-1.1.6/gamut/gui/data/images/icon.png` & `gamut-1.2.0/gamut/gui/data/images/icon.png`

 * *Files identical despite different names*

### Comparing `gamut-1.1.6/gamut/gui/data/images/logo.png` & `gamut-1.2.0/gamut/gui/data/images/logo.png`

 * *Files identical despite different names*

### Comparing `gamut-1.1.6/gamut/gui/data/widgets/audio.kv` & `gamut-1.2.0/gamut/gui/data/widgets/audio.kv`

 * *Files identical despite different names*

### Comparing `gamut-1.1.6/gamut/gui/data/widgets/corpus.kv` & `gamut-1.2.0/gamut/gui/data/widgets/corpus.kv`

 * *Files identical despite different names*

### Comparing `gamut-1.1.6/gamut/gui/data/widgets/dialogs.kv` & `gamut-1.2.0/gamut/gui/data/widgets/dialogs.kv`

 * *Files identical despite different names*

### Comparing `gamut-1.1.6/gamut/gui/data/widgets/main.kv` & `gamut-1.2.0/gamut/gui/data/widgets/main.kv`

 * *Files identical despite different names*

### Comparing `gamut-1.1.6/gamut/gui/data/widgets/mosaic.kv` & `gamut-1.2.0/gamut/gui/data/widgets/mosaic.kv`

 * *Files identical despite different names*

### Comparing `gamut-1.1.6/gamut/gui/data/widgets/param.kv` & `gamut-1.2.0/gamut/gui/data/widgets/param.kv`

 * *Files identical despite different names*

### Comparing `gamut-1.1.6/gamut/gui/data/widgets/widgets.kv` & `gamut-1.2.0/gamut/gui/data/widgets/widgets.kv`

 * *Files identical despite different names*

### Comparing `gamut-1.1.6/gamut/gui/dialogs.py` & `gamut-1.2.0/gamut/gui/dialogs.py`

 * *Files identical despite different names*

### Comparing `gamut-1.1.6/gamut/gui/mosaic.py` & `gamut-1.2.0/gamut/gui/mosaic.py`

 * *Files identical despite different names*

### Comparing `gamut-1.1.6/gamut/gui/theme.py` & `gamut-1.2.0/gamut/gui/theme.py`

 * *Files identical despite different names*

### Comparing `gamut-1.1.6/gamut/gui/utils.py` & `gamut-1.2.0/gamut/gui/utils.py`

 * *Files identical despite different names*

### Comparing `gamut-1.1.6/gamut/sys.py` & `gamut-1.2.0/gamut/sys.py`

 * *Files identical despite different names*

### Comparing `gamut-1.1.6/gamut/utils.py` & `gamut-1.2.0/gamut/utils.py`

 * *Files identical despite different names*

### Comparing `gamut-1.1.6/gamut.egg-info/PKG-INFO` & `gamut-1.2.0/gamut.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gamut
-Version: 1.1.6
+Version: 1.2.0
 Summary: Granular Audio Musaicing Toolkit for Python
 Author-email: Felipe Tovar-Henao <felipe.tovar.henao@gmail.com>
 License: OSI Approved :: ISC License (ISCL)
 Keywords: DSP,audio musaicking,granulation,machine learning,ML,MIR,music,sound design,concatenative synthesis
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Other Audience
 Classifier: Natural Language :: English
```

### Comparing `gamut-1.1.6/gamut.egg-info/SOURCES.txt` & `gamut-1.2.0/gamut.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gamut-1.1.6/pyproject.toml` & `gamut-1.2.0/pyproject.toml`

 * *Files identical despite different names*

