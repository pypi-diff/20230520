# Comparing `tmp/sftp_uploader-0.1.3.tar.gz` & `tmp/sftp_uploader-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sftp_uploader-0.1.3.tar", max compression
+gzip compressed data, was "sftp_uploader-0.1.4.tar", max compression
```

## Comparing `sftp_uploader-0.1.3.tar` & `sftp_uploader-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1065 2023-05-20 07:24:26.996978 sftp_uploader-0.1.3/LICENSE
--rw-r--r--   0        0        0      212 2023-05-20 08:06:11.358843 sftp_uploader-0.1.3/README.md
--rw-r--r--   0        0        0     1144 2023-05-20 09:04:50.468282 sftp_uploader-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       79 2023-05-20 09:03:36.366593 sftp_uploader-0.1.3/sftp_uploader/__init__.py
--rw-r--r--   0        0        0       26 2023-05-20 08:47:52.416740 sftp_uploader-0.1.3/sftp_uploader/upload_to_sftp.py
--rw-r--r--   0        0        0      967 1970-01-01 00:00:00.000000 sftp_uploader-0.1.3/setup.py
--rw-r--r--   0        0        0     1169 1970-01-01 00:00:00.000000 sftp_uploader-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-20 07:24:26.996978 sftp_uploader-0.1.4/LICENSE
+-rw-r--r--   0        0        0      212 2023-05-20 08:06:11.358843 sftp_uploader-0.1.4/README.md
+-rw-r--r--   0        0        0     1144 2023-05-20 09:18:39.040884 sftp_uploader-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       66 2023-05-20 09:19:40.158272 sftp_uploader-0.1.4/sftp_uploader/__init__.py
+-rw-r--r--   0        0        0       26 2023-05-20 08:47:52.416740 sftp_uploader-0.1.4/sftp_uploader/upload_to_sftp.py
+-rw-r--r--   0        0        0      967 1970-01-01 00:00:00.000000 sftp_uploader-0.1.4/setup.py
+-rw-r--r--   0        0        0     1169 1970-01-01 00:00:00.000000 sftp_uploader-0.1.4/PKG-INFO
```

### Comparing `sftp_uploader-0.1.3/LICENSE` & `sftp_uploader-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sftp_uploader-0.1.3/pyproject.toml` & `sftp_uploader-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sftp_uploader"
-version = "0.1.3"
+version = "0.1.4"
 description = "Package for upload data to sftp with different parametrs and with different methods"
 
 authors = ["Moonvent <moonvent@proton.me>"]
 
 license = "MIT"
 readme = "README.md"
```

### Comparing `sftp_uploader-0.1.3/setup.py` & `sftp_uploader-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['gitpython>=3.1.31,<4.0.0', 'paramiko>=3.1.0,<4.0.0']
 
 setup_kwargs = {
     'name': 'sftp-uploader',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': 'Package for upload data to sftp with different parametrs and with different methods',
     'long_description': '# TODO\n\n[ ] Make title, description, which problem is solve, metter of this project description\n\n[ ] Add more [classifiers](https://pypi.org/classifiers/)\n\n[ ] Add tests\n\n[ ] Add additional links to project conf\n',
     'author': 'Moonvent',
     'author_email': 'moonvent@proton.me',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/moonvent/sftp_uploader/',
```

### Comparing `sftp_uploader-0.1.3/PKG-INFO` & `sftp_uploader-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sftp-uploader
-Version: 0.1.3
+Version: 0.1.4
 Summary: Package for upload data to sftp with different parametrs and with different methods
 Home-page: https://github.com/moonvent/sftp_uploader/
 License: MIT
 Keywords: sftp,git
 Author: Moonvent
 Author-email: moonvent@proton.me
 Requires-Python: >=3.11,<4.0
```

