# Comparing `tmp/wsgi_lithium-0.1.0.tar.gz` & `tmp/wsgi_lithium-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wsgi_lithium-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "wsgi_lithium-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `wsgi_lithium-0.1.0.tar` & `wsgi_lithium-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     4336 2023-05-20 02:37:14.064353 wsgi_lithium-0.1.0/.gitignore
--rw-r--r--   0        0        0     1079 2023-05-20 02:26:08.402988 wsgi_lithium-0.1.0/LICENSE
--rw-r--r--   0        0        0      315 2023-05-20 03:48:48.259082 wsgi_lithium-0.1.0/README.md
--rw-r--r--   0        0        0      583 2023-05-20 03:45:50.332584 wsgi_lithium-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1644 2023-05-20 03:35:24.187365 wsgi_lithium-0.1.0/wsgi_lithium/__init__.py
--rw-r--r--   0        0        0     5118 2023-05-20 02:59:37.057761 wsgi_lithium-0.1.0/wsgi_lithium/load_wsgiapp.py
--rw-r--r--   0        0        0      673 1970-01-01 00:00:00.000000 wsgi_lithium-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     4336 2023-05-20 02:37:14.064353 wsgi_lithium-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1079 2023-05-20 02:26:08.402988 wsgi_lithium-0.2.0/LICENSE
+-rw-r--r--   0        0        0      360 2023-05-20 19:06:01.544901 wsgi_lithium-0.2.0/README.md
+-rw-r--r--   0        0        0      583 2023-05-20 19:05:18.592720 wsgi_lithium-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2576 2023-05-20 19:03:23.456212 wsgi_lithium-0.2.0/wsgi_lithium/__init__.py
+-rw-r--r--   0        0        0     5993 2023-05-20 19:03:13.100164 wsgi_lithium-0.2.0/wsgi_lithium/gunicorn_utils.py
+-rw-r--r--   0        0        0      718 1970-01-01 00:00:00.000000 wsgi_lithium-0.2.0/PKG-INFO
```

### Comparing `wsgi_lithium-0.1.0/.gitignore` & `wsgi_lithium-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `wsgi_lithium-0.1.0/LICENSE` & `wsgi_lithium-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wsgi_lithium-0.1.0/pyproject.toml` & `wsgi_lithium-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "wsgi_lithium"
 authors = [{name = "Léo El Amri", email = "leo@superlel.me"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License"]
-version = "0.1.0"
+version = "0.2.0"
 description = "An HTTP to WSGI server that relies on Python's included batteries"
 readme = "README.md"
 requires-python = ">=3.7"
 
 [project.urls]
 repository = "https://github.com/lel-amri/wsgi-lithium"
```

### Comparing `wsgi_lithium-0.1.0/wsgi_lithium/load_wsgiapp.py` & `wsgi_lithium-0.2.0/wsgi_lithium/gunicorn_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 # OTHER DEALINGS IN THE SOFTWARE.
 
 
 import ast
 import importlib
 import logging
 import os
+import socket
 import sys
 import traceback
 
 
 class AppImportError(Exception):
     """ Exception raised when loading an application """
 
@@ -142,7 +143,38 @@
 
     if app is None:
         raise AppImportError("Failed to find application object: %r" % obj)
 
     if not callable(app):
         raise AppImportError("Application object must be callable.")
     return app
+
+
+def parse_address(netloc, default_port='8000'):
+    if netloc.startswith("tcp://"):
+        netloc = netloc.split("tcp://")[1]
+    host, port = netloc, default_port
+
+    if '[' in netloc and ']' in netloc:
+        host = netloc.split(']')[0][1:]
+        port = (netloc.split(']:') + [default_port])[1]
+    elif ':' in netloc:
+        host, port = (netloc.split(':') + [default_port])[:2]
+    elif netloc == "":
+        host, port = "0.0.0.0", default_port
+
+    try:
+        port = int(port)
+    except ValueError:
+        raise RuntimeError("%r is not a valid port number." % port)
+
+    return host.lower(), port
+
+
+def is_ipv6(addr):
+    try:
+        socket.inet_pton(socket.AF_INET6, addr)
+    except socket.error:  # not a valid address
+        return False
+    except ValueError:  # ipv6 not supported on this platform
+        return False
+    return True
```

