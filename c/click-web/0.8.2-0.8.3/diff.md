# Comparing `tmp/click-web-0.8.2.tar.gz` & `tmp/click-web-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "click-web-0.8.2.tar", last modified: Sat May 20 19:20:54 2023, max compression
+gzip compressed data, was "click-web-0.8.3.tar", last modified: Sat May 20 20:15:01 2023, max compression
```

## Comparing `click-web-0.8.2.tar` & `click-web-0.8.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:20:54.894085 click-web-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-20 19:20:45.000000 click-web-0.8.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-20 19:20:45.000000 click-web-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-20 19:20:45.000000 click-web-0.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-05-20 19:20:54.894085 click-web-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-20 19:20:45.000000 click-web-0.8.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:20:54.890085 click-web-0.8.2/click_web/
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-05-20 19:20:45.000000 click-web-0.8.2/click_web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-20 19:20:45.000000 click-web-0.8.2/click_web/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:20:54.890085 click-web-0.8.2/click_web/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 19:20:45.000000 click-web-0.8.2/click_web/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16916 2023-05-20 19:20:45.000000 click-web-0.8.2/click_web/resources/cmd_exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-05-20 19:20:45.000000 click-web-0.8.2/click_web/resources/cmd_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-20 19:20:45.000000 click-web-0.8.2/click_web/resources/index.py
--rw-r--r--   0 runner    (1001) docker     (123)    10237 2023-05-20 19:20:45.000000 click-web-0.8.2/click_web/resources/input_fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:20:54.890085 click-web-0.8.2/click_web/static/
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-05-20 19:20:45.000000 click-web-0.8.2/click_web/static/click_web.css
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-20 19:20:45.000000 click-web-0.8.2/click_web/static/copy_to_clipboard.js
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-20 19:20:45.000000 click-web-0.8.2/click_web/static/open_form.js
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-20 19:20:45.000000 click-web-0.8.2/click_web/static/panes.css
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-20 19:20:45.000000 click-web-0.8.2/click_web/static/panes.js
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-05-20 19:20:45.000000 click-web-0.8.2/click_web/static/post_and_read.js
--rw-r--r--   0 runner    (1001) docker     (123)    28846 2023-05-20 19:20:45.000000 click-web-0.8.2/click_web/static/pure.css
--rw-r--r--   0 runner    (1001) docker     (123)    29958 2023-05-20 19:20:45.000000 click-web-0.8.2/click_web/static/split.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:20:54.894085 click-web-0.8.2/click_web/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-20 19:20:45.000000 click-web-0.8.2/click_web/templates/command_form.html.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-05-20 19:20:45.000000 click-web-0.8.2/click_web/templates/form_macros.html.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-20 19:20:45.000000 click-web-0.8.2/click_web/templates/show_tree.html.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-20 19:20:45.000000 click-web-0.8.2/click_web/web_click_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:20:54.890085 click-web-0.8.2/click_web.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-05-20 19:20:54.000000 click-web-0.8.2/click_web.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-20 19:20:54.000000 click-web-0.8.2/click_web.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 19:20:54.000000 click-web-0.8.2/click_web.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 19:20:54.000000 click-web-0.8.2/click_web.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-20 19:20:54.000000 click-web-0.8.2/click_web.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-20 19:20:54.000000 click-web-0.8.2/click_web.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-20 19:20:54.894085 click-web-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-20 19:20:45.000000 click-web-0.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:20:54.894085 click-web-0.8.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 19:20:45.000000 click-web-0.8.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-20 19:20:45.000000 click-web-0.8.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:20:54.894085 click-web-0.8.2/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 19:20:45.000000 click-web-0.8.2/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-20 19:20:45.000000 click-web-0.8.2/tests/fixtures/click_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-20 19:20:45.000000 click-web-0.8.2/tests/fixtures/flask_fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:20:54.894085 click-web-0.8.2/tests/fixtures/script/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 19:20:45.000000 click-web-0.8.2/tests/fixtures/script/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-05-20 19:20:45.000000 click-web-0.8.2/tests/fixtures/script/a_script.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-20 19:20:45.000000 click-web-0.8.2/tests/fixtures/script/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-05-20 19:20:45.000000 click-web-0.8.2/tests/test_click_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-05-20 19:20:45.000000 click-web-0.8.2/tests/test_flask_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-05-20 19:20:45.000000 click-web-0.8.2/tests/test_flask_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-20 19:20:45.000000 click-web-0.8.2/tests/test_request_parsing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:15:01.048490 click-web-0.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-20 20:14:47.000000 click-web-0.8.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-20 20:14:47.000000 click-web-0.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-20 20:14:47.000000 click-web-0.8.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-05-20 20:15:01.048490 click-web-0.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-20 20:14:47.000000 click-web-0.8.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:15:01.040489 click-web-0.8.3/click_web/
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-05-20 20:14:47.000000 click-web-0.8.3/click_web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-20 20:14:47.000000 click-web-0.8.3/click_web/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:15:01.044489 click-web-0.8.3/click_web/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 20:14:47.000000 click-web-0.8.3/click_web/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16916 2023-05-20 20:14:47.000000 click-web-0.8.3/click_web/resources/cmd_exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-05-20 20:14:47.000000 click-web-0.8.3/click_web/resources/cmd_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-20 20:14:47.000000 click-web-0.8.3/click_web/resources/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10237 2023-05-20 20:14:47.000000 click-web-0.8.3/click_web/resources/input_fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:15:01.044489 click-web-0.8.3/click_web/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-05-20 20:14:47.000000 click-web-0.8.3/click_web/static/click_web.css
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-20 20:14:47.000000 click-web-0.8.3/click_web/static/copy_to_clipboard.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-20 20:14:47.000000 click-web-0.8.3/click_web/static/open_form.js
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-20 20:14:47.000000 click-web-0.8.3/click_web/static/panes.css
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-20 20:14:47.000000 click-web-0.8.3/click_web/static/panes.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-05-20 20:14:47.000000 click-web-0.8.3/click_web/static/post_and_read.js
+-rw-r--r--   0 runner    (1001) docker     (123)    28846 2023-05-20 20:14:47.000000 click-web-0.8.3/click_web/static/pure.css
+-rw-r--r--   0 runner    (1001) docker     (123)    29958 2023-05-20 20:14:47.000000 click-web-0.8.3/click_web/static/split.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:15:01.044489 click-web-0.8.3/click_web/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-20 20:14:47.000000 click-web-0.8.3/click_web/templates/command_form.html.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-05-20 20:14:47.000000 click-web-0.8.3/click_web/templates/form_macros.html.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-20 20:14:47.000000 click-web-0.8.3/click_web/templates/show_tree.html.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-20 20:14:47.000000 click-web-0.8.3/click_web/web_click_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:15:01.044489 click-web-0.8.3/click_web.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-05-20 20:15:00.000000 click-web-0.8.3/click_web.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-20 20:15:01.000000 click-web-0.8.3/click_web.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 20:15:00.000000 click-web-0.8.3/click_web.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 20:15:00.000000 click-web-0.8.3/click_web.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-20 20:15:00.000000 click-web-0.8.3/click_web.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-20 20:15:00.000000 click-web-0.8.3/click_web.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-20 20:15:01.048490 click-web-0.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-20 20:14:47.000000 click-web-0.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:15:01.044489 click-web-0.8.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 20:14:47.000000 click-web-0.8.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-20 20:14:47.000000 click-web-0.8.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:15:01.044489 click-web-0.8.3/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 20:14:47.000000 click-web-0.8.3/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-20 20:14:47.000000 click-web-0.8.3/tests/fixtures/click_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-20 20:14:47.000000 click-web-0.8.3/tests/fixtures/flask_fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:15:01.044489 click-web-0.8.3/tests/fixtures/script/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 20:14:47.000000 click-web-0.8.3/tests/fixtures/script/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-05-20 20:14:47.000000 click-web-0.8.3/tests/fixtures/script/a_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-20 20:14:47.000000 click-web-0.8.3/tests/fixtures/script/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-05-20 20:14:47.000000 click-web-0.8.3/tests/test_click_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-05-20 20:14:47.000000 click-web-0.8.3/tests/test_flask_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-05-20 20:14:47.000000 click-web-0.8.3/tests/test_flask_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-20 20:14:47.000000 click-web-0.8.3/tests/test_request_parsing.py
```

### Comparing `click-web-0.8.2/LICENSE` & `click-web-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `click-web-0.8.2/PKG-INFO` & `click-web-0.8.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: click-web
-Version: 0.8.2
+Version: 0.8.3
 Summary: Serve click scripts over the web with minimal effort.
 Home-page: https://github.com/fredrik-corneliusson/click-web
 Author: Fredrik Corneliusson
 Author-email: fredrik.corneliusson@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `click-web-0.8.2/README.rst` & `click-web-0.8.3/README.rst`

 * *Files identical despite different names*

### Comparing `click-web-0.8.2/click_web/__init__.py` & `click-web-0.8.3/click_web/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,16 @@
 
     """
     global _flask_app, logger
     assert _flask_app is None, "Flask App already created."
 
     _register(module, command)
 
-    _flask_app = Flask(__name__)
+    _flask_app = Flask(__name__, static_url_path=root.rstrip('/') + '/static')
+
     _flask_app.config['APPLICATION_ROOT'] = root
     root = root.rstrip('/')
 
     # add the "do" extension needed by our jinja templates
     _flask_app.jinja_env.add_extension('jinja2.ext.do')
 
     _flask_app.add_url_rule(root + '/', 'index', click_web.resources.index.index)
```

### Comparing `click-web-0.8.2/click_web/resources/cmd_exec.py` & `click-web-0.8.3/click_web/resources/cmd_exec.py`

 * *Files identical despite different names*

### Comparing `click-web-0.8.2/click_web/resources/cmd_form.py` & `click-web-0.8.3/click_web/resources/cmd_form.py`

 * *Files identical despite different names*

### Comparing `click-web-0.8.2/click_web/resources/index.py` & `click-web-0.8.3/click_web/resources/index.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 def index():
     with click.Context(click_web.click_root_cmd, info_name=click_web.click_root_cmd.name, parent=None) as ctx:
         return render_template('show_tree.html.j2', ctx=ctx, tree=_click_to_tree(ctx, click_web.click_root_cmd))
 
 
-def _click_to_tree(ctx: click.Context, node: Union[click.Command, click.MultiCommand], ancestors: list=None):
+def _click_to_tree(ctx: click.Context, node: Union[click.Command, click.MultiCommand], ancestors: list = None):
     """
     Convert a click root command to a tree of dicts and lists
     :return: a json like tree
     """
     if ancestors is None:
         ancestors = []
     res_childs = []
```

### Comparing `click-web-0.8.2/click_web/resources/input_fields.py` & `click-web-0.8.3/click_web/resources/input_fields.py`

 * *Files identical despite different names*

### Comparing `click-web-0.8.2/click_web/static/click_web.css` & `click-web-0.8.3/click_web/static/click_web.css`

 * *Files identical despite different names*

### Comparing `click-web-0.8.2/click_web/static/open_form.js` & `click-web-0.8.3/click_web/static/open_form.js`

 * *Files identical despite different names*

### Comparing `click-web-0.8.2/click_web/static/panes.css` & `click-web-0.8.3/click_web/static/panes.css`

 * *Files identical despite different names*

### Comparing `click-web-0.8.2/click_web/static/post_and_read.js` & `click-web-0.8.3/click_web/static/post_and_read.js`

 * *Files identical despite different names*

### Comparing `click-web-0.8.2/click_web/static/pure.css` & `click-web-0.8.3/click_web/static/pure.css`

 * *Files identical despite different names*

### Comparing `click-web-0.8.2/click_web/static/split.js` & `click-web-0.8.3/click_web/static/split.js`

 * *Files identical despite different names*

### Comparing `click-web-0.8.2/click_web/templates/command_form.html.j2` & `click-web-0.8.3/click_web/templates/command_form.html.j2`

 * *Files identical despite different names*

### Comparing `click-web-0.8.2/click_web/templates/form_macros.html.j2` & `click-web-0.8.3/click_web/templates/form_macros.html.j2`

 * *Files identical despite different names*

### Comparing `click-web-0.8.2/click_web/templates/show_tree.html.j2` & `click-web-0.8.3/click_web/templates/show_tree.html.j2`

 * *Files identical despite different names*

### Comparing `click-web-0.8.2/click_web/web_click_types.py` & `click-web-0.8.3/click_web/web_click_types.py`

 * *Files identical despite different names*

### Comparing `click-web-0.8.2/click_web.egg-info/PKG-INFO` & `click-web-0.8.3/click_web.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: click-web
-Version: 0.8.2
+Version: 0.8.3
 Summary: Serve click scripts over the web with minimal effort.
 Home-page: https://github.com/fredrik-corneliusson/click-web
 Author: Fredrik Corneliusson
 Author-email: fredrik.corneliusson@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `click-web-0.8.2/click_web.egg-info/SOURCES.txt` & `click-web-0.8.3/click_web.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `click-web-0.8.2/setup.py` & `click-web-0.8.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     'twine>=3.4',
     'wheel'
 ]
 
 
 setup(
     name='click-web',
-    version='0.8.2',
+    version='0.8.3',
     url='https://github.com/fredrik-corneliusson/click-web',
     author='Fredrik Corneliusson',
     author_email='fredrik.corneliusson@gmail.com',
     description=SHORT_DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     license='MIT',
     include_package_data=True,
```

### Comparing `click-web-0.8.2/tests/fixtures/script/a_script.py` & `click-web-0.8.3/tests/fixtures/script/a_script.py`

 * *Files identical despite different names*

### Comparing `click-web-0.8.2/tests/test_click_web.py` & `click-web-0.8.3/tests/test_click_web.py`

 * *Files identical despite different names*

### Comparing `click-web-0.8.2/tests/test_flask_get.py` & `click-web-0.8.3/tests/test_flask_get.py`

 * *Files identical despite different names*

### Comparing `click-web-0.8.2/tests/test_flask_post.py` & `click-web-0.8.3/tests/test_flask_post.py`

 * *Files identical despite different names*

### Comparing `click-web-0.8.2/tests/test_request_parsing.py` & `click-web-0.8.3/tests/test_request_parsing.py`

 * *Files identical despite different names*

