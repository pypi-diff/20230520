# Comparing `tmp/gitea-backup-2.1.2.tar.gz` & `tmp/gitea-backup-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitea-backup-2.1.2.tar", last modified: Fri May 19 22:03:44 2023, max compression
+gzip compressed data, was "gitea-backup-2.1.3.tar", last modified: Fri May 19 22:05:16 2023, max compression
```

## Comparing `gitea-backup-2.1.2.tar` & `gitea-backup-2.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 noursofanati   (501) staff       (20)        0 2023-05-19 22:03:44.289455 gitea-backup-2.1.2/
--rw-r--r--   0 noursofanati   (501) staff       (20)    35191 2023-05-19 22:03:44.000000 gitea-backup-2.1.2/CHANGES.rst
--rw-r--r--   0 noursofanati   (501) staff       (20)     1085 2023-05-19 22:01:04.000000 gitea-backup-2.1.2/LICENSE.txt
--rw-r--r--   0 noursofanati   (501) staff       (20)       28 2023-05-19 22:01:04.000000 gitea-backup-2.1.2/MANIFEST.in
--rw-r--r--   0 noursofanati   (501) staff       (20)     9402 2023-05-19 22:03:44.289287 gitea-backup-2.1.2/PKG-INFO
--rw-r--r--   0 noursofanati   (501) staff       (20)     8740 2023-05-19 22:03:44.000000 gitea-backup-2.1.2/README
--rw-r--r--   0 noursofanati   (501) staff       (20)     8740 2023-05-19 22:03:43.000000 gitea-backup-2.1.2/README.rst
-drwxr-xr-x   0 noursofanati   (501) staff       (20)        0 2023-05-19 22:03:44.288133 gitea-backup-2.1.2/bin/
--rwxr-xr-x   0 noursofanati   (501) staff       (20)     1322 2023-05-19 22:01:04.000000 gitea-backup-2.1.2/bin/gitea-backup
-drwxr-xr-x   0 noursofanati   (501) staff       (20)        0 2023-05-19 22:03:44.288410 gitea-backup-2.1.2/gitea_backup/
--rw-------   0 noursofanati   (501) staff       (20)       22 2023-05-19 22:03:43.000000 gitea-backup-2.1.2/gitea_backup/__init__.py
--rw-r--r--   0 noursofanati   (501) staff       (20)    47181 2023-05-19 22:01:04.000000 gitea-backup-2.1.2/gitea_backup/gitea_backup.py
-drwxr-xr-x   0 noursofanati   (501) staff       (20)        0 2023-05-19 22:03:44.289009 gitea-backup-2.1.2/gitea_backup.egg-info/
--rw-r--r--   0 noursofanati   (501) staff       (20)     9402 2023-05-19 22:03:44.000000 gitea-backup-2.1.2/gitea_backup.egg-info/PKG-INFO
--rw-r--r--   0 noursofanati   (501) staff       (20)      325 2023-05-19 22:03:44.000000 gitea-backup-2.1.2/gitea_backup.egg-info/SOURCES.txt
--rw-r--r--   0 noursofanati   (501) staff       (20)        1 2023-05-19 22:03:44.000000 gitea-backup-2.1.2/gitea_backup.egg-info/dependency_links.txt
--rw-r--r--   0 noursofanati   (501) staff       (20)       13 2023-05-19 22:03:44.000000 gitea-backup-2.1.2/gitea_backup.egg-info/top_level.txt
--rw-r--r--   0 noursofanati   (501) staff       (20)        1 2023-05-19 22:03:11.000000 gitea-backup-2.1.2/gitea_backup.egg-info/zip-safe
--rw-r--r--   0 noursofanati   (501) staff       (20)        1 2023-05-19 22:01:04.000000 gitea-backup-2.1.2/requirements.txt
--rw-r--r--   0 noursofanati   (501) staff       (20)       38 2023-05-19 22:03:44.289499 gitea-backup-2.1.2/setup.cfg
--rw-r--r--   0 noursofanati   (501) staff       (20)     1568 2023-05-19 22:02:25.000000 gitea-backup-2.1.2/setup.py
+drwxr-xr-x   0 noursofanati   (501) staff       (20)        0 2023-05-19 22:05:16.849110 gitea-backup-2.1.3/
+-rw-r--r--   0 noursofanati   (501) staff       (20)    35266 2023-05-19 22:05:16.000000 gitea-backup-2.1.3/CHANGES.rst
+-rw-r--r--   0 noursofanati   (501) staff       (20)     1085 2023-05-19 22:01:04.000000 gitea-backup-2.1.3/LICENSE.txt
+-rw-r--r--   0 noursofanati   (501) staff       (20)       28 2023-05-19 22:01:04.000000 gitea-backup-2.1.3/MANIFEST.in
+-rw-r--r--   0 noursofanati   (501) staff       (20)     9402 2023-05-19 22:05:16.848894 gitea-backup-2.1.3/PKG-INFO
+-rw-r--r--   0 noursofanati   (501) staff       (20)     8740 2023-05-19 22:05:16.000000 gitea-backup-2.1.3/README
+-rw-r--r--   0 noursofanati   (501) staff       (20)     8740 2023-05-19 22:05:15.000000 gitea-backup-2.1.3/README.rst
+drwxr-xr-x   0 noursofanati   (501) staff       (20)        0 2023-05-19 22:05:16.847509 gitea-backup-2.1.3/bin/
+-rwxr-xr-x   0 noursofanati   (501) staff       (20)     1322 2023-05-19 22:01:04.000000 gitea-backup-2.1.3/bin/gitea-backup
+drwxr-xr-x   0 noursofanati   (501) staff       (20)        0 2023-05-19 22:05:16.847811 gitea-backup-2.1.3/gitea_backup/
+-rw-------   0 noursofanati   (501) staff       (20)       22 2023-05-19 22:05:15.000000 gitea-backup-2.1.3/gitea_backup/__init__.py
+-rw-r--r--   0 noursofanati   (501) staff       (20)    47181 2023-05-19 22:01:04.000000 gitea-backup-2.1.3/gitea_backup/gitea_backup.py
+drwxr-xr-x   0 noursofanati   (501) staff       (20)        0 2023-05-19 22:05:16.848588 gitea-backup-2.1.3/gitea_backup.egg-info/
+-rw-r--r--   0 noursofanati   (501) staff       (20)     9402 2023-05-19 22:05:16.000000 gitea-backup-2.1.3/gitea_backup.egg-info/PKG-INFO
+-rw-r--r--   0 noursofanati   (501) staff       (20)      325 2023-05-19 22:05:16.000000 gitea-backup-2.1.3/gitea_backup.egg-info/SOURCES.txt
+-rw-r--r--   0 noursofanati   (501) staff       (20)        1 2023-05-19 22:05:16.000000 gitea-backup-2.1.3/gitea_backup.egg-info/dependency_links.txt
+-rw-r--r--   0 noursofanati   (501) staff       (20)       13 2023-05-19 22:05:16.000000 gitea-backup-2.1.3/gitea_backup.egg-info/top_level.txt
+-rw-r--r--   0 noursofanati   (501) staff       (20)        1 2023-05-19 22:03:11.000000 gitea-backup-2.1.3/gitea_backup.egg-info/zip-safe
+-rw-r--r--   0 noursofanati   (501) staff       (20)        1 2023-05-19 22:01:04.000000 gitea-backup-2.1.3/requirements.txt
+-rw-r--r--   0 noursofanati   (501) staff       (20)       38 2023-05-19 22:05:16.849150 gitea-backup-2.1.3/setup.cfg
+-rw-r--r--   0 noursofanati   (501) staff       (20)     1568 2023-05-19 22:02:25.000000 gitea-backup-2.1.3/setup.py
```

### Comparing `gitea-backup-2.1.2/CHANGES.rst` & `gitea-backup-2.1.3/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 Changelog
 =========
 
-2.1.2 (2023-05-20)
+2.1.3 (2023-05-20)
 ------------------
 ------------------
+- Release version 2.1.2. [sb-nour]
+
+
+2.1.1 (2023-05-19)
+------------------
 - Release version 2.1.1. [sb-nour]
 - Change author and email. [sb-nour]
 
 
 2.1.0 (2023-05-18)
 ------------------
 - Release version 2.1.0. [Nour Sofanati]
```

### Comparing `gitea-backup-2.1.2/LICENSE.txt` & `gitea-backup-2.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gitea-backup-2.1.2/PKG-INFO` & `gitea-backup-2.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitea-backup
-Version: 2.1.2
+Version: 2.1.3
 Summary: backup a gitea user or organization
 Home-page: http://github.com/simplebackups/python-gitea-backup
 Author: simplebackups
 Author-email: simplebackups.io@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: System :: Archiving :: Backup
```

### Comparing `gitea-backup-2.1.2/README` & `gitea-backup-2.1.3/README`

 * *Files identical despite different names*

### Comparing `gitea-backup-2.1.2/README.rst` & `gitea-backup-2.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `gitea-backup-2.1.2/bin/gitea-backup` & `gitea-backup-2.1.3/bin/gitea-backup`

 * *Files identical despite different names*

### Comparing `gitea-backup-2.1.2/gitea_backup/gitea_backup.py` & `gitea-backup-2.1.3/gitea_backup/gitea_backup.py`

 * *Files identical despite different names*

### Comparing `gitea-backup-2.1.2/gitea_backup.egg-info/PKG-INFO` & `gitea-backup-2.1.3/gitea_backup.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitea-backup
-Version: 2.1.2
+Version: 2.1.3
 Summary: backup a gitea user or organization
 Home-page: http://github.com/simplebackups/python-gitea-backup
 Author: simplebackups
 Author-email: simplebackups.io@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: System :: Archiving :: Backup
```

### Comparing `gitea-backup-2.1.2/setup.py` & `gitea-backup-2.1.3/setup.py`

 * *Files identical despite different names*

