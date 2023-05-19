# Comparing `tmp/django_view_manager-1.0.1-py3-none-any.whl.zip` & `tmp/django_view_manager-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 11287 bytes, number of entries: 11
--rw-r--r--  2.0 unx        0 b- defN 23-May-05 22:06 django_view_manager/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-05 22:06 django_view_manager/utils/__init__.py
--rw-r--r--  2.0 unx      132 b- defN 23-May-05 22:06 django_view_manager/utils/apps.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-05 22:06 django_view_manager/utils/management/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-05 22:06 django_view_manager/utils/management/commands/__init__.py
--rw-r--r--  2.0 unx    20602 b- defN 23-May-05 22:06 django_view_manager/utils/management/commands/makeviewmigration.py
--rw-r--r--  2.0 unx     1504 b- defN 23-May-05 22:06 django_view_manager-1.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx    13800 b- defN 23-May-05 22:06 django_view_manager-1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-05 22:06 django_view_manager-1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       20 b- defN 23-May-05 22:06 django_view_manager-1.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1049 b- defN 23-May-05 22:06 django_view_manager-1.0.1.dist-info/RECORD
-11 files, 37199 bytes uncompressed, 9447 bytes compressed:  74.6%
+Zip file size: 11301 bytes, number of entries: 11
+-rw-r--r--  2.0 unx        0 b- defN 23-May-19 22:12 django_view_manager/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-19 22:12 django_view_manager/utils/__init__.py
+-rw-r--r--  2.0 unx      132 b- defN 23-May-19 22:12 django_view_manager/utils/apps.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-19 22:12 django_view_manager/utils/management/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-19 22:12 django_view_manager/utils/management/commands/__init__.py
+-rw-r--r--  2.0 unx    20250 b- defN 23-May-19 22:12 django_view_manager/utils/management/commands/makeviewmigration.py
+-rw-r--r--  2.0 unx     1504 b- defN 23-May-19 22:12 django_view_manager-1.0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx    13963 b- defN 23-May-19 22:12 django_view_manager-1.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-19 22:12 django_view_manager-1.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       20 b- defN 23-May-19 22:12 django_view_manager-1.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1049 b- defN 23-May-19 22:12 django_view_manager-1.0.2.dist-info/RECORD
+11 files, 37010 bytes uncompressed, 9461 bytes compressed:  74.4%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: django_view_manager/utils/management/commands/__init__.py
 Comment: 
 
 Filename: django_view_manager/utils/management/commands/makeviewmigration.py
 Comment: 
 
-Filename: django_view_manager-1.0.1.dist-info/LICENSE
+Filename: django_view_manager-1.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: django_view_manager-1.0.1.dist-info/METADATA
+Filename: django_view_manager-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: django_view_manager-1.0.1.dist-info/WHEEL
+Filename: django_view_manager-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: django_view_manager-1.0.1.dist-info/top_level.txt
+Filename: django_view_manager-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: django_view_manager-1.0.1.dist-info/RECORD
+Filename: django_view_manager-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## django_view_manager/utils/management/commands/makeviewmigration.py

```diff
@@ -7,36 +7,39 @@
 from django.apps import apps
 from django.core.management import BaseCommand
 from django.core.management import call_command
 from django.db import migrations
 from django.db.transaction import atomic
 
 
-COPIED_SQL_VIEW_CONTENT = """/*
-    This file was generated using django-view-manager {version}.
+VERSION = "1.0.2"
+
+
+COPIED_SQL_VIEW_CONTENT = f"""/*
+    This file was generated using django-view-manager {VERSION}.
     Modify the SQL for this view and then commit the changes.
     You can remove this comment before committing.
 
     When you have changes to make to this sql, you need to run the makeviewmigration command
     before altering the sql, so the historical sql file is created with the correct contents.
 */
 """
 
-INITIAL_SQL_VIEW_CONTENT = """/*
-    This file was generated using django-view-manager {version}.
+INITIAL_SQL_VIEW_CONTENT = f"""/*
+    This file was generated using django-view-manager {VERSION}.
     Add the SQL for this view and then commit the changes.
     You can remove this comment before committing.
 
     When you have changes to make to this sql, you need to run the makeviewmigration command
     before altering the sql, so the historical sql file is created with the correct contents.
 
     eg.
-    DROP VIEW IF EXISTS {view_name};
+    DROP VIEW IF EXISTS {{view_name}};
     CREATE VIEW
-        {view_name} AS
+        {{view_name}} AS
     SELECT
         1 AS id,
         42 AS employee_id,
         'Kittens' AS name
     UNION
         2 AS id,
         314 AS employee_id,
@@ -44,15 +47,15 @@
 */
 """
 
 LATEST_VIEW_NAME = "latest"
 LATEST_VIEW_NUMBER = decimal.Decimal("Infinity")
 
 # Add a comment right after the Django generated comment, to help find our modified migrations.
-MIGRATION_MODIFIED_COMMENT = "# Modified using django-view-manager {version}.  Please do not delete this comment.\n"
+MIGRATION_MODIFIED_COMMENT = f"# Modified using django-view-manager {VERSION}.  Please do not delete this comment.\n"
 
 
 class Command(BaseCommand):
     help = (  # noqa: A003
         "In the appropriate app, two files will get created. "
         "`sql/view-view_name-0000.sql` - contains the SQL for the view. "
         "`migrations/0000_view_name.py` - a migration that reads the appropriate files in the sql folder. "
@@ -89,19 +92,14 @@
 
         parser.add_argument(
             "migration_name",
             action="store",
             help="The name of the migration that will be created.",
         )
 
-    @staticmethod
-    def _get_our_version_number():
-        with open("VERSION", "r") as f:
-            return f.read().strip()
-
     def _call_command(self, *args):
         err = io.StringIO()
         out = io.StringIO()
 
         # If we don't do this, sometimes we can't import a newly created migration.
         # Do it here, so we don't need to know which calls require it, and which don't.
         importlib.invalidate_caches()
@@ -274,24 +272,24 @@
             content = f_in.read()
             with open(os.path.join(sql_path, historical_sql_filename), "w", encoding="utf-8") as f_out:
                 f_out.write(content)
 
             if "This file was generated using django-view-manager" not in content:
                 f_in.seek(0)
                 f_in.truncate()
-                f_in.write(COPIED_SQL_VIEW_CONTENT.format(version=self._get_our_version_number()))
+                f_in.write(COPIED_SQL_VIEW_CONTENT)
                 f_in.write(content)
 
         self.stdout.write(self.style.SUCCESS(f"\nCreated historical SQL view file - '{historical_sql_filename}'."))
 
     def _create_latest_sql_file(self, sql_path, db_table_name):
         latest_sql_filename = f"view-{db_table_name}-{LATEST_VIEW_NAME}.sql"
 
         with open(os.path.join(sql_path, latest_sql_filename), "w", encoding="utf-8") as f:
-            f.write(INITIAL_SQL_VIEW_CONTENT.format(version=self._get_our_version_number(), view_name=db_table_name))
+            f.write(INITIAL_SQL_VIEW_CONTENT.format(view_name=db_table_name))
 
         self.stdout.write(self.style.SUCCESS(f"\nCreated new SQL view file - '{latest_sql_filename}'."))
 
     def _rewrite_latest_migration(self, migrations_path, migration_name, latest_sql_filename, historical_sql_filename):
         with open(os.path.join(migrations_path, migration_name + ".py"), "r+", encoding="utf-8") as f:
             lines = f.readlines()
             generated_line_no = latest_sql_line_no = 0
@@ -304,17 +302,15 @@
                         add_modified_message = True
                 elif line.find(latest_sql_filename) != -1:
                     latest_sql_line_no = line_no
             # We write lines starting from the bottom to the top, so our line numbers are correct through the process.
             lines[latest_sql_line_no] = lines[latest_sql_line_no].replace(latest_sql_filename, historical_sql_filename)
             if add_modified_message:
                 # Insert the modified comment after the Django generated comment.
-                lines[generated_line_no + 1 : generated_line_no + 1] = MIGRATION_MODIFIED_COMMENT.format(
-                    version=self._get_our_version_number()
-                )
+                lines[generated_line_no + 1 : generated_line_no + 1] = MIGRATION_MODIFIED_COMMENT
             f.seek(0)
             f.truncate(0)
             f.writelines(lines)
 
     def _rewrite_migration(
         self,
         migrations_path,
@@ -363,17 +359,15 @@
                 "\n" if reverse_sql_filename else "",
             ]
             lines[imports_line_no - 1 : imports_line_no] = [
                 "import os\n",
                 "\n",
             ]
             # Insert the generated comment at the top.
-            lines[generated_line_no + 1 : generated_line_no + 1] = [
-                MIGRATION_MODIFIED_COMMENT.format(version=self._get_our_version_number())
-            ]
+            lines[generated_line_no + 1 : generated_line_no + 1] = [MIGRATION_MODIFIED_COMMENT]
             f.seek(0)
             f.writelines(lines)
 
     @atomic
     def handle(self, *args, **options):
         # Get passed in args.
         db_table_name = options["db_table_name"]
```

## Comparing `django_view_manager-1.0.1.dist-info/LICENSE` & `django_view_manager-1.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `django_view_manager-1.0.1.dist-info/METADATA` & `django_view_manager-1.0.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-view-manager
-Version: 1.0.1
+Version: 1.0.2
 Summary: A management command for django that provides diffs of sql views.
 Author-email: Arrai Innovations <support@arrai.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Arrai Innovations
         
         Redistribution and use in source and binary forms, with or without
@@ -105,17 +105,25 @@
 
 or
 
 ```shell
 $ pipenv install django-view-manager
 ```
 
-# Requirements
+Add `django-view-manager.utils` to the INSTALLED_APPS in settings. If possible, do this in your development settings only, as you don't need this package on a production server.
+
+```python
+INSTALLED_APPS = [
+    ...
+    "django-view-manager.utils",
+    ...
+]
+```
 
-A `Pipfile` and `dev_requirements.txt` exist for convenience. You can choose which you want to use.
+# Requirements
 
 At least a django 3.2 and python 3.7.
 
 It may work in an older django, but we only test against supported versions.
 
 # Folder and File Structure
```

## Comparing `django_view_manager-1.0.1.dist-info/RECORD` & `django_view_manager-1.0.2.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 django_view_manager/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 django_view_manager/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 django_view_manager/utils/apps.py,sha256=fZoo89eHKqypCLKzeFxUNkGrHTBs4sWGm3ZcLDDGTi8,132
 django_view_manager/utils/management/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 django_view_manager/utils/management/commands/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-django_view_manager/utils/management/commands/makeviewmigration.py,sha256=KCwaSr5YkxOgWmuobiTgqjdRS5mTJsricHGUlSRhKK8,20602
-django_view_manager-1.0.1.dist-info/LICENSE,sha256=C9Y-Cr2GS0AyKcVDN7Gwj4DjjYTUdCUrFDeASp8C8fA,1504
-django_view_manager-1.0.1.dist-info/METADATA,sha256=KnedL-RzfPDhnOkhlKxm4tk0e0KH9CvLd0eI9IPgYP0,13800
-django_view_manager-1.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-django_view_manager-1.0.1.dist-info/top_level.txt,sha256=WaJvRmbbOJ7HI_7RuTxUSjULO_00vrBXScnfiFteTT8,20
-django_view_manager-1.0.1.dist-info/RECORD,,
+django_view_manager/utils/management/commands/makeviewmigration.py,sha256=48ZzxgcXiXrHWgUNmdXpSncGpOOVvW7maqhL5SwEK2E,20250
+django_view_manager-1.0.2.dist-info/LICENSE,sha256=C9Y-Cr2GS0AyKcVDN7Gwj4DjjYTUdCUrFDeASp8C8fA,1504
+django_view_manager-1.0.2.dist-info/METADATA,sha256=XFt6tQVLOwiEEvwHs5y9ztKjPBJCzfwmKASxS32mXjs,13963
+django_view_manager-1.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+django_view_manager-1.0.2.dist-info/top_level.txt,sha256=WaJvRmbbOJ7HI_7RuTxUSjULO_00vrBXScnfiFteTT8,20
+django_view_manager-1.0.2.dist-info/RECORD,,
```

