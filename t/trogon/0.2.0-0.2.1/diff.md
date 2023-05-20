# Comparing `tmp/trogon-0.2.0.tar.gz` & `tmp/trogon-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trogon-0.2.0.tar", max compression
+gzip compressed data, was "trogon-0.2.1.tar", max compression
```

## Comparing `trogon-0.2.0.tar` & `trogon-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     3537 2023-05-20 16:10:57.055318 trogon-0.2.0/README.md
--rw-r--r--   0        0        0     1379 2023-05-20 16:10:57.062741 trogon-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       67 2023-05-20 10:29:22.256492 trogon-0.2.0/trogon/__init__.py
--rw-r--r--   0        0        0      123 2023-05-20 10:29:22.256748 trogon-0.2.0/trogon/constants.py
--rw-r--r--   0        0        0     6304 2023-05-20 10:29:22.256860 trogon-0.2.0/trogon/introspect.py
--rw-r--r--   0        0        0    11626 2023-05-20 10:29:22.257195 trogon-0.2.0/trogon/run_command.py
--rw-r--r--   0        0        0    10558 2023-05-20 10:29:22.257466 trogon-0.2.0/trogon/trogon.py
--rw-r--r--   0        0        0     3476 2023-05-20 10:29:22.257670 trogon-0.2.0/trogon/trogon.scss
--rw-r--r--   0        0        0        0 2023-05-20 10:29:22.257716 trogon-0.2.0/trogon/widgets/__init__.py
--rw-r--r--   0        0        0     2829 2023-05-20 10:29:22.258043 trogon-0.2.0/trogon/widgets/about.py
--rw-r--r--   0        0        0     3874 2023-05-20 10:29:22.258321 trogon-0.2.0/trogon/widgets/command_info.py
--rw-r--r--   0        0        0     1985 2023-05-20 10:29:22.258561 trogon-0.2.0/trogon/widgets/command_tree.py
--rw-r--r--   0        0        0     7846 2023-05-20 10:29:22.258801 trogon-0.2.0/trogon/widgets/form.py
--rw-r--r--   0        0        0     2861 2023-05-20 10:29:22.258923 trogon-0.2.0/trogon/widgets/multiple_choice.py
--rw-r--r--   0        0        0    14891 2023-05-20 10:29:22.259311 trogon-0.2.0/trogon/widgets/parameter_controls.py
--rw-r--r--   0        0        0     5011 1970-01-01 00:00:00.000000 trogon-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     3541 2023-05-20 16:36:51.472017 trogon-0.2.1/README.md
+-rw-r--r--   0        0        0     1379 2023-05-20 18:52:52.668873 trogon-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       67 2023-05-20 10:29:22.256492 trogon-0.2.1/trogon/__init__.py
+-rw-r--r--   0        0        0      123 2023-05-20 10:29:22.256748 trogon-0.2.1/trogon/constants.py
+-rw-r--r--   0        0        0     6304 2023-05-20 10:29:22.256860 trogon-0.2.1/trogon/introspect.py
+-rw-r--r--   0        0        0    11684 2023-05-20 18:52:48.934127 trogon-0.2.1/trogon/run_command.py
+-rw-r--r--   0        0        0    10610 2023-05-20 18:52:48.934509 trogon-0.2.1/trogon/trogon.py
+-rw-r--r--   0        0        0     3476 2023-05-20 16:34:18.421968 trogon-0.2.1/trogon/trogon.scss
+-rw-r--r--   0        0        0        0 2023-05-20 10:29:22.257716 trogon-0.2.1/trogon/widgets/__init__.py
+-rw-r--r--   0        0        0     2829 2023-05-20 10:29:22.258043 trogon-0.2.1/trogon/widgets/about.py
+-rw-r--r--   0        0        0     3874 2023-05-20 10:29:22.258321 trogon-0.2.1/trogon/widgets/command_info.py
+-rw-r--r--   0        0        0     1985 2023-05-20 10:29:22.258561 trogon-0.2.1/trogon/widgets/command_tree.py
+-rw-r--r--   0        0        0     7846 2023-05-20 10:29:22.258801 trogon-0.2.1/trogon/widgets/form.py
+-rw-r--r--   0        0        0     2861 2023-05-20 10:29:22.258923 trogon-0.2.1/trogon/widgets/multiple_choice.py
+-rw-r--r--   0        0        0    14891 2023-05-20 10:29:22.259311 trogon-0.2.1/trogon/widgets/parameter_controls.py
+-rw-r--r--   0        0        0     5015 1970-01-01 00:00:00.000000 trogon-0.2.1/PKG-INFO
```

### Comparing `trogon-0.2.0/README.md` & `trogon-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 <p align="center">
-    <img src="https://github.com/Textualize/textualize-cli/assets/554369/bc0b3552-88d8-4eb8-ad14-943be7221120" alt="A pitcture of a trogon (bird) sitting on a laptop" width="300" align="center">
+    <img src="https://github.com/Textualize/textualize-cli/assets/554369/bc0b3552-88d8-4eb8-ad14-943be7221120" alt="A picture of a trogon (bird) sitting on a laptop" width="300" align="center">
 </p>
     
 [![Discord](https://img.shields.io/discord/1026214085173461072)](https://discord.gg/Enf6Z3qhVr)
 
 
 # Trogon
 
 Auto-generate friendly terminal user interfaces for command line apps.
 
 
 <details>  
   <summary> 🎬 Video demonstration </summary>
-  <hr>
 
+&nbsp;
+    
 A quick tour of a Trogon app applied to [sqlite-utils](https://github.com/simonw/sqlite-utils).
 
 
 https://github.com/Textualize/trogon/assets/554369/5ad8de04-d9f9-45af-aa21-7cb593951eff
 
 </details>
 
@@ -26,15 +27,15 @@
 
 ## How it works
 
 Trogon inspects your app and extracts a *schema* which describes the options / switches / help etc.
 It then uses that information to build a form with a familiar control for each option.
 Updating the form generates a command line which you can run with <kbd>ctrl+R</kbd>.
 
-Ultimately we would like to formalize this schema and a protocol to extract or expose it from apps, which would allow Trogon to build TUIs for any CLI app, regardless of how it was build.
+Ultimately we would like to formalize this schema and a protocol to extract or expose it from apps, which would allow Trogon to build TUIs for any CLI app, regardless of how it was built.
 If you are familiar with Swagger, think Swagger for CLIs.
 
 ## Screenshots
 
 
 <table>
```

### Comparing `trogon-0.2.0/pyproject.toml` & `trogon-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "trogon"
-version = "0.2.0"
+version = "0.2.1"
 description = "Automatically generate a Textual TUI for your Cick CLI"
 authors = ["Darren Burns <darrenb900@gmail.com>"]
 readme = "README.md"
 packages = [{include = "trogon"}]
 license = "MIT"
 homepage = "https://github.com/Textualize/trogon"
 classifiers = [
```

### Comparing `trogon-0.2.0/trogon/introspect.py` & `trogon-0.2.1/trogon/introspect.py`

 * *Files identical despite different names*

### Comparing `trogon-0.2.0/trogon/run_command.py` & `trogon-0.2.1/trogon/run_command.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,14 +163,15 @@
                             # Get the value of the counting option
                             count = next(itertools.chain.from_iterable(value_data), 1)
                             try:
                                 count = int(count)
                             except ValueError:
                                 # TODO: Not sure if this is the right thing to do
                                 count = 1
+                            count = max(1, min(count, 3))
                             if option_name.startswith("--"):
                                 args.extend([option_name] * count)
                             else:
                                 clean_option_name = option_name.lstrip("-")
                                 args.append(f"-{clean_option_name * count}")
 
         for option_name, values in multiples.items():
```

### Comparing `trogon-0.2.0/trogon/trogon.py` & `trogon-0.2.1/trogon/trogon.py`

 * *Files 1% similar despite different names*

```diff
@@ -282,17 +282,17 @@
 def tui(name: str | None = None):
     def decorator(app: click.Group | click.Command):
         @click.pass_context
         def wrapped_tui(ctx, *args, **kwargs):
             Trogon(app, app_name=name, click_context=ctx).run()
 
         if isinstance(app, click.Group):
-            app.command(name="tui")(wrapped_tui)
+            app.command(name="tui", help="Open Textual TUI.")(wrapped_tui)
         else:
             new_group = click.Group()
             new_group.add_command(app)
-            new_group.command(name="tui")(wrapped_tui)
+            new_group.command(name="tui", help="Open Textual TUI.")(wrapped_tui)
             return new_group
 
         return app
 
     return decorator
```

### Comparing `trogon-0.2.0/trogon/trogon.scss` & `trogon-0.2.1/trogon/trogon.scss`

 * *Files identical despite different names*

### Comparing `trogon-0.2.0/trogon/widgets/about.py` & `trogon-0.2.1/trogon/widgets/about.py`

 * *Files identical despite different names*

### Comparing `trogon-0.2.0/trogon/widgets/command_info.py` & `trogon-0.2.1/trogon/widgets/command_info.py`

 * *Files identical despite different names*

### Comparing `trogon-0.2.0/trogon/widgets/command_tree.py` & `trogon-0.2.1/trogon/widgets/command_tree.py`

 * *Files identical despite different names*

### Comparing `trogon-0.2.0/trogon/widgets/form.py` & `trogon-0.2.1/trogon/widgets/form.py`

 * *Files identical despite different names*

### Comparing `trogon-0.2.0/trogon/widgets/multiple_choice.py` & `trogon-0.2.1/trogon/widgets/multiple_choice.py`

 * *Files identical despite different names*

### Comparing `trogon-0.2.0/trogon/widgets/parameter_controls.py` & `trogon-0.2.1/trogon/widgets/parameter_controls.py`

 * *Files identical despite different names*

### Comparing `trogon-0.2.0/PKG-INFO` & `trogon-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trogon
-Version: 0.2.0
+Version: 0.2.1
 Summary: Automatically generate a Textual TUI for your Cick CLI
 Home-page: https://github.com/Textualize/trogon
 License: MIT
 Author: Darren Burns
 Author-email: darrenb900@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -30,29 +30,30 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Documentation
 Requires-Dist: click (>=8.0.0)
 Requires-Dist: textual (>=0.26.0)
 Description-Content-Type: text/markdown
 
 <p align="center">
-    <img src="https://github.com/Textualize/textualize-cli/assets/554369/bc0b3552-88d8-4eb8-ad14-943be7221120" alt="A pitcture of a trogon (bird) sitting on a laptop" width="300" align="center">
+    <img src="https://github.com/Textualize/textualize-cli/assets/554369/bc0b3552-88d8-4eb8-ad14-943be7221120" alt="A picture of a trogon (bird) sitting on a laptop" width="300" align="center">
 </p>
     
 [![Discord](https://img.shields.io/discord/1026214085173461072)](https://discord.gg/Enf6Z3qhVr)
 
 
 # Trogon
 
 Auto-generate friendly terminal user interfaces for command line apps.
 
 
 <details>  
   <summary> 🎬 Video demonstration </summary>
-  <hr>
 
+&nbsp;
+    
 A quick tour of a Trogon app applied to [sqlite-utils](https://github.com/simonw/sqlite-utils).
 
 
 https://github.com/Textualize/trogon/assets/554369/5ad8de04-d9f9-45af-aa21-7cb593951eff
 
 </details>
 
@@ -61,15 +62,15 @@
 
 ## How it works
 
 Trogon inspects your app and extracts a *schema* which describes the options / switches / help etc.
 It then uses that information to build a form with a familiar control for each option.
 Updating the form generates a command line which you can run with <kbd>ctrl+R</kbd>.
 
-Ultimately we would like to formalize this schema and a protocol to extract or expose it from apps, which would allow Trogon to build TUIs for any CLI app, regardless of how it was build.
+Ultimately we would like to formalize this schema and a protocol to extract or expose it from apps, which would allow Trogon to build TUIs for any CLI app, regardless of how it was built.
 If you are familiar with Swagger, think Swagger for CLIs.
 
 ## Screenshots
 
 
 <table>
```

