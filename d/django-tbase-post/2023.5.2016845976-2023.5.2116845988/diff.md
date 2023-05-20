# Comparing `tmp/django_tbase_post-2023.5.2016845976.tar.gz` & `tmp/django_tbase_post-2023.5.2116845988.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_tbase_post-2023.5.2016845976.tar", last modified: Sat May 20 15:48:14 2023, max compression
+gzip compressed data, was "django_tbase_post-2023.5.2116845988.tar", last modified: Sat May 20 16:08:03 2023, max compression
```

## Comparing `django_tbase_post-2023.5.2016845976.tar` & `django_tbase_post-2023.5.2116845988.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 15:48:14.331420 django_tbase_post-2023.5.2016845976/
--rw-r--r--   0 terry     (1000) terry     (1000)      976 2023-05-20 15:48:14.331420 django_tbase_post-2023.5.2016845976/PKG-INFO
--rw-r--r--   0 terry     (1000) terry     (1000)      669 2023-05-20 15:21:16.000000 django_tbase_post-2023.5.2016845976/README.md
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 15:48:14.331420 django_tbase_post-2023.5.2016845976/django_tbase_post.egg-info/
--rw-r--r--   0 terry     (1000) terry     (1000)      976 2023-05-20 15:48:14.000000 django_tbase_post-2023.5.2016845976/django_tbase_post.egg-info/PKG-INFO
--rw-r--r--   0 terry     (1000) terry     (1000)      364 2023-05-20 15:48:14.000000 django_tbase_post-2023.5.2016845976/django_tbase_post.egg-info/SOURCES.txt
--rw-r--r--   0 terry     (1000) terry     (1000)        1 2023-05-20 15:48:14.000000 django_tbase_post-2023.5.2016845976/django_tbase_post.egg-info/dependency_links.txt
--rw-r--r--   0 terry     (1000) terry     (1000)       83 2023-05-20 15:48:14.000000 django_tbase_post-2023.5.2016845976/django_tbase_post.egg-info/requires.txt
--rw-r--r--   0 terry     (1000) terry     (1000)       11 2023-05-20 15:48:14.000000 django_tbase_post-2023.5.2016845976/django_tbase_post.egg-info/top_level.txt
--rw-r--r--   0 terry     (1000) terry     (1000)       38 2023-05-20 15:48:14.331420 django_tbase_post-2023.5.2016845976/setup.cfg
--rw-r--r--   0 terry     (1000) terry     (1000)     2288 2023-05-20 15:47:45.000000 django_tbase_post-2023.5.2016845976/setup.py
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 15:48:14.331420 django_tbase_post-2023.5.2016845976/tbase_post/
--rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:08.000000 django_tbase_post-2023.5.2016845976/tbase_post/__init__.py
--rw-r--r--   0 terry     (1000) terry     (1000)      817 2023-04-27 16:40:08.000000 django_tbase_post-2023.5.2016845976/tbase_post/admin.py
--rw-r--r--   0 terry     (1000) terry     (1000)      146 2023-04-27 16:40:08.000000 django_tbase_post-2023.5.2016845976/tbase_post/apps.py
--rw-r--r--   0 terry     (1000) terry     (1000)     1424 2023-04-27 16:40:08.000000 django_tbase_post-2023.5.2016845976/tbase_post/models.py
--rw-r--r--   0 terry     (1000) terry     (1000)       60 2023-04-27 16:40:08.000000 django_tbase_post-2023.5.2016845976/tbase_post/tests.py
--rw-r--r--   0 terry     (1000) terry     (1000)      451 2023-05-01 19:22:36.000000 django_tbase_post-2023.5.2016845976/tbase_post/urls.py
--rw-r--r--   0 terry     (1000) terry     (1000)     3232 2023-05-01 19:22:30.000000 django_tbase_post-2023.5.2016845976/tbase_post/views.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 16:08:03.021269 django_tbase_post-2023.5.2116845988/
+-rw-r--r--   0 terry     (1000) terry     (1000)     1274 2023-05-20 16:08:03.021269 django_tbase_post-2023.5.2116845988/PKG-INFO
+-rw-r--r--   0 terry     (1000) terry     (1000)      967 2023-05-20 15:52:14.000000 django_tbase_post-2023.5.2116845988/README.md
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 16:08:03.021269 django_tbase_post-2023.5.2116845988/django_tbase_post.egg-info/
+-rw-r--r--   0 terry     (1000) terry     (1000)     1274 2023-05-20 16:08:02.000000 django_tbase_post-2023.5.2116845988/django_tbase_post.egg-info/PKG-INFO
+-rw-r--r--   0 terry     (1000) terry     (1000)      364 2023-05-20 16:08:02.000000 django_tbase_post-2023.5.2116845988/django_tbase_post.egg-info/SOURCES.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)        1 2023-05-20 16:08:02.000000 django_tbase_post-2023.5.2116845988/django_tbase_post.egg-info/dependency_links.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)       83 2023-05-20 16:08:02.000000 django_tbase_post-2023.5.2116845988/django_tbase_post.egg-info/requires.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)       11 2023-05-20 16:08:02.000000 django_tbase_post-2023.5.2116845988/django_tbase_post.egg-info/top_level.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)       38 2023-05-20 16:08:03.021269 django_tbase_post-2023.5.2116845988/setup.cfg
+-rw-r--r--   0 terry     (1000) terry     (1000)     2288 2023-05-20 15:53:05.000000 django_tbase_post-2023.5.2116845988/setup.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 16:08:03.021269 django_tbase_post-2023.5.2116845988/tbase_post/
+-rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:08.000000 django_tbase_post-2023.5.2116845988/tbase_post/__init__.py
+-rw-r--r--   0 terry     (1000) terry     (1000)      817 2023-04-27 16:40:08.000000 django_tbase_post-2023.5.2116845988/tbase_post/admin.py
+-rw-r--r--   0 terry     (1000) terry     (1000)      146 2023-04-27 16:40:08.000000 django_tbase_post-2023.5.2116845988/tbase_post/apps.py
+-rw-r--r--   0 terry     (1000) terry     (1000)     1424 2023-04-27 16:40:08.000000 django_tbase_post-2023.5.2116845988/tbase_post/models.py
+-rw-r--r--   0 terry     (1000) terry     (1000)       60 2023-04-27 16:40:08.000000 django_tbase_post-2023.5.2116845988/tbase_post/tests.py
+-rw-r--r--   0 terry     (1000) terry     (1000)      451 2023-05-01 19:22:36.000000 django_tbase_post-2023.5.2116845988/tbase_post/urls.py
+-rw-r--r--   0 terry     (1000) terry     (1000)     3232 2023-05-01 19:22:30.000000 django_tbase_post-2023.5.2116845988/tbase_post/views.py
```

### Comparing `django_tbase_post-2023.5.2016845976/PKG-INFO` & `django_tbase_post-2023.5.2116845988/django_tbase_post.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,39 @@
 Metadata-Version: 2.1
-Name: django_tbase_post
-Version: 2023.5.2016845976
+Name: django-tbase-post
+Version: 2023.5.2116845988
 Summary: Terry django base post ,
 Home-page: https://terrychanorg.jetbrains.space/p/django-expand/repositories/tbase_post/files/README.md
 Author: Terry Chan
 Author-email: napoler2008@gmail.com
 Description-Content-Type: text/markdown
 
 # django-expand/tbase_post
+基本的文本模块
 
+安装
+```bash
+pip install django-tbase-post
+```
+
+```python
+# settings.py
+ INSTALLED_APPS = [   # 个人应用
+     # 基本配置
+    # 'tbase_page',
+    'tbase_config',
+    'tbase_theme_tailwind',
+    
+    'tbase_post',
+    # 'markdownx'
+    'martor',
+    'taggit',
+
+ ]
+```
 
 
 ## Getting Started
 
 Download links:
 
 SSH clone URL: ssh://git@git.jetbrains.space/terrychanorg/django-expand/tbase_post.git
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django_tbase_post-2023.5.2016845976/django_tbase_post.egg-info/PKG-INFO` & `django_tbase_post-2023.5.2116845988/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,39 @@
 Metadata-Version: 2.1
-Name: django-tbase-post
-Version: 2023.5.2016845976
+Name: django_tbase_post
+Version: 2023.5.2116845988
 Summary: Terry django base post ,
 Home-page: https://terrychanorg.jetbrains.space/p/django-expand/repositories/tbase_post/files/README.md
 Author: Terry Chan
 Author-email: napoler2008@gmail.com
 Description-Content-Type: text/markdown
 
 # django-expand/tbase_post
+基本的文本模块
 
+安装
+```bash
+pip install django-tbase-post
+```
+
+```python
+# settings.py
+ INSTALLED_APPS = [   # 个人应用
+     # 基本配置
+    # 'tbase_page',
+    'tbase_config',
+    'tbase_theme_tailwind',
+    
+    'tbase_post',
+    # 'markdownx'
+    'martor',
+    'taggit',
+
+ ]
+```
 
 
 ## Getting Started
 
 Download links:
 
 SSH clone URL: ssh://git@git.jetbrains.space/terrychanorg/django-expand/tbase_post.git
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django_tbase_post-2023.5.2016845976/setup.py` & `django_tbase_post-2023.5.2116845988/setup.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post-2023.5.2016845976/tbase_post/admin.py` & `django_tbase_post-2023.5.2116845988/tbase_post/admin.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post-2023.5.2016845976/tbase_post/models.py` & `django_tbase_post-2023.5.2116845988/tbase_post/models.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post-2023.5.2016845976/tbase_post/views.py` & `django_tbase_post-2023.5.2116845988/tbase_post/views.py`

 * *Files identical despite different names*

