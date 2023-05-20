# Comparing `tmp/django_tbase_config-2023.5.2016845974.tar.gz` & `tmp/django_tbase_config-2023.5.2016845975.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_tbase_config-2023.5.2016845974.tar", last modified: Sat May 20 15:43:35 2023, max compression
+gzip compressed data, was "django_tbase_config-2023.5.2016845975.tar", last modified: Sat May 20 15:45:58 2023, max compression
```

## Comparing `django_tbase_config-2023.5.2016845974.tar` & `django_tbase_config-2023.5.2016845975.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 15:43:35.021459 django_tbase_config-2023.5.2016845974/
--rw-r--r--   0 terry     (1000) terry     (1000)      988 2023-05-20 15:43:35.021459 django_tbase_config-2023.5.2016845974/PKG-INFO
--rw-r--r--   0 terry     (1000) terry     (1000)      675 2023-05-20 15:41:22.000000 django_tbase_config-2023.5.2016845974/README.md
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 15:43:35.011459 django_tbase_config-2023.5.2016845974/django_tbase_config.egg-info/
--rw-r--r--   0 terry     (1000) terry     (1000)      988 2023-05-20 15:43:34.000000 django_tbase_config-2023.5.2016845974/django_tbase_config.egg-info/PKG-INFO
--rw-r--r--   0 terry     (1000) terry     (1000)      325 2023-05-20 15:43:34.000000 django_tbase_config-2023.5.2016845974/django_tbase_config.egg-info/SOURCES.txt
--rw-r--r--   0 terry     (1000) terry     (1000)        1 2023-05-20 15:43:34.000000 django_tbase_config-2023.5.2016845974/django_tbase_config.egg-info/dependency_links.txt
--rw-r--r--   0 terry     (1000) terry     (1000)       13 2023-05-20 15:43:34.000000 django_tbase_config-2023.5.2016845974/django_tbase_config.egg-info/top_level.txt
--rw-r--r--   0 terry     (1000) terry     (1000)       38 2023-05-20 15:43:35.021459 django_tbase_config-2023.5.2016845974/setup.cfg
--rw-r--r--   0 terry     (1000) terry     (1000)     2241 2023-05-20 15:43:21.000000 django_tbase_config-2023.5.2016845974/setup.py
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 15:43:35.021459 django_tbase_config-2023.5.2016845974/tbase_config/
--rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:08.000000 django_tbase_config-2023.5.2016845974/tbase_config/__init__.py
--rw-r--r--   0 terry     (1000) terry     (1000)     1351 2023-04-27 16:40:08.000000 django_tbase_config-2023.5.2016845974/tbase_config/admin.py
--rw-r--r--   0 terry     (1000) terry     (1000)      150 2023-04-27 16:40:08.000000 django_tbase_config-2023.5.2016845974/tbase_config/apps.py
--rw-r--r--   0 terry     (1000) terry     (1000)     2554 2023-04-27 16:40:08.000000 django_tbase_config-2023.5.2016845974/tbase_config/models.py
--rw-r--r--   0 terry     (1000) terry     (1000)       60 2023-04-27 16:40:08.000000 django_tbase_config-2023.5.2016845974/tbase_config/tests.py
--rw-r--r--   0 terry     (1000) terry     (1000)       63 2023-04-27 16:40:08.000000 django_tbase_config-2023.5.2016845974/tbase_config/views.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 15:45:58.011441 django_tbase_config-2023.5.2016845975/
+-rw-r--r--   0 terry     (1000) terry     (1000)      988 2023-05-20 15:45:58.011441 django_tbase_config-2023.5.2016845975/PKG-INFO
+-rw-r--r--   0 terry     (1000) terry     (1000)      675 2023-05-20 15:41:22.000000 django_tbase_config-2023.5.2016845975/README.md
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 15:45:58.011441 django_tbase_config-2023.5.2016845975/django_tbase_config.egg-info/
+-rw-r--r--   0 terry     (1000) terry     (1000)      988 2023-05-20 15:45:57.000000 django_tbase_config-2023.5.2016845975/django_tbase_config.egg-info/PKG-INFO
+-rw-r--r--   0 terry     (1000) terry     (1000)      367 2023-05-20 15:45:57.000000 django_tbase_config-2023.5.2016845975/django_tbase_config.egg-info/SOURCES.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)        1 2023-05-20 15:45:57.000000 django_tbase_config-2023.5.2016845975/django_tbase_config.egg-info/dependency_links.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)       19 2023-05-20 15:45:57.000000 django_tbase_config-2023.5.2016845975/django_tbase_config.egg-info/requires.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)       13 2023-05-20 15:45:57.000000 django_tbase_config-2023.5.2016845975/django_tbase_config.egg-info/top_level.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)       38 2023-05-20 15:45:58.011441 django_tbase_config-2023.5.2016845975/setup.cfg
+-rw-r--r--   0 terry     (1000) terry     (1000)     2270 2023-05-20 15:45:42.000000 django_tbase_config-2023.5.2016845975/setup.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 15:45:58.011441 django_tbase_config-2023.5.2016845975/tbase_config/
+-rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:08.000000 django_tbase_config-2023.5.2016845975/tbase_config/__init__.py
+-rw-r--r--   0 terry     (1000) terry     (1000)     1351 2023-04-27 16:40:08.000000 django_tbase_config-2023.5.2016845975/tbase_config/admin.py
+-rw-r--r--   0 terry     (1000) terry     (1000)      150 2023-04-27 16:40:08.000000 django_tbase_config-2023.5.2016845975/tbase_config/apps.py
+-rw-r--r--   0 terry     (1000) terry     (1000)     2554 2023-04-27 16:40:08.000000 django_tbase_config-2023.5.2016845975/tbase_config/models.py
+-rw-r--r--   0 terry     (1000) terry     (1000)       60 2023-04-27 16:40:08.000000 django_tbase_config-2023.5.2016845975/tbase_config/tests.py
+-rw-r--r--   0 terry     (1000) terry     (1000)       63 2023-04-27 16:40:08.000000 django_tbase_config-2023.5.2016845975/tbase_config/views.py
```

### Comparing `django_tbase_config-2023.5.2016845974/PKG-INFO` & `django_tbase_config-2023.5.2016845975/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_tbase_config
-Version: 2023.5.2016845974
+Version: 2023.5.2016845975
 Summary: Terry django base config ,
 Home-page: https://terrychanorg.jetbrains.space/p/django-expand/repositories/tbase_config/files/README.md
 Author: Terry Chan
 Author-email: napoler2008@gmail.com
 Description-Content-Type: text/markdown
 
 # django-expand/tbase_config
```

### Comparing `django_tbase_config-2023.5.2016845974/README.md` & `django_tbase_config-2023.5.2016845975/README.md`

 * *Files identical despite different names*

### Comparing `django_tbase_config-2023.5.2016845974/django_tbase_config.egg-info/PKG-INFO` & `django_tbase_config-2023.5.2016845975/django_tbase_config.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-tbase-config
-Version: 2023.5.2016845974
+Version: 2023.5.2016845975
 Summary: Terry django base config ,
 Home-page: https://terrychanorg.jetbrains.space/p/django-expand/repositories/tbase_config/files/README.md
 Author: Terry Chan
 Author-email: napoler2008@gmail.com
 Description-Content-Type: text/markdown
 
 # django-expand/tbase_config
```

### Comparing `django_tbase_config-2023.5.2016845974/setup.py` & `django_tbase_config-2023.5.2016845975/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,14 +59,15 @@
     author_email=author_email,
     url=url,
     # install_requires=read_requirements('requirements.txt'),  # 指定需要安装的依赖
     long_description=long_description,
     long_description_content_type="text/markdown",
     # 依赖文件
     install_requires=[
+        'django-solo==2.0.0'
         # 'django-tbase-theme-tailwind>=2023.5.2016845966',
         # 'sentence-splitter>=1.4',
         # 'requests>=2.28.1',
         # 'nltk>=3.7'
     ],
     packages=['tbase_config'],  # 扫描的目录
     nclude_package_data=True,  # 打包包含静态文件标识
```

### Comparing `django_tbase_config-2023.5.2016845974/tbase_config/admin.py` & `django_tbase_config-2023.5.2016845975/tbase_config/admin.py`

 * *Files identical despite different names*

### Comparing `django_tbase_config-2023.5.2016845974/tbase_config/models.py` & `django_tbase_config-2023.5.2016845975/tbase_config/models.py`

 * *Files identical despite different names*

