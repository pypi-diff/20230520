# Comparing `tmp/django_tbase_post_product-2023.5.2016845970.tar.gz` & `tmp/django_tbase_post_product-2023.5.2016845980.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_tbase_post_product-2023.5.2016845970.tar", last modified: Sat May 20 15:36:52 2023, max compression
+gzip compressed data, was "django_tbase_post_product-2023.5.2016845980.tar", last modified: Sat May 20 15:54:43 2023, max compression
```

## Comparing `django_tbase_post_product-2023.5.2016845970.tar` & `django_tbase_post_product-2023.5.2016845980.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 15:36:52.271512 django_tbase_post_product-2023.5.2016845970/
--rw-r--r--   0 terry     (1000) terry     (1000)     1046 2023-05-20 15:36:52.261512 django_tbase_post_product-2023.5.2016845970/PKG-INFO
--rw-r--r--   0 terry     (1000) terry     (1000)      723 2023-05-20 14:30:47.000000 django_tbase_post_product-2023.5.2016845970/README.md
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 15:36:52.261512 django_tbase_post_product-2023.5.2016845970/django_tbase_post_product.egg-info/
--rw-r--r--   0 terry     (1000) terry     (1000)     1046 2023-05-20 15:36:52.000000 django_tbase_post_product-2023.5.2016845970/django_tbase_post_product.egg-info/PKG-INFO
--rw-r--r--   0 terry     (1000) terry     (1000)      427 2023-05-20 15:36:52.000000 django_tbase_post_product-2023.5.2016845970/django_tbase_post_product.egg-info/SOURCES.txt
--rw-r--r--   0 terry     (1000) terry     (1000)        1 2023-05-20 15:36:52.000000 django_tbase_post_product-2023.5.2016845970/django_tbase_post_product.egg-info/dependency_links.txt
--rw-r--r--   0 terry     (1000) terry     (1000)       47 2023-05-20 15:36:52.000000 django_tbase_post_product-2023.5.2016845970/django_tbase_post_product.egg-info/requires.txt
--rw-r--r--   0 terry     (1000) terry     (1000)       11 2023-05-20 15:36:52.000000 django_tbase_post_product-2023.5.2016845970/django_tbase_post_product.egg-info/top_level.txt
--rw-r--r--   0 terry     (1000) terry     (1000)       38 2023-05-20 15:36:52.271512 django_tbase_post_product-2023.5.2016845970/setup.cfg
--rw-r--r--   0 terry     (1000) terry     (1000)     2247 2023-05-20 15:36:05.000000 django_tbase_post_product-2023.5.2016845970/setup.py
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 15:36:52.261512 django_tbase_post_product-2023.5.2016845970/tbase_post/
--rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:08.000000 django_tbase_post_product-2023.5.2016845970/tbase_post/__init__.py
--rw-r--r--   0 terry     (1000) terry     (1000)     1727 2023-05-15 18:15:03.000000 django_tbase_post_product-2023.5.2016845970/tbase_post/admin.py
--rw-r--r--   0 terry     (1000) terry     (1000)      146 2023-04-27 16:40:08.000000 django_tbase_post_product-2023.5.2016845970/tbase_post/apps.py
--rw-r--r--   0 terry     (1000) terry     (1000)     3388 2023-05-05 15:46:17.000000 django_tbase_post_product-2023.5.2016845970/tbase_post/models.py
--rw-r--r--   0 terry     (1000) terry     (1000)      479 2023-05-12 18:21:31.000000 django_tbase_post_product-2023.5.2016845970/tbase_post/sitemaps.py
--rw-r--r--   0 terry     (1000) terry     (1000)       60 2023-04-27 16:40:08.000000 django_tbase_post_product-2023.5.2016845970/tbase_post/tests.py
--rw-r--r--   0 terry     (1000) terry     (1000)      725 2023-05-05 16:36:02.000000 django_tbase_post_product-2023.5.2016845970/tbase_post/urls.py
--rw-r--r--   0 terry     (1000) terry     (1000)     3256 2023-05-05 16:15:07.000000 django_tbase_post_product-2023.5.2016845970/tbase_post/views.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 15:54:43.851366 django_tbase_post_product-2023.5.2016845980/
+-rw-r--r--   0 terry     (1000) terry     (1000)     1333 2023-05-20 15:54:43.851366 django_tbase_post_product-2023.5.2016845980/PKG-INFO
+-rw-r--r--   0 terry     (1000) terry     (1000)     1010 2023-05-20 15:52:49.000000 django_tbase_post_product-2023.5.2016845980/README.md
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 15:54:43.851366 django_tbase_post_product-2023.5.2016845980/django_tbase_post_product.egg-info/
+-rw-r--r--   0 terry     (1000) terry     (1000)     1333 2023-05-20 15:54:43.000000 django_tbase_post_product-2023.5.2016845980/django_tbase_post_product.egg-info/PKG-INFO
+-rw-r--r--   0 terry     (1000) terry     (1000)      427 2023-05-20 15:54:43.000000 django_tbase_post_product-2023.5.2016845980/django_tbase_post_product.egg-info/SOURCES.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)        1 2023-05-20 15:54:43.000000 django_tbase_post_product-2023.5.2016845980/django_tbase_post_product.egg-info/dependency_links.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)       83 2023-05-20 15:54:43.000000 django_tbase_post_product-2023.5.2016845980/django_tbase_post_product.egg-info/requires.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)       11 2023-05-20 15:54:43.000000 django_tbase_post_product-2023.5.2016845980/django_tbase_post_product.egg-info/top_level.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)       38 2023-05-20 15:54:43.851366 django_tbase_post_product-2023.5.2016845980/setup.cfg
+-rw-r--r--   0 terry     (1000) terry     (1000)     2304 2023-05-20 15:53:13.000000 django_tbase_post_product-2023.5.2016845980/setup.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 15:54:43.851366 django_tbase_post_product-2023.5.2016845980/tbase_post/
+-rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:08.000000 django_tbase_post_product-2023.5.2016845980/tbase_post/__init__.py
+-rw-r--r--   0 terry     (1000) terry     (1000)     1727 2023-05-15 18:15:03.000000 django_tbase_post_product-2023.5.2016845980/tbase_post/admin.py
+-rw-r--r--   0 terry     (1000) terry     (1000)      146 2023-04-27 16:40:08.000000 django_tbase_post_product-2023.5.2016845980/tbase_post/apps.py
+-rw-r--r--   0 terry     (1000) terry     (1000)     3388 2023-05-05 15:46:17.000000 django_tbase_post_product-2023.5.2016845980/tbase_post/models.py
+-rw-r--r--   0 terry     (1000) terry     (1000)      479 2023-05-12 18:21:31.000000 django_tbase_post_product-2023.5.2016845980/tbase_post/sitemaps.py
+-rw-r--r--   0 terry     (1000) terry     (1000)       60 2023-04-27 16:40:08.000000 django_tbase_post_product-2023.5.2016845980/tbase_post/tests.py
+-rw-r--r--   0 terry     (1000) terry     (1000)      725 2023-05-05 16:36:02.000000 django_tbase_post_product-2023.5.2016845980/tbase_post/urls.py
+-rw-r--r--   0 terry     (1000) terry     (1000)     3256 2023-05-05 16:15:07.000000 django_tbase_post_product-2023.5.2016845980/tbase_post/views.py
```

### Comparing `django_tbase_post_product-2023.5.2016845970/PKG-INFO` & `django_tbase_post_product-2023.5.2016845980/django_tbase_post_product.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,45 @@
 Metadata-Version: 2.1
-Name: django_tbase_post_product
-Version: 2023.5.2016845970
+Name: django-tbase-post-product
+Version: 2023.5.2016845980
 Summary: Terry django base post ,
 Home-page: https://terrychanorg.jetbrains.space/p/django-expand/repositories/tbase_post_product/files/README.md
 Author: Terry Chan
 Author-email: napoler2008@gmail.com
 Description-Content-Type: text/markdown
 
 # django-expand/tbase_post_product
 
 用于产品的文章模块
 
 
 
+安装
+```bash
+pip install django-tbase-post-product
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
+
+
+
 
 ## Getting Started
 
 Download links:
 
 SSH clone URL: ssh://git@git.jetbrains.space/terrychanorg/django-expand/tbase_post_product.git
```

### Comparing `django_tbase_post_product-2023.5.2016845970/README.md` & `django_tbase_post_product-2023.5.2016845980/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,36 @@
 # django-expand/tbase_post_product
 
 用于产品的文章模块
 
 
 
+安装
+```bash
+pip install django-tbase-post-product
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
+
+
+
 
 ## Getting Started
 
 Download links:
 
 SSH clone URL: ssh://git@git.jetbrains.space/terrychanorg/django-expand/tbase_post_product.git
```

### Comparing `django_tbase_post_product-2023.5.2016845970/django_tbase_post_product.egg-info/PKG-INFO` & `django_tbase_post_product-2023.5.2016845980/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,45 @@
 Metadata-Version: 2.1
-Name: django-tbase-post-product
-Version: 2023.5.2016845970
+Name: django_tbase_post_product
+Version: 2023.5.2016845980
 Summary: Terry django base post ,
 Home-page: https://terrychanorg.jetbrains.space/p/django-expand/repositories/tbase_post_product/files/README.md
 Author: Terry Chan
 Author-email: napoler2008@gmail.com
 Description-Content-Type: text/markdown
 
 # django-expand/tbase_post_product
 
 用于产品的文章模块
 
 
 
+安装
+```bash
+pip install django-tbase-post-product
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
+
+
+
 
 ## Getting Started
 
 Download links:
 
 SSH clone URL: ssh://git@git.jetbrains.space/terrychanorg/django-expand/tbase_post_product.git
```

### Comparing `django_tbase_post_product-2023.5.2016845970/setup.py` & `django_tbase_post_product-2023.5.2016845980/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -60,14 +60,16 @@
     url=url,
     # install_requires=read_requirements('requirements.txt'),  # 指定需要安装的依赖
     long_description=long_description,
     long_description_content_type="text/markdown",
     # 依赖文件
     install_requires=[
         'django-tbase-theme-tailwind>=2023.5.2016845966',
+        'django-taggit==3.0.0',
+        'martor==1.6.19'
         # 'sentence-splitter>=1.4',
         # 'requests>=2.28.1',
         # 'nltk>=3.7'
     ],
     packages=['tbase_post'],  # 扫描的目录
     nclude_package_data=True,  # 打包包含静态文件标识
 )
```

### Comparing `django_tbase_post_product-2023.5.2016845970/tbase_post/admin.py` & `django_tbase_post_product-2023.5.2016845980/tbase_post/admin.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.5.2016845970/tbase_post/models.py` & `django_tbase_post_product-2023.5.2016845980/tbase_post/models.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.5.2016845970/tbase_post/urls.py` & `django_tbase_post_product-2023.5.2016845980/tbase_post/urls.py`

 * *Files identical despite different names*

### Comparing `django_tbase_post_product-2023.5.2016845970/tbase_post/views.py` & `django_tbase_post_product-2023.5.2016845980/tbase_post/views.py`

 * *Files identical despite different names*

