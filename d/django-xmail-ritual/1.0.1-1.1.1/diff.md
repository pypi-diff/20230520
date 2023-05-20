# Comparing `tmp/django-xmail-ritual-1.0.1.tar.gz` & `tmp/django-xmail-ritual-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-xmail-ritual-1.0.1.tar", last modified: Thu Mar 19 05:10:34 2020, max compression
+gzip compressed data, was "django-xmail-ritual-1.1.1.tar", last modified: Sat May 20 04:11:36 2023, max compression
```

## Comparing `django-xmail-ritual-1.0.1.tar` & `django-xmail-ritual-1.1.1.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxr-xr-x   0 luismasuelli  (1001) luismasuelli  (1001)        0 2020-03-19 05:10:34.351069 django-xmail-ritual-1.0.1/
--rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)      377 2020-03-19 05:10:34.347069 django-xmail-ritual-1.0.1/PKG-INFO
-drwxr-xr-x   0 luismasuelli  (1001) luismasuelli  (1001)        0 2020-03-19 05:10:34.179072 django-xmail-ritual-1.0.1/django_xmail_ritual.egg-info/
--rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)      377 2020-03-19 05:10:34.000000 django-xmail-ritual-1.0.1/django_xmail_ritual.egg-info/PKG-INFO
--rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)      894 2020-03-19 05:10:34.000000 django-xmail-ritual-1.0.1/django_xmail_ritual.egg-info/SOURCES.txt
--rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)        1 2020-03-19 05:10:34.000000 django-xmail-ritual-1.0.1/django_xmail_ritual.egg-info/dependency_links.txt
--rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)       35 2020-03-19 05:10:34.000000 django-xmail-ritual-1.0.1/django_xmail_ritual.egg-info/requires.txt
--rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)        9 2020-03-19 05:10:34.000000 django-xmail-ritual-1.0.1/django_xmail_ritual.egg-info/top_level.txt
-drwxr-xr-x   0 luismasuelli  (1001) luismasuelli  (1001)        0 2020-03-19 05:10:34.171072 django-xmail-ritual-1.0.1/grimoire/
-drwxr-xr-x   0 luismasuelli  (1001) luismasuelli  (1001)        0 2020-03-19 05:10:34.171072 django-xmail-ritual-1.0.1/grimoire/django/
-drwxr-xr-x   0 luismasuelli  (1001) luismasuelli  (1001)        0 2020-03-19 05:10:34.243071 django-xmail-ritual-1.0.1/grimoire/django/xmail/
--rw-rw-r--   0 luismasuelli  (1001) luismasuelli  (1001)       66 2015-04-22 03:19:43.000000 django-xmail-ritual-1.0.1/grimoire/django/xmail/__init__.py
--rw-rw-r--   0 luismasuelli  (1001) luismasuelli  (1001)      908 2020-03-14 18:28:59.000000 django-xmail-ritual-1.0.1/grimoire/django/xmail/admin.py
--rw-rw-r--   0 luismasuelli  (1001) luismasuelli  (1001)      208 2020-03-14 18:28:59.000000 django-xmail-ritual-1.0.1/grimoire/django/xmail/apps.py
--rw-rw-r--   0 luismasuelli  (1001) luismasuelli  (1001)     5985 2020-03-14 18:28:59.000000 django-xmail-ritual-1.0.1/grimoire/django/xmail/backends.py
-drwxr-xr-x   0 luismasuelli  (1001) luismasuelli  (1001)        0 2020-03-19 05:10:34.171072 django-xmail-ritual-1.0.1/grimoire/django/xmail/locale/
-drwxr-xr-x   0 luismasuelli  (1001) luismasuelli  (1001)        0 2020-03-19 05:10:34.171072 django-xmail-ritual-1.0.1/grimoire/django/xmail/locale/es/
-drwxr-xr-x   0 luismasuelli  (1001) luismasuelli  (1001)        0 2020-03-19 05:10:34.251071 django-xmail-ritual-1.0.1/grimoire/django/xmail/locale/es/LC_MESSAGES/
--rw-rw-r--   0 luismasuelli  (1001) luismasuelli  (1001)     2448 2015-04-22 03:41:58.000000 django-xmail-ritual-1.0.1/grimoire/django/xmail/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 luismasuelli  (1001) luismasuelli  (1001)     2378 2015-04-22 03:41:27.000000 django-xmail-ritual-1.0.1/grimoire/django/xmail/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 luismasuelli  (1001) luismasuelli  (1001)        0 2020-03-19 05:10:34.267071 django-xmail-ritual-1.0.1/grimoire/django/xmail/management/
--rw-rw-r--   0 luismasuelli  (1001) luismasuelli  (1001)        1 2015-03-27 03:05:16.000000 django-xmail-ritual-1.0.1/grimoire/django/xmail/management/__init__.py
-drwxr-xr-x   0 luismasuelli  (1001) luismasuelli  (1001)        0 2020-03-19 05:10:34.295070 django-xmail-ritual-1.0.1/grimoire/django/xmail/management/commands/
--rw-rw-r--   0 luismasuelli  (1001) luismasuelli  (1001)        1 2015-03-27 03:05:16.000000 django-xmail-ritual-1.0.1/grimoire/django/xmail/management/commands/__init__.py
--rw-rw-r--   0 luismasuelli  (1001) luismasuelli  (1001)     3126 2020-03-14 18:22:18.000000 django-xmail-ritual-1.0.1/grimoire/django/xmail/management/commands/send_mails.py
-drwxr-xr-x   0 luismasuelli  (1001) luismasuelli  (1001)        0 2020-03-19 05:10:34.347069 django-xmail-ritual-1.0.1/grimoire/django/xmail/migrations/
--rw-rw-r--   0 luismasuelli  (1001) luismasuelli  (1001)     2082 2015-04-20 01:52:06.000000 django-xmail-ritual-1.0.1/grimoire/django/xmail/migrations/0001_initial.py
--rw-rw-r--   0 luismasuelli  (1001) luismasuelli  (1001)      428 2015-04-20 02:20:40.000000 django-xmail-ritual-1.0.1/grimoire/django/xmail/migrations/0002_auto_20150419_2120.py
--rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)      624 2020-03-19 05:09:17.000000 django-xmail-ritual-1.0.1/grimoire/django/xmail/migrations/0003_auto_20200319_0009.py
--rw-rw-r--   0 luismasuelli  (1001) luismasuelli  (1001)        0 2015-03-14 00:17:24.000000 django-xmail-ritual-1.0.1/grimoire/django/xmail/migrations/__init__.py
--rw-rw-r--   0 luismasuelli  (1001) luismasuelli  (1001)     5967 2020-03-14 21:29:31.000000 django-xmail-ritual-1.0.1/grimoire/django/xmail/models.py
--rw-rw-r--   0 luismasuelli  (1001) luismasuelli  (1001)      314 2020-03-14 18:28:59.000000 django-xmail-ritual-1.0.1/grimoire/django/xmail/settings.py
--rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)       38 2020-03-19 05:10:34.351069 django-xmail-ritual-1.0.1/setup.cfg
--rw-rw-r--   0 luismasuelli  (1001) luismasuelli  (1001)      783 2020-03-19 05:09:51.000000 django-xmail-ritual-1.0.1/setup.py
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:11:36.480232 django-xmail-ritual-1.1.1/
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     7633 2015-03-27 02:46:53.000000 django-xmail-ritual-1.1.1/LICENSE
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      360 2023-05-20 04:11:36.476232 django-xmail-ritual-1.1.1/PKG-INFO
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:11:36.472232 django-xmail-ritual-1.1.1/django_xmail_ritual.egg-info/
+-rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)      360 2023-05-20 04:11:36.000000 django-xmail-ritual-1.1.1/django_xmail_ritual.egg-info/PKG-INFO
+-rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)      968 2023-05-20 04:11:36.000000 django-xmail-ritual-1.1.1/django_xmail_ritual.egg-info/SOURCES.txt
+-rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)        1 2023-05-20 04:11:36.000000 django-xmail-ritual-1.1.1/django_xmail_ritual.egg-info/dependency_links.txt
+-rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)       35 2023-05-20 04:11:36.000000 django-xmail-ritual-1.1.1/django_xmail_ritual.egg-info/requires.txt
+-rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)        9 2023-05-20 04:11:36.000000 django-xmail-ritual-1.1.1/django_xmail_ritual.egg-info/top_level.txt
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:11:36.472232 django-xmail-ritual-1.1.1/grimoire/
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:11:36.472232 django-xmail-ritual-1.1.1/grimoire/django/
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:11:36.476232 django-xmail-ritual-1.1.1/grimoire/django/xmail/
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)       66 2015-04-22 03:19:43.000000 django-xmail-ritual-1.1.1/grimoire/django/xmail/__init__.py
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      907 2023-04-22 04:16:39.000000 django-xmail-ritual-1.1.1/grimoire/django/xmail/admin.py
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      207 2023-04-22 04:02:59.000000 django-xmail-ritual-1.1.1/grimoire/django/xmail/apps.py
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     5985 2020-03-14 18:28:59.000000 django-xmail-ritual-1.1.1/grimoire/django/xmail/backends.py
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:11:36.472232 django-xmail-ritual-1.1.1/grimoire/django/xmail/locale/
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:11:36.472232 django-xmail-ritual-1.1.1/grimoire/django/xmail/locale/es/
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:11:36.476232 django-xmail-ritual-1.1.1/grimoire/django/xmail/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     2448 2015-04-22 03:41:58.000000 django-xmail-ritual-1.1.1/grimoire/django/xmail/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     2378 2015-04-22 03:41:27.000000 django-xmail-ritual-1.1.1/grimoire/django/xmail/locale/es/LC_MESSAGES/django.po
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:11:36.476232 django-xmail-ritual-1.1.1/grimoire/django/xmail/management/
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)        1 2015-03-27 03:05:16.000000 django-xmail-ritual-1.1.1/grimoire/django/xmail/management/__init__.py
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:11:36.476232 django-xmail-ritual-1.1.1/grimoire/django/xmail/management/commands/
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)        1 2015-03-27 03:05:16.000000 django-xmail-ritual-1.1.1/grimoire/django/xmail/management/commands/__init__.py
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     3126 2020-03-14 18:22:18.000000 django-xmail-ritual-1.1.1/grimoire/django/xmail/management/commands/send_mails.py
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:11:36.476232 django-xmail-ritual-1.1.1/grimoire/django/xmail/migrations/
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     2082 2015-04-20 01:52:06.000000 django-xmail-ritual-1.1.1/grimoire/django/xmail/migrations/0001_initial.py
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      428 2015-04-20 02:20:40.000000 django-xmail-ritual-1.1.1/grimoire/django/xmail/migrations/0002_auto_20150419_2120.py
+-rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)      624 2020-03-19 05:09:17.000000 django-xmail-ritual-1.1.1/grimoire/django/xmail/migrations/0003_auto_20200319_0009.py
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      448 2023-04-22 18:43:27.000000 django-xmail-ritual-1.1.1/grimoire/django/xmail/migrations/0004_alter_asyncemailentry_id.py
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)        0 2015-03-14 00:17:24.000000 django-xmail-ritual-1.1.1/grimoire/django/xmail/migrations/__init__.py
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     5966 2023-04-22 04:03:36.000000 django-xmail-ritual-1.1.1/grimoire/django/xmail/models.py
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      314 2020-03-14 18:28:59.000000 django-xmail-ritual-1.1.1/grimoire/django/xmail/settings.py
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)       38 2023-05-20 04:11:36.480232 django-xmail-ritual-1.1.1/setup.cfg
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      783 2023-05-20 04:07:53.000000 django-xmail-ritual-1.1.1/setup.py
```

### Comparing `django-xmail-ritual-1.0.1/django_xmail_ritual.egg-info/SOURCES.txt` & `django-xmail-ritual-1.1.1/django_xmail_ritual.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 setup.py
 django_xmail_ritual.egg-info/PKG-INFO
 django_xmail_ritual.egg-info/SOURCES.txt
 django_xmail_ritual.egg-info/dependency_links.txt
 django_xmail_ritual.egg-info/requires.txt
 django_xmail_ritual.egg-info/top_level.txt
 grimoire/django/xmail/__init__.py
@@ -14,8 +15,9 @@
 grimoire/django/xmail/locale/es/LC_MESSAGES/django.po
 grimoire/django/xmail/management/__init__.py
 grimoire/django/xmail/management/commands/__init__.py
 grimoire/django/xmail/management/commands/send_mails.py
 grimoire/django/xmail/migrations/0001_initial.py
 grimoire/django/xmail/migrations/0002_auto_20150419_2120.py
 grimoire/django/xmail/migrations/0003_auto_20200319_0009.py
+grimoire/django/xmail/migrations/0004_alter_asyncemailentry_id.py
 grimoire/django/xmail/migrations/__init__.py
```

### Comparing `django-xmail-ritual-1.0.1/grimoire/django/xmail/admin.py` & `django-xmail-ritual-1.1.1/grimoire/django/xmail/admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from django.contrib.admin import site, ModelAdmin
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 from .models import AsyncEmailEntry
 
 
 class AsyncMailAdmin(ModelAdmin):
     """
     No permite editar ni crear pero permite borrar. Muestra un subconjunto de los campos.
     """
```

### Comparing `django-xmail-ritual-1.0.1/grimoire/django/xmail/backends.py` & `django-xmail-ritual-1.1.1/grimoire/django/xmail/backends.py`

 * *Files identical despite different names*

### Comparing `django-xmail-ritual-1.0.1/grimoire/django/xmail/locale/es/LC_MESSAGES/django.mo` & `django-xmail-ritual-1.1.1/grimoire/django/xmail/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-xmail-ritual-1.0.1/grimoire/django/xmail/locale/es/LC_MESSAGES/django.po` & `django-xmail-ritual-1.1.1/grimoire/django/xmail/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-xmail-ritual-1.0.1/grimoire/django/xmail/management/commands/send_mails.py` & `django-xmail-ritual-1.1.1/grimoire/django/xmail/management/commands/send_mails.py`

 * *Files identical despite different names*

### Comparing `django-xmail-ritual-1.0.1/grimoire/django/xmail/migrations/0001_initial.py` & `django-xmail-ritual-1.1.1/grimoire/django/xmail/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-xmail-ritual-1.0.1/grimoire/django/xmail/migrations/0003_auto_20200319_0009.py` & `django-xmail-ritual-1.1.1/grimoire/django/xmail/migrations/0003_auto_20200319_0009.py`

 * *Files identical despite different names*

### Comparing `django-xmail-ritual-1.0.1/grimoire/django/xmail/models.py` & `django-xmail-ritual-1.1.1/grimoire/django/xmail/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from django.db import models
 from base64 import encodebytes, decodebytes
 from pickle import loads, dumps
 from django.utils.timezone import now
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 from .settings import XMAIL_CHUNK_SIZE
 
 
 class AsyncEmailEntryQuerySet(models.QuerySet):
     """
     Queryset capaz de obtener un subconjunto de sus elementos. Se da preferencia a los que hace mucho no son
       intentados y, en caso de empate, a los que hace mucho hayan sido creados.
```

