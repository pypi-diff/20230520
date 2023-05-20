# Comparing `tmp/geetiles-0.1.4.tar.gz` & `tmp/geetiles-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geetiles-0.1.4.tar", last modified: Sun Apr  9 18:47:40 2023, max compression
+gzip compressed data, was "geetiles-0.1.5.tar", last modified: Sat May 20 13:29:54 2023, max compression
```

## Comparing `geetiles-0.1.4.tar` & `geetiles-0.1.5.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxrwxr-x   0 rlx       (1000) rlx       (1000)        0 2023-04-09 18:47:40.617351 geetiles-0.1.4/
--rw-rw-r--   0 rlx       (1000) rlx       (1000)      104 2023-03-17 14:46:38.000000 geetiles-0.1.4/.gitignore
--rw-rw-r--   0 rlx       (1000) rlx       (1000)     1074 2023-03-17 14:46:38.000000 geetiles-0.1.4/LICENSE.txt
--rw-rw-r--   0 rlx       (1000) rlx       (1000)     6263 2023-04-09 18:47:40.617351 geetiles-0.1.4/PKG-INFO
--rw-rw-r--   0 rlx       (1000) rlx       (1000)     5967 2023-04-09 18:46:01.000000 geetiles-0.1.4/README.md
-drwxrwxr-x   0 rlx       (1000) rlx       (1000)        0 2023-04-09 18:47:40.557350 geetiles-0.1.4/data/
--rw-rw-r--   0 rlx       (1000) rlx       (1000)     1879 2023-03-21 14:53:07.000000 geetiles-0.1.4/data/luxembourg.README.txt
--rw-rw-r--   0 rlx       (1000) rlx       (1000)    13885 2023-03-17 14:46:38.000000 geetiles-0.1.4/data/luxembourg.wkt
-drwxrwxr-x   0 rlx       (1000) rlx       (1000)        0 2023-04-09 18:47:40.561350 geetiles-0.1.4/geetiles/
--rw-rw-r--   0 rlx       (1000) rlx       (1000)      220 2023-03-17 14:46:38.000000 geetiles-0.1.4/geetiles/__init__.py
--rw-rw-r--   0 rlx       (1000) rlx       (1000)    18581 2023-04-09 18:46:01.000000 geetiles-0.1.4/geetiles/cmds.py
-drwxrwxr-x   0 rlx       (1000) rlx       (1000)        0 2023-04-09 18:47:40.561350 geetiles-0.1.4/geetiles/defs/
--rw-rw-r--   0 rlx       (1000) rlx       (1000)      430 2023-04-09 18:46:01.000000 geetiles-0.1.4/geetiles/defs/esaworldcover.py
--rw-rw-r--   0 rlx       (1000) rlx       (1000)      983 2023-04-09 18:46:01.000000 geetiles-0.1.4/geetiles/defs/humanpop2015.py
--rw-rw-r--   0 rlx       (1000) rlx       (1000)     1064 2023-04-09 18:46:01.000000 geetiles-0.1.4/geetiles/defs/sentinel2rgbmedian2020.py
--rw-rw-r--   0 rlx       (1000) rlx       (1000)      438 2023-04-09 18:46:01.000000 geetiles-0.1.4/geetiles/defs/soilphbenelux.py
--rw-rw-r--   0 rlx       (1000) rlx       (1000)      417 2023-04-09 18:46:01.000000 geetiles-0.1.4/geetiles/defs/soilphcolombia.py
--rw-rw-r--   0 rlx       (1000) rlx       (1000)      659 2023-04-09 18:46:01.000000 geetiles-0.1.4/geetiles/defs/treecover2020.py
--rw-rw-r--   0 rlx       (1000) rlx       (1000)     9284 2023-03-19 04:44:24.000000 geetiles-0.1.4/geetiles/gee.py
--rw-rw-r--   0 rlx       (1000) rlx       (1000)    11745 2023-04-09 18:46:01.000000 geetiles-0.1.4/geetiles/main.py
--rw-rw-r--   0 rlx       (1000) rlx       (1000)    24339 2023-04-09 18:46:01.000000 geetiles-0.1.4/geetiles/partitions.py
--rw-rw-r--   0 rlx       (1000) rlx       (1000)     6889 2023-04-09 18:46:01.000000 geetiles-0.1.4/geetiles/utils.py
-drwxrwxr-x   0 rlx       (1000) rlx       (1000)        0 2023-04-09 18:47:40.561350 geetiles-0.1.4/geetiles.egg-info/
--rw-rw-r--   0 rlx       (1000) rlx       (1000)     6263 2023-04-09 18:47:40.000000 geetiles-0.1.4/geetiles.egg-info/PKG-INFO
--rw-rw-r--   0 rlx       (1000) rlx       (1000)      907 2023-04-09 18:47:40.000000 geetiles-0.1.4/geetiles.egg-info/SOURCES.txt
--rw-rw-r--   0 rlx       (1000) rlx       (1000)        1 2023-04-09 18:47:40.000000 geetiles-0.1.4/geetiles.egg-info/dependency_links.txt
--rw-rw-r--   0 rlx       (1000) rlx       (1000)       44 2023-04-09 18:47:40.000000 geetiles-0.1.4/geetiles.egg-info/entry_points.txt
--rw-rw-r--   0 rlx       (1000) rlx       (1000)        1 2023-03-17 14:51:57.000000 geetiles-0.1.4/geetiles.egg-info/not-zip-safe
--rw-rw-r--   0 rlx       (1000) rlx       (1000)       91 2023-04-09 18:47:40.000000 geetiles-0.1.4/geetiles.egg-info/requires.txt
--rw-rw-r--   0 rlx       (1000) rlx       (1000)        9 2023-04-09 18:47:40.000000 geetiles-0.1.4/geetiles.egg-info/top_level.txt
--rw-rw-r--   0 rlx       (1000) rlx       (1000)       56 2023-03-17 14:46:38.000000 geetiles-0.1.4/howto-publish.txt
-drwxrwxr-x   0 rlx       (1000) rlx       (1000)        0 2023-04-09 18:47:40.609351 geetiles-0.1.4/imgs/
--rw-rw-r--   0 rlx       (1000) rlx       (1000)    82153 2023-03-19 05:37:33.000000 geetiles-0.1.4/imgs/dataframe.png
--rw-rw-r--   0 rlx       (1000) rlx       (1000)   366561 2023-03-17 14:46:38.000000 geetiles-0.1.4/imgs/landcover.png
--rw-rw-r--   0 rlx       (1000) rlx       (1000)   310721 2023-03-19 05:20:29.000000 geetiles-0.1.4/imgs/luxembourg-bands-communes.png
--rw-rw-r--   0 rlx       (1000) rlx       (1000)   306508 2023-03-19 05:14:46.000000 geetiles-0.1.4/imgs/luxembourg-bands.png
--rw-r--r--   0 rlx       (1000) rlx       (1000)  1664553 2023-03-21 21:33:01.000000 geetiles-0.1.4/imgs/luxembourg-communes-random5k.png
--rw-rw-r--   0 rlx       (1000) rlx       (1000)   959795 2023-03-17 14:46:38.000000 geetiles-0.1.4/imgs/luxembourg-communes.png
--rw-rw-r--   0 rlx       (1000) rlx       (1000)   863339 2023-03-17 14:46:38.000000 geetiles-0.1.4/imgs/luxembourg-random-5k.png
--rw-r--r--   0 rlx       (1000) rlx       (1000)  1182265 2023-03-21 21:34:06.000000 geetiles-0.1.4/imgs/luxembourg-splits.png
--rw-rw-r--   0 rlx       (1000) rlx       (1000)  1642194 2023-03-17 14:46:38.000000 geetiles-0.1.4/imgs/luxgrid.png
--rw-rw-r--   0 rlx       (1000) rlx       (1000)  1287337 2023-03-17 14:46:38.000000 geetiles-0.1.4/imgs/sentinel2.png
--rw-rw-r--   0 rlx       (1000) rlx       (1000)      385 2023-04-09 18:47:40.617351 geetiles-0.1.4/setup.cfg
--rw-rw-r--   0 rlx       (1000) rlx       (1000)      713 2023-03-17 15:10:29.000000 geetiles-0.1.4/setup.py
+drwxrwxr-x   0 rlx       (1000) rlx       (1000)        0 2023-05-20 13:29:54.216657 geetiles-0.1.5/
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)      104 2023-03-17 14:46:38.000000 geetiles-0.1.5/.gitignore
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)     1074 2023-03-17 14:46:38.000000 geetiles-0.1.5/LICENSE.txt
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)     6263 2023-05-20 13:29:54.216657 geetiles-0.1.5/PKG-INFO
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)     5967 2023-04-09 18:46:01.000000 geetiles-0.1.5/README.md
+drwxrwxr-x   0 rlx       (1000) rlx       (1000)        0 2023-05-20 13:29:54.192657 geetiles-0.1.5/data/
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)     1879 2023-03-21 14:53:07.000000 geetiles-0.1.5/data/luxembourg.README.txt
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)    13885 2023-03-17 14:46:38.000000 geetiles-0.1.5/data/luxembourg.wkt
+drwxrwxr-x   0 rlx       (1000) rlx       (1000)        0 2023-05-20 13:29:54.196657 geetiles-0.1.5/geetiles/
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)      220 2023-03-17 14:46:38.000000 geetiles-0.1.5/geetiles/__init__.py
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)    18581 2023-04-09 18:46:01.000000 geetiles-0.1.5/geetiles/cmds.py
+drwxrwxr-x   0 rlx       (1000) rlx       (1000)        0 2023-05-20 13:29:54.196657 geetiles-0.1.5/geetiles/defs/
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)      419 2023-04-11 20:51:25.000000 geetiles-0.1.5/geetiles/defs/canadacrop2020.py
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)      430 2023-04-09 18:46:01.000000 geetiles-0.1.5/geetiles/defs/esaworldcover.py
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)      986 2023-04-20 14:25:47.000000 geetiles-0.1.5/geetiles/defs/humanpop2015.py
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)     1064 2023-04-09 18:46:01.000000 geetiles-0.1.5/geetiles/defs/sentinel2rgbmedian2020.py
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)      438 2023-04-09 18:46:01.000000 geetiles-0.1.5/geetiles/defs/soilphbenelux.py
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)      417 2023-04-09 18:46:01.000000 geetiles-0.1.5/geetiles/defs/soilphcolombia.py
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)      659 2023-04-09 18:46:01.000000 geetiles-0.1.5/geetiles/defs/treecover2020.py
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)     9284 2023-03-19 04:44:24.000000 geetiles-0.1.5/geetiles/gee.py
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)    11745 2023-04-09 18:46:01.000000 geetiles-0.1.5/geetiles/main.py
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)    24339 2023-04-09 18:46:01.000000 geetiles-0.1.5/geetiles/partitions.py
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)     6889 2023-04-09 18:46:01.000000 geetiles-0.1.5/geetiles/utils.py
+drwxrwxr-x   0 rlx       (1000) rlx       (1000)        0 2023-05-20 13:29:54.196657 geetiles-0.1.5/geetiles.egg-info/
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)     6263 2023-05-20 13:29:54.000000 geetiles-0.1.5/geetiles.egg-info/PKG-INFO
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)      939 2023-05-20 13:29:54.000000 geetiles-0.1.5/geetiles.egg-info/SOURCES.txt
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)        1 2023-05-20 13:29:54.000000 geetiles-0.1.5/geetiles.egg-info/dependency_links.txt
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)       44 2023-05-20 13:29:54.000000 geetiles-0.1.5/geetiles.egg-info/entry_points.txt
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)        1 2023-03-17 14:51:57.000000 geetiles-0.1.5/geetiles.egg-info/not-zip-safe
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)      113 2023-05-20 13:29:54.000000 geetiles-0.1.5/geetiles.egg-info/requires.txt
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)        9 2023-05-20 13:29:54.000000 geetiles-0.1.5/geetiles.egg-info/top_level.txt
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)      167 2023-05-20 13:28:02.000000 geetiles-0.1.5/howto-publish.txt
+drwxrwxr-x   0 rlx       (1000) rlx       (1000)        0 2023-05-20 13:29:54.212657 geetiles-0.1.5/imgs/
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)    82153 2023-03-19 05:37:33.000000 geetiles-0.1.5/imgs/dataframe.png
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)   366561 2023-03-17 14:46:38.000000 geetiles-0.1.5/imgs/landcover.png
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)   310721 2023-03-19 05:20:29.000000 geetiles-0.1.5/imgs/luxembourg-bands-communes.png
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)   306508 2023-03-19 05:14:46.000000 geetiles-0.1.5/imgs/luxembourg-bands.png
+-rw-r--r--   0 rlx       (1000) rlx       (1000)  1664553 2023-03-21 21:33:01.000000 geetiles-0.1.5/imgs/luxembourg-communes-random5k.png
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)   959795 2023-03-17 14:46:38.000000 geetiles-0.1.5/imgs/luxembourg-communes.png
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)   863339 2023-03-17 14:46:38.000000 geetiles-0.1.5/imgs/luxembourg-random-5k.png
+-rw-r--r--   0 rlx       (1000) rlx       (1000)  1182265 2023-03-21 21:34:06.000000 geetiles-0.1.5/imgs/luxembourg-splits.png
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)  1642194 2023-03-17 14:46:38.000000 geetiles-0.1.5/imgs/luxgrid.png
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)  1287337 2023-03-17 14:46:38.000000 geetiles-0.1.5/imgs/sentinel2.png
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)      385 2023-05-20 13:29:54.216657 geetiles-0.1.5/setup.cfg
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)      741 2023-05-20 13:23:32.000000 geetiles-0.1.5/setup.py
```

### Comparing `geetiles-0.1.4/LICENSE.txt` & `geetiles-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `geetiles-0.1.4/PKG-INFO` & `geetiles-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geetiles
-Version: 0.1.4
+Version: 0.1.5
 Summary: download Google Earth Engine datasets to tiles as geotiff arrays
 Home-page: https://github.com/rramosp/geetiles
 Author: raul ramos
 Author-email: raul.ramos@udea.edu.co
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `geetiles-0.1.4/README.md` & `geetiles-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `geetiles-0.1.4/data/luxembourg.README.txt` & `geetiles-0.1.5/data/luxembourg.README.txt`

 * *Files identical despite different names*

### Comparing `geetiles-0.1.4/data/luxembourg.wkt` & `geetiles-0.1.5/data/luxembourg.wkt`

 * *Files identical despite different names*

### Comparing `geetiles-0.1.4/geetiles/cmds.py` & `geetiles-0.1.5/geetiles/cmds.py`

 * *Files identical despite different names*

### Comparing `geetiles-0.1.4/geetiles/defs/humanpop2015.py` & `geetiles-0.1.5/geetiles/defs/humanpop2015.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,12 +19,12 @@
     def map_values(self, array):
         return utils.apply_range_map(array, list(range(1,300,10)))
 
     def get_dtype(self):
         return 'uint16'
 
     def include_chip_in_dataset(self, chip_dict):
-        cprops = chip_dict['label_proportions']['partitions_aschip']
-        if '0' in cprops.keys() and cprops['0']==1. and np.random.random()>0.01:
-            return False
+        #cprops = chip_dict['label_proportions']['partitions_aschip']
+        #if '0' in cprops.keys() and cprops['0']==1. and np.random.random()>0.01:
+        #    return False
         
         return True
```

### Comparing `geetiles-0.1.4/geetiles/defs/sentinel2rgbmedian2020.py` & `geetiles-0.1.5/geetiles/defs/sentinel2rgbmedian2020.py`

 * *Files identical despite different names*

### Comparing `geetiles-0.1.4/geetiles/defs/treecover2020.py` & `geetiles-0.1.5/geetiles/defs/treecover2020.py`

 * *Files identical despite different names*

### Comparing `geetiles-0.1.4/geetiles/gee.py` & `geetiles-0.1.5/geetiles/gee.py`

 * *Files identical despite different names*

### Comparing `geetiles-0.1.4/geetiles/main.py` & `geetiles-0.1.5/geetiles/main.py`

 * *Files identical despite different names*

### Comparing `geetiles-0.1.4/geetiles/partitions.py` & `geetiles-0.1.5/geetiles/partitions.py`

 * *Files identical despite different names*

### Comparing `geetiles-0.1.4/geetiles/utils.py` & `geetiles-0.1.5/geetiles/utils.py`

 * *Files identical despite different names*

### Comparing `geetiles-0.1.4/geetiles.egg-info/PKG-INFO` & `geetiles-0.1.5/geetiles.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geetiles
-Version: 0.1.4
+Version: 0.1.5
 Summary: download Google Earth Engine datasets to tiles as geotiff arrays
 Home-page: https://github.com/rramosp/geetiles
 Author: raul ramos
 Author-email: raul.ramos@udea.edu.co
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `geetiles-0.1.4/geetiles.egg-info/SOURCES.txt` & `geetiles-0.1.5/geetiles.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 geetiles.egg-info/PKG-INFO
 geetiles.egg-info/SOURCES.txt
 geetiles.egg-info/dependency_links.txt
 geetiles.egg-info/entry_points.txt
 geetiles.egg-info/not-zip-safe
 geetiles.egg-info/requires.txt
 geetiles.egg-info/top_level.txt
+geetiles/defs/canadacrop2020.py
 geetiles/defs/esaworldcover.py
 geetiles/defs/humanpop2015.py
 geetiles/defs/sentinel2rgbmedian2020.py
 geetiles/defs/soilphbenelux.py
 geetiles/defs/soilphcolombia.py
 geetiles/defs/treecover2020.py
 imgs/dataframe.png
```

### Comparing `geetiles-0.1.4/imgs/dataframe.png` & `geetiles-0.1.5/imgs/dataframe.png`

 * *Files identical despite different names*

### Comparing `geetiles-0.1.4/imgs/landcover.png` & `geetiles-0.1.5/imgs/landcover.png`

 * *Files identical despite different names*

### Comparing `geetiles-0.1.4/imgs/luxembourg-bands-communes.png` & `geetiles-0.1.5/imgs/luxembourg-bands-communes.png`

 * *Files identical despite different names*

### Comparing `geetiles-0.1.4/imgs/luxembourg-bands.png` & `geetiles-0.1.5/imgs/luxembourg-bands.png`

 * *Files identical despite different names*

### Comparing `geetiles-0.1.4/imgs/luxembourg-communes-random5k.png` & `geetiles-0.1.5/imgs/luxembourg-communes-random5k.png`

 * *Files identical despite different names*

### Comparing `geetiles-0.1.4/imgs/luxembourg-communes.png` & `geetiles-0.1.5/imgs/luxembourg-communes.png`

 * *Files identical despite different names*

### Comparing `geetiles-0.1.4/imgs/luxembourg-random-5k.png` & `geetiles-0.1.5/imgs/luxembourg-random-5k.png`

 * *Files identical despite different names*

### Comparing `geetiles-0.1.4/imgs/luxembourg-splits.png` & `geetiles-0.1.5/imgs/luxembourg-splits.png`

 * *Files identical despite different names*

### Comparing `geetiles-0.1.4/imgs/luxgrid.png` & `geetiles-0.1.5/imgs/luxgrid.png`

 * *Files identical despite different names*

### Comparing `geetiles-0.1.4/imgs/sentinel2.png` & `geetiles-0.1.5/imgs/sentinel2.png`

 * *Files identical despite different names*

### Comparing `geetiles-0.1.4/setup.py` & `geetiles-0.1.5/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 setup(name='geetiles',
       description="download Google Earth Engine datasets to tiles as geotiff arrays",
       long_description_content_type='text/markdown',
       install_requires=['matplotlib','numpy', 'pandas','joblib',
                         'progressbar2', 'psutil', 'scipy', 'shapely',
-                        'geopandas', 'pyproj', 'rasterio'
+                        'geopandas', 'pyproj', 'rasterio', 'retry', 'earthengine-api'
                        ],
       use_scm_version=True,
       setup_requires=['setuptools_scm'],
       scripts=[],
       entry_points={
             "console_scripts": [
                   "geet = geetiles.main:main",
```

