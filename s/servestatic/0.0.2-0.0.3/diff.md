# Comparing `tmp/servestatic-0.0.2.tar.gz` & `tmp/servestatic-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "servestatic-0.0.2.tar", last modified: Sat May 20 12:27:07 2023, max compression
+gzip compressed data, was "servestatic-0.0.3.tar", last modified: Sat May 20 12:49:14 2023, max compression
```

## Comparing `servestatic-0.0.2.tar` & `servestatic-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-05-20 12:27:07.666232 servestatic-0.0.2/
--rw-r--r--   0 mujdecisy   (501) staff       (20)      335 2023-05-20 12:27:07.666080 servestatic-0.0.2/PKG-INFO
--rw-r--r--   0 mujdecisy   (501) staff       (20)       14 2023-05-20 12:21:40.000000 servestatic-0.0.2/README.md
-drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-05-20 12:27:07.665075 servestatic-0.0.2/servestatic/
--rw-r--r--   0 mujdecisy   (501) staff       (20)      151 2023-05-20 12:25:26.000000 servestatic-0.0.2/servestatic/__main__.py
--rw-r--r--   0 mujdecisy   (501) staff       (20)     3170 2023-05-20 12:08:56.000000 servestatic-0.0.2/servestatic/server.py
-drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-05-20 12:27:07.665703 servestatic-0.0.2/servestatic.egg-info/
--rw-r--r--   0 mujdecisy   (501) staff       (20)      335 2023-05-20 12:27:07.000000 servestatic-0.0.2/servestatic.egg-info/PKG-INFO
--rw-r--r--   0 mujdecisy   (501) staff       (20)      222 2023-05-20 12:27:07.000000 servestatic-0.0.2/servestatic.egg-info/SOURCES.txt
--rw-r--r--   0 mujdecisy   (501) staff       (20)        1 2023-05-20 12:27:07.000000 servestatic-0.0.2/servestatic.egg-info/dependency_links.txt
--rw-r--r--   0 mujdecisy   (501) staff       (20)       12 2023-05-20 12:27:07.000000 servestatic-0.0.2/servestatic.egg-info/top_level.txt
--rw-r--r--   0 mujdecisy   (501) staff       (20)       38 2023-05-20 12:27:07.666277 servestatic-0.0.2/setup.cfg
--rw-r--r--   0 mujdecisy   (501) staff       (20)      677 2023-05-20 12:27:04.000000 servestatic-0.0.2/setup.py
-drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-05-20 12:27:07.665860 servestatic-0.0.2/test/
--rw-r--r--   0 mujdecisy   (501) staff       (20)      970 2023-05-20 11:40:57.000000 servestatic-0.0.2/test/test_path.py
+drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-05-20 12:49:14.752508 servestatic-0.0.3/
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     1275 2023-05-20 12:49:14.752350 servestatic-0.0.3/PKG-INFO
+-rw-r--r--   0 mujdecisy   (501) staff       (20)      955 2023-05-20 12:48:47.000000 servestatic-0.0.3/README.md
+drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-05-20 12:49:14.751340 servestatic-0.0.3/servestatic/
+-rw-r--r--   0 mujdecisy   (501) staff       (20)      151 2023-05-20 12:25:26.000000 servestatic-0.0.3/servestatic/__main__.py
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     3170 2023-05-20 12:08:56.000000 servestatic-0.0.3/servestatic/server.py
+drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-05-20 12:49:14.751981 servestatic-0.0.3/servestatic.egg-info/
+-rw-r--r--   0 mujdecisy   (501) staff       (20)     1275 2023-05-20 12:49:14.000000 servestatic-0.0.3/servestatic.egg-info/PKG-INFO
+-rw-r--r--   0 mujdecisy   (501) staff       (20)      222 2023-05-20 12:49:14.000000 servestatic-0.0.3/servestatic.egg-info/SOURCES.txt
+-rw-r--r--   0 mujdecisy   (501) staff       (20)        1 2023-05-20 12:49:14.000000 servestatic-0.0.3/servestatic.egg-info/dependency_links.txt
+-rw-r--r--   0 mujdecisy   (501) staff       (20)       12 2023-05-20 12:49:14.000000 servestatic-0.0.3/servestatic.egg-info/top_level.txt
+-rw-r--r--   0 mujdecisy   (501) staff       (20)       38 2023-05-20 12:49:14.752553 servestatic-0.0.3/setup.cfg
+-rw-r--r--   0 mujdecisy   (501) staff       (20)      677 2023-05-20 12:49:03.000000 servestatic-0.0.3/setup.py
+drwxr-xr-x   0 mujdecisy   (501) staff       (20)        0 2023-05-20 12:49:14.752133 servestatic-0.0.3/test/
+-rw-r--r--   0 mujdecisy   (501) staff       (20)      970 2023-05-20 11:40:57.000000 servestatic-0.0.3/test/test_path.py
```

### Comparing `servestatic-0.0.2/servestatic/server.py` & `servestatic-0.0.3/servestatic/server.py`

 * *Files identical despite different names*

### Comparing `servestatic-0.0.2/setup.py` & `servestatic-0.0.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 HERE = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(HERE, "README.md")) as fid:
     README = fid.read()
 
 setup(
     name="servestatic",
-    version="0.0.2",
+    version="0.0.3",
     description="static web server cli tool",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/mujdecisy/serve-static",
     keywords=["python", "static", "web", "server"],
     author="mujdecisy",
     author_email="mujdecisy@gmail.com",
```

### Comparing `servestatic-0.0.2/test/test_path.py` & `servestatic-0.0.3/test/test_path.py`

 * *Files identical despite different names*

