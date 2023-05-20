# Comparing `tmp/typer_shell-0.1.4.tar.gz` & `tmp/typer_shell-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typer_shell-0.1.4.tar", max compression
+gzip compressed data, was "typer_shell-0.1.6.tar", max compression
```

## Comparing `typer_shell-0.1.4.tar` & `typer_shell-0.1.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1653 2023-05-19 12:57:58.395975 typer_shell-0.1.4/README.md
--rw-r--r--   0        0        0      536 2023-05-20 12:21:08.126108 typer_shell-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       74 2023-05-19 12:45:11.119837 typer_shell-0.1.4/typer_shell/__init__.py
--rw-r--r--   0        0        0     6778 2023-05-20 12:20:56.498186 typer_shell-0.1.4/typer_shell/typer_shell.py
--rw-r--r--   0        0        0     2337 1970-01-01 00:00:00.000000 typer_shell-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1653 2023-05-19 12:57:58.395975 typer_shell-0.1.6/README.md
+-rw-r--r--   0        0        0      536 2023-05-20 12:40:08.553418 typer_shell-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0       74 2023-05-19 12:45:11.119837 typer_shell-0.1.6/typer_shell/__init__.py
+-rw-r--r--   0        0        0     6854 2023-05-20 12:39:45.161616 typer_shell-0.1.6/typer_shell/typer_shell.py
+-rw-r--r--   0        0        0     2337 1970-01-01 00:00:00.000000 typer_shell-0.1.6/PKG-INFO
```

### Comparing `typer_shell-0.1.4/README.md` & `typer_shell-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `typer_shell-0.1.4/pyproject.toml` & `typer_shell-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "typer-shell"
-version = "0.1.4"
+version = "0.1.6"
 description = "A shell for typer apps with autocompletion and history"
 authors = ["fergus <fergusfettes@gmail.com>"]
 readme = "README.md"
 packages = [{include = "typer_shell"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
```

### Comparing `typer_shell-0.1.4/typer_shell/typer_shell.py` & `typer_shell-0.1.6/typer_shell/typer_shell.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     app.command(hidden=True)(help)
     app.command(hidden=True)(shell)
 
     if params and not params_path:
         params_path = Path(tempfile.NamedTemporaryFile().name)
     if params_path:
         params_path = Path(params_path)
-    if params_path:
+    if params_path and params_path.exists():
         with params_path.open('r') as f:
             params = yaml.load(f, Loader=yaml.FullLoader)
 
     @app.callback(invoke_without_command=True)
     def main(ctx: Context):
         _obj(ctx, params, params_path, obj)
         if ctx.invoked_subcommand is None:
@@ -137,14 +137,15 @@
     IPython.embed()
 
 
 def save(ctx: Context):
     """(s) Save the local params to a file"""
     params = ctx.obj.params_groups[ctx.parent.command.name]['params']
     path = ctx.obj.params_groups[ctx.parent.command.name]['path']
+    path.parent.mkdir(parents=True, exist_ok=True)
     with path.open('w') as f:
         yaml.dump(params, f)
     print(f"Saved params to {path}")
 
 
 def load(ctx: Context):
     """(l) Load the local params from a file"""
```

### Comparing `typer_shell-0.1.4/PKG-INFO` & `typer_shell-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typer-shell
-Version: 0.1.4
+Version: 0.1.6
 Summary: A shell for typer apps with autocompletion and history
 Author: fergus
 Author-email: fergusfettes@gmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

