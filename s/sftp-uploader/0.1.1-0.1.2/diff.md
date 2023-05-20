# Comparing `tmp/sftp_uploader-0.1.1.tar.gz` & `tmp/sftp_uploader-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sftp_uploader-0.1.1.tar", max compression
+gzip compressed data, was "sftp_uploader-0.1.2.tar", max compression
```

## Comparing `sftp_uploader-0.1.1.tar` & `sftp_uploader-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1065 2023-05-20 07:24:26.996978 sftp_uploader-0.1.1/LICENSE
--rw-r--r--   0        0        0      212 2023-05-20 08:06:11.358843 sftp_uploader-0.1.1/README.md
--rw-r--r--   0        0        0     1196 2023-05-20 08:11:32.541097 sftp_uploader-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       33 2023-05-20 08:09:20.089658 sftp_uploader-0.1.1/sftp_uploader/__init__.py
--rw-r--r--   0        0        0       26 2023-05-20 08:09:33.845077 sftp_uploader-0.1.1/sftp_uploader/upload_to_sftp.py
--rw-r--r--   0        0        0      877 1970-01-01 00:00:00.000000 sftp_uploader-0.1.1/setup.py
--rw-r--r--   0        0        0      678 1970-01-01 00:00:00.000000 sftp_uploader-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-20 07:24:26.996978 sftp_uploader-0.1.2/LICENSE
+-rw-r--r--   0        0        0      212 2023-05-20 08:06:11.358843 sftp_uploader-0.1.2/README.md
+-rw-r--r--   0        0        0     1144 2023-05-20 08:53:49.688893 sftp_uploader-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       33 2023-05-20 08:09:20.089658 sftp_uploader-0.1.2/sftp_uploader/__init__.py
+-rw-r--r--   0        0        0       26 2023-05-20 08:47:52.416740 sftp_uploader-0.1.2/sftp_uploader/upload_to_sftp.py
+-rw-r--r--   0        0        0      967 1970-01-01 00:00:00.000000 sftp_uploader-0.1.2/setup.py
+-rw-r--r--   0        0        0     1169 1970-01-01 00:00:00.000000 sftp_uploader-0.1.2/PKG-INFO
```

### Comparing `sftp_uploader-0.1.1/LICENSE` & `sftp_uploader-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sftp_uploader-0.1.1/setup.py` & `sftp_uploader-0.1.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 {'': ['*']}
 
 install_requires = \
 ['gitpython>=3.1.31,<4.0.0', 'paramiko>=3.1.0,<4.0.0']
 
 setup_kwargs = {
     'name': 'sftp-uploader',
-    'version': '0.1.1',
-    'description': 'Script for upload files to sftp',
+    'version': '0.1.2',
+    'description': 'Package for upload data to sftp with different parametrs and with different methods',
     'long_description': '# TODO\n\n[ ] Make title, description, which problem is solve, metter of this project description\n\n[ ] Add more [classifiers](https://pypi.org/classifiers/)\n\n[ ] Add tests\n\n[ ] Add additional links to project conf\n',
     'author': 'Moonvent',
     'author_email': 'moonvent@proton.me',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'None',
+    'url': 'https://github.com/moonvent/sftp_uploader/',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.11,<4.0',
 }
```

### Comparing `sftp_uploader-0.1.1/PKG-INFO` & `sftp_uploader-0.1.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 Metadata-Version: 2.1
 Name: sftp-uploader
-Version: 0.1.1
-Summary: Script for upload files to sftp
+Version: 0.1.2
+Summary: Package for upload data to sftp with different parametrs and with different methods
+Home-page: https://github.com/moonvent/sftp_uploader/
 License: MIT
+Keywords: sftp,git
 Author: Moonvent
 Author-email: moonvent@proton.me
 Requires-Python: >=3.11,<4.0
+Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
 Requires-Dist: gitpython (>=3.1.31,<4.0.0)
 Requires-Dist: paramiko (>=3.1.0,<4.0.0)
+Project-URL: Bug Tracker, https://github.com/moonvent/sftp_uploader/issues/
+Project-URL: Documentation, https://github.com/moonvent/sftp_uploader/blob/master/README.md
+Project-URL: Repository, https://github.com/moonvent/sftp_uploader/
 Description-Content-Type: text/markdown
 
 # TODO
 
 [ ] Make title, description, which problem is solve, metter of this project description
 
 [ ] Add more [classifiers](https://pypi.org/classifiers/)
```

