# Comparing `tmp/django_tbase_post-2023.5.2016845963.tar.gz` & `tmp/django_tbase_post-2023.5.2016845969.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_tbase_post-2023.5.2016845963.tar", last modified: Sat May 20 15:25:51 2023, max compression
+gzip compressed data, was "django_tbase_post-2023.5.2016845969.tar", last modified: Sat May 20 15:35:26 2023, max compression
```

## Comparing `django_tbase_post-2023.5.2016845963.tar` & `django_tbase_post-2023.5.2016845969.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 15:25:51.891600 django_tbase_post-2023.5.2016845963/
--rw-r--r--   0 terry     (1000) terry     (1000)      976 2023-05-20 15:25:51.891600 django_tbase_post-2023.5.2016845963/PKG-INFO
--rw-r--r--   0 terry     (1000) terry     (1000)      669 2023-05-20 15:21:16.000000 django_tbase_post-2023.5.2016845963/README.md
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 15:25:51.891600 django_tbase_post-2023.5.2016845963/django_tbase_post.egg-info/
--rw-r--r--   0 terry     (1000) terry     (1000)      976 2023-05-20 15:25:51.000000 django_tbase_post-2023.5.2016845963/django_tbase_post.egg-info/PKG-INFO
--rw-r--r--   0 terry     (1000) terry     (1000)      324 2023-05-20 15:25:51.000000 django_tbase_post-2023.5.2016845963/django_tbase_post.egg-info/SOURCES.txt
--rw-r--r--   0 terry     (1000) terry     (1000)        1 2023-05-20 15:25:51.000000 django_tbase_post-2023.5.2016845963/django_tbase_post.egg-info/dependency_links.txt
--rw-r--r--   0 terry     (1000) terry     (1000)       11 2023-05-20 15:25:51.000000 django_tbase_post-2023.5.2016845963/django_tbase_post.egg-info/top_level.txt
--rw-r--r--   0 terry     (1000) terry     (1000)       38 2023-05-20 15:25:51.891600 django_tbase_post-2023.5.2016845963/setup.cfg
--rw-r--r--   0 terry     (1000) terry     (1000)     2200 2023-05-20 15:24:31.000000 django_tbase_post-2023.5.2016845963/setup.py
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 15:25:51.891600 django_tbase_post-2023.5.2016845963/tbase_post/
--rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:08.000000 django_tbase_post-2023.5.2016845963/tbase_post/__init__.py
--rw-r--r--   0 terry     (1000) terry     (1000)      817 2023-04-27 16:40:08.000000 django_tbase_post-2023.5.2016845963/tbase_post/admin.py
--rw-r--r--   0 terry     (1000) terry     (1000)      146 2023-04-27 16:40:08.000000 django_tbase_post-2023.5.2016845963/tbase_post/apps.py
--rw-r--r--   0 terry     (1000) terry     (1000)     1424 2023-04-27 16:40:08.000000 django_tbase_post-2023.5.2016845963/tbase_post/models.py
--rw-r--r--   0 terry     (1000) terry     (1000)       60 2023-04-27 16:40:08.000000 django_tbase_post-2023.5.2016845963/tbase_post/tests.py
--rw-r--r--   0 terry     (1000) terry     (1000)      451 2023-05-01 19:22:36.000000 django_tbase_post-2023.5.2016845963/tbase_post/urls.py
--rw-r--r--   0 terry     (1000) terry     (1000)     3232 2023-05-01 19:22:30.000000 django_tbase_post-2023.5.2016845963/tbase_post/views.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 15:35:26.811523 django_tbase_post-2023.5.2016845969/
+-rw-r--r--   0 terry     (1000) terry     (1000)      976 2023-05-20 15:35:26.811523 django_tbase_post-2023.5.2016845969/PKG-INFO
+-rw-r--r--   0 terry     (1000) terry     (1000)      669 2023-05-20 15:21:16.000000 django_tbase_post-2023.5.2016845969/README.md
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 15:35:26.811523 django_tbase_post-2023.5.2016845969/django_tbase_post.egg-info/
+-rw-r--r--   0 terry     (1000) terry     (1000)      976 2023-05-20 15:35:26.000000 django_tbase_post-2023.5.2016845969/django_tbase_post.egg-info/PKG-INFO
+-rw-r--r--   0 terry     (1000) terry     (1000)      364 2023-05-20 15:35:26.000000 django_tbase_post-2023.5.2016845969/django_tbase_post.egg-info/SOURCES.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)        1 2023-05-20 15:35:26.000000 django_tbase_post-2023.5.2016845969/django_tbase_post.egg-info/dependency_links.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)       47 2023-05-20 15:35:26.000000 django_tbase_post-2023.5.2016845969/django_tbase_post.egg-info/requires.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)       11 2023-05-20 15:35:26.000000 django_tbase_post-2023.5.2016845969/django_tbase_post.egg-info/top_level.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)       38 2023-05-20 15:35:26.811523 django_tbase_post-2023.5.2016845969/setup.cfg
+-rw-r--r--   0 terry     (1000) terry     (1000)     2231 2023-05-20 15:35:20.000000 django_tbase_post-2023.5.2016845969/setup.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 15:35:26.811523 django_tbase_post-2023.5.2016845969/tbase_post/
+-rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:08.000000 django_tbase_post-2023.5.2016845969/tbase_post/__init__.py
+-rw-r--r--   0 terry     (1000) terry     (1000)      817 2023-04-27 16:40:08.000000 django_tbase_post-2023.5.2016845969/tbase_post/admin.py
+-rw-r--r--   0 terry     (1000) terry     (1000)      146 2023-04-27 16:40:08.000000 django_tbase_post-2023.5.2016845969/tbase_post/apps.py
+-rw-r--r--   0 terry     (1000) terry     (1000)     1424 2023-04-27 16:40:08.000000 django_tbase_post-2023.5.2016845969/tbase_post/models.py
+-rw-r--r--   0 terry     (1000) terry     (1000)       60 2023-04-27 16:40:08.000000 django_tbase_post-2023.5.2016845969/tbase_post/tests.py
+-rw-r--r--   0 terry     (1000) terry     (1000)      451 2023-05-01 19:22:36.000000 django_tbase_post-2023.5.2016845969/tbase_post/urls.py
+-rw-r--r--   0 terry     (1000) terry     (1000)     3232 2023-05-01 19:22:30.000000 django_tbase_post-2023.5.2016845969/tbase_post/views.py
```

### Comparing `django_tbase_post-2023.5.2016845963/PKG-INFO` & `django_tbase_post-2023.5.2016845969/django_tbase_post.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: django_tbase_post
-Version: 2023.5.2016845963
+Name: django-tbase-post
+Version: 2023.5.2016845969
 Summary: Terry django base post ,
 Home-page: https://terrychanorg.jetbrains.space/p/django-expand/repositories/tbase_post/files/README.md
 Author: Terry Chan
 Author-email: napoler2008@gmail.com
 Description-Content-Type: text/markdown
 
 # django-expand/tbase_post
```

### Comparing `django_tbase_post-2023.5.2016845963/README.md` & `django_tbase_post-2023.5.2016845969/README.md`

 * *Files identical despite different names*

### Comparing `django_tbase_post-2023.5.2016845963/django_tbase_post.egg-info/PKG-INFO` & `django_tbase_post-2023.5.2016845969/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: django-tbase-post
-Version: 2023.5.2016845963
+Name: django_tbase_post
+Version: 2023.5.2016845969
 Summary: Terry django base post ,
 Home-page: https://terrychanorg.jetbrains.space/p/django-expand/repositories/tbase_post/files/README.md
 Author: Terry Chan
 Author-email: napoler2008@gmail.com
 Description-Content-Type: text/markdown
 
 # django-expand/tbase_post
```

### Comparing `django_tbase_post-2023.5.2016845963/setup.py` & `django_tbase_post-2023.5.2016845969/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     author_email=author_email,
     url=url,
     # install_requires=read_requirements('requirements.txt'),  # 指定需要安装的依赖
     long_description=long_description,
     long_description_content_type="text/markdown",
     # 依赖文件
     install_requires=[
-        # 'pregex>=2.1.0',
+        'django-tbase-theme-tailwind>=2023.5.2016845966',
         # 'sentence-splitter>=1.4',
         # 'requests>=2.28.1',
         # 'nltk>=3.7'
     ],
     packages=['tbase_post'],  # 扫描的目录
     nclude_package_data=True,  # 打包包含静态文件标识
 )
```

### Comparing `django_tbase_post-2023.5.2016845963/tbase_post/admin.py` & `django_tbase_post-2023.5.2016845969/tbase_post/admin.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post-2023.5.2016845963/tbase_post/models.py` & `django_tbase_post-2023.5.2016845969/tbase_post/models.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post-2023.5.2016845963/tbase_post/views.py` & `django_tbase_post-2023.5.2016845969/tbase_post/views.py`

 * *Files identical despite different names*

