# Comparing `tmp/django_tbase_theme_tailwind-2023.5.2016845966.tar.gz` & `tmp/django_tbase_theme_tailwind-2023.5.2116846002.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_tbase_theme_tailwind-2023.5.2016845966.tar", last modified: Sat May 20 15:30:03 2023, max compression
+gzip compressed data, was "django_tbase_theme_tailwind-2023.5.2116846002.tar", last modified: Sat May 20 16:30:05 2023, max compression
```

## Comparing `django_tbase_theme_tailwind-2023.5.2016845966.tar` & `django_tbase_theme_tailwind-2023.5.2116846002.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 15:30:03.821567 django_tbase_theme_tailwind-2023.5.2016845966/
--rw-r--r--   0 terry     (1000) terry     (1000)     1026 2023-05-20 15:30:03.821567 django_tbase_theme_tailwind-2023.5.2016845966/PKG-INFO
--rw-r--r--   0 terry     (1000) terry     (1000)      699 2023-05-20 15:27:39.000000 django_tbase_theme_tailwind-2023.5.2016845966/README.md
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 15:30:03.811567 django_tbase_theme_tailwind-2023.5.2016845966/django_tbase_theme_tailwind.egg-info/
--rw-r--r--   0 terry     (1000) terry     (1000)     1026 2023-05-20 15:30:03.000000 django_tbase_theme_tailwind-2023.5.2016845966/django_tbase_theme_tailwind.egg-info/PKG-INFO
--rw-r--r--   0 terry     (1000) terry     (1000)      405 2023-05-20 15:30:03.000000 django_tbase_theme_tailwind-2023.5.2016845966/django_tbase_theme_tailwind.egg-info/SOURCES.txt
--rw-r--r--   0 terry     (1000) terry     (1000)        1 2023-05-20 15:30:03.000000 django_tbase_theme_tailwind-2023.5.2016845966/django_tbase_theme_tailwind.egg-info/dependency_links.txt
--rw-r--r--   0 terry     (1000) terry     (1000)       21 2023-05-20 15:30:03.000000 django_tbase_theme_tailwind-2023.5.2016845966/django_tbase_theme_tailwind.egg-info/top_level.txt
--rw-r--r--   0 terry     (1000) terry     (1000)       38 2023-05-20 15:30:03.821567 django_tbase_theme_tailwind-2023.5.2016845966/setup.cfg
--rw-r--r--   0 terry     (1000) terry     (1000)     2230 2023-05-20 15:29:51.000000 django_tbase_theme_tailwind-2023.5.2016845966/setup.py
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 15:30:03.821567 django_tbase_theme_tailwind-2023.5.2016845966/tbase_theme_tailwind/
--rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:09.000000 django_tbase_theme_tailwind-2023.5.2016845966/tbase_theme_tailwind/__init__.py
--rw-r--r--   0 terry     (1000) terry     (1000)       63 2023-04-27 16:40:09.000000 django_tbase_theme_tailwind-2023.5.2016845966/tbase_theme_tailwind/admin.py
--rw-r--r--   0 terry     (1000) terry     (1000)      165 2023-04-27 16:40:09.000000 django_tbase_theme_tailwind-2023.5.2016845966/tbase_theme_tailwind/apps.py
--rw-r--r--   0 terry     (1000) terry     (1000)       57 2023-04-27 16:40:09.000000 django_tbase_theme_tailwind-2023.5.2016845966/tbase_theme_tailwind/models.py
--rw-r--r--   0 terry     (1000) terry     (1000)       60 2023-04-27 16:40:09.000000 django_tbase_theme_tailwind-2023.5.2016845966/tbase_theme_tailwind/tests.py
--rw-r--r--   0 terry     (1000) terry     (1000)       63 2023-04-27 16:40:09.000000 django_tbase_theme_tailwind-2023.5.2016845966/tbase_theme_tailwind/views.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 16:30:05.211087 django_tbase_theme_tailwind-2023.5.2116846002/
+-rw-r--r--   0 terry     (1000) terry     (1000)     1101 2023-05-20 16:30:05.211087 django_tbase_theme_tailwind-2023.5.2116846002/PKG-INFO
+-rw-r--r--   0 terry     (1000) terry     (1000)      774 2023-05-20 16:10:56.000000 django_tbase_theme_tailwind-2023.5.2116846002/README.md
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 16:30:05.211087 django_tbase_theme_tailwind-2023.5.2116846002/django_tbase_theme_tailwind.egg-info/
+-rw-r--r--   0 terry     (1000) terry     (1000)     1101 2023-05-20 16:30:05.000000 django_tbase_theme_tailwind-2023.5.2116846002/django_tbase_theme_tailwind.egg-info/PKG-INFO
+-rw-r--r--   0 terry     (1000) terry     (1000)      455 2023-05-20 16:30:05.000000 django_tbase_theme_tailwind-2023.5.2116846002/django_tbase_theme_tailwind.egg-info/SOURCES.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)        1 2023-05-20 16:30:05.000000 django_tbase_theme_tailwind-2023.5.2116846002/django_tbase_theme_tailwind.egg-info/dependency_links.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)       24 2023-05-20 16:30:05.000000 django_tbase_theme_tailwind-2023.5.2116846002/django_tbase_theme_tailwind.egg-info/requires.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)       21 2023-05-20 16:30:05.000000 django_tbase_theme_tailwind-2023.5.2116846002/django_tbase_theme_tailwind.egg-info/top_level.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)       38 2023-05-20 16:30:05.211087 django_tbase_theme_tailwind-2023.5.2116846002/setup.cfg
+-rw-r--r--   0 terry     (1000) terry     (1000)     2238 2023-05-20 16:28:52.000000 django_tbase_theme_tailwind-2023.5.2116846002/setup.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 16:30:05.211087 django_tbase_theme_tailwind-2023.5.2116846002/tbase_theme_tailwind/
+-rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:09.000000 django_tbase_theme_tailwind-2023.5.2116846002/tbase_theme_tailwind/__init__.py
+-rw-r--r--   0 terry     (1000) terry     (1000)       63 2023-04-27 16:40:09.000000 django_tbase_theme_tailwind-2023.5.2116846002/tbase_theme_tailwind/admin.py
+-rw-r--r--   0 terry     (1000) terry     (1000)      165 2023-04-27 16:40:09.000000 django_tbase_theme_tailwind-2023.5.2116846002/tbase_theme_tailwind/apps.py
+-rw-r--r--   0 terry     (1000) terry     (1000)       57 2023-04-27 16:40:09.000000 django_tbase_theme_tailwind-2023.5.2116846002/tbase_theme_tailwind/models.py
+-rw-r--r--   0 terry     (1000) terry     (1000)       60 2023-04-27 16:40:09.000000 django_tbase_theme_tailwind-2023.5.2116846002/tbase_theme_tailwind/tests.py
+-rw-r--r--   0 terry     (1000) terry     (1000)       63 2023-04-27 16:40:09.000000 django_tbase_theme_tailwind-2023.5.2116846002/tbase_theme_tailwind/views.py
```

### Comparing `django_tbase_theme_tailwind-2023.5.2016845966/PKG-INFO` & `django_tbase_theme_tailwind-2023.5.2116846002/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,28 @@
 Metadata-Version: 2.1
 Name: django_tbase_theme_tailwind
-Version: 2023.5.2016845966
+Version: 2023.5.2116846002
 Summary: Terry django base post ,
 Home-page: https://terrychanorg.jetbrains.space/p/django-expand/repositories/tbase_theme_tailwind/files/README.md
 Author: Terry Chan
 Author-email: napoler2008@gmail.com
 Description-Content-Type: text/markdown
 
 # django-expand/tbase_theme_tailwind
 
+集成tailwind
+
+集成
+
+在自己的模板文件中引用即可
+
+```
+
+
+```
 
 
 ## Getting Started
 
 Download links:
 
 SSH clone URL: ssh://git@git.jetbrains.space/terrychanorg/django-expand/tbase_theme_tailwind.git
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django_tbase_theme_tailwind-2023.5.2016845966/django_tbase_theme_tailwind.egg-info/PKG-INFO` & `django_tbase_theme_tailwind-2023.5.2116846002/django_tbase_theme_tailwind.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,28 @@
 Metadata-Version: 2.1
 Name: django-tbase-theme-tailwind
-Version: 2023.5.2016845966
+Version: 2023.5.2116846002
 Summary: Terry django base post ,
 Home-page: https://terrychanorg.jetbrains.space/p/django-expand/repositories/tbase_theme_tailwind/files/README.md
 Author: Terry Chan
 Author-email: napoler2008@gmail.com
 Description-Content-Type: text/markdown
 
 # django-expand/tbase_theme_tailwind
 
+集成tailwind
+
+集成
+
+在自己的模板文件中引用即可
+
+```
+
+
+```
 
 
 ## Getting Started
 
 Download links:
 
 SSH clone URL: ssh://git@git.jetbrains.space/terrychanorg/django-expand/tbase_theme_tailwind.git
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django_tbase_theme_tailwind-2023.5.2016845966/setup.py` & `django_tbase_theme_tailwind-2023.5.2116846002/setup.py`

 * *Files 11% similar despite different names*

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
+        'django-sitetree==1.17.2',
         # 'sentence-splitter>=1.4',
         # 'requests>=2.28.1',
         # 'nltk>=3.7'
     ],
     packages=['tbase_theme_tailwind'],  # 扫描的目录
     nclude_package_data=True,  # 打包包含静态文件标识
 )
```

