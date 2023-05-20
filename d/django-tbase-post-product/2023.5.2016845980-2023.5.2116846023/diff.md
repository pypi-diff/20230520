# Comparing `tmp/django_tbase_post_product-2023.5.2016845980.tar.gz` & `tmp/django_tbase_post_product-2023.5.2116846023.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_tbase_post_product-2023.5.2016845980.tar", last modified: Sat May 20 15:54:43 2023, max compression
+gzip compressed data, was "django_tbase_post_product-2023.5.2116846023.tar", last modified: Sat May 20 17:06:02 2023, max compression
```

## Comparing `django_tbase_post_product-2023.5.2016845980.tar` & `django_tbase_post_product-2023.5.2116846023.tar`

### file list

```diff
@@ -1,20 +1,59 @@
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 15:54:43.851366 django_tbase_post_product-2023.5.2016845980/
--rw-r--r--   0 terry     (1000) terry     (1000)     1333 2023-05-20 15:54:43.851366 django_tbase_post_product-2023.5.2016845980/PKG-INFO
--rw-r--r--   0 terry     (1000) terry     (1000)     1010 2023-05-20 15:52:49.000000 django_tbase_post_product-2023.5.2016845980/README.md
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 15:54:43.851366 django_tbase_post_product-2023.5.2016845980/django_tbase_post_product.egg-info/
--rw-r--r--   0 terry     (1000) terry     (1000)     1333 2023-05-20 15:54:43.000000 django_tbase_post_product-2023.5.2016845980/django_tbase_post_product.egg-info/PKG-INFO
--rw-r--r--   0 terry     (1000) terry     (1000)      427 2023-05-20 15:54:43.000000 django_tbase_post_product-2023.5.2016845980/django_tbase_post_product.egg-info/SOURCES.txt
--rw-r--r--   0 terry     (1000) terry     (1000)        1 2023-05-20 15:54:43.000000 django_tbase_post_product-2023.5.2016845980/django_tbase_post_product.egg-info/dependency_links.txt
--rw-r--r--   0 terry     (1000) terry     (1000)       83 2023-05-20 15:54:43.000000 django_tbase_post_product-2023.5.2016845980/django_tbase_post_product.egg-info/requires.txt
--rw-r--r--   0 terry     (1000) terry     (1000)       11 2023-05-20 15:54:43.000000 django_tbase_post_product-2023.5.2016845980/django_tbase_post_product.egg-info/top_level.txt
--rw-r--r--   0 terry     (1000) terry     (1000)       38 2023-05-20 15:54:43.851366 django_tbase_post_product-2023.5.2016845980/setup.cfg
--rw-r--r--   0 terry     (1000) terry     (1000)     2304 2023-05-20 15:53:13.000000 django_tbase_post_product-2023.5.2016845980/setup.py
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 15:54:43.851366 django_tbase_post_product-2023.5.2016845980/tbase_post/
--rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:08.000000 django_tbase_post_product-2023.5.2016845980/tbase_post/__init__.py
--rw-r--r--   0 terry     (1000) terry     (1000)     1727 2023-05-15 18:15:03.000000 django_tbase_post_product-2023.5.2016845980/tbase_post/admin.py
--rw-r--r--   0 terry     (1000) terry     (1000)      146 2023-04-27 16:40:08.000000 django_tbase_post_product-2023.5.2016845980/tbase_post/apps.py
--rw-r--r--   0 terry     (1000) terry     (1000)     3388 2023-05-05 15:46:17.000000 django_tbase_post_product-2023.5.2016845980/tbase_post/models.py
--rw-r--r--   0 terry     (1000) terry     (1000)      479 2023-05-12 18:21:31.000000 django_tbase_post_product-2023.5.2016845980/tbase_post/sitemaps.py
--rw-r--r--   0 terry     (1000) terry     (1000)       60 2023-04-27 16:40:08.000000 django_tbase_post_product-2023.5.2016845980/tbase_post/tests.py
--rw-r--r--   0 terry     (1000) terry     (1000)      725 2023-05-05 16:36:02.000000 django_tbase_post_product-2023.5.2016845980/tbase_post/urls.py
--rw-r--r--   0 terry     (1000) terry     (1000)     3256 2023-05-05 16:15:07.000000 django_tbase_post_product-2023.5.2016845980/tbase_post/views.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 17:06:02.590803 django_tbase_post_product-2023.5.2116846023/
+-rw-r--r--   0 terry     (1000) terry     (1000)      143 2023-05-20 17:05:28.000000 django_tbase_post_product-2023.5.2116846023/MANIFEST.in
+-rw-r--r--   0 terry     (1000) terry     (1000)     1370 2023-05-20 17:06:02.590803 django_tbase_post_product-2023.5.2116846023/PKG-INFO
+-rw-r--r--   0 terry     (1000) terry     (1000)     1010 2023-05-20 15:52:49.000000 django_tbase_post_product-2023.5.2116846023/README.md
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 17:06:02.590803 django_tbase_post_product-2023.5.2116846023/django_tbase_post_product.egg-info/
+-rw-r--r--   0 terry     (1000) terry     (1000)     1370 2023-05-20 17:06:02.000000 django_tbase_post_product-2023.5.2116846023/django_tbase_post_product.egg-info/PKG-INFO
+-rw-r--r--   0 terry     (1000) terry     (1000)     2109 2023-05-20 17:06:02.000000 django_tbase_post_product-2023.5.2116846023/django_tbase_post_product.egg-info/SOURCES.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)        1 2023-05-20 17:06:02.000000 django_tbase_post_product-2023.5.2116846023/django_tbase_post_product.egg-info/dependency_links.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)       83 2023-05-20 17:06:02.000000 django_tbase_post_product-2023.5.2116846023/django_tbase_post_product.egg-info/requires.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)       11 2023-05-20 17:06:02.000000 django_tbase_post_product-2023.5.2116846023/django_tbase_post_product.egg-info/top_level.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)       38 2023-05-20 17:06:02.590803 django_tbase_post_product-2023.5.2116846023/setup.cfg
+-rw-r--r--   0 terry     (1000) terry     (1000)     2305 2023-05-20 16:52:58.000000 django_tbase_post_product-2023.5.2116846023/setup.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 17:06:02.590803 django_tbase_post_product-2023.5.2116846023/tbase_post/
+-rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:08.000000 django_tbase_post_product-2023.5.2116846023/tbase_post/__init__.py
+-rw-r--r--   0 terry     (1000) terry     (1000)     1727 2023-05-15 18:15:03.000000 django_tbase_post_product-2023.5.2116846023/tbase_post/admin.py
+-rw-r--r--   0 terry     (1000) terry     (1000)      146 2023-04-27 16:40:08.000000 django_tbase_post_product-2023.5.2116846023/tbase_post/apps.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 17:06:02.590803 django_tbase_post_product-2023.5.2116846023/tbase_post/migrations/
+-rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.5.2116846023/tbase_post/migrations/__init__.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 17:06:02.590803 django_tbase_post_product-2023.5.2116846023/tbase_post/migrations/__pycache__/
+-rw-r--r--   0 terry     (1000) terry     (1000)     1062 2023-04-27 16:50:46.000000 django_tbase_post_product-2023.5.2116846023/tbase_post/migrations/__pycache__/0001_initial.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     1092 2023-04-27 16:50:46.000000 django_tbase_post_product-2023.5.2116846023/tbase_post/migrations/__pycache__/0002_auto_20230421_1307.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     1081 2023-05-05 14:25:13.000000 django_tbase_post_product-2023.5.2116846023/tbase_post/migrations/__pycache__/0003_auto_20230505_1424.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     1498 2023-05-05 15:03:52.000000 django_tbase_post_product-2023.5.2116846023/tbase_post/migrations/__pycache__/0004_auto_20230505_1503.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)      591 2023-05-05 15:05:58.000000 django_tbase_post_product-2023.5.2116846023/tbase_post/migrations/__pycache__/0005_rename_banner_img_post_article_img.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     1059 2023-05-05 15:46:35.000000 django_tbase_post_product-2023.5.2116846023/tbase_post/migrations/__pycache__/0006_auto_20230505_1546.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)      168 2023-04-27 16:50:46.000000 django_tbase_post_product-2023.5.2116846023/tbase_post/migrations/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     3388 2023-05-05 15:46:17.000000 django_tbase_post_product-2023.5.2116846023/tbase_post/models.py
+-rw-r--r--   0 terry     (1000) terry     (1000)      479 2023-05-12 18:21:31.000000 django_tbase_post_product-2023.5.2116846023/tbase_post/sitemaps.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 17:06:02.590803 django_tbase_post_product-2023.5.2116846023/tbase_post/static/
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 17:06:02.590803 django_tbase_post_product-2023.5.2116846023/tbase_post/static/images/
+-rw-r--r--   0 terry     (1000) terry     (1000)    59619 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.5.2116846023/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg
+-rw-r--r--   0 terry     (1000) terry     (1000)       94 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.5.2116846023/tbase_post/static/images/photo-1578707399887-e6d183c9e598.jpeg:Zone.Identifier
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 17:06:02.590803 django_tbase_post_product-2023.5.2116846023/tbase_post/templates/
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 17:06:02.590803 django_tbase_post_product-2023.5.2116846023/tbase_post/templates/post/
+-rw-r--r--   0 terry     (1000) terry     (1000)     2723 2023-05-09 11:19:05.000000 django_tbase_post_product-2023.5.2116846023/tbase_post/templates/post/article_list_by_tag.html
+-rw-r--r--   0 terry     (1000) terry     (1000)       94 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.5.2116846023/tbase_post/templates/post/article_list_by_tag.html:Zone.Identifier
+-rw-r--r--   0 terry     (1000) terry     (1000)     2120 2023-05-09 11:29:39.000000 django_tbase_post_product-2023.5.2116846023/tbase_post/templates/post/blog_index.html
+-rw-r--r--   0 terry     (1000) terry     (1000)       94 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.5.2116846023/tbase_post/templates/post/blog_index.html:Zone.Identifier
+-rw-r--r--   0 terry     (1000) terry     (1000)     4110 2023-05-09 11:42:20.000000 django_tbase_post_product-2023.5.2116846023/tbase_post/templates/post/detail.html
+-rw-r--r--   0 terry     (1000) terry     (1000)       94 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.5.2116846023/tbase_post/templates/post/detail.html:Zone.Identifier
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 17:06:02.590803 django_tbase_post_product-2023.5.2116846023/tbase_post/templates/post/extras/
+-rw-r--r--   0 terry     (1000) terry     (1000)      443 2023-05-09 11:22:22.000000 django_tbase_post_product-2023.5.2116846023/tbase_post/templates/post/extras/amazon_link.html
+-rw-r--r--   0 terry     (1000) terry     (1000)      376 2023-05-08 23:37:48.000000 django_tbase_post_product-2023.5.2116846023/tbase_post/templates/post/extras/last_update.html
+-rw-r--r--   0 terry     (1000) terry     (1000)      294 2023-05-08 23:37:59.000000 django_tbase_post_product-2023.5.2116846023/tbase_post/templates/post/extras/related_post_by_tags.html
+-rw-r--r--   0 terry     (1000) terry     (1000)       94 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.5.2116846023/tbase_post/templates/post/extras/related_post_by_tags.html:Zone.Identifier
+-rw-r--r--   0 terry     (1000) terry     (1000)      415 2023-05-01 19:23:09.000000 django_tbase_post_product-2023.5.2116846023/tbase_post/templates/post/extras/tags.html
+-rw-r--r--   0 terry     (1000) terry     (1000)       94 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.5.2116846023/tbase_post/templates/post/extras/tags.html:Zone.Identifier
+-rw-r--r--   0 terry     (1000) terry     (1000)      391 2023-05-05 16:55:19.000000 django_tbase_post_product-2023.5.2116846023/tbase_post/templates/sitemap.xml
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 17:06:02.590803 django_tbase_post_product-2023.5.2116846023/tbase_post/templatetags/
+-rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.5.2116846023/tbase_post/templatetags/__init__.py
+-rw-r--r--   0 terry     (1000) terry     (1000)       94 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.5.2116846023/tbase_post/templatetags/__init__.py:Zone.Identifier
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 17:06:02.590803 django_tbase_post_product-2023.5.2116846023/tbase_post/templatetags/__pycache__/
+-rw-r--r--   0 terry     (1000) terry     (1000)      170 2023-04-27 16:50:46.000000 django_tbase_post_product-2023.5.2116846023/tbase_post/templatetags/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     3002 2023-05-11 17:20:31.000000 django_tbase_post_product-2023.5.2116846023/tbase_post/templatetags/__pycache__/post_extras.cpython-310.pyc
+-rw-r--r--   0 terry     (1000) terry     (1000)     5044 2023-05-09 11:42:47.000000 django_tbase_post_product-2023.5.2116846023/tbase_post/templatetags/post_extras.py
+-rw-r--r--   0 terry     (1000) terry     (1000)       94 2023-04-27 16:40:09.000000 django_tbase_post_product-2023.5.2116846023/tbase_post/templatetags/post_extras.py:Zone.Identifier
+-rw-r--r--   0 terry     (1000) terry     (1000)       60 2023-04-27 16:40:08.000000 django_tbase_post_product-2023.5.2116846023/tbase_post/tests.py
+-rw-r--r--   0 terry     (1000) terry     (1000)      725 2023-05-05 16:36:02.000000 django_tbase_post_product-2023.5.2116846023/tbase_post/urls.py
+-rw-r--r--   0 terry     (1000) terry     (1000)     3256 2023-05-05 16:15:07.000000 django_tbase_post_product-2023.5.2116846023/tbase_post/views.py
```

### Comparing `django_tbase_post_product-2023.5.2016845980/PKG-INFO` & `django_tbase_post_product-2023.5.2116846023/django_tbase_post_product.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
-Name: django_tbase_post_product
-Version: 2023.5.2016845980
+Name: django-tbase-post-product
+Version: 2023.5.2116846023
 Summary: Terry django base post ,
 Home-page: https://terrychanorg.jetbrains.space/p/django-expand/repositories/tbase_post_product/files/README.md
 Author: Terry Chan
 Author-email: napoler2008@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # django-expand/tbase_post_product
 
 用于产品的文章模块
 
 
@@ -60,7 +62,9 @@
 ## Deployment
 
 Add additional notes about how to deploy this on a production system.
 
 ## Resources
 
 Add links to external resources for this project, such as CI server, bug tracker, etc.
+
+
```

### Comparing `django_tbase_post_product-2023.5.2016845980/README.md` & `django_tbase_post_product-2023.5.2116846023/README.md`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.5.2016845980/django_tbase_post_product.egg-info/PKG-INFO` & `django_tbase_post_product-2023.5.2116846023/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
-Name: django-tbase-post-product
-Version: 2023.5.2016845980
+Name: django_tbase_post_product
+Version: 2023.5.2116846023
 Summary: Terry django base post ,
 Home-page: https://terrychanorg.jetbrains.space/p/django-expand/repositories/tbase_post_product/files/README.md
 Author: Terry Chan
 Author-email: napoler2008@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # django-expand/tbase_post_product
 
 用于产品的文章模块
 
 
@@ -60,7 +62,9 @@
 ## Deployment
 
 Add additional notes about how to deploy this on a production system.
 
 ## Resources
 
 Add links to external resources for this project, such as CI server, bug tracker, etc.
+
+
```

### Comparing `django_tbase_post_product-2023.5.2016845980/setup.py` & `django_tbase_post_product-2023.5.2116846023/setup.py`

 * *Files 0% similar despite different names*

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

### Comparing `django_tbase_post_product-2023.5.2016845980/tbase_post/admin.py` & `django_tbase_post_product-2023.5.2116846023/tbase_post/admin.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.5.2016845980/tbase_post/models.py` & `django_tbase_post_product-2023.5.2116846023/tbase_post/models.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.5.2016845980/tbase_post/urls.py` & `django_tbase_post_product-2023.5.2116846023/tbase_post/urls.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.5.2016845980/tbase_post/views.py` & `django_tbase_post_product-2023.5.2116846023/tbase_post/views.py`

 * *Files identical despite different names*

