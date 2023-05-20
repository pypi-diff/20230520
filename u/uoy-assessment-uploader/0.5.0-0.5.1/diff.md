# Comparing `tmp/uoy_assessment_uploader-0.5.0.tar.gz` & `tmp/uoy_assessment_uploader-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uoy_assessment_uploader-0.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "uoy_assessment_uploader-0.5.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `uoy_assessment_uploader-0.5.0.tar` & `uoy_assessment_uploader-0.5.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    32422 2023-05-20 19:23:43.854447 uoy_assessment_uploader-0.5.0/LICENSE
--rw-r--r--   0        0        0     1337 2023-05-20 19:23:43.854447 uoy_assessment_uploader-0.5.0/README.md
--rw-r--r--   0        0        0      767 2023-05-20 19:23:43.854447 uoy_assessment_uploader-0.5.0/pyproject.toml
--rwxr-xr-x   0        0        0     7144 2023-05-20 19:23:43.854447 uoy_assessment_uploader-0.5.0/uoy_assessment_uploader/__init__.py
--rw-r--r--   0        0        0       27 2023-05-20 19:23:43.854447 uoy_assessment_uploader-0.5.0/uoy_assessment_uploader/__main__.py
--rw-r--r--   0        0        0     2535 2023-05-20 19:23:43.854447 uoy_assessment_uploader-0.5.0/uoy_assessment_uploader/argument_parser.py
--rw-r--r--   0        0        0     2320 2023-05-20 19:23:43.854447 uoy_assessment_uploader-0.5.0/uoy_assessment_uploader/credentials.py
--rw-r--r--   0        0        0     6032 2023-05-20 19:23:43.854447 uoy_assessment_uploader-0.5.0/uoy_assessment_uploader/teaching-cs-york-ac-uk-chain.pem
--rw-r--r--   0        0        0     2007 1970-01-01 00:00:00.000000 uoy_assessment_uploader-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    32422 2023-05-20 19:32:40.780263 uoy_assessment_uploader-0.5.1/LICENSE
+-rw-r--r--   0        0        0     1399 2023-05-20 19:32:40.780263 uoy_assessment_uploader-0.5.1/README.md
+-rw-r--r--   0        0        0      857 2023-05-20 19:32:40.780263 uoy_assessment_uploader-0.5.1/pyproject.toml
+-rwxr-xr-x   0        0        0     7233 2023-05-20 19:32:40.780263 uoy_assessment_uploader-0.5.1/uoy_assessment_uploader/__init__.py
+-rw-r--r--   0        0        0       27 2023-05-20 19:32:40.780263 uoy_assessment_uploader-0.5.1/uoy_assessment_uploader/__main__.py
+-rw-r--r--   0        0        0     2535 2023-05-20 19:32:40.780263 uoy_assessment_uploader-0.5.1/uoy_assessment_uploader/argument_parser.py
+-rw-r--r--   0        0        0     2320 2023-05-20 19:32:40.780263 uoy_assessment_uploader-0.5.1/uoy_assessment_uploader/credentials.py
+-rw-r--r--   0        0        0     6032 2023-05-20 19:32:40.780263 uoy_assessment_uploader-0.5.1/uoy_assessment_uploader/teaching-cs-york-ac-uk-chain.pem
+-rw-r--r--   0        0        0     2174 1970-01-01 00:00:00.000000 uoy_assessment_uploader-0.5.1/PKG-INFO
```

### Comparing `uoy_assessment_uploader-0.5.0/LICENSE` & `uoy_assessment_uploader-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `uoy_assessment_uploader-0.5.0/README.md` & `uoy_assessment_uploader-0.5.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # uoy_assessment_uploader
 
-**If you have an open exam, help me test the new and improved version!! See here: https://github.com/joelsgp/uoy-assessment-uploader/pull/1**
+PyPI page: https://pypi.org/project/uoy-assessment-uploader/
 
+**If you have an open exam, help me test the new and improved version!! See here: https://github.com/joelsgp/uoy-assessment-uploader/pull/1**
 
 ## Install
 1. When you have Python and Pip ready, it's as easy as:
    ```shell
    python -m pip install "uoy-assessment-uploader"
    ```
    - or, directly from the repo:
@@ -31,14 +32,15 @@
 
 If this matches the hash shown by the program, you can be certain you successfully uploaded the right file.
 
 ## Example
 ```shell
 uoy-assessment-uploader --username "ab1234" --exam-number "Y1234567" --submit-url "/2021-2/submit/COM00012C/901/A"
 ```
+
 ```
 Found file 'exam.zip'.
 MD5 hash of file: 05086595c7c7c1a962d6eff6872e18c0
 Loading cookie file 'cookies.txt'
 No cookies to load!
 Logging in..
 Password: <PASSWORD HIDDEN>
```

### Comparing `uoy_assessment_uploader-0.5.0/pyproject.toml` & `uoy_assessment_uploader-0.5.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -5,18 +5,21 @@
 [project]
 name = "uoy-assessment-uploader"
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [{name = "jmcb", email = "joelsgp@protonmail.com"}]
 license = {file = "LICENSE"}
 classifiers = [
+    "Development Status :: 4 - Beta",
     "Environment :: Console",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Natural Language :: English",
     "Operating System :: OS Independent",
+    "Topic :: Education",
+    "Topic :: Utilities",
 ]
 dependencies = [
     "beautifulsoup4 ~= 4.12.2",
     "keyring ~= 23.13.1",
     "requests ~= 2.30.0",
 ]
 dynamic = ["version", "description"]
```

### Comparing `uoy_assessment_uploader-0.5.0/uoy_assessment_uploader/__init__.py` & `uoy_assessment_uploader-0.5.1/uoy_assessment_uploader/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     delete_from_keyring,
     ensure_exam_number,
     ensure_password,
     ensure_username,
 )
 
 
-__version__ = "0.5.0"
+__version__ = "0.5.1"
 
 
 # used for service_name in keyring calls
 # see here:
 # https://stackoverflow.com/questions/27068163/python-requests-not-handling-missing-intermediate-certificate-only-from-one-mach
 # https://pypi.org/project/aia/
 PEM_FILE = "teaching-cs-york-ac-uk-chain.pem"
@@ -114,43 +114,48 @@
     2. If login is requested, enter username and password with selenium. Get the shibsession cookie.
     3. Retrieve the csrf-token needed alongside the shibsession token for the next steps.
     3. If exam number is requested, submit exam number.
     4. Upload the actual file.
     """
     r = session.get(submit_url)
     r.raise_for_status()
-    token = get_token(r)
+    csrf_token = get_token(r)
 
     if r.url == URL_LOGIN:
         print("Logging in..")
         username = ensure_username(username)
         password = ensure_password(username, password, use_keyring=use_keyring)
         exam_number = ensure_exam_number(username, exam_number, use_keyring=use_keyring)
 
-        r = login_saml(session, username, password, token)
+        r = login_saml(
+            session,
+            csrf_token,
+            username,
+            password,
+        )
         # the token changes after login
-        token = get_token(r)
-        login_exam_number(session, token, exam_number)
+        csrf_token = get_token(r)
+        login_exam_number(session, csrf_token, exam_number)
         print("Logged in.")
     elif r.url == URL_EXAM_NUMBER:
         print("Entering exam number..")
         exam_number = ensure_exam_number(username, exam_number, use_keyring=use_keyring)
 
-        login_exam_number(session, token, exam_number)
+        login_exam_number(session, csrf_token, exam_number)
         print("Entered exam number.")
     elif r.url == submit_url:
         pass
     else:
         raise RuntimeError(f"Unexpected redirect '{r.url}'")
 
     print("Uploading file...")
     if dry_run:
         print("Skipped actual upload.")
     else:
-        r = upload_assignment(session, token, submit_url, file_path)
+        r = upload_assignment(session, csrf_token, submit_url, file_path)
         r.raise_for_status()
         print("Uploaded fine.")
 
 
 def resolve_submit_url(submit_url: str) -> str:
     base = URL_SUBMIT_BASE
     submit_url = submit_url.removeprefix(base).strip("/")
```

### Comparing `uoy_assessment_uploader-0.5.0/uoy_assessment_uploader/argument_parser.py` & `uoy_assessment_uploader-0.5.1/uoy_assessment_uploader/argument_parser.py`

 * *Files identical despite different names*

### Comparing `uoy_assessment_uploader-0.5.0/uoy_assessment_uploader/credentials.py` & `uoy_assessment_uploader-0.5.1/uoy_assessment_uploader/credentials.py`

 * *Files identical despite different names*

### Comparing `uoy_assessment_uploader-0.5.0/uoy_assessment_uploader/teaching-cs-york-ac-uk-chain.pem` & `uoy_assessment_uploader-0.5.1/uoy_assessment_uploader/teaching-cs-york-ac-uk-chain.pem`

 * *Files identical despite different names*

### Comparing `uoy_assessment_uploader-0.5.0/PKG-INFO` & `uoy_assessment_uploader-0.5.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 Metadata-Version: 2.1
 Name: uoy-assessment-uploader
-Version: 0.5.0
+Version: 0.5.1
 Summary: Tool for automating submitting assessments to the University of York Computer Science department.
 Author-email: jmcb <joelsgp@protonmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
+Classifier: Topic :: Education
+Classifier: Topic :: Utilities
 Requires-Dist: beautifulsoup4 ~= 4.12.2
 Requires-Dist: keyring ~= 23.13.1
 Requires-Dist: requests ~= 2.30.0
 Project-URL: Home, https://github.com/joelsgp/uoy-assessment-uploader
 
 # uoy_assessment_uploader
 
-**If you have an open exam, help me test the new and improved version!! See here: https://github.com/joelsgp/uoy-assessment-uploader/pull/1**
+PyPI page: https://pypi.org/project/uoy-assessment-uploader/
 
+**If you have an open exam, help me test the new and improved version!! See here: https://github.com/joelsgp/uoy-assessment-uploader/pull/1**
 
 ## Install
 1. When you have Python and Pip ready, it's as easy as:
    ```shell
    python -m pip install "uoy-assessment-uploader"
    ```
    - or, directly from the repo:
@@ -47,14 +51,15 @@
 
 If this matches the hash shown by the program, you can be certain you successfully uploaded the right file.
 
 ## Example
 ```shell
 uoy-assessment-uploader --username "ab1234" --exam-number "Y1234567" --submit-url "/2021-2/submit/COM00012C/901/A"
 ```
+
 ```
 Found file 'exam.zip'.
 MD5 hash of file: 05086595c7c7c1a962d6eff6872e18c0
 Loading cookie file 'cookies.txt'
 No cookies to load!
 Logging in..
 Password: <PASSWORD HIDDEN>
```

