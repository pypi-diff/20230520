# Comparing `tmp/SportStatIQ-DataCollectors-0.0.0.tar.gz` & `tmp/SportStatIQ-DataCollectors-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SportStatIQ-DataCollectors-0.0.0.tar", last modified: Sat May 20 19:06:08 2023, max compression
+gzip compressed data, was "SportStatIQ-DataCollectors-1.0.3.tar", last modified: Sat May 20 19:01:51 2023, max compression
```

## Comparing `SportStatIQ-DataCollectors-0.0.0.tar` & `SportStatIQ-DataCollectors-1.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:06:08.926894 SportStatIQ-DataCollectors-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-20 19:06:08.926894 SportStatIQ-DataCollectors-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-20 19:05:49.000000 SportStatIQ-DataCollectors-0.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-20 19:05:49.000000 SportStatIQ-DataCollectors-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 19:06:08.926894 SportStatIQ-DataCollectors-0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-20 19:05:49.000000 SportStatIQ-DataCollectors-0.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:06:08.918893 SportStatIQ-DataCollectors-0.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:06:08.922894 SportStatIQ-DataCollectors-0.0.0/src/DataCollector/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-20 19:05:49.000000 SportStatIQ-DataCollectors-0.0.0/src/DataCollector/DataCollector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:06:08.922894 SportStatIQ-DataCollectors-0.0.0/src/DataCollector/NBA/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-20 19:05:49.000000 SportStatIQ-DataCollectors-0.0.0/src/DataCollector/NBA/NbaDataCollectorLibrary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:06:08.922894 SportStatIQ-DataCollectors-0.0.0/src/DataCollector/NBA/PlayerRawStats/
--rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-05-20 19:05:49.000000 SportStatIQ-DataCollectors-0.0.0/src/DataCollector/NBA/PlayerRawStats/PlayerRawStats.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 19:05:49.000000 SportStatIQ-DataCollectors-0.0.0/src/DataCollector/NBA/PlayerRawStats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 19:05:49.000000 SportStatIQ-DataCollectors-0.0.0/src/DataCollector/NBA/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 19:05:49.000000 SportStatIQ-DataCollectors-0.0.0/src/DataCollector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:06:08.926894 SportStatIQ-DataCollectors-0.0.0/src/SportStatIQ_DataCollectors.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-20 19:06:08.000000 SportStatIQ-DataCollectors-0.0.0/src/SportStatIQ_DataCollectors.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-20 19:06:08.000000 SportStatIQ-DataCollectors-0.0.0/src/SportStatIQ_DataCollectors.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 19:06:08.000000 SportStatIQ-DataCollectors-0.0.0/src/SportStatIQ_DataCollectors.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-20 19:06:08.000000 SportStatIQ-DataCollectors-0.0.0/src/SportStatIQ_DataCollectors.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-20 19:06:08.000000 SportStatIQ-DataCollectors-0.0.0/src/SportStatIQ_DataCollectors.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-20 19:01:51.144507 SportStatIQ-DataCollectors-1.0.3/
+-rw-rw-rw-   0        0        0     1863 2023-05-20 19:01:51.144507 SportStatIQ-DataCollectors-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1020 2023-05-15 22:48:34.000000 SportStatIQ-DataCollectors-1.0.3/README.md
+-rw-rw-rw-   0        0        0      106 2023-05-17 21:50:02.000000 SportStatIQ-DataCollectors-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-20 19:01:51.144507 SportStatIQ-DataCollectors-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1500 2023-05-20 19:01:25.000000 SportStatIQ-DataCollectors-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 19:01:51.051851 SportStatIQ-DataCollectors-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-20 19:01:51.101221 SportStatIQ-DataCollectors-1.0.3/src/DataCollector/
+-rw-rw-rw-   0        0        0      394 2023-05-19 15:32:26.000000 SportStatIQ-DataCollectors-1.0.3/src/DataCollector/DataCollector.py
+drwxrwxrwx   0        0        0        0 2023-05-20 19:01:51.107820 SportStatIQ-DataCollectors-1.0.3/src/DataCollector/NBA/
+-rw-rw-rw-   0        0        0       78 2023-05-19 15:32:12.000000 SportStatIQ-DataCollectors-1.0.3/src/DataCollector/NBA/NbaDataCollectorLibrary.py
+drwxrwxrwx   0        0        0        0 2023-05-20 19:01:51.111224 SportStatIQ-DataCollectors-1.0.3/src/DataCollector/NBA/PlayerRawStats/
+-rw-rw-rw-   0        0        0     4983 2023-05-15 23:42:41.000000 SportStatIQ-DataCollectors-1.0.3/src/DataCollector/NBA/PlayerRawStats/PlayerRawStats.py
+-rw-rw-rw-   0        0        0        0 2023-05-19 00:11:18.000000 SportStatIQ-DataCollectors-1.0.3/src/DataCollector/NBA/PlayerRawStats/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-19 00:11:09.000000 SportStatIQ-DataCollectors-1.0.3/src/DataCollector/NBA/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-20 18:24:23.000000 SportStatIQ-DataCollectors-1.0.3/src/DataCollector/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-20 19:01:51.142171 SportStatIQ-DataCollectors-1.0.3/src/SportStatIQ_DataCollectors.egg-info/
+-rw-rw-rw-   0        0        0     1863 2023-05-20 19:01:51.000000 SportStatIQ-DataCollectors-1.0.3/src/SportStatIQ_DataCollectors.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      554 2023-05-20 19:01:51.000000 SportStatIQ-DataCollectors-1.0.3/src/SportStatIQ_DataCollectors.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 19:01:51.000000 SportStatIQ-DataCollectors-1.0.3/src/SportStatIQ_DataCollectors.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-05-20 19:01:51.000000 SportStatIQ-DataCollectors-1.0.3/src/SportStatIQ_DataCollectors.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-20 19:01:51.000000 SportStatIQ-DataCollectors-1.0.3/src/SportStatIQ_DataCollectors.egg-info/top_level.txt
```

### Comparing `SportStatIQ-DataCollectors-0.0.0/PKG-INFO` & `SportStatIQ-DataCollectors-1.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-Metadata-Version: 2.1
-Name: SportStatIQ-DataCollectors
-Version: 0.0.0
-Summary: Collects data from various sports websites
-Home-page: https://github.com/SportStatIQ/SportStatIQ-DataCollectors
-Author: Matthew Myrick
-Author-email: MatthewMyrick2@gmail.com
-License: MIT
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Utilities
-Description-Content-Type: text/markdown
-
-# DataCollector
-
-This Python class provides a data collection functionality through the `NbaDataCollector` library.
-
-## Class: `DataCollector`
-
-### Initialization
-```python
-def __init__(self)
-```
-This function initializes the `DataCollector` class.
-
-### Method: `NbaDataCollector`
-```python
-def NbaDataCollector(self)
-```
-This function returns the `NbaDataCollector` library.
-
-Returns:
-- `NbaDataCollector`: The `NbaDataCollector` library.
-
-## Usage Example
-
-```python
-# Instantiate the DataCollector class
-collector = DataCollector()
-
-# Access the NbaDataCollector library
-nba_collector = collector.NbaDataCollector()
-
-# Use the NbaDataCollector library for data collection
-# ...
-```
-
-Please note that the `NbaDataCollector` library is not defined within the provided code snippet, and it is assumed to be a separate module or library that is imported by the `DataCollector` class. Make sure to import or define the `NbaDataCollector` library accordingly for the code to work properly.
+Metadata-Version: 2.1
+Name: SportStatIQ-DataCollectors
+Version: 1.0.3
+Summary: Collects data from various sports websites
+Home-page: https://github.com/SportStatIQ/SportStatIQ-DataCollectors
+Author: Matthew Myrick
+Author-email: MatthewMyrick2@gmail.com
+License: MIT
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Utilities
+Description-Content-Type: text/markdown
+
+# DataCollector
+
+This Python class provides a data collection functionality through the `NbaDataCollector` library.
+
+## Class: `DataCollector`
+
+### Initialization
+```python
+def __init__(self)
+```
+This function initializes the `DataCollector` class.
+
+### Method: `NbaDataCollector`
+```python
+def NbaDataCollector(self)
+```
+This function returns the `NbaDataCollector` library.
+
+Returns:
+- `NbaDataCollector`: The `NbaDataCollector` library.
+
+## Usage Example
+
+```python
+# Instantiate the DataCollector class
+collector = DataCollector()
+
+# Access the NbaDataCollector library
+nba_collector = collector.NbaDataCollector()
+
+# Use the NbaDataCollector library for data collection
+# ...
+```
+
+Please note that the `NbaDataCollector` library is not defined within the provided code snippet, and it is assumed to be a separate module or library that is imported by the `DataCollector` class. Make sure to import or define the `NbaDataCollector` library accordingly for the code to work properly.
```

### Comparing `SportStatIQ-DataCollectors-0.0.0/setup.py` & `SportStatIQ-DataCollectors-1.0.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-from setuptools import setup, find_packages
-import os
-
-# Get long description from README.md
-with open('README.md', 'r', encoding='utf-8') as f:
-    long_description = f.read()
-f.close()
-
-version_file = os.environ.get('GITHUB_WORKSPACE') + '/version.txt'
-with open(version_file, 'r', encoding='utf-8') as f:
-    _version = f.read().strip()
-f.close()
-
-setup(
-    name='SportStatIQ-DataCollectors',
-    version=_version,
-    author='Matthew Myrick',
-    author_email='MatthewMyrick2@gmail.com',
-    description='Collects data from various sports websites',
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    url='https://github.com/SportStatIQ/SportStatIQ-DataCollectors',
-    license='MIT',
-    packages=find_packages('src'),
-    package_dir={'': 'src'},
-    package_data={'reader': ['*.txt']},
-    install_requires=[
-        'pandas',
-        'requests',
-        'bs4'
-    ],
-    classifiers=[
-        'Development Status :: 3 - Alpha',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Topic :: Software Development :: Libraries',
-        'Topic :: Utilities',
-    ],
-)
+from setuptools import setup, find_packages
+import os
+
+# Get long description from README.md
+with open('README.md', 'r', encoding='utf-8') as f:
+    long_description = f.read()
+f.close()
+
+# version_file = os.environ.get('GITHUB_WORKSPACE') + '/version.txt'
+# with open(version_file, 'r', encoding='utf-8') as f:
+#     _version = f.read().strip()
+# f.close()
+
+setup(
+    name='SportStatIQ-DataCollectors',
+    version="1.0.3",
+    author='Matthew Myrick',
+    author_email='MatthewMyrick2@gmail.com',
+    description='Collects data from various sports websites',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    url='https://github.com/SportStatIQ/SportStatIQ-DataCollectors',
+    license='MIT',
+    packages=find_packages('src'),
+    package_dir={'': 'src'},
+    package_data={'reader': ['*.txt']},
+    install_requires=[
+        'pandas',
+        'requests',
+        'bs4'
+    ],
+    classifiers=[
+        'Development Status :: 3 - Alpha',
+        'Intended Audience :: Developers',
+        'License :: OSI Approved :: MIT License',
+        'Operating System :: OS Independent',
+        'Programming Language :: Python',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Topic :: Software Development :: Libraries',
+        'Topic :: Utilities',
+    ],
+)
```

### Comparing `SportStatIQ-DataCollectors-0.0.0/src/DataCollector/NBA/PlayerRawStats/PlayerRawStats.py` & `SportStatIQ-DataCollectors-1.0.3/src/DataCollector/NBA/PlayerRawStats/PlayerRawStats.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,305 +1,312 @@
-00000000: 0a66 726f 6d20 6273 3420 696d 706f 7274  .from bs4 import
-00000010: 2042 6561 7574 6966 756c 536f 7570 0a69   BeautifulSoup.i
-00000020: 6d70 6f72 7420 7265 7175 6573 7473 0a69  mport requests.i
-00000030: 6d70 6f72 7420 7061 6e64 6173 2061 7320  mport pandas as 
-00000040: 7064 0a0a 636c 6173 7320 506c 6179 6572  pd..class Player
-00000050: 5261 7753 7461 7473 3a0a 2020 2020 6465  RawStats:.    de
-00000060: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
-00000070: 2073 6176 655f 746f 5f64 6174 6162 6173   save_to_databas
-00000080: 653d 4661 6c73 6529 3a0a 2020 2020 2020  e=False):.      
-00000090: 2020 2727 270a 2020 2020 2020 2020 5468    '''.        Th
-000000a0: 6973 2066 756e 6374 696f 6e20 696e 6974  is function init
-000000b0: 6961 6c69 7a65 7320 7468 6520 506c 6179  ializes the Play
-000000c0: 6572 5261 7753 7461 7473 2063 6c61 7373  erRawStats class
-000000d0: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
-000000e0: 2020 2020 2020 2020 2020 2020 7361 7665              save
-000000f0: 5f74 6f5f 6461 7461 6261 7365 2028 626f  _to_database (bo
-00000100: 6f6c 2c20 6f70 7469 6f6e 616c 293a 2057  ol, optional): W
-00000110: 6865 7468 6572 206f 7220 6e6f 7420 746f  hether or not to
-00000120: 2073 6176 6520 7468 6520 6461 7461 2074   save the data t
-00000130: 6f20 7468 6520 6461 7461 6261 7365 2e20  o the database. 
-00000140: 4465 6661 756c 7473 2074 6f20 4661 6c73  Defaults to Fals
-00000150: 652e 0a20 2020 2020 2020 2027 2727 0a0a  e..        '''..
-00000160: 2020 2020 2020 2020 2320 5361 7665 2074          # Save t
-00000170: 6865 2064 6174 6120 746f 2074 6865 2064  he data to the d
-00000180: 6174 6162 6173 6520 6966 2073 7065 6369  atabase if speci
-00000190: 6669 6564 0a20 2020 2020 2020 2069 6620  fied.        if 
-000001a0: 7361 7665 5f74 6f5f 6461 7461 6261 7365  save_to_database
-000001b0: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
-000001c0: 436f 6e6e 6563 7420 746f 2074 6865 2064  Connect to the d
-000001d0: 6174 6162 6173 650a 2020 2020 2020 2020  atabase.        
-000001e0: 2020 2020 7072 696e 7428 2243 6f6e 6e65      print("Conne
-000001f0: 6374 696e 6720 746f 2074 6865 2064 6174  cting to the dat
-00000200: 6162 6173 652e 2e2e 2229 0a20 2020 200a  abase...").    .
-00000210: 0a20 2020 2064 6566 2067 6574 5f65 6163  .    def get_eac
-00000220: 685f 6761 6d65 2873 656c 662c 2070 6c61  h_game(self, pla
-00000230: 7965 725f 6669 7273 745f 6e61 6d65 2c20  yer_first_name, 
-00000240: 706c 6179 6572 5f6c 6173 745f 6e61 6d65  player_last_name
-00000250: 2c20 7365 6173 6f6e 2c20 706c 6179 6f66  , season, playof
-00000260: 6673 3d46 616c 7365 293a 0a20 2020 2020  fs=False):.     
-00000270: 2020 2027 2727 0a20 2020 2020 2020 2054     '''.        T
-00000280: 6869 7320 6675 6e63 7469 6f6e 2072 6574  his function ret
-00000290: 7572 6e73 2074 6865 2073 7461 7473 2066  urns the stats f
-000002a0: 6f72 2065 6163 6820 6761 6d65 2066 6f72  or each game for
-000002b0: 2061 2070 6c61 7965 7220 696e 2061 2073   a player in a s
-000002c0: 6561 736f 6e0a 2020 2020 2020 2020 0a20  eason.        . 
-000002d0: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
-000002e0: 2020 2020 2020 2020 2070 6c61 7965 725f           player_
-000002f0: 6669 7273 745f 6e61 6d65 2028 7374 7229  first_name (str)
-00000300: 3a20 5468 6520 6669 7273 7420 6e61 6d65  : The first name
-00000310: 206f 6620 7468 6520 706c 6179 6572 0a20   of the player. 
-00000320: 2020 2020 2020 2020 2020 2070 6c61 7965             playe
-00000330: 725f 6c61 7374 5f6e 616d 6520 2873 7472  r_last_name (str
-00000340: 293a 2054 6865 206c 6173 7420 6e61 6d65  ): The last name
-00000350: 206f 6620 7468 6520 706c 6179 6572 0a20   of the player. 
-00000360: 2020 2020 2020 2020 2020 2073 6561 736f             seaso
-00000370: 6e20 2873 7472 293a 2054 6865 2073 6561  n (str): The sea
-00000380: 736f 6e20 746f 2067 6574 2074 6865 2073  son to get the s
-00000390: 7461 7473 2066 6f72 0a20 2020 2020 2020  tats for.       
-000003a0: 2020 2020 2070 6c61 796f 6666 7320 2862       playoffs (b
-000003b0: 6f6f 6c2c 206f 7074 696f 6e61 6c29 3a20  ool, optional): 
-000003c0: 5768 6574 6865 7220 6f72 206e 6f74 2074  Whether or not t
-000003d0: 6f20 6765 7420 7468 6520 706c 6179 6f66  o get the playof
-000003e0: 6620 7374 6174 732e 2044 6566 6175 6c74  f stats. Default
-000003f0: 7320 746f 2046 616c 7365 2e0a 2020 2020  s to False..    
-00000400: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00000410: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
-00000420: 2020 2020 2020 6469 6374 3a20 4120 6469        dict: A di
-00000430: 6374 696f 6e61 7279 2063 6f6e 7461 696e  ctionary contain
-00000440: 696e 6720 7468 6520 706c 6179 6572 2073  ing the player s
-00000450: 7461 7473 206d 6174 7269 782c 2074 6865  tats matrix, the
-00000460: 2073 7461 7473 2064 6963 7469 6f6e 6172   stats dictionar
-00000470: 792c 2061 6e64 2074 6865 2073 7461 7473  y, and the stats
-00000480: 2064 6174 6166 7261 6d65 0a20 2020 2020   dataframe.     
-00000490: 2020 2027 2727 0a0a 2020 2020 2020 2020     '''..        
-000004a0: 2320 666f 726d 6174 2070 6c61 7965 7220  # format player 
-000004b0: 6e61 6d65 2066 6f72 2075 726c 0a20 2020  name for url.   
-000004c0: 2020 2020 206e 756d 5f69 6420 3d20 2230       num_id = "0
-000004d0: 3122 0a20 2020 2020 2020 2069 6620 6c65  1".        if le
-000004e0: 6e28 706c 6179 6572 5f6c 6173 745f 6e61  n(player_last_na
-000004f0: 6d65 2920 3e20 353a 0a20 2020 2020 2020  me) > 5:.       
-00000500: 2020 2020 2070 6c61 7965 725f 6e61 6d65       player_name
-00000510: 203d 2070 6c61 7965 725f 6c61 7374 5f6e   = player_last_n
-00000520: 616d 655b 3a35 5d20 2b20 706c 6179 6572  ame[:5] + player
-00000530: 5f66 6972 7374 5f6e 616d 655b 3a32 5d0a  _first_name[:2].
-00000540: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00000550: 2020 2020 2020 2020 2020 706c 6179 6572            player
-00000560: 5f6e 616d 6520 3d20 706c 6179 6572 5f6c  _name = player_l
-00000570: 6173 745f 6e61 6d65 202b 2070 6c61 7965  ast_name + playe
-00000580: 725f 6669 7273 745f 6e61 6d65 5b3a 325d  r_first_name[:2]
-00000590: 0a0a 2020 2020 2020 2020 2320 666f 726d  ..        # form
-000005a0: 6174 2075 726c 0a20 2020 2020 2020 2075  at url.        u
-000005b0: 726c 203d 2066 2268 7474 7073 3a2f 2f77  rl = f"https://w
-000005c0: 7777 2e62 6173 6b65 7462 616c 6c2d 7265  ww.basketball-re
-000005d0: 6665 7265 6e63 652e 636f 6d2f 706c 6179  ference.com/play
-000005e0: 6572 732f 682f 7b70 6c61 7965 725f 6e61  ers/h/{player_na
-000005f0: 6d65 2e6c 6f77 6572 2829 7d7b 6e75 6d5f  me.lower()}{num_
-00000600: 6964 7d2f 6761 6d65 6c6f 672f 7b73 6561  id}/gamelog/{sea
-00000610: 736f 6e7d 220a 2020 2020 2020 2020 7072  son}".        pr
-00000620: 696e 7428 6622 5573 696e 6720 5552 4c3a  int(f"Using URL:
-00000630: 207b 7572 6c7d 2229 0a0a 2020 2020 2020   {url}")..      
-00000640: 2020 2320 4765 7420 7468 6520 7265 7370    # Get the resp
-00000650: 6f6e 7365 0a20 2020 2020 2020 2072 6573  onse.        res
-00000660: 706f 6e73 6520 3d20 7265 7175 6573 7473  ponse = requests
-00000670: 2e67 6574 2875 726c 290a 0a20 2020 2020  .get(url)..     
-00000680: 2020 2023 2043 6865 636b 2069 6620 7468     # Check if th
-00000690: 6520 7265 7370 6f6e 7365 2077 6173 2073  e response was s
-000006a0: 7563 6365 7373 6675 6c0a 2020 2020 2020  uccessful.      
-000006b0: 2020 6966 2072 6573 706f 6e73 652e 7374    if response.st
-000006c0: 6174 7573 5f63 6f64 6520 213d 2032 3030  atus_code != 200
-000006d0: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
-000006e0: 5072 696e 7420 6572 726f 7220 6d65 7373  Print error mess
-000006f0: 6167 6573 0a20 2020 2020 2020 2020 2020  ages.           
-00000700: 2070 7269 6e74 2866 2246 6169 6c65 6420   print(f"Failed 
-00000710: 746f 2072 6574 7269 6576 6520 6461 7461  to retrieve data
-00000720: 2066 6f72 207b 706c 6179 6572 5f6e 616d   for {player_nam
-00000730: 657d 2069 6e20 7b73 6561 736f 6e7d 2229  e} in {season}")
-00000740: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-00000750: 6e74 2866 2253 7461 7475 7320 636f 6465  nt(f"Status code
-00000760: 3a20 7b72 6573 706f 6e73 652e 7374 6174  : {response.stat
-00000770: 7573 5f63 6f64 657d 2229 0a20 2020 2020  us_code}").     
-00000780: 2020 2020 2020 2070 7269 6e74 2866 2252         print(f"R
-00000790: 6561 736f 6e3a 207b 7265 7370 6f6e 7365  eason: {response
-000007a0: 2e72 6561 736f 6e7d 2229 0a20 2020 2020  .reason}").     
-000007b0: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
-000007c0: 6e65 0a0a 2020 2020 2020 2020 2320 5061  ne..        # Pa
-000007d0: 7273 6520 7468 6520 7265 7370 6f6e 7365  rse the response
-000007e0: 0a20 2020 2020 2020 2073 6f75 7020 3d20  .        soup = 
-000007f0: 4265 6175 7469 6675 6c53 6f75 7028 7265  BeautifulSoup(re
-00000800: 7370 6f6e 7365 2e74 6578 742c 2027 6874  sponse.text, 'ht
-00000810: 6d6c 2e70 6172 7365 7227 290a 0a20 2020  ml.parser')..   
-00000820: 2020 2020 2023 2046 696e 6420 7468 6520       # Find the 
-00000830: 7461 626c 6520 7769 7468 2074 6865 2073  table with the s
-00000840: 7461 7473 0a20 2020 2020 2020 2074 6162  tats.        tab
-00000850: 6c65 203d 2073 6f75 702e 6669 6e64 2827  le = soup.find('
-00000860: 7461 626c 6527 2c20 7b27 6964 273a 2027  table', {'id': '
-00000870: 7067 6c5f 6261 7369 6327 7d29 0a0a 2020  pgl_basic'})..  
-00000880: 2020 2020 2020 2320 4765 7420 7468 6520        # Get the 
-00000890: 6865 6164 6572 730a 2020 2020 2020 2020  headers.        
-000008a0: 6865 6164 6572 7320 3d20 5b74 682e 6765  headers = [th.ge
-000008b0: 7454 6578 7428 2920 666f 7220 7468 2069  tText() for th i
-000008c0: 6e20 7461 626c 652e 6669 6e64 416c 6c28  n table.findAll(
-000008d0: 2774 7227 295b 305d 2e66 696e 6441 6c6c  'tr')[0].findAll
-000008e0: 2827 7468 2729 5d5b 313a 5d0a 0a20 2020  ('th')][1:]..   
-000008f0: 2020 2020 2023 2047 6574 2074 6865 2072       # Get the r
-00000900: 6f77 730a 2020 2020 2020 2020 726f 7773  ows.        rows
-00000910: 203d 2074 6162 6c65 2e66 696e 6441 6c6c   = table.findAll
-00000920: 2827 7472 2729 5b31 3a5d 0a20 2020 2020  ('tr')[1:].     
-00000930: 2020 2070 6c61 7965 725f 7374 6174 735f     player_stats_
-00000940: 6d61 7472 6978 203d 205b 5b74 642e 6765  matrix = [[td.ge
-00000950: 7454 6578 7428 2920 666f 7220 7464 2069  tText() for td i
-00000960: 6e20 726f 7773 5b69 5d2e 6669 6e64 416c  n rows[i].findAl
-00000970: 6c28 2774 6427 295d 0a20 2020 2020 2020  l('td')].       
-00000980: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00000990: 2069 2069 6e20 7261 6e67 6528 6c65 6e28   i in range(len(
-000009a0: 726f 7773 2929 5d0a 2020 2020 2020 2020  rows))].        
-000009b0: 2320 666f 726d 6174 2074 6865 2064 6174  # format the dat
-000009c0: 6120 666f 7220 7061 6e64 6173 2064 6174  a for pandas dat
-000009d0: 6166 7261 6d65 0a20 2020 2020 2020 2073  aframe.        s
-000009e0: 7461 7473 5f64 6963 7420 3d20 7b7d 0a20  tats_dict = {}. 
-000009f0: 2020 2020 2020 2023 2069 7465 7261 7465         # iterate
-00000a00: 2074 6872 6f75 6768 2065 6163 6820 726f   through each ro
-00000a10: 770a 2020 2020 2020 2020 666f 7220 726f  w.        for ro
-00000a20: 775f 696e 6465 7820 696e 2072 616e 6765  w_index in range
-00000a30: 286c 656e 2870 6c61 7965 725f 7374 6174  (len(player_stat
-00000a40: 735f 6d61 7472 6978 2929 3a0a 2020 2020  s_matrix)):.    
-00000a50: 2020 2020 2020 2020 2320 6368 6563 6b20          # check 
-00000a60: 6966 2074 6865 2072 6f77 2069 7320 656d  if the row is em
-00000a70: 7074 790a 2020 2020 2020 2020 2020 2020  pty.            
-00000a80: 6966 2070 6c61 7965 725f 7374 6174 735f  if player_stats_
-00000a90: 6d61 7472 6978 5b72 6f77 5f69 6e64 6578  matrix[row_index
-00000aa0: 5d20 213d 205b 5d3a 0a20 2020 2020 2020  ] != []:.       
-00000ab0: 2020 2020 2020 2020 2023 2043 6865 636b           # Check
-00000ac0: 206c 6173 7420 636f 6c75 6d6e 2074 6f20   last column to 
-00000ad0: 7365 6520 6966 2070 6c61 7965 7220 706c  see if player pl
-00000ae0: 6179 6564 2069 6e20 7468 6520 6761 6d65  ayed in the game
-00000af0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000b00: 2069 6620 2822 2b22 206e 6f74 2069 6e20   if ("+" not in 
-00000b10: 706c 6179 6572 5f73 7461 7473 5f6d 6174  player_stats_mat
-00000b20: 7269 785b 726f 775f 696e 6465 785d 5b2d  rix[row_index][-
-00000b30: 315d 2920 616e 6420 2822 2d22 206e 6f74  1]) and ("-" not
-00000b40: 2069 6e20 706c 6179 6572 5f73 7461 7473   in player_stats
-00000b50: 5f6d 6174 7269 785b 726f 775f 696e 6465  _matrix[row_inde
-00000b60: 785d 5b2d 315d 293a 0a20 2020 2020 2020  x][-1]):.       
-00000b70: 2020 2020 2020 2020 2020 2020 2023 2067               # g
-00000b80: 6574 2074 6865 2064 6966 6665 7265 6e63  et the differenc
-00000b90: 6520 696e 206c 656e 6774 6820 6265 7477  e in length betw
-00000ba0: 6565 6e20 7468 6520 6865 6164 6572 7320  een the headers 
-00000bb0: 616e 6420 7468 6520 726f 770a 2020 2020  and the row.    
-00000bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000bd0: 726f 775f 6469 6666 203d 206c 656e 2868  row_diff = len(h
-00000be0: 6561 6465 7273 2920 2d20 6c65 6e28 706c  eaders) - len(pl
-00000bf0: 6179 6572 5f73 7461 7473 5f6d 6174 7269  ayer_stats_matri
-00000c00: 785b 726f 775f 696e 6465 785d 290a 2020  x[row_index]).  
-00000c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c20: 2020 2320 6170 7065 6e64 696e 6720 6c61    # appending la
-00000c30: 7374 2076 616c 7565 206f 6620 706c 6179  st value of play
+00000000: 0d0a 6672 6f6d 2062 7334 2069 6d70 6f72  ..from bs4 impor
+00000010: 7420 4265 6175 7469 6675 6c53 6f75 700d  t BeautifulSoup.
+00000020: 0a69 6d70 6f72 7420 7265 7175 6573 7473  .import requests
+00000030: 0d0a 696d 706f 7274 2070 616e 6461 7320  ..import pandas 
+00000040: 6173 2070 640d 0a0d 0a63 6c61 7373 2050  as pd....class P
+00000050: 6c61 7965 7252 6177 5374 6174 733a 0d0a  layerRawStats:..
+00000060: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+00000070: 2873 656c 662c 2073 6176 655f 746f 5f64  (self, save_to_d
+00000080: 6174 6162 6173 653d 4661 6c73 6529 3a0d  atabase=False):.
+00000090: 0a20 2020 2020 2020 2027 2727 0d0a 2020  .        '''..  
+000000a0: 2020 2020 2020 5468 6973 2066 756e 6374        This funct
+000000b0: 696f 6e20 696e 6974 6961 6c69 7a65 7320  ion initializes 
+000000c0: 7468 6520 506c 6179 6572 5261 7753 7461  the PlayerRawSta
+000000d0: 7473 2063 6c61 7373 0d0a 0d0a 2020 2020  ts class....    
+000000e0: 2020 2020 4172 6773 3a0d 0a20 2020 2020      Args:..     
+000000f0: 2020 2020 2020 2073 6176 655f 746f 5f64         save_to_d
+00000100: 6174 6162 6173 6520 2862 6f6f 6c2c 206f  atabase (bool, o
+00000110: 7074 696f 6e61 6c29 3a20 5768 6574 6865  ptional): Whethe
+00000120: 7220 6f72 206e 6f74 2074 6f20 7361 7665  r or not to save
+00000130: 2074 6865 2064 6174 6120 746f 2074 6865   the data to the
+00000140: 2064 6174 6162 6173 652e 2044 6566 6175   database. Defau
+00000150: 6c74 7320 746f 2046 616c 7365 2e0d 0a20  lts to False... 
+00000160: 2020 2020 2020 2027 2727 0d0a 0d0a 2020         '''....  
+00000170: 2020 2020 2020 2320 5361 7665 2074 6865        # Save the
+00000180: 2064 6174 6120 746f 2074 6865 2064 6174   data to the dat
+00000190: 6162 6173 6520 6966 2073 7065 6369 6669  abase if specifi
+000001a0: 6564 0d0a 2020 2020 2020 2020 6966 2073  ed..        if s
+000001b0: 6176 655f 746f 5f64 6174 6162 6173 653a  ave_to_database:
+000001c0: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+000001d0: 436f 6e6e 6563 7420 746f 2074 6865 2064  Connect to the d
+000001e0: 6174 6162 6173 650d 0a20 2020 2020 2020  atabase..       
+000001f0: 2020 2020 2070 7269 6e74 2822 436f 6e6e       print("Conn
+00000200: 6563 7469 6e67 2074 6f20 7468 6520 6461  ecting to the da
+00000210: 7461 6261 7365 2e2e 2e22 290d 0a20 2020  tabase...")..   
+00000220: 200d 0a0d 0a20 2020 2064 6566 2067 6574   ....    def get
+00000230: 5f65 6163 685f 6761 6d65 2873 656c 662c  _each_game(self,
+00000240: 2070 6c61 7965 725f 6669 7273 745f 6e61   player_first_na
+00000250: 6d65 2c20 706c 6179 6572 5f6c 6173 745f  me, player_last_
+00000260: 6e61 6d65 2c20 7365 6173 6f6e 2c20 706c  name, season, pl
+00000270: 6179 6f66 6673 3d46 616c 7365 293a 0d0a  ayoffs=False):..
+00000280: 2020 2020 2020 2020 2727 270d 0a20 2020          '''..   
+00000290: 2020 2020 2054 6869 7320 6675 6e63 7469       This functi
+000002a0: 6f6e 2072 6574 7572 6e73 2074 6865 2073  on returns the s
+000002b0: 7461 7473 2066 6f72 2065 6163 6820 6761  tats for each ga
+000002c0: 6d65 2066 6f72 2061 2070 6c61 7965 7220  me for a player 
+000002d0: 696e 2061 2073 6561 736f 6e0d 0a20 2020  in a season..   
+000002e0: 2020 2020 200d 0a20 2020 2020 2020 2041       ..        A
+000002f0: 7267 733a 0d0a 2020 2020 2020 2020 2020  rgs:..          
+00000300: 2020 706c 6179 6572 5f66 6972 7374 5f6e    player_first_n
+00000310: 616d 6520 2873 7472 293a 2054 6865 2066  ame (str): The f
+00000320: 6972 7374 206e 616d 6520 6f66 2074 6865  irst name of the
+00000330: 2070 6c61 7965 720d 0a20 2020 2020 2020   player..       
+00000340: 2020 2020 2070 6c61 7965 725f 6c61 7374       player_last
+00000350: 5f6e 616d 6520 2873 7472 293a 2054 6865  _name (str): The
+00000360: 206c 6173 7420 6e61 6d65 206f 6620 7468   last name of th
+00000370: 6520 706c 6179 6572 0d0a 2020 2020 2020  e player..      
+00000380: 2020 2020 2020 7365 6173 6f6e 2028 7374        season (st
+00000390: 7229 3a20 5468 6520 7365 6173 6f6e 2074  r): The season t
+000003a0: 6f20 6765 7420 7468 6520 7374 6174 7320  o get the stats 
+000003b0: 666f 720d 0a20 2020 2020 2020 2020 2020  for..           
+000003c0: 2070 6c61 796f 6666 7320 2862 6f6f 6c2c   playoffs (bool,
+000003d0: 206f 7074 696f 6e61 6c29 3a20 5768 6574   optional): Whet
+000003e0: 6865 7220 6f72 206e 6f74 2074 6f20 6765  her or not to ge
+000003f0: 7420 7468 6520 706c 6179 6f66 6620 7374  t the playoff st
+00000400: 6174 732e 2044 6566 6175 6c74 7320 746f  ats. Defaults to
+00000410: 2046 616c 7365 2e0d 0a20 2020 2020 2020   False...       
+00000420: 2020 2020 200d 0a20 2020 2020 2020 2052       ..        R
+00000430: 6574 7572 6e73 3a0d 0a20 2020 2020 2020  eturns:..       
+00000440: 2020 2020 2064 6963 743a 2041 2064 6963       dict: A dic
+00000450: 7469 6f6e 6172 7920 636f 6e74 6169 6e69  tionary containi
+00000460: 6e67 2074 6865 2070 6c61 7965 7220 7374  ng the player st
+00000470: 6174 7320 6d61 7472 6978 2c20 7468 6520  ats matrix, the 
+00000480: 7374 6174 7320 6469 6374 696f 6e61 7279  stats dictionary
+00000490: 2c20 616e 6420 7468 6520 7374 6174 7320  , and the stats 
+000004a0: 6461 7461 6672 616d 650d 0a20 2020 2020  dataframe..     
+000004b0: 2020 2027 2727 0d0a 0d0a 2020 2020 2020     '''....      
+000004c0: 2020 2320 666f 726d 6174 2070 6c61 7965    # format playe
+000004d0: 7220 6e61 6d65 2066 6f72 2075 726c 0d0a  r name for url..
+000004e0: 2020 2020 2020 2020 6e75 6d5f 6964 203d          num_id =
+000004f0: 2022 3031 220d 0a20 2020 2020 2020 2069   "01"..        i
+00000500: 6620 6c65 6e28 706c 6179 6572 5f6c 6173  f len(player_las
+00000510: 745f 6e61 6d65 2920 3e20 353a 0d0a 2020  t_name) > 5:..  
+00000520: 2020 2020 2020 2020 2020 706c 6179 6572            player
+00000530: 5f6e 616d 6520 3d20 706c 6179 6572 5f6c  _name = player_l
+00000540: 6173 745f 6e61 6d65 5b3a 355d 202b 2070  ast_name[:5] + p
+00000550: 6c61 7965 725f 6669 7273 745f 6e61 6d65  layer_first_name
+00000560: 5b3a 325d 0d0a 2020 2020 2020 2020 656c  [:2]..        el
+00000570: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+00000580: 2070 6c61 7965 725f 6e61 6d65 203d 2070   player_name = p
+00000590: 6c61 7965 725f 6c61 7374 5f6e 616d 6520  layer_last_name 
+000005a0: 2b20 706c 6179 6572 5f66 6972 7374 5f6e  + player_first_n
+000005b0: 616d 655b 3a32 5d0d 0a0d 0a20 2020 2020  ame[:2]....     
+000005c0: 2020 2023 2066 6f72 6d61 7420 7572 6c0d     # format url.
+000005d0: 0a20 2020 2020 2020 2075 726c 203d 2066  .        url = f
+000005e0: 2268 7474 7073 3a2f 2f77 7777 2e62 6173  "https://www.bas
+000005f0: 6b65 7462 616c 6c2d 7265 6665 7265 6e63  ketball-referenc
+00000600: 652e 636f 6d2f 706c 6179 6572 732f 682f  e.com/players/h/
+00000610: 7b70 6c61 7965 725f 6e61 6d65 2e6c 6f77  {player_name.low
+00000620: 6572 2829 7d7b 6e75 6d5f 6964 7d2f 6761  er()}{num_id}/ga
+00000630: 6d65 6c6f 672f 7b73 6561 736f 6e7d 220d  melog/{season}".
+00000640: 0a20 2020 2020 2020 2070 7269 6e74 2866  .        print(f
+00000650: 2255 7369 6e67 2055 524c 3a20 7b75 726c  "Using URL: {url
+00000660: 7d22 290d 0a0d 0a20 2020 2020 2020 2023  }")....        #
+00000670: 2047 6574 2074 6865 2072 6573 706f 6e73   Get the respons
+00000680: 650d 0a20 2020 2020 2020 2072 6573 706f  e..        respo
+00000690: 6e73 6520 3d20 7265 7175 6573 7473 2e67  nse = requests.g
+000006a0: 6574 2875 726c 290d 0a0d 0a20 2020 2020  et(url)....     
+000006b0: 2020 2023 2043 6865 636b 2069 6620 7468     # Check if th
+000006c0: 6520 7265 7370 6f6e 7365 2077 6173 2073  e response was s
+000006d0: 7563 6365 7373 6675 6c0d 0a20 2020 2020  uccessful..     
+000006e0: 2020 2069 6620 7265 7370 6f6e 7365 2e73     if response.s
+000006f0: 7461 7475 735f 636f 6465 2021 3d20 3230  tatus_code != 20
+00000700: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
+00000710: 2320 5072 696e 7420 6572 726f 7220 6d65  # Print error me
+00000720: 7373 6167 6573 0d0a 2020 2020 2020 2020  ssages..        
+00000730: 2020 2020 7072 696e 7428 6622 4661 696c      print(f"Fail
+00000740: 6564 2074 6f20 7265 7472 6965 7665 2064  ed to retrieve d
+00000750: 6174 6120 666f 7220 7b70 6c61 7965 725f  ata for {player_
+00000760: 6e61 6d65 7d20 696e 207b 7365 6173 6f6e  name} in {season
+00000770: 7d22 290d 0a20 2020 2020 2020 2020 2020  }")..           
+00000780: 2070 7269 6e74 2866 2253 7461 7475 7320   print(f"Status 
+00000790: 636f 6465 3a20 7b72 6573 706f 6e73 652e  code: {response.
+000007a0: 7374 6174 7573 5f63 6f64 657d 2229 0d0a  status_code}")..
+000007b0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+000007c0: 7428 6622 5265 6173 6f6e 3a20 7b72 6573  t(f"Reason: {res
+000007d0: 706f 6e73 652e 7265 6173 6f6e 7d22 290d  ponse.reason}").
+000007e0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000007f0: 7572 6e20 4e6f 6e65 0d0a 0d0a 2020 2020  urn None....    
+00000800: 2020 2020 2320 5061 7273 6520 7468 6520      # Parse the 
+00000810: 7265 7370 6f6e 7365 0d0a 2020 2020 2020  response..      
+00000820: 2020 736f 7570 203d 2042 6561 7574 6966    soup = Beautif
+00000830: 756c 536f 7570 2872 6573 706f 6e73 652e  ulSoup(response.
+00000840: 7465 7874 2c20 2768 746d 6c2e 7061 7273  text, 'html.pars
+00000850: 6572 2729 0d0a 0d0a 2020 2020 2020 2020  er')....        
+00000860: 2320 4669 6e64 2074 6865 2074 6162 6c65  # Find the table
+00000870: 2077 6974 6820 7468 6520 7374 6174 730d   with the stats.
+00000880: 0a20 2020 2020 2020 2074 6162 6c65 203d  .        table =
+00000890: 2073 6f75 702e 6669 6e64 2827 7461 626c   soup.find('tabl
+000008a0: 6527 2c20 7b27 6964 273a 2027 7067 6c5f  e', {'id': 'pgl_
+000008b0: 6261 7369 6327 7d29 0d0a 0d0a 2020 2020  basic'})....    
+000008c0: 2020 2020 2320 4765 7420 7468 6520 6865      # Get the he
+000008d0: 6164 6572 730d 0a20 2020 2020 2020 2068  aders..        h
+000008e0: 6561 6465 7273 203d 205b 7468 2e67 6574  eaders = [th.get
+000008f0: 5465 7874 2829 2066 6f72 2074 6820 696e  Text() for th in
+00000900: 2074 6162 6c65 2e66 696e 6441 6c6c 2827   table.findAll('
+00000910: 7472 2729 5b30 5d2e 6669 6e64 416c 6c28  tr')[0].findAll(
+00000920: 2774 6827 295d 5b31 3a5d 0d0a 0d0a 2020  'th')][1:]....  
+00000930: 2020 2020 2020 2320 4765 7420 7468 6520        # Get the 
+00000940: 726f 7773 0d0a 2020 2020 2020 2020 726f  rows..        ro
+00000950: 7773 203d 2074 6162 6c65 2e66 696e 6441  ws = table.findA
+00000960: 6c6c 2827 7472 2729 5b31 3a5d 0d0a 2020  ll('tr')[1:]..  
+00000970: 2020 2020 2020 706c 6179 6572 5f73 7461        player_sta
+00000980: 7473 5f6d 6174 7269 7820 3d20 5b5b 7464  ts_matrix = [[td
+00000990: 2e67 6574 5465 7874 2829 2066 6f72 2074  .getText() for t
+000009a0: 6420 696e 2072 6f77 735b 695d 2e66 696e  d in rows[i].fin
+000009b0: 6441 6c6c 2827 7464 2729 5d0d 0a20 2020  dAll('td')]..   
+000009c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000009d0: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+000009e0: 6c65 6e28 726f 7773 2929 5d0d 0a20 2020  len(rows))]..   
+000009f0: 2020 2020 2023 2066 6f72 6d61 7420 7468       # format th
+00000a00: 6520 6461 7461 2066 6f72 2070 616e 6461  e data for panda
+00000a10: 7320 6461 7461 6672 616d 650d 0a20 2020  s dataframe..   
+00000a20: 2020 2020 2073 7461 7473 5f64 6963 7420       stats_dict 
+00000a30: 3d20 7b7d 0d0a 2020 2020 2020 2020 2320  = {}..        # 
+00000a40: 6974 6572 6174 6520 7468 726f 7567 6820  iterate through 
+00000a50: 6561 6368 2072 6f77 0d0a 2020 2020 2020  each row..      
+00000a60: 2020 666f 7220 726f 775f 696e 6465 7820    for row_index 
+00000a70: 696e 2072 616e 6765 286c 656e 2870 6c61  in range(len(pla
+00000a80: 7965 725f 7374 6174 735f 6d61 7472 6978  yer_stats_matrix
+00000a90: 2929 3a0d 0a20 2020 2020 2020 2020 2020  )):..           
+00000aa0: 2023 2063 6865 636b 2069 6620 7468 6520   # check if the 
+00000ab0: 726f 7720 6973 2065 6d70 7479 0d0a 2020  row is empty..  
+00000ac0: 2020 2020 2020 2020 2020 6966 2070 6c61            if pla
+00000ad0: 7965 725f 7374 6174 735f 6d61 7472 6978  yer_stats_matrix
+00000ae0: 5b72 6f77 5f69 6e64 6578 5d20 213d 205b  [row_index] != [
+00000af0: 5d3a 0d0a 2020 2020 2020 2020 2020 2020  ]:..            
+00000b00: 2020 2020 2320 4368 6563 6b20 6c61 7374      # Check last
+00000b10: 2063 6f6c 756d 6e20 746f 2073 6565 2069   column to see i
+00000b20: 6620 706c 6179 6572 2070 6c61 7965 6420  f player played 
+00000b30: 696e 2074 6865 2067 616d 650d 0a20 2020  in the game..   
+00000b40: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00000b50: 2822 2b22 206e 6f74 2069 6e20 706c 6179  ("+" not in play
+00000b60: 6572 5f73 7461 7473 5f6d 6174 7269 785b  er_stats_matrix[
+00000b70: 726f 775f 696e 6465 785d 5b2d 315d 2920  row_index][-1]) 
+00000b80: 616e 6420 2822 2d22 206e 6f74 2069 6e20  and ("-" not in 
+00000b90: 706c 6179 6572 5f73 7461 7473 5f6d 6174  player_stats_mat
+00000ba0: 7269 785b 726f 775f 696e 6465 785d 5b2d  rix[row_index][-
+00000bb0: 315d 293a 0d0a 2020 2020 2020 2020 2020  1]):..          
+00000bc0: 2020 2020 2020 2020 2020 2320 6765 7420            # get 
+00000bd0: 7468 6520 6469 6666 6572 656e 6365 2069  the difference i
+00000be0: 6e20 6c65 6e67 7468 2062 6574 7765 656e  n length between
+00000bf0: 2074 6865 2068 6561 6465 7273 2061 6e64   the headers and
+00000c00: 2074 6865 2072 6f77 0d0a 2020 2020 2020   the row..      
+00000c10: 2020 2020 2020 2020 2020 2020 2020 726f                ro
+00000c20: 775f 6469 6666 203d 206c 656e 2868 6561  w_diff = len(hea
+00000c30: 6465 7273 2920 2d20 6c65 6e28 706c 6179  ders) - len(play
 00000c40: 6572 5f73 7461 7473 5f6d 6174 7269 785b  er_stats_matrix[
-00000c50: 726f 775f 696e 6465 785d 2074 6f20 7468  row_index] to th
-00000c60: 6520 656e 6420 6f66 2074 6865 206c 6973  e end of the lis
-00000c70: 7420 726f 775f 6469 6666 2074 696d 6573  t row_diff times
-00000c80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000c90: 2020 2020 2070 6c61 7965 725f 7374 6174       player_stat
-00000ca0: 735f 6d61 7472 6978 5b72 6f77 5f69 6e64  s_matrix[row_ind
-00000cb0: 6578 5d20 3d20 706c 6179 6572 5f73 7461  ex] = player_sta
-00000cc0: 7473 5f6d 6174 7269 785b 726f 775f 696e  ts_matrix[row_in
-00000cd0: 6465 785d 202b 205b 706c 6179 6572 5f73  dex] + [player_s
-00000ce0: 7461 7473 5f6d 6174 7269 785b 726f 775f  tats_matrix[row_
-00000cf0: 696e 6465 785d 5b2d 315d 5d20 2a20 726f  index][-1]] * ro
-00000d00: 775f 6469 6666 0a20 2020 2020 2020 2020  w_diff.         
-00000d10: 2020 2020 2020 2023 2069 7465 7261 7465         # iterate
-00000d20: 2074 6872 6f75 6768 2065 6163 6820 636f   through each co
-00000d30: 6c75 6d6e 0a20 2020 2020 2020 2020 2020  lumn.           
-00000d40: 2020 2020 2066 6f72 2068 6561 6465 725f       for header_
-00000d50: 696e 6465 7820 696e 2072 616e 6765 286c  index in range(l
-00000d60: 656e 2868 6561 6465 7273 2929 3a0a 2020  en(headers)):.  
-00000d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d80: 2020 2320 4368 6563 6b20 6966 2077 6520    # Check if we 
-00000d90: 6172 6520 696e 2074 6865 2048 6f6d 2f41  are in the Hom/A
-00000da0: 7761 7920 636f 6c75 6d6e 2061 6e64 2073  way column and s
-00000db0: 6574 2074 6865 2072 6967 6874 2068 6561  et the right hea
-00000dc0: 6465 720a 2020 2020 2020 2020 2020 2020  der.            
-00000dd0: 2020 2020 2020 2020 6966 2028 6865 6164          if (head
-00000de0: 6572 735b 6865 6164 6572 5f69 6e64 6578  ers[header_index
-00000df0: 2d31 5d20 3d3d 2022 546d 2229 2061 6e64  -1] == "Tm") and
-00000e00: 2028 6865 6164 6572 735b 6865 6164 6572   (headers[header
-00000e10: 5f69 6e64 6578 2b31 5d20 3d3d 2022 4f70  _index+1] == "Op
-00000e20: 7022 293a 0a20 2020 2020 2020 2020 2020  p"):.           
-00000e30: 2020 2020 2020 2020 2020 2020 2068 6561               hea
-00000e40: 6465 7273 5b68 6561 6465 725f 696e 6465  ders[header_inde
-00000e50: 785d 203d 2022 486f 6d65 2f41 7761 7922  x] = "Home/Away"
-00000e60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000e70: 2020 2020 2020 2020 2023 2073 6574 2074           # set t
-00000e80: 6865 206e 6577 2076 616c 7565 2074 6f20  he new value to 
-00000e90: 486f 6d65 206f 7220 4177 6179 0a20 2020  Home or Away.   
-00000ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000eb0: 2020 2020 2069 6620 2240 2220 696e 2070       if "@" in p
-00000ec0: 6c61 7965 725f 7374 6174 735f 6d61 7472  layer_stats_matr
-00000ed0: 6978 5b72 6f77 5f69 6e64 6578 5d5b 6865  ix[row_index][he
-00000ee0: 6164 6572 5f69 6e64 6578 5d3a 0a20 2020  ader_index]:.   
-00000ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f00: 2020 2020 2020 2020 2070 6c61 7965 725f           player_
-00000f10: 7374 6174 735f 6d61 7472 6978 5b72 6f77  stats_matrix[row
-00000f20: 5f69 6e64 6578 5d5b 6865 6164 6572 5f69  _index][header_i
-00000f30: 6e64 6578 5d20 3d20 2241 7761 7922 0a20  ndex] = "Away". 
-00000f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f50: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00000f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f70: 2020 2020 2020 2020 2070 6c61 7965 725f           player_
-00000f80: 7374 6174 735f 6d61 7472 6978 5b72 6f77  stats_matrix[row
-00000f90: 5f69 6e64 6578 5d5b 6865 6164 6572 5f69  _index][header_i
-00000fa0: 6e64 6578 5d20 3d20 2248 6f6d 6522 0a20  ndex] = "Home". 
-00000fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000fc0: 2020 2023 2043 6865 636b 2069 6620 7765     # Check if we
-00000fd0: 2061 7265 2069 6e20 7468 6520 572f 4c20   are in the W/L 
-00000fe0: 636f 6c75 6d6e 2061 6e64 2073 6574 2074  column and set t
-00000ff0: 6865 2072 6967 6874 2068 6561 6465 7220  he right header 
-00001000: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00001010: 2020 2020 2020 2020 2020 2020 6966 2028              if (
-00001020: 6865 6164 6572 735b 6865 6164 6572 5f69  headers[header_i
-00001030: 6e64 6578 2d31 5d20 3d3d 2022 4f70 7022  ndex-1] == "Opp"
-00001040: 2920 616e 6420 2868 6561 6465 7273 5b68  ) and (headers[h
-00001050: 6561 6465 725f 696e 6465 782b 315d 203d  eader_index+1] =
-00001060: 3d20 2247 5322 293a 0a20 2020 2020 2020  = "GS"):.       
-00001070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001080: 2023 2073 6574 2074 6865 206e 6577 2068   # set the new h
-00001090: 6561 6465 720a 2020 2020 2020 2020 2020  eader.          
-000010a0: 2020 2020 2020 2020 2020 2020 2020 6865                he
-000010b0: 6164 6572 735b 6865 6164 6572 5f69 6e64  aders[header_ind
-000010c0: 6578 5d20 3d20 2257 2f4c 220a 2020 2020  ex] = "W/L".    
-000010d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000010e0: 2320 7365 7420 7468 6520 6b65 7920 696e  # set the key in
-000010f0: 2074 6865 2064 6963 7469 6f6e 6172 7920   the dictionary 
-00001100: 6966 2069 7420 646f 6573 6e27 7420 6578  if it doesn't ex
-00001110: 6973 740a 2020 2020 2020 2020 2020 2020  ist.            
-00001120: 2020 2020 2020 2020 6966 2073 7461 7473          if stats
-00001130: 5f64 6963 742e 6765 7428 6865 6164 6572  _dict.get(header
-00001140: 735b 6865 6164 6572 5f69 6e64 6578 5d29  s[header_index])
-00001150: 203d 3d20 4e6f 6e65 3a0a 2020 2020 2020   == None:.      
-00001160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001170: 2020 7374 6174 735f 6469 6374 5b68 6561    stats_dict[hea
-00001180: 6465 7273 5b68 6561 6465 725f 696e 6465  ders[header_inde
-00001190: 785d 5d20 3d20 5b5d 0a20 2020 2020 2020  x]] = [].       
-000011a0: 2020 2020 2020 2020 2020 2020 2023 2061               # a
-000011b0: 7070 656e 6420 7468 6520 7661 6c75 6520  ppend the value 
-000011c0: 746f 2074 6865 2064 6963 7469 6f6e 6172  to the dictionar
-000011d0: 790a 2020 2020 2020 2020 2020 2020 2020  y.              
-000011e0: 2020 2020 2020 7374 6174 735f 6469 6374        stats_dict
-000011f0: 5b68 6561 6465 7273 5b68 6561 6465 725f  [headers[header_
-00001200: 696e 6465 785d 5d2e 6170 7065 6e64 2870  index]].append(p
-00001210: 6c61 7965 725f 7374 6174 735f 6d61 7472  layer_stats_matr
-00001220: 6978 5b72 6f77 5f69 6e64 6578 5d5b 6865  ix[row_index][he
-00001230: 6164 6572 5f69 6e64 6578 5d29 0a0a 2020  ader_index])..  
-00001240: 2020 2020 2020 2320 4372 6561 7465 2061        # Create a
-00001250: 2064 6174 6166 7261 6d65 0a20 2020 2020   dataframe.     
-00001260: 2020 2073 7461 7473 5f64 6620 3d20 7064     stats_df = pd
-00001270: 2e44 6174 6146 7261 6d65 2873 7461 7473  .DataFrame(stats
-00001280: 5f64 6963 7429 0a0a 2020 2020 2020 2020  _dict)..        
-00001290: 2320 5265 7475 726e 2074 6865 2073 7461  # Return the sta
-000012a0: 7473 0a20 2020 2020 2020 2072 6574 7572  ts.        retur
-000012b0: 6e20 7b22 706c 6179 6572 5f73 7461 7473  n {"player_stats
-000012c0: 5f6d 6174 7269 7822 3a20 706c 6179 6572  _matrix": player
-000012d0: 5f73 7461 7473 5f6d 6174 7269 782c 2022  _stats_matrix, "
-000012e0: 7374 6174 735f 6469 6374 223a 2073 7461  stats_dict": sta
-000012f0: 7473 5f64 6963 742c 2022 7374 6174 735f  ts_dict, "stats_
-00001300: 6466 223a 2073 7461 7473 5f64 667d       df": stats_df}
+00000c50: 726f 775f 696e 6465 785d 290d 0a20 2020  row_index])..   
+00000c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c70: 2023 2061 7070 656e 6469 6e67 206c 6173   # appending las
+00000c80: 7420 7661 6c75 6520 6f66 2070 6c61 7965  t value of playe
+00000c90: 725f 7374 6174 735f 6d61 7472 6978 5b72  r_stats_matrix[r
+00000ca0: 6f77 5f69 6e64 6578 5d20 746f 2074 6865  ow_index] to the
+00000cb0: 2065 6e64 206f 6620 7468 6520 6c69 7374   end of the list
+00000cc0: 2072 6f77 5f64 6966 6620 7469 6d65 730d   row_diff times.
+00000cd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000ce0: 2020 2020 2070 6c61 7965 725f 7374 6174       player_stat
+00000cf0: 735f 6d61 7472 6978 5b72 6f77 5f69 6e64  s_matrix[row_ind
+00000d00: 6578 5d20 3d20 706c 6179 6572 5f73 7461  ex] = player_sta
+00000d10: 7473 5f6d 6174 7269 785b 726f 775f 696e  ts_matrix[row_in
+00000d20: 6465 785d 202b 205b 706c 6179 6572 5f73  dex] + [player_s
+00000d30: 7461 7473 5f6d 6174 7269 785b 726f 775f  tats_matrix[row_
+00000d40: 696e 6465 785d 5b2d 315d 5d20 2a20 726f  index][-1]] * ro
+00000d50: 775f 6469 6666 0d0a 2020 2020 2020 2020  w_diff..        
+00000d60: 2020 2020 2020 2020 2320 6974 6572 6174          # iterat
+00000d70: 6520 7468 726f 7567 6820 6561 6368 2063  e through each c
+00000d80: 6f6c 756d 6e0d 0a20 2020 2020 2020 2020  olumn..         
+00000d90: 2020 2020 2020 2066 6f72 2068 6561 6465         for heade
+00000da0: 725f 696e 6465 7820 696e 2072 616e 6765  r_index in range
+00000db0: 286c 656e 2868 6561 6465 7273 2929 3a0d  (len(headers)):.
+00000dc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000dd0: 2020 2020 2023 2043 6865 636b 2069 6620       # Check if 
+00000de0: 7765 2061 7265 2069 6e20 7468 6520 486f  we are in the Ho
+00000df0: 6d2f 4177 6179 2063 6f6c 756d 6e20 616e  m/Away column an
+00000e00: 6420 7365 7420 7468 6520 7269 6768 7420  d set the right 
+00000e10: 6865 6164 6572 0d0a 2020 2020 2020 2020  header..        
+00000e20: 2020 2020 2020 2020 2020 2020 6966 2028              if (
+00000e30: 6865 6164 6572 735b 6865 6164 6572 5f69  headers[header_i
+00000e40: 6e64 6578 2d31 5d20 3d3d 2022 546d 2229  ndex-1] == "Tm")
+00000e50: 2061 6e64 2028 6865 6164 6572 735b 6865   and (headers[he
+00000e60: 6164 6572 5f69 6e64 6578 2b31 5d20 3d3d  ader_index+1] ==
+00000e70: 2022 4f70 7022 293a 0d0a 2020 2020 2020   "Opp"):..      
+00000e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e90: 2020 6865 6164 6572 735b 6865 6164 6572    headers[header
+00000ea0: 5f69 6e64 6578 5d20 3d20 2248 6f6d 652f  _index] = "Home/
+00000eb0: 4177 6179 220d 0a20 2020 2020 2020 2020  Away"..         
+00000ec0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00000ed0: 2073 6574 2074 6865 206e 6577 2076 616c   set the new val
+00000ee0: 7565 2074 6f20 486f 6d65 206f 7220 4177  ue to Home or Aw
+00000ef0: 6179 0d0a 2020 2020 2020 2020 2020 2020  ay..            
+00000f00: 2020 2020 2020 2020 2020 2020 6966 2022              if "
+00000f10: 4022 2069 6e20 706c 6179 6572 5f73 7461  @" in player_sta
+00000f20: 7473 5f6d 6174 7269 785b 726f 775f 696e  ts_matrix[row_in
+00000f30: 6465 785d 5b68 6561 6465 725f 696e 6465  dex][header_inde
+00000f40: 785d 3a0d 0a20 2020 2020 2020 2020 2020  x]:..           
+00000f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f60: 2070 6c61 7965 725f 7374 6174 735f 6d61   player_stats_ma
+00000f70: 7472 6978 5b72 6f77 5f69 6e64 6578 5d5b  trix[row_index][
+00000f80: 6865 6164 6572 5f69 6e64 6578 5d20 3d20  header_index] = 
+00000f90: 2241 7761 7922 0d0a 2020 2020 2020 2020  "Away"..        
+00000fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000fb0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+00000fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000fd0: 2020 2070 6c61 7965 725f 7374 6174 735f     player_stats_
+00000fe0: 6d61 7472 6978 5b72 6f77 5f69 6e64 6578  matrix[row_index
+00000ff0: 5d5b 6865 6164 6572 5f69 6e64 6578 5d20  ][header_index] 
+00001000: 3d20 2248 6f6d 6522 0d0a 2020 2020 2020  = "Home"..      
+00001010: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00001020: 4368 6563 6b20 6966 2077 6520 6172 6520  Check if we are 
+00001030: 696e 2074 6865 2057 2f4c 2063 6f6c 756d  in the W/L colum
+00001040: 6e20 616e 6420 7365 7420 7468 6520 7269  n and set the ri
+00001050: 6768 7420 6865 6164 6572 2020 2020 2020  ght header      
+00001060: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00001070: 2020 2020 2020 2020 6966 2028 6865 6164          if (head
+00001080: 6572 735b 6865 6164 6572 5f69 6e64 6578  ers[header_index
+00001090: 2d31 5d20 3d3d 2022 4f70 7022 2920 616e  -1] == "Opp") an
+000010a0: 6420 2868 6561 6465 7273 5b68 6561 6465  d (headers[heade
+000010b0: 725f 696e 6465 782b 315d 203d 3d20 2247  r_index+1] == "G
+000010c0: 5322 293a 0d0a 2020 2020 2020 2020 2020  S"):..          
+000010d0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+000010e0: 7365 7420 7468 6520 6e65 7720 6865 6164  set the new head
+000010f0: 6572 0d0a 2020 2020 2020 2020 2020 2020  er..            
+00001100: 2020 2020 2020 2020 2020 2020 6865 6164              head
+00001110: 6572 735b 6865 6164 6572 5f69 6e64 6578  ers[header_index
+00001120: 5d20 3d20 2257 2f4c 220d 0a20 2020 2020  ] = "W/L"..     
+00001130: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00001140: 2073 6574 2074 6865 206b 6579 2069 6e20   set the key in 
+00001150: 7468 6520 6469 6374 696f 6e61 7279 2069  the dictionary i
+00001160: 6620 6974 2064 6f65 736e 2774 2065 7869  f it doesn't exi
+00001170: 7374 0d0a 2020 2020 2020 2020 2020 2020  st..            
+00001180: 2020 2020 2020 2020 6966 2073 7461 7473          if stats
+00001190: 5f64 6963 742e 6765 7428 6865 6164 6572  _dict.get(header
+000011a0: 735b 6865 6164 6572 5f69 6e64 6578 5d29  s[header_index])
+000011b0: 203d 3d20 4e6f 6e65 3a0d 0a20 2020 2020   == None:..     
+000011c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000011d0: 2020 2073 7461 7473 5f64 6963 745b 6865     stats_dict[he
+000011e0: 6164 6572 735b 6865 6164 6572 5f69 6e64  aders[header_ind
+000011f0: 6578 5d5d 203d 205b 5d0d 0a20 2020 2020  ex]] = []..     
+00001200: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00001210: 2061 7070 656e 6420 7468 6520 7661 6c75   append the valu
+00001220: 6520 746f 2074 6865 2064 6963 7469 6f6e  e to the diction
+00001230: 6172 790d 0a20 2020 2020 2020 2020 2020  ary..           
+00001240: 2020 2020 2020 2020 2073 7461 7473 5f64           stats_d
+00001250: 6963 745b 6865 6164 6572 735b 6865 6164  ict[headers[head
+00001260: 6572 5f69 6e64 6578 5d5d 2e61 7070 656e  er_index]].appen
+00001270: 6428 706c 6179 6572 5f73 7461 7473 5f6d  d(player_stats_m
+00001280: 6174 7269 785b 726f 775f 696e 6465 785d  atrix[row_index]
+00001290: 5b68 6561 6465 725f 696e 6465 785d 290d  [header_index]).
+000012a0: 0a0d 0a20 2020 2020 2020 2023 2043 7265  ...        # Cre
+000012b0: 6174 6520 6120 6461 7461 6672 616d 650d  ate a dataframe.
+000012c0: 0a20 2020 2020 2020 2073 7461 7473 5f64  .        stats_d
+000012d0: 6620 3d20 7064 2e44 6174 6146 7261 6d65  f = pd.DataFrame
+000012e0: 2873 7461 7473 5f64 6963 7429 0d0a 0d0a  (stats_dict)....
+000012f0: 2020 2020 2020 2020 2320 5265 7475 726e          # Return
+00001300: 2074 6865 2073 7461 7473 0d0a 2020 2020   the stats..    
+00001310: 2020 2020 7265 7475 726e 207b 2270 6c61      return {"pla
+00001320: 7965 725f 7374 6174 735f 6d61 7472 6978  yer_stats_matrix
+00001330: 223a 2070 6c61 7965 725f 7374 6174 735f  ": player_stats_
+00001340: 6d61 7472 6978 2c20 2273 7461 7473 5f64  matrix, "stats_d
+00001350: 6963 7422 3a20 7374 6174 735f 6469 6374  ict": stats_dict
+00001360: 2c20 2273 7461 7473 5f64 6622 3a20 7374  , "stats_df": st
+00001370: 6174 735f 6466 7d                        ats_df}
```

### Comparing `SportStatIQ-DataCollectors-0.0.0/src/SportStatIQ_DataCollectors.egg-info/PKG-INFO` & `SportStatIQ-DataCollectors-1.0.3/src/SportStatIQ_DataCollectors.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-Metadata-Version: 2.1
-Name: SportStatIQ-DataCollectors
-Version: 0.0.0
-Summary: Collects data from various sports websites
-Home-page: https://github.com/SportStatIQ/SportStatIQ-DataCollectors
-Author: Matthew Myrick
-Author-email: MatthewMyrick2@gmail.com
-License: MIT
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Utilities
-Description-Content-Type: text/markdown
-
-# DataCollector
-
-This Python class provides a data collection functionality through the `NbaDataCollector` library.
-
-## Class: `DataCollector`
-
-### Initialization
-```python
-def __init__(self)
-```
-This function initializes the `DataCollector` class.
-
-### Method: `NbaDataCollector`
-```python
-def NbaDataCollector(self)
-```
-This function returns the `NbaDataCollector` library.
-
-Returns:
-- `NbaDataCollector`: The `NbaDataCollector` library.
-
-## Usage Example
-
-```python
-# Instantiate the DataCollector class
-collector = DataCollector()
-
-# Access the NbaDataCollector library
-nba_collector = collector.NbaDataCollector()
-
-# Use the NbaDataCollector library for data collection
-# ...
-```
-
-Please note that the `NbaDataCollector` library is not defined within the provided code snippet, and it is assumed to be a separate module or library that is imported by the `DataCollector` class. Make sure to import or define the `NbaDataCollector` library accordingly for the code to work properly.
+Metadata-Version: 2.1
+Name: SportStatIQ-DataCollectors
+Version: 1.0.3
+Summary: Collects data from various sports websites
+Home-page: https://github.com/SportStatIQ/SportStatIQ-DataCollectors
+Author: Matthew Myrick
+Author-email: MatthewMyrick2@gmail.com
+License: MIT
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Utilities
+Description-Content-Type: text/markdown
+
+# DataCollector
+
+This Python class provides a data collection functionality through the `NbaDataCollector` library.
+
+## Class: `DataCollector`
+
+### Initialization
+```python
+def __init__(self)
+```
+This function initializes the `DataCollector` class.
+
+### Method: `NbaDataCollector`
+```python
+def NbaDataCollector(self)
+```
+This function returns the `NbaDataCollector` library.
+
+Returns:
+- `NbaDataCollector`: The `NbaDataCollector` library.
+
+## Usage Example
+
+```python
+# Instantiate the DataCollector class
+collector = DataCollector()
+
+# Access the NbaDataCollector library
+nba_collector = collector.NbaDataCollector()
+
+# Use the NbaDataCollector library for data collection
+# ...
+```
+
+Please note that the `NbaDataCollector` library is not defined within the provided code snippet, and it is assumed to be a separate module or library that is imported by the `DataCollector` class. Make sure to import or define the `NbaDataCollector` library accordingly for the code to work properly.
```

### Comparing `SportStatIQ-DataCollectors-0.0.0/src/SportStatIQ_DataCollectors.egg-info/SOURCES.txt` & `SportStatIQ-DataCollectors-1.0.3/src/SportStatIQ_DataCollectors.egg-info/SOURCES.txt`

 * *Files identical despite different names*

