# Comparing `tmp/pyBIG-0.1.5.tar.gz` & `tmp/pyBIG-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyBIG-0.1.5.tar", last modified: Tue Jan 24 13:20:36 2023, max compression
+gzip compressed data, was "pyBIG-0.2.0.tar", last modified: Fri May 19 22:25:24 2023, max compression
```

## Comparing `pyBIG-0.1.5.tar` & `pyBIG-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-01-24 13:20:36.844216 pyBIG-0.1.5/
--rw-rw-rw-   0        0        0     1088 2023-01-24 12:01:18.000000 pyBIG-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     3089 2023-01-24 13:20:36.844216 pyBIG-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     2364 2023-01-24 12:01:18.000000 pyBIG-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-01-24 13:20:36.831216 pyBIG-0.1.5/pyBIG/
--rw-rw-rw-   0        0        0       51 2023-01-24 12:10:47.000000 pyBIG-0.1.5/pyBIG/__init__.py
--rw-rw-rw-   0        0        0    14050 2023-01-24 12:10:35.000000 pyBIG-0.1.5/pyBIG/big.py
-drwxrwxrwx   0        0        0        0 2023-01-24 13:20:36.843217 pyBIG-0.1.5/pyBIG.egg-info/
--rw-rw-rw-   0        0        0     3089 2023-01-24 13:20:36.000000 pyBIG-0.1.5/pyBIG.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      173 2023-01-24 13:20:36.000000 pyBIG-0.1.5/pyBIG.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-24 13:20:36.000000 pyBIG-0.1.5/pyBIG.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-01-24 13:20:36.000000 pyBIG-0.1.5/pyBIG.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-24 13:20:36.845219 pyBIG-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1172 2023-01-24 12:01:18.000000 pyBIG-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 22:25:24.816227 pyBIG-0.2.0/
+-rw-rw-rw-   0        0        0     1088 2023-01-24 12:01:18.000000 pyBIG-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     4161 2023-05-19 22:25:24.815277 pyBIG-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2897 2023-05-19 22:24:23.000000 pyBIG-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-19 22:25:24.794226 pyBIG-0.2.0/pyBIG/
+-rw-rw-rw-   0        0        0       96 2023-05-19 14:30:19.000000 pyBIG-0.2.0/pyBIG/__init__.py
+-rw-rw-rw-   0        0        0     7522 2023-05-19 14:30:03.000000 pyBIG-0.2.0/pyBIG/archive.py
+-rw-rw-rw-   0        0        0     7875 2023-05-19 14:28:40.000000 pyBIG-0.2.0/pyBIG/base_archive.py
+-rw-rw-rw-   0        0        0     8831 2023-05-19 22:23:27.000000 pyBIG-0.2.0/pyBIG/large_archive.py
+drwxrwxrwx   0        0        0        0 2023-05-19 22:25:24.813260 pyBIG-0.2.0/pyBIG.egg-info/
+-rw-rw-rw-   0        0        0     4161 2023-05-19 22:25:24.000000 pyBIG-0.2.0/pyBIG.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-05-19 22:25:24.000000 pyBIG-0.2.0/pyBIG.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 22:25:24.000000 pyBIG-0.2.0/pyBIG.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-19 22:25:24.000000 pyBIG-0.2.0/pyBIG.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-19 22:25:24.816227 pyBIG-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1173 2023-05-19 12:37:26.000000 pyBIG-0.2.0/setup.py
```

### Comparing `pyBIG-0.1.5/LICENSE` & `pyBIG-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyBIG-0.1.5/PKG-INFO` & `pyBIG-0.2.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,11 @@
-Metadata-Version: 2.1
-Name: pyBIG
-Version: 0.1.5
-Summary: A library for manipulating BIG format archives
-Home-page: https://github.com/ClementJ18/pyBIG
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # pyBIG
-Python library to programatically manipulate .big files, the archive format used in many of the game titles created by EA studios.
+Python library to programatically manipulate .big files, the archive format used in many of the game titles created by Westwood studios.
 
-This library is largely possible due to the work done by the OpenSage team ([Link](https://github.com/OpenSAGE/Docs/blob/master/file-formats/big/index.rst)). Eseentially this library is a python wrapper around the knowledge they gathered with some helper functions.
+This library is largely possible due to the work done by the OpenSage team ([Link](https://github.com/OpenSAGE/Docs/blob/master/file-formats/big/index.rst)). Essentially this library is a python wrapper around the knowledge they gathered with some helper functions.
 
 ## Installation
 
 You can get it from Pypi: https://pypi.org/project/pyBIG/
 
 ```
 pip install pyBIG
@@ -67,7 +49,16 @@
 # extract all the files in the archive
 archive.extract("output/")
 
 # load an archive from a directory
 archive = Archive.from_directory("output/")
 
 ```
+
+### Advanced
+In version 0.2.0, this library also makes the `LargeArchive` object available. This special object does not store the entire file into memory, allowing for manipulation of large files. It works essentially the same except that reading is done from the file present on disk and functions are tied to that location. Repacking is disabled since it implies that no changes are done to the file, instead use the save function.
+
+```python
+from pyBIG import LargeArchive
+
+archive = LargeArchive("test.big")
+```
```

### Comparing `pyBIG-0.1.5/setup.py` & `pyBIG-0.2.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 from setuptools import setup, find_packages
 import re
 
-version = ''
-with open('pyBIG/__init__.py') as f:
+version = ""
+with open("pyBIG/__init__.py") as f:
     version = re.search(r'^__version__\s*=\s*[\'"]([^\'"]*)[\'"]', f.read(), re.MULTILINE).group(1)
 
 if not version:
-    raise RuntimeError('version is not set')
+    raise RuntimeError("version is not set")
 
-readme = ''
-with open('README.md') as f:
+readme = ""
+with open("README.md") as f:
     readme = f.read()
 
 setup(
-    name='pyBIG',
+    name="pyBIG",
     version=version,
-    url='https://github.com/ClementJ18/pyBIG',
-    packages=find_packages(include=['pyBIG', 'pyBIG.*']),
-    description='A library for manipulating BIG format archives',
+    url="https://github.com/ClementJ18/pyBIG",
+    packages=find_packages(include=["pyBIG", "pyBIG.*"]),
+    description="A library for manipulating BIG format archives",
     long_description_content_type="text/markdown",
     long_description=readme,
     classifiers=[
-        'License :: OSI Approved :: MIT License',
-        'Intended Audience :: Developers',
-        'Natural Language :: English',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Topic :: Software Development :: Libraries',
-        'Topic :: Software Development :: Libraries :: Python Modules',
-        'Topic :: Utilities',
-    ]
+        "License :: OSI Approved :: MIT License",
+        "Intended Audience :: Developers",
+        "Natural Language :: English",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Topic :: Software Development :: Libraries",
+        "Topic :: Software Development :: Libraries :: Python Modules",
+        "Topic :: Utilities",
+    ],
 )
```

