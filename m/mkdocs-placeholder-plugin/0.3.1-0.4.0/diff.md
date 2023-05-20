# Comparing `tmp/mkdocs-placeholder-plugin-0.3.1.tar.gz` & `tmp/mkdocs-placeholder-plugin-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-placeholder-plugin-0.3.1.tar", last modified: Mon May  1 19:01:17 2023, max compression
+gzip compressed data, was "mkdocs-placeholder-plugin-0.4.0.tar", last modified: Sat May 20 15:16:05 2023, max compression
```

## Comparing `mkdocs-placeholder-plugin-0.3.1.tar` & `mkdocs-placeholder-plugin-0.4.0.tar`

### file list

```diff
@@ -1,34 +1,49 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-01 19:01:17.277819 mkdocs-placeholder-plugin-0.3.1/
--rw-r--r--   0 user       (501) staff       (20)     1063 2022-07-29 16:34:40.000000 mkdocs-placeholder-plugin-0.3.1/LICENSE
--rw-r--r--   0 user       (501) staff       (20)       65 2023-03-27 05:22:55.000000 mkdocs-placeholder-plugin-0.3.1/MANIFEST.in
--rw-r--r--   0 user       (501) staff       (20)     7362 2023-05-01 19:01:17.277870 mkdocs-placeholder-plugin-0.3.1/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)     6724 2023-05-01 19:00:26.000000 mkdocs-placeholder-plugin-0.3.1/README.md
--rw-r--r--   0 user       (501) staff       (20)       85 2022-07-29 16:34:40.000000 mkdocs-placeholder-plugin-0.3.1/pyproject.toml
--rw-r--r--   0 user       (501) staff       (20)      943 2023-05-01 19:01:17.278105 mkdocs-placeholder-plugin-0.3.1/setup.cfg
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-01 19:01:17.273761 mkdocs-placeholder-plugin-0.3.1/src/
--rwxr-xr-x   0 user       (501) staff       (20)     1467 2023-05-01 19:00:27.000000 mkdocs-placeholder-plugin-0.3.1/src/mkdocs-placeholder-replace-static.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-01 19:01:17.275727 mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/
--rw-r--r--   0 user       (501) staff       (20)      626 2023-05-01 19:00:27.000000 mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/__init__.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-01 19:01:17.277294 mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/assets/
--rw-r--r--   0 user       (501) staff       (20)      312 2023-03-27 05:34:32.000000 mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/assets/placeholder-data.js
--rw-------   0 user       (501) staff       (20)    21736 2023-05-01 19:00:55.000000 mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/assets/placeholder.min.js
--rw-------   0 user       (501) staff       (20)    91944 2023-05-01 19:00:55.000000 mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/assets/placeholder.min.js.map
--rw-r--r--   0 user       (501) staff       (20)     5288 2023-05-01 19:00:27.000000 mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/assets.py
--rw-r--r--   0 user       (501) staff       (20)     3275 2023-05-01 19:00:27.000000 mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/auto_input_table.py
--rw-r--r--   0 user       (501) staff       (20)     1315 2023-05-01 19:00:27.000000 mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/html_tag_parser.py
--rw-r--r--   0 user       (501) staff       (20)     7847 2023-05-01 19:00:27.000000 mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/input_table.py
--rw-r--r--   0 user       (501) staff       (20)     4122 2023-05-01 19:00:27.000000 mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/input_tag_handler.py
--rw-r--r--   0 user       (501) staff       (20)    13905 2023-05-01 19:00:27.000000 mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/placeholder_data.py
--rw-r--r--   0 user       (501) staff       (20)     6016 2023-05-01 19:00:27.000000 mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/plugin.py
--rw-r--r--   0 user       (501) staff       (20)     2239 2023-05-01 19:00:27.000000 mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/plugin_config.py
--rw-r--r--   0 user       (501) staff       (20)     5202 2023-05-01 19:00:27.000000 mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/static_replacer.py
--rw-r--r--   0 user       (501) staff       (20)     2196 2023-05-01 19:00:27.000000 mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/style.py
--rw-r--r--   0 user       (501) staff       (20)     5043 2023-05-01 19:00:27.000000 mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/validators.py
--rw-r--r--   0 user       (501) staff       (20)     8885 2023-05-01 19:00:27.000000 mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/validators_predefined.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-01 19:01:17.276613 mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     7362 2023-05-01 19:01:17.000000 mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)     1189 2023-05-01 19:01:17.000000 mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2023-05-01 19:01:17.000000 mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)       75 2023-05-01 19:01:17.000000 mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin.egg-info/entry_points.txt
--rw-r--r--   0 user       (501) staff       (20)       14 2023-05-01 19:01:17.000000 mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin.egg-info/requires.txt
--rw-r--r--   0 user       (501) staff       (20)       26 2023-05-01 19:01:17.000000 mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin.egg-info/top_level.txt
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-20 15:16:05.483419 mkdocs-placeholder-plugin-0.4.0/
+-rw-r--r--   0 user       (501) staff       (20)     1063 2022-07-29 16:34:40.000000 mkdocs-placeholder-plugin-0.4.0/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)       65 2023-03-27 05:22:55.000000 mkdocs-placeholder-plugin-0.4.0/MANIFEST.in
+-rw-r--r--   0 user       (501) staff       (20)     9691 2023-05-20 15:16:05.483501 mkdocs-placeholder-plugin-0.4.0/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)     9053 2023-05-20 15:14:57.000000 mkdocs-placeholder-plugin-0.4.0/README.md
+-rw-r--r--   0 user       (501) staff       (20)       85 2022-07-29 16:34:40.000000 mkdocs-placeholder-plugin-0.4.0/pyproject.toml
+-rw-r--r--   0 user       (501) staff       (20)      897 2023-05-20 15:16:05.483852 mkdocs-placeholder-plugin-0.4.0/setup.cfg
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-20 15:16:05.473693 mkdocs-placeholder-plugin-0.4.0/src/
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-20 15:16:05.474890 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-05-10 18:48:15.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/__init__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-20 15:16:05.476815 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/assets/
+-rw-r--r--   0 user       (501) staff       (20)     2944 2023-05-10 18:48:15.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/assets/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)      312 2023-03-27 05:34:32.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/assets/placeholder-data.js
+-rw-r--r--   0 user       (501) staff       (20)    27967 2023-05-20 14:27:02.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/assets/placeholder.min.js
+-rw-r--r--   0 user       (501) staff       (20)   110866 2023-05-20 14:27:02.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/assets/placeholder.min.js.map
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-20 15:16:05.479618 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/
+-rw-r--r--   0 user       (501) staff       (20)      911 2023-05-10 18:48:15.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/__init__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-20 15:16:05.481209 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/config/
+-rw-r--r--   0 user       (501) staff       (20)      277 2023-05-10 18:48:15.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/config/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     4971 2023-05-18 19:10:30.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/config/configuration.py
+-rw-r--r--   0 user       (501) staff       (20)     4601 2023-05-10 18:48:15.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/config/parser_utils.py
+-rw-r--r--   0 user       (501) staff       (20)    10414 2023-05-13 17:10:01.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/config/placeholder.py
+-rw-r--r--   0 user       (501) staff       (20)     3491 2023-05-10 18:48:15.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/config/validator.py
+-rw-r--r--   0 user       (501) staff       (20)     2552 2023-05-20 14:26:55.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/generic_style.py
+-rw-r--r--   0 user       (501) staff       (20)     4885 2023-05-13 17:36:39.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/html_tag_handler.py
+-rw-r--r--   0 user       (501) staff       (20)     1315 2023-05-10 18:48:15.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/html_tag_parser.py
+-rw-r--r--   0 user       (501) staff       (20)     4371 2023-05-18 18:43:12.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/json_generator.py
+-rw-r--r--   0 user       (501) staff       (20)     2209 2023-05-20 14:14:46.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/page_processor.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-20 15:16:05.482277 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/static/
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-05-10 18:48:15.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/static/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     2383 2023-05-13 15:32:30.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/static/input_elements.py
+-rw-r--r--   0 user       (501) staff       (20)     5157 2023-05-13 17:38:11.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/static/placeholder_replacer.py
+-rw-r--r--   0 user       (501) staff       (20)     4168 2023-05-13 16:30:00.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/static/table_generator.py
+-rw-r--r--   0 user       (501) staff       (20)     1348 2023-05-13 15:52:07.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/static/table_replacer.py
+-rw-r--r--   0 user       (501) staff       (20)     3742 2023-05-10 18:48:15.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/validator_functions.py
+-rw-r--r--   0 user       (501) staff       (20)     8731 2023-05-10 18:48:15.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/validators_predefined.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-20 15:16:05.483279 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/mkdocs/
+-rw-r--r--   0 user       (501) staff       (20)      114 2023-05-10 18:48:15.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/mkdocs/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     3048 2023-05-10 18:48:15.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/mkdocs/plugin.py
+-rw-r--r--   0 user       (501) staff       (20)      983 2023-05-10 18:48:15.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/mkdocs/plugin_config.py
+-rw-r--r--   0 user       (501) staff       (20)     1466 2023-05-18 11:04:08.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/mkdocs/style.py
+-rw-r--r--   0 user       (501) staff       (20)     4661 2023-05-10 18:48:15.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/mkdocs/utils.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-20 15:16:05.475559 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     9691 2023-05-20 15:16:05.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)     1950 2023-05-20 15:16:05.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2023-05-20 15:16:05.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)       82 2023-05-20 15:16:05.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 user       (501) staff       (20)       14 2023-05-20 15:16:05.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin.egg-info/requires.txt
+-rw-r--r--   0 user       (501) staff       (20)       26 2023-05-20 15:16:05.000000 mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin.egg-info/top_level.txt
```

### Comparing `mkdocs-placeholder-plugin-0.3.1/LICENSE` & `mkdocs-placeholder-plugin-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-placeholder-plugin-0.3.1/PKG-INFO` & `mkdocs-placeholder-plugin-0.4.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-placeholder-plugin
-Version: 0.3.1
+Version: 0.4.0
 Summary: Add dynamic placeholders to your mkdocs page
 Home-page: https://github.com/six-two/mkdocs-placeholder-plugin
 Author: six-two
 Author-email: pip@six-two.dev
 License: MIT License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
@@ -29,45 +29,74 @@
 
 This README is just a short intro to the package.
 For a quick start and detailed information please see the [documentation for the last release](https://mkdocs-placeholder-plugin.six-two.dev/).
 The documentation is also available in the `docs` folder of the source code and can be built localy with [MkDocs](https://www.mkdocs.org/).
 
 ## Development version
 
-If you want to use the latest development version (may be broken/buggy from time to time), you can install it with:
-```bash
-python3 -m pip install git+https://github.com/six-two/mkdocs-placeholder-plugin
-```
+If you want to use the latest development version (may be broken/buggy from time to time), you can install it by:
+
+1. Cloning the repository:
+    ```bash
+    git clone https://github.com/six-two/mkdocs-placeholder-plugin
+    cd mkdocs-placeholder-plugin
+    ```
+2. Building/Downloading the JavaScript files.
+    Choose any of the following ways:
+    
+    - Build it with npm (natively), by running the `./build-docs.sh` script.
+    - Build it in a (docker/podman) container by using the `Doeckerfile` in the `typescript` directory:
+        ```bash
+        cd typescript
+        podman build --tag placeholder-npm .
+        cd ..
+        ```
+
+        And then running the `./build.sh` script.
+        Once you see mkdocs running, you can terminate it with `Ctrl-C`.
+    - Downloading the files from the development version of the documentation (hosted and built by Vercel):
+        ```bash
+        curl https://dev.mkdocs-placeholder-plugin.six-two.dev/assets/javascripts/placeholder.min.js -o src/mkdocs_placeholder_plugin/assets/placeholder.min.js
+        curl https://dev.mkdocs-placeholder-plugin.six-two.dev/assets/javascripts/placeholder.min.js.map -o src/mkdocs_placeholder_plugin/assets/placeholder.min.js.map
+        ```
+3. Installing the package with pip:
+    ```bash
+    python3 -m pip install .
+    ```
 
 The corresponding documentation is hosted at <https://dev.mkdocs-placeholder-plugin.six-two.dev>.
 
 ## Notable changes
 
-### TODOs
-
-- Rewrite python code and decouple it from MkDocs (to be able to use it with other projects).
-- Implement propper exception handling for TypeScript code to recover from / compartmentalize non-critical errors.
-- Update the documentation.
-
 ### HEAD
 
+- Configuration format changed:
+    - Validators are no longer defined in-line and instead defined in a `validators` section -> easier to reuse custom validators.
+    - Placeholders now need to be specified in a `placeholders` section.
+    - Most settings are now in the configuration file instead of in your `mkdocs.yml`.
+- Some actions can now be toggled by visitors of the site. The settings open when you click the gear icon on a (dynamic) placeholder input table.
+- (By default) values are saved when the focus leaves a text field.
+- Removed static placeholder input tables (`<placeholdertable>`).
+- Uncoupled the code from MkDocs.
+    You should now be able to relatively easy port the project to other Markdown based static site generators if you want to.
+
 ### Version 0.3.1
 
 - Removed `Apply all changes` buttons. See [issue #3](https://github.com/six-two/mkdocs-placeholder-plugin/issues/3)
 
 ### Version 0.3.0
 
 This release may be a bit buggy due to the rewrite and the documentation is not entirely accurate yet.
 I will update the docs after I also clean up / rewrite the python code (planed for v0.4.0).
 
 - Rewrote the JavaScript code in TypeScript:
     - Packed and minified using Webpack, so the file is a bit smaller
     - Should find stupid errors I make in code paths that I do not test (often)
     - Sophisticated update logic: Instead of always reloading the page it tries to update the DOM in-place (if possible), which should improve user experience a bit and is much faster
-    - Recursive placeholders (placeholders that contain placeholders that contain placeholder...) no longer need to be specified in a speific order in the configuration file.
+    - Nested placeholders (placeholders that contain placeholders that contain placeholder...) no longer need to be specified in a speific order in the configuration file.
     - A placeholder's `default-function` and a validator rule's `match_function` are now evaluated using [`new Function(...)`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function) instead of `eval(...)`, so you need to add a return statement.
 
 ### Version 0.2.5
 
 - When an JavaScript generated `auto-input-table` is empty, now a info box is shown (instead of nothing / an empty table).
 - Bugfixes:
     - `auto_placeholder_tables_javascript` had no effect.
@@ -155,7 +184,42 @@
     git tag 0.X.Y
     ```
 7. Update the `latest-release` branch, so that the documentation website gets updated:
     ```
     git branch --force latest-release HEAD
     git push --tags origin latest-release
     ```
+
+### Updating python dependencies
+
+If you don't have them, install `pip-tools`:
+```bash
+python3 -m pip install pip-tools
+```
+
+Then update `requirements.txt`:
+```bash
+pip-compile -U
+```
+
+### Updating npm dependencies
+
+These are only used for the build process, so keeping them up to date is not that critical.
+
+Start a container with nodeJS:
+```bash
+podman run -it --rm -v "$(pwd)/typescript:/mnt" node:latest bash
+```
+
+In the container run the following commands to update the `typescript/package*.json` files on the host:
+```bash
+cd /mnt
+npm i -g npm-check-updates
+ncu -u
+npm i --package-lock-only
+```
+
+Then rebuild the docker image on the host:
+```bash
+cd typescript/
+podman build --tag placeholder-npm .
+```
```

### Comparing `mkdocs-placeholder-plugin-0.3.1/README.md` & `mkdocs-placeholder-plugin-0.4.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -11,45 +11,74 @@
 
 This README is just a short intro to the package.
 For a quick start and detailed information please see the [documentation for the last release](https://mkdocs-placeholder-plugin.six-two.dev/).
 The documentation is also available in the `docs` folder of the source code and can be built localy with [MkDocs](https://www.mkdocs.org/).
 
 ## Development version
 
-If you want to use the latest development version (may be broken/buggy from time to time), you can install it with:
-```bash
-python3 -m pip install git+https://github.com/six-two/mkdocs-placeholder-plugin
-```
+If you want to use the latest development version (may be broken/buggy from time to time), you can install it by:
+
+1. Cloning the repository:
+    ```bash
+    git clone https://github.com/six-two/mkdocs-placeholder-plugin
+    cd mkdocs-placeholder-plugin
+    ```
+2. Building/Downloading the JavaScript files.
+    Choose any of the following ways:
+    
+    - Build it with npm (natively), by running the `./build-docs.sh` script.
+    - Build it in a (docker/podman) container by using the `Doeckerfile` in the `typescript` directory:
+        ```bash
+        cd typescript
+        podman build --tag placeholder-npm .
+        cd ..
+        ```
+
+        And then running the `./build.sh` script.
+        Once you see mkdocs running, you can terminate it with `Ctrl-C`.
+    - Downloading the files from the development version of the documentation (hosted and built by Vercel):
+        ```bash
+        curl https://dev.mkdocs-placeholder-plugin.six-two.dev/assets/javascripts/placeholder.min.js -o src/mkdocs_placeholder_plugin/assets/placeholder.min.js
+        curl https://dev.mkdocs-placeholder-plugin.six-two.dev/assets/javascripts/placeholder.min.js.map -o src/mkdocs_placeholder_plugin/assets/placeholder.min.js.map
+        ```
+3. Installing the package with pip:
+    ```bash
+    python3 -m pip install .
+    ```
 
 The corresponding documentation is hosted at <https://dev.mkdocs-placeholder-plugin.six-two.dev>.
 
 ## Notable changes
 
-### TODOs
-
-- Rewrite python code and decouple it from MkDocs (to be able to use it with other projects).
-- Implement propper exception handling for TypeScript code to recover from / compartmentalize non-critical errors.
-- Update the documentation.
-
 ### HEAD
 
+- Configuration format changed:
+    - Validators are no longer defined in-line and instead defined in a `validators` section -> easier to reuse custom validators.
+    - Placeholders now need to be specified in a `placeholders` section.
+    - Most settings are now in the configuration file instead of in your `mkdocs.yml`.
+- Some actions can now be toggled by visitors of the site. The settings open when you click the gear icon on a (dynamic) placeholder input table.
+- (By default) values are saved when the focus leaves a text field.
+- Removed static placeholder input tables (`<placeholdertable>`).
+- Uncoupled the code from MkDocs.
+    You should now be able to relatively easy port the project to other Markdown based static site generators if you want to.
+
 ### Version 0.3.1
 
 - Removed `Apply all changes` buttons. See [issue #3](https://github.com/six-two/mkdocs-placeholder-plugin/issues/3)
 
 ### Version 0.3.0
 
 This release may be a bit buggy due to the rewrite and the documentation is not entirely accurate yet.
 I will update the docs after I also clean up / rewrite the python code (planed for v0.4.0).
 
 - Rewrote the JavaScript code in TypeScript:
     - Packed and minified using Webpack, so the file is a bit smaller
     - Should find stupid errors I make in code paths that I do not test (often)
     - Sophisticated update logic: Instead of always reloading the page it tries to update the DOM in-place (if possible), which should improve user experience a bit and is much faster
-    - Recursive placeholders (placeholders that contain placeholders that contain placeholder...) no longer need to be specified in a speific order in the configuration file.
+    - Nested placeholders (placeholders that contain placeholders that contain placeholder...) no longer need to be specified in a speific order in the configuration file.
     - A placeholder's `default-function` and a validator rule's `match_function` are now evaluated using [`new Function(...)`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function) instead of `eval(...)`, so you need to add a return statement.
 
 ### Version 0.2.5
 
 - When an JavaScript generated `auto-input-table` is empty, now a info box is shown (instead of nothing / an empty table).
 - Bugfixes:
     - `auto_placeholder_tables_javascript` had no effect.
@@ -137,7 +166,42 @@
     git tag 0.X.Y
     ```
 7. Update the `latest-release` branch, so that the documentation website gets updated:
     ```
     git branch --force latest-release HEAD
     git push --tags origin latest-release
     ```
+
+### Updating python dependencies
+
+If you don't have them, install `pip-tools`:
+```bash
+python3 -m pip install pip-tools
+```
+
+Then update `requirements.txt`:
+```bash
+pip-compile -U
+```
+
+### Updating npm dependencies
+
+These are only used for the build process, so keeping them up to date is not that critical.
+
+Start a container with nodeJS:
+```bash
+podman run -it --rm -v "$(pwd)/typescript:/mnt" node:latest bash
+```
+
+In the container run the following commands to update the `typescript/package*.json` files on the host:
+```bash
+cd /mnt
+npm i -g npm-check-updates
+ncu -u
+npm i --package-lock-only
+```
+
+Then rebuild the docker image on the host:
+```bash
+cd typescript/
+podman build --tag placeholder-npm .
+```
```

### Comparing `mkdocs-placeholder-plugin-0.3.1/setup.cfg` & `mkdocs-placeholder-plugin-0.4.0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mkdocs-placeholder-plugin
-version = 0.3.1
+version = 0.4.0
 author = six-two
 author_email = pip@six-two.dev
 description = Add dynamic placeholders to your mkdocs page
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/six-two/mkdocs-placeholder-plugin
 license = MIT License
@@ -18,22 +18,20 @@
 
 [options]
 include_package_data = True
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.9
-scripts = 
-	src/mkdocs-placeholder-replace-static.py
 install_requires = 
 	mkdocs>=1.4.0
 
 [options.entry_points]
 mkdocs.plugins = 
-	placeholder = mkdocs_placeholder_plugin:PlaceholderPlugin
+	placeholder = mkdocs_placeholder_plugin.mkdocs:PlaceholderPlugin
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/assets/placeholder.min.js` & `mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/assets/placeholder.min.js`

 * *Files 19% similar despite different names*

#### js-beautify {}

```diff
@@ -1,724 +1,818 @@
 (() => {
     "use strict";
     const e = () => `${(new Date).toISOString().slice(11,23)} (TS)`;
-    let n = !0;
+    let t = !0;
 
-    function t(...n) {
+    function n(...t) {
         console.log.apply(console, [`${e()} |`, ...arguments])
     }
 
-    function o(...n) {
+    function o(...t) {
         console.info.apply(console, [`${e()} |`, ...arguments])
     }
 
-    function r(...n) {
+    function a(...t) {
         console.debug.apply(console, [`${e()} |`, ...arguments])
     }
 
-    function a(...e) {}
+    function r(...e) {}
     const l = () => {
-            n ? window.location.reload() : o("Page reload was triggered and blocked due to PlaceholderPlugin.debug_disable_reload")
+            t ? window.location.reload() : o("Page reload was triggered and blocked due to PlaceholderPlugin.debug_disable_reload")
         },
         s = {
-            log: a,
-            info: a,
-            debug: a
+            log: r,
+            info: r,
+            debug: r
         };
-    let c = s;
-    const i = () => {
-        o("Page reload was disabled for debugging purposes"), n = !1
+    let i = s;
+    const c = () => {
+        o("Page reload was disabled for debugging purposes"), t = !1
     };
     var d, u;
     ! function(e) {
         e.Warning = "WARNING", e.Error = "ERROR"
     }(d || (d = {})),
     function(e) {
         e.Good = "GOOD", e.Warning = "WARNING", e.Error = "ERROR", e.NoValidator = "NO_VALIDATOR"
     }(u || (u = {}));
-    const p = e => {
-            const n = U("rules", "object", e);
-            if (0 == n.length) throw new Error(`Rules should not be an empty array.\nProblematic object: ${JSON.stringify(e)}`);
-            const t = A("id", e);
+    const f = e => {
+            const t = F("rules", "object", e);
+            if (0 == t.length) throw new Error(`Rules should not be an empty array.\nProblematic object: ${JSON.stringify(e)}`);
+            const n = W("id", e);
             return {
-                display_name: A("display_name", e),
-                id: t,
-                rules: n.map((e => g(e, t)))
+                display_name: W("display_name", e),
+                id: n,
+                rules: t.map((e => m(e, n)))
             }
         },
-        h = (e, n) => {
-            for (const t of e.rules)
-                if (t.is_match_function(n) != t.should_match && t.severity == d.Error) return !1;
+        p = (e, t) => {
+            for (const n of e.rules)
+                if (n.is_match_function(t) != n.should_match && n.severity == d.Error) return !1;
             return !0
         },
-        _ = (e, n) => {
+        h = (e, t) => {
             if (e.validators.length > 0) {
-                for (const t of e.validators)
-                    if (h(t, n)) return !0;
+                for (const n of e.validators)
+                    if (p(n, t)) return !0;
                 return !1
             }
             return !0
         },
-        f = (e, n) => {
-            const t = [],
+        _ = (e, t) => {
+            const n = [],
                 o = [];
-            for (const r of e.rules) r.is_match_function(n) != r.should_match && (r.severity == d.Error ? o.push(`[${e.display_name}] Error: ${r.error_message}`) : r.severity == d.Warning ? t.push(`[${e.display_name}] Warning: ${r.error_message}`) : console.warn(`Unknown rule severity ${r.severity}`));
+            for (const a of e.rules) a.is_match_function(t) != a.should_match && (a.severity == d.Error ? o.push(`[${e.display_name}] Error: ${a.error_message}`) : a.severity == d.Warning ? n.push(`[${e.display_name}] Warning: ${a.error_message}`) : console.warn(`Unknown rule severity ${a.severity}`));
             return {
                 errors: o,
-                warnings: t
+                warnings: n
             }
         },
-        m = e => {
-            let n;
-            if (1 == e.validators.length) n = `Expecting: ${e.validators[0].display_name}`;
+        g = e => {
+            let t;
+            if (1 == e.validators.length) t = `Expecting: ${e.validators[0].display_name}`;
             else {
-                n = "Expecting one of the following: ";
-                for (const t of e.validators) n += `\n - ${t.display_name}`
+                t = "Expecting one of the following: ";
+                for (const n of e.validators) t += `\n - ${n.display_name}`
             }
             return {
                 rating: u.Good,
-                message: n
+                message: t
             }
         },
-        g = (e, n) => {
-            const t = A("severity", e);
-            let o, r;
-            if ("warning" == t || "warn" == t) o = d.Warning;
+        m = (e, t) => {
+            const n = W("severity", e);
+            let o, a;
+            if ("warning" == n || "warn" == n) o = d.Warning;
             else {
-                if ("error" != t) throw new Error(`Unknown severity '${t}'`);
+                if ("error" != n) throw new Error(`Unknown severity '${n}'`);
                 o = d.Error
             }
             if (e.regex) {
-                const n = A("regex", e),
-                    t = new RegExp(n);
-                r = e => t.test(e)
+                const t = W("regex", e),
+                    n = new RegExp(t);
+                a = e => n.test(e)
             } else {
-                const t = A("match_function", e),
-                    o = new Function("value", t);
-                r = e => {
+                const n = W("match_function", e),
+                    o = new Function("value", n);
+                a = e => {
                     try {
-                        const r = o(e);
-                        if ("boolean" != typeof r) throw new Error(`Custom match_function '${t}' of validator ${n} should return a boolean, but it returned a ${typeof r}: ${r}`);
-                        return r
+                        const a = o(e);
+                        if ("boolean" != typeof a) throw new Error(`Custom match_function '${n}' of validator ${t} should return a boolean, but it returned a ${typeof a}: ${a}`);
+                        return a
                     } catch (e) {
-                        throw new Error(`Failed to evaluate match_function '${t}' of validator ${n}: ${e}`)
+                        throw new Error(`Failed to evaluate match_function '${n}' of validator ${t}: ${e}`)
                     }
                 }
             }
             return {
                 severity: o,
-                should_match: H("should_match", e),
-                error_message: A("error_message", e),
-                is_match_function: r
+                should_match: z("should_match", e),
+                error_message: W("error_message", e),
+                is_match_function: a
             }
         },
-        v = (e, n) => {
-            const t = ((e, n) => {
-                const t = [];
+        v = (e, t) => {
+            const n = ((e, t) => {
+                const n = [];
                 let o = !1;
                 if (e.validators.length > 0) {
-                    for (const r of e.validators) {
-                        const a = f(r, n);
-                        if (t.push(a), 0 == a.errors.length && (o = !0, 0 == a.warnings.length)) return m(e)
+                    for (const a of e.validators) {
+                        const r = _(a, t);
+                        if (n.push(r), 0 == r.errors.length && (o = !0, 0 == r.warnings.length)) return g(e)
                     }
                     return o ? (e => {
-                        const n = [];
-                        for (const t of e) 0 == t.errors.length && n.push(...t.warnings);
+                        const t = [];
+                        for (const n of e) 0 == n.errors.length && t.push(...n.warnings);
                         return {
                             rating: u.Warning,
-                            message: n.join("\n")
+                            message: t.join("\n")
                         }
-                    })(t) : (e => {
-                        const n = [];
-                        for (const t of e) n.push(...t.errors);
+                    })(n) : (e => {
+                        const t = [];
+                        for (const n of e) t.push(...n.errors);
                         return {
                             rating: u.Error,
-                            message: n.join("\n")
+                            message: t.join("\n")
                         }
-                    })(t)
+                    })(n)
                 }
                 return {
                     rating: u.NoValidator,
                     message: "No validators are specified for this placeholder"
                 }
-            })(e, n.value);
-            return ((e, n) => {
-                e.classList.remove("validation-error", "validation-warn", "validation-ok", "validation-none"), n.rating == u.Good ? e.classList.add("validation-ok") : n.rating == u.Warning ? e.classList.add("validation-warn") : n.rating == u.Error ? e.classList.add("validation-error") : n.rating == u.NoValidator ? e.classList.add("validation-none") : console.warn(`Unknown placeholder validity: ${n.rating}`), e.title = n.message
-            })(n, t), c.debug("Validation: name =", e.name, ", value =", n.value, ", results =", t.rating), t.rating != u.Error
-        },
-        w = "PLACEHOLDER_",
-        b = (e, n) => {
-            localStorage.setItem(w + e, n)
-        },
-        x = e => localStorage.getItem(w + e),
-        y = () => {
-            console.warn(`Clearing all localStorage items starting with '${w}'`);
-            let e = 0;
-            for (; e < localStorage.length;) {
-                const n = localStorage.key(e);
-                (null == n ? void 0 : n.startsWith(w)) ? localStorage.removeItem(n): e++
+            })(e, t.value);
+            return ((e, t) => {
+                e.classList.remove("validation-error", "validation-warn", "validation-ok", "validation-none"), t.rating == u.Good ? e.classList.add("validation-ok") : t.rating == u.Warning ? e.classList.add("validation-warn") : t.rating == u.Error ? e.classList.add("validation-error") : t.rating == u.NoValidator ? e.classList.add("validation-none") : console.warn(`Unknown placeholder validity: ${t.rating}`), e.title = t.message
+            })(t, n), i.debug("Validation: name =", e.name, ", value =", t.value, ", results =", n.rating), n.rating != u.Error
+        },
+        b = "PLACEHOLDER_",
+        w = "PLACEHOLDER-SETTING_",
+        x = (e, t) => {
+            localStorage.setItem(b + e, t)
+        },
+        y = e => localStorage.getItem(b + e),
+        $ = (e, t) => {
+            const n = localStorage.getItem(`${w}${e}`);
+            return i.info(`Reading boolean setting '${e}' with value ${n}`), null === n ? t : "1" === n || "0" !== n && (console.warn(`Unexpected state for boolean setting. Should be null, '0' or '1', but was '${n}'`), t)
+        },
+        k = () => {
+            L(b)
+        },
+        E = () => {
+            L(w)
+        },
+        L = e => {
+            console.warn(`Clearing all localStorage items starting with '${e}'`);
+            let t = 0;
+            for (; t < localStorage.length;) {
+                const n = localStorage.key(t);
+                (null == n ? void 0 : n.startsWith(e)) ? localStorage.removeItem(n): t++
             }
             l()
         },
-        $ = (e, n) => {
+        N = (e, t) => {
             try {
-                const t = e.options[n];
-                return null != t && null != t
+                const n = e.options[t];
+                return null != n && null != n
             } catch (e) {
                 return !1
             }
         },
-        k = (e, n) => {
-            const t = _(e, n);
-            if (c.info(`Set textbox ${e.name} to '${n}'. Validation ok? ${t}`), !t) throw new Error(`Validation error: Value '${n}' is not valid for placeholder ${e.name}`);
-            b(`${e.name}_TEXT`, n)
-        },
-        E = e => {
-            const n = document.createElement("div");
-            return n.appendChild(document.createTextNode(e)), n.innerHTML
-        },
-        N = e => {
-            const n = document.createElement("span");
-            return n.classList.add("placeholder-value"), n.dataset.placeholder = e.name, n.textContent = e.expanded_value, n
+        T = (e, t) => {
+            const n = h(e, t);
+            if (i.info(`Set textbox ${e.name} to '${t}'. Validation ok? ${n}`), !n) throw new Error(`Validation error: Value '${t}' is not valid for placeholder ${e.name}`);
+            x(`${e.name}_TEXT`, t)
+        },
+        C = e => {
+            const t = document.createElement("div");
+            return t.appendChild(document.createTextNode(e)), t.innerHTML
+        },
+        I = e => {
+            const t = document.createElement("span");
+            return t.classList.add("placeholder-value"), t.dataset.placeholder = e.name, t.textContent = e.expanded_value, t
         },
-        T = (e, n, t) => {
-            var o;
+        R = (e, t, n, o) => {
+            var a;
             const r = document.createTreeWalker(e, NodeFilter.SHOW_TEXT);
-            let a;
-            n.global || console.warn(`You should set the global flag for the regex. Context: replacing '${n.source}' with '${t.current_value}'`);
-            const l = [];
-            for (; a = r.nextNode();) a.nodeValue && a.nodeValue.match(n) && l.push(a);
-            const s = `<span class="placeholder-value" data-placeholder="${E(t.name)}">TEMPORARY PLACEHOLDER</span>`;
-            for (const e of l)
+            let l;
+            t.global || console.warn(`You should set the global flag for the regex. Context: replacing '${t.source}' with '${n.current_value}'`);
+            let s = 0;
+            if (o) {
+                const e = document.querySelectorAll(".placeholder-value[data-placeholder]");
+                for (const t of e) t.getAttribute("data-placeholder") === n.name && s++;
+                s > 0 && i.debug(`${s} dynamic placeholder elements already exist for placeholder ${n.name}`)
+            }
+            const c = [];
+            for (; l = r.nextNode();) l.nodeValue && l.nodeValue.match(t) && c.push(l);
+            const d = `<span class="placeholder-value" data-placeholder="${C(n.name)}">TEMPORARY PLACEHOLDER</span>`;
+            for (const e of c)
                 if (e.nodeValue) {
-                    const t = E(e.nodeValue).replace(n, s),
-                        r = document.createElement("span");
-                    r.innerHTML = t, null === (o = e.parentElement) || void 0 === o || o.replaceChild(r, e)
-                } return l.length
-        },
-        C = (e, n, t) => {
-            const o = T(e, n.regex_dynamic, n);
-            o > 0 && (c.debug(`Replaced ${n.name} via dynamic method at least ${o} time(s)`), n.count_on_page += o)
-        },
-        L = (e, n, t) => {
-            const o = T(e, n.regex_normal, n);
-            o > 0 && (c.debug(`Replaced ${n.name} via normal (dynamic) method at least ${o} time(s)`), n.count_on_page += o)
+                    const n = C(e.nodeValue).replace(t, d),
+                        o = document.createElement("span");
+                    o.innerHTML = n, null === (a = e.parentElement) || void 0 === a || a.replaceChild(o, e)
+                } return c.length + s
+        },
+        S = (e, t, n) => {
+            const o = R(e, t.regex_dynamic, t, !0);
+            o > 0 && (i.debug(`Replaced ${t.name} via dynamic method at least ${o} time(s)`), t.count_on_page += o)
+        },
+        P = (e, t, n) => {
+            const o = R(e, t.regex_normal, t, !1);
+            o > 0 && (i.debug(`Replaced ${t.name} via normal (dynamic) method at least ${o} time(s)`), t.count_on_page += o)
         },
-        R = (e, n, t) => {
-            const o = ((e, n, t) => {
+        D = (e, t, n) => {
+            const o = ((e, t, n) => {
                 const o = document.createTreeWalker(e, NodeFilter.SHOW_TEXT);
-                let r, a = 0;
-                for (n.global || console.warn(`You should set the global flag for the regex. Context: replacing '${n.source}' with '${t}'`); r = o.nextNode();)
-                    if (r.nodeValue) {
-                        const e = r.nodeValue.replace(n, t);
-                        r.nodeValue != e && (r.nodeValue = e, a++)
-                    } return a
-            })(e, n.regex_static, n.expanded_value);
-            o > 0 && (c.debug(`Replaced ${n.name} via static method at least ${o} time(s)`), n.count_on_page += o, n.reload_page_on_change = !0)
-        },
-        O = (e, n, t) => {
-            const o = ((e, n, t) => {
-                t = E(t), n.global || console.warn(`You should set the global flag for the regex. Context: replacing '${n.source}' with '${t}'`);
-                const o = e.innerHTML.replace(n, t);
+                let a, r = 0;
+                for (t.global || console.warn(`You should set the global flag for the regex. Context: replacing '${t.source}' with '${n}'`); a = o.nextNode();)
+                    if (a.nodeValue) {
+                        const e = a.nodeValue.replace(t, n);
+                        a.nodeValue != e && (a.nodeValue = e, r++)
+                    } return r
+            })(e, t.regex_static, t.expanded_value);
+            o > 0 && (i.debug(`Replaced ${t.name} via static method at least ${o} time(s)`), t.count_on_page += o, t.reload_page_on_change = !0)
+        },
+        O = (e, t, n) => {
+            const o = ((e, t, n) => {
+                n = C(n), t.global || console.warn(`You should set the global flag for the regex. Context: replacing '${t.source}' with '${n}'`);
+                const o = e.innerHTML.replace(t, n);
                 return o != e.innerHTML ? (e.innerHTML = o, 1) : 0
-            })(e, n.regex_html, n.expanded_value);
-            o > 0 && (c.debug(`Replaced ${n.name} via innerHTML method at least ${o} time(s)`), n.count_on_page += o, n.reload_page_on_change = !0)
+            })(e, t.regex_html, t.expanded_value);
+            o > 0 && (i.debug(`Replaced ${t.name} via innerHTML method at least ${o} time(s)`), t.count_on_page += o, t.reload_page_on_change = !0)
         },
-        D = e => {
-            for (const n of e)
-                for (const e of n.output_elements) {
+        A = (e, t, n) => e.replace(t.regex_dynamic, n).replace(t.regex_html, n).replace(t.regex_normal, n).replace(t.regex_static, n),
+        H = e => {
+            for (const t of e)
+                for (const e of t.output_elements) {
                     e.innerHTML = "";
-                    const t = document.createTextNode(n.expanded_value);
-                    e.appendChild(t)
+                    const n = document.createTextNode(t.expanded_value);
+                    e.appendChild(n)
                 }
         };
-    class I {
+    class j {
         constructor(e) {
             this.nodes = new Map;
-            for (const n of e.values()) this.nodes.set(n.name, new P(n));
-            for (const n of e.values()) try {
-                this.on_placeholder_value_change(n)
+            for (const t of e.values()) this.nodes.set(t.name, new U(t));
+            for (const t of e.values()) try {
+                this.on_placeholder_value_change(t)
             } catch (e) {
-                console.error("Error while building dependency graph", e), console.warn("Placeholder values may be inconsistent. Clearing your localStorage should fix this problem."), confirm("We detected a problem with your placeholder values. Resetting them to the defaults should fix this. Should we reset your placeholders?") && y()
+                console.error("Error while building dependency graph", e), console.warn("Placeholder values may be inconsistent. Clearing your localStorage should fix this problem."), confirm("We detected a problem with your placeholder values. Resetting them to the defaults should fix this. Should we reset your placeholders?") && k()
             }
             for (const e of this.nodes.values()) 0 == e.downlinks.length && e.recalculate_expanded_value(!0)
         }
         debug_print_representation() {
             let e = "Dependency graph nodes (DEBUG view):";
-            for (const n of this.nodes.values()) {
-                const t = n.downlinks.map((e => e.placeholder.name)).join(", ");
-                0 == t.length ? e += `\n${n.placeholder.name} (${n.placeholder.expanded_value}) has no dependencies` : e += `\n${n.placeholder.name} (${n.placeholder.expanded_value}) depends on ${t}`
+            for (const t of this.nodes.values()) {
+                const n = t.downlinks.map((e => e.placeholder.name)).join(", ");
+                0 == n.length ? e += `\n${t.placeholder.name} (${t.placeholder.expanded_value}) has no dependencies` : e += `\n${t.placeholder.name} (${t.placeholder.expanded_value}) depends on ${n}`
             }
-            c.debug(e)
+            i.debug(e)
         }
         unmark_everything() {
             for (const e of this.nodes.values()) e.marked = !1
         }
         get_node(e) {
-            const n = this.nodes.get(e.name);
-            if (null == n) throw new Error(`Placeholder ${e.name} is not part of the dependency graph`);
-            return n
+            const t = this.nodes.get(e.name);
+            if (null == t) throw new Error(`Placeholder ${e.name} is not part of the dependency graph`);
+            return t
         }
         on_placeholder_value_change(e) {
-            const n = this.get_node(e);
-            if (this.update_placeholder_downlinks(e), this.has_loop()) throw e.expanded_value = e.current_value, n.downlinks = [], new Error(`Placeholder ${e.name} was part of a loop and has temporarily been made non-recursive`);
-            n.recalculate_expanded_value(!0)
+            const t = this.get_node(e);
+            if (this.update_placeholder_downlinks(e), this.has_loop()) throw e.expanded_value = e.current_value, t.downlinks = [], new Error(`Placeholder ${e.name} was part of a loop and has temporarily been made non-recursive`);
+            t.recalculate_expanded_value(!0)
         }
         get_all_marked() {
             const e = [];
-            for (const n of this.nodes.values()) n.marked && e.push(n.placeholder);
+            for (const t of this.nodes.values()) t.marked && e.push(t.placeholder);
             return e
         }
         get_all_upstream(e) {
             return this.unmark_everything(), this.get_node(e).recursive_mark_upstream(), this.get_all_marked()
         }
         update_placeholder_downlinks(e) {
-            if (0 == e.allow_recursive) return;
-            const n = this.get_node(e);
-            for (const e of n.downlinks) e.remove_uplink(n);
-            n.downlinks = [];
-            for (const t of this.nodes.values()) t != n && S(e.current_value, t.placeholder) && (n.downlinks.push(t), t.uplinks.push(n))
+            if (!e.allow_nested) return void i.debug(`${e.name} can not contain nested placeholders`);
+            const t = this.get_node(e);
+            for (const e of t.downlinks) e.remove_uplink(t);
+            t.downlinks = [];
+            for (const n of this.nodes.values()) n != t && M(e.current_value, n.placeholder) && (t.downlinks.push(n), n.uplinks.push(t))
         }
         get_all_used_placeholders() {
             this.unmark_everything();
             for (const e of this.nodes.values()) e.placeholder.count_on_page > 0 && e.recursive_mark_downstream();
             return this.get_all_marked()
         }
         has_loop() {
             this.unmark_everything();
             for (const e of this.nodes.values())
                 if (!e.marked && this._has_loop([], e)) return !0;
             return !1
         }
-        _has_loop(e, n) {
-            const t = [...e, n],
-                o = e.indexOf(n);
+        _has_loop(e, t) {
+            const n = [...e, t],
+                o = e.indexOf(t);
             if (-1 != o) {
                 let e = "Dependency cycle in placeholders detected:";
-                for (let n = o; n < t.length; n++) {
-                    const o = t[n].placeholder;
+                for (let t = o; t < n.length; t++) {
+                    const o = n[t].placeholder;
                     e += `\n$ -> ${o.name}: ${o.current_value}`
                 }
                 return console.warn(e), !0
             }
-            if (n.marked) return !1;
-            n.marked = !0;
-            for (const e of n.downlinks)
-                if (this._has_loop(t, e)) return !0;
+            if (t.marked) return !1;
+            t.marked = !0;
+            for (const e of t.downlinks)
+                if (this._has_loop(n, e)) return !0;
             return !1
         }
     }
-    const S = (e, n) => n.regex_dynamic.test(e) || n.regex_html.test(e) || n.regex_normal.test(e) || n.regex_static.test(e);
-    class P {
+    const M = (e, t) => t.regex_dynamic.test(e) || t.regex_html.test(e) || t.regex_normal.test(e) || t.regex_static.test(e);
+    class U {
         constructor(e) {
             this.uplinks = [], this.downlinks = [], this.marked = !1, this.placeholder = e
         }
         remove_uplink(e) {
-            this.uplinks = this.uplinks.filter((n => n != e))
+            this.uplinks = this.uplinks.filter((t => t != e))
         }
         recalculate_expanded_value(e) {
-            let n = this.placeholder.current_value;
-            for (const e of this.downlinks) t = n, o = e.placeholder, n = t.replace(o.regex_dynamic, o.expanded_value).replace(o.regex_html, o.expanded_value).replace(o.regex_normal, o.expanded_value).replace(o.regex_static, o.expanded_value);
-            var t, o;
-            if (this.placeholder.expanded_value = n, e)
-                for (const n of this.uplinks) n.recalculate_expanded_value(e)
+            let t = this.placeholder.current_value;
+            if (this.placeholder.allow_nested && (t = ((e, t) => {
+                    if (0 == t.length) return e;
+                    if (1 == t.length) {
+                        const n = t[0];
+                        return A(e, n, n.expanded_value)
+                    } {
+                        const n = `${Date.now()}_${Math.random()}`;
+                        for (const o of t) e = A(e, o, `x${o.name}#${n}x`);
+                        for (const o of t) {
+                            const t = new RegExp(`x${o.name}#${n}x`, "g");
+                            e = e.replace(t, o.expanded_value)
+                        }
+                        return e
+                    }
+                })(t, this.downlinks.map((e => e.placeholder)))), this.placeholder.expanded_value = t, e)
+                for (const t of this.uplinks) t.recalculate_expanded_value(e)
         }
         recursive_mark_upstream() {
             this.marked = !0;
             for (const e of this.uplinks) e.recursive_mark_upstream()
         }
         recursive_mark_downstream() {
             this.marked = !0;
             for (const e of this.downlinks) e.recursive_mark_downstream()
         }
     }
-    const j = (e, n, t) => {
-            const o = t[e],
-                r = typeof o;
-            if (r != n) throw new Error(`Type mismatch: ${e} should be ${n}, but is ${r}.\nProblematic object: ${JSON.stringify(t)}`);
+    const V = (e, t, n) => {
+            const o = n[e],
+                a = typeof o;
+            if (a != t) throw new Error(`Type mismatch: ${e} should be ${t}, but is ${a}.\nProblematic object: ${JSON.stringify(n)}`);
             return o
         },
-        A = (e, n) => j(e, "string", n),
-        H = (e, n) => j(e, "boolean", n),
-        M = (e, n) => j(e, "number", n),
-        U = (e, n, t) => {
-            const o = t[e];
+        W = (e, t) => V(e, "string", t),
+        z = (e, t) => V(e, "boolean", t),
+        J = (e, t) => V(e, "number", t),
+        F = (e, t, n) => {
+            const o = n[e];
             if (Array.isArray(o)) {
-                for (const [r, a] of o.entries()) {
-                    const o = typeof a;
-                    if (o != n) {
-                        const a = `Type mismatch: ${e}'s ${r+1}th element should be ${n}, but is ${o}.\nProblematic object: ${JSON.stringify(t)}`;
-                        throw new Error(a)
+                for (const [a, r] of o.entries()) {
+                    const o = typeof r;
+                    if (o != t) {
+                        const r = `Type mismatch: ${e}'s ${a+1}th element should be ${t}, but is ${o}.\nProblematic object: ${JSON.stringify(n)}`;
+                        throw new Error(r)
                     }
                 }
                 return o
             }
-            throw new Error(`Type mismatch: ${e} should be an array, but is not.\nProblematic object: ${JSON.stringify(t)}`)
+            throw new Error(`Type mismatch: ${e} should be an array, but is not.\nProblematic object: ${JSON.stringify(n)}`)
         };
-    var V;
+    var X;
     ! function(e) {
         e.Textbox = "TEXTBOX", e.Checkbox = "CHECKBOX", e.Dropdown = "DROPDOWN"
-    }(V || (V = {}));
-    const W = (e, n, t, o) => {
-            const r = A("type", e),
-                a = A("name", e);
+    }(X || (X = {}));
+    const G = e => e.replace(/[.*+?^${}()|[\]\\]/g, "\\$&"),
+        B = (e, t, n, o) => {
+            const a = W("type", e),
+                r = W("name", e);
             let l = {
-                name: a,
+                name: r,
                 order_index: o,
-                regex_dynamic: RegExp(t.dynamic_prefix + a + t.dynamic_suffix, "g"),
-                regex_html: RegExp(t.html_prefix + a + t.html_suffix, "g"),
-                regex_normal: RegExp(t.normal_prefix + a + t.normal_suffix, "g"),
-                regex_static: RegExp(t.static_prefix + a + t.static_suffix, "g"),
-                description: A("description", e),
-                read_only: H("read_only", e),
-                allow_inner_html: H("allow_inner_html", e),
-                allow_recursive: !1,
+                regex_dynamic: RegExp(G(n.dynamic_prefix) + r + G(n.dynamic_suffix), "g"),
+                regex_html: RegExp(G(n.html_prefix) + r + G(n.html_suffix), "g"),
+                regex_normal: RegExp(G(n.normal_prefix) + r + G(n.normal_suffix), "g"),
+                regex_static: RegExp(G(n.static_prefix) + r + G(n.static_suffix), "g"),
+                description: W("description", e),
+                read_only: z("read_only", e),
+                allow_inner_html: z("allow_inner_html", e),
+                allow_nested: z("allow_nested", e),
                 current_value: "UNINITIALIZED",
                 expanded_value: "UNINITIALIZED",
                 count_on_page: 0,
                 reload_page_on_change: !1,
                 output_elements: []
             };
-            if ("textbox" === r) {
-                const t = F(l, e, n);
+            if ("textbox" === a) {
+                const n = q(l, e, t);
                 return (e => {
-                    const n = x(`${e.name}_TEXT`);
-                    if (null != n) {
-                        if (_(e, n)) return void(e.current_value = n);
-                        console.warn(`Stored value for placeholder ${e.name} is invalid: '${n}'. Will revert to default.`)
+                    const t = y(`${e.name}_TEXT`);
+                    if (null != t) {
+                        if (h(e, t)) return void(e.current_value = t);
+                        console.warn(`Stored value for placeholder ${e.name} is invalid: '${t}'. Will revert to default.`)
                     }
-                    if (null != e.default_value) e.current_value = e.default_value, _(e, e.default_value) || console.warn(`Default value for placeholder '${e.name}' is invalid: '${e.default_value}'`);
+                    if (null != e.default_value) e.current_value = e.default_value, h(e, e.default_value) || console.warn(`Default value for placeholder '${e.name}' is invalid: '${e.default_value}'`);
                     else {
                         if (!e.default_function) throw new Error(`Either 'default_value' or 'default_function' needs to be set for placeholder ${e.name}`);
                         try {
-                            const n = e.default_function();
-                            e.current_value = n;
+                            const t = e.default_function();
+                            e.current_value = t;
                             try {
-                                k(e, n)
-                            } catch (t) {
-                                console.warn(`Default function for placeholder '${e.name}' returned invalid value: '${n}'`)
+                                T(e, t)
+                            } catch (n) {
+                                console.warn(`Default function for placeholder '${e.name}' returned invalid value: '${t}'`)
                             }
-                        } catch (n) {
-                            console.error(`Error while loading default textbox state for placeholder ${e.name}:`, n), e.current_value = "DEFAULT_FUNCTION_ERROR"
+                        } catch (t) {
+                            console.error(`Error while loading default textbox state for placeholder ${e.name}:`, t), e.current_value = "DEFAULT_FUNCTION_ERROR"
                         }
                     }
-                })(t), t
+                })(n), n
             }
-            if ("checkbox" == r) {
-                const n = J(l, e);
+            if ("checkbox" == a) {
+                const t = Y(l, e);
                 return (e => {
-                    const n = x(`${e.name}_IS_CHECKED`);
-                    null == n ? e.current_is_checked = e.checked_by_default : "0" == n || "1" == n ? e.current_is_checked = "1" == n : (console.warn(`Unexpected state for checkbox. Should be '0' or '1', but was '${n}'`), e.current_is_checked = e.checked_by_default), e.current_value = e.current_is_checked ? e.value_checked : e.value_unchecked
-                })(n), n
+                    const t = y(`${e.name}_IS_CHECKED`);
+                    null == t ? e.current_is_checked = e.checked_by_default : "0" == t || "1" == t ? e.current_is_checked = "1" == t : (console.warn(`Unexpected state for checkbox. Should be '0' or '1', but was '${t}'`), e.current_is_checked = e.checked_by_default), e.current_value = e.current_is_checked ? e.value_checked : e.value_unchecked
+                })(t), t
             }
-            if ("dropdown" == r) {
-                const n = X(l, e);
+            if ("dropdown" == a) {
+                const t = K(l, e);
                 return (e => {
-                    const n = x(`${e.name}_INDEX`);
-                    if (null == n) e.current_index = e.default_index;
+                    const t = y(`${e.name}_INDEX`);
+                    if (null == t) e.current_index = e.default_index;
                     else {
-                        const t = Number(n);
-                        $(e, t) ? e.current_index = t : (console.warn(`Unexpected state for dropdown. Should be a whole number N, where 0 <= N < ${e.options.length}. But it is ${n}`), e.current_index = e.default_index)
+                        const n = Number(t);
+                        N(e, n) ? e.current_index = n : (console.warn(`Unexpected state for dropdown. Should be a whole number N, where 0 <= N < ${e.options.length}. But it is ${t}`), e.current_index = e.default_index)
                     }
                     e.current_value = e.options[e.current_index].value
-                })(n), n
+                })(t), t
             }
-            throw new Error(`Unsupported placeholder type '${r}'`)
+            throw new Error(`Unsupported placeholder type '${a}'`)
         },
-        F = (e, n, t) => {
-            let o, r;
-            if (null != n.default_value) r = A("default_value", n);
+        q = (e, t, n) => {
+            let o, a;
+            if (null != t.default_value) a = W("default_value", t);
             else {
-                const t = A("default_function", n);
+                const n = W("default_function", t);
                 o = () => {
                     try {
-                        const e = new Function(t)();
-                        if ("string" != typeof e) throw new Error(`Custom function '${t}' should return a string, but it returned a ${typeof e}: ${e}`);
+                        const e = new Function(n)();
+                        if ("string" != typeof e) throw new Error(`Custom function '${n}' should return a string, but it returned a ${typeof e}: ${e}`);
                         return e
-                    } catch (n) {
-                        throw new Error(`Failed to evaluate default_function '${t}' of placeholder ${e.name}: ${n}`)
+                    } catch (t) {
+                        throw new Error(`Failed to evaluate default_function '${n}' of placeholder ${e.name}: ${t}`)
                     }
                 }
             }
-            const a = U("validators", "string", n),
+            const r = F("validators", "string", t),
                 l = [];
-            for (const e of a) {
-                const n = t.get(e);
-                if (!n) {
-                    const n = Array.from(t.keys()).join(", ");
-                    throw new Error(`No validator with id '${e}' was found. Known validators are ${n}`)
+            for (const e of r) {
+                const t = n.get(e);
+                if (!t) {
+                    const t = Array.from(n.keys()).join(", ");
+                    throw new Error(`No validator with id '${e}' was found. Known validators are ${t}`)
                 }
-                l.push(n)
+                l.push(t)
             }
             return Object.assign(Object.assign({}, e), {
-                allow_recursive: H("allow_recursive", n),
                 default_function: o,
-                default_value: r,
+                default_value: a,
                 input_elements: [],
-                type: V.Textbox,
+                type: X.Textbox,
                 validators: l
             })
         },
-        J = (e, n) => Object.assign(Object.assign({}, e), {
-            allow_recursive: !0,
-            checked_by_default: H("checked_by_default", n),
+        Y = (e, t) => Object.assign(Object.assign({}, e), {
+            checked_by_default: z("checked_by_default", t),
             current_is_checked: !1,
             input_elements: [],
-            value_checked: A("value_checked", n),
-            value_unchecked: A("value_unchecked", n),
-            type: V.Checkbox
+            value_checked: W("value_checked", t),
+            value_unchecked: W("value_unchecked", t),
+            type: X.Checkbox
         }),
-        X = (e, n) => {
-            const t = U("options", "object", n),
+        K = (e, t) => {
+            const n = F("options", "object", t),
                 o = [];
-            for (const e of t) o.push({
-                display_name: A("display_name", e),
-                value: A("value", e)
+            for (const e of n) o.push({
+                display_name: W("display_name", e),
+                value: W("value", e)
             });
-            const r = M("default_index", n);
-            if (r < 0) throw new Error(`Invalid value: "default_index" should not be negative, but is ${r}.\nProblematic object: ${JSON.stringify(n)}`);
-            if (r >= o.length) throw new Error(`Invalid value: "default_index" should be smaller than the number of options (${o.length}), but is ${r}.\nProblematic object: ${JSON.stringify(n)}`);
+            const a = J("default_index", t);
+            if (a < 0) throw new Error(`Invalid value: "default_index" should not be negative, but is ${a}.\nProblematic object: ${JSON.stringify(t)}`);
+            if (a >= o.length) throw new Error(`Invalid value: "default_index" should be smaller than the number of options (${o.length}), but is ${a}.\nProblematic object: ${JSON.stringify(t)}`);
             return Object.assign(Object.assign({}, e), {
-                allow_recursive: !0,
                 current_index: 0,
-                default_index: r,
+                default_index: a,
                 input_elements: [],
                 options: o,
-                type: V.Dropdown
+                type: X.Dropdown
             })
         },
-        G = new Map;
-    G.set("name", "Name"), G.set("description", "Description"), G.set("value", "Value"), G.set("input", "Input element"), G.set("description-or-name", "Description / name");
-    const B = (e, n) => {
-            e.appendChild(document.createTextNode(n))
-        },
-        q = (e, n) => {
-            const t = document.createElement(n);
-            return e.appendChild(t), t
-        },
-        K = (e, n, t, o) => {
-            if (o = Y(o), e.innerHTML = "", 0 == o.length) {
-                const n = q(e, "div");
-                return n.classList.add("info-message"), void(0 == o.length && B(n, "No placeholders to be shown"))
-            }
-            c.info("Creating automatic input table at", e, "with columns", n);
-            const r = q(e, "table"),
-                a = q(r, "thead"),
-                l = q(a, "tr"),
-                s = q(r, "tbody");
-            for (const e of n) {
-                const n = q(l, "th"),
-                    t = G.get(e);
-                t ? B(n, t) : (B(n, e), console.error(`Unknown column name: ${e}`))
-            }
-            const i = [];
-            for (const e of o) {
-                if (e.read_only) {
-                    c.debug(`auto_table: Skipping ${e.name} because it is read-only`);
-                    continue
-                }
-                const o = q(s, "tr");
-                Z(o, e, n, t), i.push({
-                    element: o,
-                    placeholder: e
-                })
-            }
-            t.input_tables.push({
-                columns: n,
-                table_element: r,
-                rows: i
-            })
+        Z = new Map;
+    Z.set("name", "Name"), Z.set("description", "Description"), Z.set("value", "Value"), Z.set("input", "Input element"), Z.set("description-or-name", "Description / name");
+    const Q = (e, t) => {
+            e.appendChild(document.createTextNode(t))
+        },
+        ee = (e, t) => {
+            const n = document.createElement(t);
+            return e.appendChild(n), n
+        },
+        te = (e, t, n, o, a = (e => {})) => {
+            const r = ee(e, "label");
+            r.textContent = `${o} `;
+            const l = ee(r, "input");
+            l.type = "checkbox", l.checked = t, l.addEventListener("change", (() => {
+                ((e, t) => {
+                    i.info(`Storing boolean setting '${e}' with value ${t}`), localStorage.setItem(`${w}${e}`, t ? "1" : "0")
+                })(n, l.checked), a(l.checked)
+            }))
         },
-        Y = e => [...new Set(e)].sort(((e, n) => e.order_index - n.order_index)),
-        Z = (e, n, t, o) => {
-            for (const r of t) {
-                const t = q(e, "td");
-                if ("name" == r) B(t, n.name);
-                else if ("description" == r) B(t, n.description);
-                else if ("value" == r) {
-                    const e = N(n);
-                    t.appendChild(e), n.output_elements.push(e)
-                } else if ("input" == r) {
-                    const e = q(t, "input");
-                    Q(o, n, e)
-                } else if ("description-or-name" == r) {
-                    const e = n.description || n.name;
-                    B(t, e)
-                } else console.error(`Unknown column name: ${r}`)
+        ne = (e, t, n, o, a) => {
+            o = oe(o);
+            const r = document.createElement("div");
+            if (0 == o.length) {
+                if (!a) return void e.remove();
+                r.textContent = "No placeholders to be shown"
+            } else {
+                i.info("Creating automatic input table at", e, "with columns", t), r.classList.add("table-div"), ee(r, "b").innerHTML = "Enter different values in the table below and press <code>Enter</code> to update this page.";
+                const a = ee(r, "table"),
+                    l = ee(a, "thead"),
+                    s = ee(l, "tr"),
+                    c = ee(a, "tbody");
+                for (const e of t) {
+                    const t = ee(s, "th"),
+                        n = Z.get(e);
+                    n ? Q(t, n) : (Q(t, e), console.error(`Unknown column name: ${e}`))
+                }
+                const d = [];
+                for (const e of o) {
+                    if (e.read_only) {
+                        i.debug(`auto_table: Skipping ${e.name} because it is read-only`);
+                        continue
+                    }
+                    const o = ee(c, "tr");
+                    ae(o, e, t, n), d.push({
+                        element: o,
+                        placeholder: e
+                    })
+                }
+                n.input_tables.push({
+                    columns: t,
+                    table_element: a,
+                    rows: d
+                })
+            }((e, t, n) => {
+                t.innerHTML = "";
+                const o = ee(t, "div"),
+                    a = ee(o, "div"),
+                    r = ee(o, "div"),
+                    l = ee(t, "div"),
+                    s = ee(l, "div");
+                l.append(n);
+                const i = e => {
+                    l.style.display = e ? "flex" : "none", a.textContent = "Placeholders: Click here to " + (e ? "collapse" : "expand")
+                };
+                o.classList.add("auto-table-title"), l.classList.add("expandable_contents"), s.classList.add("settings_contents");
+                let c = e.settings.expand_auto_tables;
+                i(c), a.addEventListener("click", (() => {
+                    c = !c, i(c)
+                })), a.classList.add("text"), ((e, t, n) => {
+                    let o = !1;
+                    e.onclick = e => {
+                        e.preventDefault(), e.stopPropagation(), o = !o, t.style.display = o ? "flex" : "none", o && n()
+                    }, t.style.display = o ? "flex" : "none", e.classList.add("settings_button"), e.innerHTML = '<svg viewBox="0 0 40 40" xmlns="http://www.w3.org/2000/svg">\n <path id="svg_6" d="m7.79338,20.02127l0,0c0,-6.84327 5.74307,-12.39083 12.82751,-12.39083l0,0c3.40207,0 6.6648,1.30546 9.07042,3.62919c2.40563,2.32373 3.75709,5.47539 3.75709,8.76164l0,0c0,6.84327 -5.74307,12.39083 -12.82751,12.39083l0,0c-7.08444,0 -12.82751,-5.54757 -12.82751,-12.39083zm6.41376,0l0,0c0,3.42163 2.87154,6.19542 6.41376,6.19542c3.54222,0 6.41376,-2.77378 6.41376,-6.19542c0,-3.42163 -2.87154,-6.19542 -6.41376,-6.19542l0,0c-3.54222,0 -6.41376,2.77378 -6.41376,6.19542z" stroke="#fff" fill="#ffffff"/>\n <path id="svg_7" d="m17.46095,7.63098l1.2691,-5.24017l4.23035,0l1.2691,5.24017l-6.76856,0z" stroke="#fff" fill="#ffffff"/>\n <path transform="rotate(180, 20.9544, 35.1419)" id="svg_11" d="m17.57012,37.76199l1.2691,-5.24017l4.23035,0l1.2691,5.24017l-6.76856,0z" stroke="#fff" fill="#ffffff"/>\n <path transform="rotate(43, 31.5439, 9.59605)" id="svg_12" d="m28.15964,12.21614l1.2691,-5.24017l4.23035,0l1.2691,5.24017l-6.76856,0z" stroke="#fff" fill="#ffffff"/>\n <path transform="rotate(90, 35.9107, 19.8581)" id="svg_13" d="m32.52645,22.47815l1.2691,-5.24017l4.23035,0l1.2691,5.24017l-6.76856,0z" stroke="#fff" fill="#ffffff"/>\n <path transform="rotate(135, 31.7623, 30.2292)" id="svg_14" d="m28.37798,32.84933l1.2691,-5.24017l4.23035,0l1.2691,5.24017l-6.76856,0z" stroke="#fff" fill="#ffffff"/>\n <path transform="rotate(-45, 9.49152, 9.48688)" id="svg_15" d="m6.10724,12.10697l1.2691,-5.24017l4.23035,0l1.2691,5.24017l-6.76856,0z" stroke="#fff" fill="#ffffff"/>\n <path transform="rotate(-90, 5.01553, 19.9672)" id="svg_16" d="m1.63126,22.58732l1.2691,-5.24017l4.23035,0l1.2691,5.24017l-6.76856,0z" stroke="#fff" fill="#ffffff"/>\n <path transform="rotate(-135, 9.60069, 30.7751)" id="svg_17" d="m6.21641,33.39518l1.2691,-5.24017l4.23035,0l1.2691,5.24017l-6.76856,0z" stroke="#fff" fill="#ffffff"/>\n</svg>', e.title = "Hide / show settings"
+                })(r, s, (() => {
+                    c || (c = !0, i(c))
+                })), ((e, t) => {
+                    const n = t => {
+                        for (const n of e.placeholders.values())
+                            for (const e of n.output_elements) t ? e.classList.add("placeholder-value-highlighted") : e.classList.remove("placeholder-value-highlighted")
+                    };
+                    n(e.settings.highlight_placeholders), ee(t, "b").textContent = "Settings", te(t, e.settings.expand_auto_tables, "expand_auto_tables", "Expand placeholder tables by default*"), te(t, e.settings.apply_change_on_focus_change, "apply_change_on_focus_change", "Apply value when focus changes away*"), te(t, e.settings.debug, "debug", "Log JavaScript debug messages to console*"), te(t, e.settings.highlight_placeholders, "highlight_placeholders", "Highlight placeholders (useful for debugging)", n), ee(t, "i").textContent = "* You need to reload the page for these settings to take effect.";
+                    const o = ee(t, "div");
+                    o.classList.add("button-bar");
+                    const a = ee(o, "button");
+                    a.textContent = "Reset settings", a.addEventListener("click", E);
+                    const r = ee(o, "button");
+                    r.textContent = "Reset all placeholders", r.addEventListener("click", k)
+                })(e, s)
+            })(n, e, r)
+        },
+        oe = e => [...new Set(e)].sort(((e, t) => e.order_index - t.order_index)),
+        ae = (e, t, n, o) => {
+            for (const a of n) {
+                const n = ee(e, "td");
+                if ("name" == a) Q(n, t.name);
+                else if ("description" == a) Q(n, t.description);
+                else if ("value" == a) {
+                    const e = I(t);
+                    n.appendChild(e), t.output_elements.push(e)
+                } else if ("input" == a) {
+                    const e = ee(n, "input");
+                    le(o, t, e)
+                } else if ("description-or-name" == a) {
+                    const e = t.description || t.name;
+                    Q(n, e)
+                } else console.error(`Unknown column name: ${a}`)
             }
         },
-        z = (e, n, t) => {
-            t = Y(t);
+        re = (e, t, n) => {
+            n = oe(n);
             const o = [];
-            for (const e of n.rows) t.includes(e.placeholder) ? o.push(e) : (c.debug(`Removed table row for ${e.placeholder.name}:`, e.element), e.element.remove());
-            const r = [],
-                a = [...o].reverse(),
-                l = [...t].reverse();
+            for (const e of t.rows) n.includes(e.placeholder) ? o.push(e) : (i.debug(`Removed table row for ${e.placeholder.name}:`, e.element), e.element.remove());
+            const a = [],
+                r = [...o].reverse(),
+                l = [...n].reverse();
             let s;
             for (; s = l.pop();) {
-                const t = a.slice(-1)[0];
-                if (t && t.placeholder === s) a.pop(), r.push(t);
+                const n = r.slice(-1)[0];
+                if (n && n.placeholder === s) r.pop(), a.push(n);
                 else {
-                    const t = document.createElement("tr");
-                    0 == r.length ? n.table_element.insertBefore(t, n.table_element.firstChild) : r[r.length - 1].element.insertAdjacentElement("afterend", t), Z(t, s, n.columns, e), r.push({
-                        element: t,
+                    const n = document.createElement("tr");
+                    0 == a.length ? t.table_element.insertBefore(n, t.table_element.firstChild) : a[a.length - 1].element.insertAdjacentElement("afterend", n), ae(n, s, t.columns, e), a.push({
+                        element: n,
                         placeholder: s
-                    }), c.debug(`Added table row for ${s.name}:`, t)
+                    }), i.debug(`Added table row for ${s.name}:`, n)
                 }
             }
-            n.rows = r
+            t.rows = a
         },
-        Q = (e, n, t) => {
-            t.classList.add("input-for-variable"), n.type == V.Checkbox ? ee(e, n, t) : n.type == V.Dropdown ? ne(e, n, t) : n.type == V.Textbox ? te(e, n, t) : console.error(`Placeholder ${n.name} has unknown type '${n.type}'`)
+        le = (e, t, n) => {
+            n.classList.add("input-for-variable"), t.type == X.Checkbox ? se(e, t, n) : t.type == X.Dropdown ? ie(e, t, n) : t.type == X.Textbox ? ce(e, t, n) : console.error(`Placeholder ${t.name} has unknown type '${t.type}'`)
         },
-        ee = (e, n, t) => {
-            t.type = "checkbox", t.checked = n.current_is_checked, n.read_only ? t.disabled = !0 : t.addEventListener("change", (() => {
-                c.debug("Checkbox change", n.name, "- new value:", t.checked), ((e, n) => {
-                    e.current_is_checked = n, e.current_value = n ? e.value_checked : e.value_unchecked, b(`${e.name}_IS_CHECKED`, n ? "1" : "0")
-                })(n, t.checked), n.current_value = t.checked ? n.value_checked : n.value_unchecked, oe(e, n)
-            })), n.input_elements.push(t)
+        se = (e, t, n) => {
+            "INPUT" == n.tagName ? (n.type = "checkbox", n.checked = t.current_is_checked, t.read_only ? n.disabled = !0 : (n.disabled = !1, n.addEventListener("change", (() => {
+                i.debug("Checkbox change", t.name, "- new value:", n.checked), ((e, t) => {
+                    e.current_is_checked = t, e.current_value = t ? e.value_checked : e.value_unchecked, x(`${e.name}_IS_CHECKED`, t ? "1" : "0")
+                })(t, n.checked), t.current_value = n.checked ? t.value_checked : t.value_unchecked, de(e, t)
+            }))), t.input_elements.push(n)) : console.warn(`Input element/tag for placeholder '${t.name}' is expected to be INPUT, but is ${n.tagName}. Skipping`, n)
         },
-        ne = (e, n, t) => {
+        ie = (e, t, n) => {
             const o = document.createElement("select");
             o.classList.add("placeholder-dropdown");
-            for (const e of n.options) {
-                const n = document.createElement("option");
-                n.text = e.display_name, o.appendChild(n)
-            }
-            t.parentNode ? t.parentNode.replaceChild(o, t) : console.error("Input element", t, `for placeholder ${n.name} has no parent!`), o.selectedIndex = n.current_index, n.read_only ? o.disabled = !0 : o.addEventListener("change", (() => {
-                c.debug("Dropdown change", n.name, "- new index:", o.selectedIndex), ((e, n) => {
-                    if (!$(e, n)) throw new Error(`Index must a whole number N, where 0 <= N < ${e.options.length}. But it is ${n}`);
-                    b(`${e.name}_INDEX`, `${n}`), e.current_value = e.options[n].value, e.current_index = n
-                })(n, o.selectedIndex), n.current_index = o.selectedIndex, n.current_value = n.options[o.selectedIndex].value, oe(e, n)
-            })), n.input_elements.push(o)
-        },
-        te = (e, n, t) => {
-            if (t.value = n.current_value, n.read_only) t.disabled = !0, t.style.cursor = "not-allowed";
-            else {
-                null != n.default_value ? t.placeholder = `Default: ${n.default_value}` : t.placeholder = "Dynamic default value";
-                const o = o => {
-                    "Enter" === o.key ? (c.debug("Textbox change confirmed with Enter key for ", n.name, "- new value:", t.value), v(n, t) && (k(n, t.value), n.current_value = t.value, oe(e, n))) : "Escape" === o.key && (c.debug("Resetting input field for ", n.name, " to current placeholder value"), t.value = n.current_value)
-                };
-                0 == n.validators.length || (v(n, t), t.addEventListener("input", (() => {
-                    v(n, t)
-                }))), t.addEventListener("keypress", o)
-            }
-            n.input_elements.push(t)
+            for (const e of t.options) {
+                const t = document.createElement("option");
+                t.text = e.display_name, o.appendChild(t)
+            }
+            n.parentNode ? n.parentNode.replaceChild(o, n) : console.error("Input element", n, `for placeholder ${t.name} has no parent!`), o.selectedIndex = t.current_index, t.read_only ? o.disabled = !0 : (o.disabled = !1, o.addEventListener("change", (() => {
+                i.debug("Dropdown change", t.name, "- new index:", o.selectedIndex), ((e, t) => {
+                    if (!N(e, t)) throw new Error(`Index must a whole number N, where 0 <= N < ${e.options.length}. But it is ${t}`);
+                    x(`${e.name}_INDEX`, `${t}`), e.current_value = e.options[t].value, e.current_index = t
+                })(t, o.selectedIndex), t.current_index = o.selectedIndex, t.current_value = t.options[o.selectedIndex].value, de(e, t)
+            }))), t.input_elements.push(o)
+        },
+        ce = (e, t, n) => {
+            if ("INPUT" == n.tagName) {
+                if (n.value = t.current_value, t.read_only) n.disabled = !0, n.style.cursor = "not-allowed";
+                else {
+                    n.disabled = !1, null != t.default_value ? n.placeholder = `Default: ${t.default_value}` : n.placeholder = "Dynamic default value";
+                    const o = () => {
+                        t.current_value == n.value ? i.debug(`Value for placeholder ${t.name} was not changed`) : v(t, n) && (T(t, n.value), t.current_value = n.value, de(e, t), n.classList.remove("value-modified"))
+                    };
+                    v(t, n), n.addEventListener("input", (() => {
+                        v(t, n), n.value == t.current_value ? n.classList.remove("value-modified") : n.classList.add("value-modified")
+                    })), n.addEventListener("keypress", (e => {
+                        "Enter" === e.key && (i.debug("Textbox change confirmed with Enter key for", t.name, "- new value:", n.value), o())
+                    })), n.addEventListener("keydown", (e => {
+                        "Escape" === e.key && (i.debug("Resetting input field for ", t.name, " to current placeholder value"), n.value = t.current_value)
+                    })), n.addEventListener("focusout", (() => {
+                        e.settings.apply_change_on_focus_change && (i.debug("Textbox change confirmed by changing focus", t.name, "- new value:", n.value), o())
+                    }))
+                }
+                t.input_elements.push(n)
+            } else console.warn(`Input element/tag for placeholder '${t.name}' is expected to be INPUT, but is ${n.tagName}. Skipping`, n)
         },
-        oe = (e, n) => {
-            const t = e.dependency_graph.get_all_upstream(n);
+        de = (e, t) => {
+            const n = e.dependency_graph.get_all_upstream(t);
             let o = !1;
-            for (const e of t) o = o || e.reload_page_on_change;
-            if (c.debug(`Change of ${n.name} requires updates for placeholders:\n${t.map((e=>` - ${e.name}\n`)).join("")}\nRequires reload: ${o}`), o) l();
+            for (const e of n) o = o || e.reload_page_on_change;
+            if (i.debug(`Change of ${t.name} requires updates for placeholders:\n${n.map((e=>` - ${e.name}\n`)).join("")}\nRequires reload: ${o}`), o) l();
             else {
-                if (e.dependency_graph.on_placeholder_value_change(n), (e => {
-                        if (c.debug(`Updating ${e.input_tables.length} automatic input tables`), e.input_tables.length > 0) {
-                            const n = e.dependency_graph.get_all_used_placeholders();
-                            for (const t of e.input_tables) z(e, t, n)
+                if (e.dependency_graph.on_placeholder_value_change(t), (e => {
+                        if (i.debug(`Updating ${e.input_tables.length} automatic input tables`), e.input_tables.length > 0) {
+                            const t = e.dependency_graph.get_all_used_placeholders();
+                            for (const n of e.input_tables) re(e, n, t)
                         }
-                    })(e), n.type == V.Checkbox) {
-                    const e = n;
-                    for (const n of e.input_elements) n.checked = e.current_is_checked
-                } else if (n.type == V.Dropdown) {
-                    const e = n;
-                    for (const n of e.input_elements) n.selectedIndex = e.current_index
-                } else if (n.type == V.Textbox) {
-                    const e = n;
-                    for (const n of e.input_elements) n.value = e.current_value, v(e, n)
-                } else console.warn(`Placeholder ${n.name} has unexpected type '${n.type}'`);
-                D(t)
+                    })(e), t.type == X.Checkbox) {
+                    const e = t;
+                    for (const t of e.input_elements) t.checked = e.current_is_checked
+                } else if (t.type == X.Dropdown) {
+                    const e = t;
+                    for (const t of e.input_elements) t.selectedIndex = e.current_index
+                } else if (t.type == X.Textbox) {
+                    const e = t;
+                    for (const t of e.input_elements) t.value = e.current_value, v(e, t)
+                } else console.warn(`Placeholder ${t.name} has unexpected type '${t.type}'`);
+                H(n)
             }
         },
-        re = () => {
+        ue = () => {
             const e = (e => {
-                const n = new Map,
-                    t = new Map,
+                const t = new Map,
+                    n = new Map,
                     o = new Map,
-                    r = new Map,
                     a = new Map,
-                    l = U("validators", "object", e);
+                    r = new Map,
+                    l = F("validators", "object", e);
                 for (const e of l) {
-                    const n = p(e);
-                    if (a.has(n.id)) throw new Error(`Multiple validators with id '${n.id}'`);
-                    a.set(n.id, n)
-                }
-                const s = (e => ({
-                        debug: H("debug", e),
-                        delay_millis: M("delay_millis", e),
-                        normal_prefix: "x",
-                        normal_suffix: "x",
-                        html_prefix: "i",
-                        html_suffix: "i",
-                        static_prefix: "s",
-                        static_suffix: "s",
-                        dynamic_prefix: "d",
-                        dynamic_suffix: "d"
-                    }))(j("settings", "object", e)),
-                    c = U("placeholder_list", "object", e);
-                for (let e = 0; e < c.length; e++) {
-                    const l = W(c[e], a, s, e);
-                    n.set(l.name, l), l.type == V.Textbox ? t.set(l.name, l) : l.type == V.Checkbox ? o.set(l.name, l) : l.type == V.Dropdown ? r.set(l.name, l) : console.warn("Unknown placeholder type:", l.type)
+                    const t = f(e);
+                    if (r.has(t.id)) throw new Error(`Multiple validators with id '${t.id}'`);
+                    r.set(t.id, t)
+                }
+                const s = (e => {
+                        const t = z("apply_change_on_focus_change", e),
+                            n = z("debug", e),
+                            o = z("expand_auto_tables", e);
+                        return {
+                            apply_change_on_focus_change: $("apply_change_on_focus_change", t),
+                            debug: $("debug", n),
+                            delay_millis: J("delay_millis", e),
+                            expand_auto_tables: $("expand_auto_tables", o),
+                            highlight_placeholders: $("highlight_placeholders", !1),
+                            normal_prefix: W("normal_prefix", e),
+                            normal_suffix: W("normal_suffix", e),
+                            html_prefix: W("html_prefix", e),
+                            html_suffix: W("html_suffix", e),
+                            static_prefix: W("static_prefix", e),
+                            static_suffix: W("static_suffix", e),
+                            dynamic_prefix: W("dynamic_prefix", e),
+                            dynamic_suffix: W("dynamic_suffix", e)
+                        }
+                    })(V("settings", "object", e)),
+                    i = F("placeholder_list", "object", e);
+                for (let e = 0; e < i.length; e++) {
+                    const l = B(i[e], r, s, e);
+                    t.set(l.name, l), l.type == X.Textbox ? n.set(l.name, l) : l.type == X.Checkbox ? o.set(l.name, l) : l.type == X.Dropdown ? a.set(l.name, l) : console.warn("Unknown placeholder type:", l.type)
                 }
                 return {
-                    placeholders: n,
-                    textboxes: t,
+                    placeholders: t,
+                    textboxes: n,
                     checkboxes: o,
-                    dropdowns: r,
+                    dropdowns: a,
                     settings: s,
-                    dependency_graph: new I(n),
+                    dependency_graph: new j(t),
                     input_tables: []
                 }
             })(window.PlaceholderPluginConfigJson);
-            var n;
-            n = e.settings.debug, c = n ? {
-                log: t,
+            var t;
+            t = e.settings.debug, i = t ? {
+                log: n,
                 info: o,
-                debug: r
-            } : s, c.info("PluginConfig", e), (e => {
+                debug: a
+            } : s, i.info("PluginConfig", e), (e => {
                 window.PlaceholderPlugin = {
                     settings: e.settings,
                     placeholders: e.placeholders,
-                    debug_disable_reload: i,
+                    debug_disable_reload: c,
                     debug_print_dependency_graph: () => e.dependency_graph.debug_print_representation()
                 }
             })(e);
-            const a = e.settings.delay_millis;
-            a < 0 ? ae(e) : 0 == a ? window.addEventListener("load", (() => ae(e))) : window.addEventListener("load", (() => {
-                setTimeout((() => ae(e)), a)
+            const r = e.settings.delay_millis;
+            r < 0 ? fe(e) : 0 == r ? window.addEventListener("load", (() => fe(e))) : window.addEventListener("load", (() => {
+                setTimeout((() => fe(e)), r)
             }))
         },
-        ae = e => {
-            ((e, n) => {
-                for (const t of n.placeholders.values()) C(e, t), L(e, t), R(e, t), t.allow_inner_html && O(e, t);
+        fe = e => {
+            ((e, t) => {
+                for (const n of t.placeholders.values()) S(e, n), P(e, n), D(e, n), n.allow_inner_html && O(e, n);
                 (e => {
-                    const n = document.querySelectorAll(".placeholder-value[data-placeholder]");
-                    for (const t of n) {
-                        const n = t.getAttribute("data-placeholder");
-                        if (n) {
-                            const o = e.placeholders.get(n);
-                            o ? o.output_elements.push(t) : console.warn(`No placeholder named '${n}', that is referenced by element:`, t)
-                        } else console.warn("Element has empty/no attribute 'data-placeholder':", t)
+                    const t = document.querySelectorAll(".placeholder-value[data-placeholder]");
+                    for (const n of t) {
+                        const t = n.getAttribute("data-placeholder");
+                        if (t) {
+                            const o = e.placeholders.get(t);
+                            o ? o.output_elements.push(n) : console.warn(`No placeholder named '${t}', that is referenced by element:`, n)
+                        } else console.warn("Element has empty/no attribute 'data-placeholder':", n)
                     }
-                })(n), D([...n.placeholders.values()])
+                })(t), H([...t.placeholders.values()])
             })(document.body, e), e.dependency_graph.debug_print_representation(), (e => {
-                const n = document.querySelectorAll("input[data-input-for]");
-                for (let t of n) {
-                    const n = t.getAttribute("data-input-for");
-                    if (null == n) throw new Error("How can this be, the selector forces the 'data-input-for' attribute to exist");
-                    const o = e.placeholders.get(n);
-                    o ? Q(e, o, t) : (console.warn(`Unknown placeholder referenced in input element: '${n}'`), t.classList.add("input-for-variable"), t.value = `ERROR_UNDEFINED_PLACEHOLDER: ${n}`)
+                const t = document.querySelectorAll("input[data-input-for], select[data-input-for]");
+                for (let n of t) {
+                    const t = n.getAttribute("data-input-for");
+                    if (null == t) throw new Error("How can this be, the selector forces the 'data-input-for' attribute to exist");
+                    const o = e.placeholders.get(t);
+                    o ? le(e, o, n) : (console.warn(`Unknown placeholder referenced in input element: '${t}'`), n.classList.add("input-for-variable"), n.value = `ERROR_UNDEFINED_PLACEHOLDER: ${t}`)
                 }
             })(e), (e => {
-                const n = document.querySelectorAll("div.auto-input-table");
-                if (n.length > 0) {
-                    const t = e.dependency_graph.get_all_used_placeholders().filter((e => !e.read_only));
-                    for (let o of n) {
-                        const n = o.getAttribute("data-columns") || "name,input",
-                            r = n.includes(",") ? n.split(",") : [n];
-                        K(o, r, e, t)
-                    }
+                const t = document.querySelectorAll("div.auto-input-table");
+                if (t.length > 0) {
+                    const n = e.dependency_graph.get_all_used_placeholders().filter((e => !e.read_only));
+                    for (const o of t)
+                        if (o instanceof HTMLElement) {
+                            const t = o.getAttribute("data-columns") || "name,input",
+                                a = t.includes(",") ? t.split(",") : [t],
+                                r = null === o.getAttribute("data-hide-empty");
+                            ne(o, a, e, n, r)
+                        } else console.warn("Element", o, "is expected to be an HTMLElement, but is not")
                 }
             })(e)
         };
-    window.PlaceholderPluginConfigJson ? re() : document.addEventListener("PlaceholderPluginConfigJson", re)
+    window.PlaceholderPluginConfigJson ? ue() : document.addEventListener("PlaceholderPluginConfigJson", ue)
 })();
 //# sourceMappingURL=placeholder.min.js.map
```

### Comparing `mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/assets/placeholder.min.js.map` & `mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/assets/placeholder.min.js.map`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8657004086038086%*

 * *Differences: {"'mappings'": "'mBAAA,MAAMA,EAAY,IAAM,IAAG,IAAIC,MAAOC,cAAcC,MAAM,GAAI,WAC9D,IAAIC,GAAoB,EACxB,SAASC,KAAgBC,GACrBC,QAAQC,IAAIC,MAAMF,QAAS,CAAC,GAAGP,WAAoBU,WACvD,CACA,SAASC,KAAiBL,GACtBC,QAAQK,KAAKH,MAAMF,QAAS,CAAC,GAAGP,WAAoBU,WACxD,CACA,SAASG,KAAkBP,GACvBC,QAAQO,MAAML,MAAMF,QAAS,CAAC,GAAGP,WAAoBU,WACzD,CACA,SAASK,KAAQT,GACjB,CACO,MAAMU,EAAc,KACnBZ,EACAa,OAAOC,SAASC,SAGhBR,EAAc,sFAClB,EAEES,EAAc,CAChB,IAAOL,EACP,KAAQA,EACR,MAASA,GAiBN,IAAIM,EAASD,EAEb,MAAME,EAAuB,KAChCX,EAAc,mDACdP,GAAoB,CAAK,EC3CtB,IAAIm […]*

```diff
@@ -1,10 +1,10 @@
 {
     "file": "placeholder.min.js",
-    "mappings": "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",
+    "mappings": "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",
     "names": [
         "timestamp",
         "Date",
         "toISOString",
         "slice",
         "is_reload_enabled",
         "internal_log",
@@ -89,20 +89,27 @@
         "remove",
         "rating",
         "add",
         "title",
         "update_tooltip",
         "name",
         "STORAGE_PREFIX",
+        "SETTINGS_PREFIX",
         "store_value",
         "localStorage",
         "setItem",
         "load_value",
         "getItem",
+        "load_boolean_setting",
+        "default_value",
+        "stored",
         "clear_state",
+        "clear_by_prefix",
+        "clear_settings",
+        "prefix",
         "i",
         "key",
         "startsWith",
         "removeItem",
         "is_valid_index",
         "index",
         "item",
@@ -123,23 +130,29 @@
         "span",
         "dataset",
         "textContent",
         "expanded_value",
         "dynamic_replace",
         "root_element",
         "search_regex",
+        "search_for_pre_replaced",
         "_a",
         "walker",
         "createTreeWalker",
         "NodeFilter",
         "SHOW_TEXT",
         "node",
         "global",
         "source",
         "current_value",
+        "existing_count",
+        "already_existing_wrappers",
+        "querySelectorAll",
+        "wrapper",
+        "getAttribute",
         "nodes_to_modify",
         "nextNode",
         "nodeValue",
         "match",
         "replacement_value",
         "replaced_str",
         "replace",
@@ -156,14 +169,15 @@
         "do_static_replace",
         "static_replace",
         "regex_static",
         "reload_page_on_change",
         "do_html_replace",
         "inner_html_replace",
         "regex_html",
+        "replace_placeholder_in_string_with",
         "replace_dynamic_placeholder_values",
         "placeholder_list",
         "output_elements",
         "DependencyGraph",
         "constructor",
         "placeholders",
         "this",
@@ -185,15 +199,15 @@
         "get_node",
         "get",
         "update_placeholder_downlinks",
         "has_loop",
         "get_all_marked",
         "get_all_upstream",
         "recursive_mark_upstream",
-        "allow_recursive",
+        "allow_nested",
         "old_downlink",
         "remove_uplink",
         "other_node",
         "string_contains_placeholder",
         "uplinks",
         "get_all_used_placeholders",
         "recursive_mark_downstream",
@@ -203,29 +217,35 @@
         "new_back_stack",
         "indexOf",
         "child",
         "string_to_test",
         "placeholder_to_find",
         "filter",
         "recursive",
-        "downlink_node",
+        "unique",
+        "now",
+        "Math",
+        "random",
+        "safe_replace_multiple_placeholders_in_string",
         "uplink_node",
         "assert_field_type",
         "expected_type_str",
         "parent_object",
         "actual_type_str",
         "get_number_field",
         "element_type",
         "array",
         "Array",
         "isArray",
         "entry",
         "entries",
         "msg",
         "InputType",
+        "escapeRegExp",
+        "regex_pattern",
         "parse_any_placeholder",
         "validator_map",
         "settings",
         "type",
         "parsed",
         "dynamic_prefix",
         "dynamic_suffix",
@@ -233,15 +253,14 @@
         "html_suffix",
         "normal_prefix",
         "normal_suffix",
         "static_prefix",
         "static_suffix",
         "finish_parse_textbox",
         "stored_state",
-        "default_value",
         "default_function",
         "load_textbox_state",
         "finish_parse_checkbox",
         "current_is_checked",
         "checked_by_default",
         "value_checked",
         "value_unchecked",
@@ -267,31 +286,68 @@
         "option",
         "Dropdown",
         "TABLE_CELL_HEADINGS",
         "appendTextNode",
         "createChildElement",
         "parent",
         "tag_name",
+        "append_boolean_setting_checkbox",
+        "parent_element",
+        "label_text",
+        "custom_on_change",
+        "enabled",
+        "label",
+        "checkbox",
+        "checked",
+        "addEventListener",
+        "store_boolean_setting",
         "generate_automatic_placeholder_table",
         "columns",
         "placeholders_to_show",
+        "show_empty",
         "sort_and_remove_duplicate_placeholders",
-        "div",
         "table",
         "table_head",
         "table_head_row",
         "table_body",
         "column",
         "table_cell",
         "heading",
         "rows",
         "read_only",
         "row",
         "populate_auto_table_row",
         "input_tables",
+        "content_element",
+        "title_text",
+        "settings_button",
+        "expandable_contents",
+        "settings_contents",
+        "append",
+        "update_expanded_state",
+        "is_expanded",
+        "style",
+        "display",
+        "expanded",
+        "expand_auto_tables",
+        "expand_if_needed",
+        "show_settings",
+        "onclick",
+        "preventDefault",
+        "stopPropagation",
+        "prepare_settings_button",
+        "set_highlight_placeholders",
+        "output",
+        "highlight_placeholders",
+        "apply_change_on_focus_change",
+        "settings_button_bar",
+        "settings_reset_button",
+        "placeholder_reset_button",
+        "fill_settings_content_container",
+        "convert_to_dynamic_placeholder_table",
         "Set",
         "sort",
         "a",
         "b",
         "order_index",
         "cell",
         "description",
@@ -313,29 +369,27 @@
         "insertBefore",
         "firstChild",
         "insertAdjacentElement",
         "input_element",
         "initialize_input_checkbox",
         "initialize_input_dropdown",
         "initialize_input_textbox",
-        "checked",
+        "tagName",
         "disabled",
-        "addEventListener",
         "new_is_checked",
         "store_checkbox_state",
         "on_placeholder_change",
         "input_elements",
         "option_element",
         "parentNode",
         "selectedIndex",
         "new_index",
         "store_dropdown_state",
-        "style",
         "cursor",
-        "on_keypress",
+        "confirm_change",
         "event",
         "affected_placeholders",
         "dependency_graph",
         "require_reload",
         "ph",
         "p",
         "update_all_auto_tables",
@@ -343,36 +397,38 @@
         "placeholder_map",
         "textboxes",
         "checkboxes",
         "dropdowns",
         "validator_data_list",
         "validator_data",
         "has",
+        "apply_change_on_focus_change_default",
+        "debug_default",
+        "expand_auto_tables_default",
         "parse_settings",
         "placeholder_data",
         "parse_config",
         "PlaceholderPluginConfigJson",
         "enable_debug",
         "PlaceholderPlugin",
         "export_api_functions",
         "delay_millis",
         "do_plugin_stuff",
         "setTimeout",
         "allow_inner_html",
         "output_list",
-        "querySelectorAll",
         "placeholder_name",
-        "getAttribute",
         "find_dynamic_placeholder_wrappers",
         "replace_placeholders_in_subtree",
         "body",
         "input_list",
         "initialize_all_input_fields",
         "element_list",
         "used_placeholders",
+        "HTMLElement",
         "columns_str",
         "split",
         "initialize_auto_tables"
     ],
     "sourceRoot": "",
     "sources": [
         "webpack:///./src/debug.ts",
@@ -386,19 +442,19 @@
         "webpack:///./src/main.ts",
         "webpack:///./src/api.ts",
         "webpack:///./src/index.ts"
     ],
     "sourcesContent": [
         "const timestamp = () => `${new Date().toISOString().slice(11, 23)} (TS)`;\nlet is_reload_enabled = true;\nfunction internal_log(...args) {\n    console.log.apply(console, [`${timestamp()} |`, ...arguments]);\n}\nfunction internal_info(...args) {\n    console.info.apply(console, [`${timestamp()} |`, ...arguments]);\n}\nfunction internal_debug(...args) {\n    console.debug.apply(console, [`${timestamp()} |`, ...arguments]);\n}\nfunction noop(...args) {\n}\nexport const reload_page = () => {\n    if (is_reload_enabled) {\n        window.location.reload();\n    }\n    else {\n        internal_info(\"Page reload was triggered and blocked due to PlaceholderPlugin.debug_disable_reload\");\n    }\n};\nconst noop_logger = {\n    \"log\": noop,\n    \"info\": noop,\n    \"debug\": noop,\n};\nexport const init_logging = (enable_debug) => {\n    if (enable_debug) {\n        // Write debugging messages to console\n        logger = {\n            \"log\": internal_log,\n            \"info\": internal_info,\n            \"debug\": internal_debug,\n        };\n    }\n    else {\n        // If debugging is disabled, make the functions do nothing\n        logger = noop_logger;\n        return;\n    }\n};\nexport let logger = noop_logger;\n// You can call this manually from the browser's console to temporarily disable reloads and debug the application\nexport const debug_disable_reload = () => {\n    internal_info(\"Page reload was disabled for debugging purposes\");\n    is_reload_enabled = false;\n};\n",
         "import { logger } from \"./debug\";\nimport { get_array_field, get_boolean_field, get_string_field } from \"./parse_settings\";\nexport var ValidatorSeverity;\n(function (ValidatorSeverity) {\n    ValidatorSeverity[\"Warning\"] = \"WARNING\";\n    ValidatorSeverity[\"Error\"] = \"ERROR\";\n})(ValidatorSeverity || (ValidatorSeverity = {}));\nexport var PlaceholderValidatity;\n(function (PlaceholderValidatity) {\n    PlaceholderValidatity[\"Good\"] = \"GOOD\";\n    PlaceholderValidatity[\"Warning\"] = \"WARNING\";\n    PlaceholderValidatity[\"Error\"] = \"ERROR\";\n    PlaceholderValidatity[\"NoValidator\"] = \"NO_VALIDATOR\";\n})(PlaceholderValidatity || (PlaceholderValidatity = {}));\nexport const parse_validator = (data) => {\n    const rules = get_array_field(\"rules\", \"object\", data);\n    if (rules.length == 0) {\n        throw new Error(`Rules should not be an empty array.\\nProblematic object: ${JSON.stringify(data)}`);\n    }\n    const id = get_string_field(\"id\", data);\n    return {\n        \"display_name\": get_string_field(\"display_name\", data),\n        \"id\": id,\n        \"rules\": rules.map(x => parse_rule(x, id)),\n    };\n};\nconst is_valid_value = (validator, value) => {\n    for (const rule of validator.rules) {\n        if (rule.is_match_function(value) != rule.should_match) {\n            // this rule rejects the value\n            if (rule.severity == ValidatorSeverity.Error) {\n                // immediately return once we found a hard failure\n                return false;\n            }\n        }\n    }\n    // no real errors -> is valid\n    return true;\n};\nexport const is_valid_value_for_placeholder = (placeholder, value) => {\n    // @TODO decide: validate normal value or expanded value? Needs to be checked for every function call\n    if (placeholder.validators.length > 0) {\n        for (const validator of placeholder.validators) {\n            if (is_valid_value(validator, value)) {\n                // a single validator accepting it is enough\n                return true;\n            }\n        }\n        // no validator accepted it -> bad\n        return false;\n    }\n    else {\n        return true;\n    }\n};\nconst validate_value = (validator, value) => {\n    const warnings = [];\n    const errors = [];\n    for (const rule of validator.rules) {\n        if (rule.is_match_function(value) != rule.should_match) {\n            // this rule rejects the value\n            if (rule.severity == ValidatorSeverity.Error) {\n                errors.push(`[${validator.display_name}] Error: ${rule.error_message}`);\n            }\n            else if (rule.severity == ValidatorSeverity.Warning) {\n                warnings.push(`[${validator.display_name}] Warning: ${rule.error_message}`);\n            }\n            else {\n                console.warn(`Unknown rule severity ${rule.severity}`);\n            }\n        }\n    }\n    return {\n        \"errors\": errors,\n        \"warnings\": warnings,\n    };\n};\nconst validate_placeholder_value = (placeholder, value) => {\n    const result_list = [];\n    let has_no_error = false; // whether at least one placeholder has no errors\n    if (placeholder.validators.length > 0) {\n        for (const validator of placeholder.validators) {\n            const result = validate_value(validator, value);\n            result_list.push(result);\n            if (result.errors.length == 0) {\n                has_no_error = true;\n                if (result.warnings.length == 0) {\n                    return placeholder_is_good(placeholder);\n                }\n            }\n        }\n        if (has_no_error) {\n            return placeholder_is_warning(result_list);\n        }\n        else {\n            return placeholder_is_error(result_list);\n        }\n    }\n    else {\n        return {\n            \"rating\": PlaceholderValidatity.NoValidator,\n            \"message\": \"No validators are specified for this placeholder\",\n        };\n    }\n};\nconst placeholder_is_error = (result_list) => {\n    // If all of them have errors, we will ignore the warnings to keep it shorter\n    const errors = [];\n    for (const result of result_list) {\n        errors.push(...result.errors);\n    }\n    return {\n        \"rating\": PlaceholderValidatity.Error,\n        \"message\": errors.join(\"\\n\"),\n    };\n};\nconst placeholder_is_warning = (result_list) => {\n    // If some return warnings and some return errors, we will only show the ones with warnings.\n    const lines = [];\n    for (const result of result_list) {\n        if (result.errors.length == 0) {\n            lines.push(...result.warnings);\n        }\n    }\n    return {\n        \"rating\": PlaceholderValidatity.Warning,\n        \"message\": lines.join(\"\\n\"),\n    };\n};\nconst placeholder_is_good = (placeholder) => {\n    // If one of them has neither warnings or errors, we return Good status immediately\n    let message;\n    if (placeholder.validators.length == 1) {\n        message = `Expecting: ${placeholder.validators[0].display_name}`;\n    }\n    else {\n        message = \"Expecting one of the following: \";\n        for (const v of placeholder.validators) {\n            message += `\\n - ${v.display_name}`;\n        }\n    }\n    return {\n        \"rating\": PlaceholderValidatity.Good,\n        \"message\": message,\n    };\n};\nconst parse_rule = (data, validator_id) => {\n    const severity_str = get_string_field(\"severity\", data);\n    let severity;\n    if (severity_str == \"warning\" || severity_str == \"warn\") {\n        severity = ValidatorSeverity.Warning;\n    }\n    else if (severity_str == \"error\") {\n        severity = ValidatorSeverity.Error;\n    }\n    else {\n        throw new Error(`Unknown severity '${severity_str}'`);\n    }\n    let is_match_function;\n    if (data.regex) {\n        const regex = get_string_field(\"regex\", data);\n        const compiled_regex = new RegExp(regex);\n        is_match_function = (value) => compiled_regex.test(value);\n    }\n    else {\n        const match_function_body = get_string_field(\"match_function\", data);\n        // we need to use Function instead of eval(), since minification will rename the argument\n        // this may also be more performant, since the code is only compiled once\n        const match_function = new Function(\"value\", match_function_body);\n        is_match_function = (value) => {\n            try {\n                const result = match_function(value);\n                if (typeof (result) != \"boolean\") {\n                    throw new Error(`Custom match_function '${match_function_body}' of validator ${validator_id} should return a boolean, but it returned a ${typeof (result)}: ${result}`);\n                }\n                else {\n                    return result;\n                }\n            }\n            catch (error) {\n                throw new Error(`Failed to evaluate match_function '${match_function_body}' of validator ${validator_id}: ${error}`);\n            }\n        };\n    }\n    return {\n        \"severity\": severity,\n        \"should_match\": get_boolean_field(\"should_match\", data),\n        \"error_message\": get_string_field(\"error_message\", data),\n        \"is_match_function\": is_match_function,\n    };\n};\nconst update_tooltip = (input_field, validation_result) => {\n    // Set highlighting\n    input_field.classList.remove(\"validation-error\", \"validation-warn\", \"validation-ok\", \"validation-none\");\n    if (validation_result.rating == PlaceholderValidatity.Good) {\n        input_field.classList.add(`validation-ok`);\n    }\n    else if (validation_result.rating == PlaceholderValidatity.Warning) {\n        input_field.classList.add(`validation-warn`);\n    }\n    else if (validation_result.rating == PlaceholderValidatity.Error) {\n        input_field.classList.add(`validation-error`);\n    }\n    else if (validation_result.rating == PlaceholderValidatity.NoValidator) {\n        input_field.classList.add(`validation-none`);\n    }\n    else {\n        console.warn(`Unknown placeholder validity: ${validation_result.rating}`);\n    }\n    // Set tooltip\n    input_field.title = validation_result.message;\n};\n// Returns \"false\" if the value has an error, so for example page reloading should be cancelled.\nexport const validate_textbox_input_field = (placeholder, input_field) => {\n    const result = validate_placeholder_value(placeholder, input_field.value);\n    update_tooltip(input_field, result);\n    logger.debug(\"Validation: name =\", placeholder.name, \", value =\", input_field.value, \", results =\", result.rating);\n    const can_accept_value = result.rating != PlaceholderValidatity.Error;\n    return can_accept_value;\n};\n",
-        "import { logger, reload_page } from \"./debug\";\nimport { is_valid_value_for_placeholder } from \"./validator\";\n// These functions are here to make it easier to change the storage backend (for example locasstorage -> cookies)\n// and to make it possible to potentially have better debugging\nconst STORAGE_PREFIX = \"PLACEHOLDER_\"; // @TODO make it configurable by settings?\nconst store_value = (name, value) => {\n    localStorage.setItem(STORAGE_PREFIX + name, value);\n};\nconst load_value = (name) => {\n    return localStorage.getItem(STORAGE_PREFIX + name);\n};\n// I changed the storage model: the real value is stored in the placeholder object instead of in localstorage -> easier and safer to access\n// We pass the whole placeholder instead of just a name, so that you can not accidentally call the wrong function or use an invalid placeholder name\n// We use different values for different types (checkbox -> NAME_IS_CHECKED, textbox -> NAME_TEXT, ...) so that if a user changes the type of a placeholder it should not cause problems\nexport const store_checkbox_state = (placeholder, new_is_checked) => {\n    // Update the placeholder's value\n    placeholder.current_is_checked = new_is_checked;\n    placeholder.current_value = new_is_checked ? placeholder.value_checked : placeholder.value_unchecked;\n    // Permanently store the new state\n    store_value(`${placeholder.name}_IS_CHECKED`, new_is_checked ? \"1\" : \"0\");\n};\nexport const load_checkbox_state = (placeholder) => {\n    const stored_state = load_value(`${placeholder.name}_IS_CHECKED`);\n    if (stored_state == null) {\n        // No stored state -> use default value\n        placeholder.current_is_checked = placeholder.checked_by_default;\n    }\n    else {\n        if (stored_state == \"0\" || stored_state == \"1\") {\n            // Load the stored state\n            placeholder.current_is_checked = stored_state == \"1\";\n        }\n        else {\n            // Unexpected state, warn user and fall back to default\n            console.warn(`Unexpected state for checkbox. Should be '0' or '1', but was '${stored_state}'`);\n            placeholder.current_is_checked = placeholder.checked_by_default;\n        }\n    }\n    // Now we update the actual value based on the state\n    placeholder.current_value = placeholder.current_is_checked ? placeholder.value_checked : placeholder.value_unchecked;\n};\nexport const clear_state = () => {\n    // The easiest way would be to clear the whole storage, but that might break other plugins / scripts.\n    // So we only delete all items that start with our prefix\n    console.warn(`Clearing all localStorage items starting with '${STORAGE_PREFIX}'`);\n    let i = 0;\n    while (i < localStorage.length) {\n        const key = localStorage.key(i);\n        if (key === null || key === void 0 ? void 0 : key.startsWith(STORAGE_PREFIX)) {\n            // Delete the item\n            localStorage.removeItem(key);\n        }\n        else {\n            // Not ours, so we skip it\n            i++;\n        }\n    }\n    reload_page();\n};\nconst is_valid_index = (placeholder, index) => {\n    try {\n        const item = placeholder.options[index];\n        return item != undefined && item != null;\n    }\n    catch (error) {\n        return false;\n    }\n};\nexport const store_dropdown_state = (placeholder, new_index) => {\n    // Perform sanity checks on the index\n    if (is_valid_index(placeholder, new_index)) {\n        store_value(`${placeholder.name}_INDEX`, `${new_index}`);\n        placeholder.current_value = placeholder.options[new_index].value;\n        placeholder.current_index = new_index;\n    }\n    else {\n        throw new Error(`Index must a whole number N, where 0 <= N < ${placeholder.options.length}. But it is ${new_index}`);\n    }\n};\nexport const load_dropdown_state = (placeholder) => {\n    const stored_state = load_value(`${placeholder.name}_INDEX`);\n    if (stored_state == null) {\n        // No stored state -> use default value\n        placeholder.current_index = placeholder.default_index;\n    }\n    else {\n        const stored_index = Number(stored_state);\n        if (is_valid_index(placeholder, stored_index)) {\n            // Load the stored state\n            placeholder.current_index = stored_index;\n        }\n        else {\n            // Unexpected state, warn user and fall back to default\n            console.warn(`Unexpected state for dropdown. Should be a whole number N, where 0 <= N < ${placeholder.options.length}. But it is ${stored_state}`);\n            placeholder.current_index = placeholder.default_index;\n        }\n    }\n    // Now we update the actual value based on the state\n    placeholder.current_value = placeholder.options[placeholder.current_index].value;\n};\nexport const store_textbox_state = (placeholder, new_value) => {\n    const is_validation_ok = is_valid_value_for_placeholder(placeholder, new_value);\n    logger.info(`Set textbox ${placeholder.name} to '${new_value}'. Validation ok? ${is_validation_ok}`);\n    if (is_validation_ok) {\n        store_value(`${placeholder.name}_TEXT`, new_value);\n    }\n    else {\n        throw new Error(`Validation error: Value '${new_value}' is not valid for placeholder ${placeholder.name}`);\n    }\n};\nexport const load_textbox_state = (placeholder) => {\n    const stored_state = load_value(`${placeholder.name}_TEXT`);\n    if (stored_state != null) {\n        if (is_valid_value_for_placeholder(placeholder, stored_state)) {\n            placeholder.current_value = stored_state;\n            return; // Do not use the default value / function\n        }\n        else {\n            console.warn(`Stored value for placeholder ${placeholder.name} is invalid: '${stored_state}'. Will revert to default.`);\n            // Should we remove the value? Idk\n        }\n    }\n    // Use a default value\n    if (placeholder.default_value != undefined) {\n        placeholder.current_value = placeholder.default_value;\n        if (!is_valid_value_for_placeholder(placeholder, placeholder.default_value)) {\n            console.warn(`Default value for placeholder '${placeholder.name}' is invalid: '${placeholder.default_value}'`);\n        }\n    }\n    else if (placeholder.default_function) {\n        try {\n            const result = placeholder.default_function();\n            placeholder.current_value = result;\n            try {\n                // store the function result, since it may be different with each invocation (such as a randomly generated password)\n                store_textbox_state(placeholder, result);\n            }\n            catch (error) {\n                console.warn(`Default function for placeholder '${placeholder.name}' returned invalid value: '${result}'`);\n            }\n        }\n        catch (error) {\n            // This will be called if the placeholder's custom function fails\n            console.error(`Error while loading default textbox state for placeholder ${placeholder.name}:`, error);\n            placeholder.current_value = \"DEFAULT_FUNCTION_ERROR\";\n        }\n    }\n    else {\n        throw new Error(`Either 'default_value' or 'default_function' needs to be set for placeholder ${placeholder.name}`);\n    }\n};\n",
-        "import { logger } from \"./debug\";\n// Replace a specific placeholder and return the estimated number of occurences (underestimated, may actually be higher)\nconst static_replace = (root_element, search_regex, replacement_value) => {\n    const walker = document.createTreeWalker(root_element, NodeFilter.SHOW_TEXT);\n    let node;\n    let count = 0;\n    if (!search_regex.global) {\n        console.warn(`You should set the global flag for the regex. Context: replacing '${search_regex.source}' with '${replacement_value}'`);\n    }\n    while (node = walker.nextNode()) {\n        if (node.nodeValue) {\n            const replaced_str = node.nodeValue.replace(search_regex, replacement_value);\n            if (node.nodeValue != replaced_str) {\n                node.nodeValue = replaced_str;\n                count++; // Of course, it might have been replaced multiple times by replaceAll. But this is just for debugging\n                // and performing an accurate count would impact the performace.\n            }\n        }\n    }\n    return count;\n};\nconst escapeHTML = (text) => {\n    const element = document.createElement(\"div\");\n    element.appendChild(document.createTextNode(text));\n    return element.innerHTML;\n};\nconst inner_html_replace = (root_element, search_regex, replacement_value) => {\n    // User supplied input, HTML escape it before we inject it in the page\n    replacement_value = escapeHTML(replacement_value);\n    if (!search_regex.global) {\n        console.warn(`You should set the global flag for the regex. Context: replacing '${search_regex.source}' with '${replacement_value}'`);\n    }\n    const new_value = root_element.innerHTML.replace(search_regex, replacement_value);\n    if (new_value != root_element.innerHTML) {\n        root_element.innerHTML = new_value;\n        return 1;\n    }\n    else {\n        return 0;\n    }\n};\nexport const create_dynamic_placeholder_element = (placeholder) => {\n    const span = document.createElement(\"span\");\n    span.classList.add(\"placeholder-value\");\n    span.dataset.placeholder = placeholder.name;\n    span.textContent = placeholder.expanded_value;\n    return span;\n};\nconst dynamic_replace = (root_element, search_regex, placeholder) => {\n    var _a;\n    const walker = document.createTreeWalker(root_element, NodeFilter.SHOW_TEXT);\n    let node;\n    if (!search_regex.global) {\n        console.warn(`You should set the global flag for the regex. Context: replacing '${search_regex.source}' with '${placeholder.current_value}'`);\n    }\n    const nodes_to_modify = [];\n    while (node = walker.nextNode()) {\n        if (node.nodeValue) {\n            if (node.nodeValue.match(search_regex)) {\n                // Do not modify in-place while iterating over the DOM\n                nodes_to_modify.push(node);\n            }\n        }\n    }\n    // Do not put in the value yet, otherwise it may be replaced by other placeholders\n    const replacement_value = `<span class=\"placeholder-value\" data-placeholder=\"${escapeHTML(placeholder.name)}\">TEMPORARY PLACEHOLDER</span>`;\n    for (const node of nodes_to_modify) {\n        if (node.nodeValue) {\n            const replaced_str = escapeHTML(node.nodeValue).replace(search_regex, replacement_value);\n            const new_node = document.createElement(\"span\");\n            new_node.innerHTML = replaced_str;\n            (_a = node.parentElement) === null || _a === void 0 ? void 0 : _a.replaceChild(new_node, node);\n        }\n    }\n    return nodes_to_modify.length;\n};\nconst do_dynamic_replace = (root_element, placeholder, config) => {\n    const count = dynamic_replace(root_element, placeholder.regex_dynamic, placeholder);\n    if (count > 0) {\n        logger.debug(`Replaced ${placeholder.name} via dynamic method at least ${count} time(s)`);\n        placeholder.count_on_page += count;\n    }\n};\nconst do_normal_replace = (root_element, placeholder, config) => {\n    const count = dynamic_replace(root_element, placeholder.regex_normal, placeholder);\n    if (count > 0) {\n        logger.debug(`Replaced ${placeholder.name} via normal (dynamic) method at least ${count} time(s)`);\n        placeholder.count_on_page += count;\n    }\n};\nconst do_static_replace = (root_element, placeholder, config) => {\n    const count = static_replace(root_element, placeholder.regex_static, placeholder.expanded_value);\n    if (count > 0) {\n        logger.debug(`Replaced ${placeholder.name} via static method at least ${count} time(s)`);\n        placeholder.count_on_page += count;\n        placeholder.reload_page_on_change = true;\n    }\n};\nconst do_html_replace = (root_element, placeholder, config) => {\n    const count = inner_html_replace(root_element, placeholder.regex_html, placeholder.expanded_value);\n    if (count > 0) {\n        logger.debug(`Replaced ${placeholder.name} via innerHTML method at least ${count} time(s)`);\n        placeholder.count_on_page += count;\n        placeholder.reload_page_on_change = true;\n    }\n};\n// Replace all placeholders in the given order and return which placeholders actually were actually found in the page\nexport const replace_placeholders_in_subtree = (root_element, config) => {\n    for (const placeholder of config.placeholders.values()) {\n        do_dynamic_replace(root_element, placeholder, config);\n        do_normal_replace(root_element, placeholder, config);\n        do_static_replace(root_element, placeholder, config);\n        if (placeholder.allow_inner_html) {\n            do_html_replace(root_element, placeholder, config);\n        }\n    }\n    find_dynamic_placeholder_wrappers(config);\n    replace_dynamic_placeholder_values([...config.placeholders.values()]);\n};\nexport const replace_placeholder_in_string = (text, placeholder) => {\n    // This funtion will perform replacements, but will ignore the replacement type (all will be simple/direct replace)\n    return text.replace(placeholder.regex_dynamic, placeholder.expanded_value)\n        .replace(placeholder.regex_html, placeholder.expanded_value)\n        .replace(placeholder.regex_normal, placeholder.expanded_value)\n        .replace(placeholder.regex_static, placeholder.expanded_value);\n};\nexport const replace_dynamic_placeholder_values = (placeholder_list) => {\n    for (const placeholder of placeholder_list) {\n        for (const element of placeholder.output_elements) {\n            // Delete current contents\n            element.innerHTML = \"\";\n            // Add the value back as safely escaped text\n            const text = document.createTextNode(placeholder.expanded_value);\n            element.appendChild(text);\n        }\n    }\n};\nconst find_dynamic_placeholder_wrappers = (config) => {\n    const output_list = document.querySelectorAll(\".placeholder-value[data-placeholder]\");\n    for (const element of output_list) {\n        const placeholder_name = element.getAttribute(\"data-placeholder\");\n        if (placeholder_name) {\n            const placeholder = config.placeholders.get(placeholder_name);\n            if (placeholder) {\n                placeholder.output_elements.push(element);\n            }\n            else {\n                console.warn(`No placeholder named '${placeholder_name}', that is referenced by element:`, element);\n            }\n        }\n        else {\n            console.warn(`Element has empty/no attribute 'data-placeholder':`, element);\n        }\n    }\n};\n",
-        "import { logger } from \"./debug\";\nimport { replace_placeholder_in_string } from \"./replacer\";\nimport { clear_state } from \"./state_manager\";\n// Should be a directed acyclical graph\nexport class DependencyGraph {\n    constructor(placeholders) {\n        this.nodes = new Map();\n        for (const placeholder of placeholders.values()) {\n            this.nodes.set(placeholder.name, new GraphNode(placeholder));\n        }\n        // Needs to be in different loops to ensure that all nodes have been created first\n        for (const placeholder of placeholders.values()) {\n            try {\n                this.on_placeholder_value_change(placeholder);\n            }\n            catch (e) {\n                console.error(\"Error while building dependency graph\", e);\n                console.warn(\"Placeholder values may be inconsistent. Clearing your localStorage should fix this problem.\");\n                if (confirm(\"We detected a problem with your placeholder values. Resetting them to the defaults should fix this. Should we reset your placeholders?\")) {\n                    clear_state();\n                }\n            }\n        }\n        // Make sure that all expanded values are calculated\n        // We take every node with no downlinks (bottom of the graph) and do a recursive recalculation (upwards).\n        // Not super efficient, but simple to implement\n        for (const node of this.nodes.values()) {\n            if (node.downlinks.length == 0) {\n                node.recalculate_expanded_value(true);\n            }\n        }\n    }\n    debug_print_representation() {\n        let text = \"Dependency graph nodes (DEBUG view):\";\n        for (const node of this.nodes.values()) {\n            const dependencies = node.downlinks.map(n => n.placeholder.name).join(\", \");\n            if (dependencies.length == 0) {\n                text += `\\n${node.placeholder.name} (${node.placeholder.expanded_value}) has no dependencies`;\n            }\n            else {\n                text += `\\n${node.placeholder.name} (${node.placeholder.expanded_value}) depends on ${dependencies}`;\n            }\n        }\n        logger.debug(text);\n    }\n    unmark_everything() {\n        for (const node of this.nodes.values()) {\n            node.marked = false;\n        }\n    }\n    get_node(placeholder) {\n        const node = this.nodes.get(placeholder.name);\n        if (node == undefined) {\n            throw new Error(`Placeholder ${placeholder.name} is not part of the dependency graph`);\n        }\n        else {\n            return node;\n        }\n    }\n    on_placeholder_value_change(placeholder) {\n        const node = this.get_node(placeholder);\n        this.update_placeholder_downlinks(placeholder);\n        if (this.has_loop()) {\n            // Emergency measure: ignore any placeholders in this value. This should fix the loop\n            placeholder.expanded_value = placeholder.current_value;\n            node.downlinks = [];\n            // Also raise an exception to inform the user\n            throw new Error(`Placeholder ${placeholder.name} was part of a loop and has temporarily been made non-recursive`);\n        }\n        else {\n            node.recalculate_expanded_value(true);\n        }\n    }\n    get_all_marked() {\n        const marked = [];\n        for (const node of this.nodes.values()) {\n            if (node.marked) {\n                marked.push(node.placeholder);\n            }\n        }\n        return marked;\n    }\n    get_all_upstream(placeholder) {\n        this.unmark_everything();\n        const node = this.get_node(placeholder);\n        node.recursive_mark_upstream();\n        return this.get_all_marked();\n    }\n    update_placeholder_downlinks(placeholder) {\n        if (placeholder.allow_recursive == false) {\n            // By definition, non-recursive placeholders can not rely on other placeholders\n            return;\n        }\n        // Step 1: remove all old downlinks\n        const node = this.get_node(placeholder);\n        for (const old_downlink of node.downlinks) {\n            old_downlink.remove_uplink(node);\n        }\n        node.downlinks = [];\n        // Step 2: parse placeholder's value (again)\n        for (const other_node of this.nodes.values()) {\n            // No placeholder should directly be able to contain itself -> ignoring this case.\n            // This should lead to the placeholder's name appearing in it's text, which was probably intended\n            if (other_node != node) {\n                if (string_contains_placeholder(placeholder.current_value, other_node.placeholder)) {\n                    // This placeholders value contains a reference to the other node's placeholder\n                    //  -> This node depends on the other node\n                    node.downlinks.push(other_node);\n                    other_node.uplinks.push(node);\n                }\n            }\n        }\n    }\n    get_all_used_placeholders() {\n        // Also includes all placeholders used by the placeholders that were included\n        this.unmark_everything();\n        // Mark all used placeholders and their downstream nodes\n        for (const node of this.nodes.values()) {\n            if (node.placeholder.count_on_page > 0) {\n                node.recursive_mark_downstream();\n            }\n        }\n        return this.get_all_marked();\n    }\n    has_loop() {\n        // General algorithm: https://www.geeksforgeeks.org/detect-cycle-in-a-graph/\n        this.unmark_everything();\n        for (const node of this.nodes.values()) {\n            // Make sure that we check every single node (we likely have multiple graphs that are not connected)\n            if (!node.marked) {\n                if (this._has_loop([], node)) {\n                    return true;\n                }\n            }\n        }\n        return false;\n    }\n    _has_loop(back_stack, current_node) {\n        const new_back_stack = [...back_stack, current_node];\n        const index = back_stack.indexOf(current_node);\n        if (index != -1) {\n            let message = \"Dependency cycle in placeholders detected:\";\n            for (let i = index; i < new_back_stack.length; i++) {\n                const placeholder = new_back_stack[i].placeholder;\n                message += `\\n$ -> ${placeholder.name}: ${placeholder.current_value}`;\n            }\n            console.warn(message);\n            return true;\n        }\n        else if (!current_node.marked) {\n            // No cycle found yet, scan all children that are not yet marked\n            current_node.marked = true;\n            for (const child of current_node.downlinks) {\n                if (this._has_loop(new_back_stack, child)) {\n                    return true;\n                }\n            }\n            return false;\n        }\n        else {\n            // Already checked, so no need to start recursive scans\n            return false;\n        }\n    }\n}\nconst string_contains_placeholder = (string_to_test, placeholder_to_find) => {\n    return placeholder_to_find.regex_dynamic.test(string_to_test) ||\n        placeholder_to_find.regex_html.test(string_to_test) ||\n        placeholder_to_find.regex_normal.test(string_to_test) ||\n        placeholder_to_find.regex_static.test(string_to_test);\n};\nclass GraphNode {\n    constructor(placeholder) {\n        // These other nodes depend on this node\n        this.uplinks = [];\n        // This are the nodes this node depends on\n        this.downlinks = [];\n        // State used during operations to see if this node was already visited/processed\n        this.marked = false;\n        this.placeholder = placeholder;\n    }\n    remove_uplink(node) {\n        this.uplinks = this.uplinks.filter(x => x != node);\n    }\n    recalculate_expanded_value(recursive) {\n        let expanded_value = this.placeholder.current_value;\n        for (const downlink_node of this.downlinks) {\n            expanded_value = replace_placeholder_in_string(expanded_value, downlink_node.placeholder);\n        }\n        this.placeholder.expanded_value = expanded_value;\n        if (recursive) {\n            // Recalculate all uplink nodes in recursive too\n            for (const uplink_node of this.uplinks) {\n                uplink_node.recalculate_expanded_value(recursive);\n            }\n        }\n    }\n    recursive_mark_upstream() {\n        this.marked = true;\n        for (const node of this.uplinks) {\n            node.recursive_mark_upstream();\n        }\n    }\n    recursive_mark_downstream() {\n        this.marked = true;\n        for (const node of this.downlinks) {\n            node.recursive_mark_downstream();\n        }\n    }\n}\n",
-        "import { load_checkbox_state, load_dropdown_state, load_textbox_state } from \"./state_manager\";\nimport { parse_validator } from \"./validator\";\nimport { DependencyGraph } from \"./dependency_graph\";\n// This should be a more type safe reimplementation of 10_parse_data.js.\n// It has some breaking changes, since I try to improve how the javascript code works\nexport const assert_field_type = (name, expected_type_str, parent_object) => {\n    const value = parent_object[name];\n    const actual_type_str = typeof (value);\n    if (actual_type_str != expected_type_str) {\n        throw new Error(`Type mismatch: ${name} should be ${expected_type_str}, but is ${actual_type_str}.\\nProblematic object: ${JSON.stringify(parent_object)}`);\n    }\n    else {\n        return value;\n    }\n};\n// These functions are here to make sure, that I the type checker can properly work (since they have a specific return type)\nexport const get_string_field = (name, parent_object) => {\n    return assert_field_type(name, \"string\", parent_object);\n};\nexport const get_boolean_field = (name, parent_object) => {\n    return assert_field_type(name, \"boolean\", parent_object);\n};\nconst get_number_field = (name, parent_object) => {\n    return assert_field_type(name, \"number\", parent_object);\n};\nexport const get_array_field = (name, element_type, parent_object) => {\n    const array = parent_object[name];\n    if (Array.isArray(array)) {\n        for (const [index, entry] of array.entries()) {\n            const actual_type_str = typeof (entry);\n            if (actual_type_str != element_type) {\n                const msg = `Type mismatch: ${name}'s ${index + 1}th element should be ${element_type}, but is ${actual_type_str}.\\nProblematic object: ${JSON.stringify(parent_object)}`;\n                throw new Error(msg);\n            }\n        }\n        return array;\n    }\n    else {\n        throw new Error(`Type mismatch: ${name} should be an array, but is not.\\nProblematic object: ${JSON.stringify(parent_object)}`);\n    }\n};\nexport var InputType;\n(function (InputType) {\n    InputType[\"Textbox\"] = \"TEXTBOX\";\n    InputType[\"Checkbox\"] = \"CHECKBOX\";\n    InputType[\"Dropdown\"] = \"DROPDOWN\";\n})(InputType || (InputType = {}));\nexport const parse_config = (data) => {\n    const placeholder_map = new Map();\n    const textboxes = new Map();\n    const checkboxes = new Map();\n    const dropdowns = new Map();\n    const validator_map = new Map();\n    const validator_data_list = get_array_field(\"validators\", \"object\", data);\n    for (const validator_data of validator_data_list) {\n        const validator = parse_validator(validator_data);\n        if (validator_map.has(validator.id)) {\n            throw new Error(`Multiple validators with id '${validator.id}'`);\n        }\n        else {\n            validator_map.set(validator.id, validator);\n        }\n    }\n    const settings_data = assert_field_type(\"settings\", \"object\", data);\n    const settings = parse_settings(settings_data);\n    const placeholder_data = get_array_field(\"placeholder_list\", \"object\", data);\n    for (let i = 0; i < placeholder_data.length; i++) {\n        const placeholder = parse_any_placeholder(placeholder_data[i], validator_map, settings, i);\n        // Add the placeholder to the correct lists\n        placeholder_map.set(placeholder.name, placeholder);\n        if (placeholder.type == InputType.Textbox) {\n            textboxes.set(placeholder.name, placeholder);\n        }\n        else if (placeholder.type == InputType.Checkbox) {\n            checkboxes.set(placeholder.name, placeholder);\n        }\n        else if (placeholder.type == InputType.Dropdown) {\n            dropdowns.set(placeholder.name, placeholder);\n        }\n        else {\n            console.warn(\"Unknown placeholder type:\", placeholder.type);\n        }\n    }\n    const graph = new DependencyGraph(placeholder_map);\n    return {\n        \"placeholders\": placeholder_map,\n        \"textboxes\": textboxes,\n        \"checkboxes\": checkboxes,\n        \"dropdowns\": dropdowns,\n        \"settings\": settings,\n        \"dependency_graph\": graph,\n        \"input_tables\": [],\n    };\n};\nconst parse_settings = (data) => {\n    return {\n        \"debug\": get_boolean_field(\"debug\", data),\n        \"delay_millis\": get_number_field(\"delay_millis\", data),\n        // @TODO: If I let users specify prefixes, I will need to make sure, that they do not contain regex characters or escape them\n        // How normal placeholders are marked\n        \"normal_prefix\": \"x\",\n        \"normal_suffix\": \"x\",\n        // How placeholders using the innerHTML method are marked\n        \"html_prefix\": \"i\",\n        \"html_suffix\": \"i\",\n        // How placeholders using the direct/static replacement methodare marked\n        \"static_prefix\": \"s\",\n        \"static_suffix\": \"s\",\n        // How placeholders using the dynamic replacement methodare marked\n        \"dynamic_prefix\": \"d\",\n        \"dynamic_suffix\": \"d\",\n    };\n};\nconst parse_any_placeholder = (data, validator_map, settings, index) => {\n    const type = get_string_field(\"type\", data);\n    // Parse fields that are shared between all placeholders\n    const name = get_string_field(\"name\", data);\n    let parsed = {\n        \"name\": name,\n        \"order_index\": index,\n        // The regexes for the different replace methods. Stored here so that I only need to compile them once\n        \"regex_dynamic\": RegExp(settings.dynamic_prefix + name + settings.dynamic_suffix, \"g\"),\n        \"regex_html\": RegExp(settings.html_prefix + name + settings.html_suffix, \"g\"),\n        \"regex_normal\": RegExp(settings.normal_prefix + name + settings.normal_suffix, \"g\"),\n        \"regex_static\": RegExp(settings.static_prefix + name + settings.static_suffix, \"g\"),\n        // \n        \"description\": get_string_field(\"description\", data),\n        \"read_only\": get_boolean_field(\"read_only\", data),\n        \"allow_inner_html\": get_boolean_field(\"allow_inner_html\", data),\n        \"allow_recursive\": false,\n        \"current_value\": \"UNINITIALIZED\",\n        \"expanded_value\": \"UNINITIALIZED\",\n        \"count_on_page\": 0,\n        \"reload_page_on_change\": false,\n        \"output_elements\": [], // Will be set, when the page is searched\n    };\n    // Parse the type specific attributes\n    if (type === \"textbox\") {\n        const placeholder = finish_parse_textbox(parsed, data, validator_map);\n        load_textbox_state(placeholder);\n        return placeholder;\n    }\n    else if (type == \"checkbox\") {\n        const placeholder = finish_parse_checkbox(parsed, data);\n        load_checkbox_state(placeholder);\n        return placeholder;\n    }\n    else if (type == \"dropdown\") {\n        const placeholder = finish_parse_dropdown(parsed, data);\n        load_dropdown_state(placeholder);\n        return placeholder;\n    }\n    else {\n        throw new Error(`Unsupported placeholder type '${type}'`);\n    }\n};\nconst finish_parse_textbox = (parsed, data, validator_map) => {\n    let default_function, default_value;\n    if (data[\"default_value\"] != undefined) {\n        default_value = get_string_field(\"default_value\", data);\n    }\n    else {\n        const default_js_code = get_string_field(\"default_function\", data);\n        default_function = () => {\n            // Wrap the function, so that we can ensure that errors are properly handled\n            try {\n                const compiled_function = new Function(default_js_code);\n                const result = compiled_function();\n                if (typeof (result) != \"string\") {\n                    throw new Error(`Custom function '${default_js_code}' should return a string, but it returned a ${typeof (result)}: ${result}`);\n                }\n                else {\n                    return result;\n                }\n            }\n            catch (error) {\n                throw new Error(`Failed to evaluate default_function '${default_js_code}' of placeholder ${parsed.name}: ${error}`);\n            }\n        };\n    }\n    const validator_names = get_array_field(\"validators\", \"string\", data);\n    const validator_list = [];\n    for (const name of validator_names) {\n        const validator = validator_map.get(name);\n        if (validator) {\n            validator_list.push(validator);\n        }\n        else {\n            const known_validators = Array.from(validator_map.keys()).join(\", \");\n            throw new Error(`No validator with id '${name}' was found. Known validators are ${known_validators}`);\n        }\n    }\n    return Object.assign(Object.assign({}, parsed), { \"allow_recursive\": get_boolean_field(\"allow_recursive\", data), \"default_function\": default_function, \"default_value\": default_value, \"input_elements\": [], \"type\": InputType.Textbox, \"validators\": validator_list });\n};\nconst finish_parse_checkbox = (parsed, data) => {\n    return Object.assign(Object.assign({}, parsed), { \"allow_recursive\": true, \"checked_by_default\": get_boolean_field(\"checked_by_default\", data), \"current_is_checked\": false, \"input_elements\": [], \"value_checked\": get_string_field(\"value_checked\", data), \"value_unchecked\": get_string_field(\"value_unchecked\", data), \"type\": InputType.Checkbox });\n};\nconst finish_parse_dropdown = (parsed, data) => {\n    const raw_options = get_array_field(\"options\", \"object\", data);\n    const options = [];\n    for (const option of raw_options) {\n        options.push({\n            display_name: get_string_field(\"display_name\", option),\n            value: get_string_field(\"value\", option),\n        });\n    }\n    const default_index = get_number_field(\"default_index\", data);\n    if (default_index < 0) {\n        throw new Error(`Invalid value: \"default_index\" should not be negative, but is ${default_index}.\\nProblematic object: ${JSON.stringify(data)}`);\n    }\n    else if (default_index >= options.length) {\n        throw new Error(`Invalid value: \"default_index\" should be smaller than the number of options (${options.length}), but is ${default_index}.\\nProblematic object: ${JSON.stringify(data)}`);\n    }\n    return Object.assign(Object.assign({}, parsed), { \"allow_recursive\": true, \"current_index\": 0, \"default_index\": default_index, \"input_elements\": [], \"options\": options, \"type\": InputType.Dropdown });\n};\n",
-        "import { logger } from \"./debug\";\nimport { prepare_input_field } from \"./inputs\";\nimport { create_dynamic_placeholder_element } from \"./replacer\";\nconst TABLE_CELL_HEADINGS = new Map();\nTABLE_CELL_HEADINGS.set(\"name\", \"Name\");\nTABLE_CELL_HEADINGS.set(\"description\", \"Description\");\nTABLE_CELL_HEADINGS.set(\"value\", \"Value\");\nTABLE_CELL_HEADINGS.set(\"input\", \"Input element\");\nTABLE_CELL_HEADINGS.set(\"description-or-name\", \"Description / name\");\n// Helper functions to simplify the following code\nconst appendTextNode = (element, text) => {\n    element.appendChild(document.createTextNode(text));\n};\nconst createChildElement = (parent, tag_name) => {\n    const child = document.createElement(tag_name);\n    parent.appendChild(child);\n    return child;\n};\nconst generate_automatic_placeholder_table = (element, columns, config, placeholders_to_show) => {\n    placeholders_to_show = sort_and_remove_duplicate_placeholders(placeholders_to_show);\n    // Remove the current contents. This enables the plugin to generate fallback contents in case the JavaScript code does not work\n    element.innerHTML = \"\";\n    if (placeholders_to_show.length == 0) {\n        // Do not create an empty table. Instead show a warning on the page\n        const div = createChildElement(element, \"div\");\n        div.classList.add(\"info-message\");\n        if (placeholders_to_show.length == 0) {\n            appendTextNode(div, \"No placeholders to be shown\");\n        }\n        return;\n    }\n    logger.info(\"Creating automatic input table at\", element, \"with columns\", columns);\n    // element.innerHTML = \"\"; // remove all children\n    const table = createChildElement(element, \"table\");\n    const table_head = createChildElement(table, \"thead\");\n    const table_head_row = createChildElement(table_head, \"tr\");\n    const table_body = createChildElement(table, \"tbody\");\n    for (const column of columns) {\n        const table_cell = createChildElement(table_head_row, \"th\");\n        const heading = TABLE_CELL_HEADINGS.get(column);\n        if (heading) {\n            appendTextNode(table_cell, heading);\n        }\n        else {\n            appendTextNode(table_cell, column);\n            console.error(`Unknown column name: ${column}`);\n        }\n    }\n    const rows = [];\n    for (const placeholder of placeholders_to_show) {\n        if (placeholder.read_only) {\n            logger.debug(`auto_table: Skipping ${placeholder.name} because it is read-only`);\n            continue;\n        }\n        const row = createChildElement(table_body, \"tr\");\n        populate_auto_table_row(row, placeholder, columns, config);\n        rows.push({\n            \"element\": row,\n            \"placeholder\": placeholder,\n        });\n    }\n    config.input_tables.push({\n        \"columns\": columns,\n        \"table_element\": table,\n        \"rows\": rows,\n    });\n};\nconst sort_and_remove_duplicate_placeholders = (placeholder_list) => {\n    return [...new Set(placeholder_list)].sort((a, b) => a.order_index - b.order_index);\n};\nconst populate_auto_table_row = (row, placeholder, columns, config) => {\n    for (const column of columns) {\n        const cell = createChildElement(row, \"td\");\n        if (column == \"name\") {\n            appendTextNode(cell, placeholder.name);\n        }\n        else if (column == \"description\") {\n            appendTextNode(cell, placeholder.description);\n        }\n        else if (column == \"value\") {\n            const dynamic_placeholer = create_dynamic_placeholder_element(placeholder);\n            cell.appendChild(dynamic_placeholer);\n            placeholder.output_elements.push(dynamic_placeholer);\n        }\n        else if (column == \"input\") {\n            const input = createChildElement(cell, \"input\");\n            prepare_input_field(config, placeholder, input);\n        }\n        else if (column == \"description-or-name\") {\n            const text = placeholder.description || placeholder.name;\n            appendTextNode(cell, text);\n        }\n        else {\n            console.error(`Unknown column name: ${column}`);\n        }\n    }\n};\nconst update_auto_table = (config, table, new_placeholder_list) => {\n    // Sort them the same way they are sorted in the table -> lists are easy to compare\n    new_placeholder_list = sort_and_remove_duplicate_placeholders(new_placeholder_list);\n    // Step 1: remove rows that are no longer to be shown\n    const rows_to_keep = [];\n    for (const row of table.rows) {\n        if (new_placeholder_list.includes(row.placeholder)) {\n            rows_to_keep.push(row);\n        }\n        else {\n            logger.debug(`Removed table row for ${row.placeholder.name}:`, row.element);\n            row.element.remove();\n        }\n    }\n    // Step 2: add rows that do not yet exist\n    const final_rows = [];\n    const reversed_current = [...rows_to_keep].reverse();\n    const reversed_new = [...new_placeholder_list].reverse();\n    let next_new;\n    while (next_new = reversed_new.pop()) {\n        // const next_new = reversed_new.pop();\n        const next_current = reversed_current.slice(-1)[0];\n        if (next_current && next_current.placeholder === next_new) {\n            // The row is already in the table\n            reversed_current.pop(); // remove from queue to keep in sync with other queue\n            final_rows.push(next_current);\n        }\n        else {\n            const element = document.createElement(\"tr\");\n            // insert at the correct position in the dom\n            if (final_rows.length == 0) {\n                // adds it before the first child or if it does not exist at the end (which would also be the first element :D)\n                table.table_element.insertBefore(element, table.table_element.firstChild);\n            }\n            else {\n                // insert it after the last row that was processed\n                const last_node = final_rows[final_rows.length - 1].element;\n                last_node.insertAdjacentElement(\"afterend\", element);\n            }\n            populate_auto_table_row(element, next_new, table.columns, config);\n            final_rows.push({\n                \"element\": element,\n                \"placeholder\": next_new,\n            });\n            logger.debug(`Added table row for ${next_new.name}:`, element);\n        }\n    }\n    // Store the updated row information in the original table object\n    table.rows = final_rows;\n};\nexport const update_all_auto_tables = (config) => {\n    logger.debug(`Updating ${config.input_tables.length} automatic input tables`);\n    if (config.input_tables.length > 0) {\n        const new_placeholder_list = config.dependency_graph.get_all_used_placeholders();\n        for (const table of config.input_tables) {\n            update_auto_table(config, table, new_placeholder_list);\n        }\n    }\n};\nexport const initialize_auto_tables = (config) => {\n    const element_list = document.querySelectorAll(\"div.auto-input-table\");\n    if (element_list.length > 0) {\n        const used_placeholders = config.dependency_graph.get_all_used_placeholders().filter(x => !x.read_only);\n        for (let element of element_list) {\n            const columns_str = element.getAttribute(\"data-columns\") || \"name,input\";\n            const columns = columns_str.includes(\",\") ? columns_str.split(\",\") : [columns_str];\n            generate_automatic_placeholder_table(element, columns, config, used_placeholders);\n        }\n    }\n};\n",
-        "import { update_all_auto_tables } from \"./auto_tables\";\nimport { logger, reload_page } from \"./debug\";\nimport { InputType } from \"./parse_settings\";\nimport { replace_dynamic_placeholder_values } from \"./replacer\";\nimport { store_checkbox_state, store_dropdown_state, store_textbox_state } from \"./state_manager\";\nimport { validate_textbox_input_field } from \"./validator\";\nexport const initialize_all_input_fields = (config) => {\n    const input_list = document.querySelectorAll(\"input[data-input-for]\");\n    for (let input_element of input_list) {\n        const placeholder_name = input_element.getAttribute(\"data-input-for\");\n        if (placeholder_name == null) {\n            throw new Error(\"How can this be, the selector forces the 'data-input-for' attribute to exist\");\n        }\n        const placeholder = config.placeholders.get(placeholder_name);\n        if (placeholder) {\n            prepare_input_field(config, placeholder, input_element);\n        }\n        else {\n            console.warn(`Unknown placeholder referenced in input element: '${placeholder_name}'`);\n            input_element.classList.add(\"input-for-variable\");\n            input_element.value = `ERROR_UNDEFINED_PLACEHOLDER: ${placeholder_name}`;\n        }\n    }\n};\nexport const prepare_input_field = (config, placeholder, input_element) => {\n    input_element.classList.add(\"input-for-variable\");\n    if (placeholder.type == InputType.Checkbox) {\n        initialize_input_checkbox(config, placeholder, input_element);\n    }\n    else if (placeholder.type == InputType.Dropdown) {\n        initialize_input_dropdown(config, placeholder, input_element);\n    }\n    else if (placeholder.type == InputType.Textbox) {\n        initialize_input_textbox(config, placeholder, input_element);\n    }\n    else {\n        console.error(`Placeholder ${placeholder.name} has unknown type '${placeholder.type}'`);\n    }\n};\nconst initialize_input_checkbox = (config, placeholder, input_element) => {\n    input_element.type = \"checkbox\";\n    input_element.checked = placeholder.current_is_checked;\n    if (placeholder.read_only) {\n        // disable the checkbox\n        input_element.disabled = true;\n    }\n    else {\n        // Listen for state changes\n        input_element.addEventListener(\"change\", () => {\n            logger.debug(\"Checkbox change\", placeholder.name, \"- new value:\", input_element.checked);\n            store_checkbox_state(placeholder, input_element.checked);\n            placeholder.current_value = input_element.checked ? placeholder.value_checked : placeholder.value_unchecked;\n            on_placeholder_change(config, placeholder);\n        });\n    }\n    // Store this input element\n    placeholder.input_elements.push(input_element);\n};\nconst initialize_input_dropdown = (config, placeholder, input_element) => {\n    const new_node = document.createElement(\"select\");\n    new_node.classList.add(\"placeholder-dropdown\");\n    for (const option of placeholder.options) {\n        const option_element = document.createElement(\"option\");\n        option_element.text = option.display_name; // @TODO: allow placeholders in here\n        new_node.appendChild(option_element);\n    }\n    // Replace input element entirely with the dropdown menu\n    if (input_element.parentNode) {\n        input_element.parentNode.replaceChild(new_node, input_element);\n    }\n    else {\n        // How would we find it in the DOM if it has no parent?\n        console.error(`Input element`, input_element, `for placeholder ${placeholder.name} has no parent!`);\n    }\n    // Select the stored option\n    new_node.selectedIndex = placeholder.current_index;\n    if (placeholder.read_only) {\n        // disable the dropdown\n        new_node.disabled = true;\n    }\n    else {\n        // Add an event listener\n        new_node.addEventListener(\"change\", () => {\n            logger.debug(\"Dropdown change\", placeholder.name, \"- new index:\", new_node.selectedIndex);\n            store_dropdown_state(placeholder, new_node.selectedIndex);\n            placeholder.current_index = new_node.selectedIndex;\n            placeholder.current_value = placeholder.options[new_node.selectedIndex].value;\n            on_placeholder_change(config, placeholder);\n        });\n    }\n    // Store this input element\n    placeholder.input_elements.push(new_node);\n};\nconst initialize_input_textbox = (config, placeholder, input_element) => {\n    // Restore the stored state\n    input_element.value = placeholder.current_value;\n    if (placeholder.read_only) {\n        // disable the checkbox\n        input_element.disabled = true;\n        input_element.style.cursor = \"not-allowed\";\n    }\n    else {\n        if (placeholder.default_value != undefined) {\n            input_element.placeholder = `Default: ${placeholder.default_value}`;\n        }\n        else {\n            input_element.placeholder = \"Dynamic default value\";\n        }\n        const on_keypress = (event) => {\n            if (event.key === \"Enter\") {\n                logger.debug(\"Textbox change confirmed with Enter key for \", placeholder.name, \"- new value:\", input_element.value);\n                if (validate_textbox_input_field(placeholder, input_element)) {\n                    store_textbox_state(placeholder, input_element.value);\n                    placeholder.current_value = input_element.value;\n                    on_placeholder_change(config, placeholder);\n                }\n            }\n            else if (event.key === \"Escape\") {\n                // @TODO: why does this not get triggered? Is it intercepted by something else?\n                logger.debug(\"Resetting input field for \", placeholder.name, \" to current placeholder value\");\n                input_element.value = placeholder.current_value;\n            }\n        };\n        if (placeholder.validators.length == 0) {\n            // No validators -> no need to handle exception when validation fails\n            input_element.addEventListener(\"keypress\", on_keypress);\n        }\n        else {\n            // Check if initial value is valid\n            validate_textbox_input_field(placeholder, input_element);\n            // Listen for state changes\n            input_element.addEventListener(\"input\", () => {\n                // The text was probably modified, so we need to update the validator\n                validate_textbox_input_field(placeholder, input_element);\n            });\n            input_element.addEventListener(\"keypress\", on_keypress);\n        }\n    }\n    // Store this input element\n    placeholder.input_elements.push(input_element);\n};\nconst on_placeholder_change = (config, placeholder) => {\n    const affected_placeholders = config.dependency_graph.get_all_upstream(placeholder);\n    let require_reload = false;\n    for (const ph of affected_placeholders) {\n        require_reload = require_reload || ph.reload_page_on_change;\n    }\n    logger.debug(`Change of ${placeholder.name} requires updates for placeholders:\\n${affected_placeholders.map(p => ` - ${p.name}\\n`).join(\"\")}\\nRequires reload: ${require_reload}`);\n    if (require_reload) {\n        reload_page(); // for now we just use the full reload\n    }\n    else {\n        config.dependency_graph.on_placeholder_value_change(placeholder);\n        // update auto-tables, since downstream may be changed\n        update_all_auto_tables(config);\n        // Update all input elements for the modified placeholder\n        if (placeholder.type == InputType.Checkbox) {\n            const ph = placeholder;\n            for (const input_element of ph.input_elements) {\n                input_element.checked = ph.current_is_checked;\n            }\n        }\n        else if (placeholder.type == InputType.Dropdown) {\n            const ph = placeholder;\n            for (const input_element of ph.input_elements) {\n                input_element.selectedIndex = ph.current_index;\n            }\n        }\n        else if (placeholder.type == InputType.Textbox) {\n            const ph = placeholder;\n            for (const input_element of ph.input_elements) {\n                input_element.value = ph.current_value;\n                validate_textbox_input_field(ph, input_element);\n            }\n        }\n        else {\n            console.warn(`Placeholder ${placeholder.name} has unexpected type '${placeholder.type}'`);\n        }\n        // @TODO Not needed as long as the dropdown display name is static\n        // // Update input elements\n        // for (const ph of affected_placeholders) {\n        //     // Only dropdown's input elements can depend on other placeholders (the label)\n        //     if (ph.type == InputType.Dropdown) {\n        //         for (const input of (ph as DropdownPlaceholder).input_elements) {\n        //             // code here\n        //         }\n        //     }\n        // }\n        // Update output elements\n        replace_dynamic_placeholder_values(affected_placeholders);\n    }\n};\n",
+        "import { logger, reload_page } from \"./debug\";\nimport { is_valid_value_for_placeholder } from \"./validator\";\n// These functions are here to make it easier to change the storage backend (for example locasstorage -> cookies)\n// and to make it possible to potentially have better debugging\nconst STORAGE_PREFIX = \"PLACEHOLDER_\"; // @TODO make it configurable by settings?\nconst SETTINGS_PREFIX = \"PLACEHOLDER-SETTING_\";\nconst store_value = (name, value) => {\n    localStorage.setItem(STORAGE_PREFIX + name, value);\n};\nconst load_value = (name) => {\n    return localStorage.getItem(STORAGE_PREFIX + name);\n};\nexport const store_boolean_setting = (name, value) => {\n    logger.info(`Storing boolean setting '${name}' with value ${value}`);\n    localStorage.setItem(`${SETTINGS_PREFIX}${name}`, value ? \"1\" : \"0\");\n};\nexport const load_boolean_setting = (name, default_value) => {\n    const stored = localStorage.getItem(`${SETTINGS_PREFIX}${name}`);\n    logger.info(`Reading boolean setting '${name}' with value ${stored}`);\n    if (stored === null) {\n        return default_value;\n    }\n    else if (stored === \"1\") {\n        return true;\n    }\n    else if (stored === \"0\") {\n        return false;\n    }\n    else {\n        // Unexpected state, warn user and fall back to default\n        console.warn(`Unexpected state for boolean setting. Should be null, '0' or '1', but was '${stored}'`);\n        return default_value;\n    }\n};\n// I changed the storage model: the real value is stored in the placeholder object instead of in localstorage -> easier and safer to access\n// We pass the whole placeholder instead of just a name, so that you can not accidentally call the wrong function or use an invalid placeholder name\n// We use different values for different types (checkbox -> NAME_IS_CHECKED, textbox -> NAME_TEXT, ...) so that if a user changes the type of a placeholder it should not cause problems\nexport const store_checkbox_state = (placeholder, new_is_checked) => {\n    // Update the placeholder's value\n    placeholder.current_is_checked = new_is_checked;\n    placeholder.current_value = new_is_checked ? placeholder.value_checked : placeholder.value_unchecked;\n    // Permanently store the new state\n    store_value(`${placeholder.name}_IS_CHECKED`, new_is_checked ? \"1\" : \"0\");\n};\nexport const load_checkbox_state = (placeholder) => {\n    const stored_state = load_value(`${placeholder.name}_IS_CHECKED`);\n    if (stored_state == null) {\n        // No stored state -> use default value\n        placeholder.current_is_checked = placeholder.checked_by_default;\n    }\n    else {\n        if (stored_state == \"0\" || stored_state == \"1\") {\n            // Load the stored state\n            placeholder.current_is_checked = stored_state == \"1\";\n        }\n        else {\n            // Unexpected state, warn user and fall back to default\n            console.warn(`Unexpected state for checkbox. Should be '0' or '1', but was '${stored_state}'`);\n            placeholder.current_is_checked = placeholder.checked_by_default;\n        }\n    }\n    // Now we update the actual value based on the state\n    placeholder.current_value = placeholder.current_is_checked ? placeholder.value_checked : placeholder.value_unchecked;\n};\nexport const clear_state = () => {\n    clear_by_prefix(STORAGE_PREFIX);\n};\nexport const clear_settings = () => {\n    clear_by_prefix(SETTINGS_PREFIX);\n};\nconst clear_by_prefix = (prefix) => {\n    // The easiest way would be to clear the whole storage, but that might break other plugins / scripts.\n    // So we only delete all items that start with our prefix\n    console.warn(`Clearing all localStorage items starting with '${prefix}'`);\n    let i = 0;\n    while (i < localStorage.length) {\n        const key = localStorage.key(i);\n        if (key === null || key === void 0 ? void 0 : key.startsWith(prefix)) {\n            // Delete the item\n            localStorage.removeItem(key);\n        }\n        else {\n            // Not ours, so we skip it\n            i++;\n        }\n    }\n    reload_page();\n};\nconst is_valid_index = (placeholder, index) => {\n    try {\n        const item = placeholder.options[index];\n        return item != undefined && item != null;\n    }\n    catch (error) {\n        return false;\n    }\n};\nexport const store_dropdown_state = (placeholder, new_index) => {\n    // Perform sanity checks on the index\n    if (is_valid_index(placeholder, new_index)) {\n        store_value(`${placeholder.name}_INDEX`, `${new_index}`);\n        placeholder.current_value = placeholder.options[new_index].value;\n        placeholder.current_index = new_index;\n    }\n    else {\n        throw new Error(`Index must a whole number N, where 0 <= N < ${placeholder.options.length}. But it is ${new_index}`);\n    }\n};\nexport const load_dropdown_state = (placeholder) => {\n    const stored_state = load_value(`${placeholder.name}_INDEX`);\n    if (stored_state == null) {\n        // No stored state -> use default value\n        placeholder.current_index = placeholder.default_index;\n    }\n    else {\n        const stored_index = Number(stored_state);\n        if (is_valid_index(placeholder, stored_index)) {\n            // Load the stored state\n            placeholder.current_index = stored_index;\n        }\n        else {\n            // Unexpected state, warn user and fall back to default\n            console.warn(`Unexpected state for dropdown. Should be a whole number N, where 0 <= N < ${placeholder.options.length}. But it is ${stored_state}`);\n            placeholder.current_index = placeholder.default_index;\n        }\n    }\n    // Now we update the actual value based on the state\n    placeholder.current_value = placeholder.options[placeholder.current_index].value;\n};\nexport const store_textbox_state = (placeholder, new_value) => {\n    const is_validation_ok = is_valid_value_for_placeholder(placeholder, new_value);\n    logger.info(`Set textbox ${placeholder.name} to '${new_value}'. Validation ok? ${is_validation_ok}`);\n    if (is_validation_ok) {\n        store_value(`${placeholder.name}_TEXT`, new_value);\n    }\n    else {\n        throw new Error(`Validation error: Value '${new_value}' is not valid for placeholder ${placeholder.name}`);\n    }\n};\nexport const load_textbox_state = (placeholder) => {\n    const stored_state = load_value(`${placeholder.name}_TEXT`);\n    if (stored_state != null) {\n        if (is_valid_value_for_placeholder(placeholder, stored_state)) {\n            placeholder.current_value = stored_state;\n            return; // Do not use the default value / function\n        }\n        else {\n            console.warn(`Stored value for placeholder ${placeholder.name} is invalid: '${stored_state}'. Will revert to default.`);\n            // Should we remove the value? Idk\n        }\n    }\n    // Use a default value\n    if (placeholder.default_value != undefined) {\n        placeholder.current_value = placeholder.default_value;\n        if (!is_valid_value_for_placeholder(placeholder, placeholder.default_value)) {\n            console.warn(`Default value for placeholder '${placeholder.name}' is invalid: '${placeholder.default_value}'`);\n        }\n    }\n    else if (placeholder.default_function) {\n        try {\n            const result = placeholder.default_function();\n            placeholder.current_value = result;\n            try {\n                // store the function result, since it may be different with each invocation (such as a randomly generated password)\n                store_textbox_state(placeholder, result);\n            }\n            catch (error) {\n                console.warn(`Default function for placeholder '${placeholder.name}' returned invalid value: '${result}'`);\n            }\n        }\n        catch (error) {\n            // This will be called if the placeholder's custom function fails\n            console.error(`Error while loading default textbox state for placeholder ${placeholder.name}:`, error);\n            placeholder.current_value = \"DEFAULT_FUNCTION_ERROR\";\n        }\n    }\n    else {\n        throw new Error(`Either 'default_value' or 'default_function' needs to be set for placeholder ${placeholder.name}`);\n    }\n};\n",
+        "import { logger } from \"./debug\";\n// Replace a specific placeholder and return the estimated number of occurences (underestimated, may actually be higher)\nconst static_replace = (root_element, search_regex, replacement_value) => {\n    const walker = document.createTreeWalker(root_element, NodeFilter.SHOW_TEXT);\n    let node;\n    let count = 0;\n    if (!search_regex.global) {\n        console.warn(`You should set the global flag for the regex. Context: replacing '${search_regex.source}' with '${replacement_value}'`);\n    }\n    while (node = walker.nextNode()) {\n        if (node.nodeValue) {\n            const replaced_str = node.nodeValue.replace(search_regex, replacement_value);\n            if (node.nodeValue != replaced_str) {\n                node.nodeValue = replaced_str;\n                count++; // Of course, it might have been replaced multiple times by replaceAll. But this is just for debugging\n                // and performing an accurate count would impact the performace.\n            }\n        }\n    }\n    return count;\n};\nconst escapeHTML = (text) => {\n    const element = document.createElement(\"div\");\n    element.appendChild(document.createTextNode(text));\n    return element.innerHTML;\n};\nconst inner_html_replace = (root_element, search_regex, replacement_value) => {\n    // User supplied input, HTML escape it before we inject it in the page\n    replacement_value = escapeHTML(replacement_value);\n    if (!search_regex.global) {\n        console.warn(`You should set the global flag for the regex. Context: replacing '${search_regex.source}' with '${replacement_value}'`);\n    }\n    const new_value = root_element.innerHTML.replace(search_regex, replacement_value);\n    if (new_value != root_element.innerHTML) {\n        root_element.innerHTML = new_value;\n        return 1;\n    }\n    else {\n        return 0;\n    }\n};\nexport const create_dynamic_placeholder_element = (placeholder) => {\n    const span = document.createElement(\"span\");\n    span.classList.add(\"placeholder-value\");\n    span.dataset.placeholder = placeholder.name;\n    span.textContent = placeholder.expanded_value;\n    return span;\n};\nconst dynamic_replace = (root_element, search_regex, placeholder, search_for_pre_replaced) => {\n    var _a;\n    const walker = document.createTreeWalker(root_element, NodeFilter.SHOW_TEXT);\n    let node;\n    if (!search_regex.global) {\n        console.warn(`You should set the global flag for the regex. Context: replacing '${search_regex.source}' with '${placeholder.current_value}'`);\n    }\n    let existing_count = 0;\n    if (search_for_pre_replaced) {\n        const already_existing_wrappers = document.querySelectorAll(\".placeholder-value[data-placeholder]\");\n        for (const wrapper of already_existing_wrappers) {\n            if (wrapper.getAttribute(\"data-placeholder\") === placeholder.name) {\n                existing_count++;\n            }\n        }\n        if (existing_count > 0) {\n            logger.debug(`${existing_count} dynamic placeholder elements already exist for placeholder ${placeholder.name}`);\n        }\n    }\n    const nodes_to_modify = [];\n    while (node = walker.nextNode()) {\n        if (node.nodeValue) {\n            if (node.nodeValue.match(search_regex)) {\n                // Do not modify in-place while iterating over the DOM\n                nodes_to_modify.push(node);\n            }\n        }\n    }\n    // Do not put in the value yet, otherwise it may be replaced by other placeholders\n    const replacement_value = `<span class=\"placeholder-value\" data-placeholder=\"${escapeHTML(placeholder.name)}\">TEMPORARY PLACEHOLDER</span>`;\n    for (const node of nodes_to_modify) {\n        if (node.nodeValue) {\n            const replaced_str = escapeHTML(node.nodeValue).replace(search_regex, replacement_value);\n            const new_node = document.createElement(\"span\");\n            new_node.innerHTML = replaced_str;\n            (_a = node.parentElement) === null || _a === void 0 ? void 0 : _a.replaceChild(new_node, node);\n        }\n    }\n    return nodes_to_modify.length + existing_count;\n};\nconst do_dynamic_replace = (root_element, placeholder, config) => {\n    const count = dynamic_replace(root_element, placeholder.regex_dynamic, placeholder, true);\n    if (count > 0) {\n        logger.debug(`Replaced ${placeholder.name} via dynamic method at least ${count} time(s)`);\n        placeholder.count_on_page += count;\n    }\n};\nconst do_normal_replace = (root_element, placeholder, config) => {\n    const count = dynamic_replace(root_element, placeholder.regex_normal, placeholder, false);\n    if (count > 0) {\n        logger.debug(`Replaced ${placeholder.name} via normal (dynamic) method at least ${count} time(s)`);\n        placeholder.count_on_page += count;\n    }\n};\nconst do_static_replace = (root_element, placeholder, config) => {\n    const count = static_replace(root_element, placeholder.regex_static, placeholder.expanded_value);\n    if (count > 0) {\n        logger.debug(`Replaced ${placeholder.name} via static method at least ${count} time(s)`);\n        placeholder.count_on_page += count;\n        placeholder.reload_page_on_change = true;\n    }\n};\nconst do_html_replace = (root_element, placeholder, config) => {\n    const count = inner_html_replace(root_element, placeholder.regex_html, placeholder.expanded_value);\n    if (count > 0) {\n        logger.debug(`Replaced ${placeholder.name} via innerHTML method at least ${count} time(s)`);\n        placeholder.count_on_page += count;\n        placeholder.reload_page_on_change = true;\n    }\n};\n// Replace all placeholders in the given order and return which placeholders actually were actually found in the page\nexport const replace_placeholders_in_subtree = (root_element, config) => {\n    for (const placeholder of config.placeholders.values()) {\n        do_dynamic_replace(root_element, placeholder, config);\n        do_normal_replace(root_element, placeholder, config);\n        do_static_replace(root_element, placeholder, config);\n        if (placeholder.allow_inner_html) {\n            do_html_replace(root_element, placeholder, config);\n        }\n    }\n    find_dynamic_placeholder_wrappers(config);\n    replace_dynamic_placeholder_values([...config.placeholders.values()]);\n};\nexport const safe_replace_multiple_placeholders_in_string = (text, placeholder_list) => {\n    // Optimize for trivial cases\n    if (placeholder_list.length == 0) {\n        return text;\n    }\n    else if (placeholder_list.length == 1) {\n        // We can directly replace it without any problems\n        const placeholder = placeholder_list[0];\n        return replace_placeholder_in_string_with(text, placeholder, placeholder.expanded_value);\n    }\n    else {\n        // If we just replace the values directly in a for loop, we get bugs, when the value of one placeholder contains another placeholder that is also replaced, but later\n        // To circumvent this, we replace placeholders with randomized other placeholders and then replace these with the actual values\n        const unique = `${Date.now()}_${Math.random()}`;\n        for (const placeholder of placeholder_list) {\n            text = replace_placeholder_in_string_with(text, placeholder, `x${placeholder.name}#${unique}x`);\n        }\n        for (const placeholder of placeholder_list) {\n            const regex = new RegExp(`x${placeholder.name}#${unique}x`, \"g\");\n            text = text.replace(regex, placeholder.expanded_value);\n        }\n        return text;\n    }\n};\nconst replace_placeholder_in_string_with = (text, placeholder, value) => {\n    // This funtion will perform replacements, but will ignore the replacement type (all will be simple/direct replace)\n    return text.replace(placeholder.regex_dynamic, value)\n        .replace(placeholder.regex_html, value)\n        .replace(placeholder.regex_normal, value)\n        .replace(placeholder.regex_static, value);\n};\nexport const replace_dynamic_placeholder_values = (placeholder_list) => {\n    for (const placeholder of placeholder_list) {\n        for (const element of placeholder.output_elements) {\n            // Delete current contents\n            element.innerHTML = \"\";\n            // Add the value back as safely escaped text\n            const text = document.createTextNode(placeholder.expanded_value);\n            element.appendChild(text);\n        }\n    }\n};\nconst find_dynamic_placeholder_wrappers = (config) => {\n    const output_list = document.querySelectorAll(\".placeholder-value[data-placeholder]\");\n    for (const element of output_list) {\n        const placeholder_name = element.getAttribute(\"data-placeholder\");\n        if (placeholder_name) {\n            const placeholder = config.placeholders.get(placeholder_name);\n            if (placeholder) {\n                placeholder.output_elements.push(element);\n            }\n            else {\n                console.warn(`No placeholder named '${placeholder_name}', that is referenced by element:`, element);\n            }\n        }\n        else {\n            console.warn(`Element has empty/no attribute 'data-placeholder':`, element);\n        }\n    }\n};\n",
+        "import { logger } from \"./debug\";\nimport { safe_replace_multiple_placeholders_in_string } from \"./replacer\";\nimport { clear_state } from \"./state_manager\";\n// Should be a directed acyclical graph\nexport class DependencyGraph {\n    constructor(placeholders) {\n        this.nodes = new Map();\n        for (const placeholder of placeholders.values()) {\n            this.nodes.set(placeholder.name, new GraphNode(placeholder));\n        }\n        // Needs to be in different loops to ensure that all nodes have been created first\n        for (const placeholder of placeholders.values()) {\n            try {\n                this.on_placeholder_value_change(placeholder);\n            }\n            catch (e) {\n                console.error(\"Error while building dependency graph\", e);\n                console.warn(\"Placeholder values may be inconsistent. Clearing your localStorage should fix this problem.\");\n                if (confirm(\"We detected a problem with your placeholder values. Resetting them to the defaults should fix this. Should we reset your placeholders?\")) {\n                    clear_state();\n                }\n            }\n        }\n        // Make sure that all expanded values are calculated\n        // We take every node with no downlinks (bottom of the graph) and do a recursive recalculation (upwards).\n        // Not super efficient, but simple to implement\n        for (const node of this.nodes.values()) {\n            if (node.downlinks.length == 0) {\n                node.recalculate_expanded_value(true);\n            }\n        }\n    }\n    debug_print_representation() {\n        let text = \"Dependency graph nodes (DEBUG view):\";\n        for (const node of this.nodes.values()) {\n            const dependencies = node.downlinks.map(n => n.placeholder.name).join(\", \");\n            if (dependencies.length == 0) {\n                text += `\\n${node.placeholder.name} (${node.placeholder.expanded_value}) has no dependencies`;\n            }\n            else {\n                text += `\\n${node.placeholder.name} (${node.placeholder.expanded_value}) depends on ${dependencies}`;\n            }\n        }\n        logger.debug(text);\n    }\n    unmark_everything() {\n        for (const node of this.nodes.values()) {\n            node.marked = false;\n        }\n    }\n    get_node(placeholder) {\n        const node = this.nodes.get(placeholder.name);\n        if (node == undefined) {\n            throw new Error(`Placeholder ${placeholder.name} is not part of the dependency graph`);\n        }\n        else {\n            return node;\n        }\n    }\n    on_placeholder_value_change(placeholder) {\n        const node = this.get_node(placeholder);\n        this.update_placeholder_downlinks(placeholder);\n        if (this.has_loop()) {\n            // Emergency measure: ignore any placeholders in this value. This should fix the loop\n            placeholder.expanded_value = placeholder.current_value;\n            node.downlinks = [];\n            // Also raise an exception to inform the user\n            throw new Error(`Placeholder ${placeholder.name} was part of a loop and has temporarily been made non-recursive`);\n        }\n        else {\n            node.recalculate_expanded_value(true);\n        }\n    }\n    get_all_marked() {\n        const marked = [];\n        for (const node of this.nodes.values()) {\n            if (node.marked) {\n                marked.push(node.placeholder);\n            }\n        }\n        return marked;\n    }\n    get_all_upstream(placeholder) {\n        this.unmark_everything();\n        const node = this.get_node(placeholder);\n        node.recursive_mark_upstream();\n        return this.get_all_marked();\n    }\n    update_placeholder_downlinks(placeholder) {\n        if (!placeholder.allow_nested) {\n            // By definition, non-recursive placeholders can not rely on other placeholders\n            logger.debug(`${placeholder.name} can not contain nested placeholders`);\n            return;\n        }\n        // Step 1: remove all old downlinks\n        const node = this.get_node(placeholder);\n        for (const old_downlink of node.downlinks) {\n            old_downlink.remove_uplink(node);\n        }\n        node.downlinks = [];\n        // Step 2: parse placeholder's value (again)\n        for (const other_node of this.nodes.values()) {\n            // No placeholder should directly be able to contain itself -> ignoring this case.\n            // This should lead to the placeholder's name appearing in it's text, which was probably intended\n            if (other_node != node) {\n                if (string_contains_placeholder(placeholder.current_value, other_node.placeholder)) {\n                    // This placeholders value contains a reference to the other node's placeholder\n                    //  -> This node depends on the other node\n                    node.downlinks.push(other_node);\n                    other_node.uplinks.push(node);\n                }\n            }\n        }\n    }\n    get_all_used_placeholders() {\n        // Also includes all placeholders used by the placeholders that were included\n        this.unmark_everything();\n        // Mark all used placeholders and their downstream nodes\n        for (const node of this.nodes.values()) {\n            if (node.placeholder.count_on_page > 0) {\n                node.recursive_mark_downstream();\n            }\n        }\n        return this.get_all_marked();\n    }\n    has_loop() {\n        // General algorithm: https://www.geeksforgeeks.org/detect-cycle-in-a-graph/\n        this.unmark_everything();\n        for (const node of this.nodes.values()) {\n            // Make sure that we check every single node (we likely have multiple graphs that are not connected)\n            if (!node.marked) {\n                if (this._has_loop([], node)) {\n                    return true;\n                }\n            }\n        }\n        return false;\n    }\n    _has_loop(back_stack, current_node) {\n        const new_back_stack = [...back_stack, current_node];\n        const index = back_stack.indexOf(current_node);\n        if (index != -1) {\n            let message = \"Dependency cycle in placeholders detected:\";\n            for (let i = index; i < new_back_stack.length; i++) {\n                const placeholder = new_back_stack[i].placeholder;\n                message += `\\n$ -> ${placeholder.name}: ${placeholder.current_value}`;\n            }\n            console.warn(message);\n            return true;\n        }\n        else if (!current_node.marked) {\n            // No cycle found yet, scan all children that are not yet marked\n            current_node.marked = true;\n            for (const child of current_node.downlinks) {\n                if (this._has_loop(new_back_stack, child)) {\n                    return true;\n                }\n            }\n            return false;\n        }\n        else {\n            // Already checked, so no need to start recursive scans\n            return false;\n        }\n    }\n}\nconst string_contains_placeholder = (string_to_test, placeholder_to_find) => {\n    return placeholder_to_find.regex_dynamic.test(string_to_test) ||\n        placeholder_to_find.regex_html.test(string_to_test) ||\n        placeholder_to_find.regex_normal.test(string_to_test) ||\n        placeholder_to_find.regex_static.test(string_to_test);\n};\nclass GraphNode {\n    constructor(placeholder) {\n        // These other nodes depend on this node\n        this.uplinks = [];\n        // This are the nodes this node depends on\n        this.downlinks = [];\n        // State used during operations to see if this node was already visited/processed\n        this.marked = false;\n        this.placeholder = placeholder;\n    }\n    remove_uplink(node) {\n        this.uplinks = this.uplinks.filter(x => x != node);\n    }\n    recalculate_expanded_value(recursive) {\n        let expanded_value = this.placeholder.current_value;\n        if (this.placeholder.allow_nested) {\n            expanded_value = safe_replace_multiple_placeholders_in_string(expanded_value, this.downlinks.map(n => n.placeholder));\n        }\n        this.placeholder.expanded_value = expanded_value;\n        if (recursive) {\n            // Recalculate all uplink nodes in recursive too\n            for (const uplink_node of this.uplinks) {\n                uplink_node.recalculate_expanded_value(recursive);\n            }\n        }\n    }\n    recursive_mark_upstream() {\n        this.marked = true;\n        for (const node of this.uplinks) {\n            node.recursive_mark_upstream();\n        }\n    }\n    recursive_mark_downstream() {\n        this.marked = true;\n        for (const node of this.downlinks) {\n            node.recursive_mark_downstream();\n        }\n    }\n}\n",
+        "import { load_checkbox_state, load_dropdown_state, load_textbox_state, load_boolean_setting } from \"./state_manager\";\nimport { parse_validator } from \"./validator\";\nimport { DependencyGraph } from \"./dependency_graph\";\n// This should be a more type safe reimplementation of 10_parse_data.js.\n// It has some breaking changes, since I try to improve how the javascript code works\nexport const assert_field_type = (name, expected_type_str, parent_object) => {\n    const value = parent_object[name];\n    const actual_type_str = typeof (value);\n    if (actual_type_str != expected_type_str) {\n        throw new Error(`Type mismatch: ${name} should be ${expected_type_str}, but is ${actual_type_str}.\\nProblematic object: ${JSON.stringify(parent_object)}`);\n    }\n    else {\n        return value;\n    }\n};\n// These functions are here to make sure, that I the type checker can properly work (since they have a specific return type)\nexport const get_string_field = (name, parent_object) => {\n    return assert_field_type(name, \"string\", parent_object);\n};\nexport const get_boolean_field = (name, parent_object) => {\n    return assert_field_type(name, \"boolean\", parent_object);\n};\nconst get_number_field = (name, parent_object) => {\n    return assert_field_type(name, \"number\", parent_object);\n};\nexport const get_array_field = (name, element_type, parent_object) => {\n    const array = parent_object[name];\n    if (Array.isArray(array)) {\n        for (const [index, entry] of array.entries()) {\n            const actual_type_str = typeof (entry);\n            if (actual_type_str != element_type) {\n                const msg = `Type mismatch: ${name}'s ${index + 1}th element should be ${element_type}, but is ${actual_type_str}.\\nProblematic object: ${JSON.stringify(parent_object)}`;\n                throw new Error(msg);\n            }\n        }\n        return array;\n    }\n    else {\n        throw new Error(`Type mismatch: ${name} should be an array, but is not.\\nProblematic object: ${JSON.stringify(parent_object)}`);\n    }\n};\nexport var InputType;\n(function (InputType) {\n    InputType[\"Textbox\"] = \"TEXTBOX\";\n    InputType[\"Checkbox\"] = \"CHECKBOX\";\n    InputType[\"Dropdown\"] = \"DROPDOWN\";\n})(InputType || (InputType = {}));\nexport const parse_config = (data) => {\n    const placeholder_map = new Map();\n    const textboxes = new Map();\n    const checkboxes = new Map();\n    const dropdowns = new Map();\n    const validator_map = new Map();\n    const validator_data_list = get_array_field(\"validators\", \"object\", data);\n    for (const validator_data of validator_data_list) {\n        const validator = parse_validator(validator_data);\n        if (validator_map.has(validator.id)) {\n            throw new Error(`Multiple validators with id '${validator.id}'`);\n        }\n        else {\n            validator_map.set(validator.id, validator);\n        }\n    }\n    const settings_data = assert_field_type(\"settings\", \"object\", data);\n    const settings = parse_settings(settings_data);\n    const placeholder_data = get_array_field(\"placeholder_list\", \"object\", data);\n    for (let i = 0; i < placeholder_data.length; i++) {\n        const placeholder = parse_any_placeholder(placeholder_data[i], validator_map, settings, i);\n        // Add the placeholder to the correct lists\n        placeholder_map.set(placeholder.name, placeholder);\n        if (placeholder.type == InputType.Textbox) {\n            textboxes.set(placeholder.name, placeholder);\n        }\n        else if (placeholder.type == InputType.Checkbox) {\n            checkboxes.set(placeholder.name, placeholder);\n        }\n        else if (placeholder.type == InputType.Dropdown) {\n            dropdowns.set(placeholder.name, placeholder);\n        }\n        else {\n            console.warn(\"Unknown placeholder type:\", placeholder.type);\n        }\n    }\n    const graph = new DependencyGraph(placeholder_map);\n    return {\n        \"placeholders\": placeholder_map,\n        \"textboxes\": textboxes,\n        \"checkboxes\": checkboxes,\n        \"dropdowns\": dropdowns,\n        \"settings\": settings,\n        \"dependency_graph\": graph,\n        \"input_tables\": [],\n    };\n};\nconst parse_settings = (data) => {\n    const apply_change_on_focus_change_default = get_boolean_field(\"apply_change_on_focus_change\", data);\n    const debug_default = get_boolean_field(\"debug\", data);\n    const expand_auto_tables_default = get_boolean_field(\"expand_auto_tables\", data);\n    return {\n        \"apply_change_on_focus_change\": load_boolean_setting(\"apply_change_on_focus_change\", apply_change_on_focus_change_default),\n        \"debug\": load_boolean_setting(\"debug\", debug_default),\n        \"delay_millis\": get_number_field(\"delay_millis\", data),\n        \"expand_auto_tables\": load_boolean_setting(\"expand_auto_tables\", expand_auto_tables_default),\n        \"highlight_placeholders\": load_boolean_setting(\"highlight_placeholders\", false),\n        // How normal placeholders are marked\n        \"normal_prefix\": get_string_field(\"normal_prefix\", data),\n        \"normal_suffix\": get_string_field(\"normal_suffix\", data),\n        // How placeholders using the innerHTML method are marked\n        \"html_prefix\": get_string_field(\"html_prefix\", data),\n        \"html_suffix\": get_string_field(\"html_suffix\", data),\n        // How placeholders using the direct/static replacement methodare marked\n        \"static_prefix\": get_string_field(\"static_prefix\", data),\n        \"static_suffix\": get_string_field(\"static_suffix\", data),\n        // How placeholders using the dynamic replacement methodare marked\n        \"dynamic_prefix\": get_string_field(\"dynamic_prefix\", data),\n        \"dynamic_suffix\": get_string_field(\"dynamic_suffix\", data),\n    };\n};\nconst escapeRegExp = (regex_pattern) => {\n    // @SOURCE https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions#escaping\n    return regex_pattern.replace(/[.*+?^${}()|[\\]\\\\]/g, \"\\\\$&\"); // $& means the whole matched string\n};\nconst parse_any_placeholder = (data, validator_map, settings, index) => {\n    const type = get_string_field(\"type\", data);\n    // Parse fields that are shared between all placeholders\n    const name = get_string_field(\"name\", data);\n    let parsed = {\n        \"name\": name,\n        \"order_index\": index,\n        // The regexes for the different replace methods. Stored here so that I only need to compile them once\n        \"regex_dynamic\": RegExp(escapeRegExp(settings.dynamic_prefix) + name + escapeRegExp(settings.dynamic_suffix), \"g\"),\n        \"regex_html\": RegExp(escapeRegExp(settings.html_prefix) + name + escapeRegExp(settings.html_suffix), \"g\"),\n        \"regex_normal\": RegExp(escapeRegExp(settings.normal_prefix) + name + escapeRegExp(settings.normal_suffix), \"g\"),\n        \"regex_static\": RegExp(escapeRegExp(settings.static_prefix) + name + escapeRegExp(settings.static_suffix), \"g\"),\n        // \n        \"description\": get_string_field(\"description\", data),\n        \"read_only\": get_boolean_field(\"read_only\", data),\n        \"allow_inner_html\": get_boolean_field(\"allow_inner_html\", data),\n        \"allow_nested\": get_boolean_field(\"allow_nested\", data),\n        \"current_value\": \"UNINITIALIZED\",\n        \"expanded_value\": \"UNINITIALIZED\",\n        \"count_on_page\": 0,\n        \"reload_page_on_change\": false,\n        \"output_elements\": [], // Will be set, when the page is searched\n    };\n    // Parse the type specific attributes\n    if (type === \"textbox\") {\n        const placeholder = finish_parse_textbox(parsed, data, validator_map);\n        load_textbox_state(placeholder);\n        return placeholder;\n    }\n    else if (type == \"checkbox\") {\n        const placeholder = finish_parse_checkbox(parsed, data);\n        load_checkbox_state(placeholder);\n        return placeholder;\n    }\n    else if (type == \"dropdown\") {\n        const placeholder = finish_parse_dropdown(parsed, data);\n        load_dropdown_state(placeholder);\n        return placeholder;\n    }\n    else {\n        throw new Error(`Unsupported placeholder type '${type}'`);\n    }\n};\nconst finish_parse_textbox = (parsed, data, validator_map) => {\n    let default_function, default_value;\n    if (data[\"default_value\"] != undefined) {\n        default_value = get_string_field(\"default_value\", data);\n    }\n    else {\n        const default_js_code = get_string_field(\"default_function\", data);\n        default_function = () => {\n            // Wrap the function, so that we can ensure that errors are properly handled\n            try {\n                const compiled_function = new Function(default_js_code);\n                const result = compiled_function();\n                if (typeof (result) != \"string\") {\n                    throw new Error(`Custom function '${default_js_code}' should return a string, but it returned a ${typeof (result)}: ${result}`);\n                }\n                else {\n                    return result;\n                }\n            }\n            catch (error) {\n                throw new Error(`Failed to evaluate default_function '${default_js_code}' of placeholder ${parsed.name}: ${error}`);\n            }\n        };\n    }\n    const validator_names = get_array_field(\"validators\", \"string\", data);\n    const validator_list = [];\n    for (const name of validator_names) {\n        const validator = validator_map.get(name);\n        if (validator) {\n            validator_list.push(validator);\n        }\n        else {\n            const known_validators = Array.from(validator_map.keys()).join(\", \");\n            throw new Error(`No validator with id '${name}' was found. Known validators are ${known_validators}`);\n        }\n    }\n    return Object.assign(Object.assign({}, parsed), { \"default_function\": default_function, \"default_value\": default_value, \"input_elements\": [], \"type\": InputType.Textbox, \"validators\": validator_list });\n};\nconst finish_parse_checkbox = (parsed, data) => {\n    return Object.assign(Object.assign({}, parsed), { \"checked_by_default\": get_boolean_field(\"checked_by_default\", data), \"current_is_checked\": false, \"input_elements\": [], \"value_checked\": get_string_field(\"value_checked\", data), \"value_unchecked\": get_string_field(\"value_unchecked\", data), \"type\": InputType.Checkbox });\n};\nconst finish_parse_dropdown = (parsed, data) => {\n    const raw_options = get_array_field(\"options\", \"object\", data);\n    const options = [];\n    for (const option of raw_options) {\n        options.push({\n            display_name: get_string_field(\"display_name\", option),\n            value: get_string_field(\"value\", option),\n        });\n    }\n    const default_index = get_number_field(\"default_index\", data);\n    if (default_index < 0) {\n        throw new Error(`Invalid value: \"default_index\" should not be negative, but is ${default_index}.\\nProblematic object: ${JSON.stringify(data)}`);\n    }\n    else if (default_index >= options.length) {\n        throw new Error(`Invalid value: \"default_index\" should be smaller than the number of options (${options.length}), but is ${default_index}.\\nProblematic object: ${JSON.stringify(data)}`);\n    }\n    return Object.assign(Object.assign({}, parsed), { \"current_index\": 0, \"default_index\": default_index, \"input_elements\": [], \"options\": options, \"type\": InputType.Dropdown });\n};\n",
+        "import { logger } from \"./debug\";\nimport { prepare_input_field } from \"./inputs\";\nimport { create_dynamic_placeholder_element } from \"./replacer\";\nimport { clear_settings, clear_state, store_boolean_setting } from \"./state_manager\";\nconst TABLE_CELL_HEADINGS = new Map();\nTABLE_CELL_HEADINGS.set(\"name\", \"Name\");\nTABLE_CELL_HEADINGS.set(\"description\", \"Description\");\nTABLE_CELL_HEADINGS.set(\"value\", \"Value\");\nTABLE_CELL_HEADINGS.set(\"input\", \"Input element\");\nTABLE_CELL_HEADINGS.set(\"description-or-name\", \"Description / name\");\n// Created myself, so no licensing issues should occur. Still, a decent unicode / font awesome icon may be better if it works across themes/operating systems/browsers\nconst GEAR_SVG = `<svg viewBox=\"0 0 40 40\" xmlns=\"http://www.w3.org/2000/svg\">\n <path id=\"svg_6\" d=\"m7.79338,20.02127l0,0c0,-6.84327 5.74307,-12.39083 12.82751,-12.39083l0,0c3.40207,0 6.6648,1.30546 9.07042,3.62919c2.40563,2.32373 3.75709,5.47539 3.75709,8.76164l0,0c0,6.84327 -5.74307,12.39083 -12.82751,12.39083l0,0c-7.08444,0 -12.82751,-5.54757 -12.82751,-12.39083zm6.41376,0l0,0c0,3.42163 2.87154,6.19542 6.41376,6.19542c3.54222,0 6.41376,-2.77378 6.41376,-6.19542c0,-3.42163 -2.87154,-6.19542 -6.41376,-6.19542l0,0c-3.54222,0 -6.41376,2.77378 -6.41376,6.19542z\" stroke=\"#fff\" fill=\"#ffffff\"/>\n <path id=\"svg_7\" d=\"m17.46095,7.63098l1.2691,-5.24017l4.23035,0l1.2691,5.24017l-6.76856,0z\" stroke=\"#fff\" fill=\"#ffffff\"/>\n <path transform=\"rotate(180, 20.9544, 35.1419)\" id=\"svg_11\" d=\"m17.57012,37.76199l1.2691,-5.24017l4.23035,0l1.2691,5.24017l-6.76856,0z\" stroke=\"#fff\" fill=\"#ffffff\"/>\n <path transform=\"rotate(43, 31.5439, 9.59605)\" id=\"svg_12\" d=\"m28.15964,12.21614l1.2691,-5.24017l4.23035,0l1.2691,5.24017l-6.76856,0z\" stroke=\"#fff\" fill=\"#ffffff\"/>\n <path transform=\"rotate(90, 35.9107, 19.8581)\" id=\"svg_13\" d=\"m32.52645,22.47815l1.2691,-5.24017l4.23035,0l1.2691,5.24017l-6.76856,0z\" stroke=\"#fff\" fill=\"#ffffff\"/>\n <path transform=\"rotate(135, 31.7623, 30.2292)\" id=\"svg_14\" d=\"m28.37798,32.84933l1.2691,-5.24017l4.23035,0l1.2691,5.24017l-6.76856,0z\" stroke=\"#fff\" fill=\"#ffffff\"/>\n <path transform=\"rotate(-45, 9.49152, 9.48688)\" id=\"svg_15\" d=\"m6.10724,12.10697l1.2691,-5.24017l4.23035,0l1.2691,5.24017l-6.76856,0z\" stroke=\"#fff\" fill=\"#ffffff\"/>\n <path transform=\"rotate(-90, 5.01553, 19.9672)\" id=\"svg_16\" d=\"m1.63126,22.58732l1.2691,-5.24017l4.23035,0l1.2691,5.24017l-6.76856,0z\" stroke=\"#fff\" fill=\"#ffffff\"/>\n <path transform=\"rotate(-135, 9.60069, 30.7751)\" id=\"svg_17\" d=\"m6.21641,33.39518l1.2691,-5.24017l4.23035,0l1.2691,5.24017l-6.76856,0z\" stroke=\"#fff\" fill=\"#ffffff\"/>\n</svg>`;\n// Helper functions to simplify the following code\nconst appendTextNode = (element, text) => {\n    element.appendChild(document.createTextNode(text));\n};\nconst createChildElement = (parent, tag_name) => {\n    const child = document.createElement(tag_name);\n    parent.appendChild(child);\n    return child;\n};\nconst convert_to_dynamic_placeholder_table = (config, element, content_element) => {\n    // Remove the current contents. This enables the plugin to generate fallback contents in case the JavaScript code does not work\n    element.innerHTML = \"\";\n    const title = createChildElement(element, \"div\");\n    const title_text = createChildElement(title, \"div\");\n    const settings_button = createChildElement(title, \"div\");\n    const expandable_contents = createChildElement(element, \"div\");\n    const settings_contents = createChildElement(expandable_contents, \"div\");\n    expandable_contents.append(content_element);\n    const update_expanded_state = (is_expanded) => {\n        expandable_contents.style.display = is_expanded ? \"flex\" : \"none\";\n        title_text.textContent = \"Placeholders: Click here to \" + (is_expanded ? \"collapse\" : \"expand\");\n    };\n    title.classList.add(\"auto-table-title\");\n    expandable_contents.classList.add(\"expandable_contents\");\n    settings_contents.classList.add(\"settings_contents\");\n    let expanded = config.settings.expand_auto_tables;\n    update_expanded_state(expanded);\n    title_text.addEventListener(\"click\", () => {\n        expanded = !expanded;\n        update_expanded_state(expanded);\n    });\n    title_text.classList.add(\"text\");\n    prepare_settings_button(settings_button, settings_contents, () => {\n        if (!expanded) {\n            expanded = true;\n            update_expanded_state(expanded);\n        }\n    });\n    fill_settings_content_container(config, settings_contents);\n};\nconst prepare_settings_button = (settings_button, settings_contents, expand_if_needed) => {\n    let show_settings = false;\n    settings_button.onclick = (e) => {\n        e.preventDefault();\n        e.stopPropagation();\n        show_settings = !show_settings;\n        settings_contents.style.display = show_settings ? \"flex\" : \"none\";\n        if (show_settings) {\n            expand_if_needed();\n        }\n    };\n    settings_contents.style.display = show_settings ? \"flex\" : \"none\";\n    settings_button.classList.add(\"settings_button\");\n    settings_button.innerHTML = GEAR_SVG;\n    settings_button.title = \"Hide / show settings\";\n};\nconst fill_settings_content_container = (config, settings_contents) => {\n    const set_highlight_placeholders = (enabled) => {\n        for (const placeholder of config.placeholders.values()) {\n            for (const output of placeholder.output_elements) {\n                if (enabled) {\n                    output.classList.add(\"placeholder-value-highlighted\");\n                }\n                else {\n                    output.classList.remove(\"placeholder-value-highlighted\");\n                }\n            }\n        }\n    };\n    set_highlight_placeholders(config.settings.highlight_placeholders);\n    createChildElement(settings_contents, \"b\").textContent = \"Settings\";\n    // @TODO: later: when there are multiple settings dialogs, keep their values in sync\n    append_boolean_setting_checkbox(settings_contents, config.settings.expand_auto_tables, \"expand_auto_tables\", \"Expand placeholder tables by default*\");\n    append_boolean_setting_checkbox(settings_contents, config.settings.apply_change_on_focus_change, \"apply_change_on_focus_change\", \"Apply value when focus changes away*\");\n    append_boolean_setting_checkbox(settings_contents, config.settings.debug, \"debug\", \"Log JavaScript debug messages to console*\");\n    append_boolean_setting_checkbox(settings_contents, config.settings.highlight_placeholders, \"highlight_placeholders\", \"Highlight placeholders (useful for debugging)\", set_highlight_placeholders);\n    createChildElement(settings_contents, \"i\").textContent = \"* You need to reload the page for these settings to take effect.\";\n    const settings_button_bar = createChildElement(settings_contents, \"div\");\n    settings_button_bar.classList.add(\"button-bar\");\n    const settings_reset_button = createChildElement(settings_button_bar, \"button\");\n    settings_reset_button.textContent = \"Reset settings\";\n    settings_reset_button.addEventListener(\"click\", clear_settings);\n    const placeholder_reset_button = createChildElement(settings_button_bar, \"button\");\n    placeholder_reset_button.textContent = \"Reset all placeholders\";\n    placeholder_reset_button.addEventListener(\"click\", clear_state);\n};\nconst append_boolean_setting_checkbox = (parent_element, value, name, label_text, custom_on_change = (enabled) => { }) => {\n    const label = createChildElement(parent_element, \"label\");\n    label.textContent = `${label_text} `;\n    const checkbox = createChildElement(label, \"input\");\n    checkbox.type = \"checkbox\";\n    checkbox.checked = value;\n    checkbox.addEventListener(\"change\", () => {\n        store_boolean_setting(name, checkbox.checked);\n        custom_on_change(checkbox.checked);\n    });\n};\nconst generate_automatic_placeholder_table = (element, columns, config, placeholders_to_show, show_empty) => {\n    placeholders_to_show = sort_and_remove_duplicate_placeholders(placeholders_to_show);\n    const root_element = document.createElement(\"div\");\n    if (placeholders_to_show.length == 0) {\n        if (show_empty) {\n            root_element.textContent = \"No placeholders to be shown\";\n        }\n        else {\n            // Remove the table placeholder\n            element.remove();\n            // No need constructing something that is never added to the DOM -> return immediately\n            return;\n        }\n    }\n    else {\n        logger.info(\"Creating automatic input table at\", element, \"with columns\", columns);\n        root_element.classList.add(\"table-div\");\n        createChildElement(root_element, \"b\").innerHTML = \"Enter different values in the table below and press <code>Enter</code> to update this page.\";\n        const table = createChildElement(root_element, \"table\");\n        const table_head = createChildElement(table, \"thead\");\n        const table_head_row = createChildElement(table_head, \"tr\");\n        const table_body = createChildElement(table, \"tbody\");\n        for (const column of columns) {\n            const table_cell = createChildElement(table_head_row, \"th\");\n            const heading = TABLE_CELL_HEADINGS.get(column);\n            if (heading) {\n                appendTextNode(table_cell, heading);\n            }\n            else {\n                appendTextNode(table_cell, column);\n                console.error(`Unknown column name: ${column}`);\n            }\n        }\n        const rows = [];\n        for (const placeholder of placeholders_to_show) {\n            if (placeholder.read_only) {\n                logger.debug(`auto_table: Skipping ${placeholder.name} because it is read-only`);\n                continue;\n            }\n            const row = createChildElement(table_body, \"tr\");\n            populate_auto_table_row(row, placeholder, columns, config);\n            rows.push({\n                \"element\": row,\n                \"placeholder\": placeholder,\n            });\n        }\n        config.input_tables.push({\n            \"columns\": columns,\n            \"table_element\": table,\n            \"rows\": rows,\n        });\n    }\n    // Wrap the result in a collapsible wrapper\n    convert_to_dynamic_placeholder_table(config, element, root_element);\n};\nconst sort_and_remove_duplicate_placeholders = (placeholder_list) => {\n    return [...new Set(placeholder_list)].sort((a, b) => a.order_index - b.order_index);\n};\nconst populate_auto_table_row = (row, placeholder, columns, config) => {\n    for (const column of columns) {\n        const cell = createChildElement(row, \"td\");\n        if (column == \"name\") {\n            appendTextNode(cell, placeholder.name);\n        }\n        else if (column == \"description\") {\n            appendTextNode(cell, placeholder.description);\n        }\n        else if (column == \"value\") {\n            const dynamic_placeholer = create_dynamic_placeholder_element(placeholder);\n            cell.appendChild(dynamic_placeholer);\n            placeholder.output_elements.push(dynamic_placeholer);\n        }\n        else if (column == \"input\") {\n            const input = createChildElement(cell, \"input\");\n            prepare_input_field(config, placeholder, input);\n        }\n        else if (column == \"description-or-name\") {\n            const text = placeholder.description || placeholder.name;\n            appendTextNode(cell, text);\n        }\n        else {\n            console.error(`Unknown column name: ${column}`);\n        }\n    }\n};\nconst update_auto_table = (config, table, new_placeholder_list) => {\n    // Sort them the same way they are sorted in the table -> lists are easy to compare\n    new_placeholder_list = sort_and_remove_duplicate_placeholders(new_placeholder_list);\n    // Step 1: remove rows that are no longer to be shown\n    const rows_to_keep = [];\n    for (const row of table.rows) {\n        if (new_placeholder_list.includes(row.placeholder)) {\n            rows_to_keep.push(row);\n        }\n        else {\n            logger.debug(`Removed table row for ${row.placeholder.name}:`, row.element);\n            row.element.remove();\n        }\n    }\n    // Step 2: add rows that do not yet exist\n    const final_rows = [];\n    const reversed_current = [...rows_to_keep].reverse();\n    const reversed_new = [...new_placeholder_list].reverse();\n    let next_new;\n    while (next_new = reversed_new.pop()) {\n        // const next_new = reversed_new.pop();\n        const next_current = reversed_current.slice(-1)[0];\n        if (next_current && next_current.placeholder === next_new) {\n            // The row is already in the table\n            reversed_current.pop(); // remove from queue to keep in sync with other queue\n            final_rows.push(next_current);\n        }\n        else {\n            const element = document.createElement(\"tr\");\n            // insert at the correct position in the dom\n            if (final_rows.length == 0) {\n                // adds it before the first child or if it does not exist at the end (which would also be the first element :D)\n                table.table_element.insertBefore(element, table.table_element.firstChild);\n            }\n            else {\n                // insert it after the last row that was processed\n                const last_node = final_rows[final_rows.length - 1].element;\n                last_node.insertAdjacentElement(\"afterend\", element);\n            }\n            populate_auto_table_row(element, next_new, table.columns, config);\n            final_rows.push({\n                \"element\": element,\n                \"placeholder\": next_new,\n            });\n            logger.debug(`Added table row for ${next_new.name}:`, element);\n        }\n    }\n    // Store the updated row information in the original table object\n    table.rows = final_rows;\n};\nexport const update_all_auto_tables = (config) => {\n    logger.debug(`Updating ${config.input_tables.length} automatic input tables`);\n    if (config.input_tables.length > 0) {\n        const new_placeholder_list = config.dependency_graph.get_all_used_placeholders();\n        for (const table of config.input_tables) {\n            update_auto_table(config, table, new_placeholder_list);\n        }\n    }\n};\nexport const initialize_auto_tables = (config) => {\n    const element_list = document.querySelectorAll(\"div.auto-input-table\");\n    if (element_list.length > 0) {\n        const used_placeholders = config.dependency_graph.get_all_used_placeholders().filter(x => !x.read_only);\n        for (const element of element_list) {\n            if (element instanceof HTMLElement) {\n                const columns_str = element.getAttribute(\"data-columns\") || \"name,input\";\n                const columns = columns_str.includes(\",\") ? columns_str.split(\",\") : [columns_str];\n                const show_empty = element.getAttribute(\"data-hide-empty\") === null;\n                generate_automatic_placeholder_table(element, columns, config, used_placeholders, show_empty);\n            }\n            else {\n                console.warn(\"Element\", element, \"is expected to be an HTMLElement, but is not\");\n            }\n        }\n    }\n};\n",
+        "import { update_all_auto_tables } from \"./auto_tables\";\nimport { logger, reload_page } from \"./debug\";\nimport { InputType } from \"./parse_settings\";\nimport { replace_dynamic_placeholder_values } from \"./replacer\";\nimport { store_checkbox_state, store_dropdown_state, store_textbox_state } from \"./state_manager\";\nimport { validate_textbox_input_field } from \"./validator\";\nexport const initialize_all_input_fields = (config) => {\n    const input_list = document.querySelectorAll(\"input[data-input-for], select[data-input-for]\");\n    for (let input_element of input_list) {\n        const placeholder_name = input_element.getAttribute(\"data-input-for\");\n        if (placeholder_name == null) {\n            throw new Error(\"How can this be, the selector forces the 'data-input-for' attribute to exist\");\n        }\n        const placeholder = config.placeholders.get(placeholder_name);\n        if (placeholder) {\n            prepare_input_field(config, placeholder, input_element);\n        }\n        else {\n            console.warn(`Unknown placeholder referenced in input element: '${placeholder_name}'`);\n            input_element.classList.add(\"input-for-variable\");\n            input_element.value = `ERROR_UNDEFINED_PLACEHOLDER: ${placeholder_name}`;\n        }\n    }\n};\nexport const prepare_input_field = (config, placeholder, input_element) => {\n    input_element.classList.add(\"input-for-variable\");\n    if (placeholder.type == InputType.Checkbox) {\n        initialize_input_checkbox(config, placeholder, input_element);\n    }\n    else if (placeholder.type == InputType.Dropdown) {\n        initialize_input_dropdown(config, placeholder, input_element);\n    }\n    else if (placeholder.type == InputType.Textbox) {\n        initialize_input_textbox(config, placeholder, input_element);\n    }\n    else {\n        console.error(`Placeholder ${placeholder.name} has unknown type '${placeholder.type}'`);\n    }\n};\nconst initialize_input_checkbox = (config, placeholder, input_element) => {\n    if (input_element.tagName != \"INPUT\") {\n        console.warn(`Input element/tag for placeholder '${placeholder.name}' is expected to be INPUT, but is ${input_element.tagName}. Skipping`, input_element);\n        return;\n    }\n    input_element.type = \"checkbox\";\n    input_element.checked = placeholder.current_is_checked;\n    if (placeholder.read_only) {\n        // disable the checkbox\n        input_element.disabled = true;\n    }\n    else {\n        input_element.disabled = false;\n        // Listen for state changes\n        input_element.addEventListener(\"change\", () => {\n            logger.debug(\"Checkbox change\", placeholder.name, \"- new value:\", input_element.checked);\n            store_checkbox_state(placeholder, input_element.checked);\n            placeholder.current_value = input_element.checked ? placeholder.value_checked : placeholder.value_unchecked;\n            on_placeholder_change(config, placeholder);\n        });\n    }\n    // Store this input element\n    placeholder.input_elements.push(input_element);\n};\nconst initialize_input_dropdown = (config, placeholder, input_element) => {\n    const new_node = document.createElement(\"select\");\n    new_node.classList.add(\"placeholder-dropdown\");\n    for (const option of placeholder.options) {\n        const option_element = document.createElement(\"option\");\n        option_element.text = option.display_name; // @TODO: allow placeholders in here\n        new_node.appendChild(option_element);\n    }\n    // Replace input element entirely with the dropdown menu\n    if (input_element.parentNode) {\n        input_element.parentNode.replaceChild(new_node, input_element);\n    }\n    else {\n        // How would we find it in the DOM if it has no parent?\n        console.error(`Input element`, input_element, `for placeholder ${placeholder.name} has no parent!`);\n    }\n    // Select the stored option\n    new_node.selectedIndex = placeholder.current_index;\n    if (placeholder.read_only) {\n        // disable the dropdown\n        new_node.disabled = true;\n    }\n    else {\n        new_node.disabled = false;\n        // Add an event listener\n        new_node.addEventListener(\"change\", () => {\n            logger.debug(\"Dropdown change\", placeholder.name, \"- new index:\", new_node.selectedIndex);\n            store_dropdown_state(placeholder, new_node.selectedIndex);\n            placeholder.current_index = new_node.selectedIndex;\n            placeholder.current_value = placeholder.options[new_node.selectedIndex].value;\n            on_placeholder_change(config, placeholder);\n        });\n    }\n    // Store this input element\n    placeholder.input_elements.push(new_node);\n};\nconst initialize_input_textbox = (config, placeholder, input_element) => {\n    if (input_element.tagName != \"INPUT\") {\n        console.warn(`Input element/tag for placeholder '${placeholder.name}' is expected to be INPUT, but is ${input_element.tagName}. Skipping`, input_element);\n        return;\n    }\n    // Restore the stored state\n    input_element.value = placeholder.current_value;\n    if (placeholder.read_only) {\n        // disable the checkbox\n        input_element.disabled = true;\n        input_element.style.cursor = \"not-allowed\";\n    }\n    else {\n        input_element.disabled = false;\n        if (placeholder.default_value != undefined) {\n            input_element.placeholder = `Default: ${placeholder.default_value}`;\n        }\n        else {\n            input_element.placeholder = \"Dynamic default value\";\n        }\n        const confirm_change = () => {\n            if (placeholder.current_value == input_element.value) {\n                logger.debug(`Value for placeholder ${placeholder.name} was not changed`);\n            }\n            else {\n                // Expensive actions, only perform them if the value was actually changed\n                if (validate_textbox_input_field(placeholder, input_element)) {\n                    store_textbox_state(placeholder, input_element.value);\n                    placeholder.current_value = input_element.value;\n                    on_placeholder_change(config, placeholder);\n                    // The new value is applied, so it now is the same as the stored one\n                    input_element.classList.remove(\"value-modified\");\n                }\n            }\n        };\n        // Check if initial value is valid and initialize the tooltip\n        validate_textbox_input_field(placeholder, input_element);\n        // Listen for state changes\n        input_element.addEventListener(\"input\", () => {\n            // The text was probably modified, so we need to update the validator\n            validate_textbox_input_field(placeholder, input_element);\n            // Update the changed status of the placeholder\n            if (input_element.value == placeholder.current_value) {\n                input_element.classList.remove(\"value-modified\");\n            }\n            else {\n                input_element.classList.add(\"value-modified\");\n            }\n        });\n        input_element.addEventListener(\"keypress\", (event) => {\n            if (event.key === \"Enter\") {\n                logger.debug(\"Textbox change confirmed with Enter key for\", placeholder.name, \"- new value:\", input_element.value);\n                confirm_change();\n            }\n        });\n        input_element.addEventListener(\"keydown\", (event) => {\n            // I have no idea, why Escape does not work with the keypress event (Safari on MacOS). As a work aroud, we listen to the keydown event\n            if (event.key === \"Escape\") {\n                logger.debug(\"Resetting input field for \", placeholder.name, \" to current placeholder value\");\n                input_element.value = placeholder.current_value;\n            }\n        });\n        input_element.addEventListener(\"focusout\", () => {\n            // The value may change on the fly (use changes settings), so we can not just conditionally add the event listener, but need to check each time\n            if (config.settings.apply_change_on_focus_change) {\n                logger.debug(\"Textbox change confirmed by changing focus\", placeholder.name, \"- new value:\", input_element.value);\n                confirm_change();\n            }\n        });\n    }\n    // Store this input element\n    placeholder.input_elements.push(input_element);\n};\nconst on_placeholder_change = (config, placeholder) => {\n    const affected_placeholders = config.dependency_graph.get_all_upstream(placeholder);\n    let require_reload = false;\n    for (const ph of affected_placeholders) {\n        require_reload = require_reload || ph.reload_page_on_change;\n    }\n    logger.debug(`Change of ${placeholder.name} requires updates for placeholders:\\n${affected_placeholders.map(p => ` - ${p.name}\\n`).join(\"\")}\\nRequires reload: ${require_reload}`);\n    if (require_reload) {\n        reload_page(); // for now we just use the full reload\n    }\n    else {\n        config.dependency_graph.on_placeholder_value_change(placeholder);\n        // update auto-tables, since downstream may be changed\n        update_all_auto_tables(config);\n        // Update all input elements for the modified placeholder\n        if (placeholder.type == InputType.Checkbox) {\n            const ph = placeholder;\n            for (const input_element of ph.input_elements) {\n                input_element.checked = ph.current_is_checked;\n            }\n        }\n        else if (placeholder.type == InputType.Dropdown) {\n            const ph = placeholder;\n            for (const input_element of ph.input_elements) {\n                input_element.selectedIndex = ph.current_index;\n            }\n        }\n        else if (placeholder.type == InputType.Textbox) {\n            const ph = placeholder;\n            for (const input_element of ph.input_elements) {\n                input_element.value = ph.current_value;\n                validate_textbox_input_field(ph, input_element);\n            }\n        }\n        else {\n            console.warn(`Placeholder ${placeholder.name} has unexpected type '${placeholder.type}'`);\n        }\n        // @TODO Not needed as long as the dropdown display name is static\n        // // Update input elements\n        // for (const ph of affected_placeholders) {\n        //     // Only dropdown's input elements can depend on other placeholders (the label)\n        //     if (ph.type == InputType.Dropdown) {\n        //         for (const input of (ph as DropdownPlaceholder).input_elements) {\n        //             // code here\n        //         }\n        //     }\n        // }\n        // Update output elements\n        replace_dynamic_placeholder_values(affected_placeholders);\n    }\n};\n",
         "import { parse_config } from \"./parse_settings\";\nimport { init_logging, logger } from \"./debug\";\nimport { replace_placeholders_in_subtree } from \"./replacer\";\nimport { initialize_all_input_fields } from \"./inputs\";\nimport { export_api_functions } from \"./api\";\nimport { initialize_auto_tables } from \"./auto_tables\";\nexport const main = () => {\n    const config = parse_config(window.PlaceholderPluginConfigJson);\n    init_logging(config.settings.debug);\n    logger.info(\"PluginConfig\", config);\n    export_api_functions(config);\n    const delay_millis = config.settings.delay_millis;\n    // Then do the placeholder replacing at the user-specified time\n    if (delay_millis < 0) {\n        // For values smaller than 0, immediately do the replacements\n        do_plugin_stuff(config);\n    }\n    else if (delay_millis == 0) {\n        // Replace placeholders as soon as the page finished loading\n        window.addEventListener(\"load\", () => do_plugin_stuff(config));\n    }\n    else {\n        // Wait the amount of millis specified by the user\n        window.addEventListener(\"load\", () => {\n            setTimeout(() => do_plugin_stuff(config), delay_millis);\n        });\n    }\n};\nconst do_plugin_stuff = (config) => {\n    replace_placeholders_in_subtree(document.body, config);\n    config.dependency_graph.debug_print_representation();\n    initialize_all_input_fields(config);\n    initialize_auto_tables(config);\n};\n",
         "import { debug_disable_reload } from \"./debug\";\nexport const export_api_functions = (config) => {\n    window.PlaceholderPlugin = {\n        \"settings\": config.settings,\n        \"placeholders\": config.placeholders,\n        \"debug_disable_reload\": debug_disable_reload,\n        \"debug_print_dependency_graph\": () => config.dependency_graph.debug_print_representation(),\n    };\n};\n",
         "import { main } from \"./main\";\n// If the data is loaded via another script, make it work in any order\nif (window.PlaceholderPluginConfigJson) {\n    main();\n}\nelse {\n    document.addEventListener(\"PlaceholderPluginConfigJson\", main);\n}\n"
     ],
     "version": 3
 }
```

### Comparing `mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/assets.py` & `mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/static/placeholder_replacer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,127 +1,104 @@
-import json
-import os
-import shutil
-from typing import Any
+import html
+import random
+import string
+import time
 # local
-from mkdocs.config.defaults import MkDocsConfig
-from .plugin_config import PlaceholderPluginConfig
-from .placeholder_data import Placeholder, InputType
-from .style import generate_style_sheet
-from .validators import validator_to_dict
+from ..config import PlaceholderConfig, Placeholder
 
+SAFE_CHARS_IN_MARKDOWN = list(string.ascii_letters + string.digits)
+CACHED_EXPANDED_DEFAULT_VALUES: dict[str,str] = {}
 
-def _write_to_file(config: MkDocsConfig, relative_path: str, contents: str, open_mode: str) -> None:
-    file_path = os.path.join(config.site_dir, relative_path)
-    parent_dir = os.path.dirname(file_path)
-    os.makedirs(parent_dir, exist_ok=True)
-    with open(file_path, open_mode) as f:
-        f.write(contents)
-
-def copy_assets_to_mkdocs_site_directory(config: MkDocsConfig, plugin_config: PlaceholderPluginConfig, placeholders: dict[str, Placeholder]):
-    """
-    Copy the JavaScript file to the site (if necessary) and replace the placeholder string with the actual data
+def paraniod_html_escape(input: str) -> str:
     """
-    # @TODO: merge everything into a single file if debug==false
-    custom_js_path = os.path.join(config.site_dir, plugin_config.placeholder_js)
-    if os.path.exists(custom_js_path):
-        # use the file that is already in the site directory
-        with open(custom_js_path, "r") as f:
-            text = f.read()
-    else:
-        # use the default file supplied by the plugin
-        input_file = get_resource_path("assets/placeholder-data.js")
-        with open(input_file, "r") as f:
-            text = f.read()
-
-    if plugin_config.placeholder_css:
-        theme_name = config.theme.name or "mkdocs"
-        css_text = generate_style_sheet(theme_name, plugin_config.debug_javascript)
-        _write_to_file(config, plugin_config.placeholder_css, css_text, "a")
-
-    # Add extra JS
-    if (plugin_config.placeholder_extra_js):
-        with open(plugin_config.placeholder_extra_js, "r") as f:
-            extra_js = f.read()
-
-        text = "///// Custom extra JS code /////\n" + extra_js + "\n///// Normal JS code /////\n" + text
-
-    # Generate placeholder data and inject them in the JavaScript file
-    text = text.replace("__MKDOCS_PLACEHOLDER_PLUGIN_NEW_JSON__", generate_new_placeholder_json(placeholders, plugin_config))
-    _write_to_file(config, plugin_config.placeholder_js, text, "w")
-
-    parent_dir = os.path.dirname(custom_js_path)
-    shutil.copy(get_resource_path("assets/placeholder.min.js"), parent_dir)
-    shutil.copy(get_resource_path("assets/placeholder.min.js.map"), parent_dir)
-
-
-def get_resource_path(name: str) -> str:
-    """
-    Gets the path to a file in the same directory as this file
-    """
-    current_dir = os.path.dirname(__file__)
-    return os.path.join(current_dir, name)
+    Escapes every character as HTML entities except a couple allow listed ones.
+    Why? Because a lot of characters can cause unwanted problems in markdown parsing (*, \n, _, `, (, |, space, etc).
+    """
+    return "".join([char if char in SAFE_CHARS_IN_MARKDOWN else f"&#{ord(char)};"
+         for char in input])
+
+def html_for_dynamic_placeholder(placeholder: Placeholder, config: PlaceholderConfig) -> str:
+    placeholder_default_value = placeholder_expanded_default_value(placeholder, config)
+    # no need to escape the placeholder name, since I do strict validation on it when I parse the placeholders
+    return f'<span class="placeholder-value" data-placeholder="{placeholder.name}">{html.escape(placeholder_default_value)}</span>'
+
+def get_all_placeholder_patterns(placeholder: Placeholder, config: PlaceholderConfig) -> list[str]:
+    s = config.settings
+    return [
+        s.dynamic_prefix + placeholder.name + s.dynamic_suffix,
+        s.html_prefix + placeholder.name + s.html_suffix,
+        s.normal_prefix + placeholder.name + s.normal_suffix,
+        s.static_prefix + placeholder.name + s.static_suffix,
+    ]
+
+def placeholder_expanded_default_value(placeholder: Placeholder, config: PlaceholderConfig) -> str:
+    # This speeds up the somewhat expensive operation by caching the results
+    value = CACHED_EXPANDED_DEFAULT_VALUES.get(placeholder.name)
+    if value is None:
+        value = _placeholder_expanded_default_value(placeholder, config)
+        CACHED_EXPANDED_DEFAULT_VALUES[placeholder.name] = value
+    return value
+
+def _placeholder_expanded_default_value(placeholder: Placeholder, config: PlaceholderConfig) -> str:
+    if placeholder.default_function:
+        return "<JAVASCRIPT_FUNCTION>"
+
+    default_value = placeholder.default_value
+    if placeholder.values:
+        default_value = placeholder.values[default_value]
 
+    if not placeholder.allow_nested:
+        return default_value
+    else:
+        # This works similar to safe_replace_multiple_placeholders_in_string in replacer.ts.
+        # The roundabout way is needed to ensure that placeholders that are in a previously replaced placeholder's value are not replaced
+        string = default_value
+        unique = f"{int(time.time())}_{random.randint(0, 10000)}"
+        for placeholder in config.placeholders.values():
+            for pattern in get_all_placeholder_patterns(placeholder, config):
+                string = string.replace(pattern, f"x{placeholder.name}_{unique}x")
+
+        for placeholder in config.placeholders.values():
+            pattern = f"x{placeholder.name}_{unique}x"
+            if pattern in string:
+                expanded_value = placeholder_expanded_default_value(placeholder, config)
+                string = string.replace(pattern, expanded_value)
+
+        return string
+
+
+class DynamicPlaceholderPreprocessor:
+    """
+    This class replaces dynamic placeholders with the same elements as the javascript would.
+    However, if JavaScript is disabled, it will show the default value instead of the placeholder name.
+    """
+    def __init__(self, config: PlaceholderConfig) -> None:
+        self.config = config
+        self.unique = f"{int(time.time())}_{random.randint(0, 10000)}"
+
+    def handle_markdown_page(self, page_markdown: str) -> str:
+        # Mark placeholders to replace in the Markdown, so that the automatic input tables, input replacements, etc
+
+        # This works similar to safe_replace_multiple_placeholders_in_string in replacer.ts.
+        # The roundabout way is needed to ensure that placeholders that are in a previously replaced placeholder's value are not replaced
+        for placeholder in self.config.placeholders.values():
+            replace_with_value = f"x{placeholder.name}_{self.unique}x"
+
+            # Handle explicitely maked dynamic placeholders
+            search_expression = self.config.settings.dynamic_prefix + placeholder.name + self.config.settings.dynamic_suffix
+            page_markdown = page_markdown.replace(search_expression, replace_with_value)
+
+            # Handle normal placeholders, whic are currently just an alias for dynamic placeholders
+            search_expression = self.config.settings.normal_prefix + placeholder.name + self.config.settings.normal_suffix
+            page_markdown = page_markdown.replace(search_expression, replace_with_value)
+        
+        return page_markdown
+
+    def handle_html_page(self, page_html: str) -> str:
+        # needs to happen in the HTML document, since otherwise listings will screw things up
+        for placeholder in self.config.placeholders.values():
+            search_expression = f"x{placeholder.name}_{self.unique}x"
+            replace_with_value = html_for_dynamic_placeholder(placeholder, self.config)
+            page_html = page_html.replace(search_expression, replace_with_value)
 
-def generate_new_placeholder_json(placeholders: dict[str, Placeholder], plugin_config: PlaceholderPluginConfig) -> str:
-    """
-    Generate the JSON string, that will replace the placeholder in the JavaScript file
-    """
-    placeholder_data_list = []
-    validator_map = {}
+        return page_html
 
-    for placeholder in placeholders.values():
-        placeholder_data = {
-            "name": placeholder.name,
-            "description": placeholder.description,
-            "read_only": placeholder.read_only,
-            "allow_inner_html": placeholder.replace_everywhere,
-        }
-        if placeholder.input_type == InputType.Checkbox:
-            placeholder_data.update({
-                "type": "checkbox",
-                "value_checked": placeholder.values["checked"],
-                "value_unchecked": placeholder.values["unchecked"],
-                "checked_by_default": bool(placeholder.default_value == "checked"),
-            })
-        elif placeholder.input_type == InputType.Dropdown:
-            # Figure out the index of the item selected by default
-            default_index = 0
-            for index, value in enumerate(placeholder.values.keys()):
-                if placeholder.default_value == value:
-                    default_index = index
-
-            placeholder_data.update({
-                "type": "dropdown",
-                "default_index": default_index,
-                "options": [{"display_name": key, "value": value} for key, value in placeholder.values.items()],
-            })
-        elif placeholder.input_type == InputType.Field:
-            placeholder_data.update({
-                "type": "textbox",
-                "allow_recursive": True, # @TODO: read from config
-                "validators": [v.id for v in placeholder.validator_list],
-            })
-
-            if placeholder.default_function:
-                placeholder_data["default_function"] = placeholder.default_function
-            else:
-                placeholder_data["default_value"] = placeholder.default_value
-
-        else:
-            raise Exception(f"Unexpected input type: {placeholder.input_type}")
-
-        placeholder_data_list.append(placeholder_data)
-
-        for validator in placeholder.validator_list:
-            # deduplicate validators
-            validator_map[validator.id] = validator_to_dict(validator)
-
-    result_object = {
-        "placeholder_list": placeholder_data_list,
-        "settings": {
-            "debug": plugin_config.debug_javascript,
-            "delay_millis": plugin_config.replace_delay_millis,
-        },
-        "validators": list(validator_map.values()),
-    }
-    return json.dumps(result_object, indent=None, sort_keys=False)
```

### Comparing `mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/html_tag_parser.py` & `mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/html_tag_parser.py`

 * *Files identical despite different names*

### Comparing `mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/input_tag_handler.py` & `mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/html_tag_handler.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,55 +1,69 @@
 import re
-from typing import Callable, Optional, Any
+from typing import Optional
 # local
 from . import warning
 from .html_tag_parser import ParsedHtmlTag, parse_html_tag, create_html_opening_tag
 
-INPUT_TAG_START = re.compile("<input", re.IGNORECASE)
 
-
-class InputTagHandler:
-    def __init__(self, replace_function: Callable[[Any,str,ParsedHtmlTag],str], add_line_in_warning: bool) -> None:
-        self.replace_function = replace_function
+from typing import TypeVar
+# SEE: https://peps.python.org/pep-0673/
+THtmlTagHandler = TypeVar("THtmlTagHandler", bound="HtmlTagHandler")
+
+class HtmlTagHandler:
+    def __init__(self, start_regex: re.Pattern, end_regex: Optional[re.Pattern], add_line_in_warning: bool) -> None:
+        self.start_regex = start_regex
+        self.end_regex = end_regex
         # The line index may need to be disabled, if you run it aginst the HTML file
         self.add_line_in_warning = add_line_in_warning
         self.location = "Not yet initialized"
+        self.full_text_string = ""
+
+    def replace_function(self, old_value: str, parsed: ParsedHtmlTag) -> str:
+        raise Exception("You need to subclass HtmlTagHandler and overwrite the 'replace_function' method")
 
-    def process_string(self, file_name: str, html: str) -> str:
+    def process_string(self, file_name: str, file_contents: str) -> str:
+        self.full_text_string = file_contents
         search_start_pos = 0
-        while True:
-            match = INPUT_TAG_START.search(html, search_start_pos)
-            if match:
-                start = match.span()[0]
-                # Determine where we are (for useful error messages)
-                if self.add_line_in_warning:
-                    line_nr = html.count("\n", 0, start) + 1
-                    self.location = f"{file_name}:{line_nr}"
-                else:
-                    self.location = file_name
-
-                end_and_parsed = self.find_where_tag_ends(html, start)
-                if end_and_parsed:
-                    end, parsed = end_and_parsed
-                    old_value = html[start:end]
-
-
-                    # Give the replace_function the chance to replace the part of the string
-                    new_value = self.replace_function(self, old_value, parsed)
-                    if new_value != old_value:
-                        html = html[:start] + new_value + html[end:]
-
-                    # Continue searching after the end of the tag
-                    search_start_pos = start + len(new_value)
-                else:
-                    # we cound not find out where the tag ended, so we just make sure we do not encounter it again
-                    search_start_pos = start + 1
+
+        # replace / handle all matches
+        while match := self.start_regex.search(file_contents, search_start_pos):
+            file_contents, search_start_pos = self.handle_potential_occurence(file_name, file_contents, match)
+
+        return file_contents
+
+    def handle_potential_occurence(self, file_name: str, html: str, match: re.Match) -> tuple[str,int]:
+        start = match.span()[0]
+        # Determine where we are (for useful error messages)
+        if self.add_line_in_warning:
+            line_nr = html.count("\n", 0, start) + 1
+            self.location = f"{file_name}:{line_nr}"
+        else:
+            self.location = file_name
+
+        end_and_parsed = self.find_where_tag_ends(html, start)
+        if end_and_parsed:
+            end, parsed = end_and_parsed
+            old_value = html[start:end]
+
+            if self.end_regex and not self.end_regex.match(html[end:]):
+                # End pattern does not match, so we skip it
+                return (html, start + 1)
             else:
-                return html
+                # Only process it if no end pattern exist or if it matches
+                # Give the replace_function the chance to replace the part of the string
+                new_value = self.replace_function(old_value, parsed)
+                if new_value != old_value:
+                    html = html[:start] + new_value + html[end:]
 
+                # Continue searching after the end of the tag
+                return (html, start + len(new_value))
+        else:
+            # we cound not find out where the tag ended, so we just make sure we do not encounter it again
+            return (html, start + 1)
 
     def find_where_tag_ends(self, html: str, start: int) -> Optional[tuple[int,ParsedHtmlTag]]:
         search_pos = start
         # Limit to small number to prevent huge performance problems if this is buggy
         for _ in range(10):
             end = html.find(">", search_pos)
             if end == -1:
@@ -65,29 +79,30 @@
                     search_pos = end
 
         # If not successful after a couple attempts, print a warning
         warning(f"{self.location} - Could not find end of tag")
         return None
 
 
-def create_normal_input_class_handler(placeholders: dict, add_line_in_warning: bool) -> InputTagHandler:
-    def replace_function(handler, tag: str, parsed: ParsedHtmlTag) -> str:
+class NormalHtmlInputElementHandler(HtmlTagHandler):
+    def __init__(self, placeholders: dict, add_line_in_warning: bool) -> None:
+        super().__init__(re.compile("<input", re.IGNORECASE), None, add_line_in_warning)
+        self.placeholders = placeholders
+
+    def replace_function(self, tag: str, parsed: ParsedHtmlTag) -> str:
         """
         If the tag is an input tag, it's value will be replaced with a warning that tells the user to enable JavaScript.
         If JavaScript is enabled, it will replace the value with the stored/default value of the placeholder.
         """
         placeholder_name = parsed.attributes.get("data-input-for")
         if placeholder_name:
             attrs = dict(parsed.attributes)
             # Set a value that will be shown, when the script can not run (because JS is disabled)
             attrs["value"] = "Please enable JavaScript"
 
             # Print a warning if the placeholder does not exist
-            if placeholder_name not in placeholders:
-                warning(f"{handler.location} - Input element is linked to non-existent variable '{placeholder_name}'. Is this a typo or did you forget to set a default value for it?")
+            if placeholder_name not in self.placeholders:
+                warning(f"{self.location} - Input element is linked to non-existent variable '{placeholder_name}'. Is this a typo or did you forget to set a default value for it?")
 
             return create_html_opening_tag(parsed.tag, attrs)
         else:
             return tag
-
-    handler = InputTagHandler(replace_function, add_line_in_warning)
-    return handler
```

### Comparing `mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/placeholder_data.py` & `mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/config/placeholder.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,54 +1,38 @@
 from enum import Enum, auto
-import json
-import os
 import re
 from typing import NamedTuple, Any
-# pip packages
-from mkdocs.exceptions import PluginError
-import yaml
 # local
-from . import warning
-from .validators import Validator, ValidatorRule, assert_matches_one_validator
-from .validators_predefined import VALIDATOR_PRESETS
+from .. import warning, PlaceholderConfigError
+from .validator import Validator
+from ..validator_functions import assert_matches_one_validator
+from ..validators_predefined import VALIDATOR_PRESETS
+from .parser_utils import assert_no_unknown_fields, add_problematic_data_to_exceptions, get_bool, get_string
+
 
 # Should only contain letters, numbers, and underscores (hopefully prevents them from being broken up by syntax highlighting)
 # Should not begin with a number (this prevents placeholders like `1`)
 # Should not begin or end with a underscore (they are reserved for internal purposes like state tracking)
 VARIABLE_NAME_REGEX = re.compile("^[A-Z]([A-Z0-9_]*[A-Z0-9])?$")
+SAFE_NAME_REGEX = re.compile("^[A-Za-z0-9_]+$")
+JUST_UNDERSCORES = re.compile("^_+$")
 # The types to accept for fields, where a string is accepted
 TYPES_PRIMITIVE = [bool, float, int, str]
 # Only these fields are allowed in placeholders
 PLACEHOLDER_FIELD_NAMES = {
+    "allow_nested",
     "default",
     "default-function",
     "description",
     "read_only",
     "replace_everywhere",
     "values",
     "validators",
 }
 
-VALIDATOR_FIELD_NAMES = {
-    "name",
-    "rules",
-}
-
-VALIDATOR_RULE_FIELD_NAMES = {
-    "severity",
-    "regex",
-    "match_function",
-    "should_match",
-    "error_message",
-}
-
-SEVERITY_LIST = [
-    "error",
-    "warn",
-]
 
 class InputType(Enum):
     Field = auto()
     Checkbox = auto()
     Dropdown = auto()
 
 class Placeholder(NamedTuple):
@@ -62,261 +46,179 @@
     # A javascript snippet to generate the default value
     default_function: str
     # The description to show when generating the input table
     description: str
     # Whether the placeholder should be protected from users editing it.
     # Use true to have hidden convenience variables. Example "COMB_EMAIL: xCOMB_FIRST_NAMEx.xCOMB_SURNAMEx@xCOMB_DOMAINx"
     read_only: bool
+    # Whether to replace placeholders in this placeholder's value. By default off for text fields and on for everything else
+    allow_nested: bool
     # Whether to only replace visible text or to try to replace it anywhere in the DOM
     replace_everywhere: bool
     # For supporting advanced input fields such as dropdown menus and checkboxes
     values: dict[str,str]
     # The type is not specified directly by the user, but is instead determined from the `values` field.
     # It is stored here for internal use
     input_type: InputType
     # The input must conform to one of the validators. This allows mixed input such as "IPv4 address or IPv6 address or Hostname"
     validator_list: list[Validator]
 
 
-def load_placeholder_data(path: str) -> dict[str, Placeholder]:
-    """
-    Load placeholder data from a file and run some checks on the parsed contents
-    """
-    if os.path.exists(path):
-        with open(path, "rb") as f:
-            data = yaml.safe_load(f)
-
-        placeholders: dict[str,Placeholder] = {}
-
-        if type(data) != dict:
-            raise PluginError(f"[placeholder] Config file error: Expected root element of type 'dict', but got '{type(data).__name__}'")
-        for key, value in data.items():
-            # Make sure that values are strings (or convert them to strings if possible)
-            if isinstance(value, dict):
-                # New style entry with attributes
-                # debug(f"dict: {value}")
-                placeholders[key] = parse_placeholder_dict(key, value)
-            elif type(value) in TYPES_PRIMITIVE:
-                # Old config style, will only set name and default_value
-                # For consistency's sake, we also parse it wit the parse_palceholder_dict() function
-                # debug(f"primitive: {value}")
-                placeholders[key] = parse_placeholder_dict(key, {"default": value})
-            else:
-                raise PluginError(f"Expected a single value or object for key '{key}', but got type {type(value).__name__}")
+@add_problematic_data_to_exceptions
+def parse_placeholders(data: dict, location: str, validators: dict[str,Validator]) -> dict[str,Placeholder]:
+    placeholders: dict[str,Placeholder] = {}
+
+    if type(data) != dict:
+        raise PlaceholderConfigError(f"[placeholder] Config file error: Expected root element of type 'dict', but got '{type(data).__name__}'")
+    for key, value in data.items():
+        # Check that the variable name matches expected format
+        if not VARIABLE_NAME_REGEX.match(key):
+            warning(f"Potentially problematic variable name: '{key}'. A valid name should only contain capital letters, digits, and underscores and it should start with a letter")
+        
+        if JUST_UNDERSCORES.match(key):
+            raise PlaceholderConfigError("You can not have a placeholder name that is just underscores!")
+
+        if not SAFE_NAME_REGEX.match(key):
+            raise PlaceholderConfigError(f"The placeholder name '{key}' contains prohibited characters. Please only use letters, digits, and underscores")
+
+        # Make sure that values are strings (or convert them to strings if possible)
+        if isinstance(value, dict):
+            # New style entry with attributes
+            # debug(f"dict: {value}")
+            placeholders[key] = parse_placeholder_dict(value, f"{location}:{key}", key, validators)
+        elif type(value) in TYPES_PRIMITIVE:
+            # Old config style, will only set name and default_value
+            # For consistency's sake, we also parse it wit the parse_palceholder_dict() function
+            # debug(f"primitive: {value}")
+            placeholders[key] = parse_placeholder_dict({"default": value}, f"{location}:{key}", key, validators)
+        else:
+            raise PlaceholderConfigError(f"Expected a single value or object for key '{key}', but got type {type(value).__name__}")
 
-            # Check that the variable name matches expected format
-            if not VARIABLE_NAME_REGEX.match(key):
-                warning(f"Potentially problematic variable name: '{key}'. A valid name should only contain capital letters and underscores.")
 
-        return placeholders
-    else:
-        raise PluginError(f"Placeholder data file '{path}' does not exist")
+    return placeholders
 
 
-def parse_placeholder_dict(name: str, data: dict[str,Any]) -> Placeholder:
+@add_problematic_data_to_exceptions
+def parse_placeholder_dict(data: dict[str,Any], location: str, name: str, validators: dict[str,Validator]) -> Placeholder:
     """
     Parse a dictionary that contains the information for a single placeholder.
     """
-    try:
-        # Check for unexpected fields
-        unexpected_fields = set(data).difference(PLACEHOLDER_FIELD_NAMES)
-        if unexpected_fields:
-            raise PluginError(f"Unexpected field(s): {', '.join(unexpected_fields)}")
-
-        # Readonly is optional, defaults to False
-        read_only = data.get("read_only", False)
-        if type(read_only) != bool:
-            raise PluginError(f"Wrong type for key 'read_only': Expected 'bool', got '{type(read_only).__name__}'")
-
-        # Replace-everywhere is optional, defaults to False
-        replace_everywhere = data.get("replace_everywhere", False)
-        if type(replace_everywhere) != bool:
-            raise PluginError(f"Wrong type for key 'replace_everywhere': Expected 'bool', got '{type(replace_everywhere).__name__}'")
-
-        # Description is optional
-        description = str(data.get("description", ""))
-
-        values = parse_values(data)
-        default_value, default_function = parse_defaults(data, values)
-        input_type = determine_input_type(values, default_value)
-        validator_list = parse_validator_list(name, data, input_type, default_value)
-
-        return Placeholder(
-            name=name,
-            default_value=default_value,
-            default_function=default_function,
-            description=description,
-            replace_everywhere=replace_everywhere,
-            read_only=read_only,
-            values=values,
-            input_type=input_type,
-            validator_list=validator_list,
-        )
-    except Exception as ex:
-        message = f"Missing key {ex}" if type(ex) == KeyError else str(ex)
-        raise PluginError(f"Failed to parse placeholder '{name}': {message}\n\nCaused by placeholder {name}")
+    assert_no_unknown_fields(data, PLACEHOLDER_FIELD_NAMES)
+
+    read_only = get_bool(data, "read_only", False)
+    replace_everywhere = get_bool(data, "replace_everywhere", False)
+    description = get_string(data, "description", default="")
+
+    values = parse_values(data)
+    default_value, default_function = parse_defaults(data, values)
+    input_type = determine_input_type(values, default_value)
+
+    # Make sure to set the default_value to a falback if it is optional
+    if not default_value:
+        if input_type == InputType.Checkbox:
+            default_value = "unchecked"
+        elif input_type == InputType.Dropdown:
+            default_value = list(values.keys())[0]
+    validator_list = parse_validator_list(name, data, input_type, default_value, validators)
+
+    # By default only allow nested placeholders when the user can not specify custom values / when only predefined values have to be used
+    default_allow_nested = input_type == InputType.Checkbox or input_type == InputType.Dropdown or read_only
+    allow_nested = get_bool(data, "allow_nested", default_allow_nested)
+
+    return Placeholder(
+        allow_nested=allow_nested,
+        name=name,
+        default_value=default_value,
+        default_function=default_function,
+        description=description,
+        replace_everywhere=replace_everywhere,
+        read_only=read_only,
+        values=values,
+        input_type=input_type,
+        validator_list=validator_list,
+    )
 
 
 def parse_defaults(data: dict[str,Any], values: dict[str,str]) -> tuple[str, str]:
     # default (default_value) is required, unless values or default_function exists
-    default_function = str(data.get("default-function", ""))
+    default_function = get_string(data, "default-function", default="")
     try:
-        default_value = str(data["default"])
+        default_value = get_string(data, "default", allow_numeric=True)
         if default_function:
-            raise PluginError("Both 'default' and 'default-function' are defined")
+            raise PlaceholderConfigError("Both 'default' and 'default-function' are defined")
     except KeyError:
         default_value = ""
         if not default_function and not values:
-            raise PluginError("Missing key 'default' or 'default-function'")
+            raise PlaceholderConfigError("Missing key 'default' or 'default-function'")
     return default_value, default_function
 
 
 def parse_values(data: dict[str,Any]) -> dict[str,str]:
     # Values are optional
     values_original: dict = data.get("values", {})
     values: dict[str,str] = {}
     for key, value in values_original.items():
         if type(value) in TYPES_PRIMITIVE:
             values[str(key)] = str(value)
         else:
-            raise PluginError(f"Field 'values': Expected a dictionary with primitive values, but got {value} ({type(value).__name__}) in key {key}")
+            raise PlaceholderConfigError(f"Field 'values': Expected a dictionary with primitive values, but got {value} ({type(value).__name__}) in key {key}")
     return values
 
 
 def determine_input_type(values: dict[str,str], default_value: str) -> InputType:
     # Determine the type, and do some extra type dependent validation
     if values:
         if set(values.keys()) == {"checked", "unchecked"}:
             if default_value not in ["", "checked", "unchecked"]:
-                raise PluginError("Field 'default': Allowed values for check boxes are '' (empty string), 'checked', 'unchecked'")
+                raise PlaceholderConfigError("Field 'default': Allowed values for check boxes are '' (empty string), 'checked', 'unchecked'")
             return InputType.Checkbox
         else:
             if default_value != "" and default_value not in values.keys():
-                raise PluginError("Field 'default': Allowed values for a dropdown box are '' (empty string), or one of the keys defined in the 'values' field")
+                raise PlaceholderConfigError("Field 'default': Allowed values for a dropdown box are '' (empty string), or one of the keys defined in the 'values' field")
             return InputType.Dropdown
     else:
         return InputType.Field
 
 
-def parse_validator_list(placeholder_name: str, data: dict[str,Any], input_type: InputType, default_value: str) -> list[Validator]:
-    validator_list: list[Validator] = []
+def parse_validator_list(placeholder_name: str, data: dict[str,Any], input_type: InputType, default_value: str, known_validators: dict[str,Validator]) -> list[Validator]:
     # Validators only exist for textboxes:
     if input_type == InputType.Field:
         if "validators" in data:
             validators = data["validators"]
             if type(validators) == str:
-                validator_data_list = [validators]
+                validator_list = [validators]
             elif type(validators) == list:
-                validator_data_list = validators
+                validator_list = validators
             else:
-                raise PluginError(f"Field 'validators': Should be either a string or a list, but is type {type(validators).__name__}")
+                raise PlaceholderConfigError(f"Field 'validators': Should be either a string or a list, but is type {type(validators).__name__}")
 
-            for validator in validator_data_list:
+            # Check validator list entries
+            resolved_validators: list[Validator] = []
+            for validator in validator_list:
                 if type(validator) == str:
                     # This is a validator preset
-                    validation_preset = VALIDATOR_PRESETS.get(validator)
-                    if validation_preset:
-                        validator_list.append(validation_preset)
+                    validator_object = known_validators.get(validator)
+                    if validator_object:
+                        validator_object.mark_used()
+                        resolved_validators.append(validator_object)
                     else:
-                        raise PluginError(f"No validator preset named '{validator}', valid values are: {', '.join(VALIDATOR_PRESETS)}")
-                elif type(validator) == dict:
-                    validator_list.append(parse_validator_object(validator))
+                        raise PlaceholderConfigError(f"No validator preset named '{validator}', valid values are: {', '.join(VALIDATOR_PRESETS)}")
                 else:
-                    raise PluginError(f"Wrong type for validator entry: Expected 'string' or 'dict', got '{type(validator).__name__}'")
+                    raise PlaceholderConfigError(f"Wrong type for validator list entry: Expected 'string', got '{type(validator).__name__}'")
 
 
             if validator_list:
-                assert_matches_one_validator(validator_list, default_value)
+                assert_matches_one_validator(resolved_validators, default_value)
 
-                validator_names = [v.name for v in validator_list]
-                duplicate_names = [x for x in validator_names if validator_names.count(x) > 1]
+                duplicate_names = [x for x in validator_list if validator_list.count(x) > 1]
                 if duplicate_names:
                     pretty_names_list = ", ".join(sorted(set(duplicate_names)))
-                    warning(f"Placeholder {placeholder_name} has multiple validators with the same name(s). Are they redundant? Duplicate(s): {pretty_names_list}")
+                    warning(f"Placeholder {placeholder_name} has the same validator multiple times. Duplicate(s): {pretty_names_list}")
+
+            return resolved_validators
+        else:
+            return []
     else:
         if "validators" in data:
             warning(f"Placeholder {placeholder_name} has field 'validators', but is not a text field. Any validators for it will be ignored.")
 
-    return validator_list
-
-
-def parse_validator_object(data: dict[str,Any]) -> Validator:
-    try:
-        id = data["id"]
-        if type(id) != str:
-            raise PluginError(f"Wrong type for key 'name': Expected 'string', got '{type(id).__name__}'")
-
-        name = data["name"]
-        if type(name) != str:
-            raise PluginError(f"Wrong type for key 'name': Expected 'string', got '{type(name).__name__}'")
-
-        rules_data = data["rules"]
-        if type(rules_data) != list:
-            raise PluginError(f"Wrong type for key 'rules_data': Expected 'list', got '{type(rules_data).__name__}'")
-
-        if not rules_data:
-            raise PluginError("Validators neet to have at least a rule, but received an empty list")
-
-        rules = [parse_validator_rule(x) for x in rules_data]
-        return Validator(
-            id=id,
-            name=name,
-            rules=rules,
-        )
-    except Exception as ex:
-        message = f"Missing key {ex}" if type(ex) == KeyError else str(ex)
-        raise PluginError(f"{message}\n\nCaused by validator: {json.dumps(data, indent=4)}")
-
-
-def parse_validator_rule(data: dict[str,Any]) -> ValidatorRule:
-    try:
-        unexpected_fields = set(data).difference(VALIDATOR_RULE_FIELD_NAMES)
-        if unexpected_fields:
-            raise PluginError(f"Unexpected field(s) in validator rule: {', '.join(unexpected_fields)}")
-
-        severity = data.get("severity", "error")
-        if severity not in SEVERITY_LIST:
-            raise PluginError(f"Unknown severity '{severity}'. Should be one of {', '.join(unexpected_fields)}")
-
-        regex = ""
-        match_function = ""
-        if "regex" in data:
-            if "match_function" in data:
-                raise PluginError("Keys 'regex' and 'match_function' are mutually exclusive, but both are defined")
-            else:
-                regex = data["regex"]
-                if type(regex) != str:
-                    raise PluginError(f"Wrong type for key 'regex': Expected 'string', got '{type(regex).__name__}'")
-                elif not regex:
-                    raise PluginError("Key 'regex' can not be an empty string")
-        else:
-            if "match_function" in data:
-                match_function = data["match_function"]
-                if type(match_function) != str:
-                    raise PluginError(f"Wrong type for key 'match_function': Expected 'string', got '{type(match_function).__name__}'")
-                elif not match_function:
-                    raise PluginError("Key 'match_function' can not be an empty string")
-            else:
-                raise PluginError("Missing key: you need to specify either 'regex' or 'match_function'")
-
-
-        should_match = data["should_match"]
-        if type(should_match) != bool:
-            raise PluginError(f"Wrong type for key 'should_match': Expected 'bool', got '{type(should_match).__name__}'")
-
-        error_message = data.get("error_message")
-        if type(error_message) != str:
-            raise PluginError(f"Wrong type for key 'error_message': Expected 'string', got '{type(error_message).__name__}'")
-        if not error_message:
-            error_message = "Should match" if should_match else "Should not match"
-            error_message += f" the regular expression '{regex}'"
-
-        return ValidatorRule(
-            severity=severity,
-            regex_string=regex,
-            match_function=match_function,
-            should_match=should_match,
-            error_message=error_message,
-        )
-    except Exception as ex:
-        message = f"Missing key {ex}" if type(ex) == KeyError else str(ex)
-        raise PluginError(f"{message}\n\nCaused by validator rule: {json.dumps(data, indent=4)}")
+        return []
```

### Comparing `mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/plugin_config.py` & `mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/mkdocs/plugin_config.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,36 +4,15 @@
 # Moved to an extra file to prevent cyclic dependency errors
 class PlaceholderPluginConfig(Config):
     """
     The plugin config, that will be parsed from the settings supplied in `mkdocs.yaml`
     """
     # Can be used to disable the plugin
     enabled = Type(bool, default=True)
-    # Automatically add input tables to the top of each page with placeholders
-    auto_placeholder_tables = Type(bool, default=False)
-    # Use collapsible admonitions
-    auto_placeholder_tables_collapsible = Type(bool, default=True)
-    # Create placeholder tables dynamically (with JavaScript), instead of at build time
-    auto_placeholder_tables_javascript = Type(bool, default=False)
-    # Enable logging of debuggin information to the browser's console
-    debug_javascript = Type(bool, default=False)
-    # Show warnings if potential errors are found
-    show_warnings = Type(bool, default=True)
-    # Reload the page when a significant change (pressed Enter in textbox, change in checkbox or dropdown)
-    reload_on_change = Type(bool, default=True)
-    # Add the "Apply the new values by clicking on this text" to placeholder input tables
-    add_apply_table_column = Type(bool, default=False)
-    # files to perform static replacements for:
-    static_pages = Type(list, default=[])
-    # The file where you define the placeholders
-    placeholder_file = Type(str, default="placeholder-plugin.yaml")
     # Output loaction for the custom JS file. This overwrites the javascript code provided by the plugin
-    placeholder_js = Type(str, default="assets/javascripts/placeholder-plugin.js")
-    # Provide additional javascript for example for hooks, providing functions, etc
-    placeholder_extra_js = Type(str, default="")
-    # Replace delay millis
-    replace_delay_millis = Type(int, default=0)
+    js_output_dir = Type(str, default="assets/javascripts/")
     # CSS file. If it exists, the contents will be appended to. add empty string to not include the default styles
     placeholder_css = Type(str, default="assets/javascripts/placeholder-plugin.css")
-    # Default values for place4holder input tables
-    table_default_show_readonly = Type(bool, default=False)
-    table_default_type = Type(str, default="simple")
+    # Provide additional javascript for example for hooks, providing functions, etc
+    placeholder_extra_js = Type(str, default="")
+    # The file where you define the placeholders
+    placeholder_file = Type(str, default="placeholder-plugin.yaml")
```

### Comparing `mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/validators.py` & `mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/validator_functions.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,13 @@
 from typing import NamedTuple
-from mkdocs.exceptions import PluginError
 import re
 # local
-from . import warning
+from . import warning, PlaceholderConfigError
+from .config import Validator, ValidatorRule
 
-class ValidatorRule(NamedTuple):
-    severity: str # warn or error
-    # you need to either specify regex_string or match_function
-    regex_string: str
-    match_function: str
-    should_match: bool
-    error_message: str
 
 def should_match(regex_string: str, error_message: str) -> ValidatorRule:
     return ValidatorRule(
         severity="warn",
         regex_string=regex_string,
         match_function="",
         should_match=True,
@@ -45,49 +38,14 @@
         regex_string=regex_string,
         match_function="",
         should_match=False,
         error_message=error_message,
     )
 
 
-class Validator(NamedTuple):
-    id: str
-    name: str
-    rules: list[ValidatorRule]
-
-
-def validator_to_dict(v: Validator) -> dict:
-    try:
-        return {
-            "id": v.id,
-            "display_name": v.name,
-            "rules": [validator_rule_to_dict(r) for r in v.rules],
-        }
-    except Exception as ex:
-        raise PluginError(f"Error while converting validator '{v.name}' to dictionary: {ex}")
-
-def validator_rule_to_dict(r: ValidatorRule) -> dict:
-    data = {
-        "severity": r.severity,
-        "should_match": r.should_match,
-        "error_message": r.error_message,
-    }
-    if r.match_function:
-        if r.regex_string:
-            raise PluginError(f"Error in rule: 'match_function' ({r.match_function}) and 'regex_string' ({r.regex_string}) are mutually exclusive, but both are defined")
-        else:
-            data["match_function"] = r.match_function
-    else:
-        if r.regex_string:
-            data["regex"] = r.regex_string
-        else:
-            raise PluginError("Error in rule: You need to either specify 'match_function' or 'regex_string', but both are empty")
-
-    return data
-
 class ValidationResults(NamedTuple):
     validator_name: str
     value: str
     warnings: list[str]
     errors: list[str]
 
 
@@ -115,35 +73,35 @@
     else:
         # Show all warnings and errors and raise an exception
         for result in results:
             for msg in result.errors:
                 warning(f"[Validation error] '{value}' is no {result.validator_name}: {msg}")
             for msg in result.warnings:
                 warning(f"[Validation warning] '{value}' is no {result.validator_name}: {msg}")
-        raise PluginError(f"Default value '{value}' failed validation")
+        raise PlaceholderConfigError(f"Default value '{value}' failed validation")
 
 
 def check_if_matches_validator(validator: Validator, default_value: str) -> ValidationResults:
     warnings = []
     errors = []
     for rule in validator.rules:
         if rule.regex_string:
             try:
                 matches = bool(re.search(rule.regex_string, default_value))
             except Exception as ex:
-                raise PluginError(f"Error in regular expression '{rule.regex_string}': {ex}")
+                raise PlaceholderConfigError(f"Error in regular expression '{rule.regex_string}': {ex}")
 
             if matches != rule.should_match:
                 # This rule fails
                 if rule.severity == "error":
                     errors.append(rule.error_message)
                 elif rule.severity == "warn":
                     warnings.append(rule.error_message)
                 else:
-                    raise PluginError(f"Unexpected severity: '{rule.severity}'")
+                    raise PlaceholderConfigError(f"Unexpected severity: '{rule.severity}'")
         else:
             # We can not really check the custom JavaScript function at build time.
             # Do we just assume that everything is ok.
             pass
 
     return ValidationResults(
         validator_name=validator.name,
```

### Comparing `mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin/validators_predefined.py` & `mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin/generic/validators_predefined.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # local
-from .validators import Validator, must_match, must_not_match, should_match, should_not_match
+from .config import Validator
+from .validator_functions import must_match, must_not_match, should_match, should_not_match
 
 IPV4_SEGMENT = "(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)"
 IPV4_ADDRESS = f"{IPV4_SEGMENT}(?:\\.{IPV4_SEGMENT}){{3}}"
 CIDR_SUFFIX = "/(3[0-2]|[12]?[0-9])"
 URL_REGEX = r"[a-zA-Z0-9-]+://(?:[a-zA-Z]|[0-9]|[$-_@.&+]|[!*\(\),]|(?:%[0-9a-fA-F][0-9a-fA-F]))+(#\S*)?"
 RULE_URL_NO_WHITESPACE = must_not_match(r"\s", "URLs may not contain whitespace. Please URL encode it. For example a space should be replaced with '%20'")
 RULE_NOT_EMPTY = must_match("^.+$", "Can not be empty")
@@ -13,169 +14,169 @@
 # Source: https://ihateregex.io/expr/ipv6/
 # Not great, does not match that well
 MEDIOCRE_IPV6_REGEX = r"(([0-9a-fA-F]{1,4}:){7,7}[0-9a-fA-F]{1,4}|([0-9a-fA-F]{1,4}:){1,7}:|([0-9a-fA-F]{1,4}:){1,6}:[0-9a-fA-F]{1,4}|([0-9a-fA-F]{1,4}:){1,5}(:[0-9a-fA-F]{1,4}){1,2}|([0-9a-fA-F]{1,4}:){1,4}(:[0-9a-fA-F]{1,4}){1,3}|([0-9a-fA-F]{1,4}:){1,3}(:[0-9a-fA-F]{1,4}){1,4}|([0-9a-fA-F]{1,4}:){1,2}(:[0-9a-fA-F]{1,4}){1,5}|[0-9a-fA-F]{1,4}:((:[0-9a-fA-F]{1,4}){1,6})|:((:[0-9a-fA-F]{1,4}){1,7}|:)|fe80:(:[0-9a-fA-F]{0,4}){0,4}%[0-9a-zA-Z]{1,}|::(ffff(:0{1,4}){0,1}:){0,1}((25[0-5]|(2[0-4]|1{0,1}[0-9]){0,1}[0-9])\.){3,3}(25[0-5]|(2[0-4]|1{0,1}[0-9]){0,1}[0-9])|([0-9a-fA-F]{1,4}:){1,4}:((25[0-5]|(2[0-4]|1{0,1}[0-9]){0,1}[0-9])\.){3,3}(25[0-5]|(2[0-4]|1{0,1}[0-9]){0,1}[0-9]))"
 
 def generate_url_http_validator() -> Validator:
     # source: https://urlregex.com. Modified to handle the fragment part (what comes after #)
     return Validator(
-        id="url_http",
-        name="URL (HTTP / HTTPS)",
-        rules=[
+        "url_http",
+        "URL (HTTP / HTTPS)",
+        [
             must_match("^https?://", "Needs to start with 'http://' or 'https://'"),
             RULE_URL_NO_WHITESPACE,
             should_match(f"^{URL_REGEX}$", "Expected an value like https://example.com/some/page.php?x=1&y=some%20value"),
         ]
     )
 
 def generate_file_name_linux_validator() -> Validator:
     return Validator(
-        id="file_name_linux",
-        name="File name",
-        rules=[
+        "file_name_linux",
+        "File name",
+        [
             RULE_NOT_EMPTY,
             must_not_match("/", "Can not contain path separators (slash)"),
             RULE_WARN_WHITESPACE,
         ]
     )
 
 def generate_file_name_windows_validator() -> Validator:
     return Validator(
-        id="file_name_windows",
-        name="File name",
-        rules=[
+        "file_name_windows",
+        "File name",
+        [
             RULE_NOT_EMPTY,
             must_not_match(r"[/\\]", "Can not contain path separators (slash or backslash)"),
             must_not_match('[<>:"|?*]', 'Can not contain prohibited characters: \'<>:"|?*\''),
             RULE_WARN_WHITESPACE,
         ]
     )
 
 
 def generate_path_linux_validator() -> Validator:
     return Validator(
-        id="path_linux",
-        name="File path (Linux)",
-        rules=[
+        "path_linux",
+        "File path (Linux)",
+        [
             RULE_NOT_EMPTY,
             RULE_WARN_WHITESPACE,
         ]
     )
 
 def generate_path_windows_validator() -> Validator:
     return Validator(
-        id="path_windows",
-        name="File path (Windows)",
-        rules=[
+        "path_windows",
+        "File path (Windows)",
+        [
             RULE_NOT_EMPTY,
             # Colon may be in 'C:\...' (and maybe for a port number in an UNC path?)
             should_not_match('[<>"|?*]', 'Can not contain prohibited characters: \'<>"|?*\''),
             RULE_WARN_WHITESPACE,
         ]
     )
 
 
 def generate_url_validator() -> Validator:
     # source: https://urlregex.com. Modified to handle the fragment part (what comes after #)
     return Validator(
-        id="url_any",
-        name="URL (any protocol)",
-        rules=[
+        "url_any",
+        "URL (any protocol)",
+        [
             RULE_URL_NO_WHITESPACE,
             should_match(f"^{URL_REGEX}$", "Expected an value like smb://example.com:10445/share/some-file.txt"),
         ]
     )
 
 def generate_ipv6_validator() -> Validator:
     return Validator(
-        id="ipv6_address",
-        name="IPv6 address",
-        rules=[
+        "ipv6_address",
+        "IPv6 address",
+        [
             must_match("^[0-9a-fA-F:.\\[\\]]+$", "Only numbers, the letters A-F, colons, dots, and square brackets are allowed"),
             should_match(f"^{MEDIOCRE_IPV6_REGEX}$", "Should probably look like '2001:0db8:85a3:0000:0000:8a2e:0370:7334' or '::1'"),
             should_not_match(f"^{IPV4_ADDRESS}$", "Should not be an IPv4 address. If you want a IPv4-mapped IPv6 address, prefix it with '::FFFF:' like this: '::FFFF:123.4.56.78'"),
 
         ]
     )
 
 
 def generate_ipv4_validator() -> Validator:
     return Validator(
-        id="ipv4_address",
-        name="IPv4 address",
-        rules=[
+        "ipv4_address",
+        "IPv4 address",
+        [
             must_match("^[0-9.]+$", "Only numbers and dots are allowed"),
             # There are other ways of specifying IP addresses, that not all software understands. For example: 2130706433, 017700000001, and 127.1 are alternative representations of 127.0.0.1
             # So we just filter for expected characters, but not for the pattern
             should_match(f"^{IPV4_ADDRESS}$", "Expected an value like 123.4.56.78"),
         ]
     )
 
 def generate_ipv4_range_cidr_validator() -> Validator:
     return Validator(
-        id="ipv4_range_cidr",
-        name="IPv4 adress range (CIDR notation)",
-        rules=[
+        "ipv4_range_cidr",
+        "IPv4 adress range (CIDR notation)",
+        [
             must_match("^[0-9./]+$", "Only numbers, dots and a slash are allowed"),
             must_not_match("/.*/", "May only contain one slash"),
             must_match(f"{CIDR_SUFFIX}$", "The number after that slash needs to be between 0 and 32 (inclusive)"),
             # There are other ways of specifying IP addresses, that not all software understands. For example: 2130706433, 017700000001, and 127.1 are alternative representations of 127.0.0.1
             # So we just filter for expected characters, but not for the pattern
             should_match(f"^{IPV4_ADDRESS}/[0-9]+$", "Expected an value like 123.4.56.0/24"),
         ]
     )
 
 
 def generate_ipv4_range_dash_validator() -> Validator:
     IPV4_SEGMENT_DASH = f"{IPV4_SEGMENT}(-{IPV4_SEGMENT})?"
     IPV4_ADDRESS_DASHES = f"{IPV4_SEGMENT_DASH}(?:\\.{IPV4_SEGMENT_DASH}){{3}}"
     return Validator(
-        id="ipv4_range_dashes",
-        name="IPv4 adress range (dash)",
-        rules=[
+        "ipv4_range_dashes",
+        "IPv4 adress range (dash)",
+        [
             must_match("^[0-9-.]+$", "Only numbers, dots and minuses are allowed"),
             must_not_match("(-\.|\.-)", "Number should be on both sites of the dash"),
             must_not_match("--", "Consecutive dashes are not allowed"),
             # There are other ways of specifying IP addresses, that not all software understands. For example: 2130706433, 017700000001, and 127.1 are alternative representations of 127.0.0.1
             # So we just filter for expected characters, but not for the pattern
             should_match(f"^{IPV4_ADDRESS_DASHES}$", "Expected an value like 123.4-5.56.78-90"),
         ]
     )
 
 
 def generate_port_validator() -> Validator:
     port_regex="^((6553[0-5])|(655[0-2][0-9])|(65[0-4][0-9]{2})|(6[0-4][0-9]{3})|([1-5][0-9]{4})|([0-5]{0,5})|([0-9]{1,4}))$"
     return Validator(
-        id="port_number",
-        name="TCP/UDP port",
-        rules=[
+        "port_number",
+        "TCP/UDP port",
+        [
             must_match("^[0-9]+$", "Only numbers are allowed"),
             should_match(port_regex, "Expected an number between 0 and 65535 (inclusive)"),
         ]
     )
 
 RULE_DOMAIN_CHARS = must_match("^[a-zA-Z0-9-.]+$", "Only letters, numbers, dashes (minus signs), and dots are allowed")
 RULE_DOMAIN_START = must_match("^[^.-]", "Can not begin with a dot or dash (minus sign)")
 RULE_DOMAIN_END = must_match("[^.-]$", "Can not end with a dot or dash (minus sign)")
 RULE_DOMAIN_LENGTH = should_not_match("[a-zA-Z0-9-]{64}", "Subdomains should not be longer than 63 characters")
 
 def generate_domain_name_validator() -> Validator:
     return Validator(
-        id="domain",
-        name="Domain name",
-        rules=[
+        "domain",
+        "Domain name",
+        [
             RULE_DOMAIN_CHARS, RULE_DOMAIN_START, RULE_DOMAIN_END, RULE_DOMAIN_LENGTH,
             should_match("\\.", "Should contain multiple elements (for example domain.com or my.domain.com)"),
         ]
     )
 
 def generate_hostname_validator() -> Validator:
     return Validator(
-        id="hostname",
-        name="Hostname",
-        rules=[
+        "hostname",
+        "Hostname",
+        [
             RULE_DOMAIN_CHARS, RULE_DOMAIN_START, RULE_DOMAIN_END, RULE_DOMAIN_LENGTH
         ]
     )
 
 
 VALIDATOR_PRESETS = {
     "domain": generate_domain_name_validator(),
```

### Comparing `mkdocs-placeholder-plugin-0.3.1/src/mkdocs_placeholder_plugin.egg-info/PKG-INFO` & `mkdocs-placeholder-plugin-0.4.0/src/mkdocs_placeholder_plugin.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-placeholder-plugin
-Version: 0.3.1
+Version: 0.4.0
 Summary: Add dynamic placeholders to your mkdocs page
 Home-page: https://github.com/six-two/mkdocs-placeholder-plugin
 Author: six-two
 Author-email: pip@six-two.dev
 License: MIT License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
@@ -29,45 +29,74 @@
 
 This README is just a short intro to the package.
 For a quick start and detailed information please see the [documentation for the last release](https://mkdocs-placeholder-plugin.six-two.dev/).
 The documentation is also available in the `docs` folder of the source code and can be built localy with [MkDocs](https://www.mkdocs.org/).
 
 ## Development version
 
-If you want to use the latest development version (may be broken/buggy from time to time), you can install it with:
-```bash
-python3 -m pip install git+https://github.com/six-two/mkdocs-placeholder-plugin
-```
+If you want to use the latest development version (may be broken/buggy from time to time), you can install it by:
+
+1. Cloning the repository:
+    ```bash
+    git clone https://github.com/six-two/mkdocs-placeholder-plugin
+    cd mkdocs-placeholder-plugin
+    ```
+2. Building/Downloading the JavaScript files.
+    Choose any of the following ways:
+    
+    - Build it with npm (natively), by running the `./build-docs.sh` script.
+    - Build it in a (docker/podman) container by using the `Doeckerfile` in the `typescript` directory:
+        ```bash
+        cd typescript
+        podman build --tag placeholder-npm .
+        cd ..
+        ```
+
+        And then running the `./build.sh` script.
+        Once you see mkdocs running, you can terminate it with `Ctrl-C`.
+    - Downloading the files from the development version of the documentation (hosted and built by Vercel):
+        ```bash
+        curl https://dev.mkdocs-placeholder-plugin.six-two.dev/assets/javascripts/placeholder.min.js -o src/mkdocs_placeholder_plugin/assets/placeholder.min.js
+        curl https://dev.mkdocs-placeholder-plugin.six-two.dev/assets/javascripts/placeholder.min.js.map -o src/mkdocs_placeholder_plugin/assets/placeholder.min.js.map
+        ```
+3. Installing the package with pip:
+    ```bash
+    python3 -m pip install .
+    ```
 
 The corresponding documentation is hosted at <https://dev.mkdocs-placeholder-plugin.six-two.dev>.
 
 ## Notable changes
 
-### TODOs
-
-- Rewrite python code and decouple it from MkDocs (to be able to use it with other projects).
-- Implement propper exception handling for TypeScript code to recover from / compartmentalize non-critical errors.
-- Update the documentation.
-
 ### HEAD
 
+- Configuration format changed:
+    - Validators are no longer defined in-line and instead defined in a `validators` section -> easier to reuse custom validators.
+    - Placeholders now need to be specified in a `placeholders` section.
+    - Most settings are now in the configuration file instead of in your `mkdocs.yml`.
+- Some actions can now be toggled by visitors of the site. The settings open when you click the gear icon on a (dynamic) placeholder input table.
+- (By default) values are saved when the focus leaves a text field.
+- Removed static placeholder input tables (`<placeholdertable>`).
+- Uncoupled the code from MkDocs.
+    You should now be able to relatively easy port the project to other Markdown based static site generators if you want to.
+
 ### Version 0.3.1
 
 - Removed `Apply all changes` buttons. See [issue #3](https://github.com/six-two/mkdocs-placeholder-plugin/issues/3)
 
 ### Version 0.3.0
 
 This release may be a bit buggy due to the rewrite and the documentation is not entirely accurate yet.
 I will update the docs after I also clean up / rewrite the python code (planed for v0.4.0).
 
 - Rewrote the JavaScript code in TypeScript:
     - Packed and minified using Webpack, so the file is a bit smaller
     - Should find stupid errors I make in code paths that I do not test (often)
     - Sophisticated update logic: Instead of always reloading the page it tries to update the DOM in-place (if possible), which should improve user experience a bit and is much faster
-    - Recursive placeholders (placeholders that contain placeholders that contain placeholder...) no longer need to be specified in a speific order in the configuration file.
+    - Nested placeholders (placeholders that contain placeholders that contain placeholder...) no longer need to be specified in a speific order in the configuration file.
     - A placeholder's `default-function` and a validator rule's `match_function` are now evaluated using [`new Function(...)`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function) instead of `eval(...)`, so you need to add a return statement.
 
 ### Version 0.2.5
 
 - When an JavaScript generated `auto-input-table` is empty, now a info box is shown (instead of nothing / an empty table).
 - Bugfixes:
     - `auto_placeholder_tables_javascript` had no effect.
@@ -155,7 +184,42 @@
     git tag 0.X.Y
     ```
 7. Update the `latest-release` branch, so that the documentation website gets updated:
     ```
     git branch --force latest-release HEAD
     git push --tags origin latest-release
     ```
+
+### Updating python dependencies
+
+If you don't have them, install `pip-tools`:
+```bash
+python3 -m pip install pip-tools
+```
+
+Then update `requirements.txt`:
+```bash
+pip-compile -U
+```
+
+### Updating npm dependencies
+
+These are only used for the build process, so keeping them up to date is not that critical.
+
+Start a container with nodeJS:
+```bash
+podman run -it --rm -v "$(pwd)/typescript:/mnt" node:latest bash
+```
+
+In the container run the following commands to update the `typescript/package*.json` files on the host:
+```bash
+cd /mnt
+npm i -g npm-check-updates
+ncu -u
+npm i --package-lock-only
+```
+
+Then rebuild the docker image on the host:
+```bash
+cd typescript/
+podman build --tag placeholder-npm .
+```
```

