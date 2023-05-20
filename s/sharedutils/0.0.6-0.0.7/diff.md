# Comparing `tmp/sharedutils-0.0.6.tar.gz` & `tmp/sharedutils-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sharedutils-0.0.6.tar", last modified: Mon Oct 31 09:18:46 2022, max compression
+gzip compressed data, was "sharedutils-0.0.7.tar", last modified: Sat May 20 10:35:04 2023, max compression
```

## Comparing `sharedutils-0.0.6.tar` & `sharedutils-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,14 @@
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-31 09:18:46.823777 sharedutils-0.0.6/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      137 2022-08-06 21:36:11.000000 sharedutils-0.0.6/.deepsource.toml
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1928 2022-07-17 10:06:29.000000 sharedutils-0.0.6/.gitignore
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1348 2022-07-17 10:06:29.000000 sharedutils-0.0.6/LICENSE
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1231 2022-10-31 09:18:46.821240 sharedutils-0.0.6/PKG-INFO
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      452 2022-07-17 11:38:48.000000 sharedutils-0.0.6/README.md
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       68 2022-07-17 10:12:04.000000 sharedutils-0.0.6/build.sh
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       38 2022-10-31 09:18:46.823777 sharedutils-0.0.6/setup.cfg
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1126 2022-10-31 09:18:40.000000 sharedutils-0.0.6/setup.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-31 09:18:46.761383 sharedutils-0.0.6/sharedutils/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    20157 2022-10-31 09:17:36.000000 sharedutils-0.0.6/sharedutils/__init__.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-31 09:18:46.810155 sharedutils-0.0.6/sharedutils.egg-info/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1231 2022-10-31 09:18:46.000000 sharedutils-0.0.6/sharedutils.egg-info/PKG-INFO
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      261 2022-10-31 09:18:46.000000 sharedutils-0.0.6/sharedutils.egg-info/SOURCES.txt
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        1 2022-10-31 09:18:46.000000 sharedutils-0.0.6/sharedutils.egg-info/dependency_links.txt
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        6 2022-10-31 09:18:46.000000 sharedutils-0.0.6/sharedutils.egg-info/requires.txt
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       12 2022-10-31 09:18:46.000000 sharedutils-0.0.6/sharedutils.egg-info/top_level.txt
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-20 10:35:04.738659 sharedutils-0.0.7/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1323 2023-05-20 10:29:36.000000 sharedutils-0.0.7/LICENSE
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1231 2023-05-20 10:35:04.738659 sharedutils-0.0.7/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      436 2023-05-20 10:29:36.000000 sharedutils-0.0.7/README.md
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-05-20 10:35:04.738659 sharedutils-0.0.7/setup.cfg
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1094 2023-05-20 10:34:56.000000 sharedutils-0.0.7/setup.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-20 10:35:04.738659 sharedutils-0.0.7/sharedutils/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)    19890 2023-05-20 10:34:26.000000 sharedutils-0.0.7/sharedutils/__init__.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-20 10:35:04.738659 sharedutils-0.0.7/sharedutils.egg-info/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1231 2023-05-20 10:35:04.000000 sharedutils-0.0.7/sharedutils.egg-info/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      224 2023-05-20 10:35:04.000000 sharedutils-0.0.7/sharedutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-05-20 10:35:04.000000 sharedutils-0.0.7/sharedutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        6 2023-05-20 10:35:04.000000 sharedutils-0.0.7/sharedutils.egg-info/requires.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       12 2023-05-20 10:35:04.000000 sharedutils-0.0.7/sharedutils.egg-info/top_level.txt
```

### Comparing `sharedutils-0.0.6/LICENSE` & `sharedutils-0.0.7/LICENSE`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-BSD 2-Clause License
-
-Copyright (c) 2022, Lucas Nestler
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-1. Redistributions of source code must retain the above copyright notice, this
-   list of conditions and the following disclaimer.
-
-2. Redistributions in binary form must reproduce the above copyright notice,
-   this list of conditions and the following disclaimer in the documentation
-   and/or other materials provided with the distribution.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+BSD 2-Clause License
+
+Copyright (c) 2022, Lucas Nestler
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `sharedutils-0.0.6/PKG-INFO` & `sharedutils-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sharedutils
-Version: 0.0.6
+Version: 0.0.7
 Summary: Easy usage of Python's new SharedMemory for reduced memory and CPU cost
 Home-page: https://github.com/clashluke/sharedutils
 Author: Lucas Nestler
 Author-email: github.sharedutils@nestler.sh
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `sharedutils-0.0.6/setup.py` & `sharedutils-0.0.7/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-import setuptools
-
-
-with open('README.md') as f:
-    README = f.read()
-
-setuptools.setup(
-    author="Lucas Nestler",
-    author_email="github.sharedutils@nestler.sh",
-    name='sharedutils',
-    license='BSD',
-    description="Easy usage of Python's new SharedMemory for reduced memory and CPU cost",
-    version='0.0.6',
-    long_description=README,
-    url='https://github.com/clashluke/sharedutils',
-    packages=setuptools.find_packages(),
-    python_requires=">=3.8",
-    long_description_content_type="text/markdown",
-    install_requires=["numpy"],
-    classifiers=[
-        # Trove classifiers
-        # (https://pypi.python.org/pypi?%3Aaction=list_classifiers)
-        'Development Status :: 5 - Production/Stable',
-        'License :: OSI Approved :: BSD License',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Topic :: Software Development :: Libraries',
-        'Topic :: Software Development :: Libraries :: Python Modules',
-        'Intended Audience :: Developers',
-    ],
-)
+import setuptools
+
+
+with open('README.md') as f:
+    README = f.read()
+
+setuptools.setup(
+    author="Lucas Nestler",
+    author_email="github.sharedutils@nestler.sh",
+    name='sharedutils',
+    license='BSD',
+    description="Easy usage of Python's new SharedMemory for reduced memory and CPU cost",
+    version='0.0.7',
+    long_description=README,
+    url='https://github.com/clashluke/sharedutils',
+    packages=setuptools.find_packages(),
+    python_requires=">=3.8",
+    long_description_content_type="text/markdown",
+    install_requires=["numpy"],
+    classifiers=[
+        # Trove classifiers
+        # (https://pypi.python.org/pypi?%3Aaction=list_classifiers)
+        'Development Status :: 5 - Production/Stable',
+        'License :: OSI Approved :: BSD License',
+        'Programming Language :: Python',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Topic :: Software Development :: Libraries',
+        'Topic :: Software Development :: Libraries :: Python Modules',
+        'Intended Audience :: Developers',
+    ],
+)
```

### Comparing `sharedutils-0.0.6/sharedutils.egg-info/PKG-INFO` & `sharedutils-0.0.7/sharedutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sharedutils
-Version: 0.0.6
+Version: 0.0.7
 Summary: Easy usage of Python's new SharedMemory for reduced memory and CPU cost
 Home-page: https://github.com/clashluke/sharedutils
 Author: Lucas Nestler
 Author-email: github.sharedutils@nestler.sh
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

