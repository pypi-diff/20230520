# Comparing `tmp/baiduads-sdk-2023.0.0.tar.gz` & `tmp/baiduads-sdk-2023.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baiduads-sdk-2023.0.0.tar", last modified: Tue Jan 31 03:42:34 2023, max compression
+gzip compressed data, was "baiduads-sdk-2023.1.0.tar", last modified: Sat May 20 03:53:02 2023, max compression
```

## Comparing `baiduads-sdk-2023.0.0.tar` & `baiduads-sdk-2023.1.0.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 03:42:34.312292 baiduads-sdk-2023.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-01-31 03:42:34.312292 baiduads-sdk-2023.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 03:42:34.304293 baiduads-sdk-2023.0.0/baiduads_manual/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 03:42:12.000000 baiduads-sdk-2023.0.0/baiduads_manual/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 03:42:34.304293 baiduads-sdk-2023.0.0/baiduads_manual/marketingfile/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 03:42:12.000000 baiduads-sdk-2023.0.0/baiduads_manual/marketingfile/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 03:42:34.304293 baiduads-sdk-2023.0.0/baiduads_manual/marketingfile/api/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-01-31 03:42:12.000000 baiduads-sdk-2023.0.0/baiduads_manual/marketingfile/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-01-31 03:42:12.000000 baiduads-sdk-2023.0.0/baiduads_manual/marketingfile/api/marketing_file_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 03:42:34.308292 baiduads-sdk-2023.0.0/baiduads_manual/marketingfile/model/
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-01-31 03:42:12.000000 baiduads-sdk-2023.0.0/baiduads_manual/marketingfile/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10823 2023-01-31 03:42:12.000000 baiduads-sdk-2023.0.0/baiduads_manual/marketingfile/model/upload_file_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-01-31 03:42:12.000000 baiduads-sdk-2023.0.0/baiduads_manual/marketingfile/model/upload_file_params.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-01-31 03:42:12.000000 baiduads-sdk-2023.0.0/baiduads_manual/marketingfile/model/upload_file_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-01-31 03:42:12.000000 baiduads-sdk-2023.0.0/baiduads_manual/marketingfile/model/upload_file_request_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    11078 2023-01-31 03:42:12.000000 baiduads-sdk-2023.0.0/baiduads_manual/marketingfile/model/upload_file_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11465 2023-01-31 03:42:12.000000 baiduads-sdk-2023.0.0/baiduads_manual/marketingfile/model/upload_file_response_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 03:42:34.308292 baiduads-sdk-2023.0.0/baiduads_manual/oauth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 03:42:12.000000 baiduads-sdk-2023.0.0/baiduads_manual/oauth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 03:42:34.308292 baiduads-sdk-2023.0.0/baiduads_manual/oauth/api/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-01-31 03:42:12.000000 baiduads-sdk-2023.0.0/baiduads_manual/oauth/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7391 2023-01-31 03:42:12.000000 baiduads-sdk-2023.0.0/baiduads_manual/oauth/api/oauth_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 03:42:34.308292 baiduads-sdk-2023.0.0/baiduads_manual/oauth/model/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-01-31 03:42:12.000000 baiduads-sdk-2023.0.0/baiduads_manual/oauth/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-01-31 03:42:12.000000 baiduads-sdk-2023.0.0/baiduads_manual/oauth/model/access_token_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-01-31 03:42:12.000000 baiduads-sdk-2023.0.0/baiduads_manual/oauth/model/get_access_token_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-01-31 03:42:12.000000 baiduads-sdk-2023.0.0/baiduads_manual/oauth/model/get_access_token_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-01-31 03:42:12.000000 baiduads-sdk-2023.0.0/baiduads_manual/oauth/model/get_open_id_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-01-31 03:42:12.000000 baiduads-sdk-2023.0.0/baiduads_manual/oauth/model/get_open_id_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-01-31 03:42:12.000000 baiduads-sdk-2023.0.0/baiduads_manual/oauth/model/get_user_info_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-01-31 03:42:12.000000 baiduads-sdk-2023.0.0/baiduads_manual/oauth/model/get_user_info_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-01-31 03:42:12.000000 baiduads-sdk-2023.0.0/baiduads_manual/oauth/model/open_id_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-01-31 03:42:12.000000 baiduads-sdk-2023.0.0/baiduads_manual/oauth/model/refresh_token_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-01-31 03:42:12.000000 baiduads-sdk-2023.0.0/baiduads_manual/oauth/model/refresh_token_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-01-31 03:42:12.000000 baiduads-sdk-2023.0.0/baiduads_manual/oauth/model/sub_user_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-01-31 03:42:12.000000 baiduads-sdk-2023.0.0/baiduads_manual/oauth/model/user_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 03:42:34.308292 baiduads-sdk-2023.0.0/baiduads_manual/upload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 03:42:12.000000 baiduads-sdk-2023.0.0/baiduads_manual/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-01-31 03:42:12.000000 baiduads-sdk-2023.0.0/baiduads_manual/upload/mulitupload_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    14767 2023-01-31 03:42:12.000000 baiduads-sdk-2023.0.0/baiduads_manual/upload/upload_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 03:42:34.308292 baiduads-sdk-2023.0.0/baiduads_manual/videoupload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 03:42:12.000000 baiduads-sdk-2023.0.0/baiduads_manual/videoupload/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 03:42:34.308292 baiduads-sdk-2023.0.0/baiduads_manual/videoupload/api/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-01-31 03:42:12.000000 baiduads-sdk-2023.0.0/baiduads_manual/videoupload/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-01-31 03:42:12.000000 baiduads-sdk-2023.0.0/baiduads_manual/videoupload/api/video_upload_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 03:42:34.308292 baiduads-sdk-2023.0.0/baiduads_manual/videoupload/model/
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-01-31 03:42:12.000000 baiduads-sdk-2023.0.0/baiduads_manual/videoupload/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-01-31 03:42:12.000000 baiduads-sdk-2023.0.0/baiduads_manual/videoupload/model/add_video_params.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-01-31 03:42:12.000000 baiduads-sdk-2023.0.0/baiduads_manual/videoupload/model/add_video_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-01-31 03:42:12.000000 baiduads-sdk-2023.0.0/baiduads_manual/videoupload/model/add_video_request_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    11101 2023-01-31 03:42:12.000000 baiduads-sdk-2023.0.0/baiduads_manual/videoupload/model/add_video_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11510 2023-01-31 03:42:12.000000 baiduads-sdk-2023.0.0/baiduads_manual/videoupload/model/add_video_response_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    15306 2023-01-31 03:42:12.000000 baiduads-sdk-2023.0.0/baiduads_manual/videoupload/model/video_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 03:42:34.312292 baiduads-sdk-2023.0.0/baiduads_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-01-31 03:42:34.000000 baiduads-sdk-2023.0.0/baiduads_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-01-31 03:42:34.000000 baiduads-sdk-2023.0.0/baiduads_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 03:42:34.000000 baiduads-sdk-2023.0.0/baiduads_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-31 03:42:34.000000 baiduads-sdk-2023.0.0/baiduads_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-01-31 03:42:34.000000 baiduads-sdk-2023.0.0/baiduads_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-01-31 03:42:34.312292 baiduads-sdk-2023.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-01-31 03:42:12.000000 baiduads-sdk-2023.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 03:42:34.304293 baiduads-sdk-2023.0.0/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 03:42:34.312292 baiduads-sdk-2023.0.0/test/account/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 03:42:12.000000 baiduads-sdk-2023.0.0/test/account/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-01-31 03:42:12.000000 baiduads-sdk-2023.0.0/test/account/get_account_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 03:42:34.312292 baiduads-sdk-2023.0.0/test/balance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 03:42:12.000000 baiduads-sdk-2023.0.0/test/balance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-01-31 03:42:12.000000 baiduads-sdk-2023.0.0/test/balance/balance_service_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 03:42:34.312292 baiduads-sdk-2023.0.0/test/marketingfile/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 03:42:12.000000 baiduads-sdk-2023.0.0/test/marketingfile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-01-31 03:42:12.000000 baiduads-sdk-2023.0.0/test/marketingfile/marketing_file_service_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 03:42:34.312292 baiduads-sdk-2023.0.0/test/oauth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 03:42:12.000000 baiduads-sdk-2023.0.0/test/oauth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-01-31 03:42:12.000000 baiduads-sdk-2023.0.0/test/oauth/oauth_service_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 03:42:34.312292 baiduads-sdk-2023.0.0/test/payment/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 03:42:12.000000 baiduads-sdk-2023.0.0/test/payment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-01-31 03:42:12.000000 baiduads-sdk-2023.0.0/test/payment/payment_service_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 03:42:34.312292 baiduads-sdk-2023.0.0/test/upload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 03:42:12.000000 baiduads-sdk-2023.0.0/test/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-01-31 03:42:12.000000 baiduads-sdk-2023.0.0/test/upload/upload_client_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 03:42:34.312292 baiduads-sdk-2023.0.0/test/videoupload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 03:42:12.000000 baiduads-sdk-2023.0.0/test/videoupload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-01-31 03:42:12.000000 baiduads-sdk-2023.0.0/test/videoupload/video_upload_service_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:53:02.331303 baiduads-sdk-2023.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-20 03:53:02.331303 baiduads-sdk-2023.1.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:53:02.323303 baiduads-sdk-2023.1.0/baiduads_manual/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 03:52:37.000000 baiduads-sdk-2023.1.0/baiduads_manual/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:53:02.323303 baiduads-sdk-2023.1.0/baiduads_manual/marketingfile/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 03:52:37.000000 baiduads-sdk-2023.1.0/baiduads_manual/marketingfile/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:53:02.323303 baiduads-sdk-2023.1.0/baiduads_manual/marketingfile/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-20 03:52:37.000000 baiduads-sdk-2023.1.0/baiduads_manual/marketingfile/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-05-20 03:52:37.000000 baiduads-sdk-2023.1.0/baiduads_manual/marketingfile/api/marketing_file_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:53:02.327303 baiduads-sdk-2023.1.0/baiduads_manual/marketingfile/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-20 03:52:37.000000 baiduads-sdk-2023.1.0/baiduads_manual/marketingfile/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10823 2023-05-20 03:52:37.000000 baiduads-sdk-2023.1.0/baiduads_manual/marketingfile/model/upload_file_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-20 03:52:37.000000 baiduads-sdk-2023.1.0/baiduads_manual/marketingfile/model/upload_file_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-20 03:52:37.000000 baiduads-sdk-2023.1.0/baiduads_manual/marketingfile/model/upload_file_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-20 03:52:37.000000 baiduads-sdk-2023.1.0/baiduads_manual/marketingfile/model/upload_file_request_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11078 2023-05-20 03:52:37.000000 baiduads-sdk-2023.1.0/baiduads_manual/marketingfile/model/upload_file_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11465 2023-05-20 03:52:37.000000 baiduads-sdk-2023.1.0/baiduads_manual/marketingfile/model/upload_file_response_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:53:02.327303 baiduads-sdk-2023.1.0/baiduads_manual/oauth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 03:52:37.000000 baiduads-sdk-2023.1.0/baiduads_manual/oauth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:53:02.327303 baiduads-sdk-2023.1.0/baiduads_manual/oauth/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-20 03:52:37.000000 baiduads-sdk-2023.1.0/baiduads_manual/oauth/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7391 2023-05-20 03:52:37.000000 baiduads-sdk-2023.1.0/baiduads_manual/oauth/api/oauth_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:53:02.327303 baiduads-sdk-2023.1.0/baiduads_manual/oauth/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-20 03:52:37.000000 baiduads-sdk-2023.1.0/baiduads_manual/oauth/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-05-20 03:52:37.000000 baiduads-sdk-2023.1.0/baiduads_manual/oauth/model/access_token_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-20 03:52:37.000000 baiduads-sdk-2023.1.0/baiduads_manual/oauth/model/get_access_token_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-20 03:52:37.000000 baiduads-sdk-2023.1.0/baiduads_manual/oauth/model/get_access_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-20 03:52:37.000000 baiduads-sdk-2023.1.0/baiduads_manual/oauth/model/get_open_id_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-20 03:52:37.000000 baiduads-sdk-2023.1.0/baiduads_manual/oauth/model/get_open_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-20 03:52:37.000000 baiduads-sdk-2023.1.0/baiduads_manual/oauth/model/get_user_info_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-20 03:52:37.000000 baiduads-sdk-2023.1.0/baiduads_manual/oauth/model/get_user_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-20 03:52:37.000000 baiduads-sdk-2023.1.0/baiduads_manual/oauth/model/open_id_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-20 03:52:37.000000 baiduads-sdk-2023.1.0/baiduads_manual/oauth/model/refresh_token_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-20 03:52:37.000000 baiduads-sdk-2023.1.0/baiduads_manual/oauth/model/refresh_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-20 03:52:37.000000 baiduads-sdk-2023.1.0/baiduads_manual/oauth/model/sub_user_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-20 03:52:37.000000 baiduads-sdk-2023.1.0/baiduads_manual/oauth/model/user_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:53:02.327303 baiduads-sdk-2023.1.0/baiduads_manual/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 03:52:37.000000 baiduads-sdk-2023.1.0/baiduads_manual/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-20 03:52:37.000000 baiduads-sdk-2023.1.0/baiduads_manual/upload/mulitupload_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14767 2023-05-20 03:52:37.000000 baiduads-sdk-2023.1.0/baiduads_manual/upload/upload_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:53:02.327303 baiduads-sdk-2023.1.0/baiduads_manual/videoupload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 03:52:37.000000 baiduads-sdk-2023.1.0/baiduads_manual/videoupload/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:53:02.327303 baiduads-sdk-2023.1.0/baiduads_manual/videoupload/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-20 03:52:37.000000 baiduads-sdk-2023.1.0/baiduads_manual/videoupload/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-20 03:52:37.000000 baiduads-sdk-2023.1.0/baiduads_manual/videoupload/api/video_upload_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:53:02.327303 baiduads-sdk-2023.1.0/baiduads_manual/videoupload/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-20 03:52:37.000000 baiduads-sdk-2023.1.0/baiduads_manual/videoupload/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-20 03:52:37.000000 baiduads-sdk-2023.1.0/baiduads_manual/videoupload/model/add_video_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-20 03:52:37.000000 baiduads-sdk-2023.1.0/baiduads_manual/videoupload/model/add_video_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-20 03:52:37.000000 baiduads-sdk-2023.1.0/baiduads_manual/videoupload/model/add_video_request_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11101 2023-05-20 03:52:37.000000 baiduads-sdk-2023.1.0/baiduads_manual/videoupload/model/add_video_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11510 2023-05-20 03:52:37.000000 baiduads-sdk-2023.1.0/baiduads_manual/videoupload/model/add_video_response_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15306 2023-05-20 03:52:37.000000 baiduads-sdk-2023.1.0/baiduads_manual/videoupload/model/video_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:53:02.327303 baiduads-sdk-2023.1.0/baiduads_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-20 03:53:02.000000 baiduads-sdk-2023.1.0/baiduads_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-05-20 03:53:02.000000 baiduads-sdk-2023.1.0/baiduads_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 03:53:02.000000 baiduads-sdk-2023.1.0/baiduads_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-20 03:53:02.000000 baiduads-sdk-2023.1.0/baiduads_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-20 03:53:02.000000 baiduads-sdk-2023.1.0/baiduads_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-20 03:53:02.331303 baiduads-sdk-2023.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-20 03:52:37.000000 baiduads-sdk-2023.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:53:02.323303 baiduads-sdk-2023.1.0/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:53:02.331303 baiduads-sdk-2023.1.0/test/account/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 03:52:37.000000 baiduads-sdk-2023.1.0/test/account/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-20 03:52:37.000000 baiduads-sdk-2023.1.0/test/account/get_account_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:53:02.331303 baiduads-sdk-2023.1.0/test/balance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 03:52:37.000000 baiduads-sdk-2023.1.0/test/balance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-20 03:52:37.000000 baiduads-sdk-2023.1.0/test/balance/balance_service_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:53:02.331303 baiduads-sdk-2023.1.0/test/marketingfile/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 03:52:37.000000 baiduads-sdk-2023.1.0/test/marketingfile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-05-20 03:52:37.000000 baiduads-sdk-2023.1.0/test/marketingfile/marketing_file_service_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:53:02.331303 baiduads-sdk-2023.1.0/test/oauth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 03:52:37.000000 baiduads-sdk-2023.1.0/test/oauth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-05-20 03:52:37.000000 baiduads-sdk-2023.1.0/test/oauth/oauth_service_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:53:02.331303 baiduads-sdk-2023.1.0/test/payment/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 03:52:37.000000 baiduads-sdk-2023.1.0/test/payment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-20 03:52:37.000000 baiduads-sdk-2023.1.0/test/payment/payment_service_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:53:02.331303 baiduads-sdk-2023.1.0/test/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 03:52:37.000000 baiduads-sdk-2023.1.0/test/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-20 03:52:37.000000 baiduads-sdk-2023.1.0/test/upload/upload_client_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:53:02.331303 baiduads-sdk-2023.1.0/test/videoupload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 03:52:37.000000 baiduads-sdk-2023.1.0/test/videoupload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-20 03:52:37.000000 baiduads-sdk-2023.1.0/test/videoupload/video_upload_service_test.py
```

### Comparing `baiduads-sdk-2023.0.0/baiduads_manual/marketingfile/api/marketing_file_service.py` & `baiduads-sdk-2023.1.0/baiduads_manual/marketingfile/api/marketing_file_service.py`

 * *Files identical despite different names*

### Comparing `baiduads-sdk-2023.0.0/baiduads_manual/marketingfile/model/__init__.py` & `baiduads-sdk-2023.1.0/baiduads_manual/marketingfile/model/__init__.py`

 * *Files identical despite different names*

### Comparing `baiduads-sdk-2023.0.0/baiduads_manual/marketingfile/model/upload_file_info.py` & `baiduads-sdk-2023.1.0/baiduads_manual/marketingfile/model/upload_file_info.py`

 * *Files identical despite different names*

### Comparing `baiduads-sdk-2023.0.0/baiduads_manual/marketingfile/model/upload_file_params.py` & `baiduads-sdk-2023.1.0/baiduads_manual/marketingfile/model/upload_file_params.py`

 * *Files identical despite different names*

### Comparing `baiduads-sdk-2023.0.0/baiduads_manual/marketingfile/model/upload_file_request.py` & `baiduads-sdk-2023.1.0/baiduads_manual/marketingfile/model/upload_file_request.py`

 * *Files identical despite different names*

### Comparing `baiduads-sdk-2023.0.0/baiduads_manual/marketingfile/model/upload_file_response.py` & `baiduads-sdk-2023.1.0/baiduads_manual/marketingfile/model/upload_file_response.py`

 * *Files identical despite different names*

### Comparing `baiduads-sdk-2023.0.0/baiduads_manual/marketingfile/model/upload_file_response_wrapper.py` & `baiduads-sdk-2023.1.0/baiduads_manual/marketingfile/model/upload_file_response_wrapper.py`

 * *Files identical despite different names*

### Comparing `baiduads-sdk-2023.0.0/baiduads_manual/oauth/api/oauth_service.py` & `baiduads-sdk-2023.1.0/baiduads_manual/oauth/api/oauth_service.py`

 * *Files identical despite different names*

### Comparing `baiduads-sdk-2023.0.0/baiduads_manual/oauth/model/__init__.py` & `baiduads-sdk-2023.1.0/baiduads_manual/oauth/model/__init__.py`

 * *Files identical despite different names*

### Comparing `baiduads-sdk-2023.0.0/baiduads_manual/oauth/model/access_token_info.py` & `baiduads-sdk-2023.1.0/baiduads_manual/oauth/model/access_token_info.py`

 * *Files identical despite different names*

### Comparing `baiduads-sdk-2023.0.0/baiduads_manual/oauth/model/get_access_token_request.py` & `baiduads-sdk-2023.1.0/baiduads_manual/oauth/model/get_access_token_request.py`

 * *Files identical despite different names*

### Comparing `baiduads-sdk-2023.0.0/baiduads_manual/oauth/model/get_access_token_response.py` & `baiduads-sdk-2023.1.0/baiduads_manual/oauth/model/get_access_token_response.py`

 * *Files identical despite different names*

### Comparing `baiduads-sdk-2023.0.0/baiduads_manual/oauth/model/get_open_id_response.py` & `baiduads-sdk-2023.1.0/baiduads_manual/oauth/model/get_open_id_response.py`

 * *Files identical despite different names*

### Comparing `baiduads-sdk-2023.0.0/baiduads_manual/oauth/model/get_user_info_request.py` & `baiduads-sdk-2023.1.0/baiduads_manual/oauth/model/get_user_info_request.py`

 * *Files identical despite different names*

### Comparing `baiduads-sdk-2023.0.0/baiduads_manual/oauth/model/get_user_info_response.py` & `baiduads-sdk-2023.1.0/baiduads_manual/oauth/model/get_user_info_response.py`

 * *Files identical despite different names*

### Comparing `baiduads-sdk-2023.0.0/baiduads_manual/oauth/model/refresh_token_request.py` & `baiduads-sdk-2023.1.0/baiduads_manual/oauth/model/refresh_token_request.py`

 * *Files identical despite different names*

### Comparing `baiduads-sdk-2023.0.0/baiduads_manual/oauth/model/refresh_token_response.py` & `baiduads-sdk-2023.1.0/baiduads_manual/oauth/model/refresh_token_response.py`

 * *Files identical despite different names*

### Comparing `baiduads-sdk-2023.0.0/baiduads_manual/oauth/model/sub_user_info.py` & `baiduads-sdk-2023.1.0/baiduads_manual/oauth/model/sub_user_info.py`

 * *Files identical despite different names*

### Comparing `baiduads-sdk-2023.0.0/baiduads_manual/oauth/model/user_info.py` & `baiduads-sdk-2023.1.0/baiduads_manual/oauth/model/user_info.py`

 * *Files identical despite different names*

### Comparing `baiduads-sdk-2023.0.0/baiduads_manual/upload/mulitupload_options.py` & `baiduads-sdk-2023.1.0/baiduads_manual/upload/mulitupload_options.py`

 * *Files identical despite different names*

### Comparing `baiduads-sdk-2023.0.0/baiduads_manual/upload/upload_client.py` & `baiduads-sdk-2023.1.0/baiduads_manual/upload/upload_client.py`

 * *Files identical despite different names*

### Comparing `baiduads-sdk-2023.0.0/baiduads_manual/videoupload/api/video_upload_service.py` & `baiduads-sdk-2023.1.0/baiduads_manual/videoupload/api/video_upload_service.py`

 * *Files identical despite different names*

### Comparing `baiduads-sdk-2023.0.0/baiduads_manual/videoupload/model/__init__.py` & `baiduads-sdk-2023.1.0/baiduads_manual/videoupload/model/__init__.py`

 * *Files identical despite different names*

### Comparing `baiduads-sdk-2023.0.0/baiduads_manual/videoupload/model/add_video_request.py` & `baiduads-sdk-2023.1.0/baiduads_manual/videoupload/model/add_video_request.py`

 * *Files identical despite different names*

### Comparing `baiduads-sdk-2023.0.0/baiduads_manual/videoupload/model/add_video_response.py` & `baiduads-sdk-2023.1.0/baiduads_manual/videoupload/model/add_video_response.py`

 * *Files identical despite different names*

### Comparing `baiduads-sdk-2023.0.0/baiduads_manual/videoupload/model/add_video_response_wrapper.py` & `baiduads-sdk-2023.1.0/baiduads_manual/videoupload/model/add_video_response_wrapper.py`

 * *Files identical despite different names*

### Comparing `baiduads-sdk-2023.0.0/baiduads_manual/videoupload/model/video_info.py` & `baiduads-sdk-2023.1.0/baiduads_manual/videoupload/model/video_info.py`

 * *Files identical despite different names*

### Comparing `baiduads-sdk-2023.0.0/baiduads_sdk.egg-info/SOURCES.txt` & `baiduads-sdk-2023.1.0/baiduads_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `baiduads-sdk-2023.0.0/setup.py` & `baiduads-sdk-2023.1.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """ baiduads-sdk配置信息
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "baiduads-sdk"
-VERSION = "2023.0.0"
+VERSION = "2023.1.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `baiduads-sdk-2023.0.0/test/account/get_account_info.py` & `baiduads-sdk-2023.1.0/test/account/get_account_info.py`

 * *Files identical despite different names*

### Comparing `baiduads-sdk-2023.0.0/test/balance/balance_service_test.py` & `baiduads-sdk-2023.1.0/test/balance/balance_service_test.py`

 * *Files identical despite different names*

### Comparing `baiduads-sdk-2023.0.0/test/marketingfile/marketing_file_service_test.py` & `baiduads-sdk-2023.1.0/test/marketingfile/marketing_file_service_test.py`

 * *Files identical despite different names*

### Comparing `baiduads-sdk-2023.0.0/test/oauth/oauth_service_test.py` & `baiduads-sdk-2023.1.0/test/oauth/oauth_service_test.py`

 * *Files identical despite different names*

### Comparing `baiduads-sdk-2023.0.0/test/payment/payment_service_test.py` & `baiduads-sdk-2023.1.0/test/payment/payment_service_test.py`

 * *Files identical despite different names*

### Comparing `baiduads-sdk-2023.0.0/test/upload/upload_client_test.py` & `baiduads-sdk-2023.1.0/test/upload/upload_client_test.py`

 * *Files identical despite different names*

### Comparing `baiduads-sdk-2023.0.0/test/videoupload/video_upload_service_test.py` & `baiduads-sdk-2023.1.0/test/videoupload/video_upload_service_test.py`

 * *Files identical despite different names*

