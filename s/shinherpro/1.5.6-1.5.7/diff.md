# Comparing `tmp/shinherpro-1.5.6.tar.gz` & `tmp/shinherpro-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shinherpro-1.5.6.tar", last modified: Sat May 20 13:03:18 2023, max compression
+gzip compressed data, was "shinherpro-1.5.7.tar", last modified: Sat May 20 13:08:39 2023, max compression
```

## Comparing `shinherpro-1.5.6.tar` & `shinherpro-1.5.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 13:03:18.318763 shinherpro-1.5.6/
--rw-rw-rw-   0        0        0      137 2023-05-20 13:03:18.317771 shinherpro-1.5.6/PKG-INFO
--rw-rw-rw-   0        0        0     3640 2023-05-20 13:00:24.000000 shinherpro-1.5.6/README.md
--rw-rw-rw-   0        0        0       42 2023-05-20 13:03:18.318763 shinherpro-1.5.6/setup.cfg
--rw-rw-rw-   0        0        0      635 2023-05-20 13:02:00.000000 shinherpro-1.5.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-20 13:03:18.305866 shinherpro-1.5.6/shinherpro/
--rw-rw-rw-   0        0        0    10823 2023-05-20 13:03:15.000000 shinherpro-1.5.6/shinherpro/TYAI.py
--rw-rw-rw-   0        0        0        0 2023-05-18 14:47:36.000000 shinherpro-1.5.6/shinherpro/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-20 13:03:18.316778 shinherpro-1.5.6/shinherpro.egg-info/
--rw-rw-rw-   0        0        0      137 2023-05-20 13:03:18.000000 shinherpro-1.5.6/shinherpro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2023-05-20 13:03:18.000000 shinherpro-1.5.6/shinherpro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 13:03:18.000000 shinherpro-1.5.6/shinherpro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-05-20 13:03:18.000000 shinherpro-1.5.6/shinherpro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-20 13:03:18.000000 shinherpro-1.5.6/shinherpro.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-20 13:08:39.571956 shinherpro-1.5.7/
+-rw-rw-rw-   0        0        0     3820 2023-05-20 13:08:39.571461 shinherpro-1.5.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3640 2023-05-20 13:08:22.000000 shinherpro-1.5.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-20 13:08:39.571956 shinherpro-1.5.7/setup.cfg
+-rw-rw-rw-   0        0        0      852 2023-05-20 13:08:17.000000 shinherpro-1.5.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 13:08:39.558565 shinherpro-1.5.7/shinherpro/
+-rw-rw-rw-   0        0        0    10823 2023-05-20 13:08:34.000000 shinherpro-1.5.7/shinherpro/TYAI.py
+-rw-rw-rw-   0        0        0        0 2023-05-18 14:47:36.000000 shinherpro-1.5.7/shinherpro/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-20 13:08:39.569972 shinherpro-1.5.7/shinherpro.egg-info/
+-rw-rw-rw-   0        0        0     3820 2023-05-20 13:08:39.000000 shinherpro-1.5.7/shinherpro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2023-05-20 13:08:39.000000 shinherpro-1.5.7/shinherpro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 13:08:39.000000 shinherpro-1.5.7/shinherpro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-05-20 13:08:39.000000 shinherpro-1.5.7/shinherpro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-20 13:08:39.000000 shinherpro-1.5.7/shinherpro.egg-info/top_level.txt
```

### Comparing `shinherpro-1.5.6/README.md` & `shinherpro-1.5.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Shinher-Pro V1.5.6
+# Shinher-Pro V1.5.7
 
 ### 這個程式是一個自動化的成績查詢工具，它使用 Selenium 和 BeautifulSoup 套件來模擬網頁瀏覽和解析 HTML 內容，並使用 Keras 加載自訓練的 AI 模型進行圖形驗證碼自動辨識。它可以自動登入到支援的成績查詢網站，通常是欣河線上查詢系統，只需輸入帳號密碼，程序會自動操作到成績業面並返回成績，跳過原先繁雜的操作。
 
 ## use
 ```
 from shinherpro import TYAI
 ```
```

### Comparing `shinherpro-1.5.6/shinherpro/TYAI.py` & `shinherpro-1.5.7/shinherpro/TYAI.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import numpy as np
 import cv2
 import time
 import json
 import os
 
 ###################################################
-# V 1.5.6 By Yihuan Studio --> 2023/5/20/09:02:49  
+# V 1.5.7 By Yihuan Studio --> 2023/5/20/09:08:49  
 
 #############################################
 #  vfcCode AI model 5.1  x4307 picture
 ##  image enhancement algorithm V1 By Sam
 
 def model_setup(model_path):
     full_path = os.path.abspath(model_path)
```

