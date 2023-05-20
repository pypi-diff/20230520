# Comparing `tmp/dingtalk-stream-0.1.7.tar.gz` & `tmp/dingtalk-stream-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dingtalk-stream-0.1.7.tar", last modified: Sat May 20 02:54:56 2023, max compression
+gzip compressed data, was "dingtalk-stream-0.1.8.tar", last modified: Sat May 20 02:58:27 2023, max compression
```

## Comparing `dingtalk-stream-0.1.7.tar` & `dingtalk-stream-0.1.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 02:54:56.367342 dingtalk-stream-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-20 02:54:55.000000 dingtalk-stream-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-05-20 02:54:56.367342 dingtalk-stream-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-20 02:54:55.000000 dingtalk-stream-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 02:54:56.367342 dingtalk-stream-0.1.7/dingtalk_stream/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-20 02:54:55.000000 dingtalk-stream-0.1.7/dingtalk_stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-05-20 02:54:55.000000 dingtalk-stream-0.1.7/dingtalk_stream/chatbot.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-20 02:54:55.000000 dingtalk-stream-0.1.7/dingtalk_stream/credential.py
--rw-r--r--   0 runner    (1001) docker     (123)     7309 2023-05-20 02:54:55.000000 dingtalk-stream-0.1.7/dingtalk_stream/frames.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-20 02:54:55.000000 dingtalk-stream-0.1.7/dingtalk_stream/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-20 02:54:55.000000 dingtalk-stream-0.1.7/dingtalk_stream/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     8169 2023-05-20 02:54:55.000000 dingtalk-stream-0.1.7/dingtalk_stream/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 02:54:56.367342 dingtalk-stream-0.1.7/dingtalk_stream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-05-20 02:54:56.000000 dingtalk-stream-0.1.7/dingtalk_stream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-20 02:54:56.000000 dingtalk-stream-0.1.7/dingtalk_stream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 02:54:56.000000 dingtalk-stream-0.1.7/dingtalk_stream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-20 02:54:56.000000 dingtalk-stream-0.1.7/dingtalk_stream.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-20 02:54:56.000000 dingtalk-stream-0.1.7/dingtalk_stream.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 02:54:56.367342 dingtalk-stream-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-20 02:54:55.000000 dingtalk-stream-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 02:58:27.808897 dingtalk-stream-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-20 02:58:27.000000 dingtalk-stream-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-05-20 02:58:27.808897 dingtalk-stream-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-20 02:58:27.000000 dingtalk-stream-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 02:58:27.808897 dingtalk-stream-0.1.8/dingtalk_stream/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-20 02:58:27.000000 dingtalk-stream-0.1.8/dingtalk_stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-05-20 02:58:27.000000 dingtalk-stream-0.1.8/dingtalk_stream/chatbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-20 02:58:27.000000 dingtalk-stream-0.1.8/dingtalk_stream/credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7309 2023-05-20 02:58:27.000000 dingtalk-stream-0.1.8/dingtalk_stream/frames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-20 02:58:27.000000 dingtalk-stream-0.1.8/dingtalk_stream/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-20 02:58:27.000000 dingtalk-stream-0.1.8/dingtalk_stream/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8169 2023-05-20 02:58:27.000000 dingtalk-stream-0.1.8/dingtalk_stream/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 02:58:27.808897 dingtalk-stream-0.1.8/dingtalk_stream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-05-20 02:58:27.000000 dingtalk-stream-0.1.8/dingtalk_stream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-20 02:58:27.000000 dingtalk-stream-0.1.8/dingtalk_stream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 02:58:27.000000 dingtalk-stream-0.1.8/dingtalk_stream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-20 02:58:27.000000 dingtalk-stream-0.1.8/dingtalk_stream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-20 02:58:27.000000 dingtalk-stream-0.1.8/dingtalk_stream.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 02:58:27.808897 dingtalk-stream-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-20 02:58:27.000000 dingtalk-stream-0.1.8/setup.py
```

### Comparing `dingtalk-stream-0.1.7/LICENSE` & `dingtalk-stream-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.1.7/PKG-INFO` & `dingtalk-stream-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: dingtalk-stream
-Version: 0.1.7
-Summary: A Python package for sending messages to DingTalk chatbot
+Version: 0.1.8
+Summary: A Python library for sending messages to DingTalk chatbot
 Home-page: https://github.com/open-dingtalk/dingtalk-stream-sdk-python
 Author: Ke Jie
 Author-email: jinxi.kj@alibaba-inc.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `dingtalk-stream-0.1.7/README.md` & `dingtalk-stream-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.1.7/dingtalk_stream/chatbot.py` & `dingtalk-stream-0.1.8/dingtalk_stream/chatbot.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.1.7/dingtalk_stream/frames.py` & `dingtalk-stream-0.1.8/dingtalk_stream/frames.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.1.7/dingtalk_stream/handlers.py` & `dingtalk-stream-0.1.8/dingtalk_stream/handlers.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.1.7/dingtalk_stream/stream.py` & `dingtalk-stream-0.1.8/dingtalk_stream/stream.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.1.7/dingtalk_stream.egg-info/PKG-INFO` & `dingtalk-stream-0.1.8/dingtalk_stream.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: dingtalk-stream
-Version: 0.1.7
-Summary: A Python package for sending messages to DingTalk chatbot
+Version: 0.1.8
+Summary: A Python library for sending messages to DingTalk chatbot
 Home-page: https://github.com/open-dingtalk/dingtalk-stream-sdk-python
 Author: Ke Jie
 Author-email: jinxi.kj@alibaba-inc.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `dingtalk-stream-0.1.7/setup.py` & `dingtalk-stream-0.1.8/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name='dingtalk-stream',
-    version='0.1.7',
-    description='A Python package for sending messages to DingTalk chatbot',
+    version='0.1.8',
+    description='A Python library for sending messages to DingTalk chatbot',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/open-dingtalk/dingtalk-stream-sdk-python',
     author='Ke Jie',
     author_email='jinxi.kj@alibaba-inc.com',
     license='MIT',
     packages=['dingtalk_stream'],
```

