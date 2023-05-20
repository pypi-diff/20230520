# Comparing `tmp/typer_shell-0.1.3.tar.gz` & `tmp/typer_shell-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typer_shell-0.1.3.tar", max compression
+gzip compressed data, was "typer_shell-0.1.4.tar", max compression
```

## Comparing `typer_shell-0.1.3.tar` & `typer_shell-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1653 2023-05-19 12:57:58.395975 typer_shell-0.1.3/README.md
--rw-r--r--   0        0        0      536 2023-05-19 13:39:07.529997 typer_shell-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       74 2023-05-19 12:45:11.119837 typer_shell-0.1.3/typer_shell/__init__.py
--rw-r--r--   0        0        0     6512 2023-05-19 13:38:31.227495 typer_shell-0.1.3/typer_shell/typer_shell.py
--rw-r--r--   0        0        0     2337 1970-01-01 00:00:00.000000 typer_shell-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1653 2023-05-19 12:57:58.395975 typer_shell-0.1.4/README.md
+-rw-r--r--   0        0        0      536 2023-05-20 12:21:08.126108 typer_shell-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       74 2023-05-19 12:45:11.119837 typer_shell-0.1.4/typer_shell/__init__.py
+-rw-r--r--   0        0        0     6778 2023-05-20 12:20:56.498186 typer_shell-0.1.4/typer_shell/typer_shell.py
+-rw-r--r--   0        0        0     2337 1970-01-01 00:00:00.000000 typer_shell-0.1.4/PKG-INFO
```

### Comparing `typer_shell-0.1.3/README.md` & `typer_shell-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `typer_shell-0.1.3/pyproject.toml` & `typer_shell-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "typer-shell"
-version = "0.1.3"
+version = "0.1.4"
 description = "A shell for typer apps with autocompletion and history"
 authors = ["fergus <fergusfettes@gmail.com>"]
 readme = "README.md"
 packages = [{include = "typer_shell"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
```

### Comparing `typer_shell-0.1.3/typer_shell/typer_shell.py` & `typer_shell-0.1.4/typer_shell/typer_shell.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,14 +29,17 @@
     app.command(hidden=True)(help)
     app.command(hidden=True)(shell)
 
     if params and not params_path:
         params_path = Path(tempfile.NamedTemporaryFile().name)
     if params_path:
         params_path = Path(params_path)
+    if params_path:
+        with params_path.open('r') as f:
+            params = yaml.load(f, Loader=yaml.FullLoader)
 
     @app.callback(invoke_without_command=True)
     def main(ctx: Context):
         _obj(ctx, params, params_path, obj)
         if ctx.invoked_subcommand is None:
             shell = make_click_shell(ctx, prompt=prompt, intro=intro)
             shell.default = _default
@@ -64,18 +67,14 @@
 ):
     # If there is an object and params, make sure the object has a field in the params dict for the shell
     # If there is no object and params, make a fkae object for holding the dicts
     # If this is not the main shell and there is already an object from the main shell, print a warning
     if not obj and not params and not params_path:
         return
 
-    if params_path and not params:
-        with params_path.open('r') as f:
-            params = yaml.load(f, Loader=yaml.FullLoader)
-
     # First ensure obj
     if obj and not getattr(ctx, 'obj'):
         ctx.obj = obj
     elif obj and getattr(ctx, 'obj'):
         print("Warning: There is already an object in the context. The new object will not be added.")
     elif not obj and not getattr(ctx, 'obj') and params:
         class _obj:
@@ -185,12 +184,24 @@
         value = value.replace("\\n", "\n").replace("\\t", "\t")
 
     dict.update({key: value})
 
 
 def _print(ctx: Context, value: Annotated[Optional[str], Argument()] = None):
     """(p) Print the local params (or a specific value)"""
-    params = ctx.obj.params_groups[ctx.parent.command.name]['params']
+    params = get_params(ctx)
     if value:
         print(params[value])
     else:
         print(params)
+
+
+def get_params(ctx):
+    name = ctx.command.name
+    if name not in ctx.obj.params_groups:
+        if ctx.parent:
+            name = ctx.parent.command.name
+    if name not in ctx.obj.params_groups:
+        print("Cant find params!")
+    else:
+        params = ctx.obj.params_groups[name]['params']
+        return params
```

### Comparing `typer_shell-0.1.3/PKG-INFO` & `typer_shell-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typer-shell
-Version: 0.1.3
+Version: 0.1.4
 Summary: A shell for typer apps with autocompletion and history
 Author: fergus
 Author-email: fergusfettes@gmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

