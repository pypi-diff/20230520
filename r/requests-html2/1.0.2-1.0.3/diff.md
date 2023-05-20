# Comparing `tmp/requests_html2-1.0.2.tar.gz` & `tmp/requests_html2-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requests_html2-1.0.2.tar", last modified: Sat May 20 16:26:34 2023, max compression
+gzip compressed data, was "requests_html2-1.0.3.tar", last modified: Sat May 20 17:15:05 2023, max compression
```

## Comparing `requests_html2-1.0.2.tar` & `requests_html2-1.0.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      709 2023-05-20 14:05:30.323790 requests_html2-1.0.2/README.md
--rw-r--r--   0        0        0      706 2023-05-20 16:26:34.394118 requests_html2-1.0.2/pyproject.toml
--rw-r--r--   0        0        0    34729 2023-05-20 15:57:54.052203 requests_html2-1.0.2/requests_html2.py
--rw-r--r--   0        0        0     1265 1970-01-01 00:00:00.000000 requests_html2-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      709 2023-05-20 14:05:30.323790 requests_html2-1.0.3/README.md
+-rw-r--r--   0        0        0      706 2023-05-20 17:15:05.406946 requests_html2-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0    34846 2023-05-20 17:10:26.838207 requests_html2-1.0.3/requests_html2.py
+-rw-r--r--   0        0        0     1265 1970-01-01 00:00:00.000000 requests_html2-1.0.3/PKG-INFO
```

### Comparing `requests_html2-1.0.2/README.md` & `requests_html2-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `requests_html2-1.0.2/pyproject.toml` & `requests_html2-1.0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "requests_html2"
-version = "1.0.2"
+version = "1.0.3"
 description = "HTML Parsing for Humans"
 authors = [
     { name = "Bevis", email = "alonefire@foxmail.com" },
 ]
 dependencies = [
     "requests>=2.27.1",
     "pyquery>=1.4.3",
```

### Comparing `requests_html2-1.0.2/requests_html2.py` & `requests_html2-1.0.3/requests_html2.py`

 * *Files 1% similar despite different names*

```diff
@@ -687,14 +687,18 @@
         if isinstance(self.session.cookies, http.cookiejar.CookieJar):
             for cookie in self.session.cookies:
                 convert = self._convert_cookiejar_to_render(cookie)
                 convert["url"] = self.url
                 cookies_render.append(convert)
         return cookies_render
 
+    def close_page(self):
+        if self.page:
+            self.session.loop.run_until_complete(self.page.close())
+
     def render(
         self,
         retries: int = 8,
         script: str = None,
         wait: float = 0.2,
         scrolldown=False,
         sleep: int = 0,
```

### Comparing `requests_html2-1.0.2/PKG-INFO` & `requests_html2-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requests-html2
-Version: 1.0.2
+Version: 1.0.3
 Summary: HTML Parsing for Humans
 Author-Email: Bevis <alonefire@foxmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/AloneFire/requests_html2
 Project-URL: Bug tracker, https://github.com/AloneFire/requests_html2
 Requires-Python: >=3.7
 Requires-Dist: requests>=2.27.1
```

