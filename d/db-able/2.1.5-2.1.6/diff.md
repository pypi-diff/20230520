# Comparing `tmp/db-able-2.1.5.tar.gz` & `tmp/db-able-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "db-able-2.1.5.tar", last modified: Sun Apr  3 02:00:01 2022, max compression
+gzip compressed data, was "db-able-2.1.6.tar", last modified: Sat May 20 15:45:01 2023, max compression
```

## Comparing `db-able-2.1.5.tar` & `db-able-2.1.6.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 timdavis   (501) staff       (20)        0 2022-04-03 02:00:01.484826 db-able-2.1.5/
--rw-r--r--   0 timdavis   (501) staff       (20)     1066 2021-11-27 14:04:59.000000 db-able-2.1.5/LICENSE
--rw-r--r--   0 timdavis   (501) staff       (20)    10016 2022-04-03 02:00:01.484658 db-able-2.1.5/PKG-INFO
--rw-r--r--   0 timdavis   (501) staff       (20)     9305 2022-04-03 01:56:20.000000 db-able-2.1.5/README.md
-drwxr-xr-x   0 timdavis   (501) staff       (20)        0 2022-04-03 02:00:01.479511 db-able-2.1.5/db_able/
--rw-r--r--   0 timdavis   (501) staff       (20)      285 2021-11-30 21:22:34.000000 db-able-2.1.5/db_able/__init__.py
-drwxr-xr-x   0 timdavis   (501) staff       (20)        0 2022-04-03 02:00:01.481663 db-able-2.1.5/db_able/base_model/
--rw-r--r--   0 timdavis   (501) staff       (20)        0 2021-11-27 14:04:59.000000 db-able-2.1.5/db_able/base_model/__init__.py
--rw-r--r--   0 timdavis   (501) staff       (20)     1304 2021-11-27 14:04:59.000000 db-able-2.1.5/db_able/base_model/database_abc.py
--rw-r--r--   0 timdavis   (501) staff       (20)     2564 2021-11-27 14:04:59.000000 db-able-2.1.5/db_able/base_model/kwargs_validator.py
--rw-r--r--   0 timdavis   (501) staff       (20)      750 2021-11-27 14:04:59.000000 db-able-2.1.5/db_able/base_model/params.py
-drwxr-xr-x   0 timdavis   (501) staff       (20)        0 2022-04-03 02:00:01.481802 db-able-2.1.5/db_able/client/
--rw-r--r--   0 timdavis   (501) staff       (20)     6137 2021-11-30 21:22:34.000000 db-able-2.1.5/db_able/client/__init__.py
--rw-r--r--   0 timdavis   (501) staff       (20)     2151 2021-11-27 14:04:59.000000 db-able-2.1.5/db_able/creatable.py
--rw-r--r--   0 timdavis   (501) staff       (20)     2043 2021-11-27 14:04:59.000000 db-able-2.1.5/db_able/deletable.py
--rw-r--r--   0 timdavis   (501) staff       (20)    11479 2021-11-30 21:22:34.000000 db-able-2.1.5/db_able/listable.py
--rw-r--r--   0 timdavis   (501) staff       (20)     1813 2021-11-27 14:04:59.000000 db-able-2.1.5/db_able/loadable.py
-drwxr-xr-x   0 timdavis   (501) staff       (20)        0 2022-04-03 02:00:01.482125 db-able-2.1.5/db_able/mgmt/
--rw-r--r--   0 timdavis   (501) staff       (20)        0 2021-11-30 21:22:34.000000 db-able-2.1.5/db_able/mgmt/__init__.py
--rw-r--r--   0 timdavis   (501) staff       (20)      323 2021-11-30 21:22:34.000000 db-able-2.1.5/db_able/mgmt/const.py
--rw-r--r--   0 timdavis   (501) staff       (20)     2384 2021-11-27 14:04:59.000000 db-able-2.1.5/db_able/savable.py
-drwxr-xr-x   0 timdavis   (501) staff       (20)        0 2022-04-03 02:00:01.482394 db-able-2.1.5/db_able/utils/
--rw-r--r--   0 timdavis   (501) staff       (20)        0 2021-11-27 14:04:59.000000 db-able-2.1.5/db_able/utils/__init__.py
--rw-r--r--   0 timdavis   (501) staff       (20)    10477 2021-11-30 21:22:34.000000 db-able-2.1.5/db_able/utils/sql_generator.py
-drwxr-xr-x   0 timdavis   (501) staff       (20)        0 2022-04-03 02:00:01.480374 db-able-2.1.5/db_able.egg-info/
--rw-r--r--   0 timdavis   (501) staff       (20)    10016 2022-04-03 02:00:01.000000 db-able-2.1.5/db_able.egg-info/PKG-INFO
--rw-r--r--   0 timdavis   (501) staff       (20)      924 2022-04-03 02:00:01.000000 db-able-2.1.5/db_able.egg-info/SOURCES.txt
--rw-r--r--   0 timdavis   (501) staff       (20)        1 2022-04-03 02:00:01.000000 db-able-2.1.5/db_able.egg-info/dependency_links.txt
--rw-r--r--   0 timdavis   (501) staff       (20)       47 2022-04-03 02:00:01.000000 db-able-2.1.5/db_able.egg-info/requires.txt
--rw-r--r--   0 timdavis   (501) staff       (20)       23 2022-04-03 02:00:01.000000 db-able-2.1.5/db_able.egg-info/top_level.txt
-drwxr-xr-x   0 timdavis   (501) staff       (20)        0 2022-04-03 02:00:01.483241 db-able-2.1.5/examples/
--rw-r--r--   0 timdavis   (501) staff       (20)        0 2021-11-27 14:04:59.000000 db-able-2.1.5/examples/__init__.py
--rw-r--r--   0 timdavis   (501) staff       (20)      759 2021-11-30 18:02:16.000000 db-able-2.1.5/examples/a.py
--rw-r--r--   0 timdavis   (501) staff       (20)      569 2021-11-30 21:22:34.000000 db-able-2.1.5/examples/b.py
--rw-r--r--   0 timdavis   (501) staff       (20)      428 2021-11-30 21:22:34.000000 db-able-2.1.5/examples/c.py
--rw-r--r--   0 timdavis   (501) staff       (20)     2109 2021-11-27 14:04:59.000000 db-able-2.1.5/examples/user.py
--rw-r--r--   0 timdavis   (501) staff       (20)       38 2022-04-03 02:00:01.484871 db-able-2.1.5/setup.cfg
--rw-r--r--   0 timdavis   (501) staff       (20)     1394 2021-12-25 19:49:44.000000 db-able-2.1.5/setup.py
-drwxr-xr-x   0 timdavis   (501) staff       (20)        0 2022-04-03 02:00:01.483734 db-able-2.1.5/tests/
--rw-r--r--   0 timdavis   (501) staff       (20)        0 2021-11-27 14:04:59.000000 db-able-2.1.5/tests/__init__.py
-drwxr-xr-x   0 timdavis   (501) staff       (20)        0 2022-04-03 02:00:01.484211 db-able-2.1.5/tests/base_model/
--rw-r--r--   0 timdavis   (501) staff       (20)        0 2021-11-27 14:04:59.000000 db-able-2.1.5/tests/base_model/__init__.py
--rw-r--r--   0 timdavis   (501) staff       (20)     1152 2021-11-27 14:04:59.000000 db-able-2.1.5/tests/base_model/test_database_abc.py
--rw-r--r--   0 timdavis   (501) staff       (20)     1905 2021-11-27 14:04:59.000000 db-able-2.1.5/tests/base_model/test_kwargs_validator.py
--rw-r--r--   0 timdavis   (501) staff       (20)      903 2021-11-27 14:04:59.000000 db-able-2.1.5/tests/base_model/test_params.py
--rw-r--r--   0 timdavis   (501) staff       (20)      285 2021-11-27 14:04:59.000000 db-able-2.1.5/tests/conftest.py
--rw-r--r--   0 timdavis   (501) staff       (20)     3355 2021-11-27 14:04:59.000000 db-able-2.1.5/tests/test_client.py
--rw-r--r--   0 timdavis   (501) staff       (20)     1252 2021-11-30 21:22:34.000000 db-able-2.1.5/tests/test_db_able.py
-drwxr-xr-x   0 timdavis   (501) staff       (20)        0 2022-04-03 02:00:01.484448 db-able-2.1.5/tests/utils/
--rw-r--r--   0 timdavis   (501) staff       (20)        0 2021-11-27 14:04:59.000000 db-able-2.1.5/tests/utils/__init__.py
--rw-r--r--   0 timdavis   (501) staff       (20)    14622 2021-11-30 21:22:34.000000 db-able-2.1.5/tests/utils/test_sql_generator.py
+drwxr-xr-x   0 timdavis   (501) staff       (20)        0 2023-05-20 15:45:01.079827 db-able-2.1.6/
+-rw-r--r--   0 timdavis   (501) staff       (20)     1066 2021-11-27 14:04:59.000000 db-able-2.1.6/LICENSE
+-rw-r--r--   0 timdavis   (501) staff       (20)    10016 2023-05-20 15:45:01.079688 db-able-2.1.6/PKG-INFO
+-rw-r--r--   0 timdavis   (501) staff       (20)     9305 2022-04-03 01:56:20.000000 db-able-2.1.6/README.md
+drwxr-xr-x   0 timdavis   (501) staff       (20)        0 2023-05-20 15:45:01.076368 db-able-2.1.6/db_able/
+-rw-r--r--   0 timdavis   (501) staff       (20)      285 2021-11-30 21:22:34.000000 db-able-2.1.6/db_able/__init__.py
+drwxr-xr-x   0 timdavis   (501) staff       (20)        0 2023-05-20 15:45:01.077296 db-able-2.1.6/db_able/base_model/
+-rw-r--r--   0 timdavis   (501) staff       (20)        0 2021-11-27 14:04:59.000000 db-able-2.1.6/db_able/base_model/__init__.py
+-rw-r--r--   0 timdavis   (501) staff       (20)     1304 2021-11-27 14:04:59.000000 db-able-2.1.6/db_able/base_model/database_abc.py
+-rw-r--r--   0 timdavis   (501) staff       (20)     2564 2021-11-27 14:04:59.000000 db-able-2.1.6/db_able/base_model/kwargs_validator.py
+-rw-r--r--   0 timdavis   (501) staff       (20)      750 2021-11-27 14:04:59.000000 db-able-2.1.6/db_able/base_model/params.py
+drwxr-xr-x   0 timdavis   (501) staff       (20)        0 2023-05-20 15:45:01.077399 db-able-2.1.6/db_able/client/
+-rw-r--r--   0 timdavis   (501) staff       (20)     6137 2021-11-30 21:22:34.000000 db-able-2.1.6/db_able/client/__init__.py
+-rw-r--r--   0 timdavis   (501) staff       (20)     2151 2021-11-27 14:04:59.000000 db-able-2.1.6/db_able/creatable.py
+-rw-r--r--   0 timdavis   (501) staff       (20)     2043 2021-11-27 14:04:59.000000 db-able-2.1.6/db_able/deletable.py
+-rw-r--r--   0 timdavis   (501) staff       (20)    11479 2021-11-30 21:22:34.000000 db-able-2.1.6/db_able/listable.py
+-rw-r--r--   0 timdavis   (501) staff       (20)     1813 2021-11-27 14:04:59.000000 db-able-2.1.6/db_able/loadable.py
+drwxr-xr-x   0 timdavis   (501) staff       (20)        0 2023-05-20 15:45:01.077614 db-able-2.1.6/db_able/mgmt/
+-rw-r--r--   0 timdavis   (501) staff       (20)        0 2021-11-30 21:22:34.000000 db-able-2.1.6/db_able/mgmt/__init__.py
+-rw-r--r--   0 timdavis   (501) staff       (20)      323 2021-11-30 21:22:34.000000 db-able-2.1.6/db_able/mgmt/const.py
+-rw-r--r--   0 timdavis   (501) staff       (20)     2384 2021-11-27 14:04:59.000000 db-able-2.1.6/db_able/savable.py
+drwxr-xr-x   0 timdavis   (501) staff       (20)        0 2023-05-20 15:45:01.077804 db-able-2.1.6/db_able/utils/
+-rw-r--r--   0 timdavis   (501) staff       (20)        0 2021-11-27 14:04:59.000000 db-able-2.1.6/db_able/utils/__init__.py
+-rw-r--r--   0 timdavis   (501) staff       (20)    10477 2021-11-30 21:22:34.000000 db-able-2.1.6/db_able/utils/sql_generator.py
+drwxr-xr-x   0 timdavis   (501) staff       (20)        0 2023-05-20 15:45:01.076891 db-able-2.1.6/db_able.egg-info/
+-rw-r--r--   0 timdavis   (501) staff       (20)    10016 2023-05-20 15:45:01.000000 db-able-2.1.6/db_able.egg-info/PKG-INFO
+-rw-r--r--   0 timdavis   (501) staff       (20)      924 2023-05-20 15:45:01.000000 db-able-2.1.6/db_able.egg-info/SOURCES.txt
+-rw-r--r--   0 timdavis   (501) staff       (20)        1 2023-05-20 15:45:01.000000 db-able-2.1.6/db_able.egg-info/dependency_links.txt
+-rw-r--r--   0 timdavis   (501) staff       (20)       47 2023-05-20 15:45:01.000000 db-able-2.1.6/db_able.egg-info/requires.txt
+-rw-r--r--   0 timdavis   (501) staff       (20)       23 2023-05-20 15:45:01.000000 db-able-2.1.6/db_able.egg-info/top_level.txt
+drwxr-xr-x   0 timdavis   (501) staff       (20)        0 2023-05-20 15:45:01.078422 db-able-2.1.6/examples/
+-rw-r--r--   0 timdavis   (501) staff       (20)        0 2021-11-27 14:04:59.000000 db-able-2.1.6/examples/__init__.py
+-rw-r--r--   0 timdavis   (501) staff       (20)      759 2021-11-30 18:02:16.000000 db-able-2.1.6/examples/a.py
+-rw-r--r--   0 timdavis   (501) staff       (20)      569 2021-11-30 21:22:34.000000 db-able-2.1.6/examples/b.py
+-rw-r--r--   0 timdavis   (501) staff       (20)      428 2021-11-30 21:22:34.000000 db-able-2.1.6/examples/c.py
+-rw-r--r--   0 timdavis   (501) staff       (20)     2109 2021-11-27 14:04:59.000000 db-able-2.1.6/examples/user.py
+-rw-r--r--   0 timdavis   (501) staff       (20)       38 2023-05-20 15:45:01.079871 db-able-2.1.6/setup.cfg
+-rw-r--r--   0 timdavis   (501) staff       (20)     1394 2021-12-25 19:49:44.000000 db-able-2.1.6/setup.py
+drwxr-xr-x   0 timdavis   (501) staff       (20)        0 2023-05-20 15:45:01.078950 db-able-2.1.6/tests/
+-rw-r--r--   0 timdavis   (501) staff       (20)        0 2021-11-27 14:04:59.000000 db-able-2.1.6/tests/__init__.py
+drwxr-xr-x   0 timdavis   (501) staff       (20)        0 2023-05-20 15:45:01.079351 db-able-2.1.6/tests/base_model/
+-rw-r--r--   0 timdavis   (501) staff       (20)        0 2021-11-27 14:04:59.000000 db-able-2.1.6/tests/base_model/__init__.py
+-rw-r--r--   0 timdavis   (501) staff       (20)     1152 2021-11-27 14:04:59.000000 db-able-2.1.6/tests/base_model/test_database_abc.py
+-rw-r--r--   0 timdavis   (501) staff       (20)     1905 2021-11-27 14:04:59.000000 db-able-2.1.6/tests/base_model/test_kwargs_validator.py
+-rw-r--r--   0 timdavis   (501) staff       (20)      903 2021-11-27 14:04:59.000000 db-able-2.1.6/tests/base_model/test_params.py
+-rw-r--r--   0 timdavis   (501) staff       (20)      285 2021-11-27 14:04:59.000000 db-able-2.1.6/tests/conftest.py
+-rw-r--r--   0 timdavis   (501) staff       (20)     3355 2021-11-27 14:04:59.000000 db-able-2.1.6/tests/test_client.py
+-rw-r--r--   0 timdavis   (501) staff       (20)     1252 2021-11-30 21:22:34.000000 db-able-2.1.6/tests/test_db_able.py
+drwxr-xr-x   0 timdavis   (501) staff       (20)        0 2023-05-20 15:45:01.079537 db-able-2.1.6/tests/utils/
+-rw-r--r--   0 timdavis   (501) staff       (20)        0 2021-11-27 14:04:59.000000 db-able-2.1.6/tests/utils/__init__.py
+-rw-r--r--   0 timdavis   (501) staff       (20)    14622 2021-11-30 21:22:34.000000 db-able-2.1.6/tests/utils/test_sql_generator.py
```

### Comparing `db-able-2.1.5/LICENSE` & `db-able-2.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `db-able-2.1.5/PKG-INFO` & `db-able-2.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: db-able
-Version: 2.1.5
+Version: 2.1.6
 Summary: Implement basic CRUD operations into DataObject framework with generalized DB access.
 Home-page: https://github.com/timdaviss/db-able
 Author: Tim Davis
 Author-email: timdavis.3991@gmail.com
 License: UNKNOWN
 Keywords: development,OO
 Platform: UNKNOWN
```

### Comparing `db-able-2.1.5/README.md` & `db-able-2.1.6/README.md`

 * *Files identical despite different names*

### Comparing `db-able-2.1.5/db_able/base_model/database_abc.py` & `db-able-2.1.6/db_able/base_model/database_abc.py`

 * *Files identical despite different names*

### Comparing `db-able-2.1.5/db_able/base_model/kwargs_validator.py` & `db-able-2.1.6/db_able/base_model/kwargs_validator.py`

 * *Files identical despite different names*

### Comparing `db-able-2.1.5/db_able/base_model/params.py` & `db-able-2.1.6/db_able/base_model/params.py`

 * *Files identical despite different names*

### Comparing `db-able-2.1.5/db_able/client/__init__.py` & `db-able-2.1.6/db_able/client/__init__.py`

 * *Files identical despite different names*

### Comparing `db-able-2.1.5/db_able/creatable.py` & `db-able-2.1.6/db_able/creatable.py`

 * *Files identical despite different names*

### Comparing `db-able-2.1.5/db_able/deletable.py` & `db-able-2.1.6/db_able/deletable.py`

 * *Files identical despite different names*

### Comparing `db-able-2.1.5/db_able/listable.py` & `db-able-2.1.6/db_able/listable.py`

 * *Files identical despite different names*

### Comparing `db-able-2.1.5/db_able/loadable.py` & `db-able-2.1.6/db_able/loadable.py`

 * *Files identical despite different names*

### Comparing `db-able-2.1.5/db_able/savable.py` & `db-able-2.1.6/db_able/savable.py`

 * *Files identical despite different names*

### Comparing `db-able-2.1.5/db_able/utils/sql_generator.py` & `db-able-2.1.6/db_able/utils/sql_generator.py`

 * *Files identical despite different names*

### Comparing `db-able-2.1.5/db_able.egg-info/PKG-INFO` & `db-able-2.1.6/db_able.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: db-able
-Version: 2.1.5
+Version: 2.1.6
 Summary: Implement basic CRUD operations into DataObject framework with generalized DB access.
 Home-page: https://github.com/timdaviss/db-able
 Author: Tim Davis
 Author-email: timdavis.3991@gmail.com
 License: UNKNOWN
 Keywords: development,OO
 Platform: UNKNOWN
```

### Comparing `db-able-2.1.5/db_able.egg-info/SOURCES.txt` & `db-able-2.1.6/db_able.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `db-able-2.1.5/examples/a.py` & `db-able-2.1.6/examples/a.py`

 * *Files identical despite different names*

### Comparing `db-able-2.1.5/examples/b.py` & `db-able-2.1.6/examples/b.py`

 * *Files identical despite different names*

### Comparing `db-able-2.1.5/examples/user.py` & `db-able-2.1.6/examples/user.py`

 * *Files identical despite different names*

### Comparing `db-able-2.1.5/setup.py` & `db-able-2.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `db-able-2.1.5/tests/base_model/test_database_abc.py` & `db-able-2.1.6/tests/base_model/test_database_abc.py`

 * *Files identical despite different names*

### Comparing `db-able-2.1.5/tests/base_model/test_kwargs_validator.py` & `db-able-2.1.6/tests/base_model/test_kwargs_validator.py`

 * *Files identical despite different names*

### Comparing `db-able-2.1.5/tests/base_model/test_params.py` & `db-able-2.1.6/tests/base_model/test_params.py`

 * *Files identical despite different names*

### Comparing `db-able-2.1.5/tests/test_client.py` & `db-able-2.1.6/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `db-able-2.1.5/tests/test_db_able.py` & `db-able-2.1.6/tests/test_db_able.py`

 * *Files identical despite different names*

### Comparing `db-able-2.1.5/tests/utils/test_sql_generator.py` & `db-able-2.1.6/tests/utils/test_sql_generator.py`

 * *Files identical despite different names*

