# Comparing `tmp/django-xmail-ritual-1.1.1.tar.gz` & `tmp/django-xmail-ritual-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-xmail-ritual-1.1.1.tar", last modified: Sat May 20 04:11:36 2023, max compression
+gzip compressed data, was "django-xmail-ritual-1.1.2.tar", last modified: Sat May 20 19:37:59 2023, max compression
```

## Comparing `django-xmail-ritual-1.1.1.tar` & `django-xmail-ritual-1.1.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:11:36.480232 django-xmail-ritual-1.1.1/
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     7633 2015-03-27 02:46:53.000000 django-xmail-ritual-1.1.1/LICENSE
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      360 2023-05-20 04:11:36.476232 django-xmail-ritual-1.1.1/PKG-INFO
-drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:11:36.472232 django-xmail-ritual-1.1.1/django_xmail_ritual.egg-info/
--rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)      360 2023-05-20 04:11:36.000000 django-xmail-ritual-1.1.1/django_xmail_ritual.egg-info/PKG-INFO
--rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)      968 2023-05-20 04:11:36.000000 django-xmail-ritual-1.1.1/django_xmail_ritual.egg-info/SOURCES.txt
--rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)        1 2023-05-20 04:11:36.000000 django-xmail-ritual-1.1.1/django_xmail_ritual.egg-info/dependency_links.txt
--rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)       35 2023-05-20 04:11:36.000000 django-xmail-ritual-1.1.1/django_xmail_ritual.egg-info/requires.txt
--rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)        9 2023-05-20 04:11:36.000000 django-xmail-ritual-1.1.1/django_xmail_ritual.egg-info/top_level.txt
-drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:11:36.472232 django-xmail-ritual-1.1.1/grimoire/
-drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:11:36.472232 django-xmail-ritual-1.1.1/grimoire/django/
-drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:11:36.476232 django-xmail-ritual-1.1.1/grimoire/django/xmail/
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)       66 2015-04-22 03:19:43.000000 django-xmail-ritual-1.1.1/grimoire/django/xmail/__init__.py
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      907 2023-04-22 04:16:39.000000 django-xmail-ritual-1.1.1/grimoire/django/xmail/admin.py
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      207 2023-04-22 04:02:59.000000 django-xmail-ritual-1.1.1/grimoire/django/xmail/apps.py
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     5985 2020-03-14 18:28:59.000000 django-xmail-ritual-1.1.1/grimoire/django/xmail/backends.py
-drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:11:36.472232 django-xmail-ritual-1.1.1/grimoire/django/xmail/locale/
-drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:11:36.472232 django-xmail-ritual-1.1.1/grimoire/django/xmail/locale/es/
-drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:11:36.476232 django-xmail-ritual-1.1.1/grimoire/django/xmail/locale/es/LC_MESSAGES/
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     2448 2015-04-22 03:41:58.000000 django-xmail-ritual-1.1.1/grimoire/django/xmail/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     2378 2015-04-22 03:41:27.000000 django-xmail-ritual-1.1.1/grimoire/django/xmail/locale/es/LC_MESSAGES/django.po
-drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:11:36.476232 django-xmail-ritual-1.1.1/grimoire/django/xmail/management/
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)        1 2015-03-27 03:05:16.000000 django-xmail-ritual-1.1.1/grimoire/django/xmail/management/__init__.py
-drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:11:36.476232 django-xmail-ritual-1.1.1/grimoire/django/xmail/management/commands/
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)        1 2015-03-27 03:05:16.000000 django-xmail-ritual-1.1.1/grimoire/django/xmail/management/commands/__init__.py
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     3126 2020-03-14 18:22:18.000000 django-xmail-ritual-1.1.1/grimoire/django/xmail/management/commands/send_mails.py
-drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:11:36.476232 django-xmail-ritual-1.1.1/grimoire/django/xmail/migrations/
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     2082 2015-04-20 01:52:06.000000 django-xmail-ritual-1.1.1/grimoire/django/xmail/migrations/0001_initial.py
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      428 2015-04-20 02:20:40.000000 django-xmail-ritual-1.1.1/grimoire/django/xmail/migrations/0002_auto_20150419_2120.py
--rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)      624 2020-03-19 05:09:17.000000 django-xmail-ritual-1.1.1/grimoire/django/xmail/migrations/0003_auto_20200319_0009.py
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      448 2023-04-22 18:43:27.000000 django-xmail-ritual-1.1.1/grimoire/django/xmail/migrations/0004_alter_asyncemailentry_id.py
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)        0 2015-03-14 00:17:24.000000 django-xmail-ritual-1.1.1/grimoire/django/xmail/migrations/__init__.py
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     5966 2023-04-22 04:03:36.000000 django-xmail-ritual-1.1.1/grimoire/django/xmail/models.py
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      314 2020-03-14 18:28:59.000000 django-xmail-ritual-1.1.1/grimoire/django/xmail/settings.py
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)       38 2023-05-20 04:11:36.480232 django-xmail-ritual-1.1.1/setup.cfg
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      783 2023-05-20 04:07:53.000000 django-xmail-ritual-1.1.1/setup.py
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 19:37:59.350996 django-xmail-ritual-1.1.2/
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     7633 2015-03-27 02:46:53.000000 django-xmail-ritual-1.1.2/LICENSE
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      360 2023-05-20 19:37:59.350996 django-xmail-ritual-1.1.2/PKG-INFO
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 19:37:59.350996 django-xmail-ritual-1.1.2/django_xmail_ritual.egg-info/
+-rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)      360 2023-05-20 19:37:59.000000 django-xmail-ritual-1.1.2/django_xmail_ritual.egg-info/PKG-INFO
+-rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)      968 2023-05-20 19:37:59.000000 django-xmail-ritual-1.1.2/django_xmail_ritual.egg-info/SOURCES.txt
+-rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)        1 2023-05-20 19:37:59.000000 django-xmail-ritual-1.1.2/django_xmail_ritual.egg-info/dependency_links.txt
+-rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)       35 2023-05-20 19:37:59.000000 django-xmail-ritual-1.1.2/django_xmail_ritual.egg-info/requires.txt
+-rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)        9 2023-05-20 19:37:59.000000 django-xmail-ritual-1.1.2/django_xmail_ritual.egg-info/top_level.txt
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 19:37:59.350996 django-xmail-ritual-1.1.2/grimoire/
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 19:37:59.350996 django-xmail-ritual-1.1.2/grimoire/django/
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 19:37:59.350996 django-xmail-ritual-1.1.2/grimoire/django/xmail/
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)       66 2015-04-22 03:19:43.000000 django-xmail-ritual-1.1.2/grimoire/django/xmail/__init__.py
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      907 2023-04-22 04:16:39.000000 django-xmail-ritual-1.1.2/grimoire/django/xmail/admin.py
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      207 2023-04-22 04:02:59.000000 django-xmail-ritual-1.1.2/grimoire/django/xmail/apps.py
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     5985 2020-03-14 18:28:59.000000 django-xmail-ritual-1.1.2/grimoire/django/xmail/backends.py
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 19:37:59.350996 django-xmail-ritual-1.1.2/grimoire/django/xmail/locale/
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 19:37:59.350996 django-xmail-ritual-1.1.2/grimoire/django/xmail/locale/es/
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 19:37:59.350996 django-xmail-ritual-1.1.2/grimoire/django/xmail/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     2448 2015-04-22 03:41:58.000000 django-xmail-ritual-1.1.2/grimoire/django/xmail/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     2378 2015-04-22 03:41:27.000000 django-xmail-ritual-1.1.2/grimoire/django/xmail/locale/es/LC_MESSAGES/django.po
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 19:37:59.350996 django-xmail-ritual-1.1.2/grimoire/django/xmail/management/
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)        1 2015-03-27 03:05:16.000000 django-xmail-ritual-1.1.2/grimoire/django/xmail/management/__init__.py
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 19:37:59.350996 django-xmail-ritual-1.1.2/grimoire/django/xmail/management/commands/
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)        1 2015-03-27 03:05:16.000000 django-xmail-ritual-1.1.2/grimoire/django/xmail/management/commands/__init__.py
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     3126 2020-03-14 18:22:18.000000 django-xmail-ritual-1.1.2/grimoire/django/xmail/management/commands/send_mails.py
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 19:37:59.350996 django-xmail-ritual-1.1.2/grimoire/django/xmail/migrations/
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     2082 2015-04-20 01:52:06.000000 django-xmail-ritual-1.1.2/grimoire/django/xmail/migrations/0001_initial.py
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      428 2015-04-20 02:20:40.000000 django-xmail-ritual-1.1.2/grimoire/django/xmail/migrations/0002_auto_20150419_2120.py
+-rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)      624 2020-03-19 05:09:17.000000 django-xmail-ritual-1.1.2/grimoire/django/xmail/migrations/0003_auto_20200319_0009.py
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      448 2023-04-22 18:43:27.000000 django-xmail-ritual-1.1.2/grimoire/django/xmail/migrations/0004_alter_asyncemailentry_id.py
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)        0 2015-03-14 00:17:24.000000 django-xmail-ritual-1.1.2/grimoire/django/xmail/migrations/__init__.py
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     5966 2023-04-22 04:03:36.000000 django-xmail-ritual-1.1.2/grimoire/django/xmail/models.py
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      314 2020-03-14 18:28:59.000000 django-xmail-ritual-1.1.2/grimoire/django/xmail/settings.py
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)       38 2023-05-20 19:37:59.350996 django-xmail-ritual-1.1.2/setup.cfg
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      783 2023-05-20 19:33:09.000000 django-xmail-ritual-1.1.2/setup.py
```

### Comparing `django-xmail-ritual-1.1.1/LICENSE` & `django-xmail-ritual-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-xmail-ritual-1.1.1/django_xmail_ritual.egg-info/SOURCES.txt` & `django-xmail-ritual-1.1.2/django_xmail_ritual.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-xmail-ritual-1.1.1/grimoire/django/xmail/admin.py` & `django-xmail-ritual-1.1.2/grimoire/django/xmail/admin.py`

 * *Files identical despite different names*

### Comparing `django-xmail-ritual-1.1.1/grimoire/django/xmail/backends.py` & `django-xmail-ritual-1.1.2/grimoire/django/xmail/backends.py`

 * *Files identical despite different names*

### Comparing `django-xmail-ritual-1.1.1/grimoire/django/xmail/locale/es/LC_MESSAGES/django.mo` & `django-xmail-ritual-1.1.2/grimoire/django/xmail/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-xmail-ritual-1.1.1/grimoire/django/xmail/locale/es/LC_MESSAGES/django.po` & `django-xmail-ritual-1.1.2/grimoire/django/xmail/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-xmail-ritual-1.1.1/grimoire/django/xmail/management/commands/send_mails.py` & `django-xmail-ritual-1.1.2/grimoire/django/xmail/management/commands/send_mails.py`

 * *Files identical despite different names*

### Comparing `django-xmail-ritual-1.1.1/grimoire/django/xmail/migrations/0001_initial.py` & `django-xmail-ritual-1.1.2/grimoire/django/xmail/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-xmail-ritual-1.1.1/grimoire/django/xmail/migrations/0003_auto_20200319_0009.py` & `django-xmail-ritual-1.1.2/grimoire/django/xmail/migrations/0003_auto_20200319_0009.py`

 * *Files identical despite different names*

### Comparing `django-xmail-ritual-1.1.1/grimoire/django/xmail/models.py` & `django-xmail-ritual-1.1.2/grimoire/django/xmail/models.py`

 * *Files identical despite different names*

### Comparing `django-xmail-ritual-1.1.1/setup.py` & `django-xmail-ritual-1.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='django-xmail-ritual',
-    version='1.1.1',
+    version='1.1.2',
     packages=[
         'grimoire.django.xmail',
         'grimoire.django.xmail.management',
         'grimoire.django.xmail.management.commands',
         'grimoire.django.xmail.migrations',
     ],
     package_data={
@@ -16,9 +16,9 @@
     },
     url='https://github.com/luismasuelli/django-xmail-ritual',
     license='LGPL',
     author='Luis y Anita',
     author_email='luismasuelli@hotmail.com',
     description='The xmail library is a mail dispatching library for Django 2.2 or greater. Mails are sent asynchronously by a '
                 'management command',
-    install_requires=['python-cantrips>=1.0.0', 'Django>=4.2']
+    install_requires=['python-cantrips>=1.0.0', 'Django>=4.0']
 )
```

