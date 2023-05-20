# Comparing `tmp/thedevilseye-2022.1.4.0.tar.gz` & `tmp/thedevilseye-2022.1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thedevilseye-2022.1.4.0.tar", last modified: Thu Feb 17 23:30:14 2022, max compression
+gzip compressed data, was "thedevilseye-2022.1.5.1.tar", last modified: Fri Dec  2 20:53:46 2022, max compression
```

## Comparing `thedevilseye-2022.1.4.0.tar` & `thedevilseye-2022.1.5.1.tar`

### file list

```diff
@@ -1,21 +1,17 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2022-02-17 23:30:14.406978 thedevilseye-2022.1.4.0/
--rw-rw----   0 root         (0) everybody  (9997)    35147 2022-02-17 21:03:24.000000 thedevilseye-2022.1.4.0/LICENSE
--rw-rw----   0 root         (0) everybody  (9997)     3213 2022-02-17 23:30:14.396978 thedevilseye-2022.1.4.0/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)     2594 2022-02-17 23:20:10.000000 thedevilseye-2022.1.4.0/README.md
-drwxrwx---   0 root         (0) everybody  (9997)        0 2022-02-17 23:30:14.376978 thedevilseye-2022.1.4.0/eye/
--rw-rw----   0 root         (0) everybody  (9997)        0 2022-02-17 21:03:24.000000 thedevilseye-2022.1.4.0/eye/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)      839 2022-02-17 21:15:57.000000 thedevilseye-2022.1.4.0/eye/banner.py
--rw-rw----   0 root         (0) everybody  (9997)      380 2022-02-17 21:03:24.000000 thedevilseye-2022.1.4.0/eye/colors.py
--rw-rw----   0 root         (0) everybody  (9997)      278 2022-02-17 21:03:24.000000 thedevilseye-2022.1.4.0/eye/dump.py
--rw-rw----   0 root         (0) everybody  (9997)    35201 2022-02-17 21:03:24.000000 thedevilseye-2022.1.4.0/eye/licence.py
--rw-rw----   0 root         (0) everybody  (9997)     2893 2022-02-17 23:27:08.000000 thedevilseye-2022.1.4.0/eye/main.py
--rw-rw----   0 root         (0) everybody  (9997)      697 2022-02-17 21:19:45.000000 thedevilseye-2022.1.4.0/eye/search.py
--rw-rw----   0 root         (0) everybody  (9997)       38 2022-02-17 23:30:14.406978 thedevilseye-2022.1.4.0/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)      976 2022-02-17 21:08:56.000000 thedevilseye-2022.1.4.0/setup.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2022-02-17 23:30:14.396978 thedevilseye-2022.1.4.0/thedevilseye.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)     3213 2022-02-17 23:30:13.000000 thedevilseye-2022.1.4.0/thedevilseye.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      341 2022-02-17 23:30:13.000000 thedevilseye-2022.1.4.0/thedevilseye.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2022-02-17 23:30:13.000000 thedevilseye-2022.1.4.0/thedevilseye.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       47 2022-02-17 23:30:13.000000 thedevilseye-2022.1.4.0/thedevilseye.egg-info/entry_points.txt
--rw-rw----   0 root         (0) everybody  (9997)       24 2022-02-17 23:30:13.000000 thedevilseye-2022.1.4.0/thedevilseye.egg-info/requires.txt
--rw-rw----   0 root         (0) everybody  (9997)        4 2022-02-17 23:30:13.000000 thedevilseye-2022.1.4.0/thedevilseye.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 20:53:46.185253 thedevilseye-2022.1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (122)    35147 2022-12-02 20:53:36.000000 thedevilseye-2022.1.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1944 2022-12-02 20:53:46.185253 thedevilseye-2022.1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1311 2022-12-02 20:53:36.000000 thedevilseye-2022.1.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-02 20:53:46.185253 thedevilseye-2022.1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1022 2022-12-02 20:53:36.000000 thedevilseye-2022.1.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 20:53:46.181253 thedevilseye-2022.1.5.1/thedevilseye/
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-02 20:53:36.000000 thedevilseye-2022.1.5.1/thedevilseye/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1223 2022-12-02 20:53:36.000000 thedevilseye-2022.1.5.1/thedevilseye/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1474 2022-12-02 20:53:36.000000 thedevilseye-2022.1.5.1/thedevilseye/thedevilseye.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 20:53:46.185253 thedevilseye-2022.1.5.1/thedevilseye.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1944 2022-12-02 20:53:46.000000 thedevilseye-2022.1.5.1/thedevilseye.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      319 2022-12-02 20:53:46.000000 thedevilseye-2022.1.5.1/thedevilseye.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-02 20:53:46.000000 thedevilseye-2022.1.5.1/thedevilseye.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2022-12-02 20:53:46.000000 thedevilseye-2022.1.5.1/thedevilseye.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2022-12-02 20:53:46.000000 thedevilseye-2022.1.5.1/thedevilseye.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2022-12-02 20:53:46.000000 thedevilseye-2022.1.5.1/thedevilseye.egg-info/top_level.txt
```

### Comparing `thedevilseye-2022.1.4.0/LICENSE` & `thedevilseye-2022.1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `thedevilseye-2022.1.4.0/setup.py` & `thedevilseye-2022.1.5.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as file:
     long_description = file.read()
 
 setuptools.setup(
     name="thedevilseye",
-    version="2022.1.4.0",
+    version="2022.1.5.1",
     author="Richard Mwewa",
-    author_email="richardmwewa@duck.com",
-    packages=["eye"],
-    description="Darkweb .onion link(s) extracting tool",
+    author_email="rly0nheart@duck.com",
+    packages=["thedevilseye"],
+    description="Darkweb osint tool",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rly0nheart/thedevilseye",
     license="GNU General Public License v3 (GPLv3)",
-    install_requires=["requests","beautifulsoup4"],
+    install_requires=["rich", "selenium"],
     classifiers=[
+        'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Information Technology',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',  
-        'Operating System :: POSIX :: Linux',
+        'Operating System :: OS Independent',
         'Natural Language :: English',
-        'Programming Language :: Python :: 3',
-    ],
+        'Programming Language :: Python :: 3'
+        ],
     entry_points={
         "console_scripts": [
-            "eye=eye.main:thedevilseye",
+            "thedevilseye=thedevilseye.main:main",
         ]
     },
 )
```

