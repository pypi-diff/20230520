# Comparing `tmp/fedml_databricks-1.0.2.dev0.tar.gz` & `tmp/fedml_databricks-1.0.3.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedml_databricks-1.0.2.dev0.tar", last modified: Thu May  4 21:50:09 2023, max compression
+gzip compressed data, was "fedml_databricks-1.0.3.dev0.tar", last modified: Wed May 17 23:12:18 2023, max compression
```

## Comparing `fedml_databricks-1.0.2.dev0.tar` & `fedml_databricks-1.0.3.dev0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 I550585    (501) staff       (20)        0 2023-05-04 21:50:09.681326 fedml_databricks-1.0.2.dev0/
--rw-r--r--   0 I550585    (501) staff       (20)    11307 2023-04-27 21:31:25.000000 fedml_databricks-1.0.2.dev0/LICENSE.txt
--rw-r--r--   0 I550585    (501) staff       (20)     1348 2023-05-04 21:50:09.680856 fedml_databricks-1.0.2.dev0/PKG-INFO
--rw-r--r--   0 I550585    (501) staff       (20)      950 2023-04-27 21:31:25.000000 fedml_databricks-1.0.2.dev0/README.md
--rw-r--r--   0 I550585    (501) staff       (20)      103 2023-02-01 00:25:03.000000 fedml_databricks-1.0.2.dev0/pyproject.toml
--rw-r--r--   0 I550585    (501) staff       (20)       38 2023-05-04 21:50:09.681448 fedml_databricks-1.0.2.dev0/setup.cfg
--rw-r--r--   0 I550585    (501) staff       (20)     1102 2023-05-04 21:49:36.000000 fedml_databricks-1.0.2.dev0/setup.py
-drwxr-xr-x   0 I550585    (501) staff       (20)        0 2023-05-04 21:50:09.589121 fedml_databricks-1.0.2.dev0/src/
-drwxr-xr-x   0 I550585    (501) staff       (20)        0 2023-05-04 21:50:09.641988 fedml_databricks-1.0.2.dev0/src/fedml_databricks/
--rw-r--r--   0 I550585    (501) staff       (20)      107 2023-04-27 21:31:25.000000 fedml_databricks-1.0.2.dev0/src/fedml_databricks/__init__.py
-drwxr-xr-x   0 I550585    (501) staff       (20)        0 2023-05-04 21:50:09.662997 fedml_databricks-1.0.2.dev0/src/fedml_databricks/acr/
--rw-r--r--   0 I550585    (501) staff       (20)        0 2023-04-27 21:31:25.000000 fedml_databricks-1.0.2.dev0/src/fedml_databricks/acr/__init__.py
--rw-r--r--   0 I550585    (501) staff       (20)     1694 2023-04-27 21:31:25.000000 fedml_databricks-1.0.2.dev0/src/fedml_databricks/acr/acr_kyma_deploy.py
--rw-r--r--   0 I550585    (501) staff       (20)     6823 2023-04-27 21:31:25.000000 fedml_databricks-1.0.2.dev0/src/fedml_databricks/acr/acr_kyma_deploy.sh
--rw-r--r--   0 I550585    (501) staff       (20)      332 2023-04-27 21:31:25.000000 fedml_databricks-1.0.2.dev0/src/fedml_databricks/databricks_cli_configure.sh
--rw-r--r--   0 I550585    (501) staff       (20)    15603 2023-05-03 23:57:50.000000 fedml_databricks-1.0.2.dev0/src/fedml_databricks/dbconnection.py
--rw-r--r--   0 I550585    (501) staff       (20)      682 2023-04-27 21:31:25.000000 fedml_databricks-1.0.2.dev0/src/fedml_databricks/deployment_helper.py
-drwxr-xr-x   0 I550585    (501) staff       (20)        0 2023-05-04 21:50:09.679934 fedml_databricks-1.0.2.dev0/src/fedml_databricks/ecr/
--rw-r--r--   0 I550585    (501) staff       (20)        0 2023-04-27 21:31:25.000000 fedml_databricks-1.0.2.dev0/src/fedml_databricks/ecr/__init__.py
--rw-r--r--   0 I550585    (501) staff       (20)     1597 2023-04-27 21:31:25.000000 fedml_databricks-1.0.2.dev0/src/fedml_databricks/ecr/ecr_kyma_deploy.py
--rw-r--r--   0 I550585    (501) staff       (20)     5006 2023-04-27 21:31:25.000000 fedml_databricks-1.0.2.dev0/src/fedml_databricks/ecr/ecr_kyma_deploy.sh
--rw-r--r--   0 I550585    (501) staff       (20)     1771 2023-04-27 21:31:25.000000 fedml_databricks-1.0.2.dev0/src/fedml_databricks/kubectl_install_validate.sh
--rw-r--r--   0 I550585    (501) staff       (20)     3909 2023-04-27 21:31:25.000000 fedml_databricks-1.0.2.dev0/src/fedml_databricks/kyma_deploy.py
--rw-r--r--   0 I550585    (501) staff       (20)      656 2023-02-01 00:25:03.000000 fedml_databricks-1.0.2.dev0/src/fedml_databricks/logger.py
--rw-r--r--   0 I550585    (501) staff       (20)      701 2023-04-27 21:31:25.000000 fedml_databricks-1.0.2.dev0/src/fedml_databricks/predict.py
-drwxr-xr-x   0 I550585    (501) staff       (20)        0 2023-05-04 21:50:09.646464 fedml_databricks-1.0.2.dev0/src/fedml_databricks.egg-info/
--rw-r--r--   0 I550585    (501) staff       (20)     1348 2023-05-04 21:50:09.000000 fedml_databricks-1.0.2.dev0/src/fedml_databricks.egg-info/PKG-INFO
--rw-r--r--   0 I550585    (501) staff       (20)      823 2023-05-04 21:50:09.000000 fedml_databricks-1.0.2.dev0/src/fedml_databricks.egg-info/SOURCES.txt
--rw-r--r--   0 I550585    (501) staff       (20)        1 2023-05-04 21:50:09.000000 fedml_databricks-1.0.2.dev0/src/fedml_databricks.egg-info/dependency_links.txt
--rw-r--r--   0 I550585    (501) staff       (20)       65 2023-05-04 21:50:09.000000 fedml_databricks-1.0.2.dev0/src/fedml_databricks.egg-info/requires.txt
--rw-r--r--   0 I550585    (501) staff       (20)       17 2023-05-04 21:50:09.000000 fedml_databricks-1.0.2.dev0/src/fedml_databricks.egg-info/top_level.txt
+drwxr-xr-x   0 I550585    (501) staff       (20)        0 2023-05-17 23:12:18.249156 fedml_databricks-1.0.3.dev0/
+-rw-r--r--   0 I550585    (501) staff       (20)    11307 2023-04-27 21:31:25.000000 fedml_databricks-1.0.3.dev0/LICENSE.txt
+-rw-r--r--   0 I550585    (501) staff       (20)     1348 2023-05-17 23:12:18.247909 fedml_databricks-1.0.3.dev0/PKG-INFO
+-rw-r--r--   0 I550585    (501) staff       (20)      950 2023-04-27 21:31:25.000000 fedml_databricks-1.0.3.dev0/README.md
+-rw-r--r--   0 I550585    (501) staff       (20)      103 2023-02-01 00:25:03.000000 fedml_databricks-1.0.3.dev0/pyproject.toml
+-rw-r--r--   0 I550585    (501) staff       (20)       38 2023-05-17 23:12:18.249377 fedml_databricks-1.0.3.dev0/setup.cfg
+-rw-r--r--   0 I550585    (501) staff       (20)     1102 2023-05-17 20:51:35.000000 fedml_databricks-1.0.3.dev0/setup.py
+drwxr-xr-x   0 I550585    (501) staff       (20)        0 2023-05-17 23:12:18.203152 fedml_databricks-1.0.3.dev0/src/
+drwxr-xr-x   0 I550585    (501) staff       (20)        0 2023-05-17 23:12:18.234724 fedml_databricks-1.0.3.dev0/src/fedml_databricks/
+-rw-r--r--   0 I550585    (501) staff       (20)      107 2023-04-27 21:31:25.000000 fedml_databricks-1.0.3.dev0/src/fedml_databricks/__init__.py
+drwxr-xr-x   0 I550585    (501) staff       (20)        0 2023-05-17 23:12:18.243544 fedml_databricks-1.0.3.dev0/src/fedml_databricks/acr/
+-rw-r--r--   0 I550585    (501) staff       (20)        0 2023-04-27 21:31:25.000000 fedml_databricks-1.0.3.dev0/src/fedml_databricks/acr/__init__.py
+-rw-r--r--   0 I550585    (501) staff       (20)     1694 2023-04-27 21:31:25.000000 fedml_databricks-1.0.3.dev0/src/fedml_databricks/acr/acr_kyma_deploy.py
+-rw-r--r--   0 I550585    (501) staff       (20)     6823 2023-04-27 21:31:25.000000 fedml_databricks-1.0.3.dev0/src/fedml_databricks/acr/acr_kyma_deploy.sh
+-rw-r--r--   0 I550585    (501) staff       (20)      332 2023-04-27 21:31:25.000000 fedml_databricks-1.0.3.dev0/src/fedml_databricks/databricks_cli_configure.sh
+-rw-r--r--   0 I550585    (501) staff       (20)    15793 2023-05-17 23:11:58.000000 fedml_databricks-1.0.3.dev0/src/fedml_databricks/dbconnection.py
+-rw-r--r--   0 I550585    (501) staff       (20)      682 2023-04-27 21:31:25.000000 fedml_databricks-1.0.3.dev0/src/fedml_databricks/deployment_helper.py
+drwxr-xr-x   0 I550585    (501) staff       (20)        0 2023-05-17 23:12:18.246838 fedml_databricks-1.0.3.dev0/src/fedml_databricks/ecr/
+-rw-r--r--   0 I550585    (501) staff       (20)        0 2023-04-27 21:31:25.000000 fedml_databricks-1.0.3.dev0/src/fedml_databricks/ecr/__init__.py
+-rw-r--r--   0 I550585    (501) staff       (20)     1597 2023-04-27 21:31:25.000000 fedml_databricks-1.0.3.dev0/src/fedml_databricks/ecr/ecr_kyma_deploy.py
+-rw-r--r--   0 I550585    (501) staff       (20)     5006 2023-04-27 21:31:25.000000 fedml_databricks-1.0.3.dev0/src/fedml_databricks/ecr/ecr_kyma_deploy.sh
+-rw-r--r--   0 I550585    (501) staff       (20)     1771 2023-04-27 21:31:25.000000 fedml_databricks-1.0.3.dev0/src/fedml_databricks/kubectl_install_validate.sh
+-rw-r--r--   0 I550585    (501) staff       (20)     3909 2023-04-27 21:31:25.000000 fedml_databricks-1.0.3.dev0/src/fedml_databricks/kyma_deploy.py
+-rw-r--r--   0 I550585    (501) staff       (20)      656 2023-02-01 00:25:03.000000 fedml_databricks-1.0.3.dev0/src/fedml_databricks/logger.py
+-rw-r--r--   0 I550585    (501) staff       (20)      701 2023-04-27 21:31:25.000000 fedml_databricks-1.0.3.dev0/src/fedml_databricks/predict.py
+drwxr-xr-x   0 I550585    (501) staff       (20)        0 2023-05-17 23:12:18.240671 fedml_databricks-1.0.3.dev0/src/fedml_databricks.egg-info/
+-rw-r--r--   0 I550585    (501) staff       (20)     1348 2023-05-17 23:12:18.000000 fedml_databricks-1.0.3.dev0/src/fedml_databricks.egg-info/PKG-INFO
+-rw-r--r--   0 I550585    (501) staff       (20)      823 2023-05-17 23:12:18.000000 fedml_databricks-1.0.3.dev0/src/fedml_databricks.egg-info/SOURCES.txt
+-rw-r--r--   0 I550585    (501) staff       (20)        1 2023-05-17 23:12:18.000000 fedml_databricks-1.0.3.dev0/src/fedml_databricks.egg-info/dependency_links.txt
+-rw-r--r--   0 I550585    (501) staff       (20)       65 2023-05-17 23:12:18.000000 fedml_databricks-1.0.3.dev0/src/fedml_databricks.egg-info/requires.txt
+-rw-r--r--   0 I550585    (501) staff       (20)       17 2023-05-17 23:12:18.000000 fedml_databricks-1.0.3.dev0/src/fedml_databricks.egg-info/top_level.txt
```

### Comparing `fedml_databricks-1.0.2.dev0/LICENSE.txt` & `fedml_databricks-1.0.3.dev0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fedml_databricks-1.0.2.dev0/PKG-INFO` & `fedml_databricks-1.0.3.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedml_databricks
-Version: 1.0.2.dev0
+Version: 1.0.3.dev0
 Summary: A python library for building machine learning models on Databricks using a federated data source
 Author: SAP SE
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `fedml_databricks-1.0.2.dev0/README.md` & `fedml_databricks-1.0.3.dev0/README.md`

 * *Files identical despite different names*

### Comparing `fedml_databricks-1.0.2.dev0/setup.py` & `fedml_databricks-1.0.3.dev0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 setuptools.setup(
     name="fedml_databricks",
-    version="1.0.2.dev0",
+    version="1.0.3.dev0",
     author="SAP SE",
     description="A python library for building machine learning models on Databricks using a federated data source",
     license='Apache License 2.0',
     license_files = ['LICENSE.txt'],
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
```

### Comparing `fedml_databricks-1.0.2.dev0/src/fedml_databricks/acr/acr_kyma_deploy.py` & `fedml_databricks-1.0.3.dev0/src/fedml_databricks/acr/acr_kyma_deploy.py`

 * *Files identical despite different names*

### Comparing `fedml_databricks-1.0.2.dev0/src/fedml_databricks/acr/acr_kyma_deploy.sh` & `fedml_databricks-1.0.3.dev0/src/fedml_databricks/acr/acr_kyma_deploy.sh`

 * *Files identical despite different names*

### Comparing `fedml_databricks-1.0.2.dev0/src/fedml_databricks/dbconnection.py` & `fedml_databricks-1.0.3.dev0/src/fedml_databricks/dbconnection.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     def get_table_size(self, table_name):
         if (self.connection.isconnected()):
             cursor = self.connection.cursor()
         else:
             self._get_connection()
             cursor = self.connection.cursor()
         schema = self.config['schema']
-        sqlQuery = f'SELECT COUNT(*) FROM "{schema}"."{table_name}"'
+        sqlQuery=""" SELECT COUNT(*) FROM "{}"."{}" """.format(schema,table_name)
         try:
             cursor.execute(sqlQuery)
             res = cursor.fetchall()
             return res
         except Exception as e:
             self.logger.error('error occured during query execution %s', e)
             self.connection.rollback()
@@ -101,15 +101,15 @@
             cursor = self.connection.cursor()
         else:
             self._get_connection()
             cursor = self.connection.cursor()
         rows = self.get_table_size(table_name)
         dataset_size = int(rows[0][0]*size)
         schema = self.config['schema']
-        sqlQuery = f'SELECT TOP {str(dataset_size)} * FROM "{schema}"."{table_name}"'
+        sqlQuery=""" SELECT TOP {} * FROM "{}"."{}"  """.format(str(dataset_size),schema,table_name)
         try:
             cursor.execute(sqlQuery)
             res = cursor.fetchall()
             column_headers = [i[0] for i in cursor.description]
             return res, column_headers
         except Exception as e:
             self.logger.error('error occured during query execution %s', e)
@@ -174,15 +174,15 @@
         else:
             self._get_connection()
             cursor = self.connection.cursor()
         try:
             if 'INSERTED_AT' in query:
                 raise Exception('\nQuery Error: A column name provided was a duplicate of the automatically added INSERTED_AT timestamp column.\nPlease refer to documentation on more information about this generated column and/or change the name of the duplicated column provided in the query.')
             timestamp_column = ', INSERTED_AT TIMESTAMP NOT NULL'
-            query = query[:-1] + timestamp_column + ')'
+            query = query.rstrip()[:-1] + timestamp_column + ')'
             self.logger.info("creating table...")
             self.logger.info(query)
             cursor.execute(query)
             if self.connection.getautocommit() == False:
                 self.connection.commit()
         except Exception as e:
             self.logger.error('error occured during query execution, doing rollback %s', e)
@@ -192,15 +192,15 @@
     def drop_table(self, table_name):
         if (self.connection.isconnected()):
             cursor = self.connection.cursor()
         else:
             self._get_connection()
             cursor = self.connection.cursor()
         try:
-            query = 'DROP TABLE ' + table_name
+            query = """ DROP TABLE "{}" """.format(table_name)
             self.logger.info("deleting table...")
             cursor.execute(query)
             if self.connection.getautocommit() == False:
                 self.connection.commit()
         except Exception as e:
             self.logger.error('error occured during query execution, doing rollback %s', e)
             self.connection.rollback()
@@ -215,15 +215,16 @@
             cursor = self.connection.cursor()
         try:
             self.logger.info('inserting into table...')
             column_names = ', '.join(list(table_values.columns))
             timestamp = datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
             bound_values = column_names.replace(', ', ', ' + ':')
             bound_values = ':' + bound_values + ', :INSERTED_AT'
-            sql = 'INSERT INTO ' + table_name + ' (' + column_names + ', INSERTED_AT) VALUES (' + bound_values + ')'
+            sql=""" INSERT INTO "{}" """.format(table_name)
+            sql+= ' (' + column_names + ', INSERTED_AT) VALUES (' + bound_values + ')'
             self.logger.info(sql)
             for index, row in table_values.iterrows():
                 temp_dict = row.to_dict()
                 temp_dict['INSERTED_AT'] = timestamp
                 cursor.execute(sql, temp_dict)
             if self.connection.getautocommit() == False:
                 self.connection.commit()
@@ -276,15 +277,16 @@
         if (self.connection.isconnected()):
             cursor = self.connection.cursor()
         else:
             self._get_connection()
             cursor = self.connection.cursor()
         try:
             self.logger.info("Deleting from table '%s'",table_name)
-            query="DELETE FROM "+table_name+("" if where_clause is None else " WHERE "+where_clause)
+            query=""" DELETE FROM "{}" """.format(table_name)
+            query+=("" if where_clause is None else " WHERE "+where_clause)
             self.logger.info("The delete query is: %s",query)
             cursor.execute(query)
             if self.connection.getautocommit() == False:
                 self.connection.commit()
         except Exception as e:
             self.logger.error('error occured during query execution, doing rollback %s', e)
             self.connection.rollback()
@@ -294,15 +296,16 @@
         if (self.connection.isconnected()):
             cursor = self.connection.cursor()
         else:
             self._get_connection()
             cursor = self.connection.cursor()
         try:
             self.logger.info("Updating table '%s'",table_name)
-            query="UPDATE "+table_name+" SET "+set_clause+("" if where_clause is None else " WHERE "+where_clause)
+            query=""" UPDATE "{}" """.format(table_name)
+            query+=" SET "+set_clause+("" if where_clause is None else " WHERE "+where_clause)
             self.logger.info("The update query is: %s",query)
             cursor.execute(query)
             if self.connection.getautocommit() == False:
                 self.connection.commit()
         except Exception as e:
             self.logger.error('error occured during query execution, doing rollback %s', e)
             self.connection.rollback()
@@ -312,15 +315,16 @@
         if (self.connection.isconnected()):
             cursor = self.connection.cursor()
         else:
             self._get_connection()
             cursor = self.connection.cursor()
         try:
             self.logger.info("Altering the table '%s'",table_name)
-            query="ALTER TABLE "+table_name+" "+clause
+            query=""" ALTER TABLE "{}" """.format(table_name)
+            query+=clause
             self.logger.info("The alter query is: %s",query)
             cursor.execute(query)
         except Exception as e:
             self.logger.error('error occured during query execution, doing rollback %s', e)
             self.connection.rollback()
             raise
```

### Comparing `fedml_databricks-1.0.2.dev0/src/fedml_databricks/deployment_helper.py` & `fedml_databricks-1.0.3.dev0/src/fedml_databricks/deployment_helper.py`

 * *Files identical despite different names*

### Comparing `fedml_databricks-1.0.2.dev0/src/fedml_databricks/ecr/ecr_kyma_deploy.py` & `fedml_databricks-1.0.3.dev0/src/fedml_databricks/ecr/ecr_kyma_deploy.py`

 * *Files identical despite different names*

### Comparing `fedml_databricks-1.0.2.dev0/src/fedml_databricks/ecr/ecr_kyma_deploy.sh` & `fedml_databricks-1.0.3.dev0/src/fedml_databricks/ecr/ecr_kyma_deploy.sh`

 * *Files identical despite different names*

### Comparing `fedml_databricks-1.0.2.dev0/src/fedml_databricks/kubectl_install_validate.sh` & `fedml_databricks-1.0.3.dev0/src/fedml_databricks/kubectl_install_validate.sh`

 * *Files identical despite different names*

### Comparing `fedml_databricks-1.0.2.dev0/src/fedml_databricks/kyma_deploy.py` & `fedml_databricks-1.0.3.dev0/src/fedml_databricks/kyma_deploy.py`

 * *Files identical despite different names*

### Comparing `fedml_databricks-1.0.2.dev0/src/fedml_databricks/logger.py` & `fedml_databricks-1.0.3.dev0/src/fedml_databricks/logger.py`

 * *Files identical despite different names*

### Comparing `fedml_databricks-1.0.2.dev0/src/fedml_databricks/predict.py` & `fedml_databricks-1.0.3.dev0/src/fedml_databricks/predict.py`

 * *Files identical despite different names*

### Comparing `fedml_databricks-1.0.2.dev0/src/fedml_databricks.egg-info/PKG-INFO` & `fedml_databricks-1.0.3.dev0/src/fedml_databricks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedml-databricks
-Version: 1.0.2.dev0
+Version: 1.0.3.dev0
 Summary: A python library for building machine learning models on Databricks using a federated data source
 Author: SAP SE
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `fedml_databricks-1.0.2.dev0/src/fedml_databricks.egg-info/SOURCES.txt` & `fedml_databricks-1.0.3.dev0/src/fedml_databricks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

