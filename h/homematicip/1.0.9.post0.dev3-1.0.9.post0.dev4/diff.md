# Comparing `tmp/homematicip-1.0.9.post0.dev3.tar.gz` & `tmp/homematicip-1.0.9.post0.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "homematicip-1.0.9.post0.dev3.tar", last modified: Mon Nov 14 06:34:26 2022, max compression
+gzip compressed data, was "homematicip-1.0.9.post0.dev4.tar", last modified: Mon Nov 14 07:06:37 2022, max compression
```

## Comparing `homematicip-1.0.9.post0.dev3.tar` & `homematicip-1.0.9.post0.dev4.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 06:34:26.342294 homematicip-1.0.9.post0.dev3/
--rw-r--r--   0 runner    (1001) docker     (121)    35141 2022-11-14 06:34:11.000000 homematicip-1.0.9.post0.dev3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-11-14 06:34:11.000000 homematicip-1.0.9.post0.dev3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    13717 2022-11-14 06:34:26.342294 homematicip-1.0.9.post0.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13097 2022-11-14 06:34:11.000000 homematicip-1.0.9.post0.dev3/README.md
--rw-r--r--   0 runner    (1001) docker     (121)    28557 2022-11-14 06:34:11.000000 homematicip-1.0.9.post0.dev3/hmip_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     2309 2022-11-14 06:34:11.000000 homematicip-1.0.9.post0.dev3/hmip_generate_auth_token.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 06:34:26.342294 homematicip-1.0.9.post0.dev3/homematicip/
--rw-r--r--   0 runner    (1001) docker     (121)      470 2022-11-14 06:34:11.000000 homematicip-1.0.9.post0.dev3/homematicip/EventHook.py
--rw-r--r--   0 runner    (1001) docker     (121)      297 2022-11-14 06:34:11.000000 homematicip-1.0.9.post0.dev3/homematicip/HomeMaticIPObject.py
--rw-r--r--   0 runner    (1001) docker     (121)     2237 2022-11-14 06:34:11.000000 homematicip-1.0.9.post0.dev3/homematicip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      507 2022-11-14 06:34:26.342294 homematicip-1.0.9.post0.dev3/homematicip/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 06:34:26.338294 homematicip-1.0.9.post0.dev3/homematicip/aio/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-14 06:34:11.000000 homematicip-1.0.9.post0.dev3/homematicip/aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2487 2022-11-14 06:34:11.000000 homematicip-1.0.9.post0.dev3/homematicip/aio/auth.py
--rw-r--r--   0 runner    (1001) docker     (121)     8557 2022-11-14 06:34:11.000000 homematicip-1.0.9.post0.dev3/homematicip/aio/class_maps.py
--rw-r--r--   0 runner    (1001) docker     (121)     7140 2022-11-14 06:34:11.000000 homematicip-1.0.9.post0.dev3/homematicip/aio/connection.py
--rw-r--r--   0 runner    (1001) docker     (121)    20568 2022-11-14 06:34:11.000000 homematicip-1.0.9.post0.dev3/homematicip/aio/device.py
--rw-r--r--   0 runner    (1001) docker     (121)     9396 2022-11-14 06:34:11.000000 homematicip-1.0.9.post0.dev3/homematicip/aio/group.py
--rw-r--r--   0 runner    (1001) docker     (121)     5624 2022-11-14 06:34:11.000000 homematicip-1.0.9.post0.dev3/homematicip/aio/home.py
--rw-r--r--   0 runner    (1001) docker     (121)      840 2022-11-14 06:34:11.000000 homematicip-1.0.9.post0.dev3/homematicip/aio/rule.py
--rw-r--r--   0 runner    (1001) docker     (121)     1474 2022-11-14 06:34:11.000000 homematicip-1.0.9.post0.dev3/homematicip/aio/securityEvent.py
--rw-r--r--   0 runner    (1001) docker     (121)     1899 2022-11-14 06:34:11.000000 homematicip-1.0.9.post0.dev3/homematicip/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 06:34:26.342294 homematicip-1.0.9.post0.dev3/homematicip/base/
--rw-r--r--   0 runner    (1001) docker     (121)     3501 2022-11-14 06:34:11.000000 homematicip-1.0.9.post0.dev3/homematicip/base/HomeMaticIPObject.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-14 06:34:11.000000 homematicip-1.0.9.post0.dev3/homematicip/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2832 2022-11-14 06:34:11.000000 homematicip-1.0.9.post0.dev3/homematicip/base/base_connection.py
--rw-r--r--   0 runner    (1001) docker     (121)     3363 2022-11-14 06:34:11.000000 homematicip-1.0.9.post0.dev3/homematicip/base/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)    16726 2022-11-14 06:34:11.000000 homematicip-1.0.9.post0.dev3/homematicip/base/enums.py
--rw-r--r--   0 runner    (1001) docker     (121)    45031 2022-11-14 06:34:11.000000 homematicip-1.0.9.post0.dev3/homematicip/base/functionalChannels.py
--rw-r--r--   0 runner    (1001) docker     (121)     3448 2022-11-14 06:34:11.000000 homematicip-1.0.9.post0.dev3/homematicip/base/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)    12980 2022-11-14 06:34:11.000000 homematicip-1.0.9.post0.dev3/homematicip/class_maps.py
--rw-r--r--   0 runner    (1001) docker     (121)     2003 2022-11-14 06:34:11.000000 homematicip-1.0.9.post0.dev3/homematicip/connection.py
--rw-r--r--   0 runner    (1001) docker     (121)    84554 2022-11-14 06:34:11.000000 homematicip-1.0.9.post0.dev3/homematicip/device.py
--rw-r--r--   0 runner    (1001) docker     (121)     5710 2022-11-14 06:34:11.000000 homematicip-1.0.9.post0.dev3/homematicip/functionalHomes.py
--rw-r--r--   0 runner    (1001) docker     (121)    44365 2022-11-14 06:34:11.000000 homematicip-1.0.9.post0.dev3/homematicip/group.py
--rw-r--r--   0 runner    (1001) docker     (121)    33503 2022-11-14 06:34:11.000000 homematicip-1.0.9.post0.dev3/homematicip/home.py
--rw-r--r--   0 runner    (1001) docker     (121)     2461 2022-11-14 06:34:11.000000 homematicip-1.0.9.post0.dev3/homematicip/rule.py
--rw-r--r--   0 runner    (1001) docker     (121)     2225 2022-11-14 06:34:11.000000 homematicip-1.0.9.post0.dev3/homematicip/securityEvent.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 06:34:26.338294 homematicip-1.0.9.post0.dev3/homematicip.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    13717 2022-11-14 06:34:26.000000 homematicip-1.0.9.post0.dev3/homematicip.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1297 2022-11-14 06:34:26.000000 homematicip-1.0.9.post0.dev3/homematicip.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-14 06:34:26.000000 homematicip-1.0.9.post0.dev3/homematicip.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-11-14 06:34:26.000000 homematicip-1.0.9.post0.dev3/homematicip.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-11-14 06:34:26.000000 homematicip-1.0.9.post0.dev3/homematicip.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 06:34:26.342294 homematicip-1.0.9.post0.dev3/homematicip_demo/
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-11-14 06:34:11.000000 homematicip-1.0.9.post0.dev3/homematicip_demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    38418 2022-11-14 06:34:11.000000 homematicip-1.0.9.post0.dev3/homematicip_demo/fake_cloud_server.py
--rw-r--r--   0 runner    (1001) docker     (121)      821 2022-11-14 06:34:11.000000 homematicip-1.0.9.post0.dev3/homematicip_demo/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 06:34:26.342294 homematicip-1.0.9.post0.dev3/homematicip_demo/json_data/
--rw-r--r--   0 runner    (1001) docker     (121)   439101 2022-11-14 06:34:11.000000 homematicip-1.0.9.post0.dev3/homematicip_demo/json_data/home.json
--rw-r--r--   0 runner    (1001) docker     (121)     1474 2022-11-14 06:34:11.000000 homematicip-1.0.9.post0.dev3/homematicip_demo/json_data/security_journal.json
--rw-r--r--   0 runner    (1001) docker     (121)     4698 2022-11-14 06:34:11.000000 homematicip-1.0.9.post0.dev3/homematicip_demo/json_data/unknown_types.json
--rw-r--r--   0 runner    (1001) docker     (121)      227 2022-11-14 06:34:26.342294 homematicip-1.0.9.post0.dev3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1485 2022-11-14 06:34:11.000000 homematicip-1.0.9.post0.dev3/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    68752 2022-11-14 06:34:11.000000 homematicip-1.0.9.post0.dev3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 07:06:37.184981 homematicip-1.0.9.post0.dev4/
+-rw-r--r--   0 runner    (1001) docker     (121)    35141 2022-11-14 07:06:23.000000 homematicip-1.0.9.post0.dev4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      126 2022-11-14 07:06:23.000000 homematicip-1.0.9.post0.dev4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    13717 2022-11-14 07:06:37.184981 homematicip-1.0.9.post0.dev4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    13097 2022-11-14 07:06:23.000000 homematicip-1.0.9.post0.dev4/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)    28800 2022-11-14 07:06:23.000000 homematicip-1.0.9.post0.dev4/hmip_cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2309 2022-11-14 07:06:23.000000 homematicip-1.0.9.post0.dev4/hmip_generate_auth_token.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 07:06:37.184981 homematicip-1.0.9.post0.dev4/homematicip/
+-rw-r--r--   0 runner    (1001) docker     (121)      470 2022-11-14 07:06:23.000000 homematicip-1.0.9.post0.dev4/homematicip/EventHook.py
+-rw-r--r--   0 runner    (1001) docker     (121)      297 2022-11-14 07:06:23.000000 homematicip-1.0.9.post0.dev4/homematicip/HomeMaticIPObject.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2237 2022-11-14 07:06:23.000000 homematicip-1.0.9.post0.dev4/homematicip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      507 2022-11-14 07:06:37.188981 homematicip-1.0.9.post0.dev4/homematicip/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 07:06:37.184981 homematicip-1.0.9.post0.dev4/homematicip/aio/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-14 07:06:23.000000 homematicip-1.0.9.post0.dev4/homematicip/aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2487 2022-11-14 07:06:23.000000 homematicip-1.0.9.post0.dev4/homematicip/aio/auth.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8557 2022-11-14 07:06:23.000000 homematicip-1.0.9.post0.dev4/homematicip/aio/class_maps.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7140 2022-11-14 07:06:23.000000 homematicip-1.0.9.post0.dev4/homematicip/aio/connection.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20568 2022-11-14 07:06:23.000000 homematicip-1.0.9.post0.dev4/homematicip/aio/device.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9396 2022-11-14 07:06:23.000000 homematicip-1.0.9.post0.dev4/homematicip/aio/group.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5624 2022-11-14 07:06:23.000000 homematicip-1.0.9.post0.dev4/homematicip/aio/home.py
+-rw-r--r--   0 runner    (1001) docker     (121)      840 2022-11-14 07:06:23.000000 homematicip-1.0.9.post0.dev4/homematicip/aio/rule.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1474 2022-11-14 07:06:23.000000 homematicip-1.0.9.post0.dev4/homematicip/aio/securityEvent.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1899 2022-11-14 07:06:23.000000 homematicip-1.0.9.post0.dev4/homematicip/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 07:06:37.184981 homematicip-1.0.9.post0.dev4/homematicip/base/
+-rw-r--r--   0 runner    (1001) docker     (121)     3501 2022-11-14 07:06:23.000000 homematicip-1.0.9.post0.dev4/homematicip/base/HomeMaticIPObject.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-14 07:06:23.000000 homematicip-1.0.9.post0.dev4/homematicip/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2832 2022-11-14 07:06:23.000000 homematicip-1.0.9.post0.dev4/homematicip/base/base_connection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3363 2022-11-14 07:06:23.000000 homematicip-1.0.9.post0.dev4/homematicip/base/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16726 2022-11-14 07:06:23.000000 homematicip-1.0.9.post0.dev4/homematicip/base/enums.py
+-rw-r--r--   0 runner    (1001) docker     (121)    45031 2022-11-14 07:06:23.000000 homematicip-1.0.9.post0.dev4/homematicip/base/functionalChannels.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3448 2022-11-14 07:06:23.000000 homematicip-1.0.9.post0.dev4/homematicip/base/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12980 2022-11-14 07:06:23.000000 homematicip-1.0.9.post0.dev4/homematicip/class_maps.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2003 2022-11-14 07:06:23.000000 homematicip-1.0.9.post0.dev4/homematicip/connection.py
+-rw-r--r--   0 runner    (1001) docker     (121)    84554 2022-11-14 07:06:23.000000 homematicip-1.0.9.post0.dev4/homematicip/device.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5710 2022-11-14 07:06:23.000000 homematicip-1.0.9.post0.dev4/homematicip/functionalHomes.py
+-rw-r--r--   0 runner    (1001) docker     (121)    44365 2022-11-14 07:06:23.000000 homematicip-1.0.9.post0.dev4/homematicip/group.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33503 2022-11-14 07:06:23.000000 homematicip-1.0.9.post0.dev4/homematicip/home.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2461 2022-11-14 07:06:23.000000 homematicip-1.0.9.post0.dev4/homematicip/rule.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2225 2022-11-14 07:06:23.000000 homematicip-1.0.9.post0.dev4/homematicip/securityEvent.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 07:06:37.184981 homematicip-1.0.9.post0.dev4/homematicip.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    13717 2022-11-14 07:06:37.000000 homematicip-1.0.9.post0.dev4/homematicip.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1297 2022-11-14 07:06:37.000000 homematicip-1.0.9.post0.dev4/homematicip.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-14 07:06:37.000000 homematicip-1.0.9.post0.dev4/homematicip.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      106 2022-11-14 07:06:37.000000 homematicip-1.0.9.post0.dev4/homematicip.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2022-11-14 07:06:37.000000 homematicip-1.0.9.post0.dev4/homematicip.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 07:06:37.184981 homematicip-1.0.9.post0.dev4/homematicip_demo/
+-rw-r--r--   0 runner    (1001) docker     (121)       36 2022-11-14 07:06:23.000000 homematicip-1.0.9.post0.dev4/homematicip_demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    38418 2022-11-14 07:06:23.000000 homematicip-1.0.9.post0.dev4/homematicip_demo/fake_cloud_server.py
+-rw-r--r--   0 runner    (1001) docker     (121)      821 2022-11-14 07:06:23.000000 homematicip-1.0.9.post0.dev4/homematicip_demo/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 07:06:37.184981 homematicip-1.0.9.post0.dev4/homematicip_demo/json_data/
+-rw-r--r--   0 runner    (1001) docker     (121)   439101 2022-11-14 07:06:23.000000 homematicip-1.0.9.post0.dev4/homematicip_demo/json_data/home.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1474 2022-11-14 07:06:23.000000 homematicip-1.0.9.post0.dev4/homematicip_demo/json_data/security_journal.json
+-rw-r--r--   0 runner    (1001) docker     (121)     4698 2022-11-14 07:06:23.000000 homematicip-1.0.9.post0.dev4/homematicip_demo/json_data/unknown_types.json
+-rw-r--r--   0 runner    (1001) docker     (121)      227 2022-11-14 07:06:37.184981 homematicip-1.0.9.post0.dev4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1485 2022-11-14 07:06:23.000000 homematicip-1.0.9.post0.dev4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)    68752 2022-11-14 07:06:23.000000 homematicip-1.0.9.post0.dev4/versioneer.py
```

### Comparing `homematicip-1.0.9.post0.dev3/LICENSE.txt` & `homematicip-1.0.9.post0.dev4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `homematicip-1.0.9.post0.dev3/PKG-INFO` & `homematicip-1.0.9.post0.dev4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: homematicip
-Version: 1.0.9.post0.dev3
+Version: 1.0.9.post0.dev4
 Summary: An API for the homematicip cloud
 Home-page: https://github.com/hahn-th/homematicip-rest-api
-Download-URL: https://github.com/hahn-th/homematicip-rest-api/tarball/1.0.9.post.dev3
+Download-URL: https://github.com/hahn-th/homematicip-rest-api/tarball/1.0.9.post.dev4
 Author: Thomas Hahn
 Author-email: post@thomas-hahn.org
 Keywords: homematicip
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `homematicip-1.0.9.post0.dev3/README.md` & `homematicip-1.0.9.post0.dev4/README.md`

 * *Files identical despite different names*

### Comparing `homematicip-1.0.9.post0.dev3/hmip_cli.py` & `homematicip-1.0.9.post0.dev4/hmip_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -578,29 +578,32 @@
             if args.device_switch_state is not None:
                 if (
                     isinstance(device, Switch)
                     or isinstance(device, Dimmer)
                     or isinstance(device, WallMountedUniversalActuator)
                 ):
                     for c in args.channels:
-                        device.set_switch_state(args.device_switch_state, c)
+                        res = device.set_switch_state(args.device_switch_state, c)
+                        print("Result from channel {0}: {1}".format(c, json.dumps(res)))
                 else:
                     logger.error(
                         "can't turn on/off device %s of type %s",
                         device.id,
                         device.deviceType,
                     )
                 command_entered = True
 
             if args.device_dim_level is not None:
                 if isinstance(device, Dimmer) or isinstance(
                     device, WallMountedUniversalActuator
-                ):
+                ) or isinstance(device, TemperatureDifferenceSensor2):
+
                     for c in args.channels:
-                        device.set_dim_level(args.device_dim_level, c)
+                        res = device.set_dim_level(args.device_dim_level, c)
+                        print("Result from channel {0}: {1}".format(c, json.dumps(res)))
                 else:
                     logger.error(
                         "can't set dim level of device %s of type %s",
                         device.id,
                         device.deviceType,
                     )
                 command_entered = True
```

### Comparing `homematicip-1.0.9.post0.dev3/hmip_generate_auth_token.py` & `homematicip-1.0.9.post0.dev4/hmip_generate_auth_token.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.0.9.post0.dev3/homematicip/__init__.py` & `homematicip-1.0.9.post0.dev4/homematicip/__init__.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.0.9.post0.dev3/homematicip/aio/auth.py` & `homematicip-1.0.9.post0.dev4/homematicip/aio/auth.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.0.9.post0.dev3/homematicip/aio/class_maps.py` & `homematicip-1.0.9.post0.dev4/homematicip/aio/class_maps.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.0.9.post0.dev3/homematicip/aio/connection.py` & `homematicip-1.0.9.post0.dev4/homematicip/aio/connection.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.0.9.post0.dev3/homematicip/aio/device.py` & `homematicip-1.0.9.post0.dev4/homematicip/aio/device.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.0.9.post0.dev3/homematicip/aio/group.py` & `homematicip-1.0.9.post0.dev4/homematicip/aio/group.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.0.9.post0.dev3/homematicip/aio/home.py` & `homematicip-1.0.9.post0.dev4/homematicip/aio/home.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.0.9.post0.dev3/homematicip/aio/rule.py` & `homematicip-1.0.9.post0.dev4/homematicip/aio/rule.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.0.9.post0.dev3/homematicip/aio/securityEvent.py` & `homematicip-1.0.9.post0.dev4/homematicip/aio/securityEvent.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.0.9.post0.dev3/homematicip/auth.py` & `homematicip-1.0.9.post0.dev4/homematicip/auth.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.0.9.post0.dev3/homematicip/base/HomeMaticIPObject.py` & `homematicip-1.0.9.post0.dev4/homematicip/base/HomeMaticIPObject.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.0.9.post0.dev3/homematicip/base/base_connection.py` & `homematicip-1.0.9.post0.dev4/homematicip/base/base_connection.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.0.9.post0.dev3/homematicip/base/constants.py` & `homematicip-1.0.9.post0.dev4/homematicip/base/constants.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.0.9.post0.dev3/homematicip/base/enums.py` & `homematicip-1.0.9.post0.dev4/homematicip/base/enums.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.0.9.post0.dev3/homematicip/base/functionalChannels.py` & `homematicip-1.0.9.post0.dev4/homematicip/base/functionalChannels.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.0.9.post0.dev3/homematicip/base/helpers.py` & `homematicip-1.0.9.post0.dev4/homematicip/base/helpers.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.0.9.post0.dev3/homematicip/class_maps.py` & `homematicip-1.0.9.post0.dev4/homematicip/class_maps.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.0.9.post0.dev3/homematicip/connection.py` & `homematicip-1.0.9.post0.dev4/homematicip/connection.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.0.9.post0.dev3/homematicip/device.py` & `homematicip-1.0.9.post0.dev4/homematicip/device.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.0.9.post0.dev3/homematicip/functionalHomes.py` & `homematicip-1.0.9.post0.dev4/homematicip/functionalHomes.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.0.9.post0.dev3/homematicip/group.py` & `homematicip-1.0.9.post0.dev4/homematicip/group.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.0.9.post0.dev3/homematicip/home.py` & `homematicip-1.0.9.post0.dev4/homematicip/home.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.0.9.post0.dev3/homematicip/rule.py` & `homematicip-1.0.9.post0.dev4/homematicip/rule.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.0.9.post0.dev3/homematicip/securityEvent.py` & `homematicip-1.0.9.post0.dev4/homematicip/securityEvent.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.0.9.post0.dev3/homematicip.egg-info/PKG-INFO` & `homematicip-1.0.9.post0.dev4/homematicip.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: homematicip
-Version: 1.0.9.post0.dev3
+Version: 1.0.9.post0.dev4
 Summary: An API for the homematicip cloud
 Home-page: https://github.com/hahn-th/homematicip-rest-api
-Download-URL: https://github.com/hahn-th/homematicip-rest-api/tarball/1.0.9.post.dev3
+Download-URL: https://github.com/hahn-th/homematicip-rest-api/tarball/1.0.9.post.dev4
 Author: Thomas Hahn
 Author-email: post@thomas-hahn.org
 Keywords: homematicip
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `homematicip-1.0.9.post0.dev3/homematicip.egg-info/SOURCES.txt` & `homematicip-1.0.9.post0.dev4/homematicip.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `homematicip-1.0.9.post0.dev3/homematicip_demo/fake_cloud_server.py` & `homematicip-1.0.9.post0.dev4/homematicip_demo/fake_cloud_server.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.0.9.post0.dev3/homematicip_demo/helper.py` & `homematicip-1.0.9.post0.dev4/homematicip_demo/helper.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.0.9.post0.dev3/homematicip_demo/json_data/home.json` & `homematicip-1.0.9.post0.dev4/homematicip_demo/json_data/home.json`

 * *Files identical despite different names*

### Comparing `homematicip-1.0.9.post0.dev3/homematicip_demo/json_data/security_journal.json` & `homematicip-1.0.9.post0.dev4/homematicip_demo/json_data/security_journal.json`

 * *Files identical despite different names*

### Comparing `homematicip-1.0.9.post0.dev3/homematicip_demo/json_data/unknown_types.json` & `homematicip-1.0.9.post0.dev4/homematicip_demo/json_data/unknown_types.json`

 * *Files identical despite different names*

### Comparing `homematicip-1.0.9.post0.dev3/setup.py` & `homematicip-1.0.9.post0.dev4/setup.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.0.9.post0.dev3/versioneer.py` & `homematicip-1.0.9.post0.dev4/versioneer.py`

 * *Files identical despite different names*

