# Comparing `tmp/click-web-0.8.1.tar.gz` & `tmp/click-web-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "click-web-0.8.1.tar", last modified: Mon May  8 21:19:40 2023, max compression
+gzip compressed data, was "click-web-0.8.2.tar", last modified: Sat May 20 19:20:54 2023, max compression
```

## Comparing `click-web-0.8.1.tar` & `click-web-0.8.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:19:40.177404 click-web-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-08 21:19:25.000000 click-web-0.8.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-08 21:19:25.000000 click-web-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-08 21:19:25.000000 click-web-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-05-08 21:19:40.177404 click-web-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-08 21:19:25.000000 click-web-0.8.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:19:40.173404 click-web-0.8.1/click_web/
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-05-08 21:19:25.000000 click-web-0.8.1/click_web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-08 21:19:25.000000 click-web-0.8.1/click_web/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:19:40.177404 click-web-0.8.1/click_web/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:19:25.000000 click-web-0.8.1/click_web/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16921 2023-05-08 21:19:25.000000 click-web-0.8.1/click_web/resources/cmd_exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-05-08 21:19:25.000000 click-web-0.8.1/click_web/resources/cmd_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-05-08 21:19:25.000000 click-web-0.8.1/click_web/resources/index.py
--rw-r--r--   0 runner    (1001) docker     (123)    10237 2023-05-08 21:19:25.000000 click-web-0.8.1/click_web/resources/input_fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:19:40.177404 click-web-0.8.1/click_web/static/
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-05-08 21:19:25.000000 click-web-0.8.1/click_web/static/click_web.css
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-08 21:19:25.000000 click-web-0.8.1/click_web/static/copy_to_clipboard.js
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-08 21:19:25.000000 click-web-0.8.1/click_web/static/open_form.js
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-08 21:19:25.000000 click-web-0.8.1/click_web/static/panes.css
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-08 21:19:25.000000 click-web-0.8.1/click_web/static/panes.js
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-05-08 21:19:25.000000 click-web-0.8.1/click_web/static/post_and_read.js
--rw-r--r--   0 runner    (1001) docker     (123)    28846 2023-05-08 21:19:25.000000 click-web-0.8.1/click_web/static/pure.css
--rw-r--r--   0 runner    (1001) docker     (123)    29958 2023-05-08 21:19:25.000000 click-web-0.8.1/click_web/static/split.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:19:40.177404 click-web-0.8.1/click_web/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-08 21:19:25.000000 click-web-0.8.1/click_web/templates/command_form.html.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-08 21:19:25.000000 click-web-0.8.1/click_web/templates/form_macros.html.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-08 21:19:25.000000 click-web-0.8.1/click_web/templates/show_tree.html.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-08 21:19:25.000000 click-web-0.8.1/click_web/web_click_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:19:40.173404 click-web-0.8.1/click_web.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-05-08 21:19:40.000000 click-web-0.8.1/click_web.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-08 21:19:40.000000 click-web-0.8.1/click_web.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 21:19:40.000000 click-web-0.8.1/click_web.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 21:19:40.000000 click-web-0.8.1/click_web.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-08 21:19:40.000000 click-web-0.8.1/click_web.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 21:19:40.000000 click-web-0.8.1/click_web.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-08 21:19:40.177404 click-web-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-08 21:19:25.000000 click-web-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:19:40.177404 click-web-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:19:25.000000 click-web-0.8.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-08 21:19:25.000000 click-web-0.8.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:19:40.177404 click-web-0.8.1/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:19:25.000000 click-web-0.8.1/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-08 21:19:25.000000 click-web-0.8.1/tests/fixtures/click_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-08 21:19:25.000000 click-web-0.8.1/tests/fixtures/flask_fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:19:40.177404 click-web-0.8.1/tests/fixtures/script/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:19:25.000000 click-web-0.8.1/tests/fixtures/script/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-05-08 21:19:25.000000 click-web-0.8.1/tests/fixtures/script/a_script.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-08 21:19:25.000000 click-web-0.8.1/tests/fixtures/script/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-05-08 21:19:25.000000 click-web-0.8.1/tests/test_click_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-05-08 21:19:25.000000 click-web-0.8.1/tests/test_flask_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-05-08 21:19:25.000000 click-web-0.8.1/tests/test_flask_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-08 21:19:25.000000 click-web-0.8.1/tests/test_request_parsing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:20:54.894085 click-web-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-20 19:20:45.000000 click-web-0.8.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-20 19:20:45.000000 click-web-0.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-20 19:20:45.000000 click-web-0.8.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-05-20 19:20:54.894085 click-web-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-20 19:20:45.000000 click-web-0.8.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:20:54.890085 click-web-0.8.2/click_web/
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-05-20 19:20:45.000000 click-web-0.8.2/click_web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-20 19:20:45.000000 click-web-0.8.2/click_web/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:20:54.890085 click-web-0.8.2/click_web/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 19:20:45.000000 click-web-0.8.2/click_web/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16916 2023-05-20 19:20:45.000000 click-web-0.8.2/click_web/resources/cmd_exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-05-20 19:20:45.000000 click-web-0.8.2/click_web/resources/cmd_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-20 19:20:45.000000 click-web-0.8.2/click_web/resources/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10237 2023-05-20 19:20:45.000000 click-web-0.8.2/click_web/resources/input_fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:20:54.890085 click-web-0.8.2/click_web/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-05-20 19:20:45.000000 click-web-0.8.2/click_web/static/click_web.css
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-20 19:20:45.000000 click-web-0.8.2/click_web/static/copy_to_clipboard.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-20 19:20:45.000000 click-web-0.8.2/click_web/static/open_form.js
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-20 19:20:45.000000 click-web-0.8.2/click_web/static/panes.css
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-20 19:20:45.000000 click-web-0.8.2/click_web/static/panes.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-05-20 19:20:45.000000 click-web-0.8.2/click_web/static/post_and_read.js
+-rw-r--r--   0 runner    (1001) docker     (123)    28846 2023-05-20 19:20:45.000000 click-web-0.8.2/click_web/static/pure.css
+-rw-r--r--   0 runner    (1001) docker     (123)    29958 2023-05-20 19:20:45.000000 click-web-0.8.2/click_web/static/split.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:20:54.894085 click-web-0.8.2/click_web/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-20 19:20:45.000000 click-web-0.8.2/click_web/templates/command_form.html.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-05-20 19:20:45.000000 click-web-0.8.2/click_web/templates/form_macros.html.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-20 19:20:45.000000 click-web-0.8.2/click_web/templates/show_tree.html.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-20 19:20:45.000000 click-web-0.8.2/click_web/web_click_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:20:54.890085 click-web-0.8.2/click_web.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-05-20 19:20:54.000000 click-web-0.8.2/click_web.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-20 19:20:54.000000 click-web-0.8.2/click_web.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 19:20:54.000000 click-web-0.8.2/click_web.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 19:20:54.000000 click-web-0.8.2/click_web.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-20 19:20:54.000000 click-web-0.8.2/click_web.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-20 19:20:54.000000 click-web-0.8.2/click_web.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-20 19:20:54.894085 click-web-0.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-20 19:20:45.000000 click-web-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:20:54.894085 click-web-0.8.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 19:20:45.000000 click-web-0.8.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-20 19:20:45.000000 click-web-0.8.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:20:54.894085 click-web-0.8.2/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 19:20:45.000000 click-web-0.8.2/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-20 19:20:45.000000 click-web-0.8.2/tests/fixtures/click_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-20 19:20:45.000000 click-web-0.8.2/tests/fixtures/flask_fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:20:54.894085 click-web-0.8.2/tests/fixtures/script/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 19:20:45.000000 click-web-0.8.2/tests/fixtures/script/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-05-20 19:20:45.000000 click-web-0.8.2/tests/fixtures/script/a_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-20 19:20:45.000000 click-web-0.8.2/tests/fixtures/script/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-05-20 19:20:45.000000 click-web-0.8.2/tests/test_click_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-05-20 19:20:45.000000 click-web-0.8.2/tests/test_flask_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-05-20 19:20:45.000000 click-web-0.8.2/tests/test_flask_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-20 19:20:45.000000 click-web-0.8.2/tests/test_request_parsing.py
```

### Comparing `click-web-0.8.1/LICENSE` & `click-web-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `click-web-0.8.1/PKG-INFO` & `click-web-0.8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: click-web
-Version: 0.8.1
+Version: 0.8.2
 Summary: Serve click scripts over the web with minimal effort.
 Home-page: https://github.com/fredrik-corneliusson/click-web
 Author: Fredrik Corneliusson
 Author-email: fredrik.corneliusson@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `click-web-0.8.1/README.rst` & `click-web-0.8.2/README.rst`

 * *Files identical despite different names*

### Comparing `click-web-0.8.1/click_web/__init__.py` & `click-web-0.8.2/click_web/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,21 +27,22 @@
 'Where to place result files for download'
 OUTPUT_FOLDER = str(_get_output_folder())
 
 _flask_app = None
 logger = None
 
 
-def create_click_web_app(module, command: click.BaseCommand):
+def create_click_web_app(module, command: click.BaseCommand, root='/'):
     """
     Create a Flask app that wraps a click command. (Call once)
 
     :param module: the module that contains the click command, needed to get the path to the script.
     :param command: The actual click root command, needed to be able to read the command tree and arguments
                     in order to generate the index page and the html forms
+    :param root: the root url path to server click-web under.
     usage:
 
         from click_web import create_click_web_app
 
         import a_click_script
 
         app = create_click_web_app(a_click_script, a_click_script.a_group_or_command)
@@ -49,26 +50,30 @@
     """
     global _flask_app, logger
     assert _flask_app is None, "Flask App already created."
 
     _register(module, command)
 
     _flask_app = Flask(__name__)
+    _flask_app.config['APPLICATION_ROOT'] = root
+    root = root.rstrip('/')
 
     # add the "do" extension needed by our jinja templates
     _flask_app.jinja_env.add_extension('jinja2.ext.do')
 
-    _flask_app.add_url_rule('/', 'index', click_web.resources.index.index)
-    _flask_app.add_url_rule('/<path:command_path>', 'command', click_web.resources.cmd_form.get_form_for)
+    _flask_app.add_url_rule(root + '/', 'index', click_web.resources.index.index)
+    _flask_app.add_url_rule(root + '/<path:command_path>', 'command', click_web.resources.cmd_form.get_form_for)
+
     executor = click_web.resources.cmd_exec.Executor()
-    _flask_app.add_url_rule('/<path:command_path>', 'command_execute', executor.exec,
+    _flask_app.add_url_rule(root + '/<path:command_path>', 'command_execute', executor.exec,
                             methods=['POST'])
 
     _flask_app.logger.info(f'OUTPUT_FOLDER: {OUTPUT_FOLDER}')
-    results_blueprint = Blueprint('results', __name__, static_url_path='/static/results', static_folder=OUTPUT_FOLDER)
+    results_blueprint = Blueprint('results', __name__, static_url_path=root + '/static/results',
+                                  static_folder=OUTPUT_FOLDER)
     _flask_app.register_blueprint(results_blueprint)
 
     logger = _flask_app.logger
 
     return _flask_app
```

### Comparing `click-web-0.8.1/click_web/resources/cmd_exec.py` & `click-web-0.8.2/click_web/resources/cmd_exec.py`

 * *Files 0% similar despite different names*

```diff
@@ -174,15 +174,15 @@
         for fi in self.command_line_bulder.field_infos:
             fi.after_script_executed()
 
 
 def _get_python_interpreter():
     if sys.executable.endswith("uwsgi"):
         import uwsgi
-        python_interpreter = str((Path(uwsgi.opt.get("virtualenv").decode()) / "bin"/ "python").absolute())
+        python_interpreter = str((Path(uwsgi.opt.get("virtualenv").decode()) / "bin" / "python").absolute())
     else:
         # run with same python executable we are running with.
         python_interpreter = sys.executable
     return python_interpreter
 
 
 class CmdPart:
@@ -241,15 +241,15 @@
                         else:
                             for val in arg_values:
                                 self.command_line.append(val, secret=fi.param.form_type == 'password')
 
     @staticmethod
     def _is_option(cmd_option):
         return isinstance(cmd_option, str) and \
-               (cmd_option.startswith('--') or cmd_option.startswith('-'))
+            (cmd_option.startswith('--') or cmd_option.startswith('-'))
 
     def _process_option(self, field_info):
         vals = request.form.getlist(field_info.key)
         if field_info.is_file:
             if field_info.link_name:
                 # it's a file, append the file path
                 self.command_line.append(field_info.cmd_opt)
@@ -330,15 +330,15 @@
 
     def __str__(self):
         return str(self.param)
 
     def __lt__(self, other):
         # Make class sortable
         return (self.param.command_index, self.param.param_index) < \
-               (other.param.command_index, other.param.param_index)
+            (other.param.command_index, other.param.param_index)
 
     def __eq__(self, other):
         return self.key == other.key
 
 
 class FieldFileInfo(FieldInfo):
     """
```

### Comparing `click-web-0.8.1/click_web/resources/cmd_form.py` & `click-web-0.8.2/click_web/resources/cmd_form.py`

 * *Files identical despite different names*

### Comparing `click-web-0.8.1/click_web/resources/index.py` & `click-web-0.8.2/click_web/resources/index.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,19 +8,21 @@
 
 
 def index():
     with click.Context(click_web.click_root_cmd, info_name=click_web.click_root_cmd.name, parent=None) as ctx:
         return render_template('show_tree.html.j2', ctx=ctx, tree=_click_to_tree(ctx, click_web.click_root_cmd))
 
 
-def _click_to_tree(ctx: click.Context, node: Union[click.Command, click.MultiCommand], ancestors=[]):
+def _click_to_tree(ctx: click.Context, node: Union[click.Command, click.MultiCommand], ancestors: list=None):
     """
     Convert a click root command to a tree of dicts and lists
     :return: a json like tree
     """
+    if ancestors is None:
+        ancestors = []
     res_childs = []
     res = OrderedDict()
     res['is_group'] = isinstance(node, click.core.MultiCommand)
     if res['is_group']:
         # a group, recurse for every child
         children = [node.get_command(ctx, key) for key in node.list_commands(ctx)]
         # Sort so commands comes before groups
@@ -30,11 +32,12 @@
 
     res['name'] = node.name
 
     # Do not include any preformatted block (\b) for the short help.
     res['short_help'] = node.get_short_help_str().split('\b')[0]
     res['help'] = node.help
     path_parts = ancestors + [node]
-    res['path'] = '/' + '/'.join(p.name for p in path_parts)
+    root = click_web._flask_app.config['APPLICATION_ROOT'].rstrip('/')
+    res['path'] = root + '/' + '/'.join(p.name for p in path_parts)
     if res_childs:
         res['childs'] = res_childs
     return res
```

### Comparing `click-web-0.8.1/click_web/resources/input_fields.py` & `click-web-0.8.2/click_web/resources/input_fields.py`

 * *Files identical despite different names*

### Comparing `click-web-0.8.1/click_web/static/click_web.css` & `click-web-0.8.2/click_web/static/click_web.css`

 * *Files identical despite different names*

### Comparing `click-web-0.8.1/click_web/static/open_form.js` & `click-web-0.8.2/click_web/static/open_form.js`

 * *Files identical despite different names*

### Comparing `click-web-0.8.1/click_web/static/panes.css` & `click-web-0.8.2/click_web/static/panes.css`

 * *Files identical despite different names*

### Comparing `click-web-0.8.1/click_web/static/post_and_read.js` & `click-web-0.8.2/click_web/static/post_and_read.js`

 * *Files identical despite different names*

### Comparing `click-web-0.8.1/click_web/static/pure.css` & `click-web-0.8.2/click_web/static/pure.css`

 * *Files identical despite different names*

### Comparing `click-web-0.8.1/click_web/static/split.js` & `click-web-0.8.2/click_web/static/split.js`

 * *Files identical despite different names*

### Comparing `click-web-0.8.1/click_web/templates/command_form.html.j2` & `click-web-0.8.2/click_web/templates/command_form.html.j2`

 * *Files identical despite different names*

### Comparing `click-web-0.8.1/click_web/templates/form_macros.html.j2` & `click-web-0.8.2/click_web/templates/form_macros.html.j2`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
             hidden field that is always sent but with empty value.
             https://stackoverflow.com/a/1992745/1306577 #}
             <input name="{{ field.name }}" type='hidden' value='{{ field.off_flag }}'>
         {% endif %}
         {% if field.type == "textarea"  %}
             <textarea name="{{ field.name }}"
                       id="{{ field.name }}"
-                      cols="80" rows="7"
+                      cols="120" rows="10"
                       {{ 'required' if field.required else '' }}
                         >{{ field.value|default('', true) }}</textarea>
         {% else %}
 
             <input name="{{ field.name }}"
                    id="{{ field.name }}"
                    type="{{ field.type }}"
```

### Comparing `click-web-0.8.1/click_web/templates/show_tree.html.j2` & `click-web-0.8.2/click_web/templates/show_tree.html.j2`

 * *Files identical despite different names*

### Comparing `click-web-0.8.1/click_web/web_click_types.py` & `click-web-0.8.2/click_web/web_click_types.py`

 * *Files identical despite different names*

### Comparing `click-web-0.8.1/click_web.egg-info/PKG-INFO` & `click-web-0.8.2/click_web.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: click-web
-Version: 0.8.1
+Version: 0.8.2
 Summary: Serve click scripts over the web with minimal effort.
 Home-page: https://github.com/fredrik-corneliusson/click-web
 Author: Fredrik Corneliusson
 Author-email: fredrik.corneliusson@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `click-web-0.8.1/click_web.egg-info/SOURCES.txt` & `click-web-0.8.2/click_web.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `click-web-0.8.1/setup.py` & `click-web-0.8.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     'twine>=3.4',
     'wheel'
 ]
 
 
 setup(
     name='click-web',
-    version='0.8.1',
+    version='0.8.2',
     url='https://github.com/fredrik-corneliusson/click-web',
     author='Fredrik Corneliusson',
     author_email='fredrik.corneliusson@gmail.com',
     description=SHORT_DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     license='MIT',
     include_package_data=True,
```

### Comparing `click-web-0.8.1/tests/fixtures/script/a_script.py` & `click-web-0.8.2/tests/fixtures/script/a_script.py`

 * *Files identical despite different names*

### Comparing `click-web-0.8.1/tests/test_click_web.py` & `click-web-0.8.2/tests/test_click_web.py`

 * *Files identical despite different names*

### Comparing `click-web-0.8.1/tests/test_flask_get.py` & `click-web-0.8.2/tests/test_flask_get.py`

 * *Files identical despite different names*

### Comparing `click-web-0.8.1/tests/test_flask_post.py` & `click-web-0.8.2/tests/test_flask_post.py`

 * *Files identical despite different names*

### Comparing `click-web-0.8.1/tests/test_request_parsing.py` & `click-web-0.8.2/tests/test_request_parsing.py`

 * *Files identical despite different names*

