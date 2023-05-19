# Comparing `tmp/textagon-0.1.4.tar.gz` & `tmp/textagon-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textagon-0.1.4.tar", last modified: Fri May 19 20:09:52 2023, max compression
+gzip compressed data, was "textagon-0.1.5.tar", last modified: Fri May 19 22:55:53 2023, max compression
```

## Comparing `textagon-0.1.4.tar` & `textagon-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 20:09:52.800000 textagon-0.1.4/
--rw-rw-rw-   0        0        0      181 2023-05-19 20:09:52.800000 textagon-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-19 20:09:52.800000 textagon-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      528 2023-05-19 20:09:43.000000 textagon-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-19 20:09:52.789987 textagon-0.1.4/textagon/
--rw-rw-rw-   0        0        0      105 2023-05-19 19:46:12.000000 textagon-0.1.4/textagon/__init__.py
--rw-rw-rw-   0        0        0      197 2023-05-19 15:50:30.000000 textagon-0.1.4/textagon/install-dependencies.py
--rw-rw-rw-   0        0        0    60290 2023-05-19 15:50:30.000000 textagon-0.1.4/textagon/process-text.py
--rw-rw-rw-   0        0        0     5377 2023-05-19 20:09:35.000000 textagon-0.1.4/textagon/textagon.py
-drwxrwxrwx   0        0        0        0 2023-05-19 20:09:52.799000 textagon-0.1.4/textagon.egg-info/
--rw-rw-rw-   0        0        0      181 2023-05-19 20:09:52.000000 textagon-0.1.4/textagon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-05-19 20:09:52.000000 textagon-0.1.4/textagon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 20:09:52.000000 textagon-0.1.4/textagon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2023-05-19 20:09:52.000000 textagon-0.1.4/textagon.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-19 20:09:52.000000 textagon-0.1.4/textagon.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 22:55:53.404378 textagon-0.1.5/
+-rw-rw-rw-   0        0        0      181 2023-05-19 22:55:53.404378 textagon-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-19 22:55:53.404378 textagon-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      750 2023-05-19 22:55:40.000000 textagon-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 22:55:53.391753 textagon-0.1.5/textagon/
+-rw-rw-rw-   0        0        0      180 2023-05-19 22:51:03.000000 textagon-0.1.5/textagon/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 22:55:53.388784 textagon-0.1.5/textagon/external/
+drwxrwxrwx   0        0        0        0 2023-05-19 22:55:53.403373 textagon-0.1.5/textagon/external/lexicons/
+-rw-rw-rw-   0        0        0    43255 2023-05-19 15:50:35.000000 textagon-0.1.5/textagon/external/lexicons/exclusions.txt
+-rw-rw-rw-   0        0        0      197 2023-05-19 15:50:30.000000 textagon-0.1.5/textagon/install-dependencies.py
+-rw-rw-rw-   0        0        0      309 2023-05-19 22:15:17.000000 textagon-0.1.5/textagon/post_install.py
+-rw-rw-rw-   0        0        0    60290 2023-05-19 15:50:30.000000 textagon-0.1.5/textagon/process-text.py
+-rw-rw-rw-   0        0        0     7431 2023-05-19 22:54:24.000000 textagon-0.1.5/textagon/textagon.py
+drwxrwxrwx   0        0        0        0 2023-05-19 22:55:53.403373 textagon-0.1.5/textagon.egg-info/
+-rw-rw-rw-   0        0        0      181 2023-05-19 22:55:53.000000 textagon-0.1.5/textagon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      369 2023-05-19 22:55:53.000000 textagon-0.1.5/textagon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 22:55:53.000000 textagon-0.1.5/textagon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-05-19 22:55:53.000000 textagon-0.1.5/textagon.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       77 2023-05-19 22:55:53.000000 textagon-0.1.5/textagon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-19 22:55:53.000000 textagon-0.1.5/textagon.egg-info/top_level.txt
```

### Comparing `textagon-0.1.4/textagon/process-text.py` & `textagon-0.1.5/textagon/process-text.py`

 * *Files identical despite different names*

### Comparing `textagon-0.1.4/textagon/textagon.py` & `textagon-0.1.5/textagon/textagon.py`

 * *Files 24% similar despite different names*

```diff
@@ -40,26 +40,62 @@
 
 import pickle
 import mapply
 import multiprocess.context as ctx
 ctx._force_start_method('spawn')
 import collections
 from typing import Tuple, List
+import pkg_resources
 
 
 import warnings
 warnings.filterwarnings('ignore', message = '.*looks like a URL.*', category = UserWarning, module = 'bs4')
 
-
+# initialize mapply
+useCores = mp.cpu_count()
+mapply.init(
+    n_workers = useCores) # chunk_size = 5
 
 
 def say_hello():
     print("Hello, World!")
 
-### Read Custom Lexicons Function: ###
+def setSpellChecking(exclusionsFileFullPath='None'):
+    b = enchant.Broker()
+    spellcheckerLibrary = 'en'
+    b.set_ordering(spellcheckerLibrary, 'aspell')
+
+    if exclusionsFileFullPath == 'None':
+        # Use the default exclusions file
+        exclusionsFileFullPath = pkg_resources.resource_filename('textagon', 'external/lexicons/exclusions.txt')
+    elif not os.path.isfile(exclusionsFileFullPath):
+        print('Provided exclusions file does not exist. Switching to default exclusions file.')
+        # Switch to the default exclusions file if the provided one does not exist
+        exclusionsFileFullPath = pkg_resources.resource_filename('textagon', 'external/lexicons/exclusions.txt')
+
+    try:
+        spellchecker = enchant.DictWithPWL(spellcheckerLibrary, pwl = exclusionsFileFullPath, broker = b)
+
+        exclusionsFile = open(exclusionsFileFullPath, 'r')
+        exclusionsLength = len(exclusionsFile.readlines())
+        exclusionsFile.close()
+
+        print('# Spellchecker Details #')
+        print('Provider:', spellchecker.provider)
+        print('Enchant Version:', enchant.get_enchant_version())
+        print('Dictionary Tag:', spellchecker.tag)
+        print('Dictionary Location:', spellchecker.provider.file)
+        print('Total Exclusions: ' + str(exclusionsLength))
+
+        # Return the values
+        return spellcheckerLibrary, exclusionsFileFullPath, exclusionsLength, spellchecker
+    except Exception as e:
+        print(f'Error opening or reading file {exclusionsFileFullPath}: {e}')
+        return None, None, 0, None
+
 def ReadAllLexicons (lexiconFileFullPath):
 
     def is_valid_zip_file(file_path):
         # Check if file exists
         if not os.path.exists(file_path):
             print(f"Error: The file '{file_path}' does not exist.")
             print("Please ensure that you provide the full path to the file.")
@@ -170,9 +206,21 @@
         'num_classes': num_classes,
         'samples_per_class': samples_per_class,
         'raw_data': raw_data
     }
 
     return ret_dict
 
+def ReadRawText (path: str = None):
+    print("Reading raw text...")
+    pure_chunck = SanityCheck(dataPath=path, override_original_file=False)
+    classLabels = list(pure_chunck['samples_per_class'].keys())
+    raw = [x[1] for x in pure_chunck['raw_data']]
+    print("Reading raw text completed.")
+    return({'corpus': raw, 'classLabels': classLabels})
+
+
+
+
+
```

