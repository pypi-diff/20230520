# Comparing `tmp/wikiscrape-0.1.0.tar.gz` & `tmp/wikiscrape-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wikiscrape-0.1.0.tar", max compression
+gzip compressed data, was "wikiscrape-0.2.1.tar", max compression
```

## Comparing `wikiscrape-0.1.0.tar` & `wikiscrape-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      584 2023-05-19 22:37:14.132935 wikiscrape-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       58 2023-05-19 22:15:26.142574 wikiscrape-0.1.0/README.md
--rw-r--r--   0        0        0      102 2023-05-19 22:30:00.231284 wikiscrape-0.1.0/wikiscrape/__init__.py
--rw-r--r--   0        0        0      772 2023-05-19 22:23:38.068978 wikiscrape-0.1.0/wikiscrape/markdown.py
--rw-r--r--   0        0        0      896 2023-05-19 22:29:21.670918 wikiscrape-0.1.0/wikiscrape/wikipage.py
--rw-r--r--   0        0        0      486 1970-01-01 00:00:00.000000 wikiscrape-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      661 2023-05-20 15:53:34.608059 wikiscrape-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       58 2023-05-19 22:15:26.142574 wikiscrape-0.2.1/README.md
+-rw-r--r--   0        0        0      102 2023-05-19 22:41:43.658345 wikiscrape-0.2.1/wikiscrape/__init__.py
+-rw-r--r--   0        0        0      772 2023-05-19 22:41:43.658345 wikiscrape-0.2.1/wikiscrape/markdown.py
+-rw-r--r--   0        0        0     1132 2023-05-20 15:41:09.549133 wikiscrape-0.2.1/wikiscrape/wikipage.py
+-rw-r--r--   0        0        0      576 1970-01-01 00:00:00.000000 wikiscrape-0.2.1/PKG-INFO
```

### Comparing `wikiscrape-0.1.0/wikiscrape/markdown.py` & `wikiscrape-0.2.1/wikiscrape/markdown.py`

 * *Files identical despite different names*

### Comparing `wikiscrape-0.1.0/wikiscrape/wikipage.py` & `wikiscrape-0.2.1/wikiscrape/wikipage.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import requests
+from bs4 import BeautifulSoup
 from .markdown import Markdown as md
 
 
 class Wikipage:
     def __init__(self, title):
         self.title = title
 
@@ -25,12 +27,21 @@
     def is_disambiguated(self):
         return self.exists and "(" in self.title
 
     @property
     def is_redlink(self):
         return "not exist" in self.title
 
-    def derive_subject(self):
+    @property
+    def soup(self):
+        return BeautifulSoup(self.text, "html.parser")
+
+    @property
+    def subject(self):
         return self.title.split(" (")[0]
 
+    @property
+    def text(self):
+        return requests.get(self.abs_url).text
+
     def to_link(self, alias=None):
         return md.a(self.title) if not alias else md.a(self.title, alias)
```

