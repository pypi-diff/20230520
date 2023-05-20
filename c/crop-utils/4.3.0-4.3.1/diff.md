# Comparing `tmp/crop_utils-4.3.0.tar.gz` & `tmp/crop_utils-4.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crop_utils-4.3.0.tar", last modified: Fri Mar  3 09:28:24 2023, max compression
+gzip compressed data, was "crop_utils-4.3.1.tar", last modified: Sat May 20 07:33:59 2023, max compression
```

## Comparing `crop_utils-4.3.0.tar` & `crop_utils-4.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-03-03 09:28:24.307480 crop_utils-4.3.0/
--rw-rw-rw-   0        0        0     1091 2021-10-21 02:22:48.000000 crop_utils-4.3.0/LICENSE
--rw-rw-rw-   0        0        0       52 2021-10-21 06:40:49.000000 crop_utils-4.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2005 2023-03-03 09:28:24.307480 crop_utils-4.3.0/PKG-INFO
--rw-rw-rw-   0        0        0      911 2022-10-17 02:43:26.000000 crop_utils-4.3.0/README.md
--rw-rw-rw-   0        0        0      108 2021-10-20 10:50:24.000000 crop_utils-4.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-03 09:28:24.307480 crop_utils-4.3.0/setup.cfg
--rw-rw-rw-   0        0        0      901 2023-03-03 09:28:21.000000 crop_utils-4.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-03 09:28:24.281150 crop_utils-4.3.0/src/
-drwxrwxrwx   0        0        0        0 2023-03-03 09:28:24.298147 crop_utils-4.3.0/src/crop_utils/
--rw-rw-rw-   0        0        0        4 2021-10-21 03:45:02.000000 crop_utils-4.3.0/src/crop_utils/__init__.py
--rw-rw-rw-   0        0        0     2140 2022-04-29 03:15:39.000000 crop_utils-4.3.0/src/crop_utils/html_slot_config.py
--rw-rw-rw-   0        0        0    56899 2022-10-09 03:26:55.000000 crop_utils-4.3.0/src/crop_utils/image.py
--rw-rw-rw-   0        0        0    41792 2023-03-03 09:20:54.000000 crop_utils-4.3.0/src/crop_utils/img_crop.py
--rw-rw-rw-   0        0        0    41524 2021-11-19 07:30:47.000000 crop_utils-4.3.0/src/crop_utils/olg_crop.py
-drwxrwxrwx   0        0        0        0 2023-03-03 09:28:24.305474 crop_utils-4.3.0/src/crop_utils.egg-info/
--rw-rw-rw-   0        0        0     2005 2023-03-03 09:28:24.000000 crop_utils-4.3.0/src/crop_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      345 2023-03-03 09:28:24.000000 crop_utils-4.3.0/src/crop_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-03 09:28:24.000000 crop_utils-4.3.0/src/crop_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-03-03 09:28:24.000000 crop_utils-4.3.0/src/crop_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-20 07:33:59.907796 crop_utils-4.3.1/
+-rw-rw-rw-   0        0        0     1091 2021-10-21 02:22:48.000000 crop_utils-4.3.1/LICENSE
+-rw-rw-rw-   0        0        0       52 2021-10-21 06:40:49.000000 crop_utils-4.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1998 2023-05-20 07:33:59.907796 crop_utils-4.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0      910 2023-03-03 09:28:43.000000 crop_utils-4.3.1/README.md
+-rw-rw-rw-   0        0        0      108 2021-10-20 10:50:24.000000 crop_utils-4.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-20 07:33:59.907796 crop_utils-4.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      895 2023-05-20 07:33:48.000000 crop_utils-4.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 07:33:59.884804 crop_utils-4.3.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-20 07:33:59.899805 crop_utils-4.3.1/src/crop_utils/
+-rw-rw-rw-   0        0        0        4 2021-10-21 03:45:02.000000 crop_utils-4.3.1/src/crop_utils/__init__.py
+-rw-rw-rw-   0        0        0     2140 2022-04-29 03:15:39.000000 crop_utils-4.3.1/src/crop_utils/html_slot_config.py
+-rw-rw-rw-   0        0        0    56899 2022-10-09 03:26:55.000000 crop_utils-4.3.1/src/crop_utils/image.py
+-rw-rw-rw-   0        0        0    42170 2023-05-20 07:33:32.000000 crop_utils-4.3.1/src/crop_utils/img_crop.py
+-rw-rw-rw-   0        0        0    41524 2021-11-19 07:30:47.000000 crop_utils-4.3.1/src/crop_utils/olg_crop.py
+drwxrwxrwx   0        0        0        0 2023-05-20 07:33:59.905796 crop_utils-4.3.1/src/crop_utils.egg-info/
+-rw-rw-rw-   0        0        0     1998 2023-05-20 07:33:59.000000 crop_utils-4.3.1/src/crop_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      345 2023-05-20 07:33:59.000000 crop_utils-4.3.1/src/crop_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 07:33:59.000000 crop_utils-4.3.1/src/crop_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-20 07:33:59.000000 crop_utils-4.3.1/src/crop_utils.egg-info/top_level.txt
```

### Comparing `crop_utils-4.3.0/LICENSE` & `crop_utils-4.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `crop_utils-4.3.0/PKG-INFO` & `crop_utils-4.3.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: crop_utils
-Version: 4.3.0
-Summary: 资源图上下扩边
+Version: 4.3.1
+Summary: 详情页扩边
 Home-page: http://git.chaomy.com/libo/ecpro-utils.git
 Author: libo
 Author-email: 6878595@qq.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Description: 为了区分3.0与4.0版本，同时资源图与详情页也共用的一套裁剪逻辑代码。
         
@@ -74,14 +74,14 @@
         
         
         
         # 安装
         
         
         
-        pip install crop-utils==0.0.30 -i  https://pypi.python.org/simple/
+        pip install crop-utils==4.3.0 -i  https://pypi.python.org/simple/
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `crop_utils-4.3.0/README.md` & `crop_utils-4.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -65,8 +65,8 @@
 
 
 
 # 安装
 
 
 
-pip install crop-utils==0.0.30 -i  https://pypi.python.org/simple/
+pip install crop-utils==4.3.0 -i  https://pypi.python.org/simple/
```

### Comparing `crop_utils-4.3.0/setup.py` & `crop_utils-4.3.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="crop_utils",  # 包名称
-    version="4.3.0",  # 版本号
+    version="4.3.1",  # 版本号
     author="libo",
     author_email="6878595@qq.com",
-    description="资源图上下扩边",
+    description="详情页扩边",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="http://git.chaomy.com/libo/ecpro-utils.git",
     project_urls={
         "Bug Tracker": "https://github.com/pypa/sampleproject/issues",
     },
     classifiers=[
```

### Comparing `crop_utils-4.3.0/src/crop_utils/html_slot_config.py` & `crop_utils-4.3.1/src/crop_utils/html_slot_config.py`

 * *Files identical despite different names*

### Comparing `crop_utils-4.3.0/src/crop_utils/image.py` & `crop_utils-4.3.1/src/crop_utils/image.py`

 * *Files identical despite different names*

### Comparing `crop_utils-4.3.0/src/crop_utils/img_crop.py` & `crop_utils-4.3.1/src/crop_utils/img_crop.py`

 * *Files 1% similar despite different names*

```diff
@@ -590,14 +590,19 @@
         """裁剪所需信息不全，居中裁剪"""
         if crop_method == 'w':  # 宽固定，高自适应
             get_crop_point_result_dict = {'x1': 0, 'x2': 1}
             crop_x, crop_y, crop_width, crop_height, scale_x, scale_y, amend_layout_height = self. \
                 self_adaption_height_crop(0, 1, get_crop_point_result_dict, [slot_width, slot_height], img)
             amend_layout_height = 0  # 历史遗留问题，留着就行
             return crop_x, crop_y, crop_width, crop_height, scale_x, scale_y, amend_layout_height, img.width, img.height
+        elif crop_method == 'e':  # 扩边裁剪
+            crop_x, crop_y, crop_width, crop_height, scale_x, scale_y, amend_layout_height = self.__extension_crop(
+                0, 1, {'x1': 0, 'x2': 1}, [slot_width, slot_height], img
+            )
+            return crop_x, crop_y, crop_width, crop_height, scale_x, scale_y, amend_layout_height, img.width, img.height
         else:
             return self.center_crop(slot_width, slot_height, img.width, img.height)
 
     def __extension_crop(self, top, bottom, crop_point_result_dict, origin_slot, img):
         # 一定要考虑图片放缩 后 相关点的变化
 
         origin_slot_width, origin_slot_height = origin_slot
```

### Comparing `crop_utils-4.3.0/src/crop_utils/olg_crop.py` & `crop_utils-4.3.1/src/crop_utils/olg_crop.py`

 * *Files identical despite different names*

### Comparing `crop_utils-4.3.0/src/crop_utils.egg-info/PKG-INFO` & `crop_utils-4.3.1/src/crop_utils.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: crop-utils
-Version: 4.3.0
-Summary: 资源图上下扩边
+Version: 4.3.1
+Summary: 详情页扩边
 Home-page: http://git.chaomy.com/libo/ecpro-utils.git
 Author: libo
 Author-email: 6878595@qq.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Description: 为了区分3.0与4.0版本，同时资源图与详情页也共用的一套裁剪逻辑代码。
         
@@ -74,14 +74,14 @@
         
         
         
         # 安装
         
         
         
-        pip install crop-utils==0.0.30 -i  https://pypi.python.org/simple/
+        pip install crop-utils==4.3.0 -i  https://pypi.python.org/simple/
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

