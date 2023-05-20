# Comparing `tmp/vector_vault-0.1.tar.gz` & `tmp/vector_vault-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-0.1.tar", last modified: Sat May 20 06:19:56 2023, max compression
+gzip compressed data, was "vector_vault-0.1.1.tar", last modified: Sat May 20 06:44:07 2023, max compression
```

## Comparing `vector_vault-0.1.tar` & `vector_vault-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-20 06:19:56.652284 vector_vault-0.1/
--rw-r--r--   0 johnrood   (501) staff       (20)      688 2023-05-20 04:34:30.000000 vector_vault-0.1/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)     9739 2023-05-20 06:19:56.652121 vector_vault-0.1/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)     8973 2023-05-20 06:01:46.000000 vector_vault-0.1/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-05-20 06:19:56.652323 vector_vault-0.1/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1083 2023-05-20 06:19:52.000000 vector_vault-0.1/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-20 06:19:56.651356 vector_vault-0.1/vector_vault/
--rw-r--r--   0 johnrood   (501) staff       (20)      675 2023-05-20 04:33:21.000000 vector_vault-0.1/vector_vault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3660 2023-05-20 06:06:36.000000 vector_vault-0.1/vector_vault/closedai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3331 2023-05-20 04:21:10.000000 vector_vault-0.1/vector_vault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1855 2023-05-20 04:21:04.000000 vector_vault-0.1/vector_vault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-0.1/vector_vault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)    18515 2023-05-20 05:51:36.000000 vector_vault-0.1/vector_vault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-0.1/vector_vault/wrap.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-20 06:19:56.651959 vector_vault-0.1/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)     9739 2023-05-20 06:19:56.000000 vector_vault-0.1/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      374 2023-05-20 06:19:56.000000 vector_vault-0.1/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-05-20 06:19:56.000000 vector_vault-0.1/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       53 2023-05-20 06:19:56.000000 vector_vault-0.1/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       13 2023-05-20 06:19:56.000000 vector_vault-0.1/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-20 06:44:07.202324 vector_vault-0.1.1/
+-rw-r--r--   0 johnrood   (501) staff       (20)      688 2023-05-20 04:34:30.000000 vector_vault-0.1.1/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)     9738 2023-05-20 06:44:07.202173 vector_vault-0.1.1/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)     8973 2023-05-20 06:01:46.000000 vector_vault-0.1.1/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-05-20 06:44:07.202362 vector_vault-0.1.1/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1082 2023-05-20 06:44:04.000000 vector_vault-0.1.1/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-20 06:44:07.201296 vector_vault-0.1.1/vector_vault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      675 2023-05-20 04:33:21.000000 vector_vault-0.1.1/vector_vault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3660 2023-05-20 06:06:36.000000 vector_vault-0.1.1/vector_vault/closedai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3331 2023-05-20 04:21:10.000000 vector_vault-0.1.1/vector_vault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1855 2023-05-20 04:21:04.000000 vector_vault-0.1.1/vector_vault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-0.1.1/vector_vault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    18515 2023-05-20 06:39:24.000000 vector_vault-0.1.1/vector_vault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-0.1.1/vector_vault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-20 06:44:07.201974 vector_vault-0.1.1/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)     9738 2023-05-20 06:44:07.000000 vector_vault-0.1.1/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      374 2023-05-20 06:44:07.000000 vector_vault-0.1.1/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-05-20 06:44:07.000000 vector_vault-0.1.1/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       53 2023-05-20 06:44:07.000000 vector_vault-0.1.1/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       13 2023-05-20 06:44:07.000000 vector_vault-0.1.1/vector_vault.egg-info/top_level.txt
```

### Comparing `vector_vault-0.1/LICENSE` & `vector_vault-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-0.1/PKG-INFO` & `vector_vault-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 0.1
+Version: 0.1.1
 Summary: Vector Vault: Simplified vector database management and secure cloud storage for data science and machine learning workflows.
-Home-page: http://github.com/yourusername/vector_vault
+Home-page: http://github.com/John-Rood/vector_vault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vector_vault-0.1/README.md` & `vector_vault-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-0.1/setup.py` & `vector_vault-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="0.1",
+    version="0.1.1",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="Vector Vault: Simplified vector database management and secure cloud storage for data science and machine learning workflows.",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
-    url="http://github.com/yourusername/vector_vault",
+    url="http://github.com/John-Rood/vector_vault",
     classifiers=[
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
```

### Comparing `vector_vault-0.1/vector_vault/__init__.py` & `vector_vault-0.1.1/vector_vault/__init__.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.1/vector_vault/closedai.py` & `vector_vault-0.1.1/vector_vault/closedai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.1/vector_vault/cloudmanager.py` & `vector_vault-0.1.1/vector_vault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.1/vector_vault/creds.py` & `vector_vault-0.1.1/vector_vault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.1/vector_vault/download.py` & `vector_vault-0.1.1/vector_vault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.1/vector_vault/vault.py` & `vector_vault-0.1.1/vector_vault/vault.py`

 * *Files 0% similar despite different names*

```diff
@@ -418,15 +418,15 @@
         if not history:
             history = ''
         
         time.sleep(self.needed_sleep_time)
 
         if len(text) > 15000:
             if summary:
-                inputs = self.split_text(text, 15000)
+                inputs = self.split_text(text, 14000)
             else:
                 inputs = self.split_text(text)
         else:
             inputs = [text]
         response = ''
         for segment in inputs:
             start_time = time.time()
```

### Comparing `vector_vault-0.1/vector_vault/wrap.py` & `vector_vault-0.1.1/vector_vault/wrap.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.1/vector_vault.egg-info/PKG-INFO` & `vector_vault-0.1.1/vector_vault.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 0.1
+Version: 0.1.1
 Summary: Vector Vault: Simplified vector database management and secure cloud storage for data science and machine learning workflows.
-Home-page: http://github.com/yourusername/vector_vault
+Home-page: http://github.com/John-Rood/vector_vault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

