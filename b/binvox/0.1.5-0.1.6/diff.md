# Comparing `tmp/binvox-0.1.5.tar.gz` & `tmp/binvox-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "binvox-0.1.5.tar", last modified: Wed Dec  1 23:22:30 2021, max compression
+gzip compressed data, was "dist/binvox-0.1.6.tar", last modified: Sat May 20 12:42:29 2023, max compression
```

## Comparing `binvox-0.1.5.tar` & `binvox-0.1.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxr-xr-x   0 faridyagubbayli   (501) staff       (20)        0 2021-12-01 23:22:30.132842 binvox-0.1.5/
--rw-r--r--   0 faridyagubbayli   (501) staff       (20)     1866 2021-12-01 23:22:30.132986 binvox-0.1.5/PKG-INFO
--rw-r--r--   0 faridyagubbayli   (501) staff       (20)      918 2021-12-01 23:22:23.403421 binvox-0.1.5/README.rst
-drwxr-xr-x   0 faridyagubbayli   (501) staff       (20)        0 2021-12-01 23:22:30.132781 binvox-0.1.5/binvox/
--rw-r--r--   0 faridyagubbayli   (501) staff       (20)      102 2021-12-01 23:17:51.061985 binvox-0.1.5/binvox/__init__.py
--rw-r--r--   0 faridyagubbayli   (501) staff       (20)     8222 2021-11-14 08:45:46.210909 binvox-0.1.5/binvox/binvox.py
--rw-r--r--   0 faridyagubbayli   (501) staff       (20)      654 2021-11-14 06:59:23.728426 binvox-0.1.5/binvox/utils.py
--rw-r--r--   0 faridyagubbayli   (501) staff       (20)      102 2021-11-14 08:51:55.781853 binvox-0.1.5/setup.cfg
--rw-r--r--   0 faridyagubbayli   (501) staff       (20)     1319 2021-12-01 23:14:00.543238 binvox-0.1.5/setup.py
+drwxr-xr-x   0 farid      (503) staff       (20)        0 2023-05-20 12:42:29.000000 binvox-0.1.6/
+-rw-r--r--   0 farid      (503) staff       (20)     1866 2023-05-20 12:42:29.000000 binvox-0.1.6/PKG-INFO
+-rw-r--r--   0 farid      (503) staff       (20)      918 2023-05-20 12:12:38.000000 binvox-0.1.6/README.rst
+drwxr-xr-x   0 farid      (503) staff       (20)        0 2023-05-20 12:42:29.000000 binvox-0.1.6/binvox/
+-rw-r--r--   0 farid      (503) staff       (20)       79 2023-05-20 12:37:11.000000 binvox-0.1.6/binvox/__init__.py
+-rw-r--r--   0 farid      (503) staff       (20)     8222 2023-05-20 12:12:38.000000 binvox-0.1.6/binvox/binvox.py
+-rw-r--r--   0 farid      (503) staff       (20)      654 2023-05-20 12:12:38.000000 binvox-0.1.6/binvox/utils.py
+-rw-r--r--   0 farid      (503) staff       (20)      102 2023-05-20 12:12:38.000000 binvox-0.1.6/setup.cfg
+-rw-r--r--   0 farid      (503) staff       (20)     1311 2023-05-20 12:40:06.000000 binvox-0.1.6/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `binvox-0.1.5/PKG-INFO` & `binvox-0.1.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: binvox
-Version: 0.1.5
+Version: 0.1.6
 Summary: Library for loading & saving the Binvox files
 Home-page: https://github.com/faridyagubbayli/binvox
 Author: Farid Yagubbayli
 Author-email: faridyagubbayli@gmail.com
 License: MIT
 Description: binvox
         =======
```

### Comparing `binvox-0.1.5/README.rst` & `binvox-0.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `binvox-0.1.5/binvox/binvox.py` & `binvox-0.1.6/binvox/binvox.py`

 * *Files identical despite different names*

### Comparing `binvox-0.1.5/binvox/utils.py` & `binvox-0.1.6/binvox/utils.py`

 * *Files identical despite different names*

### Comparing `binvox-0.1.5/setup.py` & `binvox-0.1.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from distutils.core import setup
-from binvox import __version__
+
+__version__ = "0.1.6"
 
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.rst").read_text(encoding="utf-8")
 
 setup(
```

