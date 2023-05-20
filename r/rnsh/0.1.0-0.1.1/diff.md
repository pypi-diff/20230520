# Comparing `tmp/rnsh-0.1.0.tar.gz` & `tmp/rnsh-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rnsh-0.1.0.tar", max compression
+gzip compressed data, was "rnsh-0.1.1.tar", max compression
```

## Comparing `rnsh-0.1.0.tar` & `rnsh-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1105 2023-02-11 05:21:53.643929 rnsh-0.1.0/LICENSE
--rw-r--r--   0        0        0    11943 2023-02-25 11:21:04.980385 rnsh-0.1.0/README.md
--rw-r--r--   0        0        0      799 2023-05-12 14:08:15.604382 rnsh-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1708 2023-05-11 18:54:53.778369 rnsh-0.1.0/rnsh/__init__.py
--rw-r--r--   0        0        0     5806 2023-02-23 12:37:08.619322 rnsh-0.1.0/rnsh/args.py
--rw-r--r--   0        0        0      798 2023-02-17 16:48:38.181439 rnsh-0.1.0/rnsh/exception.py
--rw-r--r--   0        0        0      817 2023-02-19 00:35:54.411700 rnsh-0.1.0/rnsh/helpers.py
--rw-r--r--   0        0        0    14698 2023-05-11 18:27:14.823616 rnsh-0.1.0/rnsh/initiator.py
--rw-r--r--   0        0        0     7255 2023-05-11 18:27:14.823616 rnsh-0.1.0/rnsh/listener.py
--rw-r--r--   0        0        0      644 2023-02-23 12:37:08.623322 rnsh-0.1.0/rnsh/loop.py
--rw-r--r--   0        0        0    25592 2023-02-18 14:10:38.940197 rnsh-0.1.0/rnsh/process.py
--rw-r--r--   0        0        0     4206 2023-03-08 22:54:16.949580 rnsh-0.1.0/rnsh/protocol.py
--rw-r--r--   0        0        0     7661 2023-02-18 06:09:41.069929 rnsh-0.1.0/rnsh/retry.py
--rw-r--r--   0        0        0     5749 2023-05-11 18:27:14.823616 rnsh-0.1.0/rnsh/rnsh.py
--rw-r--r--   0        0        0     5225 2023-02-18 14:10:38.940197 rnsh-0.1.0/rnsh/rnslogging.py
--rw-r--r--   0        0        0    15334 2023-03-08 22:54:16.949580 rnsh-0.1.0/rnsh/session.py
--rw-r--r--   0        0        0     1609 2023-02-11 14:06:05.513301 rnsh-0.1.0/rnsh/testlogging.py
--rw-r--r--   0        0        0    12618 1970-01-01 00:00:00.000000 rnsh-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1105 2023-02-11 05:21:53.643929 rnsh-0.1.1/LICENSE
+-rw-r--r--   0        0        0    11943 2023-02-25 11:21:04.980385 rnsh-0.1.1/README.md
+-rw-r--r--   0        0        0      799 2023-05-20 11:18:26.753427 rnsh-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1708 2023-05-11 18:54:53.778369 rnsh-0.1.1/rnsh/__init__.py
+-rw-r--r--   0        0        0     5806 2023-02-23 12:37:08.619322 rnsh-0.1.1/rnsh/args.py
+-rw-r--r--   0        0        0      798 2023-02-17 16:48:38.181439 rnsh-0.1.1/rnsh/exception.py
+-rw-r--r--   0        0        0      817 2023-02-19 00:35:54.411700 rnsh-0.1.1/rnsh/helpers.py
+-rw-r--r--   0        0        0    14698 2023-05-11 18:27:14.823616 rnsh-0.1.1/rnsh/initiator.py
+-rw-r--r--   0        0        0     7255 2023-05-11 18:27:14.823616 rnsh-0.1.1/rnsh/listener.py
+-rw-r--r--   0        0        0      644 2023-02-23 12:37:08.623322 rnsh-0.1.1/rnsh/loop.py
+-rw-r--r--   0        0        0    25592 2023-02-18 14:10:38.940197 rnsh-0.1.1/rnsh/process.py
+-rw-r--r--   0        0        0     4206 2023-03-08 22:54:16.949580 rnsh-0.1.1/rnsh/protocol.py
+-rw-r--r--   0        0        0     7661 2023-02-18 06:09:41.069929 rnsh-0.1.1/rnsh/retry.py
+-rw-r--r--   0        0        0     5749 2023-05-11 18:27:14.823616 rnsh-0.1.1/rnsh/rnsh.py
+-rw-r--r--   0        0        0     5225 2023-02-18 14:10:38.940197 rnsh-0.1.1/rnsh/rnslogging.py
+-rw-r--r--   0        0        0    15334 2023-03-08 22:54:16.949580 rnsh-0.1.1/rnsh/session.py
+-rw-r--r--   0        0        0     1609 2023-02-11 14:06:05.513301 rnsh-0.1.1/rnsh/testlogging.py
+-rw-r--r--   0        0        0    12618 1970-01-01 00:00:00.000000 rnsh-0.1.1/PKG-INFO
```

### Comparing `rnsh-0.1.0/LICENSE` & `rnsh-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rnsh-0.1.0/README.md` & `rnsh-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `rnsh-0.1.0/pyproject.toml` & `rnsh-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "rnsh"
-version = "0.1.0"
+version = "0.1.1"
 description = "Shell over Reticulum"
 authors = ["acehoss <acehoss@acehoss.net>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 docopt = "^0.6.2"
-rns = "^0.5.2"
+rns = "^0.5.3"
 # rns = { git = "https://github.com/acehoss/Reticulum.git", branch = "feature/channel" }
 # rns = { path = "../Reticulum/", develop = true }
 tomli = "^2.0.1"
 
 [tool.poetry.scripts]
 rnsh = 'rnsh.rnsh:rnsh_cli'
```

### Comparing `rnsh-0.1.0/rnsh/__init__.py` & `rnsh-0.1.1/rnsh/__init__.py`

 * *Files identical despite different names*

### Comparing `rnsh-0.1.0/rnsh/args.py` & `rnsh-0.1.1/rnsh/args.py`

 * *Files identical despite different names*

### Comparing `rnsh-0.1.0/rnsh/exception.py` & `rnsh-0.1.1/rnsh/exception.py`

 * *Files identical despite different names*

### Comparing `rnsh-0.1.0/rnsh/helpers.py` & `rnsh-0.1.1/rnsh/helpers.py`

 * *Files identical despite different names*

### Comparing `rnsh-0.1.0/rnsh/initiator.py` & `rnsh-0.1.1/rnsh/initiator.py`

 * *Files identical despite different names*

### Comparing `rnsh-0.1.0/rnsh/listener.py` & `rnsh-0.1.1/rnsh/listener.py`

 * *Files identical despite different names*

### Comparing `rnsh-0.1.0/rnsh/loop.py` & `rnsh-0.1.1/rnsh/loop.py`

 * *Files identical despite different names*

### Comparing `rnsh-0.1.0/rnsh/process.py` & `rnsh-0.1.1/rnsh/process.py`

 * *Files identical despite different names*

### Comparing `rnsh-0.1.0/rnsh/protocol.py` & `rnsh-0.1.1/rnsh/protocol.py`

 * *Files identical despite different names*

### Comparing `rnsh-0.1.0/rnsh/retry.py` & `rnsh-0.1.1/rnsh/retry.py`

 * *Files identical despite different names*

### Comparing `rnsh-0.1.0/rnsh/rnsh.py` & `rnsh-0.1.1/rnsh/rnsh.py`

 * *Files identical despite different names*

### Comparing `rnsh-0.1.0/rnsh/rnslogging.py` & `rnsh-0.1.1/rnsh/rnslogging.py`

 * *Files identical despite different names*

### Comparing `rnsh-0.1.0/rnsh/session.py` & `rnsh-0.1.1/rnsh/session.py`

 * *Files identical despite different names*

### Comparing `rnsh-0.1.0/rnsh/testlogging.py` & `rnsh-0.1.1/rnsh/testlogging.py`

 * *Files identical despite different names*

### Comparing `rnsh-0.1.0/PKG-INFO` & `rnsh-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: rnsh
-Version: 0.1.0
+Version: 0.1.1
 Summary: Shell over Reticulum
 License: MIT
 Author: acehoss
 Author-email: acehoss@acehoss.net
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: docopt (>=0.6.2,<0.7.0)
-Requires-Dist: rns (>=0.5.2,<0.6.0)
+Requires-Dist: rns (>=0.5.3,<0.6.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # `r n s h`  Shell over Reticulum 
 [![CI](https://github.com/acehoss/rnsh/actions/workflows/python-package.yml/badge.svg)](https://github.com/acehoss/rnsh/actions/workflows/python-package.yml) 
 [![Release](https://github.com/acehoss/rnsh/actions/workflows/python-publish.yml/badge.svg)](https://github.com/acehoss/rnsh/actions/workflows/python-publish.yml) 
 [![PyPI version](https://badge.fury.io/py/rnsh.svg)](https://badge.fury.io/py/rnsh)
```

