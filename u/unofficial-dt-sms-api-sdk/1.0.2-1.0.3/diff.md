# Comparing `tmp/unofficial-dt-sms-api-sdk-1.0.2.tar.gz` & `tmp/unofficial-dt-sms-api-sdk-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unofficial-dt-sms-api-sdk-1.0.2.tar", last modified: Thu May 18 19:12:04 2023, max compression
+gzip compressed data, was "unofficial-dt-sms-api-sdk-1.0.3.tar", last modified: Sat May 20 16:31:32 2023, max compression
```

## Comparing `unofficial-dt-sms-api-sdk-1.0.2.tar` & `unofficial-dt-sms-api-sdk-1.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:12:04.597357 unofficial-dt-sms-api-sdk-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-18 19:11:54.000000 unofficial-dt-sms-api-sdk-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-18 19:11:54.000000 unofficial-dt-sms-api-sdk-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-05-18 19:12:04.597357 unofficial-dt-sms-api-sdk-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10014 2023-05-18 19:11:54.000000 unofficial-dt-sms-api-sdk-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:12:04.597357 unofficial-dt-sms-api-sdk-1.0.2/dt_sms_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-18 19:11:54.000000 unofficial-dt-sms-api-sdk-1.0.2/dt_sms_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20174 2023-05-18 19:11:54.000000 unofficial-dt-sms-api-sdk-1.0.2/dt_sms_sdk/account.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-18 19:11:54.000000 unofficial-dt-sms-api-sdk-1.0.2/dt_sms_sdk/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    16215 2023-05-18 19:11:54.000000 unofficial-dt-sms-api-sdk-1.0.2/dt_sms_sdk/iso2_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     9663 2023-05-18 19:11:54.000000 unofficial-dt-sms-api-sdk-1.0.2/dt_sms_sdk/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-05-18 19:11:54.000000 unofficial-dt-sms-api-sdk-1.0.2/dt_sms_sdk/phone_number.py
--rw-r--r--   0 runner    (1001) docker     (123)    39567 2023-05-18 19:11:54.000000 unofficial-dt-sms-api-sdk-1.0.2/dt_sms_sdk/pricing.py
--rw-r--r--   0 runner    (1001) docker     (123)    18260 2023-05-18 19:11:54.000000 unofficial-dt-sms-api-sdk-1.0.2/dt_sms_sdk/sms_api.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-18 19:11:54.000000 unofficial-dt-sms-api-sdk-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-18 19:11:54.000000 unofficial-dt-sms-api-sdk-1.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 19:12:04.597357 unofficial-dt-sms-api-sdk-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-18 19:11:54.000000 unofficial-dt-sms-api-sdk-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:12:04.597357 unofficial-dt-sms-api-sdk-1.0.2/unofficial_dt_sms_api_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-05-18 19:12:04.000000 unofficial-dt-sms-api-sdk-1.0.2/unofficial_dt_sms_api_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-18 19:12:04.000000 unofficial-dt-sms-api-sdk-1.0.2/unofficial_dt_sms_api_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 19:12:04.000000 unofficial-dt-sms-api-sdk-1.0.2/unofficial_dt_sms_api_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-18 19:12:04.000000 unofficial-dt-sms-api-sdk-1.0.2/unofficial_dt_sms_api_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-18 19:12:04.000000 unofficial-dt-sms-api-sdk-1.0.2/unofficial_dt_sms_api_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 16:31:32.541830 unofficial-dt-sms-api-sdk-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-20 16:31:22.000000 unofficial-dt-sms-api-sdk-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-20 16:31:22.000000 unofficial-dt-sms-api-sdk-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10533 2023-05-20 16:31:32.541830 unofficial-dt-sms-api-sdk-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10187 2023-05-20 16:31:22.000000 unofficial-dt-sms-api-sdk-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 16:31:32.541830 unofficial-dt-sms-api-sdk-1.0.3/dt_sms_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-20 16:31:22.000000 unofficial-dt-sms-api-sdk-1.0.3/dt_sms_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20174 2023-05-20 16:31:22.000000 unofficial-dt-sms-api-sdk-1.0.3/dt_sms_sdk/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-20 16:31:22.000000 unofficial-dt-sms-api-sdk-1.0.3/dt_sms_sdk/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16215 2023-05-20 16:31:22.000000 unofficial-dt-sms-api-sdk-1.0.3/dt_sms_sdk/iso2_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9663 2023-05-20 16:31:22.000000 unofficial-dt-sms-api-sdk-1.0.3/dt_sms_sdk/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-05-20 16:31:22.000000 unofficial-dt-sms-api-sdk-1.0.3/dt_sms_sdk/phone_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39567 2023-05-20 16:31:22.000000 unofficial-dt-sms-api-sdk-1.0.3/dt_sms_sdk/pricing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18260 2023-05-20 16:31:22.000000 unofficial-dt-sms-api-sdk-1.0.3/dt_sms_sdk/sms_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-20 16:31:22.000000 unofficial-dt-sms-api-sdk-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-20 16:31:22.000000 unofficial-dt-sms-api-sdk-1.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 16:31:32.541830 unofficial-dt-sms-api-sdk-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-20 16:31:22.000000 unofficial-dt-sms-api-sdk-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 16:31:32.541830 unofficial-dt-sms-api-sdk-1.0.3/unofficial_dt_sms_api_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10533 2023-05-20 16:31:32.000000 unofficial-dt-sms-api-sdk-1.0.3/unofficial_dt_sms_api_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-20 16:31:32.000000 unofficial-dt-sms-api-sdk-1.0.3/unofficial_dt_sms_api_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 16:31:32.000000 unofficial-dt-sms-api-sdk-1.0.3/unofficial_dt_sms_api_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-20 16:31:32.000000 unofficial-dt-sms-api-sdk-1.0.3/unofficial_dt_sms_api_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-20 16:31:32.000000 unofficial-dt-sms-api-sdk-1.0.3/unofficial_dt_sms_api_sdk.egg-info/top_level.txt
```

### Comparing `unofficial-dt-sms-api-sdk-1.0.2/LICENSE` & `unofficial-dt-sms-api-sdk-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `unofficial-dt-sms-api-sdk-1.0.2/PKG-INFO` & `unofficial-dt-sms-api-sdk-1.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: unofficial-dt-sms-api-sdk
-Version: 1.0.2
-Summary: Unofficial Python-SDK for the SMS API of Deutsche Telekom
-Home-page: https://github.com/Anrufliste/dt-sms-api-sdk-python
-Author: Emil Thies
-Author-email: uDTSMSAPISDK@anrufliste.com
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # dt-sms-api-sdk-python ![GitHub release (latest by date)](https://img.shields.io/github/v/release/Anrufliste/dt-sms-api-sdk-python) [![Test](https://github.com/Anrufliste/dt-sms-api-sdk-python/actions/workflows/test.yml/badge.svg)](https://github.com/Anrufliste/dt-sms-api-sdk-python/actions/workflows/test.yml)
 
 This library is meant as an unofficial SDK (Software Development Kit) for the [Deutsche Telekom Developer SMS API](https://developer.telekom.com/products/sms-api/summary) and to give Python developers a quick start to use it withing their code.
 
 Please read the instructions on Deutsche Telekom Developer Portal and set up your account there to get the needed credentials. To use the SDK, you may install it with pip:
 
 ```
@@ -126,15 +115,15 @@
 
 The next step is to use this SMSAPIClient object and give it the message to send:
 
 ```
 response = c.send(message=m)
 ```
 
-Be aware, that multiple exceptions can happen while trying to send an SMS. In general they are from the type SMSAPIError and specified with descended types. So please invoke that method with a try block!
+Be aware, that multiple exceptions can happen while trying to send an SMS. In general, they are from the type SMSAPIError and specified with descended types. An  [example script](https://github.com/Anrufliste/dt-sms-api-sdk-python/tree/main/examples/using_token.py) is provided, which just needs your token and sender phone number (which is also taken as the receiver number).
 
 #### Status
 
 The response of the send method above will return an object of the class SMSAPIResponse, which includes a direct status of the invocation and the sid of the request, to query the status later on to see when/if the SMS got delivered. Just invoke the status method with the sid (or for easiness with the response itself - the method will take the sid itself ) and you will get a new SMSAPIResponse object for that Message.
 
 ```
 updated_response = c.status(response)
```

### Comparing `unofficial-dt-sms-api-sdk-1.0.2/README.md` & `unofficial-dt-sms-api-sdk-1.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: unofficial-dt-sms-api-sdk
+Version: 1.0.3
+Summary: Unofficial Python-SDK for the SMS API of Deutsche Telekom
+Home-page: https://github.com/Anrufliste/dt-sms-api-sdk-python
+Author: Emil Thies
+Author-email: uDTSMSAPISDK@anrufliste.com
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # dt-sms-api-sdk-python ![GitHub release (latest by date)](https://img.shields.io/github/v/release/Anrufliste/dt-sms-api-sdk-python) [![Test](https://github.com/Anrufliste/dt-sms-api-sdk-python/actions/workflows/test.yml/badge.svg)](https://github.com/Anrufliste/dt-sms-api-sdk-python/actions/workflows/test.yml)
 
 This library is meant as an unofficial SDK (Software Development Kit) for the [Deutsche Telekom Developer SMS API](https://developer.telekom.com/products/sms-api/summary) and to give Python developers a quick start to use it withing their code.
 
 Please read the instructions on Deutsche Telekom Developer Portal and set up your account there to get the needed credentials. To use the SDK, you may install it with pip:
 
 ```
@@ -115,15 +126,15 @@
 
 The next step is to use this SMSAPIClient object and give it the message to send:
 
 ```
 response = c.send(message=m)
 ```
 
-Be aware, that multiple exceptions can happen while trying to send an SMS. In general they are from the type SMSAPIError and specified with descended types. So please invoke that method with a try block!
+Be aware, that multiple exceptions can happen while trying to send an SMS. In general, they are from the type SMSAPIError and specified with descended types. An  [example script](https://github.com/Anrufliste/dt-sms-api-sdk-python/tree/main/examples/using_token.py) is provided, which just needs your token and sender phone number (which is also taken as the receiver number).
 
 #### Status
 
 The response of the send method above will return an object of the class SMSAPIResponse, which includes a direct status of the invocation and the sid of the request, to query the status later on to see when/if the SMS got delivered. Just invoke the status method with the sid (or for easiness with the response itself - the method will take the sid itself ) and you will get a new SMSAPIResponse object for that Message.
 
 ```
 updated_response = c.status(response)
```

### Comparing `unofficial-dt-sms-api-sdk-1.0.2/dt_sms_sdk/account.py` & `unofficial-dt-sms-api-sdk-1.0.3/dt_sms_sdk/account.py`

 * *Files identical despite different names*

### Comparing `unofficial-dt-sms-api-sdk-1.0.2/dt_sms_sdk/iso2_mapper.py` & `unofficial-dt-sms-api-sdk-1.0.3/dt_sms_sdk/iso2_mapper.py`

 * *Files identical despite different names*

### Comparing `unofficial-dt-sms-api-sdk-1.0.2/dt_sms_sdk/message.py` & `unofficial-dt-sms-api-sdk-1.0.3/dt_sms_sdk/message.py`

 * *Files identical despite different names*

### Comparing `unofficial-dt-sms-api-sdk-1.0.2/dt_sms_sdk/phone_number.py` & `unofficial-dt-sms-api-sdk-1.0.3/dt_sms_sdk/phone_number.py`

 * *Files identical despite different names*

### Comparing `unofficial-dt-sms-api-sdk-1.0.2/dt_sms_sdk/pricing.py` & `unofficial-dt-sms-api-sdk-1.0.3/dt_sms_sdk/pricing.py`

 * *Files identical despite different names*

### Comparing `unofficial-dt-sms-api-sdk-1.0.2/dt_sms_sdk/sms_api.py` & `unofficial-dt-sms-api-sdk-1.0.3/dt_sms_sdk/sms_api.py`

 * *Files identical despite different names*

### Comparing `unofficial-dt-sms-api-sdk-1.0.2/setup.py` & `unofficial-dt-sms-api-sdk-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 setuptools.setup(
     name="unofficial-dt-sms-api-sdk",
     description="Unofficial Python-SDK for the SMS API of Deutsche Telekom",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version="1.0.2",
+    version="1.0.3",
     url="https://github.com/Anrufliste/dt-sms-api-sdk-python",
     author='Emil Thies',
     author_email='uDTSMSAPISDK@anrufliste.com',
     python_requires='>=3.7',
     packages=['dt_sms_sdk'],
     package_dir={'dt_sms_sdk': 'dt_sms_sdk'},
     install_requires=requirements
```

### Comparing `unofficial-dt-sms-api-sdk-1.0.2/unofficial_dt_sms_api_sdk.egg-info/PKG-INFO` & `unofficial-dt-sms-api-sdk-1.0.3/unofficial_dt_sms_api_sdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unofficial-dt-sms-api-sdk
-Version: 1.0.2
+Version: 1.0.3
 Summary: Unofficial Python-SDK for the SMS API of Deutsche Telekom
 Home-page: https://github.com/Anrufliste/dt-sms-api-sdk-python
 Author: Emil Thies
 Author-email: uDTSMSAPISDK@anrufliste.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -126,15 +126,15 @@
 
 The next step is to use this SMSAPIClient object and give it the message to send:
 
 ```
 response = c.send(message=m)
 ```
 
-Be aware, that multiple exceptions can happen while trying to send an SMS. In general they are from the type SMSAPIError and specified with descended types. So please invoke that method with a try block!
+Be aware, that multiple exceptions can happen while trying to send an SMS. In general, they are from the type SMSAPIError and specified with descended types. An  [example script](https://github.com/Anrufliste/dt-sms-api-sdk-python/tree/main/examples/using_token.py) is provided, which just needs your token and sender phone number (which is also taken as the receiver number).
 
 #### Status
 
 The response of the send method above will return an object of the class SMSAPIResponse, which includes a direct status of the invocation and the sid of the request, to query the status later on to see when/if the SMS got delivered. Just invoke the status method with the sid (or for easiness with the response itself - the method will take the sid itself ) and you will get a new SMSAPIResponse object for that Message.
 
 ```
 updated_response = c.status(response)
```

