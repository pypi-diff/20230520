# Comparing `tmp/redfin-scraper-0.1.6.tar.gz` & `tmp/redfin-scraper-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redfin-scraper-0.1.6.tar", last modified: Sun May  7 02:04:44 2023, max compression
+gzip compressed data, was "redfin-scraper-0.2.0.tar", last modified: Sat May 20 17:18:43 2023, max compression
```

## Comparing `redfin-scraper-0.1.6.tar` & `redfin-scraper-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 02:04:44.696170 redfin-scraper-0.1.6/
--rw-rw-rw-   0        0        0     1087 2023-03-18 00:15:21.000000 redfin-scraper-0.1.6/LICENSE.txt
--rw-rw-rw-   0        0        0     4020 2023-05-07 02:04:44.693164 redfin-scraper-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     2154 2023-04-04 15:15:03.000000 redfin-scraper-0.1.6/README.md
--rw-rw-rw-   0        0        0      904 2023-05-07 02:02:00.000000 redfin-scraper-0.1.6/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-07 02:04:44.668989 redfin-scraper-0.1.6/redfin_scraper/
--rw-rw-rw-   0        0        0      120 2023-05-07 02:02:53.000000 redfin-scraper-0.1.6/redfin_scraper/__init__.py
--rw-rw-rw-   0        0        0      325 2023-03-18 17:58:54.000000 redfin-scraper-0.1.6/redfin_scraper/config.py
-drwxrwxrwx   0        0        0        0 2023-05-07 02:04:44.688654 redfin-scraper-0.1.6/redfin_scraper/core/
--rw-rw-rw-   0        0        0        0 2023-03-11 03:00:34.000000 redfin-scraper-0.1.6/redfin_scraper/core/__init__.py
--rw-rw-rw-   0        0        0    11388 2023-05-07 01:57:33.000000 redfin-scraper-0.1.6/redfin_scraper/core/redfin_scraper.py
-drwxrwxrwx   0        0        0        0 2023-05-07 02:04:44.692162 redfin-scraper-0.1.6/redfin_scraper/resources/
--rw-rw-rw-   0        0        0        0 2023-02-25 20:03:01.000000 redfin-scraper-0.1.6/redfin_scraper/resources/__init__.py
--rw-rw-rw-   0        0        0     1116 2023-03-11 03:00:17.000000 redfin-scraper-0.1.6/redfin_scraper/resources/json_tools.py
--rw-rw-rw-   0        0        0     2462 2023-04-04 15:04:28.000000 redfin-scraper-0.1.6/redfin_scraper/resources/logging.py
-drwxrwxrwx   0        0        0        0 2023-05-07 02:04:44.686656 redfin-scraper-0.1.6/redfin_scraper.egg-info/
--rw-rw-rw-   0        0        0     4020 2023-05-07 02:04:44.000000 redfin-scraper-0.1.6/redfin_scraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      459 2023-05-07 02:04:44.000000 redfin-scraper-0.1.6/redfin_scraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 02:04:44.000000 redfin-scraper-0.1.6/redfin_scraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-05-07 02:04:44.000000 redfin-scraper-0.1.6/redfin_scraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-07 02:04:44.000000 redfin-scraper-0.1.6/redfin_scraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-07 02:04:44.696170 redfin-scraper-0.1.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-20 17:18:43.846596 redfin-scraper-0.2.0/
+-rw-rw-rw-   0        0        0     1087 2023-03-18 00:15:21.000000 redfin-scraper-0.2.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     4232 2023-05-20 17:18:43.845597 redfin-scraper-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2366 2023-05-20 17:17:34.000000 redfin-scraper-0.2.0/README.md
+-rw-rw-rw-   0        0        0      904 2023-05-20 17:02:08.000000 redfin-scraper-0.2.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-20 17:18:43.816437 redfin-scraper-0.2.0/redfin_scraper/
+-rw-rw-rw-   0        0        0      120 2023-05-20 17:02:04.000000 redfin-scraper-0.2.0/redfin_scraper/__init__.py
+-rw-rw-rw-   0        0        0      381 2023-05-20 17:01:49.000000 redfin-scraper-0.2.0/redfin_scraper/config.py
+drwxrwxrwx   0        0        0        0 2023-05-20 17:18:43.839595 redfin-scraper-0.2.0/redfin_scraper/core/
+-rw-rw-rw-   0        0        0        0 2023-03-11 03:00:34.000000 redfin-scraper-0.2.0/redfin_scraper/core/__init__.py
+-rw-rw-rw-   0        0        0    12326 2023-05-20 17:01:58.000000 redfin-scraper-0.2.0/redfin_scraper/core/redfin_scraper.py
+drwxrwxrwx   0        0        0        0 2023-05-20 17:18:43.844596 redfin-scraper-0.2.0/redfin_scraper/resources/
+-rw-rw-rw-   0        0        0        0 2023-02-25 20:03:01.000000 redfin-scraper-0.2.0/redfin_scraper/resources/__init__.py
+-rw-rw-rw-   0        0        0     1116 2023-03-11 03:00:17.000000 redfin-scraper-0.2.0/redfin_scraper/resources/json_tools.py
+-rw-rw-rw-   0        0        0     2462 2023-04-04 15:04:28.000000 redfin-scraper-0.2.0/redfin_scraper/resources/logging.py
+drwxrwxrwx   0        0        0        0 2023-05-20 17:18:43.835589 redfin-scraper-0.2.0/redfin_scraper.egg-info/
+-rw-rw-rw-   0        0        0     4232 2023-05-20 17:18:43.000000 redfin-scraper-0.2.0/redfin_scraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      459 2023-05-20 17:18:43.000000 redfin-scraper-0.2.0/redfin_scraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 17:18:43.000000 redfin-scraper-0.2.0/redfin_scraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-05-20 17:18:43.000000 redfin-scraper-0.2.0/redfin_scraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-20 17:18:43.000000 redfin-scraper-0.2.0/redfin_scraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-20 17:18:43.847596 redfin-scraper-0.2.0/setup.cfg
```

### Comparing `redfin-scraper-0.1.6/LICENSE.txt` & `redfin-scraper-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `redfin-scraper-0.1.6/PKG-INFO` & `redfin-scraper-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redfin-scraper
-Version: 0.1.6
+Version: 0.2.0
 Summary: A Python library used to scrape data from Redfin.com using the unofficial Stringray API.
 Author-email: Ryan Sherby <ryan.m.sherby@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Ryan Sherby
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -59,26 +59,30 @@
 `from redfin_scraper import RedfinScraper`  
 
 ### Initialize Module
 `scraper = RedfinScraper()`
 
 ## Using The Scraper
 ### Required Setup
-`scraper.setup(zip_database_path:str,multiprocessing:bool=False)`
+`scraper.setup(zip_database_path:str, multiprocessing:bool=False)`
 
 > **zip_database_path**: Binary path to the zip_code_database.csv  
 
 > **multiprocessing**: Allow for multiprocessing
 
 ### Activating The Scraper
-`scraper.scrape(city_states:list[str]=None,zip_codes:list[str],lat_tuner:float=1.5,lon_tuner:float=1.5)`
+`scraper.scrape(city_states:list[str]=None, zip_codes:list[str], sold:bool=False, sale_period:str=None, lat_tuner:float=1.5, lon_tuner:float=1.5)`
 >**city_states**: List of strings representing US cities formatted as "City, State"  
 
 >**zip_codes**: List of strings representing US zip codes  
 
+>**sold**: Select whether to scrape for-sale data (default) or sold data  
+
+>**sale_period**: Must be selected whenever sold is True (1mo, 3mo, 6mo, 1yr, 3yr, 5yr)
+
 >**lat_tuner**: Represents # of standard deviations beyond the local latitude average that a zip code may exist within   
 
 >**lon_tuner**: Represents # of standard deviations beyond the local longitude average that a zip code may exist within  
 
 ### Accessing Prior Scrapes
 `scraper.get_data(id:str)`
 >**id**: IDs are indexed at 1 and increase in the format "D00#"
```

### Comparing `redfin-scraper-0.1.6/README.md` & `redfin-scraper-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -23,26 +23,30 @@
 `from redfin_scraper import RedfinScraper`  
 
 ### Initialize Module
 `scraper = RedfinScraper()`
 
 ## Using The Scraper
 ### Required Setup
-`scraper.setup(zip_database_path:str,multiprocessing:bool=False)`
+`scraper.setup(zip_database_path:str, multiprocessing:bool=False)`
 
 > **zip_database_path**: Binary path to the zip_code_database.csv  
 
 > **multiprocessing**: Allow for multiprocessing
 
 ### Activating The Scraper
-`scraper.scrape(city_states:list[str]=None,zip_codes:list[str],lat_tuner:float=1.5,lon_tuner:float=1.5)`
+`scraper.scrape(city_states:list[str]=None, zip_codes:list[str], sold:bool=False, sale_period:str=None, lat_tuner:float=1.5, lon_tuner:float=1.5)`
 >**city_states**: List of strings representing US cities formatted as "City, State"  
 
 >**zip_codes**: List of strings representing US zip codes  
 
+>**sold**: Select whether to scrape for-sale data (default) or sold data  
+
+>**sale_period**: Must be selected whenever sold is True (1mo, 3mo, 6mo, 1yr, 3yr, 5yr)
+
 >**lat_tuner**: Represents # of standard deviations beyond the local latitude average that a zip code may exist within   
 
 >**lon_tuner**: Represents # of standard deviations beyond the local longitude average that a zip code may exist within  
 
 ### Accessing Prior Scrapes
 `scraper.get_data(id:str)`
 >**id**: IDs are indexed at 1 and increase in the format "D00#"
```

### Comparing `redfin-scraper-0.1.6/pyproject.toml` & `redfin-scraper-0.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "redfin-scraper"
-version = "0.1.6"
+version = "0.2.0"
 description = "A Python library used to scrape data from Redfin.com using the unofficial Stringray API."
 readme = "README.md"
 authors = [{ name = "Ryan Sherby", email = "ryan.m.sherby@gmail.com" }]
 license = { file = "LICENSE.txt" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `redfin-scraper-0.1.6/redfin_scraper/core/redfin_scraper.py` & `redfin-scraper-0.2.0/redfin_scraper/core/redfin_scraper.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,16 +103,33 @@
 
 
 
 
     @rsrl.timing_log
     def scrape(self,city_states:list[str]=rsrj.get_config_value('city_states'),
                zip_codes:list[str]=rsrj.get_config_value('zip_codes'),
+               sold:bool=rsrj.get_config_value('sold'),
+               sale_period:str=rsrj.get_config_value('sale_period'),
                lat_tuner:float=rsrj.get_config_value('lat_tuner'),
                lon_tuner:float=rsrj.get_config_value('lon_tuner')):
+        
+        
+        
+        self._sold=False
+        
+        if sold=='True' or sold=='true' or sold == True:
+            self._sold=True
+            
+        self._sale_period=sale_period
+        
+        if(self._sold):
+            if self._sale_period not in ('1mo','3mo','6mo','1yr','2yr','3yr','5yr'):
+                raise ValueError("Sale Period must be '1mo','3mo','6mo','1yr','2yr','3yr','5yr' if Sold selected.")
+            
+            
     
 
         if lat_tuner==None:
             lat_tuner=rsc.DEFAULT_TUNER_VARIABLE
         if lon_tuner==None:
             lon_tuner=rsc.DEFAULT_TUNER_VARIABLE
 
@@ -310,19 +327,26 @@
 
 
 
 
 
     def _generate_urls(self,**kwargs):
         urls=[]
-        try:
-            for zip in kwargs['zip_codes']:
-                urls.append(rsc.REDFIN_URL.format(rsc.REDFIN_ZIP_URL.format(zip_code=zip)))
-        except:
-            pass
+        if(self._sold):
+            try:
+                for zip in kwargs['zip_codes']:
+                    urls.append(rsc.REDFIN_URL.format(rsc.REDFIN_ZIP_URL.format(zip_code=zip))+rsc.REDFIN_FILTER_URL.format(sale_period=self._sale_period))
+            except:
+                pass
+        else:
+            try:
+                for zip in kwargs['zip_codes']:
+                    urls.append(rsc.REDFIN_URL.format(rsc.REDFIN_ZIP_URL.format(zip_code=zip)))
+            except:
+                pass            
 
         try:
             for link in kwargs['api_links']:
                 urls.append(rsc.REDFIN_URL.format(link))
         except:
             pass
```

### Comparing `redfin-scraper-0.1.6/redfin_scraper/resources/json_tools.py` & `redfin-scraper-0.2.0/redfin_scraper/resources/json_tools.py`

 * *Files identical despite different names*

### Comparing `redfin-scraper-0.1.6/redfin_scraper/resources/logging.py` & `redfin-scraper-0.2.0/redfin_scraper/resources/logging.py`

 * *Files identical despite different names*

### Comparing `redfin-scraper-0.1.6/redfin_scraper.egg-info/PKG-INFO` & `redfin-scraper-0.2.0/redfin_scraper.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redfin-scraper
-Version: 0.1.6
+Version: 0.2.0
 Summary: A Python library used to scrape data from Redfin.com using the unofficial Stringray API.
 Author-email: Ryan Sherby <ryan.m.sherby@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Ryan Sherby
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -59,26 +59,30 @@
 `from redfin_scraper import RedfinScraper`  
 
 ### Initialize Module
 `scraper = RedfinScraper()`
 
 ## Using The Scraper
 ### Required Setup
-`scraper.setup(zip_database_path:str,multiprocessing:bool=False)`
+`scraper.setup(zip_database_path:str, multiprocessing:bool=False)`
 
 > **zip_database_path**: Binary path to the zip_code_database.csv  
 
 > **multiprocessing**: Allow for multiprocessing
 
 ### Activating The Scraper
-`scraper.scrape(city_states:list[str]=None,zip_codes:list[str],lat_tuner:float=1.5,lon_tuner:float=1.5)`
+`scraper.scrape(city_states:list[str]=None, zip_codes:list[str], sold:bool=False, sale_period:str=None, lat_tuner:float=1.5, lon_tuner:float=1.5)`
 >**city_states**: List of strings representing US cities formatted as "City, State"  
 
 >**zip_codes**: List of strings representing US zip codes  
 
+>**sold**: Select whether to scrape for-sale data (default) or sold data  
+
+>**sale_period**: Must be selected whenever sold is True (1mo, 3mo, 6mo, 1yr, 3yr, 5yr)
+
 >**lat_tuner**: Represents # of standard deviations beyond the local latitude average that a zip code may exist within   
 
 >**lon_tuner**: Represents # of standard deviations beyond the local longitude average that a zip code may exist within  
 
 ### Accessing Prior Scrapes
 `scraper.get_data(id:str)`
 >**id**: IDs are indexed at 1 and increase in the format "D00#"
```

