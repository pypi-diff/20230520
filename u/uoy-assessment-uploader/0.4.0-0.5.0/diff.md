# Comparing `tmp/uoy-assessment-uploader-0.4.0.tar.gz` & `tmp/uoy_assessment_uploader-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uoy-assessment-uploader-0.4.0.tar", last modified: Fri May 12 20:03:35 2023, max compression
+gzip compressed data, was "uoy_assessment_uploader-0.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `uoy-assessment-uploader-0.4.0.tar` & `uoy_assessment_uploader-0.5.0.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0    32422 2023-05-12 20:03:22.969493 uoy-assessment-uploader-0.4.0/LICENSE
--rw-r--r--   0        0        0     1369 2023-05-12 20:03:22.969493 uoy-assessment-uploader-0.4.0/README.md
--rw-r--r--   0        0        0      768 2023-05-12 20:03:22.969493 uoy-assessment-uploader-0.4.0/pyproject.toml
--rwxr-xr-x   0        0        0     7942 2023-05-12 20:03:22.973493 uoy-assessment-uploader-0.4.0/uoy_assessment_uploader/__init__.py
--rw-r--r--   0        0        0       27 2023-05-12 20:03:22.973493 uoy-assessment-uploader-0.4.0/uoy_assessment_uploader/__main__.py
--rw-r--r--   0        0        0     1551 2023-05-12 20:03:22.973493 uoy-assessment-uploader-0.4.0/uoy_assessment_uploader/selenium.py
--rw-r--r--   0        0        0     2040 1970-01-01 00:00:00.000000 uoy-assessment-uploader-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    32422 2023-05-20 19:23:43.854447 uoy_assessment_uploader-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1337 2023-05-20 19:23:43.854447 uoy_assessment_uploader-0.5.0/README.md
+-rw-r--r--   0        0        0      767 2023-05-20 19:23:43.854447 uoy_assessment_uploader-0.5.0/pyproject.toml
+-rwxr-xr-x   0        0        0     7144 2023-05-20 19:23:43.854447 uoy_assessment_uploader-0.5.0/uoy_assessment_uploader/__init__.py
+-rw-r--r--   0        0        0       27 2023-05-20 19:23:43.854447 uoy_assessment_uploader-0.5.0/uoy_assessment_uploader/__main__.py
+-rw-r--r--   0        0        0     2535 2023-05-20 19:23:43.854447 uoy_assessment_uploader-0.5.0/uoy_assessment_uploader/argument_parser.py
+-rw-r--r--   0        0        0     2320 2023-05-20 19:23:43.854447 uoy_assessment_uploader-0.5.0/uoy_assessment_uploader/credentials.py
+-rw-r--r--   0        0        0     6032 2023-05-20 19:23:43.854447 uoy_assessment_uploader-0.5.0/uoy_assessment_uploader/teaching-cs-york-ac-uk-chain.pem
+-rw-r--r--   0        0        0     2007 1970-01-01 00:00:00.000000 uoy_assessment_uploader-0.5.0/PKG-INFO
```

### Comparing `uoy-assessment-uploader-0.4.0/LICENSE` & `uoy_assessment_uploader-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `uoy-assessment-uploader-0.4.0/pyproject.toml` & `uoy_assessment_uploader-0.5.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 classifiers = [
     "Environment :: Console",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Natural Language :: English",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "selenium ~= 4.9.0",
-    "webdriver-manager ~= 3.8.6",
+    "beautifulsoup4 ~= 4.12.2",
     "keyring ~= 23.13.1",
+    "requests ~= 2.30.0",
 ]
 dynamic = ["version", "description"]
 
 [project.urls]
 Home = "https://github.com/joelsgp/uoy-assessment-uploader"
 
 [project.scripts]
```

### Comparing `uoy-assessment-uploader-0.4.0/PKG-INFO` & `uoy_assessment_uploader-0.5.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 Metadata-Version: 2.1
 Name: uoy-assessment-uploader
-Version: 0.4.0
+Version: 0.5.0
 Summary: Tool for automating submitting assessments to the University of York Computer Science department.
 Author-email: jmcb <joelsgp@protonmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Requires-Dist: selenium ~= 4.9.0
-Requires-Dist: webdriver-manager ~= 3.8.6
+Requires-Dist: beautifulsoup4 ~= 4.12.2
 Requires-Dist: keyring ~= 23.13.1
+Requires-Dist: requests ~= 2.30.0
 Project-URL: Home, https://github.com/joelsgp/uoy-assessment-uploader
 
 # uoy_assessment_uploader
 
+**If you have an open exam, help me test the new and improved version!! See here: https://github.com/joelsgp/uoy-assessment-uploader/pull/1**
+
+
 ## Install
 1. When you have Python and Pip ready, it's as easy as:
    ```shell
    python -m pip install "uoy-assessment-uploader"
    ```
    - or, directly from the repo:
       ```shell
       python -m pip install "git+https://github.com/joelsgp/uoy-assessment-uploader"
       ```
-2. You need the Chrome browser installed. Sorry!
-    - I need a cookie management feature Firefox doesn't have.
-    - Chromium and Ungoogled Chrome should work too.
+2. As shrimple as that
 
 ## Use
 Like this:
 - ```shell
   python -m uoy_assessment_uploader --help
   ```
   or
@@ -49,18 +50,20 @@
 ## Example
 ```shell
 uoy-assessment-uploader --username "ab1234" --exam-number "Y1234567" --submit-url "/2021-2/submit/COM00012C/901/A"
 ```
 ```
 Found file 'exam.zip'.
 MD5 hash of file: 05086595c7c7c1a962d6eff6872e18c0
-[WDM] - Downloading: 100%|██████████| 6.98M/6.98M [00:00<00:00, 8.98MB/s]
-Loading cookies.
+Loading cookie file 'cookies.txt'
+No cookies to load!
 Logging in..
 Password: <PASSWORD HIDDEN>
+Logged in.
 Entering exam number..
+Entered exam number.
 Uploading file...
-Uploaded successfully.
-Saving cookies.
+Uploaded fine.
+Saved cookies.
 Finished!
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

