# Comparing `tmp/novadata_utils-0.2.4.tar.gz` & `tmp/novadata_utils-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "novadata_utils-0.2.4.tar", last modified: Thu Apr 20 10:40:54 2023, max compression
+gzip compressed data, was "novadata_utils-0.2.5.tar", last modified: Sat May 20 14:16:37 2023, max compression
```

## Comparing `novadata_utils-0.2.4.tar` & `novadata_utils-0.2.5.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-20 10:40:53.998432 novadata_utils-0.2.4/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)     1066 2023-04-04 12:57:52.000000 novadata_utils-0.2.4/LICENSE
--rw-rw-r--   0 flavio    (1000) flavio    (1000)     1018 2023-04-20 10:40:53.998432 novadata_utils-0.2.4/PKG-INFO
--rw-rw-r--   0 flavio    (1000) flavio    (1000)      573 2023-04-16 16:52:43.000000 novadata_utils-0.2.4/README.md
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-20 10:40:53.994428 novadata_utils-0.2.4/novadata_utils/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       60 2023-04-04 12:57:52.000000 novadata_utils-0.2.4/novadata_utils/__init__.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-20 10:40:53.994428 novadata_utils-0.2.4/novadata_utils/admin/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       92 2023-04-04 12:57:52.000000 novadata_utils-0.2.4/novadata_utils/admin/__init__.py
--rw-rw-r--   0 flavio    (1000) flavio    (1000)     4353 2023-04-10 14:26:47.000000 novadata_utils-0.2.4/novadata_utils/admin/novadata_model_admin.py
--rw-rw-r--   0 flavio    (1000) flavio    (1000)      219 2023-04-04 12:57:52.000000 novadata_utils-0.2.4/novadata_utils/apps.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-20 10:40:53.994428 novadata_utils-0.2.4/novadata_utils/auth/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       92 2023-04-04 12:57:52.000000 novadata_utils-0.2.4/novadata_utils/auth/__init__.py
--rw-rw-r--   0 flavio    (1000) flavio    (1000)      729 2023-04-04 12:57:52.000000 novadata_utils-0.2.4/novadata_utils/auth/login_username_email.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-20 10:40:53.994428 novadata_utils-0.2.4/novadata_utils/forms/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       20 2023-04-04 12:57:52.000000 novadata_utils-0.2.4/novadata_utils/forms/__init__.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-20 10:40:53.994428 novadata_utils-0.2.4/novadata_utils/functions/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)      177 2023-04-16 18:28:57.000000 novadata_utils-0.2.4/novadata_utils/functions/__init__.py
--rw-rw-r--   0 flavio    (1000) flavio    (1000)     2186 2023-04-16 18:28:38.000000 novadata_utils-0.2.4/novadata_utils/functions/get_prop.py
--rw-rw-r--   0 flavio    (1000) flavio    (1000)     2979 2023-04-16 18:28:07.000000 novadata_utils-0.2.4/novadata_utils/functions/props_dict.py
--rw-rw-r--   0 flavio    (1000) flavio    (1000)      416 2023-04-10 14:19:49.000000 novadata_utils-0.2.4/novadata_utils/functions/transform_field.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-20 10:40:53.998432 novadata_utils-0.2.4/novadata_utils/managers/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       20 2023-04-04 12:57:52.000000 novadata_utils-0.2.4/novadata_utils/managers/__init__.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-20 10:40:53.998432 novadata_utils-0.2.4/novadata_utils/middlewares/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       20 2023-04-04 12:57:52.000000 novadata_utils-0.2.4/novadata_utils/middlewares/__init__.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-20 10:40:53.998432 novadata_utils-0.2.4/novadata_utils/migrations/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)     1232 2023-04-04 12:57:52.000000 novadata_utils-0.2.4/novadata_utils/migrations/0001_initial.py
--rw-rw-r--   0 flavio    (1000) flavio    (1000)        0 2023-04-04 12:57:52.000000 novadata_utils-0.2.4/novadata_utils/migrations/__init__.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-20 10:40:53.998432 novadata_utils-0.2.4/novadata_utils/models/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       76 2023-04-04 12:57:52.000000 novadata_utils-0.2.4/novadata_utils/models/__init__.py
--rw-rw-r--   0 flavio    (1000) flavio    (1000)     1188 2023-04-04 12:57:52.000000 novadata_utils-0.2.4/novadata_utils/models/novadata_model.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-20 10:40:53.998432 novadata_utils-0.2.4/novadata_utils/redirect/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       87 2023-04-04 12:57:52.000000 novadata_utils-0.2.4/novadata_utils/redirect/__init__.py
--rw-rw-r--   0 flavio    (1000) flavio    (1000)     1130 2023-04-04 12:57:52.000000 novadata_utils-0.2.4/novadata_utils/redirect/reverse_lazy_plus.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-20 10:40:53.998432 novadata_utils-0.2.4/novadata_utils/save/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)      130 2023-04-04 12:57:52.000000 novadata_utils-0.2.4/novadata_utils/save/__init__.py
--rw-rw-r--   0 flavio    (1000) flavio    (1000)     1749 2023-04-04 12:57:52.000000 novadata_utils-0.2.4/novadata_utils/save/create_logs.py
--rw-rw-r--   0 flavio    (1000) flavio    (1000)     2152 2023-04-04 12:57:52.000000 novadata_utils-0.2.4/novadata_utils/save/get_changes.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-20 10:40:53.998432 novadata_utils-0.2.4/novadata_utils/serializers/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)      107 2023-04-04 12:57:52.000000 novadata_utils-0.2.4/novadata_utils/serializers/__init__.py
--rw-rw-r--   0 flavio    (1000) flavio    (1000)     1934 2023-04-16 16:54:07.000000 novadata_utils-0.2.4/novadata_utils/serializers/novadata_model_serializer.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-20 10:40:53.998432 novadata_utils-0.2.4/novadata_utils/signals/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       20 2023-04-04 12:57:52.000000 novadata_utils-0.2.4/novadata_utils/signals/__init__.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-20 10:40:53.998432 novadata_utils-0.2.4/novadata_utils/templatetags/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)        0 2023-04-04 12:57:52.000000 novadata_utils-0.2.4/novadata_utils/templatetags/__init__.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-20 10:40:53.998432 novadata_utils-0.2.4/novadata_utils/tests/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)        0 2023-04-04 12:57:52.000000 novadata_utils-0.2.4/novadata_utils/tests/__init__.py
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       58 2023-04-04 12:57:52.000000 novadata_utils-0.2.4/novadata_utils/urls.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-20 10:40:53.998432 novadata_utils-0.2.4/novadata_utils/views/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       20 2023-04-04 12:57:52.000000 novadata_utils-0.2.4/novadata_utils/views/__init__.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-20 10:40:53.998432 novadata_utils-0.2.4/novadata_utils/viewsets/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       98 2023-04-04 12:57:52.000000 novadata_utils-0.2.4/novadata_utils/viewsets/__init__.py
--rw-rw-r--   0 flavio    (1000) flavio    (1000)     5457 2023-04-16 18:25:27.000000 novadata_utils-0.2.4/novadata_utils/viewsets/novadata_model_viewset.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-04-20 10:40:53.994428 novadata_utils-0.2.4/novadata_utils.egg-info/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)     1018 2023-04-20 10:40:53.000000 novadata_utils-0.2.4/novadata_utils.egg-info/PKG-INFO
--rw-rw-r--   0 flavio    (1000) flavio    (1000)     1366 2023-04-20 10:40:53.000000 novadata_utils-0.2.4/novadata_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 flavio    (1000) flavio    (1000)        1 2023-04-20 10:40:53.000000 novadata_utils-0.2.4/novadata_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 flavio    (1000) flavio    (1000)      123 2023-04-20 10:40:53.000000 novadata_utils-0.2.4/novadata_utils.egg-info/requires.txt
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       15 2023-04-20 10:40:53.000000 novadata_utils-0.2.4/novadata_utils.egg-info/top_level.txt
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       38 2023-04-20 10:40:53.998432 novadata_utils-0.2.4/setup.cfg
--rw-rw-r--   0 flavio    (1000) flavio    (1000)      878 2023-04-20 10:40:48.000000 novadata_utils-0.2.4/setup.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-05-20 14:16:37.618249 novadata_utils-0.2.5/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)     1066 2023-04-04 12:57:52.000000 novadata_utils-0.2.5/LICENSE
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)     1179 2023-05-20 14:16:37.618249 novadata_utils-0.2.5/PKG-INFO
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)      734 2023-05-20 14:16:14.000000 novadata_utils-0.2.5/README.md
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-05-20 14:16:37.614249 novadata_utils-0.2.5/novadata_utils/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       60 2023-04-04 12:57:52.000000 novadata_utils-0.2.5/novadata_utils/__init__.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-05-20 14:16:37.614249 novadata_utils-0.2.5/novadata_utils/admin/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       92 2023-04-04 12:57:52.000000 novadata_utils-0.2.5/novadata_utils/admin/__init__.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)     4435 2023-05-20 14:12:24.000000 novadata_utils-0.2.5/novadata_utils/admin/novadata_model_admin.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)      219 2023-04-04 12:57:52.000000 novadata_utils-0.2.5/novadata_utils/apps.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-05-20 14:16:37.614249 novadata_utils-0.2.5/novadata_utils/auth/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       92 2023-04-04 12:57:52.000000 novadata_utils-0.2.5/novadata_utils/auth/__init__.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)      729 2023-04-04 12:57:52.000000 novadata_utils-0.2.5/novadata_utils/auth/login_username_email.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-05-20 14:16:37.614249 novadata_utils-0.2.5/novadata_utils/forms/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       20 2023-04-04 12:57:52.000000 novadata_utils-0.2.5/novadata_utils/forms/__init__.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-05-20 14:16:37.614249 novadata_utils-0.2.5/novadata_utils/functions/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)      177 2023-04-16 18:28:57.000000 novadata_utils-0.2.5/novadata_utils/functions/__init__.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)     2186 2023-04-16 18:28:38.000000 novadata_utils-0.2.5/novadata_utils/functions/get_prop.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)     2979 2023-04-16 18:28:07.000000 novadata_utils-0.2.5/novadata_utils/functions/props_dict.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)      416 2023-04-10 14:19:49.000000 novadata_utils-0.2.5/novadata_utils/functions/transform_field.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-05-20 14:16:37.614249 novadata_utils-0.2.5/novadata_utils/managers/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       20 2023-04-04 12:57:52.000000 novadata_utils-0.2.5/novadata_utils/managers/__init__.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-05-20 14:16:37.614249 novadata_utils-0.2.5/novadata_utils/middlewares/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       20 2023-04-04 12:57:52.000000 novadata_utils-0.2.5/novadata_utils/middlewares/__init__.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-05-20 14:16:37.618249 novadata_utils-0.2.5/novadata_utils/migrations/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)     1232 2023-04-04 12:57:52.000000 novadata_utils-0.2.5/novadata_utils/migrations/0001_initial.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)        0 2023-04-04 12:57:52.000000 novadata_utils-0.2.5/novadata_utils/migrations/__init__.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-05-20 14:16:37.618249 novadata_utils-0.2.5/novadata_utils/models/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       76 2023-04-04 12:57:52.000000 novadata_utils-0.2.5/novadata_utils/models/__init__.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)     1188 2023-04-04 12:57:52.000000 novadata_utils-0.2.5/novadata_utils/models/novadata_model.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-05-20 14:16:37.618249 novadata_utils-0.2.5/novadata_utils/redirect/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       87 2023-04-04 12:57:52.000000 novadata_utils-0.2.5/novadata_utils/redirect/__init__.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)     1130 2023-04-04 12:57:52.000000 novadata_utils-0.2.5/novadata_utils/redirect/reverse_lazy_plus.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-05-20 14:16:37.618249 novadata_utils-0.2.5/novadata_utils/save/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)      130 2023-04-04 12:57:52.000000 novadata_utils-0.2.5/novadata_utils/save/__init__.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)     1749 2023-04-04 12:57:52.000000 novadata_utils-0.2.5/novadata_utils/save/create_logs.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)     2152 2023-04-04 12:57:52.000000 novadata_utils-0.2.5/novadata_utils/save/get_changes.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-05-20 14:16:37.618249 novadata_utils-0.2.5/novadata_utils/serializers/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)      107 2023-04-04 12:57:52.000000 novadata_utils-0.2.5/novadata_utils/serializers/__init__.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)     1934 2023-04-16 16:54:07.000000 novadata_utils-0.2.5/novadata_utils/serializers/novadata_model_serializer.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-05-20 14:16:37.618249 novadata_utils-0.2.5/novadata_utils/signals/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       20 2023-04-04 12:57:52.000000 novadata_utils-0.2.5/novadata_utils/signals/__init__.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-05-20 14:16:37.618249 novadata_utils-0.2.5/novadata_utils/templatetags/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)        0 2023-04-04 12:57:52.000000 novadata_utils-0.2.5/novadata_utils/templatetags/__init__.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-05-20 14:16:37.618249 novadata_utils-0.2.5/novadata_utils/tests/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)        0 2023-04-04 12:57:52.000000 novadata_utils-0.2.5/novadata_utils/tests/__init__.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       58 2023-04-04 12:57:52.000000 novadata_utils-0.2.5/novadata_utils/urls.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-05-20 14:16:37.618249 novadata_utils-0.2.5/novadata_utils/views/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       20 2023-04-04 12:57:52.000000 novadata_utils-0.2.5/novadata_utils/views/__init__.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-05-20 14:16:37.618249 novadata_utils-0.2.5/novadata_utils/viewsets/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       98 2023-04-04 12:57:52.000000 novadata_utils-0.2.5/novadata_utils/viewsets/__init__.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)     5457 2023-04-16 18:25:27.000000 novadata_utils-0.2.5/novadata_utils/viewsets/novadata_model_viewset.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-05-20 14:16:37.614249 novadata_utils-0.2.5/novadata_utils.egg-info/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)     1179 2023-05-20 14:16:37.000000 novadata_utils-0.2.5/novadata_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)     1366 2023-05-20 14:16:37.000000 novadata_utils-0.2.5/novadata_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)        1 2023-05-20 14:16:37.000000 novadata_utils-0.2.5/novadata_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)      147 2023-05-20 14:16:37.000000 novadata_utils-0.2.5/novadata_utils.egg-info/requires.txt
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       15 2023-05-20 14:16:37.000000 novadata_utils-0.2.5/novadata_utils.egg-info/top_level.txt
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       38 2023-05-20 14:16:37.618249 novadata_utils-0.2.5/setup.cfg
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)      913 2023-05-20 14:16:34.000000 novadata_utils-0.2.5/setup.py
```

### Comparing `novadata_utils-0.2.4/LICENSE` & `novadata_utils-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `novadata_utils-0.2.4/PKG-INFO` & `novadata_utils-0.2.5/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: novadata_utils
-Version: 0.2.4
+Version: 0.2.5
 Summary: novadata utils
 Home-page: https://github.com/TimeNovaData/novadata_utils/
 Author: Flávio Silva
 Author-email: flavio.nogueira.profissional@gmail.com
 License: MIT License
 Project-URL: GitHub, https://github.com/TimeNovaData/novadata_utils/
 Keywords: Django,utils,ndt,novadata,nova data,nova,data
@@ -26,21 +26,32 @@
 pip install novadata-utils
 ```
 
 Settings.py:
 ```python
 INSTALLED_APPS = [
     ...
+    'advanced_filters',
     'django_admin_listfilter_dropdown',
     'django_object_actions',
     'import_export',
     'novadata_utils',
     'rest_framework',
     ...
 ]
+```
+
+Urls.py principal:
+```python
+urlpatterns = [
+    ...
+    path('advanced_filters/', include('advanced_filters.urls')),
+    ...
+]
+```
 
 MIDDLEWARE += ('crum.CurrentRequestUserMiddleware',)
 ```
 
 Rode os seguintes comandos:
 ```python
 python manage.py makemigrations
```

### Comparing `novadata_utils-0.2.4/README.md` & `novadata_utils-0.2.5/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -12,21 +12,32 @@
 pip install novadata-utils
 ```
 
 Settings.py:
 ```python
 INSTALLED_APPS = [
     ...
+    'advanced_filters',
     'django_admin_listfilter_dropdown',
     'django_object_actions',
     'import_export',
     'novadata_utils',
     'rest_framework',
     ...
 ]
+```
+
+Urls.py principal:
+```python
+urlpatterns = [
+    ...
+    path('advanced_filters/', include('advanced_filters.urls')),
+    ...
+]
+```
 
 MIDDLEWARE += ('crum.CurrentRequestUserMiddleware',)
 ```
 
 Rode os seguintes comandos:
 ```python
 python manage.py makemigrations
```

### Comparing `novadata_utils-0.2.4/novadata_utils/admin/novadata_model_admin.py` & `novadata_utils-0.2.5/novadata_utils/admin/novadata_model_admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from functools import partial
 
+from advanced_filters.admin import AdminAdvancedFiltersMixin
 from django.contrib import admin
 from django_object_actions import DjangoObjectActions
-from import_export.admin import ImportExportModelAdmin
+from import_export.admin import ImportExportMixin
 
 from novadata_utils.functions import get_prop, transform_field
 
 
 class NovadataModelAdmin(
+    AdminAdvancedFiltersMixin,
+    ImportExportMixin,
     DjangoObjectActions,
-    ImportExportModelAdmin,
     admin.ModelAdmin,
 ):
     """
     Classe para realizar funcionalidades default em todas as classes do admin.
 
     A mesma adiciona todos os campos possíveis nas seguintes propriedades:
     - list_display
```

### Comparing `novadata_utils-0.2.4/novadata_utils/auth/login_username_email.py` & `novadata_utils-0.2.5/novadata_utils/auth/login_username_email.py`

 * *Files identical despite different names*

### Comparing `novadata_utils-0.2.4/novadata_utils/functions/get_prop.py` & `novadata_utils-0.2.5/novadata_utils/functions/get_prop.py`

 * *Files identical despite different names*

### Comparing `novadata_utils-0.2.4/novadata_utils/functions/props_dict.py` & `novadata_utils-0.2.5/novadata_utils/functions/props_dict.py`

 * *Files identical despite different names*

### Comparing `novadata_utils-0.2.4/novadata_utils/migrations/0001_initial.py` & `novadata_utils-0.2.5/novadata_utils/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `novadata_utils-0.2.4/novadata_utils/models/novadata_model.py` & `novadata_utils-0.2.5/novadata_utils/models/novadata_model.py`

 * *Files identical despite different names*

### Comparing `novadata_utils-0.2.4/novadata_utils/redirect/reverse_lazy_plus.py` & `novadata_utils-0.2.5/novadata_utils/redirect/reverse_lazy_plus.py`

 * *Files identical despite different names*

### Comparing `novadata_utils-0.2.4/novadata_utils/save/create_logs.py` & `novadata_utils-0.2.5/novadata_utils/save/create_logs.py`

 * *Files identical despite different names*

### Comparing `novadata_utils-0.2.4/novadata_utils/save/get_changes.py` & `novadata_utils-0.2.5/novadata_utils/save/get_changes.py`

 * *Files identical despite different names*

### Comparing `novadata_utils-0.2.4/novadata_utils/serializers/novadata_model_serializer.py` & `novadata_utils-0.2.5/novadata_utils/serializers/novadata_model_serializer.py`

 * *Files identical despite different names*

### Comparing `novadata_utils-0.2.4/novadata_utils/viewsets/novadata_model_viewset.py` & `novadata_utils-0.2.5/novadata_utils/viewsets/novadata_model_viewset.py`

 * *Files identical despite different names*

### Comparing `novadata_utils-0.2.4/novadata_utils.egg-info/PKG-INFO` & `novadata_utils-0.2.5/novadata_utils.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: novadata-utils
-Version: 0.2.4
+Version: 0.2.5
 Summary: novadata utils
 Home-page: https://github.com/TimeNovaData/novadata_utils/
 Author: Flávio Silva
 Author-email: flavio.nogueira.profissional@gmail.com
 License: MIT License
 Project-URL: GitHub, https://github.com/TimeNovaData/novadata_utils/
 Keywords: Django,utils,ndt,novadata,nova data,nova,data
@@ -26,21 +26,32 @@
 pip install novadata-utils
 ```
 
 Settings.py:
 ```python
 INSTALLED_APPS = [
     ...
+    'advanced_filters',
     'django_admin_listfilter_dropdown',
     'django_object_actions',
     'import_export',
     'novadata_utils',
     'rest_framework',
     ...
 ]
+```
+
+Urls.py principal:
+```python
+urlpatterns = [
+    ...
+    path('advanced_filters/', include('advanced_filters.urls')),
+    ...
+]
+```
 
 MIDDLEWARE += ('crum.CurrentRequestUserMiddleware',)
 ```
 
 Rode os seguintes comandos:
 ```python
 python manage.py makemigrations
```

### Comparing `novadata_utils-0.2.4/novadata_utils.egg-info/SOURCES.txt` & `novadata_utils-0.2.5/novadata_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `novadata_utils-0.2.4/setup.py` & `novadata_utils-0.2.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     readme = fh.read()
 
 setup(
     name="novadata_utils",
-    version="0.2.4",
+    version="0.2.5",
     url="https://github.com/TimeNovaData/novadata_utils/",
     license="MIT License",
     author="Flávio Silva",
     long_description=readme,
     long_description_content_type="text/markdown",
     author_email="flavio.nogueira.profissional@gmail.com",
     keywords="Django, utils, ndt, novadata, nova data, nova, data",
     description="novadata utils",
     packages=find_packages(),
     install_requires=[
         "django",
         "djangorestframework",
         "django-admin-list-filter-dropdown",
+        "django-advanced-filters",
         "django-crum",
         "django-import-export",
         "django-object-actions>=4.0.0",
     ],
     project_urls={
         "GitHub": "https://github.com/TimeNovaData/novadata_utils/",
     },
```

