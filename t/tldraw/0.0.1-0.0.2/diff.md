# Comparing `tmp/tldraw-0.0.1.tar.gz` & `tmp/tldraw-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tldraw-0.0.1.tar", max compression
+gzip compressed data, was "tldraw-0.0.2.tar", max compression
```

## Comparing `tldraw-0.0.1.tar` & `tldraw-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1067 2023-04-24 08:16:11.663668 tldraw-0.0.1/LICENSE
--rw-r--r--   0        0        0      483 2023-05-03 20:18:54.308762 tldraw-0.0.1/README.md
--rw-r--r--   0        0        0      571 2023-05-03 21:17:26.584840 tldraw-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      165 2023-05-03 20:25:16.227279 tldraw-0.0.1/tldraw/__init__.py
--rw-r--r--   0        0        0     1524 2023-05-03 21:00:05.493614 tldraw-0.0.1/tldraw/tldraw.py
--rw-r--r--   0        0        0      886 2023-05-03 20:32:39.619189 tldraw-0.0.1/tldraw/tldraw_component.tsx
--rw-r--r--   0        0        0     1172 1970-01-01 00:00:00.000000 tldraw-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-24 08:16:11.663668 tldraw-0.0.2/LICENSE
+-rw-r--r--   0        0        0      589 2023-05-20 17:01:11.235178 tldraw-0.0.2/README.md
+-rw-r--r--   0        0        0      571 2023-05-20 17:01:13.518917 tldraw-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      165 2023-05-15 18:16:19.953893 tldraw-0.0.2/tldraw/__init__.py
+-rw-r--r--   0        0        0      320 2023-05-15 18:18:52.187379 tldraw-0.0.2/tldraw/comp.tsx
+-rw-r--r--   0        0        0      245 2023-05-20 16:51:27.378161 tldraw-0.0.2/tldraw/tldraw.py
+-rw-r--r--   0        0        0     1278 1970-01-01 00:00:00.000000 tldraw-0.0.2/PKG-INFO
```

### Comparing `tldraw-0.0.1/LICENSE` & `tldraw-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tldraw-0.0.1/pyproject.toml` & `tldraw-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tldraw"
-version = "0.0.1"
+version = "0.0.2"
 description = "Tldraw fo Jupyter"
 authors = ["kolibril13 <44469195+kolibril13@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.14"
```

