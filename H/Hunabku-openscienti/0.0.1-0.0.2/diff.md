# Comparing `tmp/Hunabku_openscienti-0.0.1.tar.gz` & `tmp/Hunabku_openscienti-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Hunabku_openscienti-0.0.1.tar", last modified: Thu Apr 20 20:45:14 2023, max compression
+gzip compressed data, was "Hunabku_openscienti-0.0.2.tar", last modified: Sat May 20 02:59:52 2023, max compression
```

## Comparing `Hunabku_openscienti-0.0.1.tar` & `Hunabku_openscienti-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:45:14.454186 Hunabku_openscienti-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:45:14.450186 Hunabku_openscienti-0.0.1/Hunabku_openscienti.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-20 20:45:14.000000 Hunabku_openscienti-0.0.1/Hunabku_openscienti.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-20 20:45:14.000000 Hunabku_openscienti-0.0.1/Hunabku_openscienti.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 20:45:14.000000 Hunabku_openscienti-0.0.1/Hunabku_openscienti.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 20:45:14.000000 Hunabku_openscienti-0.0.1/Hunabku_openscienti.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-20 20:45:14.000000 Hunabku_openscienti-0.0.1/Hunabku_openscienti.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-20 20:44:57.000000 Hunabku_openscienti-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-20 20:45:14.454186 Hunabku_openscienti-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-20 20:44:57.000000 Hunabku_openscienti-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:45:14.454186 Hunabku_openscienti-0.0.1/hunabku_openscienti/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 20:44:57.000000 Hunabku_openscienti-0.0.1/hunabku_openscienti/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-20 20:44:57.000000 Hunabku_openscienti-0.0.1/hunabku_openscienti/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:45:14.454186 Hunabku_openscienti-0.0.1/hunabku_openscienti/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-04-20 20:44:57.000000 Hunabku_openscienti-0.0.1/hunabku_openscienti/endpoints/OpenScienti.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 20:45:14.454186 Hunabku_openscienti-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-04-20 20:44:57.000000 Hunabku_openscienti-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 02:59:52.155667 Hunabku_openscienti-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 02:59:52.151667 Hunabku_openscienti-0.0.2/Hunabku_openscienti.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-20 02:59:52.000000 Hunabku_openscienti-0.0.2/Hunabku_openscienti.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-20 02:59:52.000000 Hunabku_openscienti-0.0.2/Hunabku_openscienti.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 02:59:52.000000 Hunabku_openscienti-0.0.2/Hunabku_openscienti.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 02:59:52.000000 Hunabku_openscienti-0.0.2/Hunabku_openscienti.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-20 02:59:52.000000 Hunabku_openscienti-0.0.2/Hunabku_openscienti.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-20 02:59:36.000000 Hunabku_openscienti-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-20 02:59:52.155667 Hunabku_openscienti-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-20 02:59:36.000000 Hunabku_openscienti-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 02:59:52.151667 Hunabku_openscienti-0.0.2/hunabku_openscienti/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 02:59:36.000000 Hunabku_openscienti-0.0.2/hunabku_openscienti/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-20 02:59:36.000000 Hunabku_openscienti-0.0.2/hunabku_openscienti/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 02:59:52.155667 Hunabku_openscienti-0.0.2/hunabku_openscienti/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-05-20 02:59:36.000000 Hunabku_openscienti-0.0.2/hunabku_openscienti/endpoints/OpenScienti.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 02:59:52.155667 Hunabku_openscienti-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-20 02:59:36.000000 Hunabku_openscienti-0.0.2/setup.py
```

### Comparing `Hunabku_openscienti-0.0.1/Hunabku_openscienti.egg-info/PKG-INFO` & `Hunabku_openscienti-0.0.2/Hunabku_openscienti.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Hunabku-openscienti
-Version: 0.0.1
+Version: 0.0.2
 Summary: Hunabku plguin fro Open Data Scienti
 Home-page: https://github.com/colav/Hunabku_plugins
 Author: Colav
 Author-email: colav@udea.edu.co
 License: BSD
 Description-Content-Type: text/markdown
```

### Comparing `Hunabku_openscienti-0.0.1/PKG-INFO` & `Hunabku_openscienti-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Hunabku_openscienti
-Version: 0.0.1
+Version: 0.0.2
 Summary: Hunabku plguin fro Open Data Scienti
 Home-page: https://github.com/colav/Hunabku_plugins
 Author: Colav
 Author-email: colav@udea.edu.co
 License: BSD
 Description-Content-Type: text/markdown
```

### Comparing `Hunabku_openscienti-0.0.1/hunabku_openscienti/endpoints/OpenScienti.py` & `Hunabku_openscienti-0.0.2/hunabku_openscienti/endpoints/OpenScienti.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 from hunabku.HunabkuBase import HunabkuPluginBase, endpoint
 from hunabku.Config import Config, Param
 from pymongo import MongoClient
 import sys
-import re
 
 
 class OpenScienti(HunabkuPluginBase):
     config = Config()
     config += Param(db_uri="mongodb://localhost:27017/",
                     doc="MongoDB string connection")
     config += Param(db_name="yuku",
                     doc="MongoDB Open Scienti generated database by yuku")
 
     def __init__(self, hunabku):
         super().__init__(hunabku)
         self.dbclient = MongoClient(self.config.db_uri)
         self.db = self.dbclient[self.config.db_name]
 
-
     @endpoint('/openscienti/cvlac', methods=['GET'])
     def openscienti_cvlac(self):
         """
         @api {get} /openscienti/cvlac OpenScienti cvlac endpoint
         @apiName cvlac
         @apiGroup OpenScienti
         @apiDescription Allows to perform queries for cvlac users, given the COD_RH
@@ -37,22 +35,38 @@
             # all the info for the user
             curl -i http://apis.colav.co/openscienti/cvlac?COD_RH=0000000020
         """
         try:
             cod_rh = self.request.args.get('COD_RH')
             if cod_rh:
                 data = {}
-                data["raw_data"] = list(self.db["cvlac_data"].find({'id_persona_pr': cod_rh},{'_id':0}))
-                data["scrapped_data"] = list(self.db["cvlac_stage"].find({'id_persona_pr': cod_rh},{"_id":0}))
+                data["raw_data"] = list(self.db["cvlac_data"].find(
+                    {'id_persona_pr': cod_rh}, {'_id': 0}))
+                data["scrapped_data"] = list(self.db["cvlac_stage"].find(
+                    {'id_persona_pr': cod_rh}, {"_id": 0}))
                 response = self.app.response_class(
                     response=self.json.dumps(data),
                     status=200,
                     mimetype='application/json'
                 )
                 return response
+            else:
+                #  return all the records
+                data = {}
+                data["raw_data"] = list(
+                    self.db["cvlac_data"].find({}, {'_id': 0}))
+                data["scrapped_data"] = list(
+                    self.db["cvlac_stage"].find({}, {"_id": 0}))
+                response = self.app.response_class(
+                    response=self.json.dumps(data),
+                    status=200,
+                    mimetype='application/json'
+                )
+                return response
+
             data = {
                 "error": "Bad Request", "message": "invalid parameters, please select privide COD_RH  parameter."}
             response = self.app.response_class(
                 response=self.json.dumps(data),
                 status=400,
                 mimetype='application/json'
             )
@@ -63,15 +77,14 @@
             response = self.app.response_class(
                 response=self.json.dumps(data),
                 status=400,
                 mimetype='application/json'
             )
             return response
 
- 
     @endpoint('/openscienti/info', methods=['GET'])
     def openscienti_info(self):
         """
         @api {get} /openscienti/info OpenScienti info endpoint
         @apiName Info
         @apiGroup OpenScienti
         @apiDescription Allows to perform queries for information,
@@ -80,21 +93,22 @@
 
         @apiSuccess {Object}  Resgisters from MongoDB in Json format.
 
         @apiError (Error 401) msg  The HTTP 401 Unauthorized invalid authentication apikey for the target resource.
         @apiError (Error 400) msg  Bad request, if the query is not right.
 
         @apiExample {curl} Example usage:
-            # resume of open scienti data 
+            # resume of open scienti data
             curl -i http://apis.colav.co/scienti/info
         """
         try:
             data = {}
             data["ids"] = self.db["cvlac_data"].distinct("id_persona_pr")
-            data["dataset_info"] = self.db["cvlac_dataset_info"].find_one({},{"_id":0})
+            data["dataset_info"] = self.db["cvlac_dataset_info"].find_one({}, {
+                                                                          "_id": 0})
             response = self.app.response_class(
                 response=self.json.dumps(data),
                 status=200,
                 mimetype='application/json'
             )
             return response
```

### Comparing `Hunabku_openscienti-0.0.1/setup.py` & `Hunabku_openscienti-0.0.2/setup.py`

 * *Files identical despite different names*

