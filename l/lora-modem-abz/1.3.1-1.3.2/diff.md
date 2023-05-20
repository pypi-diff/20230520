# Comparing `tmp/lora-modem-abz-1.3.1.tar.gz` & `tmp/lora-modem-abz-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lora-modem-abz-1.3.1.tar", last modified: Sat Mar 25 01:00:49 2023, max compression
+gzip compressed data, was "lora-modem-abz-1.3.2.tar", last modified: Sat May 20 17:26:13 2023, max compression
```

## Comparing `lora-modem-abz-1.3.1.tar` & `lora-modem-abz-1.3.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 janakj     (501) staff       (20)        0 2023-03-25 01:00:49.343872 lora-modem-abz-1.3.1/
--rw-r--r--   0 janakj     (501) staff       (20)     1491 2023-03-25 00:59:58.000000 lora-modem-abz-1.3.1/LICENSE
--rw-r--r--   0 janakj     (501) staff       (20)       72 2023-03-25 00:59:58.000000 lora-modem-abz-1.3.1/MANIFEST.in
--rw-r--r--   0 janakj     (501) staff       (20)     7676 2023-03-25 01:00:49.344121 lora-modem-abz-1.3.1/PKG-INFO
--rw-r--r--   0 janakj     (501) staff       (20)     6994 2023-03-25 00:59:58.000000 lora-modem-abz-1.3.1/README.md
--rw-r--r--   0 janakj     (501) staff       (20)        7 2023-03-25 01:00:39.000000 lora-modem-abz-1.3.1/VERSION
--rwxr-xr-x   0 janakj     (501) staff       (20)   198714 2023-03-25 00:59:58.000000 lora-modem-abz-1.3.1/lora.py
-drwxr-xr-x   0 janakj     (501) staff       (20)        0 2023-03-25 01:00:49.343510 lora-modem-abz-1.3.1/lora_modem_abz.egg-info/
--rw-r--r--   0 janakj     (501) staff       (20)     7676 2023-03-25 01:00:49.000000 lora-modem-abz-1.3.1/lora_modem_abz.egg-info/PKG-INFO
--rw-r--r--   0 janakj     (501) staff       (20)      300 2023-03-25 01:00:49.000000 lora-modem-abz-1.3.1/lora_modem_abz.egg-info/SOURCES.txt
--rw-r--r--   0 janakj     (501) staff       (20)        1 2023-03-25 01:00:49.000000 lora-modem-abz-1.3.1/lora_modem_abz.egg-info/dependency_links.txt
--rw-r--r--   0 janakj     (501) staff       (20)       34 2023-03-25 01:00:49.000000 lora-modem-abz-1.3.1/lora_modem_abz.egg-info/entry_points.txt
--rw-r--r--   0 janakj     (501) staff       (20)       33 2023-03-25 01:00:49.000000 lora-modem-abz-1.3.1/lora_modem_abz.egg-info/requires.txt
--rw-r--r--   0 janakj     (501) staff       (20)        5 2023-03-25 01:00:49.000000 lora-modem-abz-1.3.1/lora_modem_abz.egg-info/top_level.txt
--rw-r--r--   0 janakj     (501) staff       (20)       82 2023-03-25 00:59:58.000000 lora-modem-abz-1.3.1/pyproject.toml
--rw-r--r--   0 janakj     (501) staff       (20)      835 2023-03-25 01:00:49.344936 lora-modem-abz-1.3.1/setup.cfg
+drwxr-xr-x   0 janakj     (501) staff       (20)        0 2023-05-20 17:26:13.524806 lora-modem-abz-1.3.2/
+-rw-r--r--   0 janakj     (501) staff       (20)     1491 2023-05-20 17:25:25.000000 lora-modem-abz-1.3.2/LICENSE
+-rw-r--r--   0 janakj     (501) staff       (20)       72 2023-05-20 17:25:25.000000 lora-modem-abz-1.3.2/MANIFEST.in
+-rw-r--r--   0 janakj     (501) staff       (20)     7676 2023-05-20 17:26:13.525260 lora-modem-abz-1.3.2/PKG-INFO
+-rw-r--r--   0 janakj     (501) staff       (20)     6994 2023-05-20 17:25:25.000000 lora-modem-abz-1.3.2/README.md
+-rw-r--r--   0 janakj     (501) staff       (20)        7 2023-05-20 17:26:04.000000 lora-modem-abz-1.3.2/VERSION
+-rwxr-xr-x   0 janakj     (501) staff       (20)   198714 2023-05-20 17:25:25.000000 lora-modem-abz-1.3.2/lora.py
+drwxr-xr-x   0 janakj     (501) staff       (20)        0 2023-05-20 17:26:13.524427 lora-modem-abz-1.3.2/lora_modem_abz.egg-info/
+-rw-r--r--   0 janakj     (501) staff       (20)     7676 2023-05-20 17:26:13.000000 lora-modem-abz-1.3.2/lora_modem_abz.egg-info/PKG-INFO
+-rw-r--r--   0 janakj     (501) staff       (20)      300 2023-05-20 17:26:13.000000 lora-modem-abz-1.3.2/lora_modem_abz.egg-info/SOURCES.txt
+-rw-r--r--   0 janakj     (501) staff       (20)        1 2023-05-20 17:26:13.000000 lora-modem-abz-1.3.2/lora_modem_abz.egg-info/dependency_links.txt
+-rw-r--r--   0 janakj     (501) staff       (20)       34 2023-05-20 17:26:13.000000 lora-modem-abz-1.3.2/lora_modem_abz.egg-info/entry_points.txt
+-rw-r--r--   0 janakj     (501) staff       (20)       33 2023-05-20 17:26:13.000000 lora-modem-abz-1.3.2/lora_modem_abz.egg-info/requires.txt
+-rw-r--r--   0 janakj     (501) staff       (20)        5 2023-05-20 17:26:13.000000 lora-modem-abz-1.3.2/lora_modem_abz.egg-info/top_level.txt
+-rw-r--r--   0 janakj     (501) staff       (20)       82 2023-05-20 17:25:25.000000 lora-modem-abz-1.3.2/pyproject.toml
+-rw-r--r--   0 janakj     (501) staff       (20)      835 2023-05-20 17:26:13.526356 lora-modem-abz-1.3.2/setup.cfg
```

### Comparing `lora-modem-abz-1.3.1/LICENSE` & `lora-modem-abz-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lora-modem-abz-1.3.1/PKG-INFO` & `lora-modem-abz-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lora-modem-abz
-Version: 1.3.1
+Version: 1.3.2
 Summary: Python library for the Murata TypeABZ LoRaWAN modem
 Home-page: https://github.com/hardwario/lora-modem-abz
 Author: Jan Janak
 Author-email: jan@janakj.org
 License: BSD 3-Clause License
 Keywords: iot,lora,lorawan,lpwan,lorawan-device,firmware,stm32
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lora-modem-abz-1.3.1/README.md` & `lora-modem-abz-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `lora-modem-abz-1.3.1/lora.py` & `lora-modem-abz-1.3.2/lora.py`

 * *Files identical despite different names*

### Comparing `lora-modem-abz-1.3.1/lora_modem_abz.egg-info/PKG-INFO` & `lora-modem-abz-1.3.2/lora_modem_abz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lora-modem-abz
-Version: 1.3.1
+Version: 1.3.2
 Summary: Python library for the Murata TypeABZ LoRaWAN modem
 Home-page: https://github.com/hardwario/lora-modem-abz
 Author: Jan Janak
 Author-email: jan@janakj.org
 License: BSD 3-Clause License
 Keywords: iot,lora,lorawan,lpwan,lorawan-device,firmware,stm32
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lora-modem-abz-1.3.1/setup.cfg` & `lora-modem-abz-1.3.2/setup.cfg`

 * *Files identical despite different names*

