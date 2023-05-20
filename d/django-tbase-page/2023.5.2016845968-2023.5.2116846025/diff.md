# Comparing `tmp/django_tbase_page-2023.5.2016845968.tar.gz` & `tmp/django_tbase_page-2023.5.2116846025.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_tbase_page-2023.5.2016845968.tar", last modified: Sat May 20 15:34:27 2023, max compression
+gzip compressed data, was "django_tbase_page-2023.5.2116846025.tar", last modified: Sat May 20 17:08:26 2023, max compression
```

## Comparing `django_tbase_page-2023.5.2016845968.tar` & `django_tbase_page-2023.5.2116846025.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 15:34:27.071534 django_tbase_page-2023.5.2016845968/
--rw-r--r--   0 terry     (1000) terry     (1000)      976 2023-05-20 15:34:27.071534 django_tbase_page-2023.5.2016845968/PKG-INFO
--rw-r--r--   0 terry     (1000) terry     (1000)      669 2023-05-20 15:31:46.000000 django_tbase_page-2023.5.2016845968/README.md
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 15:34:27.071534 django_tbase_page-2023.5.2016845968/django_tbase_page.egg-info/
--rw-r--r--   0 terry     (1000) terry     (1000)      976 2023-05-20 15:34:27.000000 django_tbase_page-2023.5.2016845968/django_tbase_page.egg-info/PKG-INFO
--rw-r--r--   0 terry     (1000) terry     (1000)      364 2023-05-20 15:34:27.000000 django_tbase_page-2023.5.2016845968/django_tbase_page.egg-info/SOURCES.txt
--rw-r--r--   0 terry     (1000) terry     (1000)        1 2023-05-20 15:34:27.000000 django_tbase_page-2023.5.2016845968/django_tbase_page.egg-info/dependency_links.txt
--rw-r--r--   0 terry     (1000) terry     (1000)       47 2023-05-20 15:34:27.000000 django_tbase_page-2023.5.2016845968/django_tbase_page.egg-info/requires.txt
--rw-r--r--   0 terry     (1000) terry     (1000)       11 2023-05-20 15:34:27.000000 django_tbase_page-2023.5.2016845968/django_tbase_page.egg-info/top_level.txt
--rw-r--r--   0 terry     (1000) terry     (1000)       38 2023-05-20 15:34:27.071534 django_tbase_page-2023.5.2016845968/setup.cfg
--rw-r--r--   0 terry     (1000) terry     (1000)     2231 2023-05-20 15:33:51.000000 django_tbase_page-2023.5.2016845968/setup.py
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 15:34:27.071534 django_tbase_page-2023.5.2016845968/tbase_page/
--rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:08.000000 django_tbase_page-2023.5.2016845968/tbase_page/__init__.py
--rw-r--r--   0 terry     (1000) terry     (1000)     2050 2023-05-12 18:40:39.000000 django_tbase_page-2023.5.2016845968/tbase_page/admin.py
--rw-r--r--   0 terry     (1000) terry     (1000)      146 2023-04-27 16:40:08.000000 django_tbase_page-2023.5.2016845968/tbase_page/apps.py
--rw-r--r--   0 terry     (1000) terry     (1000)      645 2023-05-12 18:26:57.000000 django_tbase_page-2023.5.2016845968/tbase_page/models.py
--rw-r--r--   0 terry     (1000) terry     (1000)       60 2023-04-27 16:40:08.000000 django_tbase_page-2023.5.2016845968/tbase_page/tests.py
--rw-r--r--   0 terry     (1000) terry     (1000)      855 2023-04-27 16:40:08.000000 django_tbase_page-2023.5.2016845968/tbase_page/urls.py
--rw-r--r--   0 terry     (1000) terry     (1000)      921 2023-05-12 18:42:44.000000 django_tbase_page-2023.5.2016845968/tbase_page/views.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 17:08:26.870787 django_tbase_page-2023.5.2116846025/
+-rw-r--r--   0 terry     (1000) terry     (1000)      143 2023-05-20 17:05:28.000000 django_tbase_page-2023.5.2116846025/MANIFEST.in
+-rw-r--r--   0 terry     (1000) terry     (1000)     1305 2023-05-20 17:08:26.870787 django_tbase_page-2023.5.2116846025/PKG-INFO
+-rw-r--r--   0 terry     (1000) terry     (1000)      961 2023-05-20 16:21:34.000000 django_tbase_page-2023.5.2116846025/README.md
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 17:08:26.870787 django_tbase_page-2023.5.2116846025/django_tbase_page.egg-info/
+-rw-r--r--   0 terry     (1000) terry     (1000)     1305 2023-05-20 17:08:26.000000 django_tbase_page-2023.5.2116846025/django_tbase_page.egg-info/PKG-INFO
+-rw-r--r--   0 terry     (1000) terry     (1000)      376 2023-05-20 17:08:26.000000 django_tbase_page-2023.5.2116846025/django_tbase_page.egg-info/SOURCES.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)        1 2023-05-20 17:08:26.000000 django_tbase_page-2023.5.2116846025/django_tbase_page.egg-info/dependency_links.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)       62 2023-05-20 17:08:26.000000 django_tbase_page-2023.5.2116846025/django_tbase_page.egg-info/requires.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)       11 2023-05-20 17:08:26.000000 django_tbase_page-2023.5.2116846025/django_tbase_page.egg-info/top_level.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)       38 2023-05-20 17:08:26.870787 django_tbase_page-2023.5.2116846025/setup.cfg
+-rw-r--r--   0 terry     (1000) terry     (1000)     2258 2023-05-20 17:08:12.000000 django_tbase_page-2023.5.2116846025/setup.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 17:08:26.870787 django_tbase_page-2023.5.2116846025/tbase_page/
+-rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:08.000000 django_tbase_page-2023.5.2116846025/tbase_page/__init__.py
+-rw-r--r--   0 terry     (1000) terry     (1000)     2050 2023-05-12 18:40:39.000000 django_tbase_page-2023.5.2116846025/tbase_page/admin.py
+-rw-r--r--   0 terry     (1000) terry     (1000)      146 2023-04-27 16:40:08.000000 django_tbase_page-2023.5.2116846025/tbase_page/apps.py
+-rw-r--r--   0 terry     (1000) terry     (1000)      645 2023-05-12 18:26:57.000000 django_tbase_page-2023.5.2116846025/tbase_page/models.py
+-rw-r--r--   0 terry     (1000) terry     (1000)       60 2023-04-27 16:40:08.000000 django_tbase_page-2023.5.2116846025/tbase_page/tests.py
+-rw-r--r--   0 terry     (1000) terry     (1000)      855 2023-04-27 16:40:08.000000 django_tbase_page-2023.5.2116846025/tbase_page/urls.py
+-rw-r--r--   0 terry     (1000) terry     (1000)      921 2023-05-12 18:42:44.000000 django_tbase_page-2023.5.2116846025/tbase_page/views.py
```

### Comparing `django_tbase_page-2023.5.2016845968/PKG-INFO` & `django_tbase_page-2023.5.2116846025/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,46 @@
 Metadata-Version: 2.1
 Name: django_tbase_page
-Version: 2023.5.2016845968
+Version: 2023.5.2116846025
 Summary: Terry django base post ,
 Home-page: https://terrychanorg.jetbrains.space/p/django-expand/repositories/tbase_page/files/README.md
 Author: Terry Chan
 Author-email: napoler2008@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # django-expand/tbase_page
+基本页面
 
 
 
+
+安装
+```bash
+pip install django-tbase-page
+```
+
+```python
+# settings.py
+ INSTALLED_APPS = [   # 个人应用
+     # 基本配置
+    'tbase_page',
+    'tbase_config',
+    'tbase_theme_tailwind',
+    
+    #'tbase_post',
+    # 'markdownx'
+    'martor',
+    #'taggit',
+
+ ]
+```
+
+
 ## Getting Started
 
 Download links:
 
 SSH clone URL: ssh://git@git.jetbrains.space/terrychanorg/django-expand/tbase_page.git
 
 HTTPS clone URL: https://git.jetbrains.space/terrychanorg/django-expand/tbase_page.git
@@ -34,7 +60,9 @@
 ## Deployment
 
 Add additional notes about how to deploy this on a production system.
 
 ## Resources
 
 Add links to external resources for this project, such as CI server, bug tracker, etc.
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django_tbase_page-2023.5.2016845968/django_tbase_page.egg-info/PKG-INFO` & `django_tbase_page-2023.5.2116846025/django_tbase_page.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,46 @@
 Metadata-Version: 2.1
 Name: django-tbase-page
-Version: 2023.5.2016845968
+Version: 2023.5.2116846025
 Summary: Terry django base post ,
 Home-page: https://terrychanorg.jetbrains.space/p/django-expand/repositories/tbase_page/files/README.md
 Author: Terry Chan
 Author-email: napoler2008@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # django-expand/tbase_page
+基本页面
 
 
 
+
+安装
+```bash
+pip install django-tbase-page
+```
+
+```python
+# settings.py
+ INSTALLED_APPS = [   # 个人应用
+     # 基本配置
+    'tbase_page',
+    'tbase_config',
+    'tbase_theme_tailwind',
+    
+    #'tbase_post',
+    # 'markdownx'
+    'martor',
+    #'taggit',
+
+ ]
+```
+
+
 ## Getting Started
 
 Download links:
 
 SSH clone URL: ssh://git@git.jetbrains.space/terrychanorg/django-expand/tbase_page.git
 
 HTTPS clone URL: https://git.jetbrains.space/terrychanorg/django-expand/tbase_page.git
@@ -34,7 +60,9 @@
 ## Deployment
 
 Add additional notes about how to deploy this on a production system.
 
 ## Resources
 
 Add links to external resources for this project, such as CI server, bug tracker, etc.
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django_tbase_page-2023.5.2016845968/setup.py` & `django_tbase_page-2023.5.2116846025/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,20 +60,21 @@
     url=url,
     # install_requires=read_requirements('requirements.txt'),  # 指定需要安装的依赖
     long_description=long_description,
     long_description_content_type="text/markdown",
     # 依赖文件
     install_requires=[
         'django-tbase-theme-tailwind>=2023.5.2016845966',
+        'martor==1.6.19',
         # 'sentence-splitter>=1.4',
         # 'requests>=2.28.1',
         # 'nltk>=3.7'
     ],
     packages=['tbase_page'],  # 扫描的目录
-    nclude_package_data=True,  # 打包包含静态文件标识
+    include_package_data=True,  # 打包包含静态文件标识
 )
 
 """
 pip freeze > requirements.txt
 python3 setup.py sdist
 #python3 setup.py install
 python3 setup.py sdist upload
```

### Comparing `django_tbase_page-2023.5.2016845968/tbase_page/admin.py` & `django_tbase_page-2023.5.2116846025/tbase_page/admin.py`

 * *Files identical despite different names*

### Comparing `django_tbase_page-2023.5.2016845968/tbase_page/models.py` & `django_tbase_page-2023.5.2116846025/tbase_page/models.py`

 * *Files identical despite different names*

### Comparing `django_tbase_page-2023.5.2016845968/tbase_page/urls.py` & `django_tbase_page-2023.5.2116846025/tbase_page/urls.py`

 * *Files identical despite different names*

### Comparing `django_tbase_page-2023.5.2016845968/tbase_page/views.py` & `django_tbase_page-2023.5.2116846025/tbase_page/views.py`

 * *Files identical despite different names*

