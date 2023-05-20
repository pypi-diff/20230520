# Comparing `tmp/osconfiglib-0.1.5.tar.gz` & `tmp/osconfiglib-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osconfiglib-0.1.5.tar", max compression
+gzip compressed data, was "osconfiglib-0.2.0.tar", max compression
```

## Comparing `osconfiglib-0.1.5.tar` & `osconfiglib-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     2842 2023-05-18 22:40:25.830629 osconfiglib-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-05-18 22:40:25.830629 osconfiglib-0.1.5/osconfiglib/__init__.py
--rw-r--r--   0        0        0        0 2023-05-18 22:40:25.830629 osconfiglib-0.1.5/osconfiglib/cli/__init__.py
--rw-r--r--   0        0        0     2232 2023-05-18 22:40:25.830629 osconfiglib-0.1.5/osconfiglib/cli/main.py
--rw-r--r--   0        0        0    13211 2023-05-18 22:40:25.830629 osconfiglib-0.1.5/osconfiglib/layers.py
--rw-r--r--   0        0        0     1657 2023-05-18 22:40:25.830629 osconfiglib-0.1.5/osconfiglib/utils.py
--rw-r--r--   0        0        0      526 2023-05-18 22:40:32.370761 osconfiglib-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3725 2023-05-18 22:40:41.508499 osconfiglib-0.1.5/setup.py
--rw-r--r--   0        0        0     3409 2023-05-18 22:40:41.508894 osconfiglib-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     5301 2023-05-20 21:05:40.371503 osconfiglib-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-20 21:05:40.371503 osconfiglib-0.2.0/osconfiglib/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-20 21:05:40.371503 osconfiglib-0.2.0/osconfiglib/cli/__init__.py
+-rw-r--r--   0        0        0     2634 2023-05-20 21:05:40.371503 osconfiglib-0.2.0/osconfiglib/cli/main.py
+-rw-r--r--   0        0        0    18045 2023-05-20 21:05:40.371503 osconfiglib-0.2.0/osconfiglib/layers.py
+-rw-r--r--   0        0        0     1657 2023-05-20 21:05:40.371503 osconfiglib-0.2.0/osconfiglib/utils.py
+-rw-r--r--   0        0        0     3649 2023-05-20 21:05:40.375503 osconfiglib-0.2.0/osconfiglib/virt_customize.py
+-rw-r--r--   0        0        0      526 2023-05-20 21:05:51.939597 osconfiglib-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6284 2023-05-20 21:06:01.639460 osconfiglib-0.2.0/setup.py
+-rw-r--r--   0        0        0     5868 2023-05-20 21:06:01.640059 osconfiglib-0.2.0/PKG-INFO
```

### Comparing `osconfiglib-0.1.5/osconfiglib/cli/main.py` & `osconfiglib-0.2.0/osconfiglib/cli/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # osconfiglib/cli/main.py
 import click
-from osconfiglib import layers, utils
+from osconfiglib import layers, utils, virt_customize
 
 @click.group()
 def cli():
     pass
 
 @click.command()
 @click.option('--version', is_flag=True, help='Show the version and exit.')
@@ -63,9 +63,19 @@
 @click.command()
 @click.argument('layer_name')
 def delete_layer(layer_name):
     # Here you would call the functionality that deletes a layer
     click.echo(f'Deleting layer {layer_name}.')
 cli.add_command(delete_layer, name='delete')
 
+
+@click.command()
+@click.argument('recipe')
+@click.argument('output_dir')
+def export_squashed_configs(recipe,output_dir):
+    # Here you would call the functionality that deletes a layer
+    click.echo(f'Squashing configs for {recipe} and saving them to {output_dir}.')
+    layers.toml_export(recipe,output_dir)
+cli.add_command(export_squashed_configs, name='export-squashed-configs')
+
 if __name__ == '__main__':
     cli()
```

### Comparing `osconfiglib-0.1.5/osconfiglib/utils.py` & `osconfiglib-0.2.0/osconfiglib/utils.py`

 * *Files identical despite different names*

### Comparing `osconfiglib-0.1.5/pyproject.toml` & `osconfiglib-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "osconfiglib"
-version = "v0.1.5"
+version = "v0.2.0"
 description = "Library for image configuration"
 authors = ["Brandon Geraci <brandon.geraci@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

