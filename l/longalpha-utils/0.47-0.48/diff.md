# Comparing `tmp/longalpha_utils-0.47.tar.gz` & `tmp/longalpha_utils-0.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "longalpha_utils-0.47.tar", last modified: Sat May 13 17:37:32 2023, max compression
+gzip compressed data, was "longalpha_utils-0.48.tar", last modified: Sat May 20 19:58:30 2023, max compression
```

## Comparing `longalpha_utils-0.47.tar` & `longalpha_utils-0.48.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 17:37:32.495860 longalpha_utils-0.47/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-13 17:37:32.495860 longalpha_utils-0.47/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 17:37:32.491860 longalpha_utils-0.47/longalpha_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-13 17:37:19.000000 longalpha_utils-0.47/longalpha_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-13 17:37:19.000000 longalpha_utils-0.47/longalpha_utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-13 17:37:19.000000 longalpha_utils-0.47/longalpha_utils/messenger.py
--rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-05-13 17:37:19.000000 longalpha_utils-0.47/longalpha_utils/transfers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-05-13 17:37:19.000000 longalpha_utils-0.47/longalpha_utils/us_stock_holidays.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-13 17:37:19.000000 longalpha_utils-0.47/longalpha_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 17:37:32.495860 longalpha_utils-0.47/longalpha_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-13 17:37:32.000000 longalpha_utils-0.47/longalpha_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-13 17:37:32.000000 longalpha_utils-0.47/longalpha_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 17:37:32.000000 longalpha_utils-0.47/longalpha_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-13 17:37:32.000000 longalpha_utils-0.47/longalpha_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-13 17:37:32.000000 longalpha_utils-0.47/longalpha_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 17:37:32.495860 longalpha_utils-0.47/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-13 17:37:19.000000 longalpha_utils-0.47/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:58:30.236262 longalpha_utils-0.48/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-20 19:58:30.236262 longalpha_utils-0.48/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:58:30.236262 longalpha_utils-0.48/longalpha_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-20 19:58:16.000000 longalpha_utils-0.48/longalpha_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-20 19:58:16.000000 longalpha_utils-0.48/longalpha_utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-20 19:58:16.000000 longalpha_utils-0.48/longalpha_utils/messenger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10634 2023-05-20 19:58:16.000000 longalpha_utils-0.48/longalpha_utils/transfers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-05-20 19:58:16.000000 longalpha_utils-0.48/longalpha_utils/us_stock_holidays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-20 19:58:16.000000 longalpha_utils-0.48/longalpha_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:58:30.236262 longalpha_utils-0.48/longalpha_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-20 19:58:30.000000 longalpha_utils-0.48/longalpha_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-20 19:58:30.000000 longalpha_utils-0.48/longalpha_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 19:58:30.000000 longalpha_utils-0.48/longalpha_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-20 19:58:30.000000 longalpha_utils-0.48/longalpha_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-20 19:58:30.000000 longalpha_utils-0.48/longalpha_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 19:58:30.236262 longalpha_utils-0.48/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-20 19:58:16.000000 longalpha_utils-0.48/setup.py
```

### Comparing `longalpha_utils-0.47/longalpha_utils/messenger.py` & `longalpha_utils-0.48/longalpha_utils/messenger.py`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.47/longalpha_utils/transfers.py` & `longalpha_utils-0.48/longalpha_utils/transfers.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,22 +178,21 @@
 
 
 
 def get_s3_data_spark(
         spark: SparkSession, start_date: date, end_date: date, bucket: str, subfolder: str,
 ) -> Union[DataFrame, None]:
     """
-    Get options data from minio
+    Get data from s3 for a given date range
     Args:
         spark: spark session
         start_date: start date to get options data for
         end_date: end date to get options data for
 
-    Returns: options data if exists, None otherwise.
-    Note returned options data is in wide format with calls and puts on the same row
+    Returns: a spark dataframe if data exists, None otherwise
 
     """
     options = []
     while start_date <= end_date:
         file_s3_path = "s3a://" +os.path.join(bucket, f"{subfolder}/{start_date}.parquet")
         try:
             option = spark.read.parquet(file_s3_path)
```

### Comparing `longalpha_utils-0.47/longalpha_utils/us_stock_holidays.py` & `longalpha_utils-0.48/longalpha_utils/us_stock_holidays.py`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.47/longalpha_utils/utils.py` & `longalpha_utils-0.48/longalpha_utils/utils.py`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.47/longalpha_utils.egg-info/requires.txt` & `longalpha_utils-0.48/longalpha_utils.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.47/setup.py` & `longalpha_utils-0.48/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,11 +38,11 @@
     "typing_extensions==4.4.0",
     "urllib3==1.26.14",
     "yagmail==0.15.293",
 ]
 
 setup(
     name="longalpha_utils",
-    version="0.47",
+    version="0.48",
     long_description="Shared utilities for long alpha projects",
     install_requires=REQUIREMENTS,
 )
```

