# Comparing `tmp/django_gem-1.0.0.tar.gz` & `tmp/django_gem-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_gem-1.0.0.tar", max compression
+gzip compressed data, was "django_gem-1.0.1.tar", max compression
```

## Comparing `django_gem-1.0.0.tar` & `django_gem-1.0.1.tar`

### file list

```diff
@@ -1,49 +1,53 @@
--rw-r--r--   0        0        0     1067 2023-05-18 18:58:33.968624 django_gem-1.0.0/LICENSE
--rw-r--r--   0        0        0     2785 2023-05-18 18:58:33.968624 django_gem-1.0.0/README.md
--rw-r--r--   0        0        0        0 2023-05-18 18:58:33.972624 django_gem-1.0.0/django_gem/__init__.py
--rw-r--r--   0        0        0      257 2023-05-18 18:58:33.972624 django_gem-1.0.0/django_gem/apps.py
--rw-r--r--   0        0        0      457 2023-05-18 18:58:33.972624 django_gem-1.0.0/django_gem/constants.py
--rw-r--r--   0        0        0      283 2023-05-18 18:58:33.972624 django_gem-1.0.0/django_gem/context.py
--rw-r--r--   0        0        0        0 2023-05-18 18:58:33.972624 django_gem-1.0.0/django_gem/cutters/__init__.py
--rw-r--r--   0        0        0     1026 2023-05-18 18:58:33.972624 django_gem-1.0.0/django_gem/cutters/base.py
--rw-r--r--   0        0        0       54 2023-05-18 18:58:33.972624 django_gem-1.0.0/django_gem/decorators/__init__.py
--rw-r--r--   0        0        0      220 2023-05-18 18:58:33.972624 django_gem-1.0.0/django_gem/decorators/context.py
--rw-r--r--   0        0        0     1104 2023-05-18 18:58:33.972624 django_gem-1.0.0/django_gem/decorators/cutters.py
--rw-r--r--   0        0        0     1536 2023-05-18 18:58:33.972624 django_gem-1.0.0/django_gem/decorators/models.py
--rw-r--r--   0        0        0        0 2023-05-18 18:58:33.972624 django_gem-1.0.0/django_gem/entities/__init__.py
--rw-r--r--   0        0        0      106 2023-05-18 18:58:33.972624 django_gem-1.0.0/django_gem/entities/context.py
--rw-r--r--   0        0        0      737 2023-05-18 18:58:33.972624 django_gem-1.0.0/django_gem/entities/models.py
--rw-r--r--   0        0        0     1544 2023-05-18 18:58:33.972624 django_gem-1.0.0/django_gem/entities/registry.py
--rw-r--r--   0        0        0     1108 2023-05-18 18:58:33.972624 django_gem-1.0.0/django_gem/exceptions.py
--rw-r--r--   0        0        0       58 2023-05-18 18:58:33.972624 django_gem-1.0.0/django_gem/logger.py
--rw-r--r--   0        0        0     2622 2023-05-18 18:58:33.972624 django_gem-1.0.0/django_gem/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-05-18 18:58:33.972624 django_gem-1.0.0/django_gem/migrations/__init__.py
--rw-r--r--   0        0        0       56 2023-05-18 18:58:33.972624 django_gem-1.0.0/django_gem/models/__init__.py
--rw-r--r--   0        0        0     1969 2023-05-18 18:58:33.972624 django_gem-1.0.0/django_gem/models/base.py
--rw-r--r--   0        0        0     1432 2023-05-18 18:58:33.972624 django_gem-1.0.0/django_gem/models/gem_log_entry.py
--rw-r--r--   0        0        0        0 2023-05-18 18:58:33.972624 django_gem-1.0.0/django_gem/models/managers/__init__.py
--rw-r--r--   0        0        0     1297 2023-05-18 18:58:33.972624 django_gem-1.0.0/django_gem/models/managers/gem_log_entry_manager.py
--rw-r--r--   0        0        0     2850 2023-05-18 18:58:33.972624 django_gem-1.0.0/django_gem/models/mixins.py
--rw-r--r--   0        0        0      178 2023-05-18 18:58:33.972624 django_gem-1.0.0/django_gem/overrides/__init__.py
--rw-r--r--   0        0        0     1150 2023-05-18 18:58:33.972624 django_gem-1.0.0/django_gem/overrides/delete.py
--rw-r--r--   0        0        0     1061 2023-05-18 18:58:33.972624 django_gem-1.0.0/django_gem/overrides/m2m_changed.py
--rw-r--r--   0        0        0     1331 2023-05-18 18:58:33.972624 django_gem-1.0.0/django_gem/overrides/save.py
--rw-r--r--   0        0        0      966 2023-05-18 18:58:33.972624 django_gem-1.0.0/django_gem/overrides/utils.py
--rw-r--r--   0        0        0      184 2023-05-18 18:58:33.972624 django_gem-1.0.0/django_gem/tasks/__init__.py
--rw-r--r--   0        0        0      243 2023-05-18 18:58:33.972624 django_gem-1.0.0/django_gem/tasks/cut_content_type.py
--rw-r--r--   0        0        0      187 2023-05-18 18:58:33.972624 django_gem-1.0.0/django_gem/tasks/cut_models.py
--rw-r--r--   0        0        0      229 2023-05-18 18:58:33.972624 django_gem-1.0.0/django_gem/tasks/cut_queryset.py
--rw-r--r--   0        0        0      251 2023-05-18 18:58:33.972624 django_gem-1.0.0/django_gem/toolkit/__init__.py
--rw-r--r--   0        0        0       57 2023-05-18 18:58:33.972624 django_gem-1.0.0/django_gem/toolkit/anvils/__init__.py
--rw-r--r--   0        0        0      100 2023-05-18 18:58:33.972624 django_gem-1.0.0/django_gem/toolkit/anvils/base.py
--rw-r--r--   0        0        0      272 2023-05-18 18:58:33.976624 django_gem-1.0.0/django_gem/toolkit/anvils/celery.py
--rw-r--r--   0        0        0      256 2023-05-18 18:58:33.976624 django_gem-1.0.0/django_gem/toolkit/anvils/eager.py
--rw-r--r--   0        0        0     2690 2023-05-18 18:58:33.976624 django_gem-1.0.0/django_gem/toolkit/chest.py
--rw-r--r--   0        0        0     5072 2023-05-18 18:58:33.976624 django_gem-1.0.0/django_gem/toolkit/forge.py
--rw-r--r--   0        0        0     7332 2023-05-18 18:58:33.976624 django_gem-1.0.0/django_gem/toolkit/registry.py
--rw-r--r--   0        0        0     4600 2023-05-18 18:58:33.976624 django_gem-1.0.0/django_gem/toolkit/saw.py
--rw-r--r--   0        0        0     1287 2023-05-18 18:58:33.976624 django_gem-1.0.0/django_gem/toolkit/settings.py
--rw-r--r--   0        0        0     1615 2023-05-18 18:58:33.976624 django_gem-1.0.0/django_gem/toolkit/smith.py
--rw-r--r--   0        0        0     4198 2023-05-18 18:58:33.976624 django_gem-1.0.0/django_gem/validators.py
--rw-r--r--   0        0        0      811 2023-05-18 18:58:33.980624 django_gem-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3503 1970-01-01 00:00:00.000000 django_gem-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-20 18:44:48.474899 django_gem-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2786 2023-05-20 18:44:48.474899 django_gem-1.0.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-20 18:44:48.474899 django_gem-1.0.1/django_gem/__init__.py
+-rw-r--r--   0        0        0      257 2023-05-20 18:44:48.474899 django_gem-1.0.1/django_gem/apps.py
+-rw-r--r--   0        0        0      457 2023-05-20 18:44:48.474899 django_gem-1.0.1/django_gem/constants.py
+-rw-r--r--   0        0        0      283 2023-05-20 18:44:48.474899 django_gem-1.0.1/django_gem/context.py
+-rw-r--r--   0        0        0        0 2023-05-20 18:44:48.474899 django_gem-1.0.1/django_gem/cutters/__init__.py
+-rw-r--r--   0        0        0     1026 2023-05-20 18:44:48.474899 django_gem-1.0.1/django_gem/cutters/base.py
+-rw-r--r--   0        0        0       54 2023-05-20 18:44:48.474899 django_gem-1.0.1/django_gem/decorators/__init__.py
+-rw-r--r--   0        0        0      220 2023-05-20 18:44:48.474899 django_gem-1.0.1/django_gem/decorators/context.py
+-rw-r--r--   0        0        0     1104 2023-05-20 18:44:48.474899 django_gem-1.0.1/django_gem/decorators/cutters.py
+-rw-r--r--   0        0        0     1536 2023-05-20 18:44:48.474899 django_gem-1.0.1/django_gem/decorators/models.py
+-rw-r--r--   0        0        0        0 2023-05-20 18:44:48.474899 django_gem-1.0.1/django_gem/entities/__init__.py
+-rw-r--r--   0        0        0      106 2023-05-20 18:44:48.474899 django_gem-1.0.1/django_gem/entities/context.py
+-rw-r--r--   0        0        0      737 2023-05-20 18:44:48.474899 django_gem-1.0.1/django_gem/entities/models.py
+-rw-r--r--   0        0        0     1544 2023-05-20 18:44:48.474899 django_gem-1.0.1/django_gem/entities/registry.py
+-rw-r--r--   0        0        0     1108 2023-05-20 18:44:48.474899 django_gem-1.0.1/django_gem/exceptions.py
+-rw-r--r--   0        0        0       58 2023-05-20 18:44:48.474899 django_gem-1.0.1/django_gem/logger.py
+-rw-r--r--   0        0        0        0 2023-05-20 18:44:48.474899 django_gem-1.0.1/django_gem/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-20 18:44:48.474899 django_gem-1.0.1/django_gem/management/commands/__init__.py
+-rw-r--r--   0        0        0     1042 2023-05-20 18:44:48.474899 django_gem-1.0.1/django_gem/management/commands/cutmodel.py
+-rw-r--r--   0        0        0     1090 2023-05-20 18:44:48.474899 django_gem-1.0.1/django_gem/management/commands/cutqueryset.py
+-rw-r--r--   0        0        0     2622 2023-05-20 18:44:48.474899 django_gem-1.0.1/django_gem/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-05-20 18:44:48.474899 django_gem-1.0.1/django_gem/migrations/__init__.py
+-rw-r--r--   0        0        0       56 2023-05-20 18:44:48.474899 django_gem-1.0.1/django_gem/models/__init__.py
+-rw-r--r--   0        0        0     1969 2023-05-20 18:44:48.474899 django_gem-1.0.1/django_gem/models/base.py
+-rw-r--r--   0        0        0     1432 2023-05-20 18:44:48.474899 django_gem-1.0.1/django_gem/models/gem_log_entry.py
+-rw-r--r--   0        0        0        0 2023-05-20 18:44:48.478899 django_gem-1.0.1/django_gem/models/managers/__init__.py
+-rw-r--r--   0        0        0     1297 2023-05-20 18:44:48.478899 django_gem-1.0.1/django_gem/models/managers/gem_log_entry_manager.py
+-rw-r--r--   0        0        0     2850 2023-05-20 18:44:48.478899 django_gem-1.0.1/django_gem/models/mixins.py
+-rw-r--r--   0        0        0      178 2023-05-20 18:44:48.478899 django_gem-1.0.1/django_gem/overrides/__init__.py
+-rw-r--r--   0        0        0     1150 2023-05-20 18:44:48.478899 django_gem-1.0.1/django_gem/overrides/delete.py
+-rw-r--r--   0        0        0     1061 2023-05-20 18:44:48.478899 django_gem-1.0.1/django_gem/overrides/m2m_changed.py
+-rw-r--r--   0        0        0     1522 2023-05-20 18:44:48.478899 django_gem-1.0.1/django_gem/overrides/save.py
+-rw-r--r--   0        0        0      966 2023-05-20 18:44:48.478899 django_gem-1.0.1/django_gem/overrides/utils.py
+-rw-r--r--   0        0        0      184 2023-05-20 18:44:48.478899 django_gem-1.0.1/django_gem/tasks/__init__.py
+-rw-r--r--   0        0        0      243 2023-05-20 18:44:48.478899 django_gem-1.0.1/django_gem/tasks/cut_content_type.py
+-rw-r--r--   0        0        0      187 2023-05-20 18:44:48.478899 django_gem-1.0.1/django_gem/tasks/cut_models.py
+-rw-r--r--   0        0        0      229 2023-05-20 18:44:48.478899 django_gem-1.0.1/django_gem/tasks/cut_queryset.py
+-rw-r--r--   0        0        0      251 2023-05-20 18:44:48.478899 django_gem-1.0.1/django_gem/toolkit/__init__.py
+-rw-r--r--   0        0        0       57 2023-05-20 18:44:48.478899 django_gem-1.0.1/django_gem/toolkit/anvils/__init__.py
+-rw-r--r--   0        0        0      100 2023-05-20 18:44:48.478899 django_gem-1.0.1/django_gem/toolkit/anvils/base.py
+-rw-r--r--   0        0        0      272 2023-05-20 18:44:48.478899 django_gem-1.0.1/django_gem/toolkit/anvils/celery.py
+-rw-r--r--   0        0        0      256 2023-05-20 18:44:48.478899 django_gem-1.0.1/django_gem/toolkit/anvils/eager.py
+-rw-r--r--   0        0        0     2690 2023-05-20 18:44:48.478899 django_gem-1.0.1/django_gem/toolkit/chest.py
+-rw-r--r--   0        0        0     5072 2023-05-20 18:44:48.478899 django_gem-1.0.1/django_gem/toolkit/forge.py
+-rw-r--r--   0        0        0     7332 2023-05-20 18:44:48.478899 django_gem-1.0.1/django_gem/toolkit/registry.py
+-rw-r--r--   0        0        0     4600 2023-05-20 18:44:48.478899 django_gem-1.0.1/django_gem/toolkit/saw.py
+-rw-r--r--   0        0        0     1328 2023-05-20 18:44:48.478899 django_gem-1.0.1/django_gem/toolkit/settings.py
+-rw-r--r--   0        0        0     1615 2023-05-20 18:44:48.478899 django_gem-1.0.1/django_gem/toolkit/smith.py
+-rw-r--r--   0        0        0     4198 2023-05-20 18:44:48.478899 django_gem-1.0.1/django_gem/validators.py
+-rw-r--r--   0        0        0      811 2023-05-20 18:44:48.478899 django_gem-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3504 1970-01-01 00:00:00.000000 django_gem-1.0.1/PKG-INFO
```

### Comparing `django_gem-1.0.0/LICENSE` & `django_gem-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.0/README.md` & `django_gem-1.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Django Gem
 
 Django-gem is a reusable Django package that allows user to offload on-the-fly calculations
-for Django models by putting the into database and providing and easy to use architecture to define,
+for Django models by putting them into database and providing and easy to use architecture to define,
 how and when those database fields need to be refreshed.
 
 ### Installation
 
 ---
 Using `pip`
 <pre>pip install django-gem</pre>
```

### Comparing `django_gem-1.0.0/django_gem/cutters/base.py` & `django_gem-1.0.1/django_gem/cutters/base.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.0/django_gem/decorators/cutters.py` & `django_gem-1.0.1/django_gem/decorators/cutters.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.0/django_gem/decorators/models.py` & `django_gem-1.0.1/django_gem/decorators/models.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.0/django_gem/entities/models.py` & `django_gem-1.0.1/django_gem/entities/models.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.0/django_gem/entities/registry.py` & `django_gem-1.0.1/django_gem/entities/registry.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.0/django_gem/exceptions.py` & `django_gem-1.0.1/django_gem/exceptions.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.0/django_gem/migrations/0001_initial.py` & `django_gem-1.0.1/django_gem/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.0/django_gem/models/base.py` & `django_gem-1.0.1/django_gem/models/base.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.0/django_gem/models/gem_log_entry.py` & `django_gem-1.0.1/django_gem/models/gem_log_entry.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.0/django_gem/models/managers/gem_log_entry_manager.py` & `django_gem-1.0.1/django_gem/models/managers/gem_log_entry_manager.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.0/django_gem/models/mixins.py` & `django_gem-1.0.1/django_gem/models/mixins.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.0/django_gem/overrides/delete.py` & `django_gem-1.0.1/django_gem/overrides/delete.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.0/django_gem/overrides/m2m_changed.py` & `django_gem-1.0.1/django_gem/overrides/m2m_changed.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.0/django_gem/overrides/save.py` & `django_gem-1.0.1/django_gem/overrides/save.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,25 +17,31 @@
         gem_cutting_enabled = gem_settings.GEM_CUTTING_ENABLED
 
         should_cut = True
         if isinstance(self, GemCutConditionalMixin):
             should_cut = self.should_cut_on_save(*args, **kwargs)
 
         with transaction.atomic():
+            prepared_cut_batch_items = []
             changed_cut_batch_items = []
             if should_cut:
-                for cut_batch_item in cut_batch_items:
-                    cut_batch_item.load_object_ids(self)
-                    if is_cutting_needed(self, cut_batch_item.affected_fields):
-                        changed_cut_batch_items.append(cut_batch_item)
+                prepared_cut_batch_items = [
+                    cut_batch_item
+                    for cut_batch_item in cut_batch_items
+                    if is_cutting_needed(self, cut_batch_item.affected_fields)
+                ]
 
             save_func(self, *args, **kwargs)
             if not gem_cutting_enabled or not should_cut:
                 return
 
+            for cut_batch_item in prepared_cut_batch_items:
+                cut_batch_item.load_object_ids(self)
+                changed_cut_batch_items.append(cut_batch_item)
+
             add_cut_items(smith, changed_cut_batch_items)
 
             transaction.on_commit(
                 lambda: smith.initiate_cutting(),
             )
 
     return wrapped_trigger
```

### Comparing `django_gem-1.0.0/django_gem/overrides/utils.py` & `django_gem-1.0.1/django_gem/overrides/utils.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.0/django_gem/toolkit/chest.py` & `django_gem-1.0.1/django_gem/toolkit/chest.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.0/django_gem/toolkit/forge.py` & `django_gem-1.0.1/django_gem/toolkit/forge.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.0/django_gem/toolkit/registry.py` & `django_gem-1.0.1/django_gem/toolkit/registry.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.0/django_gem/toolkit/saw.py` & `django_gem-1.0.1/django_gem/toolkit/saw.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.0/django_gem/toolkit/settings.py` & `django_gem-1.0.1/django_gem/toolkit/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,17 @@
     CUTTER_MODEL_RELATED_NAME = "cutter_target"
     CUTTER_PROPAGATED_TRIGGERS_MAX_DEPTH = 10
     GEM_IGNORED_FIELDS = []
     GEM_CUTTING_ENABLED = True
     GEM_ANVILS = []
 
     def __init__(self):
+        self.load()
+
+    def load(self):
         if hasattr(settings, "CUTTER_PROPERTY_PREFIX"):
             self.CUTTER_PROPERTY_PREFIX = settings.CUTTER_PROPERTY_PREFIX
         if hasattr(settings, "CUTTER_PROPAGATED_TRIGGERS_MAX_DEPTH"):
             self.CUTTER_PROPAGATED_TRIGGERS_MAX_DEPTH = (
                 settings.CUTTER_PROPAGATED_TRIGGERS_MAX_DEPTH
             )
         if hasattr(settings, "CUTTER_MODEL_RELATED_NAME"):
```

### Comparing `django_gem-1.0.0/django_gem/toolkit/smith.py` & `django_gem-1.0.1/django_gem/toolkit/smith.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.0/django_gem/validators.py` & `django_gem-1.0.1/django_gem/validators.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.0/pyproject.toml` & `django_gem-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 profile = "black"
 
 [tool.black]
 line-length = 100
 
 [tool.poetry]
 name = "django-gem"
-version = "1.0.0"
+version = "1.0.1"
 description = "Distrubited calculations for Django models"
 authors = ["Artur Veres <artur8118@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "django_gem"}]
 
 [tool.poetry.dependencies]
```

### Comparing `django_gem-1.0.0/PKG-INFO` & `django_gem-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-gem
-Version: 1.0.0
+Version: 1.0.1
 Summary: Distrubited calculations for Django models
 License: MIT
 Author: Artur Veres
 Author-email: artur8118@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -17,15 +17,15 @@
 Requires-Dist: django-crum (>=0.7.9,<0.8.0)
 Requires-Dist: django-dirtyfields (>=1.9.2,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Django Gem
 
 Django-gem is a reusable Django package that allows user to offload on-the-fly calculations
-for Django models by putting the into database and providing and easy to use architecture to define,
+for Django models by putting them into database and providing and easy to use architecture to define,
 how and when those database fields need to be refreshed.
 
 ### Installation
 
 ---
 Using `pip`
 <pre>pip install django-gem</pre>
```

