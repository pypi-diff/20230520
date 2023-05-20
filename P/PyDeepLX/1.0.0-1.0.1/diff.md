# Comparing `tmp/PyDeepLX-1.0.0.tar.gz` & `tmp/PyDeepLX-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyDeepLX-1.0.0.tar", last modified: Wed Apr 26 17:58:44 2023, max compression
+gzip compressed data, was "PyDeepLX-1.0.1.tar", last modified: Sat May 20 19:47:25 2023, max compression
```

## Comparing `PyDeepLX-1.0.0.tar` & `PyDeepLX-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-04-26 17:58:44.976916 PyDeepLX-1.0.0/
--rw-r--r--   0 vincent    (501) staff       (20)     1076 2023-04-26 16:41:03.000000 PyDeepLX-1.0.0/LICENSE
--rw-r--r--   0 vincent    (501) staff       (20)     2451 2023-04-26 17:58:44.976771 PyDeepLX-1.0.0/PKG-INFO
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-04-26 17:58:44.975395 PyDeepLX-1.0.0/PyDeepLX/
--rw-r--r--   0 vincent    (501) staff       (20)     3364 2023-04-26 17:50:46.000000 PyDeepLX-1.0.0/PyDeepLX/PyDeepLX.py
--rw-r--r--   0 vincent    (501) staff       (20)      258 2023-04-26 17:58:27.000000 PyDeepLX-1.0.0/PyDeepLX/__init__.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-04-26 17:58:44.976510 PyDeepLX-1.0.0/PyDeepLX.egg-info/
--rw-r--r--   0 vincent    (501) staff       (20)     2451 2023-04-26 17:58:44.000000 PyDeepLX-1.0.0/PyDeepLX.egg-info/PKG-INFO
--rw-r--r--   0 vincent    (501) staff       (20)      258 2023-04-26 17:58:44.000000 PyDeepLX-1.0.0/PyDeepLX.egg-info/SOURCES.txt
--rw-r--r--   0 vincent    (501) staff       (20)        1 2023-04-26 17:58:44.000000 PyDeepLX-1.0.0/PyDeepLX.egg-info/dependency_links.txt
--rw-r--r--   0 vincent    (501) staff       (20)        1 2023-04-26 17:58:35.000000 PyDeepLX-1.0.0/PyDeepLX.egg-info/not-zip-safe
--rw-r--r--   0 vincent    (501) staff       (20)       17 2023-04-26 17:58:44.000000 PyDeepLX-1.0.0/PyDeepLX.egg-info/requires.txt
--rw-r--r--   0 vincent    (501) staff       (20)        9 2023-04-26 17:58:44.000000 PyDeepLX-1.0.0/PyDeepLX.egg-info/top_level.txt
--rw-r--r--   0 vincent    (501) staff       (20)     1393 2023-04-26 17:55:28.000000 PyDeepLX-1.0.0/README.md
--rw-r--r--   0 vincent    (501) staff       (20)       38 2023-04-26 17:58:44.976958 PyDeepLX-1.0.0/setup.cfg
--rw-r--r--   0 vincent    (501) staff       (20)     1621 2023-04-26 17:33:36.000000 PyDeepLX-1.0.0/setup.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-05-20 19:47:25.316164 PyDeepLX-1.0.1/
+-rw-r--r--   0 vincent    (501) staff       (20)     1076 2023-04-26 16:41:03.000000 PyDeepLX-1.0.1/LICENSE
+-rw-r--r--   0 vincent    (501) staff       (20)     2570 2023-05-20 19:47:25.315709 PyDeepLX-1.0.1/PKG-INFO
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-05-20 19:47:25.314631 PyDeepLX-1.0.1/PyDeepLX/
+-rw-r--r--   0 vincent    (501) staff       (20)     3950 2023-05-20 19:45:48.000000 PyDeepLX-1.0.1/PyDeepLX/PyDeepLX.py
+-rw-r--r--   0 vincent    (501) staff       (20)      258 2023-04-26 17:58:27.000000 PyDeepLX-1.0.1/PyDeepLX/__init__.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-05-20 19:47:25.315472 PyDeepLX-1.0.1/PyDeepLX.egg-info/
+-rw-r--r--   0 vincent    (501) staff       (20)     2570 2023-05-20 19:47:25.000000 PyDeepLX-1.0.1/PyDeepLX.egg-info/PKG-INFO
+-rw-r--r--   0 vincent    (501) staff       (20)      258 2023-05-20 19:47:25.000000 PyDeepLX-1.0.1/PyDeepLX.egg-info/SOURCES.txt
+-rw-r--r--   0 vincent    (501) staff       (20)        1 2023-05-20 19:47:25.000000 PyDeepLX-1.0.1/PyDeepLX.egg-info/dependency_links.txt
+-rw-r--r--   0 vincent    (501) staff       (20)        1 2023-04-26 17:58:35.000000 PyDeepLX-1.0.1/PyDeepLX.egg-info/not-zip-safe
+-rw-r--r--   0 vincent    (501) staff       (20)       24 2023-05-20 19:47:25.000000 PyDeepLX-1.0.1/PyDeepLX.egg-info/requires.txt
+-rw-r--r--   0 vincent    (501) staff       (20)        9 2023-05-20 19:47:25.000000 PyDeepLX-1.0.1/PyDeepLX.egg-info/top_level.txt
+-rw-r--r--   0 vincent    (501) staff       (20)     1512 2023-05-20 19:43:13.000000 PyDeepLX-1.0.1/README.md
+-rw-r--r--   0 vincent    (501) staff       (20)       38 2023-05-20 19:47:25.316221 PyDeepLX-1.0.1/setup.cfg
+-rw-r--r--   0 vincent    (501) staff       (20)     1628 2023-05-20 19:46:56.000000 PyDeepLX-1.0.1/setup.py
```

### Comparing `PyDeepLX-1.0.0/LICENSE` & `PyDeepLX-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyDeepLX-1.0.0/PKG-INFO` & `PyDeepLX-1.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyDeepLX
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python package for unlimited DeepL translation
 Home-page: https://github.com/OwO-Network/PyDeepLX
 Author: missuo
 Author-email: i@yyt.moe
 License: MIT
 Platform: any
 Classifier: Environment :: Web Environment
@@ -28,35 +28,38 @@
 # PyDeepLX
 A Python package for unlimited DeepL translation
 
 ## API Version
 [OwO-Network/DeepLX](https://github.com/OwO-Network/DeepLX): Permanently free DeepL API written in Golang.
 
 ## Description
-This is a Python package translated by DeepL, I didn't limit the number of translations in the code, if there is a `429` error, it means your IP has been blocked by DeepL temporarily, please don't request it frequently in a short time.
+This is a Python package for DeepL translation, I didn't limit the number of translations in the code, if there is a `429` error, it means your IP has been blocked by DeepL temporarily, please don't request it frequently in a short time.
 
 ## Usage
 ### Install Package
 ```bash
 pip install PyDeepLX
 ```
 ### Use in code
 ```python
 from PyDeepLX import PyDeepLX
 # By default, the source language is automatically recognized and translated into English without providing any alternative results.
-targetText = PyDeepLX.translate("你好世界") # Return String
+PyDeepLX.translate("你好世界") # Return String
 
 # Specify the source and target languages
-targetText = PyDeepLX.translate("你好世界", "ZH", "JP") # Return String
+PyDeepLX.translate("你好世界", "ZH", "EN") # Return String
 
 # Need alternative results
-targetText = PyDeepLX.translate("毫无疑问的", "ZH", "JP", True) # Return List: ['Without a doubt', 'No doubt']
+PyDeepLX.translate("毫无疑问的", "ZH", "EN", True) # Return List: ['Without a doubt', 'No doubt']
 
 # Print the results
-targetText = PyDeepLX.translate("毫无疑问的", "ZH", "JP", True, True)
+PyDeepLX.translate("毫无疑问的", "ZH", "EN", True, True)
+
+# Using proxy
+PyDeepLX.translate(text="毫无疑问的", sourceLang="ZH", targetLang="EN", needAlternative=False, printResult=False, proxies="socks5://127.0.0.1:7890")
 ```
 
 ## PyPi
 <a href="https://pypi.org/project/PyDeepLX/"><img src="https://img.shields.io/badge/Pypi-000000?style=for-the-badge&logo=pypi&logoColor=red" /></a>
 
 ## Author
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyDeepLX Version: 1.0.0 Summary: A Python package
+Metadata-Version: 2.1 Name: PyDeepLX Version: 1.0.1 Summary: A Python package
 for unlimited DeepL translation Home-page: https://github.com/OwO-Network/
 PyDeepLX Author: missuo Author-email: i@yyt.moe License: MIT Platform: any
 Classifier: Environment :: Web Environment Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.3 Classifier: Programming
 Language :: Python :: 3.4 Classifier: Programming Language :: Python :: 3.5
@@ -10,23 +10,24 @@
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic
 Content Classifier: Topic :: Software Development :: Libraries :: Python
 Modules Description-Content-Type: text/markdown License-File: LICENSE #
 PyDeepLX A Python package for unlimited DeepL translation ## API Version [OwO-
 Network/DeepLX](https://github.com/OwO-Network/DeepLX): Permanently free DeepL
-API written in Golang. ## Description This is a Python package translated by
-DeepL, I didn't limit the number of translations in the code, if there is a
-`429` error, it means your IP has been blocked by DeepL temporarily, please
+API written in Golang. ## Description This is a Python package for DeepL
+translation, I didn't limit the number of translations in the code, if there is
+a `429` error, it means your IP has been blocked by DeepL temporarily, please
 don't request it frequently in a short time. ## Usage ### Install Package
 ```bash pip install PyDeepLX ``` ### Use in code ```python from PyDeepLX import
 PyDeepLX # By default, the source language is automatically recognized and
-translated into English without providing any alternative results. targetText =
+translated into English without providing any alternative results.
 PyDeepLX.translate("ä½ å¥½ä¸ç") # Return String # Specify the source and
-target languages targetText = PyDeepLX.translate("ä½ å¥½ä¸ç", "ZH", "JP") #
-Return String # Need alternative results targetText = PyDeepLX.translate
-("æ¯«æ çé®ç", "ZH", "JP", True) # Return List: ['Without a doubt', 'No
-doubt'] # Print the results targetText = PyDeepLX.translate("æ¯«æ çé®ç",
-"ZH", "JP", True, True) ``` ## PyPi [https://img.shields.io/badge/Pypi-
-000000?style=for-the-badge&logo=pypi&logoColor=red] ## Author **PyDeepLX** Â©
-[Vincent Young](https://github.com/missuo), Released under the [MIT](./LICENSE)
-License.
+target languages PyDeepLX.translate("ä½ å¥½ä¸ç", "ZH", "EN") # Return String
+# Need alternative results PyDeepLX.translate("æ¯«æ çé®ç", "ZH", "EN",
+True) # Return List: ['Without a doubt', 'No doubt'] # Print the results
+PyDeepLX.translate("æ¯«æ çé®ç", "ZH", "EN", True, True) # Using proxy
+PyDeepLX.translate(text="æ¯«æ çé®ç", sourceLang="ZH", targetLang="EN",
+needAlternative=False, printResult=False, proxies="socks5://127.0.0.1:7890")
+``` ## PyPi [https://img.shields.io/badge/Pypi-000000?style=for-the-
+badge&logo=pypi&logoColor=red] ## Author **PyDeepLX** Â© [Vincent Young](https:
+//github.com/missuo), Released under the [MIT](./LICENSE) License.
```

### Comparing `PyDeepLX-1.0.0/PyDeepLX/PyDeepLX.py` & `PyDeepLX-1.0.1/PyDeepLX/PyDeepLX.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 Author: Vincent Young
 Date: 2023-04-27 00:44:01
 LastEditors: Vincent Young
-LastEditTime: 2023-04-27 01:49:55
+LastEditTime: 2023-05-21 03:45:32
 FilePath: /PyDeepLX/PyDeepLX/PyDeepLX.py
 Telegram: https://t.me/missuo
 
 Copyright © 2023 by Vincent, All Rights Reserved. 
 '''
 import random
 import time
@@ -26,14 +26,21 @@
     "x-app-device": "iPhone13,2",
     "User-Agent": "DeepL-iOS/2.6.0 iOS 16.3.0 (iPhone13,2)",
     "x-app-build": "353933",
     "x-app-version": "2.6",
     "Connection": "keep-alive"
 }
 
+
+class TooManyRequestsException(Exception):
+    "Raised when there is a 429 error"
+    def __str__(self):
+        return "PyDeepLX Error: Too many requests, your IP has been blocked by DeepL temporarily, please don't request it frequently in a short time."
+
+
 def detectLang(translateText) -> str:
     language = detect(translateText)
     return language.upper()
 
 def getICount(translateText) -> int:
     return translateText.count('i')
 
@@ -49,15 +56,15 @@
     if iCount != 0:
         iCount += 1
         return ts - ts % iCount + iCount
     else:
         return ts
 
 
-def translate(text, sourceLang=None, targetLang=None, needAlternative=False, printResult=False):
+def translate(text, sourceLang=None, targetLang=None, needAlternative=False, printResult=False, proxies=None):
     iCount = getICount(text)
     id = getRandomNumber()
     if sourceLang == None:
         sourceLang = detectLang(text)
     if targetLang == None:
         targetLang = "EN"
 
@@ -85,33 +92,38 @@
 
     if (id+5) % 29 == 0 or (id+3) % 13 == 0:
         postDataStr = postDataStr.replace(
             "\"method\":\"", "\"method\" : \"", -1)
     else:
         postDataStr = postDataStr.replace(
             "\"method\":\"", "\"method\": \"", -1)
-    resp = httpx.post(url=deeplAPI, data=postDataStr, headers=headers)
-    respStatusCode = resp.status_code
-    respText = resp.text
-    respJson = json.loads(respText)
-    targetTextArray = []
-    if respStatusCode == 200:
-        if needAlternative == True:
-            targetText = respJson["result"]["texts"][0]["text"]
-            if printResult == True:
-                print(targetText)
-            for item in respJson["result"]["texts"][0]["alternatives"]:
-                targetTextArray.append(item["text"])
+        
+    # Add proxy (e.g. proxies='socks5://127.0.0.1:9150')
+    with httpx.Client(proxies=proxies) as client:
+        resp = client.post(url=deeplAPI, data=postDataStr, headers=headers)
+        respStatusCode = resp.status_code
+        respText = resp.text
+        respJson = json.loads(respText)
+        targetTextArray = []
+        if respStatusCode == 200:
+            if needAlternative == True:
+                targetText = respJson["result"]["texts"][0]["text"]
                 if printResult == True:
-                    print(item["text"])
-            return targetTextArray
+                    print(targetText)
+                for item in respJson["result"]["texts"][0]["alternatives"]:
+                    targetTextArray.append(item["text"])
+                    if printResult == True:
+                        print(item["text"])
+                return targetTextArray
+            else:
+                targetText = respJson["result"]["texts"][0]["text"]
+                if printResult == True:
+                    print(targetText)
+                return targetText
+        elif respStatusCode == 429:
+            raise TooManyRequestsException
         else:
-            targetText = respJson["result"]["texts"][0]["text"]
-            if printResult == True:
-                print(targetText)
-            return targetText
-    else:
-        print("Error", respStatusCode)
-        return None
+            print("Error", respStatusCode)
+            return None
 
 # Example Call
-# translate("明天你好", "ZH", "EN", True, True)
+translate("明天你好", "ZH", "EN", True, True, "socks5://127.0.0.1:7890")
```

### Comparing `PyDeepLX-1.0.0/PyDeepLX.egg-info/PKG-INFO` & `PyDeepLX-1.0.1/PyDeepLX.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyDeepLX
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python package for unlimited DeepL translation
 Home-page: https://github.com/OwO-Network/PyDeepLX
 Author: missuo
 Author-email: i@yyt.moe
 License: MIT
 Platform: any
 Classifier: Environment :: Web Environment
@@ -28,35 +28,38 @@
 # PyDeepLX
 A Python package for unlimited DeepL translation
 
 ## API Version
 [OwO-Network/DeepLX](https://github.com/OwO-Network/DeepLX): Permanently free DeepL API written in Golang.
 
 ## Description
-This is a Python package translated by DeepL, I didn't limit the number of translations in the code, if there is a `429` error, it means your IP has been blocked by DeepL temporarily, please don't request it frequently in a short time.
+This is a Python package for DeepL translation, I didn't limit the number of translations in the code, if there is a `429` error, it means your IP has been blocked by DeepL temporarily, please don't request it frequently in a short time.
 
 ## Usage
 ### Install Package
 ```bash
 pip install PyDeepLX
 ```
 ### Use in code
 ```python
 from PyDeepLX import PyDeepLX
 # By default, the source language is automatically recognized and translated into English without providing any alternative results.
-targetText = PyDeepLX.translate("你好世界") # Return String
+PyDeepLX.translate("你好世界") # Return String
 
 # Specify the source and target languages
-targetText = PyDeepLX.translate("你好世界", "ZH", "JP") # Return String
+PyDeepLX.translate("你好世界", "ZH", "EN") # Return String
 
 # Need alternative results
-targetText = PyDeepLX.translate("毫无疑问的", "ZH", "JP", True) # Return List: ['Without a doubt', 'No doubt']
+PyDeepLX.translate("毫无疑问的", "ZH", "EN", True) # Return List: ['Without a doubt', 'No doubt']
 
 # Print the results
-targetText = PyDeepLX.translate("毫无疑问的", "ZH", "JP", True, True)
+PyDeepLX.translate("毫无疑问的", "ZH", "EN", True, True)
+
+# Using proxy
+PyDeepLX.translate(text="毫无疑问的", sourceLang="ZH", targetLang="EN", needAlternative=False, printResult=False, proxies="socks5://127.0.0.1:7890")
 ```
 
 ## PyPi
 <a href="https://pypi.org/project/PyDeepLX/"><img src="https://img.shields.io/badge/Pypi-000000?style=for-the-badge&logo=pypi&logoColor=red" /></a>
 
 ## Author
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyDeepLX Version: 1.0.0 Summary: A Python package
+Metadata-Version: 2.1 Name: PyDeepLX Version: 1.0.1 Summary: A Python package
 for unlimited DeepL translation Home-page: https://github.com/OwO-Network/
 PyDeepLX Author: missuo Author-email: i@yyt.moe License: MIT Platform: any
 Classifier: Environment :: Web Environment Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.3 Classifier: Programming
 Language :: Python :: 3.4 Classifier: Programming Language :: Python :: 3.5
@@ -10,23 +10,24 @@
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic
 Content Classifier: Topic :: Software Development :: Libraries :: Python
 Modules Description-Content-Type: text/markdown License-File: LICENSE #
 PyDeepLX A Python package for unlimited DeepL translation ## API Version [OwO-
 Network/DeepLX](https://github.com/OwO-Network/DeepLX): Permanently free DeepL
-API written in Golang. ## Description This is a Python package translated by
-DeepL, I didn't limit the number of translations in the code, if there is a
-`429` error, it means your IP has been blocked by DeepL temporarily, please
+API written in Golang. ## Description This is a Python package for DeepL
+translation, I didn't limit the number of translations in the code, if there is
+a `429` error, it means your IP has been blocked by DeepL temporarily, please
 don't request it frequently in a short time. ## Usage ### Install Package
 ```bash pip install PyDeepLX ``` ### Use in code ```python from PyDeepLX import
 PyDeepLX # By default, the source language is automatically recognized and
-translated into English without providing any alternative results. targetText =
+translated into English without providing any alternative results.
 PyDeepLX.translate("ä½ å¥½ä¸ç") # Return String # Specify the source and
-target languages targetText = PyDeepLX.translate("ä½ å¥½ä¸ç", "ZH", "JP") #
-Return String # Need alternative results targetText = PyDeepLX.translate
-("æ¯«æ çé®ç", "ZH", "JP", True) # Return List: ['Without a doubt', 'No
-doubt'] # Print the results targetText = PyDeepLX.translate("æ¯«æ çé®ç",
-"ZH", "JP", True, True) ``` ## PyPi [https://img.shields.io/badge/Pypi-
-000000?style=for-the-badge&logo=pypi&logoColor=red] ## Author **PyDeepLX** Â©
-[Vincent Young](https://github.com/missuo), Released under the [MIT](./LICENSE)
-License.
+target languages PyDeepLX.translate("ä½ å¥½ä¸ç", "ZH", "EN") # Return String
+# Need alternative results PyDeepLX.translate("æ¯«æ çé®ç", "ZH", "EN",
+True) # Return List: ['Without a doubt', 'No doubt'] # Print the results
+PyDeepLX.translate("æ¯«æ çé®ç", "ZH", "EN", True, True) # Using proxy
+PyDeepLX.translate(text="æ¯«æ çé®ç", sourceLang="ZH", targetLang="EN",
+needAlternative=False, printResult=False, proxies="socks5://127.0.0.1:7890")
+``` ## PyPi [https://img.shields.io/badge/Pypi-000000?style=for-the-
+badge&logo=pypi&logoColor=red] ## Author **PyDeepLX** Â© [Vincent Young](https:
+//github.com/missuo), Released under the [MIT](./LICENSE) License.
```

### Comparing `PyDeepLX-1.0.0/README.md` & `PyDeepLX-1.0.1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 # PyDeepLX
 A Python package for unlimited DeepL translation
 
 ## API Version
 [OwO-Network/DeepLX](https://github.com/OwO-Network/DeepLX): Permanently free DeepL API written in Golang.
 
 ## Description
-This is a Python package translated by DeepL, I didn't limit the number of translations in the code, if there is a `429` error, it means your IP has been blocked by DeepL temporarily, please don't request it frequently in a short time.
+This is a Python package for DeepL translation, I didn't limit the number of translations in the code, if there is a `429` error, it means your IP has been blocked by DeepL temporarily, please don't request it frequently in a short time.
 
 ## Usage
 ### Install Package
 ```bash
 pip install PyDeepLX
 ```
 ### Use in code
 ```python
 from PyDeepLX import PyDeepLX
 # By default, the source language is automatically recognized and translated into English without providing any alternative results.
-targetText = PyDeepLX.translate("你好世界") # Return String
+PyDeepLX.translate("你好世界") # Return String
 
 # Specify the source and target languages
-targetText = PyDeepLX.translate("你好世界", "ZH", "JP") # Return String
+PyDeepLX.translate("你好世界", "ZH", "EN") # Return String
 
 # Need alternative results
-targetText = PyDeepLX.translate("毫无疑问的", "ZH", "JP", True) # Return List: ['Without a doubt', 'No doubt']
+PyDeepLX.translate("毫无疑问的", "ZH", "EN", True) # Return List: ['Without a doubt', 'No doubt']
 
 # Print the results
-targetText = PyDeepLX.translate("毫无疑问的", "ZH", "JP", True, True)
+PyDeepLX.translate("毫无疑问的", "ZH", "EN", True, True)
+
+# Using proxy
+PyDeepLX.translate(text="毫无疑问的", sourceLang="ZH", targetLang="EN", needAlternative=False, printResult=False, proxies="socks5://127.0.0.1:7890")
 ```
 
 ## PyPi
 <a href="https://pypi.org/project/PyDeepLX/"><img src="https://img.shields.io/badge/Pypi-000000?style=for-the-badge&logo=pypi&logoColor=red" /></a>
 
 ## Author
```

#### html2text {}

```diff
@@ -1,18 +1,19 @@
 # PyDeepLX A Python package for unlimited DeepL translation ## API Version
 [OwO-Network/DeepLX](https://github.com/OwO-Network/DeepLX): Permanently free
-DeepL API written in Golang. ## Description This is a Python package translated
-by DeepL, I didn't limit the number of translations in the code, if there is a
-`429` error, it means your IP has been blocked by DeepL temporarily, please
+DeepL API written in Golang. ## Description This is a Python package for DeepL
+translation, I didn't limit the number of translations in the code, if there is
+a `429` error, it means your IP has been blocked by DeepL temporarily, please
 don't request it frequently in a short time. ## Usage ### Install Package
 ```bash pip install PyDeepLX ``` ### Use in code ```python from PyDeepLX import
 PyDeepLX # By default, the source language is automatically recognized and
-translated into English without providing any alternative results. targetText =
+translated into English without providing any alternative results.
 PyDeepLX.translate("ä½ å¥½ä¸ç") # Return String # Specify the source and
-target languages targetText = PyDeepLX.translate("ä½ å¥½ä¸ç", "ZH", "JP") #
-Return String # Need alternative results targetText = PyDeepLX.translate
-("æ¯«æ çé®ç", "ZH", "JP", True) # Return List: ['Without a doubt', 'No
-doubt'] # Print the results targetText = PyDeepLX.translate("æ¯«æ çé®ç",
-"ZH", "JP", True, True) ``` ## PyPi [https://img.shields.io/badge/Pypi-
-000000?style=for-the-badge&logo=pypi&logoColor=red] ## Author **PyDeepLX** Â©
-[Vincent Young](https://github.com/missuo), Released under the [MIT](./LICENSE)
-License.
+target languages PyDeepLX.translate("ä½ å¥½ä¸ç", "ZH", "EN") # Return String
+# Need alternative results PyDeepLX.translate("æ¯«æ çé®ç", "ZH", "EN",
+True) # Return List: ['Without a doubt', 'No doubt'] # Print the results
+PyDeepLX.translate("æ¯«æ çé®ç", "ZH", "EN", True, True) # Using proxy
+PyDeepLX.translate(text="æ¯«æ çé®ç", sourceLang="ZH", targetLang="EN",
+needAlternative=False, printResult=False, proxies="socks5://127.0.0.1:7890")
+``` ## PyPi [https://img.shields.io/badge/Pypi-000000?style=for-the-
+badge&logo=pypi&logoColor=red] ## Author **PyDeepLX** Â© [Vincent Young](https:
+//github.com/missuo), Released under the [MIT](./LICENSE) License.
```

### Comparing `PyDeepLX-1.0.0/setup.py` & `PyDeepLX-1.0.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 '''
 Author: Vincent Young
 Date: 2023-04-27 00:42:10
 LastEditors: Vincent Young
-LastEditTime: 2023-04-27 01:33:36
+LastEditTime: 2023-05-21 03:46:56
 FilePath: /PyDeepLX/setup.py
 Telegram: https://t.me/missuo
 
 Copyright © 2023 by Vincent, All Rights Reserved. 
 '''
 from setuptools import setup, find_packages
 
 with open("README.md","r") as fh:
     long_description = fh.read()
 
 setup(
     name="PyDeepLX",
     author="missuo",
-    version="1.0.0",
+    version="1.0.1",
     license='MIT',
     long_description= long_description,
     long_description_content_type="text/markdown",
     author_email="i@yyt.moe",
     description="A Python package for unlimited DeepL translation",
     url='https://github.com/OwO-Network/PyDeepLX',
     packages=find_packages(),
     include_package_data=False,
     platforms='any',
     zip_safe=False,
 
     install_requires=[
-        'httpx',
+        'httpx[socks]',
         'langdetect'
     ],
     classifiers=[
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
```

