# Comparing `tmp/slim-id-0.0.1.tar.gz` & `tmp/slim-id-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slim-id-0.0.1.tar", last modified: Sat May 20 03:00:33 2023, max compression
+gzip compressed data, was "slim-id-0.0.2.tar", last modified: Sat May 20 03:03:20 2023, max compression
```

## Comparing `slim-id-0.0.1.tar` & `slim-id-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 03:00:33.796921 slim-id-0.0.1/
--rw-rw-rw-   0        0        0     4018 2023-05-20 03:00:33.795920 slim-id-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2997 2023-04-29 06:47:34.000000 slim-id-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-20 03:00:33.796921 slim-id-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      777 2023-05-20 03:00:16.000000 slim-id-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-20 03:00:33.790681 slim-id-0.0.1/slim_id/
--rw-rw-rw-   0        0        0      992 2023-05-20 02:53:20.000000 slim-id-0.0.1/slim_id/__init__.py
--rw-rw-rw-   0        0        0      709 2023-05-20 02:52:46.000000 slim-id-0.0.1/slim_id/test.py
-drwxrwxrwx   0        0        0        0 2023-05-20 03:00:33.794920 slim-id-0.0.1/slim_id.egg-info/
--rw-rw-rw-   0        0        0     4018 2023-05-20 03:00:33.000000 slim-id-0.0.1/slim_id.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      208 2023-05-20 03:00:33.000000 slim-id-0.0.1/slim_id.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 03:00:33.000000 slim-id-0.0.1/slim_id.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-05-20 03:00:33.000000 slim-id-0.0.1/slim_id.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-20 03:00:33.000000 slim-id-0.0.1/slim_id.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-20 03:03:20.531986 slim-id-0.0.2/
+-rw-rw-rw-   0        0        0     4000 2023-05-20 03:03:20.531986 slim-id-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2979 2023-05-20 03:02:01.000000 slim-id-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-20 03:03:20.531986 slim-id-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      777 2023-05-20 03:02:40.000000 slim-id-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:03:20.525833 slim-id-0.0.2/slim_id/
+-rw-rw-rw-   0        0        0      992 2023-05-20 02:53:20.000000 slim-id-0.0.2/slim_id/__init__.py
+-rw-rw-rw-   0        0        0      709 2023-05-20 02:52:46.000000 slim-id-0.0.2/slim_id/test.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:03:20.530986 slim-id-0.0.2/slim_id.egg-info/
+-rw-rw-rw-   0        0        0     4000 2023-05-20 03:03:20.000000 slim-id-0.0.2/slim_id.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      208 2023-05-20 03:03:20.000000 slim-id-0.0.2/slim_id.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 03:03:20.000000 slim-id-0.0.2/slim_id.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-05-20 03:03:20.000000 slim-id-0.0.2/slim_id.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-20 03:03:20.000000 slim-id-0.0.2/slim_id.egg-info/top_level.txt
```

### Comparing `slim-id-0.0.1/PKG-INFO` & `slim-id-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slim-id
-Version: 0.0.1
+Version: 0.0.2
 Summary: This is a tool that automatically generates short IDs
 Home-page: https://github.co.jp/
 Author: bib_inf
 Author-email: contact.bibinf@gmail.com
 License: CC0 v1.0
 Description: # Slim-ID: A Lightweight ID Generation Library for Python
         
@@ -24,25 +24,25 @@
         ## Usage Example
         ```python
         import sys
         import slim_id
         
         id_dic = {}
         
-        def is_exists(arg_id):
+        def exists(arg_id):
             return (arg_id in id_dic)
         
         # Generate an ID using Slim-ID
-        s_id = slim_id.gen(is_exists)
+        s_id = slim_id.gen(exists)
         id_dic[s_id] = True
         print(s_id)
         
         # Generate an ID using Slim-ID with custom parameters
         s_id = slim_id.gen(
-            is_exists,  # Function to determine if an ID exists in the database
+            exists,  # Function to determine if an ID exists in the database
             length = 7,  # Base length (automatically increases if a collision occurs)
             ab = "16",  # Alphabet type (base64url... URL-safe Base64, 16... hexadecimal)
         )
         id_dic[s_id] = True
         print(s_id)
         ```
         
@@ -59,25 +59,25 @@
         
         ```python
         import sys
         import slim_id
         
         id_dic = {}
         
-        def is_exists(arg_id):
+        def exists(arg_id):
             return (arg_id in id_dic)
         
         # Slim-IDを使用してIDを生成
-        s_id = slim_id.gen(is_exists)
+        s_id = slim_id.gen(exists)
         id_dic[s_id] = True
         print(s_id)
         
         # カスタムパラメータを使用してSlim-IDでIDを生成
         s_id = slim_id.gen(
-            is_exists,  # IDがデータベースに存在するかどうかを判断する関数
+            exists,  # IDがデータベースに存在するかどうかを判断する関数
             length = 7,  # 基本長（衝突が発生した場合、自動的に長くなります）
             ab = "16",  # アルファベットの種類（base64url... URLセーフな64進数、16... 16進数）
         )
         id_dic[s_id] = True
         print(s_id)
         ```
```

### Comparing `slim-id-0.0.1/README.md` & `slim-id-0.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -16,25 +16,25 @@
 ## Usage Example
 ```python
 import sys
 import slim_id
 
 id_dic = {}
 
-def is_exists(arg_id):
+def exists(arg_id):
     return (arg_id in id_dic)
 
 # Generate an ID using Slim-ID
-s_id = slim_id.gen(is_exists)
+s_id = slim_id.gen(exists)
 id_dic[s_id] = True
 print(s_id)
 
 # Generate an ID using Slim-ID with custom parameters
 s_id = slim_id.gen(
-    is_exists,  # Function to determine if an ID exists in the database
+    exists,  # Function to determine if an ID exists in the database
     length = 7,  # Base length (automatically increases if a collision occurs)
     ab = "16",  # Alphabet type (base64url... URL-safe Base64, 16... hexadecimal)
 )
 id_dic[s_id] = True
 print(s_id)
 ```
 
@@ -51,24 +51,24 @@
 
 ```python
 import sys
 import slim_id
 
 id_dic = {}
 
-def is_exists(arg_id):
+def exists(arg_id):
     return (arg_id in id_dic)
 
 # Slim-IDを使用してIDを生成
-s_id = slim_id.gen(is_exists)
+s_id = slim_id.gen(exists)
 id_dic[s_id] = True
 print(s_id)
 
 # カスタムパラメータを使用してSlim-IDでIDを生成
 s_id = slim_id.gen(
-    is_exists,  # IDがデータベースに存在するかどうかを判断する関数
+    exists,  # IDがデータベースに存在するかどうかを判断する関数
     length = 7,  # 基本長（衝突が発生した場合、自動的に長くなります）
     ab = "16",  # アルファベットの種類（base64url... URLセーフな64進数、16... 16進数）
 )
 id_dic[s_id] = True
 print(s_id)
 ```
```

### Comparing `slim-id-0.0.1/setup.py` & `slim-id-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 00000080: 205b 657a 7069 705d 0d0a 7769 7468 2065   [ezpip]..with e
 00000090: 7a70 6970 2e70 6163 6b61 6765 7228 6465  zpip.packager(de
 000000a0: 7665 6c6f 705f 6469 7220 3d20 222e 2f5f  velop_dir = "./_
 000000b0: 6465 7665 6c6f 705f 736c 696d 5f69 642f  develop_slim_id/
 000000c0: 2229 2061 7320 703a 0d0a 0973 6574 7570  ") as p:...setup
 000000d0: 280d 0a09 096e 616d 6520 3d20 2273 6c69  (....name = "sli
 000000e0: 6d2d 6964 222c 0d0a 0909 7665 7273 696f  m-id",....versio
-000000f0: 6e20 3d20 2230 2e30 2e31 222c 0d0a 0909  n = "0.0.1",....
+000000f0: 6e20 3d20 2230 2e30 2e32 222c 0d0a 0909  n = "0.0.2",....
 00000100: 6465 7363 7269 7074 696f 6e20 3d20 2254  description = "T
 00000110: 6869 7320 6973 2061 2074 6f6f 6c20 7468  his is a tool th
 00000120: 6174 2061 7574 6f6d 6174 6963 616c 6c79  at automatically
 00000130: 2067 656e 6572 6174 6573 2073 686f 7274   generates short
 00000140: 2049 4473 222c 0d0a 0909 6175 7468 6f72   IDs",....author
 00000150: 203d 2022 6269 625f 696e 6622 2c0d 0a09   = "bib_inf",...
 00000160: 0961 7574 686f 725f 656d 6169 6c20 3d20  .author_email =
```

### Comparing `slim-id-0.0.1/slim_id/__init__.py` & `slim-id-0.0.2/slim_id/__init__.py`

 * *Files identical despite different names*

### Comparing `slim-id-0.0.1/slim_id/test.py` & `slim-id-0.0.2/slim_id/test.py`

 * *Files identical despite different names*

### Comparing `slim-id-0.0.1/slim_id.egg-info/PKG-INFO` & `slim-id-0.0.2/slim_id.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slim-id
-Version: 0.0.1
+Version: 0.0.2
 Summary: This is a tool that automatically generates short IDs
 Home-page: https://github.co.jp/
 Author: bib_inf
 Author-email: contact.bibinf@gmail.com
 License: CC0 v1.0
 Description: # Slim-ID: A Lightweight ID Generation Library for Python
         
@@ -24,25 +24,25 @@
         ## Usage Example
         ```python
         import sys
         import slim_id
         
         id_dic = {}
         
-        def is_exists(arg_id):
+        def exists(arg_id):
             return (arg_id in id_dic)
         
         # Generate an ID using Slim-ID
-        s_id = slim_id.gen(is_exists)
+        s_id = slim_id.gen(exists)
         id_dic[s_id] = True
         print(s_id)
         
         # Generate an ID using Slim-ID with custom parameters
         s_id = slim_id.gen(
-            is_exists,  # Function to determine if an ID exists in the database
+            exists,  # Function to determine if an ID exists in the database
             length = 7,  # Base length (automatically increases if a collision occurs)
             ab = "16",  # Alphabet type (base64url... URL-safe Base64, 16... hexadecimal)
         )
         id_dic[s_id] = True
         print(s_id)
         ```
         
@@ -59,25 +59,25 @@
         
         ```python
         import sys
         import slim_id
         
         id_dic = {}
         
-        def is_exists(arg_id):
+        def exists(arg_id):
             return (arg_id in id_dic)
         
         # Slim-IDを使用してIDを生成
-        s_id = slim_id.gen(is_exists)
+        s_id = slim_id.gen(exists)
         id_dic[s_id] = True
         print(s_id)
         
         # カスタムパラメータを使用してSlim-IDでIDを生成
         s_id = slim_id.gen(
-            is_exists,  # IDがデータベースに存在するかどうかを判断する関数
+            exists,  # IDがデータベースに存在するかどうかを判断する関数
             length = 7,  # 基本長（衝突が発生した場合、自動的に長くなります）
             ab = "16",  # アルファベットの種類（base64url... URLセーフな64進数、16... 16進数）
         )
         id_dic[s_id] = True
         print(s_id)
         ```
```

