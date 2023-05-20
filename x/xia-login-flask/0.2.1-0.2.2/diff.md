# Comparing `tmp/xia_login_flask-0.2.1-cp39-none-win_amd64.whl.zip` & `tmp/xia_login_flask-0.2.2-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 208954 bytes, number of entries: 7
--rw-r--r--  2.0 unx      109 b- defN 23-May-14 15:53 xia_login_flask/__init__.py
--rw-r--r--  2.0 unx   558592 b- defN 23-May-14 15:56 xia_login_flask/account.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      150 b- defN 23-May-14 15:56 xia_login_flask-0.2.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      739 b- defN 23-May-14 15:56 xia_login_flask-0.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-May-14 15:56 xia_login_flask-0.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-May-14 15:56 xia_login_flask-0.2.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      612 b- defN 23-May-14 15:56 xia_login_flask-0.2.1.dist-info/RECORD
-7 files, 560317 bytes uncompressed, 207856 bytes compressed:  62.9%
+Zip file size: 208953 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      109 b- defN 23-May-20 17:09 xia_login_flask/__init__.py
+-rw-r--r--  2.0 unx   558592 b- defN 23-May-20 17:12 xia_login_flask/account.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      150 b- defN 23-May-20 17:12 xia_login_flask-0.2.2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      739 b- defN 23-May-20 17:12 xia_login_flask-0.2.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-May-20 17:12 xia_login_flask-0.2.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-May-20 17:12 xia_login_flask-0.2.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      612 b- defN 23-May-20 17:12 xia_login_flask-0.2.2.dist-info/RECORD
+7 files, 560317 bytes uncompressed, 207855 bytes compressed:  62.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_login_flask/__init__.py
 Comment: 
 
 Filename: xia_login_flask/account.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_login_flask-0.2.1.dist-info/LICENSE.txt
+Filename: xia_login_flask-0.2.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_login_flask-0.2.1.dist-info/METADATA
+Filename: xia_login_flask-0.2.2.dist-info/METADATA
 Comment: 
 
-Filename: xia_login_flask-0.2.1.dist-info/WHEEL
+Filename: xia_login_flask-0.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: xia_login_flask-0.2.1.dist-info/top_level.txt
+Filename: xia_login_flask-0.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_login_flask-0.2.1.dist-info/RECORD
+Filename: xia_login_flask-0.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_login_flask/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_login_flask.account import XiaLoginFlask
 
 __all__ = [
     "XiaLoginFlask",
 ]
 
-__version__ = "0.2.1"
+__version__ = "0.2.2"
```

## Comparing `xia_login_flask-0.2.1.dist-info/METADATA` & `xia_login_flask-0.2.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-login-flask
-Version: 0.2.1
+Version: 0.2.2
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-login-flask/0.2.1/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-login-flask/0.2.2/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_login_flask-0.2.1.dist-info/RECORD` & `xia_login_flask-0.2.2.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_login_flask/__init__.py,sha256=f-asjDKwBkqd7wt6hBd0fimlWFTWPJy2aqimnoQPE3g,109
-xia_login_flask/account.cp39-win_amd64.pyd,sha256=y80hJFByhL6-ID1_7uf4uqIHM4GsazkN64QJCbdSgR8,558592
-xia_login_flask-0.2.1.dist-info/LICENSE.txt,sha256=6lRgf9k2ZgrG5cDYuhNoHP6c9esKOIPd28rlbHJdX-g,150
-xia_login_flask-0.2.1.dist-info/METADATA,sha256=zMF97T2Rg_iDGV7Sh8coKBvgF02nJ1vGV--O2ZaYTDM,739
-xia_login_flask-0.2.1.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
-xia_login_flask-0.2.1.dist-info/top_level.txt,sha256=WWeuEwln8f9FQAukiPEoo4waPy0-AIN8YAu-kkstnos,16
-xia_login_flask-0.2.1.dist-info/RECORD,,
+xia_login_flask/__init__.py,sha256=2ZmqAXeQOTIZVGzSjMj0Hv6HukNIs87SbxuevoBZAww,109
+xia_login_flask/account.cp39-win_amd64.pyd,sha256=A6nCYKez98WAn6UmgGv_v8ihawv68g-ta_oYL-Rhc6c,558592
+xia_login_flask-0.2.2.dist-info/LICENSE.txt,sha256=6lRgf9k2ZgrG5cDYuhNoHP6c9esKOIPd28rlbHJdX-g,150
+xia_login_flask-0.2.2.dist-info/METADATA,sha256=obvbHZLcwcSHsRClqHCFfl5WBFD3DHIAlFJolCwsChY,739
+xia_login_flask-0.2.2.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
+xia_login_flask-0.2.2.dist-info/top_level.txt,sha256=WWeuEwln8f9FQAukiPEoo4waPy0-AIN8YAu-kkstnos,16
+xia_login_flask-0.2.2.dist-info/RECORD,,
```

