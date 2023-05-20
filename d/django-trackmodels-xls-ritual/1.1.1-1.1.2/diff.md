# Comparing `tmp/django-trackmodels-xls-ritual-1.1.1.tar.gz` & `tmp/django-trackmodels-xls-ritual-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-trackmodels-xls-ritual-1.1.1.tar", last modified: Sat May 20 04:10:35 2023, max compression
+gzip compressed data, was "django-trackmodels-xls-ritual-1.1.2.tar", last modified: Sat May 20 19:36:30 2023, max compression
```

## Comparing `django-trackmodels-xls-ritual-1.1.1.tar` & `django-trackmodels-xls-ritual-1.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:10:35.736299 django-trackmodels-xls-ritual-1.1.1/
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     7651 2016-05-23 00:01:21.000000 django-trackmodels-xls-ritual-1.1.1/LICENSE
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      300 2023-05-20 04:10:35.736299 django-trackmodels-xls-ritual-1.1.1/PKG-INFO
-drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:10:35.736299 django-trackmodels-xls-ritual-1.1.1/django_trackmodels_xls_ritual.egg-info/
--rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)      300 2023-05-20 04:10:35.000000 django-trackmodels-xls-ritual-1.1.1/django_trackmodels_xls_ritual.egg-info/PKG-INFO
--rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)      359 2023-05-20 04:10:35.000000 django-trackmodels-xls-ritual-1.1.1/django_trackmodels_xls_ritual.egg-info/SOURCES.txt
--rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)        1 2023-05-20 04:10:35.000000 django-trackmodels-xls-ritual-1.1.1/django_trackmodels_xls_ritual.egg-info/dependency_links.txt
--rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)       63 2023-05-20 04:10:35.000000 django-trackmodels-xls-ritual-1.1.1/django_trackmodels_xls_ritual.egg-info/requires.txt
--rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)        9 2023-05-20 04:10:35.000000 django-trackmodels-xls-ritual-1.1.1/django_trackmodels_xls_ritual.egg-info/top_level.txt
-drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:10:35.736299 django-trackmodels-xls-ritual-1.1.1/grimoire/
-drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:10:35.736299 django-trackmodels-xls-ritual-1.1.1/grimoire/django/
-drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:10:35.736299 django-trackmodels-xls-ritual-1.1.1/grimoire/django/tracked_xls/
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)        1 2016-05-23 00:30:07.000000 django-trackmodels-xls-ritual-1.1.1/grimoire/django/tracked_xls/__init__.py
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     9213 2020-03-14 05:39:36.000000 django-trackmodels-xls-ritual-1.1.1/grimoire/django/tracked_xls/reports.py
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)       38 2023-05-20 04:10:35.736299 django-trackmodels-xls-ritual-1.1.1/setup.cfg
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      474 2023-05-20 04:07:15.000000 django-trackmodels-xls-ritual-1.1.1/setup.py
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 19:36:30.333885 django-trackmodels-xls-ritual-1.1.2/
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     7651 2016-05-23 00:01:21.000000 django-trackmodels-xls-ritual-1.1.2/LICENSE
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      300 2023-05-20 19:36:30.333885 django-trackmodels-xls-ritual-1.1.2/PKG-INFO
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 19:36:30.333885 django-trackmodels-xls-ritual-1.1.2/django_trackmodels_xls_ritual.egg-info/
+-rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)      300 2023-05-20 19:36:30.000000 django-trackmodels-xls-ritual-1.1.2/django_trackmodels_xls_ritual.egg-info/PKG-INFO
+-rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)      359 2023-05-20 19:36:30.000000 django-trackmodels-xls-ritual-1.1.2/django_trackmodels_xls_ritual.egg-info/SOURCES.txt
+-rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)        1 2023-05-20 19:36:30.000000 django-trackmodels-xls-ritual-1.1.2/django_trackmodels_xls_ritual.egg-info/dependency_links.txt
+-rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)       63 2023-05-20 19:36:30.000000 django-trackmodels-xls-ritual-1.1.2/django_trackmodels_xls_ritual.egg-info/requires.txt
+-rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)        9 2023-05-20 19:36:30.000000 django-trackmodels-xls-ritual-1.1.2/django_trackmodels_xls_ritual.egg-info/top_level.txt
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 19:36:30.329885 django-trackmodels-xls-ritual-1.1.2/grimoire/
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 19:36:30.329885 django-trackmodels-xls-ritual-1.1.2/grimoire/django/
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 19:36:30.333885 django-trackmodels-xls-ritual-1.1.2/grimoire/django/tracked_xls/
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)        1 2016-05-23 00:30:07.000000 django-trackmodels-xls-ritual-1.1.2/grimoire/django/tracked_xls/__init__.py
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     9213 2020-03-14 05:39:36.000000 django-trackmodels-xls-ritual-1.1.2/grimoire/django/tracked_xls/reports.py
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)       38 2023-05-20 19:36:30.333885 django-trackmodels-xls-ritual-1.1.2/setup.cfg
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      474 2023-05-20 19:34:39.000000 django-trackmodels-xls-ritual-1.1.2/setup.py
```

### Comparing `django-trackmodels-xls-ritual-1.1.1/LICENSE` & `django-trackmodels-xls-ritual-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-trackmodels-xls-ritual-1.1.1/grimoire/django/tracked_xls/reports.py` & `django-trackmodels-xls-ritual-1.1.2/grimoire/django/tracked_xls/reports.py`

 * *Files identical despite different names*

