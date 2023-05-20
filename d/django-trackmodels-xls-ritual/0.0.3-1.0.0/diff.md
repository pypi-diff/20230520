# Comparing `tmp/django-trackmodels-xls-ritual-0.0.3.tar.gz` & `tmp/django-trackmodels-xls-ritual-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-trackmodels-xls-ritual-0.0.3.tar", last modified: Sun Sep 10 05:18:17 2017, max compression
+gzip compressed data, was "dist/django-trackmodels-xls-ritual-1.0.0.tar", last modified: Sat Mar 14 05:45:32 2020, max compression
```

## Comparing `django-trackmodels-xls-ritual-0.0.3.tar` & `django-trackmodels-xls-ritual-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,15 @@
-drwxrwxr-x   0 luismasuelli  (1001) luismasuelli  (1001)        0 2017-09-10 05:18:17.000000 django-trackmodels-xls-ritual-0.0.3/
-drwxrwxr-x   0 luismasuelli  (1001) luismasuelli  (1001)        0 2017-09-10 05:18:17.000000 django-trackmodels-xls-ritual-0.0.3/django_trackmodels_xls_ritual.egg-info/
--rw-rw-r--   0 luismasuelli  (1001) luismasuelli  (1001)       25 2017-09-10 05:18:17.000000 django-trackmodels-xls-ritual-0.0.3/django_trackmodels_xls_ritual.egg-info/namespace_packages.txt
--rw-rw-r--   0 luismasuelli  (1001) luismasuelli  (1001)       64 2017-09-10 05:18:17.000000 django-trackmodels-xls-ritual-0.0.3/django_trackmodels_xls_ritual.egg-info/requires.txt
--rw-rw-r--   0 luismasuelli  (1001) luismasuelli  (1001)      462 2017-09-10 05:18:17.000000 django-trackmodels-xls-ritual-0.0.3/django_trackmodels_xls_ritual.egg-info/SOURCES.txt
--rw-rw-r--   0 luismasuelli  (1001) luismasuelli  (1001)        9 2017-09-10 05:18:17.000000 django-trackmodels-xls-ritual-0.0.3/django_trackmodels_xls_ritual.egg-info/top_level.txt
--rw-rw-r--   0 luismasuelli  (1001) luismasuelli  (1001)      317 2017-09-10 05:18:17.000000 django-trackmodels-xls-ritual-0.0.3/django_trackmodels_xls_ritual.egg-info/PKG-INFO
--rw-rw-r--   0 luismasuelli  (1001) luismasuelli  (1001)        1 2017-09-10 05:18:17.000000 django-trackmodels-xls-ritual-0.0.3/django_trackmodels_xls_ritual.egg-info/dependency_links.txt
--rw-rw-r--   0 luismasuelli  (1001) luismasuelli  (1001)      722 2017-09-10 03:48:15.000000 django-trackmodels-xls-ritual-0.0.3/setup.py
--rw-rw-r--   0 luismasuelli  (1001) luismasuelli  (1001)      317 2017-09-10 05:18:17.000000 django-trackmodels-xls-ritual-0.0.3/PKG-INFO
--rw-rw-r--   0 luismasuelli  (1001) luismasuelli  (1001)       59 2017-09-10 05:18:17.000000 django-trackmodels-xls-ritual-0.0.3/setup.cfg
-drwxrwxr-x   0 luismasuelli  (1001) luismasuelli  (1001)        0 2017-09-10 05:18:17.000000 django-trackmodels-xls-ritual-0.0.3/grimoire/
-drwxrwxr-x   0 luismasuelli  (1001) luismasuelli  (1001)        0 2017-09-10 05:18:17.000000 django-trackmodels-xls-ritual-0.0.3/grimoire/django/
--rw-rw-r--   0 luismasuelli  (1001) luismasuelli  (1001)       56 2015-09-02 03:11:23.000000 django-trackmodels-xls-ritual-0.0.3/grimoire/django/__init__.py
-drwxrwxr-x   0 luismasuelli  (1001) luismasuelli  (1001)        0 2017-09-10 05:18:17.000000 django-trackmodels-xls-ritual-0.0.3/grimoire/django/tracked_xls/
--rw-rw-r--   0 luismasuelli  (1001) luismasuelli  (1001)        1 2016-05-23 00:30:07.000000 django-trackmodels-xls-ritual-0.0.3/grimoire/django/tracked_xls/__init__.py
--rw-rw-r--   0 luismasuelli  (1001) luismasuelli  (1001)     9261 2016-05-24 03:06:31.000000 django-trackmodels-xls-ritual-0.0.3/grimoire/django/tracked_xls/reports.py
--rw-rw-r--   0 luismasuelli  (1001) luismasuelli  (1001)       55 2015-09-02 03:11:23.000000 django-trackmodels-xls-ritual-0.0.3/grimoire/__init__.py
+drwxr-xr-x   0 luismasuelli  (1001) luismasuelli  (1001)        0 2020-03-14 05:45:32.842857 django-trackmodels-xls-ritual-1.0.0/
+-rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)      317 2020-03-14 05:45:32.842857 django-trackmodels-xls-ritual-1.0.0/PKG-INFO
+drwxr-xr-x   0 luismasuelli  (1001) luismasuelli  (1001)        0 2020-03-14 05:45:32.826857 django-trackmodels-xls-ritual-1.0.0/django_trackmodels_xls_ritual.egg-info/
+-rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)      317 2020-03-14 05:45:32.000000 django-trackmodels-xls-ritual-1.0.0/django_trackmodels_xls_ritual.egg-info/PKG-INFO
+-rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)      351 2020-03-14 05:45:32.000000 django-trackmodels-xls-ritual-1.0.0/django_trackmodels_xls_ritual.egg-info/SOURCES.txt
+-rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)        1 2020-03-14 05:45:32.000000 django-trackmodels-xls-ritual-1.0.0/django_trackmodels_xls_ritual.egg-info/dependency_links.txt
+-rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)       63 2020-03-14 05:45:32.000000 django-trackmodels-xls-ritual-1.0.0/django_trackmodels_xls_ritual.egg-info/requires.txt
+-rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)        9 2020-03-14 05:45:32.000000 django-trackmodels-xls-ritual-1.0.0/django_trackmodels_xls_ritual.egg-info/top_level.txt
+drwxr-xr-x   0 luismasuelli  (1001) luismasuelli  (1001)        0 2020-03-14 05:45:32.826857 django-trackmodels-xls-ritual-1.0.0/grimoire/
+drwxr-xr-x   0 luismasuelli  (1001) luismasuelli  (1001)        0 2020-03-14 05:45:32.826857 django-trackmodels-xls-ritual-1.0.0/grimoire/django/
+drwxr-xr-x   0 luismasuelli  (1001) luismasuelli  (1001)        0 2020-03-14 05:45:32.842857 django-trackmodels-xls-ritual-1.0.0/grimoire/django/tracked_xls/
+-rw-rw-r--   0 luismasuelli  (1001) luismasuelli  (1001)        1 2016-05-23 00:30:07.000000 django-trackmodels-xls-ritual-1.0.0/grimoire/django/tracked_xls/__init__.py
+-rw-rw-r--   0 luismasuelli  (1001) luismasuelli  (1001)     9213 2020-03-14 05:39:36.000000 django-trackmodels-xls-ritual-1.0.0/grimoire/django/tracked_xls/reports.py
+-rw-r--r--   0 luismasuelli  (1001) luismasuelli  (1001)       38 2020-03-14 05:45:32.842857 django-trackmodels-xls-ritual-1.0.0/setup.cfg
+-rw-rw-r--   0 luismasuelli  (1001) luismasuelli  (1001)      474 2020-03-14 05:33:21.000000 django-trackmodels-xls-ritual-1.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-trackmodels-xls-ritual-0.0.3/grimoire/django/tracked_xls/reports.py` & `django-trackmodels-xls-ritual-1.0.0/grimoire/django/tracked_xls/reports.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import datetime
+from io import BytesIO
+import re
+import pytz
+import xlsxwriter
 from grimoire.django.tracked.reports import RichFormatTrackingReport
 from django.utils.timezone import now
-from django.utils.six import text_type, string_types, StringIO
-import xlsxwriter
-import pytz
-import re
+
 
 _REMOVE_INVALID_CHARS = re.compile(r'[^ daAmbByYpIHMSf%/:\.-]')
 _REMOVE_INVALID_MARKS = re.compile(r'%[^daAmbByYpIHMSf%]')
 _REMOVE_INVALID_EXTRA = re.compile(r'(?<!%)[daAmbByYpIHMSf]')
 _UNIFY_SPACES = re.compile(r'\s{2,}')
 _TRIM_SPACES = re.compile(r'\s*([/:\.-])\s*')
 _MIN_AFTER_LHOURS = re.compile(r'(?<=%H:)%M')
 _MIN_AFTER_SHOURS = re.compile(r'(?<=%I:)%M')
 _MIN_BEFORE_SECONDS = re.compile(r'%M(?=:%S)')
 _FRAC_AFTER_SECONDS = re.compile(r'(?=%S)\.%f')
 _REMOVE_REMAINING_MARKS = re.compile(r'%[^%]')
 _TRIM_NONALPHA_CHARS = re.compile(r'^\s*[/:\.-]*|[/:\.-]*\s*$')
 
+
 def strftime2xls(fmt):
     """
     Converts a strftime format to an xls format.
     Discards specifiers which are not compatible to both formats.
     """
 
     fmt = _REMOVE_INVALID_CHARS.sub('', fmt)
@@ -155,15 +157,15 @@
     def dump_report_content(self, request, result):
         """
         Dumps the content to a string, suitable to being written on a file.
         :param result:
         :return: string
         """
 
-        stream = StringIO()
+        stream = BytesIO()
         workbook = xlsxwriter.Workbook(stream, {'in_memory': True})
         worksheet = workbook.add_worksheet(self.get_xls_worksheet_name(request))
         formats = {}
         headers = result.headers
         rows = result.values
         start_row = self.get_xls_worksheet_start_row(request)
         start_col = self.get_xls_worksheet_start_col(request)
@@ -190,15 +192,15 @@
                 worksheet.write_datetime(row, col, data, preprocess_format(format))
             elif isinstance(data, datetime.time):
                 format = dict(format, num_format=time_format)
                 worksheet.write_datetime(row, col, data, preprocess_format(format))
             elif isinstance(data, datetime.date):
                 format = dict(format, num_format=date_format)
                 worksheet.write_datetime(row, col, data, preprocess_format(format))
-            elif isinstance(data, string_types):
+            elif isinstance(data, str):
                 return worksheet.write_string(row, col, data, preprocess_format(format))
             else:
                 return worksheet.write(row, col, data, preprocess_format(format))
 
         for col, header in enumerate(headers):
             # Header cell_processing.
             width = self.get_col_width(request, columns_spec[col], headers[col], col)
```

