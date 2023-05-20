# Comparing `tmp/shinherpro-1.5.7.tar.gz` & `tmp/shinherpro-1.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shinherpro-1.5.7.tar", last modified: Sat May 20 13:08:39 2023, max compression
+gzip compressed data, was "shinherpro-1.5.8.tar", last modified: Sat May 20 13:12:13 2023, max compression
```

## Comparing `shinherpro-1.5.7.tar` & `shinherpro-1.5.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 13:08:39.571956 shinherpro-1.5.7/
--rw-rw-rw-   0        0        0     3820 2023-05-20 13:08:39.571461 shinherpro-1.5.7/PKG-INFO
--rw-rw-rw-   0        0        0     3640 2023-05-20 13:08:22.000000 shinherpro-1.5.7/README.md
--rw-rw-rw-   0        0        0       42 2023-05-20 13:08:39.571956 shinherpro-1.5.7/setup.cfg
--rw-rw-rw-   0        0        0      852 2023-05-20 13:08:17.000000 shinherpro-1.5.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-20 13:08:39.558565 shinherpro-1.5.7/shinherpro/
--rw-rw-rw-   0        0        0    10823 2023-05-20 13:08:34.000000 shinherpro-1.5.7/shinherpro/TYAI.py
--rw-rw-rw-   0        0        0        0 2023-05-18 14:47:36.000000 shinherpro-1.5.7/shinherpro/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-20 13:08:39.569972 shinherpro-1.5.7/shinherpro.egg-info/
--rw-rw-rw-   0        0        0     3820 2023-05-20 13:08:39.000000 shinherpro-1.5.7/shinherpro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2023-05-20 13:08:39.000000 shinherpro-1.5.7/shinherpro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 13:08:39.000000 shinherpro-1.5.7/shinherpro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-05-20 13:08:39.000000 shinherpro-1.5.7/shinherpro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-20 13:08:39.000000 shinherpro-1.5.7/shinherpro.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-20 13:12:13.177266 shinherpro-1.5.8/
+-rw-rw-rw-   0        0        0     3841 2023-05-20 13:12:13.176769 shinherpro-1.5.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3661 2023-05-20 13:10:07.000000 shinherpro-1.5.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-20 13:12:13.177266 shinherpro-1.5.8/setup.cfg
+-rw-rw-rw-   0        0        0      852 2023-05-20 13:12:07.000000 shinherpro-1.5.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 13:12:13.164371 shinherpro-1.5.8/shinherpro/
+-rw-rw-rw-   0        0        0    10823 2023-05-20 13:08:34.000000 shinherpro-1.5.8/shinherpro/TYAI.py
+-rw-rw-rw-   0        0        0        0 2023-05-18 14:47:36.000000 shinherpro-1.5.8/shinherpro/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-20 13:12:13.175778 shinherpro-1.5.8/shinherpro.egg-info/
+-rw-rw-rw-   0        0        0     3841 2023-05-20 13:12:13.000000 shinherpro-1.5.8/shinherpro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2023-05-20 13:12:13.000000 shinherpro-1.5.8/shinherpro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 13:12:13.000000 shinherpro-1.5.8/shinherpro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-05-20 13:12:13.000000 shinherpro-1.5.8/shinherpro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-20 13:12:13.000000 shinherpro-1.5.8/shinherpro.egg-info/top_level.txt
```

### Comparing `shinherpro-1.5.7/PKG-INFO` & `shinherpro-1.5.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,55 +1,47 @@
-Metadata-Version: 2.1
-Name: shinherpro
-Version: 1.5.7
-Summary: shinher-pro 1.5.7
-Author: Yihuan
-Author-email: ivan17.lai@gmail.com
-Description-Content-Type: text/markdown
-
 # Shinher-Pro V1.5.7
 
 ### 這個程式是一個自動化的成績查詢工具，它使用 Selenium 和 BeautifulSoup 套件來模擬網頁瀏覽和解析 HTML 內容，並使用 Keras 加載自訓練的 AI 模型進行圖形驗證碼自動辨識。它可以自動登入到支援的成績查詢網站，通常是欣河線上查詢系統，只需輸入帳號密碼，程序會自動操作到成績業面並返回成績，跳過原先繁雜的操作。
 
 ## use
 ```
 from shinherpro import TYAI
 ```
 ## setup model
-# model_setup(file.h5) 用於載入模型,回傳的內容將作為get grade()使用的必要引數.
+#### model_setup(file.h5) 用於載入模型,回傳的內容將作為get grade()使用的必要引數.
 ```
 model = TYAI.model_setup(model_path)
 ```
-# official_model(Version) 提供了官方的驗證碼辨識模型,目前僅支持5.1版本(開發中功能)
+### official_model(Version) 提供了官方的驗證碼辨識模型,目前僅支持5.1版本(開發中功能)
 ```
 model_path = official_model(5.1)
 model = model_setup(model_path)
 ```
 ## setup chrome driver
-# chrome_driver_setup(url,view) 用於打開chrome driver 並開啟指定網址,,回傳的內容將作為get grade()使用的必要引數.
+### chrome_driver_setup(url,view) 用於打開chrome driver 並開啟指定網址,,回傳的內容將作為get grade()使用的必要引數.
 ```
 driver = TYAI.chrome_driver_setup(url,view)
 ```
-# url為指定的網址,view可指定模擬遊覽器執行時是否要顯示實體頁面.
-# urlGet() 提供了TYAI的成績查詢連結
+### url為指定的網址,view可指定模擬遊覽器執行時是否要顯示實體頁面.
+### urlGet() 提供了TYAI的成績查詢連結
 ```
 url = TYAI.urlGet() = "https://sai.tyai.tyc.edu.tw/online/"
 driver = TYAI.chrome_driver_setup(url,True)
 ```
 ## get grade
-# TYAI.getGrades() 函式用於獲取成績資訊。你需要提供(學號、密碼(身分證字號)、WebDriver對象、AI模型、考試名稱)作為輸入參數。函式內部進行驗證碼辨識、登入操作，然後切換到成績查詢頁面，獲取成績表格的 HTML 內容,並使用json格式回傳.
+### TYAI.getGrades() 函式用於獲取成績資訊。你需要提供(學號、密碼(身分證字號)、WebDriver對象、AI模型、考試名稱)作為輸入參數。函式內部進行驗證碼辨識、登入操作，然後切換到成績查詢頁面，獲取成績表格的 HTML 內容,並使用json格式回傳.
 ```
 TYAI.getGrades(username, password, driver, model,examname):
 ```
-# driver、model 為提前初始化所取得的回傳值
+### driver、model 為提前初始化所取得的回傳值
 
-# 可以根據 code 的值來判斷返回結果的狀態，並根據需要處理相應的資訊。
-# code 0 正常回傳成績 , code 1 帳號密碼錯誤 , code 2 登入失敗次數過多 , code 3 未知的錯誤訊息 
+### 可以根據 code 的值來判斷返回結果的狀態，並根據需要處理相應的資訊。
+### code 0 正常回傳成績 , code 1 帳號密碼錯誤 , code 2 登入失敗次數過多 , code 3 未知的錯誤訊息 
 
-# 如果登入成功，成績查詢成功，則返回以下格式的json：
+### 如果登入成功，成績查詢成功，則返回以下格式的json：
 ```
 {
     "code": 0,
     "考試標題": "考試標題",
     "學號": "學號",
     "姓名": "姓名",
     "班級": "班級",
```

### Comparing `shinherpro-1.5.7/README.md` & `shinherpro-1.5.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,47 +1,55 @@
+Metadata-Version: 2.1
+Name: shinherpro
+Version: 1.5.8
+Summary: shinher-pro 1.5.8
+Author: Yihuan
+Author-email: ivan17.lai@gmail.com
+Description-Content-Type: text/markdown
+
 # Shinher-Pro V1.5.7
 
 ### 這個程式是一個自動化的成績查詢工具，它使用 Selenium 和 BeautifulSoup 套件來模擬網頁瀏覽和解析 HTML 內容，並使用 Keras 加載自訓練的 AI 模型進行圖形驗證碼自動辨識。它可以自動登入到支援的成績查詢網站，通常是欣河線上查詢系統，只需輸入帳號密碼，程序會自動操作到成績業面並返回成績，跳過原先繁雜的操作。
 
 ## use
 ```
 from shinherpro import TYAI
 ```
 ## setup model
-# model_setup(file.h5) 用於載入模型,回傳的內容將作為get grade()使用的必要引數.
+#### model_setup(file.h5) 用於載入模型,回傳的內容將作為get grade()使用的必要引數.
 ```
 model = TYAI.model_setup(model_path)
 ```
-# official_model(Version) 提供了官方的驗證碼辨識模型,目前僅支持5.1版本(開發中功能)
+### official_model(Version) 提供了官方的驗證碼辨識模型,目前僅支持5.1版本(開發中功能)
 ```
 model_path = official_model(5.1)
 model = model_setup(model_path)
 ```
 ## setup chrome driver
-# chrome_driver_setup(url,view) 用於打開chrome driver 並開啟指定網址,,回傳的內容將作為get grade()使用的必要引數.
+### chrome_driver_setup(url,view) 用於打開chrome driver 並開啟指定網址,,回傳的內容將作為get grade()使用的必要引數.
 ```
 driver = TYAI.chrome_driver_setup(url,view)
 ```
-# url為指定的網址,view可指定模擬遊覽器執行時是否要顯示實體頁面.
-# urlGet() 提供了TYAI的成績查詢連結
+### url為指定的網址,view可指定模擬遊覽器執行時是否要顯示實體頁面.
+### urlGet() 提供了TYAI的成績查詢連結
 ```
 url = TYAI.urlGet() = "https://sai.tyai.tyc.edu.tw/online/"
 driver = TYAI.chrome_driver_setup(url,True)
 ```
 ## get grade
-# TYAI.getGrades() 函式用於獲取成績資訊。你需要提供(學號、密碼(身分證字號)、WebDriver對象、AI模型、考試名稱)作為輸入參數。函式內部進行驗證碼辨識、登入操作，然後切換到成績查詢頁面，獲取成績表格的 HTML 內容,並使用json格式回傳.
+### TYAI.getGrades() 函式用於獲取成績資訊。你需要提供(學號、密碼(身分證字號)、WebDriver對象、AI模型、考試名稱)作為輸入參數。函式內部進行驗證碼辨識、登入操作，然後切換到成績查詢頁面，獲取成績表格的 HTML 內容,並使用json格式回傳.
 ```
 TYAI.getGrades(username, password, driver, model,examname):
 ```
-# driver、model 為提前初始化所取得的回傳值
+### driver、model 為提前初始化所取得的回傳值
 
-# 可以根據 code 的值來判斷返回結果的狀態，並根據需要處理相應的資訊。
-# code 0 正常回傳成績 , code 1 帳號密碼錯誤 , code 2 登入失敗次數過多 , code 3 未知的錯誤訊息 
+### 可以根據 code 的值來判斷返回結果的狀態，並根據需要處理相應的資訊。
+### code 0 正常回傳成績 , code 1 帳號密碼錯誤 , code 2 登入失敗次數過多 , code 3 未知的錯誤訊息 
 
-# 如果登入成功，成績查詢成功，則返回以下格式的json：
+### 如果登入成功，成績查詢成功，則返回以下格式的json：
 ```
 {
     "code": 0,
     "考試標題": "考試標題",
     "學號": "學號",
     "姓名": "姓名",
     "班級": "班級",
```

### Comparing `shinherpro-1.5.7/setup.py` & `shinherpro-1.5.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,16 @@
     def run(self):
         print("\033[93m 正在安裝shinher-pro...")
         install.run(self)
         print("shinherpro安裝完成！ \033[0m")
 
 setup(
     name='shinherpro',
-    version='1.5.7',
-    description='shinher-pro 1.5.7',
+    version='1.5.8',
+    description='shinher-pro 1.5.8',
     author='Yihuan',
     author_email='ivan17.lai@gmail.com',
     packages=['shinherpro'],
     install_requires=[
         'selenium',
         'beautifulsoup4',
         'keras',
```

### Comparing `shinherpro-1.5.7/shinherpro/TYAI.py` & `shinherpro-1.5.8/shinherpro/TYAI.py`

 * *Files identical despite different names*

### Comparing `shinherpro-1.5.7/shinherpro.egg-info/PKG-INFO` & `shinherpro-1.5.8/shinherpro.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 Metadata-Version: 2.1
 Name: shinherpro
-Version: 1.5.7
-Summary: shinher-pro 1.5.7
+Version: 1.5.8
+Summary: shinher-pro 1.5.8
 Author: Yihuan
 Author-email: ivan17.lai@gmail.com
 Description-Content-Type: text/markdown
 
 # Shinher-Pro V1.5.7
 
 ### 這個程式是一個自動化的成績查詢工具，它使用 Selenium 和 BeautifulSoup 套件來模擬網頁瀏覽和解析 HTML 內容，並使用 Keras 加載自訓練的 AI 模型進行圖形驗證碼自動辨識。它可以自動登入到支援的成績查詢網站，通常是欣河線上查詢系統，只需輸入帳號密碼，程序會自動操作到成績業面並返回成績，跳過原先繁雜的操作。
 
 ## use
 ```
 from shinherpro import TYAI
 ```
 ## setup model
-# model_setup(file.h5) 用於載入模型,回傳的內容將作為get grade()使用的必要引數.
+#### model_setup(file.h5) 用於載入模型,回傳的內容將作為get grade()使用的必要引數.
 ```
 model = TYAI.model_setup(model_path)
 ```
-# official_model(Version) 提供了官方的驗證碼辨識模型,目前僅支持5.1版本(開發中功能)
+### official_model(Version) 提供了官方的驗證碼辨識模型,目前僅支持5.1版本(開發中功能)
 ```
 model_path = official_model(5.1)
 model = model_setup(model_path)
 ```
 ## setup chrome driver
-# chrome_driver_setup(url,view) 用於打開chrome driver 並開啟指定網址,,回傳的內容將作為get grade()使用的必要引數.
+### chrome_driver_setup(url,view) 用於打開chrome driver 並開啟指定網址,,回傳的內容將作為get grade()使用的必要引數.
 ```
 driver = TYAI.chrome_driver_setup(url,view)
 ```
-# url為指定的網址,view可指定模擬遊覽器執行時是否要顯示實體頁面.
-# urlGet() 提供了TYAI的成績查詢連結
+### url為指定的網址,view可指定模擬遊覽器執行時是否要顯示實體頁面.
+### urlGet() 提供了TYAI的成績查詢連結
 ```
 url = TYAI.urlGet() = "https://sai.tyai.tyc.edu.tw/online/"
 driver = TYAI.chrome_driver_setup(url,True)
 ```
 ## get grade
-# TYAI.getGrades() 函式用於獲取成績資訊。你需要提供(學號、密碼(身分證字號)、WebDriver對象、AI模型、考試名稱)作為輸入參數。函式內部進行驗證碼辨識、登入操作，然後切換到成績查詢頁面，獲取成績表格的 HTML 內容,並使用json格式回傳.
+### TYAI.getGrades() 函式用於獲取成績資訊。你需要提供(學號、密碼(身分證字號)、WebDriver對象、AI模型、考試名稱)作為輸入參數。函式內部進行驗證碼辨識、登入操作，然後切換到成績查詢頁面，獲取成績表格的 HTML 內容,並使用json格式回傳.
 ```
 TYAI.getGrades(username, password, driver, model,examname):
 ```
-# driver、model 為提前初始化所取得的回傳值
+### driver、model 為提前初始化所取得的回傳值
 
-# 可以根據 code 的值來判斷返回結果的狀態，並根據需要處理相應的資訊。
-# code 0 正常回傳成績 , code 1 帳號密碼錯誤 , code 2 登入失敗次數過多 , code 3 未知的錯誤訊息 
+### 可以根據 code 的值來判斷返回結果的狀態，並根據需要處理相應的資訊。
+### code 0 正常回傳成績 , code 1 帳號密碼錯誤 , code 2 登入失敗次數過多 , code 3 未知的錯誤訊息 
 
-# 如果登入成功，成績查詢成功，則返回以下格式的json：
+### 如果登入成功，成績查詢成功，則返回以下格式的json：
 ```
 {
     "code": 0,
     "考試標題": "考試標題",
     "學號": "學號",
     "姓名": "姓名",
     "班級": "班級",
```

