# Comparing `tmp/django-dynsettings-ritual-1.0.0.tar.gz` & `tmp/django-dynsettings-ritual-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-dynsettings-ritual-1.0.0.tar", last modified: Sat Mar 14 22:34:26 2020, max compression
+gzip compressed data, was "dist/django-dynsettings-ritual-1.0.1.tar", last modified: Thu Mar 19 05:10:47 2020, max compression
```

## Comparing `django-dynsettings-ritual-1.0.0.tar` & `django-dynsettings-ritual-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 luismasuelli  (1001) luismasuelli  (1001)        0 2020-03-14 22:34:26.291661 django-dynsettings-ritual-1.0.0/
--rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)      454 2020-03-14 22:34:26.287661 django-dynsettings-ritual-1.0.0/PKG-INFO
-drwxr-xr-x   0 luismasuelli  (1001) luismasuelli  (1001)        0 2020-03-14 22:34:26.239662 django-dynsettings-ritual-1.0.0/django_dynsettings_ritual.egg-info/
--rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)      454 2020-03-14 22:34:26.000000 django-dynsettings-ritual-1.0.0/django_dynsettings_ritual.egg-info/PKG-INFO
--rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)      738 2020-03-14 22:34:26.000000 django-dynsettings-ritual-1.0.0/django_dynsettings_ritual.egg-info/SOURCES.txt
--rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)        1 2020-03-14 22:34:26.000000 django-dynsettings-ritual-1.0.0/django_dynsettings_ritual.egg-info/dependency_links.txt
--rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)       76 2020-03-14 22:34:26.000000 django-dynsettings-ritual-1.0.0/django_dynsettings_ritual.egg-info/requires.txt
--rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)        9 2020-03-14 22:34:26.000000 django-dynsettings-ritual-1.0.0/django_dynsettings_ritual.egg-info/top_level.txt
-drwxr-xr-x   0 luismasuelli  (1001) luismasuelli  (1001)        0 2020-03-14 22:34:26.231662 django-dynsettings-ritual-1.0.0/grimoire/
-drwxr-xr-x   0 luismasuelli  (1001) luismasuelli  (1001)        0 2020-03-14 22:34:26.231662 django-dynsettings-ritual-1.0.0/grimoire/django/
-drwxr-xr-x   0 luismasuelli  (1001) luismasuelli  (1001)        0 2020-03-14 22:34:26.267661 django-dynsettings-ritual-1.0.0/grimoire/django/dynsettings/
--rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)       72 2020-03-14 16:07:35.000000 django-dynsettings-ritual-1.0.0/grimoire/django/dynsettings/__init__.py
--rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)     2584 2020-03-14 06:42:28.000000 django-dynsettings-ritual-1.0.0/grimoire/django/dynsettings/admin.py
--rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)      216 2020-03-14 06:42:28.000000 django-dynsettings-ritual-1.0.0/grimoire/django/dynsettings/apps.py
-drwxr-xr-x   0 luismasuelli  (1001) luismasuelli  (1001)        0 2020-03-14 22:34:26.235662 django-dynsettings-ritual-1.0.0/grimoire/django/dynsettings/locale/
-drwxr-xr-x   0 luismasuelli  (1001) luismasuelli  (1001)        0 2020-03-14 22:34:26.235662 django-dynsettings-ritual-1.0.0/grimoire/django/dynsettings/locale/es/
-drwxr-xr-x   0 luismasuelli  (1001) luismasuelli  (1001)        0 2020-03-14 22:34:26.267661 django-dynsettings-ritual-1.0.0/grimoire/django/dynsettings/locale/es/LC_MESSAGES/
--rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)     4626 2020-03-14 06:42:28.000000 django-dynsettings-ritual-1.0.0/grimoire/django/dynsettings/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 luismasuelli  (1001) luismasuelli  (1001)        0 2020-03-14 22:34:26.287661 django-dynsettings-ritual-1.0.0/grimoire/django/dynsettings/migrations/
--rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)     4397 2020-03-14 06:42:28.000000 django-dynsettings-ritual-1.0.0/grimoire/django/dynsettings/migrations/0001_initial.py
--rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)     2508 2020-03-14 06:42:28.000000 django-dynsettings-ritual-1.0.0/grimoire/django/dynsettings/migrations/0002_auto_20150421_2247.py
--rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)      890 2020-03-14 06:42:28.000000 django-dynsettings-ritual-1.0.0/grimoire/django/dynsettings/migrations/0003_auto_20170910_0012.py
--rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)        0 2020-03-14 06:42:28.000000 django-dynsettings-ritual-1.0.0/grimoire/django/dynsettings/migrations/__init__.py
--rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)     5190 2020-03-14 06:42:28.000000 django-dynsettings-ritual-1.0.0/grimoire/django/dynsettings/models.py
--rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)      385 2020-03-14 06:42:28.000000 django-dynsettings-ritual-1.0.0/grimoire/django/dynsettings/utils.py
--rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)       38 2020-03-14 22:34:26.291661 django-dynsettings-ritual-1.0.0/setup.cfg
--rw-rw-r--   0 luismasuelli  (1001) luismasuelli  (1001)      846 2020-03-14 16:35:02.000000 django-dynsettings-ritual-1.0.0/setup.py
+drwxr-xr-x   0 luismasuelli  (1001) luismasuelli  (1001)        0 2020-03-19 05:10:47.090847 django-dynsettings-ritual-1.0.1/
+-rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)      454 2020-03-19 05:10:47.090847 django-dynsettings-ritual-1.0.1/PKG-INFO
+drwxr-xr-x   0 luismasuelli  (1001) luismasuelli  (1001)        0 2020-03-19 05:10:46.754853 django-dynsettings-ritual-1.0.1/django_dynsettings_ritual.egg-info/
+-rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)      454 2020-03-19 05:10:46.000000 django-dynsettings-ritual-1.0.1/django_dynsettings_ritual.egg-info/PKG-INFO
+-rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)      804 2020-03-19 05:10:46.000000 django-dynsettings-ritual-1.0.1/django_dynsettings_ritual.egg-info/SOURCES.txt
+-rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)        1 2020-03-19 05:10:46.000000 django-dynsettings-ritual-1.0.1/django_dynsettings_ritual.egg-info/dependency_links.txt
+-rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)       76 2020-03-19 05:10:46.000000 django-dynsettings-ritual-1.0.1/django_dynsettings_ritual.egg-info/requires.txt
+-rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)        9 2020-03-19 05:10:46.000000 django-dynsettings-ritual-1.0.1/django_dynsettings_ritual.egg-info/top_level.txt
+drwxr-xr-x   0 luismasuelli  (1001) luismasuelli  (1001)        0 2020-03-19 05:10:46.746853 django-dynsettings-ritual-1.0.1/grimoire/
+drwxr-xr-x   0 luismasuelli  (1001) luismasuelli  (1001)        0 2020-03-19 05:10:46.750853 django-dynsettings-ritual-1.0.1/grimoire/django/
+drwxr-xr-x   0 luismasuelli  (1001) luismasuelli  (1001)        0 2020-03-19 05:10:47.034848 django-dynsettings-ritual-1.0.1/grimoire/django/dynsettings/
+-rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)       72 2020-03-14 16:07:35.000000 django-dynsettings-ritual-1.0.1/grimoire/django/dynsettings/__init__.py
+-rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)     2584 2020-03-14 06:42:28.000000 django-dynsettings-ritual-1.0.1/grimoire/django/dynsettings/admin.py
+-rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)      216 2020-03-14 06:42:28.000000 django-dynsettings-ritual-1.0.1/grimoire/django/dynsettings/apps.py
+drwxr-xr-x   0 luismasuelli  (1001) luismasuelli  (1001)        0 2020-03-19 05:10:46.750853 django-dynsettings-ritual-1.0.1/grimoire/django/dynsettings/locale/
+drwxr-xr-x   0 luismasuelli  (1001) luismasuelli  (1001)        0 2020-03-19 05:10:46.750853 django-dynsettings-ritual-1.0.1/grimoire/django/dynsettings/locale/es/
+drwxr-xr-x   0 luismasuelli  (1001) luismasuelli  (1001)        0 2020-03-19 05:10:47.042848 django-dynsettings-ritual-1.0.1/grimoire/django/dynsettings/locale/es/LC_MESSAGES/
+-rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)     4626 2020-03-14 06:42:28.000000 django-dynsettings-ritual-1.0.1/grimoire/django/dynsettings/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 luismasuelli  (1001) luismasuelli  (1001)        0 2020-03-19 05:10:47.086847 django-dynsettings-ritual-1.0.1/grimoire/django/dynsettings/migrations/
+-rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)     4397 2020-03-14 06:42:28.000000 django-dynsettings-ritual-1.0.1/grimoire/django/dynsettings/migrations/0001_initial.py
+-rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)     2508 2020-03-14 06:42:28.000000 django-dynsettings-ritual-1.0.1/grimoire/django/dynsettings/migrations/0002_auto_20150421_2247.py
+-rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)      890 2020-03-14 06:42:28.000000 django-dynsettings-ritual-1.0.1/grimoire/django/dynsettings/migrations/0003_auto_20170910_0012.py
+-rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)     1808 2020-03-19 05:07:11.000000 django-dynsettings-ritual-1.0.1/grimoire/django/dynsettings/migrations/0004_auto_20200319_0007.py
+-rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)        0 2020-03-14 06:42:28.000000 django-dynsettings-ritual-1.0.1/grimoire/django/dynsettings/migrations/__init__.py
+-rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)     5190 2020-03-14 06:42:28.000000 django-dynsettings-ritual-1.0.1/grimoire/django/dynsettings/models.py
+-rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)      385 2020-03-14 06:42:28.000000 django-dynsettings-ritual-1.0.1/grimoire/django/dynsettings/utils.py
+-rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)       38 2020-03-19 05:10:47.090847 django-dynsettings-ritual-1.0.1/setup.cfg
+-rw-rw-r--   0 luismasuelli  (1001) luismasuelli  (1001)      846 2020-03-19 05:07:49.000000 django-dynsettings-ritual-1.0.1/setup.py
```

### Comparing `django-dynsettings-ritual-1.0.0/django_dynsettings_ritual.egg-info/SOURCES.txt` & `django-dynsettings-ritual-1.0.1/django_dynsettings_ritual.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,8 +9,9 @@
 grimoire/django/dynsettings/apps.py
 grimoire/django/dynsettings/models.py
 grimoire/django/dynsettings/utils.py
 grimoire/django/dynsettings/locale/es/LC_MESSAGES/django.po
 grimoire/django/dynsettings/migrations/0001_initial.py
 grimoire/django/dynsettings/migrations/0002_auto_20150421_2247.py
 grimoire/django/dynsettings/migrations/0003_auto_20170910_0012.py
+grimoire/django/dynsettings/migrations/0004_auto_20200319_0007.py
 grimoire/django/dynsettings/migrations/__init__.py
```

### Comparing `django-dynsettings-ritual-1.0.0/grimoire/django/dynsettings/admin.py` & `django-dynsettings-ritual-1.0.1/grimoire/django/dynsettings/admin.py`

 * *Files identical despite different names*

### Comparing `django-dynsettings-ritual-1.0.0/grimoire/django/dynsettings/locale/es/LC_MESSAGES/django.po` & `django-dynsettings-ritual-1.0.1/grimoire/django/dynsettings/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-dynsettings-ritual-1.0.0/grimoire/django/dynsettings/migrations/0001_initial.py` & `django-dynsettings-ritual-1.0.1/grimoire/django/dynsettings/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-dynsettings-ritual-1.0.0/grimoire/django/dynsettings/migrations/0002_auto_20150421_2247.py` & `django-dynsettings-ritual-1.0.1/grimoire/django/dynsettings/migrations/0002_auto_20150421_2247.py`

 * *Files identical despite different names*

### Comparing `django-dynsettings-ritual-1.0.0/grimoire/django/dynsettings/migrations/0003_auto_20170910_0012.py` & `django-dynsettings-ritual-1.0.1/grimoire/django/dynsettings/migrations/0003_auto_20170910_0012.py`

 * *Files identical despite different names*

### Comparing `django-dynsettings-ritual-1.0.0/grimoire/django/dynsettings/models.py` & `django-dynsettings-ritual-1.0.1/grimoire/django/dynsettings/models.py`

 * *Files identical despite different names*

### Comparing `django-dynsettings-ritual-1.0.0/setup.py` & `django-dynsettings-ritual-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='django-dynsettings-ritual',
-    version='1.0.0',
+    version='1.0.1',
     packages=[
         'grimoire.django.dynsettings',
         'grimoire.django.dynsettings.migrations',
     ],
     package_data={
         'grimoire.django.dynsettings': [
             'locale/*/LC_MESSAGES/*.*'
```

