# Comparing `tmp/django-trackmodels-ritual-1.0.0.tar.gz` & `tmp/django-trackmodels-ritual-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-trackmodels-ritual-1.0.0.tar", last modified: Sat Mar 14 05:45:11 2020, max compression
+gzip compressed data, was "django-trackmodels-ritual-1.1.1.tar", last modified: Sat May 20 04:10:15 2023, max compression
```

## Comparing `django-trackmodels-ritual-1.0.0.tar` & `django-trackmodels-ritual-1.1.1.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 luismasuelli  (1001) luismasuelli  (1001)        0 2020-03-14 05:45:11.666936 django-trackmodels-ritual-1.0.0/
--rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)      358 2020-03-14 05:45:11.666936 django-trackmodels-ritual-1.0.0/PKG-INFO
-drwxr-xr-x   0 luismasuelli  (1001) luismasuelli  (1001)        0 2020-03-14 05:45:11.570936 django-trackmodels-ritual-1.0.0/django_trackmodels_ritual.egg-info/
--rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)      358 2020-03-14 05:45:11.000000 django-trackmodels-ritual-1.0.0/django_trackmodels_ritual.egg-info/PKG-INFO
--rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)      842 2020-03-14 05:45:11.000000 django-trackmodels-ritual-1.0.0/django_trackmodels_ritual.egg-info/SOURCES.txt
--rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)        1 2020-03-14 05:45:11.000000 django-trackmodels-ritual-1.0.0/django_trackmodels_ritual.egg-info/dependency_links.txt
--rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)       58 2020-03-14 05:45:11.000000 django-trackmodels-ritual-1.0.0/django_trackmodels_ritual.egg-info/requires.txt
--rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)        9 2020-03-14 05:45:11.000000 django-trackmodels-ritual-1.0.0/django_trackmodels_ritual.egg-info/top_level.txt
-drwxr-xr-x   0 luismasuelli  (1001) luismasuelli  (1001)        0 2020-03-14 05:45:11.566936 django-trackmodels-ritual-1.0.0/grimoire/
-drwxr-xr-x   0 luismasuelli  (1001) luismasuelli  (1001)        0 2020-03-14 05:45:11.566936 django-trackmodels-ritual-1.0.0/grimoire/django/
-drwxr-xr-x   0 luismasuelli  (1001) luismasuelli  (1001)        0 2020-03-14 05:45:11.570936 django-trackmodels-ritual-1.0.0/grimoire/django/tracked/
--rw-rw-r--   0 luismasuelli  (1001) luismasuelli  (1001)        0 2015-09-02 03:16:13.000000 django-trackmodels-ritual-1.0.0/grimoire/django/tracked/__init__.py
--rw-rw-r--   0 luismasuelli  (1001) luismasuelli  (1001)     8593 2016-05-24 03:26:32.000000 django-trackmodels-ritual-1.0.0/grimoire/django/tracked/admin.py
-drwxr-xr-x   0 luismasuelli  (1001) luismasuelli  (1001)        0 2020-03-14 05:45:11.566936 django-trackmodels-ritual-1.0.0/grimoire/django/tracked/locale/
-drwxr-xr-x   0 luismasuelli  (1001) luismasuelli  (1001)        0 2020-03-14 05:45:11.566936 django-trackmodels-ritual-1.0.0/grimoire/django/tracked/locale/en/
-drwxr-xr-x   0 luismasuelli  (1001) luismasuelli  (1001)        0 2020-03-14 05:45:11.570936 django-trackmodels-ritual-1.0.0/grimoire/django/tracked/locale/en/LC_MESSAGES/
--rw-rw-r--   0 luismasuelli  (1001) luismasuelli  (1001)     1678 2015-09-02 05:39:06.000000 django-trackmodels-ritual-1.0.0/grimoire/django/tracked/locale/en/LC_MESSAGES/django.mo
--rw-rw-r--   0 luismasuelli  (1001) luismasuelli  (1001)     3278 2016-05-22 05:32:48.000000 django-trackmodels-ritual-1.0.0/grimoire/django/tracked/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 luismasuelli  (1001) luismasuelli  (1001)        0 2020-03-14 05:45:11.566936 django-trackmodels-ritual-1.0.0/grimoire/django/tracked/locale/es/
-drwxr-xr-x   0 luismasuelli  (1001) luismasuelli  (1001)        0 2020-03-14 05:45:11.606936 django-trackmodels-ritual-1.0.0/grimoire/django/tracked/locale/es/LC_MESSAGES/
--rw-rw-r--   0 luismasuelli  (1001) luismasuelli  (1001)     1826 2015-09-02 05:39:06.000000 django-trackmodels-ritual-1.0.0/grimoire/django/tracked/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 luismasuelli  (1001) luismasuelli  (1001)     3461 2016-05-22 05:35:02.000000 django-trackmodels-ritual-1.0.0/grimoire/django/tracked/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 luismasuelli  (1001) luismasuelli  (1001)        0 2020-03-14 05:45:11.622936 django-trackmodels-ritual-1.0.0/grimoire/django/tracked/models/
--rw-rw-r--   0 luismasuelli  (1001) luismasuelli  (1001)      235 2017-09-10 02:06:49.000000 django-trackmodels-ritual-1.0.0/grimoire/django/tracked/models/__init__.py
--rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)     9363 2019-11-06 02:37:25.000000 django-trackmodels-ritual-1.0.0/grimoire/django/tracked/models/common.py
--rw-rw-r--   0 luismasuelli  (1001) luismasuelli  (1001)     1214 2020-03-14 02:03:16.000000 django-trackmodels-ritual-1.0.0/grimoire/django/tracked/models/polymorphic.py
--rw-rw-r--   0 luismasuelli  (1001) luismasuelli  (1001)    13060 2020-03-14 03:05:05.000000 django-trackmodels-ritual-1.0.0/grimoire/django/tracked/reports.py
-drwxr-xr-x   0 luismasuelli  (1001) luismasuelli  (1001)        0 2020-03-14 05:45:11.566936 django-trackmodels-ritual-1.0.0/grimoire/django/tracked/templates/
-drwxr-xr-x   0 luismasuelli  (1001) luismasuelli  (1001)        0 2020-03-14 05:45:11.646936 django-trackmodels-ritual-1.0.0/grimoire/django/tracked/templates/admin/
-drwxr-xr-x   0 luismasuelli  (1001) luismasuelli  (1001)        0 2020-03-14 05:45:11.666936 django-trackmodels-ritual-1.0.0/grimoire/django/tracked/templates/admin/tracked/
--rw-rw-r--   0 luismasuelli  (1001) luismasuelli  (1001)     2207 2016-05-22 05:05:25.000000 django-trackmodels-ritual-1.0.0/grimoire/django/tracked/templates/admin/tracked/change_list.html
--rw-rw-r--   0 luismasuelli  (1001) luismasuelli  (1001)      735 2016-05-21 06:14:52.000000 django-trackmodels-ritual-1.0.0/grimoire/django/tracked/templates/admin/tracking_report_error.html
--rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)       38 2020-03-14 05:45:11.666936 django-trackmodels-ritual-1.0.0/setup.cfg
--rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)      759 2020-03-14 05:33:21.000000 django-trackmodels-ritual-1.0.0/setup.py
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:10:15.224324 django-trackmodels-ritual-1.1.1/
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     7652 2015-09-02 02:58:19.000000 django-trackmodels-ritual-1.1.1/LICENSE
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      341 2023-05-20 04:10:15.224324 django-trackmodels-ritual-1.1.1/PKG-INFO
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:10:15.220324 django-trackmodels-ritual-1.1.1/django_trackmodels_ritual.egg-info/
+-rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)      341 2023-05-20 04:10:15.000000 django-trackmodels-ritual-1.1.1/django_trackmodels_ritual.egg-info/PKG-INFO
+-rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)      850 2023-05-20 04:10:15.000000 django-trackmodels-ritual-1.1.1/django_trackmodels_ritual.egg-info/SOURCES.txt
+-rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)        1 2023-05-20 04:10:15.000000 django-trackmodels-ritual-1.1.1/django_trackmodels_ritual.egg-info/dependency_links.txt
+-rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)       58 2023-05-20 04:10:15.000000 django-trackmodels-ritual-1.1.1/django_trackmodels_ritual.egg-info/requires.txt
+-rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)        9 2023-05-20 04:10:15.000000 django-trackmodels-ritual-1.1.1/django_trackmodels_ritual.egg-info/top_level.txt
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:10:15.216324 django-trackmodels-ritual-1.1.1/grimoire/
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:10:15.216324 django-trackmodels-ritual-1.1.1/grimoire/django/
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:10:15.220324 django-trackmodels-ritual-1.1.1/grimoire/django/tracked/
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)        0 2015-09-02 03:16:13.000000 django-trackmodels-ritual-1.1.1/grimoire/django/tracked/__init__.py
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     8600 2023-04-22 04:17:06.000000 django-trackmodels-ritual-1.1.1/grimoire/django/tracked/admin.py
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:10:15.216324 django-trackmodels-ritual-1.1.1/grimoire/django/tracked/locale/
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:10:15.216324 django-trackmodels-ritual-1.1.1/grimoire/django/tracked/locale/en/
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:10:15.220324 django-trackmodels-ritual-1.1.1/grimoire/django/tracked/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     1678 2015-09-02 05:39:06.000000 django-trackmodels-ritual-1.1.1/grimoire/django/tracked/locale/en/LC_MESSAGES/django.mo
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     3278 2016-05-22 05:32:48.000000 django-trackmodels-ritual-1.1.1/grimoire/django/tracked/locale/en/LC_MESSAGES/django.po
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:10:15.216324 django-trackmodels-ritual-1.1.1/grimoire/django/tracked/locale/es/
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:10:15.220324 django-trackmodels-ritual-1.1.1/grimoire/django/tracked/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     1826 2015-09-02 05:39:06.000000 django-trackmodels-ritual-1.1.1/grimoire/django/tracked/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     3461 2016-05-22 05:35:02.000000 django-trackmodels-ritual-1.1.1/grimoire/django/tracked/locale/es/LC_MESSAGES/django.po
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:10:15.220324 django-trackmodels-ritual-1.1.1/grimoire/django/tracked/models/
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      235 2017-09-10 02:06:49.000000 django-trackmodels-ritual-1.1.1/grimoire/django/tracked/models/__init__.py
+-rw-r--r--   0 luismasuelli  (1000) luismasuelli  (1000)     9362 2023-04-22 04:03:28.000000 django-trackmodels-ritual-1.1.1/grimoire/django/tracked/models/common.py
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     1214 2020-03-14 02:03:16.000000 django-trackmodels-ritual-1.1.1/grimoire/django/tracked/models/polymorphic.py
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)    13060 2020-03-14 03:05:05.000000 django-trackmodels-ritual-1.1.1/grimoire/django/tracked/reports.py
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:10:15.216324 django-trackmodels-ritual-1.1.1/grimoire/django/tracked/templates/
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:10:15.220324 django-trackmodels-ritual-1.1.1/grimoire/django/tracked/templates/admin/
+drwxrwxr-x   0 luismasuelli  (1000) luismasuelli  (1000)        0 2023-05-20 04:10:15.220324 django-trackmodels-ritual-1.1.1/grimoire/django/tracked/templates/admin/tracked/
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)     2207 2016-05-22 05:05:25.000000 django-trackmodels-ritual-1.1.1/grimoire/django/tracked/templates/admin/tracked/change_list.html
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      735 2016-05-21 06:14:52.000000 django-trackmodels-ritual-1.1.1/grimoire/django/tracked/templates/admin/tracking_report_error.html
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)       38 2023-05-20 04:10:15.224324 django-trackmodels-ritual-1.1.1/setup.cfg
+-rw-rw-r--   0 luismasuelli  (1000) luismasuelli  (1000)      759 2023-05-20 04:06:38.000000 django-trackmodels-ritual-1.1.1/setup.py
```

### Comparing `django-trackmodels-ritual-1.0.0/django_trackmodels_ritual.egg-info/SOURCES.txt` & `django-trackmodels-ritual-1.1.1/django_trackmodels_ritual.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 setup.py
 django_trackmodels_ritual.egg-info/PKG-INFO
 django_trackmodels_ritual.egg-info/SOURCES.txt
 django_trackmodels_ritual.egg-info/dependency_links.txt
 django_trackmodels_ritual.egg-info/requires.txt
 django_trackmodels_ritual.egg-info/top_level.txt
 grimoire/django/tracked/__init__.py
```

### Comparing `django-trackmodels-ritual-1.0.0/grimoire/django/tracked/admin.py` & `django-trackmodels-ritual-1.1.1/grimoire/django/tracked/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import unicode_literals
-from django.conf.urls import url
+from django.urls import re_path
 from django.contrib.admin import SimpleListFilter, ModelAdmin
 from django.core.exceptions import PermissionDenied
 from django.template.response import TemplateResponse
-from django.utils.encoding import force_text
-from django.utils.translation import ugettext_lazy as _
+from django.utils.encoding import force_str
+from django.utils.translation import gettext_lazy as _
 import logging
 
 
 logger = logging.getLogger(__name__)
 
 
 PERIOD_AGO_LOOKUPS = (
@@ -142,17 +142,17 @@
         """
         Returns additional urls to add to a result of `get_urls` in a descendant ModelAdmin
         :return: A list of url declarations.
         """
 
         info = self.model._meta.app_label, self.model._meta.model_name
         return [
-            url(r'^report/(?P<key>\w+)/(?P<period>\w)$',
-                self.admin_site.admin_view(self.report_view),
-                name='%s_%s_tracking_report' % info)
+            re_path(r'^report/(?P<key>\w+)/(?P<period>\w)$',
+                    self.admin_site.admin_view(self.report_view),
+                    name='%s_%s_tracking_report' % info)
         ] + super(TrackedLiveAdmin, self).get_urls()
 
     def changelist_view(self, request, extra_context=None):
         """
         Updates the changelist view to include settings from this admin.
         """
 
@@ -169,16 +169,16 @@
         """
 
         opts = self.model._meta
         app_label = opts.app_label
         request.current_app = self.admin_site.name
         context = dict(
             self.admin_site.each_context(request),
-            module_name=force_text(opts.verbose_name_plural),
-            title=(_('Tracking report error for %s') % force_text(opts.verbose_name)),
+            module_name=force_str(opts.verbose_name_plural),
+            title=(_('Tracking report error for %s') % force_str(opts.verbose_name)),
             opts=opts, app_label=app_label, error=error
         )
 
         return TemplateResponse(request, self.report_error_template or [
             "admin/{}/{}/tracking_report_error.html".format(app_label, opts.model_name),
             "admin/{}/tracking_report_error.html".format(app_label),
             "admin/tracking_report_error.html"
```

### Comparing `django-trackmodels-ritual-1.0.0/grimoire/django/tracked/locale/en/LC_MESSAGES/django.mo` & `django-trackmodels-ritual-1.1.1/grimoire/django/tracked/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-trackmodels-ritual-1.0.0/grimoire/django/tracked/locale/en/LC_MESSAGES/django.po` & `django-trackmodels-ritual-1.1.1/grimoire/django/tracked/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-trackmodels-ritual-1.0.0/grimoire/django/tracked/locale/es/LC_MESSAGES/django.mo` & `django-trackmodels-ritual-1.1.1/grimoire/django/tracked/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-trackmodels-ritual-1.0.0/grimoire/django/tracked/locale/es/LC_MESSAGES/django.po` & `django-trackmodels-ritual-1.1.1/grimoire/django/tracked/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-trackmodels-ritual-1.0.0/grimoire/django/tracked/models/common.py` & `django-trackmodels-ritual-1.1.1/grimoire/django/tracked/models/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from django.db import models
 from django.conf import settings
 from django.db.models import Q
 from django.utils.timezone import now
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 from dateutil.relativedelta import relativedelta
 
 
 def define_all(QuerySet, Model):
 
     class TrackedLiveQuerySet(QuerySet):
         """
```

### Comparing `django-trackmodels-ritual-1.0.0/grimoire/django/tracked/models/polymorphic.py` & `django-trackmodels-ritual-1.1.1/grimoire/django/tracked/models/polymorphic.py`

 * *Files identical despite different names*

### Comparing `django-trackmodels-ritual-1.0.0/grimoire/django/tracked/reports.py` & `django-trackmodels-ritual-1.1.1/grimoire/django/tracked/reports.py`

 * *Files identical despite different names*

### Comparing `django-trackmodels-ritual-1.0.0/grimoire/django/tracked/templates/admin/tracked/change_list.html` & `django-trackmodels-ritual-1.1.1/grimoire/django/tracked/templates/admin/tracked/change_list.html`

 * *Files identical despite different names*

### Comparing `django-trackmodels-ritual-1.0.0/grimoire/django/tracked/templates/admin/tracking_report_error.html` & `django-trackmodels-ritual-1.1.1/grimoire/django/tracked/templates/admin/tracking_report_error.html`

 * *Files identical despite different names*

### Comparing `django-trackmodels-ritual-1.0.0/setup.py` & `django-trackmodels-ritual-1.1.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='django-trackmodels-ritual',
-    version='1.0.0',
+    version='1.1.1',
     packages=[
         'grimoire.django.tracked',
         'grimoire.django.tracked.models'
     ],
     package_data={
         'grimoire.django.tracked': [
             'locale/*/LC_MESSAGES/*.*',
@@ -15,9 +15,9 @@
         ]
     },
     url='https://github.com/luismasuelli/django-trackmodels-ritual',
     license='LGPL',
     author='Luis y Anita',
     author_email='luismasuelli@hotmail.com',
     description='The trackmodels library is useful to set creation/update/delete dates on models and track by them',
-    install_requires=['Django>=2.2', 'python-dateutil>=2.6.1', 'python-cantrips>=1.0.0']
+    install_requires=['Django>=4.2', 'python-dateutil>=2.6.1', 'python-cantrips>=1.0.0']
 )
```

