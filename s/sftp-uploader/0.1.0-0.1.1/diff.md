# Comparing `tmp/sftp_uploader-0.1.0.tar.gz` & `tmp/sftp_uploader-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sftp_uploader-0.1.0.tar", max compression
+gzip compressed data, was "sftp_uploader-0.1.1.tar", max compression
```

## Comparing `sftp_uploader-0.1.0.tar` & `sftp_uploader-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,7 @@
--rw-r--r--   0        0        0     1065 2023-05-20 07:24:26.996978 sftp_uploader-0.1.0/LICENSE
--rw-r--r--   0        0        0      209 2023-05-20 07:32:36.348917 sftp_uploader-0.1.0/README.md
--rw-r--r--   0        0        0     1132 2023-05-20 07:43:21.223710 sftp_uploader-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       29 2023-05-20 07:42:49.589289 sftp_uploader-0.1.0/sftp_uploader/docs/__init__.py
--rw-r--r--   0        0        0       25 2023-05-20 07:42:47.425990 sftp_uploader-0.1.0/sftp_uploader/src/__init__.py
--rw-r--r--   0        0        0       27 2023-05-20 07:42:47.426486 sftp_uploader-0.1.0/sftp_uploader/src/test_upload_to_pypl.py
--rw-r--r--   0        0        0       26 2023-05-20 07:42:51.775135 sftp_uploader-0.1.0/sftp_uploader/tests/__init__.py
--rw-r--r--   0        0        0      940 1970-01-01 00:00:00.000000 sftp_uploader-0.1.0/setup.py
--rw-r--r--   0        0        0      675 1970-01-01 00:00:00.000000 sftp_uploader-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-20 07:24:26.996978 sftp_uploader-0.1.1/LICENSE
+-rw-r--r--   0        0        0      212 2023-05-20 08:06:11.358843 sftp_uploader-0.1.1/README.md
+-rw-r--r--   0        0        0     1196 2023-05-20 08:11:32.541097 sftp_uploader-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       33 2023-05-20 08:09:20.089658 sftp_uploader-0.1.1/sftp_uploader/__init__.py
+-rw-r--r--   0        0        0       26 2023-05-20 08:09:33.845077 sftp_uploader-0.1.1/sftp_uploader/upload_to_sftp.py
+-rw-r--r--   0        0        0      877 1970-01-01 00:00:00.000000 sftp_uploader-0.1.1/setup.py
+-rw-r--r--   0        0        0      678 1970-01-01 00:00:00.000000 sftp_uploader-0.1.1/PKG-INFO
```

### Comparing `sftp_uploader-0.1.0/LICENSE` & `sftp_uploader-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sftp_uploader-0.1.0/pyproject.toml` & `sftp_uploader-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 [project.urls]
 "Homepage" = "https://github.com/moonvent/sftp_uploader"
 "Bug Tracker" = "https://github.com/moonvent/sftp_uploader/issues"
 
 [tool.poetry]
 name = "sftp_uploader"
-version = "0.1.0"
+version = "0.1.1"
 description = "Script for upload files to sftp"
 authors = ["Moonvent <moonvent@proton.me>"]
 license = "MIT License"
 readme = "README.md"
 packages = [{include = "sftp_uploader"}]
 
 [tool.poetry.dependencies]
@@ -36,10 +36,14 @@
 [tool.poetry.group.dev.dependencies]
 debugpy = "^1.6.7"
 pynvim = "^0.4.3"
 
 [tool.poetry.group.tests.dependencies]
 pytest = "^7.3.1"
 
+
+[tool.poetry.group.pypl_upload.dependencies]
+twine = "^4.0.2"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `sftp_uploader-0.1.0/setup.py` & `sftp_uploader-0.1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['sftp_uploader',
- 'sftp_uploader.docs',
- 'sftp_uploader.src',
- 'sftp_uploader.tests']
+['sftp_uploader']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['gitpython>=3.1.31,<4.0.0', 'paramiko>=3.1.0,<4.0.0']
 
 setup_kwargs = {
     'name': 'sftp-uploader',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'Script for upload files to sftp',
-    'long_description': '# TODO\n\n[ ] Make title, description, which problem is solve, metter of this project description\n[ ] Add more [classifiers](https://pypi.org/classifiers/)\n[ ] Add tests\n[ ] Add additional links to project conf\n',
+    'long_description': '# TODO\n\n[ ] Make title, description, which problem is solve, metter of this project description\n\n[ ] Add more [classifiers](https://pypi.org/classifiers/)\n\n[ ] Add tests\n\n[ ] Add additional links to project conf\n',
     'author': 'Moonvent',
     'author_email': 'moonvent@proton.me',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `sftp_uploader-0.1.0/PKG-INFO` & `sftp_uploader-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sftp-uploader
-Version: 0.1.0
+Version: 0.1.1
 Summary: Script for upload files to sftp
 License: MIT
 Author: Moonvent
 Author-email: moonvent@proton.me
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,11 +12,14 @@
 Requires-Dist: gitpython (>=3.1.31,<4.0.0)
 Requires-Dist: paramiko (>=3.1.0,<4.0.0)
 Description-Content-Type: text/markdown
 
 # TODO
 
 [ ] Make title, description, which problem is solve, metter of this project description
+
 [ ] Add more [classifiers](https://pypi.org/classifiers/)
+
 [ ] Add tests
+
 [ ] Add additional links to project conf
```

