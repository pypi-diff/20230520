# Comparing `tmp/mathtranslate-2.3.0.tar.gz` & `tmp/mathtranslate-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathtranslate-2.3.0.tar", last modified: Fri May 19 00:38:12 2023, max compression
+gzip compressed data, was "mathtranslate-2.3.1.tar", last modified: Sat May 20 06:50:08 2023, max compression
```

## Comparing `mathtranslate-2.3.0.tar` & `mathtranslate-2.3.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:38:12.796152 mathtranslate-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-05-19 00:38:12.796152 mathtranslate-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:38:12.792152 mathtranslate-2.3.0/mathtranslate/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/process_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    16148 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/process_latex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/process_text.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/tencent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:38:12.796152 mathtranslate-2.3.0/mathtranslate/tencentcloud/
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/tencentcloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:38:12.796152 mathtranslate-2.3.0/mathtranslate/tencentcloud/common/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/tencentcloud/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18688 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/tencentcloud/common/abstract_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/tencentcloud/common/abstract_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/tencentcloud/common/common_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15693 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/tencentcloud/common/credential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:38:12.796152 mathtranslate-2.3.0/mathtranslate/tencentcloud/common/exception/
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/tencentcloud/common/exception/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/tencentcloud/common/exception/tencent_cloud_sdk_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:38:12.796152 mathtranslate-2.3.0/mathtranslate/tencentcloud/common/http/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/tencentcloud/common/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/tencentcloud/common/http/request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:38:12.796152 mathtranslate-2.3.0/mathtranslate/tencentcloud/common/profile/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/tencentcloud/common/profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/tencentcloud/common/profile/client_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/tencentcloud/common/profile/http_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/tencentcloud/common/sign.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:38:12.796152 mathtranslate-2.3.0/mathtranslate/tencentcloud/tmt/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/tencentcloud/tmt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:38:12.796152 mathtranslate-2.3.0/mathtranslate/tencentcloud/tmt/v20180321/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/tencentcloud/tmt/v20180321/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/tencentcloud/tmt/v20180321/errorcodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    33836 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/tencentcloud/tmt/v20180321/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     9432 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/tencentcloud/tmt/v20180321/tmt_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/translate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/translate_arxiv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/translate_tex.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/upload_overleaf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/mathtranslate/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:38:12.796152 mathtranslate-2.3.0/mathtranslate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-05-19 00:38:12.000000 mathtranslate-2.3.0/mathtranslate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-19 00:38:12.000000 mathtranslate-2.3.0/mathtranslate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 00:38:12.000000 mathtranslate-2.3.0/mathtranslate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-19 00:38:12.000000 mathtranslate-2.3.0/mathtranslate.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-19 00:38:12.000000 mathtranslate-2.3.0/mathtranslate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-19 00:38:12.000000 mathtranslate-2.3.0/mathtranslate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 00:38:12.796152 mathtranslate-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-19 00:37:51.000000 mathtranslate-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:50:08.353432 mathtranslate-2.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-05-20 06:50:08.353432 mathtranslate-2.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:50:08.353432 mathtranslate-2.3.1/mathtranslate/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/process_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16148 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/process_latex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/process_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/tencent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:50:08.353432 mathtranslate-2.3.1/mathtranslate/tencentcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/tencentcloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:50:08.353432 mathtranslate-2.3.1/mathtranslate/tencentcloud/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/tencentcloud/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18688 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/tencentcloud/common/abstract_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/tencentcloud/common/abstract_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/tencentcloud/common/common_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15693 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/tencentcloud/common/credential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:50:08.353432 mathtranslate-2.3.1/mathtranslate/tencentcloud/common/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/tencentcloud/common/exception/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/tencentcloud/common/exception/tencent_cloud_sdk_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:50:08.353432 mathtranslate-2.3.1/mathtranslate/tencentcloud/common/http/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/tencentcloud/common/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/tencentcloud/common/http/request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:50:08.353432 mathtranslate-2.3.1/mathtranslate/tencentcloud/common/profile/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/tencentcloud/common/profile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/tencentcloud/common/profile/client_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/tencentcloud/common/profile/http_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/tencentcloud/common/sign.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:50:08.353432 mathtranslate-2.3.1/mathtranslate/tencentcloud/tmt/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/tencentcloud/tmt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:50:08.353432 mathtranslate-2.3.1/mathtranslate/tencentcloud/tmt/v20180321/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/tencentcloud/tmt/v20180321/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/tencentcloud/tmt/v20180321/errorcodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33836 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/tencentcloud/tmt/v20180321/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9432 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/tencentcloud/tmt/v20180321/tmt_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/translate_arxiv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/translate_tex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/upload_overleaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:50:08.353432 mathtranslate-2.3.1/mathtranslate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-05-20 06:50:08.000000 mathtranslate-2.3.1/mathtranslate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-20 06:50:08.000000 mathtranslate-2.3.1/mathtranslate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 06:50:08.000000 mathtranslate-2.3.1/mathtranslate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-20 06:50:08.000000 mathtranslate-2.3.1/mathtranslate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-20 06:50:08.000000 mathtranslate-2.3.1/mathtranslate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-20 06:50:08.000000 mathtranslate-2.3.1/mathtranslate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 06:50:08.353432 mathtranslate-2.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/setup.py
```

### Comparing `mathtranslate-2.3.0/LICENSE` & `mathtranslate-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.0/PKG-INFO` & `mathtranslate-2.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathtranslate
-Version: 2.3.0
+Version: 2.3.1
 Summary: Translate math-heavy papers
 Home-page: https://github.com/SUSYUSTC/MathTranslate
 Author: MathTranslate developers
 Author-email: susyustc@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -74,18 +74,14 @@
    - To translate an arxiv project: `translate_arxiv 2205.15510` will generate a translated tex project `2205.15510.zip`.
 4. Compile your tex file. For a single file, you can use the command `xelatex output.tex` from [texlive](https://www.tug.org/texlive/). Chinese translation requires the xeCJK package. For arxiv projects, we recommend uploading the obtained .zip file to overleaf for online compilation (New Project - Upload Project). **Note that you need to set the compiler to XeLatex in `Menu - Compiler`.**
 5. You can change the default settings of translation language and engine through command line arguments `-engine`, `-from`, `-to`. For example, `translate_tex -engine tencent input.tex -o output.tex`. You can also permanently change the settings through `translate_tex --setdefault`. You can view more details through `translate_tex --help`. `translate_arxiv` also provides exactly the same command line arguments, which have the same effect.
 
 ## Examples
 In the example directory, you can see `main.txt` which is the mathpix output of a part of `paper.pdf`. Run `translate_tex main.txt` and you will get the `main.tex` and `main.pdf`. `translated.png` is what you should expect to see in the `main.pdf`.
 
-## Known Issues
-1. If `\begin{env} \end{env}` is reset with `\newcommand` in latex, it will not be translated correctly.
-2. There is a small probability to get something like "XMATHX_1_2" or wrong formula during translation. The accuracy rate of Tencent translation is slightly lower than that of Google translation.
-
 ## Further developments
 1. Fix bugs in the latex translations.
 2. A more user-friendly interface.
 
 If you have any questions or have interests in making contributions, please contact me by susyustc@gmail.com or joining QQ group 288646946.
 
 ## Donation
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mathtranslate Version: 2.3.0 Summary: Translate
+Metadata-Version: 2.1 Name: mathtranslate Version: 2.3.1 Summary: Translate
 math-heavy papers Home-page: https://github.com/SUSYUSTC/MathTranslate Author:
 MathTranslate developers Author-email: susyustc@gmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: OS
 Independent Description-Content-Type: text/markdown License-File: LICENSE #
 MathTranslate
      [https://img.shields.io/pypi/v/mathtranslate.svg?logo=pypi]  [https://
        img.shields.io/badge/license-Apache%202.0-yellow.svg?logo=apache]
@@ -55,19 +55,15 @@
 from`, `-to`. For example, `translate_tex -engine tencent input.tex -
 o output.tex`. You can also permanently change the settings through
 `translate_tex --setdefault`. You can view more details through `translate_tex
 --help`. `translate_arxiv` also provides exactly the same command line
 arguments, which have the same effect. ## Examples In the example directory,
 you can see `main.txt` which is the mathpix output of a part of `paper.pdf`.
 Run `translate_tex main.txt` and you will get the `main.tex` and `main.pdf`.
-`translated.png` is what you should expect to see in the `main.pdf`. ## Known
-Issues 1. If `\begin{env} \end{env}` is reset with `\newcommand` in latex, it
-will not be translated correctly. 2. There is a small probability to get
-something like "XMATHX_1_2" or wrong formula during translation. The accuracy
-rate of Tencent translation is slightly lower than that of Google translation.
-## Further developments 1. Fix bugs in the latex translations. 2. A more user-
-friendly interface. If you have any questions or have interests in making
-contributions, please contact me by susyustc@gmail.com or joining QQ group
-288646946. ## Donation If you think this project is helping you a lot, you can
-support us by the Wechat QR code below
+`translated.png` is what you should expect to see in the `main.pdf`. ## Further
+developments 1. Fix bugs in the latex translations. 2. A more user-friendly
+interface. If you have any questions or have interests in making contributions,
+please contact me by susyustc@gmail.com or joining QQ group 288646946. ##
+Donation If you think this project is helping you a lot, you can support us by
+the Wechat QR code below
 [https://github.com/SUSYUSTC/MathTranslate/assets/30529122/16f82637-e102-4330-
                               82ad-bbcbdad1c19d]
```

### Comparing `mathtranslate-2.3.0/README.md` & `mathtranslate-2.3.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -62,18 +62,14 @@
    - To translate an arxiv project: `translate_arxiv 2205.15510` will generate a translated tex project `2205.15510.zip`.
 4. Compile your tex file. For a single file, you can use the command `xelatex output.tex` from [texlive](https://www.tug.org/texlive/). Chinese translation requires the xeCJK package. For arxiv projects, we recommend uploading the obtained .zip file to overleaf for online compilation (New Project - Upload Project). **Note that you need to set the compiler to XeLatex in `Menu - Compiler`.**
 5. You can change the default settings of translation language and engine through command line arguments `-engine`, `-from`, `-to`. For example, `translate_tex -engine tencent input.tex -o output.tex`. You can also permanently change the settings through `translate_tex --setdefault`. You can view more details through `translate_tex --help`. `translate_arxiv` also provides exactly the same command line arguments, which have the same effect.
 
 ## Examples
 In the example directory, you can see `main.txt` which is the mathpix output of a part of `paper.pdf`. Run `translate_tex main.txt` and you will get the `main.tex` and `main.pdf`. `translated.png` is what you should expect to see in the `main.pdf`.
 
-## Known Issues
-1. If `\begin{env} \end{env}` is reset with `\newcommand` in latex, it will not be translated correctly.
-2. There is a small probability to get something like "XMATHX_1_2" or wrong formula during translation. The accuracy rate of Tencent translation is slightly lower than that of Google translation.
-
 ## Further developments
 1. Fix bugs in the latex translations.
 2. A more user-friendly interface.
 
 If you have any questions or have interests in making contributions, please contact me by susyustc@gmail.com or joining QQ group 288646946.
 
 ## Donation
```

#### html2text {}

```diff
@@ -50,19 +50,15 @@
 from`, `-to`. For example, `translate_tex -engine tencent input.tex -
 o output.tex`. You can also permanently change the settings through
 `translate_tex --setdefault`. You can view more details through `translate_tex
 --help`. `translate_arxiv` also provides exactly the same command line
 arguments, which have the same effect. ## Examples In the example directory,
 you can see `main.txt` which is the mathpix output of a part of `paper.pdf`.
 Run `translate_tex main.txt` and you will get the `main.tex` and `main.pdf`.
-`translated.png` is what you should expect to see in the `main.pdf`. ## Known
-Issues 1. If `\begin{env} \end{env}` is reset with `\newcommand` in latex, it
-will not be translated correctly. 2. There is a small probability to get
-something like "XMATHX_1_2" or wrong formula during translation. The accuracy
-rate of Tencent translation is slightly lower than that of Google translation.
-## Further developments 1. Fix bugs in the latex translations. 2. A more user-
-friendly interface. If you have any questions or have interests in making
-contributions, please contact me by susyustc@gmail.com or joining QQ group
-288646946. ## Donation If you think this project is helping you a lot, you can
-support us by the Wechat QR code below
+`translated.png` is what you should expect to see in the `main.pdf`. ## Further
+developments 1. Fix bugs in the latex translations. 2. A more user-friendly
+interface. If you have any questions or have interests in making contributions,
+please contact me by susyustc@gmail.com or joining QQ group 288646946. ##
+Donation If you think this project is helping you a lot, you can support us by
+the Wechat QR code below
 [https://github.com/SUSYUSTC/MathTranslate/assets/30529122/16f82637-e102-4330-
                               82ad-bbcbdad1c19d]
```

### Comparing `mathtranslate-2.3.0/mathtranslate/cache.py` & `mathtranslate-2.3.1/mathtranslate/cache.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.0/mathtranslate/config.py` & `mathtranslate-2.3.1/mathtranslate/config.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.0/mathtranslate/encoding.py` & `mathtranslate-2.3.1/mathtranslate/encoding.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.0/mathtranslate/process_file.py` & `mathtranslate-2.3.1/mathtranslate/process_file.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.0/mathtranslate/process_latex.py` & `mathtranslate-2.3.1/mathtranslate/process_latex.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.0/mathtranslate/process_text.py` & `mathtranslate-2.3.1/mathtranslate/process_text.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.0/mathtranslate/tencent.py` & `mathtranslate-2.3.1/mathtranslate/tencent.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.0/mathtranslate/tencentcloud/__init__.py` & `mathtranslate-2.3.1/mathtranslate/tencentcloud/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.0/mathtranslate/tencentcloud/common/__init__.py` & `mathtranslate-2.3.1/mathtranslate/tencentcloud/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.0/mathtranslate/tencentcloud/common/abstract_client.py` & `mathtranslate-2.3.1/mathtranslate/tencentcloud/common/abstract_client.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.0/mathtranslate/tencentcloud/common/abstract_model.py` & `mathtranslate-2.3.1/mathtranslate/tencentcloud/common/abstract_model.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.0/mathtranslate/tencentcloud/common/common_client.py` & `mathtranslate-2.3.1/mathtranslate/tencentcloud/common/common_client.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.0/mathtranslate/tencentcloud/common/credential.py` & `mathtranslate-2.3.1/mathtranslate/tencentcloud/common/credential.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.0/mathtranslate/tencentcloud/common/exception/__init__.py` & `mathtranslate-2.3.1/mathtranslate/tencentcloud/common/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.0/mathtranslate/tencentcloud/common/exception/tencent_cloud_sdk_exception.py` & `mathtranslate-2.3.1/mathtranslate/tencentcloud/common/exception/tencent_cloud_sdk_exception.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.0/mathtranslate/tencentcloud/common/http/__init__.py` & `mathtranslate-2.3.1/mathtranslate/tencentcloud/common/http/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.0/mathtranslate/tencentcloud/common/http/request.py` & `mathtranslate-2.3.1/mathtranslate/tencentcloud/common/http/request.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.0/mathtranslate/tencentcloud/common/profile/__init__.py` & `mathtranslate-2.3.1/mathtranslate/tencentcloud/common/profile/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.0/mathtranslate/tencentcloud/common/profile/client_profile.py` & `mathtranslate-2.3.1/mathtranslate/tencentcloud/common/profile/client_profile.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.0/mathtranslate/tencentcloud/common/profile/http_profile.py` & `mathtranslate-2.3.1/mathtranslate/tencentcloud/common/profile/http_profile.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.0/mathtranslate/tencentcloud/common/sign.py` & `mathtranslate-2.3.1/mathtranslate/tencentcloud/common/sign.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.0/mathtranslate/tencentcloud/tmt/__init__.py` & `mathtranslate-2.3.1/mathtranslate/tencentcloud/tmt/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.0/mathtranslate/tencentcloud/tmt/v20180321/__init__.py` & `mathtranslate-2.3.1/mathtranslate/tencentcloud/tmt/v20180321/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.0/mathtranslate/tencentcloud/tmt/v20180321/errorcodes.py` & `mathtranslate-2.3.1/mathtranslate/tencentcloud/tmt/v20180321/errorcodes.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.0/mathtranslate/tencentcloud/tmt/v20180321/models.py` & `mathtranslate-2.3.1/mathtranslate/tencentcloud/tmt/v20180321/models.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.0/mathtranslate/tencentcloud/tmt/v20180321/tmt_client.py` & `mathtranslate-2.3.1/mathtranslate/tencentcloud/tmt/v20180321/tmt_client.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.0/mathtranslate/translate.py` & `mathtranslate-2.3.1/mathtranslate/translate.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.0/mathtranslate/translate_arxiv.py` & `mathtranslate-2.3.1/mathtranslate/translate_arxiv.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.0/mathtranslate/translate_tex.py` & `mathtranslate-2.3.1/mathtranslate/translate_tex.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.0/mathtranslate/upload_overleaf.py` & `mathtranslate-2.3.1/mathtranslate/upload_overleaf.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.0/mathtranslate/utils.py` & `mathtranslate-2.3.1/mathtranslate/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,28 +97,28 @@
 def process_options(options):
     if options.setkey:
         print('Tencent secretID')
         config.set_variable(config.tencent_secret_id_path, config.tencent_secret_id_default)
         print('Tencent secretKey')
         config.set_variable(config.tencent_secret_key_path, config.tencent_secret_key_default)
         print('saved!')
-        config.reread()
+        config.load()
         print('secretID:', config.tencent_secret_id)
         print('secretKey:', config.tencent_secret_key)
         sys.exit()
 
     if options.setdefault:
         print('Translation engine (google or tencent, default google)')
         config.set_variable(config.default_engine_path, config.default_engine_default)
         print('Translation language from (default en)')
         config.set_variable(config.default_language_from_path, config.default_language_from_default)
         print('Translation language to (default zh-CN)')
         config.set_variable(config.default_language_to_path, config.default_language_to_default)
         print('saved!')
-        config.reread()
+        config.load()
         print('engine:', config.default_engine)
         print('language from:', config.default_language_from)
         print('language to:', config.default_language_to)
         sys.exit()
 
     if options.list:
         print(language_list)
```

### Comparing `mathtranslate-2.3.0/mathtranslate.egg-info/PKG-INFO` & `mathtranslate-2.3.1/mathtranslate.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathtranslate
-Version: 2.3.0
+Version: 2.3.1
 Summary: Translate math-heavy papers
 Home-page: https://github.com/SUSYUSTC/MathTranslate
 Author: MathTranslate developers
 Author-email: susyustc@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -74,18 +74,14 @@
    - To translate an arxiv project: `translate_arxiv 2205.15510` will generate a translated tex project `2205.15510.zip`.
 4. Compile your tex file. For a single file, you can use the command `xelatex output.tex` from [texlive](https://www.tug.org/texlive/). Chinese translation requires the xeCJK package. For arxiv projects, we recommend uploading the obtained .zip file to overleaf for online compilation (New Project - Upload Project). **Note that you need to set the compiler to XeLatex in `Menu - Compiler`.**
 5. You can change the default settings of translation language and engine through command line arguments `-engine`, `-from`, `-to`. For example, `translate_tex -engine tencent input.tex -o output.tex`. You can also permanently change the settings through `translate_tex --setdefault`. You can view more details through `translate_tex --help`. `translate_arxiv` also provides exactly the same command line arguments, which have the same effect.
 
 ## Examples
 In the example directory, you can see `main.txt` which is the mathpix output of a part of `paper.pdf`. Run `translate_tex main.txt` and you will get the `main.tex` and `main.pdf`. `translated.png` is what you should expect to see in the `main.pdf`.
 
-## Known Issues
-1. If `\begin{env} \end{env}` is reset with `\newcommand` in latex, it will not be translated correctly.
-2. There is a small probability to get something like "XMATHX_1_2" or wrong formula during translation. The accuracy rate of Tencent translation is slightly lower than that of Google translation.
-
 ## Further developments
 1. Fix bugs in the latex translations.
 2. A more user-friendly interface.
 
 If you have any questions or have interests in making contributions, please contact me by susyustc@gmail.com or joining QQ group 288646946.
 
 ## Donation
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mathtranslate Version: 2.3.0 Summary: Translate
+Metadata-Version: 2.1 Name: mathtranslate Version: 2.3.1 Summary: Translate
 math-heavy papers Home-page: https://github.com/SUSYUSTC/MathTranslate Author:
 MathTranslate developers Author-email: susyustc@gmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: OS
 Independent Description-Content-Type: text/markdown License-File: LICENSE #
 MathTranslate
      [https://img.shields.io/pypi/v/mathtranslate.svg?logo=pypi]  [https://
        img.shields.io/badge/license-Apache%202.0-yellow.svg?logo=apache]
@@ -55,19 +55,15 @@
 from`, `-to`. For example, `translate_tex -engine tencent input.tex -
 o output.tex`. You can also permanently change the settings through
 `translate_tex --setdefault`. You can view more details through `translate_tex
 --help`. `translate_arxiv` also provides exactly the same command line
 arguments, which have the same effect. ## Examples In the example directory,
 you can see `main.txt` which is the mathpix output of a part of `paper.pdf`.
 Run `translate_tex main.txt` and you will get the `main.tex` and `main.pdf`.
-`translated.png` is what you should expect to see in the `main.pdf`. ## Known
-Issues 1. If `\begin{env} \end{env}` is reset with `\newcommand` in latex, it
-will not be translated correctly. 2. There is a small probability to get
-something like "XMATHX_1_2" or wrong formula during translation. The accuracy
-rate of Tencent translation is slightly lower than that of Google translation.
-## Further developments 1. Fix bugs in the latex translations. 2. A more user-
-friendly interface. If you have any questions or have interests in making
-contributions, please contact me by susyustc@gmail.com or joining QQ group
-288646946. ## Donation If you think this project is helping you a lot, you can
-support us by the Wechat QR code below
+`translated.png` is what you should expect to see in the `main.pdf`. ## Further
+developments 1. Fix bugs in the latex translations. 2. A more user-friendly
+interface. If you have any questions or have interests in making contributions,
+please contact me by susyustc@gmail.com or joining QQ group 288646946. ##
+Donation If you think this project is helping you a lot, you can support us by
+the Wechat QR code below
 [https://github.com/SUSYUSTC/MathTranslate/assets/30529122/16f82637-e102-4330-
                               82ad-bbcbdad1c19d]
```

### Comparing `mathtranslate-2.3.0/mathtranslate.egg-info/SOURCES.txt` & `mathtranslate-2.3.1/mathtranslate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.0/setup.py` & `mathtranslate-2.3.1/setup.py`

 * *Files identical despite different names*

