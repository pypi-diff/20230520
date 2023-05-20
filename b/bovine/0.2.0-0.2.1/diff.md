# Comparing `tmp/bovine-0.2.0.tar.gz` & `tmp/bovine-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bovine-0.2.0.tar", max compression
+gzip compressed data, was "bovine-0.2.1.tar", max compression
```

## Comparing `bovine-0.2.0.tar` & `bovine-0.2.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0     1436 2023-05-04 17:50:05.898856 bovine-0.2.0/README.md
--rw-r--r--   0        0        0     9265 2023-05-20 16:50:13.638326 bovine-0.2.0/bovine/__init__.py
--rw-r--r--   0        0        0        0 2023-03-30 06:22:46.640327 bovine-0.2.0/bovine/activitypub/__init__.py
--rw-r--r--   0        0        0     3339 2023-05-19 09:30:24.831748 bovine-0.2.0/bovine/activitypub/authorization_wrapper.py
--rw-r--r--   0        0        0     2837 2023-04-28 17:37:23.831618 bovine-0.2.0/bovine/activitypub/collection_helper.py
--rw-r--r--   0        0        0      434 2023-04-30 15:16:00.489352 bovine-0.2.0/bovine/activitypub/collection_iterator.py
--rw-r--r--   0        0        0     2757 2023-04-16 07:30:22.724316 bovine-0.2.0/bovine/activitypub/test_actor.py
--rw-r--r--   0        0        0      498 2023-04-28 17:37:23.831618 bovine-0.2.0/bovine/activitypub/test_collection_helper.py
--rw-r--r--   0        0        0     4957 2023-04-28 17:37:23.831618 bovine-0.2.0/bovine/activitystreams/__init__.py
--rw-r--r--   0        0        0     4203 2023-04-30 15:16:00.489352 bovine-0.2.0/bovine/activitystreams/activity_factory.py
--rw-r--r--   0        0        0     4178 2023-05-08 17:33:54.282008 bovine-0.2.0/bovine/activitystreams/object_factory.py
--rw-r--r--   0        0        0     2195 2023-04-30 15:16:00.489352 bovine-0.2.0/bovine/activitystreams/test_activity_factory.py
--rw-r--r--   0        0        0     1442 2023-04-30 15:16:00.489352 bovine-0.2.0/bovine/activitystreams/test_actor.py
--rw-r--r--   0        0        0     1257 2023-05-08 17:33:54.282008 bovine-0.2.0/bovine/activitystreams/test_object_factory.py
--rw-r--r--   0        0        0     1034 2023-04-30 15:16:00.489352 bovine-0.2.0/bovine/activitystreams/test_ordered_collection_builder.py
--rw-r--r--   0        0        0      817 2023-04-30 15:16:00.489352 bovine-0.2.0/bovine/activitystreams/test_ordered_collection_page.py
--rw-r--r--   0        0        0     2354 2023-04-10 11:15:03.230405 bovine-0.2.0/bovine/activitystreams/utils/__init__.py
--rw-r--r--   0        0        0      787 2023-03-30 06:22:46.644327 bovine-0.2.0/bovine/activitystreams/utils/print.py
--rw-r--r--   0        0        0     2266 2023-05-20 16:50:13.578325 bovine-0.2.0/bovine/activitystreams/utils/test_utils.py
--rw-r--r--   0        0        0     3826 2023-05-20 13:54:54.854025 bovine-0.2.0/bovine/clients/__init__.py
--rw-r--r--   0        0        0     1794 2023-04-30 15:16:00.489352 bovine-0.2.0/bovine/clients/bearer.py
--rw-r--r--   0        0        0       91 2023-04-01 14:40:33.451427 bovine-0.2.0/bovine/clients/consts.py
--rw-r--r--   0        0        0     1520 2023-04-30 15:16:00.489352 bovine-0.2.0/bovine/clients/event_source.py
--rw-r--r--   0        0        0      868 2023-05-20 13:54:54.854025 bovine-0.2.0/bovine/clients/lookup_account.py
--rw-r--r--   0        0        0     3001 2023-04-30 15:16:00.489352 bovine-0.2.0/bovine/clients/moo_auth.py
--rw-r--r--   0        0        0      948 2023-04-16 07:30:22.724316 bovine-0.2.0/bovine/clients/nodeinfo.py
--rw-r--r--   0        0        0     1150 2023-04-30 15:16:00.489352 bovine-0.2.0/bovine/clients/signed_http.py
--rw-r--r--   0        0        0     3278 2023-04-30 15:16:00.489352 bovine-0.2.0/bovine/clients/signed_http_methods.py
--rw-r--r--   0        0        0      609 2023-04-02 15:04:42.447683 bovine-0.2.0/bovine/clients/test_event_source.py
--rw-r--r--   0        0        0     1149 2023-05-20 16:50:13.534325 bovine-0.2.0/bovine/clients/test_lookup_account.py
--rw-r--r--   0        0        0      319 2023-04-16 07:30:22.724316 bovine-0.2.0/bovine/clients/test_nodeinfo.py
--rw-r--r--   0        0        0     1153 2023-04-30 15:16:00.489352 bovine-0.2.0/bovine/clients/test_signed_http.py
--rw-r--r--   0        0        0      522 2023-04-30 15:16:00.493353 bovine-0.2.0/bovine/clients/test_signed_http_client.py
--rw-r--r--   0        0        0     4141 2023-05-20 16:50:13.586326 bovine-0.2.0/bovine/crypto/__init__.py
--rw-r--r--   0        0        0     2664 2023-05-20 16:50:13.594326 bovine-0.2.0/bovine/crypto/helper.py
--rw-r--r--   0        0        0     2112 2023-04-13 18:39:25.192264 bovine-0.2.0/bovine/crypto/http_signature.py
--rw-r--r--   0        0        0     2942 2023-04-13 18:39:25.192264 bovine-0.2.0/bovine/crypto/signature_checker.py
--rw-r--r--   0        0        0     1266 2023-04-13 18:39:25.192264 bovine-0.2.0/bovine/crypto/signature_parser.py
--rw-r--r--   0        0        0     2199 2023-04-13 18:39:25.192264 bovine-0.2.0/bovine/crypto/test.py
--rw-r--r--   0        0        0     4995 2023-05-20 16:50:13.602326 bovine-0.2.0/bovine/crypto/test_crypto.py
--rw-r--r--   0        0        0      896 2023-05-20 16:50:13.578325 bovine-0.2.0/bovine/crypto/test_helper.py
--rw-r--r--   0        0        0     5081 2023-04-13 18:39:25.192264 bovine-0.2.0/bovine/crypto/test_http_signature.py
--rw-r--r--   0        0        0     1207 2023-04-14 06:13:18.963625 bovine-0.2.0/bovine/crypto/test_signature_parser.py
--rw-r--r--   0        0        0      302 2023-04-20 10:24:23.306509 bovine-0.2.0/bovine/ed25519_key.py
--rw-r--r--   0        0        0     3342 2023-05-20 16:49:47.490022 bovine-0.2.0/bovine/jsonld.py
--rw-r--r--   0        0        0      864 2023-05-19 17:02:04.848548 bovine-0.2.0/bovine/msg.py
--rw-r--r--   0        0        0      178 2023-03-30 06:22:46.648327 bovine-0.2.0/bovine/test_bovine_client.py
--rw-r--r--   0        0        0     5250 2023-05-20 13:54:54.854025 bovine-0.2.0/bovine/test_jsonld.py
--rw-r--r--   0        0        0      282 2023-03-30 06:22:46.648327 bovine-0.2.0/bovine/test_types.py
--rw-r--r--   0        0        0     2397 2023-05-19 10:45:30.289388 bovine-0.2.0/bovine/types.py
--rw-r--r--   0        0        0      856 2023-05-20 13:54:54.854025 bovine-0.2.0/bovine/utils/__init__.py
--rw-r--r--   0        0        0      519 2023-03-30 06:22:46.648327 bovine-0.2.0/bovine/utils/date.py
--rw-r--r--   0        0        0     1313 2023-05-20 13:54:54.854025 bovine-0.2.0/bovine/utils/msg/__init__.py
--rw-r--r--   0        0        0      599 2023-04-30 15:16:00.493353 bovine-0.2.0/bovine/utils/msg/test_validation.py
--rw-r--r--   0        0        0      261 2023-04-30 15:16:00.493353 bovine-0.2.0/bovine/utils/msg/validation.py
--rw-r--r--   0        0        0     4504 2023-05-20 16:50:12.842317 bovine-0.2.0/bovine/utils/pyld_requests.py
--rw-r--r--   0        0        0      761 2023-04-30 15:16:00.493353 bovine-0.2.0/bovine/utils/test_date.py
--rw-r--r--   0        0        0      452 2023-04-16 07:30:22.728317 bovine-0.2.0/bovine/utils/test_parse.py
--rw-r--r--   0        0        0      368 2023-05-20 13:54:54.854025 bovine-0.2.0/bovine/utils/test_webfinger.py
--rw-r--r--   0        0        0     1291 2023-05-20 16:50:03.742211 bovine-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2564 1970-01-01 00:00:00.000000 bovine-0.2.0/setup.py
--rw-r--r--   0        0        0     2498 1970-01-01 00:00:00.000000 bovine-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1436 2023-05-04 17:50:05.898856 bovine-0.2.1/README.md
+-rw-r--r--   0        0        0     9265 2023-05-20 16:50:13.638326 bovine-0.2.1/bovine/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-30 06:22:46.640327 bovine-0.2.1/bovine/activitypub/__init__.py
+-rw-r--r--   0        0        0     3339 2023-05-19 09:30:24.831748 bovine-0.2.1/bovine/activitypub/authorization_wrapper.py
+-rw-r--r--   0        0        0     2837 2023-04-28 17:37:23.831618 bovine-0.2.1/bovine/activitypub/collection_helper.py
+-rw-r--r--   0        0        0      434 2023-04-30 15:16:00.489352 bovine-0.2.1/bovine/activitypub/collection_iterator.py
+-rw-r--r--   0        0        0     2757 2023-04-16 07:30:22.724316 bovine-0.2.1/bovine/activitypub/test_actor.py
+-rw-r--r--   0        0        0      498 2023-04-28 17:37:23.831618 bovine-0.2.1/bovine/activitypub/test_collection_helper.py
+-rw-r--r--   0        0        0     4957 2023-04-28 17:37:23.831618 bovine-0.2.1/bovine/activitystreams/__init__.py
+-rw-r--r--   0        0        0     4203 2023-04-30 15:16:00.489352 bovine-0.2.1/bovine/activitystreams/activity_factory.py
+-rw-r--r--   0        0        0     4178 2023-05-08 17:33:54.282008 bovine-0.2.1/bovine/activitystreams/object_factory.py
+-rw-r--r--   0        0        0     2195 2023-04-30 15:16:00.489352 bovine-0.2.1/bovine/activitystreams/test_activity_factory.py
+-rw-r--r--   0        0        0     1442 2023-04-30 15:16:00.489352 bovine-0.2.1/bovine/activitystreams/test_actor.py
+-rw-r--r--   0        0        0     1257 2023-05-08 17:33:54.282008 bovine-0.2.1/bovine/activitystreams/test_object_factory.py
+-rw-r--r--   0        0        0     1034 2023-04-30 15:16:00.489352 bovine-0.2.1/bovine/activitystreams/test_ordered_collection_builder.py
+-rw-r--r--   0        0        0      817 2023-04-30 15:16:00.489352 bovine-0.2.1/bovine/activitystreams/test_ordered_collection_page.py
+-rw-r--r--   0        0        0     2354 2023-04-10 11:15:03.230405 bovine-0.2.1/bovine/activitystreams/utils/__init__.py
+-rw-r--r--   0        0        0      787 2023-03-30 06:22:46.644327 bovine-0.2.1/bovine/activitystreams/utils/print.py
+-rw-r--r--   0        0        0     2266 2023-05-20 16:50:13.578325 bovine-0.2.1/bovine/activitystreams/utils/test_utils.py
+-rw-r--r--   0        0        0     3826 2023-05-20 13:54:54.854025 bovine-0.2.1/bovine/clients/__init__.py
+-rw-r--r--   0        0        0     1794 2023-04-30 15:16:00.489352 bovine-0.2.1/bovine/clients/bearer.py
+-rw-r--r--   0        0        0       91 2023-04-01 14:40:33.451427 bovine-0.2.1/bovine/clients/consts.py
+-rw-r--r--   0        0        0     1520 2023-04-30 15:16:00.489352 bovine-0.2.1/bovine/clients/event_source.py
+-rw-r--r--   0        0        0      868 2023-05-20 13:54:54.854025 bovine-0.2.1/bovine/clients/lookup_account.py
+-rw-r--r--   0        0        0     3001 2023-04-30 15:16:00.489352 bovine-0.2.1/bovine/clients/moo_auth.py
+-rw-r--r--   0        0        0      948 2023-04-16 07:30:22.724316 bovine-0.2.1/bovine/clients/nodeinfo.py
+-rw-r--r--   0        0        0     1150 2023-04-30 15:16:00.489352 bovine-0.2.1/bovine/clients/signed_http.py
+-rw-r--r--   0        0        0     3278 2023-04-30 15:16:00.489352 bovine-0.2.1/bovine/clients/signed_http_methods.py
+-rw-r--r--   0        0        0      609 2023-04-02 15:04:42.447683 bovine-0.2.1/bovine/clients/test_event_source.py
+-rw-r--r--   0        0        0     1149 2023-05-20 16:50:13.534325 bovine-0.2.1/bovine/clients/test_lookup_account.py
+-rw-r--r--   0        0        0      319 2023-04-16 07:30:22.724316 bovine-0.2.1/bovine/clients/test_nodeinfo.py
+-rw-r--r--   0        0        0     1153 2023-04-30 15:16:00.489352 bovine-0.2.1/bovine/clients/test_signed_http.py
+-rw-r--r--   0        0        0      522 2023-04-30 15:16:00.493353 bovine-0.2.1/bovine/clients/test_signed_http_client.py
+-rw-r--r--   0        0        0     4141 2023-05-20 16:50:13.586326 bovine-0.2.1/bovine/crypto/__init__.py
+-rw-r--r--   0        0        0     2664 2023-05-20 16:50:13.594326 bovine-0.2.1/bovine/crypto/helper.py
+-rw-r--r--   0        0        0     2112 2023-04-13 18:39:25.192264 bovine-0.2.1/bovine/crypto/http_signature.py
+-rw-r--r--   0        0        0     2942 2023-04-13 18:39:25.192264 bovine-0.2.1/bovine/crypto/signature_checker.py
+-rw-r--r--   0        0        0     1266 2023-04-13 18:39:25.192264 bovine-0.2.1/bovine/crypto/signature_parser.py
+-rw-r--r--   0        0        0     2199 2023-04-13 18:39:25.192264 bovine-0.2.1/bovine/crypto/test.py
+-rw-r--r--   0        0        0     4995 2023-05-20 16:50:13.602326 bovine-0.2.1/bovine/crypto/test_crypto.py
+-rw-r--r--   0        0        0      896 2023-05-20 16:50:13.578325 bovine-0.2.1/bovine/crypto/test_helper.py
+-rw-r--r--   0        0        0     5081 2023-04-13 18:39:25.192264 bovine-0.2.1/bovine/crypto/test_http_signature.py
+-rw-r--r--   0        0        0     1207 2023-04-14 06:13:18.963625 bovine-0.2.1/bovine/crypto/test_signature_parser.py
+-rw-r--r--   0        0        0      302 2023-04-20 10:24:23.306509 bovine-0.2.1/bovine/ed25519_key.py
+-rw-r--r--   0        0        0     3342 2023-05-20 16:49:47.490022 bovine-0.2.1/bovine/jsonld.py
+-rw-r--r--   0        0        0      864 2023-05-19 17:02:04.848548 bovine-0.2.1/bovine/msg.py
+-rw-r--r--   0        0        0      178 2023-03-30 06:22:46.648327 bovine-0.2.1/bovine/test_bovine_client.py
+-rw-r--r--   0        0        0     5250 2023-05-20 13:54:54.854025 bovine-0.2.1/bovine/test_jsonld.py
+-rw-r--r--   0        0        0      282 2023-03-30 06:22:46.648327 bovine-0.2.1/bovine/test_types.py
+-rw-r--r--   0        0        0     2397 2023-05-19 10:45:30.289388 bovine-0.2.1/bovine/types.py
+-rw-r--r--   0        0        0      856 2023-05-20 13:54:54.854025 bovine-0.2.1/bovine/utils/__init__.py
+-rw-r--r--   0        0        0      519 2023-03-30 06:22:46.648327 bovine-0.2.1/bovine/utils/date.py
+-rw-r--r--   0        0        0     1313 2023-05-20 13:54:54.854025 bovine-0.2.1/bovine/utils/msg/__init__.py
+-rw-r--r--   0        0        0      599 2023-04-30 15:16:00.493353 bovine-0.2.1/bovine/utils/msg/test_validation.py
+-rw-r--r--   0        0        0      261 2023-04-30 15:16:00.493353 bovine-0.2.1/bovine/utils/msg/validation.py
+-rw-r--r--   0        0        0     4736 2023-05-20 18:53:31.208381 bovine-0.2.1/bovine/utils/pyld_requests.py
+-rw-r--r--   0        0        0      761 2023-04-30 15:16:00.493353 bovine-0.2.1/bovine/utils/test_date.py
+-rw-r--r--   0        0        0      452 2023-04-16 07:30:22.728317 bovine-0.2.1/bovine/utils/test_parse.py
+-rw-r--r--   0        0        0      368 2023-05-20 13:54:54.854025 bovine-0.2.1/bovine/utils/test_webfinger.py
+-rw-r--r--   0        0        0     1291 2023-05-20 19:25:54.298284 bovine-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2564 1970-01-01 00:00:00.000000 bovine-0.2.1/setup.py
+-rw-r--r--   0        0        0     2498 1970-01-01 00:00:00.000000 bovine-0.2.1/PKG-INFO
```

### Comparing `bovine-0.2.0/README.md` & `bovine-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `bovine-0.2.0/bovine/__init__.py` & `bovine-0.2.1/bovine/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.0/bovine/activitypub/authorization_wrapper.py` & `bovine-0.2.1/bovine/activitypub/authorization_wrapper.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.0/bovine/activitypub/collection_helper.py` & `bovine-0.2.1/bovine/activitypub/collection_helper.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.0/bovine/activitypub/test_actor.py` & `bovine-0.2.1/bovine/activitypub/test_actor.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.0/bovine/activitystreams/__init__.py` & `bovine-0.2.1/bovine/activitystreams/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.0/bovine/activitystreams/activity_factory.py` & `bovine-0.2.1/bovine/activitystreams/activity_factory.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.0/bovine/activitystreams/object_factory.py` & `bovine-0.2.1/bovine/activitystreams/object_factory.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.0/bovine/activitystreams/test_activity_factory.py` & `bovine-0.2.1/bovine/activitystreams/test_activity_factory.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.0/bovine/activitystreams/test_actor.py` & `bovine-0.2.1/bovine/activitystreams/test_actor.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.0/bovine/activitystreams/test_object_factory.py` & `bovine-0.2.1/bovine/activitystreams/test_object_factory.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.0/bovine/activitystreams/test_ordered_collection_builder.py` & `bovine-0.2.1/bovine/activitystreams/test_ordered_collection_builder.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.0/bovine/activitystreams/test_ordered_collection_page.py` & `bovine-0.2.1/bovine/activitystreams/test_ordered_collection_page.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.0/bovine/activitystreams/utils/__init__.py` & `bovine-0.2.1/bovine/activitystreams/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.0/bovine/activitystreams/utils/print.py` & `bovine-0.2.1/bovine/activitystreams/utils/print.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.0/bovine/activitystreams/utils/test_utils.py` & `bovine-0.2.1/bovine/activitystreams/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.0/bovine/clients/__init__.py` & `bovine-0.2.1/bovine/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.0/bovine/clients/bearer.py` & `bovine-0.2.1/bovine/clients/bearer.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.0/bovine/clients/event_source.py` & `bovine-0.2.1/bovine/clients/event_source.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.0/bovine/clients/lookup_account.py` & `bovine-0.2.1/bovine/clients/lookup_account.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.0/bovine/clients/moo_auth.py` & `bovine-0.2.1/bovine/clients/moo_auth.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.0/bovine/clients/nodeinfo.py` & `bovine-0.2.1/bovine/clients/nodeinfo.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.0/bovine/clients/signed_http.py` & `bovine-0.2.1/bovine/clients/signed_http.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.0/bovine/clients/signed_http_methods.py` & `bovine-0.2.1/bovine/clients/signed_http_methods.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.0/bovine/clients/test_event_source.py` & `bovine-0.2.1/bovine/clients/test_event_source.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.0/bovine/clients/test_lookup_account.py` & `bovine-0.2.1/bovine/clients/test_lookup_account.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.0/bovine/clients/test_signed_http.py` & `bovine-0.2.1/bovine/clients/test_signed_http.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.0/bovine/clients/test_signed_http_client.py` & `bovine-0.2.1/bovine/clients/test_signed_http_client.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.0/bovine/crypto/__init__.py` & `bovine-0.2.1/bovine/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.0/bovine/crypto/helper.py` & `bovine-0.2.1/bovine/crypto/helper.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.0/bovine/crypto/http_signature.py` & `bovine-0.2.1/bovine/crypto/http_signature.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.0/bovine/crypto/signature_checker.py` & `bovine-0.2.1/bovine/crypto/signature_checker.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.0/bovine/crypto/signature_parser.py` & `bovine-0.2.1/bovine/crypto/signature_parser.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.0/bovine/crypto/test.py` & `bovine-0.2.1/bovine/crypto/test.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.0/bovine/crypto/test_crypto.py` & `bovine-0.2.1/bovine/crypto/test_crypto.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.0/bovine/crypto/test_helper.py` & `bovine-0.2.1/bovine/crypto/test_helper.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.0/bovine/crypto/test_http_signature.py` & `bovine-0.2.1/bovine/crypto/test_http_signature.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.0/bovine/crypto/test_signature_parser.py` & `bovine-0.2.1/bovine/crypto/test_signature_parser.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.0/bovine/jsonld.py` & `bovine-0.2.1/bovine/jsonld.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.0/bovine/msg.py` & `bovine-0.2.1/bovine/msg.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.0/bovine/test_jsonld.py` & `bovine-0.2.1/bovine/test_jsonld.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.0/bovine/types.py` & `bovine-0.2.1/bovine/types.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.0/bovine/utils/__init__.py` & `bovine-0.2.1/bovine/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.0/bovine/utils/date.py` & `bovine-0.2.1/bovine/utils/date.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.0/bovine/utils/msg/__init__.py` & `bovine-0.2.1/bovine/utils/msg/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.0/bovine/utils/msg/test_validation.py` & `bovine-0.2.1/bovine/utils/msg/test_validation.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.0/bovine/utils/pyld_requests.py` & `bovine-0.2.1/bovine/utils/pyld_requests.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,14 +64,19 @@
                     "jsonld.InvalidUrl",
                     {"url": url},
                     code="loading document failed",
                 )
             headers = options.get("headers")
             if headers is None:
                 headers = {"Accept": "application/ld+json, application/json"}
+            headers["Accept"] = (
+                headers["Accept"]
+                .replace("text/html;q=0.8", "text/html;q=0.2")
+                .replace("application/xhtml+xml;q=0.8", "application/xhtml+xml;q=0.3")
+            )
             response = requests.get(url, headers=headers, **kwargs)
 
             content_type = response.headers.get("content-type")
             if not content_type:
                 content_type = "application/octet-stream"
             doc = {
                 "contentType": content_type,
```

### Comparing `bovine-0.2.0/bovine/utils/test_date.py` & `bovine-0.2.1/bovine/utils/test_date.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.0/pyproject.toml` & `bovine-0.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bovine"
-version = "0.2.0"
+version = "0.2.1"
 description = "Core functionality of bovine needed to build fediverse applications"
 authors = ["Helge <helge.krueger@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "bovine" }]
 repository = "https://codeberg.org/bovine/bovine"
 documentation = "https://bovine.readthedocs.io/en/latest/"
```

### Comparing `bovine-0.2.0/setup.py` & `bovine-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
  'python-dateutil>=2.8.2,<3.0.0',
  'requests-cache>=0.9.8,<0.10.0',
  'requests>=2.30.0,<3.0.0',
  'tomli>=2.0.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'bovine',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': 'Core functionality of bovine needed to build fediverse applications',
     'long_description': '# Bovine\n\nBovine is a basic utility library for the FediVerse. It can be used both to build ActivityPub Client applications and ActivityPub Servers. In addition to [ActivityPub](https://activitypub.rocks/) support, it also provides utilities to deal with [webfinger](https://webfinger.net), nodeinfo, and HTTP Signatures.\n\nThe bovine library can just be installed via pip\n\n```bash\npip install bovine\n```\n\nDocumentation including tutorials is available at [ReadTheDocs](https://bovine.readthedocs.io/en/latest/).\nAn entire working ActivityPub server can be found in the [bovine repository](https://codeberg.org/bovine/bovine/).\n\n## Feedback\n\nIssues about bovine should be filed as an [issue](https://codeberg.org/bovine/bovine/issues).\n\n## Contributing\n\nIf you want to contribute, you can start by working on issues labeled [Good first issue](https://codeberg.org/bovine/bovine/issues?q=&type=all&state=open&labels=110885&milestone=0&assignee=0&poster=0). The tech stack is currently based on asynchronous python, using the following components:\n\n- [aiohttp](https://docs.aiohttp.org/en/stable/index.html) for http requests.\n- [quart](https://quart.palletsprojects.com/en/latest/) as a webserver.\n- [cryptography](https://cryptography.io/en/latest/).\n- [pytest](https://docs.pytest.org/en/7.3.x/) for testing.\n- [ruff](https://pypi.org/project/ruff/) for linting.\n\n\n## Todo\n\n- [ ] Document FediVerse crawler behavior in server tutorial\n\n',
     'author': 'Helge',
     'author_email': 'helge.krueger@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://codeberg.org/bovine/bovine',
```

### Comparing `bovine-0.2.0/PKG-INFO` & `bovine-0.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bovine
-Version: 0.2.0
+Version: 0.2.1
 Summary: Core functionality of bovine needed to build fediverse applications
 Home-page: https://codeberg.org/bovine/bovine
 License: MIT
 Author: Helge
 Author-email: helge.krueger@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

