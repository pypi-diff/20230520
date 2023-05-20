# Comparing `tmp/django-dynsettings-ritual-1.1.1.tar.gz` & `tmp/django-dynsettings-ritual-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-dynsettings-ritual-1.1.1.tar", last modified: Sat May 20 04:11:07 2023, max compression
+gzip compressed data, was "django-dynsettings-ritual-1.1.2.tar", last modified: Sat May 20 19:37:33 2023, max compression
```

## Comparing `django-dynsettings-ritual-1.1.1.tar` & `django-dynsettings-ritual-1.1.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:11:07.664263 django-dynsettings-ritual-1.1.1/
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     7652 2015-04-21 03:01:15.000000 django-dynsettings-ritual-1.1.1/LICENSE
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      437 2023-05-20 04:11:07.664263 django-dynsettings-ritual-1.1.1/PKG-INFO
-drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:11:07.660263 django-dynsettings-ritual-1.1.1/django_dynsettings_ritual.egg-info/
--rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)      437 2023-05-20 04:11:07.000000 django-dynsettings-ritual-1.1.1/django_dynsettings_ritual.egg-info/PKG-INFO
--rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)      980 2023-05-20 04:11:07.000000 django-dynsettings-ritual-1.1.1/django_dynsettings_ritual.egg-info/SOURCES.txt
--rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)        1 2023-05-20 04:11:07.000000 django-dynsettings-ritual-1.1.1/django_dynsettings_ritual.egg-info/dependency_links.txt
--rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)       88 2023-05-20 04:11:07.000000 django-dynsettings-ritual-1.1.1/django_dynsettings_ritual.egg-info/requires.txt
--rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)        9 2023-05-20 04:11:07.000000 django-dynsettings-ritual-1.1.1/django_dynsettings_ritual.egg-info/top_level.txt
-drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:11:07.656263 django-dynsettings-ritual-1.1.1/grimoire/
-drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:11:07.656263 django-dynsettings-ritual-1.1.1/grimoire/django/
-drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:11:07.660263 django-dynsettings-ritual-1.1.1/grimoire/django/dynsettings/
--rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)       72 2020-03-14 16:07:35.000000 django-dynsettings-ritual-1.1.1/grimoire/django/dynsettings/__init__.py
--rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)     2583 2023-04-22 04:16:49.000000 django-dynsettings-ritual-1.1.1/grimoire/django/dynsettings/admin.py
--rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)      215 2023-04-22 04:03:15.000000 django-dynsettings-ritual-1.1.1/grimoire/django/dynsettings/apps.py
-drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:11:07.656263 django-dynsettings-ritual-1.1.1/grimoire/django/dynsettings/locale/
-drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:11:07.656263 django-dynsettings-ritual-1.1.1/grimoire/django/dynsettings/locale/es/
-drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:11:07.660263 django-dynsettings-ritual-1.1.1/grimoire/django/dynsettings/locale/es/LC_MESSAGES/
--rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)     4626 2020-03-14 06:42:28.000000 django-dynsettings-ritual-1.1.1/grimoire/django/dynsettings/locale/es/LC_MESSAGES/django.po
-drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:11:07.664263 django-dynsettings-ritual-1.1.1/grimoire/django/dynsettings/migrations/
--rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)     4397 2020-03-14 06:42:28.000000 django-dynsettings-ritual-1.1.1/grimoire/django/dynsettings/migrations/0001_initial.py
--rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)     2508 2020-03-14 06:42:28.000000 django-dynsettings-ritual-1.1.1/grimoire/django/dynsettings/migrations/0002_auto_20150421_2247.py
--rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)      890 2020-03-14 06:42:28.000000 django-dynsettings-ritual-1.1.1/grimoire/django/dynsettings/migrations/0003_auto_20170910_0012.py
--rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)     1808 2020-03-19 05:07:11.000000 django-dynsettings-ritual-1.1.1/grimoire/django/dynsettings/migrations/0004_auto_20200319_0007.py
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     1124 2023-04-22 18:43:27.000000 django-dynsettings-ritual-1.1.1/grimoire/django/dynsettings/migrations/0005_alter_booleandynamicsetting_value_and_more.py
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      891 2023-05-18 03:28:21.000000 django-dynsettings-ritual-1.1.1/grimoire/django/dynsettings/migrations/0006_alter_jsondynamicsetting_value.py
--rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)        0 2020-03-14 06:42:28.000000 django-dynsettings-ritual-1.1.1/grimoire/django/dynsettings/migrations/__init__.py
--rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)     5193 2023-04-22 21:01:26.000000 django-dynsettings-ritual-1.1.1/grimoire/django/dynsettings/models.py
--rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)      385 2020-03-14 06:42:28.000000 django-dynsettings-ritual-1.1.1/grimoire/django/dynsettings/utils.py
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)       38 2023-05-20 04:11:07.664263 django-dynsettings-ritual-1.1.1/setup.cfg
--rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      861 2023-05-12 02:51:35.000000 django-dynsettings-ritual-1.1.1/setup.py
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 19:37:33.926675 django-dynsettings-ritual-1.1.2/
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     7652 2015-04-21 03:01:15.000000 django-dynsettings-ritual-1.1.2/LICENSE
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      437 2023-05-20 19:37:33.926675 django-dynsettings-ritual-1.1.2/PKG-INFO
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 19:37:33.922675 django-dynsettings-ritual-1.1.2/django_dynsettings_ritual.egg-info/
+-rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)      437 2023-05-20 19:37:33.000000 django-dynsettings-ritual-1.1.2/django_dynsettings_ritual.egg-info/PKG-INFO
+-rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)      980 2023-05-20 19:37:33.000000 django-dynsettings-ritual-1.1.2/django_dynsettings_ritual.egg-info/SOURCES.txt
+-rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)        1 2023-05-20 19:37:33.000000 django-dynsettings-ritual-1.1.2/django_dynsettings_ritual.egg-info/dependency_links.txt
+-rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)       88 2023-05-20 19:37:33.000000 django-dynsettings-ritual-1.1.2/django_dynsettings_ritual.egg-info/requires.txt
+-rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)        9 2023-05-20 19:37:33.000000 django-dynsettings-ritual-1.1.2/django_dynsettings_ritual.egg-info/top_level.txt
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 19:37:33.922675 django-dynsettings-ritual-1.1.2/grimoire/
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 19:37:33.922675 django-dynsettings-ritual-1.1.2/grimoire/django/
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 19:37:33.922675 django-dynsettings-ritual-1.1.2/grimoire/django/dynsettings/
+-rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)       72 2020-03-14 16:07:35.000000 django-dynsettings-ritual-1.1.2/grimoire/django/dynsettings/__init__.py
+-rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)     2583 2023-04-22 04:16:49.000000 django-dynsettings-ritual-1.1.2/grimoire/django/dynsettings/admin.py
+-rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)      215 2023-04-22 04:03:15.000000 django-dynsettings-ritual-1.1.2/grimoire/django/dynsettings/apps.py
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 19:37:33.922675 django-dynsettings-ritual-1.1.2/grimoire/django/dynsettings/locale/
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 19:37:33.922675 django-dynsettings-ritual-1.1.2/grimoire/django/dynsettings/locale/es/
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 19:37:33.922675 django-dynsettings-ritual-1.1.2/grimoire/django/dynsettings/locale/es/LC_MESSAGES/
+-rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)     4626 2020-03-14 06:42:28.000000 django-dynsettings-ritual-1.1.2/grimoire/django/dynsettings/locale/es/LC_MESSAGES/django.po
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 19:37:33.926675 django-dynsettings-ritual-1.1.2/grimoire/django/dynsettings/migrations/
+-rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)     4397 2020-03-14 06:42:28.000000 django-dynsettings-ritual-1.1.2/grimoire/django/dynsettings/migrations/0001_initial.py
+-rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)     2508 2020-03-14 06:42:28.000000 django-dynsettings-ritual-1.1.2/grimoire/django/dynsettings/migrations/0002_auto_20150421_2247.py
+-rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)      890 2020-03-14 06:42:28.000000 django-dynsettings-ritual-1.1.2/grimoire/django/dynsettings/migrations/0003_auto_20170910_0012.py
+-rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)     1808 2020-03-19 05:07:11.000000 django-dynsettings-ritual-1.1.2/grimoire/django/dynsettings/migrations/0004_auto_20200319_0007.py
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     1124 2023-04-22 18:43:27.000000 django-dynsettings-ritual-1.1.2/grimoire/django/dynsettings/migrations/0005_alter_booleandynamicsetting_value_and_more.py
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      891 2023-05-18 03:28:21.000000 django-dynsettings-ritual-1.1.2/grimoire/django/dynsettings/migrations/0006_alter_jsondynamicsetting_value.py
+-rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)        0 2020-03-14 06:42:28.000000 django-dynsettings-ritual-1.1.2/grimoire/django/dynsettings/migrations/__init__.py
+-rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)     5193 2023-04-22 21:01:26.000000 django-dynsettings-ritual-1.1.2/grimoire/django/dynsettings/models.py
+-rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)      385 2020-03-14 06:42:28.000000 django-dynsettings-ritual-1.1.2/grimoire/django/dynsettings/utils.py
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)       38 2023-05-20 19:37:33.926675 django-dynsettings-ritual-1.1.2/setup.cfg
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      861 2023-05-20 19:34:39.000000 django-dynsettings-ritual-1.1.2/setup.py
```

### Comparing `django-dynsettings-ritual-1.1.1/LICENSE` & `django-dynsettings-ritual-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-dynsettings-ritual-1.1.1/django_dynsettings_ritual.egg-info/SOURCES.txt` & `django-dynsettings-ritual-1.1.2/django_dynsettings_ritual.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-dynsettings-ritual-1.1.1/grimoire/django/dynsettings/admin.py` & `django-dynsettings-ritual-1.1.2/grimoire/django/dynsettings/admin.py`

 * *Files identical despite different names*

### Comparing `django-dynsettings-ritual-1.1.1/grimoire/django/dynsettings/locale/es/LC_MESSAGES/django.po` & `django-dynsettings-ritual-1.1.2/grimoire/django/dynsettings/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-dynsettings-ritual-1.1.1/grimoire/django/dynsettings/migrations/0001_initial.py` & `django-dynsettings-ritual-1.1.2/grimoire/django/dynsettings/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-dynsettings-ritual-1.1.1/grimoire/django/dynsettings/migrations/0002_auto_20150421_2247.py` & `django-dynsettings-ritual-1.1.2/grimoire/django/dynsettings/migrations/0002_auto_20150421_2247.py`

 * *Files identical despite different names*

### Comparing `django-dynsettings-ritual-1.1.1/grimoire/django/dynsettings/migrations/0003_auto_20170910_0012.py` & `django-dynsettings-ritual-1.1.2/grimoire/django/dynsettings/migrations/0003_auto_20170910_0012.py`

 * *Files identical despite different names*

### Comparing `django-dynsettings-ritual-1.1.1/grimoire/django/dynsettings/migrations/0004_auto_20200319_0007.py` & `django-dynsettings-ritual-1.1.2/grimoire/django/dynsettings/migrations/0004_auto_20200319_0007.py`

 * *Files identical despite different names*

### Comparing `django-dynsettings-ritual-1.1.1/grimoire/django/dynsettings/migrations/0005_alter_booleandynamicsetting_value_and_more.py` & `django-dynsettings-ritual-1.1.2/grimoire/django/dynsettings/migrations/0005_alter_booleandynamicsetting_value_and_more.py`

 * *Files identical despite different names*

### Comparing `django-dynsettings-ritual-1.1.1/grimoire/django/dynsettings/migrations/0006_alter_jsondynamicsetting_value.py` & `django-dynsettings-ritual-1.1.2/grimoire/django/dynsettings/migrations/0006_alter_jsondynamicsetting_value.py`

 * *Files identical despite different names*

### Comparing `django-dynsettings-ritual-1.1.1/grimoire/django/dynsettings/models.py` & `django-dynsettings-ritual-1.1.2/grimoire/django/dynsettings/models.py`

 * *Files identical despite different names*

### Comparing `django-dynsettings-ritual-1.1.1/setup.py` & `django-dynsettings-ritual-1.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='django-dynsettings-ritual',
-    version='1.1.1',
+    version='1.1.2',
     packages=[
         'grimoire.django.dynsettings',
         'grimoire.django.dynsettings.migrations',
     ],
     package_data={
         'grimoire.django.dynsettings': [
             'locale/*/LC_MESSAGES/*.*'
@@ -15,9 +15,9 @@
     url='https://github.com/luismasuelli/django-dynsettings-ritual',
     license='LGPL',
     author='Luis y Anita',
     author_email='luismasuelli@hotmail.com',
     description='A Django application used to store dynamic settings (i.e. settings beyond the settings.py file), '
                 'and retrieve them via another special object (instead of django.conf.settings, and wrapping it).',
     install_requires=['django-trackmodels-ritual>=1.0.0', 'jsonfield>=3.0.0',
-                      'django-polymorphic>=2.1.2', 'Django>=4.2']
+                      'django-polymorphic>=2.1.2', 'Django>=4.0']
 )
```

