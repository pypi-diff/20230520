# Comparing `tmp/pynterface-0.1.1.tar.gz` & `tmp/pynterface-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynterface-0.1.1.tar", last modified: Wed May 17 14:37:14 2023, max compression
+gzip compressed data, was "pynterface-0.2.0.tar", last modified: Sat May 20 02:21:10 2023, max compression
```

## Comparing `pynterface-0.1.1.tar` & `pynterface-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-17 14:37:14.666522 pynterface-0.1.1/
--rw-r--r--   0 vivaan     (501) staff       (20)     1071 2023-05-04 02:59:32.000000 pynterface-0.1.1/LICENSE
--rw-r--r--   0 vivaan     (501) staff       (20)       33 2023-05-14 03:48:17.000000 pynterface-0.1.1/MANIFEST.in
--rw-r--r--   0 vivaan     (501) staff       (20)     1484 2023-05-17 14:37:14.666242 pynterface-0.1.1/PKG-INFO
--rw-r--r--   0 vivaan     (501) staff       (20)     1156 2023-05-14 04:10:04.000000 pynterface-0.1.1/README.md
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-17 14:37:14.664796 pynterface-0.1.1/pynterface/
--rw-r--r--   0 vivaan     (501) staff       (20)      238 2023-05-17 14:36:12.000000 pynterface-0.1.1/pynterface/__init__.py
--rw-r--r--   0 vivaan     (501) staff       (20)     2830 2023-05-17 14:35:44.000000 pynterface-0.1.1/pynterface/input.py
--rw-r--r--   0 vivaan     (501) staff       (20)     6438 2023-05-17 14:21:57.000000 pynterface-0.1.1/pynterface/loading.py
--rw-r--r--   0 vivaan     (501) staff       (20)     3367 2023-05-15 15:05:04.000000 pynterface-0.1.1/pynterface/menu.py
--rw-r--r--   0 vivaan     (501) staff       (20)     5444 2023-05-14 18:25:39.000000 pynterface-0.1.1/pynterface/printing.py
--rw-r--r--   0 vivaan     (501) staff       (20)     5848 2023-05-15 14:51:42.000000 pynterface-0.1.1/pynterface/style.py
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-17 14:37:14.665888 pynterface-0.1.1/pynterface.egg-info/
--rw-r--r--   0 vivaan     (501) staff       (20)     1484 2023-05-17 14:37:14.000000 pynterface-0.1.1/pynterface.egg-info/PKG-INFO
--rw-r--r--   0 vivaan     (501) staff       (20)      301 2023-05-17 14:37:14.000000 pynterface-0.1.1/pynterface.egg-info/SOURCES.txt
--rw-r--r--   0 vivaan     (501) staff       (20)        1 2023-05-17 14:37:14.000000 pynterface-0.1.1/pynterface.egg-info/dependency_links.txt
--rw-r--r--   0 vivaan     (501) staff       (20)       11 2023-05-17 14:37:14.000000 pynterface-0.1.1/pynterface.egg-info/top_level.txt
--rw-r--r--   0 vivaan     (501) staff       (20)       38 2023-05-17 14:37:14.666604 pynterface-0.1.1/setup.cfg
--rw-r--r--   0 vivaan     (501) staff       (20)      612 2023-05-14 04:04:56.000000 pynterface-0.1.1/setup.py
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-20 02:21:10.410116 pynterface-0.2.0/
+-rw-r--r--   0 vivaan     (501) staff       (20)     1071 2023-05-04 02:59:32.000000 pynterface-0.2.0/LICENSE
+-rw-r--r--   0 vivaan     (501) staff       (20)       33 2023-05-14 03:48:17.000000 pynterface-0.2.0/MANIFEST.in
+-rw-r--r--   0 vivaan     (501) staff       (20)     1484 2023-05-20 02:21:10.409834 pynterface-0.2.0/PKG-INFO
+-rw-r--r--   0 vivaan     (501) staff       (20)     1156 2023-05-14 04:10:04.000000 pynterface-0.2.0/README.md
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-20 02:21:10.408396 pynterface-0.2.0/pynterface/
+-rw-r--r--   0 vivaan     (501) staff       (20)      238 2023-05-20 02:20:02.000000 pynterface-0.2.0/pynterface/__init__.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     3398 2023-05-20 02:19:35.000000 pynterface-0.2.0/pynterface/input.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     6438 2023-05-17 14:21:57.000000 pynterface-0.2.0/pynterface/loading.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     3367 2023-05-15 15:05:04.000000 pynterface-0.2.0/pynterface/menu.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     5444 2023-05-14 18:25:39.000000 pynterface-0.2.0/pynterface/printing.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     5848 2023-05-15 14:51:42.000000 pynterface-0.2.0/pynterface/style.py
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-20 02:21:10.409493 pynterface-0.2.0/pynterface.egg-info/
+-rw-r--r--   0 vivaan     (501) staff       (20)     1484 2023-05-20 02:21:10.000000 pynterface-0.2.0/pynterface.egg-info/PKG-INFO
+-rw-r--r--   0 vivaan     (501) staff       (20)      301 2023-05-20 02:21:10.000000 pynterface-0.2.0/pynterface.egg-info/SOURCES.txt
+-rw-r--r--   0 vivaan     (501) staff       (20)        1 2023-05-20 02:21:10.000000 pynterface-0.2.0/pynterface.egg-info/dependency_links.txt
+-rw-r--r--   0 vivaan     (501) staff       (20)       11 2023-05-20 02:21:10.000000 pynterface-0.2.0/pynterface.egg-info/top_level.txt
+-rw-r--r--   0 vivaan     (501) staff       (20)       38 2023-05-20 02:21:10.410198 pynterface-0.2.0/setup.cfg
+-rw-r--r--   0 vivaan     (501) staff       (20)      612 2023-05-14 04:04:56.000000 pynterface-0.2.0/setup.py
```

### Comparing `pynterface-0.1.1/LICENSE` & `pynterface-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynterface-0.1.1/PKG-INFO` & `pynterface-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynterface
-Version: 0.1.1
+Version: 0.2.0
 Summary: Terminal-Based Printing Tools!
 Author: Vivaan Singhvi
 Author-email: singhvi.vivaan@gmail.com
 License: MIT
 Project-URL: Documentation, https://pynterface.readthedocs.io/en/latest/
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pynterface-0.1.1/README.md` & `pynterface-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pynterface-0.1.1/pynterface/input.py` & `pynterface-0.2.0/pynterface/input.py`

 * *Files 9% similar despite different names*

```diff
@@ -61,8 +61,31 @@
         if delimiter == "":
             items = list(row)   # splits string into char array
         else:
             items = [item for item in row.split(delimiter) if item != '']    # otherwise split by the delimiter  
         assert cols == None or (cols != None and len(items) == cols), "Column count parameter and items in the row do not match."
         output.append(list(map(item_type, items)))
 
-    return output
+    return output
+
+def yes_no(prompt: str, error_prompt: str = "Invalid choice; enter a proper form of yes or no: ") -> bool:
+    """
+
+    Here are the possible inputs: 
+
+    >>> yes = ['yes', 'y', '1']
+    >>> no = ['no', 'n', '0']
+
+    Arguments: A prompt for the option and an optional error prompt for invalid choices.
+
+    Returns: A boolean, True if 'yes' or False if 'no'
+    """
+
+    yes = ['yes', 'y', '1']
+    no = ['no', 'n', '0']
+
+    choice = input(prompt).lower()
+    
+    while choice not in yes+no:
+        choice = input(error_prompt).lower()
+
+    return choice in yes
```

### Comparing `pynterface-0.1.1/pynterface/loading.py` & `pynterface-0.2.0/pynterface/loading.py`

 * *Files identical despite different names*

### Comparing `pynterface-0.1.1/pynterface/menu.py` & `pynterface-0.2.0/pynterface/menu.py`

 * *Files identical despite different names*

### Comparing `pynterface-0.1.1/pynterface/printing.py` & `pynterface-0.2.0/pynterface/printing.py`

 * *Files identical despite different names*

### Comparing `pynterface-0.1.1/pynterface/style.py` & `pynterface-0.2.0/pynterface/style.py`

 * *Files identical despite different names*

### Comparing `pynterface-0.1.1/pynterface.egg-info/PKG-INFO` & `pynterface-0.2.0/pynterface.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynterface
-Version: 0.1.1
+Version: 0.2.0
 Summary: Terminal-Based Printing Tools!
 Author: Vivaan Singhvi
 Author-email: singhvi.vivaan@gmail.com
 License: MIT
 Project-URL: Documentation, https://pynterface.readthedocs.io/en/latest/
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pynterface-0.1.1/setup.py` & `pynterface-0.2.0/setup.py`

 * *Files identical despite different names*

