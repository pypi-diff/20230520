# Comparing `tmp/crossmark-jotform-api-0.3.2.tar.gz` & `tmp/crossmark-jotform-api-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crossmark-jotform-api-0.3.2.tar", last modified: Thu May 18 22:11:55 2023, max compression
+gzip compressed data, was "crossmark-jotform-api-0.3.3.tar", last modified: Sat May 20 20:29:00 2023, max compression
```

## Comparing `crossmark-jotform-api-0.3.2.tar` & `crossmark-jotform-api-0.3.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 22:11:55.302960 crossmark-jotform-api-0.3.2/
--rw-rw-rw-   0        0        0     1091 2023-02-01 01:57:52.000000 crossmark-jotform-api-0.3.2/LICENSE
--rw-rw-rw-   0        0        0     2770 2023-05-18 22:11:55.302960 crossmark-jotform-api-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0      870 2023-05-16 18:35:40.000000 crossmark-jotform-api-0.3.2/README.md
--rw-rw-rw-   0        0        0      789 2023-05-18 22:10:35.000000 crossmark-jotform-api-0.3.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-18 22:11:55.302960 crossmark-jotform-api-0.3.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-18 22:11:55.282965 crossmark-jotform-api-0.3.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-18 22:11:55.287957 crossmark-jotform-api-0.3.2/src/crossmark_jotform_api/
--rw-rw-rw-   0        0        0    12736 2023-05-18 21:09:04.000000 crossmark-jotform-api-0.3.2/src/crossmark_jotform_api/jotForm.py
-drwxrwxrwx   0        0        0        0 2023-05-18 22:11:55.300955 crossmark-jotform-api-0.3.2/src/crossmark_jotform_api.egg-info/
--rw-rw-rw-   0        0        0     2770 2023-05-18 22:11:55.000000 crossmark-jotform-api-0.3.2/src/crossmark_jotform_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-05-18 22:11:55.000000 crossmark-jotform-api-0.3.2/src/crossmark_jotform_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 22:11:55.000000 crossmark-jotform-api-0.3.2/src/crossmark_jotform_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-05-18 22:11:55.000000 crossmark-jotform-api-0.3.2/src/crossmark_jotform_api.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-18 22:11:55.301956 crossmark-jotform-api-0.3.2/test/
--rw-rw-rw-   0        0        0      270 2023-05-10 23:06:10.000000 crossmark-jotform-api-0.3.2/test/test_jotform_class.py
+drwxrwxrwx   0        0        0        0 2023-05-20 20:29:00.387090 crossmark-jotform-api-0.3.3/
+-rw-rw-rw-   0        0        0     1091 2023-02-01 01:57:52.000000 crossmark-jotform-api-0.3.3/LICENSE
+-rw-rw-rw-   0        0        0     2770 2023-05-20 20:29:00.385892 crossmark-jotform-api-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0      870 2023-05-16 18:35:40.000000 crossmark-jotform-api-0.3.3/README.md
+-rw-rw-rw-   0        0        0      789 2023-05-20 20:25:57.000000 crossmark-jotform-api-0.3.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-20 20:29:00.387090 crossmark-jotform-api-0.3.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-20 20:29:00.372732 crossmark-jotform-api-0.3.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-20 20:29:00.376894 crossmark-jotform-api-0.3.3/src/crossmark_jotform_api/
+-rw-rw-rw-   0        0        0    12743 2023-05-20 20:25:52.000000 crossmark-jotform-api-0.3.3/src/crossmark_jotform_api/jotForm.py
+drwxrwxrwx   0        0        0        0 2023-05-20 20:29:00.382895 crossmark-jotform-api-0.3.3/src/crossmark_jotform_api.egg-info/
+-rw-rw-rw-   0        0        0     2770 2023-05-20 20:29:00.000000 crossmark-jotform-api-0.3.3/src/crossmark_jotform_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-05-20 20:29:00.000000 crossmark-jotform-api-0.3.3/src/crossmark_jotform_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 20:29:00.000000 crossmark-jotform-api-0.3.3/src/crossmark_jotform_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-05-20 20:29:00.000000 crossmark-jotform-api-0.3.3/src/crossmark_jotform_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-20 20:29:00.383893 crossmark-jotform-api-0.3.3/test/
+-rw-rw-rw-   0        0        0      270 2023-05-10 23:06:10.000000 crossmark-jotform-api-0.3.3/test/test_jotform_class.py
```

### Comparing `crossmark-jotform-api-0.3.2/LICENSE` & `crossmark-jotform-api-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `crossmark-jotform-api-0.3.2/PKG-INFO` & `crossmark-jotform-api-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossmark-jotform-api
-Version: 0.3.2
+Version: 0.3.3
 Summary: Jotform api integration dedicated for server usage which limits calls and calling form only if there is a new submission
 Author-email: Renas Mirkan Kilic <mirkanbaba1@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `crossmark-jotform-api-0.3.2/README.md` & `crossmark-jotform-api-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `crossmark-jotform-api-0.3.2/pyproject.toml` & `crossmark-jotform-api-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0","requests>=2.22.0","wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "crossmark-jotform-api"
-version = "0.3.2"
+version = "0.3.3"
 authors = [
   { name="Renas Mirkan Kilic", email="mirkanbaba1@gmail.com" },
 ]
 description = "Jotform api integration dedicated for server usage which limits calls and calling form only if there is a new submission"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.6"
```

### Comparing `crossmark-jotform-api-0.3.2/src/crossmark_jotform_api/jotForm.py` & `crossmark-jotform-api-0.3.3/src/crossmark_jotform_api/jotForm.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         return self.submission_count
 
     def get_submission_answers(self, submission_id):
         self.update()
         return self.submission_data[submission_id].answers
 
     def get_submission_by_request(self, submission_id):
-        requests.get("https://api.jotform.com/submission/" +
+        return requests.get("https://api.jotform.com/submission/" +
                      submission_id + "?apiKey=" + self.api_key, timeout=self.timeout)
 
     def get_submission(self, submission_id):
         return self.submission_data[submission_id]
 
     def get_submission_id_by_text(self, text):
         for key, submission_object in self.submission_data.items():
```

### Comparing `crossmark-jotform-api-0.3.2/src/crossmark_jotform_api.egg-info/PKG-INFO` & `crossmark-jotform-api-0.3.3/src/crossmark_jotform_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossmark-jotform-api
-Version: 0.3.2
+Version: 0.3.3
 Summary: Jotform api integration dedicated for server usage which limits calls and calling form only if there is a new submission
 Author-email: Renas Mirkan Kilic <mirkanbaba1@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

