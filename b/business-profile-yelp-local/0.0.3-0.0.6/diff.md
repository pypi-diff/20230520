# Comparing `tmp/business-profile-yelp-local-0.0.3.tar.gz` & `tmp/business_profile_yelp_local-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "business-profile-yelp-local-0.0.3.tar", last modified: Mon May 15 01:07:01 2023, max compression
+gzip compressed data, was "business_profile_yelp_local-0.0.6.tar", last modified: Sat May 20 15:20:01 2023, max compression
```

## Comparing `business-profile-yelp-local-0.0.3.tar` & `business_profile_yelp_local-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:07:01.733058 business-profile-yelp-local-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-15 01:07:01.733058 business-profile-yelp-local-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-15 01:06:46.000000 business-profile-yelp-local-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:07:01.733058 business-profile-yelp-local-0.0.3/business_profile_yelp_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-15 01:07:01.000000 business-profile-yelp-local-0.0.3/business_profile_yelp_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-15 01:07:01.000000 business-profile-yelp-local-0.0.3/business_profile_yelp_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 01:07:01.000000 business-profile-yelp-local-0.0.3/business_profile_yelp_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 01:07:01.000000 business-profile-yelp-local-0.0.3/business_profile_yelp_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-15 01:06:46.000000 business-profile-yelp-local-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 01:07:01.733058 business-profile-yelp-local-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-15 01:06:46.000000 business-profile-yelp-local-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:07:01.733058 business-profile-yelp-local-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-15 01:06:46.000000 business-profile-yelp-local-0.0.3/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 15:20:01.021832 business_profile_yelp_local-0.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 15:20:01.017832 business_profile_yelp_local-0.0.6/LocalYelpPython/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 15:19:47.000000 business_profile_yelp_local-0.0.6/LocalYelpPython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-05-20 15:19:47.000000 business_profile_yelp_local-0.0.6/LocalYelpPython/yelp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-20 15:20:01.021832 business_profile_yelp_local-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-20 15:19:47.000000 business_profile_yelp_local-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 15:20:01.021832 business_profile_yelp_local-0.0.6/business_profile_yelp_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-20 15:20:01.000000 business_profile_yelp_local-0.0.6/business_profile_yelp_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-20 15:20:01.000000 business_profile_yelp_local-0.0.6/business_profile_yelp_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 15:20:01.000000 business_profile_yelp_local-0.0.6/business_profile_yelp_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-20 15:20:01.000000 business_profile_yelp_local-0.0.6/business_profile_yelp_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-20 15:19:47.000000 business_profile_yelp_local-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 15:20:01.021832 business_profile_yelp_local-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-20 15:19:47.000000 business_profile_yelp_local-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 15:20:01.021832 business_profile_yelp_local-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-20 15:19:47.000000 business_profile_yelp_local-0.0.6/tests/tests.py
```

### Comparing `business-profile-yelp-local-0.0.3/setup.py` & `business_profile_yelp_local-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 # used by python -m build
 # python -m build needs pyproject.toml or setup.py
 setuptools.setup(
-     name='business-profile-yelp-local',  
-     version='0.0.3',
+     name='business_profile_yelp_local',  
+     version='0.0.6',
      author="Circles",
      author_email="info@circles.life",
      description="PyPI Package for Circles Local Yelp Profile Python",
      long_description="This is a package for sharing common yelp service function used in different repositories",
      long_description_content_type="text/markdown",
      url="https://github.com/javatechy/dokr",
      packages=setuptools.find_packages(),
```

