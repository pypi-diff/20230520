# Comparing `tmp/oarepo-model-builder-tests-3.1.4.tar.gz` & `tmp/oarepo-model-builder-tests-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-model-builder-tests-3.1.4.tar", last modified: Wed Mar 22 10:28:43 2023, max compression
+gzip compressed data, was "oarepo-model-builder-tests-4.0.0.tar", last modified: Sat May 20 12:46:47 2023, max compression
```

## Comparing `oarepo-model-builder-tests-3.1.4.tar` & `oarepo-model-builder-tests-4.0.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 10:28:43.840271 oarepo-model-builder-tests-3.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-03-22 10:26:58.000000 oarepo-model-builder-tests-3.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-22 10:26:58.000000 oarepo-model-builder-tests-3.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-03-22 10:28:43.840271 oarepo-model-builder-tests-3.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-03-22 10:26:58.000000 oarepo-model-builder-tests-3.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 10:28:43.836271 oarepo-model-builder-tests-3.1.4/oarepo_model_builder_tests/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-03-22 10:26:58.000000 oarepo-model-builder-tests-3.1.4/oarepo_model_builder_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-03-22 10:26:58.000000 oarepo-model-builder-tests-3.1.4/oarepo_model_builder_tests/conftest_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-03-22 10:26:58.000000 oarepo-model-builder-tests-3.1.4/oarepo_model_builder_tests/oarepo_model_builder_setup_cfg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 10:28:43.840271 oarepo-model-builder-tests-3.1.4/oarepo_model_builder_tests/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 10:26:58.000000 oarepo-model-builder-tests-3.1.4/oarepo_model_builder_tests/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-03-22 10:26:58.000000 oarepo-model-builder-tests-3.1.4/oarepo_model_builder_tests/templates/conftest.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     8928 2023-03-22 10:26:58.000000 oarepo-model-builder-tests-3.1.4/oarepo_model_builder_tests/templates/test_resource.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-03-22 10:26:58.000000 oarepo-model-builder-tests-3.1.4/oarepo_model_builder_tests/templates/test_service.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-03-22 10:26:58.000000 oarepo-model-builder-tests-3.1.4/oarepo_model_builder_tests/templates/utils.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-03-22 10:26:58.000000 oarepo-model-builder-tests-3.1.4/oarepo_model_builder_tests/test_resource_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-03-22 10:26:58.000000 oarepo-model-builder-tests-3.1.4/oarepo_model_builder_tests/test_service_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-03-22 10:26:58.000000 oarepo-model-builder-tests-3.1.4/oarepo_model_builder_tests/utils_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 10:28:43.840271 oarepo-model-builder-tests-3.1.4/oarepo_model_builder_tests/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-03-22 10:26:58.000000 oarepo-model-builder-tests-3.1.4/oarepo_model_builder_tests/validation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 10:28:43.840271 oarepo-model-builder-tests-3.1.4/oarepo_model_builder_tests.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-03-22 10:28:43.000000 oarepo-model-builder-tests-3.1.4/oarepo_model_builder_tests.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-03-22 10:28:43.000000 oarepo-model-builder-tests-3.1.4/oarepo_model_builder_tests.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 10:28:43.000000 oarepo-model-builder-tests-3.1.4/oarepo_model_builder_tests.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-03-22 10:28:43.000000 oarepo-model-builder-tests-3.1.4/oarepo_model_builder_tests.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-22 10:28:43.000000 oarepo-model-builder-tests-3.1.4/oarepo_model_builder_tests.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-22 10:28:43.000000 oarepo-model-builder-tests-3.1.4/oarepo_model_builder_tests.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-22 10:26:58.000000 oarepo-model-builder-tests-3.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-03-22 10:28:43.840271 oarepo-model-builder-tests-3.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-22 10:26:58.000000 oarepo-model-builder-tests-3.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:46:47.601999 oarepo-model-builder-tests-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-20 12:42:46.000000 oarepo-model-builder-tests-4.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-20 12:42:46.000000 oarepo-model-builder-tests-4.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-20 12:46:47.601999 oarepo-model-builder-tests-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-20 12:42:46.000000 oarepo-model-builder-tests-4.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:46:47.601999 oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-20 12:42:46.000000 oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-20 12:42:46.000000 oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests/conftest_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:46:47.601999 oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 12:42:46.000000 oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests/datatypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-20 12:42:46.000000 oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests/datatypes/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-20 12:42:46.000000 oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests/oarepo_model_builder_setup_cfg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:46:47.601999 oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 12:42:46.000000 oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-05-20 12:42:46.000000 oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests/templates/conftest.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     9052 2023-05-20 12:42:46.000000 oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests/templates/test_resource.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-05-20 12:42:46.000000 oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests/templates/test_service.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-20 12:42:46.000000 oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests/templates/utils.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-20 12:42:46.000000 oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests/test_resource_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-20 12:42:46.000000 oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests/test_service_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-20 12:42:46.000000 oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests/utils_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:46:47.601999 oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-20 12:46:47.000000 oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-20 12:46:47.000000 oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 12:46:47.000000 oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-20 12:46:47.000000 oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-20 12:46:47.000000 oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-20 12:46:47.000000 oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-20 12:42:46.000000 oarepo-model-builder-tests-4.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-20 12:46:47.601999 oarepo-model-builder-tests-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-20 12:42:46.000000 oarepo-model-builder-tests-4.0.0/setup.py
```

### Comparing `oarepo-model-builder-tests-3.1.4/LICENSE` & `oarepo-model-builder-tests-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-tests-3.1.4/PKG-INFO` & `oarepo-model-builder-tests-4.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-tests
-Version: 3.1.4
+Version: 4.0.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # OARepo model builder tests
 Plugin for oarepo-model-builder to generate 
 test files and add test dependencies.
 The record service and its rest api are covered for now. Tests read, write,
```

### Comparing `oarepo-model-builder-tests-3.1.4/README.md` & `oarepo-model-builder-tests-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-tests-3.1.4/oarepo_model_builder_tests/templates/conftest.py.jinja2` & `oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests/templates/conftest.py.jinja2`

 * *Files 12% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 from flask_security.utils import hash_password
 from invenio_accounts.proxies import current_datastore
 from invenio_accounts.testutils import login_user_via_session
 from invenio_app.factory import create_api
 from invenio_records_resources.services.uow import UnitOfWork, RecordCommitOp
 import os
 
-from {{ schema.model.proxies_current_service|package_name }} import {{ schema.model.proxies_current_service|base_name }}
-from {{ schema.model.record_class|package_name }} import {{ schema.model.record_class|base_name }}
+from {{ vars.proxy.module }} import {{ vars.service.proxy }}
+{{ vars.record.class|generate_import }}
 
 
 @pytest.fixture(scope="function")
 def sample_metadata_list():
-    data_path = f"{Path(__file__).parent.parent}/data/sample_data.yaml"
+    data_path = f"{Path(__file__).parent.parent}/{{ vars.sample.file }}"
     docs = list(yaml.load_all(open(data_path), Loader=yaml.SafeLoader))
     return docs
 
 @pytest.fixture()
 def input_data(sample_metadata_list):
     return sample_metadata_list[0]
 
@@ -44,37 +44,40 @@
     app_config["RATELIMIT_AUTHENTICATED_USER"] = "200 per second"
     app_config["SEARCH_HOSTS"] = [
         {
             'host': os.environ.get('OPENSEARCH_HOST', 'localhost'),
             'port': os.environ.get('OPENSEARCH_PORT', '9200'),
         }
     ]
+    # disable redis cache
+    app_config["CACHE_TYPE"] = "SimpleCache"  # Flask-Caching related configs
+    app_config["CACHE_DEFAULT_TIMEOUT"] = 300
     return app_config
 
 
 @pytest.fixture(scope="function")
 def sample_record(app, db, input_data):
-    # record = current_service.create(system_identity, sample_data[0])
+    # record = {{ vars.service.proxy }}.create(system_identity, sample_data[0])
     # return record
     with UnitOfWork(db.session) as uow:
-        record = {{ schema.model.record_class|base_name }}.create(input_data)
-        uow.register(RecordCommitOp(record, current_service.indexer, True))
+        record = {{ vars.record.class|base_name }}.create(input_data)
+        uow.register(RecordCommitOp(record, {{ vars.service.proxy }}.indexer, True))
         uow.commit()
         return record
 
 
 @pytest.fixture(scope="function")
 def sample_records(app, db, sample_metadata_list):
-    # record = current_service.create(system_identity, sample_data[0])
+    # record = {{ vars.service.proxy }}.create(system_identity, sample_data[0])
     # return record
     with UnitOfWork(db.session) as uow:
         records = []
         for sample_metadata in sample_metadata_list:
-            record = {{ schema.model.record_class|base_name }}.create(sample_metadata)
-            uow.register(RecordCommitOp(record, current_service.indexer, True))
+            record = {{ vars.record.class|base_name }}.create(sample_metadata)
+            uow.register(RecordCommitOp(record, {{ vars.service.proxy }}.indexer, True))
             records.append(record)
         uow.commit()
         return records
 
 
 @pytest.fixture()
 def user(app, db):
@@ -108,8 +111,10 @@
     current_datastore.add_role_to_user(user, role)
     action = current_access.actions["superuser-access"]
     db.session.add(ActionUsers.allow(action, user_id=user.id))
 
     login_user(user, remember=True)
     login_user_via_session(client, email=user.email)
 
-    return client
+    return client
+
+{{ vars.tests.extra_code }}
```

### Comparing `oarepo-model-builder-tests-3.1.4/oarepo_model_builder_tests/templates/test_resource.py.jinja2` & `oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests/templates/test_resource.py.jinja2`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+import pytest
 import datetime
 from invenio_records.dictutils import dict_lookup
-from {{ schema.model.record_resource_config_class|package_name }} import {{ schema.model.record_resource_config_class|base_name }}
-from {{ schema.model.proxies_current_service|package_name }} import {{ schema.model.proxies_current_service|base_name }}
+{{ vars.resource_config.class|generate_import }}
+from {{ vars.proxy.module }} import {{ vars.service.proxy }}
 from invenio_records_permissions.generators import AuthenticatedUser, AnyUser, SystemProcess
 
 def _get_paths(cur_path, cur_val):
     ret_paths = []
     if isinstance(cur_val, list):
         return ret_paths
     elif isinstance(cur_val, dict):
@@ -17,25 +18,25 @@
         ret_paths.append(f"{cur_path}")
     return ret_paths
 
 
 def get_paths(prefix, data):
     return _get_paths(prefix, data)
 
-BASE_URL = f"http://localhost{{ "{" }} {{ schema.model.record_resource_config_class|base_name }}.url_prefix{{ "}" }}"
+BASE_URL = f"http://localhost{{ "{" }} {{ vars.resource_config.class|base_name }}.url_prefix{{ "}" }}"
 """
 def check_allowed(action_name):
-    permission_cls = current_service.config.permission_policy_cls
+    permission_cls = {{ vars.service.proxy }}.config.permission_policy_cls
     permission = permission_cls(action_name)
     identity = g.identity
     auth = permission.allows(identity)
     return auth
 """
 def is_action_allowed(action_name, user_is_auth):
-    permission_cls = current_service.config.permission_policy_cls
+    permission_cls = {{ vars.service.proxy }}.config.permission_policy_cls
     permission = permission_cls(action_name)
     action_name = f"can_{action_name}"
     action_permissions = getattr(permission, action_name, [])
     action_can_auth = False
     action_can_any = False
     for perm in action_permissions:
         if type(perm) == AnyUser:
@@ -53,26 +54,26 @@
     if action_allowed and response.status_code == authorized_response_code:
         return True
     elif not action_allowed and response.status_code == 403:
         return True
     return False
 
 
-def test_get_item({% for ef in current_model.extra_fixtures %}{{ ef }},{% endfor %}client_with_credentials, sample_record, search_clear):
+def test_get_item({{ vars.tests.extra_fixtures|generate_list(end=true) }} client_with_credentials, sample_record, search_clear):
     non_existing = client_with_credentials.get(f"{BASE_URL}yjuykyukyuk")
     assert non_existing.status_code == 404
 
     get_response = client_with_credentials.get(f"{BASE_URL}{sample_record['id']}")
     assert response_code_ok("read", True, get_response, 200)
     if is_action_allowed("read", True):
         assert get_response.json["metadata"] == sample_record["metadata"]
 
 
 def test_create(
-    {% for ef in current_model.extra_fixtures %}{{ ef }},{% endfor %}client_with_credentials, client, sample_metadata_list, app, search_clear
+    {{ vars.tests.extra_fixtures|generate_list(end=true) }}client_with_credentials, client, sample_metadata_list, app, search_clear
 ):
     created_responses = []
     for sample_metadata_point in sample_metadata_list:
         created_responses.append(
             client_with_credentials.post(f"{BASE_URL}", json=sample_metadata_point)
         )
         with app.test_client() as unauth_client:
@@ -92,25 +93,25 @@
             assert response_code_ok("read", True, created_response_reread, 200)
             assert (
                 created_response_reread.json["metadata"]
                 == sample_metadata_point["metadata"]
             )
 
 
-def test_listing({% for ef in current_model.extra_fixtures %}{{ ef }},{% endfor %}client_with_credentials, sample_records, search_clear):
+def test_listing({{ vars.tests.extra_fixtures|generate_list(end=true) }} client_with_credentials, sample_records, search_clear):
     listing_response = client_with_credentials.get(BASE_URL)
     hits = listing_response.json["hits"]["hits"]
-    assert len(hits) == 25
+    assert len(hits) == 10
 
 
 def test_update(
-    {% for ef in current_model.extra_fixtures %}{{ ef }},{% endfor %}client_with_credentials, sample_record, sample_metadata_list, search_clear
+    {{ vars.tests.extra_fixtures|generate_list(end=true) }} client_with_credentials, sample_record, sample_metadata_list, search_clear
 ):
     non_existing = client_with_credentials.put(
-        f"{BASE_URL}yjuykyukyuk", json=sample_metadata_list[15]
+        f"{BASE_URL}yjuykyukyuk", json=sample_metadata_list[5]
     )
 
     old_record_read_response_json = client_with_credentials.get(
         f"{BASE_URL}{sample_record['id']}"
     ).json
 
     update_response = client_with_credentials.put(
@@ -144,15 +145,15 @@
     # to make it work change create_url_rules in resource and allow jsonpatch in request_body_parsers in resource config
     # patch_response = client_with_credentials.patch(f"{BASE_URL}{sample_record['id']}",
     #                                                              json={"path": "/metadata/title",
     #                                                              "op": "replace",
     #                                                              "value": "UPDATED!"})
 
 
-def test_delete({% for ef in current_model.extra_fixtures %}{{ ef }},{% endfor %}client_with_credentials, sample_record, app, search_clear):
+def test_delete({{ vars.tests.extra_fixtures|generate_list(end=true) }} client_with_credentials, sample_record, app, search_clear):
     non_existing = client_with_credentials.delete(f"{BASE_URL}yjuykyukyuk")
     assert response_code_ok("delete", True, non_existing, 404)
 
     read_response = client_with_credentials.get(f"{BASE_URL}{sample_record['id']}")
     assert response_code_ok("read", True, read_response, 200)
 
     delete_response = client_with_credentials.delete(f"{BASE_URL}{sample_record['id']}")
@@ -168,16 +169,16 @@
     with app.test_client() as unauth_client:
         unauth_delete_response = unauth_client.delete(
             f"{BASE_URL}{sample_record['id']}"
         )
         assert response_code_ok("delete", False, unauth_delete_response, 204)
 
 
-
-def test_search({% for ef in current_model.extra_fixtures %}{{ ef }},{% endfor %}client_with_credentials, sample_records, sample_metadata_list, search_clear):
+@pytest.mark.xfail
+def test_search({{ vars.tests.extra_fixtures|generate_list(end=true) }} client_with_credentials, sample_records, sample_metadata_list, search_clear):
     if is_action_allowed("search", True):
         paths = get_paths("metadata", sample_metadata_list[0]["metadata"])
 
         for record in sample_records:
             for path in paths:
                 field_value = dict_lookup(record, path)
                 path_search_results = client_with_credentials.get(
@@ -187,19 +188,26 @@
                 for field_result in [dict_lookup(res, path) for res in path_search_results]:
                     if field_result == field_value:
                         break
                 else:
                     raise AssertionError("Queried field value not found in search results.")
 
         res_fail = client_with_credentials.get(f"{BASE_URL}?q=wefrtghthy")
+
+        start_datetime = (
+            datetime.datetime.utcnow() - datetime.timedelta(minutes=5)
+        ).isoformat() + "Z"
+        end_datetime = (
+            datetime.datetime.utcnow() + datetime.timedelta(minutes=5)
+        ).isoformat() + "Z"
+
         res_created = client_with_credentials.get(
-            f"{BASE_URL}?q={str(datetime.datetime.now().date())}"
+            f'{BASE_URL}?q=created:["{start_datetime}" TO "{end_datetime}"]'
         )
         res_created_fail = client_with_credentials.get(f"{BASE_URL}?q=2022-10-16")
-        res_facets = client_with_credentials.get(
-            f"{BASE_URL}?created={sample_records[0].created.isoformat()}"
-        )
+        record_created = sample_records[0].created.isoformat() + "Z"
+        res_facets = client_with_credentials.get(f"{BASE_URL}?created={record_created}")
 
         assert len(res_fail.json["hits"]["hits"]) == 0
-        assert len(res_created.json["hits"]["hits"]) == 25
+        assert len(res_created.json["hits"]["hits"]) == 10
         assert len(res_created_fail.json["hits"]["hits"]) == 0
         assert len(res_facets.json["hits"]["hits"]) == 1
```

### Comparing `oarepo-model-builder-tests-3.1.4/oarepo_model_builder_tests/templates/test_service.py.jinja2` & `oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests/templates/test_service.py.jinja2`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import pytest
 import pytz
 from invenio_records.dictutils import dict_lookup
 from invenio_access.permissions import system_identity
 from invenio_pidstore.errors import PIDDoesNotExistError, PIDDeletedError
 import datetime
+from {{ vars.proxy.module }} import {{ vars.service.proxy }}
+
 
 def _get_paths(cur_path, cur_val):
     ret_paths = []
     if isinstance(cur_val, list):
         return ret_paths
     elif isinstance(cur_val, dict):
         for k, v in cur_val.items():
@@ -18,25 +20,23 @@
         ret_paths.append(f"{cur_path}")
     return ret_paths
 
 
 def get_paths(prefix, data):
     return _get_paths(prefix, data)
 
-from {{ schema.model.proxies_current_service|package_name }} import {{ schema.model.proxies_current_service|base_name }}
-
 
-def test_read({% for ef in current_model.extra_fixtures %}{{ ef }},{% endfor %}app, db, sample_record, sample_metadata_list, search_clear):
+def test_read({{ vars.tests.extra_fixtures|generate_list(end=true) }} app, db, sample_record, sample_metadata_list, search_clear):
     with pytest.raises(PIDDoesNotExistError):
         current_service.read(system_identity, "fwegthi8op")
     read_record = current_service.read(system_identity, sample_record["id"])
     assert read_record.data["metadata"] == sample_record.metadata
 
 
-def test_create({% for ef in current_model.extra_fixtures %}{{ ef }},{% endfor %}app, db, sample_metadata_list, search_clear):
+def test_create({{ vars.tests.extra_fixtures|generate_list(end=true) }} app, db, sample_metadata_list, search_clear):
     created_records = []
     for sample_metadata_point in sample_metadata_list:
         created_records.append(
             current_service.create(system_identity, sample_metadata_point)
         )
     for sample_metadata_point, created_record in zip(
         sample_metadata_list, created_records
@@ -45,15 +45,15 @@
             system_identity, created_record["id"]
         )
         assert (
             created_record_reread.data["metadata"] == sample_metadata_point["metadata"]
         )
 
 
-def test_update({% for ef in current_model.extra_fixtures %}{{ ef }},{% endfor %}app, db, sample_record, sample_metadata_list, search_clear):
+def test_update({{ vars.tests.extra_fixtures|generate_list(end=true) }} app, db, sample_record, sample_metadata_list, search_clear):
     with pytest.raises(PIDDoesNotExistError):
         current_service.update(
             system_identity, "fwsegerhjtyuk754dh", sample_metadata_list[2]
         )
 
     old_record_data = current_service.read(system_identity, sample_record["id"]).data
     updated_record = current_service.update(
@@ -70,27 +70,28 @@
     assert (
         updated_record.data["revision_id"]
         == updated_record_read.data["revision_id"]
         == old_record_data["revision_id"] + 1
     )
 
 
-def test_delete({% for ef in current_model.extra_fixtures %}{{ ef }},{% endfor %}app, db, sample_record, search_clear):
+def test_delete({{ vars.tests.extra_fixtures|generate_list(end=true) }} app, db, sample_record, search_clear):
     with pytest.raises(PIDDoesNotExistError):
         current_service.delete(system_identity, "fwsegerhjtyuk754dh")
 
     to_delete_record = current_service.read(system_identity, sample_record["id"])
     assert to_delete_record
     current_service.delete(system_identity, sample_record["id"])
     with pytest.raises(PIDDeletedError):
         current_service.read(system_identity, sample_record["id"])
 
 
+@pytest.mark.xfail
 def test_search(
-    {% for ef in current_model.extra_fixtures %}{{ ef }},{% endfor %}app, db, sample_records, sample_metadata_list, search_clear
+    {{ vars.tests.extra_fixtures|generate_list(end=true) }} app, db, sample_records, sample_metadata_list, search_clear
 ):
     paths = get_paths("metadata", sample_metadata_list[0]["metadata"])
 
     for record in sample_records:
         for path in paths:
             field_value = dict_lookup(record, path)
             path_search_results = current_service.search(system_identity, params={"q": f"{path}:\"{field_value}\""})
@@ -99,34 +100,45 @@
                 if field_result == field_value:
                     break
             else:
                 raise AssertionError("Queried field value not found in search results.")
 
 
     res_fail = list(current_service.search(system_identity, params={"q": "wefrtghthy"}))
+
+    start_datetime = (
+        datetime.datetime.utcnow() - datetime.timedelta(minutes=5)
+    ).isoformat() + "Z"
+    end_datetime = (
+        datetime.datetime.utcnow() + datetime.timedelta(minutes=5)
+    ).isoformat() + "Z"
+
     res_created = list(
         current_service.search(
-            system_identity, params={"q": str(datetime.datetime.now().date())}
+            system_identity,
+            params={"q": f'created:["{start_datetime}" TO "{end_datetime}"]'},
         )
     )
 
     res_created_fail = list(
         current_service.search(system_identity, params={"q": "2022-10-16"})
     )
     res_facets = list(
         current_service.scan(
             system_identity,
             params={
                 "facets": {
-                    "created": [pytz.utc.localize(sample_records[0].created).isoformat()]
+                    "created": [
+                        pytz.utc.localize(sample_records[0].created).isoformat() + "Z"
+                    ]
                 }
             },
         ).hits
     )
 
     res_listing = list(current_service.search(system_identity))
 
     assert len(res_fail) == 0
-    assert len(res_listing) == 25
-    assert len(res_created) == 25
+    assert len(res_listing) == 10
+    assert len(res_created) == 10
     assert len(res_created_fail) == 0
     assert len(res_facets) == 1
```

### Comparing `oarepo-model-builder-tests-3.1.4/oarepo_model_builder_tests/templates/utils.py.jinja2` & `oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests/templates/utils.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-tests-3.1.4/oarepo_model_builder_tests.egg-info/PKG-INFO` & `oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-tests
-Version: 3.1.4
+Version: 4.0.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # OARepo model builder tests
 Plugin for oarepo-model-builder to generate 
 test files and add test dependencies.
 The record service and its rest api are covered for now. Tests read, write,
```

### Comparing `oarepo-model-builder-tests-3.1.4/oarepo_model_builder_tests.egg-info/SOURCES.txt` & `oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -12,13 +12,14 @@
 oarepo_model_builder_tests/utils_builder.py
 oarepo_model_builder_tests.egg-info/PKG-INFO
 oarepo_model_builder_tests.egg-info/SOURCES.txt
 oarepo_model_builder_tests.egg-info/dependency_links.txt
 oarepo_model_builder_tests.egg-info/entry_points.txt
 oarepo_model_builder_tests.egg-info/requires.txt
 oarepo_model_builder_tests.egg-info/top_level.txt
+oarepo_model_builder_tests/datatypes/__init__.py
+oarepo_model_builder_tests/datatypes/components.py
 oarepo_model_builder_tests/templates/__init__.py
 oarepo_model_builder_tests/templates/conftest.py.jinja2
 oarepo_model_builder_tests/templates/test_resource.py.jinja2
 oarepo_model_builder_tests/templates/test_service.py.jinja2
-oarepo_model_builder_tests/templates/utils.py.jinja2
-oarepo_model_builder_tests/validation/__init__.py
+oarepo_model_builder_tests/templates/utils.py.jinja2
```

### Comparing `oarepo-model-builder-tests-3.1.4/oarepo_model_builder_tests.egg-info/entry_points.txt` & `oarepo-model-builder-tests-4.0.0/oarepo_model_builder_tests.egg-info/entry_points.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-[oarepo_model_builder.builders.model]
+[oarepo_model_builder.builders.record]
 2010-oarepo_model_builder_setup_cfg = oarepo_model_builder_tests.oarepo_model_builder_setup_cfg:OarepoModelBuilderSetupCfgBuilder
 5020-conftest = oarepo_model_builder_tests.conftest_builder:ConftestBuilder
 5020-test_utils = oarepo_model_builder_tests.utils_builder:TestUtilsBuilder
 5021-test_resource = oarepo_model_builder_tests.test_resource_builder:TestResourceBuilder
 5022-test_service = oarepo_model_builder_tests.test_service_builder:TestServiceBuilder
 
+[oarepo_model_builder.datatypes.components]
+0200-tests = oarepo_model_builder_tests.datatypes.components:components
+
 [oarepo_model_builder.templates]
 99-tests_templates = oarepo_model_builder_tests
-
-[oarepo_model_builder.validation]
-test-fixtures-validation = oarepo_model_builder_tests.validation:validators
```

### Comparing `oarepo-model-builder-tests-3.1.4/setup.cfg` & `oarepo-model-builder-tests-4.0.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 [metadata]
 name = oarepo-model-builder-tests
-version = 3.1.4
+version = 4.0.0
 description = 
 authors = Ronald Krist <krist@cesnet.cz>
 readme = README.md
 long_description = file:README.md
 long_description_content_type = text/markdown
 
 [options]
 python = >=3.9
 install_requires = 
-	oarepo-model-builder>=3.1.0
+	oarepo-model-builder>=4.0.0
 packages = find:
 
 [options.package_data]
 * = *.json, *.rst, *.md, *.json5, *.jinja2
 
 [options.packages.find]
 exclude = example_model
 
 [options.entry_points]
-oarepo_model_builder.validation = 
-	test-fixtures-validation = oarepo_model_builder_tests.validation:validators
-oarepo_model_builder.builders.model = 
+oarepo_model_builder.datatypes.components = 
+	0200-tests = oarepo_model_builder_tests.datatypes.components:components
+oarepo_model_builder.builders.record = 
 	2010-oarepo_model_builder_setup_cfg = oarepo_model_builder_tests.oarepo_model_builder_setup_cfg:OarepoModelBuilderSetupCfgBuilder
 	5020-conftest  = oarepo_model_builder_tests.conftest_builder:ConftestBuilder
 	5020-test_utils = oarepo_model_builder_tests.utils_builder:TestUtilsBuilder
 	5021-test_resource  = oarepo_model_builder_tests.test_resource_builder:TestResourceBuilder
 	5022-test_service  = oarepo_model_builder_tests.test_service_builder:TestServiceBuilder
 oarepo_model_builder.templates = 
 	99-tests_templates  = oarepo_model_builder_tests
```

