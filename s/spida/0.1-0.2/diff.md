# Comparing `tmp/spida-0.1.tar.gz` & `tmp/spida-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spida-0.1.tar", last modified: Sat May 20 06:21:28 2023, max compression
+gzip compressed data, was "spida-0.2.tar", last modified: Sat May 20 19:51:20 2023, max compression
```

## Comparing `spida-0.1.tar` & `spida-0.2.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 06:21:28.413220 spida-0.1/
--rw-rw-rw-   0        0        0     1081 2023-05-20 00:50:35.000000 spida-0.1/LICENSE
--rw-rw-rw-   0        0        0     6595 2023-05-20 06:21:28.412214 spida-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     6139 2023-05-20 03:13:16.000000 spida-0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-20 06:21:28.414227 spida-0.1/setup.cfg
--rw-rw-rw-   0        0        0      745 2023-05-20 06:18:49.000000 spida-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-20 06:21:28.367271 spida-0.1/spida/
--rw-rw-rw-   0        0        0       59 2023-05-19 17:08:20.000000 spida-0.1/spida/__init__.py
--rw-rw-rw-   0        0        0    15353 2023-05-20 04:43:06.000000 spida-0.1/spida/stable_diffusion.py
-drwxrwxrwx   0        0        0        0 2023-05-20 06:21:28.411206 spida-0.1/spida/utils/
--rw-rw-rw-   0        0        0       30 2023-05-19 15:45:28.000000 spida-0.1/spida/utils/__init__.py
--rw-rw-rw-   0        0        0     5943 2023-05-19 20:05:30.000000 spida-0.1/spida/utils/img.py
--rw-rw-rw-   0        0        0     1042 2023-05-19 13:56:29.000000 spida-0.1/spida/utils/misc.py
--rw-rw-rw-   0        0        0      861 2023-05-17 04:00:18.000000 spida-0.1/spida/utils/net.py
-drwxrwxrwx   0        0        0        0 2023-05-20 06:21:28.403398 spida-0.1/spida.egg-info/
--rw-rw-rw-   0        0        0     6595 2023-05-20 06:21:28.000000 spida-0.1/spida.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-05-20 06:21:28.000000 spida-0.1/spida.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 06:21:28.000000 spida-0.1/spida.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      268 2023-05-20 06:21:28.000000 spida-0.1/spida.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-20 06:21:28.000000 spida-0.1/spida.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-20 19:51:20.802600 spida-0.2/
+-rw-rw-rw-   0        0        0     1081 2023-05-20 00:50:35.000000 spida-0.2/LICENSE
+-rw-rw-rw-   0        0        0       30 2023-05-20 17:17:43.000000 spida-0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     6619 2023-05-20 19:51:20.801581 spida-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6163 2023-05-20 06:34:04.000000 spida-0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-20 19:51:20.803606 spida-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      777 2023-05-20 19:51:03.000000 spida-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 19:51:20.762864 spida-0.2/spida/
+-rw-rw-rw-   0        0        0       59 2023-05-19 17:08:20.000000 spida-0.2/spida/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-20 19:51:20.781863 spida-0.2/spida/data/
+-rw-rw-rw-   0        0        0        2 2023-05-20 19:45:58.000000 spida-0.2/spida/data/config.json
+-rw-rw-rw-   0        0        0    16070 2023-05-20 19:42:14.000000 spida-0.2/spida/stable_diffusion.py
+drwxrwxrwx   0        0        0        0 2023-05-20 19:51:20.799271 spida-0.2/spida/utils/
+-rw-rw-rw-   0        0        0       30 2023-05-19 15:45:28.000000 spida-0.2/spida/utils/__init__.py
+-rw-rw-rw-   0        0        0     5943 2023-05-19 20:05:30.000000 spida-0.2/spida/utils/img.py
+-rw-rw-rw-   0        0        0     1042 2023-05-19 13:56:29.000000 spida-0.2/spida/utils/misc.py
+-rw-rw-rw-   0        0        0      861 2023-05-17 04:00:18.000000 spida-0.2/spida/utils/net.py
+drwxrwxrwx   0        0        0        0 2023-05-20 19:51:20.781863 spida-0.2/spida.egg-info/
+-rw-rw-rw-   0        0        0     6619 2023-05-20 19:51:20.000000 spida-0.2/spida.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2023-05-20 19:51:20.000000 spida-0.2/spida.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 19:51:20.000000 spida-0.2/spida.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      268 2023-05-20 19:51:20.000000 spida-0.2/spida.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-20 19:51:20.000000 spida-0.2/spida.egg-info/top_level.txt
```

### Comparing `spida-0.1/LICENSE` & `spida-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spida-0.1/PKG-INFO` & `spida-0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: spida
-Version: 0.1
+Version: 0.2
 Summary: A Stable Diffusion API Wrapper for AUTOMATIC1111/stable-diffusion-webui
 Home-page: https://github.com/h2see/spida
 Author: h2see
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10, <3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Spida: Stable Diffusion API Wrapper for Automatic1111 WebUI
 
 [![PyPI Version](https://img.shields.io/pypi/v/spida.svg)](https://pypi.org/project/spida/)
-[![License](https://img.shields.io/pypi/l/spida.svg)](https://github.com/h2see/spida/LICENSE)
+[![License](https://img.shields.io/pypi/l/spida.svg)](https://github.com/h2see/spida/blob/master/LICENSE)
 
 Spida is a Python package that serves as a wrapper for the Stable Diffusion API provided by the Automatic1111 WebUI. It simplifies the usage of the Stable Diffusion model for generating AI-generated images from text prompts. Spida also includes support for the ControlNet extension, allowing users to condition the generation process using ControlNet modules. Spida is an anagram of SDAPI (Stable Diffusion API).
 
 ## Dependencies
 
 Spida requires the [Stable Diffusion WebUI](https://github.com/AUTOMATIC1111/stable-diffusion-webui) with the [ControlNet Extension](https://github.com/Mikubill/sd-webui-controlnet). Spida was tested with Stable Diffusion WebUI git commit hash `89f9faa63388756314e8a1d96cf86bf5e0663045` and ControlNet Extension git commit hash `d831043cb81e97724ccf9f071da391d479440a77`.
 
@@ -187,8 +187,8 @@
 
 # Use the settings for conditioning the generation process
 spida.txt2img("text_prompt", cnet_settings=settings)
 ```
 
 ## License
 
-This project is licensed under the [MIT License](https://github.com/h2see/spida/LICENSE).
+This project is licensed under the [MIT License](https://github.com/h2see/spida/blob/master/LICENSE).
```

### Comparing `spida-0.1/README.md` & `spida-0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Spida: Stable Diffusion API Wrapper for Automatic1111 WebUI
 
 [![PyPI Version](https://img.shields.io/pypi/v/spida.svg)](https://pypi.org/project/spida/)
-[![License](https://img.shields.io/pypi/l/spida.svg)](https://github.com/h2see/spida/LICENSE)
+[![License](https://img.shields.io/pypi/l/spida.svg)](https://github.com/h2see/spida/blob/master/LICENSE)
 
 Spida is a Python package that serves as a wrapper for the Stable Diffusion API provided by the Automatic1111 WebUI. It simplifies the usage of the Stable Diffusion model for generating AI-generated images from text prompts. Spida also includes support for the ControlNet extension, allowing users to condition the generation process using ControlNet modules. Spida is an anagram of SDAPI (Stable Diffusion API).
 
 ## Dependencies
 
 Spida requires the [Stable Diffusion WebUI](https://github.com/AUTOMATIC1111/stable-diffusion-webui) with the [ControlNet Extension](https://github.com/Mikubill/sd-webui-controlnet). Spida was tested with Stable Diffusion WebUI git commit hash `89f9faa63388756314e8a1d96cf86bf5e0663045` and ControlNet Extension git commit hash `d831043cb81e97724ccf9f071da391d479440a77`.
 
@@ -173,8 +173,8 @@
 
 # Use the settings for conditioning the generation process
 spida.txt2img("text_prompt", cnet_settings=settings)
 ```
 
 ## License
 
-This project is licensed under the [MIT License](https://github.com/h2see/spida/LICENSE).
+This project is licensed under the [MIT License](https://github.com/h2see/spida/blob/master/LICENSE).
```

### Comparing `spida-0.1/setup.py` & `spida-0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from setuptools import setup, find_packages
 
 with open("requirements.txt") as f:
     required_packages = f.read().splitlines()
 
 setup(
     name="spida",
-    version="0.1",
+    version="0.2",
     packages=find_packages(),
+    include_package_data=True,
     license="MIT",
     description="A Stable Diffusion API Wrapper for AUTOMATIC1111/stable-diffusion-webui",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="h2see",
     url="https://github.com/h2see/spida",
     classifiers=[
```

### Comparing `spida-0.1/spida/stable_diffusion.py` & `spida-0.2/spida/stable_diffusion.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,41 @@
 import json
-from json.decoder import JSONDecodeError
 import numpy as np
+import importlib.resources as impr
 import os
 import pprint
 
 from . import utils
 
-# LOAD CONFIG
-with open(os.path.join(os.path.dirname(__file__), "config.json"), "a+") as f:
-    try:
-        config = json.load(f)
-    except JSONDecodeError:
-        print("Running first use configuration...\n")
-        config = {}
+# initialize config variable
+config = {}
+
+# get config.json path
+with impr.as_file(impr.files("spida").joinpath("data")) as data_path:
+    config_path = data_path.joinpath("config.json")
+
+
+def set_config(config_dict: dict = None):
+    """
+    Configures Spida.
+
+    By default prompts the user to input configuration settings via the terminal,
+    but will use config_dict instead if specified.
+
+    Parameters
+    ----------
+    config_dict : dict
+        A dictionary of configuration settings for Spida, by default None.
+
+    Returns
+    -------
+    None
+        This function does not return a value; it changes Spida's config.json file.
+    """
+    if config_dict is None:
         config["fail_message"] = "Local server not running, starting..."
         config["webui_path"] = input(
             "Please input Stable Diffusion WebUI folder path\n"
         )
         webui_startfile = input(
             "\nPlease input Stable Diffusion WebUI startfile\n(if ENTER defaults to webui-user.bat)\n"
         )
@@ -24,17 +43,26 @@
             webui_startfile if webui_startfile else "webui-user.bat"
         )
         url = input(
             "\nPlease input API url\n(if ENTER defaults to http://127.0.0.1:7860)\n"
         )
         config["url"] = url if url else "http://127.0.0.1:7860"
         print()
-        f.seek(0)
-        f.write(json.dumps(config))
-        f.truncate()
+    else:
+        config.update(config_dict)
+    with open(config_path, "w") as f:
+        json.dump(config, f)
+
+
+with open(config_path, "r") as f:
+    config.update(json.load(f))
+    if not config:
+        print("Running one time configuration...\n")
+        set_config()
+        print("One time configuration complete!\n")
 
 
 # PRIMARY FUNCTIONS
 
 
 def start():
     """
```

### Comparing `spida-0.1/spida/utils/img.py` & `spida-0.2/spida/utils/img.py`

 * *Files identical despite different names*

### Comparing `spida-0.1/spida/utils/misc.py` & `spida-0.2/spida/utils/misc.py`

 * *Files identical despite different names*

### Comparing `spida-0.1/spida/utils/net.py` & `spida-0.2/spida/utils/net.py`

 * *Files identical despite different names*

### Comparing `spida-0.1/spida.egg-info/PKG-INFO` & `spida-0.2/spida.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: spida
-Version: 0.1
+Version: 0.2
 Summary: A Stable Diffusion API Wrapper for AUTOMATIC1111/stable-diffusion-webui
 Home-page: https://github.com/h2see/spida
 Author: h2see
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10, <3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Spida: Stable Diffusion API Wrapper for Automatic1111 WebUI
 
 [![PyPI Version](https://img.shields.io/pypi/v/spida.svg)](https://pypi.org/project/spida/)
-[![License](https://img.shields.io/pypi/l/spida.svg)](https://github.com/h2see/spida/LICENSE)
+[![License](https://img.shields.io/pypi/l/spida.svg)](https://github.com/h2see/spida/blob/master/LICENSE)
 
 Spida is a Python package that serves as a wrapper for the Stable Diffusion API provided by the Automatic1111 WebUI. It simplifies the usage of the Stable Diffusion model for generating AI-generated images from text prompts. Spida also includes support for the ControlNet extension, allowing users to condition the generation process using ControlNet modules. Spida is an anagram of SDAPI (Stable Diffusion API).
 
 ## Dependencies
 
 Spida requires the [Stable Diffusion WebUI](https://github.com/AUTOMATIC1111/stable-diffusion-webui) with the [ControlNet Extension](https://github.com/Mikubill/sd-webui-controlnet). Spida was tested with Stable Diffusion WebUI git commit hash `89f9faa63388756314e8a1d96cf86bf5e0663045` and ControlNet Extension git commit hash `d831043cb81e97724ccf9f071da391d479440a77`.
 
@@ -187,8 +187,8 @@
 
 # Use the settings for conditioning the generation process
 spida.txt2img("text_prompt", cnet_settings=settings)
 ```
 
 ## License
 
-This project is licensed under the [MIT License](https://github.com/h2see/spida/LICENSE).
+This project is licensed under the [MIT License](https://github.com/h2see/spida/blob/master/LICENSE).
```

