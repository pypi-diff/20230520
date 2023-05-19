# Comparing `tmp/BTKSorgu-1.2.1.tar.gz` & `tmp/BTKSorgu-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BTKSorgu-1.2.1.tar", last modified: Fri May 19 23:08:09 2023, max compression
+gzip compressed data, was "BTKSorgu-1.2.2.tar", last modified: Fri May 19 23:32:40 2023, max compression
```

## Comparing `BTKSorgu-1.2.1.tar` & `BTKSorgu-1.2.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 23:08:09.763294 BTKSorgu-1.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 23:08:09.759294 BTKSorgu-1.2.1/BTKSorgu/
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-19 23:07:45.000000 BTKSorgu-1.2.1/BTKSorgu/Erisim_Engeli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-05-19 23:07:45.000000 BTKSorgu-1.2.1/BTKSorgu/KekikGUI.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-19 23:07:45.000000 BTKSorgu-1.2.1/BTKSorgu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 23:07:45.000000 BTKSorgu-1.2.1/BTKSorgu/arayuz.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-19 23:07:45.000000 BTKSorgu-1.2.1/BTKSorgu/ekstra.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-19 23:07:45.000000 BTKSorgu-1.2.1/BTKSorgu/konsol.py
--rw-r--r--   0 runner    (1001) docker     (123)    15717 2023-05-19 23:07:45.000000 BTKSorgu-1.2.1/BTKSorgu/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 23:08:09.759294 BTKSorgu-1.2.1/BTKSorgu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8567 2023-05-19 23:08:09.000000 BTKSorgu-1.2.1/BTKSorgu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-19 23:08:09.000000 BTKSorgu-1.2.1/BTKSorgu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 23:08:09.000000 BTKSorgu-1.2.1/BTKSorgu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-19 23:08:09.000000 BTKSorgu-1.2.1/BTKSorgu.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-19 23:08:09.000000 BTKSorgu-1.2.1/BTKSorgu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-19 23:08:09.000000 BTKSorgu-1.2.1/BTKSorgu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-19 23:07:45.000000 BTKSorgu-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-19 23:07:45.000000 BTKSorgu-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8567 2023-05-19 23:08:09.763294 BTKSorgu-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7994 2023-05-19 23:07:45.000000 BTKSorgu-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 23:08:09.759294 BTKSorgu-1.2.1/Shared/
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-05-19 23:07:45.000000 BTKSorgu-1.2.1/Shared/org.KekikAkademi.BTKSorgu.appdata.xml
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-19 23:07:45.000000 BTKSorgu-1.2.1/Shared/org.KekikAkademi.BTKSorgu.desktop
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-19 23:07:45.000000 BTKSorgu-1.2.1/Shared/org.KekikAkademi.BTKSorgu.svg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 23:08:09.763294 BTKSorgu-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-19 23:07:45.000000 BTKSorgu-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 23:32:40.100299 BTKSorgu-1.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 23:32:40.100299 BTKSorgu-1.2.2/BTKSorgu/
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-19 23:32:17.000000 BTKSorgu-1.2.2/BTKSorgu/Erisim_Engeli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-05-19 23:32:17.000000 BTKSorgu-1.2.2/BTKSorgu/KekikGUI.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-19 23:32:17.000000 BTKSorgu-1.2.2/BTKSorgu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 23:32:17.000000 BTKSorgu-1.2.2/BTKSorgu/arayuz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-19 23:32:17.000000 BTKSorgu-1.2.2/BTKSorgu/ekstra.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-19 23:32:17.000000 BTKSorgu-1.2.2/BTKSorgu/konsol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10945 2023-05-19 23:32:17.000000 BTKSorgu-1.2.2/BTKSorgu/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 23:32:40.100299 BTKSorgu-1.2.2/BTKSorgu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8567 2023-05-19 23:32:39.000000 BTKSorgu-1.2.2/BTKSorgu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-19 23:32:39.000000 BTKSorgu-1.2.2/BTKSorgu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 23:32:39.000000 BTKSorgu-1.2.2/BTKSorgu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-19 23:32:39.000000 BTKSorgu-1.2.2/BTKSorgu.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-19 23:32:39.000000 BTKSorgu-1.2.2/BTKSorgu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-19 23:32:39.000000 BTKSorgu-1.2.2/BTKSorgu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-19 23:32:17.000000 BTKSorgu-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-19 23:32:17.000000 BTKSorgu-1.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8567 2023-05-19 23:32:40.100299 BTKSorgu-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7994 2023-05-19 23:32:17.000000 BTKSorgu-1.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 23:32:40.100299 BTKSorgu-1.2.2/Shared/
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-05-19 23:32:17.000000 BTKSorgu-1.2.2/Shared/org.KekikAkademi.BTKSorgu.appdata.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-19 23:32:17.000000 BTKSorgu-1.2.2/Shared/org.KekikAkademi.BTKSorgu.desktop
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-19 23:32:17.000000 BTKSorgu-1.2.2/Shared/org.KekikAkademi.BTKSorgu.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 23:32:40.100299 BTKSorgu-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-19 23:32:17.000000 BTKSorgu-1.2.2/setup.py
```

### Comparing `BTKSorgu-1.2.1/BTKSorgu/Erisim_Engeli.py` & `BTKSorgu-1.2.2/BTKSorgu/Erisim_Engeli.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.2.1/BTKSorgu/KekikGUI.py` & `BTKSorgu-1.2.2/BTKSorgu/KekikGUI.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.2.1/BTKSorgu/konsol.py` & `BTKSorgu-1.2.2/BTKSorgu/konsol.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.2.1/BTKSorgu.egg-info/PKG-INFO` & `BTKSorgu-1.2.2/BTKSorgu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BTKSorgu
-Version: 1.2.1
+Version: 1.2.2
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
-Metadata-Version: 2.1 Name: BTKSorgu Version: 1.2.1 Summary: Hedef websitesinin
+Metadata-Version: 2.1 Name: BTKSorgu Version: 1.2.2 Summary: Hedef websitesinin
 BTK TarafÄ±ndan EriÅim Engeli Sorgusu Home-page: https://github.com/
 keyiflerolsun/BTKSorgu Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 BTKSorgu,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
```

### Comparing `BTKSorgu-1.2.1/LICENSE` & `BTKSorgu-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.2.1/PKG-INFO` & `BTKSorgu-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BTKSorgu
-Version: 1.2.1
+Version: 1.2.2
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
-Metadata-Version: 2.1 Name: BTKSorgu Version: 1.2.1 Summary: Hedef websitesinin
+Metadata-Version: 2.1 Name: BTKSorgu Version: 1.2.2 Summary: Hedef websitesinin
 BTK TarafÄ±ndan EriÅim Engeli Sorgusu Home-page: https://github.com/
 keyiflerolsun/BTKSorgu Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 BTKSorgu,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
```

### Comparing `BTKSorgu-1.2.1/README.md` & `BTKSorgu-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.2.1/Shared/org.KekikAkademi.BTKSorgu.appdata.xml` & `BTKSorgu-1.2.2/Shared/org.KekikAkademi.BTKSorgu.appdata.xml`

 * *Files 1% similar despite different names*

#### Comparing `BTKSorgu-1.2.1/Shared/org.KekikAkademi.BTKSorgu.appdata.xml` & `BTKSorgu-1.2.2/Shared/org.KekikAkademi.BTKSorgu.appdata.xml`

```diff
@@ -28,15 +28,15 @@
       <image>https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/SS.png</image>
     </screenshot>
   </screenshots>
   <categories>
     <category>Education</category>
   </categories>
   <releases>
-    <release version="1.2.1" date="2023-5-20">
+    <release version="1.2.2" date="2023-5-20">
       <description>
         <p>Tk Tabanı Güncellendi..</p>
       </description>
     </release>
     <release version="1.1.8" date="2023-5-19">
       <description>
         <p>Çeşitli hatalar giderildi..</p>
```

### Comparing `BTKSorgu-1.2.1/Shared/org.KekikAkademi.BTKSorgu.svg` & `BTKSorgu-1.2.2/Shared/org.KekikAkademi.BTKSorgu.svg`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.2.1/setup.py` & `BTKSorgu-1.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 from io         import open
 
 setup(
     # ? Genel Bilgiler
     name         = "BTKSorgu",
-    version      = "1.2.1",
+    version      = "1.2.2",
     url          = "https://github.com/keyiflerolsun/BTKSorgu",
     description  = "Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu",
     keywords     = ["BTKSorgu", "KekikAkademi", "keyiflerolsun"],
 
     author       = "keyiflerolsun",
     author_email = "keyiflerolsun@gmail.com",
```

