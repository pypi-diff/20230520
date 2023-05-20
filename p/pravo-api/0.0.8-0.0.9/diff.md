# Comparing `tmp/pravo-api-0.0.8.tar.gz` & `tmp/pravo-api-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pravo-api-0.0.8.tar", last modified: Thu Sep 15 17:24:22 2022, max compression
+gzip compressed data, was "pravo-api-0.0.9.tar", last modified: Sun Oct  2 11:33:41 2022, max compression
```

## Comparing `pravo-api-0.0.8.tar` & `pravo-api-0.0.9.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2022-09-15 17:24:22.141023 pravo-api-0.0.8/
--rw-rw-rw-   0        0        0     1084 2022-09-15 17:04:01.000000 pravo-api-0.0.8/LICENSE
--rw-rw-rw-   0        0        0       82 2022-09-15 15:24:11.000000 pravo-api-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0    42814 2022-09-15 17:24:22.140023 pravo-api-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0    42558 2022-09-15 17:18:43.000000 pravo-api-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2022-09-15 17:24:21.914043 pravo-api-0.0.8/pravo_api/
--rw-rw-rw-   0        0        0       28 2022-09-13 14:43:04.000000 pravo-api-0.0.8/pravo_api/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-15 17:24:21.985128 pravo-api-0.0.8/pravo_api/api/
--rw-rw-rw-   0        0        0       27 2022-09-15 16:37:20.000000 pravo-api-0.0.8/pravo_api/api/__init__.py
--rw-rw-rw-   0        0        0     5914 2022-09-15 16:37:59.000000 pravo-api-0.0.8/pravo_api/api/config.py
-drwxrwxrwx   0        0        0        0 2022-09-15 17:24:22.011084 pravo-api-0.0.8/pravo_api/api/downloader/
--rw-rw-rw-   0        0        0       43 2022-09-15 16:34:14.000000 pravo-api-0.0.8/pravo_api/api/downloader/__init__.py
--rw-rw-rw-   0        0        0     7100 2022-09-15 15:58:00.000000 pravo-api-0.0.8/pravo_api/api/downloader/aio_downloader.py
--rw-rw-rw-   0        0        0      758 2022-09-14 07:41:42.000000 pravo-api-0.0.8/pravo_api/api/downloader/meta_data_getter.py
-drwxrwxrwx   0        0        0        0 2022-09-15 17:24:22.032988 pravo-api-0.0.8/pravo_api/api/links_getter/
--rw-rw-rw-   0        0        0       37 2022-09-15 16:34:44.000000 pravo-api-0.0.8/pravo_api/api/links_getter/__init__.py
--rw-rw-rw-   0        0        0    10093 2022-09-15 16:33:46.000000 pravo-api-0.0.8/pravo_api/api/links_getter/links_getter.py
--rw-rw-rw-   0        0        0      221 2022-09-15 16:33:32.000000 pravo-api-0.0.8/pravo_api/api/links_getter/models.py
--rw-rw-rw-   0        0        0     1087 2022-09-15 16:33:09.000000 pravo-api-0.0.8/pravo_api/api/main.py
--rw-rw-rw-   0        0        0       39 2022-09-15 15:53:52.000000 pravo-api-0.0.8/pravo_api/api/temp.py
-drwxrwxrwx   0        0        0        0 2022-09-15 17:24:22.051109 pravo-api-0.0.8/pravo_api/api/utils/
--rw-rw-rw-   0        0        0        0 2022-08-01 07:27:14.000000 pravo-api-0.0.8/pravo_api/api/utils/__init__.py
--rw-rw-rw-   0        0        0     1694 2022-07-15 12:27:00.000000 pravo-api-0.0.8/pravo_api/api/utils/back_off.py
--rw-rw-rw-   0        0        0     2260 2022-09-15 09:34:54.000000 pravo-api-0.0.8/pravo_api/api/utils/my_logger.py
-drwxrwxrwx   0        0        0        0 2022-09-15 17:24:22.072275 pravo-api-0.0.8/pravo_api/appoint_parser/
--rw-rw-rw-   0        0        0       33 2022-09-15 16:35:19.000000 pravo-api-0.0.8/pravo_api/appoint_parser/__init__.py
--rw-rw-rw-   0        0        0      509 2022-08-02 13:32:08.000000 pravo-api-0.0.8/pravo_api/appoint_parser/__main__.py
--rw-rw-rw-   0        0        0     7357 2022-09-15 09:38:35.000000 pravo-api-0.0.8/pravo_api/appoint_parser/decree_parser.py
-drwxrwxrwx   0        0        0        0 2022-09-15 17:24:22.097426 pravo-api-0.0.8/pravo_api/appoint_parser/parsers/
--rw-rw-rw-   0        0        0       88 2022-09-15 16:36:39.000000 pravo-api-0.0.8/pravo_api/appoint_parser/parsers/__init__.py
--rw-rw-rw-   0        0        0     6140 2022-09-15 16:30:53.000000 pravo-api-0.0.8/pravo_api/appoint_parser/parsers/multi_app.py
--rw-rw-rw-   0        0        0     6021 2022-09-15 15:58:00.000000 pravo-api-0.0.8/pravo_api/appoint_parser/parsers/single_appo.py
-drwxrwxrwx   0        0        0        0 2022-09-15 17:24:22.119565 pravo-api-0.0.8/pravo_api/appoint_parser/tools/
--rw-rw-rw-   0        0        0       74 2022-09-15 16:37:00.000000 pravo-api-0.0.8/pravo_api/appoint_parser/tools/__init__.py
--rw-rw-rw-   0        0        0     9967 2022-09-15 16:39:17.000000 pravo-api-0.0.8/pravo_api/appoint_parser/tools/name_parser.py
--rw-rw-rw-   0        0        0     1058 2022-09-15 16:40:06.000000 pravo-api-0.0.8/pravo_api/appoint_parser/tools/text_cleaner.py
-drwxrwxrwx   0        0        0        0 2022-09-15 17:24:22.138022 pravo-api-0.0.8/pravo_api/appoint_parser/utils/
--rw-rw-rw-   0        0        0       22 2022-07-27 13:45:22.000000 pravo-api-0.0.8/pravo_api/appoint_parser/utils/__init__.py
--rw-rw-rw-   0        0        0      973 2022-09-13 17:42:01.000000 pravo-api-0.0.8/pravo_api/appoint_parser/utils/models.py
--rw-rw-rw-   0        0        0     3005 2022-09-15 16:32:31.000000 pravo-api-0.0.8/pravo_api/appoint_parser/utils/my_logger.py
--rw-rw-rw-   0        0        0        0 2022-09-13 13:59:26.000000 pravo-api-0.0.8/pravo_api/temp.py
--rw-rw-rw-   0        0        0     2154 2022-09-15 16:41:46.000000 pravo-api-0.0.8/pravo_api/worker.py
-drwxrwxrwx   0        0        0        0 2022-09-15 17:24:21.944383 pravo-api-0.0.8/pravo_api.egg-info/
--rw-rw-rw-   0        0        0    42814 2022-09-15 17:24:21.000000 pravo-api-0.0.8/pravo_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1231 2022-09-15 17:24:21.000000 pravo-api-0.0.8/pravo_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-15 17:24:21.000000 pravo-api-0.0.8/pravo_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      322 2022-09-15 17:24:21.000000 pravo-api-0.0.8/pravo_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-09-15 17:24:21.000000 pravo-api-0.0.8/pravo_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      742 2022-09-15 17:23:58.000000 pravo-api-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-09-15 17:24:22.141023 pravo-api-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0       39 2022-09-15 17:10:12.000000 pravo-api-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-10-02 11:33:41.263582 pravo-api-0.0.9/
+-rw-rw-rw-   0        0        0     1084 2022-09-15 17:04:01.000000 pravo-api-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0       82 2022-09-15 15:24:11.000000 pravo-api-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0    42814 2022-10-02 11:33:41.262581 pravo-api-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0    42558 2022-09-15 17:18:43.000000 pravo-api-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2022-10-02 11:33:41.207580 pravo-api-0.0.9/pravo_api/
+-rw-rw-rw-   0        0        0       28 2022-09-13 14:43:04.000000 pravo-api-0.0.9/pravo_api/__init__.py
+drwxrwxrwx   0        0        0        0 2022-10-02 11:33:41.231580 pravo-api-0.0.9/pravo_api/api/
+-rw-rw-rw-   0        0        0       27 2022-09-15 16:37:20.000000 pravo-api-0.0.9/pravo_api/api/__init__.py
+-rw-rw-rw-   0        0        0     5914 2022-09-15 16:37:59.000000 pravo-api-0.0.9/pravo_api/api/config.py
+drwxrwxrwx   0        0        0        0 2022-10-02 11:33:41.235586 pravo-api-0.0.9/pravo_api/api/downloader/
+-rw-rw-rw-   0        0        0       43 2022-09-15 16:34:14.000000 pravo-api-0.0.9/pravo_api/api/downloader/__init__.py
+-rw-rw-rw-   0        0        0     7100 2022-09-15 15:58:00.000000 pravo-api-0.0.9/pravo_api/api/downloader/aio_downloader.py
+-rw-rw-rw-   0        0        0      758 2022-09-14 07:41:42.000000 pravo-api-0.0.9/pravo_api/api/downloader/meta_data_getter.py
+drwxrwxrwx   0        0        0        0 2022-10-02 11:33:41.239584 pravo-api-0.0.9/pravo_api/api/links_getter/
+-rw-rw-rw-   0        0        0       37 2022-09-15 16:34:44.000000 pravo-api-0.0.9/pravo_api/api/links_getter/__init__.py
+-rw-rw-rw-   0        0        0    10093 2022-09-15 16:33:46.000000 pravo-api-0.0.9/pravo_api/api/links_getter/links_getter.py
+-rw-rw-rw-   0        0        0      221 2022-09-15 16:33:32.000000 pravo-api-0.0.9/pravo_api/api/links_getter/models.py
+-rw-rw-rw-   0        0        0     1087 2022-09-15 16:33:09.000000 pravo-api-0.0.9/pravo_api/api/main.py
+-rw-rw-rw-   0        0        0       39 2022-09-15 15:53:52.000000 pravo-api-0.0.9/pravo_api/api/temp.py
+drwxrwxrwx   0        0        0        0 2022-10-02 11:33:41.242584 pravo-api-0.0.9/pravo_api/api/utils/
+-rw-rw-rw-   0        0        0        0 2022-08-01 07:27:14.000000 pravo-api-0.0.9/pravo_api/api/utils/__init__.py
+-rw-rw-rw-   0        0        0     1694 2022-07-15 12:27:00.000000 pravo-api-0.0.9/pravo_api/api/utils/back_off.py
+-rw-rw-rw-   0        0        0     2260 2022-09-15 09:34:54.000000 pravo-api-0.0.9/pravo_api/api/utils/my_logger.py
+drwxrwxrwx   0        0        0        0 2022-10-02 11:33:41.247591 pravo-api-0.0.9/pravo_api/appoint_parser/
+-rw-rw-rw-   0        0        0       33 2022-09-15 16:35:19.000000 pravo-api-0.0.9/pravo_api/appoint_parser/__init__.py
+-rw-rw-rw-   0        0        0      509 2022-08-02 13:32:08.000000 pravo-api-0.0.9/pravo_api/appoint_parser/__main__.py
+-rw-rw-rw-   0        0        0     7357 2022-09-15 09:38:35.000000 pravo-api-0.0.9/pravo_api/appoint_parser/decree_parser.py
+drwxrwxrwx   0        0        0        0 2022-10-02 11:33:41.251581 pravo-api-0.0.9/pravo_api/appoint_parser/parsers/
+-rw-rw-rw-   0        0        0       88 2022-09-15 16:36:39.000000 pravo-api-0.0.9/pravo_api/appoint_parser/parsers/__init__.py
+-rw-rw-rw-   0        0        0     6140 2022-09-15 16:30:53.000000 pravo-api-0.0.9/pravo_api/appoint_parser/parsers/multi_app.py
+-rw-rw-rw-   0        0        0     6021 2022-09-15 15:58:00.000000 pravo-api-0.0.9/pravo_api/appoint_parser/parsers/single_appo.py
+drwxrwxrwx   0        0        0        0 2022-10-02 11:33:41.256580 pravo-api-0.0.9/pravo_api/appoint_parser/tools/
+-rw-rw-rw-   0        0        0       74 2022-09-15 16:37:00.000000 pravo-api-0.0.9/pravo_api/appoint_parser/tools/__init__.py
+-rw-rw-rw-   0        0        0     9967 2022-09-15 16:39:17.000000 pravo-api-0.0.9/pravo_api/appoint_parser/tools/name_parser.py
+-rw-rw-rw-   0        0        0     1058 2022-09-15 16:40:06.000000 pravo-api-0.0.9/pravo_api/appoint_parser/tools/text_cleaner.py
+drwxrwxrwx   0        0        0        0 2022-10-02 11:33:41.260580 pravo-api-0.0.9/pravo_api/appoint_parser/utils/
+-rw-rw-rw-   0        0        0       22 2022-07-27 13:45:22.000000 pravo-api-0.0.9/pravo_api/appoint_parser/utils/__init__.py
+-rw-rw-rw-   0        0        0      973 2022-09-13 17:42:01.000000 pravo-api-0.0.9/pravo_api/appoint_parser/utils/models.py
+-rw-rw-rw-   0        0        0     3005 2022-09-15 16:32:31.000000 pravo-api-0.0.9/pravo_api/appoint_parser/utils/my_logger.py
+-rw-rw-rw-   0        0        0        0 2022-09-13 13:59:26.000000 pravo-api-0.0.9/pravo_api/temp.py
+-rw-rw-rw-   0        0        0     2154 2022-09-15 16:41:46.000000 pravo-api-0.0.9/pravo_api/worker.py
+drwxrwxrwx   0        0        0        0 2022-10-02 11:33:41.226579 pravo-api-0.0.9/pravo_api.egg-info/
+-rw-rw-rw-   0        0        0    42814 2022-10-02 11:33:41.000000 pravo-api-0.0.9/pravo_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1231 2022-10-02 11:33:41.000000 pravo-api-0.0.9/pravo_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-10-02 11:33:41.000000 pravo-api-0.0.9/pravo_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      322 2022-10-02 11:33:41.000000 pravo-api-0.0.9/pravo_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2022-10-02 11:33:41.000000 pravo-api-0.0.9/pravo_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      742 2022-10-02 11:33:17.000000 pravo-api-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2022-10-02 11:33:41.264581 pravo-api-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0       66 2022-10-02 11:23:31.000000 pravo-api-0.0.9/setup.py
```

### Comparing `pravo-api-0.0.8/LICENSE` & `pravo-api-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pravo-api-0.0.8/PKG-INFO` & `pravo-api-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pravo-api
-Version: 0.0.8
+Version: 0.0.9
 Summary: Get Russian laws, federal and regional decrees.
 Author-email: Kirill Bondar <ironbondar@gmail.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 #  API портала правовой информации
```

### Comparing `pravo-api-0.0.8/README.md` & `pravo-api-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pravo-api-0.0.8/pravo_api/api/config.py` & `pravo-api-0.0.9/pravo_api/api/config.py`

 * *Files identical despite different names*

### Comparing `pravo-api-0.0.8/pravo_api/api/downloader/aio_downloader.py` & `pravo-api-0.0.9/pravo_api/api/downloader/aio_downloader.py`

 * *Files identical despite different names*

### Comparing `pravo-api-0.0.8/pravo_api/api/downloader/meta_data_getter.py` & `pravo-api-0.0.9/pravo_api/api/downloader/meta_data_getter.py`

 * *Files identical despite different names*

### Comparing `pravo-api-0.0.8/pravo_api/api/links_getter/links_getter.py` & `pravo-api-0.0.9/pravo_api/api/links_getter/links_getter.py`

 * *Files identical despite different names*

### Comparing `pravo-api-0.0.8/pravo_api/api/main.py` & `pravo-api-0.0.9/pravo_api/api/main.py`

 * *Files identical despite different names*

### Comparing `pravo-api-0.0.8/pravo_api/api/utils/back_off.py` & `pravo-api-0.0.9/pravo_api/api/utils/back_off.py`

 * *Files identical despite different names*

### Comparing `pravo-api-0.0.8/pravo_api/api/utils/my_logger.py` & `pravo-api-0.0.9/pravo_api/api/utils/my_logger.py`

 * *Files identical despite different names*

### Comparing `pravo-api-0.0.8/pravo_api/appoint_parser/decree_parser.py` & `pravo-api-0.0.9/pravo_api/appoint_parser/decree_parser.py`

 * *Files identical despite different names*

### Comparing `pravo-api-0.0.8/pravo_api/appoint_parser/parsers/multi_app.py` & `pravo-api-0.0.9/pravo_api/appoint_parser/parsers/multi_app.py`

 * *Files identical despite different names*

### Comparing `pravo-api-0.0.8/pravo_api/appoint_parser/parsers/single_appo.py` & `pravo-api-0.0.9/pravo_api/appoint_parser/parsers/single_appo.py`

 * *Files identical despite different names*

### Comparing `pravo-api-0.0.8/pravo_api/appoint_parser/tools/name_parser.py` & `pravo-api-0.0.9/pravo_api/appoint_parser/tools/name_parser.py`

 * *Files identical despite different names*

### Comparing `pravo-api-0.0.8/pravo_api/appoint_parser/tools/text_cleaner.py` & `pravo-api-0.0.9/pravo_api/appoint_parser/tools/text_cleaner.py`

 * *Files identical despite different names*

### Comparing `pravo-api-0.0.8/pravo_api/appoint_parser/utils/models.py` & `pravo-api-0.0.9/pravo_api/appoint_parser/utils/models.py`

 * *Files identical despite different names*

### Comparing `pravo-api-0.0.8/pravo_api/appoint_parser/utils/my_logger.py` & `pravo-api-0.0.9/pravo_api/appoint_parser/utils/my_logger.py`

 * *Files identical despite different names*

### Comparing `pravo-api-0.0.8/pravo_api/worker.py` & `pravo-api-0.0.9/pravo_api/worker.py`

 * *Files identical despite different names*

### Comparing `pravo-api-0.0.8/pravo_api.egg-info/PKG-INFO` & `pravo-api-0.0.9/pravo_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pravo-api
-Version: 0.0.8
+Version: 0.0.9
 Summary: Get Russian laws, federal and regional decrees.
 Author-email: Kirill Bondar <ironbondar@gmail.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 #  API портала правовой информации
```

### Comparing `pravo-api-0.0.8/pravo_api.egg-info/SOURCES.txt` & `pravo-api-0.0.9/pravo_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pravo-api-0.0.8/pyproject.toml` & `pravo-api-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pravo-api"
-version = "0.0.8"
+version = "0.0.9"
 description = "Get Russian laws, federal and regional decrees."
 readme = "README.md"
 authors = [{ name = "Kirill Bondar", email = "ironbondar@gmail.com" }]
 
 dependencies = [
 "requests>=2.27.1",
 "aiohttp>=3.8.1",
```

