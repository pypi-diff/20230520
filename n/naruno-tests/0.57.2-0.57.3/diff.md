# Comparing `tmp/naruno_tests-0.57.2.tar.gz` & `tmp/naruno_tests-0.57.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naruno_tests-0.57.2.tar", last modified: Tue Apr 25 06:37:11 2023, max compression
+gzip compressed data, was "naruno_tests-0.57.3.tar", last modified: Sat May 20 13:25:38 2023, max compression
```

## Comparing `naruno_tests-0.57.2.tar` & `naruno_tests-0.57.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:37:11.496193 naruno_tests-0.57.2/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-25 06:37:11.496193 naruno_tests-0.57.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 06:37:11.496193 naruno_tests-0.57.2/naruno_tests.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-25 06:37:11.000000 naruno_tests-0.57.2/naruno_tests.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-25 06:37:11.000000 naruno_tests-0.57.2/naruno_tests.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 06:37:11.000000 naruno_tests-0.57.2/naruno_tests.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 06:37:11.000000 naruno_tests-0.57.2/naruno_tests.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-25 06:37:11.000000 naruno_tests-0.57.2/naruno_tests.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 06:37:11.000000 naruno_tests-0.57.2/naruno_tests.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 06:37:11.496193 naruno_tests-0.57.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-25 06:36:46.000000 naruno_tests-0.57.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:25:38.383193 naruno_tests-0.57.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-20 13:25:38.383193 naruno_tests-0.57.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:25:38.383193 naruno_tests-0.57.3/naruno_tests.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-20 13:25:38.000000 naruno_tests-0.57.3/naruno_tests.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-20 13:25:38.000000 naruno_tests-0.57.3/naruno_tests.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 13:25:38.000000 naruno_tests-0.57.3/naruno_tests.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 13:25:38.000000 naruno_tests-0.57.3/naruno_tests.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-20 13:25:38.000000 naruno_tests-0.57.3/naruno_tests.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 13:25:38.000000 naruno_tests-0.57.3/naruno_tests.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 13:25:38.383193 naruno_tests-0.57.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-20 13:25:14.000000 naruno_tests-0.57.3/setup.py
```

### Comparing `naruno_tests-0.57.2/setup.py` & `naruno_tests-0.57.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from setuptools import setup
 
 setup(
     name="naruno_tests",
-    version="0.57.2",
+    version="0.57.3",
     description="""This is a tool for tests on Naruno""",
     url="https://docs.naruno.org/",
     author="Naruno Developers",
     author_email="onur.atakan.ulusoy@naruno.org",
     license="MPL-2.0",
     install_requires="""
 requests==2.28.2
 pytest==7.1.2
 speed_calculator==0.4.1
-naruno_api==0.57.2
+naruno_api==0.57.3
 """,
     python_requires=">=3.8",
     zip_safe=False,
 )
```

