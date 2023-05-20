# Comparing `tmp/django_tbase_post-2023.5.2016845958.tar.gz` & `tmp/django_tbase_post-2023.5.2016845963.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_tbase_post-2023.5.2016845958.tar", last modified: Sat May 20 15:18:18 2023, max compression
+gzip compressed data, was "django_tbase_post-2023.5.2016845963.tar", last modified: Sat May 20 15:25:51 2023, max compression
```

## Comparing `django_tbase_post-2023.5.2016845958.tar` & `django_tbase_post-2023.5.2016845963.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 15:18:18.351652 django_tbase_post-2023.5.2016845958/
--rw-r--r--   0 terry     (1000) terry     (1000)     1038 2023-05-20 15:18:18.351652 django_tbase_post-2023.5.2016845958/PKG-INFO
--rw-r--r--   0 terry     (1000) terry     (1000)      723 2023-05-20 14:30:47.000000 django_tbase_post-2023.5.2016845958/README.md
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 15:18:18.351652 django_tbase_post-2023.5.2016845958/django_tbase_post.egg-info/
--rw-r--r--   0 terry     (1000) terry     (1000)     1038 2023-05-20 15:18:18.000000 django_tbase_post-2023.5.2016845958/django_tbase_post.egg-info/PKG-INFO
--rw-r--r--   0 terry     (1000) terry     (1000)      347 2023-05-20 15:18:18.000000 django_tbase_post-2023.5.2016845958/django_tbase_post.egg-info/SOURCES.txt
--rw-r--r--   0 terry     (1000) terry     (1000)        1 2023-05-20 15:18:18.000000 django_tbase_post-2023.5.2016845958/django_tbase_post.egg-info/dependency_links.txt
--rw-r--r--   0 terry     (1000) terry     (1000)       11 2023-05-20 15:18:18.000000 django_tbase_post-2023.5.2016845958/django_tbase_post.egg-info/top_level.txt
--rw-r--r--   0 terry     (1000) terry     (1000)       38 2023-05-20 15:18:18.351652 django_tbase_post-2023.5.2016845958/setup.cfg
--rw-r--r--   0 terry     (1000) terry     (1000)     2208 2023-05-20 14:43:46.000000 django_tbase_post-2023.5.2016845958/setup.py
-drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 15:18:18.351652 django_tbase_post-2023.5.2016845958/tbase_post/
--rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:08.000000 django_tbase_post-2023.5.2016845958/tbase_post/__init__.py
--rw-r--r--   0 terry     (1000) terry     (1000)     1727 2023-05-15 18:15:03.000000 django_tbase_post-2023.5.2016845958/tbase_post/admin.py
--rw-r--r--   0 terry     (1000) terry     (1000)      146 2023-04-27 16:40:08.000000 django_tbase_post-2023.5.2016845958/tbase_post/apps.py
--rw-r--r--   0 terry     (1000) terry     (1000)     3388 2023-05-05 15:46:17.000000 django_tbase_post-2023.5.2016845958/tbase_post/models.py
--rw-r--r--   0 terry     (1000) terry     (1000)      479 2023-05-12 18:21:31.000000 django_tbase_post-2023.5.2016845958/tbase_post/sitemaps.py
--rw-r--r--   0 terry     (1000) terry     (1000)       60 2023-04-27 16:40:08.000000 django_tbase_post-2023.5.2016845958/tbase_post/tests.py
--rw-r--r--   0 terry     (1000) terry     (1000)      725 2023-05-05 16:36:02.000000 django_tbase_post-2023.5.2016845958/tbase_post/urls.py
--rw-r--r--   0 terry     (1000) terry     (1000)     3256 2023-05-05 16:15:07.000000 django_tbase_post-2023.5.2016845958/tbase_post/views.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 15:25:51.891600 django_tbase_post-2023.5.2016845963/
+-rw-r--r--   0 terry     (1000) terry     (1000)      976 2023-05-20 15:25:51.891600 django_tbase_post-2023.5.2016845963/PKG-INFO
+-rw-r--r--   0 terry     (1000) terry     (1000)      669 2023-05-20 15:21:16.000000 django_tbase_post-2023.5.2016845963/README.md
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 15:25:51.891600 django_tbase_post-2023.5.2016845963/django_tbase_post.egg-info/
+-rw-r--r--   0 terry     (1000) terry     (1000)      976 2023-05-20 15:25:51.000000 django_tbase_post-2023.5.2016845963/django_tbase_post.egg-info/PKG-INFO
+-rw-r--r--   0 terry     (1000) terry     (1000)      324 2023-05-20 15:25:51.000000 django_tbase_post-2023.5.2016845963/django_tbase_post.egg-info/SOURCES.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)        1 2023-05-20 15:25:51.000000 django_tbase_post-2023.5.2016845963/django_tbase_post.egg-info/dependency_links.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)       11 2023-05-20 15:25:51.000000 django_tbase_post-2023.5.2016845963/django_tbase_post.egg-info/top_level.txt
+-rw-r--r--   0 terry     (1000) terry     (1000)       38 2023-05-20 15:25:51.891600 django_tbase_post-2023.5.2016845963/setup.cfg
+-rw-r--r--   0 terry     (1000) terry     (1000)     2200 2023-05-20 15:24:31.000000 django_tbase_post-2023.5.2016845963/setup.py
+drwxr-xr-x   0 terry     (1000) terry     (1000)        0 2023-05-20 15:25:51.891600 django_tbase_post-2023.5.2016845963/tbase_post/
+-rw-r--r--   0 terry     (1000) terry     (1000)        0 2023-04-27 16:40:08.000000 django_tbase_post-2023.5.2016845963/tbase_post/__init__.py
+-rw-r--r--   0 terry     (1000) terry     (1000)      817 2023-04-27 16:40:08.000000 django_tbase_post-2023.5.2016845963/tbase_post/admin.py
+-rw-r--r--   0 terry     (1000) terry     (1000)      146 2023-04-27 16:40:08.000000 django_tbase_post-2023.5.2016845963/tbase_post/apps.py
+-rw-r--r--   0 terry     (1000) terry     (1000)     1424 2023-04-27 16:40:08.000000 django_tbase_post-2023.5.2016845963/tbase_post/models.py
+-rw-r--r--   0 terry     (1000) terry     (1000)       60 2023-04-27 16:40:08.000000 django_tbase_post-2023.5.2016845963/tbase_post/tests.py
+-rw-r--r--   0 terry     (1000) terry     (1000)      451 2023-05-01 19:22:36.000000 django_tbase_post-2023.5.2016845963/tbase_post/urls.py
+-rw-r--r--   0 terry     (1000) terry     (1000)     3232 2023-05-01 19:22:30.000000 django_tbase_post-2023.5.2016845963/tbase_post/views.py
```

### Comparing `django_tbase_post-2023.5.2016845958/PKG-INFO` & `django_tbase_post-2023.5.2016845963/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 Metadata-Version: 2.1
 Name: django_tbase_post
-Version: 2023.5.2016845958
+Version: 2023.5.2016845963
 Summary: Terry django base post ,
-Home-page: https://terrychanorg.jetbrains.space/p/django-expand/repositories/tbase_post_product/files/README.md
+Home-page: https://terrychanorg.jetbrains.space/p/django-expand/repositories/tbase_post/files/README.md
 Author: Terry Chan
 Author-email: napoler2008@gmail.com
 Description-Content-Type: text/markdown
 
-# django-expand/tbase_post_product
-
-用于产品的文章模块
-
+# django-expand/tbase_post
 
 
 
 ## Getting Started
 
 Download links:
 
-SSH clone URL: ssh://git@git.jetbrains.space/terrychanorg/django-expand/tbase_post_product.git
+SSH clone URL: ssh://git@git.jetbrains.space/terrychanorg/django-expand/tbase_post.git
 
-HTTPS clone URL: https://git.jetbrains.space/terrychanorg/django-expand/tbase_post_product.git
+HTTPS clone URL: https://git.jetbrains.space/terrychanorg/django-expand/tbase_post.git
 
 
 
 These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.
 
 ## Prerequisites
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `django_tbase_post-2023.5.2016845958/README.md` & `django_tbase_post-2023.5.2016845963/django_tbase_post.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,27 @@
-# django-expand/tbase_post_product
-
-用于产品的文章模块
+Metadata-Version: 2.1
+Name: django-tbase-post
+Version: 2023.5.2016845963
+Summary: Terry django base post ,
+Home-page: https://terrychanorg.jetbrains.space/p/django-expand/repositories/tbase_post/files/README.md
+Author: Terry Chan
+Author-email: napoler2008@gmail.com
+Description-Content-Type: text/markdown
 
+# django-expand/tbase_post
 
 
 
 ## Getting Started
 
 Download links:
 
-SSH clone URL: ssh://git@git.jetbrains.space/terrychanorg/django-expand/tbase_post_product.git
+SSH clone URL: ssh://git@git.jetbrains.space/terrychanorg/django-expand/tbase_post.git
 
-HTTPS clone URL: https://git.jetbrains.space/terrychanorg/django-expand/tbase_post_product.git
+HTTPS clone URL: https://git.jetbrains.space/terrychanorg/django-expand/tbase_post.git
 
 
 
 These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.
 
 ## Prerequisites
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `django_tbase_post-2023.5.2016845958/setup.py` & `django_tbase_post-2023.5.2016845963/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # 这里是基本的信息
 
 name = 'django_tbase_post'  # 修改包名字-
 version = f'{year}.{month}.{day}' + str(time.time())[:8]
 description = 'Terry django base post ,'
 author = 'Terry Chan'
 author_email = 'napoler2008@gmail.com'
-url = 'https://terrychanorg.jetbrains.space/p/django-expand/repositories/tbase_post_product/files/README.md'
+url = 'https://terrychanorg.jetbrains.space/p/django-expand/repositories/tbase_post/files/README.md'
 
 copyright = '2021, Terry Chan'
 language = 'zh_cn'
 
 this_directory = os_path.abspath(os_path.dirname(__file__))
 """帮助[https://www.notion.so/6bade2c6a5f4479f82a4e67eafcebb3a]
 上传到anaconda
```

### Comparing `django_tbase_post-2023.5.2016845958/tbase_post/views.py` & `django_tbase_post-2023.5.2016845963/tbase_post/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     template_name = 'post/detail.html'
     # context_object_name = 'post'
     # def get(request, pk):
     #     """Return the last five published questions."""
     #     return Post.objects.get(id=pk)
     model = models.Post
     context_object_name = 'detail'
-    ordering = ['-created_on']
+    ordering = ['-pk']
     # # 控制访问权限
     # @method_decorator(login_required)
     # @method_decorator(permission_required('dashboard.view_server'))
     # def get(self, request, *args, **kwargs):
     #     print("kwargs", kwargs)
     #     # context = self.model.objects.get(id=pk)
     #     context = super().get_context_data(**kwargs)
@@ -55,15 +55,15 @@
 
     # def get(self, request, *args, **kwargs):
     #     return HttpResponse('Hello, World! index')
 
     template_name = 'post/blog_index.html'
     model = models.Post
     paginate_by = 10
-    ordering = ['-created_on']
+    ordering = ['-pk']
 
 
     # context_object_name = 'model_list'
     # def get(self, request, *args, **kwargs):
     #     return HttpResponse('Hello, World! index')
     #     # return {}
     def get_context_data(self, *args, **kwargs):
@@ -77,15 +77,15 @@
 
 
 class TagListView(generic.ListView):
     model = models.Post
     template_name = 'post/article_list_by_tag.html'
     context_object_name = 'posts'
     paginate_by = 10
-    ordering = ['-created_on']
+    ordering = ['-pk']
     def get_queryset(self):
         # retrieve the tag from the URL
         tag_slug = self.kwargs['pk']
         # get the tag object based on the slug
         tag = Tag.objects.get(pk=tag_slug)
         # filter articles based on the tag
         articles = self.model.objects.filter(tags=tag)
```

