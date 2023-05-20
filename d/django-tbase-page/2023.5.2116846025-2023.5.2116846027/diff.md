# Comparing `tmp/django_tbase_page-2023.5.2116846025.tar.gz` & `tmp/django_tbase_page-2023.5.2116846027.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_tbase_page-2023.5.2116846025.tar", last modified: Sat May 20 17:08:26 2023, max compression
+gzip compressed data, was "django_tbase_page-2023.5.2116846027.tar", last modified: Sat May 20 17:11:42 2023, max compression
```

## Comparing `django_tbase_page-2023.5.2116846025.tar` & `django_tbase_page-2023.5.2116846027.tar`

### file list

```diff
@@ -1,20 +1,52 @@
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 17:08:26.870787 django_tbase_page-2023.5.2116846025/
--rw-r--r--   0 terry     (1000) terry     (1000)      143 2023-05-20 17:05:28.000000 django_tbase_page-2023.5.2116846025/MANIFEST.in
--rw-r--r--   0 terry     (1000) terry     (1000)     1305 2023-05-20 17:08:26.870787 django_tbase_page-2023.5.2116846025/PKG-INFO
--rw-r--r--   0 terry     (1000) terry     (1000)      961 2023-05-20 16:21:34.000000 django_tbase_page-2023.5.2116846025/README.md
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 17:08:26.870787 django_tbase_page-2023.5.2116846025/django_tbase_page.egg-info/
--rw-r--r--   0 terry     (1000) terry     (1000)     1305 2023-05-20 17:08:26.000000 django_tbase_page-2023.5.2116846025/django_tbase_page.egg-info/PKG-INFO
--rw-r--r--   0 terry     (1000) terry     (1000)      376 2023-05-20 17:08:26.000000 django_tbase_page-2023.5.2116846025/django_tbase_page.egg-info/SOURCES.txt
--rw-r--r--   0 terry     (1000) terry     (1000)        1 2023-05-20 17:08:26.000000 django_tbase_page-2023.5.2116846025/django_tbase_page.egg-info/dependency_links.txt
--rw-r--r--   0 terry     (1000) terry     (1000)       62 2023-05-20 17:08:26.000000 django_tbase_page-2023.5.2116846025/django_tbase_page.egg-info/requires.txt
--rw-r--r--   0 terry     (1000) terry     (1000)       11 2023-05-20 17:08:26.000000 django_tbase_page-2023.5.2116846025/django_tbase_page.egg-info/top_level.txt
--rw-r--r--   0 terry     (1000) terry     (1000)       38 2023-05-20 17:08:26.870787 django_tbase_page-2023.5.2116846025/setup.cfg
--rw-r--r--   0 terry     (1000) terry     (1000)     2258 2023-05-20 17:08:12.000000 django_tbase_page-2023.5.2116846025/setup.py
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 17:08:26.870787 django_tbase_page-2023.5.2116846025/tbase_page/
--rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:08.000000 django_tbase_page-2023.5.2116846025/tbase_page/__init__.py
--rw-r--r--   0 terry     (1000) terry     (1000)     2050 2023-05-12 18:40:39.000000 django_tbase_page-2023.5.2116846025/tbase_page/admin.py
--rw-r--r--   0 terry     (1000) terry     (1000)      146 2023-04-27 16:40:08.000000 django_tbase_page-2023.5.2116846025/tbase_page/apps.py
--rw-r--r--   0 terry     (1000) terry     (1000)      645 2023-05-12 18:26:57.000000 django_tbase_page-2023.5.2116846025/tbase_page/models.py
--rw-r--r--   0 terry     (1000) terry     (1000)       60 2023-04-27 16:40:08.000000 django_tbase_page-2023.5.2116846025/tbase_page/tests.py
--rw-r--r--   0 terry     (1000) terry     (1000)      855 2023-04-27 16:40:08.000000 django_tbase_page-2023.5.2116846025/tbase_page/urls.py
--rw-r--r--   0 terry     (1000) terry     (1000)      921 2023-05-12 18:42:44.000000 django_tbase_page-2023.5.2116846025/tbase_page/views.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 17:11:42.780759 django_tbase_page-2023.5.2116846027/
+-rw-r--r--   0 terry     (1000) terry     (1000)      143 2023-05-20 17:11:29.000000 django_tbase_page-2023.5.2116846027/MANIFEST.in
+-rw-r--r--   0 terry     (1000) terry     (1000)     1305 2023-05-20 17:11:42.780759 django_tbase_page-2023.5.2116846027/PKG-INFO
+-rw-r--r--   0 terry     (1000) terry     (1000)      961 2023-05-20 16:21:34.000000 django_tbase_page-2023.5.2116846027/README.md
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 17:11:42.770759 django_tbase_page-2023.5.2116846027/django_tbase_page.egg-info/
+-rw-r--r--   0 terry     (1000) terry     (1000)     1305 2023-05-20 17:11:42.000000 django_tbase_page-2023.5.2116846027/django_tbase_page.egg-info/PKG-INFO
+-rw-r--r--   0 terry     (1000) terry     (1000)     1758 2023-05-20 17:11:42.000000 django_tbase_page-2023.5.2116846027/django_tbase_page.egg-info/SOURCES.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)        1 2023-05-20 17:11:42.000000 django_tbase_page-2023.5.2116846027/django_tbase_page.egg-info/dependency_links.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)       62 2023-05-20 17:11:42.000000 django_tbase_page-2023.5.2116846027/django_tbase_page.egg-info/requires.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)       11 2023-05-20 17:11:42.000000 django_tbase_page-2023.5.2116846027/django_tbase_page.egg-info/top_level.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)       38 2023-05-20 17:11:42.780759 django_tbase_page-2023.5.2116846027/setup.cfg
+-rw-r--r--   0 terry     (1000) terry     (1000)     2258 2023-05-20 17:08:12.000000 django_tbase_page-2023.5.2116846027/setup.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 17:11:42.770759 django_tbase_page-2023.5.2116846027/tbase_page/
+-rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:08.000000 django_tbase_page-2023.5.2116846027/tbase_page/__init__.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 17:11:42.770759 django_tbase_page-2023.5.2116846027/tbase_page/__pycache__/
+-rw-r--r--   0 terry     (1000) terry     (1000)      157 2023-04-27 16:50:39.000000 django_tbase_page-2023.5.2116846027/tbase_page/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)      858 2023-05-12 18:40:40.000000 django_tbase_page-2023.5.2116846027/tbase_page/__pycache__/admin.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)      438 2023-04-27 16:50:39.000000 django_tbase_page-2023.5.2116846027/tbase_page/__pycache__/apps.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)      965 2023-05-12 18:27:52.000000 django_tbase_page-2023.5.2116846027/tbase_page/__pycache__/models.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)      563 2023-04-27 16:50:46.000000 django_tbase_page-2023.5.2116846027/tbase_page/__pycache__/urls.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     1391 2023-05-12 18:42:45.000000 django_tbase_page-2023.5.2116846027/tbase_page/__pycache__/views.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     2050 2023-05-12 18:40:39.000000 django_tbase_page-2023.5.2116846027/tbase_page/admin.py
+-rw-r--r--   0 terry     (1000) terry     (1000)      146 2023-04-27 16:40:08.000000 django_tbase_page-2023.5.2116846027/tbase_page/apps.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 17:11:42.770759 django_tbase_page-2023.5.2116846027/tbase_page/migrations/
+-rw-r--r--   0 terry     (1000) terry     (1000)      788 2023-04-27 16:40:08.000000 django_tbase_page-2023.5.2116846027/tbase_page/migrations/0001_initial.py
+-rw-r--r--   0 terry     (1000) terry     (1000)       94 2023-04-27 16:40:08.000000 django_tbase_page-2023.5.2116846027/tbase_page/migrations/0001_initial.py:Zone.Identifier
+-rw-r--r--   0 terry     (1000) terry     (1000)      908 2023-04-27 16:40:08.000000 django_tbase_page-2023.5.2116846027/tbase_page/migrations/0002_auto_20230421_1307.py
+-rw-r--r--   0 terry     (1000) terry     (1000)       94 2023-04-27 16:40:08.000000 django_tbase_page-2023.5.2116846027/tbase_page/migrations/0002_auto_20230421_1307.py:Zone.Identifier
+-rw-r--r--   0 terry     (1000) terry     (1000)      443 2023-05-12 18:27:53.000000 django_tbase_page-2023.5.2116846027/tbase_page/migrations/0003_basepage_robots_txt.py
+-rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:08.000000 django_tbase_page-2023.5.2116846027/tbase_page/migrations/__init__.py
+-rw-r--r--   0 terry     (1000) terry     (1000)       94 2023-04-27 16:40:08.000000 django_tbase_page-2023.5.2116846027/tbase_page/migrations/__init__.py:Zone.Identifier
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 17:11:42.770759 django_tbase_page-2023.5.2116846027/tbase_page/migrations/__pycache__/
+-rw-r--r--   0 terry     (1000) terry     (1000)      817 2023-04-27 16:50:46.000000 django_tbase_page-2023.5.2116846027/tbase_page/migrations/__pycache__/0001_initial.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)      776 2023-04-27 16:50:46.000000 django_tbase_page-2023.5.2116846027/tbase_page/migrations/__pycache__/0002_auto_20230421_1307.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)      675 2023-05-12 18:28:03.000000 django_tbase_page-2023.5.2116846027/tbase_page/migrations/__pycache__/0003_basepage_robots_txt.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)      168 2023-04-27 16:50:46.000000 django_tbase_page-2023.5.2116846027/tbase_page/migrations/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)      645 2023-05-12 18:26:57.000000 django_tbase_page-2023.5.2116846027/tbase_page/models.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 17:11:42.780759 django_tbase_page-2023.5.2116846027/tbase_page/templates/
+-rw-r--r--   0 terry     (1000) terry     (1000)      253 2023-04-27 16:40:08.000000 django_tbase_page-2023.5.2116846027/tbase_page/templates/about_us.html
+-rw-r--r--   0 terry     (1000) terry     (1000)       94 2023-04-27 16:40:08.000000 django_tbase_page-2023.5.2116846027/tbase_page/templates/about_us.html:Zone.Identifier
+-rw-r--r--   0 terry     (1000) terry     (1000)      257 2023-04-27 16:40:08.000000 django_tbase_page-2023.5.2116846027/tbase_page/templates/contact_us.html
+-rw-r--r--   0 terry     (1000) terry     (1000)       94 2023-04-27 16:40:08.000000 django_tbase_page-2023.5.2116846027/tbase_page/templates/contact_us.html:Zone.Identifier
+-rw-r--r--   0 terry     (1000) terry     (1000)      107 2023-04-27 16:40:08.000000 django_tbase_page-2023.5.2116846027/tbase_page/templates/home.html
+-rw-r--r--   0 terry     (1000) terry     (1000)       94 2023-04-27 16:40:08.000000 django_tbase_page-2023.5.2116846027/tbase_page/templates/home.html:Zone.Identifier
+-rw-r--r--   0 terry     (1000) terry     (1000)      265 2023-04-27 16:40:08.000000 django_tbase_page-2023.5.2116846027/tbase_page/templates/privacy_policy.html
+-rw-r--r--   0 terry     (1000) terry     (1000)       94 2023-04-27 16:40:08.000000 django_tbase_page-2023.5.2116846027/tbase_page/templates/privacy_policy.html:Zone.Identifier
+-rw-r--r--   0 terry     (1000) terry     (1000)      116 2023-05-12 18:50:04.000000 django_tbase_page-2023.5.2116846027/tbase_page/templates/robots_txt.html
+-rw-r--r--   0 terry     (1000) terry     (1000)      275 2023-04-27 16:40:08.000000 django_tbase_page-2023.5.2116846027/tbase_page/templates/terms_and_conditions.html
+-rw-r--r--   0 terry     (1000) terry     (1000)       94 2023-04-27 16:40:08.000000 django_tbase_page-2023.5.2116846027/tbase_page/templates/terms_and_conditions.html:Zone.Identifier
+-rw-r--r--   0 terry     (1000) terry     (1000)       60 2023-04-27 16:40:08.000000 django_tbase_page-2023.5.2116846027/tbase_page/tests.py
+-rw-r--r--   0 terry     (1000) terry     (1000)      855 2023-04-27 16:40:08.000000 django_tbase_page-2023.5.2116846027/tbase_page/urls.py
+-rw-r--r--   0 terry     (1000) terry     (1000)      921 2023-05-12 18:42:44.000000 django_tbase_page-2023.5.2116846027/tbase_page/views.py
```

### Comparing `django_tbase_page-2023.5.2116846025/PKG-INFO` & `django_tbase_page-2023.5.2116846027/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_tbase_page
-Version: 2023.5.2116846025
+Version: 2023.5.2116846027
 Summary: Terry django base post ,
 Home-page: https://terrychanorg.jetbrains.space/p/django-expand/repositories/tbase_page/files/README.md
 Author: Terry Chan
 Author-email: napoler2008@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `django_tbase_page-2023.5.2116846025/README.md` & `django_tbase_page-2023.5.2116846027/README.md`

 * *Files identical despite different names*

### Comparing `django_tbase_page-2023.5.2116846025/django_tbase_page.egg-info/PKG-INFO` & `django_tbase_page-2023.5.2116846027/django_tbase_page.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-tbase-page
-Version: 2023.5.2116846025
+Version: 2023.5.2116846027
 Summary: Terry django base post ,
 Home-page: https://terrychanorg.jetbrains.space/p/django-expand/repositories/tbase_page/files/README.md
 Author: Terry Chan
 Author-email: napoler2008@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `django_tbase_page-2023.5.2116846025/setup.py` & `django_tbase_page-2023.5.2116846027/setup.py`

 * *Files identical despite different names*

### Comparing `django_tbase_page-2023.5.2116846025/tbase_page/admin.py` & `django_tbase_page-2023.5.2116846027/tbase_page/admin.py`

 * *Files identical despite different names*

### Comparing `django_tbase_page-2023.5.2116846025/tbase_page/models.py` & `django_tbase_page-2023.5.2116846027/tbase_page/models.py`

 * *Files identical despite different names*

### Comparing `django_tbase_page-2023.5.2116846025/tbase_page/urls.py` & `django_tbase_page-2023.5.2116846027/tbase_page/urls.py`

 * *Files identical despite different names*

### Comparing `django_tbase_page-2023.5.2116846025/tbase_page/views.py` & `django_tbase_page-2023.5.2116846027/tbase_page/views.py`

 * *Files identical despite different names*

