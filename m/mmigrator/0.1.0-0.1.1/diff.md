# Comparing `tmp/mmigrator-0.1.0.tar.gz` & `tmp/mmigrator-0.1.1.tar.gz`

## Comparing `mmigrator-0.1.0.tar` & `mmigrator-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rwxr-xr-x   0        0        0       95 2020-02-02 00:00:00.000000 mmigrator-0.1.0/package.sh
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 mmigrator-0.1.0/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mmigrator-0.1.0/src/__init__.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 mmigrator-0.1.0/src/mmigrator/__init__.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 mmigrator-0.1.0/src/mmigrator/cli.py
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 mmigrator-0.1.0/src/mmigrator/config_manager.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 mmigrator-0.1.0/src/mmigrator/constants.py
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 mmigrator-0.1.0/src/mmigrator/db.py
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 mmigrator-0.1.0/src/mmigrator/migration.py
--rw-r--r--   0        0        0     2949 2020-02-02 00:00:00.000000 mmigrator-0.1.0/src/mmigrator/migration_manager.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 mmigrator-0.1.0/src/mmigrator/process.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mmigrator-0.1.0/src/mmigrator/types/__init__.py
--rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 mmigrator-0.1.0/tests/helpers.py
--rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 mmigrator-0.1.0/tests/test_migration_manager.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 mmigrator-0.1.0/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 mmigrator-0.1.0/LICENSE
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 mmigrator-0.1.0/README.md
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 mmigrator-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 mmigrator-0.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0       95 2020-02-02 00:00:00.000000 mmigrator-0.1.1/package.sh
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 mmigrator-0.1.1/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mmigrator-0.1.1/src/__init__.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 mmigrator-0.1.1/src/mmigrator/__init__.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 mmigrator-0.1.1/src/mmigrator/cli.py
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 mmigrator-0.1.1/src/mmigrator/config_manager.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 mmigrator-0.1.1/src/mmigrator/constants.py
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 mmigrator-0.1.1/src/mmigrator/db.py
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 mmigrator-0.1.1/src/mmigrator/migration.py
+-rw-r--r--   0        0        0     2949 2020-02-02 00:00:00.000000 mmigrator-0.1.1/src/mmigrator/migration_manager.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 mmigrator-0.1.1/src/mmigrator/process.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mmigrator-0.1.1/src/mmigrator/types/__init__.py
+-rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 mmigrator-0.1.1/tests/helpers.py
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 mmigrator-0.1.1/tests/test_migration_manager.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 mmigrator-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 mmigrator-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 mmigrator-0.1.1/README.md
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 mmigrator-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 mmigrator-0.1.1/PKG-INFO
```

### Comparing `mmigrator-0.1.0/src/mmigrator/cli.py` & `mmigrator-0.1.1/src/mmigrator/cli.py`

 * *Files identical despite different names*

### Comparing `mmigrator-0.1.0/src/mmigrator/config_manager.py` & `mmigrator-0.1.1/src/mmigrator/config_manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         if not os.path.exists(CONFIG_FILE_NAME):
             init()
 
     @staticmethod
     def read_config() -> dict:
         def load_env_var(filename: str, varname: str) -> str:
             with open(filename, 'r') as f:
-                m = re.match(r'var\s=\s(.+)', f.read())
+                m = re.match(fr'{varname}\s?=\s?(.+)', f.read())
 
                 if not m:
                     raise Exception(f'Cannot parse {varname} variable from file {filename}')
 
                 return m[1]
 
         with open(CONFIG_FILE_NAME, 'r') as f:
```

### Comparing `mmigrator-0.1.0/src/mmigrator/constants.py` & `mmigrator-0.1.1/src/mmigrator/constants.py`

 * *Files identical despite different names*

### Comparing `mmigrator-0.1.0/src/mmigrator/db.py` & `mmigrator-0.1.1/src/mmigrator/db.py`

 * *Files identical despite different names*

### Comparing `mmigrator-0.1.0/src/mmigrator/migration.py` & `mmigrator-0.1.1/src/mmigrator/migration.py`

 * *Files identical despite different names*

### Comparing `mmigrator-0.1.0/src/mmigrator/migration_manager.py` & `mmigrator-0.1.1/src/mmigrator/migration_manager.py`

 * *Files identical despite different names*

### Comparing `mmigrator-0.1.0/tests/helpers.py` & `mmigrator-0.1.1/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `mmigrator-0.1.0/tests/test_migration_manager.py` & `mmigrator-0.1.1/tests/test_migration_manager.py`

 * *Files identical despite different names*

### Comparing `mmigrator-0.1.0/LICENSE` & `mmigrator-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mmigrator-0.1.0/README.md` & `mmigrator-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `mmigrator-0.1.0/pyproject.toml` & `mmigrator-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mmigrator"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Serhii Kovalov", email="moiserge.k@gmail.com" },
 ]
 description = "Migration engine for MongoDB"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `mmigrator-0.1.0/PKG-INFO` & `mmigrator-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmigrator
-Version: 0.1.0
+Version: 0.1.1
 Summary: Migration engine for MongoDB
 Project-URL: Homepage, https://github.com/sergekovalev/mmigrator
 Project-URL: Bug Tracker, https://github.com/sergekovalev/mmigrator/issues
 Author-email: Serhii Kovalov <moiserge.k@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

