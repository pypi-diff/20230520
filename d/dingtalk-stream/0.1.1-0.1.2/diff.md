# Comparing `tmp/dingtalk-stream-0.1.1.tar.gz` & `tmp/dingtalk-stream-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dingtalk-stream-0.1.1.tar", last modified: Fri May 19 22:16:41 2023, max compression
+gzip compressed data, was "dingtalk-stream-0.1.2.tar", last modified: Fri May 19 22:21:18 2023, max compression
```

## Comparing `dingtalk-stream-0.1.1.tar` & `dingtalk-stream-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:16:41.544184 dingtalk-stream-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-19 22:16:41.000000 dingtalk-stream-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-19 22:16:41.544184 dingtalk-stream-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-19 22:16:41.000000 dingtalk-stream-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:16:41.544184 dingtalk-stream-0.1.1/dingtalk_stream/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-19 22:16:41.000000 dingtalk-stream-0.1.1/dingtalk_stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-05-19 22:16:41.000000 dingtalk-stream-0.1.1/dingtalk_stream/chatbot.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-19 22:16:41.000000 dingtalk-stream-0.1.1/dingtalk_stream/credential.py
--rw-r--r--   0 runner    (1001) docker     (123)     7309 2023-05-19 22:16:41.000000 dingtalk-stream-0.1.1/dingtalk_stream/frames.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-19 22:16:41.000000 dingtalk-stream-0.1.1/dingtalk_stream/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-05-19 22:16:41.000000 dingtalk-stream-0.1.1/dingtalk_stream/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:16:41.544184 dingtalk-stream-0.1.1/dingtalk_stream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-19 22:16:41.000000 dingtalk-stream-0.1.1/dingtalk_stream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-19 22:16:41.000000 dingtalk-stream-0.1.1/dingtalk_stream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 22:16:41.000000 dingtalk-stream-0.1.1/dingtalk_stream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-19 22:16:41.000000 dingtalk-stream-0.1.1/dingtalk_stream.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-19 22:16:41.000000 dingtalk-stream-0.1.1/dingtalk_stream.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 22:16:41.544184 dingtalk-stream-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-19 22:16:41.000000 dingtalk-stream-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:21:18.087712 dingtalk-stream-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-19 22:21:17.000000 dingtalk-stream-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-05-19 22:21:18.087712 dingtalk-stream-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-19 22:21:17.000000 dingtalk-stream-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:21:18.087712 dingtalk-stream-0.1.2/dingtalk_stream/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-19 22:21:17.000000 dingtalk-stream-0.1.2/dingtalk_stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-05-19 22:21:17.000000 dingtalk-stream-0.1.2/dingtalk_stream/chatbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-19 22:21:17.000000 dingtalk-stream-0.1.2/dingtalk_stream/credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7309 2023-05-19 22:21:17.000000 dingtalk-stream-0.1.2/dingtalk_stream/frames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-19 22:21:17.000000 dingtalk-stream-0.1.2/dingtalk_stream/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-05-19 22:21:17.000000 dingtalk-stream-0.1.2/dingtalk_stream/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 22:21:18.087712 dingtalk-stream-0.1.2/dingtalk_stream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-05-19 22:21:18.000000 dingtalk-stream-0.1.2/dingtalk_stream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-19 22:21:18.000000 dingtalk-stream-0.1.2/dingtalk_stream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 22:21:18.000000 dingtalk-stream-0.1.2/dingtalk_stream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-19 22:21:18.000000 dingtalk-stream-0.1.2/dingtalk_stream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-19 22:21:18.000000 dingtalk-stream-0.1.2/dingtalk_stream.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 22:21:18.087712 dingtalk-stream-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-19 22:21:17.000000 dingtalk-stream-0.1.2/setup.py
```

### Comparing `dingtalk-stream-0.1.1/LICENSE` & `dingtalk-stream-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.1.1/README.md` & `dingtalk-stream-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.1.1/dingtalk_stream/chatbot.py` & `dingtalk-stream-0.1.2/dingtalk_stream/chatbot.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.1.1/dingtalk_stream/frames.py` & `dingtalk-stream-0.1.2/dingtalk_stream/frames.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.1.1/dingtalk_stream/handlers.py` & `dingtalk-stream-0.1.2/dingtalk_stream/handlers.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.1.1/dingtalk_stream/stream.py` & `dingtalk-stream-0.1.2/dingtalk_stream/stream.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.1.1/setup.py` & `dingtalk-stream-0.1.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from setuptools import setup
 
 setup(
     name='dingtalk-stream',
-    version='0.1.1',
+    version='0.1.2',
     description='A Python package for sending messages to DingTalk chatbot',
+    long_description=open('README.md').read(),
+    long_description_content_type='text/markdown',
     url='https://github.com/open-dingtalk/dingtalk-stream-sdk-python',
     author='Ke Jie',
     author_email='jinxi.kj@alibaba-inc.com',
     license='MIT',
     packages=['dingtalk_stream'],
     install_requires=[
         'websockets>=11.0.2',
```

