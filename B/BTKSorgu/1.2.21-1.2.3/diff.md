# Comparing `tmp/BTKSorgu-1.2.21.tar.gz` & `tmp/BTKSorgu-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BTKSorgu-1.2.21.tar", last modified: Sat May 20 12:22:52 2023, max compression
+gzip compressed data, was "BTKSorgu-1.2.3.tar", last modified: Sat May 20 18:44:46 2023, max compression
```

## Comparing `BTKSorgu-1.2.21.tar` & `BTKSorgu-1.2.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 keyiflerolsun  (1000) keyiflerolsun  (1000)        0 2023-05-20 12:22:52.234112 BTKSorgu-1.2.21/
-drwxr-xr-x   0 keyiflerolsun  (1000) keyiflerolsun  (1000)        0 2023-05-20 12:22:52.234112 BTKSorgu-1.2.21/BTKSorgu/
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)     3332 2023-05-20 12:20:31.000000 BTKSorgu-1.2.21/BTKSorgu/Erisim_Engeli.py
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)     4043 2023-05-20 12:20:31.000000 BTKSorgu-1.2.21/BTKSorgu/KekikGUI.py
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)      165 2023-05-20 12:20:31.000000 BTKSorgu-1.2.21/BTKSorgu/__init__.py
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)      159 2023-05-20 12:20:31.000000 BTKSorgu-1.2.21/BTKSorgu/arayuz.py
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)      278 2023-05-20 12:20:31.000000 BTKSorgu-1.2.21/BTKSorgu/ekstra.py
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)      602 2023-05-20 12:20:31.000000 BTKSorgu-1.2.21/BTKSorgu/konsol.py
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)    10945 2023-05-20 12:20:31.000000 BTKSorgu-1.2.21/BTKSorgu/logo.png
-drwxr-xr-x   0 keyiflerolsun  (1000) keyiflerolsun  (1000)        0 2023-05-20 12:22:52.234112 BTKSorgu-1.2.21/BTKSorgu.egg-info/
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)     9062 2023-05-20 12:22:52.000000 BTKSorgu-1.2.21/BTKSorgu.egg-info/PKG-INFO
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)      498 2023-05-20 12:22:52.000000 BTKSorgu-1.2.21/BTKSorgu.egg-info/SOURCES.txt
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)        1 2023-05-20 12:22:52.000000 BTKSorgu-1.2.21/BTKSorgu.egg-info/dependency_links.txt
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)       87 2023-05-20 12:22:52.000000 BTKSorgu-1.2.21/BTKSorgu.egg-info/entry_points.txt
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)      100 2023-05-20 12:22:52.000000 BTKSorgu-1.2.21/BTKSorgu.egg-info/requires.txt
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)        9 2023-05-20 12:22:52.000000 BTKSorgu-1.2.21/BTKSorgu.egg-info/top_level.txt
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)    35149 2023-05-20 12:20:31.000000 BTKSorgu-1.2.21/LICENSE
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)       28 2023-05-20 12:20:31.000000 BTKSorgu-1.2.21/MANIFEST.in
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)     9062 2023-05-20 12:22:52.234112 BTKSorgu-1.2.21/PKG-INFO
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)     8489 2023-05-20 12:20:31.000000 BTKSorgu-1.2.21/README.md
-drwxr-xr-x   0 keyiflerolsun  (1000) keyiflerolsun  (1000)        0 2023-05-20 12:22:52.234112 BTKSorgu-1.2.21/Shared/
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)     2916 2023-05-20 12:20:31.000000 BTKSorgu-1.2.21/Shared/org.KekikAkademi.BTKSorgu.appdata.xml
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)      315 2023-05-20 12:20:31.000000 BTKSorgu-1.2.21/Shared/org.KekikAkademi.BTKSorgu.desktop
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)     1858 2023-05-20 12:20:31.000000 BTKSorgu-1.2.21/Shared/org.KekikAkademi.BTKSorgu.svg
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)       38 2023-05-20 12:22:52.234112 BTKSorgu-1.2.21/setup.cfg
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)     1915 2023-05-20 12:22:32.000000 BTKSorgu-1.2.21/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:44:46.056804 BTKSorgu-1.2.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:44:46.056804 BTKSorgu-1.2.3/BTKSorgu/
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-20 18:44:09.000000 BTKSorgu-1.2.3/BTKSorgu/Erisim_Engeli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-05-20 18:44:09.000000 BTKSorgu-1.2.3/BTKSorgu/KekikGUI.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-20 18:44:09.000000 BTKSorgu-1.2.3/BTKSorgu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 18:44:09.000000 BTKSorgu-1.2.3/BTKSorgu/arayuz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-20 18:44:09.000000 BTKSorgu-1.2.3/BTKSorgu/ekstra.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-20 18:44:09.000000 BTKSorgu-1.2.3/BTKSorgu/konsol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10945 2023-05-20 18:44:09.000000 BTKSorgu-1.2.3/BTKSorgu/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:44:46.056804 BTKSorgu-1.2.3/BTKSorgu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9061 2023-05-20 18:44:27.000000 BTKSorgu-1.2.3/BTKSorgu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-20 18:44:27.000000 BTKSorgu-1.2.3/BTKSorgu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 18:44:27.000000 BTKSorgu-1.2.3/BTKSorgu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-20 18:44:27.000000 BTKSorgu-1.2.3/BTKSorgu.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-20 18:44:27.000000 BTKSorgu-1.2.3/BTKSorgu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-20 18:44:27.000000 BTKSorgu-1.2.3/BTKSorgu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-20 18:44:09.000000 BTKSorgu-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-20 18:44:09.000000 BTKSorgu-1.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9061 2023-05-20 18:44:46.056804 BTKSorgu-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-05-20 18:44:09.000000 BTKSorgu-1.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:44:46.056804 BTKSorgu-1.2.3/Shared/
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-05-20 18:44:09.000000 BTKSorgu-1.2.3/Shared/org.KekikAkademi.BTKSorgu.appdata.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-20 18:44:09.000000 BTKSorgu-1.2.3/Shared/org.KekikAkademi.BTKSorgu.desktop
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-20 18:44:09.000000 BTKSorgu-1.2.3/Shared/org.KekikAkademi.BTKSorgu.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 18:44:46.056804 BTKSorgu-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-20 18:44:09.000000 BTKSorgu-1.2.3/setup.py
```

### Comparing `BTKSorgu-1.2.21/BTKSorgu/Erisim_Engeli.py` & `BTKSorgu-1.2.3/BTKSorgu/Erisim_Engeli.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.2.21/BTKSorgu/KekikGUI.py` & `BTKSorgu-1.2.3/BTKSorgu/KekikGUI.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.2.21/BTKSorgu/konsol.py` & `BTKSorgu-1.2.3/BTKSorgu/konsol.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.2.21/BTKSorgu/logo.png` & `BTKSorgu-1.2.3/BTKSorgu/logo.png`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.2.21/BTKSorgu.egg-info/PKG-INFO` & `BTKSorgu-1.2.3/BTKSorgu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BTKSorgu
-Version: 1.2.21
+Version: 1.2.3
 Summary: Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu
 Home-page: https://github.com/keyiflerolsun/BTKSorgu
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: BTKSorgu,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: BTKSorgu Version: 1.2.21 Summary: Hedef
-websitesinin BTK TarafÄ±ndan EriÅim Engeli Sorgusu Home-page: https://
-github.com/keyiflerolsun/BTKSorgu Author: keyiflerolsun Author-email:
+Metadata-Version: 2.1 Name: BTKSorgu Version: 1.2.3 Summary: Hedef websitesinin
+BTK TarafÄ±ndan EriÅim Engeli Sorgusu Home-page: https://github.com/
+keyiflerolsun/BTKSorgu Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 BTKSorgu,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
 LICENSE # [https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/
 Shared/org.KekikAkademi.BTKSorgu.svg] BTKSorgu [![Boyut](https://
```

### Comparing `BTKSorgu-1.2.21/LICENSE` & `BTKSorgu-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.2.21/PKG-INFO` & `BTKSorgu-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BTKSorgu
-Version: 1.2.21
+Version: 1.2.3
 Summary: Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu
 Home-page: https://github.com/keyiflerolsun/BTKSorgu
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: BTKSorgu,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: BTKSorgu Version: 1.2.21 Summary: Hedef
-websitesinin BTK TarafÄ±ndan EriÅim Engeli Sorgusu Home-page: https://
-github.com/keyiflerolsun/BTKSorgu Author: keyiflerolsun Author-email:
+Metadata-Version: 2.1 Name: BTKSorgu Version: 1.2.3 Summary: Hedef websitesinin
+BTK TarafÄ±ndan EriÅim Engeli Sorgusu Home-page: https://github.com/
+keyiflerolsun/BTKSorgu Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 BTKSorgu,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
 LICENSE # [https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/
 Shared/org.KekikAkademi.BTKSorgu.svg] BTKSorgu [![Boyut](https://
```

### Comparing `BTKSorgu-1.2.21/README.md` & `BTKSorgu-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.2.21/Shared/org.KekikAkademi.BTKSorgu.appdata.xml` & `BTKSorgu-1.2.3/Shared/org.KekikAkademi.BTKSorgu.appdata.xml`

 * *Files 3% similar despite different names*

#### Comparing `BTKSorgu-1.2.21/Shared/org.KekikAkademi.BTKSorgu.appdata.xml` & `BTKSorgu-1.2.3/Shared/org.KekikAkademi.BTKSorgu.appdata.xml`

```diff
@@ -28,14 +28,19 @@
       <image>https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/SS.png</image>
     </screenshot>
   </screenshots>
   <categories>
     <category>Education</category>
   </categories>
   <releases>
+    <release version="1.2.3" date="2023-5-20">
+      <description>
+        <p>`tess_yukle()` fonksiyonu eklendi..</p>
+      </description>
+    </release>
     <release version="1.2.2" date="2023-5-20">
       <description>
         <p>Tk Tabanı Güncellendi..</p>
       </description>
     </release>
     <release version="1.1.8" date="2023-5-19">
       <description>
```

### Comparing `BTKSorgu-1.2.21/Shared/org.KekikAkademi.BTKSorgu.svg` & `BTKSorgu-1.2.3/Shared/org.KekikAkademi.BTKSorgu.svg`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.2.21/setup.py` & `BTKSorgu-1.2.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # Bu araç @keyiflerolsun tarafından | @KekikAkademi için yazılmıştır.
 
 from setuptools import setup
 from io         import open
+from tess_yukle import TesseractYukle
 
 setup(
     # ? Genel Bilgiler
     name         = "BTKSorgu",
-    version      = "1.2.21",
+    version      = "1.2.3",
     url          = "https://github.com/keyiflerolsun/BTKSorgu",
     description  = "Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu",
     keywords     = ["BTKSorgu", "KekikAkademi", "keyiflerolsun"],
 
     author       = "keyiflerolsun",
     author_email = "keyiflerolsun@gmail.com",
 
@@ -53,9 +54,14 @@
         ("share/appdata",                     ["Shared/org.KekikAkademi.BTKSorgu.appdata.xml"]),
         ("share/icons/hicolor/scalable/apps", ["Shared/org.KekikAkademi.BTKSorgu.svg"])
     ],
 
     # ? PyPI Bilgileri
     long_description_content_type = "text/markdown",
     long_description              = "".join(open("README.md", encoding="utf-8").readlines()),
-    include_package_data          = True
-)
+    include_package_data          = True,
+
+    # ? Dışarıdan Yüklenenler
+    cmdclass = {
+        "install" : TesseractYukle
+    }
+)
```

