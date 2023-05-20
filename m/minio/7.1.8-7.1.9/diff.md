# Comparing `tmp/minio-7.1.8.tar.gz` & `tmp/minio-7.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minio-7.1.8.tar", last modified: Thu May  5 00:21:07 2022, max compression
+gzip compressed data, was "minio-7.1.9.tar", last modified: Sat Jun 11 21:34:02 2022, max compression
```

## Comparing `minio-7.1.8.tar` & `minio-7.1.9.tar`

### file list

```diff
@@ -1,153 +1,153 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-05 00:21:07.007438 minio-7.1.8/
--rw-r--r--   0 root         (0) root         (0)    11358 2022-05-05 00:19:09.000000 minio-7.1.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)      235 2022-05-05 00:19:09.000000 minio-7.1.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4111 2022-05-05 00:21:07.007438 minio-7.1.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3173 2022-05-05 00:19:09.000000 minio-7.1.8/README.md
--rw-r--r--   0 root         (0) root         (0)     8876 2022-05-05 00:19:09.000000 minio-7.1.8/README_zh_CN.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-05 00:21:06.991438 minio-7.1.8/docs/
--rw-r--r--   0 root         (0) root         (0)    60994 2022-05-05 00:19:09.000000 minio-7.1.8/docs/API.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-05 00:21:06.991438 minio-7.1.8/docs/zh_CN/
--rw-r--r--   0 root         (0) root         (0)    33823 2022-05-05 00:19:09.000000 minio-7.1.8/docs/zh_CN/API.md
--rw-r--r--   0 root         (0) root         (0)      688 2022-05-05 00:19:09.000000 minio-7.1.8/docs/zh_CN/CONTRIBUTING.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-05 00:21:06.999438 minio-7.1.8/examples/
--rw-r--r--   0 root         (0) root         (0)      930 2022-05-05 00:19:09.000000 minio-7.1.8/examples/bucket_exists.py
--rw-r--r--   0 root         (0) root         (0)     1744 2022-05-05 00:19:09.000000 minio-7.1.8/examples/compose_object.py
--rw-r--r--   0 root         (0) root         (0)     1733 2022-05-05 00:19:09.000000 minio-7.1.8/examples/copy_object.py
--rw-r--r--   0 root         (0) root         (0)      873 2022-05-05 00:19:09.000000 minio-7.1.8/examples/delete_bucket_encryption.py
--rw-r--r--   0 root         (0) root         (0)      872 2022-05-05 00:19:09.000000 minio-7.1.8/examples/delete_bucket_lifecycle.py
--rw-r--r--   0 root         (0) root         (0)      875 2022-05-05 00:19:09.000000 minio-7.1.8/examples/delete_bucket_notification.py
--rw-r--r--   0 root         (0) root         (0)      869 2022-05-05 00:19:09.000000 minio-7.1.8/examples/delete_bucket_policy.py
--rw-r--r--   0 root         (0) root         (0)      874 2022-05-05 00:19:09.000000 minio-7.1.8/examples/delete_bucket_replication.py
--rw-r--r--   0 root         (0) root         (0)      867 2022-05-05 00:19:09.000000 minio-7.1.8/examples/delete_bucket_tags.py
--rw-r--r--   0 root         (0) root         (0)      874 2022-05-05 00:19:09.000000 minio-7.1.8/examples/delete_object_lock_config.py
--rw-r--r--   0 root         (0) root         (0)      880 2022-05-05 00:19:09.000000 minio-7.1.8/examples/delete_object_tags.py
--rw-r--r--   0 root         (0) root         (0)      887 2022-05-05 00:19:09.000000 minio-7.1.8/examples/disable_object_legal_hold.py
--rw-r--r--   0 root         (0) root         (0)      886 2022-05-05 00:19:09.000000 minio-7.1.8/examples/enable_object_legal_hold.py
--rw-r--r--   0 root         (0) root         (0)     1288 2022-05-05 00:19:09.000000 minio-7.1.8/examples/fget_object.py
--rw-r--r--   0 root         (0) root         (0)     3561 2022-05-05 00:19:09.000000 minio-7.1.8/examples/fput_object.py
--rw-r--r--   0 root         (0) root         (0)      879 2022-05-05 00:19:09.000000 minio-7.1.8/examples/get_bucket_encryption.py
--rw-r--r--   0 root         (0) root         (0)      878 2022-05-05 00:19:09.000000 minio-7.1.8/examples/get_bucket_lifecycle.py
--rw-r--r--   0 root         (0) root         (0)      881 2022-05-05 00:19:09.000000 minio-7.1.8/examples/get_bucket_notification.py
--rw-r--r--   0 root         (0) root         (0)      875 2022-05-05 00:19:09.000000 minio-7.1.8/examples/get_bucket_policy.py
--rw-r--r--   0 root         (0) root         (0)      880 2022-05-05 00:19:09.000000 minio-7.1.8/examples/get_bucket_replication.py
--rw-r--r--   0 root         (0) root         (0)      871 2022-05-05 00:19:09.000000 minio-7.1.8/examples/get_bucket_tags.py
--rw-r--r--   0 root         (0) root         (0)      900 2022-05-05 00:19:09.000000 minio-7.1.8/examples/get_bucket_versioning.py
--rw-r--r--   0 root         (0) root         (0)     1818 2022-05-05 00:19:09.000000 minio-7.1.8/examples/get_object.py
--rw-r--r--   0 root         (0) root         (0)      880 2022-05-05 00:19:09.000000 minio-7.1.8/examples/get_object_lock_config.py
--rw-r--r--   0 root         (0) root         (0)      891 2022-05-05 00:19:09.000000 minio-7.1.8/examples/get_object_retention.py
--rw-r--r--   0 root         (0) root         (0)      884 2022-05-05 00:19:09.000000 minio-7.1.8/examples/get_object_tags.py
--rw-r--r--   0 root         (0) root         (0)     1600 2022-05-05 00:19:09.000000 minio-7.1.8/examples/get_presigned_url.py
--rw-r--r--   0 root         (0) root         (0)     1000 2022-05-05 00:19:09.000000 minio-7.1.8/examples/is_object_legal_hold_enabled.py
--rw-r--r--   0 root         (0) root         (0)      918 2022-05-05 00:19:09.000000 minio-7.1.8/examples/list_buckets.py
--rw-r--r--   0 root         (0) root         (0)     1641 2022-05-05 00:19:09.000000 minio-7.1.8/examples/list_objects.py
--rw-r--r--   0 root         (0) root         (0)     1026 2022-05-05 00:19:09.000000 minio-7.1.8/examples/listen_bucket_notification.py
--rw-r--r--   0 root         (0) root         (0)     1074 2022-05-05 00:19:09.000000 minio-7.1.8/examples/make_bucket.py
--rw-r--r--   0 root         (0) root         (0)     1635 2022-05-05 00:19:09.000000 minio-7.1.8/examples/minio_with_assume_role_provider.py
--rw-r--r--   0 root         (0) root         (0)      897 2022-05-05 00:19:09.000000 minio-7.1.8/examples/minio_with_aws_config_provider.py
--rw-r--r--   0 root         (0) root         (0)     1209 2022-05-05 00:19:09.000000 minio-7.1.8/examples/minio_with_certificate_identity_provider.py
--rw-r--r--   0 root         (0) root         (0)     1274 2022-05-05 00:19:09.000000 minio-7.1.8/examples/minio_with_chained_provider.py
--rw-r--r--   0 root         (0) root         (0)     1686 2022-05-05 00:19:09.000000 minio-7.1.8/examples/minio_with_client_grants_provider.py
--rw-r--r--   0 root         (0) root         (0)      891 2022-05-05 00:19:09.000000 minio-7.1.8/examples/minio_with_env_aws_provider.py
--rw-r--r--   0 root         (0) root         (0)      900 2022-05-05 00:19:09.000000 minio-7.1.8/examples/minio_with_env_minio_provider.py
--rw-r--r--   0 root         (0) root         (0)      891 2022-05-05 00:19:09.000000 minio-7.1.8/examples/minio_with_iam_aws_provider.py
--rw-r--r--   0 root         (0) root         (0)     1161 2022-05-05 00:19:09.000000 minio-7.1.8/examples/minio_with_ldap_identity_provider.py
--rw-r--r--   0 root         (0) root         (0)      925 2022-05-05 00:19:09.000000 minio-7.1.8/examples/minio_with_minio_client_config_provider.py
--rw-r--r--   0 root         (0) root         (0)     2009 2022-05-05 00:19:09.000000 minio-7.1.8/examples/minio_with_web_identity_provider.py
--rw-r--r--   0 root         (0) root         (0)     1222 2022-05-05 00:19:09.000000 minio-7.1.8/examples/presigned_get_object.py
--rw-r--r--   0 root         (0) root         (0)     1357 2022-05-05 00:19:09.000000 minio-7.1.8/examples/presigned_post_policy.py
--rw-r--r--   0 root         (0) root         (0)     1234 2022-05-05 00:19:09.000000 minio-7.1.8/examples/presigned_put_object.py
--rw-r--r--   0 root         (0) root         (0)     6203 2022-05-05 00:19:09.000000 minio-7.1.8/examples/progress.py
--rw-r--r--   0 root         (0) root         (0)     4036 2022-05-05 00:19:09.000000 minio-7.1.8/examples/put_object.py
--rw-r--r--   0 root         (0) root         (0)      852 2022-05-05 00:19:09.000000 minio-7.1.8/examples/remove_bucket.py
--rw-r--r--   0 root         (0) root         (0)     1023 2022-05-05 00:19:09.000000 minio-7.1.8/examples/remove_object.py
--rw-r--r--   0 root         (0) root         (0)     1488 2022-05-05 00:19:09.000000 minio-7.1.8/examples/remove_objects.py
--rw-r--r--   0 root         (0) root         (0)     1297 2022-05-05 00:19:09.000000 minio-7.1.8/examples/select_object_content.py
--rw-r--r--   0 root         (0) root         (0)      956 2022-05-05 00:19:09.000000 minio-7.1.8/examples/set_bucket_encryption.py
--rw-r--r--   0 root         (0) root         (0)     1410 2022-05-05 00:19:09.000000 minio-7.1.8/examples/set_bucket_lifecycle.py
--rw-r--r--   0 root         (0) root         (0)     1260 2022-05-05 00:19:09.000000 minio-7.1.8/examples/set_bucket_notification.py
--rw-r--r--   0 root         (0) root         (0)     2252 2022-05-05 00:19:09.000000 minio-7.1.8/examples/set_bucket_policy.py
--rw-r--r--   0 root         (0) root         (0)     1650 2022-05-05 00:19:09.000000 minio-7.1.8/examples/set_bucket_replication.py
--rw-r--r--   0 root         (0) root         (0)      992 2022-05-05 00:19:09.000000 minio-7.1.8/examples/set_bucket_tags.py
--rw-r--r--   0 root         (0) root         (0)      988 2022-05-05 00:19:09.000000 minio-7.1.8/examples/set_bucket_versioning.py
--rw-r--r--   0 root         (0) root         (0)     1027 2022-05-05 00:19:09.000000 minio-7.1.8/examples/set_object_lock_config.py
--rw-r--r--   0 root         (0) root         (0)     1083 2022-05-05 00:19:09.000000 minio-7.1.8/examples/set_object_retention.py
--rw-r--r--   0 root         (0) root         (0)     1005 2022-05-05 00:19:09.000000 minio-7.1.8/examples/set_object_tags.py
--rw-r--r--   0 root         (0) root         (0)     1567 2022-05-05 00:19:09.000000 minio-7.1.8/examples/stat_object.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-05 00:21:06.999438 minio-7.1.8/minio/
--rw-r--r--   0 root         (0) root         (0)     1546 2022-05-05 00:19:09.000000 minio-7.1.8/minio/__init__.py
--rw-r--r--   0 root         (0) root         (0)   103089 2022-05-05 00:19:09.000000 minio-7.1.8/minio/api.py
--rw-r--r--   0 root         (0) root         (0)    14815 2022-05-05 00:19:09.000000 minio-7.1.8/minio/commonconfig.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-05 00:21:07.003438 minio-7.1.8/minio/credentials/
--rw-r--r--   0 root         (0) root         (0)     1096 2022-05-05 00:19:09.000000 minio-7.1.8/minio/credentials/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2017 2022-05-05 00:19:09.000000 minio-7.1.8/minio/credentials/credentials.py
--rw-r--r--   0 root         (0) root         (0)    21375 2022-05-05 00:19:09.000000 minio-7.1.8/minio/credentials/providers.py
--rw-r--r--   0 root         (0) root         (0)    26465 2022-05-05 00:19:09.000000 minio-7.1.8/minio/datatypes.py
--rw-r--r--   0 root         (0) root         (0)     4837 2022-05-05 00:19:09.000000 minio-7.1.8/minio/deleteobjects.py
--rw-r--r--   0 root         (0) root         (0)     4162 2022-05-05 00:19:09.000000 minio-7.1.8/minio/error.py
--rw-r--r--   0 root         (0) root         (0)    22458 2022-05-05 00:19:09.000000 minio-7.1.8/minio/helpers.py
--rw-r--r--   0 root         (0) root         (0)     1430 2022-05-05 00:19:09.000000 minio-7.1.8/minio/legalhold.py
--rw-r--r--   0 root         (0) root         (0)    12285 2022-05-05 00:19:09.000000 minio-7.1.8/minio/lifecycleconfig.py
--rw-r--r--   0 root         (0) root         (0)    10253 2022-05-05 00:19:09.000000 minio-7.1.8/minio/minioadmin.py
--rw-r--r--   0 root         (0) root         (0)     9775 2022-05-05 00:19:09.000000 minio-7.1.8/minio/notificationconfig.py
--rw-r--r--   0 root         (0) root         (0)     2987 2022-05-05 00:19:09.000000 minio-7.1.8/minio/objectlockconfig.py
--rw-r--r--   0 root         (0) root         (0)    15277 2022-05-05 00:19:09.000000 minio-7.1.8/minio/replicationconfig.py
--rw-r--r--   0 root         (0) root         (0)     2243 2022-05-05 00:19:09.000000 minio-7.1.8/minio/retention.py
--rw-r--r--   0 root         (0) root         (0)    14453 2022-05-05 00:19:09.000000 minio-7.1.8/minio/select.py
--rw-r--r--   0 root         (0) root         (0)     8286 2022-05-05 00:19:09.000000 minio-7.1.8/minio/signer.py
--rw-r--r--   0 root         (0) root         (0)     3160 2022-05-05 00:19:09.000000 minio-7.1.8/minio/sse.py
--rw-r--r--   0 root         (0) root         (0)     3038 2022-05-05 00:19:09.000000 minio-7.1.8/minio/sseconfig.py
--rw-r--r--   0 root         (0) root         (0)     1508 2022-05-05 00:19:09.000000 minio-7.1.8/minio/tagging.py
--rw-r--r--   0 root         (0) root         (0)     2815 2022-05-05 00:19:09.000000 minio-7.1.8/minio/time.py
--rw-r--r--   0 root         (0) root         (0)     2141 2022-05-05 00:19:09.000000 minio-7.1.8/minio/versioningconfig.py
--rw-r--r--   0 root         (0) root         (0)     2896 2022-05-05 00:19:09.000000 minio-7.1.8/minio/xml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-05 00:21:06.999438 minio-7.1.8/minio.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4111 2022-05-05 00:21:05.000000 minio-7.1.8/minio.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4083 2022-05-05 00:21:06.000000 minio-7.1.8/minio.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-05 00:21:05.000000 minio-7.1.8/minio.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       16 2022-05-05 00:21:06.000000 minio-7.1.8/minio.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2022-05-05 00:21:06.000000 minio-7.1.8/minio.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-05-05 00:21:07.007438 minio-7.1.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2256 2022-05-05 00:19:09.000000 minio-7.1.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-05 00:21:07.003438 minio-7.1.8/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2022-05-05 00:19:09.000000 minio-7.1.8/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-05 00:21:07.003438 minio-7.1.8/tests/certs/
--rw-r--r--   0 root         (0) root         (0)     1708 2022-05-05 00:19:09.000000 minio-7.1.8/tests/certs/private.key
--rw-r--r--   0 root         (0) root         (0)     1115 2022-05-05 00:19:09.000000 minio-7.1.8/tests/certs/public.crt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-05 00:21:07.003438 minio-7.1.8/tests/functional/
--rw-r--r--   0 root         (0) root         (0)      119 2022-05-05 00:19:09.000000 minio-7.1.8/tests/functional/play.min.io.kes.root.key
--rw-r--r--   0 root         (0) root         (0)    68158 2022-05-05 00:19:09.000000 minio-7.1.8/tests/functional/tests.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-05 00:21:07.007438 minio-7.1.8/tests/unit/
--rw-r--r--   0 root         (0) root         (0)      656 2022-05-05 00:19:09.000000 minio-7.1.8/tests/unit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2759 2022-05-05 00:19:09.000000 minio-7.1.8/tests/unit/bucket_exist_test.py
--rw-r--r--   0 root         (0) root         (0)      334 2022-05-05 00:19:09.000000 minio-7.1.8/tests/unit/config.json.sample
--rw-r--r--   0 root         (0) root         (0)     1662 2022-05-05 00:19:09.000000 minio-7.1.8/tests/unit/copy_object_test.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-05-05 00:19:09.000000 minio-7.1.8/tests/unit/credentials.empty
--rw-r--r--   0 root         (0) root         (0)      242 2022-05-05 00:19:09.000000 minio-7.1.8/tests/unit/credentials.sample
--rw-r--r--   0 root         (0) root         (0)     9163 2022-05-05 00:19:09.000000 minio-7.1.8/tests/unit/credentials_test.py
--rw-r--r--   0 root         (0) root         (0)     3613 2022-05-05 00:19:09.000000 minio-7.1.8/tests/unit/get_bucket_policy_test.py
--rw-r--r--   0 root         (0) root         (0)     2102 2022-05-05 00:19:09.000000 minio-7.1.8/tests/unit/get_object_test.py
--rw-r--r--   0 root         (0) root         (0)     1110 2022-05-05 00:19:09.000000 minio-7.1.8/tests/unit/helpers.py
--rw-r--r--   0 root         (0) root         (0)     1118 2022-05-05 00:19:09.000000 minio-7.1.8/tests/unit/legelhold_test.py
--rw-r--r--   0 root         (0) root         (0)     3045 2022-05-05 00:19:09.000000 minio-7.1.8/tests/unit/lifecycleconfig_test.py
--rw-r--r--   0 root         (0) root         (0)     3437 2022-05-05 00:19:09.000000 minio-7.1.8/tests/unit/list_buckets_test.py
--rw-r--r--   0 root         (0) root         (0)     3714 2022-05-05 00:19:09.000000 minio-7.1.8/tests/unit/list_objects_test.py
--rw-r--r--   0 root         (0) root         (0)     7281 2022-05-05 00:19:09.000000 minio-7.1.8/tests/unit/list_objects_v1_test.py
--rw-r--r--   0 root         (0) root         (0)     2522 2022-05-05 00:19:09.000000 minio-7.1.8/tests/unit/make_bucket_test.py
--rw-r--r--   0 root         (0) root         (0)     2856 2022-05-05 00:19:09.000000 minio-7.1.8/tests/unit/minio_mocks.py
--rw-r--r--   0 root         (0) root         (0)     5966 2022-05-05 00:19:09.000000 minio-7.1.8/tests/unit/minio_test.py
--rw-r--r--   0 root         (0) root         (0)     2190 2022-05-05 00:19:09.000000 minio-7.1.8/tests/unit/notificationconfig_test.py
--rw-r--r--   0 root         (0) root         (0)     1486 2022-05-05 00:19:09.000000 minio-7.1.8/tests/unit/objectlockconfig_test.py
--rw-r--r--   0 root         (0) root         (0)     2015 2022-05-05 00:19:09.000000 minio-7.1.8/tests/unit/presigned_get_object_test.py
--rw-r--r--   0 root         (0) root         (0)     1383 2022-05-05 00:19:09.000000 minio-7.1.8/tests/unit/presigned_put_object_test.py
--rw-r--r--   0 root         (0) root         (0)     1595 2022-05-05 00:19:09.000000 minio-7.1.8/tests/unit/put_object_test.py
--rw-r--r--   0 root         (0) root         (0)     1807 2022-05-05 00:19:09.000000 minio-7.1.8/tests/unit/remove_bucket_test.py
--rw-r--r--   0 root         (0) root         (0)     1873 2022-05-05 00:19:09.000000 minio-7.1.8/tests/unit/remove_object_test.py
--rw-r--r--   0 root         (0) root         (0)     3065 2022-05-05 00:19:09.000000 minio-7.1.8/tests/unit/remove_objects_test.py
--rw-r--r--   0 root         (0) root         (0)     2548 2022-05-05 00:19:09.000000 minio-7.1.8/tests/unit/replicationconfig_test.py
--rw-r--r--   0 root         (0) root         (0)     1477 2022-05-05 00:19:09.000000 minio-7.1.8/tests/unit/retention_test.py
--rw-r--r--   0 root         (0) root         (0)     7856 2022-05-05 00:19:09.000000 minio-7.1.8/tests/unit/sign_test.py
--rw-r--r--   0 root         (0) root         (0)     1572 2022-05-05 00:19:09.000000 minio-7.1.8/tests/unit/sseconfig_test.py
--rw-r--r--   0 root         (0) root         (0)     2131 2022-05-05 00:19:09.000000 minio-7.1.8/tests/unit/stat_object_test.py
--rw-r--r--   0 root         (0) root         (0)     1339 2022-05-05 00:19:09.000000 minio-7.1.8/tests/unit/tagging_test.py
--rw-r--r--   0 root         (0) root         (0)      886 2022-05-05 00:19:09.000000 minio-7.1.8/tests/unit/trace_test.py
--rw-r--r--   0 root         (0) root         (0)     1917 2022-05-05 00:19:09.000000 minio-7.1.8/tests/unit/versioningconfig_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-11 21:34:02.843320 minio-7.1.9/
+-rw-r--r--   0 root         (0) root         (0)    11358 2022-06-11 21:29:34.000000 minio-7.1.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      235 2022-06-11 21:29:34.000000 minio-7.1.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4092 2022-06-11 21:34:02.843320 minio-7.1.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3173 2022-06-11 21:29:34.000000 minio-7.1.9/README.md
+-rw-r--r--   0 root         (0) root         (0)     8876 2022-06-11 21:29:34.000000 minio-7.1.9/README_zh_CN.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-11 21:34:02.595321 minio-7.1.9/docs/
+-rw-r--r--   0 root         (0) root         (0)    60994 2022-06-11 21:29:34.000000 minio-7.1.9/docs/API.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-11 21:34:02.615321 minio-7.1.9/docs/zh_CN/
+-rw-r--r--   0 root         (0) root         (0)    33823 2022-06-11 21:29:34.000000 minio-7.1.9/docs/zh_CN/API.md
+-rw-r--r--   0 root         (0) root         (0)      688 2022-06-11 21:29:34.000000 minio-7.1.9/docs/zh_CN/CONTRIBUTING.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-11 21:34:02.723321 minio-7.1.9/examples/
+-rw-r--r--   0 root         (0) root         (0)      930 2022-06-11 21:29:34.000000 minio-7.1.9/examples/bucket_exists.py
+-rw-r--r--   0 root         (0) root         (0)     1744 2022-06-11 21:29:34.000000 minio-7.1.9/examples/compose_object.py
+-rw-r--r--   0 root         (0) root         (0)     1733 2022-06-11 21:29:34.000000 minio-7.1.9/examples/copy_object.py
+-rw-r--r--   0 root         (0) root         (0)      873 2022-06-11 21:29:34.000000 minio-7.1.9/examples/delete_bucket_encryption.py
+-rw-r--r--   0 root         (0) root         (0)      872 2022-06-11 21:29:34.000000 minio-7.1.9/examples/delete_bucket_lifecycle.py
+-rw-r--r--   0 root         (0) root         (0)      875 2022-06-11 21:29:34.000000 minio-7.1.9/examples/delete_bucket_notification.py
+-rw-r--r--   0 root         (0) root         (0)      869 2022-06-11 21:29:34.000000 minio-7.1.9/examples/delete_bucket_policy.py
+-rw-r--r--   0 root         (0) root         (0)      874 2022-06-11 21:29:34.000000 minio-7.1.9/examples/delete_bucket_replication.py
+-rw-r--r--   0 root         (0) root         (0)      867 2022-06-11 21:29:34.000000 minio-7.1.9/examples/delete_bucket_tags.py
+-rw-r--r--   0 root         (0) root         (0)      874 2022-06-11 21:29:34.000000 minio-7.1.9/examples/delete_object_lock_config.py
+-rw-r--r--   0 root         (0) root         (0)      880 2022-06-11 21:29:34.000000 minio-7.1.9/examples/delete_object_tags.py
+-rw-r--r--   0 root         (0) root         (0)      887 2022-06-11 21:29:34.000000 minio-7.1.9/examples/disable_object_legal_hold.py
+-rw-r--r--   0 root         (0) root         (0)      886 2022-06-11 21:29:34.000000 minio-7.1.9/examples/enable_object_legal_hold.py
+-rw-r--r--   0 root         (0) root         (0)     1288 2022-06-11 21:29:34.000000 minio-7.1.9/examples/fget_object.py
+-rw-r--r--   0 root         (0) root         (0)     3561 2022-06-11 21:29:34.000000 minio-7.1.9/examples/fput_object.py
+-rw-r--r--   0 root         (0) root         (0)      879 2022-06-11 21:29:34.000000 minio-7.1.9/examples/get_bucket_encryption.py
+-rw-r--r--   0 root         (0) root         (0)      878 2022-06-11 21:29:34.000000 minio-7.1.9/examples/get_bucket_lifecycle.py
+-rw-r--r--   0 root         (0) root         (0)      881 2022-06-11 21:29:34.000000 minio-7.1.9/examples/get_bucket_notification.py
+-rw-r--r--   0 root         (0) root         (0)      875 2022-06-11 21:29:34.000000 minio-7.1.9/examples/get_bucket_policy.py
+-rw-r--r--   0 root         (0) root         (0)      880 2022-06-11 21:29:34.000000 minio-7.1.9/examples/get_bucket_replication.py
+-rw-r--r--   0 root         (0) root         (0)      871 2022-06-11 21:29:34.000000 minio-7.1.9/examples/get_bucket_tags.py
+-rw-r--r--   0 root         (0) root         (0)      900 2022-06-11 21:29:34.000000 minio-7.1.9/examples/get_bucket_versioning.py
+-rw-r--r--   0 root         (0) root         (0)     1818 2022-06-11 21:29:34.000000 minio-7.1.9/examples/get_object.py
+-rw-r--r--   0 root         (0) root         (0)      880 2022-06-11 21:29:34.000000 minio-7.1.9/examples/get_object_lock_config.py
+-rw-r--r--   0 root         (0) root         (0)      891 2022-06-11 21:29:34.000000 minio-7.1.9/examples/get_object_retention.py
+-rw-r--r--   0 root         (0) root         (0)      884 2022-06-11 21:29:34.000000 minio-7.1.9/examples/get_object_tags.py
+-rw-r--r--   0 root         (0) root         (0)     1600 2022-06-11 21:29:34.000000 minio-7.1.9/examples/get_presigned_url.py
+-rw-r--r--   0 root         (0) root         (0)     1000 2022-06-11 21:29:34.000000 minio-7.1.9/examples/is_object_legal_hold_enabled.py
+-rw-r--r--   0 root         (0) root         (0)      918 2022-06-11 21:29:34.000000 minio-7.1.9/examples/list_buckets.py
+-rw-r--r--   0 root         (0) root         (0)     1641 2022-06-11 21:29:34.000000 minio-7.1.9/examples/list_objects.py
+-rw-r--r--   0 root         (0) root         (0)     1026 2022-06-11 21:29:34.000000 minio-7.1.9/examples/listen_bucket_notification.py
+-rw-r--r--   0 root         (0) root         (0)     1074 2022-06-11 21:29:34.000000 minio-7.1.9/examples/make_bucket.py
+-rw-r--r--   0 root         (0) root         (0)     1635 2022-06-11 21:29:34.000000 minio-7.1.9/examples/minio_with_assume_role_provider.py
+-rw-r--r--   0 root         (0) root         (0)      897 2022-06-11 21:29:34.000000 minio-7.1.9/examples/minio_with_aws_config_provider.py
+-rw-r--r--   0 root         (0) root         (0)     1209 2022-06-11 21:29:34.000000 minio-7.1.9/examples/minio_with_certificate_identity_provider.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2022-06-11 21:29:34.000000 minio-7.1.9/examples/minio_with_chained_provider.py
+-rw-r--r--   0 root         (0) root         (0)     1686 2022-06-11 21:29:34.000000 minio-7.1.9/examples/minio_with_client_grants_provider.py
+-rw-r--r--   0 root         (0) root         (0)      891 2022-06-11 21:29:34.000000 minio-7.1.9/examples/minio_with_env_aws_provider.py
+-rw-r--r--   0 root         (0) root         (0)      900 2022-06-11 21:29:34.000000 minio-7.1.9/examples/minio_with_env_minio_provider.py
+-rw-r--r--   0 root         (0) root         (0)      891 2022-06-11 21:29:34.000000 minio-7.1.9/examples/minio_with_iam_aws_provider.py
+-rw-r--r--   0 root         (0) root         (0)     1161 2022-06-11 21:29:34.000000 minio-7.1.9/examples/minio_with_ldap_identity_provider.py
+-rw-r--r--   0 root         (0) root         (0)      925 2022-06-11 21:29:34.000000 minio-7.1.9/examples/minio_with_minio_client_config_provider.py
+-rw-r--r--   0 root         (0) root         (0)     2009 2022-06-11 21:29:34.000000 minio-7.1.9/examples/minio_with_web_identity_provider.py
+-rw-r--r--   0 root         (0) root         (0)     1222 2022-06-11 21:29:34.000000 minio-7.1.9/examples/presigned_get_object.py
+-rw-r--r--   0 root         (0) root         (0)     1357 2022-06-11 21:29:34.000000 minio-7.1.9/examples/presigned_post_policy.py
+-rw-r--r--   0 root         (0) root         (0)     1234 2022-06-11 21:29:34.000000 minio-7.1.9/examples/presigned_put_object.py
+-rw-r--r--   0 root         (0) root         (0)     6203 2022-06-11 21:29:34.000000 minio-7.1.9/examples/progress.py
+-rw-r--r--   0 root         (0) root         (0)     4036 2022-06-11 21:29:34.000000 minio-7.1.9/examples/put_object.py
+-rw-r--r--   0 root         (0) root         (0)      852 2022-06-11 21:29:34.000000 minio-7.1.9/examples/remove_bucket.py
+-rw-r--r--   0 root         (0) root         (0)     1023 2022-06-11 21:29:34.000000 minio-7.1.9/examples/remove_object.py
+-rw-r--r--   0 root         (0) root         (0)     1488 2022-06-11 21:29:34.000000 minio-7.1.9/examples/remove_objects.py
+-rw-r--r--   0 root         (0) root         (0)     1297 2022-06-11 21:29:34.000000 minio-7.1.9/examples/select_object_content.py
+-rw-r--r--   0 root         (0) root         (0)      956 2022-06-11 21:29:34.000000 minio-7.1.9/examples/set_bucket_encryption.py
+-rw-r--r--   0 root         (0) root         (0)     1410 2022-06-11 21:29:34.000000 minio-7.1.9/examples/set_bucket_lifecycle.py
+-rw-r--r--   0 root         (0) root         (0)     1260 2022-06-11 21:29:34.000000 minio-7.1.9/examples/set_bucket_notification.py
+-rw-r--r--   0 root         (0) root         (0)     2252 2022-06-11 21:29:34.000000 minio-7.1.9/examples/set_bucket_policy.py
+-rw-r--r--   0 root         (0) root         (0)     1650 2022-06-11 21:29:34.000000 minio-7.1.9/examples/set_bucket_replication.py
+-rw-r--r--   0 root         (0) root         (0)      992 2022-06-11 21:29:34.000000 minio-7.1.9/examples/set_bucket_tags.py
+-rw-r--r--   0 root         (0) root         (0)      988 2022-06-11 21:29:34.000000 minio-7.1.9/examples/set_bucket_versioning.py
+-rw-r--r--   0 root         (0) root         (0)     1027 2022-06-11 21:29:34.000000 minio-7.1.9/examples/set_object_lock_config.py
+-rw-r--r--   0 root         (0) root         (0)     1083 2022-06-11 21:29:34.000000 minio-7.1.9/examples/set_object_retention.py
+-rw-r--r--   0 root         (0) root         (0)     1005 2022-06-11 21:29:34.000000 minio-7.1.9/examples/set_object_tags.py
+-rw-r--r--   0 root         (0) root         (0)     1567 2022-06-11 21:29:34.000000 minio-7.1.9/examples/stat_object.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-11 21:34:02.735321 minio-7.1.9/minio/
+-rw-r--r--   0 root         (0) root         (0)     1546 2022-06-11 21:29:34.000000 minio-7.1.9/minio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   103356 2022-06-11 21:29:34.000000 minio-7.1.9/minio/api.py
+-rw-r--r--   0 root         (0) root         (0)    14815 2022-06-11 21:29:34.000000 minio-7.1.9/minio/commonconfig.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-11 21:34:02.739321 minio-7.1.9/minio/credentials/
+-rw-r--r--   0 root         (0) root         (0)     1096 2022-06-11 21:29:34.000000 minio-7.1.9/minio/credentials/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2017 2022-06-11 21:29:34.000000 minio-7.1.9/minio/credentials/credentials.py
+-rw-r--r--   0 root         (0) root         (0)    21375 2022-06-11 21:29:34.000000 minio-7.1.9/minio/credentials/providers.py
+-rw-r--r--   0 root         (0) root         (0)    26465 2022-06-11 21:29:34.000000 minio-7.1.9/minio/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)     4837 2022-06-11 21:29:34.000000 minio-7.1.9/minio/deleteobjects.py
+-rw-r--r--   0 root         (0) root         (0)     4394 2022-06-11 21:29:34.000000 minio-7.1.9/minio/error.py
+-rw-r--r--   0 root         (0) root         (0)    22626 2022-06-11 21:29:34.000000 minio-7.1.9/minio/helpers.py
+-rw-r--r--   0 root         (0) root         (0)     1430 2022-06-11 21:29:34.000000 minio-7.1.9/minio/legalhold.py
+-rw-r--r--   0 root         (0) root         (0)    12285 2022-06-11 21:29:34.000000 minio-7.1.9/minio/lifecycleconfig.py
+-rw-r--r--   0 root         (0) root         (0)    10253 2022-06-11 21:29:34.000000 minio-7.1.9/minio/minioadmin.py
+-rw-r--r--   0 root         (0) root         (0)     9775 2022-06-11 21:29:34.000000 minio-7.1.9/minio/notificationconfig.py
+-rw-r--r--   0 root         (0) root         (0)     2987 2022-06-11 21:29:34.000000 minio-7.1.9/minio/objectlockconfig.py
+-rw-r--r--   0 root         (0) root         (0)    15277 2022-06-11 21:29:34.000000 minio-7.1.9/minio/replicationconfig.py
+-rw-r--r--   0 root         (0) root         (0)     2243 2022-06-11 21:29:34.000000 minio-7.1.9/minio/retention.py
+-rw-r--r--   0 root         (0) root         (0)    14453 2022-06-11 21:29:34.000000 minio-7.1.9/minio/select.py
+-rw-r--r--   0 root         (0) root         (0)     8286 2022-06-11 21:29:34.000000 minio-7.1.9/minio/signer.py
+-rw-r--r--   0 root         (0) root         (0)     3168 2022-06-11 21:29:34.000000 minio-7.1.9/minio/sse.py
+-rw-r--r--   0 root         (0) root         (0)     3038 2022-06-11 21:29:34.000000 minio-7.1.9/minio/sseconfig.py
+-rw-r--r--   0 root         (0) root         (0)     1508 2022-06-11 21:29:34.000000 minio-7.1.9/minio/tagging.py
+-rw-r--r--   0 root         (0) root         (0)     2815 2022-06-11 21:29:34.000000 minio-7.1.9/minio/time.py
+-rw-r--r--   0 root         (0) root         (0)     2141 2022-06-11 21:29:34.000000 minio-7.1.9/minio/versioningconfig.py
+-rw-r--r--   0 root         (0) root         (0)     2896 2022-06-11 21:29:34.000000 minio-7.1.9/minio/xml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-11 21:34:02.735321 minio-7.1.9/minio.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4092 2022-06-11 21:33:59.000000 minio-7.1.9/minio.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4083 2022-06-11 21:34:01.000000 minio-7.1.9/minio.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-06-11 21:33:59.000000 minio-7.1.9/minio.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2022-06-11 21:33:59.000000 minio-7.1.9/minio.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2022-06-11 21:33:59.000000 minio-7.1.9/minio.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2022-06-11 21:34:02.843320 minio-7.1.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2257 2022-06-11 21:29:34.000000 minio-7.1.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-11 21:34:02.739321 minio-7.1.9/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-11 21:29:34.000000 minio-7.1.9/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-11 21:34:02.795320 minio-7.1.9/tests/certs/
+-rw-r--r--   0 root         (0) root         (0)     1708 2022-06-11 21:29:34.000000 minio-7.1.9/tests/certs/private.key
+-rw-r--r--   0 root         (0) root         (0)     1115 2022-06-11 21:29:34.000000 minio-7.1.9/tests/certs/public.crt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-11 21:34:02.823320 minio-7.1.9/tests/functional/
+-rw-r--r--   0 root         (0) root         (0)      119 2022-06-11 21:29:34.000000 minio-7.1.9/tests/functional/play.min.io.kes.root.key
+-rw-r--r--   0 root         (0) root         (0)    68158 2022-06-11 21:29:34.000000 minio-7.1.9/tests/functional/tests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-11 21:34:02.843320 minio-7.1.9/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)      656 2022-06-11 21:29:34.000000 minio-7.1.9/tests/unit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2758 2022-06-11 21:29:34.000000 minio-7.1.9/tests/unit/bucket_exist_test.py
+-rw-r--r--   0 root         (0) root         (0)      334 2022-06-11 21:29:34.000000 minio-7.1.9/tests/unit/config.json.sample
+-rw-r--r--   0 root         (0) root         (0)     1662 2022-06-11 21:29:34.000000 minio-7.1.9/tests/unit/copy_object_test.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-11 21:29:34.000000 minio-7.1.9/tests/unit/credentials.empty
+-rw-r--r--   0 root         (0) root         (0)      242 2022-06-11 21:29:34.000000 minio-7.1.9/tests/unit/credentials.sample
+-rw-r--r--   0 root         (0) root         (0)     9162 2022-06-11 21:29:34.000000 minio-7.1.9/tests/unit/credentials_test.py
+-rw-r--r--   0 root         (0) root         (0)     3612 2022-06-11 21:29:34.000000 minio-7.1.9/tests/unit/get_bucket_policy_test.py
+-rw-r--r--   0 root         (0) root         (0)     2101 2022-06-11 21:29:34.000000 minio-7.1.9/tests/unit/get_object_test.py
+-rw-r--r--   0 root         (0) root         (0)     1110 2022-06-11 21:29:34.000000 minio-7.1.9/tests/unit/helpers.py
+-rw-r--r--   0 root         (0) root         (0)     1118 2022-06-11 21:29:34.000000 minio-7.1.9/tests/unit/legelhold_test.py
+-rw-r--r--   0 root         (0) root         (0)     3045 2022-06-11 21:29:34.000000 minio-7.1.9/tests/unit/lifecycleconfig_test.py
+-rw-r--r--   0 root         (0) root         (0)     3436 2022-06-11 21:29:34.000000 minio-7.1.9/tests/unit/list_buckets_test.py
+-rw-r--r--   0 root         (0) root         (0)     3713 2022-06-11 21:29:34.000000 minio-7.1.9/tests/unit/list_objects_test.py
+-rw-r--r--   0 root         (0) root         (0)     7280 2022-06-11 21:29:34.000000 minio-7.1.9/tests/unit/list_objects_v1_test.py
+-rw-r--r--   0 root         (0) root         (0)     2521 2022-06-11 21:29:34.000000 minio-7.1.9/tests/unit/make_bucket_test.py
+-rw-r--r--   0 root         (0) root         (0)     2856 2022-06-11 21:29:34.000000 minio-7.1.9/tests/unit/minio_mocks.py
+-rw-r--r--   0 root         (0) root         (0)     5966 2022-06-11 21:29:34.000000 minio-7.1.9/tests/unit/minio_test.py
+-rw-r--r--   0 root         (0) root         (0)     2190 2022-06-11 21:29:34.000000 minio-7.1.9/tests/unit/notificationconfig_test.py
+-rw-r--r--   0 root         (0) root         (0)     1486 2022-06-11 21:29:34.000000 minio-7.1.9/tests/unit/objectlockconfig_test.py
+-rw-r--r--   0 root         (0) root         (0)     2014 2022-06-11 21:29:34.000000 minio-7.1.9/tests/unit/presigned_get_object_test.py
+-rw-r--r--   0 root         (0) root         (0)     1383 2022-06-11 21:29:34.000000 minio-7.1.9/tests/unit/presigned_put_object_test.py
+-rw-r--r--   0 root         (0) root         (0)     1595 2022-06-11 21:29:34.000000 minio-7.1.9/tests/unit/put_object_test.py
+-rw-r--r--   0 root         (0) root         (0)     1806 2022-06-11 21:29:34.000000 minio-7.1.9/tests/unit/remove_bucket_test.py
+-rw-r--r--   0 root         (0) root         (0)     1872 2022-06-11 21:29:34.000000 minio-7.1.9/tests/unit/remove_object_test.py
+-rw-r--r--   0 root         (0) root         (0)     3064 2022-06-11 21:29:34.000000 minio-7.1.9/tests/unit/remove_objects_test.py
+-rw-r--r--   0 root         (0) root         (0)     2548 2022-06-11 21:29:34.000000 minio-7.1.9/tests/unit/replicationconfig_test.py
+-rw-r--r--   0 root         (0) root         (0)     1477 2022-06-11 21:29:34.000000 minio-7.1.9/tests/unit/retention_test.py
+-rw-r--r--   0 root         (0) root         (0)     7856 2022-06-11 21:29:34.000000 minio-7.1.9/tests/unit/sign_test.py
+-rw-r--r--   0 root         (0) root         (0)     1572 2022-06-11 21:29:34.000000 minio-7.1.9/tests/unit/sseconfig_test.py
+-rw-r--r--   0 root         (0) root         (0)     2130 2022-06-11 21:29:34.000000 minio-7.1.9/tests/unit/stat_object_test.py
+-rw-r--r--   0 root         (0) root         (0)     1339 2022-06-11 21:29:34.000000 minio-7.1.9/tests/unit/tagging_test.py
+-rw-r--r--   0 root         (0) root         (0)      886 2022-06-11 21:29:34.000000 minio-7.1.9/tests/unit/trace_test.py
+-rw-r--r--   0 root         (0) root         (0)     1917 2022-06-11 21:29:34.000000 minio-7.1.9/tests/unit/versioningconfig_test.py
```

### Comparing `minio-7.1.8/LICENSE` & `minio-7.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/PKG-INFO` & `minio-7.1.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 Metadata-Version: 2.1
 Name: minio
-Version: 7.1.8
+Version: 7.1.9
 Summary: MinIO Python SDK for Amazon S3 Compatible Cloud Storage
 Home-page: https://github.com/minio/minio-py
 Download-URL: https://github.com/minio/minio-py/releases
 Author: MinIO, Inc.
 Author-email: dev@min.io
 License: Apache License 2.0
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MinIO Python SDK for Amazon S3 Compatible Cloud Storage [![Slack](https://slack.min.io/slack?type=svg)](https://slack.min.io)
 
 MinIO Python SDK is Simple Storage Service (aka S3) client to perform bucket and object operations to any Amazon S3 compatible object storage service.
 
 For a complete list of APIs and examples, please take a look at the [Python Client API Reference](https://docs.min.io/docs/python-client-api-reference)
 
 ## Minimum Requirements
-Python 3.6 or higher.
+Python 3.7 or higher.
 
 ## Download using pip
 
 ```sh
 pip3 install minio
 ```
 
@@ -114,9 +113,7 @@
 ## Explore Further
 * [Complete Documentation](https://docs.min.io)
 
 ## Contribute
 Please refer [Contributors Guide](https://github.com/minio/minio-py/blob/release/CONTRIBUTING.md)
 
 [![PYPI](https://img.shields.io/pypi/v/minio.svg)](https://pypi.python.org/pypi/minio)
-
-
```

### Comparing `minio-7.1.8/README.md` & `minio-7.1.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # MinIO Python SDK for Amazon S3 Compatible Cloud Storage [![Slack](https://slack.min.io/slack?type=svg)](https://slack.min.io)
 
 MinIO Python SDK is Simple Storage Service (aka S3) client to perform bucket and object operations to any Amazon S3 compatible object storage service.
 
 For a complete list of APIs and examples, please take a look at the [Python Client API Reference](https://docs.min.io/docs/python-client-api-reference)
 
 ## Minimum Requirements
-Python 3.6 or higher.
+Python 3.7 or higher.
 
 ## Download using pip
 
 ```sh
 pip3 install minio
 ```
```

### Comparing `minio-7.1.8/README_zh_CN.md` & `minio-7.1.9/README_zh_CN.md`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/docs/API.md` & `minio-7.1.9/docs/API.md`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/docs/zh_CN/API.md` & `minio-7.1.9/docs/zh_CN/API.md`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/docs/zh_CN/CONTRIBUTING.md` & `minio-7.1.9/docs/zh_CN/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/bucket_exists.py` & `minio-7.1.9/examples/bucket_exists.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/compose_object.py` & `minio-7.1.9/examples/compose_object.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/copy_object.py` & `minio-7.1.9/examples/copy_object.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/delete_bucket_encryption.py` & `minio-7.1.9/examples/delete_bucket_encryption.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/delete_bucket_lifecycle.py` & `minio-7.1.9/examples/delete_bucket_lifecycle.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/delete_bucket_notification.py` & `minio-7.1.9/examples/delete_bucket_notification.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/delete_bucket_policy.py` & `minio-7.1.9/examples/delete_bucket_policy.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/delete_bucket_replication.py` & `minio-7.1.9/examples/delete_bucket_replication.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/delete_bucket_tags.py` & `minio-7.1.9/examples/delete_bucket_tags.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/delete_object_lock_config.py` & `minio-7.1.9/examples/delete_object_lock_config.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/delete_object_tags.py` & `minio-7.1.9/examples/delete_object_tags.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/disable_object_legal_hold.py` & `minio-7.1.9/examples/disable_object_legal_hold.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/enable_object_legal_hold.py` & `minio-7.1.9/examples/enable_object_legal_hold.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/fget_object.py` & `minio-7.1.9/examples/fget_object.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/fput_object.py` & `minio-7.1.9/examples/fput_object.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/get_bucket_encryption.py` & `minio-7.1.9/examples/get_bucket_encryption.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/get_bucket_lifecycle.py` & `minio-7.1.9/examples/get_bucket_lifecycle.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/get_bucket_notification.py` & `minio-7.1.9/examples/get_bucket_notification.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/get_bucket_policy.py` & `minio-7.1.9/examples/get_bucket_policy.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/get_bucket_replication.py` & `minio-7.1.9/examples/get_bucket_replication.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/get_bucket_tags.py` & `minio-7.1.9/examples/get_bucket_tags.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/get_bucket_versioning.py` & `minio-7.1.9/examples/get_bucket_versioning.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/get_object.py` & `minio-7.1.9/examples/get_object.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/get_object_lock_config.py` & `minio-7.1.9/examples/get_object_lock_config.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/get_object_retention.py` & `minio-7.1.9/examples/get_object_retention.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/get_object_tags.py` & `minio-7.1.9/examples/get_object_tags.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/get_presigned_url.py` & `minio-7.1.9/examples/get_presigned_url.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/is_object_legal_hold_enabled.py` & `minio-7.1.9/examples/is_object_legal_hold_enabled.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/list_buckets.py` & `minio-7.1.9/examples/list_buckets.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/list_objects.py` & `minio-7.1.9/examples/list_objects.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/listen_bucket_notification.py` & `minio-7.1.9/examples/listen_bucket_notification.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/make_bucket.py` & `minio-7.1.9/examples/make_bucket.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/minio_with_assume_role_provider.py` & `minio-7.1.9/examples/minio_with_assume_role_provider.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/minio_with_aws_config_provider.py` & `minio-7.1.9/examples/minio_with_aws_config_provider.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/minio_with_certificate_identity_provider.py` & `minio-7.1.9/examples/minio_with_certificate_identity_provider.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/minio_with_chained_provider.py` & `minio-7.1.9/examples/minio_with_chained_provider.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/minio_with_client_grants_provider.py` & `minio-7.1.9/examples/minio_with_client_grants_provider.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/minio_with_env_aws_provider.py` & `minio-7.1.9/examples/minio_with_env_aws_provider.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/minio_with_env_minio_provider.py` & `minio-7.1.9/examples/minio_with_env_minio_provider.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/minio_with_iam_aws_provider.py` & `minio-7.1.9/examples/minio_with_iam_aws_provider.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/minio_with_ldap_identity_provider.py` & `minio-7.1.9/examples/minio_with_ldap_identity_provider.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/minio_with_minio_client_config_provider.py` & `minio-7.1.9/examples/minio_with_minio_client_config_provider.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/minio_with_web_identity_provider.py` & `minio-7.1.9/examples/minio_with_web_identity_provider.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/presigned_get_object.py` & `minio-7.1.9/examples/presigned_get_object.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/presigned_post_policy.py` & `minio-7.1.9/examples/presigned_post_policy.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/presigned_put_object.py` & `minio-7.1.9/examples/presigned_put_object.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/progress.py` & `minio-7.1.9/examples/progress.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/put_object.py` & `minio-7.1.9/examples/put_object.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/remove_bucket.py` & `minio-7.1.9/examples/remove_bucket.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/remove_object.py` & `minio-7.1.9/examples/remove_object.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/remove_objects.py` & `minio-7.1.9/examples/remove_objects.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/select_object_content.py` & `minio-7.1.9/examples/select_object_content.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/set_bucket_encryption.py` & `minio-7.1.9/examples/set_bucket_encryption.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/set_bucket_lifecycle.py` & `minio-7.1.9/examples/set_bucket_lifecycle.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/set_bucket_notification.py` & `minio-7.1.9/examples/set_bucket_notification.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/set_bucket_policy.py` & `minio-7.1.9/examples/set_bucket_policy.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/set_bucket_replication.py` & `minio-7.1.9/examples/set_bucket_replication.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/set_bucket_tags.py` & `minio-7.1.9/examples/set_bucket_tags.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/set_bucket_versioning.py` & `minio-7.1.9/examples/set_bucket_versioning.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/set_object_lock_config.py` & `minio-7.1.9/examples/set_object_lock_config.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/set_object_retention.py` & `minio-7.1.9/examples/set_object_retention.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/set_object_tags.py` & `minio-7.1.9/examples/set_object_tags.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/examples/stat_object.py` & `minio-7.1.9/examples/stat_object.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/minio/__init__.py` & `minio-7.1.9/minio/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 :copyright: (C) 2015-2020 MinIO, Inc.
 :license: Apache 2.0, see LICENSE for more details.
 """
 
 __title__ = "minio-py"
 __author__ = "MinIO, Inc."
-__version__ = "7.1.8"
+__version__ = "7.1.9"
 __license__ = "Apache 2.0"
 __copyright__ = "Copyright 2015, 2016, 2017, 2018, 2019, 2020 MinIO, Inc."
 
 import threading
 
 __LOCALE_LOCK__ = threading.Lock()
```

### Comparing `minio-7.1.8/minio/api.py` & `minio-7.1.9/minio/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -299,14 +299,19 @@
                 method != "HEAD" and
                 "application/xml" not in response.getheader(
                     "content-type", "",
                 ).split(";")
         ):
             if self._trace_stream:
                 self._trace_stream.write("----------END-HTTP----------\n")
+            if response.status == 304 and not response.data:
+                raise ServerError(
+                    f"server failed with HTTP status code {response.status}",
+                    response.status,
+                )
             raise InvalidResponseError(
                 response.status,
                 response.getheader("content-type"),
                 response.data.decode() if response.data else None,
             )
 
         if not response.data and method != "HEAD":
@@ -357,15 +362,16 @@
         }
 
         if not response_error:
             func = error_map.get(response.status)
             code, message = func() if func else (None, None)
             if not code:
                 raise ServerError(
-                    f"server failed with HTTP status code {response.status}"
+                    f"server failed with HTTP status code {response.status}",
+                    response.status,
                 )
             response_error = S3Error(
                 code,
                 message,
                 url.path,
                 response.getheader("x-amz-request-id"),
                 response.getheader("x-amz-id-2"),
```

### Comparing `minio-7.1.8/minio/commonconfig.py` & `minio-7.1.9/minio/commonconfig.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/minio/credentials/__init__.py` & `minio-7.1.9/minio/credentials/__init__.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/minio/credentials/credentials.py` & `minio-7.1.9/minio/credentials/credentials.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/minio/credentials/providers.py` & `minio-7.1.9/minio/credentials/providers.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/minio/datatypes.py` & `minio-7.1.9/minio/datatypes.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/minio/deleteobjects.py` & `minio-7.1.9/minio/deleteobjects.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/minio/error.py` & `minio-7.1.9/minio/error.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,23 @@
     def __reduce__(self):
         return type(self), (self._code, self._content_type, self._body)
 
 
 class ServerError(MinioException):
     """Raised to indicate that S3 service returning HTTP server error."""
 
+    def __init__(self, message, status_code):
+        self._status_code = status_code
+        super().__init__(message)
+
+    @property
+    def status_code(self):
+        """Get HTTP status code."""
+        return self._status_code
+
 
 class S3Error(MinioException):
     """
     Raised to indicate that error response is received
     when executing S3 operation.
     """
```

### Comparing `minio-7.1.8/minio/helpers.py` & `minio-7.1.9/minio/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
     if part_size > 0:
         if part_size < MIN_PART_SIZE:
             raise ValueError(
                 f"part size {part_size} is not supported; minimum allowed 5MiB",
             )
         if part_size > MAX_PART_SIZE:
             raise ValueError(
-                f"part size {part_size} is not supported; minimum allowed 5GiB",
+                f"part size {part_size} is not supported; maximum allowed 5GiB",
             )
 
     if object_size >= 0:
         if object_size > MAX_MULTIPART_OBJECT_SIZE:
             raise ValueError(
                 f"object size {object_size} is not supported; "
                 f"maximum allowed 5TiB"
@@ -251,15 +251,17 @@
 
 
 def md5sum_hash(data):
     """Compute MD5 of data and return hash as Base64 encoded value."""
     if data is None:
         return None
 
-    hasher = hashlib.md5()
+    # indicate md5 hashing algorithm is not used in a security context.
+    # Refer https://bugs.python.org/issue9216 for more information.
+    hasher = hashlib.new("md5", usedforsecurity=False)
     hasher.update(data.encode() if isinstance(data, str) else data)
     md5sum = base64.b64encode(hasher.digest())
     return md5sum.decode() if isinstance(md5sum, bytes) else md5sum
 
 
 def sha256_hash(data):
     """Compute SHA-256 of data and return hash as hex encoded value."""
```

### Comparing `minio-7.1.8/minio/legalhold.py` & `minio-7.1.9/minio/legalhold.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/minio/lifecycleconfig.py` & `minio-7.1.9/minio/lifecycleconfig.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/minio/minioadmin.py` & `minio-7.1.9/minio/minioadmin.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/minio/notificationconfig.py` & `minio-7.1.9/minio/notificationconfig.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/minio/objectlockconfig.py` & `minio-7.1.9/minio/objectlockconfig.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/minio/replicationconfig.py` & `minio-7.1.9/minio/replicationconfig.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/minio/retention.py` & `minio-7.1.9/minio/retention.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/minio/select.py` & `minio-7.1.9/minio/select.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/minio/signer.py` & `minio-7.1.9/minio/signer.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/minio/sse.py` & `minio-7.1.9/minio/sse.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 This module contains core API parsers.
 
 :copyright: (c) 2018 by MinIO, Inc.
 :license: Apache 2.0, see LICENSE for more details.
 
 """
 import base64
-import hashlib
 import json
 from abc import ABCMeta, abstractmethod
 
 
 class Sse:
     """Server-side encryption base class."""
     __metaclass__ = ABCMeta
@@ -52,17 +51,17 @@
 
     def __init__(self, key):
         if len(key) != 32:
             raise ValueError(
                 "SSE-C keys need to be 256 bit base64 encoded",
             )
         b64key = base64.b64encode(key).decode()
-        md5 = hashlib.md5()
-        md5.update(key)
-        md5key = base64.b64encode(md5.digest()).decode()
+        from .helpers import \
+            md5sum_hash  # pylint: disable=import-outside-toplevel
+        md5key = md5sum_hash(key)
         self._headers = {
             "X-Amz-Server-Side-Encryption-Customer-Algorithm": "AES256",
             "X-Amz-Server-Side-Encryption-Customer-Key": b64key,
             "X-Amz-Server-Side-Encryption-Customer-Key-MD5": md5key,
         }
         self._copy_headers = {
             "X-Amz-Copy-Source-Server-Side-Encryption-Customer-Algorithm":
```

### Comparing `minio-7.1.8/minio/sseconfig.py` & `minio-7.1.9/minio/sseconfig.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/minio/tagging.py` & `minio-7.1.9/minio/tagging.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/minio/time.py` & `minio-7.1.9/minio/time.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/minio/versioningconfig.py` & `minio-7.1.9/minio/versioningconfig.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/minio/xml.py` & `minio-7.1.9/minio/xml.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/minio.egg-info/PKG-INFO` & `minio-7.1.9/minio.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 Metadata-Version: 2.1
 Name: minio
-Version: 7.1.8
+Version: 7.1.9
 Summary: MinIO Python SDK for Amazon S3 Compatible Cloud Storage
 Home-page: https://github.com/minio/minio-py
 Download-URL: https://github.com/minio/minio-py/releases
 Author: MinIO, Inc.
 Author-email: dev@min.io
 License: Apache License 2.0
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MinIO Python SDK for Amazon S3 Compatible Cloud Storage [![Slack](https://slack.min.io/slack?type=svg)](https://slack.min.io)
 
 MinIO Python SDK is Simple Storage Service (aka S3) client to perform bucket and object operations to any Amazon S3 compatible object storage service.
 
 For a complete list of APIs and examples, please take a look at the [Python Client API Reference](https://docs.min.io/docs/python-client-api-reference)
 
 ## Minimum Requirements
-Python 3.6 or higher.
+Python 3.7 or higher.
 
 ## Download using pip
 
 ```sh
 pip3 install minio
 ```
 
@@ -114,9 +113,7 @@
 ## Explore Further
 * [Complete Documentation](https://docs.min.io)
 
 ## Contribute
 Please refer [Contributors Guide](https://github.com/minio/minio-py/blob/release/CONTRIBUTING.md)
 
 [![PYPI](https://img.shields.io/pypi/v/minio.svg)](https://pypi.python.org/pypi/minio)
-
-
```

### Comparing `minio-7.1.8/minio.egg-info/SOURCES.txt` & `minio-7.1.9/minio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/setup.py` & `minio-7.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,17 +49,17 @@
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     long_description=readme,
     package_data={"": ["LICENSE", "README.md"]},
     include_package_data=True,
 )
```

### Comparing `minio-7.1.8/tests/certs/private.key` & `minio-7.1.9/tests/certs/private.key`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/tests/certs/public.crt` & `minio-7.1.9/tests/certs/public.crt`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/tests/functional/tests.py` & `minio-7.1.9/tests/functional/tests.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/tests/unit/__init__.py` & `minio-7.1.9/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/tests/unit/bucket_exist_test.py` & `minio-7.1.9/tests/unit/bucket_exist_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,17 +10,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from unittest import TestCase
-
 import unittest.mock as mock
+from unittest import TestCase
 
 from minio import Minio
 from minio.api import _DEFAULT_USER_AGENT
 from minio.error import S3Error
 
 from .minio_mocks import MockConnection, MockResponse
```

### Comparing `minio-7.1.8/tests/unit/copy_object_test.py` & `minio-7.1.9/tests/unit/copy_object_test.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/tests/unit/credentials_test.py` & `minio-7.1.9/tests/unit/credentials_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,19 +12,18 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import json
 import os
+import unittest.mock as mock
 from datetime import datetime, timedelta
 from unittest import TestCase
 
-import unittest.mock as mock
-
 from minio.credentials.credentials import Credentials
 from minio.credentials.providers import (AWSConfigProvider, ChainedProvider,
                                          EnvAWSProvider, EnvMinioProvider,
                                          IamAwsProvider,
                                          MinioClientConfigProvider,
                                          StaticProvider)
```

### Comparing `minio-7.1.8/tests/unit/get_bucket_policy_test.py` & `minio-7.1.9/tests/unit/get_bucket_policy_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,17 +12,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 import json
-from unittest import TestCase
-
 import unittest.mock as mock
+from unittest import TestCase
 
 from minio import Minio
 from minio.api import _DEFAULT_USER_AGENT
 from minio.error import S3Error
 from tests.unit.minio_mocks import MockConnection, MockResponse
```

### Comparing `minio-7.1.8/tests/unit/get_object_test.py` & `minio-7.1.9/tests/unit/get_object_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,17 +10,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from unittest import TestCase
-
 import unittest.mock as mock
+from unittest import TestCase
 
 from minio import Minio
 from minio.api import _DEFAULT_USER_AGENT
 from minio.error import S3Error
 
 from .helpers import generate_error
 from .minio_mocks import MockConnection, MockResponse
```

### Comparing `minio-7.1.8/tests/unit/helpers.py` & `minio-7.1.9/tests/unit/helpers.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/tests/unit/legelhold_test.py` & `minio-7.1.9/tests/unit/legelhold_test.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/tests/unit/lifecycleconfig_test.py` & `minio-7.1.9/tests/unit/lifecycleconfig_test.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/tests/unit/list_buckets_test.py` & `minio-7.1.9/tests/unit/list_buckets_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,19 +10,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import unittest.mock as mock
 from datetime import datetime, timezone
 from unittest import TestCase
 
-import unittest.mock as mock
-
 from minio import Minio
 from minio.api import _DEFAULT_USER_AGENT
 
 from .minio_mocks import MockConnection, MockResponse
 
 
 class ListBucketsTest(TestCase):
```

### Comparing `minio-7.1.8/tests/unit/list_objects_test.py` & `minio-7.1.9/tests/unit/list_objects_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,17 +11,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import time
-from unittest import TestCase
-
 import unittest.mock as mock
+from unittest import TestCase
 
 from minio import Minio
 from minio.api import _DEFAULT_USER_AGENT
 
 from .minio_mocks import MockConnection, MockResponse
```

### Comparing `minio-7.1.8/tests/unit/list_objects_v1_test.py` & `minio-7.1.9/tests/unit/list_objects_v1_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,17 +11,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import time
-from unittest import TestCase
-
 import unittest.mock as mock
+from unittest import TestCase
 
 from minio import Minio
 from minio.api import _DEFAULT_USER_AGENT
 
 from .minio_mocks import MockConnection, MockResponse
```

### Comparing `minio-7.1.8/tests/unit/make_bucket_test.py` & `minio-7.1.9/tests/unit/make_bucket_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,17 +10,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from unittest import TestCase
-
 import unittest.mock as mock
+from unittest import TestCase
 
 from minio import Minio
 from minio.api import _DEFAULT_USER_AGENT
 from minio.error import S3Error
 
 from .helpers import generate_error
 from .minio_mocks import MockConnection, MockResponse
```

### Comparing `minio-7.1.8/tests/unit/minio_mocks.py` & `minio-7.1.9/tests/unit/minio_mocks.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/tests/unit/minio_test.py` & `minio-7.1.9/tests/unit/minio_test.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/tests/unit/notificationconfig_test.py` & `minio-7.1.9/tests/unit/notificationconfig_test.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/tests/unit/objectlockconfig_test.py` & `minio-7.1.9/tests/unit/objectlockconfig_test.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/tests/unit/presigned_get_object_test.py` & `minio-7.1.9/tests/unit/presigned_get_object_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,19 +10,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import unittest.mock as mock
 from datetime import timedelta
 from unittest import TestCase
 
-import unittest.mock as mock
-
 from minio import Minio
 
 
 class PresignedGetObjectTest(TestCase):
     def test_object_is_string(self):
         client = Minio('localhost:9000')
         self.assertRaises(
```

### Comparing `minio-7.1.8/tests/unit/presigned_put_object_test.py` & `minio-7.1.9/tests/unit/presigned_put_object_test.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/tests/unit/put_object_test.py` & `minio-7.1.9/tests/unit/put_object_test.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/tests/unit/remove_bucket_test.py` & `minio-7.1.9/tests/unit/remove_bucket_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,17 +10,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from unittest import TestCase
-
 import unittest.mock as mock
+from unittest import TestCase
 
 from minio import Minio
 from minio.api import _DEFAULT_USER_AGENT
 
 from .minio_mocks import MockConnection, MockResponse
```

### Comparing `minio-7.1.8/tests/unit/remove_object_test.py` & `minio-7.1.9/tests/unit/remove_object_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,17 +10,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an 'AS IS' BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from unittest import TestCase
-
 import unittest.mock as mock
+from unittest import TestCase
 
 from minio import Minio
 from minio.api import _DEFAULT_USER_AGENT
 
 from .minio_mocks import MockConnection, MockResponse
```

### Comparing `minio-7.1.8/tests/unit/remove_objects_test.py` & `minio-7.1.9/tests/unit/remove_objects_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an 'AS IS' BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import itertools
-from unittest import TestCase
-
 import unittest.mock as mock
+from unittest import TestCase
 
 from minio import Minio
 from minio.api import _DEFAULT_USER_AGENT
 from minio.deleteobjects import DeleteObject
 
 from .minio_mocks import MockConnection, MockResponse
```

### Comparing `minio-7.1.8/tests/unit/replicationconfig_test.py` & `minio-7.1.9/tests/unit/replicationconfig_test.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/tests/unit/retention_test.py` & `minio-7.1.9/tests/unit/retention_test.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/tests/unit/sign_test.py` & `minio-7.1.9/tests/unit/sign_test.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/tests/unit/sseconfig_test.py` & `minio-7.1.9/tests/unit/sseconfig_test.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/tests/unit/stat_object_test.py` & `minio-7.1.9/tests/unit/stat_object_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,17 +10,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an 'AS IS' BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from unittest import TestCase
-
 import unittest.mock as mock
+from unittest import TestCase
 
 from minio import Minio
 from minio.api import _DEFAULT_USER_AGENT
 
 from .minio_mocks import MockConnection, MockResponse
```

### Comparing `minio-7.1.8/tests/unit/tagging_test.py` & `minio-7.1.9/tests/unit/tagging_test.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/tests/unit/trace_test.py` & `minio-7.1.9/tests/unit/trace_test.py`

 * *Files identical despite different names*

### Comparing `minio-7.1.8/tests/unit/versioningconfig_test.py` & `minio-7.1.9/tests/unit/versioningconfig_test.py`

 * *Files identical despite different names*

