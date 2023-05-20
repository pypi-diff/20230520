# Comparing `tmp/claudia-0.0.6.tar.gz` & `tmp/claudia-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "claudia-0.0.6.tar", last modified: Fri May 19 02:25:04 2023, max compression
+gzip compressed data, was "claudia-0.0.7.tar", last modified: Sat May 20 01:18:38 2023, max compression
```

## Comparing `claudia-0.0.6.tar` & `claudia-0.0.7.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-19 02:25:04.220667 claudia-0.0.6/
--rw-r--r--   0 ksaxena    (502) staff       (20)     1073 2023-05-11 10:47:00.000000 claudia-0.0.6/LICENSE
--rw-r--r--   0 ksaxena    (502) staff       (20)     1918 2023-05-19 02:25:04.220495 claudia-0.0.6/PKG-INFO
--rw-r--r--   0 ksaxena    (502) staff       (20)     3140 2023-05-18 03:10:36.000000 claudia-0.0.6/README.md
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-19 02:25:04.202772 claudia-0.0.6/claudia.egg-info/
--rw-r--r--   0 ksaxena    (502) staff       (20)     1918 2023-05-19 02:25:04.000000 claudia-0.0.6/claudia.egg-info/PKG-INFO
--rw-r--r--   0 ksaxena    (502) staff       (20)     2610 2023-05-19 02:25:04.000000 claudia-0.0.6/claudia.egg-info/SOURCES.txt
--rw-r--r--   0 ksaxena    (502) staff       (20)        1 2023-05-19 02:25:04.000000 claudia-0.0.6/claudia.egg-info/dependency_links.txt
--rw-r--r--   0 ksaxena    (502) staff       (20)       49 2023-05-19 02:25:04.000000 claudia-0.0.6/claudia.egg-info/entry_points.txt
--rw-r--r--   0 ksaxena    (502) staff       (20)       79 2023-05-19 02:25:04.000000 claudia-0.0.6/claudia.egg-info/requires.txt
--rw-r--r--   0 ksaxena    (502) staff       (20)        8 2023-05-19 02:25:04.000000 claudia-0.0.6/claudia.egg-info/top_level.txt
--rw-r--r--   0 ksaxena    (502) staff       (20)       38 2023-05-19 02:25:04.220719 claudia-0.0.6/setup.cfg
--rw-r--r--   0 ksaxena    (502) staff       (20)     1477 2023-05-19 02:23:54.000000 claudia-0.0.6/setup.py
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-19 02:25:04.195561 claudia-0.0.6/src/
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-19 02:25:04.204067 claudia-0.0.6/src/claudia/
--rw-r--r--   0 ksaxena    (502) staff       (20)     1569 2023-05-18 03:11:01.000000 claudia-0.0.6/src/claudia/README.md
--rw-r--r--   0 ksaxena    (502) staff       (20)        0 2023-05-15 18:14:02.000000 claudia-0.0.6/src/claudia/__init__.py
--rw-r--r--   0 ksaxena    (502) staff       (20)    10793 2023-05-19 02:19:34.000000 claudia-0.0.6/src/claudia/claudia.py
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-19 02:25:04.204915 claudia-0.0.6/src/claudia/features/
--rw-r--r--   0 ksaxena    (502) staff       (20)    14321 2023-05-15 18:14:02.000000 claudia-0.0.6/src/claudia/features/nft_burn_mint.feature
--rw-r--r--   0 ksaxena    (502) staff       (20)     5371 2023-05-15 18:14:02.000000 claudia-0.0.6/src/claudia/features/payments.feature
--rw-r--r--   0 ksaxena    (502) staff       (20)    11071 2023-05-15 18:14:02.000000 claudia-0.0.6/src/claudia/features/trustline.feature
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-19 02:25:04.206683 claudia-0.0.6/src/claudia/javascript/
--rwxr-xr-x   0 ksaxena    (502) staff       (20)      118 2023-05-15 18:14:02.000000 claudia-0.0.6/src/claudia/javascript/cleanup
--rw-r--r--   0 ksaxena    (502) staff       (20)      145 2023-05-15 18:14:02.000000 claudia-0.0.6/src/claudia/javascript/cucumber.js
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-19 02:25:04.206901 claudia-0.0.6/src/claudia/javascript/features/
--rw-r--r--   0 ksaxena    (502) staff       (20)     1226 2023-05-15 18:14:02.000000 claudia-0.0.6/src/claudia/javascript/features/context.js
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-19 02:25:04.207270 claudia-0.0.6/src/claudia/javascript/features/lib/
--rw-r--r--   0 ksaxena    (502) staff       (20)     2106 2023-05-15 18:14:02.000000 claudia-0.0.6/src/claudia/javascript/features/lib/ObjFactory.js
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-19 02:25:04.208812 claudia-0.0.6/src/claudia/javascript/features/steps/
--rw-r--r--   0 ksaxena    (502) staff       (20)    38728 2023-05-15 18:14:02.000000 claudia-0.0.6/src/claudia/javascript/features/steps/common.js
--rw-r--r--   0 ksaxena    (502) staff       (20)      300 2023-05-15 18:14:02.000000 claudia-0.0.6/src/claudia/javascript/features/steps/constants.js
--rw-r--r--   0 ksaxena    (502) staff       (20)    71153 2023-05-15 18:14:02.000000 claudia-0.0.6/src/claudia/javascript/features/steps/nft_mint_burn.js
--rw-r--r--   0 ksaxena    (502) staff       (20)    19024 2023-05-15 18:14:02.000000 claudia-0.0.6/src/claudia/javascript/features/steps/payments.js
--rw-r--r--   0 ksaxena    (502) staff       (20)    59478 2023-05-15 18:14:02.000000 claudia-0.0.6/src/claudia/javascript/features/steps/trustline.js
--rw-r--r--   0 ksaxena    (502) staff       (20)   129466 2023-05-15 18:14:02.000000 claudia-0.0.6/src/claudia/javascript/package-lock.json
--rw-r--r--   0 ksaxena    (502) staff       (20)      221 2023-05-15 18:14:02.000000 claudia-0.0.6/src/claudia/javascript/package.json
--rwxr-xr-x   0 ksaxena    (502) staff       (20)      869 2023-05-15 18:14:02.000000 claudia-0.0.6/src/claudia/javascript/runSetup
--rwxr-xr-x   0 ksaxena    (502) staff       (20)     4674 2023-05-15 18:14:02.000000 claudia-0.0.6/src/claudia/javascript/runTest
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-19 02:25:04.209584 claudia-0.0.6/src/claudia/network_setup/
--rw-rw-r--   0 ksaxena    (502) staff       (20)      251 2023-05-18 02:32:34.000000 claudia-0.0.6/src/claudia/network_setup/Dockerfile
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-19 02:25:04.210251 claudia-0.0.6/src/claudia/network_setup/configs/
--rw-rw-r--   0 ksaxena    (502) staff       (20)     1520 2023-05-18 02:32:34.000000 claudia-0.0.6/src/claudia/network_setup/configs/rippled.cfg
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-19 02:25:04.210884 claudia-0.0.6/src/claudia/network_setup/configs/rippled_1/
--rw-rw-r--   0 ksaxena    (502) staff       (20)     2150 2023-05-18 02:32:34.000000 claudia-0.0.6/src/claudia/network_setup/configs/rippled_1/rippled.cfg
--rw-rw-r--   0 ksaxena    (502) staff       (20)      278 2023-05-18 02:32:34.000000 claudia-0.0.6/src/claudia/network_setup/configs/rippled_1/validators.txt
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-19 02:25:04.211592 claudia-0.0.6/src/claudia/network_setup/configs/rippled_2/
--rw-rw-r--   0 ksaxena    (502) staff       (20)     2191 2023-05-18 02:32:34.000000 claudia-0.0.6/src/claudia/network_setup/configs/rippled_2/rippled.cfg
--rw-rw-r--   0 ksaxena    (502) staff       (20)      278 2023-05-18 02:32:34.000000 claudia-0.0.6/src/claudia/network_setup/configs/rippled_2/validators.txt
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-19 02:25:04.212345 claudia-0.0.6/src/claudia/network_setup/configs/rippled_3/
--rw-rw-r--   0 ksaxena    (502) staff       (20)     2191 2023-05-18 02:32:34.000000 claudia-0.0.6/src/claudia/network_setup/configs/rippled_3/rippled.cfg
--rw-rw-r--   0 ksaxena    (502) staff       (20)      278 2023-05-18 02:32:34.000000 claudia-0.0.6/src/claudia/network_setup/configs/rippled_3/validators.txt
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-19 02:25:04.212911 claudia-0.0.6/src/claudia/network_setup/configs/rippled_4/
--rw-rw-r--   0 ksaxena    (502) staff       (20)     2190 2023-05-18 02:32:34.000000 claudia-0.0.6/src/claudia/network_setup/configs/rippled_4/rippled.cfg
--rw-rw-r--   0 ksaxena    (502) staff       (20)      278 2023-05-18 02:32:34.000000 claudia-0.0.6/src/claudia/network_setup/configs/rippled_4/validators.txt
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-19 02:25:04.213475 claudia-0.0.6/src/claudia/network_setup/configs/rippled_5/
--rw-rw-r--   0 ksaxena    (502) staff       (20)     2226 2023-05-18 02:32:34.000000 claudia-0.0.6/src/claudia/network_setup/configs/rippled_5/rippled.cfg
--rw-rw-r--   0 ksaxena    (502) staff       (20)      278 2023-05-18 02:32:34.000000 claudia-0.0.6/src/claudia/network_setup/configs/rippled_5/validators.txt
--rw-rw-r--   0 ksaxena    (502) staff       (20)      279 2023-05-18 02:32:34.000000 claudia-0.0.6/src/claudia/network_setup/configs/validators.txt
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-19 02:25:04.214829 claudia-0.0.6/src/claudia/network_setup/lib/
--rw-rw-r--   0 ksaxena    (502) staff       (20)     1619 2023-05-18 02:32:34.000000 claudia-0.0.6/src/claudia/network_setup/lib/build_rippled.sh
--rw-rw-r--   0 ksaxena    (502) staff       (20)     2161 2023-05-18 02:32:34.000000 claudia-0.0.6/src/claudia/network_setup/lib/rippled_network.yml
--rw-rw-r--   0 ksaxena    (502) staff       (20)     8966 2023-05-18 02:32:34.000000 claudia-0.0.6/src/claudia/network_setup/lib/setup_helper.sh
--rw-rw-r--   0 ksaxena    (502) staff       (20)     5094 2023-05-18 02:32:34.000000 claudia-0.0.6/src/claudia/network_setup/lib/validate_network.py
--rw-rw-r--   0 ksaxena    (502) staff       (20)     3784 2023-05-18 02:32:34.000000 claudia-0.0.6/src/claudia/network_setup/setup.sh
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-19 02:25:04.216327 claudia-0.0.6/src/claudia/python/
--rw-r--r--   0 ksaxena    (502) staff       (20)        0 2023-05-15 18:14:02.000000 claudia-0.0.6/src/claudia/python/__init__.py
--rw-r--r--   0 ksaxena    (502) staff       (20)      107 2023-05-15 18:14:02.000000 claudia-0.0.6/src/claudia/python/behave.ini
--rwxr-xr-x   0 ksaxena    (502) staff       (20)      123 2023-05-15 18:14:02.000000 claudia-0.0.6/src/claudia/python/cleanup
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-19 02:25:04.216960 claudia-0.0.6/src/claudia/python/features/
--rw-r--r--   0 ksaxena    (502) staff       (20)        0 2023-05-15 18:14:02.000000 claudia-0.0.6/src/claudia/python/features/__init__.py
--rw-r--r--   0 ksaxena    (502) staff       (20)     2977 2023-05-15 18:14:02.000000 claudia-0.0.6/src/claudia/python/features/environment.py
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-19 02:25:04.217616 claudia-0.0.6/src/claudia/python/features/exceptions/
--rw-r--r--   0 ksaxena    (502) staff       (20)       49 2023-05-15 18:14:02.000000 claudia-0.0.6/src/claudia/python/features/exceptions/InvalidInputException.py
--rw-r--r--   0 ksaxena    (502) staff       (20)       60 2023-05-15 18:14:02.000000 claudia-0.0.6/src/claudia/python/features/exceptions/UnconfiguredEnvironmentException.py
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-19 02:25:04.218298 claudia-0.0.6/src/claudia/python/features/lib/
--rw-r--r--   0 ksaxena    (502) staff       (20)      301 2023-05-15 18:14:02.000000 claudia-0.0.6/src/claudia/python/features/lib/Helpers.py
--rw-r--r--   0 ksaxena    (502) staff       (20)     7674 2023-05-15 18:14:02.000000 claudia-0.0.6/src/claudia/python/features/lib/ObjFactory.py
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-19 02:25:04.220099 claudia-0.0.6/src/claudia/python/features/steps/
--rw-r--r--   0 ksaxena    (502) staff       (20)    24750 2023-05-15 18:14:02.000000 claudia-0.0.6/src/claudia/python/features/steps/common.py
--rw-r--r--   0 ksaxena    (502) staff       (20)      251 2023-05-15 18:14:02.000000 claudia-0.0.6/src/claudia/python/features/steps/constants.py
--rw-r--r--   0 ksaxena    (502) staff       (20)    66340 2023-05-15 18:14:02.000000 claudia-0.0.6/src/claudia/python/features/steps/nft_mint_burn.py
--rw-r--r--   0 ksaxena    (502) staff       (20)    21822 2023-05-15 18:14:02.000000 claudia-0.0.6/src/claudia/python/features/steps/payments.py
--rw-r--r--   0 ksaxena    (502) staff       (20)    54620 2023-05-15 18:14:02.000000 claudia-0.0.6/src/claudia/python/features/steps/trustline.py
--rwxr-xr-x   0 ksaxena    (502) staff       (20)     1381 2023-05-15 18:14:02.000000 claudia-0.0.6/src/claudia/python/runSetup
--rwxr-xr-x   0 ksaxena    (502) staff       (20)     5634 2023-05-15 18:14:02.000000 claudia-0.0.6/src/claudia/python/runTest
--rw-r--r--   0 ksaxena    (502) staff       (20)       79 2023-05-16 18:21:22.000000 claudia-0.0.6/src/claudia/requirements.txt
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-20 01:18:38.610778 claudia-0.0.7/
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1073 2023-05-11 10:47:00.000000 claudia-0.0.7/LICENSE
+-rw-r--r--   0 ksaxena    (502) staff       (20)     3533 2023-05-20 01:18:38.610561 claudia-0.0.7/PKG-INFO
+-rw-r--r--   0 ksaxena    (502) staff       (20)     4935 2023-05-20 01:17:00.000000 claudia-0.0.7/README.md
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-20 01:18:38.584480 claudia-0.0.7/claudia.egg-info/
+-rw-r--r--   0 ksaxena    (502) staff       (20)     3533 2023-05-20 01:18:38.000000 claudia-0.0.7/claudia.egg-info/PKG-INFO
+-rw-r--r--   0 ksaxena    (502) staff       (20)     2610 2023-05-20 01:18:38.000000 claudia-0.0.7/claudia.egg-info/SOURCES.txt
+-rw-r--r--   0 ksaxena    (502) staff       (20)        1 2023-05-20 01:18:38.000000 claudia-0.0.7/claudia.egg-info/dependency_links.txt
+-rw-r--r--   0 ksaxena    (502) staff       (20)       49 2023-05-20 01:18:38.000000 claudia-0.0.7/claudia.egg-info/entry_points.txt
+-rw-r--r--   0 ksaxena    (502) staff       (20)       88 2023-05-20 01:18:38.000000 claudia-0.0.7/claudia.egg-info/requires.txt
+-rw-r--r--   0 ksaxena    (502) staff       (20)        8 2023-05-20 01:18:38.000000 claudia-0.0.7/claudia.egg-info/top_level.txt
+-rw-r--r--   0 ksaxena    (502) staff       (20)       38 2023-05-20 01:18:38.610831 claudia-0.0.7/setup.cfg
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1477 2023-05-19 20:45:53.000000 claudia-0.0.7/setup.py
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-20 01:18:38.577495 claudia-0.0.7/src/
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-20 01:18:38.585861 claudia-0.0.7/src/claudia/
+-rw-r--r--   0 ksaxena    (502) staff       (20)     3184 2023-05-20 01:12:37.000000 claudia-0.0.7/src/claudia/README.md
+-rw-r--r--   0 ksaxena    (502) staff       (20)        0 2023-05-15 18:14:02.000000 claudia-0.0.7/src/claudia/__init__.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)    12019 2023-05-20 00:12:23.000000 claudia-0.0.7/src/claudia/claudia.py
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-20 01:18:38.587475 claudia-0.0.7/src/claudia/features/
+-rw-r--r--   0 ksaxena    (502) staff       (20)    14321 2023-05-15 18:14:02.000000 claudia-0.0.7/src/claudia/features/nft_burn_mint.feature
+-rw-r--r--   0 ksaxena    (502) staff       (20)     5371 2023-05-15 18:14:02.000000 claudia-0.0.7/src/claudia/features/payments.feature
+-rw-r--r--   0 ksaxena    (502) staff       (20)    11071 2023-05-15 18:14:02.000000 claudia-0.0.7/src/claudia/features/trustline.feature
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-20 01:18:38.591024 claudia-0.0.7/src/claudia/javascript/
+-rwxr-xr-x   0 ksaxena    (502) staff       (20)      118 2023-05-15 18:14:02.000000 claudia-0.0.7/src/claudia/javascript/cleanup
+-rw-r--r--   0 ksaxena    (502) staff       (20)      145 2023-05-15 18:14:02.000000 claudia-0.0.7/src/claudia/javascript/cucumber.js
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-20 01:18:38.591387 claudia-0.0.7/src/claudia/javascript/features/
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1226 2023-05-15 18:14:02.000000 claudia-0.0.7/src/claudia/javascript/features/context.js
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-20 01:18:38.591779 claudia-0.0.7/src/claudia/javascript/features/lib/
+-rw-r--r--   0 ksaxena    (502) staff       (20)     2106 2023-05-15 18:14:02.000000 claudia-0.0.7/src/claudia/javascript/features/lib/ObjFactory.js
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-20 01:18:38.594896 claudia-0.0.7/src/claudia/javascript/features/steps/
+-rw-r--r--   0 ksaxena    (502) staff       (20)    38728 2023-05-15 18:14:02.000000 claudia-0.0.7/src/claudia/javascript/features/steps/common.js
+-rw-r--r--   0 ksaxena    (502) staff       (20)      300 2023-05-15 18:14:02.000000 claudia-0.0.7/src/claudia/javascript/features/steps/constants.js
+-rw-r--r--   0 ksaxena    (502) staff       (20)    71153 2023-05-15 18:14:02.000000 claudia-0.0.7/src/claudia/javascript/features/steps/nft_mint_burn.js
+-rw-r--r--   0 ksaxena    (502) staff       (20)    19024 2023-05-15 18:14:02.000000 claudia-0.0.7/src/claudia/javascript/features/steps/payments.js
+-rw-r--r--   0 ksaxena    (502) staff       (20)    59478 2023-05-15 18:14:02.000000 claudia-0.0.7/src/claudia/javascript/features/steps/trustline.js
+-rw-r--r--   0 ksaxena    (502) staff       (20)   129466 2023-05-15 18:14:02.000000 claudia-0.0.7/src/claudia/javascript/package-lock.json
+-rw-r--r--   0 ksaxena    (502) staff       (20)      221 2023-05-15 18:14:02.000000 claudia-0.0.7/src/claudia/javascript/package.json
+-rwxr-xr-x   0 ksaxena    (502) staff       (20)      869 2023-05-15 18:14:02.000000 claudia-0.0.7/src/claudia/javascript/runSetup
+-rwxr-xr-x   0 ksaxena    (502) staff       (20)     4674 2023-05-15 18:14:02.000000 claudia-0.0.7/src/claudia/javascript/runTest
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-20 01:18:38.595740 claudia-0.0.7/src/claudia/network_setup/
+-rw-rw-r--   0 ksaxena    (502) staff       (20)      251 2023-05-18 02:32:34.000000 claudia-0.0.7/src/claudia/network_setup/Dockerfile
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-20 01:18:38.597026 claudia-0.0.7/src/claudia/network_setup/configs/
+-rw-rw-r--   0 ksaxena    (502) staff       (20)     1520 2023-05-18 02:32:34.000000 claudia-0.0.7/src/claudia/network_setup/configs/rippled.cfg
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-20 01:18:38.597842 claudia-0.0.7/src/claudia/network_setup/configs/rippled_1/
+-rw-rw-r--   0 ksaxena    (502) staff       (20)     2150 2023-05-18 02:32:34.000000 claudia-0.0.7/src/claudia/network_setup/configs/rippled_1/rippled.cfg
+-rw-rw-r--   0 ksaxena    (502) staff       (20)      278 2023-05-18 02:32:34.000000 claudia-0.0.7/src/claudia/network_setup/configs/rippled_1/validators.txt
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-20 01:18:38.598531 claudia-0.0.7/src/claudia/network_setup/configs/rippled_2/
+-rw-rw-r--   0 ksaxena    (502) staff       (20)     2191 2023-05-18 02:32:34.000000 claudia-0.0.7/src/claudia/network_setup/configs/rippled_2/rippled.cfg
+-rw-rw-r--   0 ksaxena    (502) staff       (20)      278 2023-05-18 02:32:34.000000 claudia-0.0.7/src/claudia/network_setup/configs/rippled_2/validators.txt
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-20 01:18:38.599389 claudia-0.0.7/src/claudia/network_setup/configs/rippled_3/
+-rw-rw-r--   0 ksaxena    (502) staff       (20)     2191 2023-05-18 02:32:34.000000 claudia-0.0.7/src/claudia/network_setup/configs/rippled_3/rippled.cfg
+-rw-rw-r--   0 ksaxena    (502) staff       (20)      278 2023-05-18 02:32:34.000000 claudia-0.0.7/src/claudia/network_setup/configs/rippled_3/validators.txt
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-20 01:18:38.600149 claudia-0.0.7/src/claudia/network_setup/configs/rippled_4/
+-rw-rw-r--   0 ksaxena    (502) staff       (20)     2190 2023-05-18 02:32:34.000000 claudia-0.0.7/src/claudia/network_setup/configs/rippled_4/rippled.cfg
+-rw-rw-r--   0 ksaxena    (502) staff       (20)      278 2023-05-18 02:32:34.000000 claudia-0.0.7/src/claudia/network_setup/configs/rippled_4/validators.txt
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-20 01:18:38.600916 claudia-0.0.7/src/claudia/network_setup/configs/rippled_5/
+-rw-rw-r--   0 ksaxena    (502) staff       (20)     2226 2023-05-18 02:32:34.000000 claudia-0.0.7/src/claudia/network_setup/configs/rippled_5/rippled.cfg
+-rw-rw-r--   0 ksaxena    (502) staff       (20)      278 2023-05-18 02:32:34.000000 claudia-0.0.7/src/claudia/network_setup/configs/rippled_5/validators.txt
+-rw-rw-r--   0 ksaxena    (502) staff       (20)      279 2023-05-18 02:32:34.000000 claudia-0.0.7/src/claudia/network_setup/configs/validators.txt
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-20 01:18:38.602617 claudia-0.0.7/src/claudia/network_setup/lib/
+-rw-rw-r--   0 ksaxena    (502) staff       (20)     1619 2023-05-18 02:32:34.000000 claudia-0.0.7/src/claudia/network_setup/lib/build_rippled.sh
+-rw-rw-r--   0 ksaxena    (502) staff       (20)     2161 2023-05-18 02:32:34.000000 claudia-0.0.7/src/claudia/network_setup/lib/rippled_network.yml
+-rw-rw-r--   0 ksaxena    (502) staff       (20)     8966 2023-05-18 02:32:34.000000 claudia-0.0.7/src/claudia/network_setup/lib/setup_helper.sh
+-rw-rw-r--   0 ksaxena    (502) staff       (20)     5094 2023-05-18 02:32:34.000000 claudia-0.0.7/src/claudia/network_setup/lib/validate_network.py
+-rw-rw-r--   0 ksaxena    (502) staff       (20)     3784 2023-05-18 02:32:34.000000 claudia-0.0.7/src/claudia/network_setup/setup.sh
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-20 01:18:38.605339 claudia-0.0.7/src/claudia/python/
+-rw-r--r--   0 ksaxena    (502) staff       (20)        0 2023-05-15 18:14:02.000000 claudia-0.0.7/src/claudia/python/__init__.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)      107 2023-05-15 18:14:02.000000 claudia-0.0.7/src/claudia/python/behave.ini
+-rwxr-xr-x   0 ksaxena    (502) staff       (20)      123 2023-05-15 18:14:02.000000 claudia-0.0.7/src/claudia/python/cleanup
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-20 01:18:38.606219 claudia-0.0.7/src/claudia/python/features/
+-rw-r--r--   0 ksaxena    (502) staff       (20)        0 2023-05-15 18:14:02.000000 claudia-0.0.7/src/claudia/python/features/__init__.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)     2977 2023-05-15 18:14:02.000000 claudia-0.0.7/src/claudia/python/features/environment.py
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-20 01:18:38.607088 claudia-0.0.7/src/claudia/python/features/exceptions/
+-rw-r--r--   0 ksaxena    (502) staff       (20)       49 2023-05-15 18:14:02.000000 claudia-0.0.7/src/claudia/python/features/exceptions/InvalidInputException.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)       60 2023-05-15 18:14:02.000000 claudia-0.0.7/src/claudia/python/features/exceptions/UnconfiguredEnvironmentException.py
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-20 01:18:38.607946 claudia-0.0.7/src/claudia/python/features/lib/
+-rw-r--r--   0 ksaxena    (502) staff       (20)      301 2023-05-15 18:14:02.000000 claudia-0.0.7/src/claudia/python/features/lib/Helpers.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)     7674 2023-05-15 18:14:02.000000 claudia-0.0.7/src/claudia/python/features/lib/ObjFactory.py
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-20 01:18:38.610124 claudia-0.0.7/src/claudia/python/features/steps/
+-rw-r--r--   0 ksaxena    (502) staff       (20)    24750 2023-05-15 18:14:02.000000 claudia-0.0.7/src/claudia/python/features/steps/common.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)      251 2023-05-15 18:14:02.000000 claudia-0.0.7/src/claudia/python/features/steps/constants.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)    66340 2023-05-15 18:14:02.000000 claudia-0.0.7/src/claudia/python/features/steps/nft_mint_burn.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)    21822 2023-05-15 18:14:02.000000 claudia-0.0.7/src/claudia/python/features/steps/payments.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)    54620 2023-05-15 18:14:02.000000 claudia-0.0.7/src/claudia/python/features/steps/trustline.py
+-rwxr-xr-x   0 ksaxena    (502) staff       (20)     1381 2023-05-15 18:14:02.000000 claudia-0.0.7/src/claudia/python/runSetup
+-rwxr-xr-x   0 ksaxena    (502) staff       (20)     5634 2023-05-15 18:14:02.000000 claudia-0.0.7/src/claudia/python/runTest
+-rw-r--r--   0 ksaxena    (502) staff       (20)       88 2023-05-19 20:42:19.000000 claudia-0.0.7/src/claudia/requirements.txt
```

### Comparing `claudia-0.0.6/LICENSE` & `claudia-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `claudia-0.0.6/claudia.egg-info/SOURCES.txt` & `claudia-0.0.7/claudia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `claudia-0.0.6/setup.py` & `claudia-0.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         requirements = content.split('\n')
 
     return requirements
 
 
 setup(
     name='claudia',
-    version='0.0.6',
+    version='0.0.7',
     description='Run XRPL Automated Tests',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     author="Kausty Saxena",
     author_email="ksaxena@ripple.com",
     keywords="ripple xrpl python javascript",
     url='https://xrpl.org/',
```

### Comparing `claudia-0.0.6/src/claudia/claudia.py` & `claudia-0.0.7/src/claudia/claudia.py`

 * *Files 14% similar despite different names*

```diff
@@ -61,14 +61,15 @@
     features = os.listdir('./features/')
     for i in range(0, len(features)):
         message += "'{}', ".format(features[i].replace(".feature", ""))
     message += "and 'all' and is defaulted to 'payments'. \n\nMore information: https://behave.readthedocs.io/en/latest/tutorial.html?highlight=feature#feature-files."
     return message
 
 @click.group()
+@click.version_option(message=('%(prog)s version %(version)s'))
 def main():
     """Claudia says hi! Please choose a command to perform an action. A command can have multiple sub-commands and options. Use '--help' option for more information."""
 
 @main.group()
 def rippled():
     """Build or install rippled"""
 
@@ -77,14 +78,42 @@
     """Setup Rippled Network"""
 
 @main.group()
 @click.pass_context
 def run(context):
     """Run XRPL automated tests"""
 
+@main.group()
+def list():
+    """List supported options"""
+
+@list.command()
+def e2e_features():
+    """List all supported features to be tested"""
+    set_to_project_root_wd()
+    features = os.listdir('./features/')
+    message = "Following features were found:\n"
+    for i in range(0, len(features)):
+        message += "   - {}\n".format(features[i].replace(".feature", ""))
+    click.echo(message)
+
+@list.command()
+def system_requirements():
+    """List all system requirements before continuing further with claudia"""
+    message = """
+    1. Common requirements:
+        - Python3: More information: https://www.python.org/downloads/
+        - pip: More information: https://pip.pypa.io/en/stable/installation/
+        - docker: More information: https://docs.docker.com/engine/install/
+    2. Pull down a fresh copy of rippled code base from https://github.com/XRPLF/rippled
+    3. Optional: Following depedencies are only required if you intend to run Javascript tests:
+        - node: More information: https://nodejs.org/en/download
+        - npm: More information: https://www.npmjs.com/package/download
+    """
+    click.echo(message)
 
 @rippled.command()
 @click.option('--repo', required=True, help="The path to a local rippled repo")
 def build(repo):
     """Build rippled from source"""
     set_to_project_root_wd()
     command = "sh network_setup/setup.sh --buildRippled --rippledRepo {}".format(repo)
@@ -118,19 +147,17 @@
 @network.command()
 def status():
     """rippled network status"""
     set_to_project_root_wd()
     command = "sh ./network_setup/setup.sh --networkStatus"
     subprocess.call(command, shell=True)
 
-
 def print_explorer_message(network):
     if(network=='local'):
-        print("INFO: Navigate to 'https://custom.xrpl.org/localhost:6001' to open explorer for this test run against local network.\n")
-
+        click.echo("INFO: Navigate to 'https://custom.xrpl.org/localhost:6001' to open explorer for this test run against local network.\n")
 
 @run.command()
 @click.pass_context
 @click.option('--lib', default='py',
               help="The type of client library to be used for running the tests. Allowed values are 'py' and 'js' and is defaulted to 'py'.  \n\nMore information: https://xrpl.org/client-libraries.html#client-libraries")
 @click.option('--client_type', default='websocket',
               help="The type of client to be used. This flag should only be used with 'py' library. Allowed values are 'websocket' and 'jsonrpc' and is defaulted to 'websocket'.  \n\nMore information: https://xrpl.org/get-started-using-http-websocket-apis.html#differences-between-json-rpc-and-websocket")
@@ -163,21 +190,21 @@
 # def customcommand(context, text):
 #     """Run a debug command"""
 #     click.echo("Running command: {}".format(text))
 #     subprocess.call(text, shell=True)
 
 
 def invalidate_cache_and_rebuild():
-    print("Invalidating cache...")
+    click.echo("Invalidating cache...")
     os.popen('rm -rf ./node_modules')
     install_js_dependencies_if_needed()
 
 
 def first_time_build():
-    print("Need to install missing dependencies. It is a one time action. Please wait...")
+    click.echo("Need to install missing dependencies. It is a one time action. Please wait...")
     install_js_dependencies_if_needed()
 
 
 def set_python_launch_vars(network, client_type):
     if network == "local":
         if client_type == "websocket":
             connectionScheme = "ws"
```

### Comparing `claudia-0.0.6/src/claudia/features/nft_burn_mint.feature` & `claudia-0.0.7/src/claudia/features/nft_burn_mint.feature`

 * *Files identical despite different names*

### Comparing `claudia-0.0.6/src/claudia/features/payments.feature` & `claudia-0.0.7/src/claudia/features/payments.feature`

 * *Files identical despite different names*

### Comparing `claudia-0.0.6/src/claudia/features/trustline.feature` & `claudia-0.0.7/src/claudia/features/trustline.feature`

 * *Files identical despite different names*

### Comparing `claudia-0.0.6/src/claudia/javascript/features/context.js` & `claudia-0.0.7/src/claudia/javascript/features/context.js`

 * *Files identical despite different names*

### Comparing `claudia-0.0.6/src/claudia/javascript/features/lib/ObjFactory.js` & `claudia-0.0.7/src/claudia/javascript/features/lib/ObjFactory.js`

 * *Files identical despite different names*

### Comparing `claudia-0.0.6/src/claudia/javascript/features/steps/common.js` & `claudia-0.0.7/src/claudia/javascript/features/steps/common.js`

 * *Files identical despite different names*

### Comparing `claudia-0.0.6/src/claudia/javascript/features/steps/nft_mint_burn.js` & `claudia-0.0.7/src/claudia/javascript/features/steps/nft_mint_burn.js`

 * *Files identical despite different names*

### Comparing `claudia-0.0.6/src/claudia/javascript/features/steps/payments.js` & `claudia-0.0.7/src/claudia/javascript/features/steps/payments.js`

 * *Files identical despite different names*

### Comparing `claudia-0.0.6/src/claudia/javascript/features/steps/trustline.js` & `claudia-0.0.7/src/claudia/javascript/features/steps/trustline.js`

 * *Files identical despite different names*

### Comparing `claudia-0.0.6/src/claudia/javascript/package-lock.json` & `claudia-0.0.7/src/claudia/javascript/package-lock.json`

 * *Files identical despite different names*

### Comparing `claudia-0.0.6/src/claudia/javascript/runSetup` & `claudia-0.0.7/src/claudia/javascript/runSetup`

 * *Files identical despite different names*

### Comparing `claudia-0.0.6/src/claudia/javascript/runTest` & `claudia-0.0.7/src/claudia/javascript/runTest`

 * *Files identical despite different names*

### Comparing `claudia-0.0.6/src/claudia/network_setup/configs/rippled.cfg` & `claudia-0.0.7/src/claudia/network_setup/configs/rippled.cfg`

 * *Files identical despite different names*

### Comparing `claudia-0.0.6/src/claudia/network_setup/configs/rippled_1/rippled.cfg` & `claudia-0.0.7/src/claudia/network_setup/configs/rippled_1/rippled.cfg`

 * *Files identical despite different names*

### Comparing `claudia-0.0.6/src/claudia/network_setup/configs/rippled_2/rippled.cfg` & `claudia-0.0.7/src/claudia/network_setup/configs/rippled_2/rippled.cfg`

 * *Files identical despite different names*

### Comparing `claudia-0.0.6/src/claudia/network_setup/configs/rippled_3/rippled.cfg` & `claudia-0.0.7/src/claudia/network_setup/configs/rippled_3/rippled.cfg`

 * *Files identical despite different names*

### Comparing `claudia-0.0.6/src/claudia/network_setup/configs/rippled_4/rippled.cfg` & `claudia-0.0.7/src/claudia/network_setup/configs/rippled_4/rippled.cfg`

 * *Files identical despite different names*

### Comparing `claudia-0.0.6/src/claudia/network_setup/configs/rippled_5/rippled.cfg` & `claudia-0.0.7/src/claudia/network_setup/configs/rippled_5/rippled.cfg`

 * *Files identical despite different names*

### Comparing `claudia-0.0.6/src/claudia/network_setup/lib/build_rippled.sh` & `claudia-0.0.7/src/claudia/network_setup/lib/build_rippled.sh`

 * *Files identical despite different names*

### Comparing `claudia-0.0.6/src/claudia/network_setup/lib/rippled_network.yml` & `claudia-0.0.7/src/claudia/network_setup/lib/rippled_network.yml`

 * *Files identical despite different names*

### Comparing `claudia-0.0.6/src/claudia/network_setup/lib/setup_helper.sh` & `claudia-0.0.7/src/claudia/network_setup/lib/setup_helper.sh`

 * *Files identical despite different names*

### Comparing `claudia-0.0.6/src/claudia/network_setup/lib/validate_network.py` & `claudia-0.0.7/src/claudia/network_setup/lib/validate_network.py`

 * *Files identical despite different names*

### Comparing `claudia-0.0.6/src/claudia/network_setup/setup.sh` & `claudia-0.0.7/src/claudia/network_setup/setup.sh`

 * *Files identical despite different names*

### Comparing `claudia-0.0.6/src/claudia/python/features/environment.py` & `claudia-0.0.7/src/claudia/python/features/environment.py`

 * *Files identical despite different names*

### Comparing `claudia-0.0.6/src/claudia/python/features/lib/ObjFactory.py` & `claudia-0.0.7/src/claudia/python/features/lib/ObjFactory.py`

 * *Files identical despite different names*

### Comparing `claudia-0.0.6/src/claudia/python/features/steps/common.py` & `claudia-0.0.7/src/claudia/python/features/steps/common.py`

 * *Files identical despite different names*

### Comparing `claudia-0.0.6/src/claudia/python/features/steps/nft_mint_burn.py` & `claudia-0.0.7/src/claudia/python/features/steps/nft_mint_burn.py`

 * *Files identical despite different names*

### Comparing `claudia-0.0.6/src/claudia/python/features/steps/payments.py` & `claudia-0.0.7/src/claudia/python/features/steps/payments.py`

 * *Files identical despite different names*

### Comparing `claudia-0.0.6/src/claudia/python/features/steps/trustline.py` & `claudia-0.0.7/src/claudia/python/features/steps/trustline.py`

 * *Files identical despite different names*

### Comparing `claudia-0.0.6/src/claudia/python/runSetup` & `claudia-0.0.7/src/claudia/python/runSetup`

 * *Files identical despite different names*

### Comparing `claudia-0.0.6/src/claudia/python/runTest` & `claudia-0.0.7/src/claudia/python/runTest`

 * *Files identical despite different names*

