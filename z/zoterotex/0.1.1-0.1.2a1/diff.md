# Comparing `tmp/zoterotex-0.1.1.tar.gz` & `tmp/zoterotex-0.1.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zoterotex-0.1.1.tar", last modified: Tue May  9 00:10:31 2023, max compression
+gzip compressed data, was "zoterotex-0.1.2a1.tar", last modified: Sat May 20 03:14:49 2023, max compression
```

## Comparing `zoterotex-0.1.1.tar` & `zoterotex-0.1.2a1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-09 00:10:31.479727 zoterotex-0.1.1/
--rw-r--r--   0 galer    (1959091754) 1971611142     1340 2023-05-09 00:10:31.479525 zoterotex-0.1.1/PKG-INFO
--rw-r--r--   0 galer    (1959091754) 1971611142      930 2023-05-08 23:58:38.000000 zoterotex-0.1.1/README.md
--rw-r--r--   0 galer    (1959091754) 1971611142      695 2023-05-08 23:50:23.000000 zoterotex-0.1.1/pyproject.toml
--rw-r--r--   0 galer    (1959091754) 1971611142       38 2023-05-09 00:10:31.479788 zoterotex-0.1.1/setup.cfg
-drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-09 00:10:31.477328 zoterotex-0.1.1/zoterotex/
--rw-r--r--   0 galer    (1959091754) 1971611142       92 2023-05-09 00:09:01.000000 zoterotex-0.1.1/zoterotex/__init__.py
--rw-r--r--   0 galer    (1959091754) 1971611142      996 2023-05-09 00:08:13.000000 zoterotex-0.1.1/zoterotex/__main__.py
--rw-r--r--   0 galer    (1959091754) 1971611142     2700 2023-05-09 00:08:33.000000 zoterotex-0.1.1/zoterotex/_sync.py
-drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-09 00:10:31.479272 zoterotex-0.1.1/zoterotex.egg-info/
--rw-r--r--   0 galer    (1959091754) 1971611142     1340 2023-05-09 00:10:31.000000 zoterotex-0.1.1/zoterotex.egg-info/PKG-INFO
--rw-r--r--   0 galer    (1959091754) 1971611142      287 2023-05-09 00:10:31.000000 zoterotex-0.1.1/zoterotex.egg-info/SOURCES.txt
--rw-r--r--   0 galer    (1959091754) 1971611142        1 2023-05-09 00:10:31.000000 zoterotex-0.1.1/zoterotex.egg-info/dependency_links.txt
--rw-r--r--   0 galer    (1959091754) 1971611142       54 2023-05-09 00:10:31.000000 zoterotex-0.1.1/zoterotex.egg-info/entry_points.txt
--rw-r--r--   0 galer    (1959091754) 1971611142       32 2023-05-09 00:10:31.000000 zoterotex-0.1.1/zoterotex.egg-info/requires.txt
--rw-r--r--   0 galer    (1959091754) 1971611142       10 2023-05-09 00:10:31.000000 zoterotex-0.1.1/zoterotex.egg-info/top_level.txt
+drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-20 03:14:49.512920 zoterotex-0.1.2a1/
+-rw-r--r--   0 galer    (1959091754) 1971611142     1654 2023-05-20 03:14:49.512688 zoterotex-0.1.2a1/PKG-INFO
+-rw-r--r--   0 galer    (1959091754) 1971611142     1242 2023-05-09 00:26:36.000000 zoterotex-0.1.2a1/README.md
+-rw-r--r--   0 galer    (1959091754) 1971611142      695 2023-05-08 23:50:23.000000 zoterotex-0.1.2a1/pyproject.toml
+-rw-r--r--   0 galer    (1959091754) 1971611142       38 2023-05-20 03:14:49.512978 zoterotex-0.1.2a1/setup.cfg
+drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-20 03:14:49.510284 zoterotex-0.1.2a1/zoterotex/
+-rw-r--r--   0 galer    (1959091754) 1971611142       94 2023-05-20 03:14:22.000000 zoterotex-0.1.2a1/zoterotex/__init__.py
+-rw-r--r--   0 galer    (1959091754) 1971611142      996 2023-05-09 00:08:13.000000 zoterotex-0.1.2a1/zoterotex/__main__.py
+-rw-r--r--   0 galer    (1959091754) 1971611142     2720 2023-05-20 03:14:08.000000 zoterotex-0.1.2a1/zoterotex/_sync.py
+drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-20 03:14:49.512370 zoterotex-0.1.2a1/zoterotex.egg-info/
+-rw-r--r--   0 galer    (1959091754) 1971611142     1654 2023-05-20 03:14:49.000000 zoterotex-0.1.2a1/zoterotex.egg-info/PKG-INFO
+-rw-r--r--   0 galer    (1959091754) 1971611142      287 2023-05-20 03:14:49.000000 zoterotex-0.1.2a1/zoterotex.egg-info/SOURCES.txt
+-rw-r--r--   0 galer    (1959091754) 1971611142        1 2023-05-20 03:14:49.000000 zoterotex-0.1.2a1/zoterotex.egg-info/dependency_links.txt
+-rw-r--r--   0 galer    (1959091754) 1971611142       54 2023-05-20 03:14:49.000000 zoterotex-0.1.2a1/zoterotex.egg-info/entry_points.txt
+-rw-r--r--   0 galer    (1959091754) 1971611142       32 2023-05-20 03:14:49.000000 zoterotex-0.1.2a1/zoterotex.egg-info/requires.txt
+-rw-r--r--   0 galer    (1959091754) 1971611142       10 2023-05-20 03:14:49.000000 zoterotex-0.1.2a1/zoterotex.egg-info/top_level.txt
```

### Comparing `zoterotex-0.1.1/PKG-INFO` & `zoterotex-0.1.2a1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: zoterotex
-Version: 0.1.1
+Version: 0.1.2a1
 Summary: Wrapper for [`pyzotero`](https://github.com/urschrei/pyzotero) that keeps a BibTeX file in sync with a Zotero library.
 Author-email: Robert Gale <rcgale@gmail.com>
 Project-URL: homepage, https://github.com/rcgale/zoterotex
 Project-URL: repository, https://github.com/rcgale/zoterotex
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # zoterotex
 
-Wrapper for [`pyzotero`](https://github.com/urschrei/pyzotero) that keeps a BibTeX file in sync with a Zotero library.
+Command line wrapper for [`pyzotero`](https://github.com/urschrei/pyzotero) that keeps a BibTeX file in sync with a Zotero library.
 
 ## Setup
 
 ### API Key
 
 You'll need an API key to use `zoterotex`, which can be created in
 [your Zotero account](https://www.zotero.org/settings/keys/new).
@@ -22,26 +22,31 @@
 ### Installation
 
 ```bash
 pip install zoterotex
 ```
 
 
-## Example usage
+## Usage
 
-### For a user library
+After installation, a new command `zoterotex` (a.k.a. `python -m zoterotek`) should be available in your shell. You can 
+test this, and get usage instructions with `zoterotex --help`.
+
+Example commands—covering basically all the features—are included below.
+
+### Syncing with a user library
 
 You can retrieve your userid from [your Zotero keys settings](https://www.zotero.org/settings/keys). For example, if 
 your username is 54321, you can sync with:
 
 ```bash
 zoterotex sync user 54321 myuser.bib --api-key aabbccdd11223344
 ```
 
-### For a group library
+### Syncing a group library
 
-If you navigate to [your Zotero groups], you can grab a group ID from the url. For example, group
+If you navigate to [your Zotero groups](https://www.zotero.org/groups), you can grab a group ID from the url. For example, group
 12345678 has the URL https://www.zotero.org/groups/12345678/my_group_name, and you can sync like so:
 
 ```bash
 zoterotex sync group 12345678 mygroup.bib --api-key aabbccdd11223344
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `zoterotex-0.1.1/README.md` & `zoterotex-0.1.2a1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # zoterotex
 
-Wrapper for [`pyzotero`](https://github.com/urschrei/pyzotero) that keeps a BibTeX file in sync with a Zotero library.
+Command line wrapper for [`pyzotero`](https://github.com/urschrei/pyzotero) that keeps a BibTeX file in sync with a Zotero library.
 
 ## Setup
 
 ### API Key
 
 You'll need an API key to use `zoterotex`, which can be created in
 [your Zotero account](https://www.zotero.org/settings/keys/new).
@@ -12,26 +12,31 @@
 ### Installation
 
 ```bash
 pip install zoterotex
 ```
 
 
-## Example usage
+## Usage
 
-### For a user library
+After installation, a new command `zoterotex` (a.k.a. `python -m zoterotek`) should be available in your shell. You can 
+test this, and get usage instructions with `zoterotex --help`.
+
+Example commands—covering basically all the features—are included below.
+
+### Syncing with a user library
 
 You can retrieve your userid from [your Zotero keys settings](https://www.zotero.org/settings/keys). For example, if 
 your username is 54321, you can sync with:
 
 ```bash
 zoterotex sync user 54321 myuser.bib --api-key aabbccdd11223344
 ```
 
-### For a group library
+### Syncing a group library
 
-If you navigate to [your Zotero groups], you can grab a group ID from the url. For example, group
+If you navigate to [your Zotero groups](https://www.zotero.org/groups), you can grab a group ID from the url. For example, group
 12345678 has the URL https://www.zotero.org/groups/12345678/my_group_name, and you can sync like so:
 
 ```bash
 zoterotex sync group 12345678 mygroup.bib --api-key aabbccdd11223344
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `zoterotex-0.1.1/pyproject.toml` & `zoterotex-0.1.2a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `zoterotex-0.1.1/zoterotex/__main__.py` & `zoterotex-0.1.2a1/zoterotex/__main__.py`

 * *Files identical despite different names*

### Comparing `zoterotex-0.1.1/zoterotex/_sync.py` & `zoterotex-0.1.2a1/zoterotex/_sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         header = ZoterotexHeader.from_file(out_file)
         if header and header.library == library.library_id and header.version == library.last_modified_version():
             logging.info(f"No updates since version {header.version} (retrieved on {header.retrieved}). Quitting.")
             return
     except ValueError:
         logging.warning(f"Problem parsing headers for {out_file}. Will try to replace it.")
 
-    bibtex_database = library.items(format="bibtex")
+    bibtex_database = library.everything(library.items(format="bibtex"))
 
     if "/" in out_file:
         os.makedirs(os.path.dirname(out_file), exist_ok=True)
 
     temp_file = f"{out_file}.tmp"
     with open(temp_file, "w") as f:
         header = ZoterotexHeader(
```

### Comparing `zoterotex-0.1.1/zoterotex.egg-info/PKG-INFO` & `zoterotex-0.1.2a1/zoterotex.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: zoterotex
-Version: 0.1.1
+Version: 0.1.2a1
 Summary: Wrapper for [`pyzotero`](https://github.com/urschrei/pyzotero) that keeps a BibTeX file in sync with a Zotero library.
 Author-email: Robert Gale <rcgale@gmail.com>
 Project-URL: homepage, https://github.com/rcgale/zoterotex
 Project-URL: repository, https://github.com/rcgale/zoterotex
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # zoterotex
 
-Wrapper for [`pyzotero`](https://github.com/urschrei/pyzotero) that keeps a BibTeX file in sync with a Zotero library.
+Command line wrapper for [`pyzotero`](https://github.com/urschrei/pyzotero) that keeps a BibTeX file in sync with a Zotero library.
 
 ## Setup
 
 ### API Key
 
 You'll need an API key to use `zoterotex`, which can be created in
 [your Zotero account](https://www.zotero.org/settings/keys/new).
@@ -22,26 +22,31 @@
 ### Installation
 
 ```bash
 pip install zoterotex
 ```
 
 
-## Example usage
+## Usage
 
-### For a user library
+After installation, a new command `zoterotex` (a.k.a. `python -m zoterotek`) should be available in your shell. You can 
+test this, and get usage instructions with `zoterotex --help`.
+
+Example commands—covering basically all the features—are included below.
+
+### Syncing with a user library
 
 You can retrieve your userid from [your Zotero keys settings](https://www.zotero.org/settings/keys). For example, if 
 your username is 54321, you can sync with:
 
 ```bash
 zoterotex sync user 54321 myuser.bib --api-key aabbccdd11223344
 ```
 
-### For a group library
+### Syncing a group library
 
-If you navigate to [your Zotero groups], you can grab a group ID from the url. For example, group
+If you navigate to [your Zotero groups](https://www.zotero.org/groups), you can grab a group ID from the url. For example, group
 12345678 has the URL https://www.zotero.org/groups/12345678/my_group_name, and you can sync like so:
 
 ```bash
 zoterotex sync group 12345678 mygroup.bib --api-key aabbccdd11223344
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

