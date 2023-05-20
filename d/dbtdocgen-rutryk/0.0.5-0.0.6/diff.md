# Comparing `tmp/dbtdocgen_rutryk-0.0.5.tar.gz` & `tmp/dbtdocgen_rutryk-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbtdocgen_rutryk-0.0.5.tar", last modified: Sat May 20 16:01:10 2023, max compression
+gzip compressed data, was "dbtdocgen_rutryk-0.0.6.tar", last modified: Sat May 20 16:20:24 2023, max compression
```

## Comparing `dbtdocgen_rutryk-0.0.5.tar` & `dbtdocgen_rutryk-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 patrykpacholek   (501) staff       (20)        0 2023-05-20 16:01:10.763580 dbtdocgen_rutryk-0.0.5/
--rw-r--r--   0 patrykpacholek   (501) staff       (20)      190 2023-05-20 16:01:10.761002 dbtdocgen_rutryk-0.0.5/PKG-INFO
--rw-r--r--   0 patrykpacholek   (501) staff       (20)      192 2023-05-20 15:41:31.000000 dbtdocgen_rutryk-0.0.5/README.md
-drwxr-xr-x   0 patrykpacholek   (501) staff       (20)        0 2023-05-20 16:01:10.748628 dbtdocgen_rutryk-0.0.5/dbtdocgen_rutryk/
--rw-r--r--   0 patrykpacholek   (501) staff       (20)        0 2023-05-20 14:43:00.000000 dbtdocgen_rutryk-0.0.5/dbtdocgen_rutryk/__init__.py
--rw-r--r--   0 patrykpacholek   (501) staff       (20)     1663 2023-05-20 15:43:18.000000 dbtdocgen_rutryk-0.0.5/dbtdocgen_rutryk/dbtdocgen.py
-drwxr-xr-x   0 patrykpacholek   (501) staff       (20)        0 2023-05-20 16:01:10.760202 dbtdocgen_rutryk-0.0.5/dbtdocgen_rutryk.egg-info/
--rw-r--r--   0 patrykpacholek   (501) staff       (20)      190 2023-05-20 16:01:10.000000 dbtdocgen_rutryk-0.0.5/dbtdocgen_rutryk.egg-info/PKG-INFO
--rw-r--r--   0 patrykpacholek   (501) staff       (20)      334 2023-05-20 16:01:10.000000 dbtdocgen_rutryk-0.0.5/dbtdocgen_rutryk.egg-info/SOURCES.txt
--rw-r--r--   0 patrykpacholek   (501) staff       (20)        1 2023-05-20 16:01:10.000000 dbtdocgen_rutryk-0.0.5/dbtdocgen_rutryk.egg-info/dependency_links.txt
--rw-r--r--   0 patrykpacholek   (501) staff       (20)       90 2023-05-20 16:01:10.000000 dbtdocgen_rutryk-0.0.5/dbtdocgen_rutryk.egg-info/entry_points.txt
--rw-r--r--   0 patrykpacholek   (501) staff       (20)        6 2023-05-20 16:01:10.000000 dbtdocgen_rutryk-0.0.5/dbtdocgen_rutryk.egg-info/requires.txt
--rw-r--r--   0 patrykpacholek   (501) staff       (20)       17 2023-05-20 16:01:10.000000 dbtdocgen_rutryk-0.0.5/dbtdocgen_rutryk.egg-info/top_level.txt
--rw-r--r--   0 patrykpacholek   (501) staff       (20)      437 2023-05-20 16:00:17.000000 dbtdocgen_rutryk-0.0.5/pyproject.toml
--rw-r--r--   0 patrykpacholek   (501) staff       (20)       38 2023-05-20 16:01:10.763724 dbtdocgen_rutryk-0.0.5/setup.cfg
--rw-r--r--   0 patrykpacholek   (501) staff       (20)      294 2023-05-20 16:00:39.000000 dbtdocgen_rutryk-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 16:20:24.891824 dbtdocgen_rutryk-0.0.6/
+-rw-rw-rw-   0        0        0     1091 2023-05-20 16:16:45.000000 dbtdocgen_rutryk-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      174 2023-05-20 16:20:24.890825 dbtdocgen_rutryk-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      194 2023-05-20 16:16:45.000000 dbtdocgen_rutryk-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-20 16:20:24.845749 dbtdocgen_rutryk-0.0.6/dbtdocgen_rutryk/
+-rw-rw-rw-   0        0        0        0 2023-05-20 16:16:45.000000 dbtdocgen_rutryk-0.0.6/dbtdocgen_rutryk/__init__.py
+-rw-rw-rw-   0        0        0     1757 2023-05-20 16:18:52.000000 dbtdocgen_rutryk-0.0.6/dbtdocgen_rutryk/dbtdocgen.py
+drwxrwxrwx   0        0        0        0 2023-05-20 16:20:24.889830 dbtdocgen_rutryk-0.0.6/dbtdocgen_rutryk.egg-info/
+-rw-rw-rw-   0        0        0      174 2023-05-20 16:20:24.000000 dbtdocgen_rutryk-0.0.6/dbtdocgen_rutryk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2023-05-20 16:20:24.000000 dbtdocgen_rutryk-0.0.6/dbtdocgen_rutryk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 16:20:24.000000 dbtdocgen_rutryk-0.0.6/dbtdocgen_rutryk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2023-05-20 16:20:24.000000 dbtdocgen_rutryk-0.0.6/dbtdocgen_rutryk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-05-20 16:20:24.000000 dbtdocgen_rutryk-0.0.6/dbtdocgen_rutryk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-20 16:20:24.000000 dbtdocgen_rutryk-0.0.6/dbtdocgen_rutryk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      448 2023-05-20 16:19:23.000000 dbtdocgen_rutryk-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-20 16:20:24.891824 dbtdocgen_rutryk-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      306 2023-05-20 16:19:32.000000 dbtdocgen_rutryk-0.0.6/setup.py
```

### Comparing `dbtdocgen_rutryk-0.0.5/dbtdocgen_rutryk/dbtdocgen.py` & `dbtdocgen_rutryk-0.0.6/dbtdocgen_rutryk/dbtdocgen.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-import click
-import json
-import os
-
-@click.command()
-def dbtdocgen():
-    with open(r"target\manifest.json") as file:
-        manifest_data = json.load(file)
- 
-    names_set = set()
-
-    for node, data in manifest_data['nodes'].items():
-        if 'unique_key' in data['unrendered_config']:
-            names = str(data['fqn'][-2])
-            names_set.add(names)
-
-    distinct_names = list(names_set)
-
-    for name in distinct_names:
-        yaml = '\nversion: 2\n\nmodels:\n\n'
-
-        for node, data in list(manifest_data['nodes'].items()):
-            if name in data['fqn'][-2]:
-                if 'unique_key' in data['unrendered_config'] and len(data['fqn']) != 0 and 'biz_internal_kimball' in data['fqn']:
-                    yaml += f"- name: {data['fqn'][-1]}\n"
-                    yaml += "  description: This is a table in staging\n"
-                    yaml += "  columns:\n"
-                    yaml += f"   - name: {data['unrendered_config']['unique_key']}\n"
-                    yaml += "     description: This is a surrogate key\n"
-                    yaml += "     tests:\n"
-                    yaml += f"      - not_null\n"
-                    yaml += f"      - unique\n"
-                    yaml += f"      \n"
-                    file_name = f"_{name}_doc.yml"  # Use the name as the file name
-                    file_path = os.path.join("\\".join(data['original_file_path'].split('\\')[:-1]), file_name)  # Specify the output folder path
-
-                else:
-                    continue
-            
-
-
-                with open(file_path, 'w') as file:
-                    file.write(yaml)
-
-if __name__ == '__main__':
-    dbtdocgen()
+import click
+import json
+import os
+
+@click.command()
+def dbtdocgen():
+    with open(r"target\manifest.json") as file:
+        manifest_data = json.load(file)
+ 
+    names_set = set()
+
+    for node, data in sorted(list(manifest_data['nodes'].items()), key=lambda x: x[1]['fqn'][-1]):   
+        if 'unique_key' in data['unrendered_config']:
+            names = str(data['fqn'][-2])
+            names_set.add(names)
+
+    distinct_names = list(names_set)
+
+    for name in distinct_names:
+        yaml = '\nversion: 2\n\nmodels:\n\n'
+
+        for node, data in list(manifest_data['nodes'].items()):
+            if name in data['fqn'][-2]:
+                if 'unique_key' in data['unrendered_config'] and len(data['fqn']) != 0 and 'biz_internal_kimball' in data['fqn']:
+                    yaml += f"- name: {data['fqn'][-1]}\n"
+                    yaml += "  description: This is a table in staging\n"
+                    yaml += "  columns:\n"
+                    yaml += f"   - name: {data['unrendered_config']['unique_key']}\n"
+                    yaml += "     description: This is a surrogate key\n"
+                    yaml += "     tests:\n"
+                    yaml += f"      - not_null\n"
+                    yaml += f"      - unique\n"
+                    yaml += f"      \n"
+                    file_name = f"_{name}_doc.yml"  # Use the name as the file name
+                    file_path = os.path.join("\\".join(data['original_file_path'].split('\\')[:-1]), file_name)  # Specify the output folder path
+
+                else:
+                    continue
+            
+
+
+                with open(file_path, 'w') as file:
+                    file.write(yaml)
+
+if __name__ == '__main__':
+    dbtdocgen()
```

