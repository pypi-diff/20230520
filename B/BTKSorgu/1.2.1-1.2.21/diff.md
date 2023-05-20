# Comparing `tmp/BTKSorgu-1.2.1.tar.gz` & `tmp/BTKSorgu-1.2.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BTKSorgu-1.2.1.tar", last modified: Fri May 19 23:08:09 2023, max compression
+gzip compressed data, was "BTKSorgu-1.2.21.tar", last modified: Sat May 20 12:22:52 2023, max compression
```

## Comparing `BTKSorgu-1.2.1.tar` & `BTKSorgu-1.2.21.tar`

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
+drwxr-xr-x   0 keyiflerolsun  (1000) keyiflerolsun  (1000)        0 2023-05-20 12:22:52.234112 BTKSorgu-1.2.21/
+drwxr-xr-x   0 keyiflerolsun  (1000) keyiflerolsun  (1000)        0 2023-05-20 12:22:52.234112 BTKSorgu-1.2.21/BTKSorgu/
+-rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)     3332 2023-05-20 12:20:31.000000 BTKSorgu-1.2.21/BTKSorgu/Erisim_Engeli.py
+-rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)     4043 2023-05-20 12:20:31.000000 BTKSorgu-1.2.21/BTKSorgu/KekikGUI.py
+-rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)      165 2023-05-20 12:20:31.000000 BTKSorgu-1.2.21/BTKSorgu/__init__.py
+-rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)      159 2023-05-20 12:20:31.000000 BTKSorgu-1.2.21/BTKSorgu/arayuz.py
+-rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)      278 2023-05-20 12:20:31.000000 BTKSorgu-1.2.21/BTKSorgu/ekstra.py
+-rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)      602 2023-05-20 12:20:31.000000 BTKSorgu-1.2.21/BTKSorgu/konsol.py
+-rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)    10945 2023-05-20 12:20:31.000000 BTKSorgu-1.2.21/BTKSorgu/logo.png
+drwxr-xr-x   0 keyiflerolsun  (1000) keyiflerolsun  (1000)        0 2023-05-20 12:22:52.234112 BTKSorgu-1.2.21/BTKSorgu.egg-info/
+-rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)     9062 2023-05-20 12:22:52.000000 BTKSorgu-1.2.21/BTKSorgu.egg-info/PKG-INFO
+-rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)      498 2023-05-20 12:22:52.000000 BTKSorgu-1.2.21/BTKSorgu.egg-info/SOURCES.txt
+-rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)        1 2023-05-20 12:22:52.000000 BTKSorgu-1.2.21/BTKSorgu.egg-info/dependency_links.txt
+-rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)       87 2023-05-20 12:22:52.000000 BTKSorgu-1.2.21/BTKSorgu.egg-info/entry_points.txt
+-rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)      100 2023-05-20 12:22:52.000000 BTKSorgu-1.2.21/BTKSorgu.egg-info/requires.txt
+-rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)        9 2023-05-20 12:22:52.000000 BTKSorgu-1.2.21/BTKSorgu.egg-info/top_level.txt
+-rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)    35149 2023-05-20 12:20:31.000000 BTKSorgu-1.2.21/LICENSE
+-rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)       28 2023-05-20 12:20:31.000000 BTKSorgu-1.2.21/MANIFEST.in
+-rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)     9062 2023-05-20 12:22:52.234112 BTKSorgu-1.2.21/PKG-INFO
+-rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)     8489 2023-05-20 12:20:31.000000 BTKSorgu-1.2.21/README.md
+drwxr-xr-x   0 keyiflerolsun  (1000) keyiflerolsun  (1000)        0 2023-05-20 12:22:52.234112 BTKSorgu-1.2.21/Shared/
+-rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)     2916 2023-05-20 12:20:31.000000 BTKSorgu-1.2.21/Shared/org.KekikAkademi.BTKSorgu.appdata.xml
+-rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)      315 2023-05-20 12:20:31.000000 BTKSorgu-1.2.21/Shared/org.KekikAkademi.BTKSorgu.desktop
+-rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)     1858 2023-05-20 12:20:31.000000 BTKSorgu-1.2.21/Shared/org.KekikAkademi.BTKSorgu.svg
+-rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)       38 2023-05-20 12:22:52.234112 BTKSorgu-1.2.21/setup.cfg
+-rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)     1915 2023-05-20 12:22:32.000000 BTKSorgu-1.2.21/setup.py
```

### Comparing `BTKSorgu-1.2.1/BTKSorgu/Erisim_Engeli.py` & `BTKSorgu-1.2.21/BTKSorgu/Erisim_Engeli.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.2.1/BTKSorgu/KekikGUI.py` & `BTKSorgu-1.2.21/BTKSorgu/KekikGUI.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.2.1/BTKSorgu/konsol.py` & `BTKSorgu-1.2.21/BTKSorgu/konsol.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.2.1/BTKSorgu.egg-info/PKG-INFO` & `BTKSorgu-1.2.21/BTKSorgu.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 Metadata-Version: 2.1
 Name: BTKSorgu
-Version: 1.2.1
+Version: 1.2.21
 Summary: Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu
 Home-page: https://github.com/keyiflerolsun/BTKSorgu
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: BTKSorgu,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# 🔍 BTKSorgu
+# <a href="#"><img width="32" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/Shared/org.KekikAkademi.BTKSorgu.svg"></a> BTKSorgu
 
-[![Repo Boyutu](https://img.shields.io/github/repo-size/keyiflerolsun/BTKSorgu?logo=git&logoColor=white)](#)
+[![Boyut](https://img.shields.io/github/repo-size/keyiflerolsun/BTKSorgu?logo=git&logoColor=white&label=Boyut)](#)
 [![Görüntülenme](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/keyiflerolsun/BTKSorgu&title=Görüntülenme)](#)
 <a href="https://KekikAkademi.org/Kahve" target="_blank"><img src="https://img.shields.io/badge/☕️-Kahve Ismarla-ffdd00" title="☕️ Kahve Ismarla" style="padding-left:5px;"></a>
 
-[![Python Version](https://img.shields.io/pypi/pyversions/BTKSorgu?logo=python&logoColor=white)](#)
-[![License](https://img.shields.io/pypi/l/BTKSorgu?logo=gnu&logoColor=white)](#)
-[![Status](https://img.shields.io/pypi/status/BTKSorgu?logo=windowsterminal&logoColor=white)](#)
-
-[![PyPI](https://img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white)](https://pypi.org/project/BTKSorgu)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/BTKSorgu?logo=pypi&logoColor=white)](https://pypi.org/project/BTKSorgu)
-[![PyPI - Wheel](https://img.shields.io/pypi/wheel/BTKSorgu?logo=pypi&logoColor=white)](https://pypi.org/project/BTKSorgu)
-
-[![PyPI Yükleyici](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/pypiYukle.yml/badge.svg)](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/pypiYukle.yml)
-[![Flatpak Yükleyici](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/flatpakYukle.yml/badge.svg)](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/flatpakYukle.yml)
-
-[![FlatHub](https://img.shields.io/flathub/v/org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white)](https://flathub.org/tr/apps/org.KekikAkademi.BTKSorgu)
-[![FlatHub - Downloads](https://img.shields.io/flathub/downloads/org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white)](https://flathub.org/tr/apps/org.KekikAkademi.BTKSorgu)
+[![GitHub](https://img.shields.io/github/v/release/keyiflerolsun/BTKSorgu?logo=github&label=GitHub)](https://github.com/keyiflerolsun/BTKSorgu/releases)
+[![PyPi Yükleyici](https://img.shields.io/github/actions/workflow/status/keyiflerolsun/BTKSorgu/pypiYukle.yml?label=PyPi%20Y%C3%BCkleyici&logo=github)](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/pypiYukle.yml)
+[![Flatpak Yükleyici](https://img.shields.io/github/actions/workflow/status/keyiflerolsun/BTKSorgu/flatpakYukle.yml?label=Flatpak%20Y%C3%BCkleyici&logo=github)](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/flatpakYukle.yml)
+
+[![FlatHub](https://img.shields.io/flathub/v/org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white&label=FlatHub)](https://flathub.org/tr/apps/org.KekikAkademi.BTKSorgu)
+[![FlatHub - Yüklenme](https://img.shields.io/flathub/downloads/org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white&label=Yüklenme)](https://flathub.org/tr/apps/org.KekikAkademi.BTKSorgu)
+
+[![PyPi](https://img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white&label=PyPi)](https://pypi.org/project/BTKSorgu)
+[![PyPi - Yüklenme](https://img.shields.io/pypi/dm/BTKSorgu?logo=pypi&logoColor=white&label=Yüklenme)](https://pypi.org/project/BTKSorgu)
+[![PyPi - Wheel](https://img.shields.io/pypi/wheel/BTKSorgu?logo=pypi&logoColor=white&label=Wheel)](https://pypi.org/project/BTKSorgu)
+
+[![Python Version](https://img.shields.io/pypi/pyversions/BTKSorgu?logo=python&logoColor=white&label=Python)](#)
+[![Lisans](https://img.shields.io/pypi/l/BTKSorgu?logo=gnu&logoColor=white&label=Lisans)](#)
+[![Durum](https://img.shields.io/pypi/status/BTKSorgu?logo=windowsterminal&logoColor=white&label=Durum)](#)
 
 *Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu..*
 
 [![BTKSorgu](https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/SS.png)](#)
 
 [![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
```

#### html2text {}

```diff
@@ -1,45 +1,53 @@
-Metadata-Version: 2.1 Name: BTKSorgu Version: 1.2.1 Summary: Hedef websitesinin
-BTK TarafÄ±ndan EriÅim Engeli Sorgusu Home-page: https://github.com/
-keyiflerolsun/BTKSorgu Author: keyiflerolsun Author-email:
+Metadata-Version: 2.1 Name: BTKSorgu Version: 1.2.21 Summary: Hedef
+websitesinin BTK TarafÄ±ndan EriÅim Engeli Sorgusu Home-page: https://
+github.com/keyiflerolsun/BTKSorgu Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 BTKSorgu,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
-LICENSE # ð BTKSorgu [![Repo Boyutu](https://img.shields.io/github/repo-
-size/keyiflerolsun/BTKSorgu?logo=git&logoColor=white)](#) [![GÃ¶rÃ¼ntÃ¼lenme]
-(https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/
+LICENSE # [https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/
+Shared/org.KekikAkademi.BTKSorgu.svg] BTKSorgu [![Boyut](https://
+img.shields.io/github/repo-size/keyiflerolsun/
+BTKSorgu?logo=git&logoColor=white&label=Boyut)](#) [![GÃ¶rÃ¼ntÃ¼lenme](https://
+hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/
 keyiflerolsun/BTKSorgu&title=GÃ¶rÃ¼ntÃ¼lenme)](#) [https://img.shields.io/
-badge/âï¸-Kahve_Ismarla-ffdd00] [![Python Version](https://img.shields.io/
-pypi/pyversions/BTKSorgu?logo=python&logoColor=white)](#) [![License](https://
-img.shields.io/pypi/l/BTKSorgu?logo=gnu&logoColor=white)](#) [![Status](https:/
-/img.shields.io/pypi/status/BTKSorgu?logo=windowsterminal&logoColor=white)](#)
-[![PyPI](https://img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white)]
-(https://pypi.org/project/BTKSorgu) [![PyPI - Downloads](https://
-img.shields.io/pypi/dm/BTKSorgu?logo=pypi&logoColor=white)](https://pypi.org/
-project/BTKSorgu) [![PyPI - Wheel](https://img.shields.io/pypi/wheel/
-BTKSorgu?logo=pypi&logoColor=white)](https://pypi.org/project/BTKSorgu) [![PyPI
-YÃ¼kleyici](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/
-pypiYukle.yml/badge.svg)](https://github.com/keyiflerolsun/BTKSorgu/actions/
-workflows/pypiYukle.yml) [![Flatpak YÃ¼kleyici](https://github.com/
-keyiflerolsun/BTKSorgu/actions/workflows/flatpakYukle.yml/badge.svg)](https://
+badge/âï¸-Kahve_Ismarla-ffdd00] [![GitHub](https://img.shields.io/github/v/
+release/keyiflerolsun/BTKSorgu?logo=github&label=GitHub)](https://github.com/
+keyiflerolsun/BTKSorgu/releases) [![PyPi YÃ¼kleyici](https://img.shields.io/
+github/actions/workflow/status/keyiflerolsun/BTKSorgu/
+pypiYukle.yml?label=PyPi%20Y%C3%BCkleyici&logo=github)](https://github.com/
+keyiflerolsun/BTKSorgu/actions/workflows/pypiYukle.yml) [![Flatpak YÃ¼kleyici]
+(https://img.shields.io/github/actions/workflow/status/keyiflerolsun/BTKSorgu/
+flatpakYukle.yml?label=Flatpak%20Y%C3%BCkleyici&logo=github)](https://
 github.com/keyiflerolsun/BTKSorgu/actions/workflows/flatpakYukle.yml) [!
 [FlatHub](https://img.shields.io/flathub/v/
-org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white)](https://flathub.org/
-tr/apps/org.KekikAkademi.BTKSorgu) [![FlatHub - Downloads](https://
+org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white&label=FlatHub)](https://
+flathub.org/tr/apps/org.KekikAkademi.BTKSorgu) [![FlatHub - YÃ¼klenme](https://
 img.shields.io/flathub/downloads/
-org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white)](https://flathub.org/
-tr/apps/org.KekikAkademi.BTKSorgu) *Hedef websitesinin BTK TarafÄ±ndan EriÅim
-Engeli Sorgusu..* [![BTKSorgu](https://raw.githubusercontent.com/keyiflerolsun/
-BTKSorgu/main/.github/icons/SS.png)](#) [![ForTheBadge made-with-python](https:
-//ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/
-) [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-
-with-love.svg)](https://GitHub.com/keyiflerolsun/) ## ð Kurulum ### [https:/
-/raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/pypi.svg]
+org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white&label=YÃ¼klenme)](https:
+//flathub.org/tr/apps/org.KekikAkademi.BTKSorgu) [![PyPi](https://
+img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white&label=PyPi)](https://
+pypi.org/project/BTKSorgu) [![PyPi - YÃ¼klenme](https://img.shields.io/pypi/dm/
+BTKSorgu?logo=pypi&logoColor=white&label=YÃ¼klenme)](https://pypi.org/project/
+BTKSorgu) [![PyPi - Wheel](https://img.shields.io/pypi/wheel/
+BTKSorgu?logo=pypi&logoColor=white&label=Wheel)](https://pypi.org/project/
+BTKSorgu) [![Python Version](https://img.shields.io/pypi/pyversions/
+BTKSorgu?logo=python&logoColor=white&label=Python)](#) [![Lisans](https://
+img.shields.io/pypi/l/BTKSorgu?logo=gnu&logoColor=white&label=Lisans)](#) [!
+[Durum](https://img.shields.io/pypi/status/
+BTKSorgu?logo=windowsterminal&logoColor=white&label=Durum)](#) *Hedef
+websitesinin BTK TarafÄ±ndan EriÅim Engeli Sorgusu..* [![BTKSorgu](https://
+raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/SS.png)](#)
+[![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-
+with-python.svg)](https://www.python.org/) [![ForTheBadge built-with-love]
+(https://ForTheBadge.com/images/badges/built-with-love.svg)](https://
+GitHub.com/keyiflerolsun/) ## ð Kurulum ### [https://
+raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/pypi.svg]
 PyPi (Lib - CLI - UI) ```bash # YÃ¼klemek pip install BTKSorgu # GÃ¼ncellemek
 pip install -U BTKSorgu ``` ### [https://raw.githubusercontent.com/
 keyiflerolsun/BTKSorgu/main/.github/icons/flathub.svg] FlatHub (UI) ```bash #
 YÃ¼klemek flatpak install flathub org.KekikAkademi.BTKSorgu # ÃalÄ±ÅtÄ±rmak
 flatpak run org.KekikAkademi.BTKSorgu ``` ## ð KullanÄ±m ### [https://
 raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/python.svg]
 Lib ```python from BTKSorgu import BTKSorgu from time import time basla = time
```

### Comparing `BTKSorgu-1.2.1/LICENSE` & `BTKSorgu-1.2.21/LICENSE`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.2.1/PKG-INFO` & `BTKSorgu-1.2.21/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 Metadata-Version: 2.1
 Name: BTKSorgu
-Version: 1.2.1
+Version: 1.2.21
 Summary: Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu
 Home-page: https://github.com/keyiflerolsun/BTKSorgu
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: BTKSorgu,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# 🔍 BTKSorgu
+# <a href="#"><img width="32" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/Shared/org.KekikAkademi.BTKSorgu.svg"></a> BTKSorgu
 
-[![Repo Boyutu](https://img.shields.io/github/repo-size/keyiflerolsun/BTKSorgu?logo=git&logoColor=white)](#)
+[![Boyut](https://img.shields.io/github/repo-size/keyiflerolsun/BTKSorgu?logo=git&logoColor=white&label=Boyut)](#)
 [![Görüntülenme](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/keyiflerolsun/BTKSorgu&title=Görüntülenme)](#)
 <a href="https://KekikAkademi.org/Kahve" target="_blank"><img src="https://img.shields.io/badge/☕️-Kahve Ismarla-ffdd00" title="☕️ Kahve Ismarla" style="padding-left:5px;"></a>
 
-[![Python Version](https://img.shields.io/pypi/pyversions/BTKSorgu?logo=python&logoColor=white)](#)
-[![License](https://img.shields.io/pypi/l/BTKSorgu?logo=gnu&logoColor=white)](#)
-[![Status](https://img.shields.io/pypi/status/BTKSorgu?logo=windowsterminal&logoColor=white)](#)
-
-[![PyPI](https://img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white)](https://pypi.org/project/BTKSorgu)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/BTKSorgu?logo=pypi&logoColor=white)](https://pypi.org/project/BTKSorgu)
-[![PyPI - Wheel](https://img.shields.io/pypi/wheel/BTKSorgu?logo=pypi&logoColor=white)](https://pypi.org/project/BTKSorgu)
-
-[![PyPI Yükleyici](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/pypiYukle.yml/badge.svg)](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/pypiYukle.yml)
-[![Flatpak Yükleyici](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/flatpakYukle.yml/badge.svg)](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/flatpakYukle.yml)
-
-[![FlatHub](https://img.shields.io/flathub/v/org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white)](https://flathub.org/tr/apps/org.KekikAkademi.BTKSorgu)
-[![FlatHub - Downloads](https://img.shields.io/flathub/downloads/org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white)](https://flathub.org/tr/apps/org.KekikAkademi.BTKSorgu)
+[![GitHub](https://img.shields.io/github/v/release/keyiflerolsun/BTKSorgu?logo=github&label=GitHub)](https://github.com/keyiflerolsun/BTKSorgu/releases)
+[![PyPi Yükleyici](https://img.shields.io/github/actions/workflow/status/keyiflerolsun/BTKSorgu/pypiYukle.yml?label=PyPi%20Y%C3%BCkleyici&logo=github)](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/pypiYukle.yml)
+[![Flatpak Yükleyici](https://img.shields.io/github/actions/workflow/status/keyiflerolsun/BTKSorgu/flatpakYukle.yml?label=Flatpak%20Y%C3%BCkleyici&logo=github)](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/flatpakYukle.yml)
+
+[![FlatHub](https://img.shields.io/flathub/v/org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white&label=FlatHub)](https://flathub.org/tr/apps/org.KekikAkademi.BTKSorgu)
+[![FlatHub - Yüklenme](https://img.shields.io/flathub/downloads/org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white&label=Yüklenme)](https://flathub.org/tr/apps/org.KekikAkademi.BTKSorgu)
+
+[![PyPi](https://img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white&label=PyPi)](https://pypi.org/project/BTKSorgu)
+[![PyPi - Yüklenme](https://img.shields.io/pypi/dm/BTKSorgu?logo=pypi&logoColor=white&label=Yüklenme)](https://pypi.org/project/BTKSorgu)
+[![PyPi - Wheel](https://img.shields.io/pypi/wheel/BTKSorgu?logo=pypi&logoColor=white&label=Wheel)](https://pypi.org/project/BTKSorgu)
+
+[![Python Version](https://img.shields.io/pypi/pyversions/BTKSorgu?logo=python&logoColor=white&label=Python)](#)
+[![Lisans](https://img.shields.io/pypi/l/BTKSorgu?logo=gnu&logoColor=white&label=Lisans)](#)
+[![Durum](https://img.shields.io/pypi/status/BTKSorgu?logo=windowsterminal&logoColor=white&label=Durum)](#)
 
 *Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu..*
 
 [![BTKSorgu](https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/SS.png)](#)
 
 [![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
```

#### html2text {}

```diff
@@ -1,45 +1,53 @@
-Metadata-Version: 2.1 Name: BTKSorgu Version: 1.2.1 Summary: Hedef websitesinin
-BTK TarafÄ±ndan EriÅim Engeli Sorgusu Home-page: https://github.com/
-keyiflerolsun/BTKSorgu Author: keyiflerolsun Author-email:
+Metadata-Version: 2.1 Name: BTKSorgu Version: 1.2.21 Summary: Hedef
+websitesinin BTK TarafÄ±ndan EriÅim Engeli Sorgusu Home-page: https://
+github.com/keyiflerolsun/BTKSorgu Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 BTKSorgu,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
-LICENSE # ð BTKSorgu [![Repo Boyutu](https://img.shields.io/github/repo-
-size/keyiflerolsun/BTKSorgu?logo=git&logoColor=white)](#) [![GÃ¶rÃ¼ntÃ¼lenme]
-(https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/
+LICENSE # [https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/
+Shared/org.KekikAkademi.BTKSorgu.svg] BTKSorgu [![Boyut](https://
+img.shields.io/github/repo-size/keyiflerolsun/
+BTKSorgu?logo=git&logoColor=white&label=Boyut)](#) [![GÃ¶rÃ¼ntÃ¼lenme](https://
+hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/
 keyiflerolsun/BTKSorgu&title=GÃ¶rÃ¼ntÃ¼lenme)](#) [https://img.shields.io/
-badge/âï¸-Kahve_Ismarla-ffdd00] [![Python Version](https://img.shields.io/
-pypi/pyversions/BTKSorgu?logo=python&logoColor=white)](#) [![License](https://
-img.shields.io/pypi/l/BTKSorgu?logo=gnu&logoColor=white)](#) [![Status](https:/
-/img.shields.io/pypi/status/BTKSorgu?logo=windowsterminal&logoColor=white)](#)
-[![PyPI](https://img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white)]
-(https://pypi.org/project/BTKSorgu) [![PyPI - Downloads](https://
-img.shields.io/pypi/dm/BTKSorgu?logo=pypi&logoColor=white)](https://pypi.org/
-project/BTKSorgu) [![PyPI - Wheel](https://img.shields.io/pypi/wheel/
-BTKSorgu?logo=pypi&logoColor=white)](https://pypi.org/project/BTKSorgu) [![PyPI
-YÃ¼kleyici](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/
-pypiYukle.yml/badge.svg)](https://github.com/keyiflerolsun/BTKSorgu/actions/
-workflows/pypiYukle.yml) [![Flatpak YÃ¼kleyici](https://github.com/
-keyiflerolsun/BTKSorgu/actions/workflows/flatpakYukle.yml/badge.svg)](https://
+badge/âï¸-Kahve_Ismarla-ffdd00] [![GitHub](https://img.shields.io/github/v/
+release/keyiflerolsun/BTKSorgu?logo=github&label=GitHub)](https://github.com/
+keyiflerolsun/BTKSorgu/releases) [![PyPi YÃ¼kleyici](https://img.shields.io/
+github/actions/workflow/status/keyiflerolsun/BTKSorgu/
+pypiYukle.yml?label=PyPi%20Y%C3%BCkleyici&logo=github)](https://github.com/
+keyiflerolsun/BTKSorgu/actions/workflows/pypiYukle.yml) [![Flatpak YÃ¼kleyici]
+(https://img.shields.io/github/actions/workflow/status/keyiflerolsun/BTKSorgu/
+flatpakYukle.yml?label=Flatpak%20Y%C3%BCkleyici&logo=github)](https://
 github.com/keyiflerolsun/BTKSorgu/actions/workflows/flatpakYukle.yml) [!
 [FlatHub](https://img.shields.io/flathub/v/
-org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white)](https://flathub.org/
-tr/apps/org.KekikAkademi.BTKSorgu) [![FlatHub - Downloads](https://
+org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white&label=FlatHub)](https://
+flathub.org/tr/apps/org.KekikAkademi.BTKSorgu) [![FlatHub - YÃ¼klenme](https://
 img.shields.io/flathub/downloads/
-org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white)](https://flathub.org/
-tr/apps/org.KekikAkademi.BTKSorgu) *Hedef websitesinin BTK TarafÄ±ndan EriÅim
-Engeli Sorgusu..* [![BTKSorgu](https://raw.githubusercontent.com/keyiflerolsun/
-BTKSorgu/main/.github/icons/SS.png)](#) [![ForTheBadge made-with-python](https:
-//ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/
-) [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-
-with-love.svg)](https://GitHub.com/keyiflerolsun/) ## ð Kurulum ### [https:/
-/raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/pypi.svg]
+org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white&label=YÃ¼klenme)](https:
+//flathub.org/tr/apps/org.KekikAkademi.BTKSorgu) [![PyPi](https://
+img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white&label=PyPi)](https://
+pypi.org/project/BTKSorgu) [![PyPi - YÃ¼klenme](https://img.shields.io/pypi/dm/
+BTKSorgu?logo=pypi&logoColor=white&label=YÃ¼klenme)](https://pypi.org/project/
+BTKSorgu) [![PyPi - Wheel](https://img.shields.io/pypi/wheel/
+BTKSorgu?logo=pypi&logoColor=white&label=Wheel)](https://pypi.org/project/
+BTKSorgu) [![Python Version](https://img.shields.io/pypi/pyversions/
+BTKSorgu?logo=python&logoColor=white&label=Python)](#) [![Lisans](https://
+img.shields.io/pypi/l/BTKSorgu?logo=gnu&logoColor=white&label=Lisans)](#) [!
+[Durum](https://img.shields.io/pypi/status/
+BTKSorgu?logo=windowsterminal&logoColor=white&label=Durum)](#) *Hedef
+websitesinin BTK TarafÄ±ndan EriÅim Engeli Sorgusu..* [![BTKSorgu](https://
+raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/SS.png)](#)
+[![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-
+with-python.svg)](https://www.python.org/) [![ForTheBadge built-with-love]
+(https://ForTheBadge.com/images/badges/built-with-love.svg)](https://
+GitHub.com/keyiflerolsun/) ## ð Kurulum ### [https://
+raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/pypi.svg]
 PyPi (Lib - CLI - UI) ```bash # YÃ¼klemek pip install BTKSorgu # GÃ¼ncellemek
 pip install -U BTKSorgu ``` ### [https://raw.githubusercontent.com/
 keyiflerolsun/BTKSorgu/main/.github/icons/flathub.svg] FlatHub (UI) ```bash #
 YÃ¼klemek flatpak install flathub org.KekikAkademi.BTKSorgu # ÃalÄ±ÅtÄ±rmak
 flatpak run org.KekikAkademi.BTKSorgu ``` ## ð KullanÄ±m ### [https://
 raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/python.svg]
 Lib ```python from BTKSorgu import BTKSorgu from time import time basla = time
```

### Comparing `BTKSorgu-1.2.1/README.md` & `BTKSorgu-1.2.21/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-# 🔍 BTKSorgu
+# <a href="#"><img width="32" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/Shared/org.KekikAkademi.BTKSorgu.svg"></a> BTKSorgu
 
-[![Repo Boyutu](https://img.shields.io/github/repo-size/keyiflerolsun/BTKSorgu?logo=git&logoColor=white)](#)
+[![Boyut](https://img.shields.io/github/repo-size/keyiflerolsun/BTKSorgu?logo=git&logoColor=white&label=Boyut)](#)
 [![Görüntülenme](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/keyiflerolsun/BTKSorgu&title=Görüntülenme)](#)
 <a href="https://KekikAkademi.org/Kahve" target="_blank"><img src="https://img.shields.io/badge/☕️-Kahve Ismarla-ffdd00" title="☕️ Kahve Ismarla" style="padding-left:5px;"></a>
 
-[![Python Version](https://img.shields.io/pypi/pyversions/BTKSorgu?logo=python&logoColor=white)](#)
-[![License](https://img.shields.io/pypi/l/BTKSorgu?logo=gnu&logoColor=white)](#)
-[![Status](https://img.shields.io/pypi/status/BTKSorgu?logo=windowsterminal&logoColor=white)](#)
-
-[![PyPI](https://img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white)](https://pypi.org/project/BTKSorgu)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/BTKSorgu?logo=pypi&logoColor=white)](https://pypi.org/project/BTKSorgu)
-[![PyPI - Wheel](https://img.shields.io/pypi/wheel/BTKSorgu?logo=pypi&logoColor=white)](https://pypi.org/project/BTKSorgu)
-
-[![PyPI Yükleyici](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/pypiYukle.yml/badge.svg)](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/pypiYukle.yml)
-[![Flatpak Yükleyici](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/flatpakYukle.yml/badge.svg)](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/flatpakYukle.yml)
-
-[![FlatHub](https://img.shields.io/flathub/v/org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white)](https://flathub.org/tr/apps/org.KekikAkademi.BTKSorgu)
-[![FlatHub - Downloads](https://img.shields.io/flathub/downloads/org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white)](https://flathub.org/tr/apps/org.KekikAkademi.BTKSorgu)
+[![GitHub](https://img.shields.io/github/v/release/keyiflerolsun/BTKSorgu?logo=github&label=GitHub)](https://github.com/keyiflerolsun/BTKSorgu/releases)
+[![PyPi Yükleyici](https://img.shields.io/github/actions/workflow/status/keyiflerolsun/BTKSorgu/pypiYukle.yml?label=PyPi%20Y%C3%BCkleyici&logo=github)](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/pypiYukle.yml)
+[![Flatpak Yükleyici](https://img.shields.io/github/actions/workflow/status/keyiflerolsun/BTKSorgu/flatpakYukle.yml?label=Flatpak%20Y%C3%BCkleyici&logo=github)](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/flatpakYukle.yml)
+
+[![FlatHub](https://img.shields.io/flathub/v/org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white&label=FlatHub)](https://flathub.org/tr/apps/org.KekikAkademi.BTKSorgu)
+[![FlatHub - Yüklenme](https://img.shields.io/flathub/downloads/org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white&label=Yüklenme)](https://flathub.org/tr/apps/org.KekikAkademi.BTKSorgu)
+
+[![PyPi](https://img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white&label=PyPi)](https://pypi.org/project/BTKSorgu)
+[![PyPi - Yüklenme](https://img.shields.io/pypi/dm/BTKSorgu?logo=pypi&logoColor=white&label=Yüklenme)](https://pypi.org/project/BTKSorgu)
+[![PyPi - Wheel](https://img.shields.io/pypi/wheel/BTKSorgu?logo=pypi&logoColor=white&label=Wheel)](https://pypi.org/project/BTKSorgu)
+
+[![Python Version](https://img.shields.io/pypi/pyversions/BTKSorgu?logo=python&logoColor=white&label=Python)](#)
+[![Lisans](https://img.shields.io/pypi/l/BTKSorgu?logo=gnu&logoColor=white&label=Lisans)](#)
+[![Durum](https://img.shields.io/pypi/status/BTKSorgu?logo=windowsterminal&logoColor=white&label=Durum)](#)
 
 *Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu..*
 
 [![BTKSorgu](https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/SS.png)](#)
 
 [![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
@@ -185,8 +186,8 @@
 
 ## 💸 Bağış Yap
 
 **[☕️ Kahve Ismarla](https://KekikAkademi.org/Kahve)**
 
 ***
 
-> **[@KekikAkademi](https://t.me/KekikAkademi)** *için yazılmıştır..*
+> **[@KekikAkademi](https://t.me/KekikAkademi)** *için yazılmıştır..*
```

#### html2text {}

```diff
@@ -1,37 +1,45 @@
-# ð BTKSorgu [![Repo Boyutu](https://img.shields.io/github/repo-size/
-keyiflerolsun/BTKSorgu?logo=git&logoColor=white)](#) [![GÃ¶rÃ¼ntÃ¼lenme](https:
-//hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/
-keyiflerolsun/BTKSorgu&title=GÃ¶rÃ¼ntÃ¼lenme)](#) [https://img.shields.io/
-badge/âï¸-Kahve_Ismarla-ffdd00] [![Python Version](https://img.shields.io/
-pypi/pyversions/BTKSorgu?logo=python&logoColor=white)](#) [![License](https://
-img.shields.io/pypi/l/BTKSorgu?logo=gnu&logoColor=white)](#) [![Status](https:/
-/img.shields.io/pypi/status/BTKSorgu?logo=windowsterminal&logoColor=white)](#)
-[![PyPI](https://img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white)]
-(https://pypi.org/project/BTKSorgu) [![PyPI - Downloads](https://
-img.shields.io/pypi/dm/BTKSorgu?logo=pypi&logoColor=white)](https://pypi.org/
-project/BTKSorgu) [![PyPI - Wheel](https://img.shields.io/pypi/wheel/
-BTKSorgu?logo=pypi&logoColor=white)](https://pypi.org/project/BTKSorgu) [![PyPI
-YÃ¼kleyici](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/
-pypiYukle.yml/badge.svg)](https://github.com/keyiflerolsun/BTKSorgu/actions/
-workflows/pypiYukle.yml) [![Flatpak YÃ¼kleyici](https://github.com/
-keyiflerolsun/BTKSorgu/actions/workflows/flatpakYukle.yml/badge.svg)](https://
+# [https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/Shared/
+org.KekikAkademi.BTKSorgu.svg] BTKSorgu [![Boyut](https://img.shields.io/
+github/repo-size/keyiflerolsun/BTKSorgu?logo=git&logoColor=white&label=Boyut)]
+(#) [![GÃ¶rÃ¼ntÃ¼lenme](https://hits.seeyoufarm.com/api/count/incr/
+badge.svg?url=https://github.com/keyiflerolsun/BTKSorgu&title=GÃ¶rÃ¼ntÃ¼lenme)]
+(#) [https://img.shields.io/badge/âï¸-Kahve_Ismarla-ffdd00] [![GitHub]
+(https://img.shields.io/github/v/release/keyiflerolsun/
+BTKSorgu?logo=github&label=GitHub)](https://github.com/keyiflerolsun/BTKSorgu/
+releases) [![PyPi YÃ¼kleyici](https://img.shields.io/github/actions/workflow/
+status/keyiflerolsun/BTKSorgu/
+pypiYukle.yml?label=PyPi%20Y%C3%BCkleyici&logo=github)](https://github.com/
+keyiflerolsun/BTKSorgu/actions/workflows/pypiYukle.yml) [![Flatpak YÃ¼kleyici]
+(https://img.shields.io/github/actions/workflow/status/keyiflerolsun/BTKSorgu/
+flatpakYukle.yml?label=Flatpak%20Y%C3%BCkleyici&logo=github)](https://
 github.com/keyiflerolsun/BTKSorgu/actions/workflows/flatpakYukle.yml) [!
 [FlatHub](https://img.shields.io/flathub/v/
-org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white)](https://flathub.org/
-tr/apps/org.KekikAkademi.BTKSorgu) [![FlatHub - Downloads](https://
+org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white&label=FlatHub)](https://
+flathub.org/tr/apps/org.KekikAkademi.BTKSorgu) [![FlatHub - YÃ¼klenme](https://
 img.shields.io/flathub/downloads/
-org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white)](https://flathub.org/
-tr/apps/org.KekikAkademi.BTKSorgu) *Hedef websitesinin BTK TarafÄ±ndan EriÅim
-Engeli Sorgusu..* [![BTKSorgu](https://raw.githubusercontent.com/keyiflerolsun/
-BTKSorgu/main/.github/icons/SS.png)](#) [![ForTheBadge made-with-python](https:
-//ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/
-) [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-
-with-love.svg)](https://GitHub.com/keyiflerolsun/) ## ð Kurulum ### [https:/
-/raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/pypi.svg]
+org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white&label=YÃ¼klenme)](https:
+//flathub.org/tr/apps/org.KekikAkademi.BTKSorgu) [![PyPi](https://
+img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white&label=PyPi)](https://
+pypi.org/project/BTKSorgu) [![PyPi - YÃ¼klenme](https://img.shields.io/pypi/dm/
+BTKSorgu?logo=pypi&logoColor=white&label=YÃ¼klenme)](https://pypi.org/project/
+BTKSorgu) [![PyPi - Wheel](https://img.shields.io/pypi/wheel/
+BTKSorgu?logo=pypi&logoColor=white&label=Wheel)](https://pypi.org/project/
+BTKSorgu) [![Python Version](https://img.shields.io/pypi/pyversions/
+BTKSorgu?logo=python&logoColor=white&label=Python)](#) [![Lisans](https://
+img.shields.io/pypi/l/BTKSorgu?logo=gnu&logoColor=white&label=Lisans)](#) [!
+[Durum](https://img.shields.io/pypi/status/
+BTKSorgu?logo=windowsterminal&logoColor=white&label=Durum)](#) *Hedef
+websitesinin BTK TarafÄ±ndan EriÅim Engeli Sorgusu..* [![BTKSorgu](https://
+raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/SS.png)](#)
+[![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-
+with-python.svg)](https://www.python.org/) [![ForTheBadge built-with-love]
+(https://ForTheBadge.com/images/badges/built-with-love.svg)](https://
+GitHub.com/keyiflerolsun/) ## ð Kurulum ### [https://
+raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/pypi.svg]
 PyPi (Lib - CLI - UI) ```bash # YÃ¼klemek pip install BTKSorgu # GÃ¼ncellemek
 pip install -U BTKSorgu ``` ### [https://raw.githubusercontent.com/
 keyiflerolsun/BTKSorgu/main/.github/icons/flathub.svg] FlatHub (UI) ```bash #
 YÃ¼klemek flatpak install flathub org.KekikAkademi.BTKSorgu # ÃalÄ±ÅtÄ±rmak
 flatpak run org.KekikAkademi.BTKSorgu ``` ## ð KullanÄ±m ### [https://
 raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/python.svg]
 Lib ```python from BTKSorgu import BTKSorgu from time import time basla = time
```

### Comparing `BTKSorgu-1.2.1/Shared/org.KekikAkademi.BTKSorgu.appdata.xml` & `BTKSorgu-1.2.21/Shared/org.KekikAkademi.BTKSorgu.appdata.xml`

 * *Files 1% similar despite different names*

#### Comparing `BTKSorgu-1.2.1/Shared/org.KekikAkademi.BTKSorgu.appdata.xml` & `BTKSorgu-1.2.21/Shared/org.KekikAkademi.BTKSorgu.appdata.xml`

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

### Comparing `BTKSorgu-1.2.1/Shared/org.KekikAkademi.BTKSorgu.svg` & `BTKSorgu-1.2.21/Shared/org.KekikAkademi.BTKSorgu.svg`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.2.1/setup.py` & `BTKSorgu-1.2.21/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 from io         import open
 
 setup(
     # ? Genel Bilgiler
     name         = "BTKSorgu",
-    version      = "1.2.1",
+    version      = "1.2.21",
     url          = "https://github.com/keyiflerolsun/BTKSorgu",
     description  = "Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu",
     keywords     = ["BTKSorgu", "KekikAkademi", "keyiflerolsun"],
 
     author       = "keyiflerolsun",
     author_email = "keyiflerolsun@gmail.com",
 
@@ -54,8 +54,8 @@
         ("share/icons/hicolor/scalable/apps", ["Shared/org.KekikAkademi.BTKSorgu.svg"])
     ],
 
     # ? PyPI Bilgileri
     long_description_content_type = "text/markdown",
     long_description              = "".join(open("README.md", encoding="utf-8").readlines()),
     include_package_data          = True
-)
+)
```

