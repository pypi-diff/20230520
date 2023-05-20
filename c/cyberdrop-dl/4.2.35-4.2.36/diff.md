# Comparing `tmp/cyberdrop-dl-4.2.35.tar.gz` & `tmp/cyberdrop-dl-4.2.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyberdrop-dl-4.2.35.tar", last modified: Sat May 20 01:31:41 2023, max compression
+gzip compressed data, was "cyberdrop-dl-4.2.36.tar", last modified: Sat May 20 03:18:33 2023, max compression
```

## Comparing `cyberdrop-dl-4.2.35.tar` & `cyberdrop-dl-4.2.36.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:31:41.020496 cyberdrop-dl-4.2.35/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-20 01:31:32.000000 cyberdrop-dl-4.2.35/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18155 2023-05-20 01:31:41.020496 cyberdrop-dl-4.2.35/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17720 2023-05-20 01:31:32.000000 cyberdrop-dl-4.2.35/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:31:41.012496 cyberdrop-dl-4.2.35/cyberdrop_dl/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-20 01:31:32.000000 cyberdrop-dl-4.2.35/cyberdrop_dl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:31:41.016496 cyberdrop-dl-4.2.35/cyberdrop_dl/base_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 01:31:32.000000 cyberdrop-dl-4.2.35/cyberdrop_dl/base_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-05-20 01:31:32.000000 cyberdrop-dl-4.2.35/cyberdrop_dl/base_functions/base_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-05-20 01:31:32.000000 cyberdrop-dl-4.2.35/cyberdrop_dl/base_functions/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-05-20 01:31:32.000000 cyberdrop-dl-4.2.35/cyberdrop_dl/base_functions/config_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-05-20 01:31:32.000000 cyberdrop-dl-4.2.35/cyberdrop_dl/base_functions/data_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-20 01:31:32.000000 cyberdrop-dl-4.2.35/cyberdrop_dl/base_functions/error_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-20 01:31:32.000000 cyberdrop-dl-4.2.35/cyberdrop_dl/base_functions/sorting_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-05-20 01:31:32.000000 cyberdrop-dl-4.2.35/cyberdrop_dl/base_functions/sql_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:31:41.016496 cyberdrop-dl-4.2.35/cyberdrop_dl/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 01:31:32.000000 cyberdrop-dl-4.2.35/cyberdrop_dl/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10099 2023-05-20 01:31:32.000000 cyberdrop-dl-4.2.35/cyberdrop_dl/client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:31:41.020496 cyberdrop-dl-4.2.35/cyberdrop_dl/crawlers/
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-20 01:31:32.000000 cyberdrop-dl-4.2.35/cyberdrop_dl/crawlers/Anonfiles_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7802 2023-05-20 01:31:32.000000 cyberdrop-dl-4.2.35/cyberdrop_dl/crawlers/Bunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-05-20 01:31:32.000000 cyberdrop-dl-4.2.35/cyberdrop_dl/crawlers/Coomeno_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-05-20 01:31:32.000000 cyberdrop-dl-4.2.35/cyberdrop_dl/crawlers/CyberFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-20 01:31:32.000000 cyberdrop-dl-4.2.35/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-05-20 01:31:32.000000 cyberdrop-dl-4.2.35/cyberdrop_dl/crawlers/EHentai_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-05-20 01:31:32.000000 cyberdrop-dl-4.2.35/cyberdrop_dl/crawlers/Erome_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-05-20 01:31:32.000000 cyberdrop-dl-4.2.35/cyberdrop_dl/crawlers/Fapello_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-20 01:31:32.000000 cyberdrop-dl-4.2.35/cyberdrop_dl/crawlers/Gfycat_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-05-20 01:31:32.000000 cyberdrop-dl-4.2.35/cyberdrop_dl/crawlers/GoFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-05-20 01:31:32.000000 cyberdrop-dl-4.2.35/cyberdrop_dl/crawlers/HGameCG_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-20 01:31:32.000000 cyberdrop-dl-4.2.35/cyberdrop_dl/crawlers/ImgBox_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-05-20 01:31:32.000000 cyberdrop-dl-4.2.35/cyberdrop_dl/crawlers/LoveFap_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-05-20 01:31:32.000000 cyberdrop-dl-4.2.35/cyberdrop_dl/crawlers/NSFWXXX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-05-20 01:31:32.000000 cyberdrop-dl-4.2.35/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-20 01:31:32.000000 cyberdrop-dl-4.2.35/cyberdrop_dl/crawlers/PixelDrain_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-05-20 01:31:32.000000 cyberdrop-dl-4.2.35/cyberdrop_dl/crawlers/PostImg_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-20 01:31:32.000000 cyberdrop-dl-4.2.35/cyberdrop_dl/crawlers/Saint_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-05-20 01:31:32.000000 cyberdrop-dl-4.2.35/cyberdrop_dl/crawlers/ShareX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-20 01:31:32.000000 cyberdrop-dl-4.2.35/cyberdrop_dl/crawlers/XBunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    13919 2023-05-20 01:31:32.000000 cyberdrop-dl-4.2.35/cyberdrop_dl/crawlers/Xenforo_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 01:31:32.000000 cyberdrop-dl-4.2.35/cyberdrop_dl/crawlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:31:41.020496 cyberdrop-dl-4.2.35/cyberdrop_dl/downloader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 01:31:32.000000 cyberdrop-dl-4.2.35/cyberdrop_dl/downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-05-20 01:31:32.000000 cyberdrop-dl-4.2.35/cyberdrop_dl/downloader/downloader_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18477 2023-05-20 01:31:32.000000 cyberdrop-dl-4.2.35/cyberdrop_dl/downloader/downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    12795 2023-05-20 01:31:32.000000 cyberdrop-dl-4.2.35/cyberdrop_dl/downloader/old_downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    17463 2023-05-20 01:31:32.000000 cyberdrop-dl-4.2.35/cyberdrop_dl/downloader/progress_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    20522 2023-05-20 01:31:32.000000 cyberdrop-dl-4.2.35/cyberdrop_dl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:31:41.020496 cyberdrop-dl-4.2.35/cyberdrop_dl/scraper/
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-20 01:31:32.000000 cyberdrop-dl-4.2.35/cyberdrop_dl/scraper/JDownloader_Integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    20427 2023-05-20 01:31:32.000000 cyberdrop-dl-4.2.35/cyberdrop_dl/scraper/Scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 01:31:32.000000 cyberdrop-dl-4.2.35/cyberdrop_dl/scraper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 01:31:41.016496 cyberdrop-dl-4.2.35/cyberdrop_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18155 2023-05-20 01:31:41.000000 cyberdrop-dl-4.2.35/cyberdrop_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-20 01:31:41.000000 cyberdrop-dl-4.2.35/cyberdrop_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 01:31:41.000000 cyberdrop-dl-4.2.35/cyberdrop_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-20 01:31:41.000000 cyberdrop-dl-4.2.35/cyberdrop_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-20 01:31:41.000000 cyberdrop-dl-4.2.35/cyberdrop_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-20 01:31:41.000000 cyberdrop-dl-4.2.35/cyberdrop_dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-20 01:31:32.000000 cyberdrop-dl-4.2.35/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-20 01:31:41.020496 cyberdrop-dl-4.2.35/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 01:31:32.000000 cyberdrop-dl-4.2.35/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:18:33.430883 cyberdrop-dl-4.2.36/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-20 03:18:24.000000 cyberdrop-dl-4.2.36/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18155 2023-05-20 03:18:33.430883 cyberdrop-dl-4.2.36/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17720 2023-05-20 03:18:24.000000 cyberdrop-dl-4.2.36/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:18:33.426883 cyberdrop-dl-4.2.36/cyberdrop_dl/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-20 03:18:24.000000 cyberdrop-dl-4.2.36/cyberdrop_dl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:18:33.426883 cyberdrop-dl-4.2.36/cyberdrop_dl/base_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 03:18:24.000000 cyberdrop-dl-4.2.36/cyberdrop_dl/base_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-05-20 03:18:24.000000 cyberdrop-dl-4.2.36/cyberdrop_dl/base_functions/base_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-05-20 03:18:24.000000 cyberdrop-dl-4.2.36/cyberdrop_dl/base_functions/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-05-20 03:18:24.000000 cyberdrop-dl-4.2.36/cyberdrop_dl/base_functions/config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-05-20 03:18:24.000000 cyberdrop-dl-4.2.36/cyberdrop_dl/base_functions/data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-20 03:18:24.000000 cyberdrop-dl-4.2.36/cyberdrop_dl/base_functions/error_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-20 03:18:24.000000 cyberdrop-dl-4.2.36/cyberdrop_dl/base_functions/sorting_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-05-20 03:18:24.000000 cyberdrop-dl-4.2.36/cyberdrop_dl/base_functions/sql_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:18:33.426883 cyberdrop-dl-4.2.36/cyberdrop_dl/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 03:18:24.000000 cyberdrop-dl-4.2.36/cyberdrop_dl/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10099 2023-05-20 03:18:24.000000 cyberdrop-dl-4.2.36/cyberdrop_dl/client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:18:33.430883 cyberdrop-dl-4.2.36/cyberdrop_dl/crawlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-20 03:18:24.000000 cyberdrop-dl-4.2.36/cyberdrop_dl/crawlers/Anonfiles_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7802 2023-05-20 03:18:24.000000 cyberdrop-dl-4.2.36/cyberdrop_dl/crawlers/Bunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-05-20 03:18:24.000000 cyberdrop-dl-4.2.36/cyberdrop_dl/crawlers/Coomeno_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-05-20 03:18:24.000000 cyberdrop-dl-4.2.36/cyberdrop_dl/crawlers/CyberFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-20 03:18:24.000000 cyberdrop-dl-4.2.36/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-05-20 03:18:24.000000 cyberdrop-dl-4.2.36/cyberdrop_dl/crawlers/EHentai_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-05-20 03:18:24.000000 cyberdrop-dl-4.2.36/cyberdrop_dl/crawlers/Erome_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-05-20 03:18:24.000000 cyberdrop-dl-4.2.36/cyberdrop_dl/crawlers/Fapello_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-20 03:18:24.000000 cyberdrop-dl-4.2.36/cyberdrop_dl/crawlers/Gfycat_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-05-20 03:18:24.000000 cyberdrop-dl-4.2.36/cyberdrop_dl/crawlers/GoFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-05-20 03:18:24.000000 cyberdrop-dl-4.2.36/cyberdrop_dl/crawlers/HGameCG_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-20 03:18:24.000000 cyberdrop-dl-4.2.36/cyberdrop_dl/crawlers/ImgBox_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-05-20 03:18:24.000000 cyberdrop-dl-4.2.36/cyberdrop_dl/crawlers/LoveFap_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-05-20 03:18:24.000000 cyberdrop-dl-4.2.36/cyberdrop_dl/crawlers/NSFWXXX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-05-20 03:18:24.000000 cyberdrop-dl-4.2.36/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-20 03:18:24.000000 cyberdrop-dl-4.2.36/cyberdrop_dl/crawlers/PixelDrain_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-05-20 03:18:24.000000 cyberdrop-dl-4.2.36/cyberdrop_dl/crawlers/PostImg_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-20 03:18:24.000000 cyberdrop-dl-4.2.36/cyberdrop_dl/crawlers/Saint_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-05-20 03:18:24.000000 cyberdrop-dl-4.2.36/cyberdrop_dl/crawlers/ShareX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-20 03:18:24.000000 cyberdrop-dl-4.2.36/cyberdrop_dl/crawlers/XBunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13919 2023-05-20 03:18:24.000000 cyberdrop-dl-4.2.36/cyberdrop_dl/crawlers/Xenforo_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 03:18:24.000000 cyberdrop-dl-4.2.36/cyberdrop_dl/crawlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:18:33.430883 cyberdrop-dl-4.2.36/cyberdrop_dl/downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 03:18:24.000000 cyberdrop-dl-4.2.36/cyberdrop_dl/downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-05-20 03:18:24.000000 cyberdrop-dl-4.2.36/cyberdrop_dl/downloader/downloader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18477 2023-05-20 03:18:24.000000 cyberdrop-dl-4.2.36/cyberdrop_dl/downloader/downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12870 2023-05-20 03:18:24.000000 cyberdrop-dl-4.2.36/cyberdrop_dl/downloader/old_downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17463 2023-05-20 03:18:24.000000 cyberdrop-dl-4.2.36/cyberdrop_dl/downloader/progress_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20536 2023-05-20 03:18:24.000000 cyberdrop-dl-4.2.36/cyberdrop_dl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:18:33.430883 cyberdrop-dl-4.2.36/cyberdrop_dl/scraper/
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-20 03:18:24.000000 cyberdrop-dl-4.2.36/cyberdrop_dl/scraper/JDownloader_Integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20427 2023-05-20 03:18:24.000000 cyberdrop-dl-4.2.36/cyberdrop_dl/scraper/Scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 03:18:24.000000 cyberdrop-dl-4.2.36/cyberdrop_dl/scraper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 03:18:33.426883 cyberdrop-dl-4.2.36/cyberdrop_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18155 2023-05-20 03:18:33.000000 cyberdrop-dl-4.2.36/cyberdrop_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-20 03:18:33.000000 cyberdrop-dl-4.2.36/cyberdrop_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 03:18:33.000000 cyberdrop-dl-4.2.36/cyberdrop_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-20 03:18:33.000000 cyberdrop-dl-4.2.36/cyberdrop_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-20 03:18:33.000000 cyberdrop-dl-4.2.36/cyberdrop_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-20 03:18:33.000000 cyberdrop-dl-4.2.36/cyberdrop_dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-20 03:18:24.000000 cyberdrop-dl-4.2.36/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-20 03:18:33.430883 cyberdrop-dl-4.2.36/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 03:18:24.000000 cyberdrop-dl-4.2.36/setup.py
```

### Comparing `cyberdrop-dl-4.2.35/LICENSE` & `cyberdrop-dl-4.2.36/LICENSE`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.35/PKG-INFO` & `cyberdrop-dl-4.2.36/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.2.35
+Version: 4.2.36
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.35 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.36 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
```

### Comparing `cyberdrop-dl-4.2.35/README.md` & `cyberdrop-dl-4.2.36/README.md`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.35/cyberdrop_dl/base_functions/base_functions.py` & `cyberdrop-dl-4.2.36/cyberdrop_dl/base_functions/base_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.35/cyberdrop_dl/base_functions/config_manager.py` & `cyberdrop-dl-4.2.36/cyberdrop_dl/base_functions/config_manager.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.35/cyberdrop_dl/base_functions/config_schema.py` & `cyberdrop-dl-4.2.36/cyberdrop_dl/base_functions/config_schema.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.35/cyberdrop_dl/base_functions/data_classes.py` & `cyberdrop-dl-4.2.36/cyberdrop_dl/base_functions/data_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.35/cyberdrop_dl/base_functions/error_classes.py` & `cyberdrop-dl-4.2.36/cyberdrop_dl/base_functions/error_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.35/cyberdrop_dl/base_functions/sorting_functions.py` & `cyberdrop-dl-4.2.36/cyberdrop_dl/base_functions/sorting_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.35/cyberdrop_dl/base_functions/sql_helper.py` & `cyberdrop-dl-4.2.36/cyberdrop_dl/base_functions/sql_helper.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.35/cyberdrop_dl/client/client.py` & `cyberdrop-dl-4.2.36/cyberdrop_dl/client/client.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.35/cyberdrop_dl/crawlers/Anonfiles_Spider.py` & `cyberdrop-dl-4.2.36/cyberdrop_dl/crawlers/Anonfiles_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.35/cyberdrop_dl/crawlers/Bunkr_Spider.py` & `cyberdrop-dl-4.2.36/cyberdrop_dl/crawlers/Bunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.35/cyberdrop_dl/crawlers/Coomeno_Spider.py` & `cyberdrop-dl-4.2.36/cyberdrop_dl/crawlers/Coomeno_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.35/cyberdrop_dl/crawlers/CyberFile_Spider.py` & `cyberdrop-dl-4.2.36/cyberdrop_dl/crawlers/CyberFile_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.35/cyberdrop_dl/crawlers/Cyberdrop_Spider.py` & `cyberdrop-dl-4.2.36/cyberdrop_dl/crawlers/Cyberdrop_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.35/cyberdrop_dl/crawlers/EHentai_Spider.py` & `cyberdrop-dl-4.2.36/cyberdrop_dl/crawlers/EHentai_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.35/cyberdrop_dl/crawlers/Erome_Spider.py` & `cyberdrop-dl-4.2.36/cyberdrop_dl/crawlers/Erome_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.35/cyberdrop_dl/crawlers/Fapello_Spider.py` & `cyberdrop-dl-4.2.36/cyberdrop_dl/crawlers/Fapello_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.35/cyberdrop_dl/crawlers/Gfycat_Spider.py` & `cyberdrop-dl-4.2.36/cyberdrop_dl/crawlers/Gfycat_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.35/cyberdrop_dl/crawlers/GoFile_Spider.py` & `cyberdrop-dl-4.2.36/cyberdrop_dl/crawlers/GoFile_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.35/cyberdrop_dl/crawlers/HGameCG_Spider.py` & `cyberdrop-dl-4.2.36/cyberdrop_dl/crawlers/HGameCG_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.35/cyberdrop_dl/crawlers/ImgBox_Spider.py` & `cyberdrop-dl-4.2.36/cyberdrop_dl/crawlers/ImgBox_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.35/cyberdrop_dl/crawlers/LoveFap_Spider.py` & `cyberdrop-dl-4.2.36/cyberdrop_dl/crawlers/LoveFap_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.35/cyberdrop_dl/crawlers/NSFWXXX_Spider.py` & `cyberdrop-dl-4.2.36/cyberdrop_dl/crawlers/NSFWXXX_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.35/cyberdrop_dl/crawlers/PimpAndHost_Spider.py` & `cyberdrop-dl-4.2.36/cyberdrop_dl/crawlers/PimpAndHost_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.35/cyberdrop_dl/crawlers/PixelDrain_Spider.py` & `cyberdrop-dl-4.2.36/cyberdrop_dl/crawlers/PixelDrain_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.35/cyberdrop_dl/crawlers/PostImg_Spider.py` & `cyberdrop-dl-4.2.36/cyberdrop_dl/crawlers/PostImg_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.35/cyberdrop_dl/crawlers/Saint_Spider.py` & `cyberdrop-dl-4.2.36/cyberdrop_dl/crawlers/Saint_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.35/cyberdrop_dl/crawlers/ShareX_Spider.py` & `cyberdrop-dl-4.2.36/cyberdrop_dl/crawlers/ShareX_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.35/cyberdrop_dl/crawlers/XBunkr_Spider.py` & `cyberdrop-dl-4.2.36/cyberdrop_dl/crawlers/XBunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.35/cyberdrop_dl/crawlers/Xenforo_Spider.py` & `cyberdrop-dl-4.2.36/cyberdrop_dl/crawlers/Xenforo_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.35/cyberdrop_dl/downloader/downloader_utils.py` & `cyberdrop-dl-4.2.36/cyberdrop_dl/downloader/downloader_utils.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.35/cyberdrop_dl/downloader/downloaders.py` & `cyberdrop-dl-4.2.36/cyberdrop_dl/downloader/downloaders.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.35/cyberdrop_dl/downloader/old_downloaders.py` & `cyberdrop-dl-4.2.36/cyberdrop_dl/downloader/old_downloaders.py`

 * *Files 2% similar despite different names*

```diff
@@ -265,23 +265,24 @@
             media.filename = downloaded_filename
             complete_file = (self.download_dir / album / media.filename)
             partial_file = complete_file.with_suffix(complete_file.suffix + '.part')
 
         return complete_file, partial_file, proceed
 
 
-async def old_download_forums(args: Dict, Forums: ForumItem, SQL_Helper: SQLHelper, client: Client) -> None:
+async def old_download_forums(args: Dict, Forums: ForumItem, SQL_Helper: SQLHelper, client: Client,
+                              error_writer: ErrorFileWriter) -> None:
     """Handler for forum threads and the progress bars for it"""
     total_files = await Forums.get_total()
     with tqdm(total=total_files, unit_scale=True, unit='Files', leave=True, initial=0,
               desc="Files Downloaded") as progress:
         files = Files(progress)
         for title, Cascade in Forums.threads.items():
             tasks = []
             for domain, domain_obj in Cascade.domains.items():
-                downloader = Old_Downloader(args, client, SQL_Helper, domain, domain_obj, files)
+                downloader = Old_Downloader(args, client, SQL_Helper, domain, domain_obj, files, error_writer)
                 tasks.append(downloader.start_domain())
             await asyncio.gather(*tasks)
 
     await clear()
     log(f"| [green]Files Complete: {files.completed_files}[/green] - [yellow]Files Skipped: "
               f"{files.skipped_files}[/yellow] - [red]Files Failed: {files.failed_files}[/red] |")
```

### Comparing `cyberdrop-dl-4.2.35/cyberdrop_dl/downloader/progress_definitions.py` & `cyberdrop-dl-4.2.36/cyberdrop_dl/downloader/progress_definitions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.35/cyberdrop_dl/main.py` & `cyberdrop-dl-4.2.36/cyberdrop_dl/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -257,15 +257,15 @@
     if links:
         Forums = await scrape_links(Scraper, links)
         await asyncio.sleep(5)
         await clear()
 
         if not await Forums.is_empty():
             if args['Progress_Options']['hide_new_progress']:
-                await old_download_forums(args, Forums, SQL_Helper, client)
+                await old_download_forums(args, Forums, SQL_Helper, client, error_writer)
             else:
                 download_director = DownloadDirector(args, Forums, SQL_Helper, client, error_writer)
                 await download_director.start()
 
     if args['Files']['output_folder'].is_dir():
         if args['Sorting']['sort_downloads']:
             log("")
```

### Comparing `cyberdrop-dl-4.2.35/cyberdrop_dl/scraper/JDownloader_Integration.py` & `cyberdrop-dl-4.2.36/cyberdrop_dl/scraper/JDownloader_Integration.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.35/cyberdrop_dl/scraper/Scraper.py` & `cyberdrop-dl-4.2.36/cyberdrop_dl/scraper/Scraper.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.35/cyberdrop_dl.egg-info/PKG-INFO` & `cyberdrop-dl-4.2.36/cyberdrop_dl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.2.35
+Version: 4.2.36
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.35 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.36 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
```

### Comparing `cyberdrop-dl-4.2.35/cyberdrop_dl.egg-info/SOURCES.txt` & `cyberdrop-dl-4.2.36/cyberdrop_dl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.35/setup.cfg` & `cyberdrop-dl-4.2.36/setup.cfg`

 * *Files identical despite different names*

