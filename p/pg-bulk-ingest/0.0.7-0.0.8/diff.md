# Comparing `tmp/pg_bulk_ingest-0.0.7.tar.gz` & `tmp/pg_bulk_ingest-0.0.8.tar.gz`

## Comparing `pg_bulk_ingest-0.0.7.tar` & `pg_bulk_ingest-0.0.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     6864 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.7/pg_bulk_ingest.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.7/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.7/LICENSE
--rw-r--r--   0        0        0     2886 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.7/README.md
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     4273 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0    13856 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.8/pg_bulk_ingest.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.8/LICENSE
+-rw-r--r--   0        0        0     6089 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.8/README.md
+-rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     7516 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.8/PKG-INFO
```

### Comparing `pg_bulk_ingest-0.0.7/.gitignore` & `pg_bulk_ingest-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `pg_bulk_ingest-0.0.7/LICENSE` & `pg_bulk_ingest-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pg_bulk_ingest-0.0.7/pyproject.toml` & `pg_bulk_ingest-0.0.8/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pg-bulk-ingest"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Department for International Trade", email="sre@digital.trade.gov.uk" },
 ]
 description = "A collection of Python utility functions for ingesting data into SQLAlchemy-defined PostgreSQL tables, automatically migrating them as needed, and minimising locking"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "sqlalchemy>=1.4.24", 
+    "sqlalchemy>=1.4.24",
+    "pg-force-execute>=0.0.10",
 ]
 
 [project.optional-dependencies]
 dev = [
     "psycopg>=3.1.4",
     "psycopg2>=2.9.2",
     "pytest>=7.2.1",
```

