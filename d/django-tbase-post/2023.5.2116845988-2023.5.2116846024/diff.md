# Comparing `tmp/django_tbase_post-2023.5.2116845988.tar.gz` & `tmp/django_tbase_post-2023.5.2116846024.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_tbase_post-2023.5.2116845988.tar", last modified: Sat May 20 16:08:03 2023, max compression
+gzip compressed data, was "django_tbase_post-2023.5.2116846024.tar", last modified: Sat May 20 17:06:56 2023, max compression
```

## Comparing `django_tbase_post-2023.5.2116845988.tar` & `django_tbase_post-2023.5.2116846024.tar`

### file list

```diff
@@ -1,19 +1,49 @@
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 16:08:03.021269 django_tbase_post-2023.5.2116845988/
--rw-r--r--   0 terry     (1000) terry     (1000)     1274 2023-05-20 16:08:03.021269 django_tbase_post-2023.5.2116845988/PKG-INFO
--rw-r--r--   0 terry     (1000) terry     (1000)      967 2023-05-20 15:52:14.000000 django_tbase_post-2023.5.2116845988/README.md
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 16:08:03.021269 django_tbase_post-2023.5.2116845988/django_tbase_post.egg-info/
--rw-r--r--   0 terry     (1000) terry     (1000)     1274 2023-05-20 16:08:02.000000 django_tbase_post-2023.5.2116845988/django_tbase_post.egg-info/PKG-INFO
--rw-r--r--   0 terry     (1000) terry     (1000)      364 2023-05-20 16:08:02.000000 django_tbase_post-2023.5.2116845988/django_tbase_post.egg-info/SOURCES.txt
--rw-r--r--   0 terry     (1000) terry     (1000)        1 2023-05-20 16:08:02.000000 django_tbase_post-2023.5.2116845988/django_tbase_post.egg-info/dependency_links.txt
--rw-r--r--   0 terry     (1000) terry     (1000)       83 2023-05-20 16:08:02.000000 django_tbase_post-2023.5.2116845988/django_tbase_post.egg-info/requires.txt
--rw-r--r--   0 terry     (1000) terry     (1000)       11 2023-05-20 16:08:02.000000 django_tbase_post-2023.5.2116845988/django_tbase_post.egg-info/top_level.txt
--rw-r--r--   0 terry     (1000) terry     (1000)       38 2023-05-20 16:08:03.021269 django_tbase_post-2023.5.2116845988/setup.cfg
--rw-r--r--   0 terry     (1000) terry     (1000)     2288 2023-05-20 15:53:05.000000 django_tbase_post-2023.5.2116845988/setup.py
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 16:08:03.021269 django_tbase_post-2023.5.2116845988/tbase_post/
--rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:08.000000 django_tbase_post-2023.5.2116845988/tbase_post/__init__.py
--rw-r--r--   0 terry     (1000) terry     (1000)      817 2023-04-27 16:40:08.000000 django_tbase_post-2023.5.2116845988/tbase_post/admin.py
--rw-r--r--   0 terry     (1000) terry     (1000)      146 2023-04-27 16:40:08.000000 django_tbase_post-2023.5.2116845988/tbase_post/apps.py
--rw-r--r--   0 terry     (1000) terry     (1000)     1424 2023-04-27 16:40:08.000000 django_tbase_post-2023.5.2116845988/tbase_post/models.py
--rw-r--r--   0 terry     (1000) terry     (1000)       60 2023-04-27 16:40:08.000000 django_tbase_post-2023.5.2116845988/tbase_post/tests.py
--rw-r--r--   0 terry     (1000) terry     (1000)      451 2023-05-01 19:22:36.000000 django_tbase_post-2023.5.2116845988/tbase_post/urls.py
--rw-r--r--   0 terry     (1000) terry     (1000)     3232 2023-05-01 19:22:30.000000 django_tbase_post-2023.5.2116845988/tbase_post/views.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 17:06:56.420798 django_tbase_post-2023.5.2116846024/
+-rw-r--r--   0 terry     (1000) terry     (1000)      143 2023-05-20 17:05:28.000000 django_tbase_post-2023.5.2116846024/MANIFEST.in
+-rw-r--r--   0 terry     (1000) terry     (1000)     1311 2023-05-20 17:06:56.420798 django_tbase_post-2023.5.2116846024/PKG-INFO
+-rw-r--r--   0 terry     (1000) terry     (1000)      967 2023-05-20 15:52:14.000000 django_tbase_post-2023.5.2116846024/README.md
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 17:06:56.420798 django_tbase_post-2023.5.2116846024/django_tbase_post.egg-info/
+-rw-r--r--   0 terry     (1000) terry     (1000)     1311 2023-05-20 17:06:56.000000 django_tbase_post-2023.5.2116846024/django_tbase_post.egg-info/PKG-INFO
+-rw-r--r--   0 terry     (1000) terry     (1000)     1458 2023-05-20 17:06:56.000000 django_tbase_post-2023.5.2116846024/django_tbase_post.egg-info/SOURCES.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)        1 2023-05-20 17:06:56.000000 django_tbase_post-2023.5.2116846024/django_tbase_post.egg-info/dependency_links.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)       83 2023-05-20 17:06:56.000000 django_tbase_post-2023.5.2116846024/django_tbase_post.egg-info/requires.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)       11 2023-05-20 17:06:56.000000 django_tbase_post-2023.5.2116846024/django_tbase_post.egg-info/top_level.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)       38 2023-05-20 17:06:56.420798 django_tbase_post-2023.5.2116846024/setup.cfg
+-rw-r--r--   0 terry     (1000) terry     (1000)     2289 2023-05-20 17:06:42.000000 django_tbase_post-2023.5.2116846024/setup.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 17:06:56.420798 django_tbase_post-2023.5.2116846024/tbase_post/
+-rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:08.000000 django_tbase_post-2023.5.2116846024/tbase_post/__init__.py
+-rw-r--r--   0 terry     (1000) terry     (1000)      817 2023-04-27 16:40:08.000000 django_tbase_post-2023.5.2116846024/tbase_post/admin.py
+-rw-r--r--   0 terry     (1000) terry     (1000)      146 2023-04-27 16:40:08.000000 django_tbase_post-2023.5.2116846024/tbase_post/apps.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 17:06:56.420798 django_tbase_post-2023.5.2116846024/tbase_post/migrations/
+-rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:09.000000 django_tbase_post-2023.5.2116846024/tbase_post/migrations/__init__.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 17:06:56.420798 django_tbase_post-2023.5.2116846024/tbase_post/migrations/__pycache__/
+-rw-r--r--   0 terry     (1000) terry     (1000)     1062 2023-04-27 16:50:46.000000 django_tbase_post-2023.5.2116846024/tbase_post/migrations/__pycache__/0001_initial.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     1092 2023-04-27 16:50:46.000000 django_tbase_post-2023.5.2116846024/tbase_post/migrations/__pycache__/0002_auto_20230421_1307.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)      168 2023-04-27 16:50:46.000000 django_tbase_post-2023.5.2116846024/tbase_post/migrations/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     1424 2023-04-27 16:40:08.000000 django_tbase_post-2023.5.2116846024/tbase_post/models.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 17:06:56.420798 django_tbase_post-2023.5.2116846024/tbase_post/static/
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 17:06:56.420798 django_tbase_post-2023.5.2116846024/tbase_post/static/images/
+-rw-r--r--   0 terry     (1000) terry     (1000)    59619 2023-04-27 16:40:09.000000 django_tbase_post-2023.5.2116846024/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg
+-rw-r--r--   0 terry     (1000) terry     (1000)       94 2023-04-27 16:40:09.000000 django_tbase_post-2023.5.2116846024/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg:Zone.Identifier
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 17:06:56.420798 django_tbase_post-2023.5.2116846024/tbase_post/templates/
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 17:06:56.420798 django_tbase_post-2023.5.2116846024/tbase_post/templates/post/
+-rw-r--r--   0 terry     (1000) terry     (1000)     2498 2023-04-27 16:40:09.000000 django_tbase_post-2023.5.2116846024/tbase_post/templates/post/article_list_by_tag.html
+-rw-r--r--   0 terry     (1000) terry     (1000)     1881 2023-04-27 16:40:09.000000 django_tbase_post-2023.5.2116846024/tbase_post/templates/post/blog_index.html
+-rw-r--r--   0 terry     (1000) terry     (1000)     3666 2023-04-27 18:02:44.000000 django_tbase_post-2023.5.2116846024/tbase_post/templates/post/detail.html
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 17:06:56.420798 django_tbase_post-2023.5.2116846024/tbase_post/templates/post/extras/
+-rw-r--r--   0 terry     (1000) terry     (1000)      294 2023-04-27 16:40:09.000000 django_tbase_post-2023.5.2116846024/tbase_post/templates/post/extras/related_post_by_tags.html
+-rw-r--r--   0 terry     (1000) terry     (1000)       94 2023-04-27 16:40:09.000000 django_tbase_post-2023.5.2116846024/tbase_post/templates/post/extras/related_post_by_tags.html:Zone.Identifier
+-rw-r--r--   0 terry     (1000) terry     (1000)      415 2023-05-01 19:23:09.000000 django_tbase_post-2023.5.2116846024/tbase_post/templates/post/extras/tags.html
+-rw-r--r--   0 terry     (1000) terry     (1000)       94 2023-04-27 16:40:09.000000 django_tbase_post-2023.5.2116846024/tbase_post/templates/post/extras/tags.html:Zone.Identifier
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 17:06:56.420798 django_tbase_post-2023.5.2116846024/tbase_post/templatetags/
+-rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:09.000000 django_tbase_post-2023.5.2116846024/tbase_post/templatetags/__init__.py
+-rw-r--r--   0 terry     (1000) terry     (1000)       94 2023-04-27 16:40:09.000000 django_tbase_post-2023.5.2116846024/tbase_post/templatetags/__init__.py:Zone.Identifier
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 17:06:56.420798 django_tbase_post-2023.5.2116846024/tbase_post/templatetags/__pycache__/
+-rw-r--r--   0 terry     (1000) terry     (1000)      170 2023-04-27 16:50:46.000000 django_tbase_post-2023.5.2116846024/tbase_post/templatetags/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     1888 2023-05-01 18:59:55.000000 django_tbase_post-2023.5.2116846024/tbase_post/templatetags/__pycache__/post_extras.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     3047 2023-05-01 18:59:54.000000 django_tbase_post-2023.5.2116846024/tbase_post/templatetags/post_extras.py
+-rw-r--r--   0 terry     (1000) terry     (1000)       94 2023-04-27 16:40:09.000000 django_tbase_post-2023.5.2116846024/tbase_post/templatetags/post_extras.py:Zone.Identifier
+-rw-r--r--   0 terry     (1000) terry     (1000)       60 2023-04-27 16:40:08.000000 django_tbase_post-2023.5.2116846024/tbase_post/tests.py
+-rw-r--r--   0 terry     (1000) terry     (1000)      451 2023-05-01 19:22:36.000000 django_tbase_post-2023.5.2116846024/tbase_post/urls.py
+-rw-r--r--   0 terry     (1000) terry     (1000)     3232 2023-05-01 19:22:30.000000 django_tbase_post-2023.5.2116846024/tbase_post/views.py
+-rw-r--r--   0 terry     (1000) terry     (1000)       94 2023-04-27 16:40:08.000000 django_tbase_post-2023.5.2116846024/tbase_post/views.py:Zone.Identifier
```

### Comparing `django_tbase_post-2023.5.2116845988/PKG-INFO` & `django_tbase_post-2023.5.2116846024/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: django_tbase_post
-Version: 2023.5.2116845988
-Summary: Terry django base post ,
-Home-page: https://terrychanorg.jetbrains.space/p/django-expand/repositories/tbase_post/files/README.md
-Author: Terry Chan
-Author-email: napoler2008@gmail.com
-Description-Content-Type: text/markdown
-
 # django-expand/tbase_post
 基本的文本模块
 
 安装
 ```bash
 pip install django-tbase-post
 ```
```

### Comparing `django_tbase_post-2023.5.2116845988/django_tbase_post.egg-info/PKG-INFO` & `django_tbase_post-2023.5.2116846024/django_tbase_post.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: django-tbase-post
-Version: 2023.5.2116845988
+Version: 2023.5.2116846024
 Summary: Terry django base post ,
 Home-page: https://terrychanorg.jetbrains.space/p/django-expand/repositories/tbase_post/files/README.md
 Author: Terry Chan
 Author-email: napoler2008@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # django-expand/tbase_post
 基本的文本模块
 
 安装
 ```bash
@@ -55,7 +57,9 @@
 ## Deployment
 
 Add additional notes about how to deploy this on a production system.
 
 ## Resources
 
 Add links to external resources for this project, such as CI server, bug tracker, etc.
+
+
```

### Comparing `django_tbase_post-2023.5.2116845988/setup.py` & `django_tbase_post-2023.5.2116846024/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         'django-taggit==3.0.0',
         'martor==1.6.19'
         # 'sentence-splitter>=1.4',
         # 'requests>=2.28.1',
         # 'nltk>=3.7'
     ],
     packages=['tbase_post'],  # 扫描的目录
-    nclude_package_data=True,  # 打包包含静态文件标识
+    include_package_data=True,  # 打包包含静态文件标识
 )
 
 """
 pip freeze > requirements.txt
 python3 setup.py sdist
 #python3 setup.py install
 python3 setup.py sdist upload
```

### Comparing `django_tbase_post-2023.5.2116845988/tbase_post/admin.py` & `django_tbase_post-2023.5.2116846024/tbase_post/admin.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post-2023.5.2116845988/tbase_post/models.py` & `django_tbase_post-2023.5.2116846024/tbase_post/models.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post-2023.5.2116845988/tbase_post/views.py` & `django_tbase_post-2023.5.2116846024/tbase_post/views.py`

 * *Files identical despite different names*

