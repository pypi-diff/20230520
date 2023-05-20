# Comparing `tmp/arxiv-dl-1.1.2.tar.gz` & `tmp/arxiv-dl-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arxiv-dl-1.1.2.tar", last modified: Wed Jun  8 02:53:38 2022, max compression
+gzip compressed data, was "arxiv-dl-1.1.3.tar", last modified: Sat May 20 08:32:34 2023, max compression
```

## Comparing `arxiv-dl-1.1.2.tar` & `arxiv-dl-1.1.3.tar`

### file list

```diff
@@ -1,20 +1,28 @@
-drwxr-xr-x   0 markhuang   (501) staff       (20)        0 2022-06-08 02:53:38.723546 arxiv-dl-1.1.2/
--rw-r--r--   0 markhuang   (501) staff       (20)     1072 2022-01-31 07:24:42.000000 arxiv-dl-1.1.2/LICENSE
--rw-r--r--   0 markhuang   (501) staff       (20)     5383 2022-06-08 02:53:38.723422 arxiv-dl-1.1.2/PKG-INFO
--rw-r--r--   0 markhuang   (501) staff       (20)     4619 2022-06-08 02:46:14.000000 arxiv-dl-1.1.2/README.md
-drwxr-xr-x   0 markhuang   (501) staff       (20)        0 2022-06-08 02:53:38.722656 arxiv-dl-1.1.2/arxiv_dl/
--rw-r--r--   0 markhuang   (501) staff       (20)     4454 2022-06-08 02:42:38.000000 arxiv-dl-1.1.2/arxiv_dl/arxiv_dl.py
-drwxr-xr-x   0 markhuang   (501) staff       (20)        0 2022-06-08 02:53:38.723260 arxiv-dl-1.1.2/arxiv_dl/bin/
--rwxr-xr-x   0 markhuang   (501) staff       (20)      973 2022-06-08 02:42:24.000000 arxiv-dl-1.1.2/arxiv_dl/bin/getpaper
--rw-r--r--   0 markhuang   (501) staff       (20)    16176 2022-06-08 02:38:02.000000 arxiv-dl-1.1.2/arxiv_dl/helpers.py
--rw-r--r--   0 markhuang   (501) staff       (20)      617 2022-05-31 11:29:42.000000 arxiv-dl-1.1.2/arxiv_dl/logger.py
--rw-r--r--   0 markhuang   (501) staff       (20)      654 2022-06-01 15:07:20.000000 arxiv-dl-1.1.2/arxiv_dl/models.py
--rw-r--r--   0 markhuang   (501) staff       (20)     4964 2022-06-08 02:34:25.000000 arxiv-dl-1.1.2/arxiv_dl/scrapers.py
-drwxr-xr-x   0 markhuang   (501) staff       (20)        0 2022-06-08 02:53:38.723134 arxiv-dl-1.1.2/arxiv_dl.egg-info/
--rw-r--r--   0 markhuang   (501) staff       (20)     5383 2022-06-08 02:53:38.000000 arxiv-dl-1.1.2/arxiv_dl.egg-info/PKG-INFO
--rw-r--r--   0 markhuang   (501) staff       (20)      307 2022-06-08 02:53:38.000000 arxiv-dl-1.1.2/arxiv_dl.egg-info/SOURCES.txt
--rw-r--r--   0 markhuang   (501) staff       (20)        1 2022-06-08 02:53:38.000000 arxiv-dl-1.1.2/arxiv_dl.egg-info/dependency_links.txt
--rw-r--r--   0 markhuang   (501) staff       (20)       94 2022-06-08 02:53:38.000000 arxiv-dl-1.1.2/arxiv_dl.egg-info/requires.txt
--rw-r--r--   0 markhuang   (501) staff       (20)        9 2022-06-08 02:53:38.000000 arxiv-dl-1.1.2/arxiv_dl.egg-info/top_level.txt
--rw-r--r--   0 markhuang   (501) staff       (20)       38 2022-06-08 02:53:38.723584 arxiv-dl-1.1.2/setup.cfg
--rw-r--r--   0 markhuang   (501) staff       (20)     1417 2022-06-08 02:53:28.000000 arxiv-dl-1.1.2/setup.py
+drwxr-xr-x   0 markhuang   (501) staff       (20)        0 2023-05-20 08:32:34.559983 arxiv-dl-1.1.3/
+-rw-r--r--   0 markhuang   (501) staff       (20)     1075 2023-05-20 08:32:15.000000 arxiv-dl-1.1.3/LICENSE
+-rw-r--r--   0 markhuang   (501) staff       (20)     5441 2023-05-20 08:32:34.559849 arxiv-dl-1.1.3/PKG-INFO
+-rw-r--r--   0 markhuang   (501) staff       (20)     4677 2023-05-20 08:31:03.000000 arxiv-dl-1.1.3/README.md
+drwxr-xr-x   0 markhuang   (501) staff       (20)        0 2023-05-20 08:32:34.558147 arxiv-dl-1.1.3/arxiv_dl/
+-rw-r--r--   0 markhuang   (501) staff       (20)     4517 2023-05-20 07:41:48.000000 arxiv-dl-1.1.3/arxiv_dl/arxiv_dl.py
+drwxr-xr-x   0 markhuang   (501) staff       (20)        0 2023-05-20 08:32:34.559074 arxiv-dl-1.1.3/arxiv_dl/bin/
+-rwxr-xr-x   0 markhuang   (501) staff       (20)     1130 2023-05-20 07:41:48.000000 arxiv-dl-1.1.3/arxiv_dl/bin/arxiv-dl
+-rwxr-xr-x   0 markhuang   (501) staff       (20)     1130 2023-05-20 07:41:48.000000 arxiv-dl-1.1.3/arxiv_dl/bin/getpaper
+-rwxr-xr-x   0 markhuang   (501) staff       (20)     1130 2023-05-20 07:41:48.000000 arxiv-dl-1.1.3/arxiv_dl/bin/paper
+-rw-r--r--   0 markhuang   (501) staff       (20)    20000 2023-05-20 07:41:48.000000 arxiv-dl-1.1.3/arxiv_dl/dl_utils.py
+-rw-r--r--   0 markhuang   (501) staff       (20)    16052 2023-05-20 07:41:48.000000 arxiv-dl-1.1.3/arxiv_dl/helpers.py
+-rw-r--r--   0 markhuang   (501) staff       (20)      617 2022-05-31 11:29:42.000000 arxiv-dl-1.1.3/arxiv_dl/logger.py
+-rw-r--r--   0 markhuang   (501) staff       (20)      654 2022-06-01 15:07:20.000000 arxiv-dl-1.1.3/arxiv_dl/models.py
+-rw-r--r--   0 markhuang   (501) staff       (20)     4970 2023-05-20 07:41:48.000000 arxiv-dl-1.1.3/arxiv_dl/scrapers.py
+drwxr-xr-x   0 markhuang   (501) staff       (20)        0 2023-05-20 08:32:34.558733 arxiv-dl-1.1.3/arxiv_dl.egg-info/
+-rw-r--r--   0 markhuang   (501) staff       (20)     5441 2023-05-20 08:32:34.000000 arxiv-dl-1.1.3/arxiv_dl.egg-info/PKG-INFO
+-rw-r--r--   0 markhuang   (501) staff       (20)      478 2023-05-20 08:32:34.000000 arxiv-dl-1.1.3/arxiv_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 markhuang   (501) staff       (20)        1 2023-05-20 08:32:34.000000 arxiv-dl-1.1.3/arxiv_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 markhuang   (501) staff       (20)       94 2023-05-20 08:32:34.000000 arxiv-dl-1.1.3/arxiv_dl.egg-info/requires.txt
+-rw-r--r--   0 markhuang   (501) staff       (20)        9 2023-05-20 08:32:34.000000 arxiv-dl-1.1.3/arxiv_dl.egg-info/top_level.txt
+-rw-r--r--   0 markhuang   (501) staff       (20)       38 2023-05-20 08:32:34.560022 arxiv-dl-1.1.3/setup.cfg
+-rw-r--r--   0 markhuang   (501) staff       (20)     1626 2023-05-20 08:31:17.000000 arxiv-dl-1.1.3/setup.py
+drwxr-xr-x   0 markhuang   (501) staff       (20)        0 2023-05-20 08:32:34.559544 arxiv-dl-1.1.3/tests/
+-rw-r--r--   0 markhuang   (501) staff       (20)     2261 2022-03-12 13:41:52.000000 arxiv-dl-1.1.3/tests/test_arxiv_id_validator.py
+-rw-r--r--   0 markhuang   (501) staff       (20)     1354 2022-06-01 15:07:20.000000 arxiv-dl-1.1.3/tests/test_cli.py
+-rw-r--r--   0 markhuang   (501) staff       (20)    39773 2023-05-18 05:56:12.000000 arxiv-dl-1.1.3/tests/test_process_cvf_target.py
+-rw-r--r--   0 markhuang   (501) staff       (20)    15214 2023-05-18 05:57:07.000000 arxiv-dl-1.1.3/tests/test_scrape_cvf.py
```

### Comparing `arxiv-dl-1.1.2/LICENSE` & `arxiv-dl-1.1.3/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021-2022 Mark Huang
+Copyright (c) 2021-2023 Mark He Huang
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `arxiv-dl-1.1.2/PKG-INFO` & `arxiv-dl-1.1.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arxiv-dl
-Version: 1.1.2
+Version: 1.1.3
 Summary: Command-line arXiv Papers Downloader. Citation extraction and PDF naming automation.
 Home-page: https://github.com/MarkHershey/arxiv-dl
 Author: Mark He Huang
 Author-email: dev@markhh.com
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -30,80 +30,78 @@
 [![](https://img.shields.io/pypi/wheel/arxiv-dl)](https://github.com/MarkHershey/arxiv-dl/releases)
 [![](https://img.shields.io/pypi/dm/Arxiv-dl)](https://pypistats.org/packages/arxiv-dl)
 [![](https://img.shields.io/badge/license-MIT-blue)](https://github.com/MarkHershey/arxiv-dl/blob/master/LICENSE)
 [![](https://img.shields.io/badge/code%20style-black-black)](https://github.com/psf/black)
 
 _Disclaimer: This is a highly-opinionated CLI tool for downloading papers. It priorities ease of use for researchers. Obviously, this is not an official project._
 
-## Features
+## What does it do?
 
--   Download papers from via simple command line interface.
--   Support papers from [ArXiv](https://arxiv.org/) and [CVPR, ICCV, WACV](https://openaccess.thecvf.com/menu).
+-   Support downloading papers from [ArXiv](https://arxiv.org/), [CVPR, ICCV, WACV](https://openaccess.thecvf.com/menu) via simple CLI.
 -   Support downloading speedup by using [aria2c](https://aria2.github.io/).
--   Automatically maintain a local list of downloaded papers.
--   Retrieve the paper's metadata and citation:
-    -   Paper Title
+-   Retrieve the paper's metadata such as:
+    -   Title, Abstract, Year
     -   Authors
-    -   Abstract
     -   Comments (Conference acceptance info)
-    -   Source Code Links
-    -   Citation (`BibTeX`)
--   Configure the desired download destination via environment variables.
--   All downloaded papers will be named by its arXiv ID and paper title without whitespace.
-
-### Why?
-
--   Save time and effort to download, rename, and organize papers.
--   Speedup downloading process by using parallel connections.
--   Local paper list would be handy for quick local lookup, locate, and cite papers.
+    -   Repository URLs
+    -   `BibTeX` Citation
+-   Automatically maintain a list of local papers and their metadata in a JSON file.
+-   Configure the desired download destination via an environment variable or a command-line argument.
+-   All downloaded papers will have standardized filename for easy browsing.
+
+## Why?
+
+-   Save time and effort to download and organize papers on your machine.
+-   Speedup downloading process by using multiple parallel connections.
+-   Local paper list would be handy for quick local lookup, making notes, and doing citations.
 
-## Install
+## How to install it?
 
 This is a command-line tool, use `pip` to install the package globally.
 
 -   Pre-requisite: `Python 3.x`
 
 ```bash
 python3 -m pip install --upgrade arxiv-dl
 ```
 
 (Optional) Install [aria2c](https://aria2.github.io/) for download speedup.
 
 -   MacOS: `brew install aria2`
 -   Linux: `sudo snap install aria2c`
 
-## Usage
+## How to use it?
 
-After installation, the command `getpaper` should be available in your terminal.
+After installation, three equivalent commands `arxiv-dl`, `getpaper`, `paper` should be available in your terminal.
 
 ```bash
-$ getpaper [-h] [-v] [-p] [-d DOWNLOAD_DIR] [-n N_THREADS] urls [urls ...]
+$ paper [-h] [-v] [-p] [-d DOWNLOAD_DIR] [-n N_THREADS] urls [urls ...]
 ```
 
 Options:
 
 -   `-v`, `--verbose` (optional): Print paper metadata.
 -   `-p`, `--pdf_only` (optional): Download PDF only without creating Markdown notes
 -   `-d`, `--download_dir` (optional): Specify one-time download directory. This option will override the default download directory or the one specified in the environment variable `ARXIV_DOWNLOAD_FOLDER`.
 -   `-n`, `--n_threads` (optional): Specify the number of parallel connections to be used by `aria2`.
 
 ### Usage Examples:
 
 ```bash
 # Use ArXiv Paper ID
-$ getpaper 1512.03385 2103.15538
+$ paper 1512.03385 2103.15538
 
 # Use ArXiv Abstract Page URL
-$ getpaper https://arxiv.org/abs/2103.15538
+$ paper https://arxiv.org/abs/2103.15538
 
 # Use ArXiv PDF Page URL
-$ getpaper https://arxiv.org/pdf/1512.03385.pdf
+$ paper https://arxiv.org/pdf/1512.03385.pdf
 
 # Use CVF Open Access URL
-$ getpaper "https://openaccess.thecvf.com/content/CVPR2021/html/Lin_Real-Time_High-Resolution_Background_Matting_CVPR_2021_paper.html"
+$ paper "https://openaccess.thecvf.com/content/CVPR2021/html/Lin_Real-Time_High-Resolution_Background_Matting_CVPR_2021_paper.html"
 ```
 
 ![](imgs/demo.png)
 
 ## Configurations
 
 ### Set Custom Download Destination _(Optional)_
```

### Comparing `arxiv-dl-1.1.2/README.md` & `arxiv-dl-1.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -9,80 +9,78 @@
 [![](https://img.shields.io/pypi/wheel/arxiv-dl)](https://github.com/MarkHershey/arxiv-dl/releases)
 [![](https://img.shields.io/pypi/dm/Arxiv-dl)](https://pypistats.org/packages/arxiv-dl)
 [![](https://img.shields.io/badge/license-MIT-blue)](https://github.com/MarkHershey/arxiv-dl/blob/master/LICENSE)
 [![](https://img.shields.io/badge/code%20style-black-black)](https://github.com/psf/black)
 
 _Disclaimer: This is a highly-opinionated CLI tool for downloading papers. It priorities ease of use for researchers. Obviously, this is not an official project._
 
-## Features
+## What does it do?
 
--   Download papers from via simple command line interface.
--   Support papers from [ArXiv](https://arxiv.org/) and [CVPR, ICCV, WACV](https://openaccess.thecvf.com/menu).
+-   Support downloading papers from [ArXiv](https://arxiv.org/), [CVPR, ICCV, WACV](https://openaccess.thecvf.com/menu) via simple CLI.
 -   Support downloading speedup by using [aria2c](https://aria2.github.io/).
--   Automatically maintain a local list of downloaded papers.
--   Retrieve the paper's metadata and citation:
-    -   Paper Title
+-   Retrieve the paper's metadata such as:
+    -   Title, Abstract, Year
     -   Authors
-    -   Abstract
     -   Comments (Conference acceptance info)
-    -   Source Code Links
-    -   Citation (`BibTeX`)
--   Configure the desired download destination via environment variables.
--   All downloaded papers will be named by its arXiv ID and paper title without whitespace.
-
-### Why?
-
--   Save time and effort to download, rename, and organize papers.
--   Speedup downloading process by using parallel connections.
--   Local paper list would be handy for quick local lookup, locate, and cite papers.
+    -   Repository URLs
+    -   `BibTeX` Citation
+-   Automatically maintain a list of local papers and their metadata in a JSON file.
+-   Configure the desired download destination via an environment variable or a command-line argument.
+-   All downloaded papers will have standardized filename for easy browsing.
+
+## Why?
+
+-   Save time and effort to download and organize papers on your machine.
+-   Speedup downloading process by using multiple parallel connections.
+-   Local paper list would be handy for quick local lookup, making notes, and doing citations.
 
-## Install
+## How to install it?
 
 This is a command-line tool, use `pip` to install the package globally.
 
 -   Pre-requisite: `Python 3.x`
 
 ```bash
 python3 -m pip install --upgrade arxiv-dl
 ```
 
 (Optional) Install [aria2c](https://aria2.github.io/) for download speedup.
 
 -   MacOS: `brew install aria2`
 -   Linux: `sudo snap install aria2c`
 
-## Usage
+## How to use it?
 
-After installation, the command `getpaper` should be available in your terminal.
+After installation, three equivalent commands `arxiv-dl`, `getpaper`, `paper` should be available in your terminal.
 
 ```bash
-$ getpaper [-h] [-v] [-p] [-d DOWNLOAD_DIR] [-n N_THREADS] urls [urls ...]
+$ paper [-h] [-v] [-p] [-d DOWNLOAD_DIR] [-n N_THREADS] urls [urls ...]
 ```
 
 Options:
 
 -   `-v`, `--verbose` (optional): Print paper metadata.
 -   `-p`, `--pdf_only` (optional): Download PDF only without creating Markdown notes
 -   `-d`, `--download_dir` (optional): Specify one-time download directory. This option will override the default download directory or the one specified in the environment variable `ARXIV_DOWNLOAD_FOLDER`.
 -   `-n`, `--n_threads` (optional): Specify the number of parallel connections to be used by `aria2`.
 
 ### Usage Examples:
 
 ```bash
 # Use ArXiv Paper ID
-$ getpaper 1512.03385 2103.15538
+$ paper 1512.03385 2103.15538
 
 # Use ArXiv Abstract Page URL
-$ getpaper https://arxiv.org/abs/2103.15538
+$ paper https://arxiv.org/abs/2103.15538
 
 # Use ArXiv PDF Page URL
-$ getpaper https://arxiv.org/pdf/1512.03385.pdf
+$ paper https://arxiv.org/pdf/1512.03385.pdf
 
 # Use CVF Open Access URL
-$ getpaper "https://openaccess.thecvf.com/content/CVPR2021/html/Lin_Real-Time_High-Resolution_Background_Matting_CVPR_2021_paper.html"
+$ paper "https://openaccess.thecvf.com/content/CVPR2021/html/Lin_Real-Time_High-Resolution_Background_Matting_CVPR_2021_paper.html"
 ```
 
 ![](imgs/demo.png)
 
 ## Configurations
 
 ### Set Custom Download Destination _(Optional)_
```

### Comparing `arxiv-dl-1.1.2/arxiv_dl/arxiv_dl.py` & `arxiv-dl-1.1.3/arxiv_dl/arxiv_dl.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,15 +55,17 @@
         logger.error("[Abort] Target is not specified correctly")
         return False
 
     if (
         not target.startswith(("http://", "https://", "www."))
         and not target[0].isdigit()
     ):
-        logger.error(f"[Abort] Unknown target: {target}")
+        logger.error(
+            f"[Abort] Target should be a URL or an ArXiv ID. Unknown target: '{target}'"
+        )
         return False
 
     ### Identify Paper Source/Venues
     if target[0].isdigit() or "arxiv.org" in target:
         # assume target is an ArXiv ID
         paper_data: PaperData = process_arxiv_target(target)
     elif "openaccess.thecvf.com" in target:  # assume target is a CVF URL
```

### Comparing `arxiv-dl-1.1.2/arxiv_dl/helpers.py` & `arxiv-dl-1.1.3/arxiv_dl/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 import re
 import shlex
 import string
 import subprocess
 from pathlib import Path
 from typing import Union
 
-import requests
-
+from .dl_utils import download
 from .logger import logger
 from .models import PaperData
 
 DEFAULT_DOWNLOAD_PATH = Path.home() / "Downloads/ArXiv_Papers"
 
 
 ###########################################################################
@@ -105,19 +104,15 @@
     """
     download_dir = Path(download_dir)
     assert download_dir.is_dir(), "Download directory does not exist."
     download_path: Path = download_dir / download_name
     assert download_path.is_file() is False, "File already exists"
 
     logger.debug("[Downloading] Using HTTP")
-    logger.setLevel(logging.WARNING)
-    response = requests.get(url)
-    with download_path.open(mode="wb") as f:
-        f.write(response.content)
-    logger.setLevel(logging.DEBUG)
+    download(url=url, out=str(download_path))
     return download_path
 
 
 def aria2_download(
     url: str,
     download_dir: Union[str, Path],
     download_name: str,
```

### Comparing `arxiv-dl-1.1.2/arxiv_dl/logger.py` & `arxiv-dl-1.1.3/arxiv_dl/logger.py`

 * *Files identical despite different names*

### Comparing `arxiv-dl-1.1.2/arxiv_dl/models.py` & `arxiv-dl-1.1.3/arxiv_dl/models.py`

 * *Files identical despite different names*

### Comparing `arxiv-dl-1.1.2/arxiv_dl/scrapers.py` & `arxiv-dl-1.1.3/arxiv_dl/scrapers.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from .helpers import normalize_paper_title
 from .logger import logger
 from .models import PaperData
 
 
 def scrape_metadata_arxiv(paper_data: PaperData) -> None:
     logger.setLevel(logging.DEBUG)
-    logger.debug("[Processing] Retrieving paper metadata")
+    logger.debug("[Processing] Retrieving paper metadata...")
     logger.setLevel(logging.WARNING)
 
     response = requests.get(paper_data.abs_url)
     if response.status_code != 200:
         logger.error(f"Cannot connect to {paper_data.abs_url}")
         raise Exception(f"Cannot connect to {paper_data.abs_url}")
     # make soup
@@ -83,15 +83,15 @@
     )
 
     return None
 
 
 def scrape_metadata_cvf(paper_data: PaperData) -> None:
     logger.setLevel(logging.DEBUG)
-    logger.debug("[Processing] Retrieving paper metadata from CVF")
+    logger.debug("[Processing] Retrieving paper metadata from CVF...")
     logger.setLevel(logging.WARNING)
 
     response = requests.get(paper_data.abs_url)
     if response.status_code != 200:
         logger.error(f"Cannot connect to {paper_data.abs_url}")
         raise Exception(f"Cannot connect to {paper_data.abs_url}")
     # make soup
```

### Comparing `arxiv-dl-1.1.2/arxiv_dl.egg-info/PKG-INFO` & `arxiv-dl-1.1.3/arxiv_dl.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arxiv-dl
-Version: 1.1.2
+Version: 1.1.3
 Summary: Command-line arXiv Papers Downloader. Citation extraction and PDF naming automation.
 Home-page: https://github.com/MarkHershey/arxiv-dl
 Author: Mark He Huang
 Author-email: dev@markhh.com
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -30,80 +30,78 @@
 [![](https://img.shields.io/pypi/wheel/arxiv-dl)](https://github.com/MarkHershey/arxiv-dl/releases)
 [![](https://img.shields.io/pypi/dm/Arxiv-dl)](https://pypistats.org/packages/arxiv-dl)
 [![](https://img.shields.io/badge/license-MIT-blue)](https://github.com/MarkHershey/arxiv-dl/blob/master/LICENSE)
 [![](https://img.shields.io/badge/code%20style-black-black)](https://github.com/psf/black)
 
 _Disclaimer: This is a highly-opinionated CLI tool for downloading papers. It priorities ease of use for researchers. Obviously, this is not an official project._
 
-## Features
+## What does it do?
 
--   Download papers from via simple command line interface.
--   Support papers from [ArXiv](https://arxiv.org/) and [CVPR, ICCV, WACV](https://openaccess.thecvf.com/menu).
+-   Support downloading papers from [ArXiv](https://arxiv.org/), [CVPR, ICCV, WACV](https://openaccess.thecvf.com/menu) via simple CLI.
 -   Support downloading speedup by using [aria2c](https://aria2.github.io/).
--   Automatically maintain a local list of downloaded papers.
--   Retrieve the paper's metadata and citation:
-    -   Paper Title
+-   Retrieve the paper's metadata such as:
+    -   Title, Abstract, Year
     -   Authors
-    -   Abstract
     -   Comments (Conference acceptance info)
-    -   Source Code Links
-    -   Citation (`BibTeX`)
--   Configure the desired download destination via environment variables.
--   All downloaded papers will be named by its arXiv ID and paper title without whitespace.
-
-### Why?
-
--   Save time and effort to download, rename, and organize papers.
--   Speedup downloading process by using parallel connections.
--   Local paper list would be handy for quick local lookup, locate, and cite papers.
+    -   Repository URLs
+    -   `BibTeX` Citation
+-   Automatically maintain a list of local papers and their metadata in a JSON file.
+-   Configure the desired download destination via an environment variable or a command-line argument.
+-   All downloaded papers will have standardized filename for easy browsing.
+
+## Why?
+
+-   Save time and effort to download and organize papers on your machine.
+-   Speedup downloading process by using multiple parallel connections.
+-   Local paper list would be handy for quick local lookup, making notes, and doing citations.
 
-## Install
+## How to install it?
 
 This is a command-line tool, use `pip` to install the package globally.
 
 -   Pre-requisite: `Python 3.x`
 
 ```bash
 python3 -m pip install --upgrade arxiv-dl
 ```
 
 (Optional) Install [aria2c](https://aria2.github.io/) for download speedup.
 
 -   MacOS: `brew install aria2`
 -   Linux: `sudo snap install aria2c`
 
-## Usage
+## How to use it?
 
-After installation, the command `getpaper` should be available in your terminal.
+After installation, three equivalent commands `arxiv-dl`, `getpaper`, `paper` should be available in your terminal.
 
 ```bash
-$ getpaper [-h] [-v] [-p] [-d DOWNLOAD_DIR] [-n N_THREADS] urls [urls ...]
+$ paper [-h] [-v] [-p] [-d DOWNLOAD_DIR] [-n N_THREADS] urls [urls ...]
 ```
 
 Options:
 
 -   `-v`, `--verbose` (optional): Print paper metadata.
 -   `-p`, `--pdf_only` (optional): Download PDF only without creating Markdown notes
 -   `-d`, `--download_dir` (optional): Specify one-time download directory. This option will override the default download directory or the one specified in the environment variable `ARXIV_DOWNLOAD_FOLDER`.
 -   `-n`, `--n_threads` (optional): Specify the number of parallel connections to be used by `aria2`.
 
 ### Usage Examples:
 
 ```bash
 # Use ArXiv Paper ID
-$ getpaper 1512.03385 2103.15538
+$ paper 1512.03385 2103.15538
 
 # Use ArXiv Abstract Page URL
-$ getpaper https://arxiv.org/abs/2103.15538
+$ paper https://arxiv.org/abs/2103.15538
 
 # Use ArXiv PDF Page URL
-$ getpaper https://arxiv.org/pdf/1512.03385.pdf
+$ paper https://arxiv.org/pdf/1512.03385.pdf
 
 # Use CVF Open Access URL
-$ getpaper "https://openaccess.thecvf.com/content/CVPR2021/html/Lin_Real-Time_High-Resolution_Background_Matting_CVPR_2021_paper.html"
+$ paper "https://openaccess.thecvf.com/content/CVPR2021/html/Lin_Real-Time_High-Resolution_Background_Matting_CVPR_2021_paper.html"
 ```
 
 ![](imgs/demo.png)
 
 ## Configurations
 
 ### Set Custom Download Destination _(Optional)_
```

### Comparing `arxiv-dl-1.1.2/setup.py` & `arxiv-dl-1.1.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,40 @@
 from setuptools import find_namespace_packages, setup
 
 MAJOR = 1
 MINOR = 1
-MICRO = 2
+MICRO = 3
 VERSION = "%d.%d.%d" % (MAJOR, MINOR, MICRO)
 
+
+def update_version_file():
+    VERSION_FILE = "VERSION"
+    with open(VERSION_FILE, "w") as f:
+        f.write(VERSION)
+
+
+update_version_file()
+
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="arxiv-dl",
     version=VERSION,
     author="Mark He Huang",
     author_email="dev@markhh.com",
     description="Command-line arXiv Papers Downloader. Citation extraction and PDF naming automation.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/MarkHershey/arxiv-dl",
     packages=find_namespace_packages(include=["arxiv_dl"]),
     scripts=[
+        "arxiv_dl/bin/arxiv-dl",
         "arxiv_dl/bin/getpaper",
+        "arxiv_dl/bin/paper",
     ],
     install_requires=[
         "colorlog>=4.1.0",
         "requests",
         "pydantic",
         "beautifulsoup4",
     ],
```

