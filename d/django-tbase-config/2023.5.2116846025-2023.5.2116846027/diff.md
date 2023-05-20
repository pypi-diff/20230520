# Comparing `tmp/django_tbase_config-2023.5.2116846025.tar.gz` & `tmp/django_tbase_config-2023.5.2116846027.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_tbase_config-2023.5.2116846025.tar", last modified: Sat May 20 17:09:48 2023, max compression
+gzip compressed data, was "django_tbase_config-2023.5.2116846027.tar", last modified: Sat May 20 17:12:44 2023, max compression
```

## Comparing `django_tbase_config-2023.5.2116846025.tar` & `django_tbase_config-2023.5.2116846027.tar`

### file list

```diff
@@ -1,19 +1,31 @@
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 17:09:48.570776 django_tbase_config-2023.5.2116846025/
--rw-r--r--   0 terry     (1000) terry     (1000)      143 2023-05-20 17:05:28.000000 django_tbase_config-2023.5.2116846025/MANIFEST.in
--rw-r--r--   0 terry     (1000) terry     (1000)     1214 2023-05-20 17:09:48.570776 django_tbase_config-2023.5.2116846025/PKG-INFO
--rw-r--r--   0 terry     (1000) terry     (1000)      864 2023-05-20 16:25:04.000000 django_tbase_config-2023.5.2116846025/README.md
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 17:09:48.570776 django_tbase_config-2023.5.2116846025/django_tbase_config.egg-info/
--rw-r--r--   0 terry     (1000) terry     (1000)     1214 2023-05-20 17:09:48.000000 django_tbase_config-2023.5.2116846025/django_tbase_config.egg-info/PKG-INFO
--rw-r--r--   0 terry     (1000) terry     (1000)      379 2023-05-20 17:09:48.000000 django_tbase_config-2023.5.2116846025/django_tbase_config.egg-info/SOURCES.txt
--rw-r--r--   0 terry     (1000) terry     (1000)        1 2023-05-20 17:09:48.000000 django_tbase_config-2023.5.2116846025/django_tbase_config.egg-info/dependency_links.txt
--rw-r--r--   0 terry     (1000) terry     (1000)       19 2023-05-20 17:09:48.000000 django_tbase_config-2023.5.2116846025/django_tbase_config.egg-info/requires.txt
--rw-r--r--   0 terry     (1000) terry     (1000)       13 2023-05-20 17:09:48.000000 django_tbase_config-2023.5.2116846025/django_tbase_config.egg-info/top_level.txt
--rw-r--r--   0 terry     (1000) terry     (1000)       38 2023-05-20 17:09:48.570776 django_tbase_config-2023.5.2116846025/setup.cfg
--rw-r--r--   0 terry     (1000) terry     (1000)     2271 2023-05-20 17:09:29.000000 django_tbase_config-2023.5.2116846025/setup.py
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 17:09:48.570776 django_tbase_config-2023.5.2116846025/tbase_config/
--rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:08.000000 django_tbase_config-2023.5.2116846025/tbase_config/__init__.py
--rw-r--r--   0 terry     (1000) terry     (1000)     1351 2023-04-27 16:40:08.000000 django_tbase_config-2023.5.2116846025/tbase_config/admin.py
--rw-r--r--   0 terry     (1000) terry     (1000)      150 2023-04-27 16:40:08.000000 django_tbase_config-2023.5.2116846025/tbase_config/apps.py
--rw-r--r--   0 terry     (1000) terry     (1000)     2554 2023-04-27 16:40:08.000000 django_tbase_config-2023.5.2116846025/tbase_config/models.py
--rw-r--r--   0 terry     (1000) terry     (1000)       60 2023-04-27 16:40:08.000000 django_tbase_config-2023.5.2116846025/tbase_config/tests.py
--rw-r--r--   0 terry     (1000) terry     (1000)       63 2023-04-27 16:40:08.000000 django_tbase_config-2023.5.2116846025/tbase_config/views.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 17:12:44.890751 django_tbase_config-2023.5.2116846027/
+-rw-r--r--   0 terry     (1000) terry     (1000)      145 2023-05-20 17:12:40.000000 django_tbase_config-2023.5.2116846027/MANIFEST.in
+-rw-r--r--   0 terry     (1000) terry     (1000)     1214 2023-05-20 17:12:44.890751 django_tbase_config-2023.5.2116846027/PKG-INFO
+-rw-r--r--   0 terry     (1000) terry     (1000)      864 2023-05-20 16:25:04.000000 django_tbase_config-2023.5.2116846027/README.md
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 17:12:44.880751 django_tbase_config-2023.5.2116846027/django_tbase_config.egg-info/
+-rw-r--r--   0 terry     (1000) terry     (1000)     1214 2023-05-20 17:12:44.000000 django_tbase_config-2023.5.2116846027/django_tbase_config.egg-info/PKG-INFO
+-rw-r--r--   0 terry     (1000) terry     (1000)      883 2023-05-20 17:12:44.000000 django_tbase_config-2023.5.2116846027/django_tbase_config.egg-info/SOURCES.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)        1 2023-05-20 17:12:44.000000 django_tbase_config-2023.5.2116846027/django_tbase_config.egg-info/dependency_links.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)       19 2023-05-20 17:12:44.000000 django_tbase_config-2023.5.2116846027/django_tbase_config.egg-info/requires.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)       13 2023-05-20 17:12:44.000000 django_tbase_config-2023.5.2116846027/django_tbase_config.egg-info/top_level.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)       38 2023-05-20 17:12:44.890751 django_tbase_config-2023.5.2116846027/setup.cfg
+-rw-r--r--   0 terry     (1000) terry     (1000)     2271 2023-05-20 17:09:29.000000 django_tbase_config-2023.5.2116846027/setup.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 17:12:44.880751 django_tbase_config-2023.5.2116846027/tbase_config/
+-rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:08.000000 django_tbase_config-2023.5.2116846027/tbase_config/__init__.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 17:12:44.880751 django_tbase_config-2023.5.2116846027/tbase_config/__pycache__/
+-rw-r--r--   0 terry     (1000) terry     (1000)      159 2023-04-27 16:50:39.000000 django_tbase_config-2023.5.2116846027/tbase_config/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)      863 2023-04-27 16:50:40.000000 django_tbase_config-2023.5.2116846027/tbase_config/__pycache__/admin.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)      444 2023-04-27 16:50:39.000000 django_tbase_config-2023.5.2116846027/tbase_config/__pycache__/apps.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     1792 2023-04-27 16:50:40.000000 django_tbase_config-2023.5.2116846027/tbase_config/__pycache__/models.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     1351 2023-04-27 16:40:08.000000 django_tbase_config-2023.5.2116846027/tbase_config/admin.py
+-rw-r--r--   0 terry     (1000) terry     (1000)      150 2023-04-27 16:40:08.000000 django_tbase_config-2023.5.2116846027/tbase_config/apps.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 17:12:44.880751 django_tbase_config-2023.5.2116846027/tbase_config/migrations/
+-rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:08.000000 django_tbase_config-2023.5.2116846027/tbase_config/migrations/__init__.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 17:12:44.880751 django_tbase_config-2023.5.2116846027/tbase_config/migrations/__pycache__/
+-rw-r--r--   0 terry     (1000) terry     (1000)     1578 2023-04-27 16:50:46.000000 django_tbase_config-2023.5.2116846027/tbase_config/migrations/__pycache__/0001_initial.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)      635 2023-04-27 16:50:46.000000 django_tbase_config-2023.5.2116846027/tbase_config/migrations/__pycache__/0002_general_copyright.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)      933 2023-04-27 16:53:32.000000 django_tbase_config-2023.5.2116846027/tbase_config/migrations/__pycache__/0003_auto_20230427_1653.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)      170 2023-04-27 16:50:46.000000 django_tbase_config-2023.5.2116846027/tbase_config/migrations/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     2554 2023-04-27 16:40:08.000000 django_tbase_config-2023.5.2116846027/tbase_config/models.py
+-rw-r--r--   0 terry     (1000) terry     (1000)       60 2023-04-27 16:40:08.000000 django_tbase_config-2023.5.2116846027/tbase_config/tests.py
+-rw-r--r--   0 terry     (1000) terry     (1000)       63 2023-04-27 16:40:08.000000 django_tbase_config-2023.5.2116846027/tbase_config/views.py
```

### Comparing `django_tbase_config-2023.5.2116846025/PKG-INFO` & `django_tbase_config-2023.5.2116846027/django_tbase_config.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: django_tbase_config
-Version: 2023.5.2116846025
+Name: django-tbase-config
+Version: 2023.5.2116846027
 Summary: Terry django base config ,
 Home-page: https://terrychanorg.jetbrains.space/p/django-expand/repositories/tbase_config/files/README.md
 Author: Terry Chan
 Author-email: napoler2008@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `django_tbase_config-2023.5.2116846025/README.md` & `django_tbase_config-2023.5.2116846027/README.md`

 * *Files identical despite different names*

### Comparing `django_tbase_config-2023.5.2116846025/django_tbase_config.egg-info/PKG-INFO` & `django_tbase_config-2023.5.2116846027/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: django-tbase-config
-Version: 2023.5.2116846025
+Name: django_tbase_config
+Version: 2023.5.2116846027
 Summary: Terry django base config ,
 Home-page: https://terrychanorg.jetbrains.space/p/django-expand/repositories/tbase_config/files/README.md
 Author: Terry Chan
 Author-email: napoler2008@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `django_tbase_config-2023.5.2116846025/setup.py` & `django_tbase_config-2023.5.2116846027/setup.py`

 * *Files identical despite different names*

### Comparing `django_tbase_config-2023.5.2116846025/tbase_config/admin.py` & `django_tbase_config-2023.5.2116846027/tbase_config/admin.py`

 * *Files identical despite different names*

### Comparing `django_tbase_config-2023.5.2116846025/tbase_config/models.py` & `django_tbase_config-2023.5.2116846027/tbase_config/models.py`

 * *Files identical despite different names*

