# Comparing `tmp/importer-local-0.0.4.tar.gz` & `tmp/importer-local-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "importer-local-0.0.4.tar", last modified: Sun May 14 16:22:42 2023, max compression
+gzip compressed data, was "importer-local-0.0.5.tar", last modified: Sat May 20 08:02:03 2023, max compression
```

## Comparing `importer-local-0.0.4.tar` & `importer-local-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:22:42.380521 importer-local-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:22:42.380521 importer-local-0.0.4/CirclesImporter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 16:22:29.000000 importer-local-0.0.4/CirclesImporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-14 16:22:29.000000 importer-local-0.0.4/CirclesImporter/example_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-05-14 16:22:29.000000 importer-local-0.0.4/CirclesImporter/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-14 16:22:42.380521 importer-local-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-14 16:22:29.000000 importer-local-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:22:42.380521 importer-local-0.0.4/importer_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-14 16:22:42.000000 importer-local-0.0.4/importer_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-14 16:22:42.000000 importer-local-0.0.4/importer_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 16:22:42.000000 importer-local-0.0.4/importer_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-14 16:22:42.000000 importer-local-0.0.4/importer_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 16:22:42.380521 importer-local-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-14 16:22:29.000000 importer-local-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 16:22:42.380521 importer-local-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-05-14 16:22:29.000000 importer-local-0.0.4/tests/test_importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:02:03.427306 importer-local-0.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:02:03.423306 importer-local-0.0.5/CirclesImporter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 08:01:45.000000 importer-local-0.0.5/CirclesImporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-05-20 08:01:45.000000 importer-local-0.0.5/CirclesImporter/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-20 08:02:03.427306 importer-local-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-20 08:01:45.000000 importer-local-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:02:03.427306 importer-local-0.0.5/importer_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-20 08:02:03.000000 importer-local-0.0.5/importer_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-20 08:02:03.000000 importer-local-0.0.5/importer_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 08:02:03.000000 importer-local-0.0.5/importer_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-20 08:02:03.000000 importer-local-0.0.5/importer_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 08:02:03.427306 importer-local-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-20 08:01:45.000000 importer-local-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:02:03.427306 importer-local-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-05-20 08:01:45.000000 importer-local-0.0.5/tests/test_importer.py
```

### Comparing `importer-local-0.0.4/CirclesImporter/importer.py` & `importer-local-0.0.5/CirclesImporter/importer.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,24 +21,17 @@
     return wrapper
 
 
 class Importer:
     def __init__(self, source):
         self.source_name = source
 
-    def get_logger_message(self, current_function_name):
-        start_message = "Function %s started." % current_function_name
-        finish_message = "Function '%s' completed." % current_function_name
-        return start_message, finish_message
-
     @log_function_execution
     def get_country_name(self, location):
         # Create a geocoder instance
-        # current_function_name = inspect.currentframe().f_code.co_name
-        # message = self.get_logger_message(current_function_name)[0]
         api_key = os.getenv("RDS_OPENCAGE_KEY")
 
         # Define the city or state
         geocoder = OpenCageGeocode(api_key)
 
         # Use geocoding to get the location details
         results = geocoder.geocode(location)
@@ -75,15 +68,15 @@
             last_inserted_id = cursor.lastrowid
             query_entity_ml = "INSERT INTO {}(`entity_type_name`,`entity_type_id`,`lang_code`,`created_user_id`,`updated_user_id`)" \
                               " VALUES (%s, %s, %s, 1, 1)".format('entity_type.entity_type_ml_table')
             cursor.execute(query_entity_ml, (entity_type_name, last_inserted_id, 'en'))
 
             db.commit()
         else:
-            print("Entity already exist")
+            locallgr.log("Entity already exist")
         db.close()
 
     @log_function_execution
     def insert_new_source(self):
         database_conn = database()
         db = database_conn.connect_to_database()
         cursor = db.cursor()
@@ -100,15 +93,15 @@
             last_inserted_id = cursor.lastrowid
             query_importer_source_ml = "INSERT INTO {}(`source_name`,`source_id`,`created_user_id`,`updated_user_id`)" \
                               " VALUES (%s, %s, 1, 1)".format('source.source_ml_table')
             cursor.execute(query_importer_source_ml, (self.source_name, last_inserted_id))
 
             db.commit()
         else:
-            print("Source already exist")
+            locallgr.log("Source already exist")
         db.close()
 
     @log_function_execution
     def insert_record_source(self, location, entity_type_name, entity_id, url):
         database_conn = database()
         db = database_conn.connect_to_database()
         cursor = db.cursor()
@@ -131,9 +124,8 @@
 
         db.commit()
         db.close()
 
 
 if __name__ == "__main__":
     pass
-    # imp = Importer("monster")
-    # print(imp.get_country_name("new york"))
+
```

### Comparing `importer-local-0.0.4/setup.py` & `importer-local-0.0.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 # used by python -m build
 # python -m build needs pyproject.toml or setup.py
 setuptools.setup(
      # TODO: Please update the name
      name='importer-local',
-     version='0.0.4',
+     version='0.0.5',
      author="Circles",
      author_email="info@circles.life",
      description="PyPI Package for Circles Local importer Python",
      long_description="This is a package for sharing common importer function used in different repositories",
      long_description_content_type="text/markdown",
      url="https://github.com/javatechy/dokr",
      packages=setuptools.find_packages(),
```

### Comparing `importer-local-0.0.4/tests/test_importer.py` & `importer-local-0.0.5/tests/test_importer.py`

 * *Files identical despite different names*

