# Comparing `tmp/django-smart-media-0.2.2.tar.gz` & `tmp/django-smart-media-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-smart-media-0.2.2.tar", last modified: Tue Apr  4 00:09:39 2023, max compression
+gzip compressed data, was "django-smart-media-0.3.0.tar", last modified: Sat May 20 00:31:43 2023, max compression
```

## Comparing `django-smart-media-0.2.2.tar` & `django-smart-media-0.3.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-04 00:09:39.566499 django-smart-media-0.2.2/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1070 2023-01-11 02:27:58.000000 django-smart-media-0.2.2/LICENCE.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      322 2022-12-29 00:34:40.000000 django-smart-media-0.2.2/MANIFEST.in
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2644 2023-04-04 00:09:39.566499 django-smart-media-0.2.2/PKG-INFO
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1706 2023-01-11 02:25:08.000000 django-smart-media-0.2.2/README.rst
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-04 00:09:39.566499 django-smart-media-0.2.2/django_smart_media.egg-info/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2644 2023-04-04 00:09:39.000000 django-smart-media-0.2.2/django_smart_media.egg-info/PKG-INFO
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1086 2023-04-04 00:09:39.000000 django-smart-media-0.2.2/django_smart_media.egg-info/SOURCES.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        1 2023-04-04 00:09:39.000000 django-smart-media-0.2.2/django_smart_media.egg-info/dependency_links.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      217 2023-04-04 00:09:39.000000 django-smart-media-0.2.2/django_smart_media.egg-info/requires.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)       20 2023-04-04 00:09:39.000000 django-smart-media-0.2.2/django_smart_media.egg-info/top_level.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        1 2022-12-29 00:37:35.000000 django-smart-media-0.2.2/django_smart_media.egg-info/zip-safe
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1664 2023-04-04 00:09:39.570499 django-smart-media-0.2.2/setup.cfg
--rw-rw-r--   0 emencia   (1001) emencia   (1001)       84 2022-12-29 00:34:40.000000 django-smart-media-0.2.2/setup.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-04 00:09:39.566499 django-smart-media-0.2.2/smart_media/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      156 2022-12-29 00:34:39.000000 django-smart-media-0.2.2/smart_media/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1412 2023-01-11 02:25:08.000000 django-smart-media-0.2.2/smart_media/admin.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      249 2022-12-29 00:34:39.000000 django-smart-media-0.2.2/smart_media/apps.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-04 00:09:39.566499 django-smart-media-0.2.2/smart_media/contrib/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2023-04-04 00:09:20.000000 django-smart-media-0.2.2/smart_media/contrib/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1037 2023-04-04 00:09:20.000000 django-smart-media-0.2.2/smart_media/contrib/django_configuration.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      709 2023-01-11 02:25:08.000000 django-smart-media-0.2.2/smart_media/exceptions.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      919 2023-01-04 01:50:26.000000 django-smart-media-0.2.2/smart_media/fields.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1997 2023-04-04 00:09:20.000000 django-smart-media-0.2.2/smart_media/mixins.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2471 2023-01-11 02:25:08.000000 django-smart-media-0.2.2/smart_media/modelfields.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2079 2023-01-11 02:25:08.000000 django-smart-media-0.2.2/smart_media/settings.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     5841 2023-01-11 02:25:08.000000 django-smart-media-0.2.2/smart_media/signals.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-04 00:09:39.562499 django-smart-media-0.2.2/smart_media/static/
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-04 00:09:39.562499 django-smart-media-0.2.2/smart_media/static/smart_image/
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-04 00:09:39.566499 django-smart-media-0.2.2/smart_media/static/smart_image/css/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     3671 2022-12-29 00:42:32.000000 django-smart-media-0.2.2/smart_media/static/smart_image/css/fileinputbutton.css
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-04 00:09:39.566499 django-smart-media-0.2.2/smart_media/static/smart_image/js/
--rw-r--r--   0 emencia   (1001) emencia   (1001)     2644 2022-12-29 00:34:39.000000 django-smart-media-0.2.2/smart_media/static/smart_image/js/fileinputbutton.js
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-04 00:09:39.562499 django-smart-media-0.2.2/smart_media/templates/
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-04 00:09:39.566499 django-smart-media-0.2.2/smart_media/templates/smart_image/
--rw-r--r--   0 emencia   (1001) emencia   (1001)      632 2022-12-29 00:34:39.000000 django-smart-media-0.2.2/smart_media/templates/smart_image/fileinputbutton_basic.html
--rw-r--r--   0 emencia   (1001) emencia   (1001)     2003 2022-12-29 00:34:39.000000 django-smart-media-0.2.2/smart_media/templates/smart_image/fileinputbutton_clearable.html
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-04 00:09:39.566499 django-smart-media-0.2.2/smart_media/templatetags/
--rw-r--r--   0 emencia   (1001) emencia   (1001)        0 2022-12-29 00:34:39.000000 django-smart-media-0.2.2/smart_media/templatetags/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     4829 2023-04-04 00:09:20.000000 django-smart-media-0.2.2/smart_media/templatetags/smart_image.py
--rw-r--r--   0 emencia   (1001) emencia   (1001)     1039 2022-12-29 00:34:39.000000 django-smart-media-0.2.2/smart_media/thumbnailing.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-04-04 00:09:39.566499 django-smart-media-0.2.2/smart_media/utils/
--rw-r--r--   0 emencia   (1001) emencia   (1001)        0 2022-12-29 00:34:39.000000 django-smart-media-0.2.2/smart_media/utils/__init__.py
--rw-r--r--   0 emencia   (1001) emencia   (1001)     2317 2022-12-29 00:34:39.000000 django-smart-media-0.2.2/smart_media/utils/factories.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1369 2023-01-11 02:25:08.000000 django-smart-media-0.2.2/smart_media/utils/file.py
--rw-r--r--   0 emencia   (1001) emencia   (1001)     8838 2022-12-29 00:34:39.000000 django-smart-media-0.2.2/smart_media/utils/tests.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1543 2023-01-11 02:25:08.000000 django-smart-media-0.2.2/smart_media/validators.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2697 2023-01-11 02:25:08.000000 django-smart-media-0.2.2/smart_media/widgets.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-20 00:31:43.860581 django-smart-media-0.3.0/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1070 2023-01-11 02:27:58.000000 django-smart-media-0.3.0/LICENCE.txt
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      322 2022-12-29 00:34:40.000000 django-smart-media-0.3.0/MANIFEST.in
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2516 2023-05-20 00:31:43.860581 django-smart-media-0.3.0/PKG-INFO
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1570 2023-05-20 00:30:57.000000 django-smart-media-0.3.0/README.rst
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-20 00:31:43.856581 django-smart-media-0.3.0/django_smart_media.egg-info/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2516 2023-05-20 00:31:43.000000 django-smart-media-0.3.0/django_smart_media.egg-info/PKG-INFO
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1086 2023-05-20 00:31:43.000000 django-smart-media-0.3.0/django_smart_media.egg-info/SOURCES.txt
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)        1 2023-05-20 00:31:43.000000 django-smart-media-0.3.0/django_smart_media.egg-info/dependency_links.txt
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      212 2023-05-20 00:31:43.000000 django-smart-media-0.3.0/django_smart_media.egg-info/requires.txt
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)       20 2023-05-20 00:31:43.000000 django-smart-media-0.3.0/django_smart_media.egg-info/top_level.txt
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)        1 2022-12-29 00:37:35.000000 django-smart-media-0.3.0/django_smart_media.egg-info/zip-safe
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1698 2023-05-20 00:31:43.860581 django-smart-media-0.3.0/setup.cfg
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)       84 2022-12-29 00:34:40.000000 django-smart-media-0.3.0/setup.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-20 00:31:43.860581 django-smart-media-0.3.0/smart_media/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      156 2022-12-29 00:34:39.000000 django-smart-media-0.3.0/smart_media/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2146 2023-05-20 00:30:57.000000 django-smart-media-0.3.0/smart_media/admin.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      249 2022-12-29 00:34:39.000000 django-smart-media-0.3.0/smart_media/apps.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-20 00:31:43.860581 django-smart-media-0.3.0/smart_media/contrib/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2023-04-04 00:09:20.000000 django-smart-media-0.3.0/smart_media/contrib/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1037 2023-04-04 00:09:20.000000 django-smart-media-0.3.0/smart_media/contrib/django_configuration.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      709 2023-01-11 02:25:08.000000 django-smart-media-0.3.0/smart_media/exceptions.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1159 2023-05-20 00:30:57.000000 django-smart-media-0.3.0/smart_media/fields.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1997 2023-04-04 00:09:20.000000 django-smart-media-0.3.0/smart_media/mixins.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2471 2023-01-11 02:25:08.000000 django-smart-media-0.3.0/smart_media/modelfields.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2079 2023-01-11 02:25:08.000000 django-smart-media-0.3.0/smart_media/settings.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     5841 2023-01-11 02:25:08.000000 django-smart-media-0.3.0/smart_media/signals.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-20 00:31:43.856581 django-smart-media-0.3.0/smart_media/static/
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-20 00:31:43.856581 django-smart-media-0.3.0/smart_media/static/smart_image/
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-20 00:31:43.860581 django-smart-media-0.3.0/smart_media/static/smart_image/css/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     3785 2023-05-20 00:30:57.000000 django-smart-media-0.3.0/smart_media/static/smart_image/css/fileinputbutton.css
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-20 00:31:43.860581 django-smart-media-0.3.0/smart_media/static/smart_image/js/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2373 2023-05-20 00:30:57.000000 django-smart-media-0.3.0/smart_media/static/smart_image/js/fileinputbutton.js
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-20 00:31:43.856581 django-smart-media-0.3.0/smart_media/templates/
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-20 00:31:43.860581 django-smart-media-0.3.0/smart_media/templates/smart_image/
+-rw-r--r--   0 emencia   (1001) emencia   (1001)      632 2022-12-29 00:34:39.000000 django-smart-media-0.3.0/smart_media/templates/smart_image/fileinputbutton_basic.html
+-rw-r--r--   0 emencia   (1001) emencia   (1001)     2003 2022-12-29 00:34:39.000000 django-smart-media-0.3.0/smart_media/templates/smart_image/fileinputbutton_clearable.html
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-20 00:31:43.860581 django-smart-media-0.3.0/smart_media/templatetags/
+-rw-r--r--   0 emencia   (1001) emencia   (1001)        0 2022-12-29 00:34:39.000000 django-smart-media-0.3.0/smart_media/templatetags/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     4966 2023-05-20 00:30:57.000000 django-smart-media-0.3.0/smart_media/templatetags/smart_image.py
+-rw-r--r--   0 emencia   (1001) emencia   (1001)     1039 2022-12-29 00:34:39.000000 django-smart-media-0.3.0/smart_media/thumbnailing.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-20 00:31:43.860581 django-smart-media-0.3.0/smart_media/utils/
+-rw-r--r--   0 emencia   (1001) emencia   (1001)        0 2022-12-29 00:34:39.000000 django-smart-media-0.3.0/smart_media/utils/__init__.py
+-rw-r--r--   0 emencia   (1001) emencia   (1001)     2317 2022-12-29 00:34:39.000000 django-smart-media-0.3.0/smart_media/utils/factories.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1369 2023-01-11 02:25:08.000000 django-smart-media-0.3.0/smart_media/utils/file.py
+-rw-r--r--   0 emencia   (1001) emencia   (1001)     8838 2022-12-29 00:34:39.000000 django-smart-media-0.3.0/smart_media/utils/tests.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1543 2023-01-11 02:25:08.000000 django-smart-media-0.3.0/smart_media/validators.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     3207 2023-05-20 00:30:57.000000 django-smart-media-0.3.0/smart_media/widgets.py
```

### Comparing `django-smart-media-0.2.2/LICENCE.txt` & `django-smart-media-0.3.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `django-smart-media-0.2.2/PKG-INFO` & `django-smart-media-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: django-smart-media
-Version: 0.2.2
+Version: 0.3.0
 Summary: Django file fields with SVG support
 Home-page: https://github.com/sveetch/django-smart-media
 Author: David Thenon
 Author-email: sveetch@gmail.com
 License: MIT
 Keywords: Python Django
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -50,24 +50,22 @@
 ********
 
 Concretely this contains:
 
 * Form widgets to build HTML for a ``FileField`` either with or without clearable
   mode. Both mode have a version to include needed layout assets (CSS and Javascript)
   and another one without assets;
+* Form fields which already set a "smart" widget;
 * Templates to build the widgets HTML;
 * CSS and Javascript for the widget layout;
-* Form fields which already set a "smart" widget;
 * Field validator;
 * Model signals to purge stale files;
 * Model field with all "smart" features;
-* A template tag to make a thumbnail that can be used either in the form for preview
-  or to be used in frontend for content thumbnail. By default, the thumbnail is
-  made in the original content format. Also not than a SVG cannot be converted to a
-  Bitmap and vice versa;
+* A template tag to make thumbnail safely with SVG image (original SVG is just used
+  without Sorl raising issue for a non bitmap image);
 * Some helpers to ease some specific implementations;
 
 Although this can work with ``ImageField``, SVG support will only work with
 ``FileField`` since ``ImageField`` rely on PIL that does not support SVG format.
 
 
 Links
```

### Comparing `django-smart-media-0.2.2/README.rst` & `django-smart-media-0.3.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -22,24 +22,22 @@
 ********
 
 Concretely this contains:
 
 * Form widgets to build HTML for a ``FileField`` either with or without clearable
   mode. Both mode have a version to include needed layout assets (CSS and Javascript)
   and another one without assets;
+* Form fields which already set a "smart" widget;
 * Templates to build the widgets HTML;
 * CSS and Javascript for the widget layout;
-* Form fields which already set a "smart" widget;
 * Field validator;
 * Model signals to purge stale files;
 * Model field with all "smart" features;
-* A template tag to make a thumbnail that can be used either in the form for preview
-  or to be used in frontend for content thumbnail. By default, the thumbnail is
-  made in the original content format. Also not than a SVG cannot be converted to a
-  Bitmap and vice versa;
+* A template tag to make thumbnail safely with SVG image (original SVG is just used
+  without Sorl raising issue for a non bitmap image);
 * Some helpers to ease some specific implementations;
 
 Although this can work with ``ImageField``, SVG support will only work with
 ``FileField`` since ``ImageField`` rely on PIL that does not support SVG format.
 
 
 Links
```

### Comparing `django-smart-media-0.2.2/django_smart_media.egg-info/PKG-INFO` & `django-smart-media-0.3.0/django_smart_media.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: django-smart-media
-Version: 0.2.2
+Version: 0.3.0
 Summary: Django file fields with SVG support
 Home-page: https://github.com/sveetch/django-smart-media
 Author: David Thenon
 Author-email: sveetch@gmail.com
 License: MIT
 Keywords: Python Django
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -50,24 +50,22 @@
 ********
 
 Concretely this contains:
 
 * Form widgets to build HTML for a ``FileField`` either with or without clearable
   mode. Both mode have a version to include needed layout assets (CSS and Javascript)
   and another one without assets;
+* Form fields which already set a "smart" widget;
 * Templates to build the widgets HTML;
 * CSS and Javascript for the widget layout;
-* Form fields which already set a "smart" widget;
 * Field validator;
 * Model signals to purge stale files;
 * Model field with all "smart" features;
-* A template tag to make a thumbnail that can be used either in the form for preview
-  or to be used in frontend for content thumbnail. By default, the thumbnail is
-  made in the original content format. Also not than a SVG cannot be converted to a
-  Bitmap and vice versa;
+* A template tag to make thumbnail safely with SVG image (original SVG is just used
+  without Sorl raising issue for a non bitmap image);
 * Some helpers to ease some specific implementations;
 
 Although this can work with ``ImageField``, SVG support will only work with
 ``FileField`` since ``ImageField`` rely on PIL that does not support SVG format.
 
 
 Links
```

### Comparing `django-smart-media-0.2.2/django_smart_media.egg-info/SOURCES.txt` & `django-smart-media-0.3.0/django_smart_media.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-smart-media-0.2.2/setup.cfg` & `django-smart-media-0.3.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [metadata]
 name = django-smart-media
-version = 0.2.2
+version = 0.3.0
 description = Django file fields with SVG support
 long_description = file:README.rst
 long_description_content_type = text/x-rst
 author = David Thenon
 author_email = sveetch@gmail.com
 url = https://github.com/sveetch/django-smart-media
 license = MIT
 keywords = Python Django
 classifiers = 
-	Development Status :: 2 - Pre-Alpha
+	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Natural Language :: English
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
@@ -22,15 +22,15 @@
 	Framework :: Django :: 3.2
 	Framework :: Django :: 4.0
 	Framework :: Django :: 4.1
 
 [options]
 include_package_data = True
 install_requires = 
-	Django>=3.1,<4.2
+	Django>=3.1
 	pillow>=8.0.0
 	sorl-thumbnail>=12.9.0
 packages = find:
 zip_safe = True
 
 [options.extras_require]
 dev = 
@@ -76,21 +76,22 @@
 python_files = 
 	*.py
 testpaths = 
 	tests
 
 [tox:tox]
 minversion = 3.4.0
-envlist = py{38,310}-django{32,40,41}
+envlist = py{38,310}-django{32,40,41,42}
 
 [testenv]
 deps = 
-	django32: Django>=3.2,<3.3
+	django32: Django>=3.2,<4.0
 	django40: Django>=4.0,<4.1
 	django41: Django>=4.1,<4.2
+	django42: Django>=4.2,<5.0
 commands = 
 	pip install -e .[dev]
 	pytest -vv tests
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `django-smart-media-0.2.2/smart_media/admin.py` & `django-smart-media-0.3.0/smart_media/admin.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,66 @@
 from django.contrib import admin as django_admin
 
 from .modelfields import SmartMediaField
 from .widgets import ClearableFileInputButton
 
 
-class SmartModelAdmin(django_admin.ModelAdmin):
+class SmartAdminMixin:
     """
-    A model admin class to include the right widget definition for model field
-    ``modelfields.SmartMediaField``.
+    A class to mix with a Django admin class to the use right widget definition for
+    model field ``modelfields.SmartMediaField``.
 
-    This is required because ModelAdmin translate model field to widgets using a list
-    of harcoded relations between fields and widgets. It results field definition in
-    ``SmartMediaField.formfield`` is ignored and translate ``SmartMediaField`` to
-    ``AdminFileWidget`` instead of expected ``ClearableFileInputButton``.
+    .. Note::
+        This is required because ModelAdmin translate model fields to widgets using a
+        list of harcoded relations between fields and widgets.
+
+        It results in field definitions from ``SmartMediaField.formfield`` to be
+        ignored and ``SmartMediaField`` using admin widget ``AdminFileWidget`` instead
+        of expected ``ClearableFileInputButton``.
 
-    So either your model admin inherits from ``SmartModelAdmin`` or simply copy its
-    ``SmartModelAdmin.formfield_overrides`` into it.
-
-    It is only required with model forms in Django admin.
+        This mixin will be safe to use with specific model admins that does not allows
+        to inherit from ``SmartModelAdmin``.
 
     Example:
 
-        Your model admin just have to inherit from this class: ::
+        Your model admin just have to inherit from this class in addition to the model
+        admin class: ::
 
             from django.contrib import admin
-            from smart_media.admin import SmartModelAdmin
+            from smart_media.admin import SmartAdminMixin
             from myapp.models import MyModel
 
             @admin.register(MyModel)
-            class MyModelAdmin(SmartModelAdmin):
+            class MyModelAdmin(SmartAdminMixin, admin.ModelAdmin):
                 ...
 
-    Or copy the source of ``SmartModelAdmin.formfield_overrides`` (see source) into
-    your own model admin.
+    If you can't use it, just copy the source of
+    ``SmartAdminMixin.formfield_overrides`` (see source) into your own model admin.
     """
     formfield_overrides = {
         SmartMediaField: {
             "widget": ClearableFileInputButton,
         },
     }
+
+
+class SmartModelAdmin(SmartAdminMixin, django_admin.ModelAdmin):
+    """
+    A model admin class to include ``SmartAdminMixin``.
+
+    It is only required with model forms in Django admin. If your model admin already
+    inherit from a specific admin class, you will prefer to use the
+    ``SmartAdminMixin``.
+
+    Example:
+
+        Your model admin just have to inherit from this class: ::
+
+            from django.contrib import admin
+            from smart_media.admin import SmartModelAdmin
+            from myapp.models import MyModel
+
+            @admin.register(MyModel)
+            class MyModelAdmin(SmartModelAdmin):
+                ...
+    """
+    pass
```

### Comparing `django-smart-media-0.2.2/smart_media/contrib/django_configuration.py` & `django-smart-media-0.3.0/smart_media/contrib/django_configuration.py`

 * *Files identical despite different names*

### Comparing `django-smart-media-0.2.2/smart_media/exceptions.py` & `django-smart-media-0.3.0/smart_media/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-smart-media-0.2.2/smart_media/fields.py` & `django-smart-media-0.3.0/smart_media/fields.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,14 +6,19 @@
 
 
 class SmartMediaField(FileField):
     """
     A FileField which define the widget ``ClearableFileInputButton`` and default
     validator ``FileExtensionValidator`` for allowed extensions (as defined from
     setting ``SMARTIMAGE_ALLOWED_IMAGE_EXTENSIONS``).
+
+    .. Note::
+        Validation is pretty basic since it works on file extension, no malicious
+        Bitmap or SVG image files would be detected here. If it is a concern, you
+        will have to develop or use an additional validator.
     """
     widget = ClearableFileInputButton
     default_validators = [
         FileExtensionValidator(
             allowed_extensions=settings.SMARTIMAGE_ALLOWED_IMAGE_EXTENSIONS
         ),
     ]
```

### Comparing `django-smart-media-0.2.2/smart_media/mixins.py` & `django-smart-media-0.3.0/smart_media/mixins.py`

 * *Files identical despite different names*

### Comparing `django-smart-media-0.2.2/smart_media/modelfields.py` & `django-smart-media-0.3.0/smart_media/modelfields.py`

 * *Files identical despite different names*

### Comparing `django-smart-media-0.2.2/smart_media/settings.py` & `django-smart-media-0.3.0/smart_media/settings.py`

 * *Files identical despite different names*

### Comparing `django-smart-media-0.2.2/smart_media/signals.py` & `django-smart-media-0.3.0/smart_media/signals.py`

 * *Files identical despite different names*

### Comparing `django-smart-media-0.2.2/smart_media/static/smart_image/css/fileinputbutton.css` & `django-smart-media-0.3.0/smart_media/static/smart_image/css/fileinputbutton.css`

 * *Files 4% similar despite different names*

```diff
@@ -87,14 +87,18 @@
 }
 
 .fileinputbutton.fileinputbutton--has-preview .fileinputbutton__preview a img {
   display: inline-block;
   margin: 0 auto;
 }
 
+.fileinputbutton.fileinputbutton--has-preview .fileinputbutton__preview a img[src$=".svg"] {
+  width: 3.75rem;
+}
+
 .fileinputbutton.fileinputbutton--has-preview .fileinputbutton__controls {
   flex-grow: 1;
   flex-shrink: 0;
   flex-basis: auto;
   display: flex;
   flex-wrap: wrap;
   flex-direction: column;
```

### Comparing `django-smart-media-0.2.2/smart_media/static/smart_image/js/fileinputbutton.js` & `django-smart-media-0.3.0/smart_media/static/smart_image/js/fileinputbutton.js`

 * *Files 20% similar despite different names*

#### js-beautify {}

```diff
@@ -20,30 +20,23 @@
  * with something like "{count} files selected".
  *
  * States:
  *
  * - When input is focused, a classname "has-focus" is added;
  * - When one or more files are selected, a classname "has-selection" is added;
  *
- * Original source has been enclosed into jQuery "on ready" function since medias from
- * a form are always loaded in the header and so we need to prevent executing this code
- * before the DOM is ready.
- *
- * This is safe in Django context since jQuery is alread loaded but won't work in
- * frontends without jQuery.
- *
  * Original credits:
  *
  * By Osvaldas Valutis, www.osvaldas.info
  * Available for use under the MIT License
  *
  * From: https://tympanus.net/codrops/2015/09/15/styling-customizing-file-inputs-smart-way/
  */
 
-$(function($) {
+window.addEventListener('DOMContentLoaded', function() {
     var inputs = document.querySelectorAll('.fileinputbutton__input');
     Array.prototype.forEach.call(inputs, function(input) {
         var label = input.nextElementSibling,
             labelVal = label.innerHTML;
 
         input.addEventListener('change', function(e) {
             var fileName = '';
@@ -66,8 +59,8 @@
         input.addEventListener('focus', function() {
             input.classList.add('has-focus');
         });
         input.addEventListener('blur', function() {
             input.classList.remove('has-focus');
         });
     });
-});
+}, false);
```

### Comparing `django-smart-media-0.2.2/smart_media/templates/smart_image/fileinputbutton_basic.html` & `django-smart-media-0.3.0/smart_media/templates/smart_image/fileinputbutton_basic.html`

 * *Files identical despite different names*

### Comparing `django-smart-media-0.2.2/smart_media/templates/smart_image/fileinputbutton_clearable.html` & `django-smart-media-0.3.0/smart_media/templates/smart_image/fileinputbutton_clearable.html`

 * *Files identical despite different names*

### Comparing `django-smart-media-0.2.2/smart_media/templatetags/smart_image.py` & `django-smart-media-0.3.0/smart_media/templatetags/smart_image.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,24 +11,27 @@
 
 register = template.Library()
 
 
 @register.simple_tag
 def media_thumb(source, geometry, *args, **kwargs):
     """
+
     Determine the right format and return the Sorl thumb file url path for
     given image file.
 
+    .. _Sorl: https://github.com/jazzband/sorl-thumbnail
+
     Arguments:
         source (object): Either a FileField or an ImageField.
         geometry (string): Geometry string as expected by Sorl. It should be
             something like ``200`` for 200px width and automatic height or
             ``200x100`` for 200px width and 100px height.
         *args: Not used, there is no other expected positionnal arguments.
-        **kwargs: Keyword arguments are passed to Sorl, watch its documentation
+        **kwargs: Keyword arguments are passed to `Sorl`_, watch its documentation
             for more details.
 
     Keyword Arguments:
         format (string):
             An available format name from settings ``SMART_FORMAT_AVAILABLE_FORMATS``:
 
             * ``PNG``, ``JPEG`` and ``GIF`` enforce the thumb format no matter
@@ -63,14 +66,16 @@
         Every argument but ``format`` is passed to Sorl, so for cropping an image you
         can do : ::
 
             {% load smart_image %}
             {% media_thumb instance.image "250x200" crop="center" as thumb %}
             <img src="{{ thumb.url }}" alt="">
 
+        Again, see `Sorl`_ documentation to know about available options.
+
     Return:
         sorl.thumbnail.images.ImageFile or SvgFile: Either Sorl ImageFile instance for
         created thumb or SvgFile which mimic Sorl ImageFile.
     """
     # Safe return when there is no source file
     # NOTE: Should trigger a warning log ?
     if not source:
```

### Comparing `django-smart-media-0.2.2/smart_media/thumbnailing.py` & `django-smart-media-0.3.0/smart_media/thumbnailing.py`

 * *Files identical despite different names*

### Comparing `django-smart-media-0.2.2/smart_media/utils/factories.py` & `django-smart-media-0.3.0/smart_media/utils/factories.py`

 * *Files identical despite different names*

### Comparing `django-smart-media-0.2.2/smart_media/utils/file.py` & `django-smart-media-0.3.0/smart_media/utils/file.py`

 * *Files identical despite different names*

### Comparing `django-smart-media-0.2.2/smart_media/utils/tests.py` & `django-smart-media-0.3.0/smart_media/utils/tests.py`

 * *Files identical despite different names*

### Comparing `django-smart-media-0.2.2/smart_media/validators.py` & `django-smart-media-0.3.0/smart_media/validators.py`

 * *Files identical despite different names*

### Comparing `django-smart-media-0.2.2/smart_media/widgets.py` & `django-smart-media-0.3.0/smart_media/widgets.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from django.forms.widgets import FileInput, ClearableFileInput
 
 
 class FileInputButtonBase(FileInput):
     """
     A simple FileInput override to use a custom template.
 
-    The base version does not include the required medias so you can include
-    them yourself in your form controler, this is a good idea in some
-    environment like DjangoCMS which needs to use a lot of ``!important`` marks
-    to override the admin stylesheets and is not included from this widget stylesheets.
+    The custom template is located at ``smart_image/fileinputbutton_basic.html``, you
+    may override it in your project if needed, but mind it is global to all SmartMedia
+    widgets.
 
     Default behavior if no ``class`` attribute is given is to apply the CSS
     classname ``fileinputbutton__input`` to the input.
 
     .. Note::
         When your input file enable the ``multiple`` attribute to accept more
         than one file, label input will be rendered to a default string like
@@ -27,39 +26,52 @@
             })
 
         Pattern ``{count}`` will be replaced with the number of selected files.
     """
     template_name = "smart_image/fileinputbutton_basic.html"
 
     def __init__(self, attrs=None):
-        default_attrs = {'class': 'fileinputbutton__input'}
+        default_attrs = {"class": "fileinputbutton__input"}
         if attrs:
             default_attrs.update(attrs)
         super().__init__(default_attrs)
 
 
 class ClearableFileInputButtonBase(ClearableFileInput):
     """
     Alike ``FileInputButtonBase`` but to extend with the additional clear checkbox.
 
     This won't support the "multiple" input file feature.
     """
     template_name = "smart_image/fileinputbutton_clearable.html"
 
     def __init__(self, attrs=None):
-        default_attrs = {'class': 'fileinputbutton__input'}
+        default_attrs = {"class": "fileinputbutton__input"}
         if attrs:
             default_attrs.update(attrs)
         super().__init__(default_attrs)
 
 
 class FileInputButton(FileInputButtonBase):
     """
     ``FileInputButtonBase`` version which includes the required assets to customize
     its layout and turn the file input as a button.
+
+    This widget will define a stylesheet and a Javascript asset to load as
+    `form medias <https://docs.djangoproject.com/en/4.2/topics/forms/media/>`_, this
+    automatically done from admin but you will probably have to load them on your own
+    in a custom form.
+
+    * Stylesheet is located at ``smart_image/css/fileinputbutton.css`` (relative to
+      static directory);
+    * Javascript is located at ``smart_image/js/fileinputbutton.js`` (relative to
+      static directory);
+
+    You can retrieve these assets sources in repository, note than the CSS is built
+    from a Sass source you may copy into your project Sass sources.
     """
     class Media:
         css = {
             "all": ("smart_image/css/fileinputbutton.css",),
         }
         js = ("smart_image/js/fileinputbutton.js",)
```

