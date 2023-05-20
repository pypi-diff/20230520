# Comparing `tmp/requests_html2-1.0.1.tar.gz` & `tmp/requests_html2-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requests_html2-1.0.1.tar", last modified: Sat May 20 14:08:09 2023, max compression
+gzip compressed data, was "requests_html2-1.0.2.tar", last modified: Sat May 20 16:26:34 2023, max compression
```

## Comparing `requests_html2-1.0.1.tar` & `requests_html2-1.0.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      709 2023-05-20 14:05:30.323790 requests_html2-1.0.1/README.md
--rw-r--r--   0        0        0      706 2023-05-20 14:08:09.267300 requests_html2-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    34597 2023-05-19 20:42:02.854036 requests_html2-1.0.1/requests_html2.py
--rw-r--r--   0        0        0     1265 1970-01-01 00:00:00.000000 requests_html2-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      709 2023-05-20 14:05:30.323790 requests_html2-1.0.2/README.md
+-rw-r--r--   0        0        0      706 2023-05-20 16:26:34.394118 requests_html2-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0    34729 2023-05-20 15:57:54.052203 requests_html2-1.0.2/requests_html2.py
+-rw-r--r--   0        0        0     1265 1970-01-01 00:00:00.000000 requests_html2-1.0.2/PKG-INFO
```

### Comparing `requests_html2-1.0.1/README.md` & `requests_html2-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `requests_html2-1.0.1/pyproject.toml` & `requests_html2-1.0.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "requests_html2"
-version = "1.0.1"
+version = "1.0.2"
 description = "HTML Parsing for Humans"
 authors = [
     { name = "Bevis", email = "alonefire@foxmail.com" },
 ]
 dependencies = [
     "requests>=2.27.1",
     "pyquery>=1.4.3",
```

### Comparing `requests_html2-1.0.1/requests_html2.py` & `requests_html2-1.0.2/requests_html2.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,22 +33,22 @@
 cleaner.javascript = True
 cleaner.style = True
 
 useragent = None
 
 
 class FindQueryList(list):
-    def select(self, result_filter=None, first=True, default=None):
+    def select(self, result_filter=None, first=False, default=None):
         if first:
             if not self:
                 return default
             else:
                 return result_filter(self[0]) if result_filter else self[0]
         if result_filter:
-            return map(result_filter, self)
+            return FindQueryList(map(result_filter, self))
 
     def where(self, result_filter):
         return FindQueryList(filter(result_filter, self))
 
 
 # Typing.
 _Find = Union[FindQueryList["Element"], "Element"]
@@ -61,15 +61,15 @@
 _URL = str
 _RawHTML = bytes
 _Encoding = str
 _LXML = HtmlElement
 _Text = str
 _Search = Result
 _Containing = Union[str, List[str]]
-_Links = Set[str]
+_Links = FindQueryList[str]
 _Attrs = MutableMapping
 _Next = Union["HTML", List[str]]
 _NextSymbol = List[str]
 
 # Sanity checking.
 try:
     assert sys.version_info.major == 3
@@ -346,15 +346,15 @@
                         and not (href.startswith("#") and self.skip_anchors)
                         and not href.startswith(("javascript:", "mailto:"))
                     ):
                         yield href
                 except KeyError:
                     pass
 
-        return set(gen())
+        return FindQueryList(set(gen()))
 
     def _make_absolute(self, link):
         """将给定链接转换为绝对链接。"""
 
         # Parse the link with stdlib.
         parsed = urlparse(link)._asdict()
 
@@ -379,15 +379,15 @@
         (`learn more <https://www.navegabem.com/absolute-or-relative-links.html>`_).
         """
 
         def gen():
             for link in self.links:
                 yield self._make_absolute(link)
 
-        return set(gen())
+        return FindQueryList(set(gen()))
 
     @property
     def base_url(self) -> _URL:
         """The base URL for the page. Supports the ``<base>`` tag
         (`learn more <https://www.w3schools.com/tags/tag_base.asp>`_)."""
 
         # Support for <base> tag.
@@ -682,15 +682,17 @@
         """
         Convert HTMLSession.cookies for browser.newPage().setCookie
         Return a list of dict
         """
         cookies_render = []
         if isinstance(self.session.cookies, http.cookiejar.CookieJar):
             for cookie in self.session.cookies:
-                cookies_render.append(self._convert_cookiejar_to_render(cookie))
+                convert = self._convert_cookiejar_to_render(cookie)
+                convert["url"] = self.url
+                cookies_render.append(convert)
         return cookies_render
 
     def render(
         self,
         retries: int = 8,
         script: str = None,
         wait: float = 0.2,
```

### Comparing `requests_html2-1.0.1/PKG-INFO` & `requests_html2-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requests-html2
-Version: 1.0.1
+Version: 1.0.2
 Summary: HTML Parsing for Humans
 Author-Email: Bevis <alonefire@foxmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/AloneFire/requests_html2
 Project-URL: Bug tracker, https://github.com/AloneFire/requests_html2
 Requires-Python: >=3.7
 Requires-Dist: requests>=2.27.1
```

