# Comparing `tmp/mmigrator-0.1.2.tar.gz` & `tmp/mmigrator-0.1.3.tar.gz`

## Comparing `mmigrator-0.1.2.tar` & `mmigrator-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rwxr-xr-x   0        0        0       95 2020-02-02 00:00:00.000000 mmigrator-0.1.2/package.sh
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 mmigrator-0.1.2/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mmigrator-0.1.2/src/__init__.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 mmigrator-0.1.2/src/mmigrator/__init__.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 mmigrator-0.1.2/src/mmigrator/cli.py
--rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 mmigrator-0.1.2/src/mmigrator/config_manager.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 mmigrator-0.1.2/src/mmigrator/constants.py
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 mmigrator-0.1.2/src/mmigrator/db.py
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 mmigrator-0.1.2/src/mmigrator/migration.py
--rw-r--r--   0        0        0     2949 2020-02-02 00:00:00.000000 mmigrator-0.1.2/src/mmigrator/migration_manager.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 mmigrator-0.1.2/src/mmigrator/process.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mmigrator-0.1.2/src/mmigrator/types/__init__.py
--rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 mmigrator-0.1.2/tests/helpers.py
--rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 mmigrator-0.1.2/tests/test_migration_manager.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 mmigrator-0.1.2/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 mmigrator-0.1.2/LICENSE
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 mmigrator-0.1.2/README.md
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 mmigrator-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 mmigrator-0.1.2/PKG-INFO
+-rwxr-xr-x   0        0        0       95 2020-02-02 00:00:00.000000 mmigrator-0.1.3/package.sh
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 mmigrator-0.1.3/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mmigrator-0.1.3/src/__init__.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 mmigrator-0.1.3/src/mmigrator/__init__.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 mmigrator-0.1.3/src/mmigrator/cli.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 mmigrator-0.1.3/src/mmigrator/config_manager.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 mmigrator-0.1.3/src/mmigrator/constants.py
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 mmigrator-0.1.3/src/mmigrator/db.py
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 mmigrator-0.1.3/src/mmigrator/migration.py
+-rw-r--r--   0        0        0     2949 2020-02-02 00:00:00.000000 mmigrator-0.1.3/src/mmigrator/migration_manager.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 mmigrator-0.1.3/src/mmigrator/process.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mmigrator-0.1.3/src/mmigrator/types/__init__.py
+-rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 mmigrator-0.1.3/tests/helpers.py
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 mmigrator-0.1.3/tests/test_migration_manager.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 mmigrator-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 mmigrator-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 mmigrator-0.1.3/README.md
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 mmigrator-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 mmigrator-0.1.3/PKG-INFO
```

### Comparing `mmigrator-0.1.2/src/mmigrator/cli.py` & `mmigrator-0.1.3/src/mmigrator/cli.py`

 * *Files identical despite different names*

### Comparing `mmigrator-0.1.2/src/mmigrator/config_manager.py` & `mmigrator-0.1.3/src/mmigrator/config_manager.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,30 +16,40 @@
                 f.write(conf)
             
         if not os.path.exists(CONFIG_FILE_NAME):
             init()
 
     @staticmethod
     def read_config() -> dict:
-        def load_env_var(filename: str, varname: str) -> str:
-            with open(filename, 'r') as f:
-                m = re.search(fr'{varname}\s?=\s?(.+)', f.read())
-
-                if not m:
-                    raise Exception(f'Cannot parse {varname} variable from file {filename}')
+        def load_var(filename: str, varname: str) -> str:
+            var_value = None
 
-                return m[1]
+            with open(filename, 'r') as f:
+                data = f.read()
+                
+            if re.match(r'^.*\.json$', filename):
+                data = json.loads(data)
+                var_value = data.get(varname)
+            else:
+                m = re.search(fr'{varname}\s?=\s?(.+)', data)
+                if m:
+                    var_value = m[1]
+            
+            if not var_value:
+                raise Exception(f'Cannot parse {varname} variable from file {filename}')
+            
+            return var_value
 
         with open(CONFIG_FILE_NAME, 'r') as f:
             cfg = json.loads(f.read())
 
         for k, v in cfg['connection'].items():
             if v and re.match(r'^.+\[.+\]$', v):
                 file, var = re.sub(r'[\[\]]', ' ', v).strip().split(' ')
-                cfg['connection'][k] = load_env_var(file, var)
+                cfg['connection'][k] = load_var(file, var)
 
         return cfg
 
     @staticmethod
     def init_dist(dist: str):
         if not os.path.exists(dist):
             os.mkdir(dist)
```

### Comparing `mmigrator-0.1.2/src/mmigrator/constants.py` & `mmigrator-0.1.3/src/mmigrator/constants.py`

 * *Files identical despite different names*

### Comparing `mmigrator-0.1.2/src/mmigrator/db.py` & `mmigrator-0.1.3/src/mmigrator/db.py`

 * *Files identical despite different names*

### Comparing `mmigrator-0.1.2/src/mmigrator/migration.py` & `mmigrator-0.1.3/src/mmigrator/migration.py`

 * *Files identical despite different names*

### Comparing `mmigrator-0.1.2/src/mmigrator/migration_manager.py` & `mmigrator-0.1.3/src/mmigrator/migration_manager.py`

 * *Files identical despite different names*

### Comparing `mmigrator-0.1.2/tests/helpers.py` & `mmigrator-0.1.3/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `mmigrator-0.1.2/tests/test_migration_manager.py` & `mmigrator-0.1.3/tests/test_migration_manager.py`

 * *Files identical despite different names*

### Comparing `mmigrator-0.1.2/LICENSE` & `mmigrator-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mmigrator-0.1.2/README.md` & `mmigrator-0.1.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         "port": "",
         "database": "",
         "user": "",
         "password": ""
     }
 }
 ```
-Connection variables could be set from any file.\
+Connection variables could be set from .env|.json files.\
 e.g. from .env file:
 ```json
 "host": ".env[MONGO_HOST]",
 "port": ".env[MONGO_PORT]",
 "database": ".env[MONGO_DB]",
 "user": ".env[MONGO_USER]",
 "password": ".env[MONGO_PASSWORD]"
```

### Comparing `mmigrator-0.1.2/pyproject.toml` & `mmigrator-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mmigrator"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Serhii Kovalov", email="moiserge.k@gmail.com" },
 ]
 description = "Migration engine for MongoDB"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `mmigrator-0.1.2/PKG-INFO` & `mmigrator-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmigrator
-Version: 0.1.2
+Version: 0.1.3
 Summary: Migration engine for MongoDB
 Project-URL: Homepage, https://github.com/sergekovalev/mmigrator
 Project-URL: Bug Tracker, https://github.com/sergekovalev/mmigrator/issues
 Author-email: Serhii Kovalov <moiserge.k@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -36,15 +36,15 @@
         "port": "",
         "database": "",
         "user": "",
         "password": ""
     }
 }
 ```
-Connection variables could be set from any file.\
+Connection variables could be set from .env|.json files.\
 e.g. from .env file:
 ```json
 "host": ".env[MONGO_HOST]",
 "port": ".env[MONGO_PORT]",
 "database": ".env[MONGO_DB]",
 "user": ".env[MONGO_USER]",
 "password": ".env[MONGO_PASSWORD]"
```

