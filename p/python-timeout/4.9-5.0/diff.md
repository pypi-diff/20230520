# Comparing `tmp/python-timeout-4.9.tar.gz` & `tmp/python-timeout-5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-timeout-4.9.tar", last modified: Fri Apr 21 11:33:58 2023, max compression
+gzip compressed data, was "python-timeout-5.0.tar", last modified: Sat May 20 18:00:26 2023, max compression
```

## Comparing `python-timeout-4.9.tar` & `python-timeout-5.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 11:33:58.252148 python-timeout-4.9/
--rw-rw-rw-   0        0        0       35 2022-03-16 16:24:46.000000 python-timeout-4.9/.gitignore
--rw-rw-rw-   0        0        0      973 2023-04-21 11:33:58.253146 python-timeout-4.9/PKG-INFO
--rw-rw-rw-   0        0        0      757 2022-05-11 17:10:57.000000 python-timeout-4.9/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 11:33:58.250148 python-timeout-4.9/python_timeout.egg-info/
--rw-rw-rw-   0        0        0      973 2023-04-21 11:33:56.000000 python-timeout-4.9/python_timeout.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2023-04-21 11:33:56.000000 python-timeout-4.9/python_timeout.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 11:33:56.000000 python-timeout-4.9/python_timeout.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-21 11:33:56.000000 python-timeout-4.9/python_timeout.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-21 11:33:56.000000 python-timeout-4.9/python_timeout.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-21 11:33:58.253146 python-timeout-4.9/setup.cfg
--rw-rw-rw-   0        0        0      394 2023-04-21 11:33:51.000000 python-timeout-4.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-21 11:33:58.251148 python-timeout-4.9/timeout/
--rw-rw-rw-   0        0        0     5817 2023-04-21 11:31:43.000000 python-timeout-4.9/timeout/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-20 18:00:26.361305 python-timeout-5.0/
+-rw-rw-rw-   0        0        0       35 2022-03-16 16:24:46.000000 python-timeout-5.0/.gitignore
+-rw-rw-rw-   0        0        0      973 2023-05-20 18:00:26.362304 python-timeout-5.0/PKG-INFO
+-rw-rw-rw-   0        0        0      757 2022-05-11 17:10:57.000000 python-timeout-5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-20 18:00:26.359306 python-timeout-5.0/python_timeout.egg-info/
+-rw-rw-rw-   0        0        0      973 2023-05-20 18:00:25.000000 python-timeout-5.0/python_timeout.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2023-05-20 18:00:26.000000 python-timeout-5.0/python_timeout.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 18:00:25.000000 python-timeout-5.0/python_timeout.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-05-20 18:00:25.000000 python-timeout-5.0/python_timeout.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-20 18:00:25.000000 python-timeout-5.0/python_timeout.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-20 18:00:26.362304 python-timeout-5.0/setup.cfg
+-rw-rw-rw-   0        0        0      413 2023-05-20 18:00:13.000000 python-timeout-5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 18:00:26.360305 python-timeout-5.0/timeout/
+-rw-rw-rw-   0        0        0     7673 2023-05-20 18:00:10.000000 python-timeout-5.0/timeout/__init__.py
```

### Comparing `python-timeout-4.9/PKG-INFO` & `python-timeout-5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-timeout
-Version: 4.9
+Version: 5.0
 Summary: Random timeout between minimum and maximum values
 Home-page: https://github.com/xjxckk/python-timeout/
 Description-Content-Type: text/markdown
 
 ### Timeout
 Random timeout between minimum and maximum values
```

### Comparing `python-timeout-4.9/README.md` & `python-timeout-5.0/README.md`

 * *Files identical despite different names*

### Comparing `python-timeout-4.9/python_timeout.egg-info/PKG-INFO` & `python-timeout-5.0/python_timeout.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-timeout
-Version: 4.9
+Version: 5.0
 Summary: Random timeout between minimum and maximum values
 Home-page: https://github.com/xjxckk/python-timeout/
 Description-Content-Type: text/markdown
 
 ### Timeout
 Random timeout between minimum and maximum values
```

