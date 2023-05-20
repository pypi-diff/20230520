# Comparing `tmp/BTKSorgu-1.2.8.tar.gz` & `tmp/BTKSorgu-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BTKSorgu-1.2.8.tar", last modified: Sat May 20 19:31:22 2023, max compression
+gzip compressed data, was "BTKSorgu-1.2.9.tar", last modified: Sat May 20 21:15:05 2023, max compression
```

## Comparing `BTKSorgu-1.2.8.tar` & `BTKSorgu-1.2.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:31:22.152994 BTKSorgu-1.2.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:31:22.152994 BTKSorgu-1.2.8/BTKSorgu/
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-20 19:30:35.000000 BTKSorgu-1.2.8/BTKSorgu/Erisim_Engeli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-05-20 19:30:35.000000 BTKSorgu-1.2.8/BTKSorgu/KekikGUI.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-20 19:30:35.000000 BTKSorgu-1.2.8/BTKSorgu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-20 19:30:35.000000 BTKSorgu-1.2.8/BTKSorgu/arayuz.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-20 19:30:35.000000 BTKSorgu-1.2.8/BTKSorgu/ekstra.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-20 19:30:35.000000 BTKSorgu-1.2.8/BTKSorgu/konsol.py
--rw-r--r--   0 runner    (1001) docker     (123)    10945 2023-05-20 19:30:35.000000 BTKSorgu-1.2.8/BTKSorgu/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:31:22.152994 BTKSorgu-1.2.8/BTKSorgu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9061 2023-05-20 19:30:57.000000 BTKSorgu-1.2.8/BTKSorgu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-20 19:30:57.000000 BTKSorgu-1.2.8/BTKSorgu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 19:30:57.000000 BTKSorgu-1.2.8/BTKSorgu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-20 19:30:57.000000 BTKSorgu-1.2.8/BTKSorgu.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-20 19:30:57.000000 BTKSorgu-1.2.8/BTKSorgu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-20 19:30:57.000000 BTKSorgu-1.2.8/BTKSorgu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-20 19:30:35.000000 BTKSorgu-1.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-20 19:30:35.000000 BTKSorgu-1.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9061 2023-05-20 19:31:22.152994 BTKSorgu-1.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-05-20 19:30:35.000000 BTKSorgu-1.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:31:22.152994 BTKSorgu-1.2.8/Shared/
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-05-20 19:30:35.000000 BTKSorgu-1.2.8/Shared/org.KekikAkademi.BTKSorgu.appdata.xml
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-20 19:30:35.000000 BTKSorgu-1.2.8/Shared/org.KekikAkademi.BTKSorgu.desktop
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-20 19:30:35.000000 BTKSorgu-1.2.8/Shared/org.KekikAkademi.BTKSorgu.svg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 19:31:22.152994 BTKSorgu-1.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-20 19:30:35.000000 BTKSorgu-1.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 21:15:05.226631 BTKSorgu-1.2.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 21:15:05.226631 BTKSorgu-1.2.9/BTKSorgu/
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-20 21:14:10.000000 BTKSorgu-1.2.9/BTKSorgu/Erisim_Engeli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-05-20 21:14:10.000000 BTKSorgu-1.2.9/BTKSorgu/KekikGUI.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-20 21:14:10.000000 BTKSorgu-1.2.9/BTKSorgu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-20 21:14:10.000000 BTKSorgu-1.2.9/BTKSorgu/arayuz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-20 21:14:10.000000 BTKSorgu-1.2.9/BTKSorgu/ekstra.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-20 21:14:10.000000 BTKSorgu-1.2.9/BTKSorgu/konsol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10945 2023-05-20 21:14:10.000000 BTKSorgu-1.2.9/BTKSorgu/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 21:15:05.226631 BTKSorgu-1.2.9/BTKSorgu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9061 2023-05-20 21:14:30.000000 BTKSorgu-1.2.9/BTKSorgu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-20 21:14:30.000000 BTKSorgu-1.2.9/BTKSorgu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 21:14:30.000000 BTKSorgu-1.2.9/BTKSorgu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-20 21:14:30.000000 BTKSorgu-1.2.9/BTKSorgu.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-20 21:14:30.000000 BTKSorgu-1.2.9/BTKSorgu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-20 21:14:30.000000 BTKSorgu-1.2.9/BTKSorgu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-20 21:14:10.000000 BTKSorgu-1.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-20 21:14:10.000000 BTKSorgu-1.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9061 2023-05-20 21:15:05.226631 BTKSorgu-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-05-20 21:14:10.000000 BTKSorgu-1.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 21:15:05.226631 BTKSorgu-1.2.9/Shared/
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-05-20 21:14:10.000000 BTKSorgu-1.2.9/Shared/org.KekikAkademi.BTKSorgu.appdata.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-20 21:14:10.000000 BTKSorgu-1.2.9/Shared/org.KekikAkademi.BTKSorgu.desktop
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-20 21:14:10.000000 BTKSorgu-1.2.9/Shared/org.KekikAkademi.BTKSorgu.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 21:15:05.226631 BTKSorgu-1.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-20 21:14:10.000000 BTKSorgu-1.2.9/setup.py
```

### Comparing `BTKSorgu-1.2.8/BTKSorgu/Erisim_Engeli.py` & `BTKSorgu-1.2.9/BTKSorgu/Erisim_Engeli.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.2.8/BTKSorgu/KekikGUI.py` & `BTKSorgu-1.2.9/BTKSorgu/KekikGUI.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.2.8/BTKSorgu/konsol.py` & `BTKSorgu-1.2.9/BTKSorgu/konsol.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.2.8/BTKSorgu/logo.png` & `BTKSorgu-1.2.9/BTKSorgu/logo.png`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.2.8/BTKSorgu.egg-info/PKG-INFO` & `BTKSorgu-1.2.9/BTKSorgu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BTKSorgu
-Version: 1.2.8
+Version: 1.2.9
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
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: BTKSorgu Version: 1.2.8 Summary: Hedef websitesinin
+Metadata-Version: 2.1 Name: BTKSorgu Version: 1.2.9 Summary: Hedef websitesinin
 BTK TarafÄ±ndan EriÅim Engeli Sorgusu Home-page: https://github.com/
 keyiflerolsun/BTKSorgu Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 BTKSorgu,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
```

### Comparing `BTKSorgu-1.2.8/LICENSE` & `BTKSorgu-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.2.8/PKG-INFO` & `BTKSorgu-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BTKSorgu
-Version: 1.2.8
+Version: 1.2.9
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
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: BTKSorgu Version: 1.2.8 Summary: Hedef websitesinin
+Metadata-Version: 2.1 Name: BTKSorgu Version: 1.2.9 Summary: Hedef websitesinin
 BTK TarafÄ±ndan EriÅim Engeli Sorgusu Home-page: https://github.com/
 keyiflerolsun/BTKSorgu Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 BTKSorgu,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
```

### Comparing `BTKSorgu-1.2.8/README.md` & `BTKSorgu-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.2.8/Shared/org.KekikAkademi.BTKSorgu.appdata.xml` & `BTKSorgu-1.2.9/Shared/org.KekikAkademi.BTKSorgu.appdata.xml`

 * *Files 1% similar despite different names*

#### Comparing `BTKSorgu-1.2.8/Shared/org.KekikAkademi.BTKSorgu.appdata.xml` & `BTKSorgu-1.2.9/Shared/org.KekikAkademi.BTKSorgu.appdata.xml`

```diff
@@ -28,15 +28,15 @@
       <image>https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/SS.png</image>
     </screenshot>
   </screenshots>
   <categories>
     <category>Education</category>
   </categories>
   <releases>
-    <release version="1.2.8" date="2023-5-20">
+    <release version="1.2.9" date="2023-5-20">
       <description>
         <p>`tess_yukle()` fonksiyonu eklendi..</p>
       </description>
     </release>
     <release version="1.2.2" date="2023-5-20">
       <description>
         <p>Tk Tabanı Güncellendi..</p>
```

### Comparing `BTKSorgu-1.2.8/Shared/org.KekikAkademi.BTKSorgu.svg` & `BTKSorgu-1.2.9/Shared/org.KekikAkademi.BTKSorgu.svg`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.2.8/setup.py` & `BTKSorgu-1.2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 from io         import open
 from tess_yukle import TesseractYukle
 
 setup(
     # ? Genel Bilgiler
     name         = "BTKSorgu",
-    version      = "1.2.8",
+    version      = "1.2.9",
     url          = "https://github.com/keyiflerolsun/BTKSorgu",
     description  = "Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu",
     keywords     = ["BTKSorgu", "KekikAkademi", "keyiflerolsun"],
 
     author       = "keyiflerolsun",
     author_email = "keyiflerolsun@gmail.com",
 
@@ -35,14 +35,19 @@
         "cssselect",
         "regex",
         "Pillow",
         "pytesseract",
         "sv_ttk"
     ],
 
+    # ? Dışarıdan Yüklenenler
+    cmdclass = {
+        "install" : TesseractYukle
+    },
+
     # ? Konsoldan Çalıştırılabilir
     entry_points = {
         "console_scripts": [
             "BTKSorgu    = BTKSorgu.konsol:basla",
             "BTKSorguGUI = BTKSorgu.arayuz:basla"
         ]
     },
@@ -54,14 +59,9 @@
         ("share/appdata",                     ["Shared/org.KekikAkademi.BTKSorgu.appdata.xml"]),
         ("share/icons/hicolor/scalable/apps", ["Shared/org.KekikAkademi.BTKSorgu.svg"])
     ],
 
     # ? PyPI Bilgileri
     long_description_content_type = "text/markdown",
     long_description              = "".join(open("README.md", encoding="utf-8").readlines()),
-    include_package_data          = True,
-
-    # ? Dışarıdan Yüklenenler
-    cmdclass = {
-        "install" : TesseractYukle
-    }
+    include_package_data          = True
 )
```

