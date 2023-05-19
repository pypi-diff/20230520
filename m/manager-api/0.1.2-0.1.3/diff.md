# Comparing `tmp/manager-api-0.1.2.tar.gz` & `tmp/manager-api-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manager-api-0.1.2.tar", last modified: Thu Apr  6 10:06:30 2023, max compression
+gzip compressed data, was "manager-api-0.1.3.tar", last modified: Fri May 19 21:34:14 2023, max compression
```

## Comparing `manager-api-0.1.2.tar` & `manager-api-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 kirk      (1000) kirk      (1001)        0 2023-04-06 10:06:30.113206 manager-api-0.1.2/
--rw-r--r--   0 kirk      (1000) kirk      (1001)     1072 2023-01-07 17:10:23.000000 manager-api-0.1.2/LICENSE
--rw-r--r--   0 kirk      (1000) kirk      (1001)      715 2023-04-06 10:06:30.113206 manager-api-0.1.2/PKG-INFO
--rw-r--r--   0 kirk      (1000) kirk      (1001)     1127 2023-02-04 17:00:52.000000 manager-api-0.1.2/README.md
-drwxr-xr-x   0 kirk      (1000) kirk      (1001)        0 2023-04-06 10:06:30.113206 manager-api-0.1.2/manager_api/
--rwxr-xr-x   0 kirk      (1000) kirk      (1001)     2685 2023-04-06 09:59:43.000000 manager-api-0.1.2/manager_api/__init__.py
--rw-r--r--   0 kirk      (1000) kirk      (1001)     5335 2023-04-04 12:01:14.000000 manager-api-0.1.2/manager_api/enums.py
--rw-r--r--   0 kirk      (1000) kirk      (1001)   135911 2023-04-04 12:01:14.000000 manager-api-0.1.2/manager_api/model.py
--rw-r--r--   0 kirk      (1000) kirk      (1001)     3902 2023-04-06 10:04:38.000000 manager-api-0.1.2/manager_api/object.py
-drwxr-xr-x   0 kirk      (1000) kirk      (1001)        0 2023-04-06 10:06:30.113206 manager-api-0.1.2/manager_api.egg-info/
--rw-r--r--   0 kirk      (1000) kirk      (1001)      715 2023-04-06 10:06:30.000000 manager-api-0.1.2/manager_api.egg-info/PKG-INFO
--rw-r--r--   0 kirk      (1000) kirk      (1001)      288 2023-04-06 10:06:30.000000 manager-api-0.1.2/manager_api.egg-info/SOURCES.txt
--rw-r--r--   0 kirk      (1000) kirk      (1001)        1 2023-04-06 10:06:30.000000 manager-api-0.1.2/manager_api.egg-info/dependency_links.txt
--rw-r--r--   0 kirk      (1000) kirk      (1001)       17 2023-04-06 10:06:30.000000 manager-api-0.1.2/manager_api.egg-info/requires.txt
--rw-r--r--   0 kirk      (1000) kirk      (1001)       12 2023-04-06 10:06:30.000000 manager-api-0.1.2/manager_api.egg-info/top_level.txt
--rw-r--r--   0 kirk      (1000) kirk      (1001)       38 2023-04-06 10:06:30.113206 manager-api-0.1.2/setup.cfg
--rw-r--r--   0 kirk      (1000) kirk      (1001)      877 2023-04-06 10:05:02.000000 manager-api-0.1.2/setup.py
+drwxr-xr-x   0 kirk      (1000) kirk      (1001)        0 2023-05-19 21:34:14.800201 manager-api-0.1.3/
+-rw-r--r--   0 kirk      (1000) kirk      (1001)     1072 2023-01-07 17:10:23.000000 manager-api-0.1.3/LICENSE
+-rw-r--r--   0 kirk      (1000) kirk      (1001)      716 2023-05-19 21:34:14.800201 manager-api-0.1.3/PKG-INFO
+-rw-r--r--   0 kirk      (1000) kirk      (1001)     1127 2023-02-04 17:00:52.000000 manager-api-0.1.3/README.md
+drwxr-xr-x   0 kirk      (1000) kirk      (1001)        0 2023-05-19 21:34:14.800201 manager-api-0.1.3/manager_api/
+-rwxr-xr-x   0 kirk      (1000) kirk      (1001)     2741 2023-05-19 21:26:58.000000 manager-api-0.1.3/manager_api/__init__.py
+-rw-r--r--   0 kirk      (1000) kirk      (1001)     5335 2023-04-04 12:01:14.000000 manager-api-0.1.3/manager_api/enums.py
+-rw-r--r--   0 kirk      (1000) kirk      (1001)   135911 2023-04-04 12:01:14.000000 manager-api-0.1.3/manager_api/model.py
+-rw-r--r--   0 kirk      (1000) kirk      (1001)     4455 2023-05-19 21:28:32.000000 manager-api-0.1.3/manager_api/object.py
+drwxr-xr-x   0 kirk      (1000) kirk      (1001)        0 2023-05-19 21:34:14.800201 manager-api-0.1.3/manager_api.egg-info/
+-rw-r--r--   0 kirk      (1000) kirk      (1001)      716 2023-05-19 21:34:14.000000 manager-api-0.1.3/manager_api.egg-info/PKG-INFO
+-rw-r--r--   0 kirk      (1000) kirk      (1001)      288 2023-05-19 21:34:14.000000 manager-api-0.1.3/manager_api.egg-info/SOURCES.txt
+-rw-r--r--   0 kirk      (1000) kirk      (1001)        1 2023-05-19 21:34:14.000000 manager-api-0.1.3/manager_api.egg-info/dependency_links.txt
+-rw-r--r--   0 kirk      (1000) kirk      (1001)       17 2023-05-19 21:34:14.000000 manager-api-0.1.3/manager_api.egg-info/requires.txt
+-rw-r--r--   0 kirk      (1000) kirk      (1001)       12 2023-05-19 21:34:14.000000 manager-api-0.1.3/manager_api.egg-info/top_level.txt
+-rw-r--r--   0 kirk      (1000) kirk      (1001)       38 2023-05-19 21:34:14.800201 manager-api-0.1.3/setup.cfg
+-rw-r--r--   0 kirk      (1000) kirk      (1001)      877 2023-05-19 21:29:45.000000 manager-api-0.1.3/setup.py
```

### Comparing `manager-api-0.1.2/LICENSE` & `manager-api-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `manager-api-0.1.2/PKG-INFO` & `manager-api-0.1.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: manager-api
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python module to access the API provided by Manager accounting software 
 Home-page: https://github.com/isotherm/python-manager-api/
 Author: Kirk Meyer
 Author-email: kirk.meyer@alpaxo.com
 License: MIT
-Description: UNKNOWN
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+License-File: LICENSE
```

### Comparing `manager-api-0.1.2/README.md` & `manager-api-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `manager-api-0.1.2/manager_api/__init__.py` & `manager-api-0.1.3/manager_api/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -54,24 +54,25 @@
                 assert(base.Guid == item["Key"])
                 setattr(self, name, base)
             except (AssertionError, AttributeError):
                 continue
 
     def request(self, method, url, **kwargs):
         kwargs["auth"] = self._auth
-        url = urljoin(self._api_url, url)
-        url = url.rstrip("/") + ".json"
+        url = urljoin(self._api_url, url).rstrip("/")
+        if "-attachment?" not in url:
+            url += ".json"
         return super().request(method, url, **kwargs)
 
-    def _get_url(self, action, uuid=None):
+    def _get_url(self, action, uuid=None, field=b"\xc2\x0c"):
         action = re.sub(r'(?<!^)(?=[A-Z])', '-', action).lower()
         name = self._name.encode()
         protobuf = b"\xa2\x06" + bytes([len(name)]) + name
         if uuid:
-            protobuf += b"\xc2\x0c\x12"
+            protobuf += field + b"\x12"
             protobuf += b"\x09" + uuid.bytes_le[:8]
             protobuf += b"\x11" + uuid.bytes_le[8:]
         protobuf = _b64encode(protobuf)
         return urljoin(self._url, f"{action}?{protobuf}")
 
 
 __all__ = [
```

### Comparing `manager-api-0.1.2/manager_api/enums.py` & `manager-api-0.1.3/manager_api/enums.py`

 * *Files identical despite different names*

### Comparing `manager-api-0.1.2/manager_api/model.py` & `manager-api-0.1.3/manager_api/model.py`

 * *Files identical despite different names*

### Comparing `manager-api-0.1.2/manager_api/object.py` & `manager-api-0.1.3/manager_api/object.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 import json
+import mimetypes
+import os
 from requests import Session
 from typing import ClassVar, Dict, Optional
 from uuid import UUID
 
 from pydantic import BaseModel
 
 
@@ -45,15 +47,18 @@
         kwargs.update({"Key": Key})
         return super().__init__(**kwargs)
 
     def __hash__(self):
         return hash(self.Key or self.Guid)
 
     def __eq__(self, other):
-        return self.Key == other.Key
+        try:
+            return self.Key == other.Key
+        except AttributeError:
+            return False
 
     def _read_if_necessary(self, attr):
         if attr in super().__getattribute__("__fields__"):
             fs = super().__getattribute__("__fields_set__")
             if fs.difference({"Name"}).issubset({"Key", "Timestamp"}) and attr not in fs:
                 self.read()
 
@@ -62,15 +67,15 @@
         return super().__getattribute__(attr)
 
     def __setattr__(self, attr, value):
         super().__getattribute__("_read_if_necessary")(attr)
         super().__setattr__(attr, value)
 
     def __class_getitem__(cls, key):
-        items = [i for i in cls.list() if key == i.Name.split(" - ", 1)[0]]
+        items = [i for i in cls.list() if key == (i.Name or "").split(" - ", 1)[0].split(" — ", 1)[0]]
         if not items:
             raise KeyError(f"Object not found with name {key}")
         elif len(items) != 1:
             raise KeyError(f"More than one object found with name {key}")
         else:
             return items[0]
 
@@ -118,7 +123,17 @@
     def delete(self):
         response = self._session.delete(self._path)
         self._parse_response(response)
         self.Key = None
 
     def get_url(self):
         return self._session._get_url(f"{type(self).__name__}View", self.Key)
+
+    def attach_file(self, filename):
+        url = self._session._get_url("NewAttachment", self.Key, b"\x0a")
+        headers = {
+            "Content-Type": "application/octet-stream",
+            "X-File-Name": os.path.basename(filename),
+            "X-File-Type": mimetypes.guess_type(filename)[0],
+        }
+        with open(filename, "rb") as fp:
+            self._session.post(url, data=fp.read(), headers=headers)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `manager-api-0.1.2/manager_api.egg-info/PKG-INFO` & `manager-api-0.1.3/manager_api.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: manager-api
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python module to access the API provided by Manager accounting software 
 Home-page: https://github.com/isotherm/python-manager-api/
 Author: Kirk Meyer
 Author-email: kirk.meyer@alpaxo.com
 License: MIT
-Description: UNKNOWN
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+License-File: LICENSE
```

### Comparing `manager-api-0.1.2/setup.py` & `manager-api-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 setup(
     name='manager-api',
     description='Python module to access the API provided by Manager accounting software ',
     url='https://github.com/isotherm/python-manager-api/',
-    version='0.1.2',
+    version='0.1.3',
     author=u'Kirk Meyer',
     author_email='kirk.meyer@alpaxo.com',
     license='MIT',
     platforms='any',
     packages=[
         'manager_api'
     ],
```

