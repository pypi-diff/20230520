# Comparing `tmp/lmn-0.2.5.tar.gz` & `tmp/lmn-0.2.6rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmn-0.2.5.tar", last modified: Tue May  9 16:09:41 2023, max compression
+gzip compressed data, was "lmn-0.2.6rc0.tar", last modified: Sat May 20 17:48:27 2023, max compression
```

## Comparing `lmn-0.2.5.tar` & `lmn-0.2.6rc0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     1016 2023-05-09 16:09:26.364040 lmn-0.2.5/README.md
--rw-r--r--   0        0        0      685 2023-05-09 16:09:26.364040 lmn-0.2.5/lmn/__init__.py
--rw-r--r--   0        0        0       22 2023-05-09 16:09:26.364040 lmn-0.2.5/lmn/_version.py
--rw-r--r--   0        0        0     2088 2023-05-09 16:09:26.364040 lmn-0.2.5/lmn/cli/__init__.py
--rw-r--r--   0        0        0     5598 2023-05-09 16:09:26.364040 lmn-0.2.5/lmn/cli/_config_loader.py
--rw-r--r--   0        0        0     2157 2023-05-09 16:09:26.364040 lmn-0.2.5/lmn/cli/_utils.py
--rw-r--r--   0        0        0    18967 2023-05-09 16:09:26.364040 lmn-0.2.5/lmn/cli/run.py
--rw-r--r--   0        0        0     3442 2023-05-09 16:09:26.364040 lmn-0.2.5/lmn/cli/sync.py
--rw-r--r--   0        0        0     5413 2023-05-09 16:09:26.364040 lmn-0.2.5/lmn/config.py
--rw-r--r--   0        0        0      238 2023-05-09 16:09:26.364040 lmn-0.2.5/lmn/const.py
--rw-r--r--   0        0        0     7584 2023-05-09 16:09:26.368039 lmn-0.2.5/lmn/helpers.py
--rw-r--r--   0        0        0     3795 2023-05-09 16:09:26.368039 lmn-0.2.5/lmn/machine.py
--rw-r--r--   0        0        0    16591 2023-05-09 16:09:26.368039 lmn-0.2.5/lmn/runner.py
--rw-r--r--   0        0        0     1157 2023-05-09 16:09:26.368039 lmn-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     2170 2023-05-09 16:09:26.368039 lmn-0.2.5/tests/test_config.py
--rw-r--r--   0        0        0     1778 1970-01-01 00:00:00.000000 lmn-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1016 2023-05-20 17:48:17.601751 lmn-0.2.6rc0/README.md
+-rw-r--r--   0        0        0      685 2023-05-20 17:48:17.601751 lmn-0.2.6rc0/lmn/__init__.py
+-rw-r--r--   0        0        0       25 2023-05-20 17:48:17.601751 lmn-0.2.6rc0/lmn/_version.py
+-rw-r--r--   0        0        0     2088 2023-05-20 17:48:17.601751 lmn-0.2.6rc0/lmn/cli/__init__.py
+-rw-r--r--   0        0        0     5598 2023-05-20 17:48:17.601751 lmn-0.2.6rc0/lmn/cli/_config_loader.py
+-rw-r--r--   0        0        0     2157 2023-05-20 17:48:17.601751 lmn-0.2.6rc0/lmn/cli/_utils.py
+-rw-r--r--   0        0        0     2939 2023-05-20 17:48:17.601751 lmn-0.2.6rc0/lmn/cli/nv.py
+-rw-r--r--   0        0        0    18967 2023-05-20 17:48:17.601751 lmn-0.2.6rc0/lmn/cli/run.py
+-rw-r--r--   0        0        0     3442 2023-05-20 17:48:17.601751 lmn-0.2.6rc0/lmn/cli/sync.py
+-rw-r--r--   0        0        0     5413 2023-05-20 17:48:17.601751 lmn-0.2.6rc0/lmn/config.py
+-rw-r--r--   0        0        0      238 2023-05-20 17:48:17.601751 lmn-0.2.6rc0/lmn/const.py
+-rw-r--r--   0        0        0     7584 2023-05-20 17:48:17.601751 lmn-0.2.6rc0/lmn/helpers.py
+-rw-r--r--   0        0        0     3795 2023-05-20 17:48:17.601751 lmn-0.2.6rc0/lmn/machine.py
+-rw-r--r--   0        0        0    16591 2023-05-20 17:48:17.601751 lmn-0.2.6rc0/lmn/runner.py
+-rw-r--r--   0        0        0     1160 2023-05-20 17:48:17.601751 lmn-0.2.6rc0/pyproject.toml
+-rw-r--r--   0        0        0     2170 2023-05-20 17:48:17.601751 lmn-0.2.6rc0/tests/test_config.py
+-rw-r--r--   0        0        0     1781 1970-01-01 00:00:00.000000 lmn-0.2.6rc0/PKG-INFO
```

### Comparing `lmn-0.2.5/README.md` & `lmn-0.2.6rc0/README.md`

 * *Files identical despite different names*

### Comparing `lmn-0.2.5/lmn/__init__.py` & `lmn-0.2.6rc0/lmn/__init__.py`

 * *Files identical despite different names*

### Comparing `lmn-0.2.5/lmn/cli/__init__.py` & `lmn-0.2.6rc0/lmn/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `lmn-0.2.5/lmn/cli/_config_loader.py` & `lmn-0.2.6rc0/lmn/cli/_config_loader.py`

 * *Files identical despite different names*

### Comparing `lmn-0.2.5/lmn/cli/_utils.py` & `lmn-0.2.6rc0/lmn/cli/_utils.py`

 * *Files identical despite different names*

### Comparing `lmn-0.2.5/lmn/cli/run.py` & `lmn-0.2.6rc0/lmn/cli/run.py`

 * *Files identical despite different names*

### Comparing `lmn-0.2.5/lmn/cli/sync.py` & `lmn-0.2.6rc0/lmn/cli/sync.py`

 * *Files identical despite different names*

### Comparing `lmn-0.2.5/lmn/config.py` & `lmn-0.2.6rc0/lmn/config.py`

 * *Files identical despite different names*

### Comparing `lmn-0.2.5/lmn/helpers.py` & `lmn-0.2.6rc0/lmn/helpers.py`

 * *Files identical despite different names*

### Comparing `lmn-0.2.5/lmn/machine.py` & `lmn-0.2.6rc0/lmn/machine.py`

 * *Files identical despite different names*

### Comparing `lmn-0.2.5/lmn/runner.py` & `lmn-0.2.6rc0/lmn/runner.py`

 * *Files identical despite different names*

### Comparing `lmn-0.2.5/pyproject.toml` & `lmn-0.2.6rc0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "lmn"
-version = "0.2.5"
+version = "0.2.6rc0"
 description = "LMN: LaMbda functions across servers for Noobs"
 authors = [
     { name = "Takuma Yoneda", email = "takuma-yoneda@users.noreply.github.com" },
     { name = "Takuma Yoneda", email = "takuma.ynd@gmail.com" },
 ]
 dependencies = [
     "colorlog",
```

### Comparing `lmn-0.2.5/tests/test_config.py` & `lmn-0.2.6rc0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `lmn-0.2.5/PKG-INFO` & `lmn-0.2.6rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmn
-Version: 0.2.5
+Version: 0.2.6rc0
 Summary: LMN: LaMbda functions across servers for Noobs
 License: MIT License
 Author-email: Takuma Yoneda <takuma-yoneda@users.noreply.github.com>,Takuma Yoneda <takuma.ynd@gmail.com>
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
-Metadata-Version: 2.1 Name: lmn Version: 0.2.5 Summary: LMN: LaMbda functions
-across servers for Noobs License: MIT License Author-email: Takuma Yoneda
+Metadata-Version: 2.1 Name: lmn Version: 0.2.6rc0 Summary: LMN: LaMbda
+functions across servers for Noobs License: MIT License Author-email: Takuma
+Yoneda
 users.noreply.github.com>,Takuma Yoneda
 ynd@gmail.com> Requires-Python: >=3.8 Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: MacOS Classifier: Operating System
 :: POSIX Classifier: Operating System :: Unix Classifier: Programming Language
 :: Python Classifier: Programming Language :: Python :: 3.6 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Project-URL:
```

