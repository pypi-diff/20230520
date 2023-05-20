# Comparing `tmp/postnormalism-0.0.1.tar.gz` & `tmp/postnormalism-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postnormalism-0.0.1.tar", last modified: Sat May  6 17:26:53 2023, max compression
+gzip compressed data, was "postnormalism-0.0.2.tar", last modified: Sat May 20 00:50:16 2023, max compression
```

## Comparing `postnormalism-0.0.1.tar` & `postnormalism-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 17:26:53.997204 postnormalism-0.0.1/
--rw-rw-rw-   0        0        0     1119 2023-05-06 02:54:20.000000 postnormalism-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     6183 2023-05-06 17:26:53.996673 postnormalism-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     5022 2023-05-06 17:12:44.000000 postnormalism-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 17:26:53.975554 postnormalism-0.0.1/postnormalism/
--rw-rw-rw-   0        0        0        5 2023-05-06 04:45:59.000000 postnormalism-0.0.1/postnormalism/VERSION
--rw-rw-rw-   0        0        0        0 2023-05-06 02:40:21.000000 postnormalism-0.0.1/postnormalism/__init__.py
--rw-rw-rw-   0        0        0     1450 2023-05-06 04:09:41.000000 postnormalism-0.0.1/postnormalism/core.py
-drwxrwxrwx   0        0        0        0 2023-05-06 17:26:53.993485 postnormalism-0.0.1/postnormalism/schema/
--rw-rw-rw-   0        0        0       95 2023-05-06 03:22:42.000000 postnormalism-0.0.1/postnormalism/schema/__init__.py
--rw-rw-rw-   0        0        0      193 2023-05-06 03:22:43.000000 postnormalism-0.0.1/postnormalism/schema/function.py
--rw-rw-rw-   0        0        0      430 2023-05-06 03:22:42.000000 postnormalism-0.0.1/postnormalism/schema/schema_item.py
--rw-rw-rw-   0        0        0      427 2023-05-06 03:22:43.000000 postnormalism-0.0.1/postnormalism/schema/table.py
--rw-rw-rw-   0        0        0      711 2023-05-06 03:40:39.000000 postnormalism-0.0.1/postnormalism/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-06 17:26:53.989243 postnormalism-0.0.1/postnormalism.egg-info/
--rw-rw-rw-   0        0        0     6183 2023-05-06 17:26:53.000000 postnormalism-0.0.1/postnormalism.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      445 2023-05-06 17:26:53.000000 postnormalism-0.0.1/postnormalism.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 17:26:53.000000 postnormalism-0.0.1/postnormalism.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-06 17:26:53.000000 postnormalism-0.0.1/postnormalism.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1342 2023-05-06 17:09:12.000000 postnormalism-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-06 17:26:53.997204 postnormalism-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-06 17:26:53.995616 postnormalism-0.0.1/tests/
--rw-rw-rw-   0        0        0     1778 2023-05-06 17:12:44.000000 postnormalism-0.0.1/tests/test_core.py
--rw-rw-rw-   0        0        0     2288 2023-05-06 17:12:44.000000 postnormalism-0.0.1/tests/test_schema.py
+drwxrwxrwx   0        0        0        0 2023-05-20 00:50:16.482985 postnormalism-0.0.2/
+-rw-rw-rw-   0        0        0     1119 2023-05-06 02:54:20.000000 postnormalism-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     6560 2023-05-20 00:50:16.481987 postnormalism-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5399 2023-05-20 00:44:01.000000 postnormalism-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-20 00:50:16.460985 postnormalism-0.0.2/postnormalism/
+-rw-rw-rw-   0        0        0        5 2023-05-20 00:46:34.000000 postnormalism-0.0.2/postnormalism/VERSION
+-rw-rw-rw-   0        0        0        0 2023-05-06 02:40:21.000000 postnormalism-0.0.2/postnormalism/__init__.py
+-rw-rw-rw-   0        0        0     2143 2023-05-17 02:28:23.000000 postnormalism-0.0.2/postnormalism/core.py
+drwxrwxrwx   0        0        0        0 2023-05-20 00:50:16.478983 postnormalism-0.0.2/postnormalism/schema/
+-rw-rw-rw-   0        0        0      131 2023-05-08 03:58:46.000000 postnormalism-0.0.2/postnormalism/schema/__init__.py
+-rw-rw-rw-   0        0        0     1509 2023-05-17 02:29:40.000000 postnormalism-0.0.2/postnormalism/schema/database.py
+-rw-rw-rw-   0        0        0     1082 2023-05-17 02:15:23.000000 postnormalism-0.0.2/postnormalism/schema/database_item.py
+-rw-rw-rw-   0        0        0      408 2023-05-08 03:58:46.000000 postnormalism-0.0.2/postnormalism/schema/function.py
+-rw-rw-rw-   0        0        0      774 2023-05-17 02:19:15.000000 postnormalism-0.0.2/postnormalism/schema/table.py
+-rw-rw-rw-   0        0        0      711 2023-05-06 03:40:39.000000 postnormalism-0.0.2/postnormalism/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-20 00:50:16.473984 postnormalism-0.0.2/postnormalism.egg-info/
+-rw-rw-rw-   0        0        0     6560 2023-05-20 00:50:16.000000 postnormalism-0.0.2/postnormalism.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      480 2023-05-20 00:50:16.000000 postnormalism-0.0.2/postnormalism.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 00:50:16.000000 postnormalism-0.0.2/postnormalism.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-20 00:50:16.000000 postnormalism-0.0.2/postnormalism.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1342 2023-05-20 00:26:25.000000 postnormalism-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-20 00:50:16.482985 postnormalism-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-20 00:50:16.480983 postnormalism-0.0.2/tests/
+-rw-rw-rw-   0        0        0     1778 2023-05-06 17:12:44.000000 postnormalism-0.0.2/tests/test_core.py
+-rw-rw-rw-   0        0        0     2288 2023-05-06 17:12:44.000000 postnormalism-0.0.2/tests/test_schema.py
```

### Comparing `postnormalism-0.0.1/LICENSE` & `postnormalism-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `postnormalism-0.0.1/PKG-INFO` & `postnormalism-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: postnormalism
-Version: 0.0.1
+Version: 0.0.2
 Summary: Postnormalism is Not an Object Relational Mapper (NORM) it is a lightweight and simple-to-use Python library for managing PostgreSQL database schemas. It provides an easy way to define tables and functions, organize schema items, and create them in a database with a specified load order.
 Author-email: Zac Miller <zac@informatical.info>
 Maintainer-email: Zac Miller <zac@informatical.info>
 License: MIT License
 Project-URL: Homepage, https://github.com/jzmiller1/postnormalism
 Project-URL: Bug Tracker, https://github.com/jzmiller1/postnormalism/issues
 Project-URL: Repository, https://github.com/jzmiller1/postnormalism.git
@@ -22,17 +22,19 @@
 # postnormalism: PostgreSQL Schema Management  
   
 postnormalism is Not an Object Relational Mapper (NORM) it is a lightweight and simple-to-use Python library for managing PostgreSQL database schemas. It provides an easy way to define tables and functions, organize schema items, and create them in a database with a specified load order.  
   
 ## Features  
   
 - Define tables and functions using Python dataclasses  
-- Create schema items (Tables, Functions) with comments
-- Load schema items in a specified load order  
-- Group related schema items and create them within a single transaction  
+- Create database items (Tables, Functions) with comments
+- Group related database items and create them within a single transaction  
+- Create a Database object that allows loading database items in a specified load order and managing database extensions
+- IF NOT EXISTS mode for loading
+
   
 ## NORM vs. ORM: Features Comparison  
   
 postnormalism is a lightweight and simple-to-use Python library for managing PostgreSQL database schemas. It does not possess all the characteristics of a full-fledged ORM, focusing mainly on schema management and organization.  
   
 Here is a comparison of postnormalism's features with typical ORM characteristics:  
   
@@ -60,37 +62,41 @@
   
 ```sh  
 pip install postnormalism  
 ```  
   
 ## Usage  
   
-### Defining Schema Items  
+### Defining Database Items  
   
 To define a table or a function, use the `Table` and `Function` dataclasses from the `postnormalism` module:  
   
 ```python  
-from postnormalism import Table, Function  
+from postnormalism.schema import Table, Function  
 ```
   
 ### Define a Table
 ```python
+from postnormalism.schema import Table
+
 create_table_sql = """  
 CREATE TABLE material (  
 id uuid PRIMARY KEY DEFAULT uuid_generate_v4(),  
 name varchar(120) NOT NULL,  
 description varchar(240)  
 );  
 """  
   
 Material = Table(create=create_table_sql)  
 ```
   
 ### Define a Postgresql Function  
 ```python
+from postnormalism.schema import Function
+
 create_function_sql = """  
 CREATE FUNCTION get_material_for_variant(variant uuid)  
 RETURNS uuid  
 AS $$  
 material_plan = plpy.prepare("SELECT material FROM material_variant WHERE id = $1",  
 ["uuid"])  
 material = plpy.execute(material_plan, [variant])[0]["material"]  
@@ -102,29 +108,37 @@
 COMMENT ON FUNCTION get_material_for_variant IS  
 $$ An example function $$;  
 """  
   
 get_material_for_variant = Function(create=create_function_sql, comment=comment_function_sql)  
 ```  
   
-### Creating Schema Items in a Database  
+### Creating Database Items in a Database  
   
-To create schema items in a PostgreSQL database, use the `create_schema` function from the `postnormalism` module:  
+To create database items in a PostgreSQL database, use the `Database` class:  
   
 ```python  
 import psycopg  
-from postnormalism import create_schema  
+from postnormalism.schema import Database
 from your_example_file import Material, get_material_for_variant
 
-db_connection_string = "dbname=test user=postgres password=secret host=localhost port=5432"  
+universe = Database(
+    load_order=[
+        Material, get_material_for_variant,
+        [Player, Inventory],  # example of grouping DatabaseItems into a transaction
+    ],
+    extensions=['uuid-ossp', 'plpython3u', 'pgcrypto']
+)
+
+db_connection_string = "dbname=test user=postgres password=secret host=localhost port=port"  
 
 connection = psycopg.connect(db_connection_string)  
 cursor = connection.cursor()  
 
-create_schema([Material, get_material_for_variant], cursor)  
+universe.create(cursor)  
 
 connection.commit()  
 connection.close()  
 ```  
 
   
 ## Contributing
```

### Comparing `postnormalism-0.0.1/README.md` & `postnormalism-0.0.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # postnormalism: PostgreSQL Schema Management  
   
 postnormalism is Not an Object Relational Mapper (NORM) it is a lightweight and simple-to-use Python library for managing PostgreSQL database schemas. It provides an easy way to define tables and functions, organize schema items, and create them in a database with a specified load order.  
   
 ## Features  
   
 - Define tables and functions using Python dataclasses  
-- Create schema items (Tables, Functions) with comments
-- Load schema items in a specified load order  
-- Group related schema items and create them within a single transaction  
+- Create database items (Tables, Functions) with comments
+- Group related database items and create them within a single transaction  
+- Create a Database object that allows loading database items in a specified load order and managing database extensions
+- IF NOT EXISTS mode for loading
+
   
 ## NORM vs. ORM: Features Comparison  
   
 postnormalism is a lightweight and simple-to-use Python library for managing PostgreSQL database schemas. It does not possess all the characteristics of a full-fledged ORM, focusing mainly on schema management and organization.  
   
 Here is a comparison of postnormalism's features with typical ORM characteristics:  
   
@@ -39,37 +41,41 @@
   
 ```sh  
 pip install postnormalism  
 ```  
   
 ## Usage  
   
-### Defining Schema Items  
+### Defining Database Items  
   
 To define a table or a function, use the `Table` and `Function` dataclasses from the `postnormalism` module:  
   
 ```python  
-from postnormalism import Table, Function  
+from postnormalism.schema import Table, Function  
 ```
   
 ### Define a Table
 ```python
+from postnormalism.schema import Table
+
 create_table_sql = """  
 CREATE TABLE material (  
 id uuid PRIMARY KEY DEFAULT uuid_generate_v4(),  
 name varchar(120) NOT NULL,  
 description varchar(240)  
 );  
 """  
   
 Material = Table(create=create_table_sql)  
 ```
   
 ### Define a Postgresql Function  
 ```python
+from postnormalism.schema import Function
+
 create_function_sql = """  
 CREATE FUNCTION get_material_for_variant(variant uuid)  
 RETURNS uuid  
 AS $$  
 material_plan = plpy.prepare("SELECT material FROM material_variant WHERE id = $1",  
 ["uuid"])  
 material = plpy.execute(material_plan, [variant])[0]["material"]  
@@ -81,29 +87,37 @@
 COMMENT ON FUNCTION get_material_for_variant IS  
 $$ An example function $$;  
 """  
   
 get_material_for_variant = Function(create=create_function_sql, comment=comment_function_sql)  
 ```  
   
-### Creating Schema Items in a Database  
+### Creating Database Items in a Database  
   
-To create schema items in a PostgreSQL database, use the `create_schema` function from the `postnormalism` module:  
+To create database items in a PostgreSQL database, use the `Database` class:  
   
 ```python  
 import psycopg  
-from postnormalism import create_schema  
+from postnormalism.schema import Database
 from your_example_file import Material, get_material_for_variant
 
-db_connection_string = "dbname=test user=postgres password=secret host=localhost port=5432"  
+universe = Database(
+    load_order=[
+        Material, get_material_for_variant,
+        [Player, Inventory],  # example of grouping DatabaseItems into a transaction
+    ],
+    extensions=['uuid-ossp', 'plpython3u', 'pgcrypto']
+)
+
+db_connection_string = "dbname=test user=postgres password=secret host=localhost port=port"  
 
 connection = psycopg.connect(db_connection_string)  
 cursor = connection.cursor()  
 
-create_schema([Material, get_material_for_variant], cursor)  
+universe.create(cursor)  
 
 connection.commit()  
 connection.close()  
 ```  
 
   
 ## Contributing
```

### Comparing `postnormalism-0.0.1/postnormalism/utils.py` & `postnormalism-0.0.2/postnormalism/utils.py`

 * *Files identical despite different names*

### Comparing `postnormalism-0.0.1/postnormalism.egg-info/PKG-INFO` & `postnormalism-0.0.2/postnormalism.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: postnormalism
-Version: 0.0.1
+Version: 0.0.2
 Summary: Postnormalism is Not an Object Relational Mapper (NORM) it is a lightweight and simple-to-use Python library for managing PostgreSQL database schemas. It provides an easy way to define tables and functions, organize schema items, and create them in a database with a specified load order.
 Author-email: Zac Miller <zac@informatical.info>
 Maintainer-email: Zac Miller <zac@informatical.info>
 License: MIT License
 Project-URL: Homepage, https://github.com/jzmiller1/postnormalism
 Project-URL: Bug Tracker, https://github.com/jzmiller1/postnormalism/issues
 Project-URL: Repository, https://github.com/jzmiller1/postnormalism.git
@@ -22,17 +22,19 @@
 # postnormalism: PostgreSQL Schema Management  
   
 postnormalism is Not an Object Relational Mapper (NORM) it is a lightweight and simple-to-use Python library for managing PostgreSQL database schemas. It provides an easy way to define tables and functions, organize schema items, and create them in a database with a specified load order.  
   
 ## Features  
   
 - Define tables and functions using Python dataclasses  
-- Create schema items (Tables, Functions) with comments
-- Load schema items in a specified load order  
-- Group related schema items and create them within a single transaction  
+- Create database items (Tables, Functions) with comments
+- Group related database items and create them within a single transaction  
+- Create a Database object that allows loading database items in a specified load order and managing database extensions
+- IF NOT EXISTS mode for loading
+
   
 ## NORM vs. ORM: Features Comparison  
   
 postnormalism is a lightweight and simple-to-use Python library for managing PostgreSQL database schemas. It does not possess all the characteristics of a full-fledged ORM, focusing mainly on schema management and organization.  
   
 Here is a comparison of postnormalism's features with typical ORM characteristics:  
   
@@ -60,37 +62,41 @@
   
 ```sh  
 pip install postnormalism  
 ```  
   
 ## Usage  
   
-### Defining Schema Items  
+### Defining Database Items  
   
 To define a table or a function, use the `Table` and `Function` dataclasses from the `postnormalism` module:  
   
 ```python  
-from postnormalism import Table, Function  
+from postnormalism.schema import Table, Function  
 ```
   
 ### Define a Table
 ```python
+from postnormalism.schema import Table
+
 create_table_sql = """  
 CREATE TABLE material (  
 id uuid PRIMARY KEY DEFAULT uuid_generate_v4(),  
 name varchar(120) NOT NULL,  
 description varchar(240)  
 );  
 """  
   
 Material = Table(create=create_table_sql)  
 ```
   
 ### Define a Postgresql Function  
 ```python
+from postnormalism.schema import Function
+
 create_function_sql = """  
 CREATE FUNCTION get_material_for_variant(variant uuid)  
 RETURNS uuid  
 AS $$  
 material_plan = plpy.prepare("SELECT material FROM material_variant WHERE id = $1",  
 ["uuid"])  
 material = plpy.execute(material_plan, [variant])[0]["material"]  
@@ -102,29 +108,37 @@
 COMMENT ON FUNCTION get_material_for_variant IS  
 $$ An example function $$;  
 """  
   
 get_material_for_variant = Function(create=create_function_sql, comment=comment_function_sql)  
 ```  
   
-### Creating Schema Items in a Database  
+### Creating Database Items in a Database  
   
-To create schema items in a PostgreSQL database, use the `create_schema` function from the `postnormalism` module:  
+To create database items in a PostgreSQL database, use the `Database` class:  
   
 ```python  
 import psycopg  
-from postnormalism import create_schema  
+from postnormalism.schema import Database
 from your_example_file import Material, get_material_for_variant
 
-db_connection_string = "dbname=test user=postgres password=secret host=localhost port=5432"  
+universe = Database(
+    load_order=[
+        Material, get_material_for_variant,
+        [Player, Inventory],  # example of grouping DatabaseItems into a transaction
+    ],
+    extensions=['uuid-ossp', 'plpython3u', 'pgcrypto']
+)
+
+db_connection_string = "dbname=test user=postgres password=secret host=localhost port=port"  
 
 connection = psycopg.connect(db_connection_string)  
 cursor = connection.cursor()  
 
-create_schema([Material, get_material_for_variant], cursor)  
+universe.create(cursor)  
 
 connection.commit()  
 connection.close()  
 ```  
 
   
 ## Contributing
```

### Comparing `postnormalism-0.0.1/pyproject.toml` & `postnormalism-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `postnormalism-0.0.1/tests/test_core.py` & `postnormalism-0.0.2/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `postnormalism-0.0.1/tests/test_schema.py` & `postnormalism-0.0.2/tests/test_schema.py`

 * *Files identical despite different names*

