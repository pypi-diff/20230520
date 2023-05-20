# Comparing `tmp/django-trackmodels-ritual-1.1.1.tar.gz` & `tmp/django-trackmodels-ritual-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-trackmodels-ritual-1.1.1.tar", last modified: Sat May 20 04:10:15 2023, max compression
+gzip compressed data, was "django-trackmodels-ritual-1.1.2.tar", last modified: Sat May 20 19:35:52 2023, max compression
```

## Comparing `django-trackmodels-ritual-1.1.1.tar` & `django-trackmodels-ritual-1.1.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:10:15.224324 django-trackmodels-ritual-1.1.1/
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     7652 2015-09-02 02:58:19.000000 django-trackmodels-ritual-1.1.1/LICENSE
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      341 2023-05-20 04:10:15.224324 django-trackmodels-ritual-1.1.1/PKG-INFO
-drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:10:15.220324 django-trackmodels-ritual-1.1.1/django_trackmodels_ritual.egg-info/
--rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)      341 2023-05-20 04:10:15.000000 django-trackmodels-ritual-1.1.1/django_trackmodels_ritual.egg-info/PKG-INFO
--rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)      850 2023-05-20 04:10:15.000000 django-trackmodels-ritual-1.1.1/django_trackmodels_ritual.egg-info/SOURCES.txt
--rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)        1 2023-05-20 04:10:15.000000 django-trackmodels-ritual-1.1.1/django_trackmodels_ritual.egg-info/dependency_links.txt
--rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)       58 2023-05-20 04:10:15.000000 django-trackmodels-ritual-1.1.1/django_trackmodels_ritual.egg-info/requires.txt
--rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)        9 2023-05-20 04:10:15.000000 django-trackmodels-ritual-1.1.1/django_trackmodels_ritual.egg-info/top_level.txt
-drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:10:15.216324 django-trackmodels-ritual-1.1.1/grimoire/
-drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:10:15.216324 django-trackmodels-ritual-1.1.1/grimoire/django/
-drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:10:15.220324 django-trackmodels-ritual-1.1.1/grimoire/django/tracked/
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)        0 2015-09-02 03:16:13.000000 django-trackmodels-ritual-1.1.1/grimoire/django/tracked/__init__.py
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     8600 2023-04-22 04:17:06.000000 django-trackmodels-ritual-1.1.1/grimoire/django/tracked/admin.py
-drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:10:15.216324 django-trackmodels-ritual-1.1.1/grimoire/django/tracked/locale/
-drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:10:15.216324 django-trackmodels-ritual-1.1.1/grimoire/django/tracked/locale/en/
-drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:10:15.220324 django-trackmodels-ritual-1.1.1/grimoire/django/tracked/locale/en/LC_MESSAGES/
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     1678 2015-09-02 05:39:06.000000 django-trackmodels-ritual-1.1.1/grimoire/django/tracked/locale/en/LC_MESSAGES/django.mo
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     3278 2016-05-22 05:32:48.000000 django-trackmodels-ritual-1.1.1/grimoire/django/tracked/locale/en/LC_MESSAGES/django.po
-drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:10:15.216324 django-trackmodels-ritual-1.1.1/grimoire/django/tracked/locale/es/
-drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:10:15.220324 django-trackmodels-ritual-1.1.1/grimoire/django/tracked/locale/es/LC_MESSAGES/
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     1826 2015-09-02 05:39:06.000000 django-trackmodels-ritual-1.1.1/grimoire/django/tracked/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     3461 2016-05-22 05:35:02.000000 django-trackmodels-ritual-1.1.1/grimoire/django/tracked/locale/es/LC_MESSAGES/django.po
-drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:10:15.220324 django-trackmodels-ritual-1.1.1/grimoire/django/tracked/models/
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      235 2017-09-10 02:06:49.000000 django-trackmodels-ritual-1.1.1/grimoire/django/tracked/models/__init__.py
--rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)     9362 2023-04-22 04:03:28.000000 django-trackmodels-ritual-1.1.1/grimoire/django/tracked/models/common.py
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     1214 2020-03-14 02:03:16.000000 django-trackmodels-ritual-1.1.1/grimoire/django/tracked/models/polymorphic.py
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)    13060 2020-03-14 03:05:05.000000 django-trackmodels-ritual-1.1.1/grimoire/django/tracked/reports.py
-drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:10:15.216324 django-trackmodels-ritual-1.1.1/grimoire/django/tracked/templates/
-drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:10:15.220324 django-trackmodels-ritual-1.1.1/grimoire/django/tracked/templates/admin/
-drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:10:15.220324 django-trackmodels-ritual-1.1.1/grimoire/django/tracked/templates/admin/tracked/
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     2207 2016-05-22 05:05:25.000000 django-trackmodels-ritual-1.1.1/grimoire/django/tracked/templates/admin/tracked/change_list.html
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      735 2016-05-21 06:14:52.000000 django-trackmodels-ritual-1.1.1/grimoire/django/tracked/templates/admin/tracking_report_error.html
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)       38 2023-05-20 04:10:15.224324 django-trackmodels-ritual-1.1.1/setup.cfg
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      759 2023-05-20 04:06:38.000000 django-trackmodels-ritual-1.1.1/setup.py
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 19:35:52.421424 django-trackmodels-ritual-1.1.2/
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     7652 2015-09-02 02:58:19.000000 django-trackmodels-ritual-1.1.2/LICENSE
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      341 2023-05-20 19:35:52.421424 django-trackmodels-ritual-1.1.2/PKG-INFO
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 19:35:52.421424 django-trackmodels-ritual-1.1.2/django_trackmodels_ritual.egg-info/
+-rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)      341 2023-05-20 19:35:52.000000 django-trackmodels-ritual-1.1.2/django_trackmodels_ritual.egg-info/PKG-INFO
+-rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)      850 2023-05-20 19:35:52.000000 django-trackmodels-ritual-1.1.2/django_trackmodels_ritual.egg-info/SOURCES.txt
+-rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)        1 2023-05-20 19:35:52.000000 django-trackmodels-ritual-1.1.2/django_trackmodels_ritual.egg-info/dependency_links.txt
+-rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)       58 2023-05-20 19:35:52.000000 django-trackmodels-ritual-1.1.2/django_trackmodels_ritual.egg-info/requires.txt
+-rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)        9 2023-05-20 19:35:52.000000 django-trackmodels-ritual-1.1.2/django_trackmodels_ritual.egg-info/top_level.txt
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 19:35:52.417424 django-trackmodels-ritual-1.1.2/grimoire/
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 19:35:52.417424 django-trackmodels-ritual-1.1.2/grimoire/django/
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 19:35:52.421424 django-trackmodels-ritual-1.1.2/grimoire/django/tracked/
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)        0 2015-09-02 03:16:13.000000 django-trackmodels-ritual-1.1.2/grimoire/django/tracked/__init__.py
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     8600 2023-04-22 04:17:06.000000 django-trackmodels-ritual-1.1.2/grimoire/django/tracked/admin.py
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 19:35:52.417424 django-trackmodels-ritual-1.1.2/grimoire/django/tracked/locale/
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 19:35:52.417424 django-trackmodels-ritual-1.1.2/grimoire/django/tracked/locale/en/
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 19:35:52.421424 django-trackmodels-ritual-1.1.2/grimoire/django/tracked/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     1678 2015-09-02 05:39:06.000000 django-trackmodels-ritual-1.1.2/grimoire/django/tracked/locale/en/LC_MESSAGES/django.mo
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     3278 2016-05-22 05:32:48.000000 django-trackmodels-ritual-1.1.2/grimoire/django/tracked/locale/en/LC_MESSAGES/django.po
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 19:35:52.417424 django-trackmodels-ritual-1.1.2/grimoire/django/tracked/locale/es/
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 19:35:52.421424 django-trackmodels-ritual-1.1.2/grimoire/django/tracked/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     1826 2015-09-02 05:39:06.000000 django-trackmodels-ritual-1.1.2/grimoire/django/tracked/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     3461 2016-05-22 05:35:02.000000 django-trackmodels-ritual-1.1.2/grimoire/django/tracked/locale/es/LC_MESSAGES/django.po
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 19:35:52.421424 django-trackmodels-ritual-1.1.2/grimoire/django/tracked/models/
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      235 2017-09-10 02:06:49.000000 django-trackmodels-ritual-1.1.2/grimoire/django/tracked/models/__init__.py
+-rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)     9362 2023-04-22 04:03:28.000000 django-trackmodels-ritual-1.1.2/grimoire/django/tracked/models/common.py
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     1214 2020-03-14 02:03:16.000000 django-trackmodels-ritual-1.1.2/grimoire/django/tracked/models/polymorphic.py
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)    13060 2020-03-14 03:05:05.000000 django-trackmodels-ritual-1.1.2/grimoire/django/tracked/reports.py
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 19:35:52.417424 django-trackmodels-ritual-1.1.2/grimoire/django/tracked/templates/
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 19:35:52.421424 django-trackmodels-ritual-1.1.2/grimoire/django/tracked/templates/admin/
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 19:35:52.421424 django-trackmodels-ritual-1.1.2/grimoire/django/tracked/templates/admin/tracked/
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     2207 2016-05-22 05:05:25.000000 django-trackmodels-ritual-1.1.2/grimoire/django/tracked/templates/admin/tracked/change_list.html
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      735 2016-05-21 06:14:52.000000 django-trackmodels-ritual-1.1.2/grimoire/django/tracked/templates/admin/tracking_report_error.html
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)       38 2023-05-20 19:35:52.421424 django-trackmodels-ritual-1.1.2/setup.cfg
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      759 2023-05-20 19:34:39.000000 django-trackmodels-ritual-1.1.2/setup.py
```

### Comparing `django-trackmodels-ritual-1.1.1/LICENSE` & `django-trackmodels-ritual-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-trackmodels-ritual-1.1.1/django_trackmodels_ritual.egg-info/SOURCES.txt` & `django-trackmodels-ritual-1.1.2/django_trackmodels_ritual.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-trackmodels-ritual-1.1.1/grimoire/django/tracked/admin.py` & `django-trackmodels-ritual-1.1.2/grimoire/django/tracked/admin.py`

 * *Files identical despite different names*

### Comparing `django-trackmodels-ritual-1.1.1/grimoire/django/tracked/locale/en/LC_MESSAGES/django.mo` & `django-trackmodels-ritual-1.1.2/grimoire/django/tracked/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-trackmodels-ritual-1.1.1/grimoire/django/tracked/locale/en/LC_MESSAGES/django.po` & `django-trackmodels-ritual-1.1.2/grimoire/django/tracked/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-trackmodels-ritual-1.1.1/grimoire/django/tracked/locale/es/LC_MESSAGES/django.mo` & `django-trackmodels-ritual-1.1.2/grimoire/django/tracked/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-trackmodels-ritual-1.1.1/grimoire/django/tracked/locale/es/LC_MESSAGES/django.po` & `django-trackmodels-ritual-1.1.2/grimoire/django/tracked/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-trackmodels-ritual-1.1.1/grimoire/django/tracked/models/common.py` & `django-trackmodels-ritual-1.1.2/grimoire/django/tracked/models/common.py`

 * *Files identical despite different names*

### Comparing `django-trackmodels-ritual-1.1.1/grimoire/django/tracked/models/polymorphic.py` & `django-trackmodels-ritual-1.1.2/grimoire/django/tracked/models/polymorphic.py`

 * *Files identical despite different names*

### Comparing `django-trackmodels-ritual-1.1.1/grimoire/django/tracked/reports.py` & `django-trackmodels-ritual-1.1.2/grimoire/django/tracked/reports.py`

 * *Files identical despite different names*

### Comparing `django-trackmodels-ritual-1.1.1/grimoire/django/tracked/templates/admin/tracked/change_list.html` & `django-trackmodels-ritual-1.1.2/grimoire/django/tracked/templates/admin/tracked/change_list.html`

 * *Files identical despite different names*

### Comparing `django-trackmodels-ritual-1.1.1/grimoire/django/tracked/templates/admin/tracking_report_error.html` & `django-trackmodels-ritual-1.1.2/grimoire/django/tracked/templates/admin/tracking_report_error.html`

 * *Files identical despite different names*

