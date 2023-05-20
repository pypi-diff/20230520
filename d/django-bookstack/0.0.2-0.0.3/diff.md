# Comparing `tmp/django-bookstack-0.0.2.tar.gz` & `tmp/django-bookstack-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-bookstack-0.0.2.tar", last modified: Fri May 19 19:17:14 2023, max compression
+gzip compressed data, was "django-bookstack-0.0.3.tar", last modified: Sat May 20 17:16:28 2023, max compression
```

## Comparing `django-bookstack-0.0.2.tar` & `django-bookstack-0.0.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:17:14.628420 django-bookstack-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-19 19:17:05.000000 django-bookstack-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-19 19:17:05.000000 django-bookstack-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-19 19:17:14.628420 django-bookstack-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-19 19:17:05.000000 django-bookstack-0.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:17:14.624420 django-bookstack-0.0.2/django_bookstack/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:17:05.000000 django-bookstack-0.0.2/django_bookstack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-19 19:17:05.000000 django-bookstack-0.0.2/django_bookstack/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-19 19:17:05.000000 django-bookstack-0.0.2/django_bookstack/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:17:14.628420 django-bookstack-0.0.2/django_bookstack/bookstack/
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-05-19 19:17:05.000000 django-bookstack-0.0.2/django_bookstack/bookstack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-05-19 19:17:05.000000 django-bookstack-0.0.2/django_bookstack/bookstack/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-05-19 19:17:05.000000 django-bookstack-0.0.2/django_bookstack/bookstack/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:17:14.628420 django-bookstack-0.0.2/django_bookstack/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:17:05.000000 django-bookstack-0.0.2/django_bookstack/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-19 19:17:05.000000 django-bookstack-0.0.2/django_bookstack/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:17:14.624420 django-bookstack-0.0.2/django_bookstack/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:17:14.628420 django-bookstack-0.0.2/django_bookstack/templates/django_bookstack/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-19 19:17:05.000000 django-bookstack-0.0.2/django_bookstack/templates/django_bookstack/bookstack_wrapper.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:17:14.628420 django-bookstack-0.0.2/django_bookstack/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-19 19:17:05.000000 django-bookstack-0.0.2/django_bookstack/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-05-19 19:17:05.000000 django-bookstack-0.0.2/django_bookstack/templatetags/bookstack.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-19 19:17:05.000000 django-bookstack-0.0.2/django_bookstack/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-19 19:17:05.000000 django-bookstack-0.0.2/django_bookstack/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-19 19:17:05.000000 django-bookstack-0.0.2/django_bookstack/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:17:14.628420 django-bookstack-0.0.2/django_bookstack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-19 19:17:14.000000 django-bookstack-0.0.2/django_bookstack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-19 19:17:14.000000 django-bookstack-0.0.2/django_bookstack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 19:17:14.000000 django-bookstack-0.0.2/django_bookstack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-19 19:17:14.000000 django-bookstack-0.0.2/django_bookstack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-19 19:17:14.000000 django-bookstack-0.0.2/django_bookstack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-19 19:17:05.000000 django-bookstack-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-19 19:17:14.628420 django-bookstack-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-19 19:17:05.000000 django-bookstack-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:28.875116 django-bookstack-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-20 17:16:20.000000 django-bookstack-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-20 17:16:20.000000 django-bookstack-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-20 17:16:28.875116 django-bookstack-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-20 17:16:20.000000 django-bookstack-0.0.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:28.875116 django-bookstack-0.0.3/django_bookstack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:20.000000 django-bookstack-0.0.3/django_bookstack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-20 17:16:20.000000 django-bookstack-0.0.3/django_bookstack/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-20 17:16:20.000000 django-bookstack-0.0.3/django_bookstack/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:28.875116 django-bookstack-0.0.3/django_bookstack/bookstack/
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-05-20 17:16:20.000000 django-bookstack-0.0.3/django_bookstack/bookstack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-05-20 17:16:20.000000 django-bookstack-0.0.3/django_bookstack/bookstack/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-05-20 17:16:20.000000 django-bookstack-0.0.3/django_bookstack/bookstack/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:28.875116 django-bookstack-0.0.3/django_bookstack/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:20.000000 django-bookstack-0.0.3/django_bookstack/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-20 17:16:20.000000 django-bookstack-0.0.3/django_bookstack/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:28.871116 django-bookstack-0.0.3/django_bookstack/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:28.875116 django-bookstack-0.0.3/django_bookstack/templates/django_bookstack/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-20 17:16:20.000000 django-bookstack-0.0.3/django_bookstack/templates/django_bookstack/bookstack_wrapper.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:28.875116 django-bookstack-0.0.3/django_bookstack/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-20 17:16:20.000000 django-bookstack-0.0.3/django_bookstack/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-05-20 17:16:20.000000 django-bookstack-0.0.3/django_bookstack/templatetags/bookstack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-20 17:16:20.000000 django-bookstack-0.0.3/django_bookstack/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-20 17:16:20.000000 django-bookstack-0.0.3/django_bookstack/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-20 17:16:20.000000 django-bookstack-0.0.3/django_bookstack/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:28.875116 django-bookstack-0.0.3/django_bookstack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-20 17:16:28.000000 django-bookstack-0.0.3/django_bookstack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-20 17:16:28.000000 django-bookstack-0.0.3/django_bookstack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 17:16:28.000000 django-bookstack-0.0.3/django_bookstack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-20 17:16:28.000000 django-bookstack-0.0.3/django_bookstack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-20 17:16:28.000000 django-bookstack-0.0.3/django_bookstack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-20 17:16:20.000000 django-bookstack-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-20 17:16:28.875116 django-bookstack-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-20 17:16:20.000000 django-bookstack-0.0.3/setup.py
```

### Comparing `django-bookstack-0.0.2/LICENSE` & `django-bookstack-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-bookstack-0.0.2/PKG-INFO` & `django-bookstack-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-bookstack
-Version: 0.0.2
+Version: 0.0.3
 Summary: This project is a integration beteween Bookstack and Django.
 Home-page: https://github.com/jraylan/django-bookstack
 Author: Jefferson Raylan
 Author-email: JRaylan <jeffersonraylan@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/jraylan/django-bookstack
 Project-URL: Bug Tracker, https://github.com/jraylan/django-bookstack/issues
```

### Comparing `django-bookstack-0.0.2/django_bookstack/bookstack/__init__.py` & `django-bookstack-0.0.3/django_bookstack/bookstack/__init__.py`

 * *Files identical despite different names*

### Comparing `django-bookstack-0.0.2/django_bookstack/bookstack/api.py` & `django-bookstack-0.0.3/django_bookstack/bookstack/api.py`

 * *Files identical despite different names*

### Comparing `django-bookstack-0.0.2/django_bookstack/bookstack/utils.py` & `django-bookstack-0.0.3/django_bookstack/bookstack/utils.py`

 * *Files identical despite different names*

### Comparing `django-bookstack-0.0.2/django_bookstack/templatetags/bookstack.py` & `django-bookstack-0.0.3/django_bookstack/templatetags/bookstack.py`

 * *Files identical despite different names*

### Comparing `django-bookstack-0.0.2/django_bookstack/views.py` & `django-bookstack-0.0.3/django_bookstack/views.py`

 * *Files identical despite different names*

### Comparing `django-bookstack-0.0.2/django_bookstack.egg-info/PKG-INFO` & `django-bookstack-0.0.3/django_bookstack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-bookstack
-Version: 0.0.2
+Version: 0.0.3
 Summary: This project is a integration beteween Bookstack and Django.
 Home-page: https://github.com/jraylan/django-bookstack
 Author: Jefferson Raylan
 Author-email: JRaylan <jeffersonraylan@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/jraylan/django-bookstack
 Project-URL: Bug Tracker, https://github.com/jraylan/django-bookstack/issues
```

### Comparing `django-bookstack-0.0.2/django_bookstack.egg-info/SOURCES.txt` & `django-bookstack-0.0.3/django_bookstack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-bookstack-0.0.2/pyproject.toml` & `django-bookstack-0.0.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 [build-system]
 requires = ['setuptools>=40.8.0', 'wheel', 'simplejson']
 build-backend = 'setuptools.build_meta:__legacy__'
 
 [project]
 name = "django-bookstack"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="JRaylan", email="jeffersonraylan@gmail.com" },
 ]
 description = "This project is a integration beteween Bookstack and Django."
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 2",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: Unix",
 ]
 dependencies = [
-  "websockets == 11.0.1",
   "Django >= 1.11.29",
   "requests",
   "simplejson"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/jraylan/django-bookstack"
```

### Comparing `django-bookstack-0.0.2/setup.cfg` & `django-bookstack-0.0.3/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-bookstack
-version = 0.0.2
+version = 0.0.3
 description = A Django app to consume the bookstack API.
 long_description = file: README.rst
 url = https://github.com/jraylan/django-bookstack
 author = Jefferson Raylan
 author_email = jeffersonraylan@gmail.com
 license = BSD-3-Clause
 classifiers =
```

