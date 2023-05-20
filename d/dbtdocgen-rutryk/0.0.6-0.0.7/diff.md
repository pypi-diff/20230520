# Comparing `tmp/dbtdocgen_rutryk-0.0.6.tar.gz` & `tmp/dbtdocgen_rutryk-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbtdocgen_rutryk-0.0.6.tar", last modified: Sat May 20 16:20:24 2023, max compression
+gzip compressed data, was "dbtdocgen_rutryk-0.0.7.tar", last modified: Sat May 20 16:38:40 2023, max compression
```

## Comparing `dbtdocgen_rutryk-0.0.6.tar` & `dbtdocgen_rutryk-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 16:20:24.891824 dbtdocgen_rutryk-0.0.6/
--rw-rw-rw-   0        0        0     1091 2023-05-20 16:16:45.000000 dbtdocgen_rutryk-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      174 2023-05-20 16:20:24.890825 dbtdocgen_rutryk-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      194 2023-05-20 16:16:45.000000 dbtdocgen_rutryk-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-20 16:20:24.845749 dbtdocgen_rutryk-0.0.6/dbtdocgen_rutryk/
--rw-rw-rw-   0        0        0        0 2023-05-20 16:16:45.000000 dbtdocgen_rutryk-0.0.6/dbtdocgen_rutryk/__init__.py
--rw-rw-rw-   0        0        0     1757 2023-05-20 16:18:52.000000 dbtdocgen_rutryk-0.0.6/dbtdocgen_rutryk/dbtdocgen.py
-drwxrwxrwx   0        0        0        0 2023-05-20 16:20:24.889830 dbtdocgen_rutryk-0.0.6/dbtdocgen_rutryk.egg-info/
--rw-rw-rw-   0        0        0      174 2023-05-20 16:20:24.000000 dbtdocgen_rutryk-0.0.6/dbtdocgen_rutryk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2023-05-20 16:20:24.000000 dbtdocgen_rutryk-0.0.6/dbtdocgen_rutryk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 16:20:24.000000 dbtdocgen_rutryk-0.0.6/dbtdocgen_rutryk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2023-05-20 16:20:24.000000 dbtdocgen_rutryk-0.0.6/dbtdocgen_rutryk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-05-20 16:20:24.000000 dbtdocgen_rutryk-0.0.6/dbtdocgen_rutryk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-20 16:20:24.000000 dbtdocgen_rutryk-0.0.6/dbtdocgen_rutryk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      448 2023-05-20 16:19:23.000000 dbtdocgen_rutryk-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-20 16:20:24.891824 dbtdocgen_rutryk-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      306 2023-05-20 16:19:32.000000 dbtdocgen_rutryk-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 16:38:40.805122 dbtdocgen_rutryk-0.0.7/
+-rw-rw-rw-   0        0        0     1091 2023-05-20 16:16:45.000000 dbtdocgen_rutryk-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      579 2023-05-20 16:38:40.804122 dbtdocgen_rutryk-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      194 2023-05-20 16:24:13.000000 dbtdocgen_rutryk-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-20 16:38:40.791255 dbtdocgen_rutryk-0.0.7/dbtdocgen_rutryk/
+-rw-rw-rw-   0        0        0        0 2023-05-20 16:16:45.000000 dbtdocgen_rutryk-0.0.7/dbtdocgen_rutryk/__init__.py
+-rw-rw-rw-   0        0        0     1744 2023-05-20 16:36:29.000000 dbtdocgen_rutryk-0.0.7/dbtdocgen_rutryk/dbtdocgen.py
+drwxrwxrwx   0        0        0        0 2023-05-20 16:38:40.801789 dbtdocgen_rutryk-0.0.7/dbtdocgen_rutryk.egg-info/
+-rw-rw-rw-   0        0        0      579 2023-05-20 16:38:40.000000 dbtdocgen_rutryk-0.0.7/dbtdocgen_rutryk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2023-05-20 16:38:40.000000 dbtdocgen_rutryk-0.0.7/dbtdocgen_rutryk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 16:38:40.000000 dbtdocgen_rutryk-0.0.7/dbtdocgen_rutryk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-05-20 16:38:40.000000 dbtdocgen_rutryk-0.0.7/dbtdocgen_rutryk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-05-20 16:38:40.000000 dbtdocgen_rutryk-0.0.7/dbtdocgen_rutryk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-20 16:38:40.000000 dbtdocgen_rutryk-0.0.7/dbtdocgen_rutryk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      448 2023-05-20 16:36:52.000000 dbtdocgen_rutryk-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-20 16:38:40.806123 dbtdocgen_rutryk-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      306 2023-05-20 16:36:56.000000 dbtdocgen_rutryk-0.0.7/setup.py
```

### Comparing `dbtdocgen_rutryk-0.0.6/LICENSE` & `dbtdocgen_rutryk-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dbtdocgen_rutryk-0.0.6/dbtdocgen_rutryk/dbtdocgen.py` & `dbtdocgen_rutryk-0.0.7/dbtdocgen_rutryk/dbtdocgen.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 @click.command()
 def dbtdocgen():
     with open(r"target\manifest.json") as file:
         manifest_data = json.load(file)
  
     names_set = set()
 
-    for node, data in sorted(list(manifest_data['nodes'].items()), key=lambda x: x[1]['fqn'][-1]):   
+    for node, data in manifest_data['nodes'].items():
         if 'unique_key' in data['unrendered_config']:
             names = str(data['fqn'][-2])
             names_set.add(names)
 
     distinct_names = list(names_set)
 
     for name in distinct_names:
         yaml = '\nversion: 2\n\nmodels:\n\n'
 
-        for node, data in list(manifest_data['nodes'].items()):
+        for node, data in sorted(list(manifest_data['nodes'].items()), key=lambda x: x[1]['fqn'][-1]):
             if name in data['fqn'][-2]:
                 if 'unique_key' in data['unrendered_config'] and len(data['fqn']) != 0 and 'biz_internal_kimball' in data['fqn']:
                     yaml += f"- name: {data['fqn'][-1]}\n"
                     yaml += "  description: This is a table in staging\n"
                     yaml += "  columns:\n"
                     yaml += f"   - name: {data['unrendered_config']['unique_key']}\n"
                     yaml += "     description: This is a surrogate key\n"
@@ -33,14 +33,12 @@
                     yaml += f"      \n"
                     file_name = f"_{name}_doc.yml"  # Use the name as the file name
                     file_path = os.path.join("\\".join(data['original_file_path'].split('\\')[:-1]), file_name)  # Specify the output folder path
 
                 else:
                     continue
             
-
-
                 with open(file_path, 'w') as file:
                     file.write(yaml)
 
 if __name__ == '__main__':
     dbtdocgen()
```

