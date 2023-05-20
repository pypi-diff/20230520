# Comparing `tmp/do-py-0.4.0.tar.gz` & `tmp/do-py-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "do-py-0.4.0.tar", last modified: Sun Apr  3 01:45:48 2022, max compression
+gzip compressed data, was "do-py-0.4.1.tar", last modified: Sat May 20 14:13:22 2023, max compression
```

## Comparing `do-py-0.4.0.tar` & `do-py-0.4.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 timdavis   (501) staff       (20)        0 2022-04-03 01:45:48.225493 do-py-0.4.0/
--rw-r--r--   0 timdavis   (501) staff       (20)     1066 2021-11-27 14:04:34.000000 do-py-0.4.0/LICENSE
--rw-r--r--   0 timdavis   (501) staff       (20)       21 2021-11-27 14:04:34.000000 do-py-0.4.0/MANIFEST.in
--rw-r--r--   0 timdavis   (501) staff       (20)    10227 2022-04-03 01:45:48.225357 do-py-0.4.0/PKG-INFO
--rw-r--r--   0 timdavis   (501) staff       (20)     9330 2021-11-27 14:04:34.000000 do-py-0.4.0/README.md
-drwxr-xr-x   0 timdavis   (501) staff       (20)        0 2022-04-03 01:45:48.221761 do-py-0.4.0/do_py/
--rw-r--r--   0 timdavis   (501) staff       (20)       58 2021-11-27 14:04:34.000000 do-py-0.4.0/do_py/__init__.py
-drwxr-xr-x   0 timdavis   (501) staff       (20)        0 2022-04-03 01:45:48.222957 do-py-0.4.0/do_py/abc/
--rw-r--r--   0 timdavis   (501) staff       (20)     9409 2021-11-27 14:04:34.000000 do-py-0.4.0/do_py/abc/__init__.py
--rw-r--r--   0 timdavis   (501) staff       (20)      460 2021-11-27 14:04:34.000000 do-py-0.4.0/do_py/abc/constants.py
--rw-r--r--   0 timdavis   (501) staff       (20)      578 2021-11-27 14:04:34.000000 do-py-0.4.0/do_py/abc/messages.py
--rw-r--r--   0 timdavis   (501) staff       (20)      688 2021-11-27 14:04:34.000000 do-py-0.4.0/do_py/abc/utils.py
-drwxr-xr-x   0 timdavis   (501) staff       (20)        0 2022-04-03 01:45:48.223492 do-py-0.4.0/do_py/common/
--rw-r--r--   0 timdavis   (501) staff       (20)     6060 2021-11-27 14:04:34.000000 do-py-0.4.0/do_py/common/__init__.py
--rw-r--r--   0 timdavis   (501) staff       (20)     5504 2021-11-27 14:04:34.000000 do-py-0.4.0/do_py/common/managed_datetime.py
--rw-r--r--   0 timdavis   (501) staff       (20)     1908 2021-11-27 14:04:34.000000 do-py-0.4.0/do_py/common/managed_list.py
-drwxr-xr-x   0 timdavis   (501) staff       (20)        0 2022-04-03 01:45:48.224291 do-py-0.4.0/do_py/data_object/
--rw-r--r--   0 timdavis   (501) staff       (20)     6890 2021-11-27 14:04:34.000000 do-py-0.4.0/do_py/data_object/__init__.py
--rw-r--r--   0 timdavis   (501) staff       (20)     7351 2021-11-27 14:04:34.000000 do-py-0.4.0/do_py/data_object/dynamic_restrictions.py
--rw-r--r--   0 timdavis   (501) staff       (20)     2872 2021-11-27 14:04:34.000000 do-py-0.4.0/do_py/data_object/restricted_dict.py
--rw-r--r--   0 timdavis   (501) staff       (20)    23730 2021-11-27 14:04:34.000000 do-py-0.4.0/do_py/data_object/restriction.py
--rw-r--r--   0 timdavis   (501) staff       (20)     2099 2021-11-27 14:04:34.000000 do-py-0.4.0/do_py/data_object/validator.py
-drwxr-xr-x   0 timdavis   (501) staff       (20)        0 2022-04-03 01:45:48.224777 do-py-0.4.0/do_py/exceptions/
--rw-r--r--   0 timdavis   (501) staff       (20)       95 2021-11-27 14:04:34.000000 do-py-0.4.0/do_py/exceptions/__init__.py
--rw-r--r--   0 timdavis   (501) staff       (20)     1024 2021-11-27 14:04:34.000000 do-py-0.4.0/do_py/exceptions/data_object_error.py
--rw-r--r--   0 timdavis   (501) staff       (20)     1583 2021-11-27 14:04:34.000000 do-py-0.4.0/do_py/exceptions/restriction_error.py
-drwxr-xr-x   0 timdavis   (501) staff       (20)        0 2022-04-03 01:45:48.225163 do-py-0.4.0/do_py/utils/
--rw-r--r--   0 timdavis   (501) staff       (20)      284 2021-11-27 14:04:34.000000 do-py-0.4.0/do_py/utils/__init__.py
--rw-r--r--   0 timdavis   (501) staff       (20)      542 2021-11-27 14:04:34.000000 do-py-0.4.0/do_py/utils/json_encoder.py
--rw-r--r--   0 timdavis   (501) staff       (20)     4070 2021-11-27 14:04:34.000000 do-py-0.4.0/do_py/utils/properties.py
-drwxr-xr-x   0 timdavis   (501) staff       (20)        0 2022-04-03 01:45:48.222386 do-py-0.4.0/do_py.egg-info/
--rw-r--r--   0 timdavis   (501) staff       (20)    10227 2022-04-03 01:45:48.000000 do-py-0.4.0/do_py.egg-info/PKG-INFO
--rw-r--r--   0 timdavis   (501) staff       (20)      757 2022-04-03 01:45:48.000000 do-py-0.4.0/do_py.egg-info/SOURCES.txt
--rw-r--r--   0 timdavis   (501) staff       (20)        1 2022-04-03 01:45:48.000000 do-py-0.4.0/do_py.egg-info/dependency_links.txt
--rw-r--r--   0 timdavis   (501) staff       (20)       13 2022-04-03 01:45:48.000000 do-py-0.4.0/do_py.egg-info/requires.txt
--rw-r--r--   0 timdavis   (501) staff       (20)        6 2022-04-03 01:45:48.000000 do-py-0.4.0/do_py.egg-info/top_level.txt
--rw-r--r--   0 timdavis   (501) staff       (20)     1051 2022-04-03 01:45:41.000000 do-py-0.4.0/package.json
--rw-r--r--   0 timdavis   (501) staff       (20)      100 2021-11-27 14:04:34.000000 do-py-0.4.0/pyproject.toml
--rw-r--r--   0 timdavis   (501) staff       (20)       38 2022-04-03 01:45:48.225532 do-py-0.4.0/setup.cfg
--rw-r--r--   0 timdavis   (501) staff       (20)     1725 2021-11-27 14:04:34.000000 do-py-0.4.0/setup.py
+drwxr-xr-x   0 timdavis   (501) staff       (20)        0 2023-05-20 14:13:22.411562 do-py-0.4.1/
+-rw-r--r--   0 timdavis   (501) staff       (20)     1066 2021-11-27 14:04:34.000000 do-py-0.4.1/LICENSE
+-rw-r--r--   0 timdavis   (501) staff       (20)       21 2021-11-27 14:04:34.000000 do-py-0.4.1/MANIFEST.in
+-rw-r--r--   0 timdavis   (501) staff       (20)    10227 2023-05-20 14:13:22.411428 do-py-0.4.1/PKG-INFO
+-rw-r--r--   0 timdavis   (501) staff       (20)     9330 2021-11-27 14:04:34.000000 do-py-0.4.1/README.md
+drwxr-xr-x   0 timdavis   (501) staff       (20)        0 2023-05-20 14:13:22.408796 do-py-0.4.1/do_py/
+-rw-r--r--   0 timdavis   (501) staff       (20)       58 2021-11-27 14:04:34.000000 do-py-0.4.1/do_py/__init__.py
+drwxr-xr-x   0 timdavis   (501) staff       (20)        0 2023-05-20 14:13:22.409753 do-py-0.4.1/do_py/abc/
+-rw-r--r--   0 timdavis   (501) staff       (20)     9409 2023-05-20 13:54:45.000000 do-py-0.4.1/do_py/abc/__init__.py
+-rw-r--r--   0 timdavis   (501) staff       (20)      460 2021-11-27 14:04:34.000000 do-py-0.4.1/do_py/abc/constants.py
+-rw-r--r--   0 timdavis   (501) staff       (20)      578 2021-11-27 14:04:34.000000 do-py-0.4.1/do_py/abc/messages.py
+-rw-r--r--   0 timdavis   (501) staff       (20)      688 2021-11-27 14:04:34.000000 do-py-0.4.1/do_py/abc/utils.py
+drwxr-xr-x   0 timdavis   (501) staff       (20)        0 2023-05-20 14:13:22.410087 do-py-0.4.1/do_py/common/
+-rw-r--r--   0 timdavis   (501) staff       (20)     6060 2021-11-27 14:04:34.000000 do-py-0.4.1/do_py/common/__init__.py
+-rw-r--r--   0 timdavis   (501) staff       (20)     5504 2021-11-27 14:04:34.000000 do-py-0.4.1/do_py/common/managed_datetime.py
+-rw-r--r--   0 timdavis   (501) staff       (20)     1908 2021-11-27 14:04:34.000000 do-py-0.4.1/do_py/common/managed_list.py
+drwxr-xr-x   0 timdavis   (501) staff       (20)        0 2023-05-20 14:13:22.410659 do-py-0.4.1/do_py/data_object/
+-rw-r--r--   0 timdavis   (501) staff       (20)     6890 2021-11-27 14:04:34.000000 do-py-0.4.1/do_py/data_object/__init__.py
+-rw-r--r--   0 timdavis   (501) staff       (20)     7351 2021-11-27 14:04:34.000000 do-py-0.4.1/do_py/data_object/dynamic_restrictions.py
+-rw-r--r--   0 timdavis   (501) staff       (20)     2872 2021-11-27 14:04:34.000000 do-py-0.4.1/do_py/data_object/restricted_dict.py
+-rw-r--r--   0 timdavis   (501) staff       (20)    23730 2021-11-27 14:04:34.000000 do-py-0.4.1/do_py/data_object/restriction.py
+-rw-r--r--   0 timdavis   (501) staff       (20)     2099 2021-11-27 14:04:34.000000 do-py-0.4.1/do_py/data_object/validator.py
+drwxr-xr-x   0 timdavis   (501) staff       (20)        0 2023-05-20 14:13:22.410950 do-py-0.4.1/do_py/exceptions/
+-rw-r--r--   0 timdavis   (501) staff       (20)       95 2021-11-27 14:04:34.000000 do-py-0.4.1/do_py/exceptions/__init__.py
+-rw-r--r--   0 timdavis   (501) staff       (20)     1024 2021-11-27 14:04:34.000000 do-py-0.4.1/do_py/exceptions/data_object_error.py
+-rw-r--r--   0 timdavis   (501) staff       (20)     1583 2021-11-27 14:04:34.000000 do-py-0.4.1/do_py/exceptions/restriction_error.py
+drwxr-xr-x   0 timdavis   (501) staff       (20)        0 2023-05-20 14:13:22.411270 do-py-0.4.1/do_py/utils/
+-rw-r--r--   0 timdavis   (501) staff       (20)      284 2021-11-27 14:04:34.000000 do-py-0.4.1/do_py/utils/__init__.py
+-rw-r--r--   0 timdavis   (501) staff       (20)      542 2021-11-27 14:04:34.000000 do-py-0.4.1/do_py/utils/json_encoder.py
+-rw-r--r--   0 timdavis   (501) staff       (20)     4070 2021-11-27 14:04:34.000000 do-py-0.4.1/do_py/utils/properties.py
+drwxr-xr-x   0 timdavis   (501) staff       (20)        0 2023-05-20 14:13:22.409320 do-py-0.4.1/do_py.egg-info/
+-rw-r--r--   0 timdavis   (501) staff       (20)    10227 2023-05-20 14:13:22.000000 do-py-0.4.1/do_py.egg-info/PKG-INFO
+-rw-r--r--   0 timdavis   (501) staff       (20)      757 2023-05-20 14:13:22.000000 do-py-0.4.1/do_py.egg-info/SOURCES.txt
+-rw-r--r--   0 timdavis   (501) staff       (20)        1 2023-05-20 14:13:22.000000 do-py-0.4.1/do_py.egg-info/dependency_links.txt
+-rw-r--r--   0 timdavis   (501) staff       (20)       13 2023-05-20 14:13:22.000000 do-py-0.4.1/do_py.egg-info/requires.txt
+-rw-r--r--   0 timdavis   (501) staff       (20)        6 2023-05-20 14:13:22.000000 do-py-0.4.1/do_py.egg-info/top_level.txt
+-rw-r--r--   0 timdavis   (501) staff       (20)     1051 2023-05-20 14:13:13.000000 do-py-0.4.1/package.json
+-rw-r--r--   0 timdavis   (501) staff       (20)      100 2021-11-27 14:04:34.000000 do-py-0.4.1/pyproject.toml
+-rw-r--r--   0 timdavis   (501) staff       (20)       38 2023-05-20 14:13:22.411599 do-py-0.4.1/setup.cfg
+-rw-r--r--   0 timdavis   (501) staff       (20)     1725 2021-11-27 14:04:34.000000 do-py-0.4.1/setup.py
```

### Comparing `do-py-0.4.0/LICENSE` & `do-py-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `do-py-0.4.0/PKG-INFO` & `do-py-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: do-py
-Version: 0.4.0
+Version: 0.4.1
 Summary: Data validation and standardization library wrapping Python dictionaries.
 Home-page: https://github.com/do-py-together/do-py
 Author: Tim Davis
 Author-email: timdavis.3991@gmail.com
 License: UNKNOWN
 Keywords: development,OO
 Platform: UNKNOWN
```

### Comparing `do-py-0.4.0/README.md` & `do-py-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `do-py-0.4.0/do_py/abc/__init__.py` & `do-py-0.4.1/do_py/abc/__init__.py`

 * *Files identical despite different names*

### Comparing `do-py-0.4.0/do_py/abc/messages.py` & `do-py-0.4.1/do_py/abc/messages.py`

 * *Files identical despite different names*

### Comparing `do-py-0.4.0/do_py/abc/utils.py` & `do-py-0.4.1/do_py/abc/utils.py`

 * *Files identical despite different names*

### Comparing `do-py-0.4.0/do_py/common/__init__.py` & `do-py-0.4.1/do_py/common/__init__.py`

 * *Files identical despite different names*

### Comparing `do-py-0.4.0/do_py/common/managed_datetime.py` & `do-py-0.4.1/do_py/common/managed_datetime.py`

 * *Files identical despite different names*

### Comparing `do-py-0.4.0/do_py/common/managed_list.py` & `do-py-0.4.1/do_py/common/managed_list.py`

 * *Files identical despite different names*

### Comparing `do-py-0.4.0/do_py/data_object/__init__.py` & `do-py-0.4.1/do_py/data_object/__init__.py`

 * *Files identical despite different names*

### Comparing `do-py-0.4.0/do_py/data_object/dynamic_restrictions.py` & `do-py-0.4.1/do_py/data_object/dynamic_restrictions.py`

 * *Files identical despite different names*

### Comparing `do-py-0.4.0/do_py/data_object/restricted_dict.py` & `do-py-0.4.1/do_py/data_object/restricted_dict.py`

 * *Files identical despite different names*

### Comparing `do-py-0.4.0/do_py/data_object/restriction.py` & `do-py-0.4.1/do_py/data_object/restriction.py`

 * *Files identical despite different names*

### Comparing `do-py-0.4.0/do_py/data_object/validator.py` & `do-py-0.4.1/do_py/data_object/validator.py`

 * *Files identical despite different names*

### Comparing `do-py-0.4.0/do_py/exceptions/data_object_error.py` & `do-py-0.4.1/do_py/exceptions/data_object_error.py`

 * *Files identical despite different names*

### Comparing `do-py-0.4.0/do_py/exceptions/restriction_error.py` & `do-py-0.4.1/do_py/exceptions/restriction_error.py`

 * *Files identical despite different names*

### Comparing `do-py-0.4.0/do_py/utils/json_encoder.py` & `do-py-0.4.1/do_py/utils/json_encoder.py`

 * *Files identical despite different names*

### Comparing `do-py-0.4.0/do_py/utils/properties.py` & `do-py-0.4.1/do_py/utils/properties.py`

 * *Files identical despite different names*

### Comparing `do-py-0.4.0/do_py.egg-info/PKG-INFO` & `do-py-0.4.1/do_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: do-py
-Version: 0.4.0
+Version: 0.4.1
 Summary: Data validation and standardization library wrapping Python dictionaries.
 Home-page: https://github.com/do-py-together/do-py
 Author: Tim Davis
 Author-email: timdavis.3991@gmail.com
 License: UNKNOWN
 Keywords: development,OO
 Platform: UNKNOWN
```

### Comparing `do-py-0.4.0/do_py.egg-info/SOURCES.txt` & `do-py-0.4.1/do_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `do-py-0.4.0/package.json` & `do-py-0.4.1/package.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'version'": "'0.4.1'"}*

```diff
@@ -12,9 +12,9 @@
         "clean": "rm -vrf ./build ./dist ./*.pyc ./*.tgz ./*.egg-info",
         "lint": "find ./do_py -type f -name \"*.py\" | xargs pylint",
         "release": "release-it",
         "release-pypi": "yarn clean && yarn build && pipenv run twine upload dist/* && yarn clean",
         "release-test": "yarn clean && yarn build && twine upload --repository-url https://test.pypi.org/legacy/ dist/*",
         "test": "pipenv run pytest -svo xfail_strict=True --durations 10 --maxfail 10 --cov ./ --cov-report html --cov-report xml --junitxml test-reports/tests.xml --cov-config=./tests/.coveragerc ./tests/"
     },
-    "version": "0.4.0"
+    "version": "0.4.1"
 }
```

### Comparing `do-py-0.4.0/setup.py` & `do-py-0.4.1/setup.py`

 * *Files identical despite different names*

